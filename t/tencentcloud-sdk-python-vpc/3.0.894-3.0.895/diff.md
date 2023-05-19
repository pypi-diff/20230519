# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.894.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.895.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.894.tar", last modified: Thu May 18 00:41:55 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.895.tar", last modified: Fri May 19 03:05:19 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.894.tar` & `tencentcloud-sdk-python-vpc-3.0.895.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:41:55.000000 tencentcloud-sdk-python-vpc-3.0.894/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:41:55.000000 tencentcloud-sdk-python-vpc-3.0.894/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:41:55.000000 tencentcloud-sdk-python-vpc-3.0.894/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-18 00:41:55.000000 tencentcloud-sdk-python-vpc-3.0.894/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:41:55.000000 tencentcloud-sdk-python-vpc-3.0.894/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:41:55.000000 tencentcloud-sdk-python-vpc-3.0.894/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-18 00:41:55.000000 tencentcloud-sdk-python-vpc-3.0.894/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:41:55.000000 tencentcloud-sdk-python-vpc-3.0.894/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:41:55.000000 tencentcloud-sdk-python-vpc-3.0.894/tencentcloud/vpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:41:55.000000 tencentcloud-sdk-python-vpc-3.0.894/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)   332014 2023-05-18 00:41:55.000000 tencentcloud-sdk-python-vpc-3.0.894/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)    41601 2023-05-18 00:41:55.000000 tencentcloud-sdk-python-vpc-3.0.894/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:41:55.000000 tencentcloud-sdk-python-vpc-3.0.894/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   849420 2023-05-18 00:41:55.000000 tencentcloud-sdk-python-vpc-3.0.894/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:41:55.000000 tencentcloud-sdk-python-vpc-3.0.894/tencentcloud/vpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:41:55.000000 tencentcloud-sdk-python-vpc-3.0.894/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:41:55.000000 tencentcloud-sdk-python-vpc-3.0.894/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-18 00:41:55.000000 tencentcloud-sdk-python-vpc-3.0.894/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:41:55.000000 tencentcloud-sdk-python-vpc-3.0.894/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/vpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   332171 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)    41601 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   851263 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/vpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.894/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.895/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.894/README.rst` & `tencentcloud-sdk-python-vpc-3.0.895/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.894/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2607,15 +2607,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DeleteVpnGatewaySslClient(self, request):
-        """删除SSL-VPN-CLIENT
+        """本接口（DeleteVpnGatewaySslClient）用于删除SSL-VPN-CLIENT。
 
         :param request: Request instance for DeleteVpnGatewaySslClient.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteVpnGatewaySslClientRequest`
         :rtype: :class:`tencentcloud.vpc.v20170312.models.DeleteVpnGatewaySslClientResponse`
 
         """
         try:
@@ -5008,15 +5008,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DownloadVpnGatewaySslClientCert(self, request):
-        """下载SSL-VPN-CLIENT 客户端证书
+        """本接口（DownloadVpnGatewaySslClientCert）用于下载SSL-VPN-CLIENT 客户端证书。
 
         :param request: Request instance for DownloadVpnGatewaySslClientCert.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DownloadVpnGatewaySslClientCertRequest`
         :rtype: :class:`tencentcloud.vpc.v20170312.models.DownloadVpnGatewaySslClientCertResponse`
 
         """
         try:
@@ -5171,15 +5171,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def EnableVpnGatewaySslClientCert(self, request):
-        """启用SSL-VPN-CLIENT 证书
+        """本接口（EnableVpnGatewaySslClientCert）用于启用SSL-VPN-CLIENT 证书。
 
         :param request: Request instance for EnableVpnGatewaySslClientCert.
         :type request: :class:`tencentcloud.vpc.v20170312.models.EnableVpnGatewaySslClientCertRequest`
         :rtype: :class:`tencentcloud.vpc.v20170312.models.EnableVpnGatewaySslClientCertResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.894/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.894/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/vpc/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5547,24 +5547,28 @@
 
     """
 
     def __init__(self):
         r"""
         :param SslVpnServerId: SSL-VPN-SERVER 实例ID。
         :type SslVpnServerId: str
-        :param SslVpnClientName: name
+        :param SslVpnClientName: SSL-VPN-CLIENT实例Name。不可和SslVpnClientNames同时使用。
         :type SslVpnClientName: str
+        :param SslVpnClientNames: SSL-VPN-CLIENT实例Name数字。批量创建时使用。不可和SslVpnClientName同时使用。
+        :type SslVpnClientNames: list of str
         """
         self.SslVpnServerId = None
         self.SslVpnClientName = None
