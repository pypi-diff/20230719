# Comparing `tmp/tencentcloud-sdk-python-tat-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tat-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tat-3.0.937.tar", last modified: Tue Jul 18 00:30:53 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tat-3.0.938.tar", last modified: Wed Jul 19 00:48:17 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tat-3.0.937.tar` & `tencentcloud-sdk-python-tat-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:53.000000 tencentcloud-sdk-python-tat-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:30:53.000000 tencentcloud-sdk-python-tat-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:53.000000 tencentcloud-sdk-python-tat-3.0.937/tencentcloud_sdk_python_tat.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:30:53.000000 tencentcloud-sdk-python-tat-3.0.937/tencentcloud_sdk_python_tat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:30:53.000000 tencentcloud-sdk-python-tat-3.0.937/tencentcloud_sdk_python_tat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:30:53.000000 tencentcloud-sdk-python-tat-3.0.937/tencentcloud_sdk_python_tat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:30:53.000000 tencentcloud-sdk-python-tat-3.0.937/tencentcloud_sdk_python_tat.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:53.000000 tencentcloud-sdk-python-tat-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:53.000000 tencentcloud-sdk-python-tat-3.0.937/tencentcloud/tat/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:53.000000 tencentcloud-sdk-python-tat-3.0.937/tencentcloud/tat/v20201028/
--rw-r--r--   0 root         (0) root         (0)    19291 2023-07-18 00:30:53.000000 tencentcloud-sdk-python-tat-3.0.937/tencentcloud/tat/v20201028/tat_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:30:53.000000 tencentcloud-sdk-python-tat-3.0.937/tencentcloud/tat/v20201028/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7342 2023-07-18 00:30:53.000000 tencentcloud-sdk-python-tat-3.0.937/tencentcloud/tat/v20201028/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   120455 2023-07-18 00:30:53.000000 tencentcloud-sdk-python-tat-3.0.937/tencentcloud/tat/v20201028/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:30:53.000000 tencentcloud-sdk-python-tat-3.0.937/tencentcloud/tat/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:30:53.000000 tencentcloud-sdk-python-tat-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:30:53.000000 tencentcloud-sdk-python-tat-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:30:53.000000 tencentcloud-sdk-python-tat-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:30:53.000000 tencentcloud-sdk-python-tat-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:17.000000 tencentcloud-sdk-python-tat-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:48:17.000000 tencentcloud-sdk-python-tat-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:17.000000 tencentcloud-sdk-python-tat-3.0.938/tencentcloud_sdk_python_tat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:48:17.000000 tencentcloud-sdk-python-tat-3.0.938/tencentcloud_sdk_python_tat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:48:17.000000 tencentcloud-sdk-python-tat-3.0.938/tencentcloud_sdk_python_tat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:48:17.000000 tencentcloud-sdk-python-tat-3.0.938/tencentcloud_sdk_python_tat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:48:17.000000 tencentcloud-sdk-python-tat-3.0.938/tencentcloud_sdk_python_tat.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:17.000000 tencentcloud-sdk-python-tat-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:17.000000 tencentcloud-sdk-python-tat-3.0.938/tencentcloud/tat/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:17.000000 tencentcloud-sdk-python-tat-3.0.938/tencentcloud/tat/v20201028/
+-rw-r--r--   0 root         (0) root         (0)    19367 2023-07-19 00:48:17.000000 tencentcloud-sdk-python-tat-3.0.938/tencentcloud/tat/v20201028/tat_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:48:17.000000 tencentcloud-sdk-python-tat-3.0.938/tencentcloud/tat/v20201028/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7342 2023-07-19 00:48:17.000000 tencentcloud-sdk-python-tat-3.0.938/tencentcloud/tat/v20201028/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   120455 2023-07-19 00:48:17.000000 tencentcloud-sdk-python-tat-3.0.938/tencentcloud/tat/v20201028/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:48:17.000000 tencentcloud-sdk-python-tat-3.0.938/tencentcloud/tat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:48:17.000000 tencentcloud-sdk-python-tat-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:48:17.000000 tencentcloud-sdk-python-tat-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:48:17.000000 tencentcloud-sdk-python-tat-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:48:17.000000 tencentcloud-sdk-python-tat-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-tat-3.0.937/setup.py` & `tencentcloud-sdk-python-tat-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tat-3.0.937/tencentcloud_sdk_python_tat.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tat-3.0.938/tencentcloud_sdk_python_tat.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tat
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tat SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tat-3.0.937/tencentcloud/tat/v20201028/tat_client.py` & `tencentcloud-sdk-python-tat-3.0.938/tencentcloud/tat/v20201028/tat_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             model = models.CancelInvocationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCommand(self, request):
         """此接口用于创建命令。
 
         :param request: Request instance for CreateCommand.
         :type request: :class:`tencentcloud.tat.v20201028.models.CreateCommandRequest`
@@ -68,15 +68,15 @@
             model = models.CreateCommandResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateInvoker(self, request):
         """此接口用于创建执行器。
 
         :param request: Request instance for CreateInvoker.
         :type request: :class:`tencentcloud.tat.v20201028.models.CreateInvokerRequest`
@@ -91,15 +91,15 @@
             model = models.CreateInvokerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCommand(self, request):
         """此接口用于删除命令。
         如果命令与执行器关联，则无法被删除。
 
         :param request: Request instance for DeleteCommand.
@@ -115,15 +115,15 @@
             model = models.DeleteCommandResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteInvoker(self, request):
         """此接口用于删除执行器。
 
         :param request: Request instance for DeleteInvoker.
         :type request: :class:`tencentcloud.tat.v20201028.models.DeleteInvokerRequest`
