# Comparing `tmp/tencentcloud-sdk-python-cme-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-cme-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cme-3.0.937.tar", last modified: Tue Jul 18 00:20:51 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cme-3.0.938.tar", last modified: Wed Jul 19 00:24:58 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cme-3.0.937.tar` & `tencentcloud-sdk-python-cme-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:51.000000 tencentcloud-sdk-python-cme-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:20:51.000000 tencentcloud-sdk-python-cme-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:51.000000 tencentcloud-sdk-python-cme-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:20:51.000000 tencentcloud-sdk-python-cme-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:51.000000 tencentcloud-sdk-python-cme-3.0.937/tencentcloud/cme/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:51.000000 tencentcloud-sdk-python-cme-3.0.937/tencentcloud/cme/v20191029/
--rw-r--r--   0 root         (0) root         (0)    55251 2023-07-18 00:20:51.000000 tencentcloud-sdk-python-cme-3.0.937/tencentcloud/cme/v20191029/cme_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:20:51.000000 tencentcloud-sdk-python-cme-3.0.937/tencentcloud/cme/v20191029/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8415 2023-07-18 00:20:51.000000 tencentcloud-sdk-python-cme-3.0.937/tencentcloud/cme/v20191029/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   444358 2023-07-18 00:20:51.000000 tencentcloud-sdk-python-cme-3.0.937/tencentcloud/cme/v20191029/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:20:51.000000 tencentcloud-sdk-python-cme-3.0.937/tencentcloud/cme/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:20:51.000000 tencentcloud-sdk-python-cme-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:51.000000 tencentcloud-sdk-python-cme-3.0.937/tencentcloud_sdk_python_cme.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:20:51.000000 tencentcloud-sdk-python-cme-3.0.937/tencentcloud_sdk_python_cme.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:20:51.000000 tencentcloud-sdk-python-cme-3.0.937/tencentcloud_sdk_python_cme.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:20:51.000000 tencentcloud-sdk-python-cme-3.0.937/tencentcloud_sdk_python_cme.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:20:51.000000 tencentcloud-sdk-python-cme-3.0.937/tencentcloud_sdk_python_cme.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:20:51.000000 tencentcloud-sdk-python-cme-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:20:51.000000 tencentcloud-sdk-python-cme-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:58.000000 tencentcloud-sdk-python-cme-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:24:57.000000 tencentcloud-sdk-python-cme-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:58.000000 tencentcloud-sdk-python-cme-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:24:57.000000 tencentcloud-sdk-python-cme-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:58.000000 tencentcloud-sdk-python-cme-3.0.938/tencentcloud/cme/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:58.000000 tencentcloud-sdk-python-cme-3.0.938/tencentcloud/cme/v20191029/
+-rw-r--r--   0 root         (0) root         (0)    55451 2023-07-19 00:24:57.000000 tencentcloud-sdk-python-cme-3.0.938/tencentcloud/cme/v20191029/cme_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:24:57.000000 tencentcloud-sdk-python-cme-3.0.938/tencentcloud/cme/v20191029/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8415 2023-07-19 00:24:57.000000 tencentcloud-sdk-python-cme-3.0.938/tencentcloud/cme/v20191029/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   444358 2023-07-19 00:24:57.000000 tencentcloud-sdk-python-cme-3.0.938/tencentcloud/cme/v20191029/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:24:57.000000 tencentcloud-sdk-python-cme-3.0.938/tencentcloud/cme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:24:58.000000 tencentcloud-sdk-python-cme-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:58.000000 tencentcloud-sdk-python-cme-3.0.938/tencentcloud_sdk_python_cme.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:24:58.000000 tencentcloud-sdk-python-cme-3.0.938/tencentcloud_sdk_python_cme.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:24:58.000000 tencentcloud-sdk-python-cme-3.0.938/tencentcloud_sdk_python_cme.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:24:58.000000 tencentcloud-sdk-python-cme-3.0.938/tencentcloud_sdk_python_cme.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:24:58.000000 tencentcloud-sdk-python-cme-3.0.938/tencentcloud_sdk_python_cme.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:24:58.000000 tencentcloud-sdk-python-cme-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:24:57.000000 tencentcloud-sdk-python-cme-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-cme-3.0.937/setup.py` & `tencentcloud-sdk-python-cme-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cme-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cme-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cme-3.0.937/tencentcloud/cme/v20191029/cme_client.py` & `tencentcloud-sdk-python-cme-3.0.938/tencentcloud/cme/v20191029/cme_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AddTeamMemberResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CopyProject(self, request):
         """复制一个项目，包括项目素材及轨道数据。目前仅普通剪辑及模板制作项目可复制，其它类型的项目不支持复制。
 
         :param request: Request instance for CopyProject.
         :type request: :class:`tencentcloud.cme.v20191029.models.CopyProjectRequest`
@@ -65,15 +65,15 @@
             model = models.CopyProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateClass(self, request):
         """新增分类，用于管理素材。分类层数不能超过20。
 
         :param request: Request instance for CreateClass.
         :type request: :class:`tencentcloud.cme.v20191029.models.CreateClassRequest`
