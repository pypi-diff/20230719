# Comparing `tmp/tencentcloud-sdk-python-lcic-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-lcic-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.937.tar", last modified: Tue Jul 18 00:26:30 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.938.tar", last modified: Wed Jul 19 00:41:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lcic-3.0.937.tar` & `tencentcloud-sdk-python-lcic-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:30.000000 tencentcloud-sdk-python-lcic-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:26:30.000000 tencentcloud-sdk-python-lcic-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:30.000000 tencentcloud-sdk-python-lcic-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:26:30.000000 tencentcloud-sdk-python-lcic-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:30.000000 tencentcloud-sdk-python-lcic-3.0.937/tencentcloud/lcic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:30.000000 tencentcloud-sdk-python-lcic-3.0.937/tencentcloud/lcic/v20220817/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:26:30.000000 tencentcloud-sdk-python-lcic-3.0.937/tencentcloud/lcic/v20220817/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48649 2023-07-18 00:26:30.000000 tencentcloud-sdk-python-lcic-3.0.937/tencentcloud/lcic/v20220817/lcic_client.py
--rw-r--r--   0 root         (0) root         (0)     4414 2023-07-18 00:26:30.000000 tencentcloud-sdk-python-lcic-3.0.937/tencentcloud/lcic/v20220817/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   229644 2023-07-18 00:26:30.000000 tencentcloud-sdk-python-lcic-3.0.937/tencentcloud/lcic/v20220817/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:26:30.000000 tencentcloud-sdk-python-lcic-3.0.937/tencentcloud/lcic/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:26:30.000000 tencentcloud-sdk-python-lcic-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:30.000000 tencentcloud-sdk-python-lcic-3.0.937/tencentcloud_sdk_python_lcic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:26:30.000000 tencentcloud-sdk-python-lcic-3.0.937/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:26:30.000000 tencentcloud-sdk-python-lcic-3.0.937/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:26:30.000000 tencentcloud-sdk-python-lcic-3.0.937/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:26:30.000000 tencentcloud-sdk-python-lcic-3.0.937/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:26:30.000000 tencentcloud-sdk-python-lcic-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:26:30.000000 tencentcloud-sdk-python-lcic-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:55.000000 tencentcloud-sdk-python-lcic-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:41:55.000000 tencentcloud-sdk-python-lcic-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:55.000000 tencentcloud-sdk-python-lcic-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:41:55.000000 tencentcloud-sdk-python-lcic-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:55.000000 tencentcloud-sdk-python-lcic-3.0.938/tencentcloud/lcic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:55.000000 tencentcloud-sdk-python-lcic-3.0.938/tencentcloud/lcic/v20220817/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:41:55.000000 tencentcloud-sdk-python-lcic-3.0.938/tencentcloud/lcic/v20220817/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48865 2023-07-19 00:41:55.000000 tencentcloud-sdk-python-lcic-3.0.938/tencentcloud/lcic/v20220817/lcic_client.py
+-rw-r--r--   0 root         (0) root         (0)     4414 2023-07-19 00:41:55.000000 tencentcloud-sdk-python-lcic-3.0.938/tencentcloud/lcic/v20220817/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   229644 2023-07-19 00:41:55.000000 tencentcloud-sdk-python-lcic-3.0.938/tencentcloud/lcic/v20220817/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:41:55.000000 tencentcloud-sdk-python-lcic-3.0.938/tencentcloud/lcic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:41:55.000000 tencentcloud-sdk-python-lcic-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:55.000000 tencentcloud-sdk-python-lcic-3.0.938/tencentcloud_sdk_python_lcic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:41:55.000000 tencentcloud-sdk-python-lcic-3.0.938/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:41:55.000000 tencentcloud-sdk-python-lcic-3.0.938/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:41:55.000000 tencentcloud-sdk-python-lcic-3.0.938/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:41:55.000000 tencentcloud-sdk-python-lcic-3.0.938/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:41:55.000000 tencentcloud-sdk-python-lcic-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:41:55.000000 tencentcloud-sdk-python-lcic-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.937/setup.py` & `tencentcloud-sdk-python-lcic-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lcic-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lcic-3.0.937/tencentcloud/lcic/v20220817/lcic_client.py` & `tencentcloud-sdk-python-lcic-3.0.938/tencentcloud/lcic/v20220817/lcic_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AddGroupMemberResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchAddGroupMember(self, request):
         """此接口用于批量添加成员列表到指定群组
 
         :param request: Request instance for BatchAddGroupMember.
         :type request: :class:`tencentcloud.lcic.v20220817.models.BatchAddGroupMemberRequest`
@@ -65,15 +65,15 @@
             model = models.BatchAddGroupMemberResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchCreateGroupWithMembers(self, request):
         """此接口用于批量创建群组
 
         :param request: Request instance for BatchCreateGroupWithMembers.
         :type request: :class:`tencentcloud.lcic.v20220817.models.BatchCreateGroupWithMembersRequest`
