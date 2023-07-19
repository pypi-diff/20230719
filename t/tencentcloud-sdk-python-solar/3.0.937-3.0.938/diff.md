# Comparing `tmp/tencentcloud-sdk-python-solar-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-solar-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-solar-3.0.937.tar", last modified: Tue Jul 18 00:30:05 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-solar-3.0.938.tar", last modified: Wed Jul 19 00:45:18 2023, max compression
```

## Comparing `tencentcloud-sdk-python-solar-3.0.937.tar` & `tencentcloud-sdk-python-solar-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:05.000000 tencentcloud-sdk-python-solar-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-18 00:30:05.000000 tencentcloud-sdk-python-solar-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:05.000000 tencentcloud-sdk-python-solar-3.0.937/tencentcloud_sdk_python_solar.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:30:05.000000 tencentcloud-sdk-python-solar-3.0.937/tencentcloud_sdk_python_solar.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-07-18 00:30:05.000000 tencentcloud-sdk-python-solar-3.0.937/tencentcloud_sdk_python_solar.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:30:05.000000 tencentcloud-sdk-python-solar-3.0.937/tencentcloud_sdk_python_solar.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:30:05.000000 tencentcloud-sdk-python-solar-3.0.937/tencentcloud_sdk_python_solar.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:05.000000 tencentcloud-sdk-python-solar-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:30:05.000000 tencentcloud-sdk-python-solar-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:05.000000 tencentcloud-sdk-python-solar-3.0.937/tencentcloud/solar/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:30:05.000000 tencentcloud-sdk-python-solar-3.0.937/tencentcloud/solar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:05.000000 tencentcloud-sdk-python-solar-3.0.937/tencentcloud/solar/v20181011/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:30:05.000000 tencentcloud-sdk-python-solar-3.0.937/tencentcloud/solar/v20181011/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-07-18 00:30:05.000000 tencentcloud-sdk-python-solar-3.0.937/tencentcloud/solar/v20181011/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    15814 2023-07-18 00:30:05.000000 tencentcloud-sdk-python-solar-3.0.937/tencentcloud/solar/v20181011/solar_client.py
--rw-r--r--   0 root         (0) root         (0)    88391 2023-07-18 00:30:05.000000 tencentcloud-sdk-python-solar-3.0.937/tencentcloud/solar/v20181011/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:30:05.000000 tencentcloud-sdk-python-solar-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:30:05.000000 tencentcloud-sdk-python-solar-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-18 00:30:05.000000 tencentcloud-sdk-python-solar-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:18.000000 tencentcloud-sdk-python-solar-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-19 00:45:18.000000 tencentcloud-sdk-python-solar-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:18.000000 tencentcloud-sdk-python-solar-3.0.938/tencentcloud_sdk_python_solar.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:45:18.000000 tencentcloud-sdk-python-solar-3.0.938/tencentcloud_sdk_python_solar.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-07-19 00:45:18.000000 tencentcloud-sdk-python-solar-3.0.938/tencentcloud_sdk_python_solar.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:45:18.000000 tencentcloud-sdk-python-solar-3.0.938/tencentcloud_sdk_python_solar.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:45:18.000000 tencentcloud-sdk-python-solar-3.0.938/tencentcloud_sdk_python_solar.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:18.000000 tencentcloud-sdk-python-solar-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:45:18.000000 tencentcloud-sdk-python-solar-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:18.000000 tencentcloud-sdk-python-solar-3.0.938/tencentcloud/solar/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:45:18.000000 tencentcloud-sdk-python-solar-3.0.938/tencentcloud/solar/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:18.000000 tencentcloud-sdk-python-solar-3.0.938/tencentcloud/solar/v20181011/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:45:18.000000 tencentcloud-sdk-python-solar-3.0.938/tencentcloud/solar/v20181011/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-07-19 00:45:18.000000 tencentcloud-sdk-python-solar-3.0.938/tencentcloud/solar/v20181011/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    15882 2023-07-19 00:45:18.000000 tencentcloud-sdk-python-solar-3.0.938/tencentcloud/solar/v20181011/solar_client.py
+-rw-r--r--   0 root         (0) root         (0)    88391 2023-07-19 00:45:18.000000 tencentcloud-sdk-python-solar-3.0.938/tencentcloud/solar/v20181011/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:45:18.000000 tencentcloud-sdk-python-solar-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:45:18.000000 tencentcloud-sdk-python-solar-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-19 00:45:18.000000 tencentcloud-sdk-python-solar-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-solar-3.0.937/setup.py` & `tencentcloud-sdk-python-solar-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-solar-3.0.937/tencentcloud_sdk_python_solar.egg-info/PKG-INFO` & `tencentcloud-sdk-python-solar-3.0.938/tencentcloud_sdk_python_solar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-solar
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Solar SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-solar-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-solar-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-solar-3.0.937/tencentcloud/solar/v20181011/errorcodes.py` & `tencentcloud-sdk-python-solar-3.0.938/tencentcloud/solar/v20181011/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-solar-3.0.937/tencentcloud/solar/v20181011/solar_client.py` & `tencentcloud-sdk-python-solar-3.0.938/tencentcloud/solar/v20181011/solar_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CheckStaffChUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CopyActivityChannel(self, request):
         """复制活动渠道的策略
 
         :param request: Request instance for CopyActivityChannel.
         :type request: :class:`tencentcloud.solar.v20181011.models.CopyActivityChannelRequest`
@@ -65,15 +65,15 @@
             model = models.CopyActivityChannelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateProject(self, request):
         """创建项目
 
         :param request: Request instance for CreateProject.
         :type request: :class:`tencentcloud.solar.v20181011.models.CreateProjectRequest`
