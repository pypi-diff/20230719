# Comparing `tmp/tencentcloud-sdk-python-vod-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-vod-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.937.tar", last modified: Tue Jul 18 00:34:55 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.938.tar", last modified: Wed Jul 19 00:53:36 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vod-3.0.937.tar` & `tencentcloud-sdk-python-vod-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud/vod/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud/vod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud/vod/v20180717/
--rw-r--r--   0 root         (0) root         (0)   182739 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud/vod/v20180717/vod_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud/vod/v20180717/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25211 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud/vod/v20180717/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1854207 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud/vod/v20180717/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud_sdk_python_vod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud_sdk_python_vod.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:36.000000 tencentcloud-sdk-python-vod-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:53:36.000000 tencentcloud-sdk-python-vod-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:36.000000 tencentcloud-sdk-python-vod-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:36.000000 tencentcloud-sdk-python-vod-3.0.938/tencentcloud/vod/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:53:36.000000 tencentcloud-sdk-python-vod-3.0.938/tencentcloud/vod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:36.000000 tencentcloud-sdk-python-vod-3.0.938/tencentcloud/vod/v20180717/
+-rw-r--r--   0 root         (0) root         (0)   183379 2023-07-19 00:53:36.000000 tencentcloud-sdk-python-vod-3.0.938/tencentcloud/vod/v20180717/vod_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:53:36.000000 tencentcloud-sdk-python-vod-3.0.938/tencentcloud/vod/v20180717/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25211 2023-07-19 00:53:36.000000 tencentcloud-sdk-python-vod-3.0.938/tencentcloud/vod/v20180717/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1854207 2023-07-19 00:53:36.000000 tencentcloud-sdk-python-vod-3.0.938/tencentcloud/vod/v20180717/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:53:36.000000 tencentcloud-sdk-python-vod-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:53:36.000000 tencentcloud-sdk-python-vod-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:53:36.000000 tencentcloud-sdk-python-vod-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:53:36.000000 tencentcloud-sdk-python-vod-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:36.000000 tencentcloud-sdk-python-vod-3.0.938/tencentcloud_sdk_python_vod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:53:36.000000 tencentcloud-sdk-python-vod-3.0.938/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:53:36.000000 tencentcloud-sdk-python-vod-3.0.938/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:53:36.000000 tencentcloud-sdk-python-vod-3.0.938/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:53:36.000000 tencentcloud-sdk-python-vod-3.0.938/tencentcloud_sdk_python_vod.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-vod-3.0.937/setup.py` & `tencentcloud-sdk-python-vod-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.937/tencentcloud/vod/v20180717/vod_client.py` & `tencentcloud-sdk-python-vod-3.0.938/tencentcloud/vod/v20180717/vod_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             model = models.ApplyUploadResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AttachMediaSubtitles(self, request):
         """关联媒资字幕，将指定的字幕关联到转自适应码流模板号对应的媒体输出文件中（或解除关联）。
 
         :param request: Request instance for AttachMediaSubtitles.
         :type request: :class:`tencentcloud.vod.v20180717.models.AttachMediaSubtitlesRequest`
@@ -67,15 +67,15 @@
             model = models.AttachMediaSubtitlesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CommitUpload(self, request):
         """该接口用于确认媒体文件（和封面文件）上传到腾讯云点播的结果，并存储媒体信息，返回文件的播放地址和文件 ID。
 
         :param request: Request instance for CommitUpload.
         :type request: :class:`tencentcloud.vod.v20180717.models.CommitUploadRequest`
