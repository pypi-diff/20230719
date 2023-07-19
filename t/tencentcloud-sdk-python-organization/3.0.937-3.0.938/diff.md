# Comparing `tmp/tencentcloud-sdk-python-organization-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-organization-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-organization-3.0.937.tar", last modified: Tue Jul 18 00:28:32 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-organization-3.0.938.tar", last modified: Wed Jul 19 00:43:52 2023, max compression
```

## Comparing `tencentcloud-sdk-python-organization-3.0.937.tar` & `tencentcloud-sdk-python-organization-3.0.938.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:32.000000 tencentcloud-sdk-python-organization-3.0.937/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:32.000000 tencentcloud-sdk-python-organization-3.0.937/tencentcloud_sdk_python_organization.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:28:32.000000 tencentcloud-sdk-python-organization-3.0.937/tencentcloud_sdk_python_organization.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      738 2023-07-18 00:28:32.000000 tencentcloud-sdk-python-organization-3.0.937/tencentcloud_sdk_python_organization.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1704 2023-07-18 00:28:32.000000 tencentcloud-sdk-python-organization-3.0.937/tencentcloud_sdk_python_organization.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:28:32.000000 tencentcloud-sdk-python-organization-3.0.937/tencentcloud_sdk_python_organization.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1024 2023-07-18 00:28:32.000000 tencentcloud-sdk-python-organization-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:32.000000 tencentcloud-sdk-python-organization-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:28:32.000000 tencentcloud-sdk-python-organization-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:32.000000 tencentcloud-sdk-python-organization-3.0.937/tencentcloud/organization/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:32.000000 tencentcloud-sdk-python-organization-3.0.937/tencentcloud/organization/v20181225/
--rw-r--r--   0 root         (0) root         (0)    19620 2023-07-18 00:28:32.000000 tencentcloud-sdk-python-organization-3.0.937/tencentcloud/organization/v20181225/organization_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:32.000000 tencentcloud-sdk-python-organization-3.0.937/tencentcloud/organization/v20181225/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3243 2023-07-18 00:28:32.000000 tencentcloud-sdk-python-organization-3.0.937/tencentcloud/organization/v20181225/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    46488 2023-07-18 00:28:32.000000 tencentcloud-sdk-python-organization-3.0.937/tencentcloud/organization/v20181225/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:32.000000 tencentcloud-sdk-python-organization-3.0.937/tencentcloud/organization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:32.000000 tencentcloud-sdk-python-organization-3.0.937/tencentcloud/organization/v20210331/
--rw-r--r--   0 root         (0) root         (0)    24418 2023-07-18 00:28:32.000000 tencentcloud-sdk-python-organization-3.0.937/tencentcloud/organization/v20210331/organization_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:32.000000 tencentcloud-sdk-python-organization-3.0.937/tencentcloud/organization/v20210331/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10778 2023-07-18 00:28:32.000000 tencentcloud-sdk-python-organization-3.0.937/tencentcloud/organization/v20210331/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   118580 2023-07-18 00:28:32.000000 tencentcloud-sdk-python-organization-3.0.937/tencentcloud/organization/v20210331/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:28:32.000000 tencentcloud-sdk-python-organization-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1704 2023-07-18 00:28:32.000000 tencentcloud-sdk-python-organization-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      764 2023-07-18 00:28:32.000000 tencentcloud-sdk-python-organization-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:52.000000 tencentcloud-sdk-python-organization-3.0.938/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:52.000000 tencentcloud-sdk-python-organization-3.0.938/tencentcloud_sdk_python_organization.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:43:52.000000 tencentcloud-sdk-python-organization-3.0.938/tencentcloud_sdk_python_organization.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      738 2023-07-19 00:43:52.000000 tencentcloud-sdk-python-organization-3.0.938/tencentcloud_sdk_python_organization.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-07-19 00:43:52.000000 tencentcloud-sdk-python-organization-3.0.938/tencentcloud_sdk_python_organization.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:43:52.000000 tencentcloud-sdk-python-organization-3.0.938/tencentcloud_sdk_python_organization.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-07-19 00:43:52.000000 tencentcloud-sdk-python-organization-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:52.000000 tencentcloud-sdk-python-organization-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:43:52.000000 tencentcloud-sdk-python-organization-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:52.000000 tencentcloud-sdk-python-organization-3.0.938/tencentcloud/organization/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:52.000000 tencentcloud-sdk-python-organization-3.0.938/tencentcloud/organization/v20181225/
+-rw-r--r--   0 root         (0) root         (0)    19700 2023-07-19 00:43:52.000000 tencentcloud-sdk-python-organization-3.0.938/tencentcloud/organization/v20181225/organization_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:43:52.000000 tencentcloud-sdk-python-organization-3.0.938/tencentcloud/organization/v20181225/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3243 2023-07-19 00:43:52.000000 tencentcloud-sdk-python-organization-3.0.938/tencentcloud/organization/v20181225/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    46488 2023-07-19 00:43:52.000000 tencentcloud-sdk-python-organization-3.0.938/tencentcloud/organization/v20181225/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:43:52.000000 tencentcloud-sdk-python-organization-3.0.938/tencentcloud/organization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:52.000000 tencentcloud-sdk-python-organization-3.0.938/tencentcloud/organization/v20210331/
+-rw-r--r--   0 root         (0) root         (0)    24514 2023-07-19 00:43:52.000000 tencentcloud-sdk-python-organization-3.0.938/tencentcloud/organization/v20210331/organization_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:43:52.000000 tencentcloud-sdk-python-organization-3.0.938/tencentcloud/organization/v20210331/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10778 2023-07-19 00:43:52.000000 tencentcloud-sdk-python-organization-3.0.938/tencentcloud/organization/v20210331/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   118580 2023-07-19 00:43:52.000000 tencentcloud-sdk-python-organization-3.0.938/tencentcloud/organization/v20210331/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:43:52.000000 tencentcloud-sdk-python-organization-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-07-19 00:43:52.000000 tencentcloud-sdk-python-organization-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      764 2023-07-19 00:43:52.000000 tencentcloud-sdk-python-organization-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-organization-3.0.937/tencentcloud_sdk_python_organization.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-organization-3.0.938/tencentcloud_sdk_python_organization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.937/tencentcloud_sdk_python_organization.egg-info/PKG-INFO` & `tencentcloud-sdk-python-organization-3.0.938/tencentcloud_sdk_python_organization.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-organization
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Organization SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-organization-3.0.937/setup.py` & `tencentcloud-sdk-python-organization-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-organization-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-organization-3.0.937/tencentcloud/organization/v20181225/organization_client.py` & `tencentcloud-sdk-python-organization-3.0.938/tencentcloud/organization/v20181225/organization_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AcceptOrganizationInvitationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddOrganizationNode(self, request):
         """添加企业组织单元
 
         :param request: Request instance for AddOrganizationNode.
         :type request: :class:`tencentcloud.organization.v20181225.models.AddOrganizationNodeRequest`
@@ -65,15 +65,15 @@
             model = models.AddOrganizationNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelOrganizationInvitation(self, request):
         """取消企业组织邀请
 
         :param request: Request instance for CancelOrganizationInvitation.
         :type request: :class:`tencentcloud.organization.v20181225.models.CancelOrganizationInvitationRequest`
