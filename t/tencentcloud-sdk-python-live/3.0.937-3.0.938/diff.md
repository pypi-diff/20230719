# Comparing `tmp/tencentcloud-sdk-python-live-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-live-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.937.tar", last modified: Tue Jul 18 00:26:44 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.938.tar", last modified: Wed Jul 19 00:42:05 2023, max compression
```

## Comparing `tencentcloud-sdk-python-live-3.0.937.tar` & `tencentcloud-sdk-python-live-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:44.000000 tencentcloud-sdk-python-live-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:26:44.000000 tencentcloud-sdk-python-live-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:44.000000 tencentcloud-sdk-python-live-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:44.000000 tencentcloud-sdk-python-live-3.0.937/tencentcloud/live/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:44.000000 tencentcloud-sdk-python-live-3.0.937/tencentcloud/live/v20180801/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:26:44.000000 tencentcloud-sdk-python-live-3.0.937/tencentcloud/live/v20180801/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20054 2023-07-18 00:26:44.000000 tencentcloud-sdk-python-live-3.0.937/tencentcloud/live/v20180801/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   154127 2023-07-18 00:26:44.000000 tencentcloud-sdk-python-live-3.0.937/tencentcloud/live/v20180801/live_client.py
--rw-r--r--   0 root         (0) root         (0)   756667 2023-07-18 00:26:44.000000 tencentcloud-sdk-python-live-3.0.937/tencentcloud/live/v20180801/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:26:44.000000 tencentcloud-sdk-python-live-3.0.937/tencentcloud/live/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:26:44.000000 tencentcloud-sdk-python-live-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:26:44.000000 tencentcloud-sdk-python-live-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:44.000000 tencentcloud-sdk-python-live-3.0.937/tencentcloud_sdk_python_live.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:26:44.000000 tencentcloud-sdk-python-live-3.0.937/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:26:44.000000 tencentcloud-sdk-python-live-3.0.937/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:26:44.000000 tencentcloud-sdk-python-live-3.0.937/tencentcloud_sdk_python_live.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:26:44.000000 tencentcloud-sdk-python-live-3.0.937/tencentcloud_sdk_python_live.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:26:44.000000 tencentcloud-sdk-python-live-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:26:44.000000 tencentcloud-sdk-python-live-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:05.000000 tencentcloud-sdk-python-live-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:42:04.000000 tencentcloud-sdk-python-live-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:05.000000 tencentcloud-sdk-python-live-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:05.000000 tencentcloud-sdk-python-live-3.0.938/tencentcloud/live/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:05.000000 tencentcloud-sdk-python-live-3.0.938/tencentcloud/live/v20180801/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:42:04.000000 tencentcloud-sdk-python-live-3.0.938/tencentcloud/live/v20180801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20054 2023-07-19 00:42:04.000000 tencentcloud-sdk-python-live-3.0.938/tencentcloud/live/v20180801/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   154723 2023-07-19 00:42:04.000000 tencentcloud-sdk-python-live-3.0.938/tencentcloud/live/v20180801/live_client.py
+-rw-r--r--   0 root         (0) root         (0)   756652 2023-07-19 00:42:04.000000 tencentcloud-sdk-python-live-3.0.938/tencentcloud/live/v20180801/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:42:04.000000 tencentcloud-sdk-python-live-3.0.938/tencentcloud/live/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:42:04.000000 tencentcloud-sdk-python-live-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:42:05.000000 tencentcloud-sdk-python-live-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:05.000000 tencentcloud-sdk-python-live-3.0.938/tencentcloud_sdk_python_live.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:42:05.000000 tencentcloud-sdk-python-live-3.0.938/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:42:05.000000 tencentcloud-sdk-python-live-3.0.938/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:42:05.000000 tencentcloud-sdk-python-live-3.0.938/tencentcloud_sdk_python_live.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:42:05.000000 tencentcloud-sdk-python-live-3.0.938/tencentcloud_sdk_python_live.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:42:05.000000 tencentcloud-sdk-python-live-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:42:04.000000 tencentcloud-sdk-python-live-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-live-3.0.937/setup.py` & `tencentcloud-sdk-python-live-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.937/tencentcloud/live/v20180801/errorcodes.py` & `tencentcloud-sdk-python-live-3.0.938/tencentcloud/live/v20180801/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.937/tencentcloud/live/v20180801/live_client.py` & `tencentcloud-sdk-python-live-3.0.938/tencentcloud/live/v20180801/live_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             model = models.AddDelayLiveStreamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddLiveDomain(self, request):
         """添加域名，一次只能提交一个域名。域名必须已备案。
 
         :param request: Request instance for AddLiveDomain.
         :type request: :class:`tencentcloud.live.v20180801.models.AddLiveDomainRequest`
@@ -67,15 +67,15 @@
             model = models.AddLiveDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddLiveWatermark(self, request):
         """添加水印，成功返回水印 ID 后，需要调用[CreateLiveWatermarkRule](/document/product/267/32629)接口将水印 ID 绑定到流使用。 水印数量上限 100，超过后需要先删除，再添加。
 
         :param request: Request instance for AddLiveWatermark.
         :type request: :class:`tencentcloud.live.v20180801.models.AddLiveWatermarkRequest`
@@ -90,15 +90,15 @@
             model = models.AddLiveWatermarkResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AuthenticateDomainOwner(self, request):
         """验证用户是否拥有特定直播域名。
 
         :param request: Request instance for AuthenticateDomainOwner.
         :type request: :class:`tencentcloud.live.v20180801.models.AuthenticateDomainOwnerRequest`
@@ -113,15 +113,15 @@
             model = models.AuthenticateDomainOwnerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelCommonMixStream(self, request):
         """该接口用来取消混流。用法与 mix_streamv2.cancel_mix_stream 基本一致。
 
         :param request: Request instance for CancelCommonMixStream.
         :type request: :class:`tencentcloud.live.v20180801.models.CancelCommonMixStreamRequest`
@@ -136,15 +136,15 @@
             model = models.CancelCommonMixStreamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCommonMixStream(self, request):
         """该接口用来创建通用混流。用法与旧接口 mix_streamv2.start_mix_stream_advanced 基本一致。
         注意：当前最多支持16路混流。
         最佳实践：https://cloud.tencent.com/document/product/267/45566
 
@@ -161,15 +161,15 @@
             model = models.CreateCommonMixStreamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLiveCallbackRule(self, request):
         """创建回调规则，需要先调用[CreateLiveCallbackTemplate](/document/product/267/32637)接口创建回调模板，将返回的模板id绑定到域名/路径进行使用。
         <br>回调协议相关文档：[事件消息通知](/document/product/267/32744)。
 
         :param request: Request instance for CreateLiveCallbackRule.
