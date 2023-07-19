# Comparing `tmp/tencentcloud-sdk-python-bda-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-bda-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-bda-3.0.937.tar", last modified: Tue Jul 18 00:17:38 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-bda-3.0.938.tar", last modified: Wed Jul 19 00:21:41 2023, max compression
```

## Comparing `tencentcloud-sdk-python-bda-3.0.937.tar` & `tencentcloud-sdk-python-bda-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:38.000000 tencentcloud-sdk-python-bda-3.0.937/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:38.000000 tencentcloud-sdk-python-bda-3.0.937/tencentcloud_sdk_python_bda.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:17:38.000000 tencentcloud-sdk-python-bda-3.0.937/tencentcloud_sdk_python_bda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:17:38.000000 tencentcloud-sdk-python-bda-3.0.937/tencentcloud_sdk_python_bda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:17:38.000000 tencentcloud-sdk-python-bda-3.0.937/tencentcloud_sdk_python_bda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:17:38.000000 tencentcloud-sdk-python-bda-3.0.937/tencentcloud_sdk_python_bda.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:17:38.000000 tencentcloud-sdk-python-bda-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:38.000000 tencentcloud-sdk-python-bda-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:17:38.000000 tencentcloud-sdk-python-bda-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:38.000000 tencentcloud-sdk-python-bda-3.0.937/tencentcloud/bda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:17:38.000000 tencentcloud-sdk-python-bda-3.0.937/tencentcloud/bda/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:38.000000 tencentcloud-sdk-python-bda-3.0.937/tencentcloud/bda/v20200324/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:17:38.000000 tencentcloud-sdk-python-bda-3.0.937/tencentcloud/bda/v20200324/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8442 2023-07-18 00:17:38.000000 tencentcloud-sdk-python-bda-3.0.937/tencentcloud/bda/v20200324/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    20595 2023-07-18 00:17:38.000000 tencentcloud-sdk-python-bda-3.0.937/tencentcloud/bda/v20200324/bda_client.py
--rw-r--r--   0 root         (0) root         (0)   112857 2023-07-18 00:17:38.000000 tencentcloud-sdk-python-bda-3.0.937/tencentcloud/bda/v20200324/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:17:38.000000 tencentcloud-sdk-python-bda-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:17:38.000000 tencentcloud-sdk-python-bda-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:17:38.000000 tencentcloud-sdk-python-bda-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:41.000000 tencentcloud-sdk-python-bda-3.0.938/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:41.000000 tencentcloud-sdk-python-bda-3.0.938/tencentcloud_sdk_python_bda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:21:41.000000 tencentcloud-sdk-python-bda-3.0.938/tencentcloud_sdk_python_bda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:21:41.000000 tencentcloud-sdk-python-bda-3.0.938/tencentcloud_sdk_python_bda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:21:41.000000 tencentcloud-sdk-python-bda-3.0.938/tencentcloud_sdk_python_bda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:21:41.000000 tencentcloud-sdk-python-bda-3.0.938/tencentcloud_sdk_python_bda.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:21:41.000000 tencentcloud-sdk-python-bda-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:41.000000 tencentcloud-sdk-python-bda-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:21:41.000000 tencentcloud-sdk-python-bda-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:41.000000 tencentcloud-sdk-python-bda-3.0.938/tencentcloud/bda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:21:41.000000 tencentcloud-sdk-python-bda-3.0.938/tencentcloud/bda/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:41.000000 tencentcloud-sdk-python-bda-3.0.938/tencentcloud/bda/v20200324/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:21:41.000000 tencentcloud-sdk-python-bda-3.0.938/tencentcloud/bda/v20200324/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8442 2023-07-19 00:21:41.000000 tencentcloud-sdk-python-bda-3.0.938/tencentcloud/bda/v20200324/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    20667 2023-07-19 00:21:41.000000 tencentcloud-sdk-python-bda-3.0.938/tencentcloud/bda/v20200324/bda_client.py
+-rw-r--r--   0 root         (0) root         (0)   112857 2023-07-19 00:21:41.000000 tencentcloud-sdk-python-bda-3.0.938/tencentcloud/bda/v20200324/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:21:41.000000 tencentcloud-sdk-python-bda-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:21:41.000000 tencentcloud-sdk-python-bda-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:21:41.000000 tencentcloud-sdk-python-bda-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-bda-3.0.937/tencentcloud_sdk_python_bda.egg-info/PKG-INFO` & `tencentcloud-sdk-python-bda-3.0.938/tencentcloud_sdk_python_bda.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bda
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Bda SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bda-3.0.937/setup.py` & `tencentcloud-sdk-python-bda-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bda-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-bda-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-bda-3.0.937/tencentcloud/bda/v20200324/errorcodes.py` & `tencentcloud-sdk-python-bda-3.0.938/tencentcloud/bda/v20200324/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bda-3.0.937/tencentcloud/bda/v20200324/bda_client.py` & `tencentcloud-sdk-python-bda-3.0.938/tencentcloud/bda/v20200324/bda_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             model = models.CreateGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePerson(self, request):
         """创建人员，添加对应人员的人体动作轨迹信息。
 
         请注意：
         - 我们希望您的输入为 严格符合动作轨迹图片 要求的图片。如果您输入的图片不符合动作轨迹图片要求，会对最终效果产生较大负面影响。请您尽量保证一个Trace中的图片人体清晰、无遮挡、连贯；
@@ -78,15 +78,15 @@
             model = models.CreatePersonResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSegmentationTask(self, request):
         """本接口为人像分割在线处理接口组中的提交任务接口，可以对提交的资源进行处理视频流/图片流识别视频作品中的人像区域，进行一键抠像、背景替换、人像虚化等后期处理。
 
         :param request: Request instance for CreateSegmentationTask.
         :type request: :class:`tencentcloud.bda.v20200324.models.CreateSegmentationTaskRequest`
