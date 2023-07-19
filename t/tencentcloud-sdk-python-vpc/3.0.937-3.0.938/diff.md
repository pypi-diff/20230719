# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.937.tar", last modified: Tue Jul 18 00:35:01 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.938.tar", last modified: Wed Jul 19 00:53:42 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.937.tar` & `tencentcloud-sdk-python-vpc-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/vpc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/vpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)   332400 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42690 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1312049 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:42.000000 tencentcloud-sdk-python-vpc-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:53:42.000000 tencentcloud-sdk-python-vpc-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:42.000000 tencentcloud-sdk-python-vpc-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:42.000000 tencentcloud-sdk-python-vpc-3.0.938/tencentcloud/vpc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:53:42.000000 tencentcloud-sdk-python-vpc-3.0.938/tencentcloud/vpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:42.000000 tencentcloud-sdk-python-vpc-3.0.938/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   333624 2023-07-19 00:53:42.000000 tencentcloud-sdk-python-vpc-3.0.938/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:53:42.000000 tencentcloud-sdk-python-vpc-3.0.938/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42690 2023-07-19 00:53:42.000000 tencentcloud-sdk-python-vpc-3.0.938/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1312049 2023-07-19 00:53:42.000000 tencentcloud-sdk-python-vpc-3.0.938/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:53:42.000000 tencentcloud-sdk-python-vpc-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:53:42.000000 tencentcloud-sdk-python-vpc-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:53:42.000000 tencentcloud-sdk-python-vpc-3.0.938/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:42.000000 tencentcloud-sdk-python-vpc-3.0.938/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:53:42.000000 tencentcloud-sdk-python-vpc-3.0.938/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:53:42.000000 tencentcloud-sdk-python-vpc-3.0.938/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:53:42.000000 tencentcloud-sdk-python-vpc-3.0.938/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:53:42.000000 tencentcloud-sdk-python-vpc-3.0.938/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:53:42.000000 tencentcloud-sdk-python-vpc-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.937/setup.py` & `tencentcloud-sdk-python-vpc-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.938/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AcceptAttachCcnInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddBandwidthPackageResources(self, request):
         """接口用于添加带宽包资源，包括[弹性公网IP](https://cloud.tencent.com/document/product/213/1941)和[负载均衡](https://cloud.tencent.com/document/product/214/517)等
 
         :param request: Request instance for AddBandwidthPackageResources.
         :type request: :class:`tencentcloud.vpc.v20170312.models.AddBandwidthPackageResourcesRequest`
@@ -65,15 +65,15 @@
             model = models.AddBandwidthPackageResourcesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddIp6Rules(self, request):
         """1. 该接口用于在转换实例下添加IPV6转换规则。
         2. 支持在同一个转换实例下批量添加转换规则，一个账户在一个地域最多50个。
         3. 一个完整的转换规则包括vip6:vport6:protocol:vip:vport，其中vip6:vport6:protocol必须是唯一。
 
@@ -90,15 +90,15 @@
             model = models.AddIp6RulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddTemplateMember(self, request):
         """增加模板对象中的IP地址、协议端口、IP地址组、协议端口组。当前仅支持北京、泰国、北美地域请求。
 
         :param request: Request instance for AddTemplateMember.
         :type request: :class:`tencentcloud.vpc.v20170312.models.AddTemplateMemberRequest`
@@ -113,15 +113,15 @@
             model = models.AddTemplateMemberResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AdjustPublicAddress(self, request):
         """本接口 (AdjustPublicAddress) 用于更换IP地址，支持更换CVM实例的普通公网IP和包月带宽的EIP。
 
         :param request: Request instance for AdjustPublicAddress.
         :type request: :class:`tencentcloud.vpc.v20170312.models.AdjustPublicAddressRequest`
@@ -136,15 +136,15 @@
             model = models.AdjustPublicAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AllocateAddresses(self, request):
         """本接口 (AllocateAddresses) 用于申请一个或多个[弹性公网IP](https://cloud.tencent.com/document/product/213/1941)（简称 EIP）。
         * EIP 是专为动态云计算设计的静态 IP 地址。借助 EIP，您可以快速将 EIP 重新映射到您的另一个实例上，从而屏蔽实例故障。
         * 您的 EIP 与腾讯云账户相关联，而不是与某个实例相关联。在您选择显式释放该地址，或欠费超过24小时之前，它会一直与您的腾讯云账户保持关联。
         * 一个腾讯云账户在每个地域能申请的 EIP 最大配额有所限制，可参见 [EIP 产品简介](https://cloud.tencent.com/document/product/213/5733)，上述配额可通过 DescribeAddressQuota 接口获取。
@@ -162,15 +162,15 @@
             model = models.AllocateAddressesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AllocateIp6AddressesBandwidth(self, request):
         """该接口用于给IPv6地址初次分配公网带宽
 
         :param request: Request instance for AllocateIp6AddressesBandwidth.
         :type request: :class:`tencentcloud.vpc.v20170312.models.AllocateIp6AddressesBandwidthRequest`
@@ -185,15 +185,15 @@
             model = models.AllocateIp6AddressesBandwidthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssignIpv6Addresses(self, request):
         """本接口（AssignIpv6Addresses）用于弹性网卡申请`IPv6`地址。<br />
         本接口是异步完成，如需查询异步任务执行结果，请使用本接口返回的`RequestId`轮询`DescribeVpcTaskResult`接口。
         * 一个弹性网卡支持绑定的IP地址是有限制的，更多资源限制信息详见<a href="/document/product/576/18527">弹性网卡使用限制</a>。
         * 可以指定`IPv6`地址申请，地址类型不能为主`IP`，`IPv6`地址暂时只支持作为辅助`IP`。
@@ -213,15 +213,15 @@
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
         * 使用本接口前，您需要已有VPC实例，如果没有可通过接口<a href="https://cloud.tencent.com/document/api/215/15774" title="CreateVpc" target="_blank">CreateVpc</a>创建。
         * 每个VPC只能申请一个IPv6网段。
 
@@ -238,15 +238,15 @@
             model = models.AssignIpv6CidrBlockResponse()
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
         * 给子网分配 `IPv6` 网段，要求子网所属 `VPC` 已获得 `IPv6` 网段。如果尚未分配，请先通过接口 `AssignIpv6CidrBlock` 给子网所属 `VPC` 分配一个 `IPv6` 网段。否则无法分配 `IPv6` 子网段。
         * 每个子网只能分配一个IPv6网段。
 
@@ -263,15 +263,15 @@
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
         """本接口（AssignPrivateIpAddresses）用于弹性网卡申请内网 IP。
         * 一个弹性网卡支持绑定的IP地址是有限制的，更多资源限制信息详见<a href="/document/product/576/18527">弹性网卡使用限制</a>。
         * 可以指定内网IP地址申请，内网IP地址类型不能为主IP，主IP已存在，不能修改，内网IP必须要弹性网卡所在子网内，而且不能被占用。
         * 在弹性网卡上申请一个到多个辅助内网IP，接口会在弹性网卡所在子网网段内返回指定数量的辅助内网IP。
