# Comparing `tmp/tencentcloud-sdk-python-cfw-3.0.894.tar.gz` & `tmp/tencentcloud-sdk-python-cfw-3.0.895.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cfw-3.0.894.tar", last modified: Thu May 18 00:20:19 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cfw-3.0.895.tar", last modified: Fri May 19 02:45:50 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cfw-3.0.894.tar` & `tencentcloud-sdk-python-cfw-3.0.895.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:20:19.000000 tencentcloud-sdk-python-cfw-3.0.894/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-18 00:20:19.000000 tencentcloud-sdk-python-cfw-3.0.894/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:20:19.000000 tencentcloud-sdk-python-cfw-3.0.894/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:20:19.000000 tencentcloud-sdk-python-cfw-3.0.894/tencentcloud/cfw/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:20:19.000000 tencentcloud-sdk-python-cfw-3.0.894/tencentcloud/cfw/v20190904/
--rw-r--r--   0 root         (0) root         (0)     1836 2023-05-18 00:20:19.000000 tencentcloud-sdk-python-cfw-3.0.894/tencentcloud/cfw/v20190904/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    65635 2023-05-18 00:20:19.000000 tencentcloud-sdk-python-cfw-3.0.894/tencentcloud/cfw/v20190904/cfw_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:20:19.000000 tencentcloud-sdk-python-cfw-3.0.894/tencentcloud/cfw/v20190904/__init__.py
--rw-r--r--   0 root         (0) root         (0)   219501 2023-05-18 00:20:19.000000 tencentcloud-sdk-python-cfw-3.0.894/tencentcloud/cfw/v20190904/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:20:19.000000 tencentcloud-sdk-python-cfw-3.0.894/tencentcloud/cfw/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:20:19.000000 tencentcloud-sdk-python-cfw-3.0.894/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:20:19.000000 tencentcloud-sdk-python-cfw-3.0.894/tencentcloud_sdk_python_cfw.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:20:19.000000 tencentcloud-sdk-python-cfw-3.0.894/tencentcloud_sdk_python_cfw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-18 00:20:19.000000 tencentcloud-sdk-python-cfw-3.0.894/tencentcloud_sdk_python_cfw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:20:19.000000 tencentcloud-sdk-python-cfw-3.0.894/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:20:19.000000 tencentcloud-sdk-python-cfw-3.0.894/tencentcloud_sdk_python_cfw.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:20:19.000000 tencentcloud-sdk-python-cfw-3.0.894/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-18 00:20:19.000000 tencentcloud-sdk-python-cfw-3.0.894/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:20:19.000000 tencentcloud-sdk-python-cfw-3.0.894/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:45:50.000000 tencentcloud-sdk-python-cfw-3.0.895/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-19 02:45:50.000000 tencentcloud-sdk-python-cfw-3.0.895/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:45:50.000000 tencentcloud-sdk-python-cfw-3.0.895/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:45:50.000000 tencentcloud-sdk-python-cfw-3.0.895/tencentcloud/cfw/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:45:50.000000 tencentcloud-sdk-python-cfw-3.0.895/tencentcloud/cfw/v20190904/
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-05-19 02:45:50.000000 tencentcloud-sdk-python-cfw-3.0.895/tencentcloud/cfw/v20190904/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    66476 2023-05-19 02:45:50.000000 tencentcloud-sdk-python-cfw-3.0.895/tencentcloud/cfw/v20190904/cfw_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:45:50.000000 tencentcloud-sdk-python-cfw-3.0.895/tencentcloud/cfw/v20190904/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223027 2023-05-19 02:45:50.000000 tencentcloud-sdk-python-cfw-3.0.895/tencentcloud/cfw/v20190904/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:45:50.000000 tencentcloud-sdk-python-cfw-3.0.895/tencentcloud/cfw/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-19 02:45:50.000000 tencentcloud-sdk-python-cfw-3.0.895/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:45:50.000000 tencentcloud-sdk-python-cfw-3.0.895/tencentcloud_sdk_python_cfw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 02:45:50.000000 tencentcloud-sdk-python-cfw-3.0.895/tencentcloud_sdk_python_cfw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-19 02:45:50.000000 tencentcloud-sdk-python-cfw-3.0.895/tencentcloud_sdk_python_cfw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 02:45:50.000000 tencentcloud-sdk-python-cfw-3.0.895/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 02:45:50.000000 tencentcloud-sdk-python-cfw-3.0.895/tencentcloud_sdk_python_cfw.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 02:45:50.000000 tencentcloud-sdk-python-cfw-3.0.895/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-19 02:45:50.000000 tencentcloud-sdk-python-cfw-3.0.895/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-19 02:45:50.000000 tencentcloud-sdk-python-cfw-3.0.895/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.894/README.rst` & `tencentcloud-sdk-python-cfw-3.0.895/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.894/tencentcloud/cfw/v20190904/errorcodes.py` & `tencentcloud-sdk-python-cfw-3.0.895/tencentcloud/cfw/v20190904/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.894/tencentcloud/cfw/v20190904/cfw_client.py` & `tencentcloud-sdk-python-cfw-3.0.895/tencentcloud/cfw/v20190904/cfw_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -597,14 +597,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeLogs(self, request):
+        """日志审计日志查询
+
+        :param request: Request instance for DescribeLogs.
+        :type request: :class:`tencentcloud.cfw.v20190904.models.DescribeLogsRequest`
+        :rtype: :class:`tencentcloud.cfw.v20190904.models.DescribeLogsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeLogs", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeLogsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeNatAcRule(self, request):
         """查询NAT访问控制列表
 
         :param request: Request instance for DescribeNatAcRule.
         :type request: :class:`tencentcloud.cfw.v20190904.models.DescribeNatAcRuleRequest`
         :rtype: :class:`tencentcloud.cfw.v20190904.models.DescribeNatAcRuleResponse`
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.894/tencentcloud/cfw/v20190904/models.py` & `tencentcloud-sdk-python-cfw-3.0.895/tencentcloud/cfw/v20190904/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2396,14 +2396,100 @@
                 obj._deserialize(item)
                 self.StatusList.append(obj)
         self.ReturnCode = params.get("ReturnCode")
         self.ReturnMsg = params.get("ReturnMsg")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeLogsRequest(AbstractModel):
