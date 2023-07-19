# Comparing `tmp/tencentcloud-sdk-python-apcas-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-apcas-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-apcas-3.0.936.tar", last modified: Mon Jul 17 00:15:35 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-apcas-3.0.938.tar", last modified: Wed Jul 19 00:20:52 2023, max compression
```

## Comparing `tencentcloud-sdk-python-apcas-3.0.936.tar` & `tencentcloud-sdk-python-apcas-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:15:35.000000 tencentcloud-sdk-python-apcas-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-17 00:15:35.000000 tencentcloud-sdk-python-apcas-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:15:35.000000 tencentcloud-sdk-python-apcas-3.0.936/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:15:35.000000 tencentcloud-sdk-python-apcas-3.0.936/tencentcloud/apcas/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:15:35.000000 tencentcloud-sdk-python-apcas-3.0.936/tencentcloud/apcas/v20201127/
--rw-r--r--   0 root         (0) root         (0)     7186 2023-07-17 00:15:35.000000 tencentcloud-sdk-python-apcas-3.0.936/tencentcloud/apcas/v20201127/apcas_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:15:35.000000 tencentcloud-sdk-python-apcas-3.0.936/tencentcloud/apcas/v20201127/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-07-17 00:15:35.000000 tencentcloud-sdk-python-apcas-3.0.936/tencentcloud/apcas/v20201127/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    35285 2023-07-17 00:15:35.000000 tencentcloud-sdk-python-apcas-3.0.936/tencentcloud/apcas/v20201127/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:15:35.000000 tencentcloud-sdk-python-apcas-3.0.936/tencentcloud/apcas/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:15:35.000000 tencentcloud-sdk-python-apcas-3.0.936/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:15:35.000000 tencentcloud-sdk-python-apcas-3.0.936/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-17 00:15:35.000000 tencentcloud-sdk-python-apcas-3.0.936/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-17 00:15:35.000000 tencentcloud-sdk-python-apcas-3.0.936/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:15:35.000000 tencentcloud-sdk-python-apcas-3.0.936/tencentcloud_sdk_python_apcas.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:15:35.000000 tencentcloud-sdk-python-apcas-3.0.936/tencentcloud_sdk_python_apcas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-07-17 00:15:35.000000 tencentcloud-sdk-python-apcas-3.0.936/tencentcloud_sdk_python_apcas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-17 00:15:35.000000 tencentcloud-sdk-python-apcas-3.0.936/tencentcloud_sdk_python_apcas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:15:35.000000 tencentcloud-sdk-python-apcas-3.0.936/tencentcloud_sdk_python_apcas.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:52.000000 tencentcloud-sdk-python-apcas-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-19 00:20:52.000000 tencentcloud-sdk-python-apcas-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:52.000000 tencentcloud-sdk-python-apcas-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:52.000000 tencentcloud-sdk-python-apcas-3.0.938/tencentcloud/apcas/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:52.000000 tencentcloud-sdk-python-apcas-3.0.938/tencentcloud/apcas/v20201127/
+-rw-r--r--   0 root         (0) root         (0)     7214 2023-07-19 00:20:52.000000 tencentcloud-sdk-python-apcas-3.0.938/tencentcloud/apcas/v20201127/apcas_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:20:52.000000 tencentcloud-sdk-python-apcas-3.0.938/tencentcloud/apcas/v20201127/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-07-19 00:20:52.000000 tencentcloud-sdk-python-apcas-3.0.938/tencentcloud/apcas/v20201127/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    35285 2023-07-19 00:20:52.000000 tencentcloud-sdk-python-apcas-3.0.938/tencentcloud/apcas/v20201127/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:20:52.000000 tencentcloud-sdk-python-apcas-3.0.938/tencentcloud/apcas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:20:52.000000 tencentcloud-sdk-python-apcas-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:20:52.000000 tencentcloud-sdk-python-apcas-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:20:52.000000 tencentcloud-sdk-python-apcas-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-19 00:20:52.000000 tencentcloud-sdk-python-apcas-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:52.000000 tencentcloud-sdk-python-apcas-3.0.938/tencentcloud_sdk_python_apcas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:20:52.000000 tencentcloud-sdk-python-apcas-3.0.938/tencentcloud_sdk_python_apcas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-07-19 00:20:52.000000 tencentcloud-sdk-python-apcas-3.0.938/tencentcloud_sdk_python_apcas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:20:52.000000 tencentcloud-sdk-python-apcas-3.0.938/tencentcloud_sdk_python_apcas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:20:52.000000 tencentcloud-sdk-python-apcas-3.0.938/tencentcloud_sdk_python_apcas.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-apcas-3.0.936/setup.py` & `tencentcloud-sdk-python-apcas-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apcas-3.0.936/tencentcloud/apcas/v20201127/apcas_client.py` & `tencentcloud-sdk-python-apcas-3.0.938/tencentcloud/apcas/v20201127/apcas_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.GetTaskDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetTaskList(self, request):
         """查询当前账号AppID下的画像洞察任务列表
 
         :param request: Request instance for GetTaskList.
         :type request: :class:`tencentcloud.apcas.v20201127.models.GetTaskListRequest`
@@ -65,15 +65,15 @@
             model = models.GetTaskListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PredictRating(self, request):
         """根据传入的设备号（IMEI、IDFA、手机号、手机号MD5），返回意向评级结果
 
         :param request: Request instance for PredictRating.
         :type request: :class:`tencentcloud.apcas.v20201127.models.PredictRatingRequest`