@@ -291,15 +291,15 @@
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
         """本接口 (AssociateAddress) 用于将[弹性公网IP](https://cloud.tencent.com/document/product/213/1941)（简称 EIP）绑定到实例或弹性网卡的指定内网 IP 上。
         * 将 EIP 绑定到实例（CVM）上，其本质是将 EIP 绑定到实例上主网卡的主内网 IP 上。
         * 将 EIP 绑定到主网卡的主内网IP上，绑定过程会把其上绑定的普通公网 IP 自动解绑并释放。
         * 将 EIP 绑定到指定网卡的内网 IP上（非主网卡的主内网IP），则必须先解绑该 EIP，才能再绑定新的。
@@ -321,15 +321,15 @@
             model = models.AssociateAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssociateDhcpIpWithAddressIp(self, request):
         """本接口（AssociateDhcpIpWithAddressIp）用于DhcpIp绑定弹性公网IP（EIP）。<br />
         >?本接口为异步接口，可调用 [DescribeVpcTaskResult](https://cloud.tencent.com/document/api/215/59037) 接口查询任务执行结果，待任务执行成功后再进行其他操作。
         >
 
@@ -346,15 +346,15 @@
             model = models.AssociateDhcpIpWithAddressIpResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssociateDirectConnectGatewayNatGateway(self, request):
         """将专线网关与NAT网关绑定，专线网关默认路由指向NAT网关
 
         :param request: Request instance for AssociateDirectConnectGatewayNatGateway.
         :type request: :class:`tencentcloud.vpc.v20170312.models.AssociateDirectConnectGatewayNatGatewayRequest`
@@ -369,15 +369,15 @@
             model = models.AssociateDirectConnectGatewayNatGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssociateNatGatewayAddress(self, request):
         """本接口(AssociateNatGatewayAddress)用于NAT网关绑定弹性IP（EIP）。
 
         :param request: Request instance for AssociateNatGatewayAddress.
         :type request: :class:`tencentcloud.vpc.v20170312.models.AssociateNatGatewayAddressRequest`
@@ -392,15 +392,15 @@
             model = models.AssociateNatGatewayAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssociateNetworkAclSubnets(self, request):
         """本接口（AssociateNetworkAclSubnets）用于网络ACL关联VPC下的子网。
 
         :param request: Request instance for AssociateNetworkAclSubnets.
         :type request: :class:`tencentcloud.vpc.v20170312.models.AssociateNetworkAclSubnetsRequest`
@@ -415,15 +415,15 @@
             model = models.AssociateNetworkAclSubnetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssociateNetworkInterfaceSecurityGroups(self, request):
         """本接口（AssociateNetworkInterfaceSecurityGroups）用于弹性网卡绑定安全组（SecurityGroup）。
 
         :param request: Request instance for AssociateNetworkInterfaceSecurityGroups.
         :type request: :class:`tencentcloud.vpc.v20170312.models.AssociateNetworkInterfaceSecurityGroupsRequest`
@@ -438,15 +438,15 @@
             model = models.AssociateNetworkInterfaceSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AttachCcnInstances(self, request):
         """本接口（AttachCcnInstances）用于将网络实例加载到云联网实例中，网络实例包括VPC和专线网关。<br />
         每个云联网能够关联的网络实例个数是有限的，详情请参考产品文档。如果需要扩充请联系在线客服。
 
         :param request: Request instance for AttachCcnInstances.
@@ -462,15 +462,15 @@
             model = models.AttachCcnInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AttachClassicLinkVpc(self, request):
         """本接口(AttachClassicLinkVpc)用于创建私有网络和基础网络设备互通。
         * 私有网络和基础网络设备必须在同一个地域。
         * 私有网络和基础网络的区别详见vpc产品文档-<a href="https://cloud.tencent.com/document/product/215/30720">私有网络与基础网络</a>。
         >?本接口为异步接口，可调用 [DescribeVpcTaskResult](https://cloud.tencent.com/document/api/215/59037) 接口查询任务执行结果，待任务执行成功后再进行其他操作。
@@ -489,15 +489,15 @@
             model = models.AttachClassicLinkVpcResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AttachNetworkInterface(self, request):
         """本接口（AttachNetworkInterface）用于弹性网卡绑定云服务器。
         * 一个弹性网卡请至少绑定一个安全组，如需绑定请参见<a href="https://cloud.tencent.com/document/product/215/43132">弹性网卡绑定安全组</a>。
         * 一个云服务器可以绑定多个弹性网卡，但只能绑定一个主网卡。更多限制信息详见<a href="https://cloud.tencent.com/document/product/576/18527">弹性网卡使用限制</a>。
         * 一个弹性网卡只能同时绑定一个云服务器。
@@ -519,15 +519,15 @@
             model = models.AttachNetworkInterfaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AttachSnapshotInstances(self, request):
         """本接口（AttachSnapshotInstances）用于快照策略关联实例。
 
         :param request: Request instance for AttachSnapshotInstances.
         :type request: :class:`tencentcloud.vpc.v20170312.models.AttachSnapshotInstancesRequest`
@@ -542,15 +542,15 @@
             model = models.AttachSnapshotInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AuditCrossBorderCompliance(self, request):
         """本接口（AuditCrossBorderCompliance）用于服务商操作合规化资质审批。
         * 服务商只能操作提交到本服务商的审批单，后台会校验身份。即只授权给服务商的`APPID` 调用本接口。
         * `APPROVED` 状态的审批单，可以再次操作为 `DENY`；`DENY` 状态的审批单，也可以再次操作为 `APPROVED`。
 
@@ -567,15 +567,15 @@
             model = models.AuditCrossBorderComplianceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckAssistantCidr(self, request):
         """本接口（CheckAssistantCidr）用于检查辅助CIDR是否与存量路由、对等连接（对端VPC的CIDR）等资源存在冲突。如果存在重叠，则返回重叠的资源。
         * 检测辅助CIDR是否与当前VPC的主CIDR和辅助CIDR存在重叠。
         * 检测辅助CIDR是否与当前VPC的路由的目的端存在重叠。
         * 检测辅助CIDR是否与当前VPC的对等连接，对端VPC下的主CIDR或辅助CIDR存在重叠。
@@ -593,15 +593,15 @@
             model = models.CheckAssistantCidrResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckDefaultSubnet(self, request):
         """本接口（CheckDefaultSubnet）用于预判是否可建默认子网。
 
         :param request: Request instance for CheckDefaultSubnet.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CheckDefaultSubnetRequest`
@@ -616,15 +616,15 @@
             model = models.CheckDefaultSubnetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckNetDetectState(self, request):
         """本接口（CheckNetDetectState）用于验证网络探测。
 
         :param request: Request instance for CheckNetDetectState.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CheckNetDetectStateRequest`
@@ -639,15 +639,15 @@
             model = models.CheckNetDetectStateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CloneSecurityGroup(self, request):
         """本接口（CloneSecurityGroup）用于根据存量的安全组，克隆创建出同样规则配置的安全组。仅克隆安全组及其规则信息，不会克隆安全组标签信息。
 
         :param request: Request instance for CloneSecurityGroup.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CloneSecurityGroupRequest`
@@ -662,15 +662,15 @@
             model = models.CloneSecurityGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAddressTemplate(self, request):
         """本接口（CreateAddressTemplate）用于创建IP地址模板。
 
         :param request: Request instance for CreateAddressTemplate.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateAddressTemplateRequest`
@@ -685,15 +685,15 @@
             model = models.CreateAddressTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAddressTemplateGroup(self, request):
         """本接口（CreateAddressTemplateGroup）用于创建IP地址模板集合。
 
         :param request: Request instance for CreateAddressTemplateGroup.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateAddressTemplateGroupRequest`
@@ -708,15 +708,15 @@
             model = models.CreateAddressTemplateGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAndAttachNetworkInterface(self, request):
         """本接口（CreateAndAttachNetworkInterface）用于创建弹性网卡并绑定云服务器。
         * 创建弹性网卡时可以指定内网IP，并且可以指定一个主IP，指定的内网IP必须在弹性网卡所在子网内，而且不能被占用。
         * 创建弹性网卡时可以指定需要申请的内网IP数量，系统会随机生成内网IP地址。
         * 一个弹性网卡支持绑定的IP地址是有限制的，更多资源限制信息详见<a href="/document/product/576/18527">弹性网卡使用限制</a>。
@@ -738,15 +738,15 @@
             model = models.CreateAndAttachNetworkInterfaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAssistantCidr(self, request):
         """本接口（CreateAssistantCidr）用于批量创建辅助CIDR。
 
         :param request: Request instance for CreateAssistantCidr.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateAssistantCidrRequest`
@@ -761,15 +761,15 @@
             model = models.CreateAssistantCidrResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateBandwidthPackage(self, request):
         """本接口 (CreateBandwidthPackage) 支持创建[设备带宽包](https://cloud.tencent.com/document/product/684/15245#bwptype)和[IP带宽包](https://cloud.tencent.com/document/product/684/15245#bwptype)。
 
         :param request: Request instance for CreateBandwidthPackage.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateBandwidthPackageRequest`
@@ -784,15 +784,15 @@
             model = models.CreateBandwidthPackageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCcn(self, request):
         """本接口（CreateCcn）用于创建云联网（CCN）。<br />
         * 创建云联网同时可以绑定标签, 应答里的标签列表代表添加成功的标签。
         * 每个账号能创建的云联网实例个数是有限的，详请参考产品文档。如果需要扩充请联系在线客服。
 
@@ -809,15 +809,15 @@
             model = models.CreateCcnResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCustomerGateway(self, request):
         """本接口（CreateCustomerGateway）用于创建对端网关。
 
         :param request: Request instance for CreateCustomerGateway.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateCustomerGatewayRequest`
@@ -832,15 +832,15 @@
             model = models.CreateCustomerGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDefaultSecurityGroup(self, request):
         """本接口（CreateDefaultSecurityGroup）用于创建（如果项目下未存在默认安全组，则创建；已存在则获取。）默认安全组（SecurityGroup）。
         * 每个账户下每个地域的每个项目的<a href="https://cloud.tencent.com/document/product/213/12453">安全组数量限制</a>。
         * 默认安全组会放通所有IPv4规则，在创建后通常您需要再调用CreateSecurityGroupPolicies将安全组的规则设置为需要的规则。
         * 创建安全组同时可以绑定标签, 应答里的标签列表代表添加成功的标签。
@@ -858,15 +858,15 @@
             model = models.CreateDefaultSecurityGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDefaultVpc(self, request):
         """本接口（CreateDefaultVpc）用于创建默认私有网络(VPC）。
 
         默认VPC适用于快速入门和启动公共实例，您可以像使用任何其他VPC一样使用默认VPC。如果您想创建标准VPC，即指定VPC名称、VPC网段、子网网段、子网可用区，请使用常规创建VPC接口（CreateVpc）
 
@@ -889,15 +889,15 @@
             model = models.CreateDefaultVpcResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDhcpIp(self, request):
         """本接口（CreateDhcpIp）用于创建DhcpIp。
 
         :param request: Request instance for CreateDhcpIp.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateDhcpIpRequest`
@@ -912,15 +912,15 @@
             model = models.CreateDhcpIpResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDirectConnectGateway(self, request):
         """本接口（CreateDirectConnectGateway）用于创建专线网关。
 
         :param request: Request instance for CreateDirectConnectGateway.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateDirectConnectGatewayRequest`
@@ -935,15 +935,15 @@
             model = models.CreateDirectConnectGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDirectConnectGatewayCcnRoutes(self, request):
         """本接口（CreateDirectConnectGatewayCcnRoutes）用于创建专线网关的云联网路由（IDC网段）
 
         :param request: Request instance for CreateDirectConnectGatewayCcnRoutes.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateDirectConnectGatewayCcnRoutesRequest`
@@ -958,15 +958,15 @@
             model = models.CreateDirectConnectGatewayCcnRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFlowLog(self, request):
         """本接口（CreateFlowLog）用于创建网络流日志。
 
         :param request: Request instance for CreateFlowLog.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateFlowLogRequest`
@@ -981,15 +981,15 @@
             model = models.CreateFlowLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateHaVip(self, request):
         """本接口（CreateHaVip）用于创建高可用虚拟IP（HAVIP）。
 
         :param request: Request instance for CreateHaVip.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateHaVipRequest`
@@ -1004,15 +1004,15 @@
             model = models.CreateHaVipResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateIp6Translators(self, request):
         """1. 该接口用于创建IPV6转换IPV4实例，支持批量
         2. 同一个账户在一个地域最多允许创建10个转换实例
 
         :param request: Request instance for CreateIp6Translators.
@@ -1028,15 +1028,15 @@
             model = models.CreateIp6TranslatorsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLocalGateway(self, request):
         """本接口（CreateLocalGateway）用于创建用于CDC的本地网关。
 
         :param request: Request instance for CreateLocalGateway.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateLocalGatewayRequest`
@@ -1051,15 +1051,15 @@
             model = models.CreateLocalGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNatGateway(self, request):
         """本接口(CreateNatGateway)用于创建NAT网关。
         在对新建的NAT网关做其他操作前，需先确认此网关已被创建完成（DescribeNatGateway接口返回的实例State字段为AVAILABLE）。
 
         :param request: Request instance for CreateNatGateway.
@@ -1075,15 +1075,15 @@
             model = models.CreateNatGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNatGatewayDestinationIpPortTranslationNatRule(self, request):
         """本接口(CreateNatGatewayDestinationIpPortTranslationNatRule)用于创建NAT网关端口转发规则。
 
         :param request: Request instance for CreateNatGatewayDestinationIpPortTranslationNatRule.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateNatGatewayDestinationIpPortTranslationNatRuleRequest`
@@ -1098,15 +1098,15 @@
             model = models.CreateNatGatewayDestinationIpPortTranslationNatRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNatGatewaySourceIpTranslationNatRule(self, request):
         """本接口(CreateNatGatewaySourceIpTranslationNatRule)用于创建NAT网关SNAT规则
 
         :param request: Request instance for CreateNatGatewaySourceIpTranslationNatRule.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateNatGatewaySourceIpTranslationNatRuleRequest`
@@ -1121,15 +1121,15 @@
             model = models.CreateNatGatewaySourceIpTranslationNatRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNetDetect(self, request):
         """本接口（CreateNetDetect）用于创建网络探测。
 
         :param request: Request instance for CreateNetDetect.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateNetDetectRequest`
@@ -1144,15 +1144,15 @@
             model = models.CreateNetDetectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNetworkAcl(self, request):
         """本接口（CreateNetworkAcl）用于创建新的<a href="https://cloud.tencent.com/document/product/215/20088">网络ACL</a>。
         * 新建的网络ACL的入站和出站规则默认都是全部拒绝，在创建后通常您需要再调用ModifyNetworkAclEntries将网络ACL的规则设置为需要的规则。
 
         :param request: Request instance for CreateNetworkAcl.
@@ -1168,15 +1168,15 @@
             model = models.CreateNetworkAclResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNetworkAclQuintupleEntries(self, request):
         """本接口（CreateNetworkAclQuintupleEntries）用于增量网络ACL五元组的入站规则和出站规则。
 
         :param request: Request instance for CreateNetworkAclQuintupleEntries.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateNetworkAclQuintupleEntriesRequest`
@@ -1191,15 +1191,15 @@
             model = models.CreateNetworkAclQuintupleEntriesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNetworkInterface(self, request):
         """本接口（CreateNetworkInterface）用于创建弹性网卡。
         * 创建弹性网卡时可以指定内网IP，并且可以指定一个主IP，指定的内网IP必须在弹性网卡所在子网内，而且不能被占用。
         * 创建弹性网卡时可以指定需要申请的内网IP数量，系统会随机生成内网IP地址。
         * 一个弹性网卡支持绑定的IP地址是有限制的，更多资源限制信息详见<a href="/document/product/576/18527">弹性网卡使用限制</a>。
@@ -1221,15 +1221,15 @@
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
         """本接口(CreateRouteTable)用于创建路由表。
         * 创建了VPC后，系统会创建一个默认路由表，所有新建的子网都会关联到默认路由表。默认情况下您可以直接使用默认路由表来管理您的路由策略。当您的路由策略较多时，您可以调用创建路由表接口创建更多路由表管理您的路由策略。
         * 创建路由表同时可以绑定标签, 应答里的标签列表代表添加成功的标签。
 
@@ -1246,15 +1246,15 @@
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
         """本接口（CreateRoutes）用于创建路由策略。
         * 向指定路由表批量新增路由策略。
 
         :param request: Request instance for CreateRoutes.
@@ -1270,15 +1270,15 @@
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
         """本接口（CreateSecurityGroup）用于创建新的安全组（SecurityGroup）。
         * 每个账户下每个地域的每个项目的<a href="https://cloud.tencent.com/document/product/213/12453">安全组数量限制</a>。
         * 新建的安全组的入站和出站规则默认都是全部拒绝，在创建后通常您需要再调用CreateSecurityGroupPolicies将安全组的规则设置为需要的规则。
         * 创建安全组同时可以绑定标签, 应答里的标签列表代表添加成功的标签。
@@ -1296,15 +1296,15 @@
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
         """本接口（CreateSecurityGroupPolicies）用于创建安全组规则（SecurityGroupPolicy）。
 
         在 SecurityGroupPolicySet 参数中：
         <ul>
@@ -1333,15 +1333,15 @@
             model = models.CreateSecurityGroupPoliciesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSecurityGroupWithPolicies(self, request):
         """本接口（CreateSecurityGroupWithPolicies）用于创建新的安全组（SecurityGroup），并且可以同时添加安全组规则（SecurityGroupPolicy）。
         * 每个账户下每个地域的每个项目的<a href="https://cloud.tencent.com/document/product/213/12453">安全组数量限制</a>。
         * 新建的安全组的入站和出站规则默认都是全部拒绝，在创建后通常您需要再调用<a href="https://cloud.tencent.com/document/product/215/15807">CreateSecurityGroupPolicies</a>
         将安全组的规则设置为需要的规则。
@@ -1370,15 +1370,15 @@
             model = models.CreateSecurityGroupWithPoliciesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateServiceTemplate(self, request):
         """本接口（CreateServiceTemplate）用于创建协议端口模板。
 
         :param request: Request instance for CreateServiceTemplate.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateServiceTemplateRequest`
@@ -1393,15 +1393,15 @@
             model = models.CreateServiceTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateServiceTemplateGroup(self, request):
         """本接口（CreateServiceTemplateGroup）用于创建协议端口模板集合。
 
         :param request: Request instance for CreateServiceTemplateGroup.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateServiceTemplateGroupRequest`
@@ -1416,15 +1416,15 @@
             model = models.CreateServiceTemplateGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSnapshotPolicies(self, request):
         """本接口（CreateSnapshotPolicies）用于创建快照策略。
 
         :param request: Request instance for CreateSnapshotPolicies.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateSnapshotPoliciesRequest`
@@ -1439,15 +1439,15 @@
             model = models.CreateSnapshotPoliciesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSubnet(self, request):
         """本接口（CreateSubnet）用于创建子网。
         * 创建子网前必须创建好 VPC。
         * 子网创建成功后，子网网段不能修改。子网网段必须在VPC网段内，可以和VPC网段相同（VPC有且只有一个子网时），建议子网网段在VPC网段内，预留网段给其他子网使用。
         * 您可以创建的最小网段子网掩码为28（有16个IP地址），最大网段子网掩码为16（65,536个IP地址）。
@@ -1468,15 +1468,15 @@
             model = models.CreateSubnetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSubnets(self, request):
         """本接口（CreateSubnets）用于批量创建子网。
         * 创建子网前必须创建好 VPC。
         * 子网创建成功后，子网网段不能修改。子网网段必须在VPC网段内，可以和VPC网段相同（VPC有且只有一个子网时），建议子网网段在VPC网段内，预留网段给其他子网使用。
         * 您可以创建的最小网段子网掩码为28（有16个IP地址），最大网段子网掩码为16（65,536个IP地址）。
@@ -1497,15 +1497,15 @@
             model = models.CreateSubnetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTrafficPackages(self, request):
         """本接口 (CreateTrafficPackages) 用于创建共享流量包。
 
         :param request: Request instance for CreateTrafficPackages.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateTrafficPackagesRequest`
@@ -1520,15 +1520,15 @@
             model = models.CreateTrafficPackagesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVpc(self, request):
         """本接口（CreateVpc）用于创建私有网络（VPC）。
         * 用户可以创建的最小网段子网掩码为28（有16个IP地址），10.0.0.0/12，172.16.0.0/12最大网段子网掩码为12（1,048,576个IP地址），192.168.0.0/16最大网段子网掩码为16（65,536个IP地址）如果需要规划VPC网段请参见[网络规划](https://cloud.tencent.com/document/product/215/30313)。
         * 同一个地域能创建的VPC资源个数也是有限制的，详见 <a href="https://cloud.tencent.com/doc/product/215/537" title="VPC使用限制">VPC使用限制</a>，如果需要申请更多资源，请提交[工单申请](https://console.cloud.tencent.com/workorder/category)。
         * 创建VPC同时可以绑定标签, 应答里的标签列表代表添加成功的标签。
@@ -1546,15 +1546,15 @@
             model = models.CreateVpcResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVpcEndPoint(self, request):
         """本接口（CreateVpcEndPoint）用于创建终端节点。
 
         :param request: Request instance for CreateVpcEndPoint.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateVpcEndPointRequest`
@@ -1569,15 +1569,15 @@
             model = models.CreateVpcEndPointResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVpcEndPointService(self, request):
         """本接口（CreateVpcEndPointService）用于创建终端节点服务。
 
         :param request: Request instance for CreateVpcEndPointService.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateVpcEndPointServiceRequest`
@@ -1592,15 +1592,15 @@
             model = models.CreateVpcEndPointServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVpcEndPointServiceWhiteList(self, request):
         """本接口（CreateVpcEndPointServiceWhiteList）创建终端服务白名单。
 
         :param request: Request instance for CreateVpcEndPointServiceWhiteList.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateVpcEndPointServiceWhiteListRequest`
@@ -1615,15 +1615,15 @@
             model = models.CreateVpcEndPointServiceWhiteListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVpnConnection(self, request):
         """本接口（CreateVpnConnection）用于创建VPN通道。
         >?本接口为异步接口，可调用 [DescribeVpcTaskResult](https://cloud.tencent.com/document/api/215/59037) 接口查询任务执行结果，待任务执行成功后再进行其他操作。
         >
 
@@ -1640,15 +1640,15 @@
             model = models.CreateVpnConnectionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVpnGateway(self, request):
         """本接口（CreateVpnGateway）用于创建VPN网关。
 
         :param request: Request instance for CreateVpnGateway.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateVpnGatewayRequest`
@@ -1663,15 +1663,15 @@
             model = models.CreateVpnGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVpnGatewayRoutes(self, request):
         """创建路由型VPN网关的目的路由
 
         :param request: Request instance for CreateVpnGatewayRoutes.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateVpnGatewayRoutesRequest`
@@ -1686,15 +1686,15 @@
             model = models.CreateVpnGatewayRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVpnGatewaySslClient(self, request):
         """创建SSL-VPN-CLIENT
 
         :param request: Request instance for CreateVpnGatewaySslClient.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateVpnGatewaySslClientRequest`
@@ -1709,15 +1709,15 @@
             model = models.CreateVpnGatewaySslClientResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVpnGatewaySslServer(self, request):
         """本接口（CreateVpnGatewaySslServer）用于创建SSL-VPN Server端。
 
         :param request: Request instance for CreateVpnGatewaySslServer.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateVpnGatewaySslServerRequest`
@@ -1732,15 +1732,15 @@
             model = models.CreateVpnGatewaySslServerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAddressTemplate(self, request):
         """本接口（DeleteAddressTemplate）用于删除IP地址模板。
 
         :param request: Request instance for DeleteAddressTemplate.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteAddressTemplateRequest`
@@ -1755,15 +1755,15 @@
             model = models.DeleteAddressTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAddressTemplateGroup(self, request):
         """本接口（DeleteAddressTemplateGroup）用于删除IP地址模板集合。
 
         :param request: Request instance for DeleteAddressTemplateGroup.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteAddressTemplateGroupRequest`
@@ -1778,15 +1778,15 @@
             model = models.DeleteAddressTemplateGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAssistantCidr(self, request):
         """本接口（DeleteAssistantCidr）用于删除辅助CIDR。
 
         :param request: Request instance for DeleteAssistantCidr.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteAssistantCidrRequest`
@@ -1801,15 +1801,15 @@
             model = models.DeleteAssistantCidrResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteBandwidthPackage(self, request):
         """接口支持删除共享带宽包，包括[设备带宽包](https://cloud.tencent.com/document/product/684/15246#.E8.AE.BE.E5.A4.87.E5.B8.A6.E5.AE.BD.E5.8C.85)和[IP带宽包](https://cloud.tencent.com/document/product/684/15246#ip-.E5.B8.A6.E5.AE.BD.E5.8C.85)
 
         :param request: Request instance for DeleteBandwidthPackage.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteBandwidthPackageRequest`
@@ -1824,15 +1824,15 @@
             model = models.DeleteBandwidthPackageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCcn(self, request):
         """本接口（DeleteCcn）用于删除云联网。
         * 删除后，云联网关联的所有实例间路由将被删除，网络将会中断，请务必确认
         * 删除云联网是不可逆的操作，请谨慎处理。
 
@@ -1849,15 +1849,15 @@
             model = models.DeleteCcnResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCustomerGateway(self, request):
         """本接口（DeleteCustomerGateway）用于删除对端网关。
 
         :param request: Request instance for DeleteCustomerGateway.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteCustomerGatewayRequest`
@@ -1872,15 +1872,15 @@
             model = models.DeleteCustomerGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDhcpIp(self, request):
         """本接口（DeleteDhcpIp）用于删除DhcpIp。
         >?本接口为异步接口，可调用 [DescribeVpcTaskResult](https://cloud.tencent.com/document/api/215/59037) 接口查询任务执行结果，待任务执行成功后再进行其他操作。
         >
 
@@ -1897,15 +1897,15 @@
             model = models.DeleteDhcpIpResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDirectConnectGateway(self, request):
         """本接口（DeleteDirectConnectGateway）用于删除专线网关。
         <li>如果是 NAT 网关，删除专线网关后，NAT 规则以及 ACL 策略都被清理了。</li>
         <li>删除专线网关后，系统会删除路由表中跟该专线网关相关的路由策略。</li>
         本接口是异步完成，如需查询异步任务执行结果，请使用本接口返回的`RequestId`轮询`QueryTask`接口
@@ -1923,15 +1923,15 @@
             model = models.DeleteDirectConnectGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDirectConnectGatewayCcnRoutes(self, request):
         """本接口（DeleteDirectConnectGatewayCcnRoutes）用于删除专线网关的云联网路由（IDC网段）
 
         :param request: Request instance for DeleteDirectConnectGatewayCcnRoutes.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteDirectConnectGatewayCcnRoutesRequest`
@@ -1946,15 +1946,15 @@
             model = models.DeleteDirectConnectGatewayCcnRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteFlowLog(self, request):
         """本接口（DeleteFlowLog）用于删除流日志。
 
         :param request: Request instance for DeleteFlowLog.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteFlowLogRequest`
@@ -1969,15 +1969,15 @@
             model = models.DeleteFlowLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteHaVip(self, request):
         """本接口（DeleteHaVip）用于删除高可用虚拟IP（HAVIP）。<br />
         本接口是异步完成，如需查询异步任务执行结果，请使用本接口返回的`RequestId`轮询`DescribeVpcTaskResult`接口。
 
         :param request: Request instance for DeleteHaVip.
@@ -1993,15 +1993,15 @@
             model = models.DeleteHaVipResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteIp6Translators(self, request):
         """1. 该接口用于释放IPV6转换实例，支持批量。
         2.  如果IPV6转换实例建立有转换规则，会一并删除。
 
         :param request: Request instance for DeleteIp6Translators.
@@ -2017,15 +2017,15 @@
             model = models.DeleteIp6TranslatorsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLocalGateway(self, request):
         """本接口（DeleteLocalGateway）用于删除CDC的本地网关。
 
         :param request: Request instance for DeleteLocalGateway.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteLocalGatewayRequest`
@@ -2040,15 +2040,15 @@
             model = models.DeleteLocalGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteNatGateway(self, request):
         """本接口（DeleteNatGateway）用于删除NAT网关。
         删除 NAT 网关后，系统会自动删除路由表中包含此 NAT 网关的路由项，同时也会解绑弹性公网IP（EIP）。
 
         :param request: Request instance for DeleteNatGateway.
@@ -2064,15 +2064,15 @@
             model = models.DeleteNatGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteNatGatewayDestinationIpPortTranslationNatRule(self, request):
         """本接口（DeleteNatGatewayDestinationIpPortTranslationNatRule）用于删除NAT网关端口转发规则。
 
         :param request: Request instance for DeleteNatGatewayDestinationIpPortTranslationNatRule.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteNatGatewayDestinationIpPortTranslationNatRuleRequest`
@@ -2087,15 +2087,15 @@
             model = models.DeleteNatGatewayDestinationIpPortTranslationNatRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteNatGatewaySourceIpTranslationNatRule(self, request):
         """本接口（DeleteNatGatewaySourceIpTranslationNatRule）用于删除NAT网关端口SNAT转发规则。
 
         :param request: Request instance for DeleteNatGatewaySourceIpTranslationNatRule.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteNatGatewaySourceIpTranslationNatRuleRequest`
@@ -2110,15 +2110,15 @@
             model = models.DeleteNatGatewaySourceIpTranslationNatRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteNetDetect(self, request):
         """本接口（DeleteNetDetect）用于删除网络探测实例。
 
         :param request: Request instance for DeleteNetDetect.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteNetDetectRequest`
@@ -2133,15 +2133,15 @@
             model = models.DeleteNetDetectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteNetworkAcl(self, request):
         """本接口（DeleteNetworkAcl）用于删除网络ACL。
 
         :param request: Request instance for DeleteNetworkAcl.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteNetworkAclRequest`
@@ -2156,15 +2156,15 @@
             model = models.DeleteNetworkAclResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteNetworkAclQuintupleEntries(self, request):
         """本接口（DeleteNetworkAclQuintupleEntries）用于删除网络ACL五元组指定的入站规则和出站规则（但不是全量删除该ACL下的所有条目）。在NetworkAclQuintupleEntrySet参数中：NetworkAclQuintupleEntry需要提供NetworkAclQuintupleEntryId。
 
         :param request: Request instance for DeleteNetworkAclQuintupleEntries.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteNetworkAclQuintupleEntriesRequest`
@@ -2179,15 +2179,15 @@
             model = models.DeleteNetworkAclQuintupleEntriesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteNetworkInterface(self, request):
         """本接口（DeleteNetworkInterface）用于删除弹性网卡。
         * 弹性网卡上绑定了云服务器时，不能被删除。
         * 删除指定弹性网卡，弹性网卡必须先和子机解绑才能删除。删除之后弹性网卡上所有内网IP都将被退还。
 
@@ -2206,15 +2206,15 @@
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
         """本接口（DeleteRouteTable）用于删除路由表。
 
         :param request: Request instance for DeleteRouteTable.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteRouteTableRequest`
@@ -2229,15 +2229,15 @@
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
         """本接口(DeleteRoutes)用于对某个路由表批量删除路由策略（Route）。
 
         :param request: Request instance for DeleteRoutes.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteRoutesRequest`
@@ -2252,15 +2252,15 @@
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
         """本接口（DeleteSecurityGroup）用于删除安全组（SecurityGroup）。
         * 只有当前账号下的安全组允许被删除。
         * 安全组实例ID如果在其他安全组的规则中被引用，则无法直接删除。这种情况下，需要先进行规则修改，再删除安全组。
         * 删除的安全组无法再找回，请谨慎调用。
@@ -2278,15 +2278,15 @@
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
         """本接口（DeleteSecurityGroupPolicies）用于用于删除安全组规则（SecurityGroupPolicy）。
         * SecurityGroupPolicySet.Version 用于指定要操作的安全组的版本。传入 Version 版本号若不等于当前安全组的最新版本，将返回失败；若不传 Version 则直接删除指定PolicyIndex的规则。
 
         :param request: Request instance for DeleteSecurityGroupPolicies.
@@ -2302,15 +2302,15 @@
             model = models.DeleteSecurityGroupPoliciesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteServiceTemplate(self, request):
         """本接口（DeleteServiceTemplate）用于删除协议端口模板。
 
         :param request: Request instance for DeleteServiceTemplate.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteServiceTemplateRequest`
@@ -2325,15 +2325,15 @@
             model = models.DeleteServiceTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteServiceTemplateGroup(self, request):
         """本接口（DeleteServiceTemplateGroup）用于删除协议端口模板集合。
 
         :param request: Request instance for DeleteServiceTemplateGroup.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteServiceTemplateGroupRequest`
@@ -2348,15 +2348,15 @@
             model = models.DeleteServiceTemplateGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSnapshotPolicies(self, request):
         """本接口（DeleteSnapshotPolicies）用于删除快照策略。
 
         :param request: Request instance for DeleteSnapshotPolicies.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteSnapshotPoliciesRequest`
@@ -2371,15 +2371,15 @@
             model = models.DeleteSnapshotPoliciesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSubnet(self, request):
         """本接口（DeleteSubnet）用于删除子网（Subnet）。
         * 删除子网前，请清理该子网下所有资源，包括云服务器、负载均衡、云数据、NoSQL、弹性网卡等资源。
 
         :param request: Request instance for DeleteSubnet.
@@ -2395,15 +2395,15 @@
             model = models.DeleteSubnetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTemplateMember(self, request):
         """删除模板对象中的IP地址、协议端口、IP地址组、协议端口组。当前仅支持北京、泰国、北美地域请求。
 
         :param request: Request instance for DeleteTemplateMember.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteTemplateMemberRequest`
@@ -2418,15 +2418,15 @@
             model = models.DeleteTemplateMemberResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTrafficPackages(self, request):
         """删除共享带宽包（仅非活动状态的流量包可删除）。
 
         :param request: Request instance for DeleteTrafficPackages.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteTrafficPackagesRequest`
@@ -2441,15 +2441,15 @@
             model = models.DeleteTrafficPackagesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteVpc(self, request):
         """本接口（DeleteVpc）用于删除私有网络。
         * 删除前请确保 VPC 内已经没有相关资源，例如云服务器、云数据库、NoSQL、VPN网关、专线网关、负载均衡、对等连接、与之互通的基础网络设备等。
         * 删除私有网络是不可逆的操作，请谨慎处理。
 
@@ -2466,15 +2466,15 @@
             model = models.DeleteVpcResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteVpcEndPoint(self, request):
         """本接口（DeleteVpcEndPoint）用于删除终端节点。
 
         :param request: Request instance for DeleteVpcEndPoint.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteVpcEndPointRequest`
@@ -2489,15 +2489,15 @@
             model = models.DeleteVpcEndPointResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteVpcEndPointService(self, request):
         """本接口（DeleteVpcEndPointService）用于删除终端节点服务。
 
         :param request: Request instance for DeleteVpcEndPointService.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteVpcEndPointServiceRequest`
@@ -2512,15 +2512,15 @@
             model = models.DeleteVpcEndPointServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteVpcEndPointServiceWhiteList(self, request):
         """本接口（DeleteVpcEndPointServiceWhiteList）用于删除终端节点服务白名单。
 
         :param request: Request instance for DeleteVpcEndPointServiceWhiteList.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteVpcEndPointServiceWhiteListRequest`
@@ -2535,15 +2535,15 @@
             model = models.DeleteVpcEndPointServiceWhiteListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteVpnConnection(self, request):
         """本接口（DeleteVpnConnection）用于删除VPN通道。
 
         :param request: Request instance for DeleteVpnConnection.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteVpnConnectionRequest`
@@ -2558,15 +2558,15 @@
             model = models.DeleteVpnConnectionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteVpnGateway(self, request):
         """本接口（DeleteVpnGateway）用于删除VPN网关。目前只支持删除运行中的按量计费的IPSEC网关实例。
 
         :param request: Request instance for DeleteVpnGateway.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteVpnGatewayRequest`
@@ -2581,15 +2581,15 @@
             model = models.DeleteVpnGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteVpnGatewayRoutes(self, request):
         """本接口（DeleteVpnGatewayRoutes）用于删除VPN网关路由
 
         :param request: Request instance for DeleteVpnGatewayRoutes.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteVpnGatewayRoutesRequest`
@@ -2604,15 +2604,15 @@
             model = models.DeleteVpnGatewayRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteVpnGatewaySslClient(self, request):
         """本接口（DeleteVpnGatewaySslClient）用于删除SSL-VPN-CLIENT。
 
         :param request: Request instance for DeleteVpnGatewaySslClient.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteVpnGatewaySslClientRequest`
@@ -2627,15 +2627,15 @@
             model = models.DeleteVpnGatewaySslClientResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteVpnGatewaySslServer(self, request):
         """删除SSL-VPN-SERVER 实例
 
         :param request: Request instance for DeleteVpnGatewaySslServer.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteVpnGatewaySslServerRequest`
@@ -2650,15 +2650,15 @@
             model = models.DeleteVpnGatewaySslServerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccountAttributes(self, request):
         """本接口（DescribeAccountAttributes）用于查询用户账号私有属性。
 
         :param request: Request instance for DescribeAccountAttributes.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeAccountAttributesRequest`
@@ -2673,15 +2673,15 @@
             model = models.DescribeAccountAttributesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAddressQuota(self, request):
         """本接口 (DescribeAddressQuota) 用于查询您账户的[弹性公网IP](https://cloud.tencent.com/document/product/213/1941)（简称 EIP）在当前地域的配额信息。配额详情可参见 [EIP 产品简介](https://cloud.tencent.com/document/product/213/5733)。
 
         :param request: Request instance for DescribeAddressQuota.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeAddressQuotaRequest`
@@ -2696,15 +2696,15 @@
             model = models.DescribeAddressQuotaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAddressTemplateGroups(self, request):
         """本接口（DescribeAddressTemplateGroups）用于查询IP地址模板集合。
 
         :param request: Request instance for DescribeAddressTemplateGroups.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeAddressTemplateGroupsRequest`
@@ -2719,15 +2719,15 @@
             model = models.DescribeAddressTemplateGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAddressTemplates(self, request):
         """本接口（DescribeAddressTemplates）用于查询IP地址模板。
 
         :param request: Request instance for DescribeAddressTemplates.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeAddressTemplatesRequest`
@@ -2742,15 +2742,15 @@
             model = models.DescribeAddressTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAddresses(self, request):
         """本接口 (DescribeAddresses) 用于查询一个或多个[弹性公网IP](https://cloud.tencent.com/document/product/213/1941)（简称 EIP）的详细信息。
         * 如果参数为空，返回当前用户一定数量（Limit所指定的数量，默认为20）的 EIP。
 
         :param request: Request instance for DescribeAddresses.
@@ -2766,15 +2766,15 @@
             model = models.DescribeAddressesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssistantCidr(self, request):
         """本接口（DescribeAssistantCidr）用于查询辅助CIDR列表。
 
         :param request: Request instance for DescribeAssistantCidr.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeAssistantCidrRequest`
@@ -2789,15 +2789,15 @@
             model = models.DescribeAssistantCidrResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBandwidthPackageBillUsage(self, request):
         """本接口 (DescribeBandwidthPackageBillUsage) 用于查询后付费共享带宽包当前的计费用量.
 
         :param request: Request instance for DescribeBandwidthPackageBillUsage.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeBandwidthPackageBillUsageRequest`
@@ -2812,15 +2812,15 @@
             model = models.DescribeBandwidthPackageBillUsageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBandwidthPackageQuota(self, request):
         """接口用于查询账户在当前地域的带宽包上限数量以及使用数量
 
         :param request: Request instance for DescribeBandwidthPackageQuota.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeBandwidthPackageQuotaRequest`
@@ -2835,15 +2835,15 @@
             model = models.DescribeBandwidthPackageQuotaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBandwidthPackageResources(self, request):
         """本接口 (DescribeBandwidthPackageResources) 用于根据共享带宽包唯一ID查询共享带宽包内的资源列表，支持按条件过滤查询结果和分页查询。
 
         :param request: Request instance for DescribeBandwidthPackageResources.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeBandwidthPackageResourcesRequest`
@@ -2858,15 +2858,15 @@
             model = models.DescribeBandwidthPackageResourcesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBandwidthPackages(self, request):
         """接口用于查询带宽包详细信息，包括带宽包唯一标识ID，类型，计费模式，名称，资源信息等
 
         :param request: Request instance for DescribeBandwidthPackages.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeBandwidthPackagesRequest`
@@ -2881,15 +2881,15 @@
             model = models.DescribeBandwidthPackagesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCcnAttachedInstances(self, request):
         """本接口（DescribeCcnAttachedInstances）用于查询云联网实例下已关联的网络实例。
 
         :param request: Request instance for DescribeCcnAttachedInstances.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeCcnAttachedInstancesRequest`
@@ -2904,15 +2904,15 @@
             model = models.DescribeCcnAttachedInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCcnRegionBandwidthLimits(self, request):
         """本接口（DescribeCcnRegionBandwidthLimits）用于查询云联网各地域出带宽上限，该接口只返回已关联网络实例包含的地域。
 
         :param request: Request instance for DescribeCcnRegionBandwidthLimits.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeCcnRegionBandwidthLimitsRequest`
@@ -2927,15 +2927,15 @@
             model = models.DescribeCcnRegionBandwidthLimitsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCcnRoutes(self, request):
         """本接口（DescribeCcnRoutes）用于查询已加入云联网（CCN）的路由。
 
         :param request: Request instance for DescribeCcnRoutes.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeCcnRoutesRequest`
@@ -2950,15 +2950,15 @@
             model = models.DescribeCcnRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCcns(self, request):
         """本接口（DescribeCcns）用于查询云联网（CCN）列表。
 
         :param request: Request instance for DescribeCcns.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeCcnsRequest`
@@ -2973,15 +2973,15 @@
             model = models.DescribeCcnsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClassicLinkInstances(self, request):
         """本接口（DescribeClassicLinkInstances）用于查询私有网络和基础网络设备互通列表。
 
         :param request: Request instance for DescribeClassicLinkInstances.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeClassicLinkInstancesRequest`
@@ -2996,15 +2996,15 @@
             model = models.DescribeClassicLinkInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCrossBorderCcnRegionBandwidthLimits(self, request):
         """本接口（DescribeCrossBorderCcnRegionBandwidthLimits）用于获取要锁定的限速实例列表。
         该接口一般用来封禁地域间限速的云联网实例下的限速实例, 目前联通内部运营系统通过云API调用, 如果是出口限速, 一般使用更粗的云联网实例粒度封禁（DescribeTenantCcns）
         如有需要, 可以封禁任意限速实例, 可接入到内部运营系统
 
@@ -3021,15 +3021,15 @@
             model = models.DescribeCrossBorderCcnRegionBandwidthLimitsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCrossBorderCompliance(self, request):
         """本接口（DescribeCrossBorderCompliance）用于查询用户创建的合规化资质审批单。
         服务商可以查询服务名下的任意 `APPID` 创建的审批单；非服务商，只能查询自己审批单。
 
         :param request: Request instance for DescribeCrossBorderCompliance.
@@ -3045,15 +3045,15 @@
             model = models.DescribeCrossBorderComplianceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCrossBorderFlowMonitor(self, request):
         """本接口（DescribeCrossBorderFlowMonitor）用于查询跨境带宽监控数据，该接口目前只提供给服务商联通使用。
 
         :param request: Request instance for DescribeCrossBorderFlowMonitor.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeCrossBorderFlowMonitorRequest`
@@ -3068,15 +3068,15 @@
             model = models.DescribeCrossBorderFlowMonitorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCustomerGatewayVendors(self, request):
         """本接口（DescribeCustomerGatewayVendors）用于查询可支持的对端网关厂商信息。
 
         :param request: Request instance for DescribeCustomerGatewayVendors.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeCustomerGatewayVendorsRequest`
@@ -3091,15 +3091,15 @@
             model = models.DescribeCustomerGatewayVendorsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCustomerGateways(self, request):
         """本接口（DescribeCustomerGateways）用于查询对端网关列表。
 
         :param request: Request instance for DescribeCustomerGateways.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeCustomerGatewaysRequest`
@@ -3114,15 +3114,15 @@
             model = models.DescribeCustomerGatewaysResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDhcpIps(self, request):
         """本接口（DescribeDhcpIps）用于查询DhcpIp列表
 
         :param request: Request instance for DescribeDhcpIps.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeDhcpIpsRequest`
@@ -3137,15 +3137,15 @@
             model = models.DescribeDhcpIpsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDirectConnectGatewayCcnRoutes(self, request):
         """本接口（DescribeDirectConnectGatewayCcnRoutes）用于查询专线网关的云联网路由（IDC网段）
 
         :param request: Request instance for DescribeDirectConnectGatewayCcnRoutes.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeDirectConnectGatewayCcnRoutesRequest`
@@ -3160,15 +3160,15 @@
             model = models.DescribeDirectConnectGatewayCcnRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDirectConnectGateways(self, request):
         """本接口（DescribeDirectConnectGateways）用于查询专线网关。
 
         :param request: Request instance for DescribeDirectConnectGateways.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeDirectConnectGatewaysRequest`
@@ -3183,15 +3183,15 @@
             model = models.DescribeDirectConnectGatewaysResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlowLog(self, request):
         """本接口（DescribeFlowLog）用于查询流日志实例信息。
 
         :param request: Request instance for DescribeFlowLog.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeFlowLogRequest`
@@ -3206,15 +3206,15 @@
             model = models.DescribeFlowLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlowLogs(self, request):
         """本接口（DescribeFlowLogs）用于查询获取流日志集合。
 
         :param request: Request instance for DescribeFlowLogs.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeFlowLogsRequest`
@@ -3229,15 +3229,15 @@
             model = models.DescribeFlowLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGatewayFlowMonitorDetail(self, request):
         """本接口（DescribeGatewayFlowMonitorDetail）用于查询网关流量监控明细。
         * 只支持单个网关实例查询。即入参 `VpnId`、 `DirectConnectGatewayId`、 `PeeringConnectionId`、 `NatId` 最多只支持传一个，且必须传一个。
         * 如果网关有流量，但调用本接口没有返回数据，请在控制台对应网关详情页确认是否开启网关流量监控。
 
@@ -3254,15 +3254,15 @@
             model = models.DescribeGatewayFlowMonitorDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGatewayFlowQos(self, request):
         """本接口（DescribeGatewayFlowQos）用于查询网关来访IP流控带宽。
 
         :param request: Request instance for DescribeGatewayFlowQos.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeGatewayFlowQosRequest`
@@ -3277,15 +3277,15 @@
             model = models.DescribeGatewayFlowQosResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHaVips(self, request):
         """本接口（DescribeHaVips）用于查询高可用虚拟IP（HAVIP）列表。
 
         :param request: Request instance for DescribeHaVips.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeHaVipsRequest`
@@ -3300,15 +3300,15 @@
             model = models.DescribeHaVipsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIp6Addresses(self, request):
         """该接口用于查询IPV6地址信息
 
         :param request: Request instance for DescribeIp6Addresses.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeIp6AddressesRequest`
@@ -3323,15 +3323,15 @@
             model = models.DescribeIp6AddressesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIp6TranslatorQuota(self, request):
         """查询账户在指定地域IPV6转换实例和规则的配额
 
         :param request: Request instance for DescribeIp6TranslatorQuota.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeIp6TranslatorQuotaRequest`
@@ -3346,15 +3346,15 @@
             model = models.DescribeIp6TranslatorQuotaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIp6Translators(self, request):
         """1. 该接口用于查询账户下的IPV6转换实例及其绑定的转换规则信息
         2. 支持过滤查询
 
         :param request: Request instance for DescribeIp6Translators.
@@ -3370,15 +3370,15 @@
             model = models.DescribeIp6TranslatorsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIpGeolocationDatabaseUrl(self, request):
         """本接口（DescribeIpGeolocationDatabaseUrl）用于获取IP地理位置库下载链接。
         <font color="#FF0000">本接口即将下线，仅供存量用户使用，暂停新增用户。</font>
 
         :param request: Request instance for DescribeIpGeolocationDatabaseUrl.
@@ -3394,15 +3394,15 @@
             model = models.DescribeIpGeolocationDatabaseUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIpGeolocationInfos(self, request):
         """本接口（DescribeIpGeolocationInfos）用于查询IP地址信息，包括地理位置信息和网络信息。
         <font color="#FF0000">本接口即将下线，仅供存量客户使用，暂停新增用户。</font>
 
         :param request: Request instance for DescribeIpGeolocationInfos.
@@ -3418,15 +3418,15 @@
             model = models.DescribeIpGeolocationInfosResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLocalGateway(self, request):
         """本接口（DescribeLocalGateway）用于查询CDC的本地网关。
 
         :param request: Request instance for DescribeLocalGateway.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeLocalGatewayRequest`
@@ -3441,15 +3441,15 @@
             model = models.DescribeLocalGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNatGatewayDestinationIpPortTranslationNatRules(self, request):
         """本接口（DescribeNatGatewayDestinationIpPortTranslationNatRules）用于查询NAT网关端口转发规则对象数组。
 
         :param request: Request instance for DescribeNatGatewayDestinationIpPortTranslationNatRules.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeNatGatewayDestinationIpPortTranslationNatRulesRequest`
@@ -3464,15 +3464,15 @@
             model = models.DescribeNatGatewayDestinationIpPortTranslationNatRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNatGatewayDirectConnectGatewayRoute(self, request):
         """查询专线绑定NAT的路由
 
         :param request: Request instance for DescribeNatGatewayDirectConnectGatewayRoute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeNatGatewayDirectConnectGatewayRouteRequest`
@@ -3487,15 +3487,15 @@
             model = models.DescribeNatGatewayDirectConnectGatewayRouteResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNatGatewaySourceIpTranslationNatRules(self, request):
         """本接口（DescribeNatGatewaySourceIpTranslationNatRules）用于查询NAT网关SNAT转发规则对象数组。
 
         :param request: Request instance for DescribeNatGatewaySourceIpTranslationNatRules.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeNatGatewaySourceIpTranslationNatRulesRequest`
@@ -3510,15 +3510,15 @@
             model = models.DescribeNatGatewaySourceIpTranslationNatRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNatGateways(self, request):
         """本接口（DescribeNatGateways）用于查询 NAT 网关。
 
         :param request: Request instance for DescribeNatGateways.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeNatGatewaysRequest`
@@ -3533,15 +3533,15 @@
             model = models.DescribeNatGatewaysResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNetDetectStates(self, request):
         """本接口(DescribeNetDetectStates)用于查询网络探测验证结果列表。
 
         :param request: Request instance for DescribeNetDetectStates.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeNetDetectStatesRequest`
@@ -3556,15 +3556,15 @@
             model = models.DescribeNetDetectStatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNetDetects(self, request):
         """本接口（DescribeNetDetects）用于查询网络探测列表。
 
         :param request: Request instance for DescribeNetDetects.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeNetDetectsRequest`
@@ -3579,15 +3579,15 @@
             model = models.DescribeNetDetectsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNetworkAccountType(self, request):
         """判断用户在网络侧的用户类型，如标准（带宽上移），传统（非上移）。
 
         :param request: Request instance for DescribeNetworkAccountType.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeNetworkAccountTypeRequest`
@@ -3602,15 +3602,15 @@
             model = models.DescribeNetworkAccountTypeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNetworkAclQuintupleEntries(self, request):
         """本接口（DescribeNetworkAclQuintupleEntries）查询入方向或出方向网络ACL五元组条目列表。
 
         :param request: Request instance for DescribeNetworkAclQuintupleEntries.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeNetworkAclQuintupleEntriesRequest`
@@ -3625,15 +3625,15 @@
             model = models.DescribeNetworkAclQuintupleEntriesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNetworkAcls(self, request):
         """本接口（DescribeNetworkAcls）用于查询网络ACL列表。
 
         :param request: Request instance for DescribeNetworkAcls.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeNetworkAclsRequest`
@@ -3648,15 +3648,15 @@
             model = models.DescribeNetworkAclsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNetworkInterfaceLimit(self, request):
         """本接口（DescribeNetworkInterfaceLimit）根据CVM实例ID或弹性网卡ID查询弹性网卡配额，返回该CVM实例或弹性网卡能绑定的弹性网卡配额，以及弹性网卡可以分配的IP配额。
 
         :param request: Request instance for DescribeNetworkInterfaceLimit.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeNetworkInterfaceLimitRequest`
@@ -3671,15 +3671,15 @@
             model = models.DescribeNetworkInterfaceLimitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNetworkInterfaces(self, request):
         """本接口（DescribeNetworkInterfaces）用于查询弹性网卡列表。
 
         :param request: Request instance for DescribeNetworkInterfaces.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeNetworkInterfacesRequest`
@@ -3694,15 +3694,15 @@
             model = models.DescribeNetworkInterfacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProductQuota(self, request):
         """本接口（DescribeProductQuota）用于查询网络产品的配额信息。
 
         :param request: Request instance for DescribeProductQuota.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeProductQuotaRequest`
@@ -3717,15 +3717,15 @@
             model = models.DescribeProductQuotaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRouteConflicts(self, request):
         """本接口（DescribeRouteConflicts）用于查询自定义路由策略与云联网路由策略冲突列表。
 
         :param request: Request instance for DescribeRouteConflicts.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeRouteConflictsRequest`
@@ -3740,15 +3740,15 @@
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
         """本接口（DescribeRouteTables）用于查询路由表。
 
         :param request: Request instance for DescribeRouteTables.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeRouteTablesRequest`
@@ -3763,15 +3763,15 @@
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
         """本接口（DescribeSecurityGroupAssociationStatistics）用于查询安全组关联的实例统计。
 
         :param request: Request instance for DescribeSecurityGroupAssociationStatistics.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeSecurityGroupAssociationStatisticsRequest`
@@ -3786,15 +3786,15 @@
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
         """本接口(DescribeSecurityGroupLimits)用于查询用户安全组配额。
 
         :param request: Request instance for DescribeSecurityGroupLimits.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeSecurityGroupLimitsRequest`
@@ -3809,15 +3809,15 @@
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
         """本接口（DescribeSecurityGroupPolicies）用于查询安全组规则。
 
         :param request: Request instance for DescribeSecurityGroupPolicies.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeSecurityGroupPoliciesRequest`
@@ -3832,15 +3832,15 @@
             model = models.DescribeSecurityGroupPoliciesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecurityGroupReferences(self, request):
         """本接口（DescribeSecurityGroupReferences）用于查询安全组被引用信息。
 
         :param request: Request instance for DescribeSecurityGroupReferences.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeSecurityGroupReferencesRequest`
@@ -3855,15 +3855,15 @@
             model = models.DescribeSecurityGroupReferencesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecurityGroups(self, request):
         """本接口（DescribeSecurityGroups）用于查询安全组。
 
         :param request: Request instance for DescribeSecurityGroups.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeSecurityGroupsRequest`
@@ -3878,15 +3878,15 @@
             model = models.DescribeSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeServiceTemplateGroups(self, request):
         """本接口（DescribeServiceTemplateGroups）用于查询协议端口模板集合。
 
         :param request: Request instance for DescribeServiceTemplateGroups.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeServiceTemplateGroupsRequest`
@@ -3901,15 +3901,15 @@
             model = models.DescribeServiceTemplateGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeServiceTemplates(self, request):
         """本接口（DescribeServiceTemplates）用于查询协议端口模板。
 
         :param request: Request instance for DescribeServiceTemplates.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeServiceTemplatesRequest`
@@ -3924,15 +3924,15 @@
             model = models.DescribeServiceTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSgSnapshotFileContent(self, request):
         """本接口（DescribeSgSnapshotFileContent）用于查询安全组快照文件内容。
 
         :param request: Request instance for DescribeSgSnapshotFileContent.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeSgSnapshotFileContentRequest`
@@ -3947,15 +3947,15 @@
             model = models.DescribeSgSnapshotFileContentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSnapshotAttachedInstances(self, request):
         """本接口（DescribeSnapshotAttachedInstances）用于查询快照策略关联实例列表。
 
         :param request: Request instance for DescribeSnapshotAttachedInstances.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeSnapshotAttachedInstancesRequest`
@@ -3970,15 +3970,15 @@
             model = models.DescribeSnapshotAttachedInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSnapshotFiles(self, request):
         """本接口（DescribeSnapshotFiles）用于查询快照文件。
 
         :param request: Request instance for DescribeSnapshotFiles.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeSnapshotFilesRequest`
@@ -3993,15 +3993,15 @@
             model = models.DescribeSnapshotFilesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSnapshotPolicies(self, request):
         """本接口（DescribeSnapshotPolicies）用于查询快照策略。
 
         :param request: Request instance for DescribeSnapshotPolicies.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeSnapshotPoliciesRequest`
@@ -4016,15 +4016,15 @@
             model = models.DescribeSnapshotPoliciesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSubnetResourceDashboard(self, request):
         """本接口(DescribeSubnetResourceDashboard)用于查看Subnet资源信息。
 
         :param request: Request instance for DescribeSubnetResourceDashboard.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeSubnetResourceDashboardRequest`
@@ -4039,15 +4039,15 @@
             model = models.DescribeSubnetResourceDashboardResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSubnets(self, request):
         """本接口（DescribeSubnets）用于查询子网列表。
 
         :param request: Request instance for DescribeSubnets.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeSubnetsRequest`
@@ -4062,15 +4062,15 @@
             model = models.DescribeSubnetsResponse()
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
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeTaskResultRequest`
@@ -4085,15 +4085,15 @@
             model = models.DescribeTaskResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTemplateLimits(self, request):
         """本接口（DescribeTemplateLimits）用于查询参数模板配额列表。
 
         :param request: Request instance for DescribeTemplateLimits.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeTemplateLimitsRequest`
@@ -4108,15 +4108,15 @@
             model = models.DescribeTemplateLimitsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTenantCcns(self, request):
         """本接口（DescribeTenantCcns）用于获取要锁定的云联网实例列表。
         该接口一般用来封禁出口限速的云联网实例, 目前联通内部运营系统通过云API调用, 因为出口限速无法按地域间封禁, 只能按更粗的云联网实例粒度封禁, 如果是地域间限速, 一般可以通过更细的限速实例粒度封禁（DescribeCrossBorderCcnRegionBandwidthLimits）
         如有需要, 可以封禁任意云联网实例, 可接入到内部运营系统
 
@@ -4133,15 +4133,15 @@
             model = models.DescribeTenantCcnsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTrafficPackages(self, request):
         """本接口 (DescribeTrafficPackages)  用于查询共享流量包详细信息，包括共享流量包唯一标识ID，名称，流量使用信息等
 
         :param request: Request instance for DescribeTrafficPackages.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeTrafficPackagesRequest`
@@ -4156,15 +4156,15 @@
             model = models.DescribeTrafficPackagesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUsedIpAddress(self, request):
         """本接口(DescribeUsedIpAddress)用于查询Subnet或者Vpc内的ip的使用情况，
         如ip被占用，返回占用ip的资源类别与id；如未被占用，返回空值
 
         :param request: Request instance for DescribeUsedIpAddress.
@@ -4180,15 +4180,15 @@
             model = models.DescribeUsedIpAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVpcEndPoint(self, request):
         """本接口（DescribeVpcEndPoint）用于查询终端节点列表。
 
         :param request: Request instance for DescribeVpcEndPoint.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeVpcEndPointRequest`
@@ -4203,15 +4203,15 @@
             model = models.DescribeVpcEndPointResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVpcEndPointService(self, request):
         """查询终端节点服务列表。
 
         :param request: Request instance for DescribeVpcEndPointService.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeVpcEndPointServiceRequest`
@@ -4226,15 +4226,15 @@
             model = models.DescribeVpcEndPointServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVpcEndPointServiceWhiteList(self, request):
         """本接口（DescribeVpcEndPointServiceWhiteList）用于查询终端节点服务的服务白名单列表。
 
         :param request: Request instance for DescribeVpcEndPointServiceWhiteList.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeVpcEndPointServiceWhiteListRequest`
@@ -4249,15 +4249,15 @@
             model = models.DescribeVpcEndPointServiceWhiteListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVpcInstances(self, request):
         """本接口（DescribeVpcInstances）用于查询VPC下的云主机实例列表。
 
         :param request: Request instance for DescribeVpcInstances.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeVpcInstancesRequest`
@@ -4272,15 +4272,15 @@
             model = models.DescribeVpcInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVpcIpv6Addresses(self, request):
         """本接口（DescribeVpcIpv6Addresses）用于查询 `VPC` `IPv6` 信息。
         只能查询已使用的`IPv6`信息，当查询未使用的IP时，本接口不会报错，但不会出现在返回结果里。
 
         :param request: Request instance for DescribeVpcIpv6Addresses.
@@ -4296,15 +4296,15 @@
             model = models.DescribeVpcIpv6AddressesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVpcLimits(self, request):
         """本接口（DescribeVpcLimits）用于获取私有网络配额，部分私有网络的配额有地域属性。
         LimitTypes取值范围：
         * appid-max-vpcs （每个开发商每个地域可创建的VPC数）。
         * vpc-max-subnets（每个VPC可创建的子网数）。
@@ -4350,15 +4350,15 @@
             model = models.DescribeVpcLimitsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVpcPrivateIpAddresses(self, request):
         """本接口（DescribeVpcPrivateIpAddresses）用于查询VPC内网IP信息。<br />
         只能查询已使用的IP信息，当查询未使用的IP时，本接口不会报错，但不会出现在返回结果里。
 
         :param request: Request instance for DescribeVpcPrivateIpAddresses.
@@ -4374,15 +4374,15 @@
             model = models.DescribeVpcPrivateIpAddressesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVpcResourceDashboard(self, request):
         """本接口(DescribeVpcResourceDashboard)用于查看VPC资源信息。
 
         :param request: Request instance for DescribeVpcResourceDashboard.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeVpcResourceDashboardRequest`
@@ -4397,15 +4397,15 @@
             model = models.DescribeVpcResourceDashboardResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVpcTaskResult(self, request):
         """本接口（DescribeVpcTaskResult）用于查询VPC任务执行结果。
 
         :param request: Request instance for DescribeVpcTaskResult.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeVpcTaskResultRequest`
@@ -4420,15 +4420,15 @@
             model = models.DescribeVpcTaskResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVpcs(self, request):
         """本接口（DescribeVpcs）用于查询私有网络列表。
 
         :param request: Request instance for DescribeVpcs.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeVpcsRequest`
@@ -4443,15 +4443,15 @@
             model = models.DescribeVpcsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVpnConnections(self, request):
         """本接口（DescribeVpnConnections）用于查询VPN通道列表。
 
         :param request: Request instance for DescribeVpnConnections.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeVpnConnectionsRequest`
@@ -4466,15 +4466,15 @@
             model = models.DescribeVpnConnectionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVpnGatewayCcnRoutes(self, request):
         """本接口（DescribeVpnGatewayCcnRoutes）用于查询VPN网关云联网路由。
 
         :param request: Request instance for DescribeVpnGatewayCcnRoutes.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeVpnGatewayCcnRoutesRequest`
@@ -4489,15 +4489,15 @@
             model = models.DescribeVpnGatewayCcnRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVpnGatewayRoutes(self, request):
         """本接口（DescribeVpnGatewayRoutes）用于查询VPN网关路由。
 
         :param request: Request instance for DescribeVpnGatewayRoutes.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeVpnGatewayRoutesRequest`
@@ -4512,15 +4512,15 @@
             model = models.DescribeVpnGatewayRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVpnGatewaySslClients(self, request):
         """本接口（DescribeVpnGatewaySslClients）用于查询SSL-VPN-CLIENT 列表。
 
         :param request: Request instance for DescribeVpnGatewaySslClients.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeVpnGatewaySslClientsRequest`
@@ -4535,15 +4535,15 @@
             model = models.DescribeVpnGatewaySslClientsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVpnGatewaySslServers(self, request):
         """本接口（DescribeVpnGatewaySslServers）用于查询SSL-VPN SERVER 列表信息。
 
         :param request: Request instance for DescribeVpnGatewaySslServers.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeVpnGatewaySslServersRequest`
@@ -4558,15 +4558,15 @@
             model = models.DescribeVpnGatewaySslServersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVpnGateways(self, request):
         """本接口（DescribeVpnGateways）用于查询VPN网关列表。
 
         :param request: Request instance for DescribeVpnGateways.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeVpnGatewaysRequest`
@@ -4581,15 +4581,15 @@
             model = models.DescribeVpnGatewaysResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetachCcnInstances(self, request):
         """本接口（DetachCcnInstances）用于从云联网实例中解关联指定的网络实例。<br />
         解关联网络实例后，相应的路由策略会一并删除。
 
         :param request: Request instance for DetachCcnInstances.
@@ -4605,15 +4605,15 @@
             model = models.DetachCcnInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetachClassicLinkVpc(self, request):
         """本接口(DetachClassicLinkVpc)用于删除私有网络和基础网络设备互通。
         >?本接口为异步接口，可调用 [DescribeVpcTaskResult](https://cloud.tencent.com/document/api/215/59037) 接口查询任务执行结果，待任务执行成功后再进行其他操作。
         >
 
@@ -4630,15 +4630,15 @@
             model = models.DetachClassicLinkVpcResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetachNetworkInterface(self, request):
         """本接口（DetachNetworkInterface）用于弹性网卡解绑云服务器。
         本接口是异步完成，如需查询异步任务执行结果，请使用本接口返回的`RequestId`轮询`DescribeVpcTaskResult`接口。
 
         :param request: Request instance for DetachNetworkInterface.
@@ -4654,15 +4654,15 @@
             model = models.DetachNetworkInterfaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetachSnapshotInstances(self, request):
         """本接口（DetachSnapshotInstances）用于快照策略解关联实例。
 
         :param request: Request instance for DetachSnapshotInstances.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DetachSnapshotInstancesRequest`
@@ -4677,15 +4677,15 @@
             model = models.DetachSnapshotInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableCcnRoutes(self, request):
         """本接口（DisableCcnRoutes）用于禁用已经启用的云联网（CCN）路由。
 
         :param request: Request instance for DisableCcnRoutes.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DisableCcnRoutesRequest`
@@ -4700,15 +4700,15 @@
             model = models.DisableCcnRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableFlowLogs(self, request):
         """本接口（DisableFlowLogs）用于停止流日志。
 
         :param request: Request instance for DisableFlowLogs.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DisableFlowLogsRequest`
@@ -4723,15 +4723,15 @@
             model = models.DisableFlowLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableGatewayFlowMonitor(self, request):
         """本接口（DisableGatewayFlowMonitor）用于关闭网关流量监控。
 
         :param request: Request instance for DisableGatewayFlowMonitor.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DisableGatewayFlowMonitorRequest`
@@ -4746,15 +4746,15 @@
             model = models.DisableGatewayFlowMonitorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableRoutes(self, request):
         """本接口（DisableRoutes）用于禁用已启用的子网路由
 
         :param request: Request instance for DisableRoutes.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DisableRoutesRequest`
@@ -4769,15 +4769,15 @@
             model = models.DisableRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableSnapshotPolicies(self, request):
         """本接口（DisableSnapshotPolicies）用于停用快照策略。
 
         :param request: Request instance for DisableSnapshotPolicies.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DisableSnapshotPoliciesRequest`
@@ -4792,15 +4792,15 @@
             model = models.DisableSnapshotPoliciesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableVpnGatewaySslClientCert(self, request):
         """禁用SSL-VPN-CLIENT 证书
 
         :param request: Request instance for DisableVpnGatewaySslClientCert.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DisableVpnGatewaySslClientCertRequest`
@@ -4815,15 +4815,15 @@
             model = models.DisableVpnGatewaySslClientCertResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisassociateAddress(self, request):
         """本接口 (DisassociateAddress) 用于解绑[弹性公网IP](https://cloud.tencent.com/document/product/213/1941)（简称 EIP）。
         * 支持CVM实例，弹性网卡上的EIP解绑
         * 不支持NAT上的EIP解绑。NAT上的EIP解绑请参考[DisassociateNatGatewayAddress](https://cloud.tencent.com/document/api/215/36716)
         * 只有状态为 BIND 和 BIND_ENI 的 EIP 才能进行解绑定操作。
@@ -4842,15 +4842,15 @@
             model = models.DisassociateAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisassociateDhcpIpWithAddressIp(self, request):
         """本接口（DisassociateDhcpIpWithAddressIp）用于将DhcpIp已绑定的弹性公网IP（EIP）解除绑定。<br />
         >?本接口为异步接口，可调用 [DescribeVpcTaskResult](https://cloud.tencent.com/document/api/215/59037) 接口查询任务执行结果，待任务执行成功后再进行其他操作。
         >
 
@@ -4867,15 +4867,15 @@
             model = models.DisassociateDhcpIpWithAddressIpResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisassociateDirectConnectGatewayNatGateway(self, request):
         """将专线网关与NAT网关解绑，解绑之后，专线网关将不能通过NAT网关访问公网
 
         :param request: Request instance for DisassociateDirectConnectGatewayNatGateway.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DisassociateDirectConnectGatewayNatGatewayRequest`
@@ -4890,15 +4890,15 @@
             model = models.DisassociateDirectConnectGatewayNatGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisassociateNatGatewayAddress(self, request):
         """本接口（DisassociateNatGatewayAddress）用于NAT网关解绑弹性IP。
 
         :param request: Request instance for DisassociateNatGatewayAddress.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DisassociateNatGatewayAddressRequest`
@@ -4913,15 +4913,15 @@
             model = models.DisassociateNatGatewayAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisassociateNetworkAclSubnets(self, request):
         """本接口（DisassociateNetworkAclSubnets）用于网络ACL解关联VPC下的子网。
 
         :param request: Request instance for DisassociateNetworkAclSubnets.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DisassociateNetworkAclSubnetsRequest`
@@ -4936,15 +4936,15 @@
             model = models.DisassociateNetworkAclSubnetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisassociateNetworkInterfaceSecurityGroups(self, request):
         """本接口（DisassociateNetworkInterfaceSecurityGroups）用于弹性网卡解绑安全组。支持弹性网卡完全解绑安全组。
 
         :param request: Request instance for DisassociateNetworkInterfaceSecurityGroups.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DisassociateNetworkInterfaceSecurityGroupsRequest`
@@ -4959,15 +4959,15 @@
             model = models.DisassociateNetworkInterfaceSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisassociateVpcEndPointSecurityGroups(self, request):
         """本接口（DisassociateVpcEndPointSecurityGroups）用于终端节点解绑安全组。
 
         :param request: Request instance for DisassociateVpcEndPointSecurityGroups.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DisassociateVpcEndPointSecurityGroupsRequest`
@@ -4982,15 +4982,15 @@
             model = models.DisassociateVpcEndPointSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DownloadCustomerGatewayConfiguration(self, request):
         """本接口（DownloadCustomerGatewayConfiguration）用于下载VPN通道配置。
 
         :param request: Request instance for DownloadCustomerGatewayConfiguration.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DownloadCustomerGatewayConfigurationRequest`
@@ -5005,15 +5005,15 @@
             model = models.DownloadCustomerGatewayConfigurationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DownloadVpnGatewaySslClientCert(self, request):
         """本接口（DownloadVpnGatewaySslClientCert）用于下载SSL-VPN-CLIENT 客户端证书。
 
         :param request: Request instance for DownloadVpnGatewaySslClientCert.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DownloadVpnGatewaySslClientCertRequest`
@@ -5028,15 +5028,15 @@
             model = models.DownloadVpnGatewaySslClientCertResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableCcnRoutes(self, request):
         """本接口（EnableCcnRoutes）用于启用已经加入云联网（CCN）的路由。<br />
         本接口会校验启用后，是否与已有路由冲突，如果冲突，则无法启用，失败处理。路由冲突时，需要先禁用与之冲突的路由，才能启用该路由。
 
         :param request: Request instance for EnableCcnRoutes.
@@ -5052,15 +5052,15 @@
             model = models.EnableCcnRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableFlowLogs(self, request):
         """本接口（EnableFlowLogs）用于启动流日志。
 
         :param request: Request instance for EnableFlowLogs.
         :type request: :class:`tencentcloud.vpc.v20170312.models.EnableFlowLogsRequest`
@@ -5075,15 +5075,15 @@
             model = models.EnableFlowLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableGatewayFlowMonitor(self, request):
         """本接口（EnableGatewayFlowMonitor）用于开启网关流量监控。
 
         :param request: Request instance for EnableGatewayFlowMonitor.
         :type request: :class:`tencentcloud.vpc.v20170312.models.EnableGatewayFlowMonitorRequest`
@@ -5098,15 +5098,15 @@
             model = models.EnableGatewayFlowMonitorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableRoutes(self, request):
         """本接口（EnableRoutes）用于启用已禁用的子网路由。<br />
         本接口会校验启用后，是否与已有路由冲突，如果冲突，则无法启用，失败处理。路由冲突时，需要先禁用与之冲突的路由，才能启用该路由。
 
         :param request: Request instance for EnableRoutes.
@@ -5122,15 +5122,15 @@
             model = models.EnableRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableSnapshotPolicies(self, request):
         """本接口（EnableSnapshotPolicies）用于启用快照策略。
 
         :param request: Request instance for EnableSnapshotPolicies.
         :type request: :class:`tencentcloud.vpc.v20170312.models.EnableSnapshotPoliciesRequest`
@@ -5145,15 +5145,15 @@
             model = models.EnableSnapshotPoliciesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableVpcEndPointConnect(self, request):
         """本接口（EnableVpcEndPointConnect）用于是否接受终端节点连接请求。
 
         :param request: Request instance for EnableVpcEndPointConnect.
         :type request: :class:`tencentcloud.vpc.v20170312.models.EnableVpcEndPointConnectRequest`
@@ -5168,15 +5168,15 @@
             model = models.EnableVpcEndPointConnectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableVpnGatewaySslClientCert(self, request):
         """本接口（EnableVpnGatewaySslClientCert）用于启用SSL-VPN-CLIENT 证书。
 
         :param request: Request instance for EnableVpnGatewaySslClientCert.
         :type request: :class:`tencentcloud.vpc.v20170312.models.EnableVpnGatewaySslClientCertRequest`
@@ -5191,15 +5191,15 @@
             model = models.EnableVpnGatewaySslClientCertResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GenerateVpnConnectionDefaultHealthCheckIp(self, request):
         """本接口（GenerateVpnConnectionDefaultHealthCheckIp）用于获取一对VPN通道健康检查地址。
 
         :param request: Request instance for GenerateVpnConnectionDefaultHealthCheckIp.
         :type request: :class:`tencentcloud.vpc.v20170312.models.GenerateVpnConnectionDefaultHealthCheckIpRequest`
@@ -5214,15 +5214,15 @@
             model = models.GenerateVpnConnectionDefaultHealthCheckIpResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetCcnRegionBandwidthLimits(self, request):
         """本接口（GetCcnRegionBandwidthLimits）用于查询云联网相关地域带宽信息，其中预付费模式的云联网仅支持地域间限速，后付费模式的云联网支持地域间限速和地域出口限速。
 
         :param request: Request instance for GetCcnRegionBandwidthLimits.
         :type request: :class:`tencentcloud.vpc.v20170312.models.GetCcnRegionBandwidthLimitsRequest`
@@ -5237,15 +5237,15 @@
             model = models.GetCcnRegionBandwidthLimitsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def HaVipAssociateAddressIp(self, request):
         """本接口（HaVipAssociateAddressIp）用于高可用虚拟IP（HAVIP）绑定弹性公网IP（EIP）。<br />
         本接口是异步完成，如需查询异步任务执行结果，请使用本接口返回的`RequestId`轮询`DescribeVpcTaskResult`接口。
 
         :param request: Request instance for HaVipAssociateAddressIp.
@@ -5261,15 +5261,15 @@
             model = models.HaVipAssociateAddressIpResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def HaVipDisassociateAddressIp(self, request):
         """本接口（HaVipDisassociateAddressIp）用于将高可用虚拟IP（HAVIP）已绑定的弹性公网IP（EIP）解除绑定。<br />
         本接口是异步完成，如需查询异步任务执行结果，请使用本接口返回的`RequestId`轮询`DescribeVpcTaskResult`接口。
 
         :param request: Request instance for HaVipDisassociateAddressIp.
@@ -5285,15 +5285,15 @@
             model = models.HaVipDisassociateAddressIpResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquirePriceCreateDirectConnectGateway(self, request):
         """本接口（DescribePriceCreateDirectConnectGateway）用于创建专线网关询价。
 
         :param request: Request instance for InquirePriceCreateDirectConnectGateway.
         :type request: :class:`tencentcloud.vpc.v20170312.models.InquirePriceCreateDirectConnectGatewayRequest`
@@ -5308,15 +5308,15 @@
             model = models.InquirePriceCreateDirectConnectGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceCreateVpnGateway(self, request):
         """本接口（InquiryPriceCreateVpnGateway）用于创建VPN网关询价。
 
         :param request: Request instance for InquiryPriceCreateVpnGateway.
         :type request: :class:`tencentcloud.vpc.v20170312.models.InquiryPriceCreateVpnGatewayRequest`
@@ -5331,15 +5331,15 @@
             model = models.InquiryPriceCreateVpnGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceRenewVpnGateway(self, request):
         """本接口（InquiryPriceRenewVpnGateway）用于续费VPN网关询价。目前仅支持IPSEC类型网关的询价。
 
         :param request: Request instance for InquiryPriceRenewVpnGateway.
         :type request: :class:`tencentcloud.vpc.v20170312.models.InquiryPriceRenewVpnGatewayRequest`
@@ -5354,15 +5354,15 @@
             model = models.InquiryPriceRenewVpnGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceResetVpnGatewayInternetMaxBandwidth(self, request):
         """本接口（InquiryPriceResetVpnGatewayInternetMaxBandwidth）调整VPN网关带宽上限询价。
 
         :param request: Request instance for InquiryPriceResetVpnGatewayInternetMaxBandwidth.
         :type request: :class:`tencentcloud.vpc.v20170312.models.InquiryPriceResetVpnGatewayInternetMaxBandwidthRequest`
@@ -5377,15 +5377,15 @@
             model = models.InquiryPriceResetVpnGatewayInternetMaxBandwidthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def LockCcnBandwidths(self, request):
         """本接口（LockCcnBandwidths）用户锁定云联网限速实例。
         该接口一般用来封禁地域间限速的云联网实例下的限速实例, 目前联通内部运营系统通过云API调用, 如果是出口限速, 一般使用更粗的云联网实例粒度封禁（LockCcns）。
         如有需要, 可以封禁任意限速实例, 可接入到内部运营系统。
 
@@ -5402,15 +5402,15 @@
             model = models.LockCcnBandwidthsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def LockCcns(self, request):
         """本接口（LockCcns）用于锁定云联网实例
 
         该接口一般用来封禁出口限速的云联网实例, 目前联通内部运营系统通过云API调用, 因为出口限速无法按地域间封禁, 只能按更粗的云联网实例粒度封禁, 如果是地域间限速, 一般可以通过更细的限速实例粒度封禁（LockCcnBandwidths）
 
@@ -5430,15 +5430,15 @@
             model = models.LockCcnsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def MigrateNetworkInterface(self, request):
         """本接口（MigrateNetworkInterface）用于弹性网卡迁移。
         本接口是异步完成，如需查询异步任务执行结果，请使用本接口返回的`RequestId`轮询`DescribeVpcTaskResult`接口。
 
         :param request: Request instance for MigrateNetworkInterface.
@@ -5454,15 +5454,15 @@
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
         """本接口（MigratePrivateIpAddress）用于弹性网卡内网IP迁移。
         * 该接口用于将一个内网IP从一个弹性网卡上迁移到另外一个弹性网卡，主IP地址不支持迁移。
         * 迁移前后的弹性网卡必须在同一个子网内。
 
@@ -5481,15 +5481,15 @@
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
         """本接口 (ModifyAddressAttribute) 用于修改[弹性公网IP](https://cloud.tencent.com/document/product/213/1941)（简称 EIP）的名称。
 
         :param request: Request instance for ModifyAddressAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyAddressAttributeRequest`
@@ -5504,15 +5504,15 @@
             model = models.ModifyAddressAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAddressInternetChargeType(self, request):
         """该接口用于调整具有带宽属性弹性公网IP的网络计费模式
         * 支持BANDWIDTH_PREPAID_BY_MONTH和TRAFFIC_POSTPAID_BY_HOUR两种网络计费模式之间的切换。
         * 每个弹性公网IP支持调整两次，次数超出则无法调整。
 
@@ -5529,15 +5529,15 @@
             model = models.ModifyAddressInternetChargeTypeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAddressTemplateAttribute(self, request):
         """本接口（ModifyAddressTemplateAttribute）用于修改IP地址模板。
 
         :param request: Request instance for ModifyAddressTemplateAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyAddressTemplateAttributeRequest`
@@ -5552,15 +5552,15 @@
             model = models.ModifyAddressTemplateAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAddressTemplateGroupAttribute(self, request):
         """本接口（ModifyAddressTemplateGroupAttribute）用于修改IP地址模板集合。
 
         :param request: Request instance for ModifyAddressTemplateGroupAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyAddressTemplateGroupAttributeRequest`
@@ -5575,15 +5575,15 @@
             model = models.ModifyAddressTemplateGroupAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAddressesBandwidth(self, request):
         """本接口（ModifyAddressesBandwidth）用于调整[弹性公网IP](https://cloud.tencent.com/document/product/213/1941)(简称EIP)带宽，支持后付费EIP, 预付费EIP和带宽包EIP
 
         :param request: Request instance for ModifyAddressesBandwidth.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyAddressesBandwidthRequest`
@@ -5598,15 +5598,15 @@
             model = models.ModifyAddressesBandwidthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAssistantCidr(self, request):
         """本接口（ModifyAssistantCidr）用于批量修改辅助CIDR，支持新增和删除。
 
         :param request: Request instance for ModifyAssistantCidr.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyAssistantCidrRequest`
@@ -5621,15 +5621,15 @@
             model = models.ModifyAssistantCidrResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyBandwidthPackageAttribute(self, request):
         """接口用于修改带宽包属性，包括带宽包名字等
 
         :param request: Request instance for ModifyBandwidthPackageAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyBandwidthPackageAttributeRequest`
@@ -5644,15 +5644,15 @@
             model = models.ModifyBandwidthPackageAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCcnAttachedInstancesAttribute(self, request):
         """修改CCN关联实例属性，目前仅修改备注description
 
         :param request: Request instance for ModifyCcnAttachedInstancesAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyCcnAttachedInstancesAttributeRequest`
@@ -5667,15 +5667,15 @@
             model = models.ModifyCcnAttachedInstancesAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCcnAttribute(self, request):
         """本接口（ModifyCcnAttribute）用于修改云联网（CCN）的相关属性。
 
         :param request: Request instance for ModifyCcnAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyCcnAttributeRequest`
@@ -5690,15 +5690,15 @@
             model = models.ModifyCcnAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCcnRegionBandwidthLimitsType(self, request):
         """本接口（ModifyCcnRegionBandwidthLimitsType）用于修改后付费云联网实例修改带宽限速策略。
 
         :param request: Request instance for ModifyCcnRegionBandwidthLimitsType.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyCcnRegionBandwidthLimitsTypeRequest`
@@ -5713,15 +5713,15 @@
             model = models.ModifyCcnRegionBandwidthLimitsTypeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCustomerGatewayAttribute(self, request):
         """本接口（ModifyCustomerGatewayAttribute）用于修改对端网关信息。
 
         :param request: Request instance for ModifyCustomerGatewayAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyCustomerGatewayAttributeRequest`
@@ -5736,15 +5736,15 @@
             model = models.ModifyCustomerGatewayAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDhcpIpAttribute(self, request):
         """本接口（ModifyDhcpIpAttribute）用于修改DhcpIp属性
 
         :param request: Request instance for ModifyDhcpIpAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyDhcpIpAttributeRequest`
@@ -5759,15 +5759,15 @@
             model = models.ModifyDhcpIpAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDirectConnectGatewayAttribute(self, request):
         """本接口（ModifyDirectConnectGatewayAttribute）用于修改专线网关属性
 
         :param request: Request instance for ModifyDirectConnectGatewayAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyDirectConnectGatewayAttributeRequest`
@@ -5782,15 +5782,15 @@
             model = models.ModifyDirectConnectGatewayAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyFlowLogAttribute(self, request):
         """本接口（ModifyFlowLogAttribute）用于修改流日志属性。
 
         :param request: Request instance for ModifyFlowLogAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyFlowLogAttributeRequest`
@@ -5805,15 +5805,15 @@
             model = models.ModifyFlowLogAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyGatewayFlowQos(self, request):
         """本接口（ModifyGatewayFlowQos）用于调整网关流控带宽。
 
         :param request: Request instance for ModifyGatewayFlowQos.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyGatewayFlowQosRequest`
@@ -5828,15 +5828,15 @@
             model = models.ModifyGatewayFlowQosResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyHaVipAttribute(self, request):
         """本接口（ModifyHaVipAttribute）用于修改高可用虚拟IP（HAVIP）属性。
 
         :param request: Request instance for ModifyHaVipAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyHaVipAttributeRequest`
@@ -5851,15 +5851,15 @@
             model = models.ModifyHaVipAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyIp6AddressesBandwidth(self, request):
         """该接口用于修改IPV6地址访问internet的带宽
 
         :param request: Request instance for ModifyIp6AddressesBandwidth.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyIp6AddressesBandwidthRequest`
@@ -5874,15 +5874,15 @@
             model = models.ModifyIp6AddressesBandwidthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyIp6Rule(self, request):
         """该接口用于修改IPV6转换规则，当前仅支持修改转换规则名称，IPV4地址和IPV4端口号
 
         :param request: Request instance for ModifyIp6Rule.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyIp6RuleRequest`
@@ -5897,15 +5897,15 @@
             model = models.ModifyIp6RuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyIp6Translator(self, request):
         """该接口用于修改IP6转换实例属性，当前仅支持修改实例名称。
 
         :param request: Request instance for ModifyIp6Translator.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyIp6TranslatorRequest`
@@ -5920,15 +5920,15 @@
             model = models.ModifyIp6TranslatorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyIpv6AddressesAttribute(self, request):
         """本接口（ModifyIpv6AddressesAttribute）用于修改弹性网卡内网IPv6地址属性。
 
         :param request: Request instance for ModifyIpv6AddressesAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyIpv6AddressesAttributeRequest`
@@ -5943,15 +5943,15 @@
             model = models.ModifyIpv6AddressesAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLocalGateway(self, request):
         """本接口（ModifyLocalGateway）用于修改CDC的本地网关。
 
         :param request: Request instance for ModifyLocalGateway.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyLocalGatewayRequest`
@@ -5966,15 +5966,15 @@
             model = models.ModifyLocalGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyNatGatewayAttribute(self, request):
         """本接口（ModifyNatGatewayAttribute）用于修改NAT网关的属性。
 
         :param request: Request instance for ModifyNatGatewayAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyNatGatewayAttributeRequest`
@@ -5989,15 +5989,15 @@
             model = models.ModifyNatGatewayAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyNatGatewayDestinationIpPortTranslationNatRule(self, request):
         """本接口（ModifyNatGatewayDestinationIpPortTranslationNatRule）用于修改NAT网关端口转发规则。
 
         :param request: Request instance for ModifyNatGatewayDestinationIpPortTranslationNatRule.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyNatGatewayDestinationIpPortTranslationNatRuleRequest`
@@ -6012,15 +6012,15 @@
             model = models.ModifyNatGatewayDestinationIpPortTranslationNatRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyNatGatewaySourceIpTranslationNatRule(self, request):
         """本接口（ModifyNatGatewaySourceIpTranslationNatRule）用于修改NAT网关SNAT转发规则。
 
         :param request: Request instance for ModifyNatGatewaySourceIpTranslationNatRule.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyNatGatewaySourceIpTranslationNatRuleRequest`
@@ -6035,15 +6035,15 @@
             model = models.ModifyNatGatewaySourceIpTranslationNatRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyNetDetect(self, request):
         """本接口(ModifyNetDetect)用于修改网络探测参数。
 
         :param request: Request instance for ModifyNetDetect.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyNetDetectRequest`
@@ -6058,15 +6058,15 @@
             model = models.ModifyNetDetectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyNetworkAclAttribute(self, request):
         """本接口（ModifyNetworkAclAttribute）用于修改网络ACL属性。
 
         :param request: Request instance for ModifyNetworkAclAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyNetworkAclAttributeRequest`
@@ -6081,15 +6081,15 @@
             model = models.ModifyNetworkAclAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyNetworkAclEntries(self, request):
         """本接口（ModifyNetworkAclEntries）用于修改（包括添加和删除）网络ACL的入站规则和出站规则。在NetworkAclEntrySet参数中：
         * 若同时传入入站规则和出站规则，则重置原有的入站规则和出站规则，并分别导入传入的规则。
         * 若仅传入入站规则，则仅重置原有的入站规则，并导入传入的规则，不影响原有的出站规则（若仅传入出站规则，处理方式类似入站方向）。
 
@@ -6106,15 +6106,15 @@
             model = models.ModifyNetworkAclEntriesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyNetworkAclQuintupleEntries(self, request):
         """本接口（ModifyNetworkAclQuintupleEntries）用于修改网络ACL五元组的入站规则和出站规则。在NetworkAclQuintupleEntrySet参数中：NetworkAclQuintupleEntry需要提供NetworkAclQuintupleEntryId。
 
         :param request: Request instance for ModifyNetworkAclQuintupleEntries.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyNetworkAclQuintupleEntriesRequest`
@@ -6129,15 +6129,15 @@
             model = models.ModifyNetworkAclQuintupleEntriesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyNetworkInterfaceAttribute(self, request):
         """本接口（ModifyNetworkInterfaceAttribute）用于修改弹性网卡属性。
 
         :param request: Request instance for ModifyNetworkInterfaceAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyNetworkInterfaceAttributeRequest`
@@ -6152,15 +6152,15 @@
             model = models.ModifyNetworkInterfaceAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyNetworkInterfaceQos(self, request):
         """本接口（ModifyNetworkInterfaceQos）用于修改弹性网卡服务质量。
 
         :param request: Request instance for ModifyNetworkInterfaceQos.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyNetworkInterfaceQosRequest`
@@ -6175,15 +6175,15 @@
             model = models.ModifyNetworkInterfaceQosResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPrivateIpAddressesAttribute(self, request):
         """本接口（ModifyPrivateIpAddressesAttribute）用于修改弹性网卡内网IP属性。
 
         :param request: Request instance for ModifyPrivateIpAddressesAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyPrivateIpAddressesAttributeRequest`
@@ -6198,15 +6198,15 @@
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
         """本接口（ModifyRouteTableAttribute）用于修改路由表（RouteTable）属性。
 
         :param request: Request instance for ModifyRouteTableAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyRouteTableAttributeRequest`
@@ -6221,15 +6221,15 @@
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
         """本接口（ModifySecurityGroupAttribute）用于修改安全组（SecurityGroupPolicy）属性。
 
         :param request: Request instance for ModifySecurityGroupAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifySecurityGroupAttributeRequest`
@@ -6244,15 +6244,15 @@
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
         """本接口（ModifySecurityGroupPolicies）用于重置安全组出站和入站规则（SecurityGroupPolicy）。
 
         <ul>
         <li>该接口不支持自定义索引 PolicyIndex。</li>
@@ -6282,15 +6282,15 @@
             model = models.ModifySecurityGroupPoliciesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyServiceTemplateAttribute(self, request):
         """本接口（ModifyServiceTemplateAttribute）用于修改协议端口模板。
 
         :param request: Request instance for ModifyServiceTemplateAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyServiceTemplateAttributeRequest`
@@ -6305,15 +6305,15 @@
             model = models.ModifyServiceTemplateAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyServiceTemplateGroupAttribute(self, request):
         """本接口（ModifyServiceTemplateGroupAttribute）用于修改协议端口模板集合。
 
         :param request: Request instance for ModifyServiceTemplateGroupAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyServiceTemplateGroupAttributeRequest`
@@ -6328,15 +6328,15 @@
             model = models.ModifyServiceTemplateGroupAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySnapshotPolicies(self, request):
         """本接口（ModifySnapshotPolicies）用于修改快照策略。
 
         :param request: Request instance for ModifySnapshotPolicies.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifySnapshotPoliciesRequest`
@@ -6351,15 +6351,15 @@
             model = models.ModifySnapshotPoliciesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySubnetAttribute(self, request):
         """本接口（ModifySubnetAttribute）用于修改子网属性。
 
         :param request: Request instance for ModifySubnetAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifySubnetAttributeRequest`
@@ -6374,15 +6374,15 @@
             model = models.ModifySubnetAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTemplateMember(self, request):
         """修改模板对象中的IP地址、协议端口、IP地址组、协议端口组。当前仅支持北京、泰国、北美地域请求。
 
         :param request: Request instance for ModifyTemplateMember.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyTemplateMemberRequest`
@@ -6397,15 +6397,15 @@
             model = models.ModifyTemplateMemberResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyVpcAttribute(self, request):
         """本接口（ModifyVpcAttribute）用于修改私有网络（VPC）的相关属性。
 
         :param request: Request instance for ModifyVpcAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyVpcAttributeRequest`
@@ -6420,15 +6420,15 @@
             model = models.ModifyVpcAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyVpcEndPointAttribute(self, request):
         """本接口（ModifyVpcEndPointAttribute）用于修改终端节点属性。
 
         :param request: Request instance for ModifyVpcEndPointAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyVpcEndPointAttributeRequest`
@@ -6443,15 +6443,15 @@
             model = models.ModifyVpcEndPointAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyVpcEndPointServiceAttribute(self, request):
         """本接口（ModifyVpcEndPointServiceAttribute）用于修改终端节点服务属性。
 
 
         :param request: Request instance for ModifyVpcEndPointServiceAttribute.
@@ -6467,15 +6467,15 @@
             model = models.ModifyVpcEndPointServiceAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyVpcEndPointServiceWhiteList(self, request):
         """本接口（ModifyVpcEndPointServiceWhiteList）用于修改终端节点服务白名单属性。
 
         :param request: Request instance for ModifyVpcEndPointServiceWhiteList.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyVpcEndPointServiceWhiteListRequest`
@@ -6490,15 +6490,15 @@
             model = models.ModifyVpcEndPointServiceWhiteListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyVpnConnectionAttribute(self, request):
         """本接口（ModifyVpnConnectionAttribute）用于修改VPN通道。
 
         :param request: Request instance for ModifyVpnConnectionAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyVpnConnectionAttributeRequest`
@@ -6513,15 +6513,15 @@
             model = models.ModifyVpnConnectionAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyVpnGatewayAttribute(self, request):
         """本接口（ModifyVpnGatewayAttribute）用于修改VPN网关属性。
 
         :param request: Request instance for ModifyVpnGatewayAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyVpnGatewayAttributeRequest`
@@ -6536,15 +6536,15 @@
             model = models.ModifyVpnGatewayAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyVpnGatewayCcnRoutes(self, request):
         """本接口（ModifyVpnGatewayCcnRoutes）用于修改VPN网关云联网路由。
 
         :param request: Request instance for ModifyVpnGatewayCcnRoutes.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyVpnGatewayCcnRoutesRequest`
@@ -6559,15 +6559,15 @@
             model = models.ModifyVpnGatewayCcnRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyVpnGatewayRoutes(self, request):
         """本接口（ModifyVpnGatewayRoutes）用于修改VPN路由是否启用。
 
         :param request: Request instance for ModifyVpnGatewayRoutes.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyVpnGatewayRoutesRequest`
@@ -6582,15 +6582,15 @@
             model = models.ModifyVpnGatewayRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def NotifyRoutes(self, request):
         """本接口（NotifyRoutes）用于路由表列表页操作增加“发布到云联网”，发布路由到云联网。
 
         :param request: Request instance for NotifyRoutes.
         :type request: :class:`tencentcloud.vpc.v20170312.models.NotifyRoutesRequest`
@@ -6605,15 +6605,15 @@
             model = models.NotifyRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RefreshDirectConnectGatewayRouteToNatGateway(self, request):
         """刷新专线直连nat路由，更新nat到专线的路由表
 
         :param request: Request instance for RefreshDirectConnectGatewayRouteToNatGateway.
         :type request: :class:`tencentcloud.vpc.v20170312.models.RefreshDirectConnectGatewayRouteToNatGatewayRequest`
@@ -6628,15 +6628,15 @@
             model = models.RefreshDirectConnectGatewayRouteToNatGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RejectAttachCcnInstances(self, request):
         """本接口（RejectAttachCcnInstances）用于跨账号关联实例时，云联网所有者拒绝关联操作。
 
         :param request: Request instance for RejectAttachCcnInstances.
         :type request: :class:`tencentcloud.vpc.v20170312.models.RejectAttachCcnInstancesRequest`
@@ -6651,15 +6651,15 @@
             model = models.RejectAttachCcnInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReleaseAddresses(self, request):
         """本接口 (ReleaseAddresses) 用于释放一个或多个[弹性公网IP](https://cloud.tencent.com/document/product/213/1941)（简称 EIP）。
         * 该操作不可逆，释放后 EIP 关联的 IP 地址将不再属于您的名下。
         * 只有状态为 UNBIND 的 EIP 才能进行释放操作。
 
@@ -6676,15 +6676,15 @@
             model = models.ReleaseAddressesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReleaseIp6AddressesBandwidth(self, request):
         """该接口用于给弹性公网IPv6地址释放带宽。
 
         :param request: Request instance for ReleaseIp6AddressesBandwidth.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ReleaseIp6AddressesBandwidthRequest`
@@ -6699,15 +6699,15 @@
             model = models.ReleaseIp6AddressesBandwidthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RemoveBandwidthPackageResources(self, request):
         """接口用于删除带宽包资源，包括[弹性公网IP](https://cloud.tencent.com/document/product/213/1941)和[负载均衡](https://cloud.tencent.com/document/product/214/517)等
 
         :param request: Request instance for RemoveBandwidthPackageResources.
         :type request: :class:`tencentcloud.vpc.v20170312.models.RemoveBandwidthPackageResourcesRequest`
@@ -6722,15 +6722,15 @@
             model = models.RemoveBandwidthPackageResourcesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RemoveIp6Rules(self, request):
         """1. 该接口用于删除IPV6转换规则
         2. 支持批量删除同一个转换实例下的多个转换规则
 
         :param request: Request instance for RemoveIp6Rules.
@@ -6746,15 +6746,15 @@
             model = models.RemoveIp6RulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RenewAddresses(self, request):
         """该接口用于续费包月带宽计费模式的弹性公网IP
 
         :param request: Request instance for RenewAddresses.
         :type request: :class:`tencentcloud.vpc.v20170312.models.RenewAddressesRequest`
@@ -6769,15 +6769,15 @@
             model = models.RenewAddressesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RenewVpnGateway(self, request):
         """本接口（RenewVpnGateway）用于预付费（包年包月）VPN网关续费。目前只支持IPSEC网关。
 
         :param request: Request instance for RenewVpnGateway.
         :type request: :class:`tencentcloud.vpc.v20170312.models.RenewVpnGatewayRequest`
@@ -6792,15 +6792,15 @@
             model = models.RenewVpnGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReplaceDirectConnectGatewayCcnRoutes(self, request):
         """本接口（ReplaceDirectConnectGatewayCcnRoutes）根据路由ID（RouteId）修改指定的路由（Route），支持批量修改。
 
         :param request: Request instance for ReplaceDirectConnectGatewayCcnRoutes.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ReplaceDirectConnectGatewayCcnRoutesRequest`
@@ -6815,15 +6815,15 @@
             model = models.ReplaceDirectConnectGatewayCcnRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReplaceRouteTableAssociation(self, request):
         """本接口（ReplaceRouteTableAssociation）用于修改子网（Subnet）关联的路由表（RouteTable）。
         * 一个子网只能关联一个路由表。
 
         :param request: Request instance for ReplaceRouteTableAssociation.
@@ -6839,15 +6839,15 @@
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
         """本接口（ReplaceRoutes）根据路由策略ID（RouteId）修改指定的路由策略（Route），支持批量修改。
 
         :param request: Request instance for ReplaceRoutes.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ReplaceRoutesRequest`
@@ -6862,15 +6862,15 @@
             model = models.ReplaceRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReplaceSecurityGroupPolicies(self, request):
         """本接口（ReplaceSecurityGroupPolicies）用于批量修改安全组规则（SecurityGroupPolicy）。
         单个请求中只能替换单个方向的一条或多条规则, 必须要指定索引（PolicyIndex）。
 
         :param request: Request instance for ReplaceSecurityGroupPolicies.
@@ -6886,15 +6886,15 @@
             model = models.ReplaceSecurityGroupPoliciesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReplaceSecurityGroupPolicy(self, request):
         """本接口（ReplaceSecurityGroupPolicy）用于替换单条安全组规则（SecurityGroupPolicy）。
         单个请求中只能替换单个方向的一条规则, 必须要指定索引（PolicyIndex）。
 
         :param request: Request instance for ReplaceSecurityGroupPolicy.
@@ -6910,15 +6910,15 @@
             model = models.ReplaceSecurityGroupPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetAttachCcnInstances(self, request):
         """本接口（ResetAttachCcnInstances）用于跨账号关联实例申请过期时，重新申请关联操作。
 
         :param request: Request instance for ResetAttachCcnInstances.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ResetAttachCcnInstancesRequest`
@@ -6933,15 +6933,15 @@
             model = models.ResetAttachCcnInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetNatGatewayConnection(self, request):
         """本接口（ResetNatGatewayConnection）用来NAT网关并发连接上限。
 
         :param request: Request instance for ResetNatGatewayConnection.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ResetNatGatewayConnectionRequest`
@@ -6956,15 +6956,15 @@
             model = models.ResetNatGatewayConnectionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetRoutes(self, request):
         """本接口（ResetRoutes）用于对某个路由表名称和所有路由策略（Route）进行重新设置。<br />
         注意: 调用本接口是先删除当前路由表中所有路由策略, 再保存新提交的路由策略内容, 会引起网络中断。
 
         :param request: Request instance for ResetRoutes.
@@ -6980,15 +6980,15 @@
             model = models.ResetRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetVpnConnection(self, request):
         """本接口（ResetVpnConnection）用于重置VPN通道。
 
         :param request: Request instance for ResetVpnConnection.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ResetVpnConnectionRequest`
@@ -7003,15 +7003,15 @@
             model = models.ResetVpnConnectionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetVpnGatewayInternetMaxBandwidth(self, request):
         """本接口（ResetVpnGatewayInternetMaxBandwidth）用于调整VPN网关带宽上限。VPN网关带宽目前仅支持部分带宽范围内升降配，如【5,100】Mbps和【200,1000】Mbps，在各自带宽范围内可提升配额，跨范围提升配额和降配暂不支持，如果是包年包月VPN网关需要在有效期内。
 
         :param request: Request instance for ResetVpnGatewayInternetMaxBandwidth.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ResetVpnGatewayInternetMaxBandwidthRequest`
@@ -7026,15 +7026,15 @@
             model = models.ResetVpnGatewayInternetMaxBandwidthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResumeSnapshotInstance(self, request):
         """本接口（ResumeSnapshotInstance）用于根据备份内容恢复安全组策略。
 
         :param request: Request instance for ResumeSnapshotInstance.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ResumeSnapshotInstanceRequest`
@@ -7049,15 +7049,15 @@
             model = models.ResumeSnapshotInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReturnNormalAddresses(self, request):
         """本接口（ReturnNormalAddresses）用于解绑并释放普通公网IP。
         为完善公网IP的访问管理功能，此接口于2022年12月15日升级优化鉴权功能，升级后子用户调用此接口需向主账号申请CAM策略授权，否则可能调用失败。您可以提前为子账号配置操作授权，详情见[授权指南](https://cloud.tencent.com/document/product/598/34545)。
 
         :param request: Request instance for ReturnNormalAddresses.
@@ -7073,15 +7073,15 @@
             model = models.ReturnNormalAddressesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetCcnRegionBandwidthLimits(self, request):
         """本接口（SetCcnRegionBandwidthLimits）用于设置云联网（CCN）各地域出带宽上限，或者地域间带宽上限。
 
         :param request: Request instance for SetCcnRegionBandwidthLimits.
         :type request: :class:`tencentcloud.vpc.v20170312.models.SetCcnRegionBandwidthLimitsRequest`
@@ -7096,15 +7096,15 @@
             model = models.SetCcnRegionBandwidthLimitsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetVpnGatewaysRenewFlag(self, request):
         """本接口（SetVpnGatewaysRenewFlag）用于设置VPNGW续费标记。
 
         :param request: Request instance for SetVpnGatewaysRenewFlag.
         :type request: :class:`tencentcloud.vpc.v20170312.models.SetVpnGatewaysRenewFlagRequest`
@@ -7119,15 +7119,15 @@
             model = models.SetVpnGatewaysRenewFlagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TransformAddress(self, request):
         """本接口 (TransformAddress) 用于将实例的普通公网 IP 转换为[弹性公网IP](https://cloud.tencent.com/document/product/213/1941)（简称 EIP）。
         * 平台对用户每地域每日解绑 EIP 重新分配普通公网 IP 次数有所限制（可参见 [EIP 产品简介](/document/product/213/1941)）。上述配额可通过 [DescribeAddressQuota](https://cloud.tencent.com/document/api/213/1378) 接口获取。
 
         :param request: Request instance for TransformAddress.
@@ -7143,15 +7143,15 @@
             model = models.TransformAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnassignIpv6Addresses(self, request):
         """本接口（UnassignIpv6Addresses）用于释放弹性网卡`IPv6`地址。<br />
         本接口是异步完成，如需查询异步任务执行结果，请使用本接口返回的`RequestId`轮询`DescribeVpcTaskResult`接口。
 
         :param request: Request instance for UnassignIpv6Addresses.
@@ -7167,15 +7167,15 @@
             model = models.UnassignIpv6AddressesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnassignIpv6CidrBlock(self, request):
         """本接口（UnassignIpv6CidrBlock）用于释放IPv6网段。<br />
         网段如果还有IP占用且未回收，则网段无法释放。
 
         :param request: Request instance for UnassignIpv6CidrBlock.
@@ -7191,15 +7191,15 @@
             model = models.UnassignIpv6CidrBlockResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnassignIpv6SubnetCidrBlock(self, request):
         """本接口（UnassignIpv6SubnetCidrBlock）用于释放IPv6子网段。<br />
         子网段如果还有IP占用且未回收，则子网段无法释放。
 
         :param request: Request instance for UnassignIpv6SubnetCidrBlock.
@@ -7215,15 +7215,15 @@
             model = models.UnassignIpv6SubnetCidrBlockResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnassignPrivateIpAddresses(self, request):
         """本接口（UnassignPrivateIpAddresses）用于弹性网卡退还内网 IP。
         * 退还弹性网卡上的辅助内网IP，接口自动解关联弹性公网 IP。不能退还弹性网卡的主内网IP。
 
         本接口是异步完成，如需查询异步任务执行结果，请使用本接口返回的`RequestId`轮询`DescribeVpcTaskResult`接口。
@@ -7241,15 +7241,15 @@
             model = models.UnassignPrivateIpAddressesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnlockCcnBandwidths(self, request):
         """本接口（UnlockCcnBandwidths）用户解锁云联网限速实例。
         该接口一般用来封禁地域间限速的云联网实例下的限速实例, 目前联通内部运营系统通过云API调用, 如果是出口限速, 一般使用更粗的云联网实例粒度封禁（SecurityUnlockCcns）。
         如有需要, 可以封禁任意限速实例, 可接入到内部运营系统。
 
@@ -7266,15 +7266,15 @@
             model = models.UnlockCcnBandwidthsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnlockCcns(self, request):
         """本接口（UnlockCcns）用于解锁云联网实例
 
         该接口一般用来解封禁出口限速的云联网实例, 目前联通内部运营系统通过云API调用, 因为出口限速无法按地域间解封禁, 只能按更粗的云联网实例粒度解封禁, 如果是地域间限速, 一般可以通过更细的限速实例粒度解封禁（UnlockCcnBandwidths）
 
@@ -7294,15 +7294,15 @@
             model = models.UnlockCcnsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def WithdrawNotifyRoutes(self, request):
         """本接口（WithdrawNotifyRoutes）用于撤销已发布到云联网的路由。路由表列表页操作增加“从云联网撤销”。
 
         :param request: Request instance for WithdrawNotifyRoutes.
         :type request: :class:`tencentcloud.vpc.v20170312.models.WithdrawNotifyRoutesRequest`
@@ -7317,8 +7317,8 @@
             model = models.WithdrawNotifyRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.938/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-vpc-3.0.938/tencentcloud/vpc/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vpc-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.938/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.937/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.938/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.937/README.rst` & `tencentcloud-sdk-python-vpc-3.0.938/README.rst`

 * *Files identical despite different names*