@@ -90,15 +90,15 @@
             model = models.CommitUploadResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ComposeMedia(self, request):
         """该接口用于合成媒体文件，可以达到以下效果：
 
         1. **画面旋转**：对视频、图片的画面旋转一定角度，或按照某个方向翻转。
         2. **声音控制**：升高降低视频、音频中声音的音量，或者对视频静音。
@@ -124,15 +124,15 @@
             model = models.ComposeMediaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ConfirmEvents(self, request):
         """* 开发者调用拉取事件通知，获取到事件后，必须调用该接口来确认消息已经收到；
         * 开发者获取到事件句柄后，等待确认的有效时间为 30 秒，超出 30 秒会报参数错误（4000）；
         * 更多参考事件通知的[可靠回调](https://cloud.tencent.com/document/product/266/33779#.E5.8F.AF.E9.9D.A0.E5.9B.9E.E8.B0.83)。
 
@@ -149,15 +149,15 @@
             model = models.ConfirmEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAIAnalysisTemplate(self, request):
         """创建用户自定义音视频内容分析模板，数量上限：50。
 
         :param request: Request instance for CreateAIAnalysisTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.CreateAIAnalysisTemplateRequest`
@@ -172,15 +172,15 @@
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
         """创建用户自定义音视频内容识别模板，数量上限：50。
 
         :param request: Request instance for CreateAIRecognitionTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.CreateAIRecognitionTemplateRequest`
@@ -195,15 +195,15 @@
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
         :type request: :class:`tencentcloud.vod.v20180717.models.CreateAdaptiveDynamicStreamingTemplateRequest`
@@ -218,15 +218,15 @@
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
         :type request: :class:`tencentcloud.vod.v20180717.models.CreateAnimatedGraphicsTemplateRequest`
@@ -241,15 +241,15 @@
             model = models.CreateAnimatedGraphicsTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateClass(self, request):
         """* 用于对媒体进行分类管理；
         * 该接口不影响既有媒体的分类，如需修改媒体分类，请调用[修改媒体文件属性](/document/product/266/31762)接口。
         * 分类层次不可超过 4 层。
         * 每个分类的子类数量不可超过 500 个。
@@ -267,15 +267,15 @@
             model = models.CreateClassResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateContentReviewTemplate(self, request):
         """该 API 已经<font color=red>不再维护</font>，新版审核模板支持音视频审核和图片审核，详细请参考 [创建审核模板](https://cloud.tencent.com/document/api/266/84391)。
         创建用户自定义音视频内容审核模板，数量上限：50。
 
         :param request: Request instance for CreateContentReviewTemplate.
@@ -291,15 +291,15 @@
             model = models.CreateContentReviewTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEnhanceMediaTemplate(self, request):
         """创建音画质重生模板。
 
         :param request: Request instance for CreateEnhanceMediaTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.CreateEnhanceMediaTemplateRequest`
@@ -314,15 +314,15 @@
             model = models.CreateEnhanceMediaTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateHeadTailTemplate(self, request):
         """创建片头片尾模板。
 
         :param request: Request instance for CreateHeadTailTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.CreateHeadTailTemplateRequest`
@@ -337,15 +337,15 @@
             model = models.CreateHeadTailTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateImageProcessingTemplate(self, request):
         """创建一个用户自定义的图片处理模板，数量上限：16。最多支持十次操作，例如：裁剪-缩略-裁剪-模糊-缩略-裁剪-缩略-裁剪-模糊-缩略。
 
         :param request: Request instance for CreateImageProcessingTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.CreateImageProcessingTemplateRequest`
@@ -360,15 +360,15 @@
             model = models.CreateImageProcessingTemplateResponse()
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
         :type request: :class:`tencentcloud.vod.v20180717.models.CreateImageSpriteTemplateRequest`
@@ -383,15 +383,15 @@
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
         """该接口用于创建素材样本，用于通过五官定位等技术，进行内容识别、不适宜视频识别等视频处理。
 
         :param request: Request instance for CreatePersonSample.
         :type request: :class:`tencentcloud.vod.v20180717.models.CreatePersonSampleRequest`
@@ -406,15 +406,15 @@
             model = models.CreatePersonSampleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateProcedureTemplate(self, request):
         """创建用户自定义的任务流模板，模板上限：50。
 
         :param request: Request instance for CreateProcedureTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.CreateProcedureTemplateRequest`
@@ -429,15 +429,15 @@
             model = models.CreateProcedureTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateQualityInspectTemplate(self, request):
         """创建音画质检测模板。
 
         :param request: Request instance for CreateQualityInspectTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.CreateQualityInspectTemplateRequest`
@@ -452,15 +452,15 @@
             model = models.CreateQualityInspectTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRebuildMediaTemplate(self, request):
         """创建视频重生模板。
 
         :param request: Request instance for CreateRebuildMediaTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.CreateRebuildMediaTemplateRequest`
@@ -475,15 +475,15 @@
             model = models.CreateRebuildMediaTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateReviewTemplate(self, request):
         """创建用户自定义审核模板，数量上限：50。
         >模板仅适用于 [音视频审核(ReviewAudioVideo)](https://cloud.tencent.com/document/api/266/80283) 和 [图片审核(ReviewImage)](https://cloud.tencent.com/document/api/266/73217) 接口。
 
         :param request: Request instance for CreateReviewTemplate.
@@ -499,15 +499,15 @@
             model = models.CreateReviewTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRoundPlay(self, request):
         """该接口用于创建轮播播单，数量上限：100。
         轮播播单的每个文件可以指定源文件，也可以指定某个转码文件。
         指定的文件必须是hls格式，所有的播单文件最好保持相同的码率和分辨率。
 
@@ -524,15 +524,15 @@
             model = models.CreateRoundPlayResponse()
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
         :type request: :class:`tencentcloud.vod.v20180717.models.CreateSampleSnapshotTemplateRequest`
@@ -547,15 +547,15 @@
             model = models.CreateSampleSnapshotTemplateResponse()
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
         :type request: :class:`tencentcloud.vod.v20180717.models.CreateSnapshotByTimeOffsetTemplateRequest`
@@ -570,15 +570,15 @@
             model = models.CreateSnapshotByTimeOffsetTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateStorageRegion(self, request):
         """该接口用于开通某地域的存储。
           1. 用户开通点播业务时，系统默认为用户开通了部分地域的存储，用户如果需要开通其它地域的存储，可以通过该接口进行开通。
           2. 通过 DescribeStorageRegions 接口可以查询到所有存储地域及已经开通的地域。
 
@@ -595,15 +595,15 @@
             model = models.CreateStorageRegionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSubAppId(self, request):
         """该接口用于创建点播子应用。
 
         :param request: Request instance for CreateSubAppId.
         :type request: :class:`tencentcloud.vod.v20180717.models.CreateSubAppIdRequest`
@@ -618,15 +618,15 @@
             model = models.CreateSubAppIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSuperPlayerConfig(self, request):
         """该 API 已经<font color='red'>不再维护</font>，新版播放器签名不再使用播放器配置模板，详细请参考 [播放器签名](https://cloud.tencent.com/document/product/266/45554)。
         创建播放器配置，数量上限：100。
 
         :param request: Request instance for CreateSuperPlayerConfig.
@@ -642,15 +642,15 @@
             model = models.CreateSuperPlayerConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTranscodeTemplate(self, request):
         """创建用户自定义转码模板，数量上限：100。
 
         :param request: Request instance for CreateTranscodeTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.CreateTranscodeTemplateRequest`
@@ -665,15 +665,15 @@
             model = models.CreateTranscodeTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVodDomain(self, request):
         """该接口用于将加速域名添加到点播，一个用户最多添加20个加速域名。
         1.域名添加成功后点播会进行域名的部署，域名由部署状态变为在线状态大概需要2分钟的时间。
 
         :param request: Request instance for CreateVodDomain.
@@ -689,15 +689,15 @@
             model = models.CreateVodDomainResponse()
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
         :type request: :class:`tencentcloud.vod.v20180717.models.CreateWatermarkTemplateRequest`
@@ -712,15 +712,15 @@
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
         :type request: :class:`tencentcloud.vod.v20180717.models.CreateWordSamplesRequest`
@@ -735,15 +735,15 @@
             model = models.CreateWordSamplesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAIAnalysisTemplate(self, request):
         """删除用户自定义音视频内容分析模板。
 
         注意：模板 ID 为 10000 以下的为系统预置模板，不允许删除。
 
@@ -760,15 +760,15 @@
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
         """删除用户自定义音视频内容识别模板。
 
         :param request: Request instance for DeleteAIRecognitionTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.DeleteAIRecognitionTemplateRequest`
@@ -783,15 +783,15 @@
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
         :type request: :class:`tencentcloud.vod.v20180717.models.DeleteAdaptiveDynamicStreamingTemplateRequest`
@@ -806,15 +806,15 @@
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
         :type request: :class:`tencentcloud.vod.v20180717.models.DeleteAnimatedGraphicsTemplateRequest`
@@ -829,15 +829,15 @@
             model = models.DeleteAnimatedGraphicsTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteClass(self, request):
         """* 仅当待删分类无子分类且无媒体关联情况下，可删除分类；
         * 否则，请先执行[删除媒体](/document/product/266/31764)及子分类，再删除该分类；
 
         :param request: Request instance for DeleteClass.
@@ -853,15 +853,15 @@
             model = models.DeleteClassResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteContentReviewTemplate(self, request):
         """该 API 已经<font color=red>不再维护</font>，新版审核模板支持音视频审核和图片审核，详细请参考 [删除审核模板](https://cloud.tencent.com/document/api/266/84390)。
         删除用户自定义音视频内容审核模板。
 
         :param request: Request instance for DeleteContentReviewTemplate.
@@ -877,15 +877,15 @@
             model = models.DeleteContentReviewTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteEnhanceMediaTemplate(self, request):
         """删除音画质重生模板。
 
         :param request: Request instance for DeleteEnhanceMediaTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.DeleteEnhanceMediaTemplateRequest`
@@ -900,15 +900,15 @@
             model = models.DeleteEnhanceMediaTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteHeadTailTemplate(self, request):
         """删除片头片尾模板。
 
         :param request: Request instance for DeleteHeadTailTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.DeleteHeadTailTemplateRequest`
@@ -923,15 +923,15 @@
             model = models.DeleteHeadTailTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteImageProcessingTemplate(self, request):
         """删除用户自定义图片处理模板。
 
         :param request: Request instance for DeleteImageProcessingTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.DeleteImageProcessingTemplateRequest`
@@ -946,15 +946,15 @@
             model = models.DeleteImageProcessingTemplateResponse()
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
         :type request: :class:`tencentcloud.vod.v20180717.models.DeleteImageSpriteTemplateRequest`
@@ -969,15 +969,15 @@
             model = models.DeleteImageSpriteTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteMedia(self, request):
         """* 删除媒体及其对应的视频处理文件（原始文件、如转码视频、雪碧图、截图、微信发布视频等）；
         * 可单独删除指定 ID 的视频文件下的原文件、转码视频、微信发布视频等；
         * 注意：原文件删除后，无法发起转码、微信发布等任何视频处理操作。
 
@@ -994,15 +994,15 @@
             model = models.DeleteMediaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePersonSample(self, request):
         """该接口用于根据人物 ID，删除素材样本。
 
         :param request: Request instance for DeletePersonSample.
         :type request: :class:`tencentcloud.vod.v20180717.models.DeletePersonSampleRequest`
@@ -1017,15 +1017,15 @@
             model = models.DeletePersonSampleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteProcedureTemplate(self, request):
         """删除用户自定义的任务流模板。
 
         :param request: Request instance for DeleteProcedureTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.DeleteProcedureTemplateRequest`
@@ -1040,15 +1040,15 @@
             model = models.DeleteProcedureTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteQualityInspectTemplate(self, request):
         """删除音画质检测模板。
 
         :param request: Request instance for DeleteQualityInspectTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.DeleteQualityInspectTemplateRequest`
@@ -1063,15 +1063,15 @@
             model = models.DeleteQualityInspectTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRebuildMediaTemplate(self, request):
         """删除视频重生模板。
 
         :param request: Request instance for DeleteRebuildMediaTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.DeleteRebuildMediaTemplateRequest`
@@ -1086,15 +1086,15 @@
             model = models.DeleteRebuildMediaTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteReviewTemplate(self, request):
         """删除用户自定义审核模板。
         >模板仅适用于 [音视频审核(ReviewAudioVideo)](https://cloud.tencent.com/document/api/266/80283) 和 [图片审核(ReviewImage)](https://cloud.tencent.com/document/api/266/73217) 接口。
 
         :param request: Request instance for DeleteReviewTemplate.
@@ -1110,15 +1110,15 @@
             model = models.DeleteReviewTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRoundPlay(self, request):
         """该接口用于删除轮播播单。
 
         :param request: Request instance for DeleteRoundPlay.
         :type request: :class:`tencentcloud.vod.v20180717.models.DeleteRoundPlayRequest`
@@ -1133,15 +1133,15 @@
             model = models.DeleteRoundPlayResponse()
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
         :type request: :class:`tencentcloud.vod.v20180717.models.DeleteSampleSnapshotTemplateRequest`
@@ -1156,15 +1156,15 @@
             model = models.DeleteSampleSnapshotTemplateResponse()
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
         :type request: :class:`tencentcloud.vod.v20180717.models.DeleteSnapshotByTimeOffsetTemplateRequest`
@@ -1179,15 +1179,15 @@
             model = models.DeleteSnapshotByTimeOffsetTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSuperPlayerConfig(self, request):
         """该 API 已经<font color='red'>不再维护</font>，新版播放器签名不再使用播放器配置模板，详细请参考 [播放器签名](https://cloud.tencent.com/document/product/266/45554)。
         删除播放器配置。
         *注：系统预置播放器配置不允许删除。*
 
@@ -1204,15 +1204,15 @@
             model = models.DeleteSuperPlayerConfigResponse()
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
         :type request: :class:`tencentcloud.vod.v20180717.models.DeleteTranscodeTemplateRequest`
@@ -1227,15 +1227,15 @@
             model = models.DeleteTranscodeTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteVodDomain(self, request):
         """该接口用于删除点播加速域名。
         1、域名删除前需要先关闭所有区域的加速。
 
         :param request: Request instance for DeleteVodDomain.
@@ -1251,15 +1251,15 @@
             model = models.DeleteVodDomainResponse()
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
         :type request: :class:`tencentcloud.vod.v20180717.models.DeleteWatermarkTemplateRequest`
@@ -1274,15 +1274,15 @@
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
         :type request: :class:`tencentcloud.vod.v20180717.models.DeleteWordSamplesRequest`
@@ -1297,15 +1297,15 @@
             model = models.DeleteWordSamplesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAIAnalysisTemplates(self, request):
         """根据音视频内容分析模板唯一标识，获取音视频内容分析模板详情列表。返回结果包含符合条件的所有用户自定义音视频内容分析模板及[系统预置音视频内容分析模板](https://cloud.tencent.com/document/product/266/33476#.E9.A2.84.E7.BD.AE.E8.A7.86.E9.A2.91.E5.86.85.E5.AE.B9.E5.88.86.E6.9E.90.E6.A8.A1.E6.9D.BF)。
 
         :param request: Request instance for DescribeAIAnalysisTemplates.
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribeAIAnalysisTemplatesRequest`
@@ -1320,15 +1320,15 @@
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
         """根据音视频内容识别模板唯一标识，获取音视频内容识别模板详情列表。返回结果包含符合条件的所有用户自定义音视频内容识别模板及[系统预置音视频内容识别模板](https://cloud.tencent.com/document/product/266/33476#.E9.A2.84.E7.BD.AE.E8.A7.86.E9.A2.91.E5.86.85.E5.AE.B9.E8.AF.86.E5.88.AB.E6.A8.A1.E6.9D.BF)。
 
         :param request: Request instance for DescribeAIRecognitionTemplates.
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribeAIRecognitionTemplatesRequest`
@@ -1343,15 +1343,15 @@
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
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribeAdaptiveDynamicStreamingTemplatesRequest`
@@ -1366,15 +1366,15 @@
             model = models.DescribeAdaptiveDynamicStreamingTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAllClass(self, request):
         """* 获得用户的所有分类信息。
 
         :param request: Request instance for DescribeAllClass.
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribeAllClassRequest`
@@ -1389,15 +1389,15 @@
             model = models.DescribeAllClassResponse()
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
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribeAnimatedGraphicsTemplatesRequest`
@@ -1412,15 +1412,15 @@
             model = models.DescribeAnimatedGraphicsTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCDNStatDetails(self, request):
         """该接口用于查询点播域名的 CDN 带宽、流量等统计数据。
         * 查询的起始时间和结束时间跨度不超过90天。
         * 可以查询不同服务区域的数据。
         * 中国境内的数据支持查询指定地区、运营商的统计数据。
@@ -1438,15 +1438,15 @@
             model = models.DescribeCDNStatDetailsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCDNUsageData(self, request):
         """该接口用于查询点播 CDN 的流量、带宽等统计数据。
            1. 可以查询最近365天内的 CDN 用量数据。
            2.  查询时间跨度不超过90天。
            3. 可以指定用量数据的时间粒度，支持5分钟、1小时、1天的时间粒度。
@@ -1465,15 +1465,15 @@
             model = models.DescribeCDNUsageDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCdnLogs(self, request):
         """查询点播域名的 CDN 访问日志的下载链接。
             1. 可以查询最近30天内的 CDN 日志下载链接。
             2. 默认情况下 CDN 每小时生成一个日志文件，如果某一个小时没有 CDN 访问，不会生成日志文件。
             3. CDN 日志下载链接的有效期为24小时。
@@ -1491,15 +1491,15 @@
             model = models.DescribeCdnLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClientUploadAccelerationUsageData(self, request):
         """该接口返回查询时间范围内客户端上传加速统计信息。
            1. 可以查询最近365天内的客户端上传加速统计数据。
            2. 查询时间跨度不超过90天。
            3. 查询时间跨度超过1天的，返回以天为粒度的数据，否则，返回以5分钟为粒度的数据。
@@ -1517,15 +1517,15 @@
             model = models.DescribeClientUploadAccelerationUsageDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeContentReviewTemplates(self, request):
         """该 API 已经<font color=red>不再维护</font>，新版审核模板支持音视频审核和图片审核，详细请参考 [获取审核模板列表](https://cloud.tencent.com/document/api/266/84389)。
         根据音视频内容审核模板唯一标识，获取音视频内容审核模板详情列表。返回结果包含符合条件的所有用户自定义模板及[系统预置内容审核模板](https://cloud.tencent.com/document/product/266/33476#.E9.A2.84.E7.BD.AE.E8.A7.86.E9.A2.91.E5.86.85.E5.AE.B9.E5.AE.A1.E6.A0.B8.E6.A8.A1.E6.9D.BF)。
 
         :param request: Request instance for DescribeContentReviewTemplates.
@@ -1541,15 +1541,15 @@
             model = models.DescribeContentReviewTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDailyMediaPlayStat(self, request):
         """该接口用于查询指定日期范围内每天的播放统计数据。
         * 可以查询最近一年的播放统计数据。
         * 结束日期和起始日期的时间跨度最大为90天。
 
@@ -1566,15 +1566,15 @@
             model = models.DescribeDailyMediaPlayStatResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDailyMostPlayedStat(self, request):
         """该接口用于查询每日播放Top100 的媒体文件的播放统计数据。
         * 可以查询最近一年的播放统计数据。
         * 可以按播放次数或者播放流量查询。
         * 播放次数统计说明：
@@ -1594,15 +1594,15 @@
             model = models.DescribeDailyMostPlayedStatResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDailyPlayStatFileList(self, request):
         """该接口用于查询播放统计文件的下载地址。
         * 可以查询最近一年的播放统计文件下载地址，查询的起始日期和结束日期的时间跨度不超过90天。
         * 云点播每天对前一天的 CDN 请求日志进行分析处理，生成播放统计文件。
         * 播放统计文件内容包含媒体文件的播放次数、播放流量等统计信息。
@@ -1624,15 +1624,15 @@
             model = models.DescribeDailyPlayStatFileListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDrmDataKey(self, request):
         """本 API 是 [旧版本加密](https://cloud.tencent.com/document/product/266/9638) 中 [DescribeDrmDataKey 的 API 2017 接口](https://cloud.tencent.com/document/product/266/9643) 的升级版本。
 
         如果您是新接入点播加密的用户，不要使用该 API，请参考 [视频加密综述](https://cloud.tencent.com/document/product/266/45552) 使用推荐的加密方式。
 
@@ -1649,15 +1649,15 @@
             model = models.DescribeDrmDataKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDrmKeyProviderInfo(self, request):
         """查询 DRM 密钥提供商信息。
 
         :param request: Request instance for DescribeDrmKeyProviderInfo.
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribeDrmKeyProviderInfoRequest`
@@ -1672,15 +1672,15 @@
             model = models.DescribeDrmKeyProviderInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEnhanceMediaTemplates(self, request):
         """获取音画质重生模板列表。
 
         :param request: Request instance for DescribeEnhanceMediaTemplates.
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribeEnhanceMediaTemplatesRequest`
@@ -1695,15 +1695,15 @@
             model = models.DescribeEnhanceMediaTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEventConfig(self, request):
         """腾讯云点播为客户提供了媒体上传、媒体管理、媒体处理等等服务，在这些服务执行过程或执行结束时，腾讯云点播也提供各种对应的事件通知，方便开发者感知服务处理状态，并做下一步的业务操作。
 
         开发者可以通过本接口来查询当前配置事件通知的接收方式、接收地址以及哪些事件开启了接收回调通知。
 
@@ -1722,15 +1722,15 @@
             model = models.DescribeEventConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEventsState(self, request):
         """* 该接口用于业务服务器获取 [可靠回调](https://cloud.tencent.com/document/product/266/33779#.E5.8F.AF.E9.9D.A0.E5.9B.9E.E8.B0.83) 事件通知的状态。
 
         :param request: Request instance for DescribeEventsState.
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribeEventsStateRequest`
@@ -1745,15 +1745,15 @@
             model = models.DescribeEventsStateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFileAttributes(self, request):
         """用于异步获取文件属性。
         - 当前仅支持获取源文件的 Md5。
         - 对输入文件为 HLS 或 DASH 的情况，仅获取索引文件的属性。
 
@@ -1770,15 +1770,15 @@
             model = models.DescribeFileAttributesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHeadTailTemplates(self, request):
         """获取片头片尾模板列表。
 
         :param request: Request instance for DescribeHeadTailTemplates.
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribeHeadTailTemplatesRequest`
@@ -1793,15 +1793,15 @@
             model = models.DescribeHeadTailTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageProcessingTemplates(self, request):
         """获取图片处理模板列表，支持根据条件，分页查询。
 
         :param request: Request instance for DescribeImageProcessingTemplates.
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribeImageProcessingTemplatesRequest`
@@ -1816,15 +1816,15 @@
             model = models.DescribeImageProcessingTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageReviewUsageData(self, request):
         """该接口返回查询时间范围内每天使用的图片审核用量信息。
            1. 可以查询最近365天内的图片审核统计数据。
            2. 查询时间跨度不超过90天。
            3. 查询时间跨度超过1天的，返回以天为粒度的数据，否则，返回以5分钟为粒度的数据。
@@ -1842,15 +1842,15 @@
             model = models.DescribeImageReviewUsageDataResponse()
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
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribeImageSpriteTemplatesRequest`
@@ -1865,15 +1865,15 @@
             model = models.DescribeImageSpriteTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLicenseUsageData(self, request):
         """该接口返回查询时间范围内每天 License 请求次数信息。
            1. 可以查询最近365天内的 License 请求次数统计数据。
            2. 查询时间跨度不超过90天。
            3. 查询时间跨度超过1天的，返回以天为粒度的数据，否则，返回以5分钟为粒度的数据。
@@ -1891,15 +1891,15 @@
             model = models.DescribeLicenseUsageDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMediaInfos(self, request):
         """1. 该接口可以获取多个媒体文件的多种信息，包括：
             1. 基础信息（basicInfo）：包括媒体名称、分类、播放地址、封面图片等。
             2. 元信息（metaData）：包括大小、时长、视频流信息、音频流信息等。
             3. 转码结果信息（transcodeInfo）：包括该媒体转码生成的各种规格的媒体地址、视频流参数、音频流参数等。
@@ -1925,15 +1925,15 @@
             model = models.DescribeMediaInfosResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMediaPlayStatDetails(self, request):
         """该接口用于查询媒体文件按指定时间粒度统计的播放数据
         * 可以查询最近一年的播放统计数据。
         * 时间粒度为小时，结束时间和起始时间的跨度最大为7天。
         * 时间粒度为天，结束时间和起始时间的跨度最大为90天。
@@ -1951,15 +1951,15 @@
             model = models.DescribeMediaPlayStatDetailsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMediaProcessUsageData(self, request):
         """该接口返回查询时间范围内每天使用的视频处理用量信息。
            1. 可以查询最近365天内的视频处理统计数据。
            2. 查询时间跨度不超过90天。
 
@@ -1976,15 +1976,15 @@
             model = models.DescribeMediaProcessUsageDataResponse()
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
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribePersonSamplesRequest`
@@ -1999,15 +1999,15 @@
             model = models.DescribePersonSamplesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrepaidProducts(self, request):
         """该接口可以查询用户已经购买的预付费商品的信息，包括：
             1. 商品的类型、生效和失效日期。
             2. 商品中每种资源的额度和剩余额度。
 
@@ -2024,15 +2024,15 @@
             model = models.DescribePrepaidProductsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProcedureTemplates(self, request):
         """根据任务流模板名字，获取任务流模板详情列表。
 
         :param request: Request instance for DescribeProcedureTemplates.
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribeProcedureTemplatesRequest`
@@ -2047,15 +2047,15 @@
             model = models.DescribeProcedureTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeQualityInspectTemplates(self, request):
         """获取音画质检测模板列表。
 
         :param request: Request instance for DescribeQualityInspectTemplates.
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribeQualityInspectTemplatesRequest`
@@ -2070,15 +2070,15 @@
             model = models.DescribeQualityInspectTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRebuildMediaTemplates(self, request):
         """获取视频重生模板列表。
 
         :param request: Request instance for DescribeRebuildMediaTemplates.
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribeRebuildMediaTemplatesRequest`
@@ -2093,15 +2093,15 @@
             model = models.DescribeRebuildMediaTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeReviewDetails(self, request):
         """<b>本接口已不推荐使用，用 [DescribeMediaProcessUsageData](/document/product/266/41464) 替代</b>
 
         该接口返回查询时间范围内每天使用的视频内容智能识别时长数据，单位： 秒。
 
@@ -2121,15 +2121,15 @@
             model = models.DescribeReviewDetailsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeReviewTemplates(self, request):
         """获取审核模板列表。
         >模板仅适用于 [音视频审核(ReviewAudioVideo)](https://cloud.tencent.com/document/api/266/80283) 和 [图片审核(ReviewImage)](https://cloud.tencent.com/document/api/266/73217) 接口。
 
         :param request: Request instance for DescribeReviewTemplates.
@@ -2145,15 +2145,15 @@
             model = models.DescribeReviewTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRoundPlays(self, request):
         """该接口用于获取轮播播单列表。
 
         :param request: Request instance for DescribeRoundPlays.
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribeRoundPlaysRequest`
@@ -2168,15 +2168,15 @@
             model = models.DescribeRoundPlaysResponse()
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
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribeSampleSnapshotTemplatesRequest`
@@ -2191,15 +2191,15 @@
             model = models.DescribeSampleSnapshotTemplatesResponse()
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
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribeSnapshotByTimeOffsetTemplatesRequest`
@@ -2214,15 +2214,15 @@
             model = models.DescribeSnapshotByTimeOffsetTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStorageData(self, request):
         """查询存储空间使用情况和文件数量。
 
         :param request: Request instance for DescribeStorageData.
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribeStorageDataRequest`
@@ -2237,15 +2237,15 @@
             model = models.DescribeStorageDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStorageDetails(self, request):
         """该接口返回查询时间范围内使用的点播存储空间，单位：字节。
             1. 可以查询最近365天内的存储空间数据；
             2. 查询时间跨度不超过90天；
             3. 分钟粒度查询跨度不超过7天；
@@ -2263,15 +2263,15 @@
             model = models.DescribeStorageDetailsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStorageRegions(self, request):
         """该接口用于：
           1. 查询点播可开通的所有存储园区列表。
           2. 查询已经开通的园区列表。
           3. 查询默认使用的存储园区。
@@ -2289,15 +2289,15 @@
             model = models.DescribeStorageRegionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSubAppIds(self, request):
         """该接口用于获取当前账号的子应用列表，包含主应用。
 
         :param request: Request instance for DescribeSubAppIds.
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribeSubAppIdsRequest`
@@ -2312,15 +2312,15 @@
             model = models.DescribeSubAppIdsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSuperPlayerConfigs(self, request):
         """该 API 已经<font color='red'>不再维护</font>，新版播放器签名不再使用播放器配置模板，详细请参考 [播放器签名](https://cloud.tencent.com/document/product/266/45554)。
         查询播放器配置，支持根据条件，分页查询。
 
         :param request: Request instance for DescribeSuperPlayerConfigs.
@@ -2336,15 +2336,15 @@
             model = models.DescribeSuperPlayerConfigsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskDetail(self, request):
         """通过任务 ID 查询任务的执行状态和结果的详细信息（最多可以查询3天之内提交的任务）。
 
         :param request: Request instance for DescribeTaskDetail.
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribeTaskDetailRequest`
@@ -2359,15 +2359,15 @@
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
         * 只能查询到最近三天（72 小时）内的任务。
 
@@ -2384,15 +2384,15 @@
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
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribeTranscodeTemplatesRequest`
@@ -2407,15 +2407,15 @@
             model = models.DescribeTranscodeTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVodDomains(self, request):
         """该接口用于查询点播域名信息列表。
 
         :param request: Request instance for DescribeVodDomains.
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribeVodDomainsRequest`
@@ -2430,15 +2430,15 @@
             model = models.DescribeVodDomainsResponse()
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
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribeWatermarkTemplatesRequest`
@@ -2453,15 +2453,15 @@
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
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribeWordSamplesRequest`
@@ -2476,15 +2476,15 @@
             model = models.DescribeWordSamplesResponse()
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
 
         1. 对点播中的一个文件进行剪辑，生成一个新的视频；
         2. 对点播中的多个文件进行拼接，生成一个新的视频；
@@ -2513,15 +2513,15 @@
             model = models.EditMediaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnhanceMediaByTemplate(self, request):
         """使用模板发起音画质重生。
 
         :param request: Request instance for EnhanceMediaByTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.EnhanceMediaByTemplateRequest`
@@ -2536,15 +2536,15 @@
             model = models.EnhanceMediaByTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExecuteFunction(self, request):
         """本接口仅用于定制开发的特殊场景，除非云点播客服人员主动告知您需要使用本接口，其它情况请勿调用。
 
         :param request: Request instance for ExecuteFunction.
         :type request: :class:`tencentcloud.vod.v20180717.models.ExecuteFunctionRequest`
@@ -2559,15 +2559,15 @@
             model = models.ExecuteFunctionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExtractCopyRightWatermark(self, request):
         """提取版权水印信息。
 
         :param request: Request instance for ExtractCopyRightWatermark.
         :type request: :class:`tencentcloud.vod.v20180717.models.ExtractCopyRightWatermarkRequest`
@@ -2582,15 +2582,15 @@
             model = models.ExtractCopyRightWatermarkResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExtractTraceWatermark(self, request):
         """用于提取溯源水印。
 
         :param request: Request instance for ExtractTraceWatermark.
         :type request: :class:`tencentcloud.vod.v20180717.models.ExtractTraceWatermarkRequest`
@@ -2605,15 +2605,15 @@
             model = models.ExtractTraceWatermarkResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ForbidMediaDistribution(self, request):
         """* 对媒体禁播后，除了点播控制台预览，其他场景访问视频各种资源的 URL（原始文件、转码输出文件、截图等）均会返回 403。
           禁播/解禁操作全网生效时间约 5~10 分钟。
 
         :param request: Request instance for ForbidMediaDistribution.
@@ -2629,15 +2629,15 @@
             model = models.ForbidMediaDistributionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InspectMediaQuality(self, request):
         """对点播中的音视频媒体发起音画质检测任务。
 
         :param request: Request instance for InspectMediaQuality.
         :type request: :class:`tencentcloud.vod.v20180717.models.InspectMediaQualityRequest`
@@ -2652,15 +2652,15 @@
             model = models.InspectMediaQualityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def LiveRealTimeClip(self, request):
         """直播即时剪辑，是指在直播过程中（即直播尚未结束时），客户可以在过往直播内容中选择一段，实时生成一个新的视频（HLS 格式），开发者可以将其立即分享出去，或者长久保存起来。
 
         腾讯云点播支持两种即时剪辑模式：
         - 剪辑固化：将剪辑出来的视频保存成独立的视频，拥有独立 FileId；适用于将精彩片段**长久保存**的场景；
@@ -2698,15 +2698,15 @@
             model = models.LiveRealTimeClipResponse()
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
         :type request: :class:`tencentcloud.vod.v20180717.models.ManageTaskRequest`
@@ -2721,15 +2721,15 @@
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
         """修改用户自定义音视频内容分析模板。
 
         注意：模板 ID 10000 以下的为系统预置模板，不允许修改。
 
@@ -2746,15 +2746,15 @@
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
         """修改用户自定义音视频内容识别模板。
 
         :param request: Request instance for ModifyAIRecognitionTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.ModifyAIRecognitionTemplateRequest`
@@ -2769,15 +2769,15 @@
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
         :type request: :class:`tencentcloud.vod.v20180717.models.ModifyAdaptiveDynamicStreamingTemplateRequest`
@@ -2792,15 +2792,15 @@
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
         :type request: :class:`tencentcloud.vod.v20180717.models.ModifyAnimatedGraphicsTemplateRequest`
@@ -2815,15 +2815,15 @@
             model = models.ModifyAnimatedGraphicsTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyClass(self, request):
         """修改媒体分类属性。
 
         :param request: Request instance for ModifyClass.
         :type request: :class:`tencentcloud.vod.v20180717.models.ModifyClassRequest`
@@ -2838,15 +2838,15 @@
             model = models.ModifyClassResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyContentReviewTemplate(self, request):
         """该 API 已经<font color=red>不再维护</font>，新版审核模板支持音视频审核和图片审核，详细请参考 [修改审核模板](https://cloud.tencent.com/document/api/266/84388)。
         修改用户自定义音视频内容审核模板。
 
         :param request: Request instance for ModifyContentReviewTemplate.
@@ -2862,15 +2862,15 @@
             model = models.ModifyContentReviewTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDefaultStorageRegion(self, request):
         """该接口用于设置默认的存储地域。上传文件时如果没有指定地域，将上传到默认地域。
 
         :param request: Request instance for ModifyDefaultStorageRegion.
         :type request: :class:`tencentcloud.vod.v20180717.models.ModifyDefaultStorageRegionRequest`
@@ -2885,15 +2885,15 @@
             model = models.ModifyDefaultStorageRegionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyEnhanceMediaTemplate(self, request):
         """修改音画质重生模板。
 
         :param request: Request instance for ModifyEnhanceMediaTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.ModifyEnhanceMediaTemplateRequest`
@@ -2908,15 +2908,15 @@
             model = models.ModifyEnhanceMediaTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyEventConfig(self, request):
         """腾讯云点播为客户提供了媒体上传、媒体管理、媒体处理等等服务，在这些服务执行过程或执行结束时，腾讯云点播也提供各种对应的事件通知，方便开发者感知服务处理状态，并做下一步的业务操作。
 
         开发者可以通过调用本接口来实现：
         - 设置接收回调通知的类型，目前有[ HTTP 回调通知](https://cloud.tencent.com/document/product/266/33779) 和 [基于消息队列的可靠通知](https://cloud.tencent.com/document/product/266/33779) 两种类型。
@@ -2936,15 +2936,15 @@
             model = models.ModifyEventConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyHeadTailTemplate(self, request):
         """修改片头片尾模板。
 
         :param request: Request instance for ModifyHeadTailTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.ModifyHeadTailTemplateRequest`
@@ -2959,15 +2959,15 @@
             model = models.ModifyHeadTailTemplateResponse()
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
         :type request: :class:`tencentcloud.vod.v20180717.models.ModifyImageSpriteTemplateRequest`
@@ -2982,15 +2982,15 @@
             model = models.ModifyImageSpriteTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyMediaInfo(self, request):
         """修改媒体文件的属性，包括分类、名称、描述、标签、过期时间、打点信息、视频封面、字幕信息等。
 
         :param request: Request instance for ModifyMediaInfo.
         :type request: :class:`tencentcloud.vod.v20180717.models.ModifyMediaInfoRequest`
@@ -3005,15 +3005,15 @@
             model = models.ModifyMediaInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyMediaStorageClass(self, request):
         """修改媒体文件的存储类型。
         当媒体文件的存储类型为标准存储时，可以修改为以下类型：
         <li>低频存储</li>
         <li>归档存储</li>
@@ -3040,15 +3040,15 @@
             model = models.ModifyMediaStorageClassResponse()
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
         :type request: :class:`tencentcloud.vod.v20180717.models.ModifyPersonSampleRequest`
@@ -3063,15 +3063,15 @@
             model = models.ModifyPersonSampleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyQualityInspectTemplate(self, request):
         """修改音画质检测模板。
 
         :param request: Request instance for ModifyQualityInspectTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.ModifyQualityInspectTemplateRequest`
@@ -3086,15 +3086,15 @@
             model = models.ModifyQualityInspectTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRebuildMediaTemplate(self, request):
         """修改视频重生模板。
 
         :param request: Request instance for ModifyRebuildMediaTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.ModifyRebuildMediaTemplateRequest`
@@ -3109,15 +3109,15 @@
             model = models.ModifyRebuildMediaTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyReviewTemplate(self, request):
         """修改用户自定义审核模板。
         >模板仅适用于 [音视频审核(ReviewAudioVideo)](https://cloud.tencent.com/document/api/266/80283) 和 [图片审核(ReviewImage)](https://cloud.tencent.com/document/api/266/73217) 接口。
 
         :param request: Request instance for ModifyReviewTemplate.
@@ -3133,15 +3133,15 @@
             model = models.ModifyReviewTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRoundPlay(self, request):
         """该接口用于修改轮播播单。
         修改后只有新的播放请求会生效，已经在播放中的用户在七天之内还可以播放修改前的播单。
 
         :param request: Request instance for ModifyRoundPlay.
@@ -3157,15 +3157,15 @@
             model = models.ModifyRoundPlayResponse()
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
         :type request: :class:`tencentcloud.vod.v20180717.models.ModifySampleSnapshotTemplateRequest`
@@ -3180,15 +3180,15 @@
             model = models.ModifySampleSnapshotTemplateResponse()
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
         :type request: :class:`tencentcloud.vod.v20180717.models.ModifySnapshotByTimeOffsetTemplateRequest`
@@ -3203,15 +3203,15 @@
             model = models.ModifySnapshotByTimeOffsetTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySubAppIdInfo(self, request):
         """该接口用于修改子应用信息，但不允许修改主应用信息。
 
         :param request: Request instance for ModifySubAppIdInfo.
         :type request: :class:`tencentcloud.vod.v20180717.models.ModifySubAppIdInfoRequest`
@@ -3226,15 +3226,15 @@
             model = models.ModifySubAppIdInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySubAppIdStatus(self, request):
         """该接口用于启用、停用子应用。被停用的子应用将封停对应域名，并限制控制台访问。
 
         :param request: Request instance for ModifySubAppIdStatus.
         :type request: :class:`tencentcloud.vod.v20180717.models.ModifySubAppIdStatusRequest`
@@ -3249,15 +3249,15 @@
             model = models.ModifySubAppIdStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySuperPlayerConfig(self, request):
         """该 API 已经<font color='red'>不再维护</font>，新版播放器签名不再使用播放器配置模板，详细请参考 [播放器签名](https://cloud.tencent.com/document/product/266/45554)。
         修改播放器配置。
 
         :param request: Request instance for ModifySuperPlayerConfig.
@@ -3273,15 +3273,15 @@
             model = models.ModifySuperPlayerConfigResponse()
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
         :type request: :class:`tencentcloud.vod.v20180717.models.ModifyTranscodeTemplateRequest`
@@ -3296,15 +3296,15 @@
             model = models.ModifyTranscodeTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyVodDomainAccelerateConfig(self, request):
         """该接口用于修改点播域名的加速区域。
         1、域名部署状态为 Online 状态时才允许修改加速区域。
 
         :param request: Request instance for ModifyVodDomainAccelerateConfig.
@@ -3320,15 +3320,15 @@
             model = models.ModifyVodDomainAccelerateConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyVodDomainConfig(self, request):
         """该接口用于修改域名配置，可以修改域名的防盗链配置。
         1、域名部署状态为 Online 状态时才允许修改域名的配置。
 
         :param request: Request instance for ModifyVodDomainConfig.
@@ -3344,15 +3344,15 @@
             model = models.ModifyVodDomainConfigResponse()
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
         :type request: :class:`tencentcloud.vod.v20180717.models.ModifyWatermarkTemplateRequest`
@@ -3367,15 +3367,15 @@
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
         :type request: :class:`tencentcloud.vod.v20180717.models.ModifyWordSampleRequest`
@@ -3390,15 +3390,15 @@
             model = models.ModifyWordSampleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ParseStreamingManifest(self, request):
         """上传 HLS 视频时，解析索引文件内容，返回待上传的分片文件列表。分片文件路径必须是当前目录或子目录的相对路径，不能是 URL，不能是绝对路径。
 
         :param request: Request instance for ParseStreamingManifest.
         :type request: :class:`tencentcloud.vod.v20180717.models.ParseStreamingManifestRequest`
@@ -3413,15 +3413,15 @@
             model = models.ParseStreamingManifestResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ProcessImage(self, request):
         """该 API 已经<font color='red'>不再维护</font>，智能识别任务请使用图片智能识别 [ReviewImage](https://cloud.tencent.com/document/api/266/73217) 接口。
 
         对点播中的图片文件发起处理任务，功能包括：
 
@@ -3444,15 +3444,15 @@
             model = models.ProcessImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ProcessMedia(self, request):
         """对点播中的音视频媒体发起处理任务，功能包括：
         1. 视频转码（带水印）；
         2. 视频转动图；
         3. 对视频按指定时间点截图；
@@ -3479,15 +3479,15 @@
             model = models.ProcessMediaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ProcessMediaByProcedure(self, request):
         """使用任务流模板，对点播中的视频发起处理任务。
         有两种方式创建任务流模板：
         1. 在控制台上创建和修改任务流模板；
         2. 通过任务流模板接口创建任务流模板。
@@ -3507,15 +3507,15 @@
             model = models.ProcessMediaByProcedureResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ProcessMediaByUrl(self, request):
         """该 API 已经<font color='red'>不再维护</font>，请使用 MPS 产品的 [ProcessMedia](https://cloud.tencent.com/document/product/862/37578) 接口，在入参 InputInfo.UrlInputInfo.Url 中指定视频 URL。
 
         :param request: Request instance for ProcessMediaByUrl.
         :type request: :class:`tencentcloud.vod.v20180717.models.ProcessMediaByUrlRequest`
@@ -3530,15 +3530,15 @@
             model = models.ProcessMediaByUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PullEvents(self, request):
         """* 该接口用于业务服务器以 [可靠回调](https://cloud.tencent.com/document/product/266/33779#.E5.8F.AF.E9.9D.A0.E5.9B.9E.E8.B0.83) 的方式获取事件通知；
         * 接口为长轮询模式，即：如果服务端存在未消费事件，则立即返回给请求方；如果服务端没有未消费事件，则后台会将请求挂起，直到有新的事件产生为止；
         * 请求最多挂起5秒，建议请求方将超时时间设置为10秒；
         * 未被拉取的事件通知最多保留4天，超过该时限的事件通知可能会被清除；
@@ -3558,15 +3558,15 @@
             model = models.PullEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PullUpload(self, request):
         """该接口用于将一个网络上的视频拉取到云点播平台。
 
         :param request: Request instance for PullUpload.
         :type request: :class:`tencentcloud.vod.v20180717.models.PullUploadRequest`
@@ -3581,15 +3581,15 @@
             model = models.PullUploadResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PushUrlCache(self, request):
         """1. 预热指定的 URL 列表。
         2. URL 的域名必须已在云点播中注册。
         3. 单次请求最多指定20个 URL。
         4. 默认预热配额为每天10000个 URL。
@@ -3607,15 +3607,15 @@
             model = models.PushUrlCacheResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RebuildMedia(self, request):
         """发起视频重生
 
         :param request: Request instance for RebuildMedia.
         :type request: :class:`tencentcloud.vod.v20180717.models.RebuildMediaRequest`
@@ -3630,15 +3630,15 @@
             model = models.RebuildMediaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RebuildMediaByTemplate(self, request):
         """使用模板发起视频重生。
 
         :param request: Request instance for RebuildMediaByTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.RebuildMediaByTemplateRequest`
@@ -3653,15 +3653,15 @@
             model = models.RebuildMediaByTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RefreshUrlCache(self, request):
         """1. 刷新指定的 URL 列表。
         2. URL 的域名必须已在云点播中注册。
         3. 单次请求最多指定20个 URL。
         4. 默认刷新配额为每天100000个 URL。
@@ -3679,15 +3679,15 @@
             model = models.RefreshUrlCacheResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RemoveWatermark(self, request):
         """智能去除水印
 
         :param request: Request instance for RemoveWatermark.
         :type request: :class:`tencentcloud.vod.v20180717.models.RemoveWatermarkRequest`
@@ -3702,15 +3702,15 @@
             model = models.RemoveWatermarkResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetProcedureTemplate(self, request):
         """重新设置用户自定义任务流模板的内容。
 
         :param request: Request instance for ResetProcedureTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.ResetProcedureTemplateRequest`
@@ -3725,15 +3725,15 @@
             model = models.ResetProcedureTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RestoreMedia(self, request):
         """当媒体文件的存储类型是归档存储或深度归档存储时，是不可访问的。如需访问，则需要调用本接口进行解冻，解冻后可访问的媒体文件是临时的，在有效期过后，则不可访问。
 
         :param request: Request instance for RestoreMedia.
         :type request: :class:`tencentcloud.vod.v20180717.models.RestoreMediaRequest`
@@ -3748,15 +3748,15 @@
             model = models.RestoreMediaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReviewAudioVideo(self, request):
         """对点播中的音视频媒体发起审核任务，智能检测视频画面、画面中的文字、语音中的文字、声音出现的违规内容。
 
         如使用事件通知，事件通知的类型为 [音视频审核完成](https://cloud.tencent.com/document/product/266/81258)。
 
@@ -3773,15 +3773,15 @@
             model = models.ReviewAudioVideoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReviewImage(self, request):
         """对点播中的图片文件发起审核（令人反感的信息、不安全的信息、不适宜的信息）任务。
 
         ><li>图片文件大小支持：文件 < 5M；</li>
         ><li>图片文件分辨率支持：建议分辨率大于256x256，否则可能会影响审核效果；</li>
@@ -3800,15 +3800,15 @@
             model = models.ReviewImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchMedia(self, request):
         """搜索媒体信息，支持多种条件筛选，以及支持对返回结果排序、过滤等功能，具体包括：
         - 指定文件 ID 集合 FileIds ，返回匹配集合中任意 ID 的媒体。
         - 根据多个媒体文件名 Names 或描述信息 Descriptions 进行模糊搜索。
         - 根据多个文件名前缀 NamePrefixes 进行搜索。
@@ -3863,15 +3863,15 @@
             model = models.SearchMediaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetDrmKeyProviderInfo(self, request):
         """设置 DRM 密钥提供商信息。
 
         :param request: Request instance for SetDrmKeyProviderInfo.
         :type request: :class:`tencentcloud.vod.v20180717.models.SetDrmKeyProviderInfoRequest`
@@ -3886,15 +3886,15 @@
             model = models.SetDrmKeyProviderInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SimpleHlsClip(self, request):
         """对 HLS 视频进行按时间段裁剪，实时生成一个新的视频（HLS 格式），开发者可以将其立即分享出去，或者长久保存起来。
 
         腾讯云点播支持两种剪辑模式：
         - 剪辑固化：将剪辑出来的视频保存成独立的视频，拥有独立 FileId；适用于将精彩片段长久保存的场景；
@@ -3931,15 +3931,15 @@
             model = models.SimpleHlsClipResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SplitMedia(self, request):
         """对点播视频进行拆条，生成多个新的点播视频。
 
         :param request: Request instance for SplitMedia.
         :type request: :class:`tencentcloud.vod.v20180717.models.SplitMediaRequest`
@@ -3954,15 +3954,15 @@
             model = models.SplitMediaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def WeChatMiniProgramPublish(self, request):
         """将点播视频发布到微信小程序，供微信小程序播放器播放。
         本接口支持发布原始视频和转码后视频，暂不支持发布自适应码流。
 
         :param request: Request instance for WeChatMiniProgramPublish.
@@ -3978,8 +3978,8 @@
             model = models.WeChatMiniProgramPublishResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-vod-3.0.937/tencentcloud/vod/v20180717/errorcodes.py` & `tencentcloud-sdk-python-vod-3.0.938/tencentcloud/vod/v20180717/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.937/tencentcloud/vod/v20180717/models.py` & `tencentcloud-sdk-python-vod-3.0.938/tencentcloud/vod/v20180717/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vod-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vod-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.937/README.rst` & `tencentcloud-sdk-python-vod-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.937/tencentcloud_sdk_python_vod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.938/tencentcloud_sdk_python_vod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