@@ -88,15 +88,15 @@
             model = models.BatchCreateGroupWithMembersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchCreateRoom(self, request):
         """批量创建房间接口
 
         :param request: Request instance for BatchCreateRoom.
         :type request: :class:`tencentcloud.lcic.v20220817.models.BatchCreateRoomRequest`
@@ -111,15 +111,15 @@
             model = models.BatchCreateRoomResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchDeleteGroupMember(self, request):
         """此接口用于批量删除成员列表到指定群组列表
 
         :param request: Request instance for BatchDeleteGroupMember.
         :type request: :class:`tencentcloud.lcic.v20220817.models.BatchDeleteGroupMemberRequest`
@@ -134,15 +134,15 @@
             model = models.BatchDeleteGroupMemberResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchDeleteRecord(self, request):
         """批量删除多个房间的录制文件
 
         :param request: Request instance for BatchDeleteRecord.
         :type request: :class:`tencentcloud.lcic.v20220817.models.BatchDeleteRecordRequest`
@@ -157,15 +157,15 @@
             model = models.BatchDeleteRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchDescribeDocument(self, request):
         """批量获取文档详情
 
         :param request: Request instance for BatchDescribeDocument.
         :type request: :class:`tencentcloud.lcic.v20220817.models.BatchDescribeDocumentRequest`
@@ -180,15 +180,15 @@
             model = models.BatchDescribeDocumentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchRegister(self, request):
         """如果批量注册的用户已存在，则会被覆盖。一次最多注册1000个用户。默认请求频率限制：10次/秒
 
         :param request: Request instance for BatchRegister.
         :type request: :class:`tencentcloud.lcic.v20220817.models.BatchRegisterRequest`
@@ -203,15 +203,15 @@
             model = models.BatchRegisterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindDocumentToRoom(self, request):
         """绑定文档到房间
 
         :param request: Request instance for BindDocumentToRoom.
         :type request: :class:`tencentcloud.lcic.v20220817.models.BindDocumentToRoomRequest`
@@ -226,15 +226,15 @@
             model = models.BindDocumentToRoomResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDocument(self, request):
         """创建房间内可以使用的文档。
 
         :param request: Request instance for CreateDocument.
         :type request: :class:`tencentcloud.lcic.v20220817.models.CreateDocumentRequest`
@@ -249,15 +249,15 @@
             model = models.CreateDocumentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateGroupWithMembers(self, request):
         """此接口根据成员列表创建群组
 
         :param request: Request instance for CreateGroupWithMembers.
         :type request: :class:`tencentcloud.lcic.v20220817.models.CreateGroupWithMembersRequest`
