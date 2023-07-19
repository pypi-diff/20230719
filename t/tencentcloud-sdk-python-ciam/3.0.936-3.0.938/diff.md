# Comparing `tmp/tencentcloud-sdk-python-ciam-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-ciam-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ciam-3.0.936.tar", last modified: Mon Jul 17 00:20:35 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ciam-3.0.938.tar", last modified: Wed Jul 19 00:24:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ciam-3.0.936.tar` & `tencentcloud-sdk-python-ciam-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:20:35.000000 tencentcloud-sdk-python-ciam-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-17 00:20:35.000000 tencentcloud-sdk-python-ciam-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:20:35.000000 tencentcloud-sdk-python-ciam-3.0.936/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:20:35.000000 tencentcloud-sdk-python-ciam-3.0.936/tencentcloud/ciam/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:20:35.000000 tencentcloud-sdk-python-ciam-3.0.936/tencentcloud/ciam/v20220331/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:20:35.000000 tencentcloud-sdk-python-ciam-3.0.936/tencentcloud/ciam/v20220331/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20629 2023-07-17 00:20:35.000000 tencentcloud-sdk-python-ciam-3.0.936/tencentcloud/ciam/v20220331/ciam_client.py
--rw-r--r--   0 root         (0) root         (0)     8558 2023-07-17 00:20:35.000000 tencentcloud-sdk-python-ciam-3.0.936/tencentcloud/ciam/v20220331/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   139059 2023-07-17 00:20:35.000000 tencentcloud-sdk-python-ciam-3.0.936/tencentcloud/ciam/v20220331/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:20:35.000000 tencentcloud-sdk-python-ciam-3.0.936/tencentcloud/ciam/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:20:35.000000 tencentcloud-sdk-python-ciam-3.0.936/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:20:35.000000 tencentcloud-sdk-python-ciam-3.0.936/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-17 00:20:35.000000 tencentcloud-sdk-python-ciam-3.0.936/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-17 00:20:35.000000 tencentcloud-sdk-python-ciam-3.0.936/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:20:35.000000 tencentcloud-sdk-python-ciam-3.0.936/tencentcloud_sdk_python_ciam.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:20:35.000000 tencentcloud-sdk-python-ciam-3.0.936/tencentcloud_sdk_python_ciam.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-17 00:20:35.000000 tencentcloud-sdk-python-ciam-3.0.936/tencentcloud_sdk_python_ciam.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-17 00:20:35.000000 tencentcloud-sdk-python-ciam-3.0.936/tencentcloud_sdk_python_ciam.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:20:35.000000 tencentcloud-sdk-python-ciam-3.0.936/tencentcloud_sdk_python_ciam.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:07.000000 tencentcloud-sdk-python-ciam-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:24:07.000000 tencentcloud-sdk-python-ciam-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:07.000000 tencentcloud-sdk-python-ciam-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:07.000000 tencentcloud-sdk-python-ciam-3.0.938/tencentcloud/ciam/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:07.000000 tencentcloud-sdk-python-ciam-3.0.938/tencentcloud/ciam/v20220331/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:24:07.000000 tencentcloud-sdk-python-ciam-3.0.938/tencentcloud/ciam/v20220331/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20721 2023-07-19 00:24:07.000000 tencentcloud-sdk-python-ciam-3.0.938/tencentcloud/ciam/v20220331/ciam_client.py
+-rw-r--r--   0 root         (0) root         (0)     8558 2023-07-19 00:24:07.000000 tencentcloud-sdk-python-ciam-3.0.938/tencentcloud/ciam/v20220331/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   139059 2023-07-19 00:24:07.000000 tencentcloud-sdk-python-ciam-3.0.938/tencentcloud/ciam/v20220331/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:24:07.000000 tencentcloud-sdk-python-ciam-3.0.938/tencentcloud/ciam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:24:07.000000 tencentcloud-sdk-python-ciam-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:24:07.000000 tencentcloud-sdk-python-ciam-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:24:07.000000 tencentcloud-sdk-python-ciam-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:24:07.000000 tencentcloud-sdk-python-ciam-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:07.000000 tencentcloud-sdk-python-ciam-3.0.938/tencentcloud_sdk_python_ciam.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:24:07.000000 tencentcloud-sdk-python-ciam-3.0.938/tencentcloud_sdk_python_ciam.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:24:07.000000 tencentcloud-sdk-python-ciam-3.0.938/tencentcloud_sdk_python_ciam.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:24:07.000000 tencentcloud-sdk-python-ciam-3.0.938/tencentcloud_sdk_python_ciam.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:24:07.000000 tencentcloud-sdk-python-ciam-3.0.938/tencentcloud_sdk_python_ciam.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-ciam-3.0.936/setup.py` & `tencentcloud-sdk-python-ciam-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ciam-3.0.936/tencentcloud/ciam/v20220331/ciam_client.py` & `tencentcloud-sdk-python-ciam-3.0.938/tencentcloud/ciam/v20220331/ciam_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateApiImportUserJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFileExportUserJob(self, request):
         """新建文件导出用户任务
 
         :param request: Request instance for CreateFileExportUserJob.
         :type request: :class:`tencentcloud.ciam.v20220331.models.CreateFileExportUserJobRequest`
@@ -65,15 +65,15 @@
             model = models.CreateFileExportUserJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateUser(self, request):
         """创建用户
 
         :param request: Request instance for CreateUser.
         :type request: :class:`tencentcloud.ciam.v20220331.models.CreateUserRequest`
