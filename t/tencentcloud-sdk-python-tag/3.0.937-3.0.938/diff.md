# Comparing `tmp/tencentcloud-sdk-python-tag-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tag-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tag-3.0.937.tar", last modified: Tue Jul 18 00:30:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tag-3.0.938.tar", last modified: Wed Jul 19 00:48:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tag-3.0.937.tar` & `tencentcloud-sdk-python-tag-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:45.000000 tencentcloud-sdk-python-tag-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:30:45.000000 tencentcloud-sdk-python-tag-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:45.000000 tencentcloud-sdk-python-tag-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:45.000000 tencentcloud-sdk-python-tag-3.0.937/tencentcloud/tag/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:45.000000 tencentcloud-sdk-python-tag-3.0.937/tencentcloud/tag/v20180813/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:30:45.000000 tencentcloud-sdk-python-tag-3.0.937/tencentcloud/tag/v20180813/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5579 2023-07-18 00:30:45.000000 tencentcloud-sdk-python-tag-3.0.937/tencentcloud/tag/v20180813/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    28544 2023-07-18 00:30:45.000000 tencentcloud-sdk-python-tag-3.0.937/tencentcloud/tag/v20180813/tag_client.py
--rw-r--r--   0 root         (0) root         (0)   121329 2023-07-18 00:30:45.000000 tencentcloud-sdk-python-tag-3.0.937/tencentcloud/tag/v20180813/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:30:45.000000 tencentcloud-sdk-python-tag-3.0.937/tencentcloud/tag/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:30:45.000000 tencentcloud-sdk-python-tag-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:30:45.000000 tencentcloud-sdk-python-tag-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:45.000000 tencentcloud-sdk-python-tag-3.0.937/tencentcloud_sdk_python_tag.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:30:45.000000 tencentcloud-sdk-python-tag-3.0.937/tencentcloud_sdk_python_tag.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:30:45.000000 tencentcloud-sdk-python-tag-3.0.937/tencentcloud_sdk_python_tag.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:30:45.000000 tencentcloud-sdk-python-tag-3.0.937/tencentcloud_sdk_python_tag.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:30:45.000000 tencentcloud-sdk-python-tag-3.0.937/tencentcloud_sdk_python_tag.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:30:45.000000 tencentcloud-sdk-python-tag-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:30:45.000000 tencentcloud-sdk-python-tag-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:07.000000 tencentcloud-sdk-python-tag-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:48:07.000000 tencentcloud-sdk-python-tag-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:07.000000 tencentcloud-sdk-python-tag-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:07.000000 tencentcloud-sdk-python-tag-3.0.938/tencentcloud/tag/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:07.000000 tencentcloud-sdk-python-tag-3.0.938/tencentcloud/tag/v20180813/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:48:07.000000 tencentcloud-sdk-python-tag-3.0.938/tencentcloud/tag/v20180813/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5579 2023-07-19 00:48:07.000000 tencentcloud-sdk-python-tag-3.0.938/tencentcloud/tag/v20180813/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    28668 2023-07-19 00:48:07.000000 tencentcloud-sdk-python-tag-3.0.938/tencentcloud/tag/v20180813/tag_client.py
+-rw-r--r--   0 root         (0) root         (0)   121329 2023-07-19 00:48:07.000000 tencentcloud-sdk-python-tag-3.0.938/tencentcloud/tag/v20180813/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:48:07.000000 tencentcloud-sdk-python-tag-3.0.938/tencentcloud/tag/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:48:07.000000 tencentcloud-sdk-python-tag-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:48:07.000000 tencentcloud-sdk-python-tag-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:07.000000 tencentcloud-sdk-python-tag-3.0.938/tencentcloud_sdk_python_tag.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:48:07.000000 tencentcloud-sdk-python-tag-3.0.938/tencentcloud_sdk_python_tag.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:48:07.000000 tencentcloud-sdk-python-tag-3.0.938/tencentcloud_sdk_python_tag.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:48:07.000000 tencentcloud-sdk-python-tag-3.0.938/tencentcloud_sdk_python_tag.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:48:07.000000 tencentcloud-sdk-python-tag-3.0.938/tencentcloud_sdk_python_tag.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:48:07.000000 tencentcloud-sdk-python-tag-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:48:07.000000 tencentcloud-sdk-python-tag-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-tag-3.0.937/setup.py` & `tencentcloud-sdk-python-tag-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tag-3.0.937/tencentcloud/tag/v20180813/errorcodes.py` & `tencentcloud-sdk-python-tag-3.0.938/tencentcloud/tag/v20180813/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tag-3.0.937/tencentcloud/tag/v20180813/tag_client.py` & `tencentcloud-sdk-python-tag-3.0.938/tencentcloud/tag/v20180813/tag_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AddProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddResourceTag(self, request):
         """本接口用于给标签关联资源
 
         :param request: Request instance for AddResourceTag.
         :type request: :class:`tencentcloud.tag.v20180813.models.AddResourceTagRequest`
@@ -65,15 +65,15 @@
             model = models.AddResourceTagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AttachResourcesTag(self, request):
         """给多个资源关联某个标签
 
         :param request: Request instance for AttachResourcesTag.
         :type request: :class:`tencentcloud.tag.v20180813.models.AttachResourcesTagRequest`
