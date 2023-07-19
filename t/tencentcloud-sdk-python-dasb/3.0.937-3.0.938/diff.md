# Comparing `tmp/tencentcloud-sdk-python-dasb-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-dasb-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dasb-3.0.937.tar", last modified: Tue Jul 18 00:21:55 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dasb-3.0.938.tar", last modified: Wed Jul 19 00:37:08 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dasb-3.0.937.tar` & `tencentcloud-sdk-python-dasb-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:55.000000 tencentcloud-sdk-python-dasb-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:21:55.000000 tencentcloud-sdk-python-dasb-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:55.000000 tencentcloud-sdk-python-dasb-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:55.000000 tencentcloud-sdk-python-dasb-3.0.937/tencentcloud/dasb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:21:55.000000 tencentcloud-sdk-python-dasb-3.0.937/tencentcloud/dasb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:55.000000 tencentcloud-sdk-python-dasb-3.0.937/tencentcloud/dasb/v20191018/
--rw-r--r--   0 root         (0) root         (0)    45577 2023-07-18 00:21:55.000000 tencentcloud-sdk-python-dasb-3.0.937/tencentcloud/dasb/v20191018/dasb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:21:55.000000 tencentcloud-sdk-python-dasb-3.0.937/tencentcloud/dasb/v20191018/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2500 2023-07-18 00:21:55.000000 tencentcloud-sdk-python-dasb-3.0.937/tencentcloud/dasb/v20191018/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   259761 2023-07-18 00:21:55.000000 tencentcloud-sdk-python-dasb-3.0.937/tencentcloud/dasb/v20191018/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:21:55.000000 tencentcloud-sdk-python-dasb-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:21:55.000000 tencentcloud-sdk-python-dasb-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:55.000000 tencentcloud-sdk-python-dasb-3.0.937/tencentcloud_sdk_python_dasb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:21:55.000000 tencentcloud-sdk-python-dasb-3.0.937/tencentcloud_sdk_python_dasb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:21:55.000000 tencentcloud-sdk-python-dasb-3.0.937/tencentcloud_sdk_python_dasb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:21:55.000000 tencentcloud-sdk-python-dasb-3.0.937/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:21:55.000000 tencentcloud-sdk-python-dasb-3.0.937/tencentcloud_sdk_python_dasb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:21:55.000000 tencentcloud-sdk-python-dasb-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:21:55.000000 tencentcloud-sdk-python-dasb-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:08.000000 tencentcloud-sdk-python-dasb-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:37:08.000000 tencentcloud-sdk-python-dasb-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:08.000000 tencentcloud-sdk-python-dasb-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:08.000000 tencentcloud-sdk-python-dasb-3.0.938/tencentcloud/dasb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:37:08.000000 tencentcloud-sdk-python-dasb-3.0.938/tencentcloud/dasb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:08.000000 tencentcloud-sdk-python-dasb-3.0.938/tencentcloud/dasb/v20191018/
+-rw-r--r--   0 root         (0) root         (0)    45781 2023-07-19 00:37:08.000000 tencentcloud-sdk-python-dasb-3.0.938/tencentcloud/dasb/v20191018/dasb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:37:08.000000 tencentcloud-sdk-python-dasb-3.0.938/tencentcloud/dasb/v20191018/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2023-07-19 00:37:08.000000 tencentcloud-sdk-python-dasb-3.0.938/tencentcloud/dasb/v20191018/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   259761 2023-07-19 00:37:08.000000 tencentcloud-sdk-python-dasb-3.0.938/tencentcloud/dasb/v20191018/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:37:08.000000 tencentcloud-sdk-python-dasb-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:37:08.000000 tencentcloud-sdk-python-dasb-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:08.000000 tencentcloud-sdk-python-dasb-3.0.938/tencentcloud_sdk_python_dasb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:37:08.000000 tencentcloud-sdk-python-dasb-3.0.938/tencentcloud_sdk_python_dasb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:37:08.000000 tencentcloud-sdk-python-dasb-3.0.938/tencentcloud_sdk_python_dasb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:37:08.000000 tencentcloud-sdk-python-dasb-3.0.938/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:37:08.000000 tencentcloud-sdk-python-dasb-3.0.938/tencentcloud_sdk_python_dasb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:37:08.000000 tencentcloud-sdk-python-dasb-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:37:08.000000 tencentcloud-sdk-python-dasb-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.937/setup.py` & `tencentcloud-sdk-python-dasb-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dasb-3.0.937/tencentcloud/dasb/v20191018/dasb_client.py` & `tencentcloud-sdk-python-dasb-3.0.938/tencentcloud/dasb/v20191018/dasb_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AddDeviceGroupMembersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddUserGroupMembers(self, request):
         """添加用户组成员
 
         :param request: Request instance for AddUserGroupMembers.
         :type request: :class:`tencentcloud.dasb.v20191018.models.AddUserGroupMembersRequest`
@@ -65,15 +65,15 @@
             model = models.AddUserGroupMembersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindDeviceAccountPassword(self, request):
         """绑定主机账号密码
 
         :param request: Request instance for BindDeviceAccountPassword.
         :type request: :class:`tencentcloud.dasb.v20191018.models.BindDeviceAccountPasswordRequest`