@@ -185,15 +185,15 @@
             model = models.CreateLiveCallbackRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLiveCallbackTemplate(self, request):
         """创建回调模板，数量上限：50，成功返回模板id后，需要调用[CreateLiveCallbackRule](/document/product/267/32638)接口将模板 ID 绑定到域名/路径使用。
         <br>回调协议相关文档：[事件消息通知](/document/product/267/32744)。
         注意：至少填写一个回调 URL。
 
@@ -210,15 +210,15 @@
             model = models.CreateLiveCallbackTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLivePadRule(self, request):
         """创建直播垫片规则。
 
         :param request: Request instance for CreateLivePadRule.
         :type request: :class:`tencentcloud.live.v20180801.models.CreateLivePadRuleRequest`
@@ -233,15 +233,15 @@
             model = models.CreateLivePadRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLivePadTemplate(self, request):
         """创建直播垫片模板。
 
         :param request: Request instance for CreateLivePadTemplate.
         :type request: :class:`tencentcloud.live.v20180801.models.CreateLivePadTemplateRequest`
@@ -256,15 +256,15 @@
             model = models.CreateLivePadTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLivePullStreamTask(self, request):
         """创建直播拉流任务。支持将外部已有的点播文件，或者直播源拉取过来转推到指定的目标地址。
         注意：
         1. 默认支持任务数上限200个，如有特殊需求，可通过提单到售后进行评估增加上限。
         2. 源流视频编码目前只支持: H264, H265。其他编码格式建议先进行转码处理。
@@ -286,15 +286,15 @@
             model = models.CreateLivePullStreamTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLiveRecord(self, request):
         """- 使用前提
           1. 录制文件存放于点播平台，所以用户如需使用录制功能，需首先自行开通点播服务。
           2. 录制文件存放后相关费用（含存储以及下行播放流量）按照点播平台计费方式收取，具体请参考 [对应文档](https://cloud.tencent.com/document/product/266/2838)。
 
@@ -324,15 +324,15 @@
             model = models.CreateLiveRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLiveRecordRule(self, request):
         """创建录制规则，需要先调用[CreateLiveRecordTemplate](/document/product/267/32614)接口创建录制模板，将返回的模板id绑定到流使用。
         <br>录制相关文档：[直播录制](/document/product/267/32739)。
 
         :param request: Request instance for CreateLiveRecordRule.
@@ -348,15 +348,15 @@
             model = models.CreateLiveRecordRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLiveRecordTemplate(self, request):
         """创建录制模板，数量上限：50，成功返回模板id后，需要调用[CreateLiveRecordRule](/document/product/267/32615)接口，将模板id绑定到流进行使用。
         <br>录制相关文档：[直播录制](/document/product/267/32739)。
 
         :param request: Request instance for CreateLiveRecordTemplate.
@@ -372,15 +372,15 @@
             model = models.CreateLiveRecordTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLiveSnapshotRule(self, request):
         """创建截图规则，需要先调用[CreateLiveSnapshotTemplate](/document/product/267/32624)接口创建截图模板，然后将返回的模板 ID 绑定到流进行使用。
         <br>截图相关文档：[直播截图](/document/product/267/32737)。
         注意：单个域名仅支持关联一个截图模板。
 
@@ -397,15 +397,15 @@
             model = models.CreateLiveSnapshotRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLiveSnapshotTemplate(self, request):
         """创建截图模板，数量上限：50，成功返回模板id后，需要调用[CreateLiveSnapshotRule](/document/product/267/32625)接口，将模板id绑定到流使用。
         <br>截图相关文档：[直播截图](/document/product/267/32737)。
 
         :param request: Request instance for CreateLiveSnapshotTemplate.
@@ -421,15 +421,15 @@
             model = models.CreateLiveSnapshotTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLiveStreamMonitor(self, request):
         """该接口用来创建直播流监播任务。
 
         :param request: Request instance for CreateLiveStreamMonitor.
         :type request: :class:`tencentcloud.live.v20180801.models.CreateLiveStreamMonitorRequest`
@@ -444,15 +444,15 @@
             model = models.CreateLiveStreamMonitorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLiveTimeShiftRule(self, request):
         """创建直播时移规则，需要先调用[CreateLiveTimeShiftTemplate](/document/product/267/86169)接口创建直播时移模板，将返回的模板id绑定到流使用。
         <br>直播时移相关文档：[直播时移](/document/product/267/86134)。
 
         :param request: Request instance for CreateLiveTimeShiftRule.
@@ -468,15 +468,15 @@
             model = models.CreateLiveTimeShiftRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLiveTimeShiftTemplate(self, request):
         """创建直播时移模板。
 
         :param request: Request instance for CreateLiveTimeShiftTemplate.
         :type request: :class:`tencentcloud.live.v20180801.models.CreateLiveTimeShiftTemplateRequest`
@@ -491,15 +491,15 @@
             model = models.CreateLiveTimeShiftTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLiveTranscodeRule(self, request):
         """创建转码规则，数量上限：50，需要先调用[CreateLiveTranscodeTemplate](/document/product/267/32646)接口创建转码模板，将返回的模板id绑定到流使用。
         <br>转码相关文档：[直播转封装及转码](/document/product/267/32736)。
 
         :param request: Request instance for CreateLiveTranscodeRule.
@@ -515,15 +515,15 @@
             model = models.CreateLiveTranscodeRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLiveTranscodeTemplate(self, request):
         """创建转码模板，数量上限：50，成功返回模板id后，需要调用[CreateLiveTranscodeRule](/document/product/267/32647)接口，将返回的模板id绑定到流使用。
         <br>转码相关文档：[直播转封装及转码](/document/product/267/32736)。
 
         :param request: Request instance for CreateLiveTranscodeTemplate.
@@ -539,15 +539,15 @@
             model = models.CreateLiveTranscodeTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLiveWatermarkRule(self, request):
         """创建水印规则，需要先调用[AddLiveWatermark](/document/product/267/30154)接口添加水印，将返回的水印id绑定到流使用。
 
         :param request: Request instance for CreateLiveWatermarkRule.
         :type request: :class:`tencentcloud.live.v20180801.models.CreateLiveWatermarkRuleRequest`
@@ -562,15 +562,15 @@
             model = models.CreateLiveWatermarkRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePullStreamConfig(self, request):
         """创建临时拉流转推任务，目前限制添加10条任务。
         该接口已下线,请使用新接口 CreateLivePullStreamTask。
 
         注意：该接口用于创建临时拉流转推任务，
@@ -590,15 +590,15 @@
             model = models.CreatePullStreamConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRecordTask(self, request):
         """创建一个在指定时间启动、结束的录制任务，并使用指定录制模板ID对应的配置进行录制。
         - 使用前提
         1. 录制文件存放于点播平台，所以用户如需使用录制功能，需首先自行开通点播服务。
         2. 录制文件存放后相关费用（含存储以及下行播放流量）按照点播平台计费方式收取，具体请参考 [对应文档](https://cloud.tencent.com/document/product/266/2837)。
@@ -622,15 +622,15 @@
             model = models.CreateRecordTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateScreenshotTask(self, request):
         """创建一个在指定时间启动、结束的截图任务，并使用指定截图模板ID对应的配置进行截图。
         - 注意事项
         1. 断流会结束当前截图。在结束时间到达之前任务仍然有效，期间只要正常推流都会正常截图，与是否多次推、断流无关。
         2. 使用上避免创建时间段相互重叠的截图任务。若同一条流当前存在多个时段重叠的任务，为避免重复系统将启动最多3个截图任务。
