# Comparing `tmp/tencentcloud-sdk-python-autoscaling-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-autoscaling-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-autoscaling-3.0.937.tar", last modified: Tue Jul 18 00:17:23 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-autoscaling-3.0.938.tar", last modified: Wed Jul 19 00:21:25 2023, max compression
```

## Comparing `tencentcloud-sdk-python-autoscaling-3.0.937.tar` & `tencentcloud-sdk-python-autoscaling-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:23.000000 tencentcloud-sdk-python-autoscaling-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1022 2023-07-18 00:17:23.000000 tencentcloud-sdk-python-autoscaling-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:23.000000 tencentcloud-sdk-python-autoscaling-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:17:23.000000 tencentcloud-sdk-python-autoscaling-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:23.000000 tencentcloud-sdk-python-autoscaling-3.0.937/tencentcloud/autoscaling/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:23.000000 tencentcloud-sdk-python-autoscaling-3.0.937/tencentcloud/autoscaling/v20180419/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:17:23.000000 tencentcloud-sdk-python-autoscaling-3.0.937/tencentcloud/autoscaling/v20180419/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19989 2023-07-18 00:17:23.000000 tencentcloud-sdk-python-autoscaling-3.0.937/tencentcloud/autoscaling/v20180419/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    60526 2023-07-18 00:17:23.000000 tencentcloud-sdk-python-autoscaling-3.0.937/tencentcloud/autoscaling/v20180419/autoscaling_client.py
--rw-r--r--   0 root         (0) root         (0)   389762 2023-07-18 00:17:23.000000 tencentcloud-sdk-python-autoscaling-3.0.937/tencentcloud/autoscaling/v20180419/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:17:23.000000 tencentcloud-sdk-python-autoscaling-3.0.937/tencentcloud/autoscaling/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:17:23.000000 tencentcloud-sdk-python-autoscaling-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:23.000000 tencentcloud-sdk-python-autoscaling-3.0.937/tencentcloud_sdk_python_autoscaling.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:17:23.000000 tencentcloud-sdk-python-autoscaling-3.0.937/tencentcloud_sdk_python_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      525 2023-07-18 00:17:23.000000 tencentcloud-sdk-python-autoscaling-3.0.937/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1699 2023-07-18 00:17:23.000000 tencentcloud-sdk-python-autoscaling-3.0.937/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:17:23.000000 tencentcloud-sdk-python-autoscaling-3.0.937/tencentcloud_sdk_python_autoscaling.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1699 2023-07-18 00:17:23.000000 tencentcloud-sdk-python-autoscaling-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      761 2023-07-18 00:17:23.000000 tencentcloud-sdk-python-autoscaling-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:25.000000 tencentcloud-sdk-python-autoscaling-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-07-19 00:21:25.000000 tencentcloud-sdk-python-autoscaling-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:25.000000 tencentcloud-sdk-python-autoscaling-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:21:25.000000 tencentcloud-sdk-python-autoscaling-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:25.000000 tencentcloud-sdk-python-autoscaling-3.0.938/tencentcloud/autoscaling/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:25.000000 tencentcloud-sdk-python-autoscaling-3.0.938/tencentcloud/autoscaling/v20180419/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:21:25.000000 tencentcloud-sdk-python-autoscaling-3.0.938/tencentcloud/autoscaling/v20180419/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19989 2023-07-19 00:21:25.000000 tencentcloud-sdk-python-autoscaling-3.0.938/tencentcloud/autoscaling/v20180419/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    60726 2023-07-19 00:21:25.000000 tencentcloud-sdk-python-autoscaling-3.0.938/tencentcloud/autoscaling/v20180419/autoscaling_client.py
+-rw-r--r--   0 root         (0) root         (0)   392015 2023-07-19 00:21:25.000000 tencentcloud-sdk-python-autoscaling-3.0.938/tencentcloud/autoscaling/v20180419/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:21:25.000000 tencentcloud-sdk-python-autoscaling-3.0.938/tencentcloud/autoscaling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:21:25.000000 tencentcloud-sdk-python-autoscaling-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:25.000000 tencentcloud-sdk-python-autoscaling-3.0.938/tencentcloud_sdk_python_autoscaling.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:21:25.000000 tencentcloud-sdk-python-autoscaling-3.0.938/tencentcloud_sdk_python_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      525 2023-07-19 00:21:25.000000 tencentcloud-sdk-python-autoscaling-3.0.938/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-07-19 00:21:25.000000 tencentcloud-sdk-python-autoscaling-3.0.938/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:21:25.000000 tencentcloud-sdk-python-autoscaling-3.0.938/tencentcloud_sdk_python_autoscaling.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-07-19 00:21:25.000000 tencentcloud-sdk-python-autoscaling-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      761 2023-07-19 00:21:25.000000 tencentcloud-sdk-python-autoscaling-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.937/setup.py` & `tencentcloud-sdk-python-autoscaling-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-autoscaling-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.937/tencentcloud/autoscaling/v20180419/errorcodes.py` & `tencentcloud-sdk-python-autoscaling-3.0.938/tencentcloud/autoscaling/v20180419/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.937/tencentcloud/autoscaling/v20180419/autoscaling_client.py` & `tencentcloud-sdk-python-autoscaling-3.0.938/tencentcloud/autoscaling/v20180419/autoscaling_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             model = models.AttachInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AttachLoadBalancers(self, request):
         """此接口（AttachLoadBalancers）用于将负载均衡器添加到伸缩组。
 
         :param request: Request instance for AttachLoadBalancers.
         :type request: :class:`tencentcloud.autoscaling.v20180419.models.AttachLoadBalancersRequest`
@@ -67,15 +67,15 @@
             model = models.AttachLoadBalancersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ClearLaunchConfigurationAttributes(self, request):
         """本接口（ClearLaunchConfigurationAttributes）用于将启动配置内的特定属性完全清空。
 
         :param request: Request instance for ClearLaunchConfigurationAttributes.
         :type request: :class:`tencentcloud.autoscaling.v20180419.models.ClearLaunchConfigurationAttributesRequest`
