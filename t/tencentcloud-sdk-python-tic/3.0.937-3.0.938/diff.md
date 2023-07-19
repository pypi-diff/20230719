# Comparing `tmp/tencentcloud-sdk-python-tic-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tic-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tic-3.0.937.tar", last modified: Tue Jul 18 00:32:51 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tic-3.0.938.tar", last modified: Wed Jul 19 00:50:31 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tic-3.0.937.tar` & `tencentcloud-sdk-python-tic-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:51.000000 tencentcloud-sdk-python-tic-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:32:51.000000 tencentcloud-sdk-python-tic-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:51.000000 tencentcloud-sdk-python-tic-3.0.937/tencentcloud_sdk_python_tic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:32:51.000000 tencentcloud-sdk-python-tic-3.0.937/tencentcloud_sdk_python_tic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:32:51.000000 tencentcloud-sdk-python-tic-3.0.937/tencentcloud_sdk_python_tic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:32:51.000000 tencentcloud-sdk-python-tic-3.0.937/tencentcloud_sdk_python_tic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:32:51.000000 tencentcloud-sdk-python-tic-3.0.937/tencentcloud_sdk_python_tic.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:51.000000 tencentcloud-sdk-python-tic-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:32:51.000000 tencentcloud-sdk-python-tic-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:51.000000 tencentcloud-sdk-python-tic-3.0.937/tencentcloud/tic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:32:51.000000 tencentcloud-sdk-python-tic-3.0.937/tencentcloud/tic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:51.000000 tencentcloud-sdk-python-tic-3.0.937/tencentcloud/tic/v20201117/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:32:51.000000 tencentcloud-sdk-python-tic-3.0.937/tencentcloud/tic/v20201117/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14412 2023-07-18 00:32:51.000000 tencentcloud-sdk-python-tic-3.0.937/tencentcloud/tic/v20201117/tic_client.py
--rw-r--r--   0 root         (0) root         (0)     1450 2023-07-18 00:32:51.000000 tencentcloud-sdk-python-tic-3.0.937/tencentcloud/tic/v20201117/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    43811 2023-07-18 00:32:51.000000 tencentcloud-sdk-python-tic-3.0.937/tencentcloud/tic/v20201117/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:32:51.000000 tencentcloud-sdk-python-tic-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:32:51.000000 tencentcloud-sdk-python-tic-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:32:51.000000 tencentcloud-sdk-python-tic-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:31.000000 tencentcloud-sdk-python-tic-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:50:31.000000 tencentcloud-sdk-python-tic-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:31.000000 tencentcloud-sdk-python-tic-3.0.938/tencentcloud_sdk_python_tic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:50:31.000000 tencentcloud-sdk-python-tic-3.0.938/tencentcloud_sdk_python_tic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:50:31.000000 tencentcloud-sdk-python-tic-3.0.938/tencentcloud_sdk_python_tic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:50:31.000000 tencentcloud-sdk-python-tic-3.0.938/tencentcloud_sdk_python_tic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:50:31.000000 tencentcloud-sdk-python-tic-3.0.938/tencentcloud_sdk_python_tic.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:31.000000 tencentcloud-sdk-python-tic-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:50:31.000000 tencentcloud-sdk-python-tic-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:31.000000 tencentcloud-sdk-python-tic-3.0.938/tencentcloud/tic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:50:31.000000 tencentcloud-sdk-python-tic-3.0.938/tencentcloud/tic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:31.000000 tencentcloud-sdk-python-tic-3.0.938/tencentcloud/tic/v20201117/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:50:31.000000 tencentcloud-sdk-python-tic-3.0.938/tencentcloud/tic/v20201117/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14464 2023-07-19 00:50:31.000000 tencentcloud-sdk-python-tic-3.0.938/tencentcloud/tic/v20201117/tic_client.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-07-19 00:50:31.000000 tencentcloud-sdk-python-tic-3.0.938/tencentcloud/tic/v20201117/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    43811 2023-07-19 00:50:31.000000 tencentcloud-sdk-python-tic-3.0.938/tencentcloud/tic/v20201117/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:50:31.000000 tencentcloud-sdk-python-tic-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:50:31.000000 tencentcloud-sdk-python-tic-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:50:31.000000 tencentcloud-sdk-python-tic-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-tic-3.0.937/setup.py` & `tencentcloud-sdk-python-tic-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tic-3.0.937/tencentcloud_sdk_python_tic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tic-3.0.938/tencentcloud_sdk_python_tic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tic
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tic-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tic-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tic-3.0.937/tencentcloud/tic/v20201117/tic_client.py` & `tencentcloud-sdk-python-tic-3.0.938/tencentcloud/tic/v20201117/tic_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             model = models.ApplyStackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateStack(self, request):
         """本接口（CreateStack）用于通过传递一个COS的terraform zip模版URL来创建一个资源栈。创建资源栈后仍需要用户调用对应的plan, apply, destory执行对应的事件。
 
         :param request: Request instance for CreateStack.
         :type request: :class:`tencentcloud.tic.v20201117.models.CreateStackRequest`
@@ -68,15 +68,15 @@
             model = models.CreateStackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateStackVersion(self, request):
         """本接口（CreateStackVersion）用于给资源栈新增一个HCL模版版本，仅限COS链接，且为zip格式。
 
         :param request: Request instance for CreateStackVersion.
         :type request: :class:`tencentcloud.tic.v20201117.models.CreateStackVersionRequest`