@@ -88,15 +88,15 @@
             model = models.CreateProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSubProject(self, request):
         """创建子项目
 
         :param request: Request instance for CreateSubProject.
         :type request: :class:`tencentcloud.solar.v20181011.models.CreateSubProjectRequest`
@@ -111,15 +111,15 @@
             model = models.CreateSubProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteProject(self, request):
         """删除项目
 
         :param request: Request instance for DeleteProject.
         :type request: :class:`tencentcloud.solar.v20181011.models.DeleteProjectRequest`
@@ -134,15 +134,15 @@
             model = models.DeleteProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCustomer(self, request):
         """客户档案查询客户详情
 
         :param request: Request instance for DescribeCustomer.
         :type request: :class:`tencentcloud.solar.v20181011.models.DescribeCustomerRequest`
@@ -157,15 +157,15 @@
             model = models.DescribeCustomerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCustomers(self, request):
         """查询客户档案列表
 
         :param request: Request instance for DescribeCustomers.
         :type request: :class:`tencentcloud.solar.v20181011.models.DescribeCustomersRequest`
@@ -180,15 +180,15 @@
             model = models.DescribeCustomersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProject(self, request):
         """项目详情展示
 
         :param request: Request instance for DescribeProject.
         :type request: :class:`tencentcloud.solar.v20181011.models.DescribeProjectRequest`
@@ -203,15 +203,15 @@
             model = models.DescribeProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProjectStock(self, request):
         """项目库存详情
 
         :param request: Request instance for DescribeProjectStock.
         :type request: :class:`tencentcloud.solar.v20181011.models.DescribeProjectStockRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeProjectStockResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProjects(self, request):
         """项目列表展示
 
         :param request: Request instance for DescribeProjects.
         :type request: :class:`tencentcloud.solar.v20181011.models.DescribeProjectsRequest`
@@ -249,15 +249,15 @@
             model = models.DescribeProjectsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourceTemplateHeaders(self, request):
         """素材查询服务号模板的列表（样例）
 
         :param request: Request instance for DescribeResourceTemplateHeaders.
         :type request: :class:`tencentcloud.solar.v20181011.models.DescribeResourceTemplateHeadersRequest`
@@ -272,15 +272,15 @@
             model = models.DescribeResourceTemplateHeadersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSubProject(self, request):
         """子项目详情
 
         :param request: Request instance for DescribeSubProject.
         :type request: :class:`tencentcloud.solar.v20181011.models.DescribeSubProjectRequest`
@@ -295,15 +295,15 @@
             model = models.DescribeSubProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExpireFlow(self, request):
         """把审批中的工单置为已失效
 
         :param request: Request instance for ExpireFlow.
         :type request: :class:`tencentcloud.solar.v20181011.models.ExpireFlowRequest`
@@ -318,15 +318,15 @@
             model = models.ExpireFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyProject(self, request):
         """修改项目
 
         :param request: Request instance for ModifyProject.
         :type request: :class:`tencentcloud.solar.v20181011.models.ModifyProjectRequest`
@@ -341,15 +341,15 @@
             model = models.ModifyProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OffLineProject(self, request):
         """下线项目
 
         :param request: Request instance for OffLineProject.
         :type request: :class:`tencentcloud.solar.v20181011.models.OffLineProjectRequest`
@@ -364,15 +364,15 @@
             model = models.OffLineProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReplenishProjectStock(self, request):
         """补充子项目库存
 
         :param request: Request instance for ReplenishProjectStock.
         :type request: :class:`tencentcloud.solar.v20181011.models.ReplenishProjectStockRequest`
@@ -387,15 +387,15 @@
             model = models.ReplenishProjectStockResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SendWxTouchTask(self, request):
         """发送企业微信触达任务
 
         :param request: Request instance for SendWxTouchTask.
         :type request: :class:`tencentcloud.solar.v20181011.models.SendWxTouchTaskRequest`
@@ -410,8 +410,8 @@
             model = models.SendWxTouchTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-solar-3.0.937/tencentcloud/solar/v20181011/models.py` & `tencentcloud-sdk-python-solar-3.0.938/tencentcloud/solar/v20181011/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-solar-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-solar-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-solar
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Solar SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-solar-3.0.937/README.rst` & `tencentcloud-sdk-python-solar-3.0.938/README.rst`

 * *Files identical despite different names*

