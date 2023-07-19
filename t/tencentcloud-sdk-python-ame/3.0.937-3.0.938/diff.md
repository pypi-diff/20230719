# Comparing `tmp/tencentcloud-sdk-python-ame-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-ame-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ame-3.0.937.tar", last modified: Tue Jul 18 00:16:12 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ame-3.0.938.tar", last modified: Wed Jul 19 00:20:29 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ame-3.0.937.tar` & `tencentcloud-sdk-python-ame-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:12.000000 tencentcloud-sdk-python-ame-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:16:11.000000 tencentcloud-sdk-python-ame-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:12.000000 tencentcloud-sdk-python-ame-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:16:11.000000 tencentcloud-sdk-python-ame-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:12.000000 tencentcloud-sdk-python-ame-3.0.937/tencentcloud/ame/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:16:11.000000 tencentcloud-sdk-python-ame-3.0.937/tencentcloud/ame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:12.000000 tencentcloud-sdk-python-ame-3.0.937/tencentcloud/ame/v20190916/
--rw-r--r--   0 root         (0) root         (0)    29455 2023-07-18 00:16:11.000000 tencentcloud-sdk-python-ame-3.0.937/tencentcloud/ame/v20190916/ame_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:16:11.000000 tencentcloud-sdk-python-ame-3.0.937/tencentcloud/ame/v20190916/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-07-18 00:16:11.000000 tencentcloud-sdk-python-ame-3.0.937/tencentcloud/ame/v20190916/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   193152 2023-07-18 00:16:12.000000 tencentcloud-sdk-python-ame-3.0.937/tencentcloud/ame/v20190916/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:16:12.000000 tencentcloud-sdk-python-ame-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:16:12.000000 tencentcloud-sdk-python-ame-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:16:11.000000 tencentcloud-sdk-python-ame-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:12.000000 tencentcloud-sdk-python-ame-3.0.937/tencentcloud_sdk_python_ame.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:16:12.000000 tencentcloud-sdk-python-ame-3.0.937/tencentcloud_sdk_python_ame.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:16:12.000000 tencentcloud-sdk-python-ame-3.0.937/tencentcloud_sdk_python_ame.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:16:12.000000 tencentcloud-sdk-python-ame-3.0.937/tencentcloud_sdk_python_ame.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:16:12.000000 tencentcloud-sdk-python-ame-3.0.937/tencentcloud_sdk_python_ame.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:29.000000 tencentcloud-sdk-python-ame-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:20:29.000000 tencentcloud-sdk-python-ame-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:29.000000 tencentcloud-sdk-python-ame-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:20:29.000000 tencentcloud-sdk-python-ame-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:29.000000 tencentcloud-sdk-python-ame-3.0.938/tencentcloud/ame/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:20:29.000000 tencentcloud-sdk-python-ame-3.0.938/tencentcloud/ame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:29.000000 tencentcloud-sdk-python-ame-3.0.938/tencentcloud/ame/v20190916/
+-rw-r--r--   0 root         (0) root         (0)    29579 2023-07-19 00:20:29.000000 tencentcloud-sdk-python-ame-3.0.938/tencentcloud/ame/v20190916/ame_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:20:29.000000 tencentcloud-sdk-python-ame-3.0.938/tencentcloud/ame/v20190916/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-07-19 00:20:29.000000 tencentcloud-sdk-python-ame-3.0.938/tencentcloud/ame/v20190916/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   193152 2023-07-19 00:20:29.000000 tencentcloud-sdk-python-ame-3.0.938/tencentcloud/ame/v20190916/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:20:29.000000 tencentcloud-sdk-python-ame-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:20:29.000000 tencentcloud-sdk-python-ame-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:20:29.000000 tencentcloud-sdk-python-ame-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:29.000000 tencentcloud-sdk-python-ame-3.0.938/tencentcloud_sdk_python_ame.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:20:29.000000 tencentcloud-sdk-python-ame-3.0.938/tencentcloud_sdk_python_ame.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:20:29.000000 tencentcloud-sdk-python-ame-3.0.938/tencentcloud_sdk_python_ame.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:20:29.000000 tencentcloud-sdk-python-ame-3.0.938/tencentcloud_sdk_python_ame.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:20:29.000000 tencentcloud-sdk-python-ame-3.0.938/tencentcloud_sdk_python_ame.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-ame-3.0.937/setup.py` & `tencentcloud-sdk-python-ame-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ame-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ame-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ame-3.0.937/tencentcloud/ame/v20190916/ame_client.py` & `tencentcloud-sdk-python-ame-3.0.938/tencentcloud/ame/v20190916/ame_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
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
         """创建机器人，支持进入 RTC 房间，播放直播互动曲库歌曲。
 
         :param request: Request instance for CreateKTVRobot.
         :type request: :class:`tencentcloud.ame.v20190916.models.CreateKTVRobotRequest`
@@ -65,15 +65,15 @@
             model = models.CreateKTVRobotResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAuthInfo(self, request):
         """获取授权项目信息列表
 
         :param request: Request instance for DescribeAuthInfo.
         :type request: :class:`tencentcloud.ame.v20190916.models.DescribeAuthInfoRequest`
