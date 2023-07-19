# Comparing `tmp/tencentcloud-sdk-python-msp-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-msp-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-msp-3.0.937.tar", last modified: Tue Jul 18 00:27:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-msp-3.0.938.tar", last modified: Wed Jul 19 00:43:19 2023, max compression
```

## Comparing `tencentcloud-sdk-python-msp-3.0.937.tar` & `tencentcloud-sdk-python-msp-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:58.000000 tencentcloud-sdk-python-msp-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:27:58.000000 tencentcloud-sdk-python-msp-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:58.000000 tencentcloud-sdk-python-msp-3.0.937/tencentcloud_sdk_python_msp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:27:58.000000 tencentcloud-sdk-python-msp-3.0.937/tencentcloud_sdk_python_msp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:27:58.000000 tencentcloud-sdk-python-msp-3.0.937/tencentcloud_sdk_python_msp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:27:58.000000 tencentcloud-sdk-python-msp-3.0.937/tencentcloud_sdk_python_msp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:27:58.000000 tencentcloud-sdk-python-msp-3.0.937/tencentcloud_sdk_python_msp.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:58.000000 tencentcloud-sdk-python-msp-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:27:58.000000 tencentcloud-sdk-python-msp-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:58.000000 tencentcloud-sdk-python-msp-3.0.937/tencentcloud/msp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:58.000000 tencentcloud-sdk-python-msp-3.0.937/tencentcloud/msp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:58.000000 tencentcloud-sdk-python-msp-3.0.937/tencentcloud/msp/v20180319/
--rw-r--r--   0 root         (0) root         (0)     7358 2023-07-18 00:27:58.000000 tencentcloud-sdk-python-msp-3.0.937/tencentcloud/msp/v20180319/msp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:58.000000 tencentcloud-sdk-python-msp-3.0.937/tencentcloud/msp/v20180319/__init__.py
--rw-r--r--   0 root         (0) root         (0)      791 2023-07-18 00:27:58.000000 tencentcloud-sdk-python-msp-3.0.937/tencentcloud/msp/v20180319/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    30960 2023-07-18 00:27:58.000000 tencentcloud-sdk-python-msp-3.0.937/tencentcloud/msp/v20180319/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:27:58.000000 tencentcloud-sdk-python-msp-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:27:58.000000 tencentcloud-sdk-python-msp-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:27:58.000000 tencentcloud-sdk-python-msp-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:19.000000 tencentcloud-sdk-python-msp-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:43:18.000000 tencentcloud-sdk-python-msp-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:19.000000 tencentcloud-sdk-python-msp-3.0.938/tencentcloud_sdk_python_msp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:43:19.000000 tencentcloud-sdk-python-msp-3.0.938/tencentcloud_sdk_python_msp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:43:19.000000 tencentcloud-sdk-python-msp-3.0.938/tencentcloud_sdk_python_msp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:43:19.000000 tencentcloud-sdk-python-msp-3.0.938/tencentcloud_sdk_python_msp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:43:19.000000 tencentcloud-sdk-python-msp-3.0.938/tencentcloud_sdk_python_msp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:19.000000 tencentcloud-sdk-python-msp-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:43:18.000000 tencentcloud-sdk-python-msp-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:19.000000 tencentcloud-sdk-python-msp-3.0.938/tencentcloud/msp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:43:18.000000 tencentcloud-sdk-python-msp-3.0.938/tencentcloud/msp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:19.000000 tencentcloud-sdk-python-msp-3.0.938/tencentcloud/msp/v20180319/
+-rw-r--r--   0 root         (0) root         (0)     7386 2023-07-19 00:43:18.000000 tencentcloud-sdk-python-msp-3.0.938/tencentcloud/msp/v20180319/msp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:43:18.000000 tencentcloud-sdk-python-msp-3.0.938/tencentcloud/msp/v20180319/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      791 2023-07-19 00:43:18.000000 tencentcloud-sdk-python-msp-3.0.938/tencentcloud/msp/v20180319/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    30960 2023-07-19 00:43:18.000000 tencentcloud-sdk-python-msp-3.0.938/tencentcloud/msp/v20180319/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:43:19.000000 tencentcloud-sdk-python-msp-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:43:19.000000 tencentcloud-sdk-python-msp-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:43:18.000000 tencentcloud-sdk-python-msp-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-msp-3.0.937/setup.py` & `tencentcloud-sdk-python-msp-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-msp-3.0.937/tencentcloud_sdk_python_msp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-msp-3.0.938/tencentcloud_sdk_python_msp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-msp
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Msp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-msp-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-msp-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-msp-3.0.937/tencentcloud/msp/v20180319/msp_client.py` & `tencentcloud-sdk-python-msp-3.0.938/tencentcloud/msp/v20180319/msp_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.DeregisterMigrationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMigrationTask(self, request):
         """获取指定迁移任务详情
 
         :param request: Request instance for DescribeMigrationTask.
         :type request: :class:`tencentcloud.msp.v20180319.models.DescribeMigrationTaskRequest`
@@ -65,15 +65,15 @@
             model = models.DescribeMigrationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListMigrationProject(self, request):
         """获取迁移项目名称列表
 
         :param request: Request instance for ListMigrationProject.
         :type request: :class:`tencentcloud.msp.v20180319.models.ListMigrationProjectRequest`
@@ -88,15 +88,15 @@
             model = models.ListMigrationProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListMigrationTask(self, request):
         """获取迁移任务列表
 
         :param request: Request instance for ListMigrationTask.
         :type request: :class:`tencentcloud.msp.v20180319.models.ListMigrationTaskRequest`
@@ -111,15 +111,15 @@
             model = models.ListMigrationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyMigrationTaskBelongToProject(self, request):
         """更改迁移任务所属项目
 
         :param request: Request instance for ModifyMigrationTaskBelongToProject.
         :type request: :class:`tencentcloud.msp.v20180319.models.ModifyMigrationTaskBelongToProjectRequest`
@@ -134,15 +134,15 @@
             model = models.ModifyMigrationTaskBelongToProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyMigrationTaskStatus(self, request):
         """更新迁移任务状态
 
         :param request: Request instance for ModifyMigrationTaskStatus.
         :type request: :class:`tencentcloud.msp.v20180319.models.ModifyMigrationTaskStatusRequest`
@@ -157,15 +157,15 @@
             model = models.ModifyMigrationTaskStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RegisterMigrationTask(self, request):
         """注册迁移任务
 
         :param request: Request instance for RegisterMigrationTask.
         :type request: :class:`tencentcloud.msp.v20180319.models.RegisterMigrationTaskRequest`
@@ -180,8 +180,8 @@
             model = models.RegisterMigrationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-msp-3.0.937/tencentcloud/msp/v20180319/errorcodes.py` & `tencentcloud-sdk-python-msp-3.0.938/tencentcloud/msp/v20180319/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-msp-3.0.937/tencentcloud/msp/v20180319/models.py` & `tencentcloud-sdk-python-msp-3.0.938/tencentcloud/msp/v20180319/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-msp-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-msp-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-msp
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Msp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-msp-3.0.937/README.rst` & `tencentcloud-sdk-python-msp-3.0.938/README.rst`

 * *Files identical despite different names*

