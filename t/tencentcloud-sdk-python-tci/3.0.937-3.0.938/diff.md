# Comparing `tmp/tencentcloud-sdk-python-tci-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tci-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tci-3.0.937.tar", last modified: Tue Jul 18 00:31:40 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tci-3.0.938.tar", last modified: Wed Jul 19 00:49:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tci-3.0.937.tar` & `tencentcloud-sdk-python-tci-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:40.000000 tencentcloud-sdk-python-tci-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:31:40.000000 tencentcloud-sdk-python-tci-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:40.000000 tencentcloud-sdk-python-tci-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:31:40.000000 tencentcloud-sdk-python-tci-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:40.000000 tencentcloud-sdk-python-tci-3.0.937/tencentcloud/tci/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:40.000000 tencentcloud-sdk-python-tci-3.0.937/tencentcloud/tci/v20190318/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:31:40.000000 tencentcloud-sdk-python-tci-3.0.937/tencentcloud/tci/v20190318/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44023 2023-07-18 00:31:40.000000 tencentcloud-sdk-python-tci-3.0.937/tencentcloud/tci/v20190318/tci_client.py
--rw-r--r--   0 root         (0) root         (0)     8913 2023-07-18 00:31:40.000000 tencentcloud-sdk-python-tci-3.0.937/tencentcloud/tci/v20190318/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   285108 2023-07-18 00:31:40.000000 tencentcloud-sdk-python-tci-3.0.937/tencentcloud/tci/v20190318/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:31:40.000000 tencentcloud-sdk-python-tci-3.0.937/tencentcloud/tci/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:31:40.000000 tencentcloud-sdk-python-tci-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:40.000000 tencentcloud-sdk-python-tci-3.0.937/tencentcloud_sdk_python_tci.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:31:40.000000 tencentcloud-sdk-python-tci-3.0.937/tencentcloud_sdk_python_tci.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:31:40.000000 tencentcloud-sdk-python-tci-3.0.937/tencentcloud_sdk_python_tci.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:31:40.000000 tencentcloud-sdk-python-tci-3.0.937/tencentcloud_sdk_python_tci.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:31:40.000000 tencentcloud-sdk-python-tci-3.0.937/tencentcloud_sdk_python_tci.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:31:40.000000 tencentcloud-sdk-python-tci-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:31:40.000000 tencentcloud-sdk-python-tci-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:06.000000 tencentcloud-sdk-python-tci-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:49:06.000000 tencentcloud-sdk-python-tci-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:06.000000 tencentcloud-sdk-python-tci-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:49:06.000000 tencentcloud-sdk-python-tci-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:06.000000 tencentcloud-sdk-python-tci-3.0.938/tencentcloud/tci/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:06.000000 tencentcloud-sdk-python-tci-3.0.938/tencentcloud/tci/v20190318/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:49:06.000000 tencentcloud-sdk-python-tci-3.0.938/tencentcloud/tci/v20190318/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44187 2023-07-19 00:49:06.000000 tencentcloud-sdk-python-tci-3.0.938/tencentcloud/tci/v20190318/tci_client.py
+-rw-r--r--   0 root         (0) root         (0)     8913 2023-07-19 00:49:06.000000 tencentcloud-sdk-python-tci-3.0.938/tencentcloud/tci/v20190318/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   285108 2023-07-19 00:49:06.000000 tencentcloud-sdk-python-tci-3.0.938/tencentcloud/tci/v20190318/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:49:06.000000 tencentcloud-sdk-python-tci-3.0.938/tencentcloud/tci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:49:06.000000 tencentcloud-sdk-python-tci-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:06.000000 tencentcloud-sdk-python-tci-3.0.938/tencentcloud_sdk_python_tci.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:49:06.000000 tencentcloud-sdk-python-tci-3.0.938/tencentcloud_sdk_python_tci.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:49:06.000000 tencentcloud-sdk-python-tci-3.0.938/tencentcloud_sdk_python_tci.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:49:06.000000 tencentcloud-sdk-python-tci-3.0.938/tencentcloud_sdk_python_tci.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:49:06.000000 tencentcloud-sdk-python-tci-3.0.938/tencentcloud_sdk_python_tci.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:49:06.000000 tencentcloud-sdk-python-tci-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:49:06.000000 tencentcloud-sdk-python-tci-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-tci-3.0.937/setup.py` & `tencentcloud-sdk-python-tci-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tci-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tci-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tci-3.0.937/tencentcloud/tci/v20190318/tci_client.py` & `tencentcloud-sdk-python-tci-3.0.938/tencentcloud/tci/v20190318/tci_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AIAssistantResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelTask(self, request):
         """用于取消已经提交的任务，目前只支持图像任务。
 
         :param request: Request instance for CancelTask.
         :type request: :class:`tencentcloud.tci.v20190318.models.CancelTaskRequest`
@@ -65,15 +65,15 @@
             model = models.CancelTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckFacePhoto(self, request):
         """检查人脸图片是否合法
 
         :param request: Request instance for CheckFacePhoto.
         :type request: :class:`tencentcloud.tci.v20190318.models.CheckFacePhotoRequest`