@@ -88,15 +88,15 @@
             model = models.BindDeviceAccountPasswordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindDeviceAccountPrivateKey(self, request):
         """绑定主机账号私钥
 
         :param request: Request instance for BindDeviceAccountPrivateKey.
         :type request: :class:`tencentcloud.dasb.v20191018.models.BindDeviceAccountPrivateKeyRequest`
@@ -111,15 +111,15 @@
             model = models.BindDeviceAccountPrivateKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindDeviceResource(self, request):
         """修改资产绑定的堡垒机服务
 
         :param request: Request instance for BindDeviceResource.
         :type request: :class:`tencentcloud.dasb.v20191018.models.BindDeviceResourceRequest`
@@ -134,15 +134,15 @@
             model = models.BindDeviceResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAcl(self, request):
         """新建访问权限
 
         :param request: Request instance for CreateAcl.
         :type request: :class:`tencentcloud.dasb.v20191018.models.CreateAclRequest`
@@ -157,15 +157,15 @@
             model = models.CreateAclResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAssetSyncJob(self, request):
         """创建手工资产同步任务
 
         :param request: Request instance for CreateAssetSyncJob.
         :type request: :class:`tencentcloud.dasb.v20191018.models.CreateAssetSyncJobRequest`
@@ -180,15 +180,15 @@
             model = models.CreateAssetSyncJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCmdTemplate(self, request):
         """新建高危命令模板
 
         :param request: Request instance for CreateCmdTemplate.
         :type request: :class:`tencentcloud.dasb.v20191018.models.CreateCmdTemplateRequest`
@@ -203,15 +203,15 @@
             model = models.CreateCmdTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDeviceAccount(self, request):
         """新建主机账号
 
         :param request: Request instance for CreateDeviceAccount.
         :type request: :class:`tencentcloud.dasb.v20191018.models.CreateDeviceAccountRequest`
@@ -226,15 +226,15 @@
             model = models.CreateDeviceAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDeviceGroup(self, request):
         """新建资产组
 
         :param request: Request instance for CreateDeviceGroup.
         :type request: :class:`tencentcloud.dasb.v20191018.models.CreateDeviceGroupRequest`
@@ -249,15 +249,15 @@
             model = models.CreateDeviceGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateUser(self, request):
         """新建用户
 
         :param request: Request instance for CreateUser.
         :type request: :class:`tencentcloud.dasb.v20191018.models.CreateUserRequest`
@@ -272,15 +272,15 @@
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
         :type request: :class:`tencentcloud.dasb.v20191018.models.CreateUserGroupRequest`
