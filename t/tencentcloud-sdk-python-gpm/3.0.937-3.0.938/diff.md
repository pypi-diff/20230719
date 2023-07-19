# Comparing `tmp/tencentcloud-sdk-python-gpm-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-gpm-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-gpm-3.0.937.tar", last modified: Tue Jul 18 00:24:32 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-gpm-3.0.938.tar", last modified: Wed Jul 19 00:39:50 2023, max compression
```

## Comparing `tencentcloud-sdk-python-gpm-3.0.937.tar` & `tencentcloud-sdk-python-gpm-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:32.000000 tencentcloud-sdk-python-gpm-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:24:32.000000 tencentcloud-sdk-python-gpm-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:32.000000 tencentcloud-sdk-python-gpm-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:32.000000 tencentcloud-sdk-python-gpm-3.0.937/tencentcloud/gpm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:24:32.000000 tencentcloud-sdk-python-gpm-3.0.937/tencentcloud/gpm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:32.000000 tencentcloud-sdk-python-gpm-3.0.937/tencentcloud/gpm/v20200820/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:24:32.000000 tencentcloud-sdk-python-gpm-3.0.937/tencentcloud/gpm/v20200820/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5641 2023-07-18 00:24:32.000000 tencentcloud-sdk-python-gpm-3.0.937/tencentcloud/gpm/v20200820/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    18197 2023-07-18 00:24:32.000000 tencentcloud-sdk-python-gpm-3.0.937/tencentcloud/gpm/v20200820/gpm_client.py
--rw-r--r--   0 root         (0) root         (0)   100825 2023-07-18 00:24:32.000000 tencentcloud-sdk-python-gpm-3.0.937/tencentcloud/gpm/v20200820/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:24:32.000000 tencentcloud-sdk-python-gpm-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:24:32.000000 tencentcloud-sdk-python-gpm-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:32.000000 tencentcloud-sdk-python-gpm-3.0.937/tencentcloud_sdk_python_gpm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:24:32.000000 tencentcloud-sdk-python-gpm-3.0.937/tencentcloud_sdk_python_gpm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:24:32.000000 tencentcloud-sdk-python-gpm-3.0.937/tencentcloud_sdk_python_gpm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:24:32.000000 tencentcloud-sdk-python-gpm-3.0.937/tencentcloud_sdk_python_gpm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:24:32.000000 tencentcloud-sdk-python-gpm-3.0.937/tencentcloud_sdk_python_gpm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:24:32.000000 tencentcloud-sdk-python-gpm-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:24:32.000000 tencentcloud-sdk-python-gpm-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:50.000000 tencentcloud-sdk-python-gpm-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:39:50.000000 tencentcloud-sdk-python-gpm-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:50.000000 tencentcloud-sdk-python-gpm-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:50.000000 tencentcloud-sdk-python-gpm-3.0.938/tencentcloud/gpm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:39:50.000000 tencentcloud-sdk-python-gpm-3.0.938/tencentcloud/gpm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:50.000000 tencentcloud-sdk-python-gpm-3.0.938/tencentcloud/gpm/v20200820/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:39:50.000000 tencentcloud-sdk-python-gpm-3.0.938/tencentcloud/gpm/v20200820/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5641 2023-07-19 00:39:50.000000 tencentcloud-sdk-python-gpm-3.0.938/tencentcloud/gpm/v20200820/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    18269 2023-07-19 00:39:50.000000 tencentcloud-sdk-python-gpm-3.0.938/tencentcloud/gpm/v20200820/gpm_client.py
+-rw-r--r--   0 root         (0) root         (0)   100825 2023-07-19 00:39:50.000000 tencentcloud-sdk-python-gpm-3.0.938/tencentcloud/gpm/v20200820/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:39:50.000000 tencentcloud-sdk-python-gpm-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:39:50.000000 tencentcloud-sdk-python-gpm-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:50.000000 tencentcloud-sdk-python-gpm-3.0.938/tencentcloud_sdk_python_gpm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:39:50.000000 tencentcloud-sdk-python-gpm-3.0.938/tencentcloud_sdk_python_gpm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:39:50.000000 tencentcloud-sdk-python-gpm-3.0.938/tencentcloud_sdk_python_gpm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:39:50.000000 tencentcloud-sdk-python-gpm-3.0.938/tencentcloud_sdk_python_gpm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:39:50.000000 tencentcloud-sdk-python-gpm-3.0.938/tencentcloud_sdk_python_gpm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:39:50.000000 tencentcloud-sdk-python-gpm-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:39:50.000000 tencentcloud-sdk-python-gpm-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-gpm-3.0.937/setup.py` & `tencentcloud-sdk-python-gpm-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gpm-3.0.937/tencentcloud/gpm/v20200820/errorcodes.py` & `tencentcloud-sdk-python-gpm-3.0.938/tencentcloud/gpm/v20200820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gpm-3.0.937/tencentcloud/gpm/v20200820/gpm_client.py` & `tencentcloud-sdk-python-gpm-3.0.938/tencentcloud/gpm/v20200820/gpm_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             model = models.CancelMatchingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateMatch(self, request):
         """此接口无法使用，游戏玩家匹配GPM已于6.1正式下架，感谢您的支持
 
         创建匹配
 
@@ -69,15 +69,15 @@
             model = models.CreateMatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRule(self, request):
         """此接口无法使用，游戏玩家匹配GPM已于6.1正式下架，感谢您的支持
 
         创建规则
 
