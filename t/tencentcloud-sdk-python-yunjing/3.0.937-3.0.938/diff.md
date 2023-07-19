# Comparing `tmp/tencentcloud-sdk-python-yunjing-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-yunjing-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-yunjing-3.0.937.tar", last modified: Tue Jul 18 00:35:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-yunjing-3.0.938.tar", last modified: Wed Jul 19 00:54:26 2023, max compression
```

## Comparing `tencentcloud-sdk-python-yunjing-3.0.937.tar` & `tencentcloud-sdk-python-yunjing-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:57.000000 tencentcloud-sdk-python-yunjing-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-18 00:35:57.000000 tencentcloud-sdk-python-yunjing-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:57.000000 tencentcloud-sdk-python-yunjing-3.0.937/tencentcloud_sdk_python_yunjing.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:35:57.000000 tencentcloud-sdk-python-yunjing-3.0.937/tencentcloud_sdk_python_yunjing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-18 00:35:57.000000 tencentcloud-sdk-python-yunjing-3.0.937/tencentcloud_sdk_python_yunjing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:35:57.000000 tencentcloud-sdk-python-yunjing-3.0.937/tencentcloud_sdk_python_yunjing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:35:57.000000 tencentcloud-sdk-python-yunjing-3.0.937/tencentcloud_sdk_python_yunjing.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:57.000000 tencentcloud-sdk-python-yunjing-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:35:57.000000 tencentcloud-sdk-python-yunjing-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:57.000000 tencentcloud-sdk-python-yunjing-3.0.937/tencentcloud/yunjing/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:35:57.000000 tencentcloud-sdk-python-yunjing-3.0.937/tencentcloud/yunjing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:57.000000 tencentcloud-sdk-python-yunjing-3.0.937/tencentcloud/yunjing/v20180228/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:35:57.000000 tencentcloud-sdk-python-yunjing-3.0.937/tencentcloud/yunjing/v20180228/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3960 2023-07-18 00:35:57.000000 tencentcloud-sdk-python-yunjing-3.0.937/tencentcloud/yunjing/v20180228/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    93972 2023-07-18 00:35:57.000000 tencentcloud-sdk-python-yunjing-3.0.937/tencentcloud/yunjing/v20180228/yunjing_client.py
--rw-r--r--   0 root         (0) root         (0)   379701 2023-07-18 00:35:57.000000 tencentcloud-sdk-python-yunjing-3.0.937/tencentcloud/yunjing/v20180228/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:35:57.000000 tencentcloud-sdk-python-yunjing-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:35:57.000000 tencentcloud-sdk-python-yunjing-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-18 00:35:57.000000 tencentcloud-sdk-python-yunjing-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:54:26.000000 tencentcloud-sdk-python-yunjing-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-19 00:54:26.000000 tencentcloud-sdk-python-yunjing-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:54:26.000000 tencentcloud-sdk-python-yunjing-3.0.938/tencentcloud_sdk_python_yunjing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:54:26.000000 tencentcloud-sdk-python-yunjing-3.0.938/tencentcloud_sdk_python_yunjing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-19 00:54:26.000000 tencentcloud-sdk-python-yunjing-3.0.938/tencentcloud_sdk_python_yunjing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:54:26.000000 tencentcloud-sdk-python-yunjing-3.0.938/tencentcloud_sdk_python_yunjing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:54:26.000000 tencentcloud-sdk-python-yunjing-3.0.938/tencentcloud_sdk_python_yunjing.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:54:26.000000 tencentcloud-sdk-python-yunjing-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:54:26.000000 tencentcloud-sdk-python-yunjing-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:54:26.000000 tencentcloud-sdk-python-yunjing-3.0.938/tencentcloud/yunjing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:54:26.000000 tencentcloud-sdk-python-yunjing-3.0.938/tencentcloud/yunjing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:54:26.000000 tencentcloud-sdk-python-yunjing-3.0.938/tencentcloud/yunjing/v20180228/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:54:26.000000 tencentcloud-sdk-python-yunjing-3.0.938/tencentcloud/yunjing/v20180228/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3960 2023-07-19 00:54:26.000000 tencentcloud-sdk-python-yunjing-3.0.938/tencentcloud/yunjing/v20180228/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    94372 2023-07-19 00:54:26.000000 tencentcloud-sdk-python-yunjing-3.0.938/tencentcloud/yunjing/v20180228/yunjing_client.py
+-rw-r--r--   0 root         (0) root         (0)   379701 2023-07-19 00:54:26.000000 tencentcloud-sdk-python-yunjing-3.0.938/tencentcloud/yunjing/v20180228/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:54:26.000000 tencentcloud-sdk-python-yunjing-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:54:26.000000 tencentcloud-sdk-python-yunjing-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-19 00:54:26.000000 tencentcloud-sdk-python-yunjing-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-yunjing-3.0.937/setup.py` & `tencentcloud-sdk-python-yunjing-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yunjing-3.0.937/tencentcloud_sdk_python_yunjing.egg-info/PKG-INFO` & `tencentcloud-sdk-python-yunjing-3.0.938/tencentcloud_sdk_python_yunjing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-yunjing
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Yunjing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-yunjing-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-yunjing-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-yunjing-3.0.937/tencentcloud/yunjing/v20180228/errorcodes.py` & `tencentcloud-sdk-python-yunjing-3.0.938/tencentcloud/yunjing/v20180228/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yunjing-3.0.937/tencentcloud/yunjing/v20180228/yunjing_client.py` & `tencentcloud-sdk-python-yunjing-3.0.938/tencentcloud/yunjing/v20180228/yunjing_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AddLoginWhiteListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddMachineTag(self, request):
         """增加机器关联标签
 
         :param request: Request instance for AddMachineTag.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.AddMachineTagRequest`
@@ -65,15 +65,15 @@
             model = models.AddMachineTagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CloseProVersion(self, request):
         """本接口 (CloseProVersion) 用于关闭专业版。
 
         :param request: Request instance for CloseProVersion.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.CloseProVersionRequest`
@@ -88,15 +88,15 @@
             model = models.CloseProVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateBaselineStrategy(self, request):
         """根据策略信息创建基线策略
 
         :param request: Request instance for CreateBaselineStrategy.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.CreateBaselineStrategyRequest`
