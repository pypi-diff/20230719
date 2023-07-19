# Comparing `tmp/tencentcloud-sdk-python-eiam-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-eiam-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-eiam-3.0.937.tar", last modified: Tue Jul 18 00:23:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-eiam-3.0.938.tar", last modified: Wed Jul 19 00:38:43 2023, max compression
```

## Comparing `tencentcloud-sdk-python-eiam-3.0.937.tar` & `tencentcloud-sdk-python-eiam-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:28.000000 tencentcloud-sdk-python-eiam-3.0.937/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:28.000000 tencentcloud-sdk-python-eiam-3.0.937/tencentcloud_sdk_python_eiam.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:23:28.000000 tencentcloud-sdk-python-eiam-3.0.937/tencentcloud_sdk_python_eiam.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:23:28.000000 tencentcloud-sdk-python-eiam-3.0.937/tencentcloud_sdk_python_eiam.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:23:28.000000 tencentcloud-sdk-python-eiam-3.0.937/tencentcloud_sdk_python_eiam.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:23:28.000000 tencentcloud-sdk-python-eiam-3.0.937/tencentcloud_sdk_python_eiam.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:23:28.000000 tencentcloud-sdk-python-eiam-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:28.000000 tencentcloud-sdk-python-eiam-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:23:28.000000 tencentcloud-sdk-python-eiam-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:28.000000 tencentcloud-sdk-python-eiam-3.0.937/tencentcloud/eiam/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:28.000000 tencentcloud-sdk-python-eiam-3.0.937/tencentcloud/eiam/v20210420/
--rw-r--r--   0 root         (0) root         (0)    38932 2023-07-18 00:23:28.000000 tencentcloud-sdk-python-eiam-3.0.937/tencentcloud/eiam/v20210420/eiam_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:28.000000 tencentcloud-sdk-python-eiam-3.0.937/tencentcloud/eiam/v20210420/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9938 2023-07-18 00:23:28.000000 tencentcloud-sdk-python-eiam-3.0.937/tencentcloud/eiam/v20210420/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   218794 2023-07-18 00:23:28.000000 tencentcloud-sdk-python-eiam-3.0.937/tencentcloud/eiam/v20210420/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:28.000000 tencentcloud-sdk-python-eiam-3.0.937/tencentcloud/eiam/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:23:28.000000 tencentcloud-sdk-python-eiam-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:23:28.000000 tencentcloud-sdk-python-eiam-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:23:28.000000 tencentcloud-sdk-python-eiam-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:43.000000 tencentcloud-sdk-python-eiam-3.0.938/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:43.000000 tencentcloud-sdk-python-eiam-3.0.938/tencentcloud_sdk_python_eiam.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:38:43.000000 tencentcloud-sdk-python-eiam-3.0.938/tencentcloud_sdk_python_eiam.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:38:43.000000 tencentcloud-sdk-python-eiam-3.0.938/tencentcloud_sdk_python_eiam.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:38:43.000000 tencentcloud-sdk-python-eiam-3.0.938/tencentcloud_sdk_python_eiam.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:38:43.000000 tencentcloud-sdk-python-eiam-3.0.938/tencentcloud_sdk_python_eiam.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:38:43.000000 tencentcloud-sdk-python-eiam-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:43.000000 tencentcloud-sdk-python-eiam-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:38:43.000000 tencentcloud-sdk-python-eiam-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:43.000000 tencentcloud-sdk-python-eiam-3.0.938/tencentcloud/eiam/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:43.000000 tencentcloud-sdk-python-eiam-3.0.938/tencentcloud/eiam/v20210420/
+-rw-r--r--   0 root         (0) root         (0)    39100 2023-07-19 00:38:43.000000 tencentcloud-sdk-python-eiam-3.0.938/tencentcloud/eiam/v20210420/eiam_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:38:43.000000 tencentcloud-sdk-python-eiam-3.0.938/tencentcloud/eiam/v20210420/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9938 2023-07-19 00:38:43.000000 tencentcloud-sdk-python-eiam-3.0.938/tencentcloud/eiam/v20210420/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   218794 2023-07-19 00:38:43.000000 tencentcloud-sdk-python-eiam-3.0.938/tencentcloud/eiam/v20210420/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:38:43.000000 tencentcloud-sdk-python-eiam-3.0.938/tencentcloud/eiam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:38:43.000000 tencentcloud-sdk-python-eiam-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:38:43.000000 tencentcloud-sdk-python-eiam-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:38:43.000000 tencentcloud-sdk-python-eiam-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-eiam-3.0.937/tencentcloud_sdk_python_eiam.egg-info/PKG-INFO` & `tencentcloud-sdk-python-eiam-3.0.938/tencentcloud_sdk_python_eiam.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-eiam
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Eiam SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-eiam-3.0.937/setup.py` & `tencentcloud-sdk-python-eiam-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eiam-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-eiam-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-eiam-3.0.937/tencentcloud/eiam/v20210420/eiam_client.py` & `tencentcloud-sdk-python-eiam-3.0.938/tencentcloud/eiam/v20210420/eiam_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AddAccountToAccountGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddUserToUserGroup(self, request):
         """加入用户到用户组
 
         :param request: Request instance for AddUserToUserGroup.
         :type request: :class:`tencentcloud.eiam.v20210420.models.AddUserToUserGroupRequest`
@@ -65,15 +65,15 @@
             model = models.AddUserToUserGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAccountGroup(self, request):
         """创建账号组
 
         :param request: Request instance for CreateAccountGroup.
         :type request: :class:`tencentcloud.eiam.v20210420.models.CreateAccountGroupRequest`
