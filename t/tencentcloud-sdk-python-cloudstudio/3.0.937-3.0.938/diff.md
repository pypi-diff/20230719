# Comparing `tmp/tencentcloud-sdk-python-cloudstudio-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-cloudstudio-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cloudstudio-3.0.937.tar", last modified: Tue Jul 18 00:20:42 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cloudstudio-3.0.938.tar", last modified: Wed Jul 19 00:24:48 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cloudstudio-3.0.937.tar` & `tencentcloud-sdk-python-cloudstudio-3.0.938.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:42.000000 tencentcloud-sdk-python-cloudstudio-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1022 2023-07-18 00:20:42.000000 tencentcloud-sdk-python-cloudstudio-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:42.000000 tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:42.000000 tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud/cloudstudio/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:20:42.000000 tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud/cloudstudio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:42.000000 tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud/cloudstudio/v20210524/
--rw-r--r--   0 root         (0) root         (0)    21809 2023-07-18 00:20:42.000000 tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud/cloudstudio/v20210524/cloudstudio_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:20:42.000000 tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud/cloudstudio/v20210524/__init__.py
--rw-r--r--   0 root         (0) root         (0)      828 2023-07-18 00:20:42.000000 tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud/cloudstudio/v20210524/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   112109 2023-07-18 00:20:42.000000 tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud/cloudstudio/v20210524/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:42.000000 tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud/cloudstudio/v20230508/
--rw-r--r--   0 root         (0) root         (0)     8959 2023-07-18 00:20:42.000000 tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud/cloudstudio/v20230508/cloudstudio_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:20:42.000000 tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud/cloudstudio/v20230508/__init__.py
--rw-r--r--   0 root         (0) root         (0)      979 2023-07-18 00:20:42.000000 tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud/cloudstudio/v20230508/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    33456 2023-07-18 00:20:42.000000 tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud/cloudstudio/v20230508/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:20:42.000000 tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:20:42.000000 tencentcloud-sdk-python-cloudstudio-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1699 2023-07-18 00:20:42.000000 tencentcloud-sdk-python-cloudstudio-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      761 2023-07-18 00:20:42.000000 tencentcloud-sdk-python-cloudstudio-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:42.000000 tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud_sdk_python_cloudstudio.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:20:42.000000 tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud_sdk_python_cloudstudio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      723 2023-07-18 00:20:42.000000 tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud_sdk_python_cloudstudio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1699 2023-07-18 00:20:42.000000 tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud_sdk_python_cloudstudio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:20:42.000000 tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud_sdk_python_cloudstudio.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:48.000000 tencentcloud-sdk-python-cloudstudio-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-07-19 00:24:48.000000 tencentcloud-sdk-python-cloudstudio-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:48.000000 tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:48.000000 tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud/cloudstudio/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:24:48.000000 tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud/cloudstudio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:48.000000 tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud/cloudstudio/v20210524/
+-rw-r--r--   0 root         (0) root         (0)    21897 2023-07-19 00:24:48.000000 tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud/cloudstudio/v20210524/cloudstudio_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:24:48.000000 tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud/cloudstudio/v20210524/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      828 2023-07-19 00:24:48.000000 tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud/cloudstudio/v20210524/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   112109 2023-07-19 00:24:48.000000 tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud/cloudstudio/v20210524/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:48.000000 tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud/cloudstudio/v20230508/
+-rw-r--r--   0 root         (0) root         (0)     8995 2023-07-19 00:24:48.000000 tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud/cloudstudio/v20230508/cloudstudio_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:24:48.000000 tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud/cloudstudio/v20230508/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      979 2023-07-19 00:24:48.000000 tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud/cloudstudio/v20230508/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    33456 2023-07-19 00:24:48.000000 tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud/cloudstudio/v20230508/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:24:48.000000 tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:24:48.000000 tencentcloud-sdk-python-cloudstudio-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-07-19 00:24:48.000000 tencentcloud-sdk-python-cloudstudio-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      761 2023-07-19 00:24:48.000000 tencentcloud-sdk-python-cloudstudio-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:48.000000 tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud_sdk_python_cloudstudio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:24:48.000000 tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud_sdk_python_cloudstudio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      723 2023-07-19 00:24:48.000000 tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud_sdk_python_cloudstudio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-07-19 00:24:48.000000 tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud_sdk_python_cloudstudio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:24:48.000000 tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud_sdk_python_cloudstudio.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.937/setup.py` & `tencentcloud-sdk-python-cloudstudio-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud/cloudstudio/v20210524/cloudstudio_client.py` & `tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud/cloudstudio/v20210524/cloudstudio_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateCustomizeTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateWorkspaceByAgent(self, request):
         """云服务器方式创建工作空间
 
         :param request: Request instance for CreateWorkspaceByAgent.
         :type request: :class:`tencentcloud.cloudstudio.v20210524.models.CreateWorkspaceByAgentRequest`
@@ -65,15 +65,15 @@
             model = models.CreateWorkspaceByAgentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateWorkspaceByTemplate(self, request):
         """快速开始, 基于模板创建工作空间
 
         :param request: Request instance for CreateWorkspaceByTemplate.
         :type request: :class:`tencentcloud.cloudstudio.v20210524.models.CreateWorkspaceByTemplateRequest`