@@ -91,15 +91,15 @@
             model = models.CreateStackVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteStack(self, request):
         """本接口（DeleteStack）用于删除一个资源栈（配置、版本、事件信息）。但不会销毁资源管理的云资源。如果需要销毁资源栈管理的云资源，请调用 DestoryStack 接口销毁云资源。
 
         :param request: Request instance for DeleteStack.
         :type request: :class:`tencentcloud.tic.v20201117.models.DeleteStackRequest`
@@ -114,15 +114,15 @@
             model = models.DeleteStackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteStackVersion(self, request):
         """本接口（DeleteStackVersion）用于删除一个版本，处于PLAN_IN_PROGRESS和APPLY_IN_PROGRESS状态中的版本无法删除。
 
         :param request: Request instance for DeleteStackVersion.
         :type request: :class:`tencentcloud.tic.v20201117.models.DeleteStackVersionRequest`
@@ -137,15 +137,15 @@
             model = models.DeleteStackVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStackEvent(self, request):
         """本接口（DescribeStackEvent）用于获取单个事件详情，尤其是可以得到事件的详细控制台输出文本。
 
         :param request: Request instance for DescribeStackEvent.
         :type request: :class:`tencentcloud.tic.v20201117.models.DescribeStackEventRequest`
@@ -160,15 +160,15 @@
             model = models.DescribeStackEventResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStackEvents(self, request):
         """本接口（DescribeStackEvents）用于查看一个或多个事件详细信息。
 
         - 可以根据事件ID过滤感兴趣的事件
         - 也可以根据版本ID，资源栈ID，事件类型，事件状态过滤事件，过滤信息详细请见过滤器Filter
@@ -187,15 +187,15 @@
             model = models.DescribeStackEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStackVersions(self, request):
         """本接口（DescribeStackVersions）用于查询一个或多个版本的详细信息。
 
         - 可以根据版本ID查询感兴趣的版本
         - 可以根据版本名字和状态来过滤版本，详见过滤器Filter
@@ -214,15 +214,15 @@
             model = models.DescribeStackVersionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStacks(self, request):
         """本接口（DescribeStacks）用于查询一个或多个资源栈的详细信息。
 
         - 可以根据资源栈ID来查询感兴趣的资源栈信息
         - 若参数为空，返回当前用户一定数量（Limit所指定的数量，默认为20）的资源栈
@@ -240,15 +240,15 @@
             model = models.DescribeStacksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DestroyStack(self, request):
         """本接口（DestroyStack）用于删除资源栈下的某个版本所创建的资源。
 
         :param request: Request instance for DestroyStack.
         :type request: :class:`tencentcloud.tic.v20201117.models.DestroyStackRequest`
@@ -263,15 +263,15 @@
             model = models.DestroyStackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PlanStack(self, request):
         """本接口（PlanStack）用于触发资源栈下某个版本的PLAN事件。
 
         - 当版本处于PLAN_IN_PROGRESS或APPLY_IN_PROGRESS状态时，将无法再执行本操作
         - 当版本处于APPLY_COMPLETED状态时，本操作无法执行
@@ -289,15 +289,15 @@
             model = models.PlanStackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateStack(self, request):
         """本接口（UpdateStack）用于更新资源栈的名称和描述。
 
         :param request: Request instance for UpdateStack.
         :type request: :class:`tencentcloud.tic.v20201117.models.UpdateStackRequest`
@@ -312,15 +312,15 @@
             model = models.UpdateStackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateStackVersion(self, request):
         """本接口（UpdateStackVersion）用于更新一个版本的模版内容，名称或描述，模版仅限COS URL，且为zip格式。
 
         :param request: Request instance for UpdateStackVersion.
         :type request: :class:`tencentcloud.tic.v20201117.models.UpdateStackVersionRequest`
@@ -335,8 +335,8 @@
             model = models.UpdateStackVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tic-3.0.937/tencentcloud/tic/v20201117/errorcodes.py` & `tencentcloud-sdk-python-tic-3.0.938/tencentcloud/tic/v20201117/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tic-3.0.937/tencentcloud/tic/v20201117/models.py` & `tencentcloud-sdk-python-tic-3.0.938/tencentcloud/tic/v20201117/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tic-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tic-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tic
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tic-3.0.937/README.rst` & `tencentcloud-sdk-python-tic-3.0.938/README.rst`

 * *Files identical despite different names*