@@ -88,15 +88,15 @@
             model = models.DescribeAuthInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudMusic(self, request):
         """获取云音乐播放信息接口
 
         :param request: Request instance for DescribeCloudMusic.
         :type request: :class:`tencentcloud.ame.v20190916.models.DescribeCloudMusicRequest`
@@ -111,15 +111,15 @@
             model = models.DescribeCloudMusicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudMusicPurchased(self, request):
         """获取授权项目下已购云音乐列表
 
         :param request: Request instance for DescribeCloudMusicPurchased.
         :type request: :class:`tencentcloud.ame.v20190916.models.DescribeCloudMusicPurchasedRequest`
@@ -134,15 +134,15 @@
             model = models.DescribeCloudMusicPurchasedResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeItemById(self, request):
         """根据歌曲ID查询歌曲信息
 
         :param request: Request instance for DescribeItemById.
         :type request: :class:`tencentcloud.ame.v20190916.models.DescribeItemByIdRequest`
@@ -157,15 +157,15 @@
             model = models.DescribeItemByIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeItems(self, request):
         """该服务后续会停用，不再建议使用
 
         :param request: Request instance for DescribeItems.
         :type request: :class:`tencentcloud.ame.v20190916.models.DescribeItemsRequest`
@@ -180,15 +180,15 @@
             model = models.DescribeItemsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKTVMusicDetail(self, request):
         """根据 Id 查询歌曲的详细信息，包含基础信息及播放信息。
 
         :param request: Request instance for DescribeKTVMusicDetail.
         :type request: :class:`tencentcloud.ame.v20190916.models.DescribeKTVMusicDetailRequest`
@@ -203,15 +203,15 @@
             model = models.DescribeKTVMusicDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKTVMusicTags(self, request):
         """获取直播互动曲库标签分组信息和标签信息
 
         :param request: Request instance for DescribeKTVMusicTags.
         :type request: :class:`tencentcloud.ame.v20190916.models.DescribeKTVMusicTagsRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeKTVMusicTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKTVPlaylistDetail(self, request):
         """根据歌单 Id 获取歌单详情，包括歌单的基础信息以及歌曲列表。
 
         :param request: Request instance for DescribeKTVPlaylistDetail.
         :type request: :class:`tencentcloud.ame.v20190916.models.DescribeKTVPlaylistDetailRequest`
@@ -249,15 +249,15 @@
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
         """获取直播互动曲库推荐歌单列表。
 
         :param request: Request instance for DescribeKTVPlaylists.
         :type request: :class:`tencentcloud.ame.v20190916.models.DescribeKTVPlaylistsRequest`
@@ -272,15 +272,15 @@
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
         :type request: :class:`tencentcloud.ame.v20190916.models.DescribeKTVRobotsRequest`
@@ -295,15 +295,15 @@
             model = models.DescribeKTVRobotsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKTVSingerCategories(self, request):
         """获取直播互动曲库歌手分类信息
 
         :param request: Request instance for DescribeKTVSingerCategories.
         :type request: :class:`tencentcloud.ame.v20190916.models.DescribeKTVSingerCategoriesRequest`
@@ -318,15 +318,15 @@
             model = models.DescribeKTVSingerCategoriesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKTVSingerMusics(self, request):
         """根据歌手id，返回该歌手下歌曲列表。
 
 
 
@@ -343,15 +343,15 @@
             model = models.DescribeKTVSingerMusicsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKTVSingers(self, request):
         """根据过滤条件，返回匹配的歌手列表。
 
         :param request: Request instance for DescribeKTVSingers.
         :type request: :class:`tencentcloud.ame.v20190916.models.DescribeKTVSingersRequest`
@@ -366,15 +366,15 @@
             model = models.DescribeKTVSingersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKTVSuggestions(self, request):
         """获取直播互动曲库联想词
 
         :param request: Request instance for DescribeKTVSuggestions.
         :type request: :class:`tencentcloud.ame.v20190916.models.DescribeKTVSuggestionsRequest`
@@ -389,15 +389,15 @@
             model = models.DescribeKTVSuggestionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKTVTopList(self, request):
         """获取直播互动曲库歌曲的周榜和月榜
 
         :param request: Request instance for DescribeKTVTopList.
         :type request: :class:`tencentcloud.ame.v20190916.models.DescribeKTVTopListRequest`
@@ -412,15 +412,15 @@
             model = models.DescribeKTVTopListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLyric(self, request):
         """根据接口的模式及歌曲ID来取得歌词信息或者波形图信息。
 
         :param request: Request instance for DescribeLyric.
         :type request: :class:`tencentcloud.ame.v20190916.models.DescribeLyricRequest`
@@ -435,15 +435,15 @@
             model = models.DescribeLyricResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMusic(self, request):
         """获取曲库包歌曲播放信息接口
 
         :param request: Request instance for DescribeMusic.
         :type request: :class:`tencentcloud.ame.v20190916.models.DescribeMusicRequest`
@@ -458,15 +458,15 @@
             model = models.DescribeMusicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMusicSaleStatus(self, request):
         """根据音乐信息查询音乐是否在售
 
         :param request: Request instance for DescribeMusicSaleStatus.
         :type request: :class:`tencentcloud.ame.v20190916.models.DescribeMusicSaleStatusRequest`
@@ -481,15 +481,15 @@
             model = models.DescribeMusicSaleStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePackageItems(self, request):
         """获取曲库包下已核销歌曲列表接口
 
         :param request: Request instance for DescribePackageItems.
         :type request: :class:`tencentcloud.ame.v20190916.models.DescribePackageItemsRequest`
@@ -504,15 +504,15 @@
             model = models.DescribePackageItemsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePackages(self, request):
         """获取已购曲库包列表接口
 
         :param request: Request instance for DescribePackages.
         :type request: :class:`tencentcloud.ame.v20190916.models.DescribePackagesRequest`
@@ -527,15 +527,15 @@
             model = models.DescribePackagesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePkgOfflineMusic(self, request):
         """根据购买曲库包用户可查询已回退的歌曲信息
 
         :param request: Request instance for DescribePkgOfflineMusic.
         :type request: :class:`tencentcloud.ame.v20190916.models.DescribePkgOfflineMusicRequest`
@@ -550,15 +550,15 @@
             model = models.DescribePkgOfflineMusicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStations(self, request):
         """该服务后续会停用，不再建议使用
 
         :param request: Request instance for DescribeStations.
         :type request: :class:`tencentcloud.ame.v20190916.models.DescribeStationsRequest`
@@ -573,15 +573,15 @@
             model = models.DescribeStationsResponse()
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
         :type request: :class:`tencentcloud.ame.v20190916.models.DestroyKTVRobotRequest`
@@ -596,15 +596,15 @@
             model = models.DestroyKTVRobotResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyMusicOnShelves(self, request):
         """根据资源方，需要变更的参数，请求该接口进行变更，为空的参数默认为无变更
 
         :param request: Request instance for ModifyMusicOnShelves.
         :type request: :class:`tencentcloud.ame.v20190916.models.ModifyMusicOnShelvesRequest`
@@ -619,15 +619,15 @@
             model = models.ModifyMusicOnShelvesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PutMusicOnTheShelves(self, request):
         """根据资源方所传歌曲信息，进行歌曲上架，多个歌曲同时请求时，需构造复合结构进行请求
 
         :param request: Request instance for PutMusicOnTheShelves.
         :type request: :class:`tencentcloud.ame.v20190916.models.PutMusicOnTheShelvesRequest`
@@ -642,15 +642,15 @@
             model = models.PutMusicOnTheShelvesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReportData(self, request):
         """客户上报用户数据功能，为了更好地为用户提供优质服务
 
         :param request: Request instance for ReportData.
         :type request: :class:`tencentcloud.ame.v20190916.models.ReportDataRequest`
@@ -665,15 +665,15 @@
             model = models.ReportDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchKTVMusics(self, request):
         """根据搜索条件，返回匹配的歌曲列表。
 
         :param request: Request instance for SearchKTVMusics.
         :type request: :class:`tencentcloud.ame.v20190916.models.SearchKTVMusicsRequest`
@@ -688,15 +688,15 @@
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
         :type request: :class:`tencentcloud.ame.v20190916.models.SyncKTVRobotCommandRequest`
@@ -711,15 +711,15 @@
             model = models.SyncKTVRobotCommandResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TakeMusicOffShelves(self, request):
         """根据资源方所传MusicId进行将歌曲进行下架，多个MusicId使用逗号隔开
 
         :param request: Request instance for TakeMusicOffShelves.
         :type request: :class:`tencentcloud.ame.v20190916.models.TakeMusicOffShelvesRequest`
@@ -734,8 +734,8 @@
             model = models.TakeMusicOffShelvesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-ame-3.0.937/tencentcloud/ame/v20190916/errorcodes.py` & `tencentcloud-sdk-python-ame-3.0.938/tencentcloud/ame/v20190916/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ame-3.0.937/tencentcloud/ame/v20190916/models.py` & `tencentcloud-sdk-python-ame-3.0.938/tencentcloud/ame/v20190916/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ame-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-ame-3.0.938/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ame
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ame SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ame-3.0.937/README.rst` & `tencentcloud-sdk-python-ame-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ame-3.0.937/tencentcloud_sdk_python_ame.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ame-3.0.938/tencentcloud_sdk_python_ame.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ame
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ame SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