@@ -88,15 +88,15 @@
             model = models.CreateClassResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLink(self, request):
         """创建媒体链接或分类路径链接，将资源信息链接到目标。
 
         :param request: Request instance for CreateLink.
         :type request: :class:`tencentcloud.cme.v20191029.models.CreateLinkRequest`
@@ -111,15 +111,15 @@
             model = models.CreateLinkResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateProject(self, request):
         """创建多媒体创作引擎项目，目前支持的项目类型有：
         <li>视频剪辑项目：用于普通视频剪辑；</li>
         <li>直播剪辑项目：用于直播流剪辑；</li>
         <li>导播台项目：用于云导播台；</li>
@@ -141,15 +141,15 @@
             model = models.CreateProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTeam(self, request):
         """创建一个团队。
 
         :param request: Request instance for CreateTeam.
         :type request: :class:`tencentcloud.cme.v20191029.models.CreateTeamRequest`
@@ -164,15 +164,15 @@
             model = models.CreateTeamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVideoEncodingPreset(self, request):
         """指定导出的参数，创建一个视频编码配置
 
         :param request: Request instance for CreateVideoEncodingPreset.
         :type request: :class:`tencentcloud.cme.v20191029.models.CreateVideoEncodingPresetRequest`
@@ -187,15 +187,15 @@
             model = models.CreateVideoEncodingPresetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteClass(self, request):
         """删除分类信息，删除时检验下述限制：
         <li>分类路径必须存在；</li>
         <li>分类下没有绑定素材。</li>
 
@@ -212,15 +212,15 @@
             model = models.DeleteClassResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLoginStatus(self, request):
         """删除用户登录态，使用户登出多媒体创作引擎平台。
 
         :param request: Request instance for DeleteLoginStatus.
         :type request: :class:`tencentcloud.cme.v20191029.models.DeleteLoginStatusRequest`
@@ -235,15 +235,15 @@
             model = models.DeleteLoginStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteMaterial(self, request):
         """根据媒体 Id 删除媒体。
 
         :param request: Request instance for DeleteMaterial.
         :type request: :class:`tencentcloud.cme.v20191029.models.DeleteMaterialRequest`
@@ -258,15 +258,15 @@
             model = models.DeleteMaterialResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteProject(self, request):
         """删除项目。处于推流状态的云转推和点播转直播项目不允许删除，若强行调用删除项目接口会返回失败。
 
         :param request: Request instance for DeleteProject.
         :type request: :class:`tencentcloud.cme.v20191029.models.DeleteProjectRequest`
@@ -281,15 +281,15 @@
             model = models.DeleteProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTeam(self, request):
         """删除一个团队。要删除团队，必须满足以下条件：
         <li>要删除的团队必须没有归属的素材；</li>
         <li>要删除的团队必须没有归属的分类。</li>
 
@@ -306,15 +306,15 @@
             model = models.DeleteTeamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTeamMembers(self, request):
         """将团队成员从团队中删除。
 
         :param request: Request instance for DeleteTeamMembers.
         :type request: :class:`tencentcloud.cme.v20191029.models.DeleteTeamMembersRequest`
@@ -329,15 +329,15 @@
             model = models.DeleteTeamMembersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteVideoEncodingPreset(self, request):
         """删除指定 ID 的视频编码配置
 
         :param request: Request instance for DeleteVideoEncodingPreset.
         :type request: :class:`tencentcloud.cme.v20191029.models.DeleteVideoEncodingPresetRequest`
@@ -352,15 +352,15 @@
             model = models.DeleteVideoEncodingPresetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccounts(self, request):
         """获取平台中所有的已注册账号。
 
         :param request: Request instance for DescribeAccounts.
         :type request: :class:`tencentcloud.cme.v20191029.models.DescribeAccountsRequest`
@@ -375,15 +375,15 @@
             model = models.DescribeAccountsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClass(self, request):
         """获取指定归属者下所有的分类信息。
 
         :param request: Request instance for DescribeClass.
         :type request: :class:`tencentcloud.cme.v20191029.models.DescribeClassRequest`
@@ -398,15 +398,15 @@
             model = models.DescribeClassResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeJoinTeams(self, request):
         """获取用户所加入的团队列表
 
         :param request: Request instance for DescribeJoinTeams.
         :type request: :class:`tencentcloud.cme.v20191029.models.DescribeJoinTeamsRequest`