@@ -138,15 +138,15 @@
             model = models.DeleteInvokerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAutomationAgentStatus(self, request):
         """此接口用于查询自动化助手客户端的状态。
 
         :param request: Request instance for DescribeAutomationAgentStatus.
         :type request: :class:`tencentcloud.tat.v20201028.models.DescribeAutomationAgentStatusRequest`
@@ -161,15 +161,15 @@
             model = models.DescribeAutomationAgentStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCommands(self, request):
         """此接口用于查询命令详情。
 
         :param request: Request instance for DescribeCommands.
         :type request: :class:`tencentcloud.tat.v20201028.models.DescribeCommandsRequest`
@@ -184,15 +184,15 @@
             model = models.DescribeCommandsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInvocationTasks(self, request):
         """此接口用于查询执行任务详情。
 
         :param request: Request instance for DescribeInvocationTasks.
         :type request: :class:`tencentcloud.tat.v20201028.models.DescribeInvocationTasksRequest`
@@ -207,15 +207,15 @@
             model = models.DescribeInvocationTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInvocations(self, request):
         """此接口用于查询执行活动详情。
 
         :param request: Request instance for DescribeInvocations.
         :type request: :class:`tencentcloud.tat.v20201028.models.DescribeInvocationsRequest`
@@ -230,15 +230,15 @@
             model = models.DescribeInvocationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInvokerRecords(self, request):
         """此接口用于查询执行器的执行记录。
 
         :param request: Request instance for DescribeInvokerRecords.
         :type request: :class:`tencentcloud.tat.v20201028.models.DescribeInvokerRecordsRequest`
@@ -253,15 +253,15 @@
             model = models.DescribeInvokerRecordsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInvokers(self, request):
         """此接口用于查询执行器信息。
 
         :param request: Request instance for DescribeInvokers.
         :type request: :class:`tencentcloud.tat.v20201028.models.DescribeInvokersRequest`
@@ -276,15 +276,15 @@
             model = models.DescribeInvokersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRegions(self, request):
         """此接口用于查询 TAT 产品后台地域列表。
         RegionState 为 AVAILABLE，代表该地域的 TAT 后台服务已经可用；未返回，代表该地域的 TAT 后台服务尚不可用。
 
         :param request: Request instance for DescribeRegions.
@@ -300,15 +300,15 @@
             model = models.DescribeRegionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableInvoker(self, request):
         """此接口用于停止执行器。
 
         :param request: Request instance for DisableInvoker.
         :type request: :class:`tencentcloud.tat.v20201028.models.DisableInvokerRequest`
@@ -323,15 +323,15 @@
             model = models.DisableInvokerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableInvoker(self, request):
         """此接口用于启用执行器。
 
         :param request: Request instance for EnableInvoker.
         :type request: :class:`tencentcloud.tat.v20201028.models.EnableInvokerRequest`
@@ -346,15 +346,15 @@
             model = models.EnableInvokerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InvokeCommand(self, request):
         """在指定的实例上触发命令，调用成功返回执行活动ID（inv-xxxxxxxx），每个执行活动内部有一个或多个执行任务（invt-xxxxxxxx），每个执行任务代表命令在一台 CVM 或一台 Lighthouse 上的执行记录。
 
         * 如果指定实例未安装 agent，或 agent 不在线，返回失败
         * 如果命令类型与 agent 运行环境不符，返回失败
@@ -375,15 +375,15 @@
             model = models.InvokeCommandResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCommand(self, request):
         """此接口用于修改命令。
 
         :param request: Request instance for ModifyCommand.
         :type request: :class:`tencentcloud.tat.v20201028.models.ModifyCommandRequest`
@@ -398,15 +398,15 @@
             model = models.ModifyCommandResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInvoker(self, request):
         """此接口用于修改执行器。
 
         :param request: Request instance for ModifyInvoker.
         :type request: :class:`tencentcloud.tat.v20201028.models.ModifyInvokerRequest`
@@ -421,15 +421,15 @@
             model = models.ModifyInvokerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PreviewReplacedCommandContent(self, request):
         """此接口用于预览自定义参数替换后的命令内容。不会触发真实执行。
 
         :param request: Request instance for PreviewReplacedCommandContent.
         :type request: :class:`tencentcloud.tat.v20201028.models.PreviewReplacedCommandContentRequest`
@@ -444,15 +444,15 @@
             model = models.PreviewReplacedCommandContentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RunCommand(self, request):
         """执行命令，调用成功返回执行活动ID（inv-xxxxxxxx），每个执行活动内部有一个或多个执行任务（invt-xxxxxxxx），每个执行任务代表命令在一台 CVM 或一台 Lighthouse 上的执行记录。
 
         * 如果指定实例未安装 agent，或 agent 不在线，返回失败
         * 如果命令类型与 agent 运行环境不符，返回失败
@@ -473,8 +473,8 @@
             model = models.RunCommandResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tat-3.0.937/tencentcloud/tat/v20201028/errorcodes.py` & `tencentcloud-sdk-python-tat-3.0.938/tencentcloud/tat/v20201028/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tat-3.0.937/tencentcloud/tat/v20201028/models.py` & `tencentcloud-sdk-python-tat-3.0.938/tencentcloud/tat/v20201028/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tat-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tat-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tat-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tat-3.0.938/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tat
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tat SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tat-3.0.937/README.rst` & `tencentcloud-sdk-python-tat-3.0.938/README.rst`

 * *Files identical despite different names*