@@ -88,15 +88,15 @@
             model = models.CheckFacePhotoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFace(self, request):
         """创建人脸
 
         :param request: Request instance for CreateFace.
         :type request: :class:`tencentcloud.tci.v20190318.models.CreateFaceRequest`
@@ -111,15 +111,15 @@
             model = models.CreateFaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLibrary(self, request):
         """创建人员库
 
         :param request: Request instance for CreateLibrary.
         :type request: :class:`tencentcloud.tci.v20190318.models.CreateLibraryRequest`
@@ -134,15 +134,15 @@
             model = models.CreateLibraryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePerson(self, request):
         """创建人员
 
         :param request: Request instance for CreatePerson.
         :type request: :class:`tencentcloud.tci.v20190318.models.CreatePersonRequest`
@@ -157,15 +157,15 @@
             model = models.CreatePersonResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVocab(self, request):
         """创建词汇
 
         :param request: Request instance for CreateVocab.
         :type request: :class:`tencentcloud.tci.v20190318.models.CreateVocabRequest`
@@ -180,15 +180,15 @@
             model = models.CreateVocabResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVocabLib(self, request):
         """建立词汇库
 
         :param request: Request instance for CreateVocabLib.
         :type request: :class:`tencentcloud.tci.v20190318.models.CreateVocabLibRequest`
@@ -203,15 +203,15 @@
             model = models.CreateVocabLibResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteFace(self, request):
         """删除人脸
 
         :param request: Request instance for DeleteFace.
         :type request: :class:`tencentcloud.tci.v20190318.models.DeleteFaceRequest`
@@ -226,15 +226,15 @@
             model = models.DeleteFaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLibrary(self, request):
         """删除人员库
 
         :param request: Request instance for DeleteLibrary.
         :type request: :class:`tencentcloud.tci.v20190318.models.DeleteLibraryRequest`
@@ -249,15 +249,15 @@
             model = models.DeleteLibraryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePerson(self, request):
         """删除人员
 
         :param request: Request instance for DeletePerson.
         :type request: :class:`tencentcloud.tci.v20190318.models.DeletePersonRequest`
@@ -272,15 +272,15 @@
             model = models.DeletePersonResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteVocab(self, request):
         """删除词汇
 
         :param request: Request instance for DeleteVocab.
         :type request: :class:`tencentcloud.tci.v20190318.models.DeleteVocabRequest`
@@ -295,15 +295,15 @@
             model = models.DeleteVocabResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteVocabLib(self, request):
         """删除词汇库
 
         :param request: Request instance for DeleteVocabLib.
         :type request: :class:`tencentcloud.tci.v20190318.models.DeleteVocabLibRequest`
