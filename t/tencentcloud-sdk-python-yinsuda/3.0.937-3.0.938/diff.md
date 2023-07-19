# Comparing `tmp/tencentcloud-sdk-python-yinsuda-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-yinsuda-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-yinsuda-3.0.937.tar", last modified: Tue Jul 18 00:35:47 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-yinsuda-3.0.938.tar", last modified: Wed Jul 19 00:54:16 2023, max compression
```

## Comparing `tencentcloud-sdk-python-yinsuda-3.0.937.tar` & `tencentcloud-sdk-python-yinsuda-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:47.000000 tencentcloud-sdk-python-yinsuda-3.0.937/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:47.000000 tencentcloud-sdk-python-yinsuda-3.0.937/tencentcloud_sdk_python_yinsuda.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:35:47.000000 tencentcloud-sdk-python-yinsuda-3.0.937/tencentcloud_sdk_python_yinsuda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-18 00:35:47.000000 tencentcloud-sdk-python-yinsuda-3.0.937/tencentcloud_sdk_python_yinsuda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:35:47.000000 tencentcloud-sdk-python-yinsuda-3.0.937/tencentcloud_sdk_python_yinsuda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:35:47.000000 tencentcloud-sdk-python-yinsuda-3.0.937/tencentcloud_sdk_python_yinsuda.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-18 00:35:47.000000 tencentcloud-sdk-python-yinsuda-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:47.000000 tencentcloud-sdk-python-yinsuda-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:47.000000 tencentcloud-sdk-python-yinsuda-3.0.937/tencentcloud/yinsuda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:35:47.000000 tencentcloud-sdk-python-yinsuda-3.0.937/tencentcloud/yinsuda/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:47.000000 tencentcloud-sdk-python-yinsuda-3.0.937/tencentcloud/yinsuda/v20220527/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:35:47.000000 tencentcloud-sdk-python-yinsuda-3.0.937/tencentcloud/yinsuda/v20220527/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-07-18 00:35:47.000000 tencentcloud-sdk-python-yinsuda-3.0.937/tencentcloud/yinsuda/v20220527/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    16900 2023-07-18 00:35:47.000000 tencentcloud-sdk-python-yinsuda-3.0.937/tencentcloud/yinsuda/v20220527/yinsuda_client.py
--rw-r--r--   0 root         (0) root         (0)   119018 2023-07-18 00:35:47.000000 tencentcloud-sdk-python-yinsuda-3.0.937/tencentcloud/yinsuda/v20220527/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:35:47.000000 tencentcloud-sdk-python-yinsuda-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:35:47.000000 tencentcloud-sdk-python-yinsuda-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:35:47.000000 tencentcloud-sdk-python-yinsuda-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-18 00:35:47.000000 tencentcloud-sdk-python-yinsuda-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:54:16.000000 tencentcloud-sdk-python-yinsuda-3.0.938/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:54:16.000000 tencentcloud-sdk-python-yinsuda-3.0.938/tencentcloud_sdk_python_yinsuda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:54:16.000000 tencentcloud-sdk-python-yinsuda-3.0.938/tencentcloud_sdk_python_yinsuda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-19 00:54:16.000000 tencentcloud-sdk-python-yinsuda-3.0.938/tencentcloud_sdk_python_yinsuda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:54:16.000000 tencentcloud-sdk-python-yinsuda-3.0.938/tencentcloud_sdk_python_yinsuda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:54:16.000000 tencentcloud-sdk-python-yinsuda-3.0.938/tencentcloud_sdk_python_yinsuda.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-19 00:54:16.000000 tencentcloud-sdk-python-yinsuda-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:54:16.000000 tencentcloud-sdk-python-yinsuda-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:54:16.000000 tencentcloud-sdk-python-yinsuda-3.0.938/tencentcloud/yinsuda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:54:16.000000 tencentcloud-sdk-python-yinsuda-3.0.938/tencentcloud/yinsuda/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:54:16.000000 tencentcloud-sdk-python-yinsuda-3.0.938/tencentcloud/yinsuda/v20220527/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:54:16.000000 tencentcloud-sdk-python-yinsuda-3.0.938/tencentcloud/yinsuda/v20220527/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-07-19 00:54:16.000000 tencentcloud-sdk-python-yinsuda-3.0.938/tencentcloud/yinsuda/v20220527/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    16968 2023-07-19 00:54:16.000000 tencentcloud-sdk-python-yinsuda-3.0.938/tencentcloud/yinsuda/v20220527/yinsuda_client.py
+-rw-r--r--   0 root         (0) root         (0)   119018 2023-07-19 00:54:16.000000 tencentcloud-sdk-python-yinsuda-3.0.938/tencentcloud/yinsuda/v20220527/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:54:16.000000 tencentcloud-sdk-python-yinsuda-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:54:16.000000 tencentcloud-sdk-python-yinsuda-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:54:16.000000 tencentcloud-sdk-python-yinsuda-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-19 00:54:16.000000 tencentcloud-sdk-python-yinsuda-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.937/tencentcloud_sdk_python_yinsuda.egg-info/PKG-INFO` & `tencentcloud-sdk-python-yinsuda-3.0.938/tencentcloud_sdk_python_yinsuda.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-yinsuda
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Yinsuda SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.937/setup.py` & `tencentcloud-sdk-python-yinsuda-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.937/tencentcloud/yinsuda/v20220527/errorcodes.py` & `tencentcloud-sdk-python-yinsuda-3.0.938/tencentcloud/yinsuda/v20220527/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.937/tencentcloud/yinsuda/v20220527/yinsuda_client.py` & `tencentcloud-sdk-python-yinsuda-3.0.938/tencentcloud/yinsuda/v20220527/yinsuda_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.ApplyChorusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchDescribeKTVMusicDetails(self, request):
         """批量获取歌曲详细信息，包括：歌词下载链接、播放凭证、音高数据下载链接信息等。
 
         :param request: Request instance for BatchDescribeKTVMusicDetails.
         :type request: :class:`tencentcloud.yinsuda.v20220527.models.BatchDescribeKTVMusicDetailsRequest`
@@ -65,15 +65,15 @@
             model = models.BatchDescribeKTVMusicDetailsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateKTVRobot(self, request):
         """创建机器人，支持进入 RTC 房间，播放曲库歌曲。
 
         :param request: Request instance for CreateKTVRobot.
         :type request: :class:`tencentcloud.yinsuda.v20220527.models.CreateKTVRobotRequest`
