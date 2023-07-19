# Comparing `tmp/tencentcloud-sdk-python-rce-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-rce-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-rce-3.0.937.tar", last modified: Tue Jul 18 00:29:03 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-rce-3.0.938.tar", last modified: Wed Jul 19 00:44:20 2023, max compression
```

## Comparing `tencentcloud-sdk-python-rce-3.0.937.tar` & `tencentcloud-sdk-python-rce-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:03.000000 tencentcloud-sdk-python-rce-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:29:03.000000 tencentcloud-sdk-python-rce-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:03.000000 tencentcloud-sdk-python-rce-3.0.937/tencentcloud_sdk_python_rce.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:29:03.000000 tencentcloud-sdk-python-rce-3.0.937/tencentcloud_sdk_python_rce.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:29:03.000000 tencentcloud-sdk-python-rce-3.0.937/tencentcloud_sdk_python_rce.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:29:03.000000 tencentcloud-sdk-python-rce-3.0.937/tencentcloud_sdk_python_rce.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:29:03.000000 tencentcloud-sdk-python-rce-3.0.937/tencentcloud_sdk_python_rce.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:03.000000 tencentcloud-sdk-python-rce-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:29:03.000000 tencentcloud-sdk-python-rce-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:03.000000 tencentcloud-sdk-python-rce-3.0.937/tencentcloud/rce/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:29:03.000000 tencentcloud-sdk-python-rce-3.0.937/tencentcloud/rce/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:03.000000 tencentcloud-sdk-python-rce-3.0.937/tencentcloud/rce/v20201103/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:29:03.000000 tencentcloud-sdk-python-rce-3.0.937/tencentcloud/rce/v20201103/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4001 2023-07-18 00:29:03.000000 tencentcloud-sdk-python-rce-3.0.937/tencentcloud/rce/v20201103/rce_client.py
--rw-r--r--   0 root         (0) root         (0)     4151 2023-07-18 00:29:03.000000 tencentcloud-sdk-python-rce-3.0.937/tencentcloud/rce/v20201103/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    46797 2023-07-18 00:29:03.000000 tencentcloud-sdk-python-rce-3.0.937/tencentcloud/rce/v20201103/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:29:03.000000 tencentcloud-sdk-python-rce-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:29:03.000000 tencentcloud-sdk-python-rce-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:29:03.000000 tencentcloud-sdk-python-rce-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:20.000000 tencentcloud-sdk-python-rce-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:44:20.000000 tencentcloud-sdk-python-rce-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:20.000000 tencentcloud-sdk-python-rce-3.0.938/tencentcloud_sdk_python_rce.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:44:20.000000 tencentcloud-sdk-python-rce-3.0.938/tencentcloud_sdk_python_rce.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:44:20.000000 tencentcloud-sdk-python-rce-3.0.938/tencentcloud_sdk_python_rce.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:44:20.000000 tencentcloud-sdk-python-rce-3.0.938/tencentcloud_sdk_python_rce.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:44:20.000000 tencentcloud-sdk-python-rce-3.0.938/tencentcloud_sdk_python_rce.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:20.000000 tencentcloud-sdk-python-rce-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:44:20.000000 tencentcloud-sdk-python-rce-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:20.000000 tencentcloud-sdk-python-rce-3.0.938/tencentcloud/rce/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:44:20.000000 tencentcloud-sdk-python-rce-3.0.938/tencentcloud/rce/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:20.000000 tencentcloud-sdk-python-rce-3.0.938/tencentcloud/rce/v20201103/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:44:20.000000 tencentcloud-sdk-python-rce-3.0.938/tencentcloud/rce/v20201103/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4013 2023-07-19 00:44:20.000000 tencentcloud-sdk-python-rce-3.0.938/tencentcloud/rce/v20201103/rce_client.py
+-rw-r--r--   0 root         (0) root         (0)     4151 2023-07-19 00:44:20.000000 tencentcloud-sdk-python-rce-3.0.938/tencentcloud/rce/v20201103/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    46797 2023-07-19 00:44:20.000000 tencentcloud-sdk-python-rce-3.0.938/tencentcloud/rce/v20201103/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:44:20.000000 tencentcloud-sdk-python-rce-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:44:20.000000 tencentcloud-sdk-python-rce-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:44:20.000000 tencentcloud-sdk-python-rce-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-rce-3.0.937/setup.py` & `tencentcloud-sdk-python-rce-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-rce-3.0.937/tencentcloud_sdk_python_rce.egg-info/PKG-INFO` & `tencentcloud-sdk-python-rce-3.0.938/tencentcloud_sdk_python_rce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-rce
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Rce SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-rce-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-rce-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-rce-3.0.937/tencentcloud/rce/v20201103/rce_client.py` & `tencentcloud-sdk-python-rce-3.0.938/tencentcloud/rce/v20201103/rce_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.DescribeRiskAssessmentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRiskTrends(self, request):
         """以图表形式展示三种请求状态的趋势变化
 
         :param request: Request instance for DescribeRiskTrends.
         :type request: :class:`tencentcloud.rce.v20201103.models.DescribeRiskTrendsRequest`
@@ -65,15 +65,15 @@
             model = models.DescribeRiskTrendsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ManageMarketingRisk(self, request):
         """全栈式风控引擎（RiskControlEngine，RCE）是基于人工智能技术和腾讯20年风控实战沉淀，依托腾讯海量业务构建的风控引擎，以轻量级的 SaaS 服务方式接入，帮助您快速解决注册、登录、营销活动等关键场景遇到的欺诈问题，实时防御黑灰产作恶。
 
         :param request: Request instance for ManageMarketingRisk.
         :type request: :class:`tencentcloud.rce.v20201103.models.ManageMarketingRiskRequest`
@@ -88,8 +88,8 @@
             model = models.ManageMarketingRiskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-rce-3.0.937/tencentcloud/rce/v20201103/errorcodes.py` & `tencentcloud-sdk-python-rce-3.0.938/tencentcloud/rce/v20201103/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-rce-3.0.937/tencentcloud/rce/v20201103/models.py` & `tencentcloud-sdk-python-rce-3.0.938/tencentcloud/rce/v20201103/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-rce-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-rce-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-rce
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Rce SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-rce-3.0.937/README.rst` & `tencentcloud-sdk-python-rce-3.0.938/README.rst`

 * *Files identical despite different names*

