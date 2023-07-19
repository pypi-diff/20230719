# Comparing `tmp/tencentcloud-sdk-python-tbm-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tbm-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tbm-3.0.937.tar", last modified: Tue Jul 18 00:31:08 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tbm-3.0.938.tar", last modified: Wed Jul 19 00:48:33 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tbm-3.0.937.tar` & `tencentcloud-sdk-python-tbm-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:08.000000 tencentcloud-sdk-python-tbm-3.0.937/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:08.000000 tencentcloud-sdk-python-tbm-3.0.937/tencentcloud_sdk_python_tbm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:31:08.000000 tencentcloud-sdk-python-tbm-3.0.937/tencentcloud_sdk_python_tbm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:31:08.000000 tencentcloud-sdk-python-tbm-3.0.937/tencentcloud_sdk_python_tbm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:31:08.000000 tencentcloud-sdk-python-tbm-3.0.937/tencentcloud_sdk_python_tbm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:31:08.000000 tencentcloud-sdk-python-tbm-3.0.937/tencentcloud_sdk_python_tbm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:31:08.000000 tencentcloud-sdk-python-tbm-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:08.000000 tencentcloud-sdk-python-tbm-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:31:08.000000 tencentcloud-sdk-python-tbm-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:08.000000 tencentcloud-sdk-python-tbm-3.0.937/tencentcloud/tbm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:31:08.000000 tencentcloud-sdk-python-tbm-3.0.937/tencentcloud/tbm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:08.000000 tencentcloud-sdk-python-tbm-3.0.937/tencentcloud/tbm/v20180129/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:31:08.000000 tencentcloud-sdk-python-tbm-3.0.937/tencentcloud/tbm/v20180129/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1235 2023-07-18 00:31:08.000000 tencentcloud-sdk-python-tbm-3.0.937/tencentcloud/tbm/v20180129/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    10423 2023-07-18 00:31:08.000000 tencentcloud-sdk-python-tbm-3.0.937/tencentcloud/tbm/v20180129/tbm_client.py
--rw-r--r--   0 root         (0) root         (0)    53389 2023-07-18 00:31:08.000000 tencentcloud-sdk-python-tbm-3.0.937/tencentcloud/tbm/v20180129/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:31:08.000000 tencentcloud-sdk-python-tbm-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:31:08.000000 tencentcloud-sdk-python-tbm-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:31:08.000000 tencentcloud-sdk-python-tbm-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:33.000000 tencentcloud-sdk-python-tbm-3.0.938/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:33.000000 tencentcloud-sdk-python-tbm-3.0.938/tencentcloud_sdk_python_tbm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:48:33.000000 tencentcloud-sdk-python-tbm-3.0.938/tencentcloud_sdk_python_tbm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:48:33.000000 tencentcloud-sdk-python-tbm-3.0.938/tencentcloud_sdk_python_tbm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:48:33.000000 tencentcloud-sdk-python-tbm-3.0.938/tencentcloud_sdk_python_tbm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:48:33.000000 tencentcloud-sdk-python-tbm-3.0.938/tencentcloud_sdk_python_tbm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:48:32.000000 tencentcloud-sdk-python-tbm-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:33.000000 tencentcloud-sdk-python-tbm-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:48:32.000000 tencentcloud-sdk-python-tbm-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:33.000000 tencentcloud-sdk-python-tbm-3.0.938/tencentcloud/tbm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:48:32.000000 tencentcloud-sdk-python-tbm-3.0.938/tencentcloud/tbm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:33.000000 tencentcloud-sdk-python-tbm-3.0.938/tencentcloud/tbm/v20180129/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:48:32.000000 tencentcloud-sdk-python-tbm-3.0.938/tencentcloud/tbm/v20180129/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-07-19 00:48:32.000000 tencentcloud-sdk-python-tbm-3.0.938/tencentcloud/tbm/v20180129/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    10459 2023-07-19 00:48:32.000000 tencentcloud-sdk-python-tbm-3.0.938/tencentcloud/tbm/v20180129/tbm_client.py
+-rw-r--r--   0 root         (0) root         (0)    53389 2023-07-19 00:48:32.000000 tencentcloud-sdk-python-tbm-3.0.938/tencentcloud/tbm/v20180129/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:48:33.000000 tencentcloud-sdk-python-tbm-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:48:33.000000 tencentcloud-sdk-python-tbm-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:48:32.000000 tencentcloud-sdk-python-tbm-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-tbm-3.0.937/tencentcloud_sdk_python_tbm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tbm-3.0.938/tencentcloud_sdk_python_tbm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tbm
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tbm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tbm-3.0.937/setup.py` & `tencentcloud-sdk-python-tbm-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbm-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tbm-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tbm-3.0.937/tencentcloud/tbm/v20180129/errorcodes.py` & `tencentcloud-sdk-python-tbm-3.0.938/tencentcloud/tbm/v20180129/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbm-3.0.937/tencentcloud/tbm/v20180129/tbm_client.py` & `tencentcloud-sdk-python-tbm-3.0.938/tencentcloud/tbm/v20180129/tbm_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.DescribeBrandCommentCountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBrandExposure(self, request):
         """监测品牌关键词命中文章标题或全文的文章篇数，按天输出数据。
 
         :param request: Request instance for DescribeBrandExposure.
         :type request: :class:`tencentcloud.tbm.v20180129.models.DescribeBrandExposureRequest`
@@ -65,15 +65,15 @@
             model = models.DescribeBrandExposureResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBrandMediaReport(self, request):
         """监测品牌关键词出现在媒体网站（新闻媒体、网络门户、政府网站、微信公众号、天天快报等）发布资讯标题和正文中的报道数。按天输出结果。
 
         :param request: Request instance for DescribeBrandMediaReport.
         :type request: :class:`tencentcloud.tbm.v20180129.models.DescribeBrandMediaReportRequest`
