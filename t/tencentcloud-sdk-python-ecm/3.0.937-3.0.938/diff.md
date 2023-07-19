# Comparing `tmp/tencentcloud-sdk-python-ecm-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-ecm-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ecm-3.0.937.tar", last modified: Tue Jul 18 00:23:23 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ecm-3.0.938.tar", last modified: Wed Jul 19 00:38:36 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ecm-3.0.937.tar` & `tencentcloud-sdk-python-ecm-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:23.000000 tencentcloud-sdk-python-ecm-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:23:23.000000 tencentcloud-sdk-python-ecm-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:23.000000 tencentcloud-sdk-python-ecm-3.0.937/tencentcloud_sdk_python_ecm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:23:23.000000 tencentcloud-sdk-python-ecm-3.0.937/tencentcloud_sdk_python_ecm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:23:23.000000 tencentcloud-sdk-python-ecm-3.0.937/tencentcloud_sdk_python_ecm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:23:23.000000 tencentcloud-sdk-python-ecm-3.0.937/tencentcloud_sdk_python_ecm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:23:23.000000 tencentcloud-sdk-python-ecm-3.0.937/tencentcloud_sdk_python_ecm.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:23.000000 tencentcloud-sdk-python-ecm-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:23:23.000000 tencentcloud-sdk-python-ecm-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:23.000000 tencentcloud-sdk-python-ecm-3.0.937/tencentcloud/ecm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:23.000000 tencentcloud-sdk-python-ecm-3.0.937/tencentcloud/ecm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:23.000000 tencentcloud-sdk-python-ecm-3.0.937/tencentcloud/ecm/v20190719/
--rw-r--r--   0 root         (0) root         (0)   135627 2023-07-18 00:23:23.000000 tencentcloud-sdk-python-ecm-3.0.937/tencentcloud/ecm/v20190719/ecm_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:23.000000 tencentcloud-sdk-python-ecm-3.0.937/tencentcloud/ecm/v20190719/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23498 2023-07-18 00:23:23.000000 tencentcloud-sdk-python-ecm-3.0.937/tencentcloud/ecm/v20190719/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   731878 2023-07-18 00:23:23.000000 tencentcloud-sdk-python-ecm-3.0.937/tencentcloud/ecm/v20190719/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:23:23.000000 tencentcloud-sdk-python-ecm-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:23:23.000000 tencentcloud-sdk-python-ecm-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:23:23.000000 tencentcloud-sdk-python-ecm-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:36.000000 tencentcloud-sdk-python-ecm-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:38:36.000000 tencentcloud-sdk-python-ecm-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:36.000000 tencentcloud-sdk-python-ecm-3.0.938/tencentcloud_sdk_python_ecm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:38:36.000000 tencentcloud-sdk-python-ecm-3.0.938/tencentcloud_sdk_python_ecm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:38:36.000000 tencentcloud-sdk-python-ecm-3.0.938/tencentcloud_sdk_python_ecm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:38:36.000000 tencentcloud-sdk-python-ecm-3.0.938/tencentcloud_sdk_python_ecm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:38:36.000000 tencentcloud-sdk-python-ecm-3.0.938/tencentcloud_sdk_python_ecm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:36.000000 tencentcloud-sdk-python-ecm-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:38:36.000000 tencentcloud-sdk-python-ecm-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:36.000000 tencentcloud-sdk-python-ecm-3.0.938/tencentcloud/ecm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:38:36.000000 tencentcloud-sdk-python-ecm-3.0.938/tencentcloud/ecm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:36.000000 tencentcloud-sdk-python-ecm-3.0.938/tencentcloud/ecm/v20190719/
+-rw-r--r--   0 root         (0) root         (0)   136183 2023-07-19 00:38:36.000000 tencentcloud-sdk-python-ecm-3.0.938/tencentcloud/ecm/v20190719/ecm_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:38:36.000000 tencentcloud-sdk-python-ecm-3.0.938/tencentcloud/ecm/v20190719/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23498 2023-07-19 00:38:36.000000 tencentcloud-sdk-python-ecm-3.0.938/tencentcloud/ecm/v20190719/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   731878 2023-07-19 00:38:36.000000 tencentcloud-sdk-python-ecm-3.0.938/tencentcloud/ecm/v20190719/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:38:36.000000 tencentcloud-sdk-python-ecm-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:38:36.000000 tencentcloud-sdk-python-ecm-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:38:36.000000 tencentcloud-sdk-python-ecm-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-ecm-3.0.937/setup.py` & `tencentcloud-sdk-python-ecm-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecm-3.0.937/tencentcloud_sdk_python_ecm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ecm-3.0.938/tencentcloud_sdk_python_ecm.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ecm
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ecm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ecm-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ecm-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ecm-3.0.937/tencentcloud/ecm/v20190719/ecm_client.py` & `tencentcloud-sdk-python-ecm-3.0.938/tencentcloud/ecm/v20190719/ecm_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AllocateAddressesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AllocateIpv6AddressesBandwidth(self, request):
         """本接口用于给IPv6地址分配公网带宽
 
         :param request: Request instance for AllocateIpv6AddressesBandwidth.
         :type request: :class:`tencentcloud.ecm.v20190719.models.AllocateIpv6AddressesBandwidthRequest`
@@ -65,15 +65,15 @@
             model = models.AllocateIpv6AddressesBandwidthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssignIpv6Addresses(self, request):
         """本接口（AssignIpv6Addresses）用于弹性网卡申请IPv6地址。
 
         :param request: Request instance for AssignIpv6Addresses.
         :type request: :class:`tencentcloud.ecm.v20190719.models.AssignIpv6AddressesRequest`
@@ -88,15 +88,15 @@
             model = models.AssignIpv6AddressesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssignIpv6CidrBlock(self, request):
         """本接口（AssignIpv6CidrBlock）用于分配IPv6网段。
 
         使用本接口前，您需要已有VPC实例，如果没有可通过接口CreateVpc创建。
 
@@ -113,15 +113,15 @@
             model = models.AssignIpv6CidrBlockResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssignIpv6CidrBlocks(self, request):
         """本接口（AssignIpv6CidrBlocks）用于分配IPv6网段。
 
         使用本接口前，您需要已有VPC实例，如果没有可通过接口CreateVpc创建。
         每个VPC 可以同时支持运营商网络('CMCC'-中国移动, 'CTCC'-中国电信, 'CUCC'-中国联调)。本接口可以同时申请不同类型的IPv6网段