@@ -651,15 +651,15 @@
             model = models.CreateScreenshotTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLiveCallbackRule(self, request):
         """删除回调规则。
 
         :param request: Request instance for DeleteLiveCallbackRule.
         :type request: :class:`tencentcloud.live.v20180801.models.DeleteLiveCallbackRuleRequest`
@@ -674,15 +674,15 @@
             model = models.DeleteLiveCallbackRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLiveCallbackTemplate(self, request):
         """删除回调模板。
 
         :param request: Request instance for DeleteLiveCallbackTemplate.
         :type request: :class:`tencentcloud.live.v20180801.models.DeleteLiveCallbackTemplateRequest`
@@ -697,15 +697,15 @@
             model = models.DeleteLiveCallbackTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLiveDomain(self, request):
         """删除已添加的直播域名
 
         :param request: Request instance for DeleteLiveDomain.
         :type request: :class:`tencentcloud.live.v20180801.models.DeleteLiveDomainRequest`
@@ -720,15 +720,15 @@
             model = models.DeleteLiveDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLivePadRule(self, request):
         """删除直播垫片规则。
 
         :param request: Request instance for DeleteLivePadRule.
         :type request: :class:`tencentcloud.live.v20180801.models.DeleteLivePadRuleRequest`
@@ -743,15 +743,15 @@
             model = models.DeleteLivePadRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLivePadTemplate(self, request):
         """删除直播垫片模板。
 
         :param request: Request instance for DeleteLivePadTemplate.
         :type request: :class:`tencentcloud.live.v20180801.models.DeleteLivePadTemplateRequest`
@@ -766,15 +766,15 @@
             model = models.DeleteLivePadTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLivePullStreamTask(self, request):
         """删除接口 CreateLivePullStreamTask 创建的拉流任务。
         注意：
         1. 入参中的 TaskId 为 CreateLivePullStreamTask 接口创建时返回的TaskId。
         2. 也可通过 DescribeLivePullStreamTasks 进行查询创建的任务。
@@ -792,15 +792,15 @@
             model = models.DeleteLivePullStreamTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLiveRecord(self, request):
         """注：DeleteLiveRecord 接口仅用于删除录制任务记录，不具备停止录制的功能，也不能删除正在进行中的录制。如果需要停止录制任务，请使用终止录制[StopLiveRecord](/document/product/267/30146) 接口。
 
         :param request: Request instance for DeleteLiveRecord.
         :type request: :class:`tencentcloud.live.v20180801.models.DeleteLiveRecordRequest`
@@ -815,15 +815,15 @@
             model = models.DeleteLiveRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLiveRecordRule(self, request):
         """删除录制规则。
 
         :param request: Request instance for DeleteLiveRecordRule.
         :type request: :class:`tencentcloud.live.v20180801.models.DeleteLiveRecordRuleRequest`
@@ -838,15 +838,15 @@
             model = models.DeleteLiveRecordRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLiveRecordTemplate(self, request):
         """删除录制模板。
 
         :param request: Request instance for DeleteLiveRecordTemplate.
         :type request: :class:`tencentcloud.live.v20180801.models.DeleteLiveRecordTemplateRequest`
@@ -861,15 +861,15 @@
             model = models.DeleteLiveRecordTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLiveSnapshotRule(self, request):
         """删除截图规则。
 
         :param request: Request instance for DeleteLiveSnapshotRule.
         :type request: :class:`tencentcloud.live.v20180801.models.DeleteLiveSnapshotRuleRequest`
@@ -884,15 +884,15 @@
             model = models.DeleteLiveSnapshotRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLiveSnapshotTemplate(self, request):
         """删除截图模板
 
         :param request: Request instance for DeleteLiveSnapshotTemplate.
         :type request: :class:`tencentcloud.live.v20180801.models.DeleteLiveSnapshotTemplateRequest`
@@ -907,15 +907,15 @@
             model = models.DeleteLiveSnapshotTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLiveStreamMonitor(self, request):
         """该接口用来删除直播流监播任务。
 
         :param request: Request instance for DeleteLiveStreamMonitor.
         :type request: :class:`tencentcloud.live.v20180801.models.DeleteLiveStreamMonitorRequest`
@@ -930,15 +930,15 @@
             model = models.DeleteLiveStreamMonitorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLiveTimeShiftRule(self, request):
         """删除直播时移规则。
 
         :param request: Request instance for DeleteLiveTimeShiftRule.
         :type request: :class:`tencentcloud.live.v20180801.models.DeleteLiveTimeShiftRuleRequest`
@@ -953,15 +953,15 @@
             model = models.DeleteLiveTimeShiftRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLiveTimeShiftTemplate(self, request):
         """删除直播时移模板。
 
         :param request: Request instance for DeleteLiveTimeShiftTemplate.
         :type request: :class:`tencentcloud.live.v20180801.models.DeleteLiveTimeShiftTemplateRequest`
@@ -976,15 +976,15 @@
             model = models.DeleteLiveTimeShiftTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLiveTranscodeRule(self, request):
         """删除转码规则。
         DomainName+AppName+StreamName+TemplateId唯一标识单个转码规则，如需删除需要强匹配。其中TemplateId必填，其余参数为空时也需要传空字符串进行强匹配。
 
         :param request: Request instance for DeleteLiveTranscodeRule.
@@ -1000,15 +1000,15 @@
             model = models.DeleteLiveTranscodeRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLiveTranscodeTemplate(self, request):
         """删除转码模板。
 
         :param request: Request instance for DeleteLiveTranscodeTemplate.
         :type request: :class:`tencentcloud.live.v20180801.models.DeleteLiveTranscodeTemplateRequest`
@@ -1023,15 +1023,15 @@
             model = models.DeleteLiveTranscodeTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLiveWatermark(self, request):
         """删除水印。
 
         :param request: Request instance for DeleteLiveWatermark.
         :type request: :class:`tencentcloud.live.v20180801.models.DeleteLiveWatermarkRequest`
@@ -1046,15 +1046,15 @@
             model = models.DeleteLiveWatermarkResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLiveWatermarkRule(self, request):
         """删除水印规则
 
         :param request: Request instance for DeleteLiveWatermarkRule.
         :type request: :class:`tencentcloud.live.v20180801.models.DeleteLiveWatermarkRuleRequest`
@@ -1069,15 +1069,15 @@
             model = models.DeleteLiveWatermarkRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePullStreamConfig(self, request):
         """删除直播拉流配置。该接口已下线,请使用新接口 DeleteLivePullStreamTask。
 
         :param request: Request instance for DeletePullStreamConfig.
         :type request: :class:`tencentcloud.live.v20180801.models.DeletePullStreamConfigRequest`
@@ -1092,15 +1092,15 @@
             model = models.DeletePullStreamConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRecordTask(self, request):
         """删除录制任务配置。删除操作不影响正在运行当中的任务，仅对删除之后新的推流有效。
 
         :param request: Request instance for DeleteRecordTask.
         :type request: :class:`tencentcloud.live.v20180801.models.DeleteRecordTaskRequest`