@@ -111,15 +111,15 @@
             model = models.CreateBaselineStrategyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOpenPortTask(self, request):
         """本接口 (CreateOpenPortTask) 用于创建实时获取端口任务。
 
         :param request: Request instance for CreateOpenPortTask.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.CreateOpenPortTaskRequest`
@@ -134,15 +134,15 @@
             model = models.CreateOpenPortTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateProcessTask(self, request):
         """本接口 (CreateProcessTask) 用于创建实时拉取进程任务。
 
         :param request: Request instance for CreateProcessTask.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.CreateProcessTaskRequest`
@@ -157,15 +157,15 @@
             model = models.CreateProcessTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateUsualLoginPlaces(self, request):
         """此接口（CreateUsualLoginPlaces）用于添加常用登录地。
 
         :param request: Request instance for CreateUsualLoginPlaces.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.CreateUsualLoginPlacesRequest`
@@ -180,15 +180,15 @@
             model = models.CreateUsualLoginPlacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAttackLogs(self, request):
         """删除网络攻击日志
 
         :param request: Request instance for DeleteAttackLogs.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DeleteAttackLogsRequest`
@@ -203,15 +203,15 @@
             model = models.DeleteAttackLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteBashEvents(self, request):
         """根据Ids删除高危命令事件
 
         :param request: Request instance for DeleteBashEvents.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DeleteBashEventsRequest`
@@ -226,15 +226,15 @@
             model = models.DeleteBashEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteBashRules(self, request):
         """删除高危命令规则
 
         :param request: Request instance for DeleteBashRules.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DeleteBashRulesRequest`
@@ -249,15 +249,15 @@
             model = models.DeleteBashRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteBruteAttacks(self, request):
         """本接口 (DeleteBruteAttacks) 用于删除暴力破解记录。
 
         :param request: Request instance for DeleteBruteAttacks.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DeleteBruteAttacksRequest`
@@ -272,15 +272,15 @@
             model = models.DeleteBruteAttacksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLoginWhiteList(self, request):
         """删除白名单规则
 
         :param request: Request instance for DeleteLoginWhiteList.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DeleteLoginWhiteListRequest`
@@ -295,15 +295,15 @@
             model = models.DeleteLoginWhiteListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteMachine(self, request):
         """本接口（DeleteMachine）用于卸载云镜客户端。
 
         :param request: Request instance for DeleteMachine.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DeleteMachineRequest`
