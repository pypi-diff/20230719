# Comparing `tmp/tencentcloud-sdk-python-gme-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-gme-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-gme-3.0.937.tar", last modified: Tue Jul 18 00:24:23 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-gme-3.0.938.tar", last modified: Wed Jul 19 00:39:41 2023, max compression
```

## Comparing `tencentcloud-sdk-python-gme-3.0.937.tar` & `tencentcloud-sdk-python-gme-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:23.000000 tencentcloud-sdk-python-gme-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:24:23.000000 tencentcloud-sdk-python-gme-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:23.000000 tencentcloud-sdk-python-gme-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:24:23.000000 tencentcloud-sdk-python-gme-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:23.000000 tencentcloud-sdk-python-gme-3.0.937/tencentcloud/gme/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:24:23.000000 tencentcloud-sdk-python-gme-3.0.937/tencentcloud/gme/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:23.000000 tencentcloud-sdk-python-gme-3.0.937/tencentcloud/gme/v20180711/
--rw-r--r--   0 root         (0) root         (0)    33250 2023-07-18 00:24:23.000000 tencentcloud-sdk-python-gme-3.0.937/tencentcloud/gme/v20180711/gme_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:24:23.000000 tencentcloud-sdk-python-gme-3.0.937/tencentcloud/gme/v20180711/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3906 2023-07-18 00:24:23.000000 tencentcloud-sdk-python-gme-3.0.937/tencentcloud/gme/v20180711/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   157807 2023-07-18 00:24:23.000000 tencentcloud-sdk-python-gme-3.0.937/tencentcloud/gme/v20180711/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:24:23.000000 tencentcloud-sdk-python-gme-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:24:23.000000 tencentcloud-sdk-python-gme-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:24:23.000000 tencentcloud-sdk-python-gme-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:23.000000 tencentcloud-sdk-python-gme-3.0.937/tencentcloud_sdk_python_gme.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:24:23.000000 tencentcloud-sdk-python-gme-3.0.937/tencentcloud_sdk_python_gme.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:24:23.000000 tencentcloud-sdk-python-gme-3.0.937/tencentcloud_sdk_python_gme.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:24:23.000000 tencentcloud-sdk-python-gme-3.0.937/tencentcloud_sdk_python_gme.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:24:23.000000 tencentcloud-sdk-python-gme-3.0.937/tencentcloud_sdk_python_gme.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:41.000000 tencentcloud-sdk-python-gme-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:39:41.000000 tencentcloud-sdk-python-gme-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:41.000000 tencentcloud-sdk-python-gme-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:39:41.000000 tencentcloud-sdk-python-gme-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:41.000000 tencentcloud-sdk-python-gme-3.0.938/tencentcloud/gme/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:39:41.000000 tencentcloud-sdk-python-gme-3.0.938/tencentcloud/gme/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:41.000000 tencentcloud-sdk-python-gme-3.0.938/tencentcloud/gme/v20180711/
+-rw-r--r--   0 root         (0) root         (0)    33362 2023-07-19 00:39:41.000000 tencentcloud-sdk-python-gme-3.0.938/tencentcloud/gme/v20180711/gme_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:39:41.000000 tencentcloud-sdk-python-gme-3.0.938/tencentcloud/gme/v20180711/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3906 2023-07-19 00:39:41.000000 tencentcloud-sdk-python-gme-3.0.938/tencentcloud/gme/v20180711/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   157807 2023-07-19 00:39:41.000000 tencentcloud-sdk-python-gme-3.0.938/tencentcloud/gme/v20180711/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:39:41.000000 tencentcloud-sdk-python-gme-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:39:41.000000 tencentcloud-sdk-python-gme-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:39:41.000000 tencentcloud-sdk-python-gme-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:41.000000 tencentcloud-sdk-python-gme-3.0.938/tencentcloud_sdk_python_gme.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:39:41.000000 tencentcloud-sdk-python-gme-3.0.938/tencentcloud_sdk_python_gme.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:39:41.000000 tencentcloud-sdk-python-gme-3.0.938/tencentcloud_sdk_python_gme.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:39:41.000000 tencentcloud-sdk-python-gme-3.0.938/tencentcloud_sdk_python_gme.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:39:41.000000 tencentcloud-sdk-python-gme-3.0.938/tencentcloud_sdk_python_gme.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-gme-3.0.937/setup.py` & `tencentcloud-sdk-python-gme-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gme-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-gme-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-gme-3.0.937/tencentcloud/gme/v20180711/gme_client.py` & `tencentcloud-sdk-python-gme-3.0.938/tencentcloud/gme/v20180711/gme_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             model = models.CreateAgeDetectTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateApp(self, request):
         """本接口(CreateApp)用于创建一个GME应用。
 
         :param request: Request instance for CreateApp.
         :type request: :class:`tencentcloud.gme.v20180711.models.CreateAppRequest`
@@ -75,15 +75,15 @@
             model = models.CreateAppResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCustomization(self, request):
         """用户使用该接口可以创建语音消息转文本热句模型，以供识别调用
 
         :param request: Request instance for CreateCustomization.
         :type request: :class:`tencentcloud.gme.v20180711.models.CreateCustomizationRequest`
