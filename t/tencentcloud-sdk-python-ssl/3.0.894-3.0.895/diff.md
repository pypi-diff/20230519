# Comparing `tmp/tencentcloud-sdk-python-ssl-3.0.894.tar.gz` & `tmp/tencentcloud-sdk-python-ssl-3.0.895.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ssl-3.0.894.tar", last modified: Thu May 18 00:35:52 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ssl-3.0.895.tar", last modified: Fri May 19 02:59:18 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ssl-3.0.894.tar` & `tencentcloud-sdk-python-ssl-3.0.895.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:35:52.000000 tencentcloud-sdk-python-ssl-3.0.894/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-18 00:35:52.000000 tencentcloud-sdk-python-ssl-3.0.894/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:35:52.000000 tencentcloud-sdk-python-ssl-3.0.894/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:35:52.000000 tencentcloud-sdk-python-ssl-3.0.894/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:35:52.000000 tencentcloud-sdk-python-ssl-3.0.894/tencentcloud/ssl/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:35:52.000000 tencentcloud-sdk-python-ssl-3.0.894/tencentcloud/ssl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:35:52.000000 tencentcloud-sdk-python-ssl-3.0.894/tencentcloud/ssl/v20191205/
--rw-r--r--   0 root         (0) root         (0)     6906 2023-05-18 00:35:52.000000 tencentcloud-sdk-python-ssl-3.0.894/tencentcloud/ssl/v20191205/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:35:52.000000 tencentcloud-sdk-python-ssl-3.0.894/tencentcloud/ssl/v20191205/__init__.py
--rw-r--r--   0 root         (0) root         (0)   133829 2023-05-18 00:35:52.000000 tencentcloud-sdk-python-ssl-3.0.894/tencentcloud/ssl/v20191205/models.py
--rw-r--r--   0 root         (0) root         (0)    28567 2023-05-18 00:35:52.000000 tencentcloud-sdk-python-ssl-3.0.894/tencentcloud/ssl/v20191205/ssl_client.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:35:52.000000 tencentcloud-sdk-python-ssl-3.0.894/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-18 00:35:52.000000 tencentcloud-sdk-python-ssl-3.0.894/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:35:52.000000 tencentcloud-sdk-python-ssl-3.0.894/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:35:52.000000 tencentcloud-sdk-python-ssl-3.0.894/tencentcloud_sdk_python_ssl.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:35:52.000000 tencentcloud-sdk-python-ssl-3.0.894/tencentcloud_sdk_python_ssl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-18 00:35:52.000000 tencentcloud-sdk-python-ssl-3.0.894/tencentcloud_sdk_python_ssl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:35:52.000000 tencentcloud-sdk-python-ssl-3.0.894/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:35:52.000000 tencentcloud-sdk-python-ssl-3.0.894/tencentcloud_sdk_python_ssl.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:59:18.000000 tencentcloud-sdk-python-ssl-3.0.895/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-19 02:59:18.000000 tencentcloud-sdk-python-ssl-3.0.895/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:59:18.000000 tencentcloud-sdk-python-ssl-3.0.895/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-19 02:59:18.000000 tencentcloud-sdk-python-ssl-3.0.895/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:59:18.000000 tencentcloud-sdk-python-ssl-3.0.895/tencentcloud/ssl/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:59:18.000000 tencentcloud-sdk-python-ssl-3.0.895/tencentcloud/ssl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:59:18.000000 tencentcloud-sdk-python-ssl-3.0.895/tencentcloud/ssl/v20191205/
+-rw-r--r--   0 root         (0) root         (0)     8810 2023-05-19 02:59:18.000000 tencentcloud-sdk-python-ssl-3.0.895/tencentcloud/ssl/v20191205/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:59:18.000000 tencentcloud-sdk-python-ssl-3.0.895/tencentcloud/ssl/v20191205/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   217317 2023-05-19 02:59:18.000000 tencentcloud-sdk-python-ssl-3.0.895/tencentcloud/ssl/v20191205/models.py
+-rw-r--r--   0 root         (0) root         (0)    48579 2023-05-19 02:59:18.000000 tencentcloud-sdk-python-ssl-3.0.895/tencentcloud/ssl/v20191205/ssl_client.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 02:59:18.000000 tencentcloud-sdk-python-ssl-3.0.895/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-19 02:59:18.000000 tencentcloud-sdk-python-ssl-3.0.895/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-19 02:59:18.000000 tencentcloud-sdk-python-ssl-3.0.895/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:59:18.000000 tencentcloud-sdk-python-ssl-3.0.895/tencentcloud_sdk_python_ssl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 02:59:18.000000 tencentcloud-sdk-python-ssl-3.0.895/tencentcloud_sdk_python_ssl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-19 02:59:18.000000 tencentcloud-sdk-python-ssl-3.0.895/tencentcloud_sdk_python_ssl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 02:59:18.000000 tencentcloud-sdk-python-ssl-3.0.895/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 02:59:18.000000 tencentcloud-sdk-python-ssl-3.0.895/tencentcloud_sdk_python_ssl.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.894/README.rst` & `tencentcloud-sdk-python-ssl-3.0.895/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.894/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ssl-3.0.895/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ssl-3.0.894/tencentcloud/ssl/v20191205/errorcodes.py` & `tencentcloud-sdk-python-ssl-3.0.895/tencentcloud/ssl/v20191205/errorcodes.py`

 * *Files 23% similar despite different names*

```diff
@@ -37,32 +37,65 @@
 
 # 免费证书申请1小时内不允许删除。
 FAILEDOPERATION_CANNOTBEDELETEDWITHINHOUR = 'FailedOperation.CannotBeDeletedWithinHour'
 
 # 获取订单信息失败，请稍后重试。
 FAILEDOPERATION_CANNOTGETORDER = 'FailedOperation.CannotGetOrder'
 
+# 记录状态必须完结才可以执行该操作。
+FAILEDOPERATION_CERTIFICATEDEPLOYDETAILROLLBACKSTATUSINVALID = 'FailedOperation.CertificateDeployDetailRollbackStatusInvalid'
+
+# 证书部署有正在进行中的任务，请部署完成后再重试。
+FAILEDOPERATION_CERTIFICATEDEPLOYHASPENDINGRECORD = 'FailedOperation.CertificateDeployHasPendingRecord'
+
+# 已选择的云资源无实例，无法更新，请重新核对后重试。
+FAILEDOPERATION_CERTIFICATEDEPLOYINSTANCEEMPTY = 'FailedOperation.CertificateDeployInstanceEmpty'
+
+# 证书部署记录不存在。
+FAILEDOPERATION_CERTIFICATEDEPLOYNOTEXIST = 'FailedOperation.CertificateDeployNotExist'
+
+# 记录状态必须失败才可以执行该操作。
+FAILEDOPERATION_CERTIFICATEDEPLOYRETRYSTATUSINVALID = 'FailedOperation.CertificateDeployRetryStatusInvalid'
+
+# 必须有部署成功的记录才可以回滚。
+FAILEDOPERATION_CERTIFICATEDEPLOYROLLBACKSTATUSINVALID = 'FailedOperation.CertificateDeployRollbackStatusInvalid'
+
 # 证书已存在。
 FAILEDOPERATION_CERTIFICATEEXISTS = 'FailedOperation.CertificateExists'
 
 # 已替换证书，无法进行托管。
 FAILEDOPERATION_CERTIFICATEHASRENEWED = 'FailedOperation.CertificateHasRenewed'
 
 # 当前证书不允许使用一键更新的功能。
 FAILEDOPERATION_CERTIFICATEHOSTDEPLOYCANNOTALLOW = 'FailedOperation.CertificateHostDeployCanNotAllow'
 
+# 当前为内部账号，账号涉及实例资源较多，无法使用部署功能，请联系SSL证书特殊处理。
+FAILEDOPERATION_CERTIFICATEHOSTRESOURCEINNERINTERRUPT = 'FailedOperation.CertificateHostResourceInnerInterrupt'
+
+# 当前账号下实例数量过多，无法正常加载，请您切换加载方式。切换后点击“刷新列表”等待一段时间后即可全部加载。
+FAILEDOPERATION_CERTIFICATEHOSTRESOURCEINSTANCEHUGELIMIT = 'FailedOperation.CertificateHostResourceInstanceHugeLimit'
+
+# 云资源类型无效。
+FAILEDOPERATION_CERTIFICATEHOSTRESOURCETYPEINVALID = 'FailedOperation.CertificateHostResourceTypeInvalid'
+
 # 证书资源托管数量超过限制。
 FAILEDOPERATION_CERTIFICATEHOSTINGTYPENUMBERLIMIT = 'FailedOperation.CertificateHostingTypeNumberLimit'
 
 # 证书不符合标准。
 FAILEDOPERATION_CERTIFICATEINVALID = 'FailedOperation.CertificateInvalid'
 
 # 证书与私钥不对应。
 FAILEDOPERATION_CERTIFICATEMISMATCH = 'FailedOperation.CertificateMismatch'
 
