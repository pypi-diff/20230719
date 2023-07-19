# Comparing `tmp/tencentcloud-sdk-python-trtc-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-trtc-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.937.tar", last modified: Tue Jul 18 00:34:11 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.938.tar", last modified: Wed Jul 19 00:52:48 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trtc-3.0.937.tar` & `tencentcloud-sdk-python-trtc-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:11.000000 tencentcloud-sdk-python-trtc-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:34:11.000000 tencentcloud-sdk-python-trtc-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:11.000000 tencentcloud-sdk-python-trtc-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:11.000000 tencentcloud-sdk-python-trtc-3.0.937/tencentcloud/trtc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:11.000000 tencentcloud-sdk-python-trtc-3.0.937/tencentcloud/trtc/v20190722/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:34:11.000000 tencentcloud-sdk-python-trtc-3.0.937/tencentcloud/trtc/v20190722/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9679 2023-07-18 00:34:11.000000 tencentcloud-sdk-python-trtc-3.0.937/tencentcloud/trtc/v20190722/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    57241 2023-07-18 00:34:11.000000 tencentcloud-sdk-python-trtc-3.0.937/tencentcloud/trtc/v20190722/trtc_client.py
--rw-r--r--   0 root         (0) root         (0)   287958 2023-07-18 00:34:11.000000 tencentcloud-sdk-python-trtc-3.0.937/tencentcloud/trtc/v20190722/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:34:11.000000 tencentcloud-sdk-python-trtc-3.0.937/tencentcloud/trtc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:34:11.000000 tencentcloud-sdk-python-trtc-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:34:11.000000 tencentcloud-sdk-python-trtc-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:34:11.000000 tencentcloud-sdk-python-trtc-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:34:11.000000 tencentcloud-sdk-python-trtc-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:11.000000 tencentcloud-sdk-python-trtc-3.0.937/tencentcloud_sdk_python_trtc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:34:11.000000 tencentcloud-sdk-python-trtc-3.0.937/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:34:11.000000 tencentcloud-sdk-python-trtc-3.0.937/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:34:11.000000 tencentcloud-sdk-python-trtc-3.0.937/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:34:11.000000 tencentcloud-sdk-python-trtc-3.0.937/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:52:48.000000 tencentcloud-sdk-python-trtc-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:52:48.000000 tencentcloud-sdk-python-trtc-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:52:48.000000 tencentcloud-sdk-python-trtc-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:52:48.000000 tencentcloud-sdk-python-trtc-3.0.938/tencentcloud/trtc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:52:48.000000 tencentcloud-sdk-python-trtc-3.0.938/tencentcloud/trtc/v20190722/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:52:48.000000 tencentcloud-sdk-python-trtc-3.0.938/tencentcloud/trtc/v20190722/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9679 2023-07-19 00:52:48.000000 tencentcloud-sdk-python-trtc-3.0.938/tencentcloud/trtc/v20190722/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    57385 2023-07-19 00:52:48.000000 tencentcloud-sdk-python-trtc-3.0.938/tencentcloud/trtc/v20190722/trtc_client.py
+-rw-r--r--   0 root         (0) root         (0)   287958 2023-07-19 00:52:48.000000 tencentcloud-sdk-python-trtc-3.0.938/tencentcloud/trtc/v20190722/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:52:48.000000 tencentcloud-sdk-python-trtc-3.0.938/tencentcloud/trtc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:52:48.000000 tencentcloud-sdk-python-trtc-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:52:48.000000 tencentcloud-sdk-python-trtc-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:52:48.000000 tencentcloud-sdk-python-trtc-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:52:48.000000 tencentcloud-sdk-python-trtc-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:52:48.000000 tencentcloud-sdk-python-trtc-3.0.938/tencentcloud_sdk_python_trtc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:52:48.000000 tencentcloud-sdk-python-trtc-3.0.938/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:52:48.000000 tencentcloud-sdk-python-trtc-3.0.938/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:52:48.000000 tencentcloud-sdk-python-trtc-3.0.938/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:52:48.000000 tencentcloud-sdk-python-trtc-3.0.938/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.937/setup.py` & `tencentcloud-sdk-python-trtc-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.937/tencentcloud/trtc/v20190722/errorcodes.py` & `tencentcloud-sdk-python-trtc-3.0.938/tencentcloud/trtc/v20190722/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.937/tencentcloud/trtc/v20190722/trtc_client.py` & `tencentcloud-sdk-python-trtc-3.0.938/tencentcloud/trtc/v20190722/trtc_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             model = models.CreateCloudRecordingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePicture(self, request):
         """如果您需要在 [云端混流转码](https://cloud.tencent.com/document/product/647/16827) 时频繁新增自定义背景图或水印，可通过此接口上传新的图片素材。无需频繁新增图片的场景，建议直接在 [控制台 > 应用管理 > 素材管理](https://cloud.tencent.com/document/product/647/50769) 中操作。
 
         :param request: Request instance for CreatePicture.
         :type request: :class:`tencentcloud.trtc.v20190722.models.CreatePictureRequest`
@@ -76,15 +76,15 @@
             model = models.CreatePictureResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCloudRecording(self, request):
         """成功开启录制后，可以使用此接口来停止录制任务。停止录制成功后不代表文件全部传输完成，如果未完成后台将会继续上传文件，成功后通过事件回调通知客户文件全部传输完成状态。
 
         :param request: Request instance for DeleteCloudRecording.
         :type request: :class:`tencentcloud.trtc.v20190722.models.DeleteCloudRecordingRequest`