@@ -88,15 +88,15 @@
             model = models.PredictRatingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryCallDetails(self, request):
         """查询调用明细
 
         :param request: Request instance for QueryCallDetails.
         :type request: :class:`tencentcloud.apcas.v20201127.models.QueryCallDetailsRequest`
@@ -111,15 +111,15 @@
             model = models.QueryCallDetailsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryCallStat(self, request):
         """按时间维度获取调用量统计
 
         :param request: Request instance for QueryCallStat.
         :type request: :class:`tencentcloud.apcas.v20201127.models.QueryCallStatRequest`
@@ -134,15 +134,15 @@
             model = models.QueryCallStatResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryGeneralStat(self, request):
         """获取日/月/周/总调用量统计数据
 
         :param request: Request instance for QueryGeneralStat.
         :type request: :class:`tencentcloud.apcas.v20201127.models.QueryGeneralStatRequest`
@@ -157,15 +157,15 @@
             model = models.QueryGeneralStatResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UploadId(self, request):
         """上传群体画像的ID列表（支持的ID类型：0:imei 7:IDFA 8:MD5(imei)），后台返回生成的画像分析任务ID
 
         :param request: Request instance for UploadId.
         :type request: :class:`tencentcloud.apcas.v20201127.models.UploadIdRequest`
@@ -180,8 +180,8 @@
             model = models.UploadIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-apcas-3.0.936/tencentcloud/apcas/v20201127/errorcodes.py` & `tencentcloud-sdk-python-apcas-3.0.938/tencentcloud/apcas/v20201127/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apcas-3.0.936/tencentcloud/apcas/v20201127/models.py` & `tencentcloud-sdk-python-apcas-3.0.938/tencentcloud/apcas/v20201127/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apcas-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-apcas-3.0.938/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.936'
+__version__ = '3.0.938'
```

### Comparing `tencentcloud-sdk-python-apcas-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-apcas-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apcas
-Version: 3.0.936
+Version: 3.0.938
 Summary: Tencent Cloud Apcas SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apcas-3.0.936/README.rst` & `tencentcloud-sdk-python-apcas-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apcas-3.0.936/tencentcloud_sdk_python_apcas.egg-info/PKG-INFO` & `tencentcloud-sdk-python-apcas-3.0.938/tencentcloud_sdk_python_apcas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apcas
-Version: 3.0.936
+Version: 3.0.938
 Summary: Tencent Cloud Apcas SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