@@ -272,15 +272,15 @@
             model = models.CreateGroupWithMembersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateGroupWithSubGroup(self, request):
         """此接口会聚合子群组创建联合群组
 
         :param request: Request instance for CreateGroupWithSubGroup.
         :type request: :class:`tencentcloud.lcic.v20220817.models.CreateGroupWithSubGroupRequest`
@@ -295,15 +295,15 @@
             model = models.CreateGroupWithSubGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRoom(self, request):
         """创建房间
 
         :param request: Request instance for CreateRoom.
         :type request: :class:`tencentcloud.lcic.v20220817.models.CreateRoomRequest`
@@ -318,15 +318,15 @@
             model = models.CreateRoomResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSupervisor(self, request):
         """创建巡课
 
         :param request: Request instance for CreateSupervisor.
         :type request: :class:`tencentcloud.lcic.v20220817.models.CreateSupervisorRequest`
@@ -341,15 +341,15 @@
             model = models.CreateSupervisorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAppCustomContent(self, request):
         """删除设置自定义元素。如果参数scenes为空则删除所有自定义元素，否则删除指定的scene自定义元素。
 
         :param request: Request instance for DeleteAppCustomContent.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DeleteAppCustomContentRequest`
@@ -364,15 +364,15 @@
             model = models.DeleteAppCustomContentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDocument(self, request):
         """删除文档
 
         :param request: Request instance for DeleteDocument.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DeleteDocumentRequest`
@@ -387,15 +387,15 @@
             model = models.DeleteDocumentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteGroup(self, request):
         """此接口用于删除指定群组，支持批量操作。
 
         :param request: Request instance for DeleteGroup.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DeleteGroupRequest`
@@ -410,15 +410,15 @@
             model = models.DeleteGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteGroupMember(self, request):
         """此接口用于删除群组中指定成员
 
         :param request: Request instance for DeleteGroupMember.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DeleteGroupMemberRequest`
@@ -433,15 +433,15 @@
             model = models.DeleteGroupMemberResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRecord(self, request):
         """删除指定房间的录制文件
 
         :param request: Request instance for DeleteRecord.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DeleteRecordRequest`
@@ -456,15 +456,15 @@
             model = models.DeleteRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRoom(self, request):
         """删除房间
 
         :param request: Request instance for DeleteRoom.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DeleteRoomRequest`
@@ -479,15 +479,15 @@
             model = models.DeleteRoomResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSupervisor(self, request):
         """删除巡课
 
         :param request: Request instance for DeleteSupervisor.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DeleteSupervisorRequest`
@@ -502,15 +502,15 @@
             model = models.DeleteSupervisorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAnswerList(self, request):
         """获取房间答题详情
 
         :param request: Request instance for DescribeAnswerList.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DescribeAnswerListRequest`
@@ -525,15 +525,15 @@
             model = models.DescribeAnswerListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAppDetail(self, request):
         """获取应用详情
 
         :param request: Request instance for DescribeAppDetail.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DescribeAppDetailRequest`
@@ -548,15 +548,15 @@
             model = models.DescribeAppDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCurrentMemberList(self, request):
         """获取当前房间的成员列表，房间结束或过期后无法使用。
 
         :param request: Request instance for DescribeCurrentMemberList.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DescribeCurrentMemberListRequest`
@@ -571,15 +571,15 @@
             model = models.DescribeCurrentMemberListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeveloper(self, request):
         """开发商信息获取
 
         :param request: Request instance for DescribeDeveloper.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DescribeDeveloperRequest`
@@ -594,15 +594,15 @@
             model = models.DescribeDeveloperResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDocument(self, request):
         """获取文档信息
 
         :param request: Request instance for DescribeDocument.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DescribeDocumentRequest`
@@ -617,15 +617,15 @@
             model = models.DescribeDocumentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDocuments(self, request):
         """有新接口替换
 
         批量获取文档信息（已废弃，替代接口BatchDescribeDocument）
 