@@ -99,15 +99,15 @@
             model = models.DeleteCloudRecordingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePicture(self, request):
         """如果您需要在 [云端混流转码](https://cloud.tencent.com/document/product/647/16827) 时频繁删除自定义背景图或水印，可通过此接口删除已上传的图片。无需频繁删除图片的场景，建议直接在 [控制台 > 应用管理 > 素材管理](https://cloud.tencent.com/document/product/647/50769) 中操作。
 
         :param request: Request instance for DeletePicture.
         :type request: :class:`tencentcloud.trtc.v20190722.models.DeletePictureRequest`
@@ -122,15 +122,15 @@
             model = models.DeletePictureResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCallDetailInfo(self, request):
         """查询指定时间内的用户列表及用户通话质量数据，可查询14天内数据。DataType 不为null，查询起止时间不超过1个小时，查询用户不超过6个，支持跨天查询。DataType为null时，查询起止时间不超过4个小时， 默认查询6个用户，同时支持每页查询100以内用户个数（PageSize不超过100）。接口用于查询质量问题，不推荐作为计费使用。（同老接口DescribeCallDetail）
         **注意**：
         1.该接口只用于历史数据统计或核对数据使用，实时类关键业务逻辑不能使用。
         2.该接口目前免费提供中，监控仪表盘商业化计费后该接口需要订阅付费版后方可调用，仪表盘商业化说明请见：https://cloud.tencent.com/document/product/647/77735
@@ -148,15 +148,15 @@
             model = models.DescribeCallDetailInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudRecording(self, request):
         """成功开启录制后，可以使用此接口来查询录制状态。仅在录制任务进行时有效，录制退出后查询将会返回错误。
         录制文件上传到云点播VOD时，StorageFileList中不会返回录制文件信息，请订阅相关录制文件回调事件，获取录制文件信息。
 
         :param request: Request instance for DescribeCloudRecording.
@@ -172,15 +172,15 @@
             model = models.DescribeCloudRecordingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMixTranscodingUsage(self, request):
         """获取TRTC混流转码的用量明细。
         - 查询时间小于等于1天时，返回每5分钟粒度的数据；查询时间大于1天时，返回按天汇总的数据。
         - 单次查询统计区间最多不能超过31天。
         - 若查询当天用量，由于统计延迟等原因，返回数据可能不够准确。
@@ -200,15 +200,15 @@
             model = models.DescribeMixTranscodingUsageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePicture(self, request):
         """如果您需要在 [云端混流转码](https://cloud.tencent.com/document/product/647/16827) 时频繁查找自定义背景图或水印信息，可通过此接口查找已上传的图片信息。无需频繁查找图片信息的场景，建议直接在 [控制台 > 应用管理 > 素材管理](https://cloud.tencent.com/document/product/647/50769) 中查看。
 
         :param request: Request instance for DescribePicture.
         :type request: :class:`tencentcloud.trtc.v20190722.models.DescribePictureRequest`
@@ -223,15 +223,15 @@
             model = models.DescribePictureResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRecordStatistic(self, request):
         """查询云端录制计费时长。
 
         - 查询时间小于等于1天时，返回每5分钟粒度的数据；查询时间大于1天时，返回按天汇总的数据。
         - 单次查询统计区间最多不能超过31天。