@@ -88,15 +88,15 @@
             model = models.CancelOrganizationInvitationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOrganization(self, request):
         """创建企业组织
 
         :param request: Request instance for CreateOrganization.
         :type request: :class:`tencentcloud.organization.v20181225.models.CreateOrganizationRequest`
@@ -111,15 +111,15 @@
             model = models.CreateOrganizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteOrganization(self, request):
         """删除企业组织
 
         :param request: Request instance for DeleteOrganization.
         :type request: :class:`tencentcloud.organization.v20181225.models.DeleteOrganizationRequest`
@@ -134,15 +134,15 @@
             model = models.DeleteOrganizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteOrganizationMemberFromNode(self, request):
         """删除企业组织成员
 
         :param request: Request instance for DeleteOrganizationMemberFromNode.
         :type request: :class:`tencentcloud.organization.v20181225.models.DeleteOrganizationMemberFromNodeRequest`
@@ -157,15 +157,15 @@
             model = models.DeleteOrganizationMemberFromNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteOrganizationMembers(self, request):
         """批量删除企业组织成员
 
         :param request: Request instance for DeleteOrganizationMembers.
         :type request: :class:`tencentcloud.organization.v20181225.models.DeleteOrganizationMembersRequest`
@@ -180,15 +180,15 @@
             model = models.DeleteOrganizationMembersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteOrganizationNodes(self, request):
         """批量删除企业组织单元
 
         :param request: Request instance for DeleteOrganizationNodes.
         :type request: :class:`tencentcloud.organization.v20181225.models.DeleteOrganizationNodesRequest`
@@ -203,15 +203,15 @@
             model = models.DeleteOrganizationNodesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DenyOrganizationInvitation(self, request):
         """拒绝企业组织邀请
 
         :param request: Request instance for DenyOrganizationInvitation.
         :type request: :class:`tencentcloud.organization.v20181225.models.DenyOrganizationInvitationRequest`
