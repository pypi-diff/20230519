# Comparing `tmp/tencentcloud-sdk-python-cdn-3.0.894.tar.gz` & `tmp/tencentcloud-sdk-python-cdn-3.0.895.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.894.tar", last modified: Thu May 18 00:19:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.895.tar", last modified: Fri May 19 02:45:10 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdn-3.0.894.tar` & `tencentcloud-sdk-python-cdn-3.0.895.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/cdn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/cdn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/cdn/v20180606/
--rw-r--r--   0 root         (0) root         (0)    21972 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/cdn/v20180606/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    80657 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/cdn/v20180606/cdn_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/cdn/v20180606/__init__.py
--rw-r--r--   0 root         (0) root         (0)   570836 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/cdn/v20180606/models.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud_sdk_python_cdn.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:19:45.000000 tencentcloud-sdk-python-cdn-3.0.894/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:45:10.000000 tencentcloud-sdk-python-cdn-3.0.895/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-19 02:45:10.000000 tencentcloud-sdk-python-cdn-3.0.895/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:45:10.000000 tencentcloud-sdk-python-cdn-3.0.895/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-19 02:45:10.000000 tencentcloud-sdk-python-cdn-3.0.895/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:45:10.000000 tencentcloud-sdk-python-cdn-3.0.895/tencentcloud/cdn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:45:10.000000 tencentcloud-sdk-python-cdn-3.0.895/tencentcloud/cdn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:45:10.000000 tencentcloud-sdk-python-cdn-3.0.895/tencentcloud/cdn/v20180606/
+-rw-r--r--   0 root         (0) root         (0)    21972 2023-05-19 02:45:10.000000 tencentcloud-sdk-python-cdn-3.0.895/tencentcloud/cdn/v20180606/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    80657 2023-05-19 02:45:10.000000 tencentcloud-sdk-python-cdn-3.0.895/tencentcloud/cdn/v20180606/cdn_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:45:10.000000 tencentcloud-sdk-python-cdn-3.0.895/tencentcloud/cdn/v20180606/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   571918 2023-05-19 02:45:10.000000 tencentcloud-sdk-python-cdn-3.0.895/tencentcloud/cdn/v20180606/models.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 02:45:10.000000 tencentcloud-sdk-python-cdn-3.0.895/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:45:10.000000 tencentcloud-sdk-python-cdn-3.0.895/tencentcloud_sdk_python_cdn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 02:45:10.000000 tencentcloud-sdk-python-cdn-3.0.895/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-19 02:45:10.000000 tencentcloud-sdk-python-cdn-3.0.895/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 02:45:10.000000 tencentcloud-sdk-python-cdn-3.0.895/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 02:45:10.000000 tencentcloud-sdk-python-cdn-3.0.895/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-19 02:45:10.000000 tencentcloud-sdk-python-cdn-3.0.895/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-19 02:45:10.000000 tencentcloud-sdk-python-cdn-3.0.895/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.894/README.rst` & `tencentcloud-sdk-python-cdn-3.0.895/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdn-3.0.895/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/cdn/v20180606/errorcodes.py` & `tencentcloud-sdk-python-cdn-3.0.895/tencentcloud/cdn/v20180606/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/cdn/v20180606/cdn_client.py` & `tencentcloud-sdk-python-cdn-3.0.895/tencentcloud/cdn/v20180606/cdn_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.894/tencentcloud/cdn/v20180606/models.py` & `tencentcloud-sdk-python-cdn-3.0.895/tencentcloud/cdn/v20180606/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 class AccessControl(AbstractModel):
     """请求头部及请求url访问控制
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: on | off 是否启用请求头部及请求url访问控制
+        :param Switch: 启用请求头部及请求url访问控制开关，取值有：
+on：开启
+off：关闭
         :type Switch: str
         :param AccessControlRules: 请求头部及请求url访问规则
 注意：此字段可能返回 null，表示取不到有效值。
         :type AccessControlRules: list of AccessControlRule
         :param ReturnCode: 返回状态码
 注意：此字段可能返回 null，表示取不到有效值。
         :type ReturnCode: int
@@ -577,15 +579,18 @@
 class AdvancedAuthentication(AbstractModel):
     """时间戳防盗链高级版配置，白名单功能
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 防盗链配置开关，on或off，开启时必须且只能配置一种模式，其余模式为null。
+        :param Switch: 防盗链配置开关，取值有：
+on：开启
+off：关闭
+开启时必须且只配置一种模式，其余模式需要设置为 null
         :type Switch: str
         :param TypeA: 时间戳防盗链高级版模式A配置。
 注意：此字段可能返回 null，表示取不到有效值。
         :type TypeA: :class:`tencentcloud.cdn.v20180606.models.AdvancedAuthenticationTypeA`
         :param TypeB: 时间戳防盗链高级版模式B配置。
 注意：此字段可能返回 null，表示取不到有效值。
         :type TypeB: :class:`tencentcloud.cdn.v20180606.models.AdvancedAuthenticationTypeB`