@@ -1115,15 +1115,15 @@
             model = models.DeleteRecordTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteScreenshotTask(self, request):
         """删除截图任务配置。删除操作不影响正在运行当中的任务，仅对删除之后新的推流有效。
 
         :param request: Request instance for DeleteScreenshotTask.
         :type request: :class:`tencentcloud.live.v20180801.models.DeleteScreenshotTaskRequest`
@@ -1138,15 +1138,15 @@
             model = models.DeleteScreenshotTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAllStreamPlayInfoList(self, request):
         """输入某个时间点（1分钟维度），查询该时间点所有流的下行信息。
 
         :param request: Request instance for DescribeAllStreamPlayInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeAllStreamPlayInfoListRequest`
@@ -1161,15 +1161,15 @@
             model = models.DescribeAllStreamPlayInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAreaBillBandwidthAndFluxList(self, request):
         """海外分区直播播放带宽和流量数据查询。
 
         :param request: Request instance for DescribeAreaBillBandwidthAndFluxList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeAreaBillBandwidthAndFluxListRequest`
@@ -1184,15 +1184,15 @@
             model = models.DescribeAreaBillBandwidthAndFluxListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBillBandwidthAndFluxList(self, request):
         """直播播放带宽和流量数据查询。
 
         :param request: Request instance for DescribeBillBandwidthAndFluxList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeBillBandwidthAndFluxListRequest`
@@ -1207,15 +1207,15 @@
             model = models.DescribeBillBandwidthAndFluxListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCallbackRecordsList(self, request):
         """用于查询回调事件。
 
         :param request: Request instance for DescribeCallbackRecordsList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeCallbackRecordsListRequest`
@@ -1230,15 +1230,15 @@
             model = models.DescribeCallbackRecordsListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConcurrentRecordStreamNum(self, request):
         """查询并发录制路数，对慢直播和普通直播适用。
 
         :param request: Request instance for DescribeConcurrentRecordStreamNum.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeConcurrentRecordStreamNumRequest`
@@ -1253,15 +1253,15 @@
             model = models.DescribeConcurrentRecordStreamNumResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeliverBandwidthList(self, request):
         """查询直播转推计费带宽，查询时间范围最大支持3个月内的数据，时间跨度最长31天。
 
         :param request: Request instance for DescribeDeliverBandwidthList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeDeliverBandwidthListRequest`
@@ -1276,15 +1276,15 @@
             model = models.DescribeDeliverBandwidthListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGroupProIspPlayInfoList(self, request):
         """查询按省份和运营商分组的下行播放数据。
 
         :param request: Request instance for DescribeGroupProIspPlayInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeGroupProIspPlayInfoListRequest`
@@ -1299,15 +1299,15 @@
             model = models.DescribeGroupProIspPlayInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHttpStatusInfoList(self, request):
         """查询某段时间内5分钟粒度的各播放http状态码的个数。
         备注：数据延迟1小时，如10:00-10:59点的数据12点才能查到。
 
         :param request: Request instance for DescribeHttpStatusInfoList.
@@ -1323,15 +1323,15 @@
             model = models.DescribeHttpStatusInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveCallbackRules(self, request):
         """获取回调规则列表
 
         :param request: Request instance for DescribeLiveCallbackRules.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveCallbackRulesRequest`
@@ -1346,15 +1346,15 @@
             model = models.DescribeLiveCallbackRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveCallbackTemplate(self, request):
         """获取单个回调模板。
 
         :param request: Request instance for DescribeLiveCallbackTemplate.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveCallbackTemplateRequest`
@@ -1369,15 +1369,15 @@
             model = models.DescribeLiveCallbackTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveCallbackTemplates(self, request):
         """获取回调模板列表
 
         :param request: Request instance for DescribeLiveCallbackTemplates.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveCallbackTemplatesRequest`
@@ -1392,15 +1392,15 @@
             model = models.DescribeLiveCallbackTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveCert(self, request):
         """获取证书信息
 
         :param request: Request instance for DescribeLiveCert.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveCertRequest`
@@ -1415,15 +1415,15 @@
             model = models.DescribeLiveCertResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveCerts(self, request):
         """获取证书信息列表
 
         :param request: Request instance for DescribeLiveCerts.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveCertsRequest`
@@ -1438,15 +1438,15 @@
             model = models.DescribeLiveCertsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveDelayInfoList(self, request):
         """获取直播延播列表。
 
         :param request: Request instance for DescribeLiveDelayInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveDelayInfoListRequest`
@@ -1461,15 +1461,15 @@
             model = models.DescribeLiveDelayInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveDomain(self, request):
         """查询直播域名信息。
 
         :param request: Request instance for DescribeLiveDomain.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveDomainRequest`
@@ -1484,15 +1484,15 @@
             model = models.DescribeLiveDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveDomainCert(self, request):
         """获取域名证书信息。
 
         :param request: Request instance for DescribeLiveDomainCert.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveDomainCertRequest`
@@ -1507,15 +1507,15 @@
             model = models.DescribeLiveDomainCertResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveDomainCertBindings(self, request):
         """查询绑定证书的域名列表。
 
         :param request: Request instance for DescribeLiveDomainCertBindings.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveDomainCertBindingsRequest`
@@ -1530,15 +1530,15 @@
             model = models.DescribeLiveDomainCertBindingsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveDomainPlayInfoList(self, request):
         """查询实时的域名维度下行播放数据，由于数据处理有耗时，接口默认查询4分钟前的准实时数据。
 
         :param request: Request instance for DescribeLiveDomainPlayInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveDomainPlayInfoListRequest`
@@ -1553,15 +1553,15 @@
             model = models.DescribeLiveDomainPlayInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveDomainReferer(self, request):
         """查询直播域名 Referer 黑白名单配置。
         由于 Referer 信息包含在 http 协议中，在开启配置后，播放协议为 rtmp 或 WebRTC 不会校验 Referer 配置，仍可正常播放。如需配置 Referer 鉴权建议使用 http-flv 或 http-hls 协议播放。
 
         :param request: Request instance for DescribeLiveDomainReferer.
@@ -1577,15 +1577,15 @@
             model = models.DescribeLiveDomainRefererResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveDomains(self, request):
         """根据域名状态、类型等信息查询用户的域名信息。
 
         :param request: Request instance for DescribeLiveDomains.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveDomainsRequest`
@@ -1600,15 +1600,15 @@
             model = models.DescribeLiveDomainsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveForbidStreamList(self, request):
         """获取禁推流列表。
 
         注意：该接口仅作为直播辅助查询接口，重要业务场景不可强依赖该接口。
 
@@ -1625,15 +1625,15 @@
             model = models.DescribeLiveForbidStreamListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLivePackageInfo(self, request):
         """查询用户套餐包总量、使用量、剩余量、包状态、购买时间和过期时间等。
 
         :param request: Request instance for DescribeLivePackageInfo.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLivePackageInfoRequest`
