# Comparing `tmp/tencentcloud-sdk-python-hasim-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-hasim-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-hasim-3.0.937.tar", last modified: Tue Jul 18 00:24:53 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-hasim-3.0.938.tar", last modified: Wed Jul 19 00:40:12 2023, max compression
```

## Comparing `tencentcloud-sdk-python-hasim-3.0.937.tar` & `tencentcloud-sdk-python-hasim-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:53.000000 tencentcloud-sdk-python-hasim-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-18 00:24:52.000000 tencentcloud-sdk-python-hasim-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:53.000000 tencentcloud-sdk-python-hasim-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:24:52.000000 tencentcloud-sdk-python-hasim-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:53.000000 tencentcloud-sdk-python-hasim-3.0.937/tencentcloud/hasim/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:24:52.000000 tencentcloud-sdk-python-hasim-3.0.937/tencentcloud/hasim/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:53.000000 tencentcloud-sdk-python-hasim-3.0.937/tencentcloud/hasim/v20210716/
--rw-r--r--   0 root         (0) root         (0)    19634 2023-07-18 00:24:52.000000 tencentcloud-sdk-python-hasim-3.0.937/tencentcloud/hasim/v20210716/hasim_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:24:52.000000 tencentcloud-sdk-python-hasim-3.0.937/tencentcloud/hasim/v20210716/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1393 2023-07-18 00:24:52.000000 tencentcloud-sdk-python-hasim-3.0.937/tencentcloud/hasim/v20210716/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   123000 2023-07-18 00:24:52.000000 tencentcloud-sdk-python-hasim-3.0.937/tencentcloud/hasim/v20210716/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:24:53.000000 tencentcloud-sdk-python-hasim-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:24:53.000000 tencentcloud-sdk-python-hasim-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-18 00:24:52.000000 tencentcloud-sdk-python-hasim-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:53.000000 tencentcloud-sdk-python-hasim-3.0.937/tencentcloud_sdk_python_hasim.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:24:53.000000 tencentcloud-sdk-python-hasim-3.0.937/tencentcloud_sdk_python_hasim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-07-18 00:24:53.000000 tencentcloud-sdk-python-hasim-3.0.937/tencentcloud_sdk_python_hasim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:24:53.000000 tencentcloud-sdk-python-hasim-3.0.937/tencentcloud_sdk_python_hasim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:24:53.000000 tencentcloud-sdk-python-hasim-3.0.937/tencentcloud_sdk_python_hasim.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:12.000000 tencentcloud-sdk-python-hasim-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-19 00:40:12.000000 tencentcloud-sdk-python-hasim-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:12.000000 tencentcloud-sdk-python-hasim-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:40:12.000000 tencentcloud-sdk-python-hasim-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:12.000000 tencentcloud-sdk-python-hasim-3.0.938/tencentcloud/hasim/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:40:12.000000 tencentcloud-sdk-python-hasim-3.0.938/tencentcloud/hasim/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:12.000000 tencentcloud-sdk-python-hasim-3.0.938/tencentcloud/hasim/v20210716/
+-rw-r--r--   0 root         (0) root         (0)    19722 2023-07-19 00:40:12.000000 tencentcloud-sdk-python-hasim-3.0.938/tencentcloud/hasim/v20210716/hasim_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:40:12.000000 tencentcloud-sdk-python-hasim-3.0.938/tencentcloud/hasim/v20210716/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-07-19 00:40:12.000000 tencentcloud-sdk-python-hasim-3.0.938/tencentcloud/hasim/v20210716/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   123000 2023-07-19 00:40:12.000000 tencentcloud-sdk-python-hasim-3.0.938/tencentcloud/hasim/v20210716/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:40:12.000000 tencentcloud-sdk-python-hasim-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:40:12.000000 tencentcloud-sdk-python-hasim-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-19 00:40:12.000000 tencentcloud-sdk-python-hasim-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:12.000000 tencentcloud-sdk-python-hasim-3.0.938/tencentcloud_sdk_python_hasim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:40:12.000000 tencentcloud-sdk-python-hasim-3.0.938/tencentcloud_sdk_python_hasim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-07-19 00:40:12.000000 tencentcloud-sdk-python-hasim-3.0.938/tencentcloud_sdk_python_hasim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:40:12.000000 tencentcloud-sdk-python-hasim-3.0.938/tencentcloud_sdk_python_hasim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:40:12.000000 tencentcloud-sdk-python-hasim-3.0.938/tencentcloud_sdk_python_hasim.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-hasim-3.0.937/setup.py` & `tencentcloud-sdk-python-hasim-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hasim-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-hasim-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-hasim-3.0.937/tencentcloud/hasim/v20210716/hasim_client.py` & `tencentcloud-sdk-python-hasim-3.0.938/tencentcloud/hasim/v20210716/hasim_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTactic(self, request):
         """创建云兔切换策略
 
         :param request: Request instance for CreateTactic.
         :type request: :class:`tencentcloud.hasim.v20210716.models.CreateTacticRequest`
@@ -65,15 +65,15 @@
             model = models.CreateTacticResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTag(self, request):
         """创建标签
 
         :param request: Request instance for CreateTag.
         :type request: :class:`tencentcloud.hasim.v20210716.models.CreateTagRequest`
@@ -88,15 +88,15 @@
             model = models.CreateTagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRule(self, request):
         """删除自动化规则
 
         :param request: Request instance for DeleteRule.
         :type request: :class:`tencentcloud.hasim.v20210716.models.DeleteRuleRequest`
@@ -111,15 +111,15 @@
             model = models.DeleteRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTactic(self, request):
         """删除策略
 
         :param request: Request instance for DeleteTactic.
         :type request: :class:`tencentcloud.hasim.v20210716.models.DeleteTacticRequest`