@@ -88,15 +88,15 @@
             model = models.CreateWorkspaceByTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateWorkspaceByVersionControl(self, request):
         """根据模板创建工作空间
 
         :param request: Request instance for CreateWorkspaceByVersionControl.
         :type request: :class:`tencentcloud.cloudstudio.v20210524.models.CreateWorkspaceByVersionControlRequest`
@@ -111,15 +111,15 @@
             model = models.CreateWorkspaceByVersionControlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateWorkspaceTemporaryToken(self, request):
         """为工作空间创建临时访问凭证，重复调用会创建新的 Token，旧的 Token 将会自动失效
 
         :param request: Request instance for CreateWorkspaceTemporaryToken.
         :type request: :class:`tencentcloud.cloudstudio.v20210524.models.CreateWorkspaceTemporaryTokenRequest`
@@ -134,15 +134,15 @@
             model = models.CreateWorkspaceTemporaryTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCustomizeTemplatesById(self, request):
         """删除自定义模板
 
         :param request: Request instance for DeleteCustomizeTemplatesById.
         :type request: :class:`tencentcloud.cloudstudio.v20210524.models.DeleteCustomizeTemplatesByIdRequest`
@@ -157,15 +157,15 @@
             model = models.DeleteCustomizeTemplatesByIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCustomizeTemplates(self, request):
         """获取所有模板列表
 
         :param request: Request instance for DescribeCustomizeTemplates.
         :type request: :class:`tencentcloud.cloudstudio.v20210524.models.DescribeCustomizeTemplatesRequest`
