# Comparing `tmp/tencentcloud-sdk-python-antiddos-3.0.894.tar.gz` & `tmp/tencentcloud-sdk-python-antiddos-3.0.895.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-antiddos-3.0.894.tar", last modified: Thu May 18 00:15:17 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-antiddos-3.0.895.tar", last modified: Fri May 19 02:40:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-antiddos-3.0.894.tar` & `tencentcloud-sdk-python-antiddos-3.0.895.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:15:17.000000 tencentcloud-sdk-python-antiddos-3.0.894/
--rw-r--r--   0 root         (0) root         (0)      752 2023-05-18 00:15:17.000000 tencentcloud-sdk-python-antiddos-3.0.894/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:15:17.000000 tencentcloud-sdk-python-antiddos-3.0.894/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:15:17.000000 tencentcloud-sdk-python-antiddos-3.0.894/tencentcloud/antiddos/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:15:17.000000 tencentcloud-sdk-python-antiddos-3.0.894/tencentcloud/antiddos/v20200309/
--rw-r--r--   0 root         (0) root         (0)    88167 2023-05-18 00:15:17.000000 tencentcloud-sdk-python-antiddos-3.0.894/tencentcloud/antiddos/v20200309/antiddos_client.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-05-18 00:15:17.000000 tencentcloud-sdk-python-antiddos-3.0.894/tencentcloud/antiddos/v20200309/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:15:17.000000 tencentcloud-sdk-python-antiddos-3.0.894/tencentcloud/antiddos/v20200309/__init__.py
--rw-r--r--   0 root         (0) root         (0)   315554 2023-05-18 00:15:17.000000 tencentcloud-sdk-python-antiddos-3.0.894/tencentcloud/antiddos/v20200309/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:15:17.000000 tencentcloud-sdk-python-antiddos-3.0.894/tencentcloud/antiddos/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:15:17.000000 tencentcloud-sdk-python-antiddos-3.0.894/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:15:17.000000 tencentcloud-sdk-python-antiddos-3.0.894/tencentcloud_sdk_python_antiddos.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:15:17.000000 tencentcloud-sdk-python-antiddos-3.0.894/tencentcloud_sdk_python_antiddos.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-05-18 00:15:17.000000 tencentcloud-sdk-python-antiddos-3.0.894/tencentcloud_sdk_python_antiddos.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-18 00:15:17.000000 tencentcloud-sdk-python-antiddos-3.0.894/tencentcloud_sdk_python_antiddos.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:15:17.000000 tencentcloud-sdk-python-antiddos-3.0.894/tencentcloud_sdk_python_antiddos.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-18 00:15:17.000000 tencentcloud-sdk-python-antiddos-3.0.894/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-05-18 00:15:17.000000 tencentcloud-sdk-python-antiddos-3.0.894/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:15:17.000000 tencentcloud-sdk-python-antiddos-3.0.894/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:40:55.000000 tencentcloud-sdk-python-antiddos-3.0.895/
+-rw-r--r--   0 root         (0) root         (0)      752 2023-05-19 02:40:55.000000 tencentcloud-sdk-python-antiddos-3.0.895/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:40:55.000000 tencentcloud-sdk-python-antiddos-3.0.895/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:40:55.000000 tencentcloud-sdk-python-antiddos-3.0.895/tencentcloud/antiddos/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:40:55.000000 tencentcloud-sdk-python-antiddos-3.0.895/tencentcloud/antiddos/v20200309/
+-rw-r--r--   0 root         (0) root         (0)    88167 2023-05-19 02:40:55.000000 tencentcloud-sdk-python-antiddos-3.0.895/tencentcloud/antiddos/v20200309/antiddos_client.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-05-19 02:40:55.000000 tencentcloud-sdk-python-antiddos-3.0.895/tencentcloud/antiddos/v20200309/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:40:55.000000 tencentcloud-sdk-python-antiddos-3.0.895/tencentcloud/antiddos/v20200309/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   316926 2023-05-19 02:40:55.000000 tencentcloud-sdk-python-antiddos-3.0.895/tencentcloud/antiddos/v20200309/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:40:55.000000 tencentcloud-sdk-python-antiddos-3.0.895/tencentcloud/antiddos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-19 02:40:55.000000 tencentcloud-sdk-python-antiddos-3.0.895/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:40:55.000000 tencentcloud-sdk-python-antiddos-3.0.895/tencentcloud_sdk_python_antiddos.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 02:40:55.000000 tencentcloud-sdk-python-antiddos-3.0.895/tencentcloud_sdk_python_antiddos.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-05-19 02:40:55.000000 tencentcloud-sdk-python-antiddos-3.0.895/tencentcloud_sdk_python_antiddos.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-19 02:40:55.000000 tencentcloud-sdk-python-antiddos-3.0.895/tencentcloud_sdk_python_antiddos.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 02:40:55.000000 tencentcloud-sdk-python-antiddos-3.0.895/tencentcloud_sdk_python_antiddos.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-19 02:40:55.000000 tencentcloud-sdk-python-antiddos-3.0.895/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-05-19 02:40:55.000000 tencentcloud-sdk-python-antiddos-3.0.895/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-19 02:40:55.000000 tencentcloud-sdk-python-antiddos-3.0.895/setup.cfg
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.894/README.rst` & `tencentcloud-sdk-python-antiddos-3.0.895/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-antiddos-3.0.894/tencentcloud/antiddos/v20200309/antiddos_client.py` & `tencentcloud-sdk-python-antiddos-3.0.895/tencentcloud/antiddos/v20200309/antiddos_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-antiddos-3.0.894/tencentcloud/antiddos/v20200309/errorcodes.py` & `tencentcloud-sdk-python-antiddos-3.0.895/tencentcloud/antiddos/v20200309/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-antiddos-3.0.894/tencentcloud/antiddos/v20200309/models.py` & `tencentcloud-sdk-python-antiddos-3.0.895/tencentcloud/antiddos/v20200309/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -814,28 +814,33 @@
         :type BizType: str
         :param InstanceId: IP所属的资源实例ID，绑定操作为必填项，解绑操作可不填。例如是弹性网卡的IP，则InstanceId填写弹性网卡的ID(eni-*); 如果绑定的是托管IP没有对应的资源实例ID，请填写"none";
         :type InstanceId: str
         :param DeviceType: 产品分类下的子类型，绑定操作为必填项，解绑操作可不填。取值[cvm（CVM），lb（负载均衡器），eni（弹性网卡），vpngw（VPN），natgw（NAT），waf（WAF），fpc（金融），gaap（GAAP），other（托管IP），eip（弹性公网常规IP）]
         :type DeviceType: str
         :param IspCode: 运营商，绑定操作为必填项，解绑操作可不填。0：电信；1：联通；2：移动；5：BGP
         :type IspCode: int