@@ -421,15 +421,15 @@
             model = models.DescribeJoinTeamsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLoginStatus(self, request):
         """查询指定用户的登录态。
 
         :param request: Request instance for DescribeLoginStatus.
         :type request: :class:`tencentcloud.cme.v20191029.models.DescribeLoginStatusRequest`
@@ -444,15 +444,15 @@
             model = models.DescribeLoginStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMaterials(self, request):
         """根据媒体 Id 批量获取媒体详情。
 
         :param request: Request instance for DescribeMaterials.
         :type request: :class:`tencentcloud.cme.v20191029.models.DescribeMaterialsRequest`
@@ -467,15 +467,15 @@
             model = models.DescribeMaterialsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePlatforms(self, request):
         """<li>支持获取所创建的所有平台列表信息；</li>
         <li>支持获取指定的平台列表信息。</li>
 
         关于平台概念，请参见文档 [平台](https://cloud.tencent.com/document/product/1156/43767)。
@@ -494,15 +494,15 @@
             model = models.DescribePlatformsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProjects(self, request):
         """支持根据多种条件过滤出项目列表。
 
         :param request: Request instance for DescribeProjects.
         :type request: :class:`tencentcloud.cme.v20191029.models.DescribeProjectsRequest`
@@ -517,15 +517,15 @@
             model = models.DescribeProjectsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourceAuthorization(self, request):
         """查询资源被授权的情况。
 
         :param request: Request instance for DescribeResourceAuthorization.
         :type request: :class:`tencentcloud.cme.v20191029.models.DescribeResourceAuthorizationRequest`
@@ -540,15 +540,15 @@
             model = models.DescribeResourceAuthorizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSharedSpace(self, request):
         """获取共享空间。当个人或团队A对个人或团队B授权某资源以后，个人或团队B的共享空间就会增加个人或团队A。
 
         :param request: Request instance for DescribeSharedSpace.
         :type request: :class:`tencentcloud.cme.v20191029.models.DescribeSharedSpaceRequest`
@@ -563,15 +563,15 @@
             model = models.DescribeSharedSpaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskDetail(self, request):
         """获取任务详情信息，包含下面几个部分：
         <li>任务基础信息：包括任务状态、错误信息、创建时间等；</li>
         <li>导出项目输出信息：包括输出的素材 Id 等。</li>
 
@@ -588,15 +588,15 @@
             model = models.DescribeTaskDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTasks(self, request):
         """获取任务列表，支持条件筛选，返回对应的任务基础信息列表。
 
         :param request: Request instance for DescribeTasks.
         :type request: :class:`tencentcloud.cme.v20191029.models.DescribeTasksRequest`
@@ -611,15 +611,15 @@
             model = models.DescribeTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTeamMembers(self, request):
         """获取指定团队的成员信息。支持获取指定成员的信息，同时也支持分页拉取指定团队的所有成员信息。
 
         :param request: Request instance for DescribeTeamMembers.
         :type request: :class:`tencentcloud.cme.v20191029.models.DescribeTeamMembersRequest`
@@ -634,15 +634,15 @@
             model = models.DescribeTeamMembersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTeams(self, request):
         """获取指定团队的信息，拉取团队信息列表。
 
         :param request: Request instance for DescribeTeams.
         :type request: :class:`tencentcloud.cme.v20191029.models.DescribeTeamsRequest`
