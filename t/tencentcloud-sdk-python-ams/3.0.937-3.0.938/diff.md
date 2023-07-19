# Comparing `tmp/tencentcloud-sdk-python-ams-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-ams-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ams-3.0.937.tar", last modified: Tue Jul 18 00:16:19 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ams-3.0.938.tar", last modified: Wed Jul 19 00:20:35 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ams-3.0.937.tar` & `tencentcloud-sdk-python-ams-3.0.938.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:19.000000 tencentcloud-sdk-python-ams-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:16:19.000000 tencentcloud-sdk-python-ams-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:19.000000 tencentcloud-sdk-python-ams-3.0.937/tencentcloud_sdk_python_ams.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:16:19.000000 tencentcloud-sdk-python-ams-3.0.937/tencentcloud_sdk_python_ams.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-18 00:16:19.000000 tencentcloud-sdk-python-ams-3.0.937/tencentcloud_sdk_python_ams.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:16:19.000000 tencentcloud-sdk-python-ams-3.0.937/tencentcloud_sdk_python_ams.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:16:19.000000 tencentcloud-sdk-python-ams-3.0.937/tencentcloud_sdk_python_ams.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:19.000000 tencentcloud-sdk-python-ams-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:16:19.000000 tencentcloud-sdk-python-ams-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:19.000000 tencentcloud-sdk-python-ams-3.0.937/tencentcloud/ams/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:19.000000 tencentcloud-sdk-python-ams-3.0.937/tencentcloud/ams/v20200608/
--rw-r--r--   0 root         (0) root         (0)     9132 2023-07-18 00:16:19.000000 tencentcloud-sdk-python-ams-3.0.937/tencentcloud/ams/v20200608/ams_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:16:19.000000 tencentcloud-sdk-python-ams-3.0.937/tencentcloud/ams/v20200608/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-07-18 00:16:19.000000 tencentcloud-sdk-python-ams-3.0.937/tencentcloud/ams/v20200608/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    89744 2023-07-18 00:16:19.000000 tencentcloud-sdk-python-ams-3.0.937/tencentcloud/ams/v20200608/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:19.000000 tencentcloud-sdk-python-ams-3.0.937/tencentcloud/ams/v20201229/
--rw-r--r--   0 root         (0) root         (0)    10418 2023-07-18 00:16:19.000000 tencentcloud-sdk-python-ams-3.0.937/tencentcloud/ams/v20201229/ams_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:16:19.000000 tencentcloud-sdk-python-ams-3.0.937/tencentcloud/ams/v20201229/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3347 2023-07-18 00:16:19.000000 tencentcloud-sdk-python-ams-3.0.937/tencentcloud/ams/v20201229/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    93055 2023-07-18 00:16:19.000000 tencentcloud-sdk-python-ams-3.0.937/tencentcloud/ams/v20201229/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:16:19.000000 tencentcloud-sdk-python-ams-3.0.937/tencentcloud/ams/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:16:19.000000 tencentcloud-sdk-python-ams-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:16:19.000000 tencentcloud-sdk-python-ams-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:16:19.000000 tencentcloud-sdk-python-ams-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:35.000000 tencentcloud-sdk-python-ams-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:20:35.000000 tencentcloud-sdk-python-ams-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:35.000000 tencentcloud-sdk-python-ams-3.0.938/tencentcloud_sdk_python_ams.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:20:35.000000 tencentcloud-sdk-python-ams-3.0.938/tencentcloud_sdk_python_ams.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-19 00:20:35.000000 tencentcloud-sdk-python-ams-3.0.938/tencentcloud_sdk_python_ams.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:20:35.000000 tencentcloud-sdk-python-ams-3.0.938/tencentcloud_sdk_python_ams.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:20:35.000000 tencentcloud-sdk-python-ams-3.0.938/tencentcloud_sdk_python_ams.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:35.000000 tencentcloud-sdk-python-ams-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:20:35.000000 tencentcloud-sdk-python-ams-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:35.000000 tencentcloud-sdk-python-ams-3.0.938/tencentcloud/ams/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:35.000000 tencentcloud-sdk-python-ams-3.0.938/tencentcloud/ams/v20200608/
+-rw-r--r--   0 root         (0) root         (0)     9160 2023-07-19 00:20:35.000000 tencentcloud-sdk-python-ams-3.0.938/tencentcloud/ams/v20200608/ams_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:20:35.000000 tencentcloud-sdk-python-ams-3.0.938/tencentcloud/ams/v20200608/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-07-19 00:20:35.000000 tencentcloud-sdk-python-ams-3.0.938/tencentcloud/ams/v20200608/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    89744 2023-07-19 00:20:35.000000 tencentcloud-sdk-python-ams-3.0.938/tencentcloud/ams/v20200608/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:35.000000 tencentcloud-sdk-python-ams-3.0.938/tencentcloud/ams/v20201229/
+-rw-r--r--   0 root         (0) root         (0)    10438 2023-07-19 00:20:35.000000 tencentcloud-sdk-python-ams-3.0.938/tencentcloud/ams/v20201229/ams_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:20:35.000000 tencentcloud-sdk-python-ams-3.0.938/tencentcloud/ams/v20201229/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3347 2023-07-19 00:20:35.000000 tencentcloud-sdk-python-ams-3.0.938/tencentcloud/ams/v20201229/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    93055 2023-07-19 00:20:35.000000 tencentcloud-sdk-python-ams-3.0.938/tencentcloud/ams/v20201229/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:20:35.000000 tencentcloud-sdk-python-ams-3.0.938/tencentcloud/ams/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:20:35.000000 tencentcloud-sdk-python-ams-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:20:35.000000 tencentcloud-sdk-python-ams-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:20:35.000000 tencentcloud-sdk-python-ams-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-ams-3.0.937/setup.py` & `tencentcloud-sdk-python-ams-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ams-3.0.937/tencentcloud_sdk_python_ams.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-ams-3.0.938/tencentcloud_sdk_python_ams.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ams-3.0.937/tencentcloud_sdk_python_ams.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ams-3.0.938/tencentcloud_sdk_python_ams.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ams
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ams SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ams-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ams-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ams-3.0.937/tencentcloud/ams/v20200608/ams_client.py` & `tencentcloud-sdk-python-ams-3.0.938/tencentcloud/ams/v20200608/ams_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CancelTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAudioModerationTask(self, request):
         """本接口（Audio Moderation）用于提交音频内容（包括音频文件或流地址）进行智能审核任务，使用前请您登陆控制台开通音频内容安全服务。
 
         ### 功能使用说明：
         - 前往“内容安全控制台-音频内容安全”开启使用音频内容安全服务，首次开通可获得20小时免费调用时长
@@ -88,15 +88,15 @@
             model = models.CreateAudioModerationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateBizConfig(self, request):
         """创建业务配置，1个账号最多可以创建20个配置，可定义音频审核的场景，如色情、谩骂等，
 
         在创建业务配置之前，你需要以下步骤：
         1. 开通COS存储桶功能，新建存储桶，例如 cms_segments，用来存储 视频转换过程中生成对音频和图片。