@@ -226,15 +226,15 @@
             model = models.DenyOrganizationInvitationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetOrganization(self, request):
         """获取企业组织信息
 
         :param request: Request instance for GetOrganization.
         :type request: :class:`tencentcloud.organization.v20181225.models.GetOrganizationRequest`
@@ -249,15 +249,15 @@
             model = models.GetOrganizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetOrganizationMember(self, request):
         """获取企业组织成员
 
         :param request: Request instance for GetOrganizationMember.
         :type request: :class:`tencentcloud.organization.v20181225.models.GetOrganizationMemberRequest`
@@ -272,15 +272,15 @@
             model = models.GetOrganizationMemberResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListOrganizationInvitations(self, request):
         """获取邀请信息列表
 
         :param request: Request instance for ListOrganizationInvitations.
         :type request: :class:`tencentcloud.organization.v20181225.models.ListOrganizationInvitationsRequest`
@@ -295,15 +295,15 @@
             model = models.ListOrganizationInvitationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListOrganizationMembers(self, request):
         """获取企业组织成员列表
 
         :param request: Request instance for ListOrganizationMembers.
         :type request: :class:`tencentcloud.organization.v20181225.models.ListOrganizationMembersRequest`
@@ -318,15 +318,15 @@
             model = models.ListOrganizationMembersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListOrganizationNodeMembers(self, request):
         """获取企业组织单元成员列表
 
         :param request: Request instance for ListOrganizationNodeMembers.
         :type request: :class:`tencentcloud.organization.v20181225.models.ListOrganizationNodeMembersRequest`
@@ -341,15 +341,15 @@
             model = models.ListOrganizationNodeMembersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListOrganizationNodes(self, request):
         """获取企业组织单元列表
 
         :param request: Request instance for ListOrganizationNodes.
         :type request: :class:`tencentcloud.organization.v20181225.models.ListOrganizationNodesRequest`
@@ -364,15 +364,15 @@
             model = models.ListOrganizationNodesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def MoveOrganizationMembersToNode(self, request):
         """移动成员到指定企业组织单元
 
         :param request: Request instance for MoveOrganizationMembersToNode.
         :type request: :class:`tencentcloud.organization.v20181225.models.MoveOrganizationMembersToNodeRequest`
@@ -387,15 +387,15 @@
             model = models.MoveOrganizationMembersToNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QuitOrganization(self, request):
         """退出企业组织
 
         :param request: Request instance for QuitOrganization.
         :type request: :class:`tencentcloud.organization.v20181225.models.QuitOrganizationRequest`
@@ -410,15 +410,15 @@
             model = models.QuitOrganizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SendOrganizationInvitation(self, request):
         """发送企业组织邀请
 
         :param request: Request instance for SendOrganizationInvitation.
         :type request: :class:`tencentcloud.organization.v20181225.models.SendOrganizationInvitationRequest`
@@ -433,15 +433,15 @@
             model = models.SendOrganizationInvitationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateOrganizationMember(self, request):
         """更新企业成员信息
 
         :param request: Request instance for UpdateOrganizationMember.
         :type request: :class:`tencentcloud.organization.v20181225.models.UpdateOrganizationMemberRequest`
@@ -456,15 +456,15 @@
             model = models.UpdateOrganizationMemberResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateOrganizationNode(self, request):
         """更新企业组织单元
 
         :param request: Request instance for UpdateOrganizationNode.
         :type request: :class:`tencentcloud.organization.v20181225.models.UpdateOrganizationNodeRequest`
@@ -479,8 +479,8 @@
             model = models.UpdateOrganizationNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-organization-3.0.937/tencentcloud/organization/v20181225/errorcodes.py` & `tencentcloud-sdk-python-organization-3.0.938/tencentcloud/organization/v20181225/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.937/tencentcloud/organization/v20181225/models.py` & `tencentcloud-sdk-python-organization-3.0.938/tencentcloud/organization/v20181225/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.937/tencentcloud/organization/v20210331/organization_client.py` & `tencentcloud-sdk-python-organization-3.0.938/tencentcloud/organization/v20210331/organization_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AddOrganizationMemberEmailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddOrganizationNode(self, request):
         """添加企业组织节点
 
         :param request: Request instance for AddOrganizationNode.
         :type request: :class:`tencentcloud.organization.v20210331.models.AddOrganizationNodeRequest`
