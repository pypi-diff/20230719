# Comparing `tmp/tencentcloud-sdk-python-ivld-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-ivld-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ivld-3.0.937.tar", last modified: Tue Jul 18 00:26:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ivld-3.0.938.tar", last modified: Wed Jul 19 00:41:41 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ivld-3.0.937.tar` & `tencentcloud-sdk-python-ivld-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:15.000000 tencentcloud-sdk-python-ivld-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:26:15.000000 tencentcloud-sdk-python-ivld-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:15.000000 tencentcloud-sdk-python-ivld-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:15.000000 tencentcloud-sdk-python-ivld-3.0.937/tencentcloud/ivld/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:15.000000 tencentcloud-sdk-python-ivld-3.0.937/tencentcloud/ivld/v20210903/
--rw-r--r--   0 root         (0) root         (0)    29455 2023-07-18 00:26:15.000000 tencentcloud-sdk-python-ivld-3.0.937/tencentcloud/ivld/v20210903/ivld_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:26:15.000000 tencentcloud-sdk-python-ivld-3.0.937/tencentcloud/ivld/v20210903/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9364 2023-07-18 00:26:15.000000 tencentcloud-sdk-python-ivld-3.0.937/tencentcloud/ivld/v20210903/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   158264 2023-07-18 00:26:15.000000 tencentcloud-sdk-python-ivld-3.0.937/tencentcloud/ivld/v20210903/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:26:15.000000 tencentcloud-sdk-python-ivld-3.0.937/tencentcloud/ivld/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:26:15.000000 tencentcloud-sdk-python-ivld-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:15.000000 tencentcloud-sdk-python-ivld-3.0.937/tencentcloud_sdk_python_ivld.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:26:15.000000 tencentcloud-sdk-python-ivld-3.0.937/tencentcloud_sdk_python_ivld.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:26:15.000000 tencentcloud-sdk-python-ivld-3.0.937/tencentcloud_sdk_python_ivld.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:26:15.000000 tencentcloud-sdk-python-ivld-3.0.937/tencentcloud_sdk_python_ivld.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:26:15.000000 tencentcloud-sdk-python-ivld-3.0.937/tencentcloud_sdk_python_ivld.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:26:15.000000 tencentcloud-sdk-python-ivld-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:26:15.000000 tencentcloud-sdk-python-ivld-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:26:15.000000 tencentcloud-sdk-python-ivld-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:41.000000 tencentcloud-sdk-python-ivld-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:41:41.000000 tencentcloud-sdk-python-ivld-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:41.000000 tencentcloud-sdk-python-ivld-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:41.000000 tencentcloud-sdk-python-ivld-3.0.938/tencentcloud/ivld/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:41.000000 tencentcloud-sdk-python-ivld-3.0.938/tencentcloud/ivld/v20210903/
+-rw-r--r--   0 root         (0) root         (0)    29555 2023-07-19 00:41:41.000000 tencentcloud-sdk-python-ivld-3.0.938/tencentcloud/ivld/v20210903/ivld_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:41:41.000000 tencentcloud-sdk-python-ivld-3.0.938/tencentcloud/ivld/v20210903/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9364 2023-07-19 00:41:41.000000 tencentcloud-sdk-python-ivld-3.0.938/tencentcloud/ivld/v20210903/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   158264 2023-07-19 00:41:41.000000 tencentcloud-sdk-python-ivld-3.0.938/tencentcloud/ivld/v20210903/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:41:41.000000 tencentcloud-sdk-python-ivld-3.0.938/tencentcloud/ivld/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:41:41.000000 tencentcloud-sdk-python-ivld-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:41.000000 tencentcloud-sdk-python-ivld-3.0.938/tencentcloud_sdk_python_ivld.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:41:41.000000 tencentcloud-sdk-python-ivld-3.0.938/tencentcloud_sdk_python_ivld.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:41:41.000000 tencentcloud-sdk-python-ivld-3.0.938/tencentcloud_sdk_python_ivld.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:41:41.000000 tencentcloud-sdk-python-ivld-3.0.938/tencentcloud_sdk_python_ivld.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:41:41.000000 tencentcloud-sdk-python-ivld-3.0.938/tencentcloud_sdk_python_ivld.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:41:41.000000 tencentcloud-sdk-python-ivld-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:41:41.000000 tencentcloud-sdk-python-ivld-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:41:41.000000 tencentcloud-sdk-python-ivld-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-ivld-3.0.937/setup.py` & `tencentcloud-sdk-python-ivld-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ivld-3.0.937/tencentcloud/ivld/v20210903/ivld_client.py` & `tencentcloud-sdk-python-ivld-3.0.938/tencentcloud/ivld/v20210903/ivld_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             model = models.AddCustomPersonImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCustomCategory(self, request):
         """创建自定义人物分类信息
 
         当L2Category为空时，将创建一级自定义分类。
         当L1Category与L2Category均不为空时，将创建二级自定义分类。请注意，**只有当一级自定义分类存在时，才可创建二级自定义分类**。
@@ -70,15 +70,15 @@
             model = models.CreateCustomCategoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCustomGroup(self, request):
         """创建自定义人物库
 
         Bucket的格式参考为 `bucketName-123456.cos.ap-shanghai.myqcloud.com`
 