+        :param Domain: 域名化资产对应的域名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Domain: str
         """
         self.Ip = None
         self.BizType = None
         self.InstanceId = None
         self.DeviceType = None
         self.IspCode = None
+        self.Domain = None
 
 
     def _deserialize(self, params):
         self.Ip = params.get("Ip")
         self.BizType = params.get("BizType")
         self.InstanceId = params.get("InstanceId")
         self.DeviceType = params.get("DeviceType")
         self.IspCode = params.get("IspCode")
+        self.Domain = params.get("Domain")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1489,20 +1494,23 @@
         :type Id: str
         :param BoundDevList: 绑定到资源实例的IP数组，当资源实例为高防包(独享包)时，数组只允许填1个IP；当没有要绑定的IP时可以为空数组；但是BoundDevList和UnBoundDevList至少有一个不为空；
         :type BoundDevList: list of BoundIpInfo
         :param UnBoundDevList: 与资源实例解绑的IP数组，当资源实例为高防包(独享包)时，数组只允许填1个IP；当没有要解绑的IP时可以为空数组；但是BoundDevList和UnBoundDevList至少有一个不为空；
         :type UnBoundDevList: list of BoundIpInfo
         :param CopyPolicy: 已弃用，不填
         :type CopyPolicy: str
+        :param FilterRegion: 如果该资源实例为域名化资产则，该参数必填
+        :type FilterRegion: str
         """
         self.Business = None
         self.Id = None
         self.BoundDevList = None
         self.UnBoundDevList = None
         self.CopyPolicy = None