@@ -318,15 +318,15 @@
             model = models.DeleteVocabLibResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAITaskResult(self, request):
         """获取标准化接口任务结果
 
         :param request: Request instance for DescribeAITaskResult.
         :type request: :class:`tencentcloud.tci.v20190318.models.DescribeAITaskResultRequest`
@@ -341,15 +341,15 @@
             model = models.DescribeAITaskResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAttendanceResult(self, request):
         """人脸考勤查询结果
 
         :param request: Request instance for DescribeAttendanceResult.
         :type request: :class:`tencentcloud.tci.v20190318.models.DescribeAttendanceResultRequest`
@@ -364,15 +364,15 @@
             model = models.DescribeAttendanceResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAudioTask(self, request):
         """音频评估任务信息查询接口，异步查询客户提交的请求的结果。
 
         :param request: Request instance for DescribeAudioTask.
         :type request: :class:`tencentcloud.tci.v20190318.models.DescribeAudioTaskRequest`
@@ -387,15 +387,15 @@
             model = models.DescribeAudioTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConversationTask(self, request):
         """音频对话任务评估任务信息查询接口，异步查询客户提交的请求的结果。
 
         :param request: Request instance for DescribeConversationTask.
         :type request: :class:`tencentcloud.tci.v20190318.models.DescribeConversationTaskRequest`
@@ -410,15 +410,15 @@
             model = models.DescribeConversationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHighlightResult(self, request):
         """视频精彩集锦结果查询接口，异步查询客户提交的请求的结果。
 
         :param request: Request instance for DescribeHighlightResult.
         :type request: :class:`tencentcloud.tci.v20190318.models.DescribeHighlightResultRequest`
@@ -433,15 +433,15 @@
             model = models.DescribeHighlightResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageTask(self, request):
         """拉取任务详情
 
         :param request: Request instance for DescribeImageTask.
         :type request: :class:`tencentcloud.tci.v20190318.models.DescribeImageTaskRequest`
@@ -456,15 +456,15 @@
             model = models.DescribeImageTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageTaskStatistic(self, request):
         """获取图像任务统计信息
 
         :param request: Request instance for DescribeImageTaskStatistic.
         :type request: :class:`tencentcloud.tci.v20190318.models.DescribeImageTaskStatisticRequest`
@@ -479,15 +479,15 @@
             model = models.DescribeImageTaskStatisticResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLibraries(self, request):
         """获取人员库列表
 
         :param request: Request instance for DescribeLibraries.
         :type request: :class:`tencentcloud.tci.v20190318.models.DescribeLibrariesRequest`
@@ -502,15 +502,15 @@
             model = models.DescribeLibrariesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePerson(self, request):
         """获取人员详情
 
         :param request: Request instance for DescribePerson.
         :type request: :class:`tencentcloud.tci.v20190318.models.DescribePersonRequest`
@@ -525,15 +525,15 @@
             model = models.DescribePersonResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePersons(self, request):
         """拉取人员列表
 
         :param request: Request instance for DescribePersons.
         :type request: :class:`tencentcloud.tci.v20190318.models.DescribePersonsRequest`
@@ -548,15 +548,15 @@
             model = models.DescribePersonsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVocab(self, request):
         """查询词汇
 
         :param request: Request instance for DescribeVocab.
         :type request: :class:`tencentcloud.tci.v20190318.models.DescribeVocabRequest`
@@ -571,15 +571,15 @@
             model = models.DescribeVocabResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVocabLib(self, request):
         """查询词汇库
 
         :param request: Request instance for DescribeVocabLib.
         :type request: :class:`tencentcloud.tci.v20190318.models.DescribeVocabLibRequest`
@@ -594,15 +594,15 @@
             model = models.DescribeVocabLibResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLibrary(self, request):
         """修改人员库信息
 
         :param request: Request instance for ModifyLibrary.
         :type request: :class:`tencentcloud.tci.v20190318.models.ModifyLibraryRequest`
@@ -617,15 +617,15 @@
             model = models.ModifyLibraryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPerson(self, request):
         """修改人员信息
 
         :param request: Request instance for ModifyPerson.
         :type request: :class:`tencentcloud.tci.v20190318.models.ModifyPersonRequest`
