# Comparing `tmp/tencentcloud-sdk-python-cmq-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-cmq-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cmq-3.0.937.tar", last modified: Tue Jul 18 00:20:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cmq-3.0.938.tar", last modified: Wed Jul 19 00:25:04 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cmq-3.0.937.tar` & `tencentcloud-sdk-python-cmq-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:57.000000 tencentcloud-sdk-python-cmq-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:20:56.000000 tencentcloud-sdk-python-cmq-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:57.000000 tencentcloud-sdk-python-cmq-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:57.000000 tencentcloud-sdk-python-cmq-3.0.937/tencentcloud/cmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:20:56.000000 tencentcloud-sdk-python-cmq-3.0.937/tencentcloud/cmq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:57.000000 tencentcloud-sdk-python-cmq-3.0.937/tencentcloud/cmq/v20190304/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:20:56.000000 tencentcloud-sdk-python-cmq-3.0.937/tencentcloud/cmq/v20190304/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15754 2023-07-18 00:20:56.000000 tencentcloud-sdk-python-cmq-3.0.937/tencentcloud/cmq/v20190304/cmq_client.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-07-18 00:20:56.000000 tencentcloud-sdk-python-cmq-3.0.937/tencentcloud/cmq/v20190304/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    98147 2023-07-18 00:20:56.000000 tencentcloud-sdk-python-cmq-3.0.937/tencentcloud/cmq/v20190304/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:20:56.000000 tencentcloud-sdk-python-cmq-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:20:57.000000 tencentcloud-sdk-python-cmq-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:57.000000 tencentcloud-sdk-python-cmq-3.0.937/tencentcloud_sdk_python_cmq.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:20:56.000000 tencentcloud-sdk-python-cmq-3.0.937/tencentcloud_sdk_python_cmq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:20:56.000000 tencentcloud-sdk-python-cmq-3.0.937/tencentcloud_sdk_python_cmq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:20:56.000000 tencentcloud-sdk-python-cmq-3.0.937/tencentcloud_sdk_python_cmq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:20:56.000000 tencentcloud-sdk-python-cmq-3.0.937/tencentcloud_sdk_python_cmq.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:20:57.000000 tencentcloud-sdk-python-cmq-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:20:56.000000 tencentcloud-sdk-python-cmq-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:04.000000 tencentcloud-sdk-python-cmq-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:25:03.000000 tencentcloud-sdk-python-cmq-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:04.000000 tencentcloud-sdk-python-cmq-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:04.000000 tencentcloud-sdk-python-cmq-3.0.938/tencentcloud/cmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:25:03.000000 tencentcloud-sdk-python-cmq-3.0.938/tencentcloud/cmq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:04.000000 tencentcloud-sdk-python-cmq-3.0.938/tencentcloud/cmq/v20190304/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:25:03.000000 tencentcloud-sdk-python-cmq-3.0.938/tencentcloud/cmq/v20190304/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15822 2023-07-19 00:25:03.000000 tencentcloud-sdk-python-cmq-3.0.938/tencentcloud/cmq/v20190304/cmq_client.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-07-19 00:25:03.000000 tencentcloud-sdk-python-cmq-3.0.938/tencentcloud/cmq/v20190304/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    98147 2023-07-19 00:25:03.000000 tencentcloud-sdk-python-cmq-3.0.938/tencentcloud/cmq/v20190304/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:25:03.000000 tencentcloud-sdk-python-cmq-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:25:04.000000 tencentcloud-sdk-python-cmq-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:04.000000 tencentcloud-sdk-python-cmq-3.0.938/tencentcloud_sdk_python_cmq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:25:04.000000 tencentcloud-sdk-python-cmq-3.0.938/tencentcloud_sdk_python_cmq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:25:04.000000 tencentcloud-sdk-python-cmq-3.0.938/tencentcloud_sdk_python_cmq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:25:04.000000 tencentcloud-sdk-python-cmq-3.0.938/tencentcloud_sdk_python_cmq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:25:04.000000 tencentcloud-sdk-python-cmq-3.0.938/tencentcloud_sdk_python_cmq.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:25:04.000000 tencentcloud-sdk-python-cmq-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:25:03.000000 tencentcloud-sdk-python-cmq-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-cmq-3.0.937/setup.py` & `tencentcloud-sdk-python-cmq-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cmq-3.0.937/tencentcloud/cmq/v20190304/cmq_client.py` & `tencentcloud-sdk-python-cmq-3.0.938/tencentcloud/cmq/v20190304/cmq_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.ClearQueueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ClearSubscriptionFilterTags(self, request):
         """清空订阅者消息标签
 
         :param request: Request instance for ClearSubscriptionFilterTags.
         :type request: :class:`tencentcloud.cmq.v20190304.models.ClearSubscriptionFilterTagsRequest`
@@ -65,15 +65,15 @@
             model = models.ClearSubscriptionFilterTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateQueue(self, request):
         """创建队列接口
 
         :param request: Request instance for CreateQueue.
         :type request: :class:`tencentcloud.cmq.v20190304.models.CreateQueueRequest`