@@ -139,15 +139,15 @@
             model = models.AssignIpv6CidrBlocksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssignIpv6SubnetCidrBlock(self, request):
         """本接口（AssignIpv6SubnetCidrBlock）用于分配IPv6子网段。
 
         给子网分配 IPv6 网段，要求子网所属 VPC 已获得 IPv6 网段。如果尚未分配，请先通过接口 AssignIpv6CidrBlock 给子网所属 VPC 分配一个 IPv6 网段。否则无法分配 IPv6 子网段。
         每个子网只能分配一个IPv6网段。
@@ -165,15 +165,15 @@
             model = models.AssignIpv6SubnetCidrBlockResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssignPrivateIpAddresses(self, request):
         """弹性网卡申请内网 IP
 
         :param request: Request instance for AssignPrivateIpAddresses.
         :type request: :class:`tencentcloud.ecm.v20190719.models.AssignPrivateIpAddressesRequest`
@@ -188,15 +188,15 @@
             model = models.AssignPrivateIpAddressesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssociateAddress(self, request):
         """将弹性公网IP（简称 EIP）绑定到实例或弹性网卡的指定内网 IP 上。
         将 EIP 绑定到实例（ECM）上，其本质是将 EIP 绑定到实例上主网卡的主内网 IP 上。
         将 EIP 绑定到指定网卡的内网 IP上，内网IP已经绑定了EIP或普通公网IP，则反馈失败。必须先解绑该 EIP，才能再绑定新的。
         只有状态为 UNBIND 的 EIP 才能够绑定内网IP。
@@ -214,15 +214,15 @@
             model = models.AssociateAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssociateSecurityGroups(self, request):
         """绑定安全组
 
         :param request: Request instance for AssociateSecurityGroups.
         :type request: :class:`tencentcloud.ecm.v20190719.models.AssociateSecurityGroupsRequest`
@@ -237,15 +237,15 @@
             model = models.AssociateSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AttachDisks(self, request):
         """本接口（AttachDisks）用于挂载云硬盘。
 
         * 支持批量操作，将多块云盘挂载到同一云主机。如果多个云盘中存在不允许挂载的云盘，则操作不执行，返回特定的错误码。
         * 本接口为异步接口，当挂载云盘的请求成功返回时，表示后台已发起挂载云盘的操作，可通过接口[DescribeDisks](/document/product/362/16315)来查询对应云盘的状态，如果云盘的状态由“ATTACHING”变为“ATTACHED”，则为挂载成功。
@@ -263,15 +263,15 @@
             model = models.AttachDisksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AttachNetworkInterface(self, request):
         """弹性网卡绑定云主机
 
         :param request: Request instance for AttachNetworkInterface.
         :type request: :class:`tencentcloud.ecm.v20190719.models.AttachNetworkInterfaceRequest`
@@ -286,15 +286,15 @@
             model = models.AttachNetworkInterfaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchDeregisterTargets(self, request):
         """批量解绑后端服务。
 
         :param request: Request instance for BatchDeregisterTargets.
         :type request: :class:`tencentcloud.ecm.v20190719.models.BatchDeregisterTargetsRequest`
@@ -309,15 +309,15 @@
             model = models.BatchDeregisterTargetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchModifyTargetWeight(self, request):
         """批量修改监听器绑定的后端机器的转发权重。
 
         :param request: Request instance for BatchModifyTargetWeight.
         :type request: :class:`tencentcloud.ecm.v20190719.models.BatchModifyTargetWeightRequest`
@@ -332,15 +332,15 @@
             model = models.BatchModifyTargetWeightResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchRegisterTargets(self, request):
         """批量绑定后端目标。
 
         :param request: Request instance for BatchRegisterTargets.
         :type request: :class:`tencentcloud.ecm.v20190719.models.BatchRegisterTargetsRequest`
@@ -355,15 +355,15 @@
             model = models.BatchRegisterTargetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDisks(self, request):
         """本接口（CreateDisks）用于创建云硬盘。
 
         * 预付费云盘的购买会预先扣除本次云盘购买所需金额，在调用本接口前请确保账户余额充足。
         * 本接口支持传入数据盘快照来创建云盘，实现将快照数据复制到新购云盘上。
@@ -382,15 +382,15 @@
             model = models.CreateDisksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateHaVip(self, request):
         """本接口（CreateHaVip）用于创建高可用虚拟IP（HAVIP）
 
         :param request: Request instance for CreateHaVip.
         :type request: :class:`tencentcloud.ecm.v20190719.models.CreateHaVipRequest`
@@ -405,15 +405,15 @@
             model = models.CreateHaVipResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateImage(self, request):
         """本接口(CreateImage)用于将实例的系统盘制作为新镜像，创建后的镜像可以用于创建实例。
 
         :param request: Request instance for CreateImage.
         :type request: :class:`tencentcloud.ecm.v20190719.models.CreateImageRequest`
@@ -428,15 +428,15 @@
             model = models.CreateImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateKeyPair(self, request):
         """用于创建一个 OpenSSH RSA 密钥对，可以用于登录 Linux 实例。
 
         :param request: Request instance for CreateKeyPair.
         :type request: :class:`tencentcloud.ecm.v20190719.models.CreateKeyPairRequest`
@@ -451,15 +451,15 @@
             model = models.CreateKeyPairResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateListener(self, request):
         """创建负载均衡监听器。
 
         :param request: Request instance for CreateListener.
         :type request: :class:`tencentcloud.ecm.v20190719.models.CreateListenerRequest`