@@ -318,15 +318,15 @@
             model = models.DeleteMachineResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteMachineTag(self, request):
         """删除服务器关联的标签
 
         :param request: Request instance for DeleteMachineTag.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DeleteMachineTagRequest`
@@ -341,15 +341,15 @@
             model = models.DeleteMachineTagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteMaliciousRequests(self, request):
         """本接口 (DeleteMaliciousRequests) 用于删除恶意请求记录。
 
         :param request: Request instance for DeleteMaliciousRequests.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DeleteMaliciousRequestsRequest`
@@ -364,15 +364,15 @@
             model = models.DeleteMaliciousRequestsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteMalwares(self, request):
         """本接口 (DeleteMalwares) 用于删除木马记录。
 
         :param request: Request instance for DeleteMalwares.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DeleteMalwaresRequest`
@@ -387,15 +387,15 @@
             model = models.DeleteMalwaresResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteNonlocalLoginPlaces(self, request):
         """本接口 (DeleteNonlocalLoginPlaces) 用于删除异地登录记录。
 
         :param request: Request instance for DeleteNonlocalLoginPlaces.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DeleteNonlocalLoginPlacesRequest`
@@ -410,15 +410,15 @@
             model = models.DeleteNonlocalLoginPlacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePrivilegeEvents(self, request):
         """根据Ids删除本地提权
 
         :param request: Request instance for DeletePrivilegeEvents.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DeletePrivilegeEventsRequest`
@@ -433,15 +433,15 @@
             model = models.DeletePrivilegeEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePrivilegeRules(self, request):
         """删除本地提权规则
 
         :param request: Request instance for DeletePrivilegeRules.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DeletePrivilegeRulesRequest`
@@ -456,15 +456,15 @@
             model = models.DeletePrivilegeRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteReverseShellEvents(self, request):
         """根据Ids删除反弹Shell事件
 
         :param request: Request instance for DeleteReverseShellEvents.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DeleteReverseShellEventsRequest`
@@ -479,15 +479,15 @@
             model = models.DeleteReverseShellEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteReverseShellRules(self, request):
         """删除反弹Shell规则
 
         :param request: Request instance for DeleteReverseShellRules.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DeleteReverseShellRulesRequest`
@@ -502,15 +502,15 @@
             model = models.DeleteReverseShellRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTags(self, request):
         """删除标签
 
         :param request: Request instance for DeleteTags.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DeleteTagsRequest`
@@ -525,15 +525,15 @@
             model = models.DeleteTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteUsualLoginPlaces(self, request):
         """本接口（DeleteUsualLoginPlaces）用于删除常用登录地。
 
         :param request: Request instance for DeleteUsualLoginPlaces.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DeleteUsualLoginPlacesRequest`
@@ -548,15 +548,15 @@
             model = models.DeleteUsualLoginPlacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccountStatistics(self, request):
         """本接口 (DescribeAccountStatistics) 用于获取帐号统计列表数据。
 
         :param request: Request instance for DescribeAccountStatistics.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeAccountStatisticsRequest`
@@ -571,15 +571,15 @@
             model = models.DescribeAccountStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccounts(self, request):
         """本接口 (DescribeAccounts) 用于获取帐号列表数据。
 
         :param request: Request instance for DescribeAccounts.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeAccountsRequest`
@@ -594,15 +594,15 @@
             model = models.DescribeAccountsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAgentVuls(self, request):
         """本接口 (DescribeAgentVuls) 用于获取单台主机的漏洞列表。
 
         :param request: Request instance for DescribeAgentVuls.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeAgentVulsRequest`
@@ -617,15 +617,15 @@
             model = models.DescribeAgentVulsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAlarmAttribute(self, request):
         """本接口 (DescribeAlarmAttribute) 用于获取告警设置。
 
         :param request: Request instance for DescribeAlarmAttribute.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeAlarmAttributeRequest`
@@ -640,15 +640,15 @@
             model = models.DescribeAlarmAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAttackLogInfo(self, request):
         """网络攻击日志详情
 
         :param request: Request instance for DescribeAttackLogInfo.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeAttackLogInfoRequest`