@@ -1376,15 +1381,15 @@
 class Authentication(AbstractModel):
     """时间戳防盗链配置
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 防盗链配置开关
+        :param Switch: 防盗链配置开关，取值有：
 on：开启
 off：关闭
 开启时必须且只配置一种模式，其余模式需要设置为 null
         :type Switch: str
         :param TypeA: 时间戳防盗链模式 A 配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type TypeA: :class:`tencentcloud.cdn.v20180606.models.AuthenticationTypeA`
@@ -1658,15 +1663,17 @@
 class AvifAdapter(AbstractModel):
     """图片优化-AvifAdapter配置
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 开关，"on/off"
+        :param Switch: 图片优化AvifAdapter配置项开关，取值有：
+on：开启
+off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         """
         self.Switch = None
 
 
     def _deserialize(self, params):
@@ -1683,15 +1690,17 @@
 class AwsPrivateAccess(AbstractModel):
     """s3源站回源鉴权。
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 开关，on/off。
+        :param Switch: s3源站回源鉴权配置项开关，取值有：
+on：开启
+off：关闭
         :type Switch: str
         :param AccessKey: 访问ID。
 注意：此字段可能返回 null，表示取不到有效值。
         :type AccessKey: str
         :param SecretKey: 密钥。
 注意：此字段可能返回 null，表示取不到有效值。
         :type SecretKey: str
@@ -1727,29 +1736,29 @@
 class BandwidthAlert(AbstractModel):
     """带宽封顶配置，默认为关闭状态
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 用量封顶配置开关
+        :param Switch: 用量封顶配置开关，取值有：
 on：开启
 off：关闭
         :type Switch: str
         :param BpsThreshold: 用量封顶阈值，带宽单位为bps，流量单位byte
 注意：此字段可能返回 null，表示取不到有效值。
         :type BpsThreshold: int
         :param CounterMeasure: 达到阈值后的操作
 RETURN_404：全部请求返回 404
 注意：此字段可能返回 null，表示取不到有效值。
         :type CounterMeasure: str
         :param LastTriggerTime: 境内区域上次触发用量封顶阈值的时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type LastTriggerTime: str
-        :param AlertSwitch: 用量封顶提醒开关
+        :param AlertSwitch: 用量封顶提醒配置开关，取值有：
 on：开启
 off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type AlertSwitch: str
         :param AlertPercentage: 用量封顶阈值提醒百分比
 注意：此字段可能返回 null，表示取不到有效值。
         :type AlertPercentage: int
@@ -2275,16 +2284,17 @@
 class CacheConfig(AbstractModel):
     """启发式自定义时间缓存配置
 
     """
 
     def __init__(self):
         r"""
-        :param HeuristicCacheTimeSwitch: on 代表开启自定义启发式缓存时间
-off 代表关闭自定义启发式缓存时间
+        :param HeuristicCacheTimeSwitch: 启发式自定义时间缓存配置开关，取值有：
+on：开启
+off：关闭
         :type HeuristicCacheTimeSwitch: str
         :param HeuristicCacheTime: 单位 秒.
         :type HeuristicCacheTime: int
         """
         self.HeuristicCacheTimeSwitch = None
         self.HeuristicCacheTime = None
 
@@ -2304,15 +2314,15 @@
 class CacheConfigCache(AbstractModel):
     """路径缓存缓存配置
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 缓存配置开关
+        :param Switch: 路径缓存配置开关，取值有：
 on：开启
 off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         :param CacheTime: 缓存过期时间设置
 单位为秒，最大可设置为 365 天
 注意：此字段可能返回 null，表示取不到有效值。