@@ -88,15 +88,15 @@
             model = models.CreateUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateUserGroup(self, request):
         """创建用户组
 
         :param request: Request instance for CreateUserGroup.
         :type request: :class:`tencentcloud.ciam.v20220331.models.CreateUserGroupRequest`
@@ -111,15 +111,15 @@
             model = models.CreateUserGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateUserStore(self, request):
         """创建用户目录
 
         :param request: Request instance for CreateUserStore.
         :type request: :class:`tencentcloud.ciam.v20220331.models.CreateUserStoreRequest`
@@ -134,15 +134,15 @@
             model = models.CreateUserStoreResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteUserGroups(self, request):
         """批量删除用户组
 
         :param request: Request instance for DeleteUserGroups.
         :type request: :class:`tencentcloud.ciam.v20220331.models.DeleteUserGroupsRequest`
@@ -157,15 +157,15 @@
             model = models.DeleteUserGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteUserStore(self, request):
         """删除用户目录
 
         :param request: Request instance for DeleteUserStore.
         :type request: :class:`tencentcloud.ciam.v20220331.models.DeleteUserStoreRequest`
@@ -180,15 +180,15 @@
             model = models.DeleteUserStoreResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteUsers(self, request):
         """批量删除用户
 
         :param request: Request instance for DeleteUsers.
         :type request: :class:`tencentcloud.ciam.v20220331.models.DeleteUsersRequest`
@@ -203,15 +203,15 @@
             model = models.DeleteUsersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUser(self, request):
         """多条件查询用户信息
 
         :param request: Request instance for DescribeUser.
         :type request: :class:`tencentcloud.ciam.v20220331.models.DescribeUserRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserById(self, request):
         """根据ID查询用户信息
 
         :param request: Request instance for DescribeUserById.
         :type request: :class:`tencentcloud.ciam.v20220331.models.DescribeUserByIdRequest`
@@ -249,15 +249,15 @@
             model = models.DescribeUserByIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def LinkAccount(self, request):
         """账号融合
 
         :param request: Request instance for LinkAccount.
         :type request: :class:`tencentcloud.ciam.v20220331.models.LinkAccountRequest`
@@ -272,15 +272,15 @@
             model = models.LinkAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListJobs(self, request):
         """查询任务详情
 
         :param request: Request instance for ListJobs.
         :type request: :class:`tencentcloud.ciam.v20220331.models.ListJobsRequest`
@@ -295,15 +295,15 @@
             model = models.ListJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListLogMessageByCondition(self, request):
         """查询日志信息
 
         :param request: Request instance for ListLogMessageByCondition.
         :type request: :class:`tencentcloud.ciam.v20220331.models.ListLogMessageByConditionRequest`
@@ -318,15 +318,15 @@
             model = models.ListLogMessageByConditionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListUser(self, request):
         """查询用户列表
 
         :param request: Request instance for ListUser.
         :type request: :class:`tencentcloud.ciam.v20220331.models.ListUserRequest`
@@ -341,15 +341,15 @@
             model = models.ListUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListUserByProperty(self, request):
         """根据属性查询用户列表
 
         :param request: Request instance for ListUserByProperty.
         :type request: :class:`tencentcloud.ciam.v20220331.models.ListUserByPropertyRequest`
@@ -364,15 +364,15 @@
             model = models.ListUserByPropertyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListUserGroups(self, request):
         """查询用户组列表
 
         :param request: Request instance for ListUserGroups.
         :type request: :class:`tencentcloud.ciam.v20220331.models.ListUserGroupsRequest`
@@ -387,15 +387,15 @@
             model = models.ListUserGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListUserStore(self, request):
         """查询用户目录列表
 
         :param request: Request instance for ListUserStore.
         :type request: :class:`tencentcloud.ciam.v20220331.models.ListUserStoreRequest`
@@ -410,15 +410,15 @@
             model = models.ListUserStoreResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetPassword(self, request):
         """重置用户密码
 
         :param request: Request instance for ResetPassword.
         :type request: :class:`tencentcloud.ciam.v20220331.models.ResetPasswordRequest`
@@ -433,15 +433,15 @@
             model = models.ResetPasswordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetPassword(self, request):
         """设置用户密码
 
         :param request: Request instance for SetPassword.
         :type request: :class:`tencentcloud.ciam.v20220331.models.SetPasswordRequest`
@@ -456,15 +456,15 @@
             model = models.SetPasswordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateUser(self, request):
         """更新用户
 
         :param request: Request instance for UpdateUser.
         :type request: :class:`tencentcloud.ciam.v20220331.models.UpdateUserRequest`
@@ -479,15 +479,15 @@
             model = models.UpdateUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateUserGroup(self, request):
         """更新用户组
 
         :param request: Request instance for UpdateUserGroup.
         :type request: :class:`tencentcloud.ciam.v20220331.models.UpdateUserGroupRequest`
@@ -502,15 +502,15 @@
             model = models.UpdateUserGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateUserStatus(self, request):
         """更新用户状态
 
         :param request: Request instance for UpdateUserStatus.
         :type request: :class:`tencentcloud.ciam.v20220331.models.UpdateUserStatusRequest`
@@ -525,15 +525,15 @@
             model = models.UpdateUserStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateUserStore(self, request):
         """更新用户目录
 
         :param request: Request instance for UpdateUserStore.
         :type request: :class:`tencentcloud.ciam.v20220331.models.UpdateUserStoreRequest`
@@ -548,8 +548,8 @@
             model = models.UpdateUserStoreResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-ciam-3.0.936/tencentcloud/ciam/v20220331/errorcodes.py` & `tencentcloud-sdk-python-ciam-3.0.938/tencentcloud/ciam/v20220331/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ciam-3.0.936/tencentcloud/ciam/v20220331/models.py` & `tencentcloud-sdk-python-ciam-3.0.938/tencentcloud/ciam/v20220331/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ciam-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ciam-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ciam-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-ciam-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ciam
-Version: 3.0.936
+Version: 3.0.938
 Summary: Tencent Cloud Ciam SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ciam-3.0.936/README.rst` & `tencentcloud-sdk-python-ciam-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ciam-3.0.936/tencentcloud_sdk_python_ciam.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ciam-3.0.938/tencentcloud_sdk_python_ciam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ciam
-Version: 3.0.936
+Version: 3.0.938
 Summary: Tencent Cloud Ciam SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