@@ -1648,15 +1648,15 @@
             model = models.DescribeLivePackageInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLivePadRules(self, request):
         """获取直播垫片规则列表。
 
         :param request: Request instance for DescribeLivePadRules.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLivePadRulesRequest`
@@ -1671,15 +1671,15 @@
             model = models.DescribeLivePadRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLivePadTemplate(self, request):
         """获取单个直播垫片模板
 
         :param request: Request instance for DescribeLivePadTemplate.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLivePadTemplateRequest`
@@ -1694,15 +1694,15 @@
             model = models.DescribeLivePadTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLivePadTemplates(self, request):
         """获取直播垫片模板。
 
         :param request: Request instance for DescribeLivePadTemplates.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLivePadTemplatesRequest`
@@ -1717,15 +1717,15 @@
             model = models.DescribeLivePadTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLivePlayAuthKey(self, request):
         """查询播放鉴权key。
 
         :param request: Request instance for DescribeLivePlayAuthKey.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLivePlayAuthKeyRequest`
@@ -1740,15 +1740,15 @@
             model = models.DescribeLivePlayAuthKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLivePullStreamTaskStatus(self, request):
         """查询直播拉流任务状态信息。
 
         :param request: Request instance for DescribeLivePullStreamTaskStatus.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLivePullStreamTaskStatusRequest`
@@ -1763,15 +1763,15 @@
             model = models.DescribeLivePullStreamTaskStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLivePullStreamTasks(self, request):
         """查询使用 CreateLivePullStreamTask 接口创建的直播拉流任务。
         排序方式：默认按更新时间 倒序排列。
 
         :param request: Request instance for DescribeLivePullStreamTasks.
@@ -1787,15 +1787,15 @@
             model = models.DescribeLivePullStreamTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLivePushAuthKey(self, request):
         """查询直播推流鉴权key
 
         :param request: Request instance for DescribeLivePushAuthKey.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLivePushAuthKeyRequest`
@@ -1810,15 +1810,15 @@
             model = models.DescribeLivePushAuthKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveRecordRules(self, request):
         """获取录制规则列表
 
         :param request: Request instance for DescribeLiveRecordRules.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveRecordRulesRequest`
@@ -1833,15 +1833,15 @@
             model = models.DescribeLiveRecordRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveRecordTemplate(self, request):
         """获取单个录制模板。
 
         :param request: Request instance for DescribeLiveRecordTemplate.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveRecordTemplateRequest`
@@ -1856,15 +1856,15 @@
             model = models.DescribeLiveRecordTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveRecordTemplates(self, request):
         """获取录制模板列表。
 
         :param request: Request instance for DescribeLiveRecordTemplates.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveRecordTemplatesRequest`
@@ -1879,15 +1879,15 @@
             model = models.DescribeLiveRecordTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveSnapshotRules(self, request):
         """获取截图规则列表
 
         :param request: Request instance for DescribeLiveSnapshotRules.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveSnapshotRulesRequest`
@@ -1902,15 +1902,15 @@
             model = models.DescribeLiveSnapshotRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveSnapshotTemplate(self, request):
         """获取单个截图模板。
 
         :param request: Request instance for DescribeLiveSnapshotTemplate.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveSnapshotTemplateRequest`
@@ -1925,15 +1925,15 @@
             model = models.DescribeLiveSnapshotTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveSnapshotTemplates(self, request):
         """获取截图模板列表。
 
         :param request: Request instance for DescribeLiveSnapshotTemplates.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveSnapshotTemplatesRequest`
@@ -1948,15 +1948,15 @@
             model = models.DescribeLiveSnapshotTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveStreamEventList(self, request):
         """用于查询推断流事件。<br>
 
         注意：
         1. 该接口提供离线推断流记录查询功能，不可作为重要业务场景强依赖接口。
@@ -1975,15 +1975,15 @@
             model = models.DescribeLiveStreamEventListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveStreamMonitor(self, request):
         """该接口用来查询某个特定监播任务的配置。
 
         :param request: Request instance for DescribeLiveStreamMonitor.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveStreamMonitorRequest`
@@ -1998,15 +1998,15 @@
             model = models.DescribeLiveStreamMonitorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveStreamMonitorList(self, request):
         """该接口用来查询直播流监播任务配置的列表信息。
 
         :param request: Request instance for DescribeLiveStreamMonitorList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveStreamMonitorListRequest`
@@ -2021,15 +2021,15 @@
             model = models.DescribeLiveStreamMonitorListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveStreamOnlineList(self, request):
         """返回正在直播中的流列表。适用于推流成功后查询在线流信息。
 
         注意：
         1. 该接口仅提供辅助查询在线流列表功能，业务重要场景不可强依赖该接口。
@@ -2048,15 +2048,15 @@
             model = models.DescribeLiveStreamOnlineListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveStreamPublishedList(self, request):
         """返回已经推过流的流列表。<br>
         注意：分页最多支持查询1万条记录，可通过调整查询时间范围来获取更多数据。
 
         :param request: Request instance for DescribeLiveStreamPublishedList.
@@ -2072,15 +2072,15 @@
             model = models.DescribeLiveStreamPublishedListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveStreamPushInfoList(self, request):
         """查询所有实时流的推流信息，包括客户端IP，服务端IP，帧率，码率，域名，开始推流时间。
 
         :param request: Request instance for DescribeLiveStreamPushInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveStreamPushInfoListRequest`
@@ -2095,15 +2095,15 @@
             model = models.DescribeLiveStreamPushInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveStreamState(self, request):
         """返回直播中、无推流或者禁播等状态。
 
         使用建议：
         该接口提供实时流状态查询功能，鉴于网络抖动等一些不可抗因素，使用该接口作为判断主播是否开播等重要业务场景时，请参考以下使用建议。
@@ -2127,15 +2127,15 @@
             model = models.DescribeLiveStreamStateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveTimeShiftBillInfoList(self, request):
         """提供给客户对账，按天统计，维度：推流域名、时移文件时长（累加）、配置天数（不累加）、时移总时长（累加）。
 
         :param request: Request instance for DescribeLiveTimeShiftBillInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveTimeShiftBillInfoListRequest`
@@ -2150,15 +2150,15 @@
             model = models.DescribeLiveTimeShiftBillInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveTimeShiftRules(self, request):
         """获取直播时移规则列表。
 
         :param request: Request instance for DescribeLiveTimeShiftRules.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveTimeShiftRulesRequest`
@@ -2173,15 +2173,15 @@
             model = models.DescribeLiveTimeShiftRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveTimeShiftTemplates(self, request):
         """获取直播时移模板。
 
         :param request: Request instance for DescribeLiveTimeShiftTemplates.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveTimeShiftTemplatesRequest`
@@ -2196,15 +2196,15 @@
             model = models.DescribeLiveTimeShiftTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveTranscodeDetailInfo(self, request):
         """支持查询某天或某段时间的转码详细信息。由于转码数据量较大，如果查询时间跨度太长可能会拉不到数据，可以尝试将查询时间范围缩小些再重试。
 
         :param request: Request instance for DescribeLiveTranscodeDetailInfo.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveTranscodeDetailInfoRequest`
@@ -2219,15 +2219,15 @@
             model = models.DescribeLiveTranscodeDetailInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveTranscodeRules(self, request):
         """获取转码规则列表
 
         :param request: Request instance for DescribeLiveTranscodeRules.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveTranscodeRulesRequest`
@@ -2242,15 +2242,15 @@
             model = models.DescribeLiveTranscodeRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveTranscodeTemplate(self, request):
         """获取单个转码模板。
 
         :param request: Request instance for DescribeLiveTranscodeTemplate.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveTranscodeTemplateRequest`
@@ -2265,15 +2265,15 @@
             model = models.DescribeLiveTranscodeTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveTranscodeTemplates(self, request):
         """获取转码模板列表。
 
         :param request: Request instance for DescribeLiveTranscodeTemplates.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveTranscodeTemplatesRequest`
@@ -2288,15 +2288,15 @@
             model = models.DescribeLiveTranscodeTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveTranscodeTotalInfo(self, request):
         """查询转码总量数据，可查询近三个月内的数据。
         注意：
         如果是查询某一天内，则返回5分钟粒度数据；
         如果是查询跨天或指定域名， 则返回1小时粒度数据。
@@ -2314,15 +2314,15 @@
             model = models.DescribeLiveTranscodeTotalInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveWatermark(self, request):
         """获取单个水印信息。
 
         :param request: Request instance for DescribeLiveWatermark.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveWatermarkRequest`
@@ -2337,15 +2337,15 @@
             model = models.DescribeLiveWatermarkResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveWatermarkRules(self, request):
         """获取水印规则列表。
 
         :param request: Request instance for DescribeLiveWatermarkRules.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveWatermarkRulesRequest`
@@ -2360,15 +2360,15 @@
             model = models.DescribeLiveWatermarkRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveWatermarks(self, request):
         """查询水印列表。
 
         :param request: Request instance for DescribeLiveWatermarks.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveWatermarksRequest`
@@ -2383,15 +2383,15 @@
             model = models.DescribeLiveWatermarksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveXP2PDetailInfoList(self, request):
         """P2P流数据查询接口，用来获取流量、卡播和起播信息。
 
         :param request: Request instance for DescribeLiveXP2PDetailInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveXP2PDetailInfoListRequest`
@@ -2406,15 +2406,15 @@
             model = models.DescribeLiveXP2PDetailInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLogDownloadList(self, request):
         """批量获取日志URL。
 
         :param request: Request instance for DescribeLogDownloadList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLogDownloadListRequest`
@@ -2429,15 +2429,15 @@
             model = models.DescribeLogDownloadListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMonitorReport(self, request):
         """用来查询监播场次7天内的智能识别、断流、低帧率等信息的汇总报告。
 
         :param request: Request instance for DescribeMonitorReport.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeMonitorReportRequest`
@@ -2452,15 +2452,15 @@
             model = models.DescribeMonitorReportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePlayErrorCodeDetailInfoList(self, request):
         """查询下行播放错误码信息，某段时间内1分钟粒度的各http错误码出现的次数，包括4xx，5xx。
 
 
         :param request: Request instance for DescribePlayErrorCodeDetailInfoList.
@@ -2476,15 +2476,15 @@
             model = models.DescribePlayErrorCodeDetailInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePlayErrorCodeSumInfoList(self, request):
         """查询下行播放错误码信息。
 
         :param request: Request instance for DescribePlayErrorCodeSumInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribePlayErrorCodeSumInfoListRequest`
@@ -2499,15 +2499,15 @@
             model = models.DescribePlayErrorCodeSumInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProIspPlaySumInfoList(self, request):
         """查询某段时间内每个国家地区每个省份每个运营商的平均每秒流量，总流量，总请求数信息。
 
         :param request: Request instance for DescribeProIspPlaySumInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeProIspPlaySumInfoListRequest`
@@ -2522,15 +2522,15 @@
             model = models.DescribeProIspPlaySumInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProvinceIspPlayInfoList(self, request):
         """查询某省份某运营商下行播放数据，包括带宽，流量，请求数，并发连接数信息。
 
         :param request: Request instance for DescribeProvinceIspPlayInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeProvinceIspPlayInfoListRequest`
@@ -2545,15 +2545,15 @@
             model = models.DescribeProvinceIspPlayInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePullStreamConfigs(self, request):
         """查询直播拉流配置。该接口已下线,请使用新接口 DescribeLivePullStreamTasks。
 
         :param request: Request instance for DescribePullStreamConfigs.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribePullStreamConfigsRequest`
@@ -2568,15 +2568,15 @@
             model = models.DescribePullStreamConfigsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePushBandwidthAndFluxList(self, request):
         """直播推流带宽和流量数据查询。
         推流计费会先取全球推流用量和全球播放用量进行比较，满足计费条件后再按各地区用量出账。详情参见[计费文档](https://cloud.tencent.com/document/product/267/34175)。
 
         :param request: Request instance for DescribePushBandwidthAndFluxList.
@@ -2592,15 +2592,15 @@
             model = models.DescribePushBandwidthAndFluxListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRecordTask(self, request):
         """查询指定时间段范围内启动和结束的录制任务列表。
         - 使用前提
         1. 仅用于查询由 CreateRecordTask 接口创建的录制任务。
         2. 不能查询被 DeleteRecordTask 接口删除以及已过期（平台侧保留3个月）的录制任务。
@@ -2618,15 +2618,15 @@
             model = models.DescribeRecordTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeScreenShotSheetNumList(self, request):
         """接口用来查询直播增值业务--截图的张数
 
         :param request: Request instance for DescribeScreenShotSheetNumList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeScreenShotSheetNumListRequest`
@@ -2641,15 +2641,15 @@
             model = models.DescribeScreenShotSheetNumListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeScreenshotTask(self, request):
         """查询指定时间段范围内启动和结束的截图任务列表。
         - 使用前提
         1. 仅用于查询由 CreateScreenshotTask接口创建的截图任务。
         2. 不能查询被 DeleteScreenshotTask接口删除以及已过期（平台侧保留3个月）的截图任务。
@@ -2667,15 +2667,15 @@
             model = models.DescribeScreenshotTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStreamDayPlayInfoList(self, request):
         """查询天维度每条流的播放数据，包括总流量等。
 
         :param request: Request instance for DescribeStreamDayPlayInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeStreamDayPlayInfoListRequest`
@@ -2690,15 +2690,15 @@
             model = models.DescribeStreamDayPlayInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStreamPlayInfoList(self, request):
         """查询播放数据，支持按流名称查询详细播放数据，也可按播放域名查询详细总数据，数据延迟4分钟左右。
 
         :param request: Request instance for DescribeStreamPlayInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeStreamPlayInfoListRequest`
@@ -2713,15 +2713,15 @@
             model = models.DescribeStreamPlayInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStreamPushInfoList(self, request):
         """查询流id的上行推流质量数据，包括音视频的帧率，码率，流逝时间，编码格式等。
 
         :param request: Request instance for DescribeStreamPushInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeStreamPushInfoListRequest`
@@ -2736,15 +2736,15 @@
             model = models.DescribeStreamPushInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTimeShiftRecordDetail(self, request):
         """前提调用 DescribeTimeShiftStreamList 获得请求必要参数。查询指定范围内的时移流录制详情，最大支持24小时范围查询。
 
         :param request: Request instance for DescribeTimeShiftRecordDetail.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeTimeShiftRecordDetailRequest`
@@ -2759,15 +2759,15 @@
             model = models.DescribeTimeShiftRecordDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTimeShiftStreamList(self, request):
         """查询某个时间范围内所有时移流列表。最大支持查询24小时内的数据。
 
         :param request: Request instance for DescribeTimeShiftStreamList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeTimeShiftStreamListRequest`
@@ -2782,15 +2782,15 @@
             model = models.DescribeTimeShiftStreamListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopClientIpSumInfoList(self, request):
         """查询某段时间top n客户端ip汇总信息（暂支持top 1000）
 
         :param request: Request instance for DescribeTopClientIpSumInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeTopClientIpSumInfoListRequest`
@@ -2805,15 +2805,15 @@
             model = models.DescribeTopClientIpSumInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTranscodeTaskNum(self, request):
         """查询转码任务数。
 
         :param request: Request instance for DescribeTranscodeTaskNum.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeTranscodeTaskNumRequest`
@@ -2828,15 +2828,15 @@
             model = models.DescribeTranscodeTaskNumResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUploadStreamNums(self, request):
         """直播上行路数查询。
 
         :param request: Request instance for DescribeUploadStreamNums.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeUploadStreamNumsRequest`
@@ -2851,15 +2851,15 @@
             model = models.DescribeUploadStreamNumsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVisitTopSumInfoList(self, request):
         """查询某时间段top n的域名或流id信息（暂支持top 1000）。
 
         :param request: Request instance for DescribeVisitTopSumInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeVisitTopSumInfoListRequest`
@@ -2874,15 +2874,15 @@
             model = models.DescribeVisitTopSumInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DropLiveStream(self, request):
         """断开推流连接，但可以重新推流。
         注：对已经不活跃的流，调用该断流接口时，接口返回成功。
 
         :param request: Request instance for DropLiveStream.
@@ -2898,15 +2898,15 @@
             model = models.DropLiveStreamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableLiveDomain(self, request):
         """启用状态为停用的直播域名。
 
         :param request: Request instance for EnableLiveDomain.
         :type request: :class:`tencentcloud.live.v20180801.models.EnableLiveDomainRequest`
@@ -2921,15 +2921,15 @@
             model = models.EnableLiveDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ForbidLiveDomain(self, request):
         """停止使用某个直播域名。
 
         :param request: Request instance for ForbidLiveDomain.
         :type request: :class:`tencentcloud.live.v20180801.models.ForbidLiveDomainRequest`
@@ -2944,15 +2944,15 @@
             model = models.ForbidLiveDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ForbidLiveStream(self, request):
         """禁止某条流的推送，可以预设某个时刻将流恢复。
         注意：
         1. 默认只要流名称正确，禁推就会生效。
         2. 如需要推流域名+推流路径+流名称 强匹配生效禁推，需提单联系售后开启配置。
@@ -2971,15 +2971,15 @@
             model = models.ForbidLiveStreamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLiveCallbackTemplate(self, request):
         """修改回调模板。
 
         :param request: Request instance for ModifyLiveCallbackTemplate.
         :type request: :class:`tencentcloud.live.v20180801.models.ModifyLiveCallbackTemplateRequest`
@@ -2994,15 +2994,15 @@
             model = models.ModifyLiveCallbackTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLiveDomainCertBindings(self, request):
         """批量绑定证书对应的播放域名，并更新启用状态。
         新建自有证书将自动上传至腾讯云ssl。
 
         :param request: Request instance for ModifyLiveDomainCertBindings.
@@ -3018,15 +3018,15 @@
             model = models.ModifyLiveDomainCertBindingsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLiveDomainReferer(self, request):
         """设置直播域名 Referer 黑白名单。
         由于 Referer 信息包含在 http 协议中，在开启配置后，播放协议为 rtmp 或 WebRTC 不会校验 Referer 配置，仍可正常播放。如需配置 Referer 鉴权建议使用 http-flv 或 http-hls 协议播放。
 
         :param request: Request instance for ModifyLiveDomainReferer.
@@ -3042,15 +3042,15 @@
             model = models.ModifyLiveDomainRefererResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLivePadTemplate(self, request):
         """修改直播垫片模板。
 
         :param request: Request instance for ModifyLivePadTemplate.
         :type request: :class:`tencentcloud.live.v20180801.models.ModifyLivePadTemplateRequest`
@@ -3065,15 +3065,15 @@
             model = models.ModifyLivePadTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLivePlayAuthKey(self, request):
         """修改播放鉴权key
 
         :param request: Request instance for ModifyLivePlayAuthKey.
         :type request: :class:`tencentcloud.live.v20180801.models.ModifyLivePlayAuthKeyRequest`
@@ -3088,15 +3088,15 @@
             model = models.ModifyLivePlayAuthKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLivePlayDomain(self, request):
         """修改播放域名信息。
 
         :param request: Request instance for ModifyLivePlayDomain.
         :type request: :class:`tencentcloud.live.v20180801.models.ModifyLivePlayDomainRequest`
@@ -3111,15 +3111,15 @@
             model = models.ModifyLivePlayDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLivePullStreamTask(self, request):
         """更新直播拉流任务。
         1. 不支持修改目标地址，如需推到新地址，请创建新任务。
         2. 不支持修改拉流源类型，如需更换，请创建新任务。
 
@@ -3136,15 +3136,15 @@
             model = models.ModifyLivePullStreamTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLivePushAuthKey(self, request):
         """修改直播推流鉴权key
 
         :param request: Request instance for ModifyLivePushAuthKey.
         :type request: :class:`tencentcloud.live.v20180801.models.ModifyLivePushAuthKeyRequest`
@@ -3159,15 +3159,15 @@
             model = models.ModifyLivePushAuthKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLiveRecordTemplate(self, request):
         """修改录制模板配置。
 
         :param request: Request instance for ModifyLiveRecordTemplate.
         :type request: :class:`tencentcloud.live.v20180801.models.ModifyLiveRecordTemplateRequest`