@@ -474,15 +474,15 @@
             model = models.CreateListenerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLoadBalancer(self, request):
         """购买负载均衡实例。
 
         :param request: Request instance for CreateLoadBalancer.
         :type request: :class:`tencentcloud.ecm.v20190719.models.CreateLoadBalancerRequest`
@@ -497,15 +497,15 @@
             model = models.CreateLoadBalancerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateModule(self, request):
         """创建模块
 
         :param request: Request instance for CreateModule.
         :type request: :class:`tencentcloud.ecm.v20190719.models.CreateModuleRequest`
@@ -520,15 +520,15 @@
             model = models.CreateModuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNetworkInterface(self, request):
         """创建弹性网卡
 
         :param request: Request instance for CreateNetworkInterface.
         :type request: :class:`tencentcloud.ecm.v20190719.models.CreateNetworkInterfaceRequest`
@@ -543,15 +543,15 @@
             model = models.CreateNetworkInterfaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRouteTable(self, request):
         """创建了VPC后，系统会创建一个默认路由表，所有新建的子网都会关联到默认路由表。默认情况下您可以直接使用默认路由表来管理您的路由策略。当您的路由策略较多时，您可以调用创建路由表接口创建更多路由表管理您的路由策略。
 
         :param request: Request instance for CreateRouteTable.
         :type request: :class:`tencentcloud.ecm.v20190719.models.CreateRouteTableRequest`
@@ -566,15 +566,15 @@
             model = models.CreateRouteTableResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRoutes(self, request):
         """创建路由策略
 
         :param request: Request instance for CreateRoutes.
         :type request: :class:`tencentcloud.ecm.v20190719.models.CreateRoutesRequest`
@@ -589,15 +589,15 @@
             model = models.CreateRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSecurityGroup(self, request):
         """创建安全组
 
         :param request: Request instance for CreateSecurityGroup.
         :type request: :class:`tencentcloud.ecm.v20190719.models.CreateSecurityGroupRequest`
@@ -612,15 +612,15 @@
             model = models.CreateSecurityGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSecurityGroupPolicies(self, request):
         """<p>本接口（CreateSecurityGroupPolicies）用于创建安全组规则（SecurityGroupPolicy）。</p>
         <p>在 SecurityGroupPolicySet 参数中：</p>
         <ul>
         <li>Version 安全组规则版本号，用户每次更新安全规则版本会自动加1，防止您更新的路由规则已过期，不填不考虑冲突。</li>
@@ -648,15 +648,15 @@
             model = models.CreateSecurityGroupPoliciesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSubnet(self, request):
         """创建子网，若创建成功，则此子网会成为此可用区的默认子网。
 
         :param request: Request instance for CreateSubnet.
         :type request: :class:`tencentcloud.ecm.v20190719.models.CreateSubnetRequest`
@@ -671,15 +671,15 @@
             model = models.CreateSubnetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVpc(self, request):
         """创建私有网络
 
         :param request: Request instance for CreateVpc.
         :type request: :class:`tencentcloud.ecm.v20190719.models.CreateVpcRequest`
@@ -694,15 +694,15 @@
             model = models.CreateVpcResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteHaVip(self, request):
         """用于删除高可用虚拟IP（HAVIP）
 
         :param request: Request instance for DeleteHaVip.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DeleteHaVipRequest`
@@ -717,15 +717,15 @@
             model = models.DeleteHaVipResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteImage(self, request):
         """删除镜像
 
         :param request: Request instance for DeleteImage.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DeleteImageRequest`
@@ -740,15 +740,15 @@
             model = models.DeleteImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteListener(self, request):
         """删除负载均衡监听器。
 
         :param request: Request instance for DeleteListener.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DeleteListenerRequest`
@@ -763,15 +763,15 @@
             model = models.DeleteListenerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLoadBalancer(self, request):
         """删除负载均衡实例。
 
         :param request: Request instance for DeleteLoadBalancer.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DeleteLoadBalancerRequest`
@@ -786,15 +786,15 @@
             model = models.DeleteLoadBalancerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLoadBalancerListeners(self, request):
         """删除负载均衡多个监听器
 
         :param request: Request instance for DeleteLoadBalancerListeners.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DeleteLoadBalancerListenersRequest`
@@ -809,15 +809,15 @@
             model = models.DeleteLoadBalancerListenersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteModule(self, request):
         """删除业务模块
 
         :param request: Request instance for DeleteModule.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DeleteModuleRequest`
@@ -832,15 +832,15 @@
             model = models.DeleteModuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteNetworkInterface(self, request):
         """删除弹性网卡
 
         :param request: Request instance for DeleteNetworkInterface.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DeleteNetworkInterfaceRequest`
@@ -855,15 +855,15 @@
             model = models.DeleteNetworkInterfaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRouteTable(self, request):
         """删除路由表
 
         :param request: Request instance for DeleteRouteTable.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DeleteRouteTableRequest`
@@ -878,15 +878,15 @@
             model = models.DeleteRouteTableResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRoutes(self, request):
         """对某个路由表批量删除路由策略
 
         :param request: Request instance for DeleteRoutes.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DeleteRoutesRequest`
@@ -901,15 +901,15 @@
             model = models.DeleteRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSecurityGroup(self, request):
         """只有当前账号下的安全组允许被删除。
         安全组实例ID如果在其他安全组的规则中被引用，则无法直接删除。这种情况下，需要先进行规则修改，再删除安全组。
         删除的安全组无法再找回，请谨慎调用。
 
@@ -926,15 +926,15 @@
             model = models.DeleteSecurityGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSecurityGroupPolicies(self, request):
         """SecurityGroupPolicySet.Version 用于指定要操作的安全组的版本。传入 Version 版本号若不等于当前安全组的最新版本，将返回失败；若不传 Version 则直接删除指定PolicyIndex的规则。
 
         :param request: Request instance for DeleteSecurityGroupPolicies.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DeleteSecurityGroupPoliciesRequest`
@@ -949,15 +949,15 @@
             model = models.DeleteSecurityGroupPoliciesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSnapshots(self, request):
         """本接口（DeleteSnapshots）用于删除快照。
 
         * 快照必须处于NORMAL状态，快照状态可以通过[DescribeSnapshots](/document/product/362/15647)接口查询，见输出参数中SnapshotState字段解释。
         * 支持批量操作。如果多个快照存在无法删除的快照，则操作不执行，以返回特定的错误码返回。
