# Comparing `tmp/tencentcloud-sdk-python-tms-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tms-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tms-3.0.937.tar", last modified: Tue Jul 18 00:33:38 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tms-3.0.938.tar", last modified: Wed Jul 19 00:51:17 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tms-3.0.937.tar` & `tencentcloud-sdk-python-tms-3.0.938.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:38.000000 tencentcloud-sdk-python-tms-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:33:38.000000 tencentcloud-sdk-python-tms-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:38.000000 tencentcloud-sdk-python-tms-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:38.000000 tencentcloud-sdk-python-tms-3.0.937/tencentcloud/tms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:38.000000 tencentcloud-sdk-python-tms-3.0.937/tencentcloud/tms/v20200713/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:33:38.000000 tencentcloud-sdk-python-tms-3.0.937/tencentcloud/tms/v20200713/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3027 2023-07-18 00:33:38.000000 tencentcloud-sdk-python-tms-3.0.937/tencentcloud/tms/v20200713/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    40163 2023-07-18 00:33:38.000000 tencentcloud-sdk-python-tms-3.0.937/tencentcloud/tms/v20200713/models.py
--rw-r--r--   0 root         (0) root         (0)     4658 2023-07-18 00:33:38.000000 tencentcloud-sdk-python-tms-3.0.937/tencentcloud/tms/v20200713/tms_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:38.000000 tencentcloud-sdk-python-tms-3.0.937/tencentcloud/tms/v20201229/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:33:38.000000 tencentcloud-sdk-python-tms-3.0.937/tencentcloud/tms/v20201229/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1723 2023-07-18 00:33:38.000000 tencentcloud-sdk-python-tms-3.0.937/tencentcloud/tms/v20201229/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    28735 2023-07-18 00:33:38.000000 tencentcloud-sdk-python-tms-3.0.937/tencentcloud/tms/v20201229/models.py
--rw-r--r--   0 root         (0) root         (0)     3547 2023-07-18 00:33:38.000000 tencentcloud-sdk-python-tms-3.0.937/tencentcloud/tms/v20201229/tms_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:33:38.000000 tencentcloud-sdk-python-tms-3.0.937/tencentcloud/tms/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:33:38.000000 tencentcloud-sdk-python-tms-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:33:38.000000 tencentcloud-sdk-python-tms-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:33:38.000000 tencentcloud-sdk-python-tms-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:33:38.000000 tencentcloud-sdk-python-tms-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:38.000000 tencentcloud-sdk-python-tms-3.0.937/tencentcloud_sdk_python_tms.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:33:38.000000 tencentcloud-sdk-python-tms-3.0.937/tencentcloud_sdk_python_tms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-18 00:33:38.000000 tencentcloud-sdk-python-tms-3.0.937/tencentcloud_sdk_python_tms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:33:38.000000 tencentcloud-sdk-python-tms-3.0.937/tencentcloud_sdk_python_tms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:33:38.000000 tencentcloud-sdk-python-tms-3.0.937/tencentcloud_sdk_python_tms.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:17.000000 tencentcloud-sdk-python-tms-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:51:17.000000 tencentcloud-sdk-python-tms-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:17.000000 tencentcloud-sdk-python-tms-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:17.000000 tencentcloud-sdk-python-tms-3.0.938/tencentcloud/tms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:17.000000 tencentcloud-sdk-python-tms-3.0.938/tencentcloud/tms/v20200713/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:51:17.000000 tencentcloud-sdk-python-tms-3.0.938/tencentcloud/tms/v20200713/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3027 2023-07-19 00:51:17.000000 tencentcloud-sdk-python-tms-3.0.938/tencentcloud/tms/v20200713/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    40163 2023-07-19 00:51:17.000000 tencentcloud-sdk-python-tms-3.0.938/tencentcloud/tms/v20200713/models.py
+-rw-r--r--   0 root         (0) root         (0)     4674 2023-07-19 00:51:17.000000 tencentcloud-sdk-python-tms-3.0.938/tencentcloud/tms/v20200713/tms_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:17.000000 tencentcloud-sdk-python-tms-3.0.938/tencentcloud/tms/v20201229/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:51:17.000000 tencentcloud-sdk-python-tms-3.0.938/tencentcloud/tms/v20201229/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1723 2023-07-19 00:51:17.000000 tencentcloud-sdk-python-tms-3.0.938/tencentcloud/tms/v20201229/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    28735 2023-07-19 00:51:17.000000 tencentcloud-sdk-python-tms-3.0.938/tencentcloud/tms/v20201229/models.py
+-rw-r--r--   0 root         (0) root         (0)     3551 2023-07-19 00:51:17.000000 tencentcloud-sdk-python-tms-3.0.938/tencentcloud/tms/v20201229/tms_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:51:17.000000 tencentcloud-sdk-python-tms-3.0.938/tencentcloud/tms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:51:17.000000 tencentcloud-sdk-python-tms-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:51:17.000000 tencentcloud-sdk-python-tms-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:51:17.000000 tencentcloud-sdk-python-tms-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:51:17.000000 tencentcloud-sdk-python-tms-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:17.000000 tencentcloud-sdk-python-tms-3.0.938/tencentcloud_sdk_python_tms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:51:17.000000 tencentcloud-sdk-python-tms-3.0.938/tencentcloud_sdk_python_tms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-19 00:51:17.000000 tencentcloud-sdk-python-tms-3.0.938/tencentcloud_sdk_python_tms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:51:17.000000 tencentcloud-sdk-python-tms-3.0.938/tencentcloud_sdk_python_tms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:51:17.000000 tencentcloud-sdk-python-tms-3.0.938/tencentcloud_sdk_python_tms.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tms-3.0.937/setup.py` & `tencentcloud-sdk-python-tms-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tms-3.0.937/tencentcloud/tms/v20200713/errorcodes.py` & `tencentcloud-sdk-python-tms-3.0.938/tencentcloud/tms/v20200713/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tms-3.0.937/tencentcloud/tms/v20200713/models.py` & `tencentcloud-sdk-python-tms-3.0.938/tencentcloud/tms/v20200713/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tms-3.0.937/tencentcloud/tms/v20200713/tms_client.py` & `tencentcloud-sdk-python-tms-3.0.938/tencentcloud/tms/v20200713/tms_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AccountTipoffAccessResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTextLib(self, request):
         """控制台获取用户词库列表
 
         :param request: Request instance for DescribeTextLib.
         :type request: :class:`tencentcloud.tms.v20200713.models.DescribeTextLibRequest`
@@ -65,15 +65,15 @@
             model = models.DescribeTextLibResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTextStat(self, request):
         """控制台识别统计
 
         :param request: Request instance for DescribeTextStat.
         :type request: :class:`tencentcloud.tms.v20200713.models.DescribeTextStatRequest`