@@ -90,15 +90,15 @@
             model = models.ClearLaunchConfigurationAttributesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CompleteLifecycleAction(self, request):
         """本接口（CompleteLifecycleAction）用于完成生命周期动作。
 
         * 用户通过调用本接口，指定一个具体的生命周期挂钩的结果（“CONITNUE”或者“ABANDON”）。如果一直不调用本接口，则生命周期挂钩会在超时后按照“DefaultResult”进行处理。
 
@@ -115,15 +115,15 @@
             model = models.CompleteLifecycleActionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAutoScalingGroup(self, request):
         """本接口（CreateAutoScalingGroup）用于创建伸缩组
 
         :param request: Request instance for CreateAutoScalingGroup.
         :type request: :class:`tencentcloud.autoscaling.v20180419.models.CreateAutoScalingGroupRequest`
@@ -138,15 +138,15 @@
             model = models.CreateAutoScalingGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAutoScalingGroupFromInstance(self, request):
         """本接口（CreateAutoScalingGroupFromInstance）用于根据实例创建启动配置及伸缩组。
 
         说明：根据按包年包月计费的实例所创建的伸缩组，其扩容的实例为按量计费实例。
 
@@ -163,15 +163,15 @@
             model = models.CreateAutoScalingGroupFromInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLaunchConfiguration(self, request):
         """本接口（CreateLaunchConfiguration）用于创建新的启动配置。
 
         * 启动配置，可以通过 `ModifyLaunchConfigurationAttributes` 修改少量字段。如需使用新的启动配置，建议重新创建启动配置。
 