@@ -251,15 +251,15 @@
             model = models.DescribeRecordStatisticResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRecordingUsage(self, request):
         """获取TRTC录制的用量明细。
         - 查询时间小于等于1天时，返回每5分钟粒度的数据；查询时间大于1天时，返回按天汇总的数据。
         - 单次查询统计区间最多不能超过31天。
         - 若查询当天用量，由于统计延迟等原因，返回数据可能不够准确。
@@ -279,15 +279,15 @@
             model = models.DescribeRecordingUsageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRelayUsage(self, request):
         """获取TRTC旁路转推的用量明细。
         - 查询时间小于等于1天时，返回每5分钟粒度的数据；查询时间大于1天时，返回按天汇总的数据。
         - 单次查询统计区间最多不能超过31天。
         - 若查询当天用量，由于统计延迟等原因，返回数据可能不够准确。
@@ -307,15 +307,15 @@
             model = models.DescribeRelayUsageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRoomInfo(self, request):
         """查询SdkAppId下的房间列表。默认返回10条通话，一次最多返回100条通话。可查询14天内的数据。（同老接口DescribeRoomInformation）
         **注意**：
         1.该接口只用于历史数据统计或核对数据使用，实时类关键业务逻辑不能使用。
         2.该接口目前免费提供中，监控仪表盘商业化计费后该接口需要订阅付费版后方可调用，仪表盘商业化说明请见：https://cloud.tencent.com/document/product/647/77735
@@ -333,15 +333,15 @@
             model = models.DescribeRoomInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeScaleInfo(self, request):
         """可查询SdkAppId每天的房间数和用户数，按天统计，可查询最近14天的数据。当天未结束，数据未统计完成，无法查到当天的房间数与用户数。（同老接口DescribeHistoryScale）
 
         :param request: Request instance for DescribeScaleInfo.
         :type request: :class:`tencentcloud.trtc.v20190722.models.DescribeScaleInfoRequest`
@@ -356,15 +356,15 @@
             model = models.DescribeScaleInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTRTCMarketQualityMetricData(self, request):
         """查询TRTC监控仪表盘-数据大盘质量指标（包括下列指标）
         joinSuccessRate：加入频道成功率。
         joinSuccessIn5sRate：5s内加入频道成功率。
         audioFreezeRate：音频卡顿率。
@@ -387,15 +387,15 @@
             model = models.DescribeTRTCMarketQualityMetricDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTRTCMarketScaleMetricData(self, request):
         """查询TRTC监控仪表盘-数据大盘规模指标（会返回通话人数，通话房间数，峰值同时在线人数，峰值同时在线频道数）
         userCount：通话人数，
         roomCount：通话房间数，从有用户加入频道到所有用户离开频道计为一个通话频道。
         peakCurrentChannels：峰值同时在线频道数。
@@ -417,15 +417,15 @@
             model = models.DescribeTRTCMarketScaleMetricDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTRTCRealTimeQualityMetricData(self, request):
         """查询TRTC监控仪表盘-实时监控质量指标（会返回下列指标）
         -视频卡顿率
         -音频卡顿率
         注意：
@@ -445,15 +445,15 @@
             model = models.DescribeTRTCRealTimeQualityMetricDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTRTCRealTimeScaleMetricData(self, request):
         """查询TRTC监控仪表盘-实时监控规模指标（会返回下列指标）
         -userCount（在线用户数）
         -roomCount（在线房间数）
         注意：
@@ -475,15 +475,15 @@
             model = models.DescribeTRTCRealTimeScaleMetricDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTrtcMcuTranscodeTime(self, request):
         """查询旁路转码计费时长。
         - 查询时间小于等于1天时，返回每5分钟粒度的数据；查询时间大于1天时，返回按天汇总的数据。
         - 单次查询统计区间最多不能超过31天。
         - 若查询当天用量，由于统计延迟等原因，返回数据可能不够准确。
@@ -502,15 +502,15 @@
             model = models.DescribeTrtcMcuTranscodeTimeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTrtcRoomUsage(self, request):
         """查询TRTC音视频房间维度用量。
         - 单次只能查询一天数据，返回查询时间段内的汇总数据；通过多次查询可以查不同天数据。若查询跨天用量，由于统计延迟等原因，返回数据可能不够准确。
         - 该接口只用于历史用量数据统计或核对数据使用，关键业务逻辑不能使用。
         - 默认接口请求频率限制：1次/15秒。