@@ -103,15 +103,15 @@
             model = models.CreateCustomGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCustomPerson(self, request):
         """创建自定义人物。
 
         输入人物名称，基本信息，分类信息与人脸图片，创建自定义人物
 
@@ -130,15 +130,15 @@
             model = models.CreateCustomPersonResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDefaultCategories(self, request):
         """创建默认自定义人物类型
 
         :param request: Request instance for CreateDefaultCategories.
         :type request: :class:`tencentcloud.ivld.v20210903.models.CreateDefaultCategoriesRequest`
@@ -153,15 +153,15 @@
             model = models.CreateDefaultCategoriesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTask(self, request):
         """创建智能标签任务。
 
         请注意，本接口为异步接口，**返回TaskId只代表任务创建成功，不代表任务执行成功**。
 
@@ -178,15 +178,15 @@
             model = models.CreateTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCustomCategory(self, request):
         """删除自定义分类信息
 
         :param request: Request instance for DeleteCustomCategory.
         :type request: :class:`tencentcloud.ivld.v20210903.models.DeleteCustomCategoryRequest`
@@ -201,15 +201,15 @@
             model = models.DeleteCustomCategoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCustomPerson(self, request):
         """删除自定义人物
 
         :param request: Request instance for DeleteCustomPerson.
         :type request: :class:`tencentcloud.ivld.v20210903.models.DeleteCustomPersonRequest`
@@ -224,15 +224,15 @@
             model = models.DeleteCustomPersonResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCustomPersonImage(self, request):
         """删除自定义人脸数据
 
         :param request: Request instance for DeleteCustomPersonImage.
         :type request: :class:`tencentcloud.ivld.v20210903.models.DeleteCustomPersonImageRequest`
@@ -247,15 +247,15 @@
             model = models.DeleteCustomPersonImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteMedia(self, request):
         """将MediaId对应的媒资文件从系统中删除。
 
         **请注意，本接口仅删除媒资文件，媒资文件对应的视频分析结果不会被删除**。如您需要删除结构化分析结果，请调用DeleteTask接口。
 
@@ -272,15 +272,15 @@
             model = models.DeleteMediaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTask(self, request):
         """删除任务信息
 
         请注意，本接口**不会**删除媒资文件
 
@@ -299,15 +299,15 @@
             model = models.DeleteTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCustomCategories(self, request):
         """批量描述自定义人物分类信息
 
         :param request: Request instance for DescribeCustomCategories.
         :type request: :class:`tencentcloud.ivld.v20210903.models.DescribeCustomCategoriesRequest`
@@ -322,15 +322,15 @@
             model = models.DescribeCustomCategoriesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCustomGroup(self, request):
         """描述自定义人物库信息，当前库大小(库中有多少人脸)，以及库中的存储桶
 
         :param request: Request instance for DescribeCustomGroup.
         :type request: :class:`tencentcloud.ivld.v20210903.models.DescribeCustomGroupRequest`