@@ -88,15 +88,15 @@
             model = models.CreateQueueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSubscribe(self, request):
         """创建订阅接口
 
         :param request: Request instance for CreateSubscribe.
         :type request: :class:`tencentcloud.cmq.v20190304.models.CreateSubscribeRequest`
@@ -111,15 +111,15 @@
             model = models.CreateSubscribeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTopic(self, request):
         """创建主题
 
         :param request: Request instance for CreateTopic.
         :type request: :class:`tencentcloud.cmq.v20190304.models.CreateTopicRequest`
@@ -134,15 +134,15 @@
             model = models.CreateTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteQueue(self, request):
         """DeleteQueue
 
         :param request: Request instance for DeleteQueue.
         :type request: :class:`tencentcloud.cmq.v20190304.models.DeleteQueueRequest`
@@ -157,15 +157,15 @@
             model = models.DeleteQueueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSubscribe(self, request):
         """删除订阅
 
         :param request: Request instance for DeleteSubscribe.
         :type request: :class:`tencentcloud.cmq.v20190304.models.DeleteSubscribeRequest`
@@ -180,15 +180,15 @@
             model = models.DeleteSubscribeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTopic(self, request):
         """删除主题
 
         :param request: Request instance for DeleteTopic.
         :type request: :class:`tencentcloud.cmq.v20190304.models.DeleteTopicRequest`
@@ -203,15 +203,15 @@
             model = models.DeleteTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeadLetterSourceQueues(self, request):
         """枚举死信队列源队列
 
         :param request: Request instance for DescribeDeadLetterSourceQueues.
         :type request: :class:`tencentcloud.cmq.v20190304.models.DescribeDeadLetterSourceQueuesRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeDeadLetterSourceQueuesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeQueueDetail(self, request):
         """枚举队列
 
         :param request: Request instance for DescribeQueueDetail.
         :type request: :class:`tencentcloud.cmq.v20190304.models.DescribeQueueDetailRequest`
@@ -249,15 +249,15 @@
             model = models.DescribeQueueDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSubscriptionDetail(self, request):
         """查询订阅详情
 
         :param request: Request instance for DescribeSubscriptionDetail.
         :type request: :class:`tencentcloud.cmq.v20190304.models.DescribeSubscriptionDetailRequest`
@@ -272,15 +272,15 @@
             model = models.DescribeSubscriptionDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopicDetail(self, request):
         """查询主题详情
 
         :param request: Request instance for DescribeTopicDetail.
         :type request: :class:`tencentcloud.cmq.v20190304.models.DescribeTopicDetailRequest`
@@ -295,15 +295,15 @@
             model = models.DescribeTopicDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyQueueAttribute(self, request):
         """修改队列属性
 
         :param request: Request instance for ModifyQueueAttribute.
         :type request: :class:`tencentcloud.cmq.v20190304.models.ModifyQueueAttributeRequest`
@@ -318,15 +318,15 @@
             model = models.ModifyQueueAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySubscriptionAttribute(self, request):
         """修改订阅属性
 
         :param request: Request instance for ModifySubscriptionAttribute.
         :type request: :class:`tencentcloud.cmq.v20190304.models.ModifySubscriptionAttributeRequest`
@@ -341,15 +341,15 @@
             model = models.ModifySubscriptionAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTopicAttribute(self, request):
         """修改主题属性
 
         :param request: Request instance for ModifyTopicAttribute.
         :type request: :class:`tencentcloud.cmq.v20190304.models.ModifyTopicAttributeRequest`
@@ -364,15 +364,15 @@
             model = models.ModifyTopicAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RewindQueue(self, request):
         """回溯队列
 
         :param request: Request instance for RewindQueue.
         :type request: :class:`tencentcloud.cmq.v20190304.models.RewindQueueRequest`
@@ -387,15 +387,15 @@
             model = models.RewindQueueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnbindDeadLetter(self, request):
         """解绑死信队列
 
         :param request: Request instance for UnbindDeadLetter.
         :type request: :class:`tencentcloud.cmq.v20190304.models.UnbindDeadLetterRequest`
@@ -410,8 +410,8 @@
             model = models.UnbindDeadLetterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-cmq-3.0.937/tencentcloud/cmq/v20190304/errorcodes.py` & `tencentcloud-sdk-python-cmq-3.0.938/tencentcloud/cmq/v20190304/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cmq-3.0.937/tencentcloud/cmq/v20190304/models.py` & `tencentcloud-sdk-python-cmq-3.0.938/tencentcloud/cmq/v20190304/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cmq-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cmq-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cmq-3.0.937/tencentcloud_sdk_python_cmq.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cmq-3.0.938/tencentcloud_sdk_python_cmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cmq
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cmq-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-cmq-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cmq
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cmq-3.0.937/README.rst` & `tencentcloud-sdk-python-cmq-3.0.938/README.rst`

 * *Files identical despite different names*