@@ -2361,15 +2371,15 @@
 class CacheConfigFollowOrigin(AbstractModel):
     """路径缓存遵循源站配置
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 遵循源站配置开关
+        :param Switch: 路径缓存遵循源站配置开关，取值有：
 on：开启
 off：关闭
         :type Switch: str
         :param HeuristicCache: 启发式缓存配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type HeuristicCache: :class:`tencentcloud.cdn.v20180606.models.HeuristicCache`
         """
@@ -2394,15 +2404,15 @@
 class CacheConfigNoCache(AbstractModel):
     """路径缓存不缓存配置
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 不缓存配置开关
+        :param Switch: 路径缓存不缓存配置配置开关，取值有：
 on：开启
 off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         :param Revalidate: 总是回源站校验
 on：开启
 off：关闭
@@ -2535,15 +2545,17 @@
 class CacheTagKey(AbstractModel):
     """组成CacheKey的一部分
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 是否使用CacheTag作为CacheKey的一部分
+        :param Switch: 使用CacheTag作为CacheKey的一部分配置开关，取值有
+on：开启，使用CacheTag作为CacheKey的一部分
+off：关闭，不使用CacheTag作为CacheKey的一部分
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         :param Value: 自定义CacheTag的值
 注意：此字段可能返回 null，表示取不到有效值。
         :type Value: str
         """
         self.Switch = None
@@ -3012,15 +3024,15 @@
 class Compression(AbstractModel):
     """智能压缩配置，默认对 js、html、css、xml、json、shtml、htm 后缀且大小为 256 ~ 2097152 字节的文件进行 GZIP 压缩
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 智能压缩配置开关
+        :param Switch: 智能压缩配置开关，取值有：
 on：开启
 off：关闭
         :type Switch: str
         :param CompressionRules: 压缩规则数组
 注意：此字段可能返回 null，表示取不到有效值。
         :type CompressionRules: list of CompressionRule
         """
@@ -3118,15 +3130,17 @@
 class CookieKey(AbstractModel):
     """组成CacheKey的一部分
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: on | off 是否使用Cookie作为Cache的一部分
+        :param Switch: 使用Cookie作为Cache的一部分配置开关，取值有：
+on：开启，使用Cookie作为Cache的一部分
+off：关闭，不使用Cookie作为Cache的一部分
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         :param Value: 使用的cookie，';' 分割
 注意：此字段可能返回 null，表示取不到有效值。
         :type Value: str
         """
         self.Switch = None
@@ -7901,15 +7915,15 @@
 class DownstreamCapping(AbstractModel):
     """单链接下行限速配置，默认为关闭状态
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 下行速度配置开关
+        :param Switch: 下行速度配置开关，取值有：
 on：开启
 off：关闭
         :type Switch: str
         :param CappingRules: 下行限速规则
 注意：此字段可能返回 null，表示取不到有效值。
         :type CappingRules: list of CappingRule
         """
@@ -8171,15 +8185,15 @@
 class ErrorPage(AbstractModel):
     """状态码重定向配置，默认为关闭状态
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 状态码重定向配置开关
+        :param Switch: 状态码重定向配置开关，取值有：
 on：开启
 off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         :param PageRules: 状态码重定向规则配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type PageRules: list of ErrorPageRule
@@ -8308,15 +8322,15 @@
 class FollowRedirect(AbstractModel):
     """回源 301/302 状态码自动跟随配置，默认为关闭状态
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 回源跟随开关
+        :param Switch: 回源跟随配置开关，取值有：
 on：开启
 off：关闭
         :type Switch: str
         :param RedirectConfig: 自定义回源302 follow请求host配置，该功能为白名单功能，需要开启请联系腾讯云工程师。
 注意：此字段可能返回 null，表示取不到有效值。
         :type RedirectConfig: :class:`tencentcloud.cdn.v20180606.models.RedirectConfig`
         """
