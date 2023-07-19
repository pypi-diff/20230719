# Comparing `tmp/tencentcloud-sdk-python-irp-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-irp-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-irp-3.0.937.tar", last modified: Tue Jul 18 00:26:11 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-irp-3.0.938.tar", last modified: Wed Jul 19 00:41:34 2023, max compression
```

## Comparing `tencentcloud-sdk-python-irp-3.0.937.tar` & `tencentcloud-sdk-python-irp-3.0.938.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:11.000000 tencentcloud-sdk-python-irp-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:26:10.000000 tencentcloud-sdk-python-irp-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:11.000000 tencentcloud-sdk-python-irp-3.0.937/tencentcloud_sdk_python_irp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:26:11.000000 tencentcloud-sdk-python-irp-3.0.937/tencentcloud_sdk_python_irp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-18 00:26:11.000000 tencentcloud-sdk-python-irp-3.0.937/tencentcloud_sdk_python_irp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:26:11.000000 tencentcloud-sdk-python-irp-3.0.937/tencentcloud_sdk_python_irp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:26:11.000000 tencentcloud-sdk-python-irp-3.0.937/tencentcloud_sdk_python_irp.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:11.000000 tencentcloud-sdk-python-irp-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:26:10.000000 tencentcloud-sdk-python-irp-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:11.000000 tencentcloud-sdk-python-irp-3.0.937/tencentcloud/irp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:11.000000 tencentcloud-sdk-python-irp-3.0.937/tencentcloud/irp/v20220805/
--rw-r--r--   0 root         (0) root         (0)     7337 2023-07-18 00:26:10.000000 tencentcloud-sdk-python-irp-3.0.937/tencentcloud/irp/v20220805/irp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:26:10.000000 tencentcloud-sdk-python-irp-3.0.937/tencentcloud/irp/v20220805/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-07-18 00:26:10.000000 tencentcloud-sdk-python-irp-3.0.937/tencentcloud/irp/v20220805/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    81404 2023-07-18 00:26:10.000000 tencentcloud-sdk-python-irp-3.0.937/tencentcloud/irp/v20220805/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:11.000000 tencentcloud-sdk-python-irp-3.0.937/tencentcloud/irp/v20220324/
--rw-r--r--   0 root         (0) root         (0)     4373 2023-07-18 00:26:10.000000 tencentcloud-sdk-python-irp-3.0.937/tencentcloud/irp/v20220324/irp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:26:10.000000 tencentcloud-sdk-python-irp-3.0.937/tencentcloud/irp/v20220324/__init__.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-07-18 00:26:10.000000 tencentcloud-sdk-python-irp-3.0.937/tencentcloud/irp/v20220324/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    54088 2023-07-18 00:26:10.000000 tencentcloud-sdk-python-irp-3.0.937/tencentcloud/irp/v20220324/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:26:10.000000 tencentcloud-sdk-python-irp-3.0.937/tencentcloud/irp/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:26:11.000000 tencentcloud-sdk-python-irp-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:26:11.000000 tencentcloud-sdk-python-irp-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:26:10.000000 tencentcloud-sdk-python-irp-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:34.000000 tencentcloud-sdk-python-irp-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:41:34.000000 tencentcloud-sdk-python-irp-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:34.000000 tencentcloud-sdk-python-irp-3.0.938/tencentcloud_sdk_python_irp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:41:34.000000 tencentcloud-sdk-python-irp-3.0.938/tencentcloud_sdk_python_irp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-19 00:41:34.000000 tencentcloud-sdk-python-irp-3.0.938/tencentcloud_sdk_python_irp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:41:34.000000 tencentcloud-sdk-python-irp-3.0.938/tencentcloud_sdk_python_irp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:41:34.000000 tencentcloud-sdk-python-irp-3.0.938/tencentcloud_sdk_python_irp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:34.000000 tencentcloud-sdk-python-irp-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:41:34.000000 tencentcloud-sdk-python-irp-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:34.000000 tencentcloud-sdk-python-irp-3.0.938/tencentcloud/irp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:34.000000 tencentcloud-sdk-python-irp-3.0.938/tencentcloud/irp/v20220805/
+-rw-r--r--   0 root         (0) root         (0)     7365 2023-07-19 00:41:34.000000 tencentcloud-sdk-python-irp-3.0.938/tencentcloud/irp/v20220805/irp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:41:34.000000 tencentcloud-sdk-python-irp-3.0.938/tencentcloud/irp/v20220805/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-07-19 00:41:34.000000 tencentcloud-sdk-python-irp-3.0.938/tencentcloud/irp/v20220805/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    81404 2023-07-19 00:41:34.000000 tencentcloud-sdk-python-irp-3.0.938/tencentcloud/irp/v20220805/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:34.000000 tencentcloud-sdk-python-irp-3.0.938/tencentcloud/irp/v20220324/
+-rw-r--r--   0 root         (0) root         (0)     4389 2023-07-19 00:41:34.000000 tencentcloud-sdk-python-irp-3.0.938/tencentcloud/irp/v20220324/irp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:41:34.000000 tencentcloud-sdk-python-irp-3.0.938/tencentcloud/irp/v20220324/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-07-19 00:41:34.000000 tencentcloud-sdk-python-irp-3.0.938/tencentcloud/irp/v20220324/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    54088 2023-07-19 00:41:34.000000 tencentcloud-sdk-python-irp-3.0.938/tencentcloud/irp/v20220324/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:41:34.000000 tencentcloud-sdk-python-irp-3.0.938/tencentcloud/irp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:41:34.000000 tencentcloud-sdk-python-irp-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:41:34.000000 tencentcloud-sdk-python-irp-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:41:34.000000 tencentcloud-sdk-python-irp-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-irp-3.0.937/setup.py` & `tencentcloud-sdk-python-irp-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-irp-3.0.937/tencentcloud_sdk_python_irp.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-irp-3.0.938/tencentcloud_sdk_python_irp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-irp-3.0.937/tencentcloud_sdk_python_irp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-irp-3.0.938/tencentcloud_sdk_python_irp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-irp
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Irp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-irp-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-irp-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-irp-3.0.937/tencentcloud/irp/v20220805/irp_client.py` & `tencentcloud-sdk-python-irp-3.0.938/tencentcloud/irp/v20220805/irp_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.DescribeGoodsRecommendResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def FeedRecommend(self, request):
         """获取信息流推荐结果
 
         :param request: Request instance for FeedRecommend.
         :type request: :class:`tencentcloud.irp.v20220805.models.FeedRecommendRequest`
@@ -65,15 +65,15 @@
             model = models.FeedRecommendResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReportFeedBehavior(self, request):
         """上报信息流场景内的行为数据，随着数据的积累，模型的效果会逐渐稳定。
 
         :param request: Request instance for ReportFeedBehavior.
         :type request: :class:`tencentcloud.irp.v20220805.models.ReportFeedBehaviorRequest`
