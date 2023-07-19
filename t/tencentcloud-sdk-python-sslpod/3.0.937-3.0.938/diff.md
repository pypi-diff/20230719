# Comparing `tmp/tencentcloud-sdk-python-sslpod-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-sslpod-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-sslpod-3.0.937.tar", last modified: Tue Jul 18 00:30:26 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-sslpod-3.0.938.tar", last modified: Wed Jul 19 00:45:39 2023, max compression
```

## Comparing `tencentcloud-sdk-python-sslpod-3.0.937.tar` & `tencentcloud-sdk-python-sslpod-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:26.000000 tencentcloud-sdk-python-sslpod-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-18 00:30:26.000000 tencentcloud-sdk-python-sslpod-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:26.000000 tencentcloud-sdk-python-sslpod-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:30:26.000000 tencentcloud-sdk-python-sslpod-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:26.000000 tencentcloud-sdk-python-sslpod-3.0.937/tencentcloud/sslpod/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:30:26.000000 tencentcloud-sdk-python-sslpod-3.0.937/tencentcloud/sslpod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:26.000000 tencentcloud-sdk-python-sslpod-3.0.937/tencentcloud/sslpod/v20190605/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:30:26.000000 tencentcloud-sdk-python-sslpod-3.0.937/tencentcloud/sslpod/v20190605/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2079 2023-07-18 00:30:26.000000 tencentcloud-sdk-python-sslpod-3.0.937/tencentcloud/sslpod/v20190605/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     9709 2023-07-18 00:30:26.000000 tencentcloud-sdk-python-sslpod-3.0.937/tencentcloud/sslpod/v20190605/sslpod_client.py
--rw-r--r--   0 root         (0) root         (0)    41178 2023-07-18 00:30:26.000000 tencentcloud-sdk-python-sslpod-3.0.937/tencentcloud/sslpod/v20190605/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:30:26.000000 tencentcloud-sdk-python-sslpod-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-18 00:30:26.000000 tencentcloud-sdk-python-sslpod-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-18 00:30:26.000000 tencentcloud-sdk-python-sslpod-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:26.000000 tencentcloud-sdk-python-sslpod-3.0.937/tencentcloud_sdk_python_sslpod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:30:26.000000 tencentcloud-sdk-python-sslpod-3.0.937/tencentcloud_sdk_python_sslpod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-18 00:30:26.000000 tencentcloud-sdk-python-sslpod-3.0.937/tencentcloud_sdk_python_sslpod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-18 00:30:26.000000 tencentcloud-sdk-python-sslpod-3.0.937/tencentcloud_sdk_python_sslpod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:30:26.000000 tencentcloud-sdk-python-sslpod-3.0.937/tencentcloud_sdk_python_sslpod.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:39.000000 tencentcloud-sdk-python-sslpod-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-19 00:45:39.000000 tencentcloud-sdk-python-sslpod-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:39.000000 tencentcloud-sdk-python-sslpod-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:45:39.000000 tencentcloud-sdk-python-sslpod-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:39.000000 tencentcloud-sdk-python-sslpod-3.0.938/tencentcloud/sslpod/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:45:39.000000 tencentcloud-sdk-python-sslpod-3.0.938/tencentcloud/sslpod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:39.000000 tencentcloud-sdk-python-sslpod-3.0.938/tencentcloud/sslpod/v20190605/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:45:39.000000 tencentcloud-sdk-python-sslpod-3.0.938/tencentcloud/sslpod/v20190605/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2079 2023-07-19 00:45:39.000000 tencentcloud-sdk-python-sslpod-3.0.938/tencentcloud/sslpod/v20190605/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     9749 2023-07-19 00:45:39.000000 tencentcloud-sdk-python-sslpod-3.0.938/tencentcloud/sslpod/v20190605/sslpod_client.py
+-rw-r--r--   0 root         (0) root         (0)    41178 2023-07-19 00:45:39.000000 tencentcloud-sdk-python-sslpod-3.0.938/tencentcloud/sslpod/v20190605/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:45:39.000000 tencentcloud-sdk-python-sslpod-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-19 00:45:39.000000 tencentcloud-sdk-python-sslpod-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-19 00:45:39.000000 tencentcloud-sdk-python-sslpod-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:39.000000 tencentcloud-sdk-python-sslpod-3.0.938/tencentcloud_sdk_python_sslpod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:45:39.000000 tencentcloud-sdk-python-sslpod-3.0.938/tencentcloud_sdk_python_sslpod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-19 00:45:39.000000 tencentcloud-sdk-python-sslpod-3.0.938/tencentcloud_sdk_python_sslpod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-19 00:45:39.000000 tencentcloud-sdk-python-sslpod-3.0.938/tencentcloud_sdk_python_sslpod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:45:39.000000 tencentcloud-sdk-python-sslpod-3.0.938/tencentcloud_sdk_python_sslpod.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-sslpod-3.0.937/setup.py` & `tencentcloud-sdk-python-sslpod-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sslpod-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-sslpod-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-sslpod-3.0.937/tencentcloud/sslpod/v20190605/errorcodes.py` & `tencentcloud-sdk-python-sslpod-3.0.938/tencentcloud/sslpod/v20190605/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sslpod-3.0.937/tencentcloud/sslpod/v20190605/sslpod_client.py` & `tencentcloud-sdk-python-sslpod-3.0.938/tencentcloud/sslpod/v20190605/sslpod_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDomain(self, request):
         """通过域名ID删除监控的域名
 
         :param request: Request instance for DeleteDomain.
         :type request: :class:`tencentcloud.sslpod.v20190605.models.DeleteDomainRequest`
@@ -65,15 +65,15 @@
             model = models.DeleteDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDashboard(self, request):
         """获取仪表盘数据
 
         :param request: Request instance for DescribeDashboard.
         :type request: :class:`tencentcloud.sslpod.v20190605.models.DescribeDashboardRequest`