+        self.SslVpnClientNames = None
 
 
     def _deserialize(self, params):
         self.SslVpnServerId = params.get("SslVpnServerId")
         self.SslVpnClientName = params.get("SslVpnClientName")
+        self.SslVpnClientNames = params.get("SslVpnClientNames")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -7612,22 +7616,26 @@
 class DeleteVpnGatewaySslClientRequest(AbstractModel):
     """DeleteVpnGatewaySslClient请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param SslVpnClientId: SSL-VPN-CLIENT 实例ID。
+        :param SslVpnClientId: SSL-VPN-CLIENT 实例ID。不可和SslVpnClientIds同时使用。
         :type SslVpnClientId: str
+        :param SslVpnClientIds: SSL-VPN-CLIENT 实例ID列表。批量删除时使用。不可和SslVpnClientId同时使用。
+        :type SslVpnClientIds: list of str
         """
         self.SslVpnClientId = None
+        self.SslVpnClientIds = None
 
 
     def _deserialize(self, params):
         self.SslVpnClientId = params.get("SslVpnClientId")
+        self.SslVpnClientIds = params.get("SslVpnClientIds")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -13982,22 +13990,26 @@
 class DisableVpnGatewaySslClientCertRequest(AbstractModel):
     """DisableVpnGatewaySslClientCert请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param SslVpnClientId: SSL-VPN-CLIENT 实例ID。
+        :param SslVpnClientId: SSL-VPN-CLIENT 实例ID。不可和SslVpnClientIds同时使用。
         :type SslVpnClientId: str
+        :param SslVpnClientIds: SSL-VPN-CLIENT 实例ID列表。批量禁用时使用。不可和SslVpnClientId同时使用。
+        :type SslVpnClientIds: list of str
         """
         self.SslVpnClientId = None
+        self.SslVpnClientIds = None
 
 
     def _deserialize(self, params):
         self.SslVpnClientId = params.get("SslVpnClientId")
+        self.SslVpnClientIds = params.get("SslVpnClientIds")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -14405,30 +14417,34 @@
 class DownloadVpnGatewaySslClientCertRequest(AbstractModel):
     """DownloadVpnGatewaySslClientCert请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param SslVpnClientId: SSL-VPN-CLIENT 实例ID。
+        :param SslVpnClientId: SSL-VPN-CLIENT 实例ID。不可以和SslVpnClientIds同时使用。
         :type SslVpnClientId: str
-        :param SamlToken: SAML-TOKEN
+        :param SamlToken: SAML Token（SAML令牌）。
         :type SamlToken: str
-        :param IsVpnPortal: VPN门户网站使用。默认Flase
+        :param IsVpnPortal: VPN门户网站使用。默认False
         :type IsVpnPortal: bool
+        :param SslVpnClientIds: SSL-VPN-CLIENT 实例ID列表。批量下载时使用。不可以和SslVpnClientId同时使用。
+        :type SslVpnClientIds: list of str
         """
         self.SslVpnClientId = None
         self.SamlToken = None
         self.IsVpnPortal = None