@@ -295,15 +295,15 @@
             model = models.CreateUserGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAcls(self, request):
         """删除访问权限
 
         :param request: Request instance for DeleteAcls.
         :type request: :class:`tencentcloud.dasb.v20191018.models.DeleteAclsRequest`
@@ -318,15 +318,15 @@
             model = models.DeleteAclsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCmdTemplates(self, request):
         """删除高危命令模板
 
         :param request: Request instance for DeleteCmdTemplates.
         :type request: :class:`tencentcloud.dasb.v20191018.models.DeleteCmdTemplatesRequest`
@@ -341,15 +341,15 @@
             model = models.DeleteCmdTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDeviceAccounts(self, request):
         """删除主机账号
 
         :param request: Request instance for DeleteDeviceAccounts.
         :type request: :class:`tencentcloud.dasb.v20191018.models.DeleteDeviceAccountsRequest`
@@ -364,15 +364,15 @@
             model = models.DeleteDeviceAccountsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDeviceGroupMembers(self, request):
         """删除资产组成员
 
         :param request: Request instance for DeleteDeviceGroupMembers.
         :type request: :class:`tencentcloud.dasb.v20191018.models.DeleteDeviceGroupMembersRequest`
@@ -387,15 +387,15 @@
             model = models.DeleteDeviceGroupMembersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDeviceGroups(self, request):
         """删除资产组
 
         :param request: Request instance for DeleteDeviceGroups.
         :type request: :class:`tencentcloud.dasb.v20191018.models.DeleteDeviceGroupsRequest`
@@ -410,15 +410,15 @@
             model = models.DeleteDeviceGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDevices(self, request):
         """删除主机
 
         :param request: Request instance for DeleteDevices.
         :type request: :class:`tencentcloud.dasb.v20191018.models.DeleteDevicesRequest`
@@ -433,15 +433,15 @@
             model = models.DeleteDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteUserGroupMembers(self, request):
         """删除用户组成员
 
         :param request: Request instance for DeleteUserGroupMembers.
         :type request: :class:`tencentcloud.dasb.v20191018.models.DeleteUserGroupMembersRequest`
@@ -456,15 +456,15 @@
             model = models.DeleteUserGroupMembersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteUserGroups(self, request):
         """删除用户组
 
         :param request: Request instance for DeleteUserGroups.
         :type request: :class:`tencentcloud.dasb.v20191018.models.DeleteUserGroupsRequest`
@@ -479,15 +479,15 @@
             model = models.DeleteUserGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteUsers(self, request):
         """删除用户
 
         :param request: Request instance for DeleteUsers.
         :type request: :class:`tencentcloud.dasb.v20191018.models.DeleteUsersRequest`
@@ -502,15 +502,15 @@
             model = models.DeleteUsersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeployResource(self, request):
         """开通服务，初始化资源，只针对新购资源
 
         :param request: Request instance for DeployResource.
         :type request: :class:`tencentcloud.dasb.v20191018.models.DeployResourceRequest`
@@ -525,15 +525,15 @@
             model = models.DeployResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAcls(self, request):
         """查询访问权限列表
 
         :param request: Request instance for DescribeAcls.
         :type request: :class:`tencentcloud.dasb.v20191018.models.DescribeAclsRequest`
@@ -548,15 +548,15 @@
             model = models.DescribeAclsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetSyncStatus(self, request):
         """查询资产同步状态
 
         :param request: Request instance for DescribeAssetSyncStatus.
         :type request: :class:`tencentcloud.dasb.v20191018.models.DescribeAssetSyncStatusRequest`
@@ -571,15 +571,15 @@
             model = models.DescribeAssetSyncStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCmdTemplates(self, request):
         """查询命令模板列表
 
         :param request: Request instance for DescribeCmdTemplates.
         :type request: :class:`tencentcloud.dasb.v20191018.models.DescribeCmdTemplatesRequest`
@@ -594,15 +594,15 @@
             model = models.DescribeCmdTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDasbImageIds(self, request):
         """获取镜像列表
 
         :param request: Request instance for DescribeDasbImageIds.
         :type request: :class:`tencentcloud.dasb.v20191018.models.DescribeDasbImageIdsRequest`