@@ -88,15 +88,15 @@
             model = models.CreateAccountGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAppAccount(self, request):
         """创建应用账号
 
         :param request: Request instance for CreateAppAccount.
         :type request: :class:`tencentcloud.eiam.v20210420.models.CreateAppAccountRequest`
@@ -111,15 +111,15 @@
             model = models.CreateAppAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOrgNode(self, request):
         """新建一个机构节点
 
         :param request: Request instance for CreateOrgNode.
         :type request: :class:`tencentcloud.eiam.v20210420.models.CreateOrgNodeRequest`
@@ -134,15 +134,15 @@
             model = models.CreateOrgNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateUser(self, request):
         """新建一个用户
 
         :param request: Request instance for CreateUser.
         :type request: :class:`tencentcloud.eiam.v20210420.models.CreateUserRequest`
@@ -157,15 +157,15 @@
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
         """新建用户组
 
         :param request: Request instance for CreateUserGroup.
         :type request: :class:`tencentcloud.eiam.v20210420.models.CreateUserGroupRequest`
@@ -180,15 +180,15 @@
             model = models.CreateUserGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAccountGroup(self, request):
         """删除账号组
 
         :param request: Request instance for DeleteAccountGroup.
         :type request: :class:`tencentcloud.eiam.v20210420.models.DeleteAccountGroupRequest`
@@ -203,15 +203,15 @@
             model = models.DeleteAccountGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAppAccount(self, request):
         """删除应用账号
 
         :param request: Request instance for DeleteAppAccount.
         :type request: :class:`tencentcloud.eiam.v20210420.models.DeleteAppAccountRequest`
@@ -226,15 +226,15 @@
             model = models.DeleteAppAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteOrgNode(self, request):
         """删除一个机构节点
 
         :param request: Request instance for DeleteOrgNode.
         :type request: :class:`tencentcloud.eiam.v20210420.models.DeleteOrgNodeRequest`
@@ -249,15 +249,15 @@
             model = models.DeleteOrgNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteUser(self, request):
         """通过用户名或用户 id 删除用户。
 
         :param request: Request instance for DeleteUser.
         :type request: :class:`tencentcloud.eiam.v20210420.models.DeleteUserRequest`
@@ -272,15 +272,15 @@
             model = models.DeleteUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteUserGroup(self, request):
         """删除一个用户组
 
         :param request: Request instance for DeleteUserGroup.
         :type request: :class:`tencentcloud.eiam.v20210420.models.DeleteUserGroupRequest`
@@ -295,15 +295,15 @@
             model = models.DeleteUserGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteUsers(self, request):
         """批量删除当前节点下的用户。如果出现个别用户删除错误，将不影响其余被勾选用户被删除的操作，同时提示未被删除的用户名称/用户ID。
 
         :param request: Request instance for DeleteUsers.
         :type request: :class:`tencentcloud.eiam.v20210420.models.DeleteUsersRequest`
@@ -318,15 +318,15 @@
             model = models.DeleteUsersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccountGroup(self, request):
         """查询账号组列表
 
         :param request: Request instance for DescribeAccountGroup.
         :type request: :class:`tencentcloud.eiam.v20210420.models.DescribeAccountGroupRequest`
@@ -341,15 +341,15 @@
             model = models.DescribeAccountGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAppAccount(self, request):
         """查询应用账号列表
 
         :param request: Request instance for DescribeAppAccount.
         :type request: :class:`tencentcloud.eiam.v20210420.models.DescribeAppAccountRequest`
@@ -364,15 +364,15 @@
             model = models.DescribeAppAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApplication(self, request):
         """获取一个应用的信息。
 
         :param request: Request instance for DescribeApplication.
         :type request: :class:`tencentcloud.eiam.v20210420.models.DescribeApplicationRequest`
@@ -387,15 +387,15 @@
             model = models.DescribeApplicationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOrgNode(self, request):
         """根据机构节点ID读取机构节点信息
 
         :param request: Request instance for DescribeOrgNode.
         :type request: :class:`tencentcloud.eiam.v20210420.models.DescribeOrgNodeRequest`