@@ -65,15 +65,15 @@
             model = models.AddOrganizationNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindOrganizationMemberAuthAccount(self, request):
         """绑定组织成员和组织管理员子账号的授权关系
 
         :param request: Request instance for BindOrganizationMemberAuthAccount.
         :type request: :class:`tencentcloud.organization.v20210331.models.BindOrganizationMemberAuthAccountRequest`
@@ -88,15 +88,15 @@
             model = models.BindOrganizationMemberAuthAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelOrganizationMemberAuthAccount(self, request):
         """取消组织成员和组织管理员子账号的授权关系
 
         :param request: Request instance for CancelOrganizationMemberAuthAccount.
         :type request: :class:`tencentcloud.organization.v20210331.models.CancelOrganizationMemberAuthAccountRequest`
@@ -111,15 +111,15 @@
             model = models.CancelOrganizationMemberAuthAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOrganizationMember(self, request):
         """创建组织成员
 
         :param request: Request instance for CreateOrganizationMember.
         :type request: :class:`tencentcloud.organization.v20210331.models.CreateOrganizationMemberRequest`
@@ -134,15 +134,15 @@
             model = models.CreateOrganizationMemberResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOrganizationMemberPolicy(self, request):
         """创建组织成员访问授权策略
 
         :param request: Request instance for CreateOrganizationMemberPolicy.
         :type request: :class:`tencentcloud.organization.v20210331.models.CreateOrganizationMemberPolicyRequest`
@@ -157,15 +157,15 @@
             model = models.CreateOrganizationMemberPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteOrganizationMembers(self, request):
         """批量删除企业组织成员
 
         :param request: Request instance for DeleteOrganizationMembers.
         :type request: :class:`tencentcloud.organization.v20210331.models.DeleteOrganizationMembersRequest`
@@ -180,15 +180,15 @@
             model = models.DeleteOrganizationMembersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteOrganizationNodes(self, request):
         """批量删除企业组织节点
 
         :param request: Request instance for DeleteOrganizationNodes.
         :type request: :class:`tencentcloud.organization.v20210331.models.DeleteOrganizationNodesRequest`
@@ -203,15 +203,15 @@
             model = models.DeleteOrganizationNodesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOrganization(self, request):
         """获取企业组织信息
 
         :param request: Request instance for DescribeOrganization.
         :type request: :class:`tencentcloud.organization.v20210331.models.DescribeOrganizationRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeOrganizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOrganizationAuthNode(self, request):
         """获取已设置管理员的互信主体关系列表
 
         :param request: Request instance for DescribeOrganizationAuthNode.
         :type request: :class:`tencentcloud.organization.v20210331.models.DescribeOrganizationAuthNodeRequest`
@@ -249,15 +249,15 @@
             model = models.DescribeOrganizationAuthNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOrganizationFinancialByMember(self, request):
         """以成员维度获取组织财务信息
 
         :param request: Request instance for DescribeOrganizationFinancialByMember.
         :type request: :class:`tencentcloud.organization.v20210331.models.DescribeOrganizationFinancialByMemberRequest`
@@ -272,15 +272,15 @@
             model = models.DescribeOrganizationFinancialByMemberResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOrganizationFinancialByMonth(self, request):
         """以月维度获取组织财务信息趋势
 
         :param request: Request instance for DescribeOrganizationFinancialByMonth.
         :type request: :class:`tencentcloud.organization.v20210331.models.DescribeOrganizationFinancialByMonthRequest`
@@ -295,15 +295,15 @@
             model = models.DescribeOrganizationFinancialByMonthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOrganizationFinancialByProduct(self, request):
         """以产品维度获取组织财务信息
 
         :param request: Request instance for DescribeOrganizationFinancialByProduct.
         :type request: :class:`tencentcloud.organization.v20210331.models.DescribeOrganizationFinancialByProductRequest`
@@ -318,15 +318,15 @@
             model = models.DescribeOrganizationFinancialByProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOrganizationMemberAuthAccounts(self, request):
         """获取组织成员被绑定授权关系的子账号列表
 
         :param request: Request instance for DescribeOrganizationMemberAuthAccounts.
         :type request: :class:`tencentcloud.organization.v20210331.models.DescribeOrganizationMemberAuthAccountsRequest`