@@ -8341,15 +8355,15 @@
 class ForceRedirect(AbstractModel):
     """访问协议强制跳转配置，默认为关闭状态
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 访问强制跳转配置开关
+        :param Switch: 访问强制跳转配置开关，取值有：
 on：开启
 off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         :param RedirectType: 访问强制跳转类型
 http：强制 http 跳转
 https：强制 https 跳转
@@ -8468,15 +8482,17 @@
 class GuetzliAdapter(AbstractModel):
     """图片优化-GuetzliAdapter配置
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 开关，"on/off"
+        :param Switch: 图片优化-GuetzliAdapter配置开关，取值有：
+on：开启
+off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         """
         self.Switch = None
 
 
     def _deserialize(self, params):
@@ -8521,15 +8537,17 @@
 class HeaderKey(AbstractModel):
     """组成CacheKey
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 是否组成Cachekey
+        :param Switch: 组成Cachekey配置开关，取值有：
+on：开启
+off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         :param Value: 组成CacheKey的header数组，';' 分割
 注意：此字段可能返回 null，表示取不到有效值。
         :type Value: str
         """
         self.Switch = None
@@ -8551,16 +8569,17 @@
 class HeuristicCache(AbstractModel):
     """启发式缓存配置
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: on 代表开启启发式缓存
-off 代表关闭启发式缓存
+        :param Switch: 启发式缓存配置开关，取值有：
+on：开启
+off：关闭
         :type Switch: str
         :param CacheConfig: 自定义启发式缓存时间配置
         :type CacheConfig: :class:`tencentcloud.cdn.v20180606.models.CacheConfig`
         """
         self.Switch = None
         self.CacheConfig = None
 
@@ -8582,15 +8601,17 @@
 class Hsts(AbstractModel):
     """HSTS 配置。
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 是否开启，on或off。
+        :param Switch: HSTS 配置开关，取值有：
+on：开启
+off：关闭
         :type Switch: str
         :param MaxAge: MaxAge数值。
 注意：此字段可能返回 null，表示取不到有效值。
         :type MaxAge: int
         :param IncludeSubDomains: 是否包含子域名，on或off。
 注意：此字段可能返回 null，表示取不到有效值。
         :type IncludeSubDomains: str
@@ -8706,15 +8727,15 @@
 class Https(AbstractModel):
     """域名 https 加速配置，默认为关闭状态
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: https 配置开关
+        :param Switch: https 配置开关，取值有：
 on：开启
 off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         :param Http2: http2 配置开关
 on：开启
 off：关闭
@@ -8799,15 +8820,18 @@
 class HttpsBilling(AbstractModel):
     """HTTPS服务，若关闭，下发配置拦截https请求，开启时会产生计费
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: HTTPS服务，缺省时默认开启【会产生计费】
+        :param Switch: HTTPS服务配置开关，取值有：
+on：开启，缺省时默认开启【会产生计费】
+off：关闭，拦截https请求
+
         :type Switch: str
         """
         self.Switch = None
 
 
     def _deserialize(self, params):
         self.Switch = params.get("Switch")
@@ -8928,15 +8952,17 @@
 class HwPrivateAccess(AbstractModel):
     """华为云对象存储回源鉴权
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 开关 on/off
+        :param Switch:  华为云对象存储回源鉴权配置开关，取值有：
+on：开启
+off：关闭
         :type Switch: str
         :param AccessKey: 访问 ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type AccessKey: str
         :param SecretKey: 密钥
 注意：此字段可能返回 null，表示取不到有效值。
         :type SecretKey: str
@@ -9015,15 +9041,15 @@
 class IpFilter(AbstractModel):
     """IP 黑白名单配置，默认为关闭状态
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: IP 黑白名单配置开关
+        :param Switch: IP 黑白名单配置开关，取值有
 on：开启
 off：关闭
         :type Switch: str
         :param FilterType: IP 黑白名单类型
 whitelist：白名单
 blacklist：黑名单
 注意：此字段可能返回 null，表示取不到有效值。
@@ -12696,15 +12722,18 @@
 class Revalidate(AbstractModel):
     """是否回源站校验
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: on | off 是否总是回源校验
+        :param Switch: 总是回源校验配置开关，取值有：
+on：开启
+off：关闭
+
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         :param Path: 只在特定请求路径回源站校验
 注意：此字段可能返回 null，表示取不到有效值。
         :type Path: str
         """
         self.Switch = None
@@ -12847,15 +12876,18 @@
 class RuleQueryString(AbstractModel):
     """路径保留参数配置
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: on | off CacheKey是否由QueryString组成
+        :param Switch: 路径保留参数配置开关，取值有：
+on：开启，CacheKey由QueryString组成
+off：关闭，CacheKey不由QueryString组成
+
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         :param Action: includeCustom 包含部分url参数
 注意：此字段可能返回 null，表示取不到有效值。
         :type Action: str
         :param Value: 使用/排除的url参数数组，';' 分割
 注意：此字段可能返回 null，表示取不到有效值。
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.894/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.895/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.894/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.895/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.894/setup.py` & `tencentcloud-sdk-python-cdn-3.0.895/setup.py`

 * *Files identical despite different names*