@@ -657,15 +657,15 @@
             model = models.DescribeTeamsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVideoEncodingPresets(self, request):
         """查询视频编码配置信息。
 
         :param request: Request instance for DescribeVideoEncodingPresets.
         :type request: :class:`tencentcloud.cme.v20191029.models.DescribeVideoEncodingPresetsRequest`
@@ -680,15 +680,15 @@
             model = models.DescribeVideoEncodingPresetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExportVideoByEditorTrackData(self, request):
         """使用 [视频合成协议](https://cloud.tencent.com/document/product/1156/51225) 合成视频，支持导出视频到 CME 云媒资或者云点播媒资。
 
         :param request: Request instance for ExportVideoByEditorTrackData.
         :type request: :class:`tencentcloud.cme.v20191029.models.ExportVideoByEditorTrackDataRequest`
@@ -703,15 +703,15 @@
             model = models.ExportVideoByEditorTrackDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExportVideoByTemplate(self, request):
         """使用视频剪辑模板直接导出视频。
 
         :param request: Request instance for ExportVideoByTemplate.
         :type request: :class:`tencentcloud.cme.v20191029.models.ExportVideoByTemplateRequest`
@@ -726,15 +726,15 @@
             model = models.ExportVideoByTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExportVideoByVideoSegmentationData(self, request):
         """使用视频智能拆条数据导出视频，将指定的视频拆条片段导出为一个视频(内测中，请勿使用)。
 
         :param request: Request instance for ExportVideoByVideoSegmentationData.
         :type request: :class:`tencentcloud.cme.v20191029.models.ExportVideoByVideoSegmentationDataRequest`
@@ -749,15 +749,15 @@
             model = models.ExportVideoByVideoSegmentationDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExportVideoEditProject(self, request):
         """导出视频编辑项目，支持指定输出的模板。
 
         :param request: Request instance for ExportVideoEditProject.
         :type request: :class:`tencentcloud.cme.v20191029.models.ExportVideoEditProjectRequest`
@@ -772,15 +772,15 @@
             model = models.ExportVideoEditProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def FlattenListMedia(self, request):
         """平铺分类路径下及其子分类下的所有媒体基础信息，返回当前分类及子分类中的所有媒体的基础信息。
 
         :param request: Request instance for FlattenListMedia.
         :type request: :class:`tencentcloud.cme.v20191029.models.FlattenListMediaRequest`
@@ -795,15 +795,15 @@
             model = models.FlattenListMediaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GenerateVideoSegmentationSchemeByAi(self, request):
         """<li>发起视频智能拆条任务，支持智能生成和平精英集锦、王者荣耀集锦、足球集锦、篮球集锦 、人物集锦、新闻拆条等任务。</li>
         <li>和平精英集锦和王者荣耀集锦根据击杀场景进行拆条，足球集锦和篮球集锦根据进球场景进行拆条，人物集锦根据人物人脸特征进行拆条，新闻拆条根据导播进行拆条。</li>
         <li>【本接口内测中，暂不建议使用】</li>
 
@@ -820,15 +820,15 @@
             model = models.GenerateVideoSegmentationSchemeByAiResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GrantResourceAuthorization(self, request):
         """资源归属者对个人或团队授予目标资源的相应权限。
 
         :param request: Request instance for GrantResourceAuthorization.
         :type request: :class:`tencentcloud.cme.v20191029.models.GrantResourceAuthorizationRequest`
@@ -843,15 +843,15 @@
             model = models.GrantResourceAuthorizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def HandleMediaCastProject(self, request):
         """对媒体转推项目进行操作。
         ### 操作类型<a id="Operation"></a>
         - `AddSource`（添加输入源），项目状态为 Idle、Working 时均可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B9-.E6.B7.BB.E5.8A.A0.E8.BE.93.E5.85.A5.E6.BA.90)；
         - `DeleteSource`（删除输入源），项目状态为 Idle、Working 时均可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B6-.E5.88.A0.E9.99.A4.E8.BE.93.E5.85.A5.E6.BA.90)；
@@ -881,15 +881,15 @@
             model = models.HandleMediaCastProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def HandleStreamConnectProject(self, request):
         """<font color=red>本接口废弃，可创建媒体转推项目替代，操作媒体转推项目可使用 <b>[HandleMediaCastProject 接口](/document/product/1156/87841) </b>实现。</font>
 
         ### 操作类型<a id="Operation"></a>
         - `AddInput`（添加输入源），包括：
@@ -920,15 +920,15 @@
             model = models.HandleStreamConnectProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ImportMaterial(self, request):
         """将云点播媒资文件导入到多媒体创作引擎媒体资源库。支持导入媒体归属团队或者个人。
 
         :param request: Request instance for ImportMaterial.
         :type request: :class:`tencentcloud.cme.v20191029.models.ImportMaterialRequest`
@@ -943,15 +943,15 @@
             model = models.ImportMaterialResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ImportMediaToProject(self, request):
         """将云点播中的媒资或者用户自有媒资文件添加到项目中与项目关联，供后续视频编辑使用。目前仅视频编辑项目和智能视频拆条项目有效。
 
         :param request: Request instance for ImportMediaToProject.
         :type request: :class:`tencentcloud.cme.v20191029.models.ImportMediaToProjectRequest`
@@ -966,15 +966,15 @@
             model = models.ImportMediaToProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListMedia(self, request):
         """浏览当前分类路径下的资源，包括媒体文件和子分类，返回媒资基础信息和分类信息。
 
         :param request: Request instance for ListMedia.
         :type request: :class:`tencentcloud.cme.v20191029.models.ListMediaRequest`
@@ -989,15 +989,15 @@
             model = models.ListMediaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyMaterial(self, request):
         """修改媒体信息，支持修改媒体名称、分类路径、标签等信息。
 
         :param request: Request instance for ModifyMaterial.
         :type request: :class:`tencentcloud.cme.v20191029.models.ModifyMaterialRequest`
@@ -1012,15 +1012,15 @@
             model = models.ModifyMaterialResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyProject(self, request):
         """修改项目信息。
 
         :param request: Request instance for ModifyProject.
         :type request: :class:`tencentcloud.cme.v20191029.models.ModifyProjectRequest`
@@ -1035,15 +1035,15 @@
             model = models.ModifyProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTeam(self, request):
         """修改团队信息，目前支持修改的操作有：
         <li>修改团队名称。</li>
 
         :param request: Request instance for ModifyTeam.
@@ -1059,15 +1059,15 @@
             model = models.ModifyTeamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTeamMember(self, request):
         """修改团队成员信息，包括成员备注、角色等。
 
         :param request: Request instance for ModifyTeamMember.
         :type request: :class:`tencentcloud.cme.v20191029.models.ModifyTeamMemberRequest`
@@ -1082,15 +1082,15 @@
             model = models.ModifyTeamMemberResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyVideoEncodingPreset(self, request):
         """修改视频编码配置信息。
 
         :param request: Request instance for ModifyVideoEncodingPreset.
         :type request: :class:`tencentcloud.cme.v20191029.models.ModifyVideoEncodingPresetRequest`
@@ -1105,15 +1105,15 @@
             model = models.ModifyVideoEncodingPresetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def MoveClass(self, request):
         """移动某一个分类到另外一个分类下，也可用于分类重命名。
         如果 SourceClassPath = /素材/视频/NBA，DestinationClassPath = /素材/视频/篮球
         <li>当 DestinationClassPath 不存在时候，操作结果为重命名 ClassPath；</li>
         <li>当 DestinationClassPath 存在时候，操作结果为产生新目录 /素材/视频/篮球/NBA</li>
@@ -1131,15 +1131,15 @@
             model = models.MoveClassResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def MoveResource(self, request):
         """移动资源，支持跨个人或团队移动媒体以及分类。如果填写了Operator，则需要校验用户对媒体和分类资源的访问以及写权限。
         <li>当原始资源为媒体时，该接口效果为将该媒体移动到目标分类下面；</li>
         <li>当原始资源为分类时，该接口效果为将原始分类移动到目标分类或者是重命名。</li>
          如果 SourceResource.Resource.Id = /素材/视频/NBA，DestinationResource.Resource.Id= /素材/视频/篮球
@@ -1159,15 +1159,15 @@
             model = models.MoveResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ParseEvent(self, request):
         """该接口接受多媒体创作引擎回调给业务的事件内容，将其转化为对应的 EventContent 结构。请不要实际调用该接口，只需要将接收到的事件内容直接使用 JSON 解析到 EventContent  结构即可使用。
 
         :param request: Request instance for ParseEvent.
         :type request: :class:`tencentcloud.cme.v20191029.models.ParseEventRequest`
@@ -1182,15 +1182,15 @@
             model = models.ParseEventResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RevokeResourceAuthorization(self, request):
         """资源所属实体对目标实体撤销目标资源的相应权限，若原本没有相应权限则不产生变更。
 
         :param request: Request instance for RevokeResourceAuthorization.
         :type request: :class:`tencentcloud.cme.v20191029.models.RevokeResourceAuthorizationRequest`
@@ -1205,15 +1205,15 @@
             model = models.RevokeResourceAuthorizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchMaterial(self, request):
         """根据检索条件搜索媒体，返回媒体的基本信息。
 
         :param request: Request instance for SearchMaterial.
         :type request: :class:`tencentcloud.cme.v20191029.models.SearchMaterialRequest`
@@ -1228,8 +1228,8 @@
             model = models.SearchMaterialResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-cme-3.0.937/tencentcloud/cme/v20191029/errorcodes.py` & `tencentcloud-sdk-python-cme-3.0.938/tencentcloud/cme/v20191029/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cme-3.0.937/tencentcloud/cme/v20191029/models.py` & `tencentcloud-sdk-python-cme-3.0.938/tencentcloud/cme/v20191029/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cme-3.0.937/tencentcloud_sdk_python_cme.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cme-3.0.938/tencentcloud_sdk_python_cme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cme
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cme SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cme-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-cme-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cme
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cme SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cme-3.0.937/README.rst` & `tencentcloud-sdk-python-cme-3.0.938/README.rst`

 * *Files identical despite different names*