@@ -663,15 +663,15 @@
             model = models.DescribeAttackLogInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAttackLogs(self, request):
         """按分页形式展示网络攻击日志列表
 
         :param request: Request instance for DescribeAttackLogs.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeAttackLogsRequest`
@@ -686,15 +686,15 @@
             model = models.DescribeAttackLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBashEvents(self, request):
         """获取高危命令列表
 
         :param request: Request instance for DescribeBashEvents.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeBashEventsRequest`
@@ -709,15 +709,15 @@
             model = models.DescribeBashEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBashRules(self, request):
         """获取高危命令规则列表
 
         :param request: Request instance for DescribeBashRules.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeBashRulesRequest`
@@ -732,15 +732,15 @@
             model = models.DescribeBashRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBruteAttacks(self, request):
         """本接口{DescribeBruteAttacks}用于获取暴力破解事件列表。
 
         :param request: Request instance for DescribeBruteAttacks.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeBruteAttacksRequest`
@@ -755,15 +755,15 @@
             model = models.DescribeBruteAttacksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeComponentInfo(self, request):
         """本接口 (DescribeComponentInfo) 用于获取组件信息数据。
 
         :param request: Request instance for DescribeComponentInfo.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeComponentInfoRequest`
@@ -778,15 +778,15 @@
             model = models.DescribeComponentInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeComponentStatistics(self, request):
         """本接口 (DescribeComponentStatistics) 用于获取组件统计列表数据。
 
         :param request: Request instance for DescribeComponentStatistics.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeComponentStatisticsRequest`
@@ -801,15 +801,15 @@
             model = models.DescribeComponentStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeComponents(self, request):
         """本接口 (DescribeComponents) 用于获取组件列表数据。
 
         :param request: Request instance for DescribeComponents.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeComponentsRequest`
@@ -824,15 +824,15 @@
             model = models.DescribeComponentsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHistoryAccounts(self, request):
         """本接口 (DescribeHistoryAccounts) 用于获取帐号变更历史列表数据。
 
         :param request: Request instance for DescribeHistoryAccounts.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeHistoryAccountsRequest`
@@ -847,15 +847,15 @@
             model = models.DescribeHistoryAccountsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImpactedHosts(self, request):
         """本接口 (DescribeImpactedHosts) 用于获取漏洞受影响机器列表。
 
         :param request: Request instance for DescribeImpactedHosts.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeImpactedHostsRequest`
@@ -870,15 +870,15 @@
             model = models.DescribeImpactedHostsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLoginWhiteList(self, request):
         """获取异地登录白名单列表
 
         :param request: Request instance for DescribeLoginWhiteList.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeLoginWhiteListRequest`
@@ -893,15 +893,15 @@
             model = models.DescribeLoginWhiteListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMachineInfo(self, request):
         """本接口（DescribeMachineInfo）用于获取机器详细信息。
 
         :param request: Request instance for DescribeMachineInfo.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeMachineInfoRequest`
@@ -916,15 +916,15 @@
             model = models.DescribeMachineInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMachines(self, request):
         """本接口 (DescribeMachines) 用于获取区域主机列表。
 
         :param request: Request instance for DescribeMachines.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeMachinesRequest`
@@ -939,15 +939,15 @@
             model = models.DescribeMachinesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMaliciousRequests(self, request):
         """本接口 (DescribeMaliciousRequests) 用于获取恶意请求数据。
 
         :param request: Request instance for DescribeMaliciousRequests.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeMaliciousRequestsRequest`
@@ -962,15 +962,15 @@
             model = models.DescribeMaliciousRequestsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMalwares(self, request):
         """本接口（DescribeMalwares）用于获取木马事件列表。
 
         :param request: Request instance for DescribeMalwares.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeMalwaresRequest`
@@ -985,15 +985,15 @@
             model = models.DescribeMalwaresResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNonlocalLoginPlaces(self, request):
         """本接口(DescribeNonlocalLoginPlaces)用于获取异地登录事件。
 
         :param request: Request instance for DescribeNonlocalLoginPlaces.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeNonlocalLoginPlacesRequest`
@@ -1008,15 +1008,15 @@
             model = models.DescribeNonlocalLoginPlacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOpenPortStatistics(self, request):
         """本接口 (DescribeOpenPortStatistics) 用于获取端口统计列表。
 
         :param request: Request instance for DescribeOpenPortStatistics.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeOpenPortStatisticsRequest`
@@ -1031,15 +1031,15 @@
             model = models.DescribeOpenPortStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOpenPortTaskStatus(self, request):
         """本接口 (DescribeOpenPortTaskStatus) 用于获取实时拉取端口任务状态。
 
         :param request: Request instance for DescribeOpenPortTaskStatus.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeOpenPortTaskStatusRequest`
@@ -1054,15 +1054,15 @@
             model = models.DescribeOpenPortTaskStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOpenPorts(self, request):
         """本接口 (DescribeOpenPorts) 用于获取端口列表数据。
 
         :param request: Request instance for DescribeOpenPorts.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeOpenPortsRequest`
@@ -1077,15 +1077,15 @@
             model = models.DescribeOpenPortsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOverviewStatistics(self, request):
         """本接口用于（DescribeOverviewStatistics）获取概览统计数据。
 
         :param request: Request instance for DescribeOverviewStatistics.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeOverviewStatisticsRequest`
@@ -1100,15 +1100,15 @@
             model = models.DescribeOverviewStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrivilegeEvents(self, request):
         """获取本地提权事件列表
 
         :param request: Request instance for DescribePrivilegeEvents.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribePrivilegeEventsRequest`
@@ -1123,15 +1123,15 @@
             model = models.DescribePrivilegeEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrivilegeRules(self, request):
         """获取本地提权规则列表
 
         :param request: Request instance for DescribePrivilegeRules.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribePrivilegeRulesRequest`
@@ -1146,15 +1146,15 @@
             model = models.DescribePrivilegeRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProVersionInfo(self, request):
         """本接口 (DescribeProVersionInfo) 用于获取专业版信息。
 
         :param request: Request instance for DescribeProVersionInfo.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeProVersionInfoRequest`
@@ -1169,15 +1169,15 @@
             model = models.DescribeProVersionInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProcessStatistics(self, request):
         """本接口 (DescribeProcessStatistics) 用于获取进程统计列表数据。
 
         :param request: Request instance for DescribeProcessStatistics.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeProcessStatisticsRequest`
@@ -1192,15 +1192,15 @@
             model = models.DescribeProcessStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProcessTaskStatus(self, request):
         """本接口 (DescribeProcessTaskStatus) 用于获取实时拉取进程任务状态。
 
         :param request: Request instance for DescribeProcessTaskStatus.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeProcessTaskStatusRequest`
@@ -1215,15 +1215,15 @@
             model = models.DescribeProcessTaskStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProcesses(self, request):
         """本接口 (DescribeProcesses) 用于获取进程列表数据。
 
         :param request: Request instance for DescribeProcesses.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeProcessesRequest`
@@ -1238,15 +1238,15 @@
             model = models.DescribeProcessesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeReverseShellEvents(self, request):
         """获取反弹Shell列表
 
         :param request: Request instance for DescribeReverseShellEvents.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeReverseShellEventsRequest`
@@ -1261,15 +1261,15 @@
             model = models.DescribeReverseShellEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeReverseShellRules(self, request):
         """获取反弹Shell规则列表
 
         :param request: Request instance for DescribeReverseShellRules.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeReverseShellRulesRequest`
@@ -1284,15 +1284,15 @@
             model = models.DescribeReverseShellRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecurityDynamics(self, request):
         """本接口 (DescribeSecurityDynamics) 用于获取安全事件消息数据。
 
         :param request: Request instance for DescribeSecurityDynamics.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeSecurityDynamicsRequest`
@@ -1307,15 +1307,15 @@
             model = models.DescribeSecurityDynamicsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecurityTrends(self, request):
         """本接口 (DescribeSecurityTrends) 用于获取安全事件统计数据。
 
         :param request: Request instance for DescribeSecurityTrends.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeSecurityTrendsRequest`
@@ -1330,15 +1330,15 @@
             model = models.DescribeSecurityTrendsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTagMachines(self, request):
         """获取指定标签关联的服务器信息
 
         :param request: Request instance for DescribeTagMachines.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeTagMachinesRequest`