@@ -3182,15 +3182,15 @@
             model = models.ModifyLiveRecordTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLiveSnapshotTemplate(self, request):
         """修改截图模板配置。
 
         :param request: Request instance for ModifyLiveSnapshotTemplate.
         :type request: :class:`tencentcloud.live.v20180801.models.ModifyLiveSnapshotTemplateRequest`
@@ -3205,15 +3205,15 @@
             model = models.ModifyLiveSnapshotTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLiveStreamMonitor(self, request):
         """该接口用来修改直播流监播任务的配置。
 
         :param request: Request instance for ModifyLiveStreamMonitor.
         :type request: :class:`tencentcloud.live.v20180801.models.ModifyLiveStreamMonitorRequest`
@@ -3228,15 +3228,15 @@
             model = models.ModifyLiveStreamMonitorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLiveTimeShiftTemplate(self, request):
         """修改直播时移模板。
 
         :param request: Request instance for ModifyLiveTimeShiftTemplate.
         :type request: :class:`tencentcloud.live.v20180801.models.ModifyLiveTimeShiftTemplateRequest`
@@ -3251,15 +3251,15 @@
             model = models.ModifyLiveTimeShiftTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLiveTranscodeTemplate(self, request):
         """修改转码模板配置。
 
         :param request: Request instance for ModifyLiveTranscodeTemplate.
         :type request: :class:`tencentcloud.live.v20180801.models.ModifyLiveTranscodeTemplateRequest`
@@ -3274,15 +3274,15 @@
             model = models.ModifyLiveTranscodeTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPullStreamConfig(self, request):
         """更新拉流配置。该接口为已下线接口，请使用新接口 ModifyLivePullStreamTask。
 
         :param request: Request instance for ModifyPullStreamConfig.
         :type request: :class:`tencentcloud.live.v20180801.models.ModifyPullStreamConfigRequest`
@@ -3297,15 +3297,15 @@
             model = models.ModifyPullStreamConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPullStreamStatus(self, request):
         """修改直播拉流配置的状态。该接口已下线,请使用新接口 ModifyLivePullStreamTask。
 
         :param request: Request instance for ModifyPullStreamStatus.
         :type request: :class:`tencentcloud.live.v20180801.models.ModifyPullStreamStatusRequest`
@@ -3320,15 +3320,15 @@
             model = models.ModifyPullStreamStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RestartLivePullStreamTask(self, request):
         """将正在运行的拉流转推任务进行重启。
         注意：
         1. 重启任务会造成推流中断。
         2. 点播源任务的重启，会根据VodRefreshType决定是续播还是从头开始播。
@@ -3346,15 +3346,15 @@
             model = models.RestartLivePullStreamTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResumeDelayLiveStream(self, request):
         """取消直播流设置的延时配置，恢复实时直播画面。
 
         :param request: Request instance for ResumeDelayLiveStream.
         :type request: :class:`tencentcloud.live.v20180801.models.ResumeDelayLiveStreamRequest`
@@ -3369,15 +3369,15 @@
             model = models.ResumeDelayLiveStreamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResumeLiveStream(self, request):
         """恢复某条流的推流。
 
         :param request: Request instance for ResumeLiveStream.
         :type request: :class:`tencentcloud.live.v20180801.models.ResumeLiveStreamRequest`
@@ -3392,15 +3392,15 @@
             model = models.ResumeLiveStreamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartLiveStreamMonitor(self, request):
         """该接口用来启动直播流监播任务。
 
         :param request: Request instance for StartLiveStreamMonitor.
         :type request: :class:`tencentcloud.live.v20180801.models.StartLiveStreamMonitorRequest`
@@ -3415,15 +3415,15 @@
             model = models.StartLiveStreamMonitorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopLiveRecord(self, request):
         """说明：录制后的文件存放于点播平台。用户如需使用录制功能，需首先自行开通点播账号并确保账号可用。录制文件存放后，相关费用（含存储以及下行播放流量）按照点播平台计费方式收取，请参考对应文档。
 
         :param request: Request instance for StopLiveRecord.
         :type request: :class:`tencentcloud.live.v20180801.models.StopLiveRecordRequest`
@@ -3438,15 +3438,15 @@
             model = models.StopLiveRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopLiveStreamMonitor(self, request):
         """该接口用来停止直播流监播任务。
 
         :param request: Request instance for StopLiveStreamMonitor.
         :type request: :class:`tencentcloud.live.v20180801.models.StopLiveStreamMonitorRequest`
@@ -3461,15 +3461,15 @@
             model = models.StopLiveStreamMonitorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopRecordTask(self, request):
         """提前结束录制，中止运行中的录制任务并生成录制文件。任务被成功终止后，本次任务将不再启动。
 
         :param request: Request instance for StopRecordTask.
         :type request: :class:`tencentcloud.live.v20180801.models.StopRecordTaskRequest`
@@ -3484,15 +3484,15 @@
             model = models.StopRecordTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopScreenshotTask(self, request):
         """提前结束截图，中止运行中的截图任务。任务被成功终止后，本次任务将不再启动。
 
         :param request: Request instance for StopScreenshotTask.
         :type request: :class:`tencentcloud.live.v20180801.models.StopScreenshotTaskRequest`
@@ -3507,15 +3507,15 @@
             model = models.StopScreenshotTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnBindLiveDomainCert(self, request):
         """解绑域名证书
 
         :param request: Request instance for UnBindLiveDomainCert.
         :type request: :class:`tencentcloud.live.v20180801.models.UnBindLiveDomainCertRequest`
@@ -3530,15 +3530,15 @@
             model = models.UnBindLiveDomainCertResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateLiveWatermark(self, request):
         """更新水印。
 
         :param request: Request instance for UpdateLiveWatermark.
         :type request: :class:`tencentcloud.live.v20180801.models.UpdateLiveWatermarkRequest`
@@ -3553,8 +3553,8 @@
             model = models.UpdateLiveWatermarkResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-live-3.0.937/tencentcloud/live/v20180801/models.py` & `tencentcloud-sdk-python-live-3.0.938/tencentcloud/live/v20180801/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2731,15 +2731,15 @@
         :param _StartTime: 开始时间。
 使用 UTC 格式时间，
 例如：2019-01-08T10:00:00Z。
 注意：北京时间值为 UTC 时间值 + 8 小时。
         :type StartTime: str
         :param _EndTime: 结束时间，注意：
 1. 结束时间必须大于开始时间；
-2. 结束时间和开始时间必须大于当前时间；
+2. 结束时间必须大于当前时间；
 3. 结束时间 和 开始时间 间隔必须小于七天。
 使用 UTC 格式时间，
 例如：2019-01-08T10:00:00Z。
 注意：北京时间值为 UTC 时间值 + 8 小时。
         :type EndTime: str
         :param _Operator: 任务操作人备注。
         :type Operator: str
```

### Comparing `tencentcloud-sdk-python-live-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-live-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-live-3.0.937/tencentcloud_sdk_python_live.egg-info/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.938/tencentcloud_sdk_python_live.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.937/README.rst` & `tencentcloud-sdk-python-live-3.0.938/README.rst`

 * *Files identical despite different names*