@@ -642,15 +642,15 @@
             model = models.DescribeDocumentsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDocumentsByRoom(self, request):
         """此接口获取指定房间下课件列表
 
         :param request: Request instance for DescribeDocumentsByRoom.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DescribeDocumentsByRoomRequest`
@@ -665,15 +665,15 @@
             model = models.DescribeDocumentsByRoomResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGroup(self, request):
         """此接口用于获取群组详情
 
         :param request: Request instance for DescribeGroup.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DescribeGroupRequest`
@@ -688,15 +688,15 @@
             model = models.DescribeGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGroupList(self, request):
         """获取群组列表
 
         :param request: Request instance for DescribeGroupList.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DescribeGroupListRequest`
@@ -711,15 +711,15 @@
             model = models.DescribeGroupListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGroupMemberList(self, request):
         """此接口用于获取群组成员列表
 
         :param request: Request instance for DescribeGroupMemberList.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DescribeGroupMemberListRequest`
@@ -734,15 +734,15 @@
             model = models.DescribeGroupMemberListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeQuestionList(self, request):
         """获取房间提问列表
 
         :param request: Request instance for DescribeQuestionList.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DescribeQuestionListRequest`
@@ -757,15 +757,15 @@
             model = models.DescribeQuestionListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRoom(self, request):
         """获取房间信息
 
         :param request: Request instance for DescribeRoom.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DescribeRoomRequest`
@@ -780,15 +780,15 @@
             model = models.DescribeRoomResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRoomStatistics(self, request):
         """获取房间统计信息，仅可在房间结束后调用。
 
         :param request: Request instance for DescribeRoomStatistics.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DescribeRoomStatisticsRequest`
@@ -803,15 +803,15 @@
             model = models.DescribeRoomStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSdkAppIdUsers(self, request):
         """此接口用于获取指定应用ID下用户列表
 
         :param request: Request instance for DescribeSdkAppIdUsers.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DescribeSdkAppIdUsersRequest`
@@ -826,15 +826,15 @@
             model = models.DescribeSdkAppIdUsersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSupervisors(self, request):
         """获取巡课列表
 
         :param request: Request instance for DescribeSupervisors.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DescribeSupervisorsRequest`
@@ -849,15 +849,15 @@
             model = models.DescribeSupervisorsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUser(self, request):
         """获取用户信息
 
         :param request: Request instance for DescribeUser.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DescribeUserRequest`
@@ -872,15 +872,15 @@
             model = models.DescribeUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EndRoom(self, request):
         """结束房间的直播
 
         :param request: Request instance for EndRoom.
         :type request: :class:`tencentcloud.lcic.v20220817.models.EndRoomRequest`
@@ -895,15 +895,15 @@
             model = models.EndRoomResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetRoomEvent(self, request):
         """获取房间事件,仅在课堂结束1小时内有效。
 
         :param request: Request instance for GetRoomEvent.
         :type request: :class:`tencentcloud.lcic.v20220817.models.GetRoomEventRequest`
@@ -918,15 +918,15 @@
             model = models.GetRoomEventResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetRoomMessage(self, request):
         """获取房间历史消息(房间历史消息保存7天)
 
         :param request: Request instance for GetRoomMessage.
         :type request: :class:`tencentcloud.lcic.v20220817.models.GetRoomMessageRequest`
@@ -941,15 +941,15 @@
             model = models.GetRoomMessageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetRooms(self, request):
         """获取房间列表
 
         :param request: Request instance for GetRooms.
         :type request: :class:`tencentcloud.lcic.v20220817.models.GetRoomsRequest`
@@ -964,15 +964,15 @@
             model = models.GetRoomsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetWatermark(self, request):
         """获取水印设置
 
         :param request: Request instance for GetWatermark.
         :type request: :class:`tencentcloud.lcic.v20220817.models.GetWatermarkRequest`
@@ -987,15 +987,15 @@
             model = models.GetWatermarkResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def KickUserFromRoom(self, request):
         """从房间里面踢出用户
 
         :param request: Request instance for KickUserFromRoom.
         :type request: :class:`tencentcloud.lcic.v20220817.models.KickUserFromRoomRequest`
@@ -1010,15 +1010,15 @@
             model = models.KickUserFromRoomResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def LoginOriginId(self, request):
         """使用源账号登录，源账号为注册时填入的originId
 
         :param request: Request instance for LoginOriginId.
         :type request: :class:`tencentcloud.lcic.v20220817.models.LoginOriginIdRequest`