@@ -1353,15 +1353,15 @@
             model = models.DescribeTagMachinesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTags(self, request):
         """获取所有主机标签
 
         :param request: Request instance for DescribeTags.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeTagsRequest`
@@ -1376,15 +1376,15 @@
             model = models.DescribeTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUsualLoginPlaces(self, request):
         """此接口（DescribeUsualLoginPlaces）用于查询常用登录地。
 
         :param request: Request instance for DescribeUsualLoginPlaces.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeUsualLoginPlacesRequest`
@@ -1399,15 +1399,15 @@
             model = models.DescribeUsualLoginPlacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulInfo(self, request):
         """本接口 (DescribeVulInfo) 用于获取漏洞详情。
 
         :param request: Request instance for DescribeVulInfo.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeVulInfoRequest`
@@ -1422,15 +1422,15 @@
             model = models.DescribeVulInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulScanResult(self, request):
         """本接口 (DescribeVulScanResult) 用于获取漏洞检测结果。
 
         :param request: Request instance for DescribeVulScanResult.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeVulScanResultRequest`
@@ -1445,15 +1445,15 @@
             model = models.DescribeVulScanResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVuls(self, request):
         """本接口 (DescribeVuls) 用于获取漏洞列表数据。
 
         :param request: Request instance for DescribeVuls.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeVulsRequest`
@@ -1468,15 +1468,15 @@
             model = models.DescribeVulsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWeeklyReportBruteAttacks(self, request):
         """本接口 (DescribeWeeklyReportBruteAttacks) 用于获取专业周报密码破解数据。
 
         :param request: Request instance for DescribeWeeklyReportBruteAttacks.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeWeeklyReportBruteAttacksRequest`
@@ -1491,15 +1491,15 @@
             model = models.DescribeWeeklyReportBruteAttacksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWeeklyReportInfo(self, request):
         """本接口 (DescribeWeeklyReportInfo) 用于获取专业周报详情数据。
 
         :param request: Request instance for DescribeWeeklyReportInfo.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeWeeklyReportInfoRequest`
@@ -1514,15 +1514,15 @@
             model = models.DescribeWeeklyReportInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWeeklyReportMalwares(self, request):
         """本接口 (DescribeWeeklyReportMalwares) 用于获取专业周报木马数据。
 
         :param request: Request instance for DescribeWeeklyReportMalwares.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeWeeklyReportMalwaresRequest`
@@ -1537,15 +1537,15 @@
             model = models.DescribeWeeklyReportMalwaresResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWeeklyReportNonlocalLoginPlaces(self, request):
         """本接口 (DescribeWeeklyReportNonlocalLoginPlaces) 用于获取专业周报异地登录数据。
 
         :param request: Request instance for DescribeWeeklyReportNonlocalLoginPlaces.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeWeeklyReportNonlocalLoginPlacesRequest`
@@ -1560,15 +1560,15 @@
             model = models.DescribeWeeklyReportNonlocalLoginPlacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWeeklyReportVuls(self, request):
         """本接口 (DescribeWeeklyReportVuls) 用于专业版周报漏洞数据。
 
         :param request: Request instance for DescribeWeeklyReportVuls.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeWeeklyReportVulsRequest`
@@ -1583,15 +1583,15 @@
             model = models.DescribeWeeklyReportVulsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWeeklyReports(self, request):
         """本接口 (DescribeWeeklyReports) 用于获取周报列表数据。
 
         :param request: Request instance for DescribeWeeklyReports.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.DescribeWeeklyReportsRequest`
@@ -1606,15 +1606,15 @@
             model = models.DescribeWeeklyReportsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EditBashRule(self, request):
         """新增或修改高危命令规则
 
         :param request: Request instance for EditBashRule.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.EditBashRuleRequest`
@@ -1629,15 +1629,15 @@
             model = models.EditBashRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EditPrivilegeRule(self, request):
         """新增或修改本地提权规则
 
         :param request: Request instance for EditPrivilegeRule.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.EditPrivilegeRuleRequest`
@@ -1652,15 +1652,15 @@
             model = models.EditPrivilegeRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EditReverseShellRule(self, request):
         """编辑反弹Shell规则
 
         :param request: Request instance for EditReverseShellRule.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.EditReverseShellRuleRequest`
@@ -1675,15 +1675,15 @@
             model = models.EditReverseShellRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EditTags(self, request):
         """新增或编辑标签
 
         :param request: Request instance for EditTags.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.EditTagsRequest`