@@ -134,15 +134,15 @@
             model = models.DeleteTacticResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTag(self, request):
         """删除标签
 
         :param request: Request instance for DeleteTag.
         :type request: :class:`tencentcloud.hasim.v20210716.models.DeleteTagRequest`
@@ -157,15 +157,15 @@
             model = models.DeleteTagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLink(self, request):
         """查询云兔连接详细信息
 
         :param request: Request instance for DescribeLink.
         :type request: :class:`tencentcloud.hasim.v20210716.models.DescribeLinkRequest`
@@ -180,15 +180,15 @@
             model = models.DescribeLinkResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLinks(self, request):
         """查询云兔连接列表
 
         :param request: Request instance for DescribeLinks.
         :type request: :class:`tencentcloud.hasim.v20210716.models.DescribeLinksRequest`
@@ -203,15 +203,15 @@
             model = models.DescribeLinksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOrders(self, request):
         """查询订单列表
 
         :param request: Request instance for DescribeOrders.
         :type request: :class:`tencentcloud.hasim.v20210716.models.DescribeOrdersRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeOrdersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRule(self, request):
         """查询自动化规则
 
         :param request: Request instance for DescribeRule.
         :type request: :class:`tencentcloud.hasim.v20210716.models.DescribeRuleRequest`
@@ -249,15 +249,15 @@
             model = models.DescribeRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRules(self, request):
         """查询自动化规则列表
 
         :param request: Request instance for DescribeRules.
         :type request: :class:`tencentcloud.hasim.v20210716.models.DescribeRulesRequest`
@@ -272,15 +272,15 @@
             model = models.DescribeRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTactic(self, request):
         """查询云兔切换策略信息
 
         :param request: Request instance for DescribeTactic.
         :type request: :class:`tencentcloud.hasim.v20210716.models.DescribeTacticRequest`
@@ -295,15 +295,15 @@
             model = models.DescribeTacticResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTactics(self, request):
         """查询云兔切换策略列表
 
         :param request: Request instance for DescribeTactics.
         :type request: :class:`tencentcloud.hasim.v20210716.models.DescribeTacticsRequest`
@@ -318,15 +318,15 @@
             model = models.DescribeTacticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTags(self, request):
         """查询标签列表
 
         :param request: Request instance for DescribeTags.
         :type request: :class:`tencentcloud.hasim.v20210716.models.DescribeTagsRequest`
@@ -341,15 +341,15 @@
             model = models.DescribeTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLinkAdvancedLog(self, request):
         """编辑云兔高级日志状态
 
         :param request: Request instance for ModifyLinkAdvancedLog.
         :type request: :class:`tencentcloud.hasim.v20210716.models.ModifyLinkAdvancedLogRequest`
@@ -364,15 +364,15 @@
             model = models.ModifyLinkAdvancedLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLinkTactic(self, request):
         """编辑云兔策略
 
         :param request: Request instance for ModifyLinkTactic.
         :type request: :class:`tencentcloud.hasim.v20210716.models.ModifyLinkTacticRequest`
@@ -387,15 +387,15 @@
             model = models.ModifyLinkTacticResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLinkTele(self, request):
         """修改云兔运营商
 
         :param request: Request instance for ModifyLinkTele.
         :type request: :class:`tencentcloud.hasim.v20210716.models.ModifyLinkTeleRequest`
@@ -410,15 +410,15 @@
             model = models.ModifyLinkTeleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRule(self, request):
         """编辑自动化规则
 
         :param request: Request instance for ModifyRule.
         :type request: :class:`tencentcloud.hasim.v20210716.models.ModifyRuleRequest`
@@ -433,15 +433,15 @@
             model = models.ModifyRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRuleStatus(self, request):
         """编辑自动化规则状态
 
         :param request: Request instance for ModifyRuleStatus.
         :type request: :class:`tencentcloud.hasim.v20210716.models.ModifyRuleStatusRequest`
@@ -456,15 +456,15 @@
             model = models.ModifyRuleStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTactic(self, request):
         """修改云兔切换策略
 
         :param request: Request instance for ModifyTactic.
         :type request: :class:`tencentcloud.hasim.v20210716.models.ModifyTacticRequest`
@@ -479,15 +479,15 @@
             model = models.ModifyTacticResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTag(self, request):
         """编辑标签
 
         :param request: Request instance for ModifyTag.
         :type request: :class:`tencentcloud.hasim.v20210716.models.ModifyTagRequest`
@@ -502,15 +502,15 @@
             model = models.ModifyTagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RenewLinkInfo(self, request):
         """刷新云兔连接信息同步
 
         :param request: Request instance for RenewLinkInfo.
         :type request: :class:`tencentcloud.hasim.v20210716.models.RenewLinkInfoRequest`
@@ -525,8 +525,8 @@
             model = models.RenewLinkInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-hasim-3.0.937/tencentcloud/hasim/v20210716/errorcodes.py` & `tencentcloud-sdk-python-hasim-3.0.938/tencentcloud/hasim/v20210716/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hasim-3.0.937/tencentcloud/hasim/v20210716/models.py` & `tencentcloud-sdk-python-hasim-3.0.938/tencentcloud/hasim/v20210716/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hasim-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-hasim-3.0.938/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-hasim
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Hasim SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-hasim-3.0.937/README.rst` & `tencentcloud-sdk-python-hasim-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hasim-3.0.937/tencentcloud_sdk_python_hasim.egg-info/PKG-INFO` & `tencentcloud-sdk-python-hasim-3.0.938/tencentcloud_sdk_python_hasim.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-hasim
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Hasim SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

