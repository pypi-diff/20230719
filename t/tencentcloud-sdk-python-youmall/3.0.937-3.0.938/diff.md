# Comparing `tmp/tencentcloud-sdk-python-youmall-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-youmall-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-youmall-3.0.937.tar", last modified: Tue Jul 18 00:35:52 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-youmall-3.0.938.tar", last modified: Wed Jul 19 00:54:20 2023, max compression
```

## Comparing `tencentcloud-sdk-python-youmall-3.0.937.tar` & `tencentcloud-sdk-python-youmall-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:52.000000 tencentcloud-sdk-python-youmall-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-18 00:35:52.000000 tencentcloud-sdk-python-youmall-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:52.000000 tencentcloud-sdk-python-youmall-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:52.000000 tencentcloud-sdk-python-youmall-3.0.937/tencentcloud/youmall/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:35:52.000000 tencentcloud-sdk-python-youmall-3.0.937/tencentcloud/youmall/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:52.000000 tencentcloud-sdk-python-youmall-3.0.937/tencentcloud/youmall/v20180228/
--rw-r--r--   0 root         (0) root         (0)    31393 2023-07-18 00:35:52.000000 tencentcloud-sdk-python-youmall-3.0.937/tencentcloud/youmall/v20180228/youmall_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:35:52.000000 tencentcloud-sdk-python-youmall-3.0.937/tencentcloud/youmall/v20180228/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2828 2023-07-18 00:35:52.000000 tencentcloud-sdk-python-youmall-3.0.937/tencentcloud/youmall/v20180228/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   184858 2023-07-18 00:35:52.000000 tencentcloud-sdk-python-youmall-3.0.937/tencentcloud/youmall/v20180228/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:35:52.000000 tencentcloud-sdk-python-youmall-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:35:52.000000 tencentcloud-sdk-python-youmall-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:52.000000 tencentcloud-sdk-python-youmall-3.0.937/tencentcloud_sdk_python_youmall.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:35:52.000000 tencentcloud-sdk-python-youmall-3.0.937/tencentcloud_sdk_python_youmall.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-18 00:35:52.000000 tencentcloud-sdk-python-youmall-3.0.937/tencentcloud_sdk_python_youmall.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:35:52.000000 tencentcloud-sdk-python-youmall-3.0.937/tencentcloud_sdk_python_youmall.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:35:52.000000 tencentcloud-sdk-python-youmall-3.0.937/tencentcloud_sdk_python_youmall.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:35:52.000000 tencentcloud-sdk-python-youmall-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-18 00:35:52.000000 tencentcloud-sdk-python-youmall-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:54:20.000000 tencentcloud-sdk-python-youmall-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-19 00:54:20.000000 tencentcloud-sdk-python-youmall-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:54:20.000000 tencentcloud-sdk-python-youmall-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:54:20.000000 tencentcloud-sdk-python-youmall-3.0.938/tencentcloud/youmall/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:54:20.000000 tencentcloud-sdk-python-youmall-3.0.938/tencentcloud/youmall/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:54:20.000000 tencentcloud-sdk-python-youmall-3.0.938/tencentcloud/youmall/v20180228/
+-rw-r--r--   0 root         (0) root         (0)    31517 2023-07-19 00:54:20.000000 tencentcloud-sdk-python-youmall-3.0.938/tencentcloud/youmall/v20180228/youmall_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:54:20.000000 tencentcloud-sdk-python-youmall-3.0.938/tencentcloud/youmall/v20180228/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2828 2023-07-19 00:54:20.000000 tencentcloud-sdk-python-youmall-3.0.938/tencentcloud/youmall/v20180228/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   184858 2023-07-19 00:54:20.000000 tencentcloud-sdk-python-youmall-3.0.938/tencentcloud/youmall/v20180228/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:54:20.000000 tencentcloud-sdk-python-youmall-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:54:20.000000 tencentcloud-sdk-python-youmall-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:54:20.000000 tencentcloud-sdk-python-youmall-3.0.938/tencentcloud_sdk_python_youmall.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:54:20.000000 tencentcloud-sdk-python-youmall-3.0.938/tencentcloud_sdk_python_youmall.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-19 00:54:20.000000 tencentcloud-sdk-python-youmall-3.0.938/tencentcloud_sdk_python_youmall.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:54:20.000000 tencentcloud-sdk-python-youmall-3.0.938/tencentcloud_sdk_python_youmall.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:54:20.000000 tencentcloud-sdk-python-youmall-3.0.938/tencentcloud_sdk_python_youmall.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:54:20.000000 tencentcloud-sdk-python-youmall-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-19 00:54:20.000000 tencentcloud-sdk-python-youmall-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-youmall-3.0.937/setup.py` & `tencentcloud-sdk-python-youmall-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-youmall-3.0.937/tencentcloud/youmall/v20180228/youmall_client.py` & `tencentcloud-sdk-python-youmall-3.0.938/tencentcloud/youmall/v20180228/youmall_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFacePicture(self, request):
         """通过上传指定规格的人脸图片，创建黑名单用户或者白名单用户。
 
         :param request: Request instance for CreateFacePicture.
         :type request: :class:`tencentcloud.youmall.v20180228.models.CreateFacePictureRequest`
@@ -65,15 +65,15 @@
             model = models.CreateFacePictureResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePersonFeature(self, request):
         """删除顾客特征，仅支持删除黑名单或者白名单用户特征。
 
         :param request: Request instance for DeletePersonFeature.
         :type request: :class:`tencentcloud.youmall.v20180228.models.DeletePersonFeatureRequest`
