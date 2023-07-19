# Comparing `tmp/tencentcloud-sdk-python-tics-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tics-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tics-3.0.937.tar", last modified: Tue Jul 18 00:33:00 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tics-3.0.938.tar", last modified: Wed Jul 19 00:50:40 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tics-3.0.937.tar` & `tencentcloud-sdk-python-tics-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:00.000000 tencentcloud-sdk-python-tics-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:33:00.000000 tencentcloud-sdk-python-tics-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:00.000000 tencentcloud-sdk-python-tics-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:00.000000 tencentcloud-sdk-python-tics-3.0.937/tencentcloud/tics/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:33:00.000000 tencentcloud-sdk-python-tics-3.0.937/tencentcloud/tics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:00.000000 tencentcloud-sdk-python-tics-3.0.937/tencentcloud/tics/v20181115/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:33:00.000000 tencentcloud-sdk-python-tics-3.0.937/tencentcloud/tics/v20181115/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1037 2023-07-18 00:33:00.000000 tencentcloud-sdk-python-tics-3.0.937/tencentcloud/tics/v20181115/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     4901 2023-07-18 00:33:00.000000 tencentcloud-sdk-python-tics-3.0.937/tencentcloud/tics/v20181115/tics_client.py
--rw-r--r--   0 root         (0) root         (0)    28834 2023-07-18 00:33:00.000000 tencentcloud-sdk-python-tics-3.0.937/tencentcloud/tics/v20181115/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:33:00.000000 tencentcloud-sdk-python-tics-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:33:00.000000 tencentcloud-sdk-python-tics-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:33:00.000000 tencentcloud-sdk-python-tics-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:33:00.000000 tencentcloud-sdk-python-tics-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:00.000000 tencentcloud-sdk-python-tics-3.0.937/tencentcloud_sdk_python_tics.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:33:00.000000 tencentcloud-sdk-python-tics-3.0.937/tencentcloud_sdk_python_tics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:33:00.000000 tencentcloud-sdk-python-tics-3.0.937/tencentcloud_sdk_python_tics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:33:00.000000 tencentcloud-sdk-python-tics-3.0.937/tencentcloud_sdk_python_tics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:33:00.000000 tencentcloud-sdk-python-tics-3.0.937/tencentcloud_sdk_python_tics.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:40.000000 tencentcloud-sdk-python-tics-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:50:40.000000 tencentcloud-sdk-python-tics-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:40.000000 tencentcloud-sdk-python-tics-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:40.000000 tencentcloud-sdk-python-tics-3.0.938/tencentcloud/tics/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:50:40.000000 tencentcloud-sdk-python-tics-3.0.938/tencentcloud/tics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:40.000000 tencentcloud-sdk-python-tics-3.0.938/tencentcloud/tics/v20181115/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:50:40.000000 tencentcloud-sdk-python-tics-3.0.938/tencentcloud/tics/v20181115/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-07-19 00:50:40.000000 tencentcloud-sdk-python-tics-3.0.938/tencentcloud/tics/v20181115/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     4917 2023-07-19 00:50:40.000000 tencentcloud-sdk-python-tics-3.0.938/tencentcloud/tics/v20181115/tics_client.py
+-rw-r--r--   0 root         (0) root         (0)    28834 2023-07-19 00:50:40.000000 tencentcloud-sdk-python-tics-3.0.938/tencentcloud/tics/v20181115/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:50:40.000000 tencentcloud-sdk-python-tics-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:50:40.000000 tencentcloud-sdk-python-tics-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:50:40.000000 tencentcloud-sdk-python-tics-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:50:40.000000 tencentcloud-sdk-python-tics-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:40.000000 tencentcloud-sdk-python-tics-3.0.938/tencentcloud_sdk_python_tics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:50:40.000000 tencentcloud-sdk-python-tics-3.0.938/tencentcloud_sdk_python_tics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:50:40.000000 tencentcloud-sdk-python-tics-3.0.938/tencentcloud_sdk_python_tics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:50:40.000000 tencentcloud-sdk-python-tics-3.0.938/tencentcloud_sdk_python_tics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:50:40.000000 tencentcloud-sdk-python-tics-3.0.938/tencentcloud_sdk_python_tics.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tics-3.0.937/setup.py` & `tencentcloud-sdk-python-tics-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tics-3.0.937/tencentcloud/tics/v20181115/errorcodes.py` & `tencentcloud-sdk-python-tics-3.0.938/tencentcloud/tics/v20181115/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tics-3.0.937/tencentcloud/tics/v20181115/tics_client.py` & `tencentcloud-sdk-python-tics-3.0.938/tencentcloud/tics/v20181115/tics_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.DescribeDomainInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFileInfo(self, request):
         """提供文件相关的基础信息以及与攻击事件（团伙、家族）、恶意文件等相关联信息。
 
         :param request: Request instance for DescribeFileInfo.
         :type request: :class:`tencentcloud.tics.v20181115.models.DescribeFileInfoRequest`
@@ -65,15 +65,15 @@
             model = models.DescribeFileInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIpInfo(self, request):
         """提供IP相关的基础信息以及与攻击事件（团伙、家族）、恶意文件等相关联信息。
 
         :param request: Request instance for DescribeIpInfo.
         :type request: :class:`tencentcloud.tics.v20181115.models.DescribeIpInfoRequest`
@@ -88,15 +88,15 @@
             model = models.DescribeIpInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeThreatInfo(self, request):
         """提供IP和域名相关威胁情报信息查询，这些信息可以辅助检测失陷主机、帮助SIEM/SOC等系统做研判决策、帮助运营团队对设备报警的编排处理。
 
         :param request: Request instance for DescribeThreatInfo.
         :type request: :class:`tencentcloud.tics.v20181115.models.DescribeThreatInfoRequest`
@@ -111,8 +111,8 @@
             model = models.DescribeThreatInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tics-3.0.937/tencentcloud/tics/v20181115/models.py` & `tencentcloud-sdk-python-tics-3.0.938/tencentcloud/tics/v20181115/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tics-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tics-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tics-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tics-3.0.938/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tics
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tics SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tics-3.0.937/README.rst` & `tencentcloud-sdk-python-tics-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tics-3.0.937/tencentcloud_sdk_python_tics.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tics-3.0.938/tencentcloud_sdk_python_tics.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tics
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tics SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