+        self.SslVpnClientIds = None
 
 
     def _deserialize(self, params):
         self.SslVpnClientId = params.get("SslVpnClientId")
         self.SamlToken = params.get("SamlToken")
         self.IsVpnPortal = params.get("IsVpnPortal")
+        self.SslVpnClientIds = params.get("SslVpnClientIds")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -14437,19 +14453,19 @@
 class DownloadVpnGatewaySslClientCertResponse(AbstractModel):
     """DownloadVpnGatewaySslClientCert返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param SslClientConfigsSet: 无
+        :param SslClientConfigsSet: SSL-VPN 客户端配置。
         :type SslClientConfigsSet: str
-        :param SslClientConfig: SSL-VPN client配置
+        :param SslClientConfig: SSL-VPN 客户端配置。
         :type SslClientConfig: list of SslClientConfig
-        :param Authenticated: 是否鉴权成功 只有传入SamlToken 才生效
+        :param Authenticated: 是否鉴权成功 只有传入SamlToken 才生效，1为成功，0为失败。
         :type Authenticated: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.SslClientConfigsSet = None
         self.SslClientConfig = None
         self.Authenticated = None
@@ -14741,22 +14757,26 @@
 class EnableVpnGatewaySslClientCertRequest(AbstractModel):
     """EnableVpnGatewaySslClientCert请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param SslVpnClientId: SSL-VPN-CLIENT 实例ID。
+        :param SslVpnClientId: SSL-VPN-CLIENT 实例ID。不可和SslVpnClientIds同时使用。
         :type SslVpnClientId: str
+        :param SslVpnClientIds: SSL-VPN-CLIENT 实例ID列表。批量启用时使用。不可和SslVpnClientId同时使用。
+        :type SslVpnClientIds: list of str
         """
         self.SslVpnClientId = None
+        self.SslVpnClientIds = None
 
 
     def _deserialize(self, params):
         self.SslVpnClientId = params.get("SslVpnClientId")
+        self.SslVpnClientIds = params.get("SslVpnClientIds")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -19927,15 +19947,15 @@
         :type IsWanIpBlocked: bool
         :param State: IP状态：
 PENDING：生产中
 MIGRATING：迁移中
 DELETING：删除中
 AVAILABLE：可用的
         :type State: str
-        :param QosLevel: IP服务质量等级，可选值：PT、AU、AG、DEFAULT，分别代表白金、金、银、默认四个等级。
+        :param QosLevel: IP服务质量等级，可选值：PT、AU、AG、DEFAULT，分别代表云金、云银、云铜、默认四个等级。
         :type QosLevel: str
         """
         self.PrivateIpAddress = None
         self.Primary = None
         self.PublicIpAddress = None
         self.AddressId = None
         self.Description = None
@@ -22352,26 +22372,30 @@
         :type SslVpnClientConfiguration: str
         :param SslVpnRootCert: 更证书
         :type SslVpnRootCert: str
         :param SslVpnKey: 客户端密钥
         :type SslVpnKey: str
         :param SslVpnCert: 客户端证书
         :type SslVpnCert: str
+        :param SslVpnClientId: SSL-VPN-CLIENT 实例ID。
+        :type SslVpnClientId: str
         """
         self.SslVpnClientConfiguration = None
         self.SslVpnRootCert = None
         self.SslVpnKey = None
         self.SslVpnCert = None
+        self.SslVpnClientId = None
 
 
     def _deserialize(self, params):
         self.SslVpnClientConfiguration = params.get("SslVpnClientConfiguration")
         self.SslVpnRootCert = params.get("SslVpnRootCert")
         self.SslVpnKey = params.get("SslVpnKey")
         self.SslVpnCert = params.get("SslVpnCert")
+        self.SslVpnClientId = params.get("SslVpnClientId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.894/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.894'
+__version__ = '3.0.895'
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.894/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.895/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.894/setup.py` & `tencentcloud-sdk-python-vpc-3.0.895/setup.py`

 * *Files identical despite different names*