@@ -88,15 +88,15 @@
             model = models.DeletePersonFeatureResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCameraPerson(self, request):
         """通过指定设备ID和指定时段，获取该时段内中收银台摄像设备抓取到顾客头像及身份ID
 
         :param request: Request instance for DescribeCameraPerson.
         :type request: :class:`tencentcloud.youmall.v20180228.models.DescribeCameraPersonRequest`
@@ -111,15 +111,15 @@
             model = models.DescribeCameraPersonResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterPersonArrivedMall(self, request):
         """输出开始时间到结束时间段内的进出场数据。按天聚合的情况下，每天多次进出场算一次，以最初进场时间为进场时间，最后离场时间为离场时间。停留时间为多次进出场的停留时间之和。
 
         :param request: Request instance for DescribeClusterPersonArrivedMall.
         :type request: :class:`tencentcloud.youmall.v20180228.models.DescribeClusterPersonArrivedMallRequest`
@@ -134,15 +134,15 @@
             model = models.DescribeClusterPersonArrivedMallResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterPersonTrace(self, request):
         """输出开始时间到结束时间段内的进出场数据。按天聚合的情况下，每天多次进出场算一次，以最初进场时间为进场时间，最后离场时间为离场时间。
 
         :param request: Request instance for DescribeClusterPersonTrace.
         :type request: :class:`tencentcloud.youmall.v20180228.models.DescribeClusterPersonTraceRequest`
@@ -157,15 +157,15 @@
             model = models.DescribeClusterPersonTraceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFaceIdByTempId(self, request):
         """通过DescribeCameraPerson接口上报的收银台身份ID查询顾客的FaceID。查询最佳时间为收银台上报的次日1点后。
 
         :param request: Request instance for DescribeFaceIdByTempId.
         :type request: :class:`tencentcloud.youmall.v20180228.models.DescribeFaceIdByTempIdRequest`