@@ -1698,15 +1698,15 @@
             model = models.EditTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExportAttackLogs(self, request):
         """导出网络攻击日志
 
         :param request: Request instance for ExportAttackLogs.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.ExportAttackLogsRequest`
@@ -1721,15 +1721,15 @@
             model = models.ExportAttackLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExportBashEvents(self, request):
         """导出高危命令事件
 
         :param request: Request instance for ExportBashEvents.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.ExportBashEventsRequest`
@@ -1744,15 +1744,15 @@
             model = models.ExportBashEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExportBruteAttacks(self, request):
         """本接口 (ExportBruteAttacks) 用于导出密码破解记录成CSV文件。
 
         :param request: Request instance for ExportBruteAttacks.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.ExportBruteAttacksRequest`
@@ -1767,15 +1767,15 @@
             model = models.ExportBruteAttacksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExportMaliciousRequests(self, request):
         """本接口 (ExportMaliciousRequests) 用于导出下载恶意请求文件。
 
         :param request: Request instance for ExportMaliciousRequests.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.ExportMaliciousRequestsRequest`
@@ -1790,15 +1790,15 @@
             model = models.ExportMaliciousRequestsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExportMalwares(self, request):
         """本接口 (ExportMalwares) 用于导出木马记录CSV文件。
 
         :param request: Request instance for ExportMalwares.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.ExportMalwaresRequest`
@@ -1813,15 +1813,15 @@
             model = models.ExportMalwaresResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExportNonlocalLoginPlaces(self, request):
         """本接口 (ExportNonlocalLoginPlaces) 用于导出异地登录事件记录CSV文件。
 
         :param request: Request instance for ExportNonlocalLoginPlaces.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.ExportNonlocalLoginPlacesRequest`
@@ -1836,15 +1836,15 @@
             model = models.ExportNonlocalLoginPlacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExportPrivilegeEvents(self, request):
         """导出本地提权事件
 
         :param request: Request instance for ExportPrivilegeEvents.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.ExportPrivilegeEventsRequest`
@@ -1859,15 +1859,15 @@
             model = models.ExportPrivilegeEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExportReverseShellEvents(self, request):
         """导出反弹Shell事件
 
         :param request: Request instance for ExportReverseShellEvents.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.ExportReverseShellEventsRequest`
@@ -1882,15 +1882,15 @@
             model = models.ExportReverseShellEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def IgnoreImpactedHosts(self, request):
         """本接口 (IgnoreImpactedHosts) 用于忽略漏洞。
 
         :param request: Request instance for IgnoreImpactedHosts.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.IgnoreImpactedHostsRequest`
@@ -1905,15 +1905,15 @@
             model = models.IgnoreImpactedHostsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceOpenProVersionPrepaid(self, request):
         """本接口 (InquiryPriceOpenProVersionPrepaid) 用于开通专业版询价(预付费)。
 
         :param request: Request instance for InquiryPriceOpenProVersionPrepaid.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.InquiryPriceOpenProVersionPrepaidRequest`
@@ -1928,15 +1928,15 @@
             model = models.InquiryPriceOpenProVersionPrepaidResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def MisAlarmNonlocalLoginPlaces(self, request):
         """本接口{MisAlarmNonlocalLoginPlaces}将设置当前地点为常用登录地。
 
         :param request: Request instance for MisAlarmNonlocalLoginPlaces.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.MisAlarmNonlocalLoginPlacesRequest`
@@ -1951,15 +1951,15 @@
             model = models.MisAlarmNonlocalLoginPlacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAlarmAttribute(self, request):
         """本接口（ModifyAlarmAttribute）用于修改告警设置。
 
         :param request: Request instance for ModifyAlarmAttribute.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.ModifyAlarmAttributeRequest`
@@ -1974,15 +1974,15 @@
             model = models.ModifyAlarmAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAutoOpenProVersionConfig(self, request):
         """本接口 (ModifyAutoOpenProVersionConfig) 用于设置新增主机自动开通专业版配置。
 
         :param request: Request instance for ModifyAutoOpenProVersionConfig.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.ModifyAutoOpenProVersionConfigRequest`
@@ -1997,15 +1997,15 @@
             model = models.ModifyAutoOpenProVersionConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLoginWhiteList(self, request):
         """编辑白名单规则
 
         :param request: Request instance for ModifyLoginWhiteList.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.ModifyLoginWhiteListRequest`
@@ -2020,15 +2020,15 @@
             model = models.ModifyLoginWhiteListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyProVersionRenewFlag(self, request):
         """本接口 (ModifyProVersionRenewFlag) 用于修改专业版包年包月续费标识。
 
         :param request: Request instance for ModifyProVersionRenewFlag.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.ModifyProVersionRenewFlagRequest`
