# Comparing `tmp/tencentcloud-sdk-python-ms-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-ms-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ms-3.0.937.tar", last modified: Tue Jul 18 00:27:53 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ms-3.0.938.tar", last modified: Wed Jul 19 00:43:13 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ms-3.0.937.tar` & `tencentcloud-sdk-python-ms-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:53.000000 tencentcloud-sdk-python-ms-3.0.937/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:53.000000 tencentcloud-sdk-python-ms-3.0.937/tencentcloud_sdk_python_ms.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:27:53.000000 tencentcloud-sdk-python-ms-3.0.937/tencentcloud_sdk_python_ms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-07-18 00:27:53.000000 tencentcloud-sdk-python-ms-3.0.937/tencentcloud_sdk_python_ms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:27:53.000000 tencentcloud-sdk-python-ms-3.0.937/tencentcloud_sdk_python_ms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:27:53.000000 tencentcloud-sdk-python-ms-3.0.937/tencentcloud_sdk_python_ms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-18 00:27:53.000000 tencentcloud-sdk-python-ms-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:53.000000 tencentcloud-sdk-python-ms-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:53.000000 tencentcloud-sdk-python-ms-3.0.937/tencentcloud/ms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:53.000000 tencentcloud-sdk-python-ms-3.0.937/tencentcloud/ms/v20180408/
--rw-r--r--   0 root         (0) root         (0)    14712 2023-07-18 00:27:53.000000 tencentcloud-sdk-python-ms-3.0.937/tencentcloud/ms/v20180408/ms_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:53.000000 tencentcloud-sdk-python-ms-3.0.937/tencentcloud/ms/v20180408/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3469 2023-07-18 00:27:53.000000 tencentcloud-sdk-python-ms-3.0.937/tencentcloud/ms/v20180408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    90316 2023-07-18 00:27:53.000000 tencentcloud-sdk-python-ms-3.0.937/tencentcloud/ms/v20180408/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:53.000000 tencentcloud-sdk-python-ms-3.0.937/tencentcloud/ms/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:27:53.000000 tencentcloud-sdk-python-ms-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:27:53.000000 tencentcloud-sdk-python-ms-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:27:53.000000 tencentcloud-sdk-python-ms-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-18 00:27:53.000000 tencentcloud-sdk-python-ms-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:13.000000 tencentcloud-sdk-python-ms-3.0.938/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:13.000000 tencentcloud-sdk-python-ms-3.0.938/tencentcloud_sdk_python_ms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:43:13.000000 tencentcloud-sdk-python-ms-3.0.938/tencentcloud_sdk_python_ms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-19 00:43:13.000000 tencentcloud-sdk-python-ms-3.0.938/tencentcloud_sdk_python_ms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:43:13.000000 tencentcloud-sdk-python-ms-3.0.938/tencentcloud_sdk_python_ms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:43:13.000000 tencentcloud-sdk-python-ms-3.0.938/tencentcloud_sdk_python_ms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-19 00:43:13.000000 tencentcloud-sdk-python-ms-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:13.000000 tencentcloud-sdk-python-ms-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:13.000000 tencentcloud-sdk-python-ms-3.0.938/tencentcloud/ms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:13.000000 tencentcloud-sdk-python-ms-3.0.938/tencentcloud/ms/v20180408/
+-rw-r--r--   0 root         (0) root         (0)    14764 2023-07-19 00:43:13.000000 tencentcloud-sdk-python-ms-3.0.938/tencentcloud/ms/v20180408/ms_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:43:13.000000 tencentcloud-sdk-python-ms-3.0.938/tencentcloud/ms/v20180408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3469 2023-07-19 00:43:13.000000 tencentcloud-sdk-python-ms-3.0.938/tencentcloud/ms/v20180408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    90316 2023-07-19 00:43:13.000000 tencentcloud-sdk-python-ms-3.0.938/tencentcloud/ms/v20180408/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:43:13.000000 tencentcloud-sdk-python-ms-3.0.938/tencentcloud/ms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:43:13.000000 tencentcloud-sdk-python-ms-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:43:13.000000 tencentcloud-sdk-python-ms-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:43:13.000000 tencentcloud-sdk-python-ms-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-19 00:43:13.000000 tencentcloud-sdk-python-ms-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-ms-3.0.937/tencentcloud_sdk_python_ms.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ms-3.0.938/tencentcloud_sdk_python_ms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ms
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ms-3.0.937/setup.py` & `tencentcloud-sdk-python-ms-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ms-3.0.937/tencentcloud/ms/v20180408/ms_client.py` & `tencentcloud-sdk-python-ms-3.0.938/tencentcloud/ms/v20180408/ms_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateBindInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCosSecKeyInstance(self, request):
         """获取云COS文件存储临时密钥，密钥仅限于临时上传文件，有访问限制和时效性，请保管好临时密钥。
 
         :param request: Request instance for CreateCosSecKeyInstance.
         :type request: :class:`tencentcloud.ms.v20180408.models.CreateCosSecKeyInstanceRequest`
@@ -65,15 +65,15 @@
             model = models.CreateCosSecKeyInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateResourceInstances(self, request):
         """用户可以使用该接口自建资源，只支持白名单用户
 
         :param request: Request instance for CreateResourceInstances.
         :type request: :class:`tencentcloud.ms.v20180408.models.CreateResourceInstancesRequest`