@@ -345,15 +345,15 @@
             model = models.DescribeCustomGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCustomPersonDetail(self, request):
         """描述自定义人物详细信息，包括人物信息与人物信息
 
         :param request: Request instance for DescribeCustomPersonDetail.
         :type request: :class:`tencentcloud.ivld.v20210903.models.DescribeCustomPersonDetailRequest`
@@ -368,15 +368,15 @@
             model = models.DescribeCustomPersonDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCustomPersons(self, request):
         """批量描述自定义人物
 
 
         :param request: Request instance for DescribeCustomPersons.
@@ -392,15 +392,15 @@
             model = models.DescribeCustomPersonsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMedia(self, request):
         """描述媒资文件信息，包括媒资状态，分辨率，帧率等。
 
         如果媒资文件未完成导入，本接口将仅输出媒资文件的状态信息；导入完成后，本接口还将输出媒资文件的其他元信息。
 
@@ -417,15 +417,15 @@
             model = models.DescribeMediaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMedias(self, request):
         """依照输入条件，描述命中的媒资文件信息，包括媒资状态，分辨率，帧率等。
 
         请注意，本接口最多支持同时描述**50**个媒资文件
 
@@ -444,15 +444,15 @@
             model = models.DescribeMediasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTask(self, request):
         """描述智能标签任务进度。
 
         请注意，**此接口仅返回任务执行状态信息，不返回任务执行结果**
 
@@ -470,15 +470,15 @@
             model = models.DescribeTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskDetail(self, request):
         """描述任务信息，如果任务成功完成，还将返回任务结果
 
         :param request: Request instance for DescribeTaskDetail.
         :type request: :class:`tencentcloud.ivld.v20210903.models.DescribeTaskDetailRequest`
@@ -493,15 +493,15 @@
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
         """依照输入条件，描述命中的任务信息，包括任务创建时间，处理时间信息等。
 
         请注意，本接口最多支持同时描述**50**个任务信息
 
@@ -518,15 +518,15 @@
             model = models.DescribeTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ImportMedia(self, request):
         """将URL指向的媒资视频文件导入系统之中。
 
         **请注意，本接口为异步接口**。接口返回MediaId仅代表导入视频任务发起，不代表任务完成，您可调用读接口(DescribeMedia/DescribeMedias)接口查询MediaId
 
@@ -549,15 +549,15 @@
             model = models.ImportMediaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCallback(self, request):
         """用户设置对应事件的回调地址
 
         ### 回调事件消息通知协议
 
@@ -606,15 +606,15 @@
             model = models.ModifyCallbackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryCallback(self, request):
         """查询用户回调设置
 
         :param request: Request instance for QueryCallback.
         :type request: :class:`tencentcloud.ivld.v20210903.models.QueryCallbackRequest`
@@ -629,15 +629,15 @@
             model = models.QueryCallbackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateCustomCategory(self, request):
         """更新自定义人物分类
 
         当L2Category为空时，代表更新CategoryId对应的一级自定义人物类型以及所有二级自定义人物类型所从属的一级自定义人物类型；
         当L2Category非空时，仅更新CategoryId对应的二级自定义人物类型
@@ -655,15 +655,15 @@
             model = models.UpdateCustomCategoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateCustomPerson(self, request):
         """更新自定义人物信息，包括姓名，简要信息，分类信息等
 
         :param request: Request instance for UpdateCustomPerson.
         :type request: :class:`tencentcloud.ivld.v20210903.models.UpdateCustomPersonRequest`
@@ -678,8 +678,8 @@
             model = models.UpdateCustomPersonResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-ivld-3.0.937/tencentcloud/ivld/v20210903/errorcodes.py` & `tencentcloud-sdk-python-ivld-3.0.938/tencentcloud/ivld/v20210903/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ivld-3.0.937/tencentcloud/ivld/v20210903/models.py` & `tencentcloud-sdk-python-ivld-3.0.938/tencentcloud/ivld/v20210903/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ivld-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ivld-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ivld-3.0.937/tencentcloud_sdk_python_ivld.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ivld-3.0.938/tencentcloud_sdk_python_ivld.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ivld
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ivld SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ivld-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-ivld-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ivld
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ivld SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ivld-3.0.937/README.rst` & `tencentcloud-sdk-python-ivld-3.0.938/README.rst`

 * *Files identical despite different names*