@@ -617,15 +617,15 @@
             model = models.DescribeDasbImageIdsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceAccounts(self, request):
         """查询主机账号列表
 
         :param request: Request instance for DescribeDeviceAccounts.
         :type request: :class:`tencentcloud.dasb.v20191018.models.DescribeDeviceAccountsRequest`
@@ -640,15 +640,15 @@
             model = models.DescribeDeviceAccountsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceGroupMembers(self, request):
         """查询资产组成员列表
 
         :param request: Request instance for DescribeDeviceGroupMembers.
         :type request: :class:`tencentcloud.dasb.v20191018.models.DescribeDeviceGroupMembersRequest`
@@ -663,15 +663,15 @@
             model = models.DescribeDeviceGroupMembersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceGroups(self, request):
         """查询资产组列表
 
         :param request: Request instance for DescribeDeviceGroups.
         :type request: :class:`tencentcloud.dasb.v20191018.models.DescribeDeviceGroupsRequest`
@@ -686,15 +686,15 @@
             model = models.DescribeDeviceGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDevices(self, request):
         """查询资产列表
 
         :param request: Request instance for DescribeDevices.
         :type request: :class:`tencentcloud.dasb.v20191018.models.DescribeDevicesRequest`
@@ -709,15 +709,15 @@
             model = models.DescribeDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLoginEvent(self, request):
         """查询登录日志
 
         :param request: Request instance for DescribeLoginEvent.
         :type request: :class:`tencentcloud.dasb.v20191018.models.DescribeLoginEventRequest`
@@ -732,15 +732,15 @@
             model = models.DescribeLoginEventResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOperationEvent(self, request):
         """查询操作日志
 
         :param request: Request instance for DescribeOperationEvent.
         :type request: :class:`tencentcloud.dasb.v20191018.models.DescribeOperationEventRequest`
@@ -755,15 +755,15 @@
             model = models.DescribeOperationEventResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResources(self, request):
         """查询用户购买的堡垒机服务信息，包括资源ID、授权点数、VPC、过期时间等。
 
         :param request: Request instance for DescribeResources.
         :type request: :class:`tencentcloud.dasb.v20191018.models.DescribeResourcesRequest`
@@ -778,15 +778,15 @@
             model = models.DescribeResourcesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserGroupMembers(self, request):
         """查询用户组成员列表
 
         :param request: Request instance for DescribeUserGroupMembers.
         :type request: :class:`tencentcloud.dasb.v20191018.models.DescribeUserGroupMembersRequest`
@@ -801,15 +801,15 @@
             model = models.DescribeUserGroupMembersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserGroups(self, request):
         """查询用户组列表
 
         :param request: Request instance for DescribeUserGroups.
         :type request: :class:`tencentcloud.dasb.v20191018.models.DescribeUserGroupsRequest`
@@ -824,15 +824,15 @@
             model = models.DescribeUserGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUsers(self, request):
         """查询用户列表
 
         :param request: Request instance for DescribeUsers.
         :type request: :class:`tencentcloud.dasb.v20191018.models.DescribeUsersRequest`
@@ -847,15 +847,15 @@
             model = models.DescribeUsersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ImportExternalDevice(self, request):
         """导入外部资产信息
 
         :param request: Request instance for ImportExternalDevice.
         :type request: :class:`tencentcloud.dasb.v20191018.models.ImportExternalDeviceRequest`
@@ -870,15 +870,15 @@
             model = models.ImportExternalDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAcl(self, request):
         """修改访问权限
 
         :param request: Request instance for ModifyAcl.
         :type request: :class:`tencentcloud.dasb.v20191018.models.ModifyAclRequest`
@@ -893,15 +893,15 @@
             model = models.ModifyAclResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDevice(self, request):
         """修改资产信息
 
         :param request: Request instance for ModifyDevice.
         :type request: :class:`tencentcloud.dasb.v20191018.models.ModifyDeviceRequest`
@@ -916,15 +916,15 @@
             model = models.ModifyDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDeviceGroup(self, request):
         """修改资产组
 
         :param request: Request instance for ModifyDeviceGroup.
         :type request: :class:`tencentcloud.dasb.v20191018.models.ModifyDeviceGroupRequest`