@@ -1033,15 +1033,15 @@
             model = models.LoginOriginIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def LoginUser(self, request):
         """登录
 
         :param request: Request instance for LoginUser.
         :type request: :class:`tencentcloud.lcic.v20220817.models.LoginUserRequest`
@@ -1056,15 +1056,15 @@
             model = models.LoginUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyApp(self, request):
         """修改应用
 
         :param request: Request instance for ModifyApp.
         :type request: :class:`tencentcloud.lcic.v20220817.models.ModifyAppRequest`
@@ -1079,15 +1079,15 @@
             model = models.ModifyAppResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyGroup(self, request):
         """此接口修改群组信息
 
         :param request: Request instance for ModifyGroup.
         :type request: :class:`tencentcloud.lcic.v20220817.models.ModifyGroupRequest`
@@ -1102,15 +1102,15 @@
             model = models.ModifyGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRoom(self, request):
         """修改房间
 
         :param request: Request instance for ModifyRoom.
         :type request: :class:`tencentcloud.lcic.v20220817.models.ModifyRoomRequest`
@@ -1125,15 +1125,15 @@
             model = models.ModifyRoomResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyUserProfile(self, request):
         """此接口用于修改用户配置，如头像，昵称/用户名等。
 
         :param request: Request instance for ModifyUserProfile.
         :type request: :class:`tencentcloud.lcic.v20220817.models.ModifyUserProfileRequest`
@@ -1148,15 +1148,15 @@
             model = models.ModifyUserProfileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RegisterUser(self, request):
         """注册用户
 
         :param request: Request instance for RegisterUser.
         :type request: :class:`tencentcloud.lcic.v20220817.models.RegisterUserRequest`
@@ -1171,15 +1171,15 @@
             model = models.RegisterUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetAppCustomContent(self, request):
         """设置应用的自定义内容，包括应用图标，自定义的代码等。如果已存在，则为更新。更新js、css内容后，要生效也需要调用该接口
 
         :param request: Request instance for SetAppCustomContent.
         :type request: :class:`tencentcloud.lcic.v20220817.models.SetAppCustomContentRequest`
@@ -1194,15 +1194,15 @@
             model = models.SetAppCustomContentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetWatermark(self, request):
         """设置水印
 
         :param request: Request instance for SetWatermark.
         :type request: :class:`tencentcloud.lcic.v20220817.models.SetWatermarkRequest`
@@ -1217,15 +1217,15 @@
             model = models.SetWatermarkResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartRoom(self, request):
         """开始房间的直播。 说明：开始房间接口调用之前需要有用户进入课堂初始化课堂信息。
 
         :param request: Request instance for StartRoom.
         :type request: :class:`tencentcloud.lcic.v20220817.models.StartRoomRequest`
@@ -1240,15 +1240,15 @@
             model = models.StartRoomResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnbindDocumentFromRoom(self, request):
         """文档从房间解绑
 
         :param request: Request instance for UnbindDocumentFromRoom.
         :type request: :class:`tencentcloud.lcic.v20220817.models.UnbindDocumentFromRoomRequest`
@@ -1263,8 +1263,8 @@
             model = models.UnbindDocumentFromRoomResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.937/tencentcloud/lcic/v20220817/errorcodes.py` & `tencentcloud-sdk-python-lcic-3.0.938/tencentcloud/lcic/v20220817/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.937/tencentcloud/lcic/v20220817/models.py` & `tencentcloud-sdk-python-lcic-3.0.938/tencentcloud/lcic/v20220817/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.937/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.938/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.938/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.937/README.rst` & `tencentcloud-sdk-python-lcic-3.0.938/README.rst`

 * *Files identical despite different names*