@@ -88,15 +88,15 @@
             model = models.DescribeDashboardResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomainCerts(self, request):
         """获取域名关联证书
 
         :param request: Request instance for DescribeDomainCerts.
         :type request: :class:`tencentcloud.sslpod.v20190605.models.DescribeDomainCertsRequest`
@@ -111,15 +111,15 @@
             model = models.DescribeDomainCertsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomainTags(self, request):
         """获取账号下所有tag
 
         :param request: Request instance for DescribeDomainTags.
         :type request: :class:`tencentcloud.sslpod.v20190605.models.DescribeDomainTagsRequest`
@@ -134,15 +134,15 @@
             model = models.DescribeDomainTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomains(self, request):
         """通过searchType搜索已经添加的域名
 
         :param request: Request instance for DescribeDomains.
         :type request: :class:`tencentcloud.sslpod.v20190605.models.DescribeDomainsRequest`
@@ -157,15 +157,15 @@
             model = models.DescribeDomainsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNoticeInfo(self, request):
         """获取通知额度信息
 
         :param request: Request instance for DescribeNoticeInfo.
         :type request: :class:`tencentcloud.sslpod.v20190605.models.DescribeNoticeInfoRequest`
@@ -180,15 +180,15 @@
             model = models.DescribeNoticeInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDomainTags(self, request):
         """修改域名tag
 
         :param request: Request instance for ModifyDomainTags.
         :type request: :class:`tencentcloud.sslpod.v20190605.models.ModifyDomainTagsRequest`
@@ -203,15 +203,15 @@
             model = models.ModifyDomainTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RefreshDomain(self, request):
         """强制重新检测域名
 
         :param request: Request instance for RefreshDomain.
         :type request: :class:`tencentcloud.sslpod.v20190605.models.RefreshDomainRequest`
@@ -226,15 +226,15 @@
             model = models.RefreshDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResolveDomain(self, request):
         """解析域名获得多个IP地址
 
         :param request: Request instance for ResolveDomain.
         :type request: :class:`tencentcloud.sslpod.v20190605.models.ResolveDomainRequest`
@@ -249,8 +249,8 @@
             model = models.ResolveDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-sslpod-3.0.937/tencentcloud/sslpod/v20190605/models.py` & `tencentcloud-sdk-python-sslpod-3.0.938/tencentcloud/sslpod/v20190605/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sslpod-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-sslpod-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sslpod
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Sslpod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sslpod-3.0.937/README.rst` & `tencentcloud-sdk-python-sslpod-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sslpod-3.0.937/tencentcloud_sdk_python_sslpod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-sslpod-3.0.938/tencentcloud_sdk_python_sslpod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sslpod
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Sslpod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