@@ -180,15 +180,15 @@
             model = models.DescribeCustomizeTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCustomizeTemplatesById(self, request):
         """获取特定模板信息
 
         :param request: Request instance for DescribeCustomizeTemplatesById.
         :type request: :class:`tencentcloud.cloudstudio.v20210524.models.DescribeCustomizeTemplatesByIdRequest`
@@ -203,15 +203,15 @@
             model = models.DescribeCustomizeTemplatesByIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCustomizeTemplatesPresets(self, request):
         """获取创建模板的预置参数
 
         :param request: Request instance for DescribeCustomizeTemplatesPresets.
         :type request: :class:`tencentcloud.cloudstudio.v20210524.models.DescribeCustomizeTemplatesPresetsRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeCustomizeTemplatesPresetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWorkspaceEnvList(self, request):
         """环境列表接口返回信息
 
         :param request: Request instance for DescribeWorkspaceEnvList.
         :type request: :class:`tencentcloud.cloudstudio.v20210524.models.DescribeWorkspaceEnvListRequest`
@@ -249,15 +249,15 @@
             model = models.DescribeWorkspaceEnvListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWorkspaceIsReady(self, request):
         """获取工作空间是否已经启动就绪
 
         :param request: Request instance for DescribeWorkspaceIsReady.
         :type request: :class:`tencentcloud.cloudstudio.v20210524.models.DescribeWorkspaceIsReadyRequest`
@@ -272,15 +272,15 @@
             model = models.DescribeWorkspaceIsReadyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWorkspaceNameExist(self, request):
         """检查工作空间是否存在
 
         :param request: Request instance for DescribeWorkspaceNameExist.
         :type request: :class:`tencentcloud.cloudstudio.v20210524.models.DescribeWorkspaceNameExistRequest`
@@ -295,15 +295,15 @@
             model = models.DescribeWorkspaceNameExistResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWorkspaceStatus(self, request):
         """获取工作空间元信息
 
         :param request: Request instance for DescribeWorkspaceStatus.
         :type request: :class:`tencentcloud.cloudstudio.v20210524.models.DescribeWorkspaceStatusRequest`
@@ -318,15 +318,15 @@
             model = models.DescribeWorkspaceStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWorkspaceStatusList(self, request):
         """获取用户工作空间列表
 
         :param request: Request instance for DescribeWorkspaceStatusList.
         :type request: :class:`tencentcloud.cloudstudio.v20210524.models.DescribeWorkspaceStatusListRequest`
@@ -341,15 +341,15 @@
             model = models.DescribeWorkspaceStatusListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCustomizeTemplateVersionControl(self, request):
         """修改模板默认代码仓库
 
         :param request: Request instance for ModifyCustomizeTemplateVersionControl.
         :type request: :class:`tencentcloud.cloudstudio.v20210524.models.ModifyCustomizeTemplateVersionControlRequest`
@@ -364,15 +364,15 @@
             model = models.ModifyCustomizeTemplateVersionControlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCustomizeTemplatesFullById(self, request):
         """全量修改自定义模板，不忽略空
 
         :param request: Request instance for ModifyCustomizeTemplatesFullById.
         :type request: :class:`tencentcloud.cloudstudio.v20210524.models.ModifyCustomizeTemplatesFullByIdRequest`
@@ -387,15 +387,15 @@
             model = models.ModifyCustomizeTemplatesFullByIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCustomizeTemplatesPartById(self, request):
         """全量修改自定义模板，忽略空
 
         :param request: Request instance for ModifyCustomizeTemplatesPartById.
         :type request: :class:`tencentcloud.cloudstudio.v20210524.models.ModifyCustomizeTemplatesPartByIdRequest`
@@ -410,15 +410,15 @@
             model = models.ModifyCustomizeTemplatesPartByIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyWorkspaceAttributes(self, request):
         """修改工作空间的名称和描述
 
         :param request: Request instance for ModifyWorkspaceAttributes.
         :type request: :class:`tencentcloud.cloudstudio.v20210524.models.ModifyWorkspaceAttributesRequest`
@@ -433,15 +433,15 @@
             model = models.ModifyWorkspaceAttributesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RecoverWorkspace(self, request):
         """恢复工作空间
 
         :param request: Request instance for RecoverWorkspace.
         :type request: :class:`tencentcloud.cloudstudio.v20210524.models.RecoverWorkspaceRequest`
@@ -456,15 +456,15 @@
             model = models.RecoverWorkspaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RemoveWorkspace(self, request):
         """删除工作空间
 
         :param request: Request instance for RemoveWorkspace.
         :type request: :class:`tencentcloud.cloudstudio.v20210524.models.RemoveWorkspaceRequest`
@@ -479,15 +479,15 @@
             model = models.RemoveWorkspaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RunWorkspace(self, request):
         """运行空间
 
         :param request: Request instance for RunWorkspace.
         :type request: :class:`tencentcloud.cloudstudio.v20210524.models.RunWorkspaceRequest`
@@ -502,15 +502,15 @@
             model = models.RunWorkspaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopWorkspace(self, request):
         """停止运行空间
 
         :param request: Request instance for StopWorkspace.
         :type request: :class:`tencentcloud.cloudstudio.v20210524.models.StopWorkspaceRequest`
@@ -525,8 +525,8 @@
             model = models.StopWorkspaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud/cloudstudio/v20210524/errorcodes.py` & `tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud/cloudstudio/v20210524/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud/cloudstudio/v20210524/models.py` & `tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud/cloudstudio/v20210524/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud/cloudstudio/v20230508/cloudstudio_client.py` & `tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud/cloudstudio/v20230508/cloudstudio_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateWorkspaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateWorkspaceToken(self, request):
         """为工作空间创建临时访问凭证，重复调用会创建新的 Token，旧的 Token 将会自动失效
 
         :param request: Request instance for CreateWorkspaceToken.
         :type request: :class:`tencentcloud.cloudstudio.v20230508.models.CreateWorkspaceTokenRequest`
@@ -65,15 +65,15 @@
             model = models.CreateWorkspaceTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConfig(self, request):
         """获取用户配置
 
         :param request: Request instance for DescribeConfig.
         :type request: :class:`tencentcloud.cloudstudio.v20230508.models.DescribeConfigRequest`
@@ -88,15 +88,15 @@
             model = models.DescribeConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImages(self, request):
         """获取基础镜像列表
 
         :param request: Request instance for DescribeImages.
         :type request: :class:`tencentcloud.cloudstudio.v20230508.models.DescribeImagesRequest`
@@ -111,15 +111,15 @@
             model = models.DescribeImagesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWorkspaces(self, request):
         """获取用户工作空间列表
 
         :param request: Request instance for DescribeWorkspaces.
         :type request: :class:`tencentcloud.cloudstudio.v20230508.models.DescribeWorkspacesRequest`
@@ -134,15 +134,15 @@
             model = models.DescribeWorkspacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyWorkspace(self, request):
         """修改工作空间
 
         :param request: Request instance for ModifyWorkspace.
         :type request: :class:`tencentcloud.cloudstudio.v20230508.models.ModifyWorkspaceRequest`
@@ -157,15 +157,15 @@
             model = models.ModifyWorkspaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RemoveWorkspace(self, request):
         """删除工作空间
 
         :param request: Request instance for RemoveWorkspace.
         :type request: :class:`tencentcloud.cloudstudio.v20230508.models.RemoveWorkspaceRequest`
@@ -180,15 +180,15 @@
             model = models.RemoveWorkspaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RunWorkspace(self, request):
         """运行空间
 
         :param request: Request instance for RunWorkspace.
         :type request: :class:`tencentcloud.cloudstudio.v20230508.models.RunWorkspaceRequest`
@@ -203,15 +203,15 @@
             model = models.RunWorkspaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopWorkspace(self, request):
         """停止运行空间
 
         :param request: Request instance for StopWorkspace.
         :type request: :class:`tencentcloud.cloudstudio.v20230508.models.StopWorkspaceRequest`
@@ -226,8 +226,8 @@
             model = models.StopWorkspaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud/cloudstudio/v20230508/errorcodes.py` & `tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud/cloudstudio/v20230508/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud/cloudstudio/v20230508/models.py` & `tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud/cloudstudio/v20230508/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-cloudstudio-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cloudstudio
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cloudstudio SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.937/README.rst` & `tencentcloud-sdk-python-cloudstudio-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud_sdk_python_cloudstudio.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud_sdk_python_cloudstudio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudstudio-3.0.937/tencentcloud_sdk_python_cloudstudio.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cloudstudio-3.0.938/tencentcloud_sdk_python_cloudstudio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cloudstudio
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cloudstudio SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