@@ -94,15 +94,15 @@
             model = models.CreateRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteMatch(self, request):
         """此接口无法使用，游戏玩家匹配GPM已于6.1正式下架，感谢您的支持
 
         删除匹配
 
@@ -119,15 +119,15 @@
             model = models.DeleteMatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRule(self, request):
         """此接口无法使用，游戏玩家匹配GPM已于6.1正式下架，感谢您的支持
 
         删除规则
 
@@ -144,15 +144,15 @@
             model = models.DeleteRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeData(self, request):
         """此接口无法使用，游戏玩家匹配GPM已于6.1正式下架，感谢您的支持
 
         统计数据
 
@@ -169,15 +169,15 @@
             model = models.DescribeDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMatch(self, request):
         """此接口无法使用，游戏玩家匹配GPM已于6.1正式下架，感谢您的支持
 
         查询匹配详情
 
@@ -194,15 +194,15 @@
             model = models.DescribeMatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMatchCodes(self, request):
         """此接口无法使用，游戏玩家匹配GPM已于6.1正式下架，感谢您的支持
 
         分页查询匹配Code
 
@@ -219,15 +219,15 @@
             model = models.DescribeMatchCodesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMatches(self, request):
         """此接口无法使用，游戏玩家匹配GPM已于6.1正式下架，感谢您的支持
 
         分页查询匹配列表
 
@@ -244,15 +244,15 @@
             model = models.DescribeMatchesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMatchingProgress(self, request):
         """此接口无法使用，游戏玩家匹配GPM已于6.1正式下架，感谢您的支持
 
         查询匹配进度。
 
@@ -269,15 +269,15 @@
             model = models.DescribeMatchingProgressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRule(self, request):
         """此接口无法使用，游戏玩家匹配GPM已于6.1正式下架，感谢您的支持
 
         查询规则详情
 
@@ -294,15 +294,15 @@
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
         """此接口无法使用，游戏玩家匹配GPM已于6.1正式下架，感谢您的支持
 
         分页查询规则集列表
 
@@ -319,15 +319,15 @@
             model = models.DescribeRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeToken(self, request):
         """此接口无法使用，游戏玩家匹配GPM已于6.1正式下架，感谢您的支持
 
         查询匹配Token，Token用于push消息验证。
 
@@ -344,15 +344,15 @@
             model = models.DescribeTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyMatch(self, request):
         """此接口无法使用，游戏玩家匹配GPM已于6.1正式下架，感谢您的支持
 
         修改匹配
 
@@ -369,15 +369,15 @@
             model = models.ModifyMatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRule(self, request):
         """此接口无法使用，游戏玩家匹配GPM已于6.1正式下架，感谢您的支持
 
         修改规则（描述、标签）
 
@@ -394,15 +394,15 @@
             model = models.ModifyRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyToken(self, request):
         """此接口无法使用，游戏玩家匹配GPM已于6.1正式下架，感谢您的支持
 
         修改匹配Token。
 
@@ -419,15 +419,15 @@
             model = models.ModifyTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartMatching(self, request):
         """此接口无法使用，游戏玩家匹配GPM已于6.1正式下架，感谢您的支持
 
         支持传入一个玩家或多个玩家发起匹配，在同一个请求内的玩家将被分到同一个对局。
 
@@ -444,15 +444,15 @@
             model = models.StartMatchingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartMatchingBackfill(self, request):
         """此接口无法使用，游戏玩家匹配GPM已于6.1正式下架，感谢您的支持
 
         通过调用StartMatchingBackfill，用户可以传入一个回填的匹配请求，GPM为回填请求搜索符合条件的ticket并形成一个新的match。
 
@@ -469,8 +469,8 @@
             model = models.StartMatchingBackfillResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-gpm-3.0.937/tencentcloud/gpm/v20200820/models.py` & `tencentcloud-sdk-python-gpm-3.0.938/tencentcloud/gpm/v20200820/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gpm-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-gpm-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-gpm-3.0.937/tencentcloud_sdk_python_gpm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-gpm-3.0.938/tencentcloud_sdk_python_gpm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gpm
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Gpm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-gpm-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-gpm-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gpm
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Gpm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-gpm-3.0.937/README.rst` & `tencentcloud-sdk-python-gpm-3.0.938/README.rst`

 * *Files identical despite different names*