@@ -98,15 +98,15 @@
             model = models.CreateCustomizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateScanUser(self, request):
         """新增自定义送检用户
 
         :param request: Request instance for CreateScanUser.
         :type request: :class:`tencentcloud.gme.v20180711.models.CreateScanUserRequest`
@@ -121,15 +121,15 @@
             model = models.CreateScanUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCustomization(self, request):
         """用户通过该接口可以删除语音消息转文本热句模型
 
         :param request: Request instance for DeleteCustomization.
         :type request: :class:`tencentcloud.gme.v20180711.models.DeleteCustomizationRequest`
@@ -144,15 +144,15 @@
             model = models.DeleteCustomizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRoomMember(self, request):
         """本接口(DeleteRoomMember)用户删除房间或者剔除房间内用户
 
         :param request: Request instance for DeleteRoomMember.
         :type request: :class:`tencentcloud.gme.v20180711.models.DeleteRoomMemberRequest`
@@ -167,15 +167,15 @@
             model = models.DeleteRoomMemberResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteScanUser(self, request):
         """删除自定义送检用户
 
         :param request: Request instance for DeleteScanUser.
         :type request: :class:`tencentcloud.gme.v20180711.models.DeleteScanUserRequest`
@@ -190,15 +190,15 @@
             model = models.DeleteScanUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAgeDetectTask(self, request):
         """查询年龄语音识别任务结果，请求频率10次/秒。该接口目前通过白名单开放试用，如有需求，请提交工单申请。
 
         :param request: Request instance for DescribeAgeDetectTask.
         :type request: :class:`tencentcloud.gme.v20180711.models.DescribeAgeDetectTaskRequest`
@@ -213,15 +213,15 @@
             model = models.DescribeAgeDetectTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAppStatistics(self, request):
         """本接口(DescribeAppStatistics)用于获取某个GME应用的用量数据。包括实时语音，语音消息及转文本，语音分析等。最长查询周期为最近60天。
 
         :param request: Request instance for DescribeAppStatistics.
         :type request: :class:`tencentcloud.gme.v20180711.models.DescribeAppStatisticsRequest`
@@ -236,15 +236,15 @@
             model = models.DescribeAppStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApplicationData(self, request):
         """本接口(DescribeApplicationData)用于获取数据详情信息，最多可拉取最近90天的数据。
 
         :param request: Request instance for DescribeApplicationData.
         :type request: :class:`tencentcloud.gme.v20180711.models.DescribeApplicationDataRequest`
@@ -259,15 +259,15 @@
             model = models.DescribeApplicationDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApplicationList(self, request):
         """本接口(DescribeApplicationList)用于查询自己账号下的应用列表
 
         :param request: Request instance for DescribeApplicationList.
         :type request: :class:`tencentcloud.gme.v20180711.models.DescribeApplicationListRequest`
@@ -282,15 +282,15 @@
             model = models.DescribeApplicationListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRealtimeScanConfig(self, request):
         """获取用户自定义送检信息
 
         :param request: Request instance for DescribeRealtimeScanConfig.
         :type request: :class:`tencentcloud.gme.v20180711.models.DescribeRealtimeScanConfigRequest`
@@ -305,15 +305,15 @@
             model = models.DescribeRealtimeScanConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRecordInfo(self, request):
         """查询录制任务信息。
 
         :param request: Request instance for DescribeRecordInfo.
         :type request: :class:`tencentcloud.gme.v20180711.models.DescribeRecordInfoRequest`
@@ -328,15 +328,15 @@
             model = models.DescribeRecordInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRoomInfo(self, request):
         """获取房间内用户信息
 
         :param request: Request instance for DescribeRoomInfo.
         :type request: :class:`tencentcloud.gme.v20180711.models.DescribeRoomInfoRequest`
@@ -351,15 +351,15 @@
             model = models.DescribeRoomInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeScanResultList(self, request):
         """本接口(DescribeScanResultList)用于查询语音检测结果，查询任务列表最多支持100个。
         <p style="color:red">如果在提交语音检测任务时未设置 Callback 字段，则需要通过本接口获取检测结果</p>
 
         :param request: Request instance for DescribeScanResultList.
@@ -375,15 +375,15 @@
             model = models.DescribeScanResultListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskInfo(self, request):
         """查询房间录制的详细信息
 
         :param request: Request instance for DescribeTaskInfo.
         :type request: :class:`tencentcloud.gme.v20180711.models.DescribeTaskInfoRequest`
@@ -398,15 +398,15 @@
             model = models.DescribeTaskInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserInAndOutTime(self, request):
         """拉取用户在房间得进出时间
 
         :param request: Request instance for DescribeUserInAndOutTime.
         :type request: :class:`tencentcloud.gme.v20180711.models.DescribeUserInAndOutTimeRequest`
