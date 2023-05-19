# Comparing `tmp/tencentcloud-sdk-python-csip-3.0.894.tar.gz` & `tmp/tencentcloud-sdk-python-csip-3.0.895.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-csip-3.0.894.tar", last modified: Thu May 18 00:22:39 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-csip-3.0.895.tar", last modified: Fri May 19 02:47:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-csip-3.0.894.tar` & `tencentcloud-sdk-python-csip-3.0.895.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:22:39.000000 tencentcloud-sdk-python-csip-3.0.894/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:22:39.000000 tencentcloud-sdk-python-csip-3.0.894/tencentcloud_sdk_python_csip.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:22:39.000000 tencentcloud-sdk-python-csip-3.0.894/tencentcloud_sdk_python_csip.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-18 00:22:39.000000 tencentcloud-sdk-python-csip-3.0.894/tencentcloud_sdk_python_csip.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-18 00:22:39.000000 tencentcloud-sdk-python-csip-3.0.894/tencentcloud_sdk_python_csip.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:22:39.000000 tencentcloud-sdk-python-csip-3.0.894/tencentcloud_sdk_python_csip.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-18 00:22:39.000000 tencentcloud-sdk-python-csip-3.0.894/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:22:39.000000 tencentcloud-sdk-python-csip-3.0.894/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:22:39.000000 tencentcloud-sdk-python-csip-3.0.894/tencentcloud/csip/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:22:39.000000 tencentcloud-sdk-python-csip-3.0.894/tencentcloud/csip/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:22:39.000000 tencentcloud-sdk-python-csip-3.0.894/tencentcloud/csip/v20221121/
--rw-r--r--   0 root         (0) root         (0)     8000 2023-05-18 00:22:39.000000 tencentcloud-sdk-python-csip-3.0.894/tencentcloud/csip/v20221121/csip_client.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-05-18 00:22:39.000000 tencentcloud-sdk-python-csip-3.0.894/tencentcloud/csip/v20221121/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:22:39.000000 tencentcloud-sdk-python-csip-3.0.894/tencentcloud/csip/v20221121/__init__.py
--rw-r--r--   0 root         (0) root         (0)    59464 2023-05-18 00:22:39.000000 tencentcloud-sdk-python-csip-3.0.894/tencentcloud/csip/v20221121/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:22:39.000000 tencentcloud-sdk-python-csip-3.0.894/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-18 00:22:39.000000 tencentcloud-sdk-python-csip-3.0.894/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-18 00:22:39.000000 tencentcloud-sdk-python-csip-3.0.894/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:22:39.000000 tencentcloud-sdk-python-csip-3.0.894/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:47:51.000000 tencentcloud-sdk-python-csip-3.0.895/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:47:51.000000 tencentcloud-sdk-python-csip-3.0.895/tencentcloud_sdk_python_csip.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 02:47:51.000000 tencentcloud-sdk-python-csip-3.0.895/tencentcloud_sdk_python_csip.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-19 02:47:51.000000 tencentcloud-sdk-python-csip-3.0.895/tencentcloud_sdk_python_csip.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-19 02:47:51.000000 tencentcloud-sdk-python-csip-3.0.895/tencentcloud_sdk_python_csip.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 02:47:51.000000 tencentcloud-sdk-python-csip-3.0.895/tencentcloud_sdk_python_csip.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-19 02:47:50.000000 tencentcloud-sdk-python-csip-3.0.895/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:47:51.000000 tencentcloud-sdk-python-csip-3.0.895/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:47:51.000000 tencentcloud-sdk-python-csip-3.0.895/tencentcloud/csip/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:47:50.000000 tencentcloud-sdk-python-csip-3.0.895/tencentcloud/csip/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:47:51.000000 tencentcloud-sdk-python-csip-3.0.895/tencentcloud/csip/v20221121/
+-rw-r--r--   0 root         (0) root         (0)     8000 2023-05-19 02:47:50.000000 tencentcloud-sdk-python-csip-3.0.895/tencentcloud/csip/v20221121/csip_client.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-05-19 02:47:50.000000 tencentcloud-sdk-python-csip-3.0.895/tencentcloud/csip/v20221121/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:47:50.000000 tencentcloud-sdk-python-csip-3.0.895/tencentcloud/csip/v20221121/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60110 2023-05-19 02:47:50.000000 tencentcloud-sdk-python-csip-3.0.895/tencentcloud/csip/v20221121/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-19 02:47:50.000000 tencentcloud-sdk-python-csip-3.0.895/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-19 02:47:51.000000 tencentcloud-sdk-python-csip-3.0.895/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-19 02:47:50.000000 tencentcloud-sdk-python-csip-3.0.895/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-19 02:47:51.000000 tencentcloud-sdk-python-csip-3.0.895/setup.cfg
```

### Comparing `tencentcloud-sdk-python-csip-3.0.894/tencentcloud_sdk_python_csip.egg-info/PKG-INFO` & `tencentcloud-sdk-python-csip-3.0.895/tencentcloud_sdk_python_csip.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-csip
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Csip SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-csip-3.0.894/README.rst` & `tencentcloud-sdk-python-csip-3.0.895/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-csip-3.0.894/tencentcloud/csip/v20221121/csip_client.py` & `tencentcloud-sdk-python-csip-3.0.895/tencentcloud/csip/v20221121/csip_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-csip-3.0.894/tencentcloud/csip/v20221121/errorcodes.py` & `tencentcloud-sdk-python-csip-3.0.895/tencentcloud/csip/v20221121/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-csip-3.0.894/tencentcloud/csip/v20221121/models.py` & `tencentcloud-sdk-python-csip-3.0.895/tencentcloud/csip/v20221121/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,14 +362,17 @@
         :type Tag: list of Tag
         :param MemberId: memberId
 注意：此字段可能返回 null，表示取不到有效值。
         :type MemberId: str
         :param Os: os全称
 注意：此字段可能返回 null，表示取不到有效值。
         :type Os: str