@@ -88,15 +88,15 @@
             model = models.ReportFeedBehaviorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReportFeedItem(self, request):
         """上报被用于推荐的信息流内容信息
 
         :param request: Request instance for ReportFeedItem.
         :type request: :class:`tencentcloud.irp.v20220805.models.ReportFeedItemRequest`
@@ -111,15 +111,15 @@
             model = models.ReportFeedItemResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReportFeedUser(self, request):
         """上报信息流用户信息，请务必确认用户的唯一性，并在请求推荐结果时指定用户的唯一标识信息（UserId），否则将无法进行千人千面的推荐
 
         :param request: Request instance for ReportFeedUser.
         :type request: :class:`tencentcloud.irp.v20220805.models.ReportFeedUserRequest`
@@ -134,15 +134,15 @@
             model = models.ReportFeedUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReportGoodsBehavior(self, request):
         """上报电商类行为数据
 
         :param request: Request instance for ReportGoodsBehavior.
         :type request: :class:`tencentcloud.irp.v20220805.models.ReportGoodsBehaviorRequest`
@@ -157,15 +157,15 @@
             model = models.ReportGoodsBehaviorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReportGoodsInfo(self, request):
         """上报电商类商品信息
 
         :param request: Request instance for ReportGoodsInfo.
         :type request: :class:`tencentcloud.irp.v20220805.models.ReportGoodsInfoRequest`
@@ -180,8 +180,8 @@
             model = models.ReportGoodsInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-irp-3.0.937/tencentcloud/irp/v20220805/errorcodes.py` & `tencentcloud-sdk-python-irp-3.0.938/tencentcloud/irp/v20220805/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-irp-3.0.937/tencentcloud/irp/v20220805/models.py` & `tencentcloud-sdk-python-irp-3.0.938/tencentcloud/irp/v20220805/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-irp-3.0.937/tencentcloud/irp/v20220324/irp_client.py` & `tencentcloud-sdk-python-irp-3.0.938/tencentcloud/irp/v20220324/irp_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.RecommendContentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReportAction(self, request):
         """上报行为
 
         :param request: Request instance for ReportAction.
         :type request: :class:`tencentcloud.irp.v20220324.models.ReportActionRequest`
@@ -65,15 +65,15 @@
             model = models.ReportActionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReportMaterial(self, request):
         """上报物料
 
         :param request: Request instance for ReportMaterial.
         :type request: :class:`tencentcloud.irp.v20220324.models.ReportMaterialRequest`
@@ -88,15 +88,15 @@
             model = models.ReportMaterialResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReportPortrait(self, request):
         """上报用户画像
 
         :param request: Request instance for ReportPortrait.
         :type request: :class:`tencentcloud.irp.v20220324.models.ReportPortraitRequest`
@@ -111,8 +111,8 @@
             model = models.ReportPortraitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-irp-3.0.937/tencentcloud/irp/v20220324/errorcodes.py` & `tencentcloud-sdk-python-irp-3.0.938/tencentcloud/irp/v20220324/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-irp-3.0.937/tencentcloud/irp/v20220324/models.py` & `tencentcloud-sdk-python-irp-3.0.938/tencentcloud/irp/v20220324/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-irp-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-irp-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-irp
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Irp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-irp-3.0.937/README.rst` & `tencentcloud-sdk-python-irp-3.0.938/README.rst`

 * *Files identical despite different names*