+        self.FilterRegion = None
 
 
     def _deserialize(self, params):
         self.Business = params.get("Business")
         self.Id = params.get("Id")
         if params.get("BoundDevList") is not None:
             self.BoundDevList = []
@@ -1513,14 +1521,15 @@
         if params.get("UnBoundDevList") is not None:
             self.UnBoundDevList = []
             for item in params.get("UnBoundDevList"):
                 obj = BoundIpInfo()
                 obj._deserialize(item)
                 self.UnBoundDevList.append(obj)
         self.CopyPolicy = params.get("CopyPolicy")
+        self.FilterRegion = params.get("FilterRegion")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3450,20 +3459,28 @@
 
     """
 
     def __init__(self):
         r"""
         :param IpList: IP 资源列表
         :type IpList: list of str
+        :param IdList: 域名化资源传id
+        :type IdList: list of str
+        :param FilterRegion: 地域名称
+        :type FilterRegion: int
         """
         self.IpList = None
+        self.IdList = None
+        self.FilterRegion = None
 
 
     def _deserialize(self, params):
         self.IpList = params.get("IpList")
+        self.IdList = params.get("IdList")
+        self.FilterRegion = params.get("FilterRegion")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3477,28 +3494,38 @@
     def __init__(self):
         r"""
         :param Data: 返回资源及状态，状态码：
 1 - 封堵状态
 2 - 正常状态
 3 - 攻击状态
         :type Data: list of KeyValue
+        :param CLBData: 域名化资产的名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CLBData: list of KeyValue
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Data = None
+        self.CLBData = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         if params.get("Data") is not None:
             self.Data = []
             for item in params.get("Data"):
                 obj = KeyValue()
                 obj._deserialize(item)
                 self.Data.append(obj)
+        if params.get("CLBData") is not None:
+            self.CLBData = []
+            for item in params.get("CLBData"):
+                obj = KeyValue()
+                obj._deserialize(item)
+                self.CLBData.append(obj)
         self.RequestId = params.get("RequestId")
 
 
 class DescribeBgpBizTrendRequest(AbstractModel):
     """DescribeBgpBizTrend请求参数结构体
 
     """
@@ -5866,34 +5893,38 @@
         :type Limit: int
         :param Offset: 页起始偏移，取值为(页码-1)*一页条数
         :type Offset: int
         :param ProtocolList: 转发协议搜索，选填，取值[http, https, http/https]
         :type ProtocolList: list of str
         :param Cname: 高防IP实例的Cname
         :type Cname: str
+        :param Export: 默认为false，当为true时，将不对各个规则做策略检查，直接导出所有规则
+        :type Export: bool
         """
         self.Business = None
         self.StatusList = None
         self.Domain = None
         self.Ip = None
         self.Limit = None
         self.Offset = None
         self.ProtocolList = None
         self.Cname = None
+        self.Export = None
 
 
     def _deserialize(self, params):
         self.Business = params.get("Business")
         self.StatusList = params.get("StatusList")
         self.Domain = params.get("Domain")
         self.Ip = params.get("Ip")
         self.Limit = params.get("Limit")
         self.Offset = params.get("Offset")
         self.ProtocolList = params.get("ProtocolList")
         self.Cname = params.get("Cname")
+        self.Export = params.get("Export")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.894/tencentcloud/__init__.py` & `tencentcloud-sdk-python-antiddos-3.0.895/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-antiddos-3.0.894/tencentcloud_sdk_python_antiddos.egg-info/PKG-INFO` & `tencentcloud-sdk-python-antiddos-3.0.895/tencentcloud_sdk_python_antiddos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-antiddos
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Antiddos SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.894/PKG-INFO` & `tencentcloud-sdk-python-antiddos-3.0.895/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-antiddos
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Antiddos SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.894/setup.py` & `tencentcloud-sdk-python-antiddos-3.0.895/setup.py`

 * *Files identical despite different names*