@@ -939,15 +939,15 @@
             model = models.ModifyDeviceGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyUser(self, request):
         """修改用户信息
 
         :param request: Request instance for ModifyUser.
         :type request: :class:`tencentcloud.dasb.v20191018.models.ModifyUserRequest`
@@ -962,15 +962,15 @@
             model = models.ModifyUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetDeviceAccountPassword(self, request):
         """清除设备账号绑定密码
 
         :param request: Request instance for ResetDeviceAccountPassword.
         :type request: :class:`tencentcloud.dasb.v20191018.models.ResetDeviceAccountPasswordRequest`
@@ -985,15 +985,15 @@
             model = models.ResetDeviceAccountPasswordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetDeviceAccountPrivateKey(self, request):
         """清除设备账号绑定的密钥
 
         :param request: Request instance for ResetDeviceAccountPrivateKey.
         :type request: :class:`tencentcloud.dasb.v20191018.models.ResetDeviceAccountPrivateKeyRequest`
@@ -1008,15 +1008,15 @@
             model = models.ResetDeviceAccountPrivateKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetUser(self, request):
         """重置用户
 
         :param request: Request instance for ResetUser.
         :type request: :class:`tencentcloud.dasb.v20191018.models.ResetUserRequest`
@@ -1031,15 +1031,15 @@
             model = models.ResetUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchAuditLog(self, request):
         """搜索审计日志
 
         :param request: Request instance for SearchAuditLog.
         :type request: :class:`tencentcloud.dasb.v20191018.models.SearchAuditLogRequest`
@@ -1054,15 +1054,15 @@
             model = models.SearchAuditLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchCommand(self, request):
         """命令执行检索
 
         :param request: Request instance for SearchCommand.
         :type request: :class:`tencentcloud.dasb.v20191018.models.SearchCommandRequest`
@@ -1077,15 +1077,15 @@
             model = models.SearchCommandResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchCommandBySid(self, request):
         """根据会话Id搜索Command
 
         :param request: Request instance for SearchCommandBySid.
         :type request: :class:`tencentcloud.dasb.v20191018.models.SearchCommandBySidRequest`
@@ -1100,15 +1100,15 @@
             model = models.SearchCommandBySidResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchFile(self, request):
         """文件传输检索
 
         :param request: Request instance for SearchFile.
         :type request: :class:`tencentcloud.dasb.v20191018.models.SearchFileRequest`
@@ -1123,15 +1123,15 @@
             model = models.SearchFileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchFileBySid(self, request):
         """搜索文件传输会话下文件操作列表
 
         :param request: Request instance for SearchFileBySid.
         :type request: :class:`tencentcloud.dasb.v20191018.models.SearchFileBySidRequest`
@@ -1146,15 +1146,15 @@
             model = models.SearchFileBySidResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchSession(self, request):
         """搜索会话
 
         :param request: Request instance for SearchSession.
         :type request: :class:`tencentcloud.dasb.v20191018.models.SearchSessionRequest`
@@ -1169,15 +1169,15 @@
             model = models.SearchSessionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchSessionCommand(self, request):
         """命令检索
 
         :param request: Request instance for SearchSessionCommand.
         :type request: :class:`tencentcloud.dasb.v20191018.models.SearchSessionCommandRequest`
@@ -1192,8 +1192,8 @@
             model = models.SearchSessionCommandResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.937/tencentcloud/dasb/v20191018/errorcodes.py` & `tencentcloud-sdk-python-dasb-3.0.938/tencentcloud/dasb/v20191018/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dasb-3.0.937/tencentcloud/dasb/v20191018/models.py` & `tencentcloud-sdk-python-dasb-3.0.938/tencentcloud/dasb/v20191018/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dasb-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dasb-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dasb-3.0.937/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dasb-3.0.938/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dasb
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Dasb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-dasb-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dasb
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Dasb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.937/README.rst` & `tencentcloud-sdk-python-dasb-3.0.938/README.rst`

 * *Files identical despite different names*