@@ -88,15 +88,15 @@
             model = models.CreateResourceInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateShieldInstance(self, request):
         """用户通过该接口提交应用进行应用加固，加固后需通过DescribeShieldResult接口查询加固结果。（注意：根据国家互联网用户实名制相关要求，使用该产品前，需先完成实名认证。）
 
         :param request: Request instance for CreateShieldInstance.
         :type request: :class:`tencentcloud.ms.v20180408.models.CreateShieldInstanceRequest`
@@ -111,15 +111,15 @@
             model = models.CreateShieldInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateShieldPlanInstance(self, request):
         """对资源进行策略新增。（注意：根据国家互联网用户实名制相关要求，使用该产品前，需先完成实名认证。）
 
         :param request: Request instance for CreateShieldPlanInstance.
         :type request: :class:`tencentcloud.ms.v20180408.models.CreateShieldPlanInstanceRequest`
@@ -134,15 +134,15 @@
             model = models.CreateShieldPlanInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteShieldInstances(self, request):
         """删除一个或者多个app加固信息。（注意：根据国家互联网用户实名制相关要求，使用该产品前，需先完成实名认证。）
 
         :param request: Request instance for DeleteShieldInstances.
         :type request: :class:`tencentcloud.ms.v20180408.models.DeleteShieldInstancesRequest`
@@ -157,15 +157,15 @@
             model = models.DeleteShieldInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApkDetectionResult(self, request):
         """该接口采用同步模式请求腾讯APK云检测服务，即时返回检测数据，需要用户用轮询的方式调用本接口来进行样本送检并获取检测结果(每隔60s发送一次请求，传相同的参数，重试30次)，一般情况下0.5h内会出检测结果，最长时间是3h。当Result为ok并且ResultList数组非空有值时，代表检测完毕，若长时间获取不到检测结果，请联系客服。
 
         :param request: Request instance for DescribeApkDetectionResult.
         :type request: :class:`tencentcloud.ms.v20180408.models.DescribeApkDetectionResultRequest`
@@ -180,15 +180,15 @@
             model = models.DescribeApkDetectionResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourceInstances(self, request):
         """获取某个用户的所有资源信息。（注意：根据国家互联网用户实名制相关要求，使用该产品前，需先完成实名认证。）
 
         :param request: Request instance for DescribeResourceInstances.
         :type request: :class:`tencentcloud.ms.v20180408.models.DescribeResourceInstancesRequest`
@@ -203,15 +203,15 @@
             model = models.DescribeResourceInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeShieldInstances(self, request):
         """本接口用于查看app列表。
         可以通过指定任务唯一标识ItemId来查询指定app的详细信息，或通过设定过滤器来查询满足过滤条件的app的详细信息。 指定偏移(Offset)和限制(Limit)来选择结果中的一部分，默认返回满足条件的前20个app信息。（注意：根据国家互联网用户实名制相关要求，使用该产品前，需先完成实名认证。）
 
         :param request: Request instance for DescribeShieldInstances.
@@ -227,15 +227,15 @@
             model = models.DescribeShieldInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeShieldPlanInstance(self, request):
         """查询加固策略。（注意：根据国家互联网用户实名制相关要求，使用该产品前，需先完成实名认证。）
 
         :param request: Request instance for DescribeShieldPlanInstance.
         :type request: :class:`tencentcloud.ms.v20180408.models.DescribeShieldPlanInstanceRequest`
@@ -250,15 +250,15 @@
             model = models.DescribeShieldPlanInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeShieldResult(self, request):
         """通过唯一标识获取加固的结果。（注意：根据国家互联网用户实名制相关要求，使用该产品前，需先完成实名认证。）
 
         :param request: Request instance for DescribeShieldResult.
         :type request: :class:`tencentcloud.ms.v20180408.models.DescribeShieldResultRequest`
@@ -273,15 +273,15 @@
             model = models.DescribeShieldResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUrlDetectionResult(self, request):
         """移动安全-网址检测服务
 
         :param request: Request instance for DescribeUrlDetectionResult.
         :type request: :class:`tencentcloud.ms.v20180408.models.DescribeUrlDetectionResultRequest`
@@ -296,15 +296,15 @@
             model = models.DescribeUrlDetectionResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserBaseInfoInstance(self, request):
         """获取用户基础信息
 
         :param request: Request instance for DescribeUserBaseInfoInstance.
         :type request: :class:`tencentcloud.ms.v20180408.models.DescribeUserBaseInfoInstanceRequest`
@@ -319,8 +319,8 @@
             model = models.DescribeUserBaseInfoInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-ms-3.0.937/tencentcloud/ms/v20180408/errorcodes.py` & `tencentcloud-sdk-python-ms-3.0.938/tencentcloud/ms/v20180408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ms-3.0.937/tencentcloud/ms/v20180408/models.py` & `tencentcloud-sdk-python-ms-3.0.938/tencentcloud/ms/v20180408/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ms-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ms-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ms-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-ms-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ms
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ms-3.0.937/README.rst` & `tencentcloud-sdk-python-ms-3.0.938/README.rst`

 * *Files identical despite different names*

