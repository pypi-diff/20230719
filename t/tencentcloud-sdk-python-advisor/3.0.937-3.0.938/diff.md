# Comparing `tmp/tencentcloud-sdk-python-advisor-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-advisor-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-advisor-3.0.937.tar", last modified: Tue Jul 18 00:15:48 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-advisor-3.0.938.tar", last modified: Wed Jul 19 00:20:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-advisor-3.0.937.tar` & `tencentcloud-sdk-python-advisor-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:15:48.000000 tencentcloud-sdk-python-advisor-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-18 00:15:48.000000 tencentcloud-sdk-python-advisor-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:15:48.000000 tencentcloud-sdk-python-advisor-3.0.937/tencentcloud_sdk_python_advisor.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:15:48.000000 tencentcloud-sdk-python-advisor-3.0.937/tencentcloud_sdk_python_advisor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-18 00:15:48.000000 tencentcloud-sdk-python-advisor-3.0.937/tencentcloud_sdk_python_advisor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:15:48.000000 tencentcloud-sdk-python-advisor-3.0.937/tencentcloud_sdk_python_advisor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:15:48.000000 tencentcloud-sdk-python-advisor-3.0.937/tencentcloud_sdk_python_advisor.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:15:48.000000 tencentcloud-sdk-python-advisor-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:15:48.000000 tencentcloud-sdk-python-advisor-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:15:48.000000 tencentcloud-sdk-python-advisor-3.0.937/tencentcloud/advisor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:15:48.000000 tencentcloud-sdk-python-advisor-3.0.937/tencentcloud/advisor/v20200721/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:15:48.000000 tencentcloud-sdk-python-advisor-3.0.937/tencentcloud/advisor/v20200721/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1113 2023-07-18 00:15:48.000000 tencentcloud-sdk-python-advisor-3.0.937/tencentcloud/advisor/v20200721/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    17704 2023-07-18 00:15:48.000000 tencentcloud-sdk-python-advisor-3.0.937/tencentcloud/advisor/v20200721/models.py
--rw-r--r--   0 root         (0) root         (0)     2840 2023-07-18 00:15:48.000000 tencentcloud-sdk-python-advisor-3.0.937/tencentcloud/advisor/v20200721/advisor_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:15:48.000000 tencentcloud-sdk-python-advisor-3.0.937/tencentcloud/advisor/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:15:48.000000 tencentcloud-sdk-python-advisor-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:15:48.000000 tencentcloud-sdk-python-advisor-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-18 00:15:48.000000 tencentcloud-sdk-python-advisor-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:07.000000 tencentcloud-sdk-python-advisor-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-19 00:20:07.000000 tencentcloud-sdk-python-advisor-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:07.000000 tencentcloud-sdk-python-advisor-3.0.938/tencentcloud_sdk_python_advisor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:20:07.000000 tencentcloud-sdk-python-advisor-3.0.938/tencentcloud_sdk_python_advisor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-19 00:20:07.000000 tencentcloud-sdk-python-advisor-3.0.938/tencentcloud_sdk_python_advisor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:20:07.000000 tencentcloud-sdk-python-advisor-3.0.938/tencentcloud_sdk_python_advisor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:20:07.000000 tencentcloud-sdk-python-advisor-3.0.938/tencentcloud_sdk_python_advisor.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:07.000000 tencentcloud-sdk-python-advisor-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:20:07.000000 tencentcloud-sdk-python-advisor-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:07.000000 tencentcloud-sdk-python-advisor-3.0.938/tencentcloud/advisor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:07.000000 tencentcloud-sdk-python-advisor-3.0.938/tencentcloud/advisor/v20200721/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:20:07.000000 tencentcloud-sdk-python-advisor-3.0.938/tencentcloud/advisor/v20200721/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-07-19 00:20:07.000000 tencentcloud-sdk-python-advisor-3.0.938/tencentcloud/advisor/v20200721/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    17704 2023-07-19 00:20:07.000000 tencentcloud-sdk-python-advisor-3.0.938/tencentcloud/advisor/v20200721/models.py
+-rw-r--r--   0 root         (0) root         (0)     2848 2023-07-19 00:20:07.000000 tencentcloud-sdk-python-advisor-3.0.938/tencentcloud/advisor/v20200721/advisor_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:20:07.000000 tencentcloud-sdk-python-advisor-3.0.938/tencentcloud/advisor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:20:07.000000 tencentcloud-sdk-python-advisor-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:20:07.000000 tencentcloud-sdk-python-advisor-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-19 00:20:07.000000 tencentcloud-sdk-python-advisor-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-advisor-3.0.937/setup.py` & `tencentcloud-sdk-python-advisor-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-advisor-3.0.937/tencentcloud_sdk_python_advisor.egg-info/PKG-INFO` & `tencentcloud-sdk-python-advisor-3.0.938/tencentcloud_sdk_python_advisor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-advisor
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Advisor SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-advisor-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-advisor-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-advisor-3.0.937/tencentcloud/advisor/v20200721/errorcodes.py` & `tencentcloud-sdk-python-advisor-3.0.938/tencentcloud/advisor/v20200721/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-advisor-3.0.937/tencentcloud/advisor/v20200721/models.py` & `tencentcloud-sdk-python-advisor-3.0.938/tencentcloud/advisor/v20200721/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-advisor-3.0.937/tencentcloud/advisor/v20200721/advisor_client.py` & `tencentcloud-sdk-python-advisor-3.0.938/tencentcloud/advisor/v20200721/advisor_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.DescribeStrategiesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskStrategyRisks(self, request):
         """查询评估项风险实例列表
 
         :param request: Request instance for DescribeTaskStrategyRisks.
         :type request: :class:`tencentcloud.advisor.v20200721.models.DescribeTaskStrategyRisksRequest`
@@ -65,8 +65,8 @@
             model = models.DescribeTaskStrategyRisksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-advisor-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-advisor-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-advisor
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Advisor SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-advisor-3.0.937/README.rst` & `tencentcloud-sdk-python-advisor-3.0.938/README.rst`

 * *Files identical despite different names*