+        :param RiskExposure: 风险服务暴露
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RiskExposure: int
         """
         self.AssetId = None
         self.AssetName = None
         self.AssetType = None
         self.Region = None
         self.CWPStatus = None
         self.AssetCreateTime = None
@@ -411,14 +414,15 @@
         self.PortRisk = None
         self.VulnerabilityRisk = None
         self.ConfigurationRisk = None
         self.ScanTask = None
         self.Tag = None
         self.MemberId = None
         self.Os = None
+        self.RiskExposure = None
 
 
     def _deserialize(self, params):
         self.AssetId = params.get("AssetId")
         self.AssetName = params.get("AssetName")
         self.AssetType = params.get("AssetType")
         self.Region = params.get("Region")
@@ -467,14 +471,15 @@
             self.Tag = []
             for item in params.get("Tag"):
                 obj = Tag()
                 obj._deserialize(item)
                 self.Tag.append(obj)
         self.MemberId = params.get("MemberId")
         self.Os = params.get("Os")
+        self.RiskExposure = params.get("RiskExposure")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -802,27 +807,31 @@
         :type IpTypeList: list of FilterDataObject
         :param AppIdList: appid列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type AppIdList: list of FilterDataObject
         :param ZoneList: 可用区列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type ZoneList: list of FilterDataObject
+        :param OsList: os列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OsList: list of FilterDataObject
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Total = None
         self.Data = None
         self.RegionList = None
         self.DefenseStatusList = None
         self.VpcList = None
         self.AssetTypeList = None
         self.SystemTypeList = None
         self.IpTypeList = None
         self.AppIdList = None
         self.ZoneList = None
+        self.OsList = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.Total = params.get("Total")
         if params.get("Data") is not None:
             self.Data = []
@@ -874,14 +883,20 @@
                 self.AppIdList.append(obj)
         if params.get("ZoneList") is not None:
             self.ZoneList = []
             for item in params.get("ZoneList"):
                 obj = FilterDataObject()
                 obj._deserialize(item)
                 self.ZoneList.append(obj)
+        if params.get("OsList") is not None:
+            self.OsList = []
+            for item in params.get("OsList"):
+                obj = FilterDataObject()
+                obj._deserialize(item)
+                self.OsList.append(obj)
         self.RequestId = params.get("RequestId")
 
 
 class DescribeDbAssetInfoRequest(AbstractModel):
     """DescribeDbAssetInfo请求参数结构体
 
     """
@@ -1271,17 +1286,17 @@
 
     def __init__(self):
         r"""
         :param Limit: 查询数量限制
         :type Limit: int
         :param Offset: 查询偏移位置
         :type Offset: int
-        :param Order: 需排序的字段
+        :param Order: 排序采用升序还是降序 升:asc 降 desc
         :type Order: str
-        :param By: 排序采用升序还是降序 升:asc 降 desc
+        :param By: 需排序的字段
         :type By: str
         :param Filters: 过滤的列及内容
         :type Filters: list of WhereFilter
         :param StartTime: 可填无， 日志使用查询时间
         :type StartTime: str
         :param EndTime: 可填无， 日志使用查询时间
         :type EndTime: str
```

### Comparing `tencentcloud-sdk-python-csip-3.0.894/tencentcloud/__init__.py` & `tencentcloud-sdk-python-csip-3.0.895/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-csip-3.0.894/PKG-INFO` & `tencentcloud-sdk-python-csip-3.0.895/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-csip
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Csip SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-csip-3.0.894/setup.py` & `tencentcloud-sdk-python-csip-3.0.895/setup.py`

 * *Files identical despite different names*