+    """DescribeLogs请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Index: 日志类型标识
+流量日志：互联网边界防火墙netflow_border，NAT边界防火墙netflow_nat，VPC间防火墙vpcnetflow，内网流量日志netflow_fl
+入侵防御日志rule_threatinfo
+访问控制日志：互联网边界规则rule_acl，NAT边界规则rule_acl，内网间规则rule_vpcacl，企业安全组rule_sg
+操作日志：防火墙开关-开关操作operate_switch，防火墙开关-实例配置operate_instance，资产中心操作operate_assetgroup，访问控制操作operate_acl，零信任防护操作operate_identity，入侵防御操作-入侵防御operate_ids，入侵防御操作-安全基线operate_baseline，常用工具操作operate_tool，网络蜜罐操作operate_honeypot，日志投递操作operate_logdelivery，通用设置操作operate_logstorage，登录日志operate_login
+        :type Index: str
+        :param Limit: 每页条数，最大支持2000
+        :type Limit: int
+        :param Offset: 偏移值，最大支持60000
+        :type Offset: int
+        :param StartTime: 筛选开始时间
+        :type StartTime: str
+        :param EndTime: 筛选结束时间
+        :type EndTime: str
+        :param Filters: 过滤条件组合，各数组元素间为AND关系，查询字段名Name参考文档https://cloud.tencent.com/document/product/1132/87894，数值类型字段不支持模糊匹配
+        :type Filters: list of CommonFilter
+        """
+        self.Index = None
+        self.Limit = None
+        self.Offset = None
+        self.StartTime = None
+        self.EndTime = None
+        self.Filters = None
+
+
+    def _deserialize(self, params):
+        self.Index = params.get("Index")
+        self.Limit = params.get("Limit")
+        self.Offset = params.get("Offset")
+        self.StartTime = params.get("StartTime")
+        self.EndTime = params.get("EndTime")
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = CommonFilter()
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
+class DescribeLogsResponse(AbstractModel):
+    """DescribeLogs返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Data: 日志列表
+        :type Data: str
+        :param Total: 总条数
+        :type Total: int
+        :param ReturnCode: 返回状态码 0 成功 非0不成功
+        :type ReturnCode: int
+        :param ReturnMsg: 返回信息  success 成功 其他 不成功
+        :type ReturnMsg: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Data = None
+        self.Total = None
+        self.ReturnCode = None
+        self.ReturnMsg = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Data = params.get("Data")
+        self.Total = params.get("Total")
+        self.ReturnCode = params.get("ReturnCode")
+        self.ReturnMsg = params.get("ReturnMsg")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeNatAcRuleRequest(AbstractModel):
     """DescribeNatAcRule请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.894/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cfw-3.0.895/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cfw-3.0.894/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cfw-3.0.895/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfw
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Cfw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.894/PKG-INFO` & `tencentcloud-sdk-python-cfw-3.0.895/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfw
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Cfw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.894/setup.py` & `tencentcloud-sdk-python-cfw-3.0.895/setup.py`

 * *Files identical despite different names*

