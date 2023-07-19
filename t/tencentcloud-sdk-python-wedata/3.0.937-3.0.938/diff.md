# Comparing `tmp/tencentcloud-sdk-python-wedata-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-wedata-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-wedata-3.0.937.tar", last modified: Tue Jul 18 00:35:35 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-wedata-3.0.938.tar", last modified: Wed Jul 19 00:54:05 2023, max compression
```

## Comparing `tencentcloud-sdk-python-wedata-3.0.937.tar` & `tencentcloud-sdk-python-wedata-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:35.000000 tencentcloud-sdk-python-wedata-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-18 00:35:35.000000 tencentcloud-sdk-python-wedata-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:35.000000 tencentcloud-sdk-python-wedata-3.0.937/tencentcloud_sdk_python_wedata.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:35:35.000000 tencentcloud-sdk-python-wedata-3.0.937/tencentcloud_sdk_python_wedata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-18 00:35:35.000000 tencentcloud-sdk-python-wedata-3.0.937/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-18 00:35:35.000000 tencentcloud-sdk-python-wedata-3.0.937/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:35:35.000000 tencentcloud-sdk-python-wedata-3.0.937/tencentcloud_sdk_python_wedata.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:35.000000 tencentcloud-sdk-python-wedata-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:35:35.000000 tencentcloud-sdk-python-wedata-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:35.000000 tencentcloud-sdk-python-wedata-3.0.937/tencentcloud/wedata/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:35:35.000000 tencentcloud-sdk-python-wedata-3.0.937/tencentcloud/wedata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:35.000000 tencentcloud-sdk-python-wedata-3.0.937/tencentcloud/wedata/v20210820/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:35:35.000000 tencentcloud-sdk-python-wedata-3.0.937/tencentcloud/wedata/v20210820/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3451 2023-07-18 00:35:35.000000 tencentcloud-sdk-python-wedata-3.0.937/tencentcloud/wedata/v20210820/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1253549 2023-07-18 00:35:35.000000 tencentcloud-sdk-python-wedata-3.0.937/tencentcloud/wedata/v20210820/models.py
--rw-r--r--   0 root         (0) root         (0)   187884 2023-07-18 00:35:35.000000 tencentcloud-sdk-python-wedata-3.0.937/tencentcloud/wedata/v20210820/wedata_client.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:35:35.000000 tencentcloud-sdk-python-wedata-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-18 00:35:35.000000 tencentcloud-sdk-python-wedata-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-18 00:35:35.000000 tencentcloud-sdk-python-wedata-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:54:05.000000 tencentcloud-sdk-python-wedata-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-19 00:54:05.000000 tencentcloud-sdk-python-wedata-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:54:05.000000 tencentcloud-sdk-python-wedata-3.0.938/tencentcloud_sdk_python_wedata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:54:05.000000 tencentcloud-sdk-python-wedata-3.0.938/tencentcloud_sdk_python_wedata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-19 00:54:05.000000 tencentcloud-sdk-python-wedata-3.0.938/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-19 00:54:05.000000 tencentcloud-sdk-python-wedata-3.0.938/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:54:05.000000 tencentcloud-sdk-python-wedata-3.0.938/tencentcloud_sdk_python_wedata.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:54:05.000000 tencentcloud-sdk-python-wedata-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:54:05.000000 tencentcloud-sdk-python-wedata-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:54:05.000000 tencentcloud-sdk-python-wedata-3.0.938/tencentcloud/wedata/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:54:05.000000 tencentcloud-sdk-python-wedata-3.0.938/tencentcloud/wedata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:54:05.000000 tencentcloud-sdk-python-wedata-3.0.938/tencentcloud/wedata/v20210820/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:54:05.000000 tencentcloud-sdk-python-wedata-3.0.938/tencentcloud/wedata/v20210820/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3640 2023-07-19 00:54:05.000000 tencentcloud-sdk-python-wedata-3.0.938/tencentcloud/wedata/v20210820/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1302444 2023-07-19 00:54:05.000000 tencentcloud-sdk-python-wedata-3.0.938/tencentcloud/wedata/v20210820/models.py
+-rw-r--r--   0 root         (0) root         (0)   195732 2023-07-19 00:54:05.000000 tencentcloud-sdk-python-wedata-3.0.938/tencentcloud/wedata/v20210820/wedata_client.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:54:05.000000 tencentcloud-sdk-python-wedata-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-19 00:54:05.000000 tencentcloud-sdk-python-wedata-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-19 00:54:05.000000 tencentcloud-sdk-python-wedata-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.937/setup.py` & `tencentcloud-sdk-python-wedata-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wedata-3.0.937/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO` & `tencentcloud-sdk-python-wedata-3.0.938/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wedata
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Wedata SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-wedata-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-wedata-3.0.937/tencentcloud/wedata/v20210820/errorcodes.py` & `tencentcloud-sdk-python-wedata-3.0.938/tencentcloud/wedata/v20210820/errorcodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,17 @@
 
 # 规则模版不存在。
 INVALIDPARAMETER_RULETEMPLATENOTEXIST = 'InvalidParameter.RuleTemplateNotExist'
 
 # 服务繁忙，请稍后重试。
 INVALIDPARAMETER_SERVICEISBUSY = 'InvalidParameter.ServiceIsBusy'
 
+# WeData_QCSRole不存在，请进行服务授权。
+INVALIDPARAMETER_WEDATAROLENOTEXISTS = 'InvalidParameter.WeDataRoleNotExists'
+
 # 工作空间不存在。
 INVALIDPARAMETER_WORKSPACENOTEXIST = 'InvalidParameter.WorkspaceNotExist'
 
 # 参数取值错误。
 INVALIDPARAMETERVALUE = 'InvalidParameterValue'
 
 # 超过配额限制。
@@ -91,14 +94,17 @@
 
 # 资源不存在。
 RESOURCENOTFOUND = 'ResourceNotFound'
 
 # 资源不可用。
 RESOURCEUNAVAILABLE = 'ResourceUnavailable'
 
+# 资源售罄。
+RESOURCESSOLDOUT = 'ResourcesSoldOut'
+
 # 未授权操作。
 UNAUTHORIZEDOPERATION = 'UnauthorizedOperation'
 
 # 用户不是当前项目成员。
 UNAUTHORIZEDOPERATION_USERNOTINPROJECT = 'UnauthorizedOperation.UserNotInProject'
 
 # 未知参数错误。
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.937/tencentcloud/wedata/v20210820/models.py` & `tencentcloud-sdk-python-wedata-3.0.938/tencentcloud/wedata/v20210820/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,195 @@
 # limitations under the License.
 
 import warnings
 
 from tencentcloud.common.abstract_model import AbstractModel
 
 