@@ -101,15 +101,15 @@
             model = models.CreateSegmentationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTrace(self, request):
         """将一个人体动作轨迹添加到一个人员中。一个人员最多允许包含 5 个人体动作轨迹。同一人的人体动作轨迹越多，搜索识别效果越好。
 
         >请注意：
         - 我们希望您的输入为 严格符合动作轨迹图片 要求的图片。如果您输入的图片不符合动作轨迹图片要求，会对最终效果产生较大负面影响。请您尽量保证一个Trace中的图片人体清晰、无遮挡、连贯。
@@ -131,15 +131,15 @@
             model = models.CreateTraceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteGroup(self, request):
         """删除该人体库及包含的所有的人员。
 
         :param request: Request instance for DeleteGroup.
         :type request: :class:`tencentcloud.bda.v20200324.models.DeleteGroupRequest`
@@ -154,15 +154,15 @@
             model = models.DeleteGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePerson(self, request):
         """删除人员。
 
         :param request: Request instance for DeletePerson.
         :type request: :class:`tencentcloud.bda.v20200324.models.DeletePersonRequest`
@@ -177,15 +177,15 @@
             model = models.DeletePersonResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSegmentationTask(self, request):
         """可以查看单条任务的处理情况，包括处理状态，处理结果。
 
         :param request: Request instance for DescribeSegmentationTask.
         :type request: :class:`tencentcloud.bda.v20200324.models.DescribeSegmentationTaskRequest`
@@ -200,15 +200,15 @@
             model = models.DescribeSegmentationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetectBody(self, request):
         """检测给定图片中的人体（Body）的位置信息及属性信息。
 
         :param request: Request instance for DetectBody.
         :type request: :class:`tencentcloud.bda.v20200324.models.DetectBodyRequest`
@@ -223,15 +223,15 @@
             model = models.DetectBodyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetectBodyJoints(self, request):
         """检测图片中人体的14个关键点。建议用于人体图像清晰、无遮挡的场景。支持一张图片中存在多个人体的识别。
 
         :param request: Request instance for DetectBodyJoints.
         :type request: :class:`tencentcloud.bda.v20200324.models.DetectBodyJointsRequest`
@@ -246,15 +246,15 @@
             model = models.DetectBodyJointsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetGroupList(self, request):
         """获取人体库列表。
 
         :param request: Request instance for GetGroupList.
         :type request: :class:`tencentcloud.bda.v20200324.models.GetGroupListRequest`
@@ -269,15 +269,15 @@
             model = models.GetGroupListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetPersonList(self, request):
         """获取指定人体库中的人员列表。
 
         :param request: Request instance for GetPersonList.
         :type request: :class:`tencentcloud.bda.v20200324.models.GetPersonListRequest`
@@ -292,15 +292,15 @@
             model = models.GetPersonListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetSummaryInfo(self, request):
         """获取人体库汇总信息。
 
         :param request: Request instance for GetSummaryInfo.
         :type request: :class:`tencentcloud.bda.v20200324.models.GetSummaryInfoRequest`
@@ -315,15 +315,15 @@
             model = models.GetSummaryInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyGroup(self, request):
         """修改人体库名称、备注。
 
         :param request: Request instance for ModifyGroup.
         :type request: :class:`tencentcloud.bda.v20200324.models.ModifyGroupRequest`
@@ -338,15 +338,15 @@
             model = models.ModifyGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPersonInfo(self, request):
         """修改人员信息。
 
         :param request: Request instance for ModifyPersonInfo.
         :type request: :class:`tencentcloud.bda.v20200324.models.ModifyPersonInfoRequest`
@@ -361,15 +361,15 @@
             model = models.ModifyPersonInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchTrace(self, request):
         """本接口用于对一组待识别的人体动作轨迹（Trace）图片，在人体库中识别出最相似的 TopK 人体，按照相似度从大到小排列。
 
         人体动作轨迹（Trace）图片要求：图片中当且仅包含一个人体。人体完整、无遮挡。
 
@@ -391,15 +391,15 @@
             model = models.SearchTraceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SegmentCustomizedPortraitPic(self, request):
         """在前后景分割的基础上优化多分类分割，支持对头发、五官等的分割，既作为换发型、挂件等底层技术，也可用于抠人头、抠人脸等玩法
 
         :param request: Request instance for SegmentCustomizedPortraitPic.
         :type request: :class:`tencentcloud.bda.v20200324.models.SegmentCustomizedPortraitPicRequest`
@@ -414,15 +414,15 @@
             model = models.SegmentCustomizedPortraitPicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SegmentPortraitPic(self, request):
         """即二分类人像分割，识别传入图片中人体的完整轮廓，进行抠像。
 
         :param request: Request instance for SegmentPortraitPic.
         :type request: :class:`tencentcloud.bda.v20200324.models.SegmentPortraitPicRequest`
@@ -437,15 +437,15 @@
             model = models.SegmentPortraitPicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TerminateSegmentationTask(self, request):
         """终止指定视频人像分割处理任务
 
         :param request: Request instance for TerminateSegmentationTask.
         :type request: :class:`tencentcloud.bda.v20200324.models.TerminateSegmentationTaskRequest`
@@ -460,8 +460,8 @@
             model = models.TerminateSegmentationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-bda-3.0.937/tencentcloud/bda/v20200324/models.py` & `tencentcloud-sdk-python-bda-3.0.938/tencentcloud/bda/v20200324/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bda-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-bda-3.0.938/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bda
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Bda SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bda-3.0.937/README.rst` & `tencentcloud-sdk-python-bda-3.0.938/README.rst`

 * *Files identical despite different names*