@@ -88,15 +88,15 @@
             model = models.AttachResourcesTagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTag(self, request):
         """本接口用于创建一对标签键和标签值
 
         :param request: Request instance for CreateTag.
         :type request: :class:`tencentcloud.tag.v20180813.models.CreateTagRequest`
@@ -111,15 +111,15 @@
             model = models.CreateTagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTags(self, request):
         """本接口用于创建多对标签键和标签值
 
         :param request: Request instance for CreateTags.
         :type request: :class:`tencentcloud.tag.v20180813.models.CreateTagsRequest`
@@ -134,15 +134,15 @@
             model = models.CreateTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteResourceTag(self, request):
         """本接口用于解除标签和资源的关联关系
 
         :param request: Request instance for DeleteResourceTag.
         :type request: :class:`tencentcloud.tag.v20180813.models.DeleteResourceTagRequest`
@@ -157,15 +157,15 @@
             model = models.DeleteResourceTagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTag(self, request):
         """本接口用于删除一对标签键和标签值
 
         :param request: Request instance for DeleteTag.
         :type request: :class:`tencentcloud.tag.v20180813.models.DeleteTagRequest`
@@ -180,15 +180,15 @@
             model = models.DeleteTagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTags(self, request):
         """本接口用于批量删除标签键和标签值。
 
         :param request: Request instance for DeleteTags.
         :type request: :class:`tencentcloud.tag.v20180813.models.DeleteTagsRequest`
@@ -203,15 +203,15 @@
             model = models.DeleteTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProjects(self, request):
         """获取项目列表
 
         :param request: Request instance for DescribeProjects.
         :type request: :class:`tencentcloud.tag.v20180813.models.DescribeProjectsRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeProjectsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourceTags(self, request):
         """查询资源关联标签
 
         :param request: Request instance for DescribeResourceTags.
         :type request: :class:`tencentcloud.tag.v20180813.models.DescribeResourceTagsRequest`
@@ -249,15 +249,15 @@
             model = models.DescribeResourceTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourceTagsByResourceIds(self, request):
         """用于批量查询已有资源关联的标签键值对
 
         :param request: Request instance for DescribeResourceTagsByResourceIds.
         :type request: :class:`tencentcloud.tag.v20180813.models.DescribeResourceTagsByResourceIdsRequest`
@@ -272,15 +272,15 @@
             model = models.DescribeResourceTagsByResourceIdsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourceTagsByResourceIdsSeq(self, request):
         """按顺序查看资源关联的标签
 
         :param request: Request instance for DescribeResourceTagsByResourceIdsSeq.
         :type request: :class:`tencentcloud.tag.v20180813.models.DescribeResourceTagsByResourceIdsSeqRequest`
@@ -295,15 +295,15 @@
             model = models.DescribeResourceTagsByResourceIdsSeqResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourceTagsByTagKeys(self, request):
         """根据标签键获取资源标签
 
         :param request: Request instance for DescribeResourceTagsByTagKeys.
         :type request: :class:`tencentcloud.tag.v20180813.models.DescribeResourceTagsByTagKeysRequest`
@@ -318,15 +318,15 @@
             model = models.DescribeResourceTagsByTagKeysResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourcesByTags(self, request):
         """通过标签查询资源列表
 
         :param request: Request instance for DescribeResourcesByTags.
         :type request: :class:`tencentcloud.tag.v20180813.models.DescribeResourcesByTagsRequest`
@@ -341,15 +341,15 @@
             model = models.DescribeResourcesByTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourcesByTagsUnion(self, request):
         """通过标签查询资源列表并集
 
         :param request: Request instance for DescribeResourcesByTagsUnion.
         :type request: :class:`tencentcloud.tag.v20180813.models.DescribeResourcesByTagsUnionRequest`
@@ -364,15 +364,15 @@
             model = models.DescribeResourcesByTagsUnionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTagKeys(self, request):
         """用于查询已建立的标签列表中的标签键。
 
         :param request: Request instance for DescribeTagKeys.
         :type request: :class:`tencentcloud.tag.v20180813.models.DescribeTagKeysRequest`
@@ -387,15 +387,15 @@
             model = models.DescribeTagKeysResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTagValues(self, request):
         """用于查询已建立的标签列表中的标签值。
 
         :param request: Request instance for DescribeTagValues.
         :type request: :class:`tencentcloud.tag.v20180813.models.DescribeTagValuesRequest`
@@ -410,15 +410,15 @@
             model = models.DescribeTagValuesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTagValuesSeq(self, request):
         """用于查询已建立的标签列表中的标签值。
 
         :param request: Request instance for DescribeTagValuesSeq.
         :type request: :class:`tencentcloud.tag.v20180813.models.DescribeTagValuesSeqRequest`
@@ -433,15 +433,15 @@
             model = models.DescribeTagValuesSeqResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTags(self, request):
         """用于查询已建立的标签列表。
 
         :param request: Request instance for DescribeTags.
         :type request: :class:`tencentcloud.tag.v20180813.models.DescribeTagsRequest`
@@ -456,15 +456,15 @@
             model = models.DescribeTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTagsSeq(self, request):
         """用于查询已建立的标签列表。
 
         :param request: Request instance for DescribeTagsSeq.
         :type request: :class:`tencentcloud.tag.v20180813.models.DescribeTagsSeqRequest`
@@ -479,15 +479,15 @@
             model = models.DescribeTagsSeqResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetachResourcesTag(self, request):
         """解绑多个资源关联的某个标签
 
         :param request: Request instance for DetachResourcesTag.
         :type request: :class:`tencentcloud.tag.v20180813.models.DetachResourcesTagRequest`
@@ -502,15 +502,15 @@
             model = models.DetachResourcesTagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetResources(self, request):
         """查询绑定了标签的资源列表。
 
         :param request: Request instance for GetResources.
         :type request: :class:`tencentcloud.tag.v20180813.models.GetResourcesRequest`
@@ -525,15 +525,15 @@
             model = models.GetResourcesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetTagKeys(self, request):
         """查询标签键列表。
 
         :param request: Request instance for GetTagKeys.
         :type request: :class:`tencentcloud.tag.v20180813.models.GetTagKeysRequest`
@@ -548,15 +548,15 @@
             model = models.GetTagKeysResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetTagValues(self, request):
         """用于查询已建立的标签列表中的标签值。
 
         :param request: Request instance for GetTagValues.
         :type request: :class:`tencentcloud.tag.v20180813.models.GetTagValuesRequest`
@@ -571,15 +571,15 @@
             model = models.GetTagValuesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetTags(self, request):
         """用于获取已建立的标签列表。
 
         :param request: Request instance for GetTags.
         :type request: :class:`tencentcloud.tag.v20180813.models.GetTagsRequest`
@@ -594,15 +594,15 @@
             model = models.GetTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyResourceTags(self, request):
         """本接口用于修改资源关联的所有标签
 
         :param request: Request instance for ModifyResourceTags.
         :type request: :class:`tencentcloud.tag.v20180813.models.ModifyResourceTagsRequest`
@@ -617,15 +617,15 @@
             model = models.ModifyResourceTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyResourcesTagValue(self, request):
         """修改多个资源关联的某个标签键对应的标签值
 
         :param request: Request instance for ModifyResourcesTagValue.
         :type request: :class:`tencentcloud.tag.v20180813.models.ModifyResourcesTagValueRequest`
@@ -640,15 +640,15 @@
             model = models.ModifyResourcesTagValueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TagResources(self, request):
         """为指定的多个云产品的多个云资源统一创建并绑定标签。
 
         :param request: Request instance for TagResources.
         :type request: :class:`tencentcloud.tag.v20180813.models.TagResourcesRequest`
@@ -663,15 +663,15 @@
             model = models.TagResourcesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnTagResources(self, request):
         """指定的多个云产品的多个云资源统一解绑标签。
 
         :param request: Request instance for UnTagResources.
         :type request: :class:`tencentcloud.tag.v20180813.models.UnTagResourcesRequest`
@@ -686,15 +686,15 @@
             model = models.UnTagResourcesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateProject(self, request):
         """修改项目
 
         :param request: Request instance for UpdateProject.
         :type request: :class:`tencentcloud.tag.v20180813.models.UpdateProjectRequest`
@@ -709,15 +709,15 @@
             model = models.UpdateProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateResourceTagValue(self, request):
         """本接口用于修改资源已关联的标签值（标签键不变）
 
         :param request: Request instance for UpdateResourceTagValue.
         :type request: :class:`tencentcloud.tag.v20180813.models.UpdateResourceTagValueRequest`
@@ -732,8 +732,8 @@
             model = models.UpdateResourceTagValueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tag-3.0.937/tencentcloud/tag/v20180813/models.py` & `tencentcloud-sdk-python-tag-3.0.938/tencentcloud/tag/v20180813/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tag-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tag-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tag-3.0.937/tencentcloud_sdk_python_tag.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tag-3.0.938/tencentcloud_sdk_python_tag.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tag
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tag SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tag-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tag-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tag
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tag SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tag-3.0.937/README.rst` & `tencentcloud-sdk-python-tag-3.0.938/README.rst`

 * *Files identical despite different names*