@@ -975,15 +975,15 @@
             model = models.DeleteSnapshotsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSubnet(self, request):
         """删除子网，若子网为可用区下的默认子网，则默认子网会回退到系统自动创建的默认子网，非用户最新创建的子网。若默认子网不满足需求，可调用设置默认子网接口设置。
 
         :param request: Request instance for DeleteSubnet.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DeleteSubnetRequest`
@@ -998,15 +998,15 @@
             model = models.DeleteSubnetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteVpc(self, request):
         """删除私有网络
 
         :param request: Request instance for DeleteVpc.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DeleteVpcRequest`
@@ -1021,15 +1021,15 @@
             model = models.DeleteVpcResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAddressQuota(self, request):
         """查询您账户的弹性公网IP（简称 EIP）在当前地域的配额信息
 
         :param request: Request instance for DescribeAddressQuota.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeAddressQuotaRequest`
@@ -1044,15 +1044,15 @@
             model = models.DescribeAddressQuotaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAddresses(self, request):
         """查询弹性公网IP列表
 
         :param request: Request instance for DescribeAddresses.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeAddressesRequest`
@@ -1067,15 +1067,15 @@
             model = models.DescribeAddressesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBaseOverview(self, request):
         """获取概览页统计的基本数据
 
         :param request: Request instance for DescribeBaseOverview.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeBaseOverviewRequest`
@@ -1090,15 +1090,15 @@
             model = models.DescribeBaseOverviewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConfig(self, request):
         """获取带宽硬盘等数据的限制
 
         :param request: Request instance for DescribeConfig.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeConfigRequest`
@@ -1113,15 +1113,15 @@
             model = models.DescribeConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCustomImageTask(self, request):
         """查询导入镜像任务
 
         :param request: Request instance for DescribeCustomImageTask.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeCustomImageTaskRequest`
@@ -1136,15 +1136,15 @@
             model = models.DescribeCustomImageTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDefaultSubnet(self, request):
         """查询可用区的默认子网
 
         :param request: Request instance for DescribeDefaultSubnet.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeDefaultSubnetRequest`
@@ -1159,15 +1159,15 @@
             model = models.DescribeDefaultSubnetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDisks(self, request):
         """本接口（DescribeDisks）用于查询云硬盘列表。
 
         * 可以根据云硬盘ID、云硬盘类型或者云硬盘状态等信息来查询云硬盘的详细信息，不同条件之间为与(AND)的关系，过滤信息详细请见过滤器`Filter`。
         * 如果参数为空，返回当前用户一定数量（`Limit`所指定的数量，默认为20）的云硬盘列表。
@@ -1185,15 +1185,15 @@
             model = models.DescribeDisksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHaVips(self, request):
         """用于查询高可用虚拟IP（HAVIP）列表。
 
         :param request: Request instance for DescribeHaVips.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeHaVipsRequest`
@@ -1208,15 +1208,15 @@
             model = models.DescribeHaVipsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImage(self, request):
         """展示镜像列表
 
         :param request: Request instance for DescribeImage.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeImageRequest`
@@ -1231,15 +1231,15 @@
             model = models.DescribeImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImportImageOs(self, request):
         """查询外部导入镜像支持的OS列表
 
         :param request: Request instance for DescribeImportImageOs.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeImportImageOsRequest`
@@ -1254,15 +1254,15 @@
             model = models.DescribeImportImageOsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceTypeConfig(self, request):
         """获取机型配置列表
 
         :param request: Request instance for DescribeInstanceTypeConfig.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeInstanceTypeConfigRequest`
@@ -1277,15 +1277,15 @@
             model = models.DescribeInstanceTypeConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceVncUrl(self, request):
         """查询实例管理终端地址
 
         :param request: Request instance for DescribeInstanceVncUrl.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeInstanceVncUrlRequest`
@@ -1300,15 +1300,15 @@
             model = models.DescribeInstanceVncUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstances(self, request):
         """获取实例的相关信息。
 
         :param request: Request instance for DescribeInstances.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeInstancesRequest`
@@ -1323,15 +1323,15 @@
             model = models.DescribeInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstancesDeniedActions(self, request):
         """通过实例id获取当前禁止的操作
 
         :param request: Request instance for DescribeInstancesDeniedActions.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeInstancesDeniedActionsRequest`
@@ -1346,15 +1346,15 @@
             model = models.DescribeInstancesDeniedActionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeListeners(self, request):
         """查询负载均衡的监听器列表。
 
         :param request: Request instance for DescribeListeners.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeListenersRequest`
@@ -1369,15 +1369,15 @@
             model = models.DescribeListenersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLoadBalanceTaskStatus(self, request):
         """查询负载均衡相关的任务状态
 
         :param request: Request instance for DescribeLoadBalanceTaskStatus.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeLoadBalanceTaskStatusRequest`
@@ -1392,15 +1392,15 @@
             model = models.DescribeLoadBalanceTaskStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLoadBalancers(self, request):
         """查询负载均衡实例列表。
 
         :param request: Request instance for DescribeLoadBalancers.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeLoadBalancersRequest`
@@ -1415,15 +1415,15 @@
             model = models.DescribeLoadBalancersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeModule(self, request):
         """获取模块列表
 
         :param request: Request instance for DescribeModule.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeModuleRequest`
@@ -1438,15 +1438,15 @@
             model = models.DescribeModuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeModuleDetail(self, request):
         """展示模块详细信息
 
         :param request: Request instance for DescribeModuleDetail.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeModuleDetailRequest`
@@ -1461,15 +1461,15 @@
             model = models.DescribeModuleDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMonthPeakNetwork(self, request):
         """获取客户节点上的出入带宽月峰和计费带宽信息
 
         :param request: Request instance for DescribeMonthPeakNetwork.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeMonthPeakNetworkRequest`
@@ -1484,15 +1484,15 @@
             model = models.DescribeMonthPeakNetworkResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNetworkInterfaces(self, request):
         """查询弹性网卡列表
 
         :param request: Request instance for DescribeNetworkInterfaces.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeNetworkInterfacesRequest`
@@ -1507,15 +1507,15 @@
             model = models.DescribeNetworkInterfacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNode(self, request):
         """获取节点列表
 
         :param request: Request instance for DescribeNode.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeNodeRequest`
@@ -1530,15 +1530,15 @@
             model = models.DescribeNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePackingQuotaGroup(self, request):
         """使用本接口获取某种机型在某些区域的装箱配额（当使用虚拟机型时，返回的是一组相互关联的装箱配额）。
 
         :param request: Request instance for DescribePackingQuotaGroup.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribePackingQuotaGroupRequest`
@@ -1553,15 +1553,15 @@
             model = models.DescribePackingQuotaGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePeakBaseOverview(self, request):
         """CPU 内存 硬盘等基础信息峰值数据
 
         :param request: Request instance for DescribePeakBaseOverview.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribePeakBaseOverviewRequest`
@@ -1576,15 +1576,15 @@
             model = models.DescribePeakBaseOverviewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePeakNetworkOverview(self, request):
         """获取网络峰值数据
 
         :param request: Request instance for DescribePeakNetworkOverview.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribePeakNetworkOverviewRequest`
@@ -1599,15 +1599,15 @@
             model = models.DescribePeakNetworkOverviewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePriceRunInstance(self, request):
         """查询实例价格
 
         :param request: Request instance for DescribePriceRunInstance.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribePriceRunInstanceRequest`
@@ -1622,15 +1622,15 @@
             model = models.DescribePriceRunInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRegionIpv6Addresses(self, request):
         """该接口（DescribeRegionIpv6Addresses）用于查询ECM地域之下的IPV6地址信息。
 
         :param request: Request instance for DescribeRegionIpv6Addresses.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeRegionIpv6AddressesRequest`
@@ -1645,15 +1645,15 @@
             model = models.DescribeRegionIpv6AddressesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRouteConflicts(self, request):
         """查询自定义路由策略与云联网路由策略冲突列表
 
         :param request: Request instance for DescribeRouteConflicts.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeRouteConflictsRequest`
@@ -1668,15 +1668,15 @@
             model = models.DescribeRouteConflictsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRouteTables(self, request):
         """查询路由表对象列表
 
         :param request: Request instance for DescribeRouteTables.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeRouteTablesRequest`
@@ -1691,15 +1691,15 @@
             model = models.DescribeRouteTablesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecurityGroupAssociationStatistics(self, request):
         """查询安全组关联实例统计
 
         :param request: Request instance for DescribeSecurityGroupAssociationStatistics.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeSecurityGroupAssociationStatisticsRequest`
@@ -1714,15 +1714,15 @@
             model = models.DescribeSecurityGroupAssociationStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecurityGroupLimits(self, request):
         """查询用户安全组配额
 
         :param request: Request instance for DescribeSecurityGroupLimits.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeSecurityGroupLimitsRequest`
@@ -1737,15 +1737,15 @@
             model = models.DescribeSecurityGroupLimitsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecurityGroupPolicies(self, request):
         """查询安全组规则
 
         :param request: Request instance for DescribeSecurityGroupPolicies.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeSecurityGroupPoliciesRequest`
@@ -1760,15 +1760,15 @@
             model = models.DescribeSecurityGroupPoliciesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecurityGroups(self, request):
         """查看安全组
 
         :param request: Request instance for DescribeSecurityGroups.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeSecurityGroupsRequest`
@@ -1783,15 +1783,15 @@
             model = models.DescribeSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSnapshots(self, request):
         """本接口（DescribeSnapshots）用于查询快照的详细信息。
 
         * 根据快照ID、创建快照的云硬盘ID、创建快照的云硬盘类型等对结果进行过滤，不同条件之间为与(AND)的关系，过滤信息详细请见过滤器`Filter`。
         *  如果参数为空，返回当前用户一定数量（`Limit`所指定的数量，默认为20）的快照列表。
@@ -1809,15 +1809,15 @@
             model = models.DescribeSnapshotsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSubnets(self, request):
         """查询子网列表
 
         :param request: Request instance for DescribeSubnets.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeSubnetsRequest`
@@ -1832,15 +1832,15 @@
             model = models.DescribeSubnetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTargetHealth(self, request):
         """获取负载均衡后端服务的健康检查状态。
 
         :param request: Request instance for DescribeTargetHealth.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeTargetHealthRequest`
@@ -1855,15 +1855,15 @@
             model = models.DescribeTargetHealthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTargets(self, request):
         """查询负载均衡绑定的后端服务列表。
 
         :param request: Request instance for DescribeTargets.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeTargetsRequest`
@@ -1878,15 +1878,15 @@
             model = models.DescribeTargetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskResult(self, request):
         """查询EIP异步任务执行结果
 
         :param request: Request instance for DescribeTaskResult.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeTaskResultRequest`
@@ -1901,15 +1901,15 @@
             model = models.DescribeTaskResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskStatus(self, request):
         """本接口(DescribeTaskStatus)用于获取异步任务状态
 
         :param request: Request instance for DescribeTaskStatus.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeTaskStatusRequest`
@@ -1924,15 +1924,15 @@
             model = models.DescribeTaskStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVpcs(self, request):
         """查询私有网络列表
 
         :param request: Request instance for DescribeVpcs.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DescribeVpcsRequest`
@@ -1947,15 +1947,15 @@
             model = models.DescribeVpcsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetachDisks(self, request):
         """本接口（DetachDisks）用于卸载云硬盘。
 
         * 支持批量操作，卸载挂载在同一主机上的多块云盘。如果多块云盘中存在不允许卸载的云盘，则操作不执行，返回特定的错误码。
         * 本接口为异步接口，当请求成功返回时，云盘并未立即从主机卸载，可通过接口[DescribeDisks](/document/product/362/16315)来查询对应云盘的状态，如果云盘的状态由“ATTACHED”变为“UNATTACHED”，则为卸载成功。
@@ -1973,15 +1973,15 @@
             model = models.DetachDisksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetachNetworkInterface(self, request):
         """弹性网卡解绑云主机
 
         :param request: Request instance for DetachNetworkInterface.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DetachNetworkInterfaceRequest`
@@ -1996,15 +1996,15 @@
             model = models.DetachNetworkInterfaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableRoutes(self, request):
         """禁用已启用的子网路由
 
         :param request: Request instance for DisableRoutes.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DisableRoutesRequest`