@@ -180,15 +180,15 @@
             model = models.DescribeFaceIdByTempIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHistoryNetworkInfo(self, request):
         """返回当前门店历史网络状态数据
 
         :param request: Request instance for DescribeHistoryNetworkInfo.
         :type request: :class:`tencentcloud.youmall.v20180228.models.DescribeHistoryNetworkInfoRequest`
@@ -203,15 +203,15 @@
             model = models.DescribeHistoryNetworkInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNetworkInfo(self, request):
         """返回当前门店最新网络状态数据
 
         :param request: Request instance for DescribeNetworkInfo.
         :type request: :class:`tencentcloud.youmall.v20180228.models.DescribeNetworkInfoRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeNetworkInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePerson(self, request):
         """查询指定某一卖场的用户信息
 
         :param request: Request instance for DescribePerson.
         :type request: :class:`tencentcloud.youmall.v20180228.models.DescribePersonRequest`
@@ -249,15 +249,15 @@
             model = models.DescribePersonResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePersonArrivedMall(self, request):
         """输出开始时间到结束时间段内的进出场数据。不做按天聚合的情况下，每次进出场，产生一条进出场数据。
 
 
         :param request: Request instance for DescribePersonArrivedMall.
@@ -273,15 +273,15 @@
             model = models.DescribePersonArrivedMallResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePersonInfo(self, request):
         """指定门店获取所有顾客详情列表，包含客户ID、图片、年龄、性别
 
         :param request: Request instance for DescribePersonInfo.
         :type request: :class:`tencentcloud.youmall.v20180228.models.DescribePersonInfoRequest`
@@ -296,15 +296,15 @@
             model = models.DescribePersonInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePersonInfoByFacePicture(self, request):
         """通过上传人脸图片检索系统face id、顾客身份信息及底图
 
         :param request: Request instance for DescribePersonInfoByFacePicture.
         :type request: :class:`tencentcloud.youmall.v20180228.models.DescribePersonInfoByFacePictureRequest`
@@ -319,15 +319,15 @@
             model = models.DescribePersonInfoByFacePictureResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePersonTrace(self, request):
         """输出开始时间到结束时间段内的进出场数据。
 
         :param request: Request instance for DescribePersonTrace.
         :type request: :class:`tencentcloud.youmall.v20180228.models.DescribePersonTraceRequest`
@@ -342,15 +342,15 @@
             model = models.DescribePersonTraceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePersonTraceDetail(self, request):
         """查询客户单次到场轨迹明细
 
         :param request: Request instance for DescribePersonTraceDetail.
         :type request: :class:`tencentcloud.youmall.v20180228.models.DescribePersonTraceDetailRequest`
@@ -365,15 +365,15 @@
             model = models.DescribePersonTraceDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePersonVisitInfo(self, request):
         """获取门店指定时间范围内的所有用户到访信息记录，支持的时间范围：过去365天，含当天。
 
         :param request: Request instance for DescribePersonVisitInfo.
         :type request: :class:`tencentcloud.youmall.v20180228.models.DescribePersonVisitInfoRequest`
@@ -388,15 +388,15 @@
             model = models.DescribePersonVisitInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeShopHourTrafficInfo(self, request):
         """按小时提供查询日期范围内门店的每天每小时累计客流人数数据，支持的时间范围：过去365天，含当天。
 
         :param request: Request instance for DescribeShopHourTrafficInfo.
         :type request: :class:`tencentcloud.youmall.v20180228.models.DescribeShopHourTrafficInfoRequest`
@@ -411,15 +411,15 @@
             model = models.DescribeShopHourTrafficInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeShopInfo(self, request):
         """根据客户身份标识获取客户下所有的门店信息列表
 
         :param request: Request instance for DescribeShopInfo.
         :type request: :class:`tencentcloud.youmall.v20180228.models.DescribeShopInfoRequest`
@@ -434,15 +434,15 @@
             model = models.DescribeShopInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeShopTrafficInfo(self, request):
         """按天提供查询日期范围内门店的单日累计客流人数，支持的时间范围：过去365天，含当天。
 
         :param request: Request instance for DescribeShopTrafficInfo.
         :type request: :class:`tencentcloud.youmall.v20180228.models.DescribeShopTrafficInfoRequest`
@@ -457,15 +457,15 @@
             model = models.DescribeShopTrafficInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTrajectoryData(self, request):
         """获取动线轨迹信息
 
         :param request: Request instance for DescribeTrajectoryData.
         :type request: :class:`tencentcloud.youmall.v20180228.models.DescribeTrajectoryDataRequest`
@@ -480,15 +480,15 @@
             model = models.DescribeTrajectoryDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeZoneFlowAgeInfoByZoneId(self, request):
         """获取指定区域人流各年龄占比
 
         :param request: Request instance for DescribeZoneFlowAgeInfoByZoneId.
         :type request: :class:`tencentcloud.youmall.v20180228.models.DescribeZoneFlowAgeInfoByZoneIdRequest`
@@ -503,15 +503,15 @@
             model = models.DescribeZoneFlowAgeInfoByZoneIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeZoneFlowAndStayTime(self, request):
         """获取区域人流和停留时间
 
         :param request: Request instance for DescribeZoneFlowAndStayTime.
         :type request: :class:`tencentcloud.youmall.v20180228.models.DescribeZoneFlowAndStayTimeRequest`
@@ -526,15 +526,15 @@
             model = models.DescribeZoneFlowAndStayTimeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeZoneFlowDailyByZoneId(self, request):
         """获取指定区域每日客流量
 
         :param request: Request instance for DescribeZoneFlowDailyByZoneId.
         :type request: :class:`tencentcloud.youmall.v20180228.models.DescribeZoneFlowDailyByZoneIdRequest`
@@ -549,15 +549,15 @@
             model = models.DescribeZoneFlowDailyByZoneIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeZoneFlowGenderAvrStayTimeByZoneId(self, request):
         """获取指定区域不同年龄段男女平均停留时间
 
         :param request: Request instance for DescribeZoneFlowGenderAvrStayTimeByZoneId.
         :type request: :class:`tencentcloud.youmall.v20180228.models.DescribeZoneFlowGenderAvrStayTimeByZoneIdRequest`
@@ -572,15 +572,15 @@
             model = models.DescribeZoneFlowGenderAvrStayTimeByZoneIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeZoneFlowGenderInfoByZoneId(self, request):
         """获取指定区域性别占比
 
         :param request: Request instance for DescribeZoneFlowGenderInfoByZoneId.
         :type request: :class:`tencentcloud.youmall.v20180228.models.DescribeZoneFlowGenderInfoByZoneIdRequest`
@@ -595,15 +595,15 @@
             model = models.DescribeZoneFlowGenderInfoByZoneIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeZoneFlowHourlyByZoneId(self, request):
         """获取指定区域分时客流量
 
         :param request: Request instance for DescribeZoneFlowHourlyByZoneId.
         :type request: :class:`tencentcloud.youmall.v20180228.models.DescribeZoneFlowHourlyByZoneIdRequest`
@@ -618,15 +618,15 @@
             model = models.DescribeZoneFlowHourlyByZoneIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeZoneTrafficInfo(self, request):
         """按天提供查询日期范围内，客户指定门店下的所有区域（优Mall部署时已配置区域）的累计客流人次和平均停留时间。支持的时间范围：过去365天，含当天。
 
         :param request: Request instance for DescribeZoneTrafficInfo.
         :type request: :class:`tencentcloud.youmall.v20180228.models.DescribeZoneTrafficInfoRequest`
@@ -641,15 +641,15 @@
             model = models.DescribeZoneTrafficInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPersonFeatureInfo(self, request):
         """支持修改黑白名单类型的顾客特征
 
         :param request: Request instance for ModifyPersonFeatureInfo.
         :type request: :class:`tencentcloud.youmall.v20180228.models.ModifyPersonFeatureInfoRequest`
@@ -664,15 +664,15 @@
             model = models.ModifyPersonFeatureInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPersonTagInfo(self, request):
         """标记到店顾客的身份类型，例如黑名单、白名单等
 
         :param request: Request instance for ModifyPersonTagInfo.
         :type request: :class:`tencentcloud.youmall.v20180228.models.ModifyPersonTagInfoRequest`
@@ -687,15 +687,15 @@
             model = models.ModifyPersonTagInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPersonType(self, request):
         """修改顾客身份类型接口
 
         :param request: Request instance for ModifyPersonType.
         :type request: :class:`tencentcloud.youmall.v20180228.models.ModifyPersonTypeRequest`
@@ -710,15 +710,15 @@
             model = models.ModifyPersonTypeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RegisterCallback(self, request):
         """调用本接口在优Mall中注册自己集团的到店通知回调接口地址，接口协议为HTTP或HTTPS。注册后，若集团有特殊身份（例如老客）到店通知，优Mall后台将主动将到店信息push给该接口
 
         :param request: Request instance for RegisterCallback.
         :type request: :class:`tencentcloud.youmall.v20180228.models.RegisterCallbackRequest`
@@ -733,8 +733,8 @@
             model = models.RegisterCallbackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-youmall-3.0.937/tencentcloud/youmall/v20180228/errorcodes.py` & `tencentcloud-sdk-python-youmall-3.0.938/tencentcloud/youmall/v20180228/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-youmall-3.0.937/tencentcloud/youmall/v20180228/models.py` & `tencentcloud-sdk-python-youmall-3.0.938/tencentcloud/youmall/v20180228/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-youmall-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-youmall-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-youmall-3.0.937/tencentcloud_sdk_python_youmall.egg-info/PKG-INFO` & `tencentcloud-sdk-python-youmall-3.0.938/tencentcloud_sdk_python_youmall.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-youmall
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Youmall SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-youmall-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-youmall-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-youmall
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Youmall SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-youmall-3.0.937/README.rst` & `tencentcloud-sdk-python-youmall-3.0.938/README.rst`

 * *Files identical despite different names*

