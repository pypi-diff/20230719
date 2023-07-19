# Comparing `tmp/tencentcloud-sdk-python-soe-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-soe-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-soe-3.0.937.tar", last modified: Tue Jul 18 00:30:00 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-soe-3.0.938.tar", last modified: Wed Jul 19 00:45:14 2023, max compression
```

## Comparing `tencentcloud-sdk-python-soe-3.0.937.tar` & `tencentcloud-sdk-python-soe-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:00.000000 tencentcloud-sdk-python-soe-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:30:00.000000 tencentcloud-sdk-python-soe-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:00.000000 tencentcloud-sdk-python-soe-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:30:00.000000 tencentcloud-sdk-python-soe-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:00.000000 tencentcloud-sdk-python-soe-3.0.937/tencentcloud/soe/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:30:00.000000 tencentcloud-sdk-python-soe-3.0.937/tencentcloud/soe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:00.000000 tencentcloud-sdk-python-soe-3.0.937/tencentcloud/soe/v20180724/
--rw-r--r--   0 root         (0) root         (0)     5903 2023-07-18 00:30:00.000000 tencentcloud-sdk-python-soe-3.0.937/tencentcloud/soe/v20180724/soe_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:30:00.000000 tencentcloud-sdk-python-soe-3.0.937/tencentcloud/soe/v20180724/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14811 2023-07-18 00:30:00.000000 tencentcloud-sdk-python-soe-3.0.937/tencentcloud/soe/v20180724/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    67959 2023-07-18 00:30:00.000000 tencentcloud-sdk-python-soe-3.0.937/tencentcloud/soe/v20180724/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:30:00.000000 tencentcloud-sdk-python-soe-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:00.000000 tencentcloud-sdk-python-soe-3.0.937/tencentcloud_sdk_python_soe.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:30:00.000000 tencentcloud-sdk-python-soe-3.0.937/tencentcloud_sdk_python_soe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:30:00.000000 tencentcloud-sdk-python-soe-3.0.937/tencentcloud_sdk_python_soe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:30:00.000000 tencentcloud-sdk-python-soe-3.0.937/tencentcloud_sdk_python_soe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:30:00.000000 tencentcloud-sdk-python-soe-3.0.937/tencentcloud_sdk_python_soe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:30:00.000000 tencentcloud-sdk-python-soe-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:30:00.000000 tencentcloud-sdk-python-soe-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:14.000000 tencentcloud-sdk-python-soe-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:45:14.000000 tencentcloud-sdk-python-soe-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:14.000000 tencentcloud-sdk-python-soe-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:45:14.000000 tencentcloud-sdk-python-soe-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:14.000000 tencentcloud-sdk-python-soe-3.0.938/tencentcloud/soe/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:45:14.000000 tencentcloud-sdk-python-soe-3.0.938/tencentcloud/soe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:14.000000 tencentcloud-sdk-python-soe-3.0.938/tencentcloud/soe/v20180724/
+-rw-r--r--   0 root         (0) root         (0)     5919 2023-07-19 00:45:14.000000 tencentcloud-sdk-python-soe-3.0.938/tencentcloud/soe/v20180724/soe_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:45:14.000000 tencentcloud-sdk-python-soe-3.0.938/tencentcloud/soe/v20180724/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14811 2023-07-19 00:45:14.000000 tencentcloud-sdk-python-soe-3.0.938/tencentcloud/soe/v20180724/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    67959 2023-07-19 00:45:14.000000 tencentcloud-sdk-python-soe-3.0.938/tencentcloud/soe/v20180724/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:45:14.000000 tencentcloud-sdk-python-soe-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:14.000000 tencentcloud-sdk-python-soe-3.0.938/tencentcloud_sdk_python_soe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:45:14.000000 tencentcloud-sdk-python-soe-3.0.938/tencentcloud_sdk_python_soe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:45:14.000000 tencentcloud-sdk-python-soe-3.0.938/tencentcloud_sdk_python_soe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:45:14.000000 tencentcloud-sdk-python-soe-3.0.938/tencentcloud_sdk_python_soe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:45:14.000000 tencentcloud-sdk-python-soe-3.0.938/tencentcloud_sdk_python_soe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:45:14.000000 tencentcloud-sdk-python-soe-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:45:14.000000 tencentcloud-sdk-python-soe-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-soe-3.0.937/setup.py` & `tencentcloud-sdk-python-soe-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-soe-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-soe-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-soe-3.0.937/tencentcloud/soe/v20180724/soe_client.py` & `tencentcloud-sdk-python-soe-3.0.938/tencentcloud/soe/v20180724/soe_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.InitOralProcessResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def KeywordEvaluate(self, request):
         """指定主题关键词词汇评估，分析语音与关键词的切合程度，可指定多个关键词，支持中文英文同时评测。分片传输时，尽量保证纯异步调用，即不等待上一个分片的传输结果边录边传，这样可以尽可能早的提供音频数据。音频源目前仅支持16k采样率16bit单声道编码方式，如有不一致可能导致评估不准确或失败。
 
         :param request: Request instance for KeywordEvaluate.
         :type request: :class:`tencentcloud.soe.v20180724.models.KeywordEvaluateRequest`
@@ -65,15 +65,15 @@
             model = models.KeywordEvaluateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TransmitOralProcess(self, request):
         """本接口可用于中英文发音评测数据传输。在使用本接口时需要注意：传输音频数据，必须在完成发音评估初始化接口之后调用，且SessonId要与初始化接口保持一致。分片传输时，尽量保证SeqId顺序传输（请确认SeqId由1开始）。音频源目前仅支持16k采样率16bit单声道编码方式，如有不一致可能导致评估不准确或失败。
 
         :param request: Request instance for TransmitOralProcess.
         :type request: :class:`tencentcloud.soe.v20180724.models.TransmitOralProcessRequest`
@@ -88,15 +88,15 @@
             model = models.TransmitOralProcessResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TransmitOralProcessWithInit(self, request):
         """本接口可用于中英文发音评测。在使用本接口时需要注意：初始化并传输音频数据，分片传输时，尽量保证SeqId顺序传输（请确认SeqId由1开始）。音频源目前仅支持16k采样率16bit单声道编码方式，如有不一致可能导致评估不准确或失败。
 
         :param request: Request instance for TransmitOralProcessWithInit.
         :type request: :class:`tencentcloud.soe.v20180724.models.TransmitOralProcessWithInitRequest`
@@ -111,8 +111,8 @@
             model = models.TransmitOralProcessWithInitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-soe-3.0.937/tencentcloud/soe/v20180724/errorcodes.py` & `tencentcloud-sdk-python-soe-3.0.938/tencentcloud/soe/v20180724/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-soe-3.0.937/tencentcloud/soe/v20180724/models.py` & `tencentcloud-sdk-python-soe-3.0.938/tencentcloud/soe/v20180724/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-soe-3.0.937/tencentcloud_sdk_python_soe.egg-info/PKG-INFO` & `tencentcloud-sdk-python-soe-3.0.938/tencentcloud_sdk_python_soe.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-soe
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Soe SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-soe-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-soe-3.0.938/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-soe
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Soe SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-soe-3.0.937/README.rst` & `tencentcloud-sdk-python-soe-3.0.938/README.rst`

 * *Files identical despite different names*