@@ -2019,15 +2019,15 @@
             model = models.DisableRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisassociateAddress(self, request):
         """解绑弹性公网IP（简称 EIP）
         只有状态为 BIND 和 BIND_ENI 的 EIP 才能进行解绑定操作。
         EIP 如果被封堵，则不能进行解绑定操作。
 
@@ -2044,15 +2044,15 @@
             model = models.DisassociateAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisassociateInstancesKeyPairs(self, request):
         """用于解除实例的密钥绑定关系。
 
         :param request: Request instance for DisassociateInstancesKeyPairs.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DisassociateInstancesKeyPairsRequest`
@@ -2067,15 +2067,15 @@
             model = models.DisassociateInstancesKeyPairsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisassociateSecurityGroups(self, request):
         """解绑安全组
 
         :param request: Request instance for DisassociateSecurityGroups.
         :type request: :class:`tencentcloud.ecm.v20190719.models.DisassociateSecurityGroupsRequest`
@@ -2090,15 +2090,15 @@
             model = models.DisassociateSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableRoutes(self, request):
         """启用已禁用的子网路由。
         本接口会校验启用后，是否与已有路由冲突，如果冲突，则无法启用，失败处理。路由冲突时，需要先禁用与之冲突的路由，才能启用该路由。
 
         :param request: Request instance for EnableRoutes.
@@ -2114,15 +2114,15 @@
             model = models.EnableRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ImportCustomImage(self, request):
         """导入自定义镜像，支持 RAW、VHD、QCOW2、VMDK 镜像格式
 
         :param request: Request instance for ImportCustomImage.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ImportCustomImageRequest`
@@ -2137,15 +2137,15 @@
             model = models.ImportCustomImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ImportImage(self, request):
         """从CVM产品导入镜像到ECM
 
         :param request: Request instance for ImportImage.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ImportImageRequest`
@@ -2160,15 +2160,15 @@
             model = models.ImportImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def MigrateNetworkInterface(self, request):
         """弹性网卡迁移
 
         :param request: Request instance for MigrateNetworkInterface.
         :type request: :class:`tencentcloud.ecm.v20190719.models.MigrateNetworkInterfaceRequest`
@@ -2183,15 +2183,15 @@
             model = models.MigrateNetworkInterfaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def MigratePrivateIpAddress(self, request):
         """弹性网卡内网IP迁移。
         该接口用于将一个内网IP从一个弹性网卡上迁移到另外一个弹性网卡，主IP地址不支持迁移。
         迁移前后的弹性网卡必须在同一个子网内。
 
@@ -2208,15 +2208,15 @@
             model = models.MigratePrivateIpAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAddressAttribute(self, request):
         """修改弹性公网IP属性
 
         :param request: Request instance for ModifyAddressAttribute.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifyAddressAttributeRequest`
@@ -2231,15 +2231,15 @@
             model = models.ModifyAddressAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAddressesBandwidth(self, request):
         """调整弹性公网IP带宽
 
         :param request: Request instance for ModifyAddressesBandwidth.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifyAddressesBandwidthRequest`
@@ -2254,15 +2254,15 @@
             model = models.ModifyAddressesBandwidthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDefaultSubnet(self, request):
         """修改在一个可用区下创建实例时使用的默认子网（创建实例时，未填写VPC参数时使用的sunbetId）
 
         :param request: Request instance for ModifyDefaultSubnet.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifyDefaultSubnetRequest`
@@ -2277,15 +2277,15 @@
             model = models.ModifyDefaultSubnetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyHaVipAttribute(self, request):
         """用于修改高可用虚拟IP（HAVIP）属性
 
         :param request: Request instance for ModifyHaVipAttribute.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifyHaVipAttributeRequest`
@@ -2300,15 +2300,15 @@
             model = models.ModifyHaVipAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyImageAttribute(self, request):
         """本接口（ModifyImageAttribute）用于修改镜像属性。
 
         :param request: Request instance for ModifyImageAttribute.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifyImageAttributeRequest`
@@ -2323,15 +2323,15 @@
             model = models.ModifyImageAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstancesAttribute(self, request):
         """修改实例的属性。
 
         :param request: Request instance for ModifyInstancesAttribute.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifyInstancesAttributeRequest`
@@ -2346,15 +2346,15 @@
             model = models.ModifyInstancesAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyIpv6AddressesAttribute(self, request):
         """本接口（ModifyIpv6AddressesAttribute）用于修改弹性网卡IPv6地址属性。
 
         :param request: Request instance for ModifyIpv6AddressesAttribute.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifyIpv6AddressesAttributeRequest`
@@ -2369,15 +2369,15 @@
             model = models.ModifyIpv6AddressesAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyIpv6AddressesBandwidth(self, request):
         """该接口(ModifyIpv6AddressesBandwidth)用于修改IPV6地址访问internet的带宽
 
         :param request: Request instance for ModifyIpv6AddressesBandwidth.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifyIpv6AddressesBandwidthRequest`
@@ -2392,15 +2392,15 @@
             model = models.ModifyIpv6AddressesBandwidthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyListener(self, request):
         """修改负载均衡监听器属性。
 
         :param request: Request instance for ModifyListener.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifyListenerRequest`
@@ -2415,15 +2415,15 @@
             model = models.ModifyListenerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLoadBalancerAttributes(self, request):
         """修改负载均衡实例的属性。
 
         :param request: Request instance for ModifyLoadBalancerAttributes.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifyLoadBalancerAttributesRequest`
@@ -2438,15 +2438,15 @@
             model = models.ModifyLoadBalancerAttributesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyModuleConfig(self, request):
         """修改模块配置，已关联实例的模块不支持调整配置。
 
         :param request: Request instance for ModifyModuleConfig.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifyModuleConfigRequest`