@@ -88,15 +88,15 @@
             model = models.DescribeBrandMediaReportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBrandNegComments(self, request):
         """通过分析用户在评价品牌时用词的正负面情绪评分，返回品牌热门差评观点列表。
 
         :param request: Request instance for DescribeBrandNegComments.
         :type request: :class:`tencentcloud.tbm.v20180129.models.DescribeBrandNegCommentsRequest`
@@ -111,15 +111,15 @@
             model = models.DescribeBrandNegCommentsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBrandPosComments(self, request):
         """通过分析用户在评价品牌时用词的正负面情绪评分，返回品牌热门好评观点列表。
 
         :param request: Request instance for DescribeBrandPosComments.
         :type request: :class:`tencentcloud.tbm.v20180129.models.DescribeBrandPosCommentsRequest`
@@ -134,15 +134,15 @@
             model = models.DescribeBrandPosCommentsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBrandSocialOpinion(self, request):
         """检测品牌关键词出现在微博、QQ兴趣部落、论坛、博客等个人公开贡献资讯中的内容，每天聚合近30天热度最高的观点列表。
 
         :param request: Request instance for DescribeBrandSocialOpinion.
         :type request: :class:`tencentcloud.tbm.v20180129.models.DescribeBrandSocialOpinionRequest`
@@ -157,15 +157,15 @@
             model = models.DescribeBrandSocialOpinionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBrandSocialReport(self, request):
         """监测品牌关键词出现在微博、QQ兴趣部落、论坛、博客等个人公开贡献资讯中的条数。按天输出数据结果。
 
         :param request: Request instance for DescribeBrandSocialReport.
         :type request: :class:`tencentcloud.tbm.v20180129.models.DescribeBrandSocialReportRequest`
@@ -180,15 +180,15 @@
             model = models.DescribeBrandSocialReportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIndustryNews(self, request):
         """根据客户定制的行业关键词，监测关键词出现在媒体网站（新闻媒体、网络门户、政府网站、微信公众号、天天快报等）发布资讯标题和正文中的报道数，以及文章列表、来源渠道、作者、发布时间等。
 
         :param request: Request instance for DescribeIndustryNews.
         :type request: :class:`tencentcloud.tbm.v20180129.models.DescribeIndustryNewsRequest`
@@ -203,15 +203,15 @@
             model = models.DescribeIndustryNewsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserPortrait(self, request):
         """通过分析洞察参与过品牌媒体互动的用户，比如公开发表品牌的新闻评论、在公开社交渠道发表过对品牌的评价观点等用户，返回用户的画像属性分布，例如性别、年龄、地域、喜爱的明星、喜爱的影视。
 
         :param request: Request instance for DescribeUserPortrait.
         :type request: :class:`tencentcloud.tbm.v20180129.models.DescribeUserPortraitRequest`
@@ -226,8 +226,8 @@
             model = models.DescribeUserPortraitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tbm-3.0.937/tencentcloud/tbm/v20180129/models.py` & `tencentcloud-sdk-python-tbm-3.0.938/tencentcloud/tbm/v20180129/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbm-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tbm-3.0.938/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tbm
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tbm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tbm-3.0.937/README.rst` & `tencentcloud-sdk-python-tbm-3.0.938/README.rst`

 * *Files identical despite different names*