@@ -115,15 +115,15 @@
             model = models.CreateBizConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAmsList(self, request):
         """音频审核明细列表
 
         :param request: Request instance for DescribeAmsList.
         :type request: :class:`tencentcloud.ams.v20200608.models.DescribeAmsListRequest`
@@ -138,15 +138,15 @@
             model = models.DescribeAmsListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAudioStat(self, request):
         """控制台识别统计
 
         :param request: Request instance for DescribeAudioStat.
         :type request: :class:`tencentcloud.ams.v20200608.models.DescribeAudioStatRequest`
@@ -161,15 +161,15 @@
             model = models.DescribeAudioStatResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBizConfig(self, request):
         """查看单个配置
 
         :param request: Request instance for DescribeBizConfig.
         :type request: :class:`tencentcloud.ams.v20200608.models.DescribeBizConfigRequest`
@@ -184,15 +184,15 @@
             model = models.DescribeBizConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskDetail(self, request):
         """查看任务详情
 
         :param request: Request instance for DescribeTaskDetail.
         :type request: :class:`tencentcloud.ams.v20200608.models.DescribeTaskDetailRequest`
@@ -207,8 +207,8 @@
             model = models.DescribeTaskDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-ams-3.0.937/tencentcloud/ams/v20200608/errorcodes.py` & `tencentcloud-sdk-python-ams-3.0.938/tencentcloud/ams/v20200608/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ams-3.0.937/tencentcloud/ams/v20200608/models.py` & `tencentcloud-sdk-python-ams-3.0.938/tencentcloud/ams/v20200608/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ams-3.0.937/tencentcloud/ams/v20201229/ams_client.py` & `tencentcloud-sdk-python-ams-3.0.938/tencentcloud/ams/v20201229/ams_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CancelTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAudioModerationSyncTask(self, request):
         """本接口（CreateAudioModerationSyncTask） 用于提交短音频内容进行智能审核任务，使用前请您使用腾讯云主账号登录控制台 [开通音频内容安全服务](https://console.cloud.tencent.com/cms/audio/package) 并调整好对应的业务配置。
 
         ### 接口使用说明：
         - 前往“[内容安全控制台-图片内容安全](https://console.cloud.tencent.com/cms/audio/package)”开启使用音频内容安全服务，首次开通服务的用户可免费领用试用套餐包，包含**10小时**免费调用时长，有效期为1个月。
@@ -77,15 +77,15 @@
             model = models.CreateAudioModerationSyncTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAudioModerationTask(self, request):
         """本接口（Audio Moderation）用于提交音频内容（包括音频文件或流地址）进行智能审核任务，使用前请您使用腾讯云主账号登录控制台[开通音频内容安全服务](https://console.cloud.tencent.com/cms/audio/package)并调整好对应的业务配置。<br>
 
         ### 功能使用说明：
         - 前往“[内容安全控制台-音频内容安全](https://console.cloud.tencent.com/cms/audio/package)”开启使用音频内容安全服务，首次开通可获得**10小时**免费调用时长，有效期为1个月。
@@ -131,15 +131,15 @@
             model = models.CreateAudioModerationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskDetail(self, request):
         """通过该接口可查看音频审核任务的详情信息，包括任务状态、检测结果、音频文件识别出的对应文本内容、检测结果所对应的恶意标签及推荐的后续操作等，具体输出内容可查看输出参数示例。<br>默认接口请求频率限制：**100次/秒**。
 
         :param request: Request instance for DescribeTaskDetail.
         :type request: :class:`tencentcloud.ams.v20201229.models.DescribeTaskDetailRequest`
@@ -154,15 +154,15 @@
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
         """通过该接口可查看审核任务列表；您也可根据多种业务信息（业务类型、审核结果、任务状态等）筛选审核任务列表。任务列表输出内容包括当前查询的任务总量、任务名称、任务状态、音频审核类型、基于检测结果的恶意标签及其后续操作等，具体输出内容可查看输出参数示例。<br>默认接口请求频率限制：**20次/秒**。
 
         :param request: Request instance for DescribeTasks.
         :type request: :class:`tencentcloud.ams.v20201229.models.DescribeTasksRequest`
@@ -177,8 +177,8 @@
             model = models.DescribeTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-ams-3.0.937/tencentcloud/ams/v20201229/errorcodes.py` & `tencentcloud-sdk-python-ams-3.0.938/tencentcloud/ams/v20201229/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ams-3.0.937/tencentcloud/ams/v20201229/models.py` & `tencentcloud-sdk-python-ams-3.0.938/tencentcloud/ams/v20201229/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ams-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-ams-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ams
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ams SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ams-3.0.937/README.rst` & `tencentcloud-sdk-python-ams-3.0.938/README.rst`

 * *Files identical despite different names*