@@ -88,15 +88,15 @@
             model = models.DescribeTextStatResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TextModeration(self, request):
         """文本内容检测（Text Moderation）服务使用了深度学习技术，识别可能令人反感、不安全或不适宜的文本内容，同时支持用户配置词库黑白名单，打击自定义识别类型的图片。
 
         :param request: Request instance for TextModeration.
         :type request: :class:`tencentcloud.tms.v20200713.models.TextModerationRequest`
@@ -111,8 +111,8 @@
             model = models.TextModerationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tms-3.0.937/tencentcloud/tms/v20201229/errorcodes.py` & `tencentcloud-sdk-python-tms-3.0.938/tencentcloud/tms/v20201229/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tms-3.0.937/tencentcloud/tms/v20201229/models.py` & `tencentcloud-sdk-python-tms-3.0.938/tencentcloud/tms/v20201229/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tms-3.0.937/tencentcloud/tms/v20201229/tms_client.py` & `tencentcloud-sdk-python-tms-3.0.938/tencentcloud/tms/v20201229/tms_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,8 +58,8 @@
             model = models.TextModerationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tms-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tms-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tms-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tms-3.0.938/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tms
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tms-3.0.937/README.rst` & `tencentcloud-sdk-python-tms-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tms-3.0.937/tencentcloud_sdk_python_tms.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-tms-3.0.938/tencentcloud_sdk_python_tms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tms-3.0.937/tencentcloud_sdk_python_tms.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tms-3.0.938/tencentcloud_sdk_python_tms.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tms
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