@@ -640,15 +640,15 @@
             model = models.ModifyPersonResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SubmitAudioTask(self, request):
         """音频任务提交接口
 
         :param request: Request instance for SubmitAudioTask.
         :type request: :class:`tencentcloud.tci.v20190318.models.SubmitAudioTaskRequest`
@@ -663,15 +663,15 @@
             model = models.SubmitAudioTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SubmitCheckAttendanceTask(self, request):
         """提交人员考勤任务，支持包括点播和直播资源；支持通过DescribeAttendanceResult查询结果，也支持通过NoticeUrl设置考勤回调结果，回调结果结构如下：
         ##### 回调事件结构
          | 参数名称 | 类型 | 描述 |
          | ----  | ---  | ------  |
@@ -699,15 +699,15 @@
             model = models.SubmitCheckAttendanceTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SubmitCheckAttendanceTaskPlus(self, request):
         """支持多路视频流，提交高级人员考勤任务
 
         :param request: Request instance for SubmitCheckAttendanceTaskPlus.
         :type request: :class:`tencentcloud.tci.v20190318.models.SubmitCheckAttendanceTaskPlusRequest`
@@ -722,15 +722,15 @@
             model = models.SubmitCheckAttendanceTaskPlusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SubmitConversationTask(self, request):
         """对话任务分析接口
 
         :param request: Request instance for SubmitConversationTask.
         :type request: :class:`tencentcloud.tci.v20190318.models.SubmitConversationTaskRequest`
@@ -745,15 +745,15 @@
             model = models.SubmitConversationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SubmitDoubleVideoHighlights(self, request):
         """发起双路视频生成精彩集锦接口。该接口可以通过客户传入的学生音视频及老师视频两路Url，自动生成一堂课程的精彩集锦。需要通过DescribeHighlightResult
         接口获取生成结果。
 
         :param request: Request instance for SubmitDoubleVideoHighlights.
@@ -769,15 +769,15 @@
             model = models.SubmitDoubleVideoHighlightsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SubmitFullBodyClassTask(self, request):
         """**传统课堂授课任务**：在此场景中，老师为站立授课，有白板或投影供老师展示课程内容，摄像头可以拍摄到老师的半身或者全身。拍摄视频为一路全局画面，且背景不动，要求画面稳定清晰。通过此接口可分析老师授课的行为及语音，以支持AI评教。
 
         **提供的功能接口有：**老师人脸识别、老师表情识别、老师肢体动作识别、语音识别。  可分析的指标维度包括：身份识别、正脸、侧脸、人脸坐标、人脸尺寸、高兴、中性、高兴、中性、惊讶、厌恶、恐惧、愤怒、蔑视、悲伤、正面讲解、写板书、指黑板、语音转文字、发音时长、非发音时长、音量、语速、指定关键词的使用等
 
@@ -798,15 +798,15 @@
             model = models.SubmitFullBodyClassTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SubmitHighlights(self, request):
         """发起视频生成精彩集锦接口。该接口可以通过客户传入的课程音频数据及相关策略（如微笑抽取，专注抽取等），自动生成一堂课程的精彩集锦。需要通过QueryHighlightResult接口获取生成结果。
 
         :param request: Request instance for SubmitHighlights.
         :type request: :class:`tencentcloud.tci.v20190318.models.SubmitHighlightsRequest`
@@ -821,15 +821,15 @@
             model = models.SubmitHighlightsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SubmitImageTask(self, request):
         """提交图像分析任务
 
         :param request: Request instance for SubmitImageTask.
         :type request: :class:`tencentcloud.tci.v20190318.models.SubmitImageTaskRequest`
