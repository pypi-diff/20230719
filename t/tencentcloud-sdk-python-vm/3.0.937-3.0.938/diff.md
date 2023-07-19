# Comparing `tmp/tencentcloud-sdk-python-vm-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-vm-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vm-3.0.937.tar", last modified: Tue Jul 18 00:34:43 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vm-3.0.938.tar", last modified: Wed Jul 19 00:53:27 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vm-3.0.937.tar` & `tencentcloud-sdk-python-vm-3.0.938.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/tencentcloud_sdk_python_vm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/tencentcloud_sdk_python_vm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      741 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/tencentcloud_sdk_python_vm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/tencentcloud_sdk_python_vm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/tencentcloud_sdk_python_vm.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/v20200709/
--rw-r--r--   0 root         (0) root         (0)     5843 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/v20200709/vm_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/v20200709/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/v20200709/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    76744 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/v20200709/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/v20201229/
--rw-r--r--   0 root         (0) root         (0)     9098 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/v20201229/vm_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/v20201229/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1967 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/v20201229/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    95095 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/v20201229/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/v20210922/
--rw-r--r--   0 root         (0) root         (0)     5289 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/v20210922/vm_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/v20210922/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1967 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/v20210922/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    84771 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/v20210922/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-18 00:34:43.000000 tencentcloud-sdk-python-vm-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:27.000000 tencentcloud-sdk-python-vm-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-19 00:53:26.000000 tencentcloud-sdk-python-vm-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:27.000000 tencentcloud-sdk-python-vm-3.0.938/tencentcloud_sdk_python_vm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:53:27.000000 tencentcloud-sdk-python-vm-3.0.938/tencentcloud_sdk_python_vm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      741 2023-07-19 00:53:27.000000 tencentcloud-sdk-python-vm-3.0.938/tencentcloud_sdk_python_vm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:53:27.000000 tencentcloud-sdk-python-vm-3.0.938/tencentcloud_sdk_python_vm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:53:27.000000 tencentcloud-sdk-python-vm-3.0.938/tencentcloud_sdk_python_vm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:27.000000 tencentcloud-sdk-python-vm-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:53:26.000000 tencentcloud-sdk-python-vm-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:27.000000 tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:27.000000 tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/v20200709/
+-rw-r--r--   0 root         (0) root         (0)     5863 2023-07-19 00:53:26.000000 tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/v20200709/vm_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:53:26.000000 tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/v20200709/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-07-19 00:53:26.000000 tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/v20200709/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    76744 2023-07-19 00:53:26.000000 tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/v20200709/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:27.000000 tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/v20201229/
+-rw-r--r--   0 root         (0) root         (0)     9114 2023-07-19 00:53:26.000000 tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/v20201229/vm_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:53:26.000000 tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/v20201229/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-07-19 00:53:26.000000 tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/v20201229/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    95095 2023-07-19 00:53:26.000000 tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/v20201229/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:53:26.000000 tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:27.000000 tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/v20210922/
+-rw-r--r--   0 root         (0) root         (0)     5305 2023-07-19 00:53:26.000000 tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/v20210922/vm_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:53:26.000000 tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/v20210922/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-07-19 00:53:26.000000 tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/v20210922/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    84771 2023-07-19 00:53:26.000000 tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/v20210922/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:53:27.000000 tencentcloud-sdk-python-vm-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:53:27.000000 tencentcloud-sdk-python-vm-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-19 00:53:26.000000 tencentcloud-sdk-python-vm-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-vm-3.0.937/setup.py` & `tencentcloud-sdk-python-vm-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vm-3.0.937/tencentcloud_sdk_python_vm.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-vm-3.0.938/tencentcloud_sdk_python_vm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vm-3.0.937/tencentcloud_sdk_python_vm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vm-3.0.938/tencentcloud_sdk_python_vm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vm
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Vm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vm-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vm-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/v20200709/vm_client.py` & `tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/v20200709/vm_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CancelTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateBizConfig(self, request):
         """创建业务配置，1个账号最多可以创建20个配置，可定义音频审核的场景，如色情、谩骂等，
 
         在创建业务配置之前，你需要以下步骤：
         1. 开通COS存储捅功能，新建存储桶，例如 cms_segments，用来存储 视频转换过程中生成对音频和图片。
@@ -69,15 +69,15 @@
             model = models.CreateBizConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVideoModerationTask(self, request):
         """通过URL或存储桶创建审核任务
 
         :param request: Request instance for CreateVideoModerationTask.
         :type request: :class:`tencentcloud.vm.v20200709.models.CreateVideoModerationTaskRequest`