@@ -341,15 +341,15 @@
             model = models.DescribeOrganizationMemberAuthAccountsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOrganizationMemberAuthIdentities(self, request):
         """获取组织成员可被管理的身份列表
 
         :param request: Request instance for DescribeOrganizationMemberAuthIdentities.
         :type request: :class:`tencentcloud.organization.v20210331.models.DescribeOrganizationMemberAuthIdentitiesRequest`
@@ -364,15 +364,15 @@
             model = models.DescribeOrganizationMemberAuthIdentitiesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOrganizationMemberEmailBind(self, request):
         """查询成员邮箱绑定详细信息
 
         :param request: Request instance for DescribeOrganizationMemberEmailBind.
         :type request: :class:`tencentcloud.organization.v20210331.models.DescribeOrganizationMemberEmailBindRequest`
@@ -387,15 +387,15 @@
             model = models.DescribeOrganizationMemberEmailBindResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOrganizationMemberPolicies(self, request):
         """获取组织成员的授权策略列表
 
         :param request: Request instance for DescribeOrganizationMemberPolicies.
         :type request: :class:`tencentcloud.organization.v20210331.models.DescribeOrganizationMemberPoliciesRequest`
@@ -410,15 +410,15 @@
             model = models.DescribeOrganizationMemberPoliciesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOrganizationMembers(self, request):
         """获取企业组织成员列表
 
         :param request: Request instance for DescribeOrganizationMembers.
         :type request: :class:`tencentcloud.organization.v20210331.models.DescribeOrganizationMembersRequest`
@@ -433,15 +433,15 @@
             model = models.DescribeOrganizationMembersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOrganizationNodes(self, request):
         """获取组织节点列表
 
         :param request: Request instance for DescribeOrganizationNodes.
         :type request: :class:`tencentcloud.organization.v20210331.models.DescribeOrganizationNodesRequest`
@@ -456,15 +456,15 @@
             model = models.DescribeOrganizationNodesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListOrganizationIdentity(self, request):
         """获取组织成员访问身份列表
 
         :param request: Request instance for ListOrganizationIdentity.
         :type request: :class:`tencentcloud.organization.v20210331.models.ListOrganizationIdentityRequest`
@@ -479,15 +479,15 @@
             model = models.ListOrganizationIdentityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def MoveOrganizationNodeMembers(self, request):
         """移动成员到指定企业组织节点
 
         :param request: Request instance for MoveOrganizationNodeMembers.
         :type request: :class:`tencentcloud.organization.v20210331.models.MoveOrganizationNodeMembersRequest`
@@ -502,15 +502,15 @@
             model = models.MoveOrganizationNodeMembersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateOrganizationMember(self, request):
         """更新组织成员信息
 
         :param request: Request instance for UpdateOrganizationMember.
         :type request: :class:`tencentcloud.organization.v20210331.models.UpdateOrganizationMemberRequest`
@@ -525,15 +525,15 @@
             model = models.UpdateOrganizationMemberResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateOrganizationMemberEmailBind(self, request):
         """修改绑定成员邮箱
 
         :param request: Request instance for UpdateOrganizationMemberEmailBind.
         :type request: :class:`tencentcloud.organization.v20210331.models.UpdateOrganizationMemberEmailBindRequest`
@@ -548,15 +548,15 @@
             model = models.UpdateOrganizationMemberEmailBindResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateOrganizationNode(self, request):
         """更新企业组织节点
 
         :param request: Request instance for UpdateOrganizationNode.
         :type request: :class:`tencentcloud.organization.v20210331.models.UpdateOrganizationNodeRequest`
@@ -571,8 +571,8 @@
             model = models.UpdateOrganizationNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-organization-3.0.937/tencentcloud/organization/v20210331/errorcodes.py` & `tencentcloud-sdk-python-organization-3.0.938/tencentcloud/organization/v20210331/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.937/tencentcloud/organization/v20210331/models.py` & `tencentcloud-sdk-python-organization-3.0.938/tencentcloud/organization/v20210331/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-organization-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-organization
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Organization SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-organization-3.0.937/README.rst` & `tencentcloud-sdk-python-organization-3.0.938/README.rst`

 * *Files identical despite different names*