@@ -2461,15 +2461,15 @@
             model = models.ModifyModuleConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyModuleDisableWanIp(self, request):
         """修改模块是否禁止分配外网ip的属性。
 
         :param request: Request instance for ModifyModuleDisableWanIp.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifyModuleDisableWanIpRequest`
@@ -2484,15 +2484,15 @@
             model = models.ModifyModuleDisableWanIpResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyModuleImage(self, request):
         """修改模块的默认镜像
 
         :param request: Request instance for ModifyModuleImage.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifyModuleImageRequest`
@@ -2507,15 +2507,15 @@
             model = models.ModifyModuleImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyModuleIpDirect(self, request):
         """修改模块IP直通。
 
         :param request: Request instance for ModifyModuleIpDirect.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifyModuleIpDirectRequest`
@@ -2530,15 +2530,15 @@
             model = models.ModifyModuleIpDirectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyModuleName(self, request):
         """修改模块名称
 
         :param request: Request instance for ModifyModuleName.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifyModuleNameRequest`
@@ -2553,15 +2553,15 @@
             model = models.ModifyModuleNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyModuleNetwork(self, request):
         """修改模块默认带宽上限
 
         :param request: Request instance for ModifyModuleNetwork.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifyModuleNetworkRequest`
@@ -2576,15 +2576,15 @@
             model = models.ModifyModuleNetworkResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyModuleSecurityGroups(self, request):
         """修改模块默认安全组
 
         :param request: Request instance for ModifyModuleSecurityGroups.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifyModuleSecurityGroupsRequest`
@@ -2599,15 +2599,15 @@
             model = models.ModifyModuleSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPrivateIpAddressesAttribute(self, request):
         """用于修改弹性网卡内网IP属性。
 
         :param request: Request instance for ModifyPrivateIpAddressesAttribute.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifyPrivateIpAddressesAttributeRequest`
@@ -2622,15 +2622,15 @@
             model = models.ModifyPrivateIpAddressesAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRouteTableAttribute(self, request):
         """修改路由表属性
 
         :param request: Request instance for ModifyRouteTableAttribute.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifyRouteTableAttributeRequest`
@@ -2645,15 +2645,15 @@
             model = models.ModifyRouteTableAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySecurityGroupAttribute(self, request):
         """修改安全组属性
 
         :param request: Request instance for ModifySecurityGroupAttribute.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifySecurityGroupAttributeRequest`
@@ -2668,15 +2668,15 @@
             model = models.ModifySecurityGroupAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySecurityGroupPolicies(self, request):
         """修改安全组出站和入站规则
 
         :param request: Request instance for ModifySecurityGroupPolicies.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifySecurityGroupPoliciesRequest`
@@ -2691,15 +2691,15 @@
             model = models.ModifySecurityGroupPoliciesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySubnetAttribute(self, request):
         """修改子网属性
 
         :param request: Request instance for ModifySubnetAttribute.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifySubnetAttributeRequest`
@@ -2714,15 +2714,15 @@
             model = models.ModifySubnetAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTargetPort(self, request):
         """修改监听器绑定的后端机器的端口。
 
         :param request: Request instance for ModifyTargetPort.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifyTargetPortRequest`
@@ -2737,15 +2737,15 @@
             model = models.ModifyTargetPortResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTargetWeight(self, request):
         """修改监听器绑定的后端机器的转发权重。
 
         :param request: Request instance for ModifyTargetWeight.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifyTargetWeightRequest`
@@ -2760,15 +2760,15 @@
             model = models.ModifyTargetWeightResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyVpcAttribute(self, request):
         """修改私有网络（VPC）的相关属性
 
         :param request: Request instance for ModifyVpcAttribute.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ModifyVpcAttributeRequest`
@@ -2783,15 +2783,15 @@
             model = models.ModifyVpcAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryVpcTaskResult(self, request):
         """查询私有网络下Vpc、子网、havip等异步任务请求结果
 
         :param request: Request instance for QueryVpcTaskResult.
         :type request: :class:`tencentcloud.ecm.v20190719.models.QueryVpcTaskResultRequest`
@@ -2806,15 +2806,15 @@
             model = models.QueryVpcTaskResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RebootInstances(self, request):
         """只有状态为RUNNING的实例才可以进行此操作；接口调用成功时，实例会进入REBOOTING状态；重启实例成功时，实例会进入RUNNING状态；支持强制重启，强制重启的效果等同于关闭物理计算机的电源开关再重新启动。强制重启可能会导致数据丢失或文件系统损坏，请仅在服务器不能正常重启时使用。
 
         :param request: Request instance for RebootInstances.
         :type request: :class:`tencentcloud.ecm.v20190719.models.RebootInstancesRequest`
@@ -2829,15 +2829,15 @@
             model = models.RebootInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReleaseAddresses(self, request):
         """释放一个或多个弹性公网IP（简称 EIP）。
         该操作不可逆，释放后 EIP 关联的 IP 地址将不再属于您的名下。
         只有状态为 UNBIND 的 EIP 才能进行释放操作。
 
@@ -2854,15 +2854,15 @@
             model = models.ReleaseAddressesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReleaseIpv6Addresses(self, request):
         """本接口（UnassignIpv6Addresses）用于释放弹性网卡IPv6地址。
 
         :param request: Request instance for ReleaseIpv6Addresses.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ReleaseIpv6AddressesRequest`
@@ -2877,15 +2877,15 @@
             model = models.ReleaseIpv6AddressesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReleaseIpv6AddressesBandwidth(self, request):
         """该接口用于给弹性公网IPv6地址释放带宽。
 
         :param request: Request instance for ReleaseIpv6AddressesBandwidth.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ReleaseIpv6AddressesBandwidthRequest`
@@ -2900,15 +2900,15 @@
             model = models.ReleaseIpv6AddressesBandwidthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RemovePrivateIpAddresses(self, request):
         """弹性网卡退还内网 IP。
         退还弹性网卡上的辅助内网IP，接口自动解关联弹性公网 IP。不能退还弹性网卡的主内网IP。
 
         :param request: Request instance for RemovePrivateIpAddresses.