@@ -844,15 +844,15 @@
             model = models.SubmitImageTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SubmitImageTaskPlus(self, request):
         """高级图像分析任务，开放了图像任务里的所有开关，可以根据场景深度定制图像分析任务。支持的图像类别有，图片链接、图片二进制数据、点播链接和直播链接。
 
         :param request: Request instance for SubmitImageTaskPlus.
         :type request: :class:`tencentcloud.tci.v20190318.models.SubmitImageTaskPlusRequest`
@@ -867,15 +867,15 @@
             model = models.SubmitImageTaskPlusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SubmitOneByOneClassTask(self, request):
         """**提交在线1对1课堂任务**
         对于在线1对1课堂，老师通过视频向学生授课，并且学生人数为1人。通过上传学生端的图像信息，可以获取学生的听课情况分析。 具体指一路全局画面且背景不动，有1位学生的头像或上半身的画面，要求画面稳定清晰。
 
         **提供的功能接口有：**学生人脸识别、学生表情识别、语音识别。可分析的指标维度包括：学生身份识别、正脸、侧脸、抬头、低头、人脸坐标、人脸尺寸、高兴、中性、高兴、中性、惊讶、厌恶、恐惧、愤怒、蔑视、悲伤、语音转文字、发音时长、非发音时长、音量、语速等。
@@ -897,15 +897,15 @@
             model = models.SubmitOneByOneClassTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SubmitOpenClassTask(self, request):
         """**提交线下小班（无课桌）课任务**
         线下小班课是指有学生无课桌的课堂，满座15人以下，全局画面且背景不动，能清晰看到。
 
         **提供的功能接口有：**学生人脸识别、学生表情识别、学生肢体动作识别。  可分析的指标维度包括：身份识别、正脸、侧脸、抬头、低头、高兴、中性、高兴、中性、惊讶、厌恶、恐惧、愤怒、蔑视、悲伤、站立、举手、坐着等。
@@ -927,15 +927,15 @@
             model = models.SubmitOpenClassTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SubmitPartialBodyClassTask(self, request):
         """**在线小班课任务**：此场景是在线授课场景，老师一般为坐着授课，摄像头可以拍摄到老师的头部及上半身。拍摄视频为一路全局画面，且背景不动，要求画面稳定清晰。通过此接口可分析老师授课的行为及语音，以支持AI评教。
 
         **提供的功能接口有：**老师人脸识别、老师表情识别、老师手势识别、光线识别、语音识别。 可分析的指标维度包括：身份识别、正脸、侧脸、人脸坐标、人脸尺寸、高兴、中性、高兴、中性、惊讶、厌恶、恐惧、愤怒、蔑视、悲伤、点赞手势、听你说手势、听我说手势、拿教具行为、语音转文字、发音时长、非发音时长、音量、语速、指定关键词的使用等
 
@@ -956,15 +956,15 @@
             model = models.SubmitPartialBodyClassTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SubmitTraditionalClassTask(self, request):
         """**提交线下传统面授大班课（含课桌）任务。**
         传统教室课堂是指有学生课堂有课桌的课堂，满座20-50人，全局画面且背景不动。
 
         **提供的功能接口有：**学生人脸识别、学生表情识别、学生肢体动作识别。可分析的指标维度包括：学生身份识别、正脸、侧脸、抬头、低头、高兴、中性、高兴、中性、惊讶、厌恶、恐惧、愤怒、蔑视、悲伤、举手、站立、坐着、趴桌子、玩手机等
@@ -987,15 +987,15 @@
             model = models.SubmitTraditionalClassTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TransmitAudioStream(self, request):
         """分析音频信息
 
         :param request: Request instance for TransmitAudioStream.
         :type request: :class:`tencentcloud.tci.v20190318.models.TransmitAudioStreamRequest`
@@ -1010,8 +1010,8 @@
             model = models.TransmitAudioStreamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tci-3.0.937/tencentcloud/tci/v20190318/errorcodes.py` & `tencentcloud-sdk-python-tci-3.0.938/tencentcloud/tci/v20190318/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tci-3.0.937/tencentcloud/tci/v20190318/models.py` & `tencentcloud-sdk-python-tci-3.0.938/tencentcloud/tci/v20190318/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tci-3.0.937/tencentcloud_sdk_python_tci.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tci-3.0.938/tencentcloud_sdk_python_tci.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tci
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tci SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tci-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tci-3.0.938/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tci
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tci SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tci-3.0.937/README.rst` & `tencentcloud-sdk-python-tci-3.0.938/README.rst`

 * *Files identical despite different names*