@@ -410,15 +410,15 @@
             model = models.DescribeOrgNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOrgResourcesAuthorization(self, request):
         """查询指定机构下的资源授权列表
 
         :param request: Request instance for DescribeOrgResourcesAuthorization.
         :type request: :class:`tencentcloud.eiam.v20210420.models.DescribeOrgResourcesAuthorizationRequest`
@@ -433,15 +433,15 @@
             model = models.DescribeOrgResourcesAuthorizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePublicKey(self, request):
         """获取JWT公钥信息。
 
         :param request: Request instance for DescribePublicKey.
         :type request: :class:`tencentcloud.eiam.v20210420.models.DescribePublicKeyRequest`
@@ -456,15 +456,15 @@
             model = models.DescribePublicKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserGroup(self, request):
         """获取用户组信息
 
         :param request: Request instance for DescribeUserGroup.
         :type request: :class:`tencentcloud.eiam.v20210420.models.DescribeUserGroupRequest`
@@ -479,15 +479,15 @@
             model = models.DescribeUserGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserGroupResourcesAuthorization(self, request):
         """查询指定用户组下的资源授权列表
 
         :param request: Request instance for DescribeUserGroupResourcesAuthorization.
         :type request: :class:`tencentcloud.eiam.v20210420.models.DescribeUserGroupResourcesAuthorizationRequest`
@@ -502,15 +502,15 @@
             model = models.DescribeUserGroupResourcesAuthorizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserInfo(self, request):
         """通过用户名或用户 id 搜索用户
 
         :param request: Request instance for DescribeUserInfo.
         :type request: :class:`tencentcloud.eiam.v20210420.models.DescribeUserInfoRequest`
@@ -525,15 +525,15 @@
             model = models.DescribeUserInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserResourcesAuthorization(self, request):
         """查询指定用户下的资源授权列表
 
         :param request: Request instance for DescribeUserResourcesAuthorization.
         :type request: :class:`tencentcloud.eiam.v20210420.models.DescribeUserResourcesAuthorizationRequest`
@@ -548,15 +548,15 @@
             model = models.DescribeUserResourcesAuthorizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserThirdPartyAccountInfo(self, request):
         """通过用户名或用户 id 获取用户的第三方账号绑定信息。
 
         :param request: Request instance for DescribeUserThirdPartyAccountInfo.
         :type request: :class:`tencentcloud.eiam.v20210420.models.DescribeUserThirdPartyAccountInfoRequest`
@@ -571,15 +571,15 @@
             model = models.DescribeUserThirdPartyAccountInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListAccountInAccountGroup(self, request):
         """获取账号组中的账号列表
 
         :param request: Request instance for ListAccountInAccountGroup.
         :type request: :class:`tencentcloud.eiam.v20210420.models.ListAccountInAccountGroupRequest`
@@ -594,15 +594,15 @@
             model = models.ListAccountInAccountGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListApplicationAuthorizations(self, request):
         """应用授权关系列表（含搜索条件匹配）。
 
         :param request: Request instance for ListApplicationAuthorizations.
         :type request: :class:`tencentcloud.eiam.v20210420.models.ListApplicationAuthorizationsRequest`
@@ -617,15 +617,15 @@
             model = models.ListApplicationAuthorizationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListApplications(self, request):
         """获取应用列表信息。
 
         :param request: Request instance for ListApplications.
         :type request: :class:`tencentcloud.eiam.v20210420.models.ListApplicationsRequest`
@@ -640,15 +640,15 @@
             model = models.ListApplicationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListAuthorizedApplicationsToOrgNode(self, request):
         """通过机构节点ID获得被授权访问的应用列表。
 
         :param request: Request instance for ListAuthorizedApplicationsToOrgNode.
         :type request: :class:`tencentcloud.eiam.v20210420.models.ListAuthorizedApplicationsToOrgNodeRequest`
@@ -663,15 +663,15 @@
             model = models.ListAuthorizedApplicationsToOrgNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListAuthorizedApplicationsToUser(self, request):
         """通过用户ID获得被授权访问的应用列表。
 
         :param request: Request instance for ListAuthorizedApplicationsToUser.
         :type request: :class:`tencentcloud.eiam.v20210420.models.ListAuthorizedApplicationsToUserRequest`