@@ -528,15 +528,15 @@
             model = models.DescribeTrtcRoomUsageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTrtcUsage(self, request):
         """获取TRTC音视频互动的用量明细。
         - 查询时间小于等于1天时，返回每5分钟粒度的数据；查询时间大于1天时，返回按天汇总的数据。
         - 单次查询统计区间最多不能超过31天。
         - 若查询当天用量，由于统计延迟等原因，返回数据可能不够准确。
@@ -556,15 +556,15 @@
             model = models.DescribeTrtcUsageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUnusualEvent(self, request):
         """查询SdkAppId下任意20条异常体验事件，返回异常体验ID与可能产生异常体验的原因。可查询14天内数据，查询起止时间不超过1个小时。支持跨天查询。（同老接口DescribeAbnormalEvent）
         异常体验ID映射见：https://cloud.tencent.com/document/product/647/44916
 
         :param request: Request instance for DescribeUnusualEvent.
@@ -580,15 +580,15 @@
             model = models.DescribeUnusualEventResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserEvent(self, request):
         """查询用户某次通话内的进退房，视频开关等详细事件。可查询14天内数据。（同接口DescribeDetailEvent）
 
         :param request: Request instance for DescribeUserEvent.
         :type request: :class:`tencentcloud.trtc.v20190722.models.DescribeUserEventRequest`
@@ -603,15 +603,15 @@
             model = models.DescribeUserEventResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserInfo(self, request):
         """查询指定时间内的用户列表，可查询14天内数据，查询起止时间不超过4小时。默认每页查询6个用户，支持每页最大查询100个用户PageSize不超过100）。（同老接口DescribeUserInformation）
         **注意**：
         1.该接口只用于历史数据统计或核对数据使用，实时类关键业务逻辑不能使用。
         2.该接口目前免费提供中，监控仪表盘商业化计费后该接口需要订阅付费版后方可调用，仪表盘商业化说明请见：https://cloud.tencent.com/document/product/647/77735
@@ -629,15 +629,15 @@
             model = models.DescribeUserInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DismissRoom(self, request):
         """接口说明：把房间所有用户从房间移出，解散房间。支持所有平台，Android、iOS、Windows 和 macOS 需升级到 TRTC SDK 6.6及以上版本。
 
         :param request: Request instance for DismissRoom.
         :type request: :class:`tencentcloud.trtc.v20190722.models.DismissRoomRequest`
@@ -652,15 +652,15 @@
             model = models.DismissRoomResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DismissRoomByStrRoomId(self, request):
         """接口说明：把房间所有用户从房间移出，解散房间。支持所有平台，Android、iOS、Windows 和 macOS 需升级到 TRTC SDK 6.6及以上版本。
 
         :param request: Request instance for DismissRoomByStrRoomId.
         :type request: :class:`tencentcloud.trtc.v20190722.models.DismissRoomByStrRoomIdRequest`