+# 证书不可用，请检查后再试。
+FAILEDOPERATION_CERTIFICATENOTAVAILABLE = 'FailedOperation.CertificateNotAvailable'
+
+# 证书不可以部署到实例列表下。
+FAILEDOPERATION_CERTIFICATENOTDEPLOYINSTANCE = 'FailedOperation.CertificateNotDeployInstance'
+
 # 证书不存在。
 FAILEDOPERATION_CERTIFICATENOTFOUND = 'FailedOperation.CertificateNotFound'
 
 # 证书确认函文件过大（需小于1.4M）。
 FAILEDOPERATION_CONFIRMLETTERTOOLARGE = 'FailedOperation.ConfirmLetterTooLarge'
 
 # 证书确认函文件过小（需大于1KB）。
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.894/tencentcloud/ssl/v20191205/models.py` & `tencentcloud-sdk-python-ssl-3.0.895/tencentcloud/ssl/v20191205/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,14 +14,55 @@
 # limitations under the License.
 
 import warnings
 
 from tencentcloud.common.abstract_model import AbstractModel
 
 
+class ApiGatewayInstanceDetail(AbstractModel):
+    """apiGateway实例详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ServiceId: 实例ID
+        :type ServiceId: str
+        :param ServiceName: 实例名称
+        :type ServiceName: str
+        :param Domain: 域名
+        :type Domain: str
+        :param CertId: 证书ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CertId: str
+        :param Protocol: 使用协议
+        :type Protocol: str
+        """
+        self.ServiceId = None
+        self.ServiceName = None
+        self.Domain = None
+        self.CertId = None
+        self.Protocol = None
+
+
+    def _deserialize(self, params):
+        self.ServiceId = params.get("ServiceId")
+        self.ServiceName = params.get("ServiceName")
+        self.Domain = params.get("Domain")
+        self.CertId = params.get("CertId")
+        self.Protocol = params.get("Protocol")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ApplyCertificateRequest(AbstractModel):
     """ApplyCertificate请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -156,14 +197,46 @@
 
 
     def _deserialize(self, params):
         self.CertificateId = params.get("CertificateId")
         self.RequestId = params.get("RequestId")
 
 
+class CdnInstanceDetail(AbstractModel):
+    """CDN实例详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Domain: 域名
+        :type Domain: str
+        :param CertId: 已部署证书ID
+        :type CertId: str
+        :param Status: 域名状态
+        :type Status: str
+        """
+        self.Domain = None
+        self.CertId = None
+        self.Status = None
+
+
+    def _deserialize(self, params):
+        self.Domain = params.get("Domain")
+        self.CertId = params.get("CertId")
+        self.Status = params.get("Status")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class CertHostingInfo(AbstractModel):
     """云资源配置详情
 
     """
 
     def __init__(self):
         r"""
@@ -195,14 +268,42 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class Certificate(AbstractModel):
+    """CLB证书详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CertId: 证书ID
+        :type CertId: str
+        :param DnsNames: 证书绑定的域名
+        :type DnsNames: list of str
+        """
+        self.CertId = None
+        self.DnsNames = None
+
+
+    def _deserialize(self, params):
+        self.CertId = params.get("CertId")
+        self.DnsNames = params.get("DnsNames")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class CertificateExtra(AbstractModel):
     """获取证书列表（DescribeCertificates）返回参数键为 Certificates 数组下，key为CertificateExtra 的内容。
 
     """
 
     def __init__(self):
         r"""
@@ -521,14 +622,154 @@
     def _deserialize(self, params):
         self.IsValid = params.get("IsValid")
         self.IsTrustedCA = params.get("IsTrustedCA")
         self.Chains = params.get("Chains")
         self.RequestId = params.get("RequestId")
 
 
+class ClbInstanceDetail(AbstractModel):
+    """clb实例详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param LoadBalancerId: CLB实例ID
+        :type LoadBalancerId: str
+        :param LoadBalancerName: CLB实例名称
+        :type LoadBalancerName: str
+        :param Listeners: CLB监听器列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Listeners: list of ClbListener
+        """
+        self.LoadBalancerId = None
+        self.LoadBalancerName = None
+        self.Listeners = None
+
+
+    def _deserialize(self, params):
+        self.LoadBalancerId = params.get("LoadBalancerId")
+        self.LoadBalancerName = params.get("LoadBalancerName")
+        if params.get("Listeners") is not None:
+            self.Listeners = []
+            for item in params.get("Listeners"):
+                obj = ClbListener()
+                obj._deserialize(item)
+                self.Listeners.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ClbListener(AbstractModel):
+    """CLB实例监听器
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ListenerId: 监听器ID
+        :type ListenerId: str
+        :param ListenerName: 监听器名称
+        :type ListenerName: str
+        :param SniSwitch: 是否开启SNI，1为开启，0为关闭
+        :type SniSwitch: int
+        :param Protocol: 监听器协议类型， HTTPS|TCP_SSL
+        :type Protocol: str
+        :param Certificate: 监听器绑定的证书数据
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Certificate: :class:`tencentcloud.ssl.v20191205.models.Certificate`
+        :param Rules: 监听器规则列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Rules: list of ClbListenerRule
+        :param NoMatchDomains: 不匹配域名列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NoMatchDomains: list of str
+        """
+        self.ListenerId = None
+        self.ListenerName = None
+        self.SniSwitch = None
+        self.Protocol = None
+        self.Certificate = None
+        self.Rules = None
+        self.NoMatchDomains = None
+
+
+    def _deserialize(self, params):
+        self.ListenerId = params.get("ListenerId")
+        self.ListenerName = params.get("ListenerName")
+        self.SniSwitch = params.get("SniSwitch")
+        self.Protocol = params.get("Protocol")
+        if params.get("Certificate") is not None:
+            self.Certificate = Certificate()
+            self.Certificate._deserialize(params.get("Certificate"))
+        if params.get("Rules") is not None:
+            self.Rules = []
+            for item in params.get("Rules"):
+                obj = ClbListenerRule()
+                obj._deserialize(item)
+                self.Rules.append(obj)
+        self.NoMatchDomains = params.get("NoMatchDomains")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ClbListenerRule(AbstractModel):
+    """CLB监听器规则
+
+    """
+
+    def __init__(self):
+        r"""
+        :param LocationId: 规则ID
+        :type LocationId: str
+        :param Domain: 规则绑定的域名
+        :type Domain: str
+        :param IsMatch: 规则是否匹配待绑定证书的域名
+        :type IsMatch: bool
+        :param Certificate: 规则已绑定的证书数据
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Certificate: :class:`tencentcloud.ssl.v20191205.models.Certificate`
+        :param NoMatchDomains: 不匹配域名列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NoMatchDomains: list of str
+        """
+        self.LocationId = None
+        self.Domain = None
+        self.IsMatch = None
+        self.Certificate = None
+        self.NoMatchDomains = None
+
+
+    def _deserialize(self, params):
+        self.LocationId = params.get("LocationId")
+        self.Domain = params.get("Domain")
+        self.IsMatch = params.get("IsMatch")
+        if params.get("Certificate") is not None:
+            self.Certificate = Certificate()
+            self.Certificate._deserialize(params.get("Certificate"))
+        self.NoMatchDomains = params.get("NoMatchDomains")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class CommitCertificateInformationRequest(AbstractModel):
     """CommitCertificateInformation请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -673,14 +914,58 @@
 
 
     def _deserialize(self, params):
         self.CertificateId = params.get("CertificateId")
         self.RequestId = params.get("RequestId")
 
 
+class CosInstanceDetail(AbstractModel):
+    """COS实例详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Domain: 域名
+        :type Domain: str
+        :param CertId: 已绑定的证书ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CertId: str
+        :param Status: ENABLED: 域名上线状态
+DISABLED:域名下线状态
+        :type Status: str
+        :param Bucket: 存储桶名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Bucket: str
+        :param Region: 存储桶地域
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Region: str
+        """
+        self.Domain = None
+        self.CertId = None
+        self.Status = None
+        self.Bucket = None
+        self.Region = None
+
+
+    def _deserialize(self, params):
+        self.Domain = params.get("Domain")
+        self.CertId = params.get("CertId")
+        self.Status = params.get("Status")
+        self.Bucket = params.get("Bucket")
+        self.Region = params.get("Region")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class CreateCertificateRequest(AbstractModel):
     """CreateCertificate请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -730,14 +1015,55 @@
 
     def _deserialize(self, params):
         self.CertificateIds = params.get("CertificateIds")
         self.DealIds = params.get("DealIds")
         self.RequestId = params.get("RequestId")
 
 
+class DdosInstanceDetail(AbstractModel):
+    """ddos复杂类型
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Domain: 域名
+        :type Domain: str
+        :param InstanceId: 实例ID
+        :type InstanceId: str
+        :param Protocol: 协议类型
+        :type Protocol: str
+        :param CertId: 证书ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CertId: str
+        :param VirtualPort: 转发端口
+        :type VirtualPort: str
+        """
+        self.Domain = None
+        self.InstanceId = None
+        self.Protocol = None
+        self.CertId = None
+        self.VirtualPort = None
+
+
+    def _deserialize(self, params):
+        self.Domain = params.get("Domain")
+        self.InstanceId = params.get("InstanceId")
+        self.Protocol = params.get("Protocol")
+        self.CertId = params.get("CertId")
+        self.VirtualPort = params.get("VirtualPort")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class DeleteCertificateRequest(AbstractModel):
     """DeleteCertificate请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -820,14 +1146,318 @@
 
 
     def _deserialize(self, params):
         self.ManagerId = params.get("ManagerId")
         self.RequestId = params.get("RequestId")
 
 