@@ -92,15 +92,15 @@
             model = models.CreateVideoModerationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskDetail(self, request):
         """查看任务详情DescribeTaskDetail
 
         :param request: Request instance for DescribeTaskDetail.
         :type request: :class:`tencentcloud.vm.v20200709.models.DescribeTaskDetailRequest`
@@ -115,15 +115,15 @@
             model = models.DescribeTaskDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVideoStat(self, request):
         """控制台识别统计
 
         :param request: Request instance for DescribeVideoStat.
         :type request: :class:`tencentcloud.vm.v20200709.models.DescribeVideoStatRequest`
@@ -138,8 +138,8 @@
             model = models.DescribeVideoStatResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/v20200709/errorcodes.py` & `tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/v20200709/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/v20200709/models.py` & `tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/v20200709/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/v20201229/vm_client.py` & `tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/v20201229/vm_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             model = models.CancelTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVideoModerationTask(self, request):
         """本接口（Video Moderation System，VM）用于提交视频文件或视频流进行智能审核任务。使用前请您使用腾讯云主账号登录控制台[开通视频内容安全服务](https://console.cloud.tencent.com/cms/video/package)并调整好对应的业务配置。<br>
         ### 功能使用说明：
 
         - 前往“[内容安全控制台-视频内容安全](https://console.cloud.tencent.com/cms/video/package)”开启使用视频内容安全服务，首次开通服务的用户可免费领用试用套餐包，包含600分钟的处理量（换算1s每帧截图，赠送**36000张图**、**600分钟的音频**处理量），有效期为1个月。
@@ -104,15 +104,15 @@
             model = models.CreateVideoModerationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskDetail(self, request):
         """通过查看任务详情 DescribeTaskDetail 接口，可主动轮询获取检测结果详情。<br>
 
         默认接口请求频率限制：**200次/秒**。
 
@@ -129,15 +129,15 @@
             model = models.DescribeTaskDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTasks(self, request):
         """通过查看审核任务列表接口，可查询任务队列；您可根据多种业务信息（业务类型、审核结果、任务状态等）筛选审核任务列表。<br>
 
         默认接口请求频率限制：**20次/秒**。
 
@@ -154,8 +154,8 @@
             model = models.DescribeTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/v20201229/errorcodes.py` & `tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/v20201229/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/v20201229/models.py` & `tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/v20201229/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/v20210922/vm_client.py` & `tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/v20210922/vm_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CancelTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVideoModerationTask(self, request):
         """通过URL或存储桶创建审核任务。
 
         ### 直播断流处理说明：
         - 请确认已对接[取消任务](https://cloud.tencent.com/document/product/1265/80018)。
@@ -72,15 +72,15 @@
             model = models.CreateVideoModerationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskDetail(self, request):
         """查看任务详情DescribeTaskDetail
 
         :param request: Request instance for DescribeTaskDetail.
         :type request: :class:`tencentcloud.vm.v20210922.models.DescribeTaskDetailRequest`
@@ -95,15 +95,15 @@
             model = models.DescribeTaskDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTasks(self, request):
         """通过查看审核任务列表接口，可查询任务队列；您可根据多种业务信息（业务类型、审核结果、任务状态等）筛选审核任务列表。<br>
 
         默认接口请求频率限制：**20次/秒**。
 
@@ -120,8 +120,8 @@
             model = models.DescribeTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/v20210922/errorcodes.py` & `tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/v20210922/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vm-3.0.937/tencentcloud/vm/v20210922/models.py` & `tencentcloud-sdk-python-vm-3.0.938/tencentcloud/vm/v20210922/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vm-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-vm-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vm
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Vm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vm-3.0.937/README.rst` & `tencentcloud-sdk-python-vm-3.0.938/README.rst`

 * *Files identical despite different names*