+class AdhocDetail(AbstractModel):
+    """子任务记录
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Id: 子任务记录Id
+        :type Id: int
+        :param _ScriptContent: 脚本内容
+        :type ScriptContent: str
+        :param _StartTime: 任务启动时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StartTime: str
+        :param _EndTime: 任务结束时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EndTime: str
+        :param _Status: 当前任务状态
+        :type Status: str
+        :param _RecordId: 提交任务id
+        :type RecordId: int
+        """
+        self._Id = None
+        self._ScriptContent = None
+        self._StartTime = None
+        self._EndTime = None
+        self._Status = None
+        self._RecordId = None
+
+    @property
+    def Id(self):
+        return self._Id
+
+    @Id.setter
+    def Id(self, Id):
+        self._Id = Id
+
+    @property
+    def ScriptContent(self):
+        return self._ScriptContent
+
+    @ScriptContent.setter
+    def ScriptContent(self, ScriptContent):
+        self._ScriptContent = ScriptContent
+
+    @property
+    def StartTime(self):
+        return self._StartTime
+
+    @StartTime.setter
+    def StartTime(self, StartTime):
+        self._StartTime = StartTime
+
+    @property
+    def EndTime(self):
+        return self._EndTime
+
+    @EndTime.setter
+    def EndTime(self, EndTime):
+        self._EndTime = EndTime
+
+    @property
+    def Status(self):
+        return self._Status
+
+    @Status.setter
+    def Status(self, Status):
+        self._Status = Status
+
+    @property
+    def RecordId(self):
+        return self._RecordId
+
+    @RecordId.setter
+    def RecordId(self, RecordId):
+        self._RecordId = RecordId
+
+
+    def _deserialize(self, params):
+        self._Id = params.get("Id")
+        self._ScriptContent = params.get("ScriptContent")
+        self._StartTime = params.get("StartTime")
+        self._EndTime = params.get("EndTime")
+        self._Status = params.get("Status")
+        self._RecordId = params.get("RecordId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class AdhocRecord(AbstractModel):
+    """任务提交记录
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Id: 任务提交记录id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Id: int
+        :param _ScriptContent: 脚本内容
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ScriptContent: str
+        :param _CreateTime: 任务提交时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateTime: str
+        :param _Status: 任务状态
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Status: str
+        :param _InstanceId: 实例id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceId: str
+        """
+        self._Id = None
+        self._ScriptContent = None
+        self._CreateTime = None
+        self._Status = None
+        self._InstanceId = None
+
+    @property
+    def Id(self):
+        return self._Id
+
+    @Id.setter
+    def Id(self, Id):
+        self._Id = Id
+
+    @property
+    def ScriptContent(self):
+        return self._ScriptContent
+
+    @ScriptContent.setter
+    def ScriptContent(self, ScriptContent):
+        self._ScriptContent = ScriptContent
+
+    @property
+    def CreateTime(self):
+        return self._CreateTime
+
+    @CreateTime.setter
+    def CreateTime(self, CreateTime):
+        self._CreateTime = CreateTime
+
+    @property
+    def Status(self):
+        return self._Status
+
+    @Status.setter
+    def Status(self, Status):
+        self._Status = Status
+
+    @property
+    def InstanceId(self):
+        return self._InstanceId
+
+    @InstanceId.setter
+    def InstanceId(self, InstanceId):
+        self._InstanceId = InstanceId
+
+
+    def _deserialize(self, params):
+        self._Id = params.get("Id")
+        self._ScriptContent = params.get("ScriptContent")
+        self._CreateTime = params.get("CreateTime")
+        self._Status = params.get("Status")
+        self._InstanceId = params.get("InstanceId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class AlarmEventInfo(AbstractModel):
     """告警事件详情
 
     """
 
     def __init__(self):
         r"""
@@ -923,14 +1104,137 @@
     def _deserialize(self, params):
         self._SuccessCount = params.get("SuccessCount")
         self._FailedCount = params.get("FailedCount")
         self._TotalCount = params.get("TotalCount")
         self._RequestId = params.get("RequestId")
 
 
+class BatchDeleteTasksDsRequest(AbstractModel):
+    """BatchDeleteTasksDs请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TaskIdList: 批量删除的任务TaskId
+        :type TaskIdList: list of str
+        :param _DeleteMode: true : 删除后下游任务可正常运行
+false：删除后下游任务不可运行
+        :type DeleteMode: bool
+        :param _OperateInform: true：通知下游任务责任人
+false:  不通知下游任务责任人
+        :type OperateInform: bool
+        :param _ProjectId: 项目Id
+        :type ProjectId: str
+        :param _DeleteScript: true: 删除任务引用的脚本
+false: 不删除任务引用的脚本
+        :type DeleteScript: bool
+        """
+        self._TaskIdList = None
+        self._DeleteMode = None
+        self._OperateInform = None
+        self._ProjectId = None
+        self._DeleteScript = None
+
+    @property
+    def TaskIdList(self):
+        return self._TaskIdList
+
+    @TaskIdList.setter
+    def TaskIdList(self, TaskIdList):
+        self._TaskIdList = TaskIdList
+
+    @property
+    def DeleteMode(self):
+        return self._DeleteMode
+
+    @DeleteMode.setter
+    def DeleteMode(self, DeleteMode):
+        self._DeleteMode = DeleteMode
+
+    @property
+    def OperateInform(self):
+        return self._OperateInform
+
+    @OperateInform.setter
+    def OperateInform(self, OperateInform):
+        self._OperateInform = OperateInform
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def DeleteScript(self):
+        return self._DeleteScript
+
+    @DeleteScript.setter
+    def DeleteScript(self, DeleteScript):
+        self._DeleteScript = DeleteScript
+
+
+    def _deserialize(self, params):
+        self._TaskIdList = params.get("TaskIdList")
+        self._DeleteMode = params.get("DeleteMode")
+        self._OperateInform = params.get("OperateInform")
+        self._ProjectId = params.get("ProjectId")
+        self._DeleteScript = params.get("DeleteScript")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class BatchDeleteTasksDsResponse(AbstractModel):
+    """BatchDeleteTasksDs返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 返回批量操作成功个数、失败个数、操作总数
+        :type Data: :class:`tencentcloud.wedata.v20210820.models.BatchOperateResult`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = BatchOperateResult()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
+
+
 class BatchDeleteTasksNewRequest(AbstractModel):
     """BatchDeleteTasksNew请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -8041,14 +8345,126 @@
 
 
     def _deserialize(self, params):
         self._Data = params.get("Data")
         self._RequestId = params.get("RequestId")
 
 
+class DeleteFilePathRequest(AbstractModel):
+    """DeleteFilePath请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ProjectId: 项目ID
+        :type ProjectId: str
+        :param _ResourceIds: 资源ID
+        :type ResourceIds: list of str
+        :param _UseStatus: 使用状态
+        :type UseStatus: str
+        :param _FilePaths: 文件路径
+        :type FilePaths: list of str
+        """
+        self._ProjectId = None
+        self._ResourceIds = None
+        self._UseStatus = None
+        self._FilePaths = None
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def ResourceIds(self):
+        return self._ResourceIds
+
+    @ResourceIds.setter
+    def ResourceIds(self, ResourceIds):
+        self._ResourceIds = ResourceIds
+
+    @property
+    def UseStatus(self):
+        return self._UseStatus
+
+    @UseStatus.setter
+    def UseStatus(self, UseStatus):
+        self._UseStatus = UseStatus
+
+    @property
+    def FilePaths(self):
+        return self._FilePaths
+
+    @FilePaths.setter
+    def FilePaths(self, FilePaths):
+        self._FilePaths = FilePaths
+
+
+    def _deserialize(self, params):
+        self._ProjectId = params.get("ProjectId")
+        self._ResourceIds = params.get("ResourceIds")
+        self._UseStatus = params.get("UseStatus")
+        self._FilePaths = params.get("FilePaths")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteFilePathResponse(AbstractModel):
+    """DeleteFilePath返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _UserFileList: 文件列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserFileList: list of UserFileInfo
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._UserFileList = None
+        self._RequestId = None
+
+    @property
+    def UserFileList(self):
+        return self._UserFileList
+
+    @UserFileList.setter
+    def UserFileList(self, UserFileList):
+        self._UserFileList = UserFileList
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("UserFileList") is not None:
+            self._UserFileList = []
+            for item in params.get("UserFileList"):
+                obj = UserFileInfo()
+                obj._deserialize(item)
+                self._UserFileList.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
 class DeleteFolderRequest(AbstractModel):
     """DeleteFolder请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -8463,14 +8879,202 @@
 
 
     def _deserialize(self, params):
         self._Data = params.get("Data")
         self._RequestId = params.get("RequestId")
 
 
+class DeleteProjectParamDsRequest(AbstractModel):
+    """DeleteProjectParamDs请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ParamKey: 参数名
+        :type ParamKey: str
+        :param _ProjectId: 项目id
+        :type ProjectId: str
+        """
+        self._ParamKey = None
+        self._ProjectId = None
+
+    @property
+    def ParamKey(self):
+        return self._ParamKey
+
+    @ParamKey.setter
+    def ParamKey(self, ParamKey):
+        self._ParamKey = ParamKey
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+
+    def _deserialize(self, params):
+        self._ParamKey = params.get("ParamKey")
+        self._ProjectId = params.get("ProjectId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteProjectParamDsResponse(AbstractModel):
+    """DeleteProjectParamDs返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 结果
+        :type Data: bool
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._Data = params.get("Data")
+        self._RequestId = params.get("RequestId")
+
+
+class DeleteResourceFilesRequest(AbstractModel):
+    """DeleteResourceFiles请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ProjectId: 项目id
+        :type ProjectId: str
+        :param _UseStatus: 使用状态
+        :type UseStatus: bool
+        :param _ResourceIds: 资源id列表
+        :type ResourceIds: list of str
+        :param _FilePaths: 资源路径列表
+        :type FilePaths: list of str
+        """
+        self._ProjectId = None
+        self._UseStatus = None
+        self._ResourceIds = None
+        self._FilePaths = None
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def UseStatus(self):
+        return self._UseStatus
+
+    @UseStatus.setter
+    def UseStatus(self, UseStatus):
+        self._UseStatus = UseStatus
+
+    @property
+    def ResourceIds(self):
+        return self._ResourceIds
+
+    @ResourceIds.setter
+    def ResourceIds(self, ResourceIds):
+        self._ResourceIds = ResourceIds
+
+    @property
+    def FilePaths(self):
+        return self._FilePaths
+
+    @FilePaths.setter
+    def FilePaths(self, FilePaths):
+        self._FilePaths = FilePaths
+
+
+    def _deserialize(self, params):
+        self._ProjectId = params.get("ProjectId")
+        self._UseStatus = params.get("UseStatus")
+        self._ResourceIds = params.get("ResourceIds")
+        self._FilePaths = params.get("FilePaths")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteResourceFilesResponse(AbstractModel):
+    """DeleteResourceFiles返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 资源批量删除结果
+        :type Data: bool
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._Data = params.get("Data")
+        self._RequestId = params.get("RequestId")
+
+
 class DeleteResourceRequest(AbstractModel):
     """DeleteResource请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -8819,14 +9423,157 @@
 
 
     def _deserialize(self, params):
         self._Data = params.get("Data")
         self._RequestId = params.get("RequestId")
 
 
+class DeleteTaskDsRequest(AbstractModel):
+    """DeleteTaskDs请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ProjectId: 项目Id
+        :type ProjectId: str
+        :param _DeleteScript: 是否删除脚本
+        :type DeleteScript: bool
+        :param _OperateInform: 任务操作是否消息通知下游任务责任人
+        :type OperateInform: bool
+        :param _TaskId: 任务ID
+        :type TaskId: str
+        :param _VirtualTaskId: 虚拟任务id
+        :type VirtualTaskId: str
+        :param _VirtualFlag: 虚拟任务标记
+        :type VirtualFlag: bool
+        :param _DeleteMode: 任务删除方式
+        :type DeleteMode: bool
+        """
+        self._ProjectId = None
+        self._DeleteScript = None
+        self._OperateInform = None
+        self._TaskId = None
+        self._VirtualTaskId = None
+        self._VirtualFlag = None
+        self._DeleteMode = None
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def DeleteScript(self):
+        return self._DeleteScript
+
+    @DeleteScript.setter
+    def DeleteScript(self, DeleteScript):
+        self._DeleteScript = DeleteScript
+
+    @property
+    def OperateInform(self):
+        return self._OperateInform
+
+    @OperateInform.setter
+    def OperateInform(self, OperateInform):
+        self._OperateInform = OperateInform
+
+    @property
+    def TaskId(self):
+        return self._TaskId
+
+    @TaskId.setter
+    def TaskId(self, TaskId):
+        self._TaskId = TaskId
+
+    @property
+    def VirtualTaskId(self):
+        return self._VirtualTaskId
+
+    @VirtualTaskId.setter
+    def VirtualTaskId(self, VirtualTaskId):
+        self._VirtualTaskId = VirtualTaskId
+
+    @property
+    def VirtualFlag(self):
+        return self._VirtualFlag
+
+    @VirtualFlag.setter
+    def VirtualFlag(self, VirtualFlag):
+        self._VirtualFlag = VirtualFlag
+
+    @property
+    def DeleteMode(self):
+        return self._DeleteMode
+
+    @DeleteMode.setter
+    def DeleteMode(self, DeleteMode):
+        self._DeleteMode = DeleteMode
+
+
+    def _deserialize(self, params):
+        self._ProjectId = params.get("ProjectId")
+        self._DeleteScript = params.get("DeleteScript")
+        self._OperateInform = params.get("OperateInform")
+        self._TaskId = params.get("TaskId")
+        self._VirtualTaskId = params.get("VirtualTaskId")
+        self._VirtualFlag = params.get("VirtualFlag")
+        self._DeleteMode = params.get("DeleteMode")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteTaskDsResponse(AbstractModel):
+    """DeleteTaskDs返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 无
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Data: bool
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._Data = params.get("Data")
+        self._RequestId = params.get("RequestId")
+
+
 class DeleteWorkflowNewRequest(AbstractModel):
     """DeleteWorkflowNew请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -32265,14 +33012,96 @@
     def _deserialize(self, params):
         if params.get("Data") is not None:
             self._Data = BatchReturn()
             self._Data._deserialize(params.get("Data"))
         self._RequestId = params.get("RequestId")
 
 
+class RemoveWorkflowDsRequest(AbstractModel):
+    """RemoveWorkflowDs请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ProjectId: 项目ID
+        :type ProjectId: str
+        :param _WorkflowId: 工作流ID
+        :type WorkflowId: str
+        """
+        self._ProjectId = None
+        self._WorkflowId = None
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def WorkflowId(self):
+        return self._WorkflowId
+
+    @WorkflowId.setter
+    def WorkflowId(self, WorkflowId):
+        self._WorkflowId = WorkflowId
+
+
+    def _deserialize(self, params):
+        self._ProjectId = params.get("ProjectId")
+        self._WorkflowId = params.get("WorkflowId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class RemoveWorkflowDsResponse(AbstractModel):
+    """RemoveWorkflowDs返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 工作流ID
+        :type Data: bool
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._Data = params.get("Data")
+        self._RequestId = params.get("RequestId")
+
+
 class RerunInstancesRequest(AbstractModel):
     """RerunInstances请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -38358,14 +39187,208 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class StageCloudApiRequest(AbstractModel):
+    """无
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ClusterId: 无
+        :type ClusterId: str
+        :param _StageId: 无
+        :type StageId: str
+        :param _JobId: 无
+        :type JobId: str
+        :param _StageName: 无
+        :type StageName: str
+        :param _Type: 无
+        :type Type: str
+        :param _Mode: 无
+        :type Mode: str
+        :param _Version: 无
+        :type Version: str
+        :param _Queue: 无
+        :type Queue: str
+        :param _Content: 无
+        :type Content: str
+        :param _Parameters: 无
+        :type Parameters: list of Property
+        :param _Description: 无
+        :type Description: str
+        :param _ProjectId: 无
+        :type ProjectId: str
+        :param _JobType: 无
+        :type JobType: str
+        :param _WorkFlowId: 无
+        :type WorkFlowId: str
+        """
+        self._ClusterId = None
+        self._StageId = None
+        self._JobId = None
+        self._StageName = None
+        self._Type = None
+        self._Mode = None
+        self._Version = None
+        self._Queue = None
+        self._Content = None
+        self._Parameters = None
+        self._Description = None
+        self._ProjectId = None
+        self._JobType = None
+        self._WorkFlowId = None
+
+    @property
+    def ClusterId(self):
+        return self._ClusterId
+
+    @ClusterId.setter
+    def ClusterId(self, ClusterId):
+        self._ClusterId = ClusterId
+
+    @property
+    def StageId(self):
+        return self._StageId
+
+    @StageId.setter
+    def StageId(self, StageId):
+        self._StageId = StageId
+
+    @property
+    def JobId(self):
+        return self._JobId
+
+    @JobId.setter
+    def JobId(self, JobId):
+        self._JobId = JobId
+
+    @property
+    def StageName(self):
+        return self._StageName
+
+    @StageName.setter
+    def StageName(self, StageName):
+        self._StageName = StageName
+
+    @property
+    def Type(self):
+        return self._Type
+
+    @Type.setter
+    def Type(self, Type):
+        self._Type = Type
+
+    @property
+    def Mode(self):
+        return self._Mode
+
+    @Mode.setter
+    def Mode(self, Mode):
+        self._Mode = Mode
+
+    @property
+    def Version(self):
+        return self._Version
+
+    @Version.setter
+    def Version(self, Version):
+        self._Version = Version
+
+    @property
+    def Queue(self):
+        return self._Queue
+
+    @Queue.setter
+    def Queue(self, Queue):
+        self._Queue = Queue
+
+    @property
+    def Content(self):
+        return self._Content
+
+    @Content.setter
+    def Content(self, Content):
+        self._Content = Content
+
+    @property
+    def Parameters(self):
+        return self._Parameters
+
+    @Parameters.setter
+    def Parameters(self, Parameters):
+        self._Parameters = Parameters
+
+    @property
+    def Description(self):
+        return self._Description
+
+    @Description.setter
+    def Description(self, Description):
+        self._Description = Description
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def JobType(self):
+        return self._JobType
+
+    @JobType.setter
+    def JobType(self, JobType):
+        self._JobType = JobType
+
+    @property
+    def WorkFlowId(self):
+        return self._WorkFlowId
+
+    @WorkFlowId.setter
+    def WorkFlowId(self, WorkFlowId):
+        self._WorkFlowId = WorkFlowId
+
+
+    def _deserialize(self, params):
+        self._ClusterId = params.get("ClusterId")
+        self._StageId = params.get("StageId")
+        self._JobId = params.get("JobId")
+        self._StageName = params.get("StageName")
+        self._Type = params.get("Type")
+        self._Mode = params.get("Mode")
+        self._Version = params.get("Version")
+        self._Queue = params.get("Queue")
+        self._Content = params.get("Content")
+        if params.get("Parameters") is not None:
+            self._Parameters = []
+            for item in params.get("Parameters"):
+                obj = Property()
+                obj._deserialize(item)
+                self._Parameters.append(obj)
+        self._Description = params.get("Description")
+        self._ProjectId = params.get("ProjectId")
+        self._JobType = params.get("JobType")
+        self._WorkFlowId = params.get("WorkFlowId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class StartIntegrationTaskRequest(AbstractModel):
     """StartIntegrationTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -38671,14 +39694,247 @@
 
     def _deserialize(self, params):
         self._FunctionId = params.get("FunctionId")
         self._ErrorMessage = params.get("ErrorMessage")
         self._RequestId = params.get("RequestId")
 
 
+class SubmitSqlTaskRequest(AbstractModel):
+    """SubmitSqlTask请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _DatabaseType: 数据库类型
+        :type DatabaseType: str
+        :param _DatasourceId: 数据源Id
+        :type DatasourceId: int
+        :param _GroupId: 资源组Id
+        :type GroupId: str
+        :param _ScriptId: 脚本文件id
+        :type ScriptId: str
+        :param _ProjectId: 项目id
+        :type ProjectId: str
+        :param _DatabaseName: 数据库名称
+        :type DatabaseName: str
+        :param _EngineId: 执行引擎实例ID
+        :type EngineId: str
+        :param _ScriptContent: 脚本内容
+        :type ScriptContent: str
+        :param _ResourceQueue: 资源队列
+        :type ResourceQueue: str
+        :param _DatasourceType: 数据库类型
+        :type DatasourceType: str
+        :param _ComputeResource: 计算资源名称
+        :type ComputeResource: str
+        :param _RunParams: 高级运行参数
+        :type RunParams: str
+        :param _ConfParams: 高级设置
+        :type ConfParams: str
+        """
+        self._DatabaseType = None
+        self._DatasourceId = None
+        self._GroupId = None
+        self._ScriptId = None
+        self._ProjectId = None
+        self._DatabaseName = None
+        self._EngineId = None
+        self._ScriptContent = None
+        self._ResourceQueue = None
+        self._DatasourceType = None
+        self._ComputeResource = None
+        self._RunParams = None
+        self._ConfParams = None
+
+    @property
+    def DatabaseType(self):
+        return self._DatabaseType
+
+    @DatabaseType.setter
+    def DatabaseType(self, DatabaseType):
+        self._DatabaseType = DatabaseType
+
+    @property
+    def DatasourceId(self):
+        return self._DatasourceId
+
+    @DatasourceId.setter
+    def DatasourceId(self, DatasourceId):
+        self._DatasourceId = DatasourceId
+
+    @property
+    def GroupId(self):
+        return self._GroupId
+
+    @GroupId.setter
+    def GroupId(self, GroupId):
+        self._GroupId = GroupId
+
+    @property
+    def ScriptId(self):
+        return self._ScriptId
+
+    @ScriptId.setter
+    def ScriptId(self, ScriptId):
+        self._ScriptId = ScriptId
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def DatabaseName(self):
+        return self._DatabaseName
+
+    @DatabaseName.setter
+    def DatabaseName(self, DatabaseName):
+        self._DatabaseName = DatabaseName
+
+    @property
+    def EngineId(self):
+        return self._EngineId
+
+    @EngineId.setter
+    def EngineId(self, EngineId):
+        self._EngineId = EngineId
+
+    @property
+    def ScriptContent(self):
+        return self._ScriptContent
+
+    @ScriptContent.setter
+    def ScriptContent(self, ScriptContent):
+        self._ScriptContent = ScriptContent
+
+    @property
+    def ResourceQueue(self):
+        return self._ResourceQueue
+
+    @ResourceQueue.setter
+    def ResourceQueue(self, ResourceQueue):
+        self._ResourceQueue = ResourceQueue
+
+    @property
+    def DatasourceType(self):
+        return self._DatasourceType
+
+    @DatasourceType.setter
+    def DatasourceType(self, DatasourceType):
+        self._DatasourceType = DatasourceType
+
+    @property
+    def ComputeResource(self):
+        return self._ComputeResource
+
+    @ComputeResource.setter
+    def ComputeResource(self, ComputeResource):
+        self._ComputeResource = ComputeResource
+
+    @property
+    def RunParams(self):
+        return self._RunParams
+
+    @RunParams.setter
+    def RunParams(self, RunParams):
+        self._RunParams = RunParams
+
+    @property
+    def ConfParams(self):
+        return self._ConfParams
+
+    @ConfParams.setter
+    def ConfParams(self, ConfParams):
+        self._ConfParams = ConfParams
+
+
+    def _deserialize(self, params):
+        self._DatabaseType = params.get("DatabaseType")
+        self._DatasourceId = params.get("DatasourceId")
+        self._GroupId = params.get("GroupId")
+        self._ScriptId = params.get("ScriptId")
+        self._ProjectId = params.get("ProjectId")
+        self._DatabaseName = params.get("DatabaseName")
+        self._EngineId = params.get("EngineId")
+        self._ScriptContent = params.get("ScriptContent")
+        self._ResourceQueue = params.get("ResourceQueue")
+        self._DatasourceType = params.get("DatasourceType")
+        self._ComputeResource = params.get("ComputeResource")
+        self._RunParams = params.get("RunParams")
+        self._ConfParams = params.get("ConfParams")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SubmitSqlTaskResponse(AbstractModel):
+    """SubmitSqlTask返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Record: 任务提交记录
+        :type Record: :class:`tencentcloud.wedata.v20210820.models.AdhocRecord`
+        :param _Details: 子任务记录列表
+        :type Details: list of AdhocDetail
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Record = None
+        self._Details = None
+        self._RequestId = None
+
+    @property
+    def Record(self):
+        return self._Record
+
+    @Record.setter
+    def Record(self, Record):
+        self._Record = Record
+
+    @property
+    def Details(self):
+        return self._Details
+
+    @Details.setter
+    def Details(self, Details):
+        self._Details = Details
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Record") is not None:
+            self._Record = AdhocRecord()
+            self._Record._deserialize(params.get("Record"))
+        if params.get("Details") is not None:
+            self._Details = []
+            for item in params.get("Details"):
+                obj = AdhocDetail()
+                obj._deserialize(item)
+                self._Details.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
 class SubmitTaskRequest(AbstractModel):
     """SubmitTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -38777,14 +40033,197 @@
 
 
     def _deserialize(self, params):
         self._Data = params.get("Data")
         self._RequestId = params.get("RequestId")
 
 
+class SubmitTaskTestRunRequest(AbstractModel):
+    """SubmitTaskTestRun请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TaskIds: 无
+        :type TaskIds: str
+        :param _ProjectId: 无
+        :type ProjectId: str
+        :param _WorkFlowId: 无
+        :type WorkFlowId: str
+        :param _Name: 无
+        :type Name: str
+        :param _Tasks: 无
+        :type Tasks: list of StageCloudApiRequest
+        :param _Description: 无
+        :type Description: str
+        :param _RunParams: 无
+        :type RunParams: str
+        :param _ScriptContent: 无
+        :type ScriptContent: str
+        :param _VersionId: 无
+        :type VersionId: str
+        """
+        self._TaskIds = None
+        self._ProjectId = None
+        self._WorkFlowId = None
+        self._Name = None
+        self._Tasks = None
+        self._Description = None
+        self._RunParams = None
+        self._ScriptContent = None
+        self._VersionId = None
+
+    @property
+    def TaskIds(self):
+        return self._TaskIds
+
+    @TaskIds.setter
+    def TaskIds(self, TaskIds):
+        self._TaskIds = TaskIds
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def WorkFlowId(self):
+        return self._WorkFlowId
+
+    @WorkFlowId.setter
+    def WorkFlowId(self, WorkFlowId):
+        self._WorkFlowId = WorkFlowId
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def Tasks(self):
+        return self._Tasks
+
+    @Tasks.setter
+    def Tasks(self, Tasks):
+        self._Tasks = Tasks
+
+    @property
+    def Description(self):
+        return self._Description
+
+    @Description.setter
+    def Description(self, Description):
+        self._Description = Description
+
+    @property
+    def RunParams(self):
+        return self._RunParams
+
+    @RunParams.setter
+    def RunParams(self, RunParams):
+        self._RunParams = RunParams
+
+    @property
+    def ScriptContent(self):
+        return self._ScriptContent
+
+    @ScriptContent.setter
+    def ScriptContent(self, ScriptContent):
+        self._ScriptContent = ScriptContent
+
+    @property
+    def VersionId(self):
+        return self._VersionId
+
+    @VersionId.setter
+    def VersionId(self, VersionId):
+        self._VersionId = VersionId
+
+
+    def _deserialize(self, params):
+        self._TaskIds = params.get("TaskIds")
+        self._ProjectId = params.get("ProjectId")
+        self._WorkFlowId = params.get("WorkFlowId")
+        self._Name = params.get("Name")
+        if params.get("Tasks") is not None:
+            self._Tasks = []
+            for item in params.get("Tasks"):
+                obj = StageCloudApiRequest()
+                obj._deserialize(item)
+                self._Tasks.append(obj)
+        self._Description = params.get("Description")
+        self._RunParams = params.get("RunParams")
+        self._ScriptContent = params.get("ScriptContent")
+        self._VersionId = params.get("VersionId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SubmitTaskTestRunResponse(AbstractModel):
+    """SubmitTaskTestRun返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _JobId: 无
+        :type JobId: int
+        :param _RecordId: 无
+        :type RecordId: list of int
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._JobId = None
+        self._RecordId = None
+        self._RequestId = None
+
+    @property
+    def JobId(self):
+        return self._JobId
+
+    @JobId.setter
+    def JobId(self, JobId):
+        self._JobId = JobId
+
+    @property
+    def RecordId(self):
+        return self._RecordId
+
+    @RecordId.setter
+    def RecordId(self, RecordId):
+        self._RecordId = RecordId
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._JobId = params.get("JobId")
+        self._RecordId = params.get("RecordId")
+        self._RequestId = params.get("RequestId")
+
+
 class SubmitWorkflow(AbstractModel):
     """提交工作流实体
 
     """
 
     def __init__(self):
         r"""
@@ -40549,14 +41988,24 @@
         :type TargetServiceType: str
         :param _AlarmType: 任务告警类型
 注意：此字段可能返回 null，表示取不到有效值。
         :type AlarmType: str
         :param _CreateTime: 任务创建时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type CreateTime: str
+        :param _UserId: UserId
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserId: str
+        :param _OwnerId: OwnerId
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OwnerId: str
+        :param _TenantId: TenantId
+
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TenantId: str
         """
         self._TaskId = None
         self._TaskName = None
         self._WorkflowId = None
         self._WorkflowName = None
         self._ProjectName = None
         self._ProjectIdent = None
@@ -40581,14 +42030,17 @@
         self._Layer = None
         self._SourceServiceId = None
         self._SourceServiceType = None
         self._TargetServiceId = None
         self._TargetServiceType = None
         self._AlarmType = None
         self._CreateTime = None
+        self._UserId = None
+        self._OwnerId = None
+        self._TenantId = None
 
     @property
     def TaskId(self):
         return self._TaskId
 
     @TaskId.setter
     def TaskId(self, TaskId):
@@ -40830,14 +42282,38 @@
     def CreateTime(self):
         return self._CreateTime
 
     @CreateTime.setter
     def CreateTime(self, CreateTime):
         self._CreateTime = CreateTime
 
+    @property
+    def UserId(self):
+        return self._UserId
+
+    @UserId.setter
+    def UserId(self, UserId):
+        self._UserId = UserId
+
+    @property
+    def OwnerId(self):
+        return self._OwnerId
+
+    @OwnerId.setter
+    def OwnerId(self, OwnerId):
+        self._OwnerId = OwnerId
+
+    @property
+    def TenantId(self):
+        return self._TenantId
+
+    @TenantId.setter
+    def TenantId(self, TenantId):
+        self._TenantId = TenantId
+
 
     def _deserialize(self, params):
         self._TaskId = params.get("TaskId")
         self._TaskName = params.get("TaskName")
         self._WorkflowId = params.get("WorkflowId")
         self._WorkflowName = params.get("WorkflowName")
         self._ProjectName = params.get("ProjectName")
@@ -40863,14 +42339,17 @@
         self._Layer = params.get("Layer")
         self._SourceServiceId = params.get("SourceServiceId")
         self._SourceServiceType = params.get("SourceServiceType")
         self._TargetServiceId = params.get("TargetServiceId")
         self._TargetServiceType = params.get("TargetServiceType")
         self._AlarmType = params.get("AlarmType")
         self._CreateTime = params.get("CreateTime")
+        self._UserId = params.get("UserId")
+        self._OwnerId = params.get("OwnerId")
+        self._TenantId = params.get("TenantId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -43811,14 +45290,352 @@
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
+class UserFileInfo(AbstractModel):
+    """开发空间-获取数据开发脚本信息响应体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ResourceId: 资源ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ResourceId: str
+        :param _FileName: 文件名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FileName: str
+        :param _FileExtensionType: 文件类型，如 jar zip 等
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FileExtensionType: str
+        :param _Type: 文件上传类型，资源管理为 resource
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Type: str
+        :param _Md5Value: 文件MD5值
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Md5Value: str
+        :param _CreateTime: 创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateTime: str
+        :param _UpdateTime: 更新时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UpdateTime: str
+        :param _Size: 文件大小，单位为字节
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Size: int
+        :param _LocalPath: 本地路径
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LocalPath: str
+        :param _LocalTempPath: 本地临时路径
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LocalTempPath: str
+        :param _RemotePath: 远程路径
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RemotePath: str
+        :param _OwnerName: 文件拥有者名字
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OwnerName: str
+        :param _Owner: 文件拥有者uin
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Owner: str
+        :param _PathDepth: 文件深度
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PathDepth: int
+        :param _ProjectId: 项目ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProjectId: str
+        :param _ExtraInfo: 附加信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExtraInfo: list of ParamInfo
+        :param _ZipPath: 本地临时压缩文件绝对路径
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ZipPath: str
+        :param _Bucket: 文件所属存储桶
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Bucket: str
+        :param _Region: 文件所属存储桶的地域
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Region: str
+        :param _DeleteName: 无
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DeleteName: str
+        :param _DeleteOwner: 无
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DeleteOwner: str
+        :param _Operator: 无
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Operator: str
+        :param _OperatorName: 无
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OperatorName: str
+        :param _EncodeExtraInfo: 附加信息 base64编码
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EncodeExtraInfo: str
+        """
+        self._ResourceId = None
+        self._FileName = None
+        self._FileExtensionType = None
+        self._Type = None
+        self._Md5Value = None
+        self._CreateTime = None
+        self._UpdateTime = None
+        self._Size = None
+        self._LocalPath = None
+        self._LocalTempPath = None
+        self._RemotePath = None
+        self._OwnerName = None
+        self._Owner = None
+        self._PathDepth = None
+        self._ProjectId = None
+        self._ExtraInfo = None
+        self._ZipPath = None
+        self._Bucket = None
+        self._Region = None
+        self._DeleteName = None
+        self._DeleteOwner = None
+        self._Operator = None
+        self._OperatorName = None
+        self._EncodeExtraInfo = None
+
+    @property
+    def ResourceId(self):
+        return self._ResourceId
+
+    @ResourceId.setter
+    def ResourceId(self, ResourceId):
+        self._ResourceId = ResourceId
+
+    @property
+    def FileName(self):
+        return self._FileName
+
+    @FileName.setter
+    def FileName(self, FileName):
+        self._FileName = FileName
+
+    @property
+    def FileExtensionType(self):
+        return self._FileExtensionType
+
+    @FileExtensionType.setter
+    def FileExtensionType(self, FileExtensionType):
+        self._FileExtensionType = FileExtensionType
+
+    @property
+    def Type(self):
+        return self._Type
+
+    @Type.setter
+    def Type(self, Type):
+        self._Type = Type
+
+    @property
+    def Md5Value(self):
+        return self._Md5Value
+
+    @Md5Value.setter
+    def Md5Value(self, Md5Value):
+        self._Md5Value = Md5Value
+
+    @property
+    def CreateTime(self):
+        return self._CreateTime
+
+    @CreateTime.setter
+    def CreateTime(self, CreateTime):
+        self._CreateTime = CreateTime
+
+    @property
+    def UpdateTime(self):
+        return self._UpdateTime
+
+    @UpdateTime.setter
+    def UpdateTime(self, UpdateTime):
+        self._UpdateTime = UpdateTime
+
+    @property
+    def Size(self):
+        return self._Size
+
+    @Size.setter
+    def Size(self, Size):
+        self._Size = Size
+
+    @property
+    def LocalPath(self):
+        return self._LocalPath
+
+    @LocalPath.setter
+    def LocalPath(self, LocalPath):
+        self._LocalPath = LocalPath
+
+    @property
+    def LocalTempPath(self):
+        return self._LocalTempPath
+
+    @LocalTempPath.setter
+    def LocalTempPath(self, LocalTempPath):
+        self._LocalTempPath = LocalTempPath
+
+    @property
+    def RemotePath(self):
+        return self._RemotePath
+
+    @RemotePath.setter
+    def RemotePath(self, RemotePath):
+        self._RemotePath = RemotePath
+
+    @property
+    def OwnerName(self):
+        return self._OwnerName
+
+    @OwnerName.setter
+    def OwnerName(self, OwnerName):
+        self._OwnerName = OwnerName
+
+    @property
+    def Owner(self):
+        return self._Owner
+
+    @Owner.setter
+    def Owner(self, Owner):
+        self._Owner = Owner
+
+    @property
+    def PathDepth(self):
+        return self._PathDepth
+
+    @PathDepth.setter
+    def PathDepth(self, PathDepth):
+        self._PathDepth = PathDepth
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def ExtraInfo(self):
+        return self._ExtraInfo
+
+    @ExtraInfo.setter
+    def ExtraInfo(self, ExtraInfo):
+        self._ExtraInfo = ExtraInfo
+
+    @property
+    def ZipPath(self):
+        return self._ZipPath
+
+    @ZipPath.setter
+    def ZipPath(self, ZipPath):
+        self._ZipPath = ZipPath
+
+    @property
+    def Bucket(self):
+        return self._Bucket
+
+    @Bucket.setter
+    def Bucket(self, Bucket):
+        self._Bucket = Bucket
+
+    @property
+    def Region(self):
+        return self._Region
+
+    @Region.setter
+    def Region(self, Region):
+        self._Region = Region
+
+    @property
+    def DeleteName(self):
+        return self._DeleteName
+
+    @DeleteName.setter
+    def DeleteName(self, DeleteName):
+        self._DeleteName = DeleteName
+
+    @property
+    def DeleteOwner(self):
+        return self._DeleteOwner
+
+    @DeleteOwner.setter
+    def DeleteOwner(self, DeleteOwner):
+        self._DeleteOwner = DeleteOwner
+
+    @property
+    def Operator(self):
+        return self._Operator
+
+    @Operator.setter
+    def Operator(self, Operator):
+        self._Operator = Operator
+
+    @property
+    def OperatorName(self):
+        return self._OperatorName
+
+    @OperatorName.setter
+    def OperatorName(self, OperatorName):
+        self._OperatorName = OperatorName
+
+    @property
+    def EncodeExtraInfo(self):
+        return self._EncodeExtraInfo
+
+    @EncodeExtraInfo.setter
+    def EncodeExtraInfo(self, EncodeExtraInfo):
+        self._EncodeExtraInfo = EncodeExtraInfo
+
+
+    def _deserialize(self, params):
+        self._ResourceId = params.get("ResourceId")
+        self._FileName = params.get("FileName")
+        self._FileExtensionType = params.get("FileExtensionType")
+        self._Type = params.get("Type")
+        self._Md5Value = params.get("Md5Value")
+        self._CreateTime = params.get("CreateTime")
+        self._UpdateTime = params.get("UpdateTime")
+        self._Size = params.get("Size")
+        self._LocalPath = params.get("LocalPath")
+        self._LocalTempPath = params.get("LocalTempPath")
+        self._RemotePath = params.get("RemotePath")
+        self._OwnerName = params.get("OwnerName")
+        self._Owner = params.get("Owner")
+        self._PathDepth = params.get("PathDepth")
+        self._ProjectId = params.get("ProjectId")
+        if params.get("ExtraInfo") is not None:
+            self._ExtraInfo = []
+            for item in params.get("ExtraInfo"):
+                obj = ParamInfo()
+                obj._deserialize(item)
+                self._ExtraInfo.append(obj)
+        self._ZipPath = params.get("ZipPath")
+        self._Bucket = params.get("Bucket")
+        self._Region = params.get("Region")
+        self._DeleteName = params.get("DeleteName")
+        self._DeleteOwner = params.get("DeleteOwner")
+        self._Operator = params.get("Operator")
+        self._OperatorName = params.get("OperatorName")
+        self._EncodeExtraInfo = params.get("EncodeExtraInfo")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class WeightInfo(AbstractModel):
     """权重信息
 
     """
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.937/tencentcloud/wedata/v20210820/wedata_client.py` & `tencentcloud-sdk-python-wedata-3.0.938/tencentcloud/wedata/v20210820/wedata_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.BatchCreateIntegrationTaskAlarmsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchDeleteIntegrationTasks(self, request):
         """批量删除集成任务
 
         :param request: Request instance for BatchDeleteIntegrationTasks.
         :type request: :class:`tencentcloud.wedata.v20210820.models.BatchDeleteIntegrationTasksRequest`
@@ -65,15 +65,38 @@
             model = models.BatchDeleteIntegrationTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def BatchDeleteTasksDs(self, request):
+        """Ds批量删除任务，仅对任务状态为”已停止“有效；
+
+        :param request: Request instance for BatchDeleteTasksDs.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.BatchDeleteTasksDsRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.BatchDeleteTasksDsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("BatchDeleteTasksDs", params, headers=headers)
+            response = json.loads(body)
+            model = models.BatchDeleteTasksDsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchDeleteTasksNew(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         批量删除任务，仅对任务状态为”已停止“有效；
 
         :param request: Request instance for BatchDeleteTasksNew.
@@ -89,15 +112,15 @@
             model = models.BatchDeleteTasksNewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchForceSuccessIntegrationTaskInstances(self, request):
         """批量置成功集成任务实例
 
         :param request: Request instance for BatchForceSuccessIntegrationTaskInstances.
         :type request: :class:`tencentcloud.wedata.v20210820.models.BatchForceSuccessIntegrationTaskInstancesRequest`
@@ -112,15 +135,15 @@
             model = models.BatchForceSuccessIntegrationTaskInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchKillIntegrationTaskInstances(self, request):
         """批量终止集成任务实例
 
         :param request: Request instance for BatchKillIntegrationTaskInstances.
         :type request: :class:`tencentcloud.wedata.v20210820.models.BatchKillIntegrationTaskInstancesRequest`
@@ -135,15 +158,15 @@
             model = models.BatchKillIntegrationTaskInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchMakeUpIntegrationTasks(self, request):
         """对集成离线任务执行批量补数据操作
 
         :param request: Request instance for BatchMakeUpIntegrationTasks.
         :type request: :class:`tencentcloud.wedata.v20210820.models.BatchMakeUpIntegrationTasksRequest`
@@ -158,15 +181,15 @@
             model = models.BatchMakeUpIntegrationTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchModifyOwnersNew(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         批量修改任务责任人
 
         :param request: Request instance for BatchModifyOwnersNew.
@@ -182,15 +205,15 @@
             model = models.BatchModifyOwnersNewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchRerunIntegrationTaskInstances(self, request):
         """批量重跑集成任务实例
 
         :param request: Request instance for BatchRerunIntegrationTaskInstances.
         :type request: :class:`tencentcloud.wedata.v20210820.models.BatchRerunIntegrationTaskInstancesRequest`
@@ -205,15 +228,15 @@
             model = models.BatchRerunIntegrationTaskInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchResumeIntegrationTasks(self, request):
         """批量继续执行集成实时任务
 
         :param request: Request instance for BatchResumeIntegrationTasks.
         :type request: :class:`tencentcloud.wedata.v20210820.models.BatchResumeIntegrationTasksRequest`
@@ -228,15 +251,15 @@
             model = models.BatchResumeIntegrationTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchStartIntegrationTasks(self, request):
         """批量运行集成任务
 
         :param request: Request instance for BatchStartIntegrationTasks.
         :type request: :class:`tencentcloud.wedata.v20210820.models.BatchStartIntegrationTasksRequest`
@@ -251,15 +274,15 @@
             model = models.BatchStartIntegrationTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchStopIntegrationTasks(self, request):
         """批量停止集成任务
 
         :param request: Request instance for BatchStopIntegrationTasks.
         :type request: :class:`tencentcloud.wedata.v20210820.models.BatchStopIntegrationTasksRequest`
@@ -274,15 +297,15 @@
             model = models.BatchStopIntegrationTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchStopTasksNew(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         仅对任务状态为”调度中“和”已暂停“有效，对所选任务的任务实例进行终止，并停止调度
 
         :param request: Request instance for BatchStopTasksNew.
@@ -298,15 +321,15 @@
             model = models.BatchStopTasksNewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchSuspendIntegrationTasks(self, request):
         """批量暂停集成任务
 
         :param request: Request instance for BatchSuspendIntegrationTasks.
         :type request: :class:`tencentcloud.wedata.v20210820.models.BatchSuspendIntegrationTasksRequest`
@@ -321,15 +344,15 @@
             model = models.BatchSuspendIntegrationTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchUpdateIntegrationTasks(self, request):
         """批量更新集成任务（暂时仅支持批量更新责任人）
 
         :param request: Request instance for BatchUpdateIntegrationTasks.
         :type request: :class:`tencentcloud.wedata.v20210820.models.BatchUpdateIntegrationTasksRequest`
@@ -344,15 +367,15 @@
             model = models.BatchUpdateIntegrationTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckAlarmRegularNameExist(self, request):
         """判断告警规则重名
 
         :param request: Request instance for CheckAlarmRegularNameExist.
         :type request: :class:`tencentcloud.wedata.v20210820.models.CheckAlarmRegularNameExistRequest`
@@ -367,15 +390,15 @@
             model = models.CheckAlarmRegularNameExistResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckDuplicateRuleName(self, request):
         """检查规则名称是否重复
 
         :param request: Request instance for CheckDuplicateRuleName.
         :type request: :class:`tencentcloud.wedata.v20210820.models.CheckDuplicateRuleNameRequest`
@@ -390,15 +413,15 @@
             model = models.CheckDuplicateRuleNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckDuplicateTemplateName(self, request):
         """检查规则模板名称是否重复
 
         :param request: Request instance for CheckDuplicateTemplateName.
         :type request: :class:`tencentcloud.wedata.v20210820.models.CheckDuplicateTemplateNameRequest`
@@ -413,15 +436,15 @@
             model = models.CheckDuplicateTemplateNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckIntegrationNodeNameExists(self, request):
         """判断集成节点名称是否存在
 
         :param request: Request instance for CheckIntegrationNodeNameExists.
         :type request: :class:`tencentcloud.wedata.v20210820.models.CheckIntegrationNodeNameExistsRequest`
@@ -436,15 +459,15 @@
             model = models.CheckIntegrationNodeNameExistsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckIntegrationTaskNameExists(self, request):
         """判断集成任务名称是否存在
 
         :param request: Request instance for CheckIntegrationTaskNameExists.
         :type request: :class:`tencentcloud.wedata.v20210820.models.CheckIntegrationTaskNameExistsRequest`
@@ -459,15 +482,15 @@
             model = models.CheckIntegrationTaskNameExistsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckTaskNameExist(self, request):
         """离线任务重名校验
 
         :param request: Request instance for CheckTaskNameExist.
         :type request: :class:`tencentcloud.wedata.v20210820.models.CheckTaskNameExistRequest`
@@ -482,15 +505,15 @@
             model = models.CheckTaskNameExistResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CommitExportTask(self, request):
         """提交数据导出任务
 
         :param request: Request instance for CommitExportTask.
         :type request: :class:`tencentcloud.wedata.v20210820.models.CommitExportTaskRequest`
@@ -505,15 +528,15 @@
             model = models.CommitExportTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CommitIntegrationTask(self, request):
         """提交集成任务
 
         :param request: Request instance for CommitIntegrationTask.
         :type request: :class:`tencentcloud.wedata.v20210820.models.CommitIntegrationTaskRequest`
@@ -528,15 +551,15 @@
             model = models.CommitIntegrationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CommitRuleGroupExecResult(self, request):
         """Runner 规则检测结果上报
 
         :param request: Request instance for CommitRuleGroupExecResult.
         :type request: :class:`tencentcloud.wedata.v20210820.models.CommitRuleGroupExecResultRequest`
@@ -551,15 +574,15 @@
             model = models.CommitRuleGroupExecResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CommitRuleGroupTask(self, request):
         """提交规则组运行任务接口
 
         :param request: Request instance for CommitRuleGroupTask.
         :type request: :class:`tencentcloud.wedata.v20210820.models.CommitRuleGroupTaskRequest`
@@ -574,15 +597,15 @@
             model = models.CommitRuleGroupTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCustomFunction(self, request):
         """创建用户自定义函数
 
         :param request: Request instance for CreateCustomFunction.
         :type request: :class:`tencentcloud.wedata.v20210820.models.CreateCustomFunctionRequest`
@@ -597,15 +620,15 @@
             model = models.CreateCustomFunctionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDataSource(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         创建数据源
 
         :param request: Request instance for CreateDataSource.
@@ -621,15 +644,15 @@
             model = models.CreateDataSourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFolder(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         创建文件夹
 
         :param request: Request instance for CreateFolder.
@@ -645,15 +668,15 @@
             model = models.CreateFolderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateHiveTable(self, request):
         """建hive表
 
         :param request: Request instance for CreateHiveTable.
         :type request: :class:`tencentcloud.wedata.v20210820.models.CreateHiveTableRequest`
@@ -668,15 +691,15 @@
             model = models.CreateHiveTableResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateHiveTableByDDL(self, request):
         """创建hive表，返回表名称
 
         :param request: Request instance for CreateHiveTableByDDL.
         :type request: :class:`tencentcloud.wedata.v20210820.models.CreateHiveTableByDDLRequest`
@@ -691,15 +714,15 @@
             model = models.CreateHiveTableByDDLResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateInLongAgent(self, request):
         """注册采集器
 
         :param request: Request instance for CreateInLongAgent.
         :type request: :class:`tencentcloud.wedata.v20210820.models.CreateInLongAgentRequest`
@@ -714,15 +737,15 @@
             model = models.CreateInLongAgentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateIntegrationNode(self, request):
         """创建集成节点
 
         :param request: Request instance for CreateIntegrationNode.
         :type request: :class:`tencentcloud.wedata.v20210820.models.CreateIntegrationNodeRequest`
@@ -737,15 +760,15 @@
             model = models.CreateIntegrationNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateIntegrationTask(self, request):
         """创建集成任务
 
         :param request: Request instance for CreateIntegrationTask.
         :type request: :class:`tencentcloud.wedata.v20210820.models.CreateIntegrationTaskRequest`
@@ -760,15 +783,15 @@
             model = models.CreateIntegrationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOfflineTask(self, request):
         """创建离线任务
 
         :param request: Request instance for CreateOfflineTask.
         :type request: :class:`tencentcloud.wedata.v20210820.models.CreateOfflineTaskRequest`
@@ -783,15 +806,15 @@
             model = models.CreateOfflineTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOrUpdateResource(self, request):
         """资源管理需要先将资源上传到cos中，然后调用该接口，将cos资源绑定到wedata
 
         :param request: Request instance for CreateOrUpdateResource.
         :type request: :class:`tencentcloud.wedata.v20210820.models.CreateOrUpdateResourceRequest`
@@ -806,15 +829,15 @@
             model = models.CreateOrUpdateResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateResourcePath(self, request):
         """文件路径的根目录为 /datastudio/resource，如果要在根目录下创建 aaa 文件夹，FilePath的值应该为 /datastudio/resource，如果根目录下已经创建了 aaa 文件夹，要在 aaa 下创建  bbb 文件夹，FilePath的值应该为 /datastudio/resource/aaa
 
         :param request: Request instance for CreateResourcePath.
         :type request: :class:`tencentcloud.wedata.v20210820.models.CreateResourcePathRequest`
@@ -829,15 +852,15 @@
             model = models.CreateResourcePathResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRule(self, request):
         """创建质量规则接口
 
         :param request: Request instance for CreateRule.
         :type request: :class:`tencentcloud.wedata.v20210820.models.CreateRuleRequest`
@@ -852,15 +875,15 @@
             model = models.CreateRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRuleTemplate(self, request):
         """创建规则模版
 
         :param request: Request instance for CreateRuleTemplate.
         :type request: :class:`tencentcloud.wedata.v20210820.models.CreateRuleTemplateRequest`
@@ -875,15 +898,15 @@
             model = models.CreateRuleTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTask(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         创建任务
 
         :param request: Request instance for CreateTask.
@@ -899,15 +922,15 @@
             model = models.CreateTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTaskAlarmRegular(self, request):
         """创建任务告警规则
 
         :param request: Request instance for CreateTaskAlarmRegular.
         :type request: :class:`tencentcloud.wedata.v20210820.models.CreateTaskAlarmRegularRequest`
@@ -922,15 +945,15 @@
             model = models.CreateTaskAlarmRegularResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateWorkflow(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         创建工作流
 
         :param request: Request instance for CreateWorkflow.
@@ -946,15 +969,15 @@
             model = models.CreateWorkflowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCustomFunction(self, request):
         """删除用户自定义函数
 
         :param request: Request instance for DeleteCustomFunction.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DeleteCustomFunctionRequest`
@@ -969,15 +992,15 @@
             model = models.DeleteCustomFunctionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDataSources(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         删除数据源
 
         :param request: Request instance for DeleteDataSources.
@@ -993,15 +1016,38 @@
             model = models.DeleteDataSourcesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DeleteFilePath(self, request):
+        """开发空间-批量删除目录和文件
+
+        :param request: Request instance for DeleteFilePath.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.DeleteFilePathRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.DeleteFilePathResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteFilePath", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteFilePathResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteFolder(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         删除文件夹
 
         :param request: Request instance for DeleteFolder.
@@ -1017,15 +1063,15 @@
             model = models.DeleteFolderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteInLongAgent(self, request):
         """删除采集器
 
         :param request: Request instance for DeleteInLongAgent.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DeleteInLongAgentRequest`
@@ -1040,15 +1086,15 @@
             model = models.DeleteInLongAgentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteIntegrationNode(self, request):
         """删除集成节点
 
         :param request: Request instance for DeleteIntegrationNode.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DeleteIntegrationNodeRequest`
@@ -1063,15 +1109,15 @@
             model = models.DeleteIntegrationNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteIntegrationTask(self, request):
         """删除集成任务
 
         :param request: Request instance for DeleteIntegrationTask.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DeleteIntegrationTaskRequest`
@@ -1086,15 +1132,15 @@
             model = models.DeleteIntegrationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteOfflineTask(self, request):
         """删除任务
 
         :param request: Request instance for DeleteOfflineTask.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DeleteOfflineTaskRequest`
@@ -1109,15 +1155,38 @@
             model = models.DeleteOfflineTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DeleteProjectParamDs(self, request):
+        """删除项目参数
+
+        :param request: Request instance for DeleteProjectParamDs.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.DeleteProjectParamDsRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.DeleteProjectParamDsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteProjectParamDs", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteProjectParamDsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteResource(self, request):
         """资源管理删除资源
 
         :param request: Request instance for DeleteResource.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DeleteResourceRequest`
@@ -1132,15 +1201,38 @@
             model = models.DeleteResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DeleteResourceFiles(self, request):
+        """资源管理-批量删除资源文件
+
+        :param request: Request instance for DeleteResourceFiles.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.DeleteResourceFilesRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.DeleteResourceFilesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteResourceFiles", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteResourceFilesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRule(self, request):
         """删除质量规则接口
 
         :param request: Request instance for DeleteRule.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DeleteRuleRequest`
@@ -1155,15 +1247,15 @@
             model = models.DeleteRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRuleTemplate(self, request):
         """删除规则模版
 
         :param request: Request instance for DeleteRuleTemplate.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DeleteRuleTemplateRequest`
@@ -1178,15 +1270,15 @@
             model = models.DeleteRuleTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTaskAlarmRegular(self, request):
         """删除任务告警规则
 
         :param request: Request instance for DeleteTaskAlarmRegular.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DeleteTaskAlarmRegularRequest`
@@ -1201,15 +1293,38 @@
             model = models.DeleteTaskAlarmRegularResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DeleteTaskDs(self, request):
+        """删除任务Ds
+
+        :param request: Request instance for DeleteTaskDs.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.DeleteTaskDsRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.DeleteTaskDsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteTaskDs", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteTaskDsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteWorkflowNew(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         删除工作流
 
         :param request: Request instance for DeleteWorkflowNew.
@@ -1225,15 +1340,15 @@
             model = models.DeleteWorkflowNewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAlarmEvents(self, request):
         """告警事件列表
 
         :param request: Request instance for DescribeAlarmEvents.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeAlarmEventsRequest`
@@ -1248,15 +1363,15 @@
             model = models.DescribeAlarmEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAlarmReceiver(self, request):
         """告警接收人详情
 
         :param request: Request instance for DescribeAlarmReceiver.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeAlarmReceiverRequest`
@@ -1271,15 +1386,15 @@
             model = models.DescribeAlarmReceiverResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBatchOperateTask(self, request):
         """批量操作任务列表
 
         :param request: Request instance for DescribeBatchOperateTask.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeBatchOperateTaskRequest`
@@ -1294,15 +1409,15 @@
             model = models.DescribeBatchOperateTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterNamespaceList(self, request):
         """获取集群命名空间列表
 
         :param request: Request instance for DescribeClusterNamespaceList.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeClusterNamespaceListRequest`
@@ -1317,15 +1432,15 @@
             model = models.DescribeClusterNamespaceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeColumnLineage(self, request):
         """列出字段血缘信息
 
         :param request: Request instance for DescribeColumnLineage.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeColumnLineageRequest`
@@ -1340,15 +1455,15 @@
             model = models.DescribeColumnLineageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataBases(self, request):
         """查询数据来源列表
 
         :param request: Request instance for DescribeDataBases.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeDataBasesRequest`
@@ -1363,15 +1478,15 @@
             model = models.DescribeDataBasesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataCheckStat(self, request):
         """数据质量的概览页面数据监测情况接口
 
         :param request: Request instance for DescribeDataCheckStat.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeDataCheckStatRequest`
@@ -1386,15 +1501,15 @@
             model = models.DescribeDataCheckStatResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataObjects(self, request):
         """查询规则组数据对象列表
 
         :param request: Request instance for DescribeDataObjects.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeDataObjectsRequest`
@@ -1409,15 +1524,15 @@
             model = models.DescribeDataObjectsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataSourceInfoList(self, request):
         """获取数据源信息-数据源分页列表
 
         :param request: Request instance for DescribeDataSourceInfoList.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeDataSourceInfoListRequest`
@@ -1432,15 +1547,15 @@
             model = models.DescribeDataSourceInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataSourceList(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         数据源详情
 
         :param request: Request instance for DescribeDataSourceList.
@@ -1456,15 +1571,15 @@
             model = models.DescribeDataSourceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataSourceWithoutInfo(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         数据源列表
 
         :param request: Request instance for DescribeDataSourceWithoutInfo.
@@ -1480,15 +1595,15 @@
             model = models.DescribeDataSourceWithoutInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataTypes(self, request):
         """获取字段类型列表
 
         :param request: Request instance for DescribeDataTypes.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeDataTypesRequest`
@@ -1503,15 +1618,15 @@
             model = models.DescribeDataTypesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDatabaseInfoList(self, request):
         """获取数据库信息
 
         :param request: Request instance for DescribeDatabaseInfoList.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeDatabaseInfoListRequest`
@@ -1526,15 +1641,15 @@
             model = models.DescribeDatabaseInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDatasource(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         数据源详情
 
         :param request: Request instance for DescribeDatasource.
@@ -1550,15 +1665,15 @@
             model = models.DescribeDatasourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDependTasksNew(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         根据层级查找上/下游任务节点
 
         :param request: Request instance for DescribeDependTasksNew.
@@ -1574,15 +1689,15 @@
             model = models.DescribeDependTasksNewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDimensionScore(self, request):
         """质量报告-查询质量评分
 
         :param request: Request instance for DescribeDimensionScore.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeDimensionScoreRequest`
@@ -1597,15 +1712,15 @@
             model = models.DescribeDimensionScoreResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeExecStrategy(self, request):
         """查询规则组执行策略
 
         :param request: Request instance for DescribeExecStrategy.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeExecStrategyRequest`
@@ -1620,15 +1735,15 @@
             model = models.DescribeExecStrategyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFolderList(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         拉取文件夹目录
 
         :param request: Request instance for DescribeFolderList.
@@ -1644,15 +1759,15 @@
             model = models.DescribeFolderListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFolderWorkflowList(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         拉取文件夹下的工作流
 
         :param request: Request instance for DescribeFolderWorkflowList.
@@ -1668,15 +1783,15 @@
             model = models.DescribeFolderWorkflowListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFunctionKinds(self, request):
         """查询函数分类
 
         :param request: Request instance for DescribeFunctionKinds.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeFunctionKindsRequest`
@@ -1691,15 +1806,15 @@
             model = models.DescribeFunctionKindsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFunctionTypes(self, request):
         """查询函数类型
 
         :param request: Request instance for DescribeFunctionTypes.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeFunctionTypesRequest`
@@ -1714,15 +1829,15 @@
             model = models.DescribeFunctionTypesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInLongAgentList(self, request):
         """获取采集器列表
 
         :param request: Request instance for DescribeInLongAgentList.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeInLongAgentListRequest`
@@ -1737,15 +1852,15 @@
             model = models.DescribeInLongAgentListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInLongAgentTaskList(self, request):
         """查询采集器关联的任务列表
 
         :param request: Request instance for DescribeInLongAgentTaskList.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeInLongAgentTaskListRequest`
@@ -1760,15 +1875,15 @@
             model = models.DescribeInLongAgentTaskListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInLongAgentVpcList(self, request):
         """获取采集器所在集群的VPC列表
 
         :param request: Request instance for DescribeInLongAgentVpcList.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeInLongAgentVpcListRequest`
@@ -1783,15 +1898,15 @@
             model = models.DescribeInLongAgentVpcListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInLongTkeClusterList(self, request):
         """获取TKE集群列表
 
         :param request: Request instance for DescribeInLongTkeClusterList.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeInLongTkeClusterListRequest`
@@ -1806,15 +1921,15 @@
             model = models.DescribeInLongTkeClusterListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceLastLog(self, request):
         """日志获取详情页面
 
         :param request: Request instance for DescribeInstanceLastLog.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeInstanceLastLogRequest`
@@ -1829,15 +1944,15 @@
             model = models.DescribeInstanceLastLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceList(self, request):
         """获取实例列表
 
         :param request: Request instance for DescribeInstanceList.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeInstanceListRequest`
@@ -1852,15 +1967,15 @@
             model = models.DescribeInstanceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceLog(self, request):
         """获取实例运行日志
 
         :param request: Request instance for DescribeInstanceLog.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeInstanceLogRequest`
@@ -1875,15 +1990,15 @@
             model = models.DescribeInstanceLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceLogList(self, request):
         """离线任务实例运行日志列表
 
         :param request: Request instance for DescribeInstanceLogList.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeInstanceLogListRequest`
@@ -1898,15 +2013,15 @@
             model = models.DescribeInstanceLogListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceLogs(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         获取实例日志列表
 
         :param request: Request instance for DescribeInstanceLogs.
@@ -1922,15 +2037,15 @@
             model = models.DescribeInstanceLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstances(self, request):
         """数据质量，查询调度任务的实例列表
 
         :param request: Request instance for DescribeInstances.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeInstancesRequest`
@@ -1945,15 +2060,15 @@
             model = models.DescribeInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIntegrationNode(self, request):
         """查询集成节点
 
         :param request: Request instance for DescribeIntegrationNode.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeIntegrationNodeRequest`
@@ -1968,15 +2083,15 @@
             model = models.DescribeIntegrationNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIntegrationStatistics(self, request):
         """数据集成大屏概览
 
         :param request: Request instance for DescribeIntegrationStatistics.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeIntegrationStatisticsRequest`
@@ -1991,15 +2106,15 @@
             model = models.DescribeIntegrationStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIntegrationStatisticsAgentStatus(self, request):
         """数据集成大屏采集器状态分布统计
 
         :param request: Request instance for DescribeIntegrationStatisticsAgentStatus.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeIntegrationStatisticsAgentStatusRequest`
@@ -2014,15 +2129,15 @@
             model = models.DescribeIntegrationStatisticsAgentStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIntegrationStatisticsInstanceTrend(self, request):
         """数据集成大屏实例状态统计趋势
 
         :param request: Request instance for DescribeIntegrationStatisticsInstanceTrend.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeIntegrationStatisticsInstanceTrendRequest`
@@ -2037,15 +2152,15 @@
             model = models.DescribeIntegrationStatisticsInstanceTrendResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIntegrationStatisticsRecordsTrend(self, request):
         """数据集成大屏同步条数统计趋势
 
         :param request: Request instance for DescribeIntegrationStatisticsRecordsTrend.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeIntegrationStatisticsRecordsTrendRequest`
@@ -2060,15 +2175,15 @@
             model = models.DescribeIntegrationStatisticsRecordsTrendResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIntegrationStatisticsTaskStatus(self, request):
         """数据集成大屏任务状态分布统计
 
         :param request: Request instance for DescribeIntegrationStatisticsTaskStatus.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeIntegrationStatisticsTaskStatusRequest`
@@ -2083,15 +2198,15 @@
             model = models.DescribeIntegrationStatisticsTaskStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIntegrationStatisticsTaskStatusTrend(self, request):
         """数据集成大屏任务状态统计趋势
 
         :param request: Request instance for DescribeIntegrationStatisticsTaskStatusTrend.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeIntegrationStatisticsTaskStatusTrendRequest`
@@ -2106,15 +2221,15 @@
             model = models.DescribeIntegrationStatisticsTaskStatusTrendResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIntegrationTask(self, request):
         """查询集成任务
 
         :param request: Request instance for DescribeIntegrationTask.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeIntegrationTaskRequest`
@@ -2129,15 +2244,15 @@
             model = models.DescribeIntegrationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIntegrationTasks(self, request):
         """查询集成任务列表
 
         :param request: Request instance for DescribeIntegrationTasks.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeIntegrationTasksRequest`
@@ -2152,15 +2267,15 @@
             model = models.DescribeIntegrationTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIntegrationVersionNodesInfo(self, request):
         """查询集成任务版本节点信息
 
         :param request: Request instance for DescribeIntegrationVersionNodesInfo.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeIntegrationVersionNodesInfoRequest`
@@ -2175,15 +2290,15 @@
             model = models.DescribeIntegrationVersionNodesInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKafkaTopicInfo(self, request):
         """获取kafka的topic信息
 
         :param request: Request instance for DescribeKafkaTopicInfo.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeKafkaTopicInfoRequest`
@@ -2198,15 +2313,15 @@
             model = models.DescribeKafkaTopicInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMonitorsByPage(self, request):
         """分页查询质量监控组
 
         :param request: Request instance for DescribeMonitorsByPage.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeMonitorsByPageRequest`
@@ -2221,15 +2336,15 @@
             model = models.DescribeMonitorsByPageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOfflineTaskToken(self, request):
         """获取离线任务长连接Token
 
         :param request: Request instance for DescribeOfflineTaskToken.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeOfflineTaskTokenRequest`
@@ -2244,15 +2359,15 @@
             model = models.DescribeOfflineTaskTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOperateTasks(self, request):
         """任务运维列表组合条件查询
 
         :param request: Request instance for DescribeOperateTasks.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeOperateTasksRequest`
@@ -2267,15 +2382,15 @@
             model = models.DescribeOperateTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOrganizationalFunctions(self, request):
         """查询全量函数
 
         :param request: Request instance for DescribeOrganizationalFunctions.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeOrganizationalFunctionsRequest`
@@ -2290,15 +2405,15 @@
             model = models.DescribeOrganizationalFunctionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProdTasks(self, request):
         """数据质量获取生产调度任务列表
 
         :param request: Request instance for DescribeProdTasks.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeProdTasksRequest`
@@ -2313,15 +2428,15 @@
             model = models.DescribeProdTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProject(self, request):
         """获取项目信息
 
         :param request: Request instance for DescribeProject.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeProjectRequest`
@@ -2336,15 +2451,15 @@
             model = models.DescribeProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeQualityScore(self, request):
         """质量报告-质量评分
 
         :param request: Request instance for DescribeQualityScore.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeQualityScoreRequest`
@@ -2359,15 +2474,15 @@
             model = models.DescribeQualityScoreResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeQualityScoreTrend(self, request):
         """质量报告-质量分周期趋势
 
         :param request: Request instance for DescribeQualityScoreTrend.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeQualityScoreTrendRequest`
@@ -2382,15 +2497,15 @@
             model = models.DescribeQualityScoreTrendResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRealTimeTaskInstanceNodeInfo(self, request):
         """查询实时任务实例节点信息
 
         :param request: Request instance for DescribeRealTimeTaskInstanceNodeInfo.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRealTimeTaskInstanceNodeInfoRequest`
@@ -2405,15 +2520,15 @@
             model = models.DescribeRealTimeTaskInstanceNodeInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRealTimeTaskMetricOverview(self, request):
         """实时任务运行指标概览
 
         :param request: Request instance for DescribeRealTimeTaskMetricOverview.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRealTimeTaskMetricOverviewRequest`
@@ -2428,15 +2543,15 @@
             model = models.DescribeRealTimeTaskMetricOverviewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRealTimeTaskSpeed(self, request):
         """实时任务同步速度趋势
 
         :param request: Request instance for DescribeRealTimeTaskSpeed.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRealTimeTaskSpeedRequest`
@@ -2451,15 +2566,15 @@
             model = models.DescribeRealTimeTaskSpeedResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRelatedInstances(self, request):
         """查询任务实例的关联实例列表
 
         :param request: Request instance for DescribeRelatedInstances.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRelatedInstancesRequest`
@@ -2474,15 +2589,15 @@
             model = models.DescribeRelatedInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourceManagePathTrees(self, request):
         """获取资源管理目录树
 
         :param request: Request instance for DescribeResourceManagePathTrees.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeResourceManagePathTreesRequest`
@@ -2497,15 +2612,15 @@
             model = models.DescribeResourceManagePathTreesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRule(self, request):
         """查询规则详情
 
         :param request: Request instance for DescribeRule.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRuleRequest`
@@ -2520,15 +2635,15 @@
             model = models.DescribeRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuleDataSources(self, request):
         """查询质量规则数据源
 
         :param request: Request instance for DescribeRuleDataSources.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRuleDataSourcesRequest`
@@ -2543,15 +2658,15 @@
             model = models.DescribeRuleDataSourcesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuleDimStat(self, request):
         """数据质量概览页面触发维度分布统计接口
 
         :param request: Request instance for DescribeRuleDimStat.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRuleDimStatRequest`
@@ -2566,15 +2681,15 @@
             model = models.DescribeRuleDimStatResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuleExecDetail(self, request):
         """查询规则执行结果详情
 
         :param request: Request instance for DescribeRuleExecDetail.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRuleExecDetailRequest`
@@ -2589,15 +2704,15 @@
             model = models.DescribeRuleExecDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuleExecExportResult(self, request):
         """查询规则执行导出结果
 
         :param request: Request instance for DescribeRuleExecExportResult.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRuleExecExportResultRequest`
@@ -2612,15 +2727,15 @@
             model = models.DescribeRuleExecExportResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuleExecHistory(self, request):
         """查询规则执行历史， 最近30条
 
         :param request: Request instance for DescribeRuleExecHistory.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRuleExecHistoryRequest`
@@ -2635,15 +2750,15 @@
             model = models.DescribeRuleExecHistoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuleExecLog(self, request):
         """规则执行日志查询
 
         :param request: Request instance for DescribeRuleExecLog.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRuleExecLogRequest`
@@ -2658,15 +2773,15 @@
             model = models.DescribeRuleExecLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuleExecResults(self, request):
         """规则执行结果列表查询
 
         :param request: Request instance for DescribeRuleExecResults.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRuleExecResultsRequest`
@@ -2681,15 +2796,15 @@
             model = models.DescribeRuleExecResultsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuleExecResultsByPage(self, request):
         """分页查询规则执行结果列表
 
         :param request: Request instance for DescribeRuleExecResultsByPage.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRuleExecResultsByPageRequest`
@@ -2704,15 +2819,15 @@
             model = models.DescribeRuleExecResultsByPageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuleExecStat(self, request):
         """数据质量概览页面规则运行情况接口
 
         :param request: Request instance for DescribeRuleExecStat.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRuleExecStatRequest`
@@ -2727,15 +2842,15 @@
             model = models.DescribeRuleExecStatResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuleGroup(self, request):
         """查询规则组详情接口
 
         :param request: Request instance for DescribeRuleGroup.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRuleGroupRequest`
@@ -2750,15 +2865,15 @@
             model = models.DescribeRuleGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuleGroupExecResultsByPage(self, request):
         """规则组执行结果分页查询接口
 
         :param request: Request instance for DescribeRuleGroupExecResultsByPage.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRuleGroupExecResultsByPageRequest`
@@ -2773,15 +2888,15 @@
             model = models.DescribeRuleGroupExecResultsByPageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuleGroupExecResultsByPageWithoutAuth(self, request):
         """规则组执行结果分页查询接口不带鉴权
 
         :param request: Request instance for DescribeRuleGroupExecResultsByPageWithoutAuth.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRuleGroupExecResultsByPageWithoutAuthRequest`
@@ -2796,15 +2911,15 @@
             model = models.DescribeRuleGroupExecResultsByPageWithoutAuthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuleGroupSubscription(self, request):
         """查询规则组订阅信息
 
         :param request: Request instance for DescribeRuleGroupSubscription.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRuleGroupSubscriptionRequest`
@@ -2819,15 +2934,15 @@
             model = models.DescribeRuleGroupSubscriptionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuleGroupTable(self, request):
         """查询表绑定执行规则组信息
 
         :param request: Request instance for DescribeRuleGroupTable.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRuleGroupTableRequest`
@@ -2842,15 +2957,15 @@
             model = models.DescribeRuleGroupTableResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuleGroupsByPage(self, request):
         """【过滤条件】
         {表名称TableName,支持模糊匹配}       {表负责人TableOwnerName,支持模糊匹配}      {监控方式MonitorTypes，1.未配置 2.关联生产调度 3.离线周期检测,支持多选}  {订阅人ReceiverUin}
         【必要字段】
         {数据来源DatasourceId}
@@ -2868,15 +2983,15 @@
             model = models.DescribeRuleGroupsByPageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuleHistoryByPage(self, request):
         """过滤条件【必要字段】{ruleId}
 
         :param request: Request instance for DescribeRuleHistoryByPage.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRuleHistoryByPageRequest`
@@ -2891,15 +3006,15 @@
             model = models.DescribeRuleHistoryByPageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuleTablesByPage(self, request):
         """获取表列表
 
         :param request: Request instance for DescribeRuleTablesByPage.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRuleTablesByPageRequest`
@@ -2914,15 +3029,15 @@
             model = models.DescribeRuleTablesByPageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuleTemplate(self, request):
         """查询模板详情
 
         :param request: Request instance for DescribeRuleTemplate.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRuleTemplateRequest`
@@ -2937,15 +3052,15 @@
             model = models.DescribeRuleTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuleTemplates(self, request):
         """查询规则模版列表
 
         :param request: Request instance for DescribeRuleTemplates.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRuleTemplatesRequest`
@@ -2960,15 +3075,15 @@
             model = models.DescribeRuleTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuleTemplatesByPage(self, request):
         """过滤条件】 {模版名称Name,支持模糊匹配} {模版类型type，1.系统模版 2.自定义模版} {质量检测维度QualityDims, 1.准确性 2.唯一性 3.完整性 4.一致性 5.及时性 6.有效性} 【排序字段】 { 引用数排序类型CitationOrderType，根据引用数量排序 ASC DESC}
 
         :param request: Request instance for DescribeRuleTemplatesByPage.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRuleTemplatesByPageRequest`
@@ -2983,15 +3098,15 @@
             model = models.DescribeRuleTemplatesByPageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRules(self, request):
         """查询质量规则列表
 
         :param request: Request instance for DescribeRules.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRulesRequest`
@@ -3006,15 +3121,15 @@
             model = models.DescribeRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRulesByPage(self, request):
         """分页查询质量规则
 
         :param request: Request instance for DescribeRulesByPage.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeRulesByPageRequest`
@@ -3029,15 +3144,15 @@
             model = models.DescribeRulesByPageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStandardRuleDetailInfoList(self, request):
         """获取数据标准规则详情
 
         :param request: Request instance for DescribeStandardRuleDetailInfoList.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeStandardRuleDetailInfoListRequest`
@@ -3052,15 +3167,15 @@
             model = models.DescribeStandardRuleDetailInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStreamTaskLogList(self, request):
         """查询实时任务日志列表
 
         :param request: Request instance for DescribeStreamTaskLogList.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeStreamTaskLogListRequest`
@@ -3075,15 +3190,15 @@
             model = models.DescribeStreamTaskLogListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTableInfoList(self, request):
         """获取数据表信息
 
         :param request: Request instance for DescribeTableInfoList.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeTableInfoListRequest`
@@ -3098,15 +3213,15 @@
             model = models.DescribeTableInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTableLineage(self, request):
         """列出表血缘信息
 
         :param request: Request instance for DescribeTableLineage.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeTableLineageRequest`
@@ -3121,15 +3236,15 @@
             model = models.DescribeTableLineageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTableQualityDetails(self, request):
         """质量报告-查询表质量详情
 
         :param request: Request instance for DescribeTableQualityDetails.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeTableQualityDetailsRequest`
@@ -3144,15 +3259,15 @@
             model = models.DescribeTableQualityDetailsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTableSchemaInfo(self, request):
         """获取表schema信息
 
         :param request: Request instance for DescribeTableSchemaInfo.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeTableSchemaInfoRequest`
@@ -3167,15 +3282,15 @@
             model = models.DescribeTableSchemaInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTableScoreTrend(self, request):
         """查询表得分趋势
 
         :param request: Request instance for DescribeTableScoreTrend.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeTableScoreTrendRequest`
@@ -3190,15 +3305,15 @@
             model = models.DescribeTableScoreTrendResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskAlarmRegulations(self, request):
         """查询任务告警规则列表
 
         :param request: Request instance for DescribeTaskAlarmRegulations.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeTaskAlarmRegulationsRequest`
@@ -3213,15 +3328,15 @@
             model = models.DescribeTaskAlarmRegulationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskDetail(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         查询任务具体详情
 
         :param request: Request instance for DescribeTaskDetail.
@@ -3237,15 +3352,15 @@
             model = models.DescribeTaskDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskInstance(self, request):
         """离线任务实例详情
 
         :param request: Request instance for DescribeTaskInstance.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeTaskInstanceRequest`
@@ -3260,15 +3375,15 @@
             model = models.DescribeTaskInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskInstanceReportDetail(self, request):
         """离线任务实例统计明细
 
         :param request: Request instance for DescribeTaskInstanceReportDetail.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeTaskInstanceReportDetailRequest`
@@ -3283,15 +3398,15 @@
             model = models.DescribeTaskInstanceReportDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskInstances(self, request):
         """查询任务实例列表
 
         :param request: Request instance for DescribeTaskInstances.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeTaskInstancesRequest`
@@ -3306,15 +3421,15 @@
             model = models.DescribeTaskInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskLockStatus(self, request):
         """查看任务锁状态信息
 
         :param request: Request instance for DescribeTaskLockStatus.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeTaskLockStatusRequest`
@@ -3329,15 +3444,15 @@
             model = models.DescribeTaskLockStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskReport(self, request):
         """按起止日期统计离线任务的所有实例的运行指标总和
 
         :param request: Request instance for DescribeTaskReport.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeTaskReportRequest`
@@ -3352,15 +3467,15 @@
             model = models.DescribeTaskReportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskReportDetailList(self, request):
         """离线任务周期统计明细
 
         :param request: Request instance for DescribeTaskReportDetailList.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeTaskReportDetailListRequest`
@@ -3375,15 +3490,15 @@
             model = models.DescribeTaskReportDetailListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskScript(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         查询任务脚本
 
         :param request: Request instance for DescribeTaskScript.
@@ -3399,15 +3514,15 @@
             model = models.DescribeTaskScriptResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTasksByPage(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         根据工作流分页查询任务
 
         :param request: Request instance for DescribeTasksByPage.
@@ -3423,15 +3538,15 @@
             model = models.DescribeTasksByPageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTemplateDimCount(self, request):
         """查询规则模版维度分布情况
 
         :param request: Request instance for DescribeTemplateDimCount.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeTemplateDimCountRequest`
@@ -3446,15 +3561,15 @@
             model = models.DescribeTemplateDimCountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTemplateHistory(self, request):
         """查询规则模版操作记录
 
         :param request: Request instance for DescribeTemplateHistory.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeTemplateHistoryRequest`
@@ -3469,15 +3584,15 @@
             model = models.DescribeTemplateHistoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopTableStat(self, request):
         """数据质量概览页面表排行接口
 
         :param request: Request instance for DescribeTopTableStat.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeTopTableStatRequest`
@@ -3492,15 +3607,15 @@
             model = models.DescribeTopTableStatResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTrendStat(self, request):
         """数据质量概览页面趋势变化接口
 
         :param request: Request instance for DescribeTrendStat.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeTrendStatRequest`
@@ -3515,15 +3630,15 @@
             model = models.DescribeTrendStatResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DryRunDIOfflineTask(self, request):
         """调试运行集成任务
 
         :param request: Request instance for DryRunDIOfflineTask.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DryRunDIOfflineTaskRequest`
@@ -3538,15 +3653,15 @@
             model = models.DryRunDIOfflineTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ForceSucInstances(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         实例批量置成功
 
         :param request: Request instance for ForceSucInstances.
@@ -3562,15 +3677,15 @@
             model = models.ForceSucInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def FreezeTasks(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         批量冻结任务
 
         :param request: Request instance for FreezeTasks.
@@ -3586,15 +3701,15 @@
             model = models.FreezeTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def FreezeTasksByMultiWorkflow(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         基于多个工作流进行批量冻结任务操作
 
         :param request: Request instance for FreezeTasksByMultiWorkflow.
@@ -3610,15 +3725,15 @@
             model = models.FreezeTasksByMultiWorkflowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GenHiveTableDDLSql(self, request):
         """生成建hive表的sql
 
         :param request: Request instance for GenHiveTableDDLSql.
         :type request: :class:`tencentcloud.wedata.v20210820.models.GenHiveTableDDLSqlRequest`
@@ -3633,15 +3748,15 @@
             model = models.GenHiveTableDDLSqlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetIntegrationNodeColumnSchema(self, request):
         """提取数据集成节点字段Schema
 
         :param request: Request instance for GetIntegrationNodeColumnSchema.
         :type request: :class:`tencentcloud.wedata.v20210820.models.GetIntegrationNodeColumnSchemaRequest`
@@ -3656,15 +3771,15 @@
             model = models.GetIntegrationNodeColumnSchemaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetOfflineDIInstanceList(self, request):
         """获取离线任务实例列表(新)
 
         :param request: Request instance for GetOfflineDIInstanceList.
         :type request: :class:`tencentcloud.wedata.v20210820.models.GetOfflineDIInstanceListRequest`
@@ -3679,15 +3794,15 @@
             model = models.GetOfflineDIInstanceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetOfflineInstanceList(self, request):
         """获取离线任务实例
 
         :param request: Request instance for GetOfflineInstanceList.
         :type request: :class:`tencentcloud.wedata.v20210820.models.GetOfflineInstanceListRequest`
@@ -3702,15 +3817,15 @@
             model = models.GetOfflineInstanceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def KillInstances(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         实例批量终止操作
 
         :param request: Request instance for KillInstances.
@@ -3726,15 +3841,15 @@
             model = models.KillInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def LockIntegrationTask(self, request):
         """锁定集成任务
 
         :param request: Request instance for LockIntegrationTask.
         :type request: :class:`tencentcloud.wedata.v20210820.models.LockIntegrationTaskRequest`
@@ -3749,15 +3864,15 @@
             model = models.LockIntegrationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def MakeUpTasksNew(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         任务批量补录，调度状态任务才可以补录；
 
 
@@ -3775,15 +3890,15 @@
             model = models.MakeUpTasksNewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def MakeUpWorkflowNew(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         工作流下所有任务的补录
 
         :param request: Request instance for MakeUpWorkflowNew.
@@ -3799,15 +3914,15 @@
             model = models.MakeUpWorkflowNewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDataSource(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         修改数据源
 
         :param request: Request instance for ModifyDataSource.
@@ -3823,15 +3938,15 @@
             model = models.ModifyDataSourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDimensionWeight(self, request):
         """质量报告-修改维度权限
 
         :param request: Request instance for ModifyDimensionWeight.
         :type request: :class:`tencentcloud.wedata.v20210820.models.ModifyDimensionWeightRequest`
@@ -3846,15 +3961,15 @@
             model = models.ModifyDimensionWeightResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyExecStrategy(self, request):
         """更新规则组执行策略
 
         :param request: Request instance for ModifyExecStrategy.
         :type request: :class:`tencentcloud.wedata.v20210820.models.ModifyExecStrategyRequest`
@@ -3869,15 +3984,15 @@
             model = models.ModifyExecStrategyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyFolder(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         文件夹更新
 
         :param request: Request instance for ModifyFolder.
@@ -3893,15 +4008,15 @@
             model = models.ModifyFolderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyIntegrationNode(self, request):
         """更新集成节点
 
         :param request: Request instance for ModifyIntegrationNode.
         :type request: :class:`tencentcloud.wedata.v20210820.models.ModifyIntegrationNodeRequest`
@@ -3916,15 +4031,15 @@
             model = models.ModifyIntegrationNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyIntegrationTask(self, request):
         """更新集成任务
 
         :param request: Request instance for ModifyIntegrationTask.
         :type request: :class:`tencentcloud.wedata.v20210820.models.ModifyIntegrationTaskRequest`
@@ -3939,15 +4054,15 @@
             model = models.ModifyIntegrationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyMonitorStatus(self, request):
         """更新监控状态
 
         :param request: Request instance for ModifyMonitorStatus.
         :type request: :class:`tencentcloud.wedata.v20210820.models.ModifyMonitorStatusRequest`
@@ -3962,15 +4077,15 @@
             model = models.ModifyMonitorStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRule(self, request):
         """更新质量规则接口
 
         :param request: Request instance for ModifyRule.
         :type request: :class:`tencentcloud.wedata.v20210820.models.ModifyRuleRequest`
@@ -3985,15 +4100,15 @@
             model = models.ModifyRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRuleGroupSubscription(self, request):
         """更新规则组订阅信息
 
         :param request: Request instance for ModifyRuleGroupSubscription.
         :type request: :class:`tencentcloud.wedata.v20210820.models.ModifyRuleGroupSubscriptionRequest`
@@ -4008,15 +4123,15 @@
             model = models.ModifyRuleGroupSubscriptionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRuleTemplate(self, request):
         """编辑规则模版
 
         :param request: Request instance for ModifyRuleTemplate.
         :type request: :class:`tencentcloud.wedata.v20210820.models.ModifyRuleTemplateRequest`
@@ -4031,15 +4146,15 @@
             model = models.ModifyRuleTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTaskAlarmRegular(self, request):
         """修改任务告警规则
 
         :param request: Request instance for ModifyTaskAlarmRegular.
         :type request: :class:`tencentcloud.wedata.v20210820.models.ModifyTaskAlarmRegularRequest`
@@ -4054,15 +4169,15 @@
             model = models.ModifyTaskAlarmRegularResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTaskInfo(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         更新任务
 
         :param request: Request instance for ModifyTaskInfo.
@@ -4078,15 +4193,15 @@
             model = models.ModifyTaskInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTaskLinks(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         添加父任务依赖
 
         :param request: Request instance for ModifyTaskLinks.
@@ -4102,15 +4217,15 @@
             model = models.ModifyTaskLinksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTaskName(self, request):
         """重命名任务（任务编辑）
 
         :param request: Request instance for ModifyTaskName.
         :type request: :class:`tencentcloud.wedata.v20210820.models.ModifyTaskNameRequest`
@@ -4125,15 +4240,15 @@
             model = models.ModifyTaskNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTaskScript(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         修改任务脚本
 
         :param request: Request instance for ModifyTaskScript.
@@ -4149,15 +4264,15 @@
             model = models.ModifyTaskScriptResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyWorkflowInfo(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         更新工作流
 
         :param request: Request instance for ModifyWorkflowInfo.
@@ -4173,15 +4288,15 @@
             model = models.ModifyWorkflowInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyWorkflowSchedule(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         更新工作流调度
 
         :param request: Request instance for ModifyWorkflowSchedule.
@@ -4197,15 +4312,15 @@
             model = models.ModifyWorkflowScheduleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RegisterEvent(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         注册事件
 
         :param request: Request instance for RegisterEvent.
@@ -4221,15 +4336,15 @@
             model = models.RegisterEventResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RegisterEventListener(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         注册事件监听器
 
         :param request: Request instance for RegisterEventListener.
@@ -4245,15 +4360,38 @@
             model = models.RegisterEventListenerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def RemoveWorkflowDs(self, request):
+        """删除编排空间工作流
+
+        :param request: Request instance for RemoveWorkflowDs.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.RemoveWorkflowDsRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.RemoveWorkflowDsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("RemoveWorkflowDs", params, headers=headers)
+            response = json.loads(body)
+            model = models.RemoveWorkflowDsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RerunInstances(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         实例批量重跑
 
         :param request: Request instance for RerunInstances.
@@ -4269,15 +4407,15 @@
             model = models.RerunInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RestartInLongAgent(self, request):
         """重启采集器
 
         :param request: Request instance for RestartInLongAgent.
         :type request: :class:`tencentcloud.wedata.v20210820.models.RestartInLongAgentRequest`
@@ -4292,15 +4430,15 @@
             model = models.RestartInLongAgentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResumeIntegrationTask(self, request):
         """继续集成任务
 
         :param request: Request instance for ResumeIntegrationTask.
         :type request: :class:`tencentcloud.wedata.v20210820.models.ResumeIntegrationTaskRequest`
@@ -4315,15 +4453,15 @@
             model = models.ResumeIntegrationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RobAndLockIntegrationTask(self, request):
         """抢占锁定集成任务
 
         :param request: Request instance for RobAndLockIntegrationTask.
         :type request: :class:`tencentcloud.wedata.v20210820.models.RobAndLockIntegrationTaskRequest`
@@ -4338,15 +4476,15 @@
             model = models.RobAndLockIntegrationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RunTask(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         运行任务
 
         :param request: Request instance for RunTask.
@@ -4362,15 +4500,15 @@
             model = models.RunTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SaveCustomFunction(self, request):
         """保存用户自定义函数
 
         :param request: Request instance for SaveCustomFunction.
         :type request: :class:`tencentcloud.wedata.v20210820.models.SaveCustomFunctionRequest`
@@ -4385,15 +4523,15 @@
             model = models.SaveCustomFunctionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetTaskAlarmNew(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         设置任务告警，新建/更新告警信息（最新）
 
         :param request: Request instance for SetTaskAlarmNew.
@@ -4409,15 +4547,15 @@
             model = models.SetTaskAlarmNewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartIntegrationTask(self, request):
         """启动集成任务
 
         :param request: Request instance for StartIntegrationTask.
         :type request: :class:`tencentcloud.wedata.v20210820.models.StartIntegrationTaskRequest`
@@ -4432,15 +4570,15 @@
             model = models.StartIntegrationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopIntegrationTask(self, request):
         """停止集成任务
 
         :param request: Request instance for StopIntegrationTask.
         :type request: :class:`tencentcloud.wedata.v20210820.models.StopIntegrationTaskRequest`
@@ -4455,15 +4593,15 @@
             model = models.StopIntegrationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SubmitCustomFunction(self, request):
         """提交自定义函数
 
         :param request: Request instance for SubmitCustomFunction.
         :type request: :class:`tencentcloud.wedata.v20210820.models.SubmitCustomFunctionRequest`
@@ -4478,15 +4616,38 @@
             model = models.SubmitCustomFunctionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def SubmitSqlTask(self, request):
+        """即席分析提交SQL任务
+
+        :param request: Request instance for SubmitSqlTask.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.SubmitSqlTaskRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.SubmitSqlTaskResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("SubmitSqlTask", params, headers=headers)
+            response = json.loads(body)
+            model = models.SubmitSqlTaskResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SubmitTask(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         提交任务
 
         :param request: Request instance for SubmitTask.
@@ -4502,15 +4663,38 @@
             model = models.SubmitTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def SubmitTaskTestRun(self, request):
+        """无
+
+        :param request: Request instance for SubmitTaskTestRun.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.SubmitTaskTestRunRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.SubmitTaskTestRunResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("SubmitTaskTestRun", params, headers=headers)
+            response = json.loads(body)
+            model = models.SubmitTaskTestRunResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SubmitWorkflow(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         提交工作流
 
         :param request: Request instance for SubmitWorkflow.
@@ -4526,15 +4710,15 @@
             model = models.SubmitWorkflowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SuspendIntegrationTask(self, request):
         """暂停集成任务
 
         :param request: Request instance for SuspendIntegrationTask.
         :type request: :class:`tencentcloud.wedata.v20210820.models.SuspendIntegrationTaskRequest`
@@ -4549,15 +4733,15 @@
             model = models.SuspendIntegrationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TaskLog(self, request):
         """查询Inlong manager日志
 
         :param request: Request instance for TaskLog.
         :type request: :class:`tencentcloud.wedata.v20210820.models.TaskLogRequest`
@@ -4572,15 +4756,15 @@
             model = models.TaskLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TriggerEvent(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         触发事件
 
         :param request: Request instance for TriggerEvent.
@@ -4596,15 +4780,15 @@
             model = models.TriggerEventResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnlockIntegrationTask(self, request):
         """解锁集成任务
 
         :param request: Request instance for UnlockIntegrationTask.
         :type request: :class:`tencentcloud.wedata.v20210820.models.UnlockIntegrationTaskRequest`
@@ -4619,15 +4803,15 @@
             model = models.UnlockIntegrationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateInLongAgent(self, request):
         """更新采集器
 
         :param request: Request instance for UpdateInLongAgent.
         :type request: :class:`tencentcloud.wedata.v20210820.models.UpdateInLongAgentRequest`
@@ -4642,15 +4826,15 @@
             model = models.UpdateInLongAgentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UploadContent(self, request):
         """保存任务信息
 
         :param request: Request instance for UploadContent.
         :type request: :class:`tencentcloud.wedata.v20210820.models.UploadContentRequest`
@@ -4665,8 +4849,8 @@
             model = models.UploadContentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-wedata-3.0.938/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wedata
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Wedata SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.937/README.rst` & `tencentcloud-sdk-python-wedata-3.0.938/README.rst`

 * *Files identical despite different names*