+class DeployCertificateInstanceRequest(AbstractModel):
+    """DeployCertificateInstance请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CertificateId: 待部署的证书ID
+        :type CertificateId: str
+        :param InstanceIdList: 需要部署实例列表
+        :type InstanceIdList: list of str
+        :param ResourceType: 部署的云资源类型
+        :type ResourceType: str
+        :param Status: 部署云资源状态：
+云直播：
+-1：域名未关联证书。
+1： 域名https已开启。
+0： 域名https已关闭。
+        :type Status: int
+        """
+        self.CertificateId = None
+        self.InstanceIdList = None
+        self.ResourceType = None
+        self.Status = None
+
+
+    def _deserialize(self, params):
+        self.CertificateId = params.get("CertificateId")
+        self.InstanceIdList = params.get("InstanceIdList")
+        self.ResourceType = params.get("ResourceType")
+        self.Status = params.get("Status")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeployCertificateInstanceResponse(AbstractModel):
+    """DeployCertificateInstance返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DeployRecordId: 云资源部署任务ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DeployRecordId: int
+        :param DeployStatus: 部署状态，1表示部署成功，0表示部署失败
+        :type DeployStatus: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.DeployRecordId = None
+        self.DeployStatus = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.DeployRecordId = params.get("DeployRecordId")
+        self.DeployStatus = params.get("DeployStatus")
+        self.RequestId = params.get("RequestId")
+
+
+class DeployCertificateRecordRetryRequest(AbstractModel):
+    """DeployCertificateRecordRetry请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DeployRecordId: 待重试部署记录ID
+        :type DeployRecordId: int
+        :param DeployRecordDetailId: 待重试部署记录详情ID
+        :type DeployRecordDetailId: int
+        """
+        self.DeployRecordId = None
+        self.DeployRecordDetailId = None
+
+
+    def _deserialize(self, params):
+        self.DeployRecordId = params.get("DeployRecordId")
+        self.DeployRecordDetailId = params.get("DeployRecordDetailId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeployCertificateRecordRetryResponse(AbstractModel):
+    """DeployCertificateRecordRetry返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class DeployCertificateRecordRollbackRequest(AbstractModel):
+    """DeployCertificateRecordRollback请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DeployRecordId: 待重试部署记录ID
+        :type DeployRecordId: int
+        """
+        self.DeployRecordId = None
+
+
+    def _deserialize(self, params):
+        self.DeployRecordId = params.get("DeployRecordId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeployCertificateRecordRollbackResponse(AbstractModel):
+    """DeployCertificateRecordRollback返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DeployRecordId: 回滚部署记录ID
+        :type DeployRecordId: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.DeployRecordId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.DeployRecordId = params.get("DeployRecordId")
+        self.RequestId = params.get("RequestId")
+
+
+class DeployRecordDetail(AbstractModel):
+    """部署记录详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Id: 部署记录详情ID
+        :type Id: int
+        :param CertId: 部署证书ID
+        :type CertId: str
+        :param OldCertId: 原绑定证书ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OldCertId: str
+        :param InstanceId: 部署实例ID
+        :type InstanceId: str
+        :param InstanceName: 部署实例名称
+        :type InstanceName: str
+        :param ListenerId: 部署监听器ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ListenerId: str
+        :param Domains: 部署域名列表
+        :type Domains: list of str
+        :param Protocol: 部署监听器协议
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Protocol: str
+        :param Status: 部署状态
+        :type Status: int
+        :param ErrorMsg: 部署错误信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ErrorMsg: str
+        :param CreateTime: 部署记录详情创建时间
+        :type CreateTime: str
+        :param UpdateTime: 部署记录详情最后一次更新时间
+        :type UpdateTime: str
+        :param ListenerName: 部署监听器名称
+        :type ListenerName: str
+        :param SniSwitch: 是否开启SNI
+        :type SniSwitch: int
+        :param Bucket: COS存储桶名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Bucket: str
+        :param Namespace: 命名空间名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Namespace: str
+        :param SecretName: secret名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SecretName: str
+        :param Port: 端口
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Port: int
+        """
+        self.Id = None
+        self.CertId = None
+        self.OldCertId = None
+        self.InstanceId = None
+        self.InstanceName = None
+        self.ListenerId = None
+        self.Domains = None
+        self.Protocol = None
+        self.Status = None
+        self.ErrorMsg = None
+        self.CreateTime = None
+        self.UpdateTime = None
+        self.ListenerName = None
+        self.SniSwitch = None
+        self.Bucket = None
+        self.Namespace = None
+        self.SecretName = None
+        self.Port = None
+
+
+    def _deserialize(self, params):
+        self.Id = params.get("Id")
+        self.CertId = params.get("CertId")
+        self.OldCertId = params.get("OldCertId")
+        self.InstanceId = params.get("InstanceId")
+        self.InstanceName = params.get("InstanceName")
+        self.ListenerId = params.get("ListenerId")
+        self.Domains = params.get("Domains")
+        self.Protocol = params.get("Protocol")
+        self.Status = params.get("Status")
+        self.ErrorMsg = params.get("ErrorMsg")
+        self.CreateTime = params.get("CreateTime")
+        self.UpdateTime = params.get("UpdateTime")
+        self.ListenerName = params.get("ListenerName")
+        self.SniSwitch = params.get("SniSwitch")
+        self.Bucket = params.get("Bucket")
+        self.Namespace = params.get("Namespace")
+        self.SecretName = params.get("SecretName")
+        self.Port = params.get("Port")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeployRecordInfo(AbstractModel):
+    """部署记录信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Id: 部署记录ID
+        :type Id: int
+        :param CertId: 部署证书ID
+        :type CertId: str
+        :param ResourceType: 部署资源类型
+        :type ResourceType: str
+        :param Region: 部署地域
+        :type Region: str
+        :param Status: 部署状态
+        :type Status: int
+        :param CreateTime: 部署时间
+        :type CreateTime: str
+        :param UpdateTime: 最近一次更新时间
+        :type UpdateTime: str
+        """
+        self.Id = None
+        self.CertId = None
+        self.ResourceType = None
+        self.Region = None
+        self.Status = None
+        self.CreateTime = None
+        self.UpdateTime = None
+
+
+    def _deserialize(self, params):
+        self.Id = params.get("Id")
+        self.CertId = params.get("CertId")
+        self.ResourceType = params.get("ResourceType")
+        self.Region = params.get("Region")
+        self.Status = params.get("Status")
+        self.CreateTime = params.get("CreateTime")
+        self.UpdateTime = params.get("UpdateTime")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class DeployedResources(AbstractModel):
     """资源详情
 
     """
 
     def __init__(self):
         r"""
@@ -1634,14 +2264,1176 @@
             for item in params.get("DeployedResources"):
                 obj = DeployedResources()
                 obj._deserialize(item)
                 self.DeployedResources.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeHostApiGatewayInstanceListRequest(AbstractModel):
+    """DescribeHostApiGatewayInstanceList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CertificateId: 待部署的证书ID
+        :type CertificateId: str
+        :param ResourceType: 部署资源类型
+        :type ResourceType: str
+        :param IsCache: 是否查询缓存，1：是； 0：否， 默认为查询缓存，缓存半小时
+        :type IsCache: int
+        :param Filters: 过滤参数列表； FilterKey：domainMatch（查询域名是否匹配的实例列表） FilterValue：1，表示查询匹配； 0，表示查询不匹配； 默认查询匹配
+        :type Filters: list of Filter
+        :param OldCertificateId: 已部署的证书ID
+        :type OldCertificateId: str
+        """
+        self.CertificateId = None
+        self.ResourceType = None
+        self.IsCache = None
+        self.Filters = None
+        self.OldCertificateId = None
+
+
+    def _deserialize(self, params):
+        self.CertificateId = params.get("CertificateId")
+        self.ResourceType = params.get("ResourceType")
+        self.IsCache = params.get("IsCache")
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self.Filters.append(obj)
+        self.OldCertificateId = params.get("OldCertificateId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeHostApiGatewayInstanceListResponse(AbstractModel):
+    """DescribeHostApiGatewayInstanceList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceList: apiGateway实例列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceList: list of ApiGatewayInstanceDetail
+        :param TotalCount: 总数
+        :type TotalCount: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.InstanceList = None
+        self.TotalCount = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("InstanceList") is not None:
+            self.InstanceList = []
+            for item in params.get("InstanceList"):
+                obj = ApiGatewayInstanceDetail()
+                obj._deserialize(item)
+                self.InstanceList.append(obj)
+        self.TotalCount = params.get("TotalCount")
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeHostCdnInstanceListRequest(AbstractModel):
+    """DescribeHostCdnInstanceList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CertificateId: 待部署的证书ID
+        :type CertificateId: str
+        :param ResourceType: 部署资源类型
+        :type ResourceType: str
+        :param IsCache: 是否查询缓存，1：是； 0：否， 默认为查询缓存，缓存半小时
+        :type IsCache: int
+        :param Filters: 过滤参数列表； FilterKey：domainMatch（查询域名是否匹配的实例列表） FilterValue：1，表示查询匹配； 0，表示查询不匹配； 默认查询匹配
+        :type Filters: list of Filter
+        :param OldCertificateId: 原证书ID
+        :type OldCertificateId: str
+        :param Offset: 分页偏移量，从0开始。	
+        :type Offset: int
+        :param Limit: 每页数量，默认10。	
+        :type Limit: int
+        """
+        self.CertificateId = None
+        self.ResourceType = None
+        self.IsCache = None
+        self.Filters = None
+        self.OldCertificateId = None
+        self.Offset = None
+        self.Limit = None
+
+
+    def _deserialize(self, params):
+        self.CertificateId = params.get("CertificateId")
+        self.ResourceType = params.get("ResourceType")
+        self.IsCache = params.get("IsCache")
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self.Filters.append(obj)
+        self.OldCertificateId = params.get("OldCertificateId")
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeHostCdnInstanceListResponse(AbstractModel):
+    """DescribeHostCdnInstanceList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceList: CDN实例列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceList: list of CdnInstanceDetail
+        :param TotalCount: CDN域名总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCount: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.InstanceList = None
+        self.TotalCount = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("InstanceList") is not None:
+            self.InstanceList = []
+            for item in params.get("InstanceList"):
+                obj = CdnInstanceDetail()
+                obj._deserialize(item)
+                self.InstanceList.append(obj)
+        self.TotalCount = params.get("TotalCount")
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeHostClbInstanceListRequest(AbstractModel):
+    """DescribeHostClbInstanceList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CertificateId: 待部署的证书ID
+        :type CertificateId: str
+        :param Offset: 分页偏移量，从0开始。
+        :type Offset: int
+        :param Limit: 每页数量，默认10。
+        :type Limit: int
+        :param IsCache: 是否查询缓存，1：是； 0：否， 默认为查询缓存，缓存半小时
+        :type IsCache: int
+        :param Filters: 过滤参数列表； FilterKey：domainMatch（查询域名是否匹配的实例列表） FilterValue：1，表示查询匹配； 0，表示查询不匹配； 默认查询匹配
+        :type Filters: list of Filter
+        :param AsyncCache: 是否异步缓存
+        :type AsyncCache: int
+        :param OldCertificateId: 原证书ID
+        :type OldCertificateId: str
+        """
+        self.CertificateId = None
+        self.Offset = None
+        self.Limit = None
+        self.IsCache = None
+        self.Filters = None
+        self.AsyncCache = None
+        self.OldCertificateId = None
+
+
+    def _deserialize(self, params):
+        self.CertificateId = params.get("CertificateId")
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        self.IsCache = params.get("IsCache")
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self.Filters.append(obj)
+        self.AsyncCache = params.get("AsyncCache")
+        self.OldCertificateId = params.get("OldCertificateId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeHostClbInstanceListResponse(AbstractModel):
+    """DescribeHostClbInstanceList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCount: int
+        :param InstanceList: CLB实例监听器列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceList: list of ClbInstanceDetail
+        :param AsyncTotalNum: 异步刷新总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AsyncTotalNum: int
+        :param AsyncOffset: 异步刷新当前执行数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AsyncOffset: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.InstanceList = None
+        self.AsyncTotalNum = None
+        self.AsyncOffset = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("InstanceList") is not None:
+            self.InstanceList = []
+            for item in params.get("InstanceList"):
+                obj = ClbInstanceDetail()
+                obj._deserialize(item)
+                self.InstanceList.append(obj)
+        self.AsyncTotalNum = params.get("AsyncTotalNum")
+        self.AsyncOffset = params.get("AsyncOffset")
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeHostCosInstanceListRequest(AbstractModel):
+    """DescribeHostCosInstanceList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CertificateId: 待部署的证书ID
+        :type CertificateId: str
+        :param ResourceType: 部署资源类型 cos
+        :type ResourceType: str
+        :param IsCache: 是否查询缓存，1：是； 0：否， 默认为查询缓存，缓存半小时
+        :type IsCache: int
+        :param Filters: 过滤参数列表
+        :type Filters: list of Filter
+        """
+        self.CertificateId = None
+        self.ResourceType = None
+        self.IsCache = None
+        self.Filters = None
+
+
+    def _deserialize(self, params):
+        self.CertificateId = params.get("CertificateId")
+        self.ResourceType = params.get("ResourceType")
+        self.IsCache = params.get("IsCache")
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self.Filters.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeHostCosInstanceListResponse(AbstractModel):
+    """DescribeHostCosInstanceList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceList: COS实例列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceList: list of CosInstanceDetail
+        :param TotalCount: 总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCount: int
+        :param AsyncTotalNum: 异步刷新总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AsyncTotalNum: int
+        :param AsyncOffset: 异步刷新当前执行数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AsyncOffset: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.InstanceList = None
+        self.TotalCount = None
+        self.AsyncTotalNum = None
+        self.AsyncOffset = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("InstanceList") is not None:
+            self.InstanceList = []
+            for item in params.get("InstanceList"):
+                obj = CosInstanceDetail()
+                obj._deserialize(item)
+                self.InstanceList.append(obj)
+        self.TotalCount = params.get("TotalCount")
+        self.AsyncTotalNum = params.get("AsyncTotalNum")
+        self.AsyncOffset = params.get("AsyncOffset")
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeHostDdosInstanceListRequest(AbstractModel):
+    """DescribeHostDdosInstanceList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CertificateId: 待部署的证书ID
+        :type CertificateId: str
+        :param ResourceType: 部署资源类型
+        :type ResourceType: str
+        :param IsCache: 是否查询缓存，1：是； 0：否， 默认为查询缓存，缓存半小时
+        :type IsCache: int
+        :param Filters: 过滤参数列表； FilterKey：domainMatch（查询域名是否匹配的实例列表） FilterValue：1，表示查询匹配； 0，表示查询不匹配； 默认查询匹配
+        :type Filters: list of Filter
+        :param OldCertificateId: 已部署的证书ID
+        :type OldCertificateId: str
+        """
+        self.CertificateId = None
+        self.ResourceType = None
+        self.IsCache = None
+        self.Filters = None
+        self.OldCertificateId = None
+
+
+    def _deserialize(self, params):
+        self.CertificateId = params.get("CertificateId")
+        self.ResourceType = params.get("ResourceType")
+        self.IsCache = params.get("IsCache")
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self.Filters.append(obj)
+        self.OldCertificateId = params.get("OldCertificateId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeHostDdosInstanceListResponse(AbstractModel):
+    """DescribeHostDdosInstanceList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceList: DDOS实例列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceList: list of DdosInstanceDetail
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.InstanceList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("InstanceList") is not None:
+            self.InstanceList = []
+            for item in params.get("InstanceList"):
+                obj = DdosInstanceDetail()
+                obj._deserialize(item)
+                self.InstanceList.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeHostDeployRecordDetailRequest(AbstractModel):
+    """DescribeHostDeployRecordDetail请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DeployRecordId: 待部署的证书ID
+        :type DeployRecordId: str
+        :param Offset: 分页偏移量，从0开始。
+        :type Offset: int
+        :param Limit: 每页数量，默认10。
+        :type Limit: int
+        """
+        self.DeployRecordId = None
+        self.Offset = None
+        self.Limit = None
+
+
+    def _deserialize(self, params):
+        self.DeployRecordId = params.get("DeployRecordId")
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeHostDeployRecordDetailResponse(AbstractModel):
+    """DescribeHostDeployRecordDetail返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCount: int
+        :param DeployRecordDetailList: 证书部署记录列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DeployRecordDetailList: list of DeployRecordDetail
+        :param SuccessTotalCount: 成功总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SuccessTotalCount: int
+        :param FailedTotalCount: 失败总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FailedTotalCount: int
+        :param RunningTotalCount: 部署中总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RunningTotalCount: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.DeployRecordDetailList = None
+        self.SuccessTotalCount = None
+        self.FailedTotalCount = None
+        self.RunningTotalCount = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("DeployRecordDetailList") is not None:
+            self.DeployRecordDetailList = []
+            for item in params.get("DeployRecordDetailList"):
+                obj = DeployRecordDetail()
+                obj._deserialize(item)
+                self.DeployRecordDetailList.append(obj)
+        self.SuccessTotalCount = params.get("SuccessTotalCount")
+        self.FailedTotalCount = params.get("FailedTotalCount")
+        self.RunningTotalCount = params.get("RunningTotalCount")
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeHostDeployRecordRequest(AbstractModel):
+    """DescribeHostDeployRecord请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CertificateId: 待部署的证书ID
+        :type CertificateId: str
+        :param Offset: 分页偏移量，从0开始。
+        :type Offset: int
+        :param Limit: 每页数量，默认10。
+        :type Limit: int
+        :param ResourceType: 资源类型
+        :type ResourceType: str
+        """
+        self.CertificateId = None
+        self.Offset = None
+        self.Limit = None
+        self.ResourceType = None
+
+
+    def _deserialize(self, params):
+        self.CertificateId = params.get("CertificateId")
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        self.ResourceType = params.get("ResourceType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeHostDeployRecordResponse(AbstractModel):
+    """DescribeHostDeployRecord返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCount: int
+        :param DeployRecordList: 证书部署记录列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DeployRecordList: list of DeployRecordInfo
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.DeployRecordList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("DeployRecordList") is not None:
+            self.DeployRecordList = []
+            for item in params.get("DeployRecordList"):
+                obj = DeployRecordInfo()
+                obj._deserialize(item)
+                self.DeployRecordList.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeHostLighthouseInstanceListRequest(AbstractModel):
+    """DescribeHostLighthouseInstanceList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CertificateId: 待部署的证书ID
+        :type CertificateId: str
+        :param ResourceType: 部署资源类型 lighthouse
+        :type ResourceType: str
+        :param IsCache: 是否查询缓存，1：是； 0：否， 默认为查询缓存，缓存半小时
+        :type IsCache: int
+        :param Filters: 过滤参数列表
+        :type Filters: list of Filter
+        """
+        self.CertificateId = None
+        self.ResourceType = None
+        self.IsCache = None
+        self.Filters = None
+
+
+    def _deserialize(self, params):
+        self.CertificateId = params.get("CertificateId")
+        self.ResourceType = params.get("ResourceType")
+        self.IsCache = params.get("IsCache")
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self.Filters.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeHostLighthouseInstanceListResponse(AbstractModel):
+    """DescribeHostLighthouseInstanceList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceList: Lighthouse实例列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceList: list of LighthouseInstanceDetail
+        :param TotalCount: 总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCount: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.InstanceList = None
+        self.TotalCount = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("InstanceList") is not None:
+            self.InstanceList = []
+            for item in params.get("InstanceList"):
+                obj = LighthouseInstanceDetail()
+                obj._deserialize(item)
+                self.InstanceList.append(obj)
+        self.TotalCount = params.get("TotalCount")
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeHostLiveInstanceListRequest(AbstractModel):
+    """DescribeHostLiveInstanceList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CertificateId: 待部署的证书ID
+        :type CertificateId: str
+        :param ResourceType: 部署资源类型
+        :type ResourceType: str
+        :param IsCache: 是否查询缓存，1：是； 0：否， 默认为查询缓存，缓存半小时
+        :type IsCache: int
+        :param Filters: 过滤参数列表； FilterKey：domainMatch（查询域名是否匹配的实例列表） FilterValue：1，表示查询匹配； 0，表示查询不匹配； 默认查询匹配
+        :type Filters: list of Filter
+        :param OldCertificateId: 已部署的证书ID
+        :type OldCertificateId: str
+        """
+        self.CertificateId = None
+        self.ResourceType = None
+        self.IsCache = None
+        self.Filters = None
+        self.OldCertificateId = None
+
+
+    def _deserialize(self, params):
+        self.CertificateId = params.get("CertificateId")
+        self.ResourceType = params.get("ResourceType")
+        self.IsCache = params.get("IsCache")
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self.Filters.append(obj)
+        self.OldCertificateId = params.get("OldCertificateId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeHostLiveInstanceListResponse(AbstractModel):
+    """DescribeHostLiveInstanceList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceList: live实例列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceList: list of LiveInstanceDetail
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.InstanceList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("InstanceList") is not None:
+            self.InstanceList = []
+            for item in params.get("InstanceList"):
+                obj = LiveInstanceDetail()
+                obj._deserialize(item)
+                self.InstanceList.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeHostTeoInstanceListRequest(AbstractModel):
+    """DescribeHostTeoInstanceList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CertificateId: 待部署的证书ID
+        :type CertificateId: str
+        :param ResourceType: 部署资源类型
+        :type ResourceType: str
+        :param IsCache: 是否查询缓存，1：是； 0：否， 默认为查询缓存，缓存半小时
+        :type IsCache: int
+        :param Filters: 过滤参数列表； FilterKey：domainMatch（查询域名是否匹配的实例列表） FilterValue：1，表示查询匹配； 0，表示查询不匹配； 默认查询匹配
+        :type Filters: list of Filter
+        :param OldCertificateId: 已部署的证书ID
+        :type OldCertificateId: str
+        """
+        self.CertificateId = None
+        self.ResourceType = None
+        self.IsCache = None
+        self.Filters = None
+        self.OldCertificateId = None
+
+
+    def _deserialize(self, params):
+        self.CertificateId = params.get("CertificateId")
+        self.ResourceType = params.get("ResourceType")
+        self.IsCache = params.get("IsCache")
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self.Filters.append(obj)
+        self.OldCertificateId = params.get("OldCertificateId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeHostTeoInstanceListResponse(AbstractModel):
+    """DescribeHostTeoInstanceList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceList: teo实例列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceList: list of TeoInstanceDetail
+        :param TotalCount: 总数
+        :type TotalCount: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.InstanceList = None
+        self.TotalCount = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("InstanceList") is not None:
+            self.InstanceList = []
+            for item in params.get("InstanceList"):
+                obj = TeoInstanceDetail()
+                obj._deserialize(item)
+                self.InstanceList.append(obj)
+        self.TotalCount = params.get("TotalCount")
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeHostTkeInstanceListRequest(AbstractModel):
+    """DescribeHostTkeInstanceList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CertificateId: 待部署的证书ID
+        :type CertificateId: str
+        :param Offset: 分页偏移量，从0开始。
+        :type Offset: int
+        :param Limit: 每页数量，默认10。
+        :type Limit: int
+        :param IsCache: 是否查询缓存，1：是； 0：否， 默认为查询缓存，缓存半小时
+        :type IsCache: int
+        :param Filters: 过滤参数列表； FilterKey：domainMatch（查询域名是否匹配的实例列表） FilterValue：1，表示查询匹配； 0，表示查询不匹配； 默认查询匹配
+        :type Filters: list of Filter
+        :param AsyncCache: 是否异步缓存
+        :type AsyncCache: int
+        :param OldCertificateId: 原证书ID
+        :type OldCertificateId: str
+        """
+        self.CertificateId = None
+        self.Offset = None
+        self.Limit = None
+        self.IsCache = None
+        self.Filters = None
+        self.AsyncCache = None
+        self.OldCertificateId = None
+
+
+    def _deserialize(self, params):
+        self.CertificateId = params.get("CertificateId")
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        self.IsCache = params.get("IsCache")
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self.Filters.append(obj)
+        self.AsyncCache = params.get("AsyncCache")
+        self.OldCertificateId = params.get("OldCertificateId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeHostTkeInstanceListResponse(AbstractModel):
+    """DescribeHostTkeInstanceList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCount: int
+        :param InstanceList: CLB实例监听器列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceList: list of TkeInstanceDetail
+        :param AsyncTotalNum: 异步刷新总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AsyncTotalNum: int
+        :param AsyncOffset: 异步刷新当前执行数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AsyncOffset: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.InstanceList = None
+        self.AsyncTotalNum = None
+        self.AsyncOffset = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("InstanceList") is not None:
+            self.InstanceList = []
+            for item in params.get("InstanceList"):
+                obj = TkeInstanceDetail()
+                obj._deserialize(item)
+                self.InstanceList.append(obj)
+        self.AsyncTotalNum = params.get("AsyncTotalNum")
+        self.AsyncOffset = params.get("AsyncOffset")
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeHostUpdateRecordDetailRequest(AbstractModel):
+    """DescribeHostUpdateRecordDetail请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DeployRecordId: 待部署的证书ID
+        :type DeployRecordId: str
+        """
+        self.DeployRecordId = None
+
+
+    def _deserialize(self, params):
+        self.DeployRecordId = params.get("DeployRecordId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeHostUpdateRecordDetailResponse(AbstractModel):
+    """DescribeHostUpdateRecordDetail返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCount: int
+        :param RecordDetailList: 证书部署记录列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RecordDetailList: list of UpdateRecordDetails
+        :param SuccessTotalCount: 成功总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SuccessTotalCount: int
+        :param FailedTotalCount: 失败总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FailedTotalCount: int
+        :param RunningTotalCount: 部署中总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RunningTotalCount: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.RecordDetailList = None
+        self.SuccessTotalCount = None
+        self.FailedTotalCount = None
+        self.RunningTotalCount = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("RecordDetailList") is not None:
+            self.RecordDetailList = []
+            for item in params.get("RecordDetailList"):
+                obj = UpdateRecordDetails()
+                obj._deserialize(item)
+                self.RecordDetailList.append(obj)
+        self.SuccessTotalCount = params.get("SuccessTotalCount")
+        self.FailedTotalCount = params.get("FailedTotalCount")
+        self.RunningTotalCount = params.get("RunningTotalCount")
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeHostUpdateRecordRequest(AbstractModel):
+    """DescribeHostUpdateRecord请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Offset: 分页偏移量，从0开始。
+        :type Offset: int
+        :param Limit: 每页数量，默认10。
+        :type Limit: int
+        :param CertificateId: 新证书ID
+        :type CertificateId: str
+        :param OldCertificateId: 原证书ID
+        :type OldCertificateId: str
+        """
+        self.Offset = None
+        self.Limit = None
+        self.CertificateId = None
+        self.OldCertificateId = None
+
+
+    def _deserialize(self, params):
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        self.CertificateId = params.get("CertificateId")
+        self.OldCertificateId = params.get("OldCertificateId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeHostUpdateRecordResponse(AbstractModel):
+    """DescribeHostUpdateRecord返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCount: int
+        :param DeployRecordList: 证书部署记录列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DeployRecordList: list of UpdateRecordInfo
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.DeployRecordList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("DeployRecordList") is not None:
+            self.DeployRecordList = []
+            for item in params.get("DeployRecordList"):
+                obj = UpdateRecordInfo()
+                obj._deserialize(item)
+                self.DeployRecordList.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeHostVodInstanceListRequest(AbstractModel):
+    """DescribeHostVodInstanceList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CertificateId: 待部署的证书ID
+        :type CertificateId: str
+        :param ResourceType: 部署资源类型 vod
+        :type ResourceType: str
+        :param IsCache: 是否查询缓存，1：是； 0：否， 默认为查询缓存，缓存半小时
+        :type IsCache: int
+        :param Filters: 过滤参数列表
+        :type Filters: list of Filter
+        :param OldCertificateId: 已部署的证书ID
+        :type OldCertificateId: str
+        """
+        self.CertificateId = None
+        self.ResourceType = None
+        self.IsCache = None
+        self.Filters = None
+        self.OldCertificateId = None
+
+
+    def _deserialize(self, params):
+        self.CertificateId = params.get("CertificateId")
+        self.ResourceType = params.get("ResourceType")
+        self.IsCache = params.get("IsCache")
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self.Filters.append(obj)
+        self.OldCertificateId = params.get("OldCertificateId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeHostVodInstanceListResponse(AbstractModel):
+    """DescribeHostVodInstanceList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceList: Vod实例列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceList: list of VodInstanceDetail
+        :param TotalCount: 总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCount: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.InstanceList = None
+        self.TotalCount = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("InstanceList") is not None:
+            self.InstanceList = []
+            for item in params.get("InstanceList"):
+                obj = VodInstanceDetail()
+                obj._deserialize(item)
+                self.InstanceList.append(obj)
+        self.TotalCount = params.get("TotalCount")
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeHostWafInstanceListRequest(AbstractModel):
+    """DescribeHostWafInstanceList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CertificateId: 待部署的证书ID
+        :type CertificateId: str
+        :param ResourceType: 部署资源类型
+        :type ResourceType: str
+        :param IsCache: 是否查询缓存，1：是； 0：否， 默认为查询缓存，缓存半小时
+        :type IsCache: int
+        :param Filters: 过滤参数列表； FilterKey：domainMatch（查询域名是否匹配的实例列表） FilterValue：1，表示查询匹配； 0，表示查询不匹配； 默认查询匹配
+        :type Filters: list of Filter
+        :param OldCertificateId: 已部署的证书ID
+        :type OldCertificateId: str
+        """
+        self.CertificateId = None
+        self.ResourceType = None
+        self.IsCache = None
+        self.Filters = None
+        self.OldCertificateId = None
+
+
+    def _deserialize(self, params):
+        self.CertificateId = params.get("CertificateId")
+        self.ResourceType = params.get("ResourceType")
+        self.IsCache = params.get("IsCache")
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self.Filters.append(obj)
+        self.OldCertificateId = params.get("OldCertificateId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeHostWafInstanceListResponse(AbstractModel):
+    """DescribeHostWafInstanceList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceList: WAF实例列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceList: list of LiveInstanceDetail
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.InstanceList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("InstanceList") is not None:
+            self.InstanceList = []
+            for item in params.get("InstanceList"):
+                obj = LiveInstanceDetail()
+                obj._deserialize(item)
+                self.InstanceList.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeManagerDetailRequest(AbstractModel):
     """DescribeManagerDetail请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2091,14 +3883,42 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class Filter(AbstractModel):
+    """过滤参数列表
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FilterKey: 过滤参数key
+        :type FilterKey: str
+        :param FilterValue: 过滤参数值
+        :type FilterValue: str
+        """
+        self.FilterKey = None
+        self.FilterValue = None
+
+
+    def _deserialize(self, params):
+        self.FilterKey = params.get("FilterKey")
+        self.FilterValue = params.get("FilterValue")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class HostCertificateRequest(AbstractModel):
     """HostCertificate请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2142,14 +3962,85 @@
     def _deserialize(self, params):
         if params.get("CertHostingInfo") is not None:
             self.CertHostingInfo = CertHostingInfo()
             self.CertHostingInfo._deserialize(params.get("CertHostingInfo"))
         self.RequestId = params.get("RequestId")
 
 
+class LighthouseInstanceDetail(AbstractModel):
+    """Lighthouse实例
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 实例ID
+        :type InstanceId: str
+        :param InstanceName: 实例名称
+        :type InstanceName: str
+        :param IP: IP地址
+        :type IP: list of str
+        :param Domain: 可选择域名
+        :type Domain: list of str
+        """
+        self.InstanceId = None
+        self.InstanceName = None
+        self.IP = None
+        self.Domain = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.InstanceName = params.get("InstanceName")
+        self.IP = params.get("IP")
+        self.Domain = params.get("Domain")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class LiveInstanceDetail(AbstractModel):
+    """live实例详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Domain: 域名
+        :type Domain: str
+        :param CertId: 已绑定的证书ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CertId: str
+        :param Status: -1：域名未关联证书。
+1： 域名https已开启。
+0： 域名https已关闭。
+        :type Status: int
+        """
+        self.Domain = None
+        self.CertId = None
+        self.Status = None
+
+
+    def _deserialize(self, params):
+        self.Domain = params.get("Domain")
+        self.CertId = params.get("CertId")
+        self.Status = params.get("Status")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ManagerInfo(AbstractModel):
     """管理人信息
 
     """
 
     def __init__(self):
         r"""
@@ -2703,14 +4594,42 @@
 
 
     def _deserialize(self, params):
         self.CertificateId = params.get("CertificateId")
         self.RequestId = params.get("RequestId")
 
 
+class ResourceTypeRegions(AbstractModel):
+    """云资源地域列表
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ResourceType: 云资源类型
+        :type ResourceType: str
+        :param Regions: 地域列表
+        :type Regions: list of str
+        """
+        self.ResourceType = None
+        self.Regions = None
+
+
+    def _deserialize(self, params):
+        self.ResourceType = params.get("ResourceType")
+        self.Regions = params.get("Regions")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class RevokeCertificateRequest(AbstractModel):
     """RevokeCertificate请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -3196,14 +5115,531 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class TeoInstanceDetail(AbstractModel):
+    """teo实例详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Host: 域名
+        :type Host: str
+        :param CertId: 证书ID
+        :type CertId: str
+        """
+        self.Host = None
+        self.CertId = None
+
+
+    def _deserialize(self, params):
+        self.Host = params.get("Host")
+        self.CertId = params.get("CertId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class TkeIngressDetail(AbstractModel):
+    """tke ingress实例详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param IngressName: ingress名称
+        :type IngressName: str
+        :param TlsDomains: tls域名列表
+        :type TlsDomains: list of str
+        :param Domains: ingress域名列表
+        :type Domains: list of str
+        """
+        self.IngressName = None
+        self.TlsDomains = None
+        self.Domains = None
+
+
+    def _deserialize(self, params):
+        self.IngressName = params.get("IngressName")
+        self.TlsDomains = params.get("TlsDomains")
+        self.Domains = params.get("Domains")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class TkeInstanceDetail(AbstractModel):
+    """tke实例详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 集群ID
+        :type ClusterId: str
+        :param ClusterName: 集群名称
+        :type ClusterName: str
+        :param NamespaceList: 集群命名空间列表
+        :type NamespaceList: list of TkeNameSpaceDetail
+        """
+        self.ClusterId = None
+        self.ClusterName = None
+        self.NamespaceList = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        self.ClusterName = params.get("ClusterName")
+        if params.get("NamespaceList") is not None:
+            self.NamespaceList = []
+            for item in params.get("NamespaceList"):
+                obj = TkeNameSpaceDetail()
+                obj._deserialize(item)
+                self.NamespaceList.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class TkeNameSpaceDetail(AbstractModel):
+    """tke namespace详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Name: namespace名称
+        :type Name: str
+        :param SecretList: secret列表
+        :type SecretList: list of TkeSecretDetail
+        """
+        self.Name = None
+        self.SecretList = None
+
+
+    def _deserialize(self, params):
+        self.Name = params.get("Name")
+        if params.get("SecretList") is not None:
+            self.SecretList = []
+            for item in params.get("SecretList"):
+                obj = TkeSecretDetail()
+                obj._deserialize(item)
+                self.SecretList.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class TkeSecretDetail(AbstractModel):
+    """tke secret详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Name: secret名称
+        :type Name: str
+        :param CertId: 证书ID
+        :type CertId: str
+        :param IngressList: ingress列表
+        :type IngressList: list of TkeIngressDetail
+        :param NoMatchDomains: 和新证书不匹配的域名列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NoMatchDomains: list of str
+        """
+        self.Name = None
+        self.CertId = None
+        self.IngressList = None
+        self.NoMatchDomains = None
+
+
+    def _deserialize(self, params):
+        self.Name = params.get("Name")
+        self.CertId = params.get("CertId")
+        if params.get("IngressList") is not None:
+            self.IngressList = []
+            for item in params.get("IngressList"):
+                obj = TkeIngressDetail()
+                obj._deserialize(item)
+                self.IngressList.append(obj)
+        self.NoMatchDomains = params.get("NoMatchDomains")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UpdateCertificateInstanceRequest(AbstractModel):
+    """UpdateCertificateInstance请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CertificateId: 一键更新新证书ID
+        :type CertificateId: str
+        :param OldCertificateId: 一键更新原证书ID
+        :type OldCertificateId: str
+        :param ResourceTypes: 需要部署的资源类型
+        :type ResourceTypes: list of str
+        :param Regions: 需要部署的地域列表（废弃）
+        :type Regions: list of str
+        :param ResourceTypesRegions: 云资源需要部署的地域列表
+        :type ResourceTypesRegions: list of ResourceTypeRegions
+        """
+        self.CertificateId = None
+        self.OldCertificateId = None
+        self.ResourceTypes = None
+        self.Regions = None
+        self.ResourceTypesRegions = None
+
+
+    def _deserialize(self, params):
+        self.CertificateId = params.get("CertificateId")
+        self.OldCertificateId = params.get("OldCertificateId")
+        self.ResourceTypes = params.get("ResourceTypes")
+        self.Regions = params.get("Regions")
+        if params.get("ResourceTypesRegions") is not None:
+            self.ResourceTypesRegions = []
+            for item in params.get("ResourceTypesRegions"):
+                obj = ResourceTypeRegions()
+                obj._deserialize(item)
+                self.ResourceTypesRegions.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UpdateCertificateInstanceResponse(AbstractModel):
+    """UpdateCertificateInstance返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DeployRecordId: 云资源部署任务ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DeployRecordId: int
+        :param DeployStatus: 部署状态，1表示部署成功，0表示部署失败
+        :type DeployStatus: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.DeployRecordId = None
+        self.DeployStatus = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.DeployRecordId = params.get("DeployRecordId")
+        self.DeployStatus = params.get("DeployStatus")
+        self.RequestId = params.get("RequestId")
+
+
+class UpdateCertificateRecordRetryRequest(AbstractModel):
+    """UpdateCertificateRecordRetry请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DeployRecordId: 待重试部署记录ID
+        :type DeployRecordId: int
+        :param DeployRecordDetailId: 待重试部署记录详情ID
+        :type DeployRecordDetailId: int
+        """
+        self.DeployRecordId = None
+        self.DeployRecordDetailId = None
+
+
+    def _deserialize(self, params):
+        self.DeployRecordId = params.get("DeployRecordId")
+        self.DeployRecordDetailId = params.get("DeployRecordDetailId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UpdateCertificateRecordRetryResponse(AbstractModel):
+    """UpdateCertificateRecordRetry返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class UpdateCertificateRecordRollbackRequest(AbstractModel):
+    """UpdateCertificateRecordRollback请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DeployRecordId: 待重试部署记录ID
+        :type DeployRecordId: int
+        """
+        self.DeployRecordId = None
+
+
+    def _deserialize(self, params):
+        self.DeployRecordId = params.get("DeployRecordId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UpdateCertificateRecordRollbackResponse(AbstractModel):
+    """UpdateCertificateRecordRollback返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DeployRecordId: 回滚部署记录ID
+        :type DeployRecordId: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.DeployRecordId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.DeployRecordId = params.get("DeployRecordId")
+        self.RequestId = params.get("RequestId")
+
+
+class UpdateRecordDetail(AbstractModel):
+    """更新记录详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Id: 详情记录id
+        :type Id: int
+        :param CertId: 新证书ID
+        :type CertId: str
+        :param OldCertId: 旧证书ID
+        :type OldCertId: str
+        :param Domains: 部署域名列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Domains: list of str
+        :param ResourceType: 部署资源类型
+        :type ResourceType: str
+        :param Region: 部署地域
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Region: str
+        :param Status: 部署状态
+        :type Status: int
+        :param ErrorMsg: 部署错误信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ErrorMsg: str
+        :param CreateTime: 部署时间
+        :type CreateTime: str
+        :param UpdateTime: 最后一次更新时间
+        :type UpdateTime: str
+        :param InstanceId: 部署实例ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceId: str
+        :param InstanceName: 部署实例名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceName: str
+        :param ListenerId: 部署监听器ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ListenerId: str
+        :param ListenerName: 部署监听器名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ListenerName: str
+        :param Protocol: 协议
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Protocol: str
+        :param SniSwitch: 是否开启SNI
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SniSwitch: int
+        :param Bucket: bucket名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Bucket: str
+        """
+        self.Id = None
+        self.CertId = None
+        self.OldCertId = None
+        self.Domains = None
+        self.ResourceType = None
+        self.Region = None
+        self.Status = None
+        self.ErrorMsg = None
+        self.CreateTime = None
+        self.UpdateTime = None
+        self.InstanceId = None
+        self.InstanceName = None
+        self.ListenerId = None
+        self.ListenerName = None
+        self.Protocol = None
+        self.SniSwitch = None
+        self.Bucket = None
+
+
+    def _deserialize(self, params):
+        self.Id = params.get("Id")
+        self.CertId = params.get("CertId")
+        self.OldCertId = params.get("OldCertId")
+        self.Domains = params.get("Domains")
+        self.ResourceType = params.get("ResourceType")
+        self.Region = params.get("Region")
+        self.Status = params.get("Status")
+        self.ErrorMsg = params.get("ErrorMsg")
+        self.CreateTime = params.get("CreateTime")
+        self.UpdateTime = params.get("UpdateTime")
+        self.InstanceId = params.get("InstanceId")
+        self.InstanceName = params.get("InstanceName")
+        self.ListenerId = params.get("ListenerId")
+        self.ListenerName = params.get("ListenerName")
+        self.Protocol = params.get("Protocol")
+        self.SniSwitch = params.get("SniSwitch")
+        self.Bucket = params.get("Bucket")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UpdateRecordDetails(AbstractModel):
+    """更新记录详情列表
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ResourceType: 部署资源类型
+        :type ResourceType: str
+        :param List: 部署资源详情列表
+        :type List: list of UpdateRecordDetail
+        """
+        self.ResourceType = None
+        self.List = None
+
+
+    def _deserialize(self, params):
+        self.ResourceType = params.get("ResourceType")
+        if params.get("List") is not None:
+            self.List = []
+            for item in params.get("List"):
+                obj = UpdateRecordDetail()
+                obj._deserialize(item)
+                self.List.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UpdateRecordInfo(AbstractModel):
+    """部署记录信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Id: 记录ID
+        :type Id: int
+        :param CertId: 新证书ID
+        :type CertId: str
+        :param OldCertId: 原证书ID
+        :type OldCertId: str
+        :param ResourceTypes: 部署资源类型列表
+        :type ResourceTypes: list of str
+        :param Regions: 部署地域列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Regions: list of str
+        :param Status: 部署状态
+        :type Status: int
+        :param CreateTime: 部署时间
+        :type CreateTime: str
+        :param UpdateTime: 最后一次更新时间
+        :type UpdateTime: str
+        """
+        self.Id = None
+        self.CertId = None
+        self.OldCertId = None
+        self.ResourceTypes = None
+        self.Regions = None
+        self.Status = None
+        self.CreateTime = None
+        self.UpdateTime = None
+
+
+    def _deserialize(self, params):
+        self.Id = params.get("Id")
+        self.CertId = params.get("CertId")
+        self.OldCertId = params.get("OldCertId")
+        self.ResourceTypes = params.get("ResourceTypes")
+        self.Regions = params.get("Regions")
+        self.Status = params.get("Status")
+        self.CreateTime = params.get("CreateTime")
+        self.UpdateTime = params.get("UpdateTime")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class UploadCertificateRequest(AbstractModel):
     """UploadCertificate请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -3418,8 +5854,36 @@
         """
         self.ManagerId = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.ManagerId = params.get("ManagerId")
-        self.RequestId = params.get("RequestId")
+        self.RequestId = params.get("RequestId")
+
+
+class VodInstanceDetail(AbstractModel):
+    """Vod实例
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Domain: 域名
+        :type Domain: str
+        :param CertId: 证书ID
+        :type CertId: str
+        """
+        self.Domain = None
+        self.CertId = None
+
+
+    def _deserialize(self, params):
+        self.Domain = params.get("Domain")
+        self.CertId = params.get("CertId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.894/tencentcloud/ssl/v20191205/ssl_client.py` & `tencentcloud-sdk-python-ssl-3.0.895/tencentcloud/ssl/v20191205/ssl_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -206,14 +206,83 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DeployCertificateInstance(self, request):
+        """证书部署到云资源实例列表
+
+        :param request: Request instance for DeployCertificateInstance.
+        :type request: :class:`tencentcloud.ssl.v20191205.models.DeployCertificateInstanceRequest`
+        :rtype: :class:`tencentcloud.ssl.v20191205.models.DeployCertificateInstanceResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeployCertificateInstance", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeployCertificateInstanceResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DeployCertificateRecordRetry(self, request):
+        """云资源部署重试部署记录
+
+        :param request: Request instance for DeployCertificateRecordRetry.
+        :type request: :class:`tencentcloud.ssl.v20191205.models.DeployCertificateRecordRetryRequest`
+        :rtype: :class:`tencentcloud.ssl.v20191205.models.DeployCertificateRecordRetryResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeployCertificateRecordRetry", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeployCertificateRecordRetryResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DeployCertificateRecordRollback(self, request):
+        """云资源部署一键回滚
+
+        :param request: Request instance for DeployCertificateRecordRollback.
+        :type request: :class:`tencentcloud.ssl.v20191205.models.DeployCertificateRecordRollbackRequest`
+        :rtype: :class:`tencentcloud.ssl.v20191205.models.DeployCertificateRecordRollbackResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeployCertificateRecordRollback", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeployCertificateRecordRollbackResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeCertificate(self, request):
         """本接口（DescribeCertificate）用于获取证书信息。
 
         :param request: Request instance for DescribeCertificate.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeCertificateRequest`
         :rtype: :class:`tencentcloud.ssl.v20191205.models.DescribeCertificateResponse`
 
@@ -344,14 +413,359 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeHostApiGatewayInstanceList(self, request):
+        """查询证书apiGateway云资源部署实例列表
+
+        :param request: Request instance for DescribeHostApiGatewayInstanceList.
+        :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostApiGatewayInstanceListRequest`
+        :rtype: :class:`tencentcloud.ssl.v20191205.models.DescribeHostApiGatewayInstanceListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeHostApiGatewayInstanceList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeHostApiGatewayInstanceListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeHostCdnInstanceList(self, request):
+        """查询证书cdn云资源部署实例列表
+
+        :param request: Request instance for DescribeHostCdnInstanceList.
+        :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostCdnInstanceListRequest`
+        :rtype: :class:`tencentcloud.ssl.v20191205.models.DescribeHostCdnInstanceListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeHostCdnInstanceList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeHostCdnInstanceListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeHostClbInstanceList(self, request):
+        """查询证书clb云资源部署实例列表
+
+        :param request: Request instance for DescribeHostClbInstanceList.
+        :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostClbInstanceListRequest`
+        :rtype: :class:`tencentcloud.ssl.v20191205.models.DescribeHostClbInstanceListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeHostClbInstanceList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeHostClbInstanceListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeHostCosInstanceList(self, request):
+        """查询证书cos云资源部署实例列表
+
+        :param request: Request instance for DescribeHostCosInstanceList.
+        :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostCosInstanceListRequest`
+        :rtype: :class:`tencentcloud.ssl.v20191205.models.DescribeHostCosInstanceListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeHostCosInstanceList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeHostCosInstanceListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeHostDdosInstanceList(self, request):
+        """查询证书ddos云资源部署实例列表
+
+        :param request: Request instance for DescribeHostDdosInstanceList.
+        :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostDdosInstanceListRequest`
+        :rtype: :class:`tencentcloud.ssl.v20191205.models.DescribeHostDdosInstanceListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeHostDdosInstanceList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeHostDdosInstanceListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeHostDeployRecord(self, request):
+        """查询证书云资源部署记录列表
+
+        :param request: Request instance for DescribeHostDeployRecord.
+        :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostDeployRecordRequest`
+        :rtype: :class:`tencentcloud.ssl.v20191205.models.DescribeHostDeployRecordResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeHostDeployRecord", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeHostDeployRecordResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeHostDeployRecordDetail(self, request):
+        """查询证书云资源部署记录详情列表
+
+        :param request: Request instance for DescribeHostDeployRecordDetail.
+        :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostDeployRecordDetailRequest`
+        :rtype: :class:`tencentcloud.ssl.v20191205.models.DescribeHostDeployRecordDetailResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeHostDeployRecordDetail", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeHostDeployRecordDetailResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeHostLighthouseInstanceList(self, request):
+        """查询证书Lighthouse云资源部署实例列表
+
+        :param request: Request instance for DescribeHostLighthouseInstanceList.
+        :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostLighthouseInstanceListRequest`
+        :rtype: :class:`tencentcloud.ssl.v20191205.models.DescribeHostLighthouseInstanceListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeHostLighthouseInstanceList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeHostLighthouseInstanceListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeHostLiveInstanceList(self, request):
+        """查询证书live云资源部署实例列表
+
+        :param request: Request instance for DescribeHostLiveInstanceList.
+        :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostLiveInstanceListRequest`
+        :rtype: :class:`tencentcloud.ssl.v20191205.models.DescribeHostLiveInstanceListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeHostLiveInstanceList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeHostLiveInstanceListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeHostTeoInstanceList(self, request):
+        """查询证书EdgeOne云资源部署实例列表
+
+        :param request: Request instance for DescribeHostTeoInstanceList.
+        :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostTeoInstanceListRequest`
+        :rtype: :class:`tencentcloud.ssl.v20191205.models.DescribeHostTeoInstanceListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeHostTeoInstanceList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeHostTeoInstanceListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeHostTkeInstanceList(self, request):
+        """查询证书tke云资源部署实例列表
+
+        :param request: Request instance for DescribeHostTkeInstanceList.
+        :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostTkeInstanceListRequest`
+        :rtype: :class:`tencentcloud.ssl.v20191205.models.DescribeHostTkeInstanceListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeHostTkeInstanceList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeHostTkeInstanceListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeHostUpdateRecord(self, request):
+        """查询证书云资源更新记录列表
+
+        :param request: Request instance for DescribeHostUpdateRecord.
+        :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostUpdateRecordRequest`
+        :rtype: :class:`tencentcloud.ssl.v20191205.models.DescribeHostUpdateRecordResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeHostUpdateRecord", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeHostUpdateRecordResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeHostUpdateRecordDetail(self, request):
+        """查询证书云资源更新记录详情列表
+
+        :param request: Request instance for DescribeHostUpdateRecordDetail.
+        :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostUpdateRecordDetailRequest`
+        :rtype: :class:`tencentcloud.ssl.v20191205.models.DescribeHostUpdateRecordDetailResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeHostUpdateRecordDetail", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeHostUpdateRecordDetailResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeHostVodInstanceList(self, request):
+        """查询证书Vod云资源部署实例列表
+
+        :param request: Request instance for DescribeHostVodInstanceList.
+        :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostVodInstanceListRequest`
+        :rtype: :class:`tencentcloud.ssl.v20191205.models.DescribeHostVodInstanceListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeHostVodInstanceList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeHostVodInstanceListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeHostWafInstanceList(self, request):
+        """查询证书waf云资源部署实例列表
+
+        :param request: Request instance for DescribeHostWafInstanceList.
+        :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostWafInstanceListRequest`
+        :rtype: :class:`tencentcloud.ssl.v20191205.models.DescribeHostWafInstanceListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeHostWafInstanceList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeHostWafInstanceListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeManagerDetail(self, request):
         """查询管理人详情
 
         :param request: Request instance for DescribeManagerDetail.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeManagerDetailRequest`
         :rtype: :class:`tencentcloud.ssl.v20191205.models.DescribeManagerDetailResponse`
 
@@ -618,14 +1032,83 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def UpdateCertificateInstance(self, request):
+        """一键更新旧证书资源
+
+        :param request: Request instance for UpdateCertificateInstance.
+        :type request: :class:`tencentcloud.ssl.v20191205.models.UpdateCertificateInstanceRequest`
+        :rtype: :class:`tencentcloud.ssl.v20191205.models.UpdateCertificateInstanceResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("UpdateCertificateInstance", params, headers=headers)
+            response = json.loads(body)
+            model = models.UpdateCertificateInstanceResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def UpdateCertificateRecordRetry(self, request):
+        """云资源更新重试部署记录
+
+        :param request: Request instance for UpdateCertificateRecordRetry.
+        :type request: :class:`tencentcloud.ssl.v20191205.models.UpdateCertificateRecordRetryRequest`
+        :rtype: :class:`tencentcloud.ssl.v20191205.models.UpdateCertificateRecordRetryResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("UpdateCertificateRecordRetry", params, headers=headers)
+            response = json.loads(body)
+            model = models.UpdateCertificateRecordRetryResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def UpdateCertificateRecordRollback(self, request):
+        """云资源更新一键回滚
+
+        :param request: Request instance for UpdateCertificateRecordRollback.
+        :type request: :class:`tencentcloud.ssl.v20191205.models.UpdateCertificateRecordRollbackRequest`
+        :rtype: :class:`tencentcloud.ssl.v20191205.models.UpdateCertificateRecordRollbackResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("UpdateCertificateRecordRollback", params, headers=headers)
+            response = json.loads(body)
+            model = models.UpdateCertificateRecordRollbackResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def UploadCertificate(self, request):
         """本接口（UploadCertificate）用于上传证书。
 
         :param request: Request instance for UploadCertificate.
         :type request: :class:`tencentcloud.ssl.v20191205.models.UploadCertificateRequest`
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.894/PKG-INFO` & `tencentcloud-sdk-python-ssl-3.0.895/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssl
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Ssl SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.894/setup.py` & `tencentcloud-sdk-python-ssl-3.0.895/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.894/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ssl-3.0.895/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssl
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Ssl SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