@@ -190,15 +190,15 @@
             model = models.CreateLaunchConfigurationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLifecycleHook(self, request):
         """本接口（CreateLifecycleHook）用于创建生命周期挂钩。
 
         * 您可以为生命周期挂钩配置消息通知或执行自动化助手命令。
 
@@ -233,15 +233,15 @@
             model = models.CreateLifecycleHookResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNotificationConfiguration(self, request):
         """本接口（CreateNotificationConfiguration）用于创建通知。
         通知到 CMQ 主题或队列时，消息内容如下：
         ```
         {
@@ -283,15 +283,15 @@
             model = models.CreateNotificationConfigurationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateScalingPolicy(self, request):
         """本接口（CreateScalingPolicy）用于创建告警触发策略。
 
         :param request: Request instance for CreateScalingPolicy.
         :type request: :class:`tencentcloud.autoscaling.v20180419.models.CreateScalingPolicyRequest`
@@ -306,15 +306,15 @@
             model = models.CreateScalingPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateScheduledAction(self, request):
         """本接口（CreateScheduledAction）用于创建定时任务。
 
         :param request: Request instance for CreateScheduledAction.
         :type request: :class:`tencentcloud.autoscaling.v20180419.models.CreateScheduledActionRequest`
@@ -329,15 +329,15 @@
             model = models.CreateScheduledActionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAutoScalingGroup(self, request):
         """本接口（DeleteAutoScalingGroup）用于删除指定伸缩组，删除前提是伸缩组内无运行中（IN_SERVICE）状态的实例且当前未在执行伸缩活动。删除伸缩组后，创建失败（CREATION_FAILED）、中止失败（TERMINATION_FAILED）、解绑失败（DETACH_FAILED）等非运行中状态的实例不会被销毁。
 
         :param request: Request instance for DeleteAutoScalingGroup.
         :type request: :class:`tencentcloud.autoscaling.v20180419.models.DeleteAutoScalingGroupRequest`
@@ -352,15 +352,15 @@
             model = models.DeleteAutoScalingGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLaunchConfiguration(self, request):
         """本接口（DeleteLaunchConfiguration）用于删除启动配置。
 
         * 若启动配置在伸缩组中属于生效状态，则该启动配置不允许删除。
 
@@ -377,15 +377,15 @@
             model = models.DeleteLaunchConfigurationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLifecycleHook(self, request):
         """本接口（DeleteLifecycleHook）用于删除生命周期挂钩。
 
         :param request: Request instance for DeleteLifecycleHook.
         :type request: :class:`tencentcloud.autoscaling.v20180419.models.DeleteLifecycleHookRequest`
@@ -400,15 +400,15 @@
             model = models.DeleteLifecycleHookResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteNotificationConfiguration(self, request):
         """本接口（DeleteNotificationConfiguration）用于删除特定的通知。
 
         :param request: Request instance for DeleteNotificationConfiguration.
         :type request: :class:`tencentcloud.autoscaling.v20180419.models.DeleteNotificationConfigurationRequest`
@@ -423,15 +423,15 @@
             model = models.DeleteNotificationConfigurationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteScalingPolicy(self, request):
         """本接口（DeleteScalingPolicy）用于删除告警触发策略。
 
         :param request: Request instance for DeleteScalingPolicy.
         :type request: :class:`tencentcloud.autoscaling.v20180419.models.DeleteScalingPolicyRequest`
@@ -446,15 +446,15 @@
             model = models.DeleteScalingPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteScheduledAction(self, request):
         """本接口（DeleteScheduledAction）用于删除特定的定时任务。
 
         :param request: Request instance for DeleteScheduledAction.
         :type request: :class:`tencentcloud.autoscaling.v20180419.models.DeleteScheduledActionRequest`
@@ -469,15 +469,15 @@
             model = models.DeleteScheduledActionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccountLimits(self, request):
         """本接口（DescribeAccountLimits）用于查询用户账户在弹性伸缩中的资源限制。
 
         :param request: Request instance for DescribeAccountLimits.
         :type request: :class:`tencentcloud.autoscaling.v20180419.models.DescribeAccountLimitsRequest`
@@ -492,15 +492,15 @@
             model = models.DescribeAccountLimitsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAutoScalingActivities(self, request):
         """本接口（DescribeAutoScalingActivities）用于查询伸缩组的伸缩活动记录。
 
         :param request: Request instance for DescribeAutoScalingActivities.
         :type request: :class:`tencentcloud.autoscaling.v20180419.models.DescribeAutoScalingActivitiesRequest`
@@ -515,15 +515,15 @@
             model = models.DescribeAutoScalingActivitiesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAutoScalingAdvices(self, request):
         """此接口用于查询伸缩组配置建议。
 
         :param request: Request instance for DescribeAutoScalingAdvices.
         :type request: :class:`tencentcloud.autoscaling.v20180419.models.DescribeAutoScalingAdvicesRequest`
@@ -538,15 +538,15 @@
             model = models.DescribeAutoScalingAdvicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAutoScalingGroupLastActivities(self, request):
         """本接口（DescribeAutoScalingGroupLastActivities）用于查询伸缩组的最新一次伸缩活动记录。
 
         :param request: Request instance for DescribeAutoScalingGroupLastActivities.
         :type request: :class:`tencentcloud.autoscaling.v20180419.models.DescribeAutoScalingGroupLastActivitiesRequest`
@@ -561,15 +561,15 @@
             model = models.DescribeAutoScalingGroupLastActivitiesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAutoScalingGroups(self, request):
         """本接口（DescribeAutoScalingGroups）用于查询伸缩组信息。
 
         * 可以根据伸缩组ID、伸缩组名称或者启动配置ID等信息来查询伸缩组的详细信息。过滤信息详细请见过滤器`Filter`。
         * 如果参数为空，返回当前用户一定数量（`Limit`所指定的数量，默认为20）的伸缩组。
@@ -587,15 +587,15 @@
             model = models.DescribeAutoScalingGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAutoScalingInstances(self, request):
         """本接口（DescribeAutoScalingInstances）用于查询弹性伸缩关联实例的信息。
 
         * 可以根据实例ID、伸缩组ID等信息来查询实例的详细信息。过滤信息详细请见过滤器`Filter`。
         * 如果参数为空，返回当前用户一定数量（`Limit`所指定的数量，默认为20）的实例。
@@ -613,15 +613,15 @@
             model = models.DescribeAutoScalingInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLaunchConfigurations(self, request):
         """本接口（DescribeLaunchConfigurations）用于查询启动配置的信息。
 
         * 可以根据启动配置ID、启动配置名称等信息来查询启动配置的详细信息。过滤信息详细请见过滤器`Filter`。
         * 如果参数为空，返回当前用户一定数量（`Limit`所指定的数量，默认为20）的启动配置。
@@ -639,15 +639,15 @@
             model = models.DescribeLaunchConfigurationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLifecycleHooks(self, request):
         """本接口（DescribeLifecycleHooks）用于查询生命周期挂钩信息。
 
         * 可以根据伸缩组ID、生命周期挂钩ID或者生命周期挂钩名称等信息来查询生命周期挂钩的详细信息。过滤信息详细请见过滤器`Filter`。
         * 如果参数为空，返回当前用户一定数量（`Limit`所指定的数量，默认为20）的生命周期挂钩。
@@ -665,15 +665,15 @@
             model = models.DescribeLifecycleHooksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNotificationConfigurations(self, request):
         """本接口 (DescribeNotificationConfigurations) 用于查询一个或多个通知的详细信息。
 
         可以根据通知ID、伸缩组ID等信息来查询通知的详细信息。过滤信息详细请见过滤器`Filter`。
         如果参数为空，返回当前用户一定数量（Limit所指定的数量，默认为20）的通知。
@@ -691,15 +691,15 @@
             model = models.DescribeNotificationConfigurationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeScalingPolicies(self, request):
         """本接口（DescribeScalingPolicies）用于查询告警触发策略。
 
         :param request: Request instance for DescribeScalingPolicies.
         :type request: :class:`tencentcloud.autoscaling.v20180419.models.DescribeScalingPoliciesRequest`
@@ -714,15 +714,15 @@
             model = models.DescribeScalingPoliciesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeScheduledActions(self, request):
         """本接口 (DescribeScheduledActions) 用于查询一个或多个定时任务的详细信息。
 
         * 可以根据定时任务ID、定时任务名称或者伸缩组ID等信息来查询定时任务的详细信息。过滤信息详细请见过滤器`Filter`。
         * 如果参数为空，返回当前用户一定数量（Limit所指定的数量，默认为20）的定时任务。
@@ -740,15 +740,15 @@
             model = models.DescribeScheduledActionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetachInstances(self, request):
         """本接口（DetachInstances）用于从伸缩组移出 CVM 实例，本接口不会销毁实例。
         * 如果移出指定实例后，伸缩组内处于`IN_SERVICE`状态的实例数量小于伸缩组最小值，接口将报错
         * 如果伸缩组处于`DISABLED`状态，移出操作不校验`IN_SERVICE`实例数量和最小值的关系
         * 对于伸缩组配置的 CLB，实例在离开伸缩组时，AS 会进行解挂载动作
@@ -766,15 +766,15 @@
             model = models.DetachInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetachLoadBalancers(self, request):
         """本接口（DetachLoadBalancers）用于从伸缩组移出负载均衡器，本接口不会销毁负载均衡器。
 
         :param request: Request instance for DetachLoadBalancers.
         :type request: :class:`tencentcloud.autoscaling.v20180419.models.DetachLoadBalancersRequest`
@@ -789,15 +789,15 @@
             model = models.DetachLoadBalancersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableAutoScalingGroup(self, request):
         """本接口（DisableAutoScalingGroup）用于停用指定伸缩组。
         * 停用伸缩组后，自动触发的伸缩活动不再进行，包括：
             - 告警策略触发的伸缩活动
             - 匹配期望实例数的伸缩活动
@@ -825,15 +825,15 @@
             model = models.DisableAutoScalingGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableAutoScalingGroup(self, request):
         """本接口（EnableAutoScalingGroup）用于启用指定伸缩组。
 
         :param request: Request instance for EnableAutoScalingGroup.
         :type request: :class:`tencentcloud.autoscaling.v20180419.models.EnableAutoScalingGroupRequest`
@@ -848,15 +848,15 @@
             model = models.EnableAutoScalingGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExecuteScalingPolicy(self, request):
         """本接口（ExecuteScalingPolicy）用于执行伸缩策略。
 
         * 可以根据伸缩策略ID执行伸缩策略。
         * 伸缩策略所属伸缩组处于伸缩活动时，会拒绝执行伸缩策略。
@@ -875,15 +875,15 @@
             model = models.ExecuteScalingPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAutoScalingGroup(self, request):
         """本接口（ModifyAutoScalingGroup）用于修改伸缩组。
 
         :param request: Request instance for ModifyAutoScalingGroup.
         :type request: :class:`tencentcloud.autoscaling.v20180419.models.ModifyAutoScalingGroupRequest`
@@ -898,15 +898,15 @@
             model = models.ModifyAutoScalingGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDesiredCapacity(self, request):
         """本接口（ModifyDesiredCapacity）用于修改指定伸缩组的期望实例数
 
         :param request: Request instance for ModifyDesiredCapacity.
         :type request: :class:`tencentcloud.autoscaling.v20180419.models.ModifyDesiredCapacityRequest`
@@ -921,15 +921,15 @@
             model = models.ModifyDesiredCapacityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLaunchConfigurationAttributes(self, request):
         """本接口（ModifyLaunchConfigurationAttributes）用于修改启动配置部分属性。
 
         * 修改启动配置后，已经使用该启动配置扩容的存量实例不会发生变更，此后使用该启动配置的新增实例会按照新的配置进行扩容。
         * 本接口支持修改部分简单类型。
@@ -947,15 +947,15 @@
             model = models.ModifyLaunchConfigurationAttributesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLifecycleHook(self, request):
         """此接口用于修改生命周期挂钩。
 
         :param request: Request instance for ModifyLifecycleHook.
         :type request: :class:`tencentcloud.autoscaling.v20180419.models.ModifyLifecycleHookRequest`
@@ -970,15 +970,15 @@
             model = models.ModifyLifecycleHookResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLoadBalancerTargetAttributes(self, request):
         """本接口（ModifyLoadBalancerTargetAttributes）用于修改伸缩组内负载均衡器的目标规则属性。
 
         :param request: Request instance for ModifyLoadBalancerTargetAttributes.
         :type request: :class:`tencentcloud.autoscaling.v20180419.models.ModifyLoadBalancerTargetAttributesRequest`
@@ -993,15 +993,15 @@
             model = models.ModifyLoadBalancerTargetAttributesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLoadBalancers(self, request):
         """本接口（ModifyLoadBalancers）用于修改伸缩组的负载均衡器。
 
         * 本接口用于为伸缩组指定新的负载均衡器配置，采用`完全覆盖`风格，无论之前配置如何，`统一按照接口参数配置为新的负载均衡器`。
         * 如果要为伸缩组清空负载均衡器，则在调用本接口时仅指定伸缩组ID，不指定具体负载均衡器。
@@ -1020,15 +1020,15 @@
             model = models.ModifyLoadBalancersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyNotificationConfiguration(self, request):
         """本接口（ModifyNotificationConfiguration）用于修改通知。
         * 通知的接收端类型不支持修改。
 
         :param request: Request instance for ModifyNotificationConfiguration.
@@ -1044,15 +1044,15 @@
             model = models.ModifyNotificationConfigurationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyScalingPolicy(self, request):
         """本接口（ModifyScalingPolicy）用于修改告警触发策略。
 
         :param request: Request instance for ModifyScalingPolicy.
         :type request: :class:`tencentcloud.autoscaling.v20180419.models.ModifyScalingPolicyRequest`
@@ -1067,15 +1067,15 @@
             model = models.ModifyScalingPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyScheduledAction(self, request):
         """本接口（ModifyScheduledAction）用于修改定时任务。
 
         :param request: Request instance for ModifyScheduledAction.
         :type request: :class:`tencentcloud.autoscaling.v20180419.models.ModifyScheduledActionRequest`
@@ -1090,15 +1090,15 @@
             model = models.ModifyScheduledActionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RemoveInstances(self, request):
         """本接口（RemoveInstances）用于从伸缩组删除 CVM 实例。根据当前的产品逻辑，如果实例由弹性伸缩自动创建，则实例会被销毁；如果实例系创建后加入伸缩组的，则会从伸缩组中移除，保留实例。
         * 如果删除指定实例后，伸缩组内处于`IN_SERVICE`状态的实例数量小于伸缩组最小值，接口将报错
         * 如果伸缩组处于`DISABLED`状态，删除操作不校验`IN_SERVICE`实例数量和最小值的关系
         * 对于伸缩组配置的 CLB，实例在离开伸缩组时，AS 会进行解挂载动作
@@ -1116,15 +1116,15 @@
             model = models.RemoveInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ScaleInInstances(self, request):
         """为伸缩组指定数量缩容实例，返回缩容活动的 ActivityId。
         * 伸缩组需要未处于活动中
         * 伸缩组处于停用状态时，该接口也会生效，可参考[停用伸缩组](https://cloud.tencent.com/document/api/377/20435)文档查看伸缩组停用状态的影响范围
         * 根据伸缩组的`TerminationPolicies`策略，选择被缩容的实例，可参考[缩容处理](https://cloud.tencent.com/document/product/377/8563)
@@ -1145,15 +1145,15 @@
             model = models.ScaleInInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ScaleOutInstances(self, request):
         """为伸缩组指定数量扩容实例，返回扩容活动的 ActivityId。
         * 伸缩组需要未处于活动中
         * 伸缩组处于停用状态时，该接口也会生效，可参考[停用伸缩组](https://cloud.tencent.com/document/api/377/20435)文档查看伸缩组停用状态的影响范围
         * 接口会增加期望实例数，新的期望实例数需要小于等于最大实例数
@@ -1173,15 +1173,15 @@
             model = models.ScaleOutInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetInstancesProtection(self, request):
         """本接口（SetInstancesProtection）用于设置实例保护。
         实例设置保护之后，当发生不健康替换、报警策略、期望值变更等触发缩容时，将不对此实例缩容操作。
 
         :param request: Request instance for SetInstancesProtection.
@@ -1197,15 +1197,15 @@
             model = models.SetInstancesProtectionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartAutoScalingInstances(self, request):
         """本接口（StartAutoScalingInstances）用于开启伸缩组内 CVM 实例。
         * 开机成功，实例转为`IN_SERVICE`状态后，会增加期望实例数，期望实例数不可超过设置的最大值
         * 本接口支持批量操作，每次请求开机实例的上限为100
 
@@ -1222,15 +1222,15 @@
             model = models.StartAutoScalingInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopAutoScalingInstances(self, request):
         """本接口（StopAutoScalingInstances）用于关闭伸缩组内 CVM 实例。
         * 关机方式采用`SOFT_FIRST`方式，表示在正常关闭失败后进行强制关闭
         * 关闭`IN_SERVICE`状态的实例，会减少期望实例数，期望实例数不可低于设置的最小值
         * 使用`STOP_CHARGING`选项关机，待关机的实例需要满足[关机不收费条件](https://cloud.tencent.com/document/product/213/19918)
@@ -1249,15 +1249,15 @@
             model = models.StopAutoScalingInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeLaunchConfiguration(self, request):
         """本接口（UpgradeLaunchConfiguration）用于升级启动配置。
 
         * 本接口用于升级启动配置，采用“完全覆盖”风格，无论之前参数如何，统一按照接口参数设置为新的配置。对于非必填字段，不填写则按照默认值赋值。
         * 升级修改启动配置后，已经使用该启动配置扩容的存量实例不会发生变更，此后使用该启动配置的新增实例会按照新的配置进行扩容。
@@ -1275,15 +1275,15 @@
             model = models.UpgradeLaunchConfigurationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeLifecycleHook(self, request):
         """本接口（UpgradeLifecycleHook）用于升级生命周期挂钩。
 
         * 本接口用于升级生命周期挂钩，采用“完全覆盖”风格，无论之前参数如何，统一按照接口参数设置为新的配置。对于非必填字段，不填写则按照默认值赋值。
 
@@ -1300,8 +1300,8 @@
             model = models.UpgradeLifecycleHookResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.937/tencentcloud/autoscaling/v20180419/models.py` & `tencentcloud-sdk-python-autoscaling-3.0.938/tencentcloud/autoscaling/v20180419/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,24 +51,26 @@
         :type Description: str
         :param _StartTime: 伸缩活动开始时间。
         :type StartTime: str
         :param _EndTime: 伸缩活动结束时间。
         :type EndTime: str
         :param _CreatedTime: 伸缩活动创建时间。
         :type CreatedTime: str
-        :param _ActivityRelatedInstanceSet: 伸缩活动相关实例信息集合。
+        :param _ActivityRelatedInstanceSet: 该参数已废弃，请勿使用。
         :type ActivityRelatedInstanceSet: list of ActivtyRelatedInstance
         :param _StatusMessageSimplified: 伸缩活动状态简要描述。
         :type StatusMessageSimplified: str
         :param _LifecycleActionResultSet: 伸缩活动中生命周期挂钩的执行结果。
         :type LifecycleActionResultSet: list of LifecycleActionResultInfo
         :param _DetailedStatusMessageSet: 伸缩活动状态详细描述。
         :type DetailedStatusMessageSet: list of DetailedStatusMessage
         :param _InvocationResultSet: 执行命令结果。
         :type InvocationResultSet: list of InvocationResult
+        :param _RelatedInstanceSet: 伸缩活动相关实例信息集合。
+        :type RelatedInstanceSet: list of RelatedInstance
         """
         self._AutoScalingGroupId = None
         self._ActivityId = None
         self._ActivityType = None
         self._StatusCode = None
         self._StatusMessage = None
         self._Cause = None
@@ -77,14 +79,15 @@
         self._EndTime = None
         self._CreatedTime = None
         self._ActivityRelatedInstanceSet = None
         self._StatusMessageSimplified = None
         self._LifecycleActionResultSet = None
         self._DetailedStatusMessageSet = None
         self._InvocationResultSet = None
+        self._RelatedInstanceSet = None
 
     @property
     def AutoScalingGroupId(self):
         return self._AutoScalingGroupId
 
     @AutoScalingGroupId.setter
     def AutoScalingGroupId(self, AutoScalingGroupId):
@@ -160,18 +163,22 @@
 
     @CreatedTime.setter
     def CreatedTime(self, CreatedTime):
         self._CreatedTime = CreatedTime
 
     @property
     def ActivityRelatedInstanceSet(self):
+        warnings.warn("parameter `ActivityRelatedInstanceSet` is deprecated", DeprecationWarning) 
+
         return self._ActivityRelatedInstanceSet
 
     @ActivityRelatedInstanceSet.setter
     def ActivityRelatedInstanceSet(self, ActivityRelatedInstanceSet):
+        warnings.warn("parameter `ActivityRelatedInstanceSet` is deprecated", DeprecationWarning) 
+
         self._ActivityRelatedInstanceSet = ActivityRelatedInstanceSet
 
     @property
     def StatusMessageSimplified(self):
         return self._StatusMessageSimplified
 
     @StatusMessageSimplified.setter
@@ -198,14 +205,22 @@
     def InvocationResultSet(self):
         return self._InvocationResultSet
 
     @InvocationResultSet.setter
     def InvocationResultSet(self, InvocationResultSet):
         self._InvocationResultSet = InvocationResultSet
 
+    @property
+    def RelatedInstanceSet(self):
+        return self._RelatedInstanceSet
+
+    @RelatedInstanceSet.setter
+    def RelatedInstanceSet(self, RelatedInstanceSet):
+        self._RelatedInstanceSet = RelatedInstanceSet
+
 
     def _deserialize(self, params):
         self._AutoScalingGroupId = params.get("AutoScalingGroupId")
         self._ActivityId = params.get("ActivityId")
         self._ActivityType = params.get("ActivityType")
         self._StatusCode = params.get("StatusCode")
         self._StatusMessage = params.get("StatusMessage")
@@ -235,14 +250,20 @@
                 self._DetailedStatusMessageSet.append(obj)
         if params.get("InvocationResultSet") is not None:
             self._InvocationResultSet = []
             for item in params.get("InvocationResultSet"):
                 obj = InvocationResult()
                 obj._deserialize(item)
                 self._InvocationResultSet.append(obj)
+        if params.get("RelatedInstanceSet") is not None:
+            self._RelatedInstanceSet = []
+            for item in params.get("RelatedInstanceSet"):
+                obj = RelatedInstance()
+                obj._deserialize(item)
+                self._RelatedInstanceSet.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -8806,14 +8827,63 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class RelatedInstance(AbstractModel):
+    """与本次伸缩活动相关的实例信息。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _InstanceId: 实例ID。
+        :type InstanceId: str
+        :param _InstanceStatus: 实例在伸缩活动中的状态。取值如下：
+INIT：初始化中
+RUNNING：实例操作中
+SUCCESSFUL：活动成功
+FAILED：活动失败
+        :type InstanceStatus: str
+        """
+        self._InstanceId = None
+        self._InstanceStatus = None
+
+    @property
+    def InstanceId(self):
+        return self._InstanceId
+
+    @InstanceId.setter
+    def InstanceId(self, InstanceId):
+        self._InstanceId = InstanceId
+
+    @property
+    def InstanceStatus(self):
+        return self._InstanceStatus
+
+    @InstanceStatus.setter
+    def InstanceStatus(self, InstanceStatus):
+        self._InstanceStatus = InstanceStatus
+
+
+    def _deserialize(self, params):
+        self._InstanceId = params.get("InstanceId")
+        self._InstanceStatus = params.get("InstanceStatus")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class RemoveInstancesRequest(AbstractModel):
     """RemoveInstances请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.937/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-autoscaling-3.0.938/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.937/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO` & `tencentcloud-sdk-python-autoscaling-3.0.938/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-autoscaling
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Autoscaling SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-autoscaling-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-autoscaling
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Autoscaling SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.937/README.rst` & `tencentcloud-sdk-python-autoscaling-3.0.938/README.rst`

 * *Files identical despite different names*

