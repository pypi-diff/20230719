# Comparing `tmp/tencentcloud-sdk-python-tkgdq-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tkgdq-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tkgdq-3.0.937.tar", last modified: Tue Jul 18 00:33:33 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tkgdq-3.0.938.tar", last modified: Wed Jul 19 00:51:12 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tkgdq-3.0.937.tar` & `tencentcloud-sdk-python-tkgdq-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:33.000000 tencentcloud-sdk-python-tkgdq-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-18 00:33:33.000000 tencentcloud-sdk-python-tkgdq-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:33.000000 tencentcloud-sdk-python-tkgdq-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:33.000000 tencentcloud-sdk-python-tkgdq-3.0.937/tencentcloud/tkgdq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:33:33.000000 tencentcloud-sdk-python-tkgdq-3.0.937/tencentcloud/tkgdq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:33.000000 tencentcloud-sdk-python-tkgdq-3.0.937/tencentcloud/tkgdq/v20190411/
--rw-r--r--   0 root         (0) root         (0)     4181 2023-07-18 00:33:33.000000 tencentcloud-sdk-python-tkgdq-3.0.937/tencentcloud/tkgdq/v20190411/tkgdq_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:33:33.000000 tencentcloud-sdk-python-tkgdq-3.0.937/tencentcloud/tkgdq/v20190411/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1685 2023-07-18 00:33:33.000000 tencentcloud-sdk-python-tkgdq-3.0.937/tencentcloud/tkgdq/v20190411/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    13153 2023-07-18 00:33:33.000000 tencentcloud-sdk-python-tkgdq-3.0.937/tencentcloud/tkgdq/v20190411/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:33:33.000000 tencentcloud-sdk-python-tkgdq-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:33:33.000000 tencentcloud-sdk-python-tkgdq-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:33:33.000000 tencentcloud-sdk-python-tkgdq-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-18 00:33:33.000000 tencentcloud-sdk-python-tkgdq-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:33.000000 tencentcloud-sdk-python-tkgdq-3.0.937/tencentcloud_sdk_python_tkgdq.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:33:33.000000 tencentcloud-sdk-python-tkgdq-3.0.937/tencentcloud_sdk_python_tkgdq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-07-18 00:33:33.000000 tencentcloud-sdk-python-tkgdq-3.0.937/tencentcloud_sdk_python_tkgdq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:33:33.000000 tencentcloud-sdk-python-tkgdq-3.0.937/tencentcloud_sdk_python_tkgdq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:33:33.000000 tencentcloud-sdk-python-tkgdq-3.0.937/tencentcloud_sdk_python_tkgdq.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:12.000000 tencentcloud-sdk-python-tkgdq-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-19 00:51:12.000000 tencentcloud-sdk-python-tkgdq-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:12.000000 tencentcloud-sdk-python-tkgdq-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:12.000000 tencentcloud-sdk-python-tkgdq-3.0.938/tencentcloud/tkgdq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:51:12.000000 tencentcloud-sdk-python-tkgdq-3.0.938/tencentcloud/tkgdq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:12.000000 tencentcloud-sdk-python-tkgdq-3.0.938/tencentcloud/tkgdq/v20190411/
+-rw-r--r--   0 root         (0) root         (0)     4193 2023-07-19 00:51:12.000000 tencentcloud-sdk-python-tkgdq-3.0.938/tencentcloud/tkgdq/v20190411/tkgdq_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:51:12.000000 tencentcloud-sdk-python-tkgdq-3.0.938/tencentcloud/tkgdq/v20190411/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-07-19 00:51:12.000000 tencentcloud-sdk-python-tkgdq-3.0.938/tencentcloud/tkgdq/v20190411/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    13153 2023-07-19 00:51:12.000000 tencentcloud-sdk-python-tkgdq-3.0.938/tencentcloud/tkgdq/v20190411/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:51:12.000000 tencentcloud-sdk-python-tkgdq-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:51:12.000000 tencentcloud-sdk-python-tkgdq-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:51:12.000000 tencentcloud-sdk-python-tkgdq-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-19 00:51:12.000000 tencentcloud-sdk-python-tkgdq-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:12.000000 tencentcloud-sdk-python-tkgdq-3.0.938/tencentcloud_sdk_python_tkgdq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:51:12.000000 tencentcloud-sdk-python-tkgdq-3.0.938/tencentcloud_sdk_python_tkgdq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-07-19 00:51:12.000000 tencentcloud-sdk-python-tkgdq-3.0.938/tencentcloud_sdk_python_tkgdq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:51:12.000000 tencentcloud-sdk-python-tkgdq-3.0.938/tencentcloud_sdk_python_tkgdq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:51:12.000000 tencentcloud-sdk-python-tkgdq-3.0.938/tencentcloud_sdk_python_tkgdq.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tkgdq-3.0.937/setup.py` & `tencentcloud-sdk-python-tkgdq-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tkgdq-3.0.937/tencentcloud/tkgdq/v20190411/tkgdq_client.py` & `tencentcloud-sdk-python-tkgdq-3.0.938/tencentcloud/tkgdq/v20190411/tkgdq_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.DescribeEntityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRelation(self, request):
         """输入两个实体，返回两个实体间的关系，例如马化腾与腾讯公司不仅是相关实体，二者还存在隶属关系（马化腾属于腾讯公司）。
 
         :param request: Request instance for DescribeRelation.
         :type request: :class:`tencentcloud.tkgdq.v20190411.models.DescribeRelationRequest`
@@ -65,15 +65,15 @@
             model = models.DescribeRelationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTriple(self, request):
         """三元组查询，主要分为两类，SP查询和PO查询。SP查询表示已知主语和谓语查询宾语，PO查询表示已知宾语和谓语查询主语。每一个SP或PO查询都是一个可独立执行的查询，TQL支持SP查询的嵌套查询，即主语可以是一个嵌套的子查询。其他复杂的三元组查询方法，请参考官网API文档示例。
 
         :param request: Request instance for DescribeTriple.
         :type request: :class:`tencentcloud.tkgdq.v20190411.models.DescribeTripleRequest`
@@ -88,8 +88,8 @@
             model = models.DescribeTripleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tkgdq-3.0.937/tencentcloud/tkgdq/v20190411/errorcodes.py` & `tencentcloud-sdk-python-tkgdq-3.0.938/tencentcloud/tkgdq/v20190411/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tkgdq-3.0.937/tencentcloud/tkgdq/v20190411/models.py` & `tencentcloud-sdk-python-tkgdq-3.0.938/tencentcloud/tkgdq/v20190411/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tkgdq-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tkgdq-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tkgdq-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tkgdq-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tkgdq
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tkgdq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tkgdq-3.0.937/README.rst` & `tencentcloud-sdk-python-tkgdq-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tkgdq-3.0.937/tencentcloud_sdk_python_tkgdq.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tkgdq-3.0.938/tencentcloud_sdk_python_tkgdq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tkgdq
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tkgdq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

