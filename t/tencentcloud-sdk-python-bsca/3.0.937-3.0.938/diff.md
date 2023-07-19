# Comparing `tmp/tencentcloud-sdk-python-bsca-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-bsca-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-bsca-3.0.937.tar", last modified: Tue Jul 18 00:18:30 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-bsca-3.0.938.tar", last modified: Wed Jul 19 00:22:39 2023, max compression
```

## Comparing `tencentcloud-sdk-python-bsca-3.0.937.tar` & `tencentcloud-sdk-python-bsca-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:18:30.000000 tencentcloud-sdk-python-bsca-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:18:30.000000 tencentcloud-sdk-python-bsca-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:18:30.000000 tencentcloud-sdk-python-bsca-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:18:30.000000 tencentcloud-sdk-python-bsca-3.0.937/tencentcloud/bsca/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:18:30.000000 tencentcloud-sdk-python-bsca-3.0.937/tencentcloud/bsca/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:18:30.000000 tencentcloud-sdk-python-bsca-3.0.937/tencentcloud/bsca/v20210811/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:18:30.000000 tencentcloud-sdk-python-bsca-3.0.937/tencentcloud/bsca/v20210811/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5955 2023-07-18 00:18:30.000000 tencentcloud-sdk-python-bsca-3.0.937/tencentcloud/bsca/v20210811/bsca_client.py
--rw-r--r--   0 root         (0) root         (0)     1057 2023-07-18 00:18:30.000000 tencentcloud-sdk-python-bsca-3.0.937/tencentcloud/bsca/v20210811/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    49093 2023-07-18 00:18:30.000000 tencentcloud-sdk-python-bsca-3.0.937/tencentcloud/bsca/v20210811/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:18:30.000000 tencentcloud-sdk-python-bsca-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:18:30.000000 tencentcloud-sdk-python-bsca-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:18:30.000000 tencentcloud-sdk-python-bsca-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:18:30.000000 tencentcloud-sdk-python-bsca-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:18:30.000000 tencentcloud-sdk-python-bsca-3.0.937/tencentcloud_sdk_python_bsca.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:18:30.000000 tencentcloud-sdk-python-bsca-3.0.937/tencentcloud_sdk_python_bsca.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:18:30.000000 tencentcloud-sdk-python-bsca-3.0.937/tencentcloud_sdk_python_bsca.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:18:30.000000 tencentcloud-sdk-python-bsca-3.0.937/tencentcloud_sdk_python_bsca.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:18:30.000000 tencentcloud-sdk-python-bsca-3.0.937/tencentcloud_sdk_python_bsca.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:22:39.000000 tencentcloud-sdk-python-bsca-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:22:39.000000 tencentcloud-sdk-python-bsca-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:22:39.000000 tencentcloud-sdk-python-bsca-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:22:39.000000 tencentcloud-sdk-python-bsca-3.0.938/tencentcloud/bsca/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:22:39.000000 tencentcloud-sdk-python-bsca-3.0.938/tencentcloud/bsca/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:22:39.000000 tencentcloud-sdk-python-bsca-3.0.938/tencentcloud/bsca/v20210811/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:22:39.000000 tencentcloud-sdk-python-bsca-3.0.938/tencentcloud/bsca/v20210811/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5975 2023-07-19 00:22:39.000000 tencentcloud-sdk-python-bsca-3.0.938/tencentcloud/bsca/v20210811/bsca_client.py
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-07-19 00:22:39.000000 tencentcloud-sdk-python-bsca-3.0.938/tencentcloud/bsca/v20210811/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    49093 2023-07-19 00:22:39.000000 tencentcloud-sdk-python-bsca-3.0.938/tencentcloud/bsca/v20210811/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:22:39.000000 tencentcloud-sdk-python-bsca-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:22:39.000000 tencentcloud-sdk-python-bsca-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:22:39.000000 tencentcloud-sdk-python-bsca-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:22:39.000000 tencentcloud-sdk-python-bsca-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:22:39.000000 tencentcloud-sdk-python-bsca-3.0.938/tencentcloud_sdk_python_bsca.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:22:39.000000 tencentcloud-sdk-python-bsca-3.0.938/tencentcloud_sdk_python_bsca.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:22:39.000000 tencentcloud-sdk-python-bsca-3.0.938/tencentcloud_sdk_python_bsca.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:22:39.000000 tencentcloud-sdk-python-bsca-3.0.938/tencentcloud_sdk_python_bsca.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:22:39.000000 tencentcloud-sdk-python-bsca-3.0.938/tencentcloud_sdk_python_bsca.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-bsca-3.0.937/setup.py` & `tencentcloud-sdk-python-bsca-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bsca-3.0.937/tencentcloud/bsca/v20210811/bsca_client.py` & `tencentcloud-sdk-python-bsca-3.0.938/tencentcloud/bsca/v20210811/bsca_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.DescribeKBComponentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKBComponentVulnerability(self, request):
         """本接口(DescribeKBComponentVulnerability)用于在知识库中查询开源组件的漏洞信息。
 
         :param request: Request instance for DescribeKBComponentVulnerability.
         :type request: :class:`tencentcloud.bsca.v20210811.models.DescribeKBComponentVulnerabilityRequest`
@@ -65,15 +65,15 @@
             model = models.DescribeKBComponentVulnerabilityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKBLicense(self, request):
         """本接口(DescribeKBLicense)用于在知识库中查询许可证信息。
 
         :param request: Request instance for DescribeKBLicense.
         :type request: :class:`tencentcloud.bsca.v20210811.models.DescribeKBLicenseRequest`
@@ -88,15 +88,15 @@
             model = models.DescribeKBLicenseResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKBVulnerability(self, request):
         """本接口(DescribeKBVulnerability)用于在知识库中查询漏洞详细信息，支持根据CVE ID查询或者根据Vul ID查询。
 
         :param request: Request instance for DescribeKBVulnerability.
         :type request: :class:`tencentcloud.bsca.v20210811.models.DescribeKBVulnerabilityRequest`
@@ -111,15 +111,15 @@
             model = models.DescribeKBVulnerabilityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def MatchKBPURLList(self, request):
         """本接口(MatchKBPURLList)用于在知识库中匹配与特征对应的开源组件列表。
 
         :param request: Request instance for MatchKBPURLList.
         :type request: :class:`tencentcloud.bsca.v20210811.models.MatchKBPURLListRequest`
@@ -134,8 +134,8 @@
             model = models.MatchKBPURLListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-bsca-3.0.937/tencentcloud/bsca/v20210811/errorcodes.py` & `tencentcloud-sdk-python-bsca-3.0.938/tencentcloud/bsca/v20210811/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bsca-3.0.937/tencentcloud/bsca/v20210811/models.py` & `tencentcloud-sdk-python-bsca-3.0.938/tencentcloud/bsca/v20210811/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bsca-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-bsca-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-bsca-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-bsca-3.0.938/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bsca
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Bsca SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bsca-3.0.937/README.rst` & `tencentcloud-sdk-python-bsca-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bsca-3.0.937/tencentcloud_sdk_python_bsca.egg-info/PKG-INFO` & `tencentcloud-sdk-python-bsca-3.0.938/tencentcloud_sdk_python_bsca.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bsca
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Bsca SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