@@ -421,15 +421,15 @@
             model = models.DescribeUserInAndOutTimeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetCustomizationList(self, request):
         """查询语音消息转文本热句模型列表
 
         :param request: Request instance for GetCustomizationList.
         :type request: :class:`tencentcloud.gme.v20180711.models.GetCustomizationListRequest`
@@ -444,15 +444,15 @@
             model = models.GetCustomizationListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAppStatus(self, request):
         """本接口(ModifyAppStatus)用于修改应用总开关状态。
 
         :param request: Request instance for ModifyAppStatus.
         :type request: :class:`tencentcloud.gme.v20180711.models.ModifyAppStatusRequest`
@@ -467,15 +467,15 @@
             model = models.ModifyAppStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCustomization(self, request):
         """用户通过该接口可以更新语音消息转文本热句模型。
 
         :param request: Request instance for ModifyCustomization.
         :type request: :class:`tencentcloud.gme.v20180711.models.ModifyCustomizationRequest`
@@ -490,15 +490,15 @@
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
         """通过该接口，用户可以修改语音消息转文本热句模型状态，上下线热句模型
 
         :param request: Request instance for ModifyCustomizationState.
         :type request: :class:`tencentcloud.gme.v20180711.models.ModifyCustomizationStateRequest`
@@ -513,15 +513,15 @@
             model = models.ModifyCustomizationStateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRecordInfo(self, request):
         """修改录制配置信息
 
         :param request: Request instance for ModifyRecordInfo.
         :type request: :class:`tencentcloud.gme.v20180711.models.ModifyRecordInfoRequest`
@@ -536,15 +536,15 @@
             model = models.ModifyRecordInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyUserMicStatus(self, request):
         """**接口作用**：此接口用于修改房间用户的麦克风状态，例如房间内用户麦克风为打开状态，可调用此接口将该用户麦克风进行关闭，关闭后即使该用户使用客户端接口 EnableMic 打开麦克风，依然无法与房间内成员通话，属于被禁言状态。该状态持续到此用户退房后失效，或者调用该接口重新打开此用户麦克风状态。
         **接口应用场景**：此接口多用于游戏业务中台或者风控后台，对一些发表不当言论的玩家进行禁言处理。
         **接口使用前提**：目前 ModifyUserMicStatus 接口通过白名单开放，如需使用，需要 [提交工单申请](https://console.cloud.tencent.com/workorder/category?level1_id=438&level2_id=445&source=0&data_title=%E6%B8%B8%E6%88%8F%E5%A4%9A%E5%AA%92%E4%BD%93%E5%BC%95%E6%93%8EGME&step=1)。
 
@@ -561,15 +561,15 @@
             model = models.ModifyUserMicStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ScanVoice(self, request):
         """本接口(ScanVoice)用于提交语音检测任务，检测任务列表最多支持100个。使用前请您登录[控制台 - 服务配置](https://console.cloud.tencent.com/gamegme/conf)开启语音内容安全服务。
         </br></br>
 
         <h4><b>功能试用说明：</b></h4>
@@ -719,15 +719,15 @@
             model = models.ScanVoiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartRecord(self, request):
         """开启录制
 
         :param request: Request instance for StartRecord.
         :type request: :class:`tencentcloud.gme.v20180711.models.StartRecordRequest`
@@ -742,15 +742,15 @@
             model = models.StartRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopRecord(self, request):
         """停止录制
 
         :param request: Request instance for StopRecord.
         :type request: :class:`tencentcloud.gme.v20180711.models.StopRecordRequest`
@@ -765,15 +765,15 @@
             model = models.StopRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateScanRooms(self, request):
         """更新自定义送检房间号
 
         :param request: Request instance for UpdateScanRooms.
         :type request: :class:`tencentcloud.gme.v20180711.models.UpdateScanRoomsRequest`
@@ -788,15 +788,15 @@
             model = models.UpdateScanRoomsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateScanUsers(self, request):
         """更新自定义送检用户号
 
         :param request: Request instance for UpdateScanUsers.
         :type request: :class:`tencentcloud.gme.v20180711.models.UpdateScanUsersRequest`
@@ -811,8 +811,8 @@
             model = models.UpdateScanUsersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-gme-3.0.937/tencentcloud/gme/v20180711/errorcodes.py` & `tencentcloud-sdk-python-gme-3.0.938/tencentcloud/gme/v20180711/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gme-3.0.937/tencentcloud/gme/v20180711/models.py` & `tencentcloud-sdk-python-gme-3.0.938/tencentcloud/gme/v20180711/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gme-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-gme-3.0.938/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gme
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Gme SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-gme-3.0.937/README.rst` & `tencentcloud-sdk-python-gme-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gme-3.0.937/tencentcloud_sdk_python_gme.egg-info/PKG-INFO` & `tencentcloud-sdk-python-gme-3.0.938/tencentcloud_sdk_python_gme.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gme
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Gme SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