@@ -2924,15 +2924,15 @@
             model = models.RemovePrivateIpAddressesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReplaceRouteTableAssociation(self, request):
         """修改子网关联的路由表，一个子网只能关联一个路由表。
 
         :param request: Request instance for ReplaceRouteTableAssociation.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ReplaceRouteTableAssociationRequest`
@@ -2947,15 +2947,15 @@
             model = models.ReplaceRouteTableAssociationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReplaceRoutes(self, request):
         """替换路由策略
 
         :param request: Request instance for ReplaceRoutes.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ReplaceRoutesRequest`
@@ -2970,15 +2970,15 @@
             model = models.ReplaceRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReplaceSecurityGroupPolicy(self, request):
         """替换单条安全组路由规则, 单个请求中只能替换单个方向的一条规则, 必须要指定索引（PolicyIndex）。
 
         :param request: Request instance for ReplaceSecurityGroupPolicy.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ReplaceSecurityGroupPolicyRequest`
@@ -2993,15 +2993,15 @@
             model = models.ReplaceSecurityGroupPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetInstances(self, request):
         """重装实例，若指定了ImageId参数，则使用指定的镜像重装；否则按照当前实例使用的镜像进行重装；若未指定密码，则密码通过站内信形式随后发送。
 
         :param request: Request instance for ResetInstances.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ResetInstancesRequest`
@@ -3016,15 +3016,15 @@
             model = models.ResetInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetInstancesMaxBandwidth(self, request):
         """重置实例的最大带宽上限。
 
         :param request: Request instance for ResetInstancesMaxBandwidth.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ResetInstancesMaxBandwidthRequest`
@@ -3039,15 +3039,15 @@
             model = models.ResetInstancesMaxBandwidthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetInstancesPassword(self, request):
         """重置处于运行中状态的实例的密码，需要显式指定强制关机参数ForceStop。如果没有显式指定强制关机参数，则只有处于关机状态的实例才允许执行重置密码操作。
 
         :param request: Request instance for ResetInstancesPassword.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ResetInstancesPasswordRequest`
@@ -3062,15 +3062,15 @@
             model = models.ResetInstancesPasswordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetRoutes(self, request):
         """对某个路由表名称和所有路由策略（Route）进行重新设置
 
         :param request: Request instance for ResetRoutes.
         :type request: :class:`tencentcloud.ecm.v20190719.models.ResetRoutesRequest`
@@ -3085,15 +3085,15 @@
             model = models.ResetRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RunInstances(self, request):
         """创建ECM实例。
 
         :param request: Request instance for RunInstances.
         :type request: :class:`tencentcloud.ecm.v20190719.models.RunInstancesRequest`
@@ -3108,15 +3108,15 @@
             model = models.RunInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetLoadBalancerSecurityGroups(self, request):
         """设置负载均衡实例的安全组。
 
         :param request: Request instance for SetLoadBalancerSecurityGroups.
         :type request: :class:`tencentcloud.ecm.v20190719.models.SetLoadBalancerSecurityGroupsRequest`
@@ -3131,15 +3131,15 @@
             model = models.SetLoadBalancerSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetSecurityGroupForLoadbalancers(self, request):
         """绑定或解绑一个安全组到多个负载均衡实例。
 
         :param request: Request instance for SetSecurityGroupForLoadbalancers.
         :type request: :class:`tencentcloud.ecm.v20190719.models.SetSecurityGroupForLoadbalancersRequest`
@@ -3154,15 +3154,15 @@
             model = models.SetSecurityGroupForLoadbalancersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartInstances(self, request):
         """只有状态为STOPPED的实例才可以进行此操作；接口调用成功时，实例会进入STARTING状态；启动实例成功时，实例会进入RUNNING状态。
 
         :param request: Request instance for StartInstances.
         :type request: :class:`tencentcloud.ecm.v20190719.models.StartInstancesRequest`
@@ -3177,15 +3177,15 @@
             model = models.StartInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopInstances(self, request):
         """只有处于"RUNNING"状态的实例才能够进行关机操作；
         调用成功时，实例会进入STOPPING状态；关闭实例成功时，实例会进入STOPPED状态；
         支持强制关闭，强制关机的效果等同于关闭物理计算机的电源开关，强制关机可能会导致数据丢失或文件系统损坏，请仅在服务器不能正常关机时使用。
 
@@ -3202,15 +3202,15 @@
             model = models.StopInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TerminateDisks(self, request):
         """本接口（TerminateDisks）用于退还云硬盘。
 
         * 不再使用的云盘，可通过本接口主动退还。
         * 本接口支持退还预付费云盘和按小时后付费云盘。按小时后付费云盘可直接退还，预付费云盘需符合退还规则。
@@ -3229,15 +3229,15 @@
             model = models.TerminateDisksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TerminateInstances(self, request):
         """销毁实例
 
         :param request: Request instance for TerminateInstances.
         :type request: :class:`tencentcloud.ecm.v20190719.models.TerminateInstancesRequest`
@@ -3252,15 +3252,15 @@
             model = models.TerminateInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnassignIpv6SubnetCidrBlock(self, request):
         """本接口（UnassignIpv6SubnetCidrBlock）用于释放IPv6子网段。
         子网段如果还有IP占用且未回收，则子网段无法释放。
 
         :param request: Request instance for UnassignIpv6SubnetCidrBlock.
@@ -3276,8 +3276,8 @@
             model = models.UnassignIpv6SubnetCidrBlockResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-ecm-3.0.937/tencentcloud/ecm/v20190719/errorcodes.py` & `tencentcloud-sdk-python-ecm-3.0.938/tencentcloud/ecm/v20190719/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecm-3.0.937/tencentcloud/ecm/v20190719/models.py` & `tencentcloud-sdk-python-ecm-3.0.938/tencentcloud/ecm/v20190719/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecm-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-ecm-3.0.938/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ecm
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ecm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ecm-3.0.937/README.rst` & `tencentcloud-sdk-python-ecm-3.0.938/README.rst`

 * *Files identical despite different names*