@@ -88,15 +88,15 @@
             model = models.CreateKTVRobotResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKTVMatchMusics(self, request):
         """根据输入的规则匹配曲库中的歌曲。
 
         :param request: Request instance for DescribeKTVMatchMusics.
         :type request: :class:`tencentcloud.yinsuda.v20220527.models.DescribeKTVMatchMusicsRequest`
@@ -111,15 +111,15 @@
             model = models.DescribeKTVMatchMusicsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKTVMusicAccompanySegmentUrl(self, request):
         """获取歌曲伴奏片段链接，可用于抢唱
 
         :param request: Request instance for DescribeKTVMusicAccompanySegmentUrl.
         :type request: :class:`tencentcloud.yinsuda.v20220527.models.DescribeKTVMusicAccompanySegmentUrlRequest`
@@ -134,15 +134,15 @@
             model = models.DescribeKTVMusicAccompanySegmentUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKTVMusicsByTag(self, request):
         """通过标签过滤歌曲列表。
 
         :param request: Request instance for DescribeKTVMusicsByTag.
         :type request: :class:`tencentcloud.yinsuda.v20220527.models.DescribeKTVMusicsByTagRequest`
@@ -157,15 +157,15 @@
             model = models.DescribeKTVMusicsByTagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKTVPlaylistDetail(self, request):
         """根据歌单 Id 获取歌单详情。
 
         :param request: Request instance for DescribeKTVPlaylistDetail.
         :type request: :class:`tencentcloud.yinsuda.v20220527.models.DescribeKTVPlaylistDetailRequest`