@@ -675,15 +675,15 @@
             model = models.DismissRoomByStrRoomIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCloudRecording(self, request):
         """成功开启录制后，可以使用此接口来更新录制任务。仅在录制任务进行时有效，录制退出后更新将会返回错误。更新操作是全量覆盖，并不是增量更新的模式，也就是说每次更新都需要携带全量的信息。
 
         :param request: Request instance for ModifyCloudRecording.
         :type request: :class:`tencentcloud.trtc.v20190722.models.ModifyCloudRecordingRequest`
@@ -698,15 +698,15 @@
             model = models.ModifyCloudRecordingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPicture(self, request):
         """如果您需要在 [云端混流转码](https://cloud.tencent.com/document/product/647/16827) 时频繁修改自定义背景图或水印素材，可通过此接口修改已上传的图片。无需频繁修改图片素材的场景，建议直接在 [控制台 > 应用管理 > 素材管理](https://cloud.tencent.com/document/product/647/50769) 中操作。
 
         :param request: Request instance for ModifyPicture.
         :type request: :class:`tencentcloud.trtc.v20190722.models.ModifyPictureRequest`
@@ -721,15 +721,15 @@
             model = models.ModifyPictureResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RemoveUser(self, request):
         """接口说明：将用户从房间移出，适用于主播/房主/管理员踢人等场景。支持所有平台，Android、iOS、Windows 和 macOS 需升级到 TRTC SDK 6.6及以上版本。
 
         :param request: Request instance for RemoveUser.
         :type request: :class:`tencentcloud.trtc.v20190722.models.RemoveUserRequest`
@@ -744,15 +744,15 @@
             model = models.RemoveUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RemoveUserByStrRoomId(self, request):
         """接口说明：将用户从房间移出，适用于主播/房主/管理员踢人等场景。支持所有平台，Android、iOS、Windows 和 macOS 需升级到 TRTC SDK 6.6及以上版本。
 
         :param request: Request instance for RemoveUserByStrRoomId.
         :type request: :class:`tencentcloud.trtc.v20190722.models.RemoveUserByStrRoomIdRequest`
@@ -767,15 +767,15 @@
             model = models.RemoveUserByStrRoomIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartMCUMixTranscode(self, request):
         """接口说明：启动云端混流，并指定混流画面中各路画面的布局位置。
 
         TRTC 的一个房间中可能会同时存在多路音视频流，您可以通过此 API 接口，通知腾讯云服务端将多路视频画面合成一路，并指定每一路画面的位置，同时将多路声音进行混音，最终形成一路音视频流，以便用于录制和直播观看。房间销毁后混流自动结束。
 
@@ -810,15 +810,15 @@
             model = models.StartMCUMixTranscodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartMCUMixTranscodeByStrRoomId(self, request):
         """接口说明：启动云端混流，并指定混流画面中各路画面的布局位置。
 
         TRTC 的一个房间中可能会同时存在多路音视频流，您可以通过此 API 接口，通知腾讯云服务端将多路视频画面合成一路，并指定每一路画面的位置，同时将多路声音进行混音，最终形成一路音视频流，以便用于录制和直播观看。
 
@@ -853,15 +853,15 @@
             model = models.StartMCUMixTranscodeByStrRoomIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartPublishCdnStream(self, request):
         """接口说明：启动旁路以及混流转推任务。TRTC 的房间中可能会同时存在多路音视频流，您可以通过此API接口，实现以下几种效果：
         1、支持将单个主播的音视频流发布（也称作“转推”）到直播CDN上，请参考示例2（发起单流音视频旁路转推）和示例3（发起单流纯音频旁路转推）。
         2、支持将同个房间多个主播或者不同房间多个主播的音视频混合成1路后再发布到直播CDN上，您可以通过AudioParams.SubscribeAudioList和VideoParams.LayoutParams调整参与混音的用户列表以及指定各路混流画面的布局位置。请参考示例1（发起混流转推）。
         3、支持预先设置一个房间的混流模板，将该房间中的多个音视频混合成1路发布到直播CDN，腾讯云后台实时监控TRTC房间中的主播变化，自动按照混流模板调整布局。目前已经支持了如下几种混流预设模板：
@@ -897,15 +897,15 @@
             model = models.StartPublishCdnStreamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopMCUMixTranscode(self, request):
         """接口说明：结束云端混流
 
         :param request: Request instance for StopMCUMixTranscode.
         :type request: :class:`tencentcloud.trtc.v20190722.models.StopMCUMixTranscodeRequest`
@@ -920,15 +920,15 @@
             model = models.StopMCUMixTranscodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopMCUMixTranscodeByStrRoomId(self, request):
         """接口说明：结束云端混流
 
         :param request: Request instance for StopMCUMixTranscodeByStrRoomId.
         :type request: :class:`tencentcloud.trtc.v20190722.models.StopMCUMixTranscodeByStrRoomIdRequest`
@@ -943,15 +943,15 @@
             model = models.StopMCUMixTranscodeByStrRoomIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopPublishCdnStream(self, request):
         """停止转推任务。
 
         :param request: Request instance for StopPublishCdnStream.
         :type request: :class:`tencentcloud.trtc.v20190722.models.StopPublishCdnStreamRequest`
@@ -966,15 +966,15 @@
             model = models.StopPublishCdnStreamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdatePublishCdnStream(self, request):
         """更新转推任务。
         注：请参见启动转推任务的接口说明和使用说明。
 
         :param request: Request instance for UpdatePublishCdnStream.
@@ -990,8 +990,8 @@
             model = models.UpdatePublishCdnStreamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.937/tencentcloud/trtc/v20190722/models.py` & `tencentcloud-sdk-python-trtc-3.0.938/tencentcloud/trtc/v20190722/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trtc-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-trtc-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.938/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.937/README.rst` & `tencentcloud-sdk-python-trtc-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.937/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.938/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