@@ -2043,15 +2043,15 @@
             model = models.ModifyProVersionRenewFlagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OpenProVersion(self, request):
         """本接口 (OpenProVersion) 用于开通专业版。
 
         :param request: Request instance for OpenProVersion.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.OpenProVersionRequest`
@@ -2066,15 +2066,15 @@
             model = models.OpenProVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OpenProVersionPrepaid(self, request):
         """本接口 (OpenProVersionPrepaid) 用于开通专业版(包年包月)。
 
         :param request: Request instance for OpenProVersionPrepaid.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.OpenProVersionPrepaidRequest`
@@ -2089,15 +2089,15 @@
             model = models.OpenProVersionPrepaidResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RecoverMalwares(self, request):
         """本接口（RecoverMalwares）用于批量恢复已经被隔离的木马文件。
 
         :param request: Request instance for RecoverMalwares.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.RecoverMalwaresRequest`
@@ -2112,15 +2112,15 @@
             model = models.RecoverMalwaresResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RenewProVersion(self, request):
         """本接口 (RenewProVersion) 用于续费专业版(包年包月)。
 
         :param request: Request instance for RenewProVersion.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.RenewProVersionRequest`
@@ -2135,15 +2135,15 @@
             model = models.RenewProVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RescanImpactedHost(self, request):
         """本接口 (RescanImpactedHost) 用于漏洞重新检测。
 
         :param request: Request instance for RescanImpactedHost.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.RescanImpactedHostRequest`
@@ -2158,15 +2158,15 @@
             model = models.RescanImpactedHostResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SeparateMalwares(self, request):
         """本接口（SeparateMalwares）用于隔离木马。
 
         :param request: Request instance for SeparateMalwares.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.SeparateMalwaresRequest`
@@ -2181,15 +2181,15 @@
             model = models.SeparateMalwaresResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetBashEventsStatus(self, request):
         """设置高危命令事件状态
 
         :param request: Request instance for SetBashEventsStatus.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.SetBashEventsStatusRequest`
@@ -2204,15 +2204,15 @@
             model = models.SetBashEventsStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SwitchBashRules(self, request):
         """切换高危命令规则状态
 
         :param request: Request instance for SwitchBashRules.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.SwitchBashRulesRequest`
@@ -2227,15 +2227,15 @@
             model = models.SwitchBashRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TrustMaliciousRequest(self, request):
         """本接口 (TrustMaliciousRequest) 用于恶意请求添加信任。
 
         :param request: Request instance for TrustMaliciousRequest.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.TrustMaliciousRequestRequest`
@@ -2250,15 +2250,15 @@
             model = models.TrustMaliciousRequestResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TrustMalwares(self, request):
         """本接口(TrustMalwares)将被识别木马文件设为信任。
 
         :param request: Request instance for TrustMalwares.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.TrustMalwaresRequest`
@@ -2273,15 +2273,15 @@
             model = models.TrustMalwaresResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UntrustMaliciousRequest(self, request):
         """本接口 (UntrustMaliciousRequest) 用于取消信任恶意请求。
 
         :param request: Request instance for UntrustMaliciousRequest.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.UntrustMaliciousRequestRequest`
@@ -2296,15 +2296,15 @@
             model = models.UntrustMaliciousRequestResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UntrustMalwares(self, request):
         """本接口（UntrustMalwares）用于取消信任木马文件。
 
         :param request: Request instance for UntrustMalwares.
         :type request: :class:`tencentcloud.yunjing.v20180228.models.UntrustMalwaresRequest`
@@ -2319,8 +2319,8 @@
             model = models.UntrustMalwaresResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-yunjing-3.0.937/tencentcloud/yunjing/v20180228/models.py` & `tencentcloud-sdk-python-yunjing-3.0.938/tencentcloud/yunjing/v20180228/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yunjing-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-yunjing-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-yunjing
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Yunjing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-yunjing-3.0.937/README.rst` & `tencentcloud-sdk-python-yunjing-3.0.938/README.rst`

 * *Files identical despite different names*