@@ -180,15 +180,15 @@
             model = models.DescribeKTVPlaylistDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKTVPlaylists(self, request):
         """获取歌单列表。
 
         :param request: Request instance for DescribeKTVPlaylists.
         :type request: :class:`tencentcloud.yinsuda.v20220527.models.DescribeKTVPlaylistsRequest`
@@ -203,15 +203,15 @@
             model = models.DescribeKTVPlaylistsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKTVRobots(self, request):
         """获取机器人列表，支持 Id、状态等过滤条件。
 
         :param request: Request instance for DescribeKTVRobots.
         :type request: :class:`tencentcloud.yinsuda.v20220527.models.DescribeKTVRobotsRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeKTVRobotsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKTVSuggestions(self, request):
         """根据关键词获取联想词列表。
 
         :param request: Request instance for DescribeKTVSuggestions.
         :type request: :class:`tencentcloud.yinsuda.v20220527.models.DescribeKTVSuggestionsRequest`
@@ -249,15 +249,15 @@
             model = models.DescribeKTVSuggestionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKTVTags(self, request):
         """获取标签分组及分组下的标签列表信息。
 
         :param request: Request instance for DescribeKTVTags.
         :type request: :class:`tencentcloud.yinsuda.v20220527.models.DescribeKTVTagsRequest`
@@ -272,15 +272,15 @@
             model = models.DescribeKTVTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveVipTradeInfos(self, request):
         """批量获取直播会员充值流水详细信息，包括：流水号，订单状态，下订单时间等
 
         :param request: Request instance for DescribeLiveVipTradeInfos.
         :type request: :class:`tencentcloud.yinsuda.v20220527.models.DescribeLiveVipTradeInfosRequest`
@@ -295,15 +295,15 @@
             model = models.DescribeLiveVipTradeInfosResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserInfo(self, request):
         """获取用户信息，包括是否为直播会员，及直播会员信息等
 
         :param request: Request instance for DescribeUserInfo.
         :type request: :class:`tencentcloud.yinsuda.v20220527.models.DescribeUserInfoRequest`
@@ -318,15 +318,15 @@
             model = models.DescribeUserInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DestroyKTVRobot(self, request):
         """销毁机器人，机器人退出 RTC 房间。
 
         :param request: Request instance for DestroyKTVRobot.
         :type request: :class:`tencentcloud.yinsuda.v20220527.models.DestroyKTVRobotRequest`
@@ -341,15 +341,15 @@
             model = models.DestroyKTVRobotResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RechargeLiveVip(self, request):
         """充值直播会员，使该用户可以在直播场景使用
 
         :param request: Request instance for RechargeLiveVip.
         :type request: :class:`tencentcloud.yinsuda.v20220527.models.RechargeLiveVipRequest`
@@ -364,15 +364,15 @@
             model = models.RechargeLiveVipResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchKTVMusics(self, request):
         """根据关键词搜索歌曲，返回相关歌曲列表。
 
         :param request: Request instance for SearchKTVMusics.
         :type request: :class:`tencentcloud.yinsuda.v20220527.models.SearchKTVMusicsRequest`
@@ -387,15 +387,15 @@
             model = models.SearchKTVMusicsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SyncKTVRobotCommand(self, request):
         """下发操作机器人指令，支持播放、暂停、恢复、歌单设置等操作指令，实现对机器人行为的控制。
 
         :param request: Request instance for SyncKTVRobotCommand.
         :type request: :class:`tencentcloud.yinsuda.v20220527.models.SyncKTVRobotCommandRequest`
@@ -410,8 +410,8 @@
             model = models.SyncKTVRobotCommandResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.937/tencentcloud/yinsuda/v20220527/models.py` & `tencentcloud-sdk-python-yinsuda-3.0.938/tencentcloud/yinsuda/v20220527/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-yinsuda-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-yinsuda-3.0.938/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-yinsuda
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Yinsuda SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.937/README.rst` & `tencentcloud-sdk-python-yinsuda-3.0.938/README.rst`

 * *Files identical despite different names*