@@ -686,15 +686,15 @@
             model = models.ListAuthorizedApplicationsToUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListAuthorizedApplicationsToUserGroup(self, request):
         """通过用户组ID获得被授权访问的应用列表。
 
         :param request: Request instance for ListAuthorizedApplicationsToUserGroup.
         :type request: :class:`tencentcloud.eiam.v20210420.models.ListAuthorizedApplicationsToUserGroupRequest`
@@ -709,15 +709,15 @@
             model = models.ListAuthorizedApplicationsToUserGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListUserGroups(self, request):
         """获取用户组列表信息（包含查询条件）。
 
         :param request: Request instance for ListUserGroups.
         :type request: :class:`tencentcloud.eiam.v20210420.models.ListUserGroupsRequest`
@@ -732,15 +732,15 @@
             model = models.ListUserGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListUserGroupsOfUser(self, request):
         """获取用户所在的用户组列表
 
         :param request: Request instance for ListUserGroupsOfUser.
         :type request: :class:`tencentcloud.eiam.v20210420.models.ListUserGroupsOfUserRequest`
@@ -755,15 +755,15 @@
             model = models.ListUserGroupsOfUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListUsers(self, request):
         """获取用户列表信息。
 
         :param request: Request instance for ListUsers.
         :type request: :class:`tencentcloud.eiam.v20210420.models.ListUsersRequest`
@@ -778,15 +778,15 @@
             model = models.ListUsersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListUsersInOrgNode(self, request):
         """根据机构节点ID读取节点下用户
 
         :param request: Request instance for ListUsersInOrgNode.
         :type request: :class:`tencentcloud.eiam.v20210420.models.ListUsersInOrgNodeRequest`
@@ -801,15 +801,15 @@
             model = models.ListUsersInOrgNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListUsersInUserGroup(self, request):
         """获取用户组中的用户列表
 
         :param request: Request instance for ListUsersInUserGroup.
         :type request: :class:`tencentcloud.eiam.v20210420.models.ListUsersInUserGroupRequest`
@@ -824,15 +824,15 @@
             model = models.ListUsersInUserGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAccountGroup(self, request):
         """修改账号组
 
         :param request: Request instance for ModifyAccountGroup.
         :type request: :class:`tencentcloud.eiam.v20210420.models.ModifyAccountGroupRequest`
@@ -847,15 +847,15 @@
             model = models.ModifyAccountGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAppAccount(self, request):
         """修改应用账号
 
         :param request: Request instance for ModifyAppAccount.
         :type request: :class:`tencentcloud.eiam.v20210420.models.ModifyAppAccountRequest`
@@ -870,15 +870,15 @@
             model = models.ModifyAppAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyApplication(self, request):
         """更新一个应用的信息
 
         :param request: Request instance for ModifyApplication.
         :type request: :class:`tencentcloud.eiam.v20210420.models.ModifyApplicationRequest`
@@ -893,15 +893,15 @@
             model = models.ModifyApplicationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyUserInfo(self, request):
         """通过用户名或用户 id 冻结用户
 
         :param request: Request instance for ModifyUserInfo.
         :type request: :class:`tencentcloud.eiam.v20210420.models.ModifyUserInfoRequest`
@@ -916,15 +916,15 @@
             model = models.ModifyUserInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RemoveAccountFromAccountGroup(self, request):
         """从账号组中移除账号
 
         :param request: Request instance for RemoveAccountFromAccountGroup.
         :type request: :class:`tencentcloud.eiam.v20210420.models.RemoveAccountFromAccountGroupRequest`
@@ -939,15 +939,15 @@
             model = models.RemoveAccountFromAccountGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RemoveUserFromUserGroup(self, request):
         """从用户组中移除用户
 
         :param request: Request instance for RemoveUserFromUserGroup.
         :type request: :class:`tencentcloud.eiam.v20210420.models.RemoveUserFromUserGroupRequest`
@@ -962,15 +962,15 @@
             model = models.RemoveUserFromUserGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateOrgNode(self, request):
         """新建一个机构节点，
 
         :param request: Request instance for UpdateOrgNode.
         :type request: :class:`tencentcloud.eiam.v20210420.models.UpdateOrgNodeRequest`
@@ -985,8 +985,8 @@
             model = models.UpdateOrgNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-eiam-3.0.937/tencentcloud/eiam/v20210420/errorcodes.py` & `tencentcloud-sdk-python-eiam-3.0.938/tencentcloud/eiam/v20210420/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eiam-3.0.937/tencentcloud/eiam/v20210420/models.py` & `tencentcloud-sdk-python-eiam-3.0.938/tencentcloud/eiam/v20210420/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eiam-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-eiam-3.0.938/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-eiam
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Eiam SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-eiam-3.0.937/README.rst` & `tencentcloud-sdk-python-eiam-3.0.938/README.rst`

 * *Files identical despite different names*

