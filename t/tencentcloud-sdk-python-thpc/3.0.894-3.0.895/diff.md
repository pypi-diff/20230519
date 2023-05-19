# Comparing `tmp/tencentcloud-sdk-python-thpc-3.0.894.tar.gz` & `tmp/tencentcloud-sdk-python-thpc-3.0.895.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-thpc-3.0.894.tar", last modified: Thu May 18 00:38:59 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-thpc-3.0.895.tar", last modified: Fri May 19 03:02:16 2023, max compression
```

## Comparing `tencentcloud-sdk-python-thpc-3.0.894.tar` & `tencentcloud-sdk-python-thpc-3.0.895.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/v20220401/
--rw-r--r--   0 root         (0) root         (0)     4733 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/v20220401/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/v20220401/__init__.py
--rw-r--r--   0 root         (0) root         (0)    97393 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/v20220401/models.py
--rw-r--r--   0 root         (0) root         (0)    16733 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/v20220401/thpc_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/v20211109/
--rw-r--r--   0 root         (0) root         (0)     2035 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/v20211109/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/v20211109/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43727 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/v20211109/models.py
--rw-r--r--   0 root         (0) root         (0)     4612 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/v20211109/thpc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/v20230321/
--rw-r--r--   0 root         (0) root         (0)     4248 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/v20230321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/v20230321/__init__.py
--rw-r--r--   0 root         (0) root         (0)   103105 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/v20230321/models.py
--rw-r--r--   0 root         (0) root         (0)    17699 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/v20230321/thpc_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/tencentcloud_sdk_python_thpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/tencentcloud_sdk_python_thpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      781 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/tencentcloud_sdk_python_thpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:38:59.000000 tencentcloud-sdk-python-thpc-3.0.894/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/v20220401/
+-rw-r--r--   0 root         (0) root         (0)     4733 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/v20220401/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/v20220401/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    97393 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/v20220401/models.py
+-rw-r--r--   0 root         (0) root         (0)    16733 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/v20220401/thpc_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/v20211109/
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/v20211109/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/v20211109/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43727 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/v20211109/models.py
+-rw-r--r--   0 root         (0) root         (0)     4612 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/v20211109/thpc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/v20230321/
+-rw-r--r--   0 root         (0) root         (0)     4248 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/v20230321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/v20230321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   105157 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/v20230321/models.py
+-rw-r--r--   0 root         (0) root         (0)    17699 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/v20230321/thpc_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/tencentcloud_sdk_python_thpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/tencentcloud_sdk_python_thpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      781 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/tencentcloud_sdk_python_thpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-19 03:02:16.000000 tencentcloud-sdk-python-thpc-3.0.895/setup.cfg
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.894/README.rst` & `tencentcloud-sdk-python-thpc-3.0.895/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/v20220401/errorcodes.py` & `tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/v20220401/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/v20220401/models.py` & `tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/v20220401/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/v20220401/thpc_client.py` & `tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/v20220401/thpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/v20211109/errorcodes.py` & `tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/v20211109/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/v20211109/models.py` & `tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/v20211109/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/v20211109/thpc_client.py` & `tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/v20211109/thpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/v20230321/errorcodes.py` & `tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/v20230321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/v20230321/models.py` & `tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/v20230321/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2122,26 +2122,35 @@
         :type DataDisks: list of DataDisk
         :param InternetAccessible: 公网带宽相关信息设置。若不指定该参数，则默认公网带宽为0Mbps。
         :type InternetAccessible: :class:`tencentcloud.thpc.v20230321.models.InternetAccessible`
         :param ExpansionNodeConfigs: 扩容节点配置信息。
         :type ExpansionNodeConfigs: list of ExpansionNodeConfig
         :param DesiredIdleNodeCapacity: 队列中期望的空闲节点数量（包含弹性节点和静态节点）。默认值：0。队列中，处于空闲状态的节点小于此值，集群会扩容弹性节点；处于空闲状态的节点大于此值，集群会缩容弹性节点。
         :type DesiredIdleNodeCapacity: int
+        :param ScaleOutRatio: 扩容比例。默认值：100。取值范围：1～100。
+如果扩容比例为50，那么每轮只会扩容当前作业负载所需的50%数量的节点。
+        :type ScaleOutRatio: int
+        :param ScaleOutNodeThreshold: 比例扩容阈值。默认值：0。取值范围：0～200。
+当作业负载需要扩容节点数量大于此值，当前扩容轮次按照ScaleOutRatio配置的的比例进行扩容。当作业负载需要扩容节点数量小于此值，当前扩容轮次扩容当前作业负载所需数量的节点。
+此参数配合ScaleOutRatio参数进行使用，用于比例扩容场景下，在作业负载所需节点数量较小时，加快收敛速度。
+        :type ScaleOutNodeThreshold: int
         """
         self.QueueName = None
         self.MinSize = None
         self.MaxSize = None
         self.EnableAutoExpansion = None
         self.EnableAutoShrink = None
         self.ImageId = None
         self.SystemDisk = None
         self.DataDisks = None
         self.InternetAccessible = None
         self.ExpansionNodeConfigs = None
         self.DesiredIdleNodeCapacity = None
+        self.ScaleOutRatio = None
+        self.ScaleOutNodeThreshold = None
 
 
     def _deserialize(self, params):
         self.QueueName = params.get("QueueName")
         self.MinSize = params.get("MinSize")
         self.MaxSize = params.get("MaxSize")
         self.EnableAutoExpansion = params.get("EnableAutoExpansion")
@@ -2162,14 +2171,16 @@
         if params.get("ExpansionNodeConfigs") is not None:
             self.ExpansionNodeConfigs = []
             for item in params.get("ExpansionNodeConfigs"):
                 obj = ExpansionNodeConfig()
                 obj._deserialize(item)
                 self.ExpansionNodeConfigs.append(obj)
         self.DesiredIdleNodeCapacity = params.get("DesiredIdleNodeCapacity")
+        self.ScaleOutRatio = params.get("ScaleOutRatio")
+        self.ScaleOutNodeThreshold = params.get("ScaleOutNodeThreshold")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2193,22 +2204,33 @@
         :param EnableAutoShrink: 是否开启自动缩容。
         :type EnableAutoShrink: bool
         :param ExpansionNodeConfigs: 扩容节点配置信息。
         :type ExpansionNodeConfigs: list of ExpansionNodeConfigOverview
         :param DesiredIdleNodeCapacity: 队列中期望的空闲节点数量（包含弹性节点和静态节点）。默认值：0。队列中，处于空闲状态的节点小于此值，集群会扩容弹性节点；处于空闲状态的节点大于此值，集群会缩容弹性节点。
 注意：此字段可能返回 null，表示取不到有效值。
         :type DesiredIdleNodeCapacity: int
+        :param ScaleOutRatio: 扩容比例。默认值：100。取值范围：1～100。
+如果扩容比例为50，那么每轮只会扩容当前作业负载所需的50%数量的节点。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ScaleOutRatio: int
+        :param ScaleOutNodeThreshold: 比例扩容阈值。默认值：0。取值范围：0～200。
+当作业负载需要扩容节点数量大于此值，当前扩容轮次按照ScaleOutRatio配置的的比例进行扩容。当作业负载需要扩容节点数量小于此值，当前扩容轮次扩容当前作业负载所需数量的节点。
+此参数配合ScaleOutRatio参数进行使用，用于比例扩容场景下，在作业负载所需节点数量较小时，加快收敛速度。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ScaleOutNodeThreshold: int
         """
         self.QueueName = None
         self.MinSize = None
         self.MaxSize = None
         self.EnableAutoExpansion = None
         self.EnableAutoShrink = None
         self.ExpansionNodeConfigs = None
         self.DesiredIdleNodeCapacity = None
+        self.ScaleOutRatio = None
+        self.ScaleOutNodeThreshold = None
 
 
     def _deserialize(self, params):
         self.QueueName = params.get("QueueName")
         self.MinSize = params.get("MinSize")
         self.MaxSize = params.get("MaxSize")
         self.EnableAutoExpansion = params.get("EnableAutoExpansion")
@@ -2216,14 +2238,16 @@
         if params.get("ExpansionNodeConfigs") is not None:
             self.ExpansionNodeConfigs = []
             for item in params.get("ExpansionNodeConfigs"):
                 obj = ExpansionNodeConfigOverview()
                 obj._deserialize(item)
                 self.ExpansionNodeConfigs.append(obj)
         self.DesiredIdleNodeCapacity = params.get("DesiredIdleNodeCapacity")
+        self.ScaleOutRatio = params.get("ScaleOutRatio")
+        self.ScaleOutNodeThreshold = params.get("ScaleOutNodeThreshold")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/thpc/v20230321/thpc_client.py` & `tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/thpc/v20230321/thpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.894/tencentcloud/__init__.py` & `tencentcloud-sdk-python-thpc-3.0.895/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-thpc-3.0.894/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-thpc-3.0.895/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.894/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-thpc-3.0.895/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-thpc
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Thpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.894/PKG-INFO` & `tencentcloud-sdk-python-thpc-3.0.895/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-thpc
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Thpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.894/setup.py` & `tencentcloud-sdk-python-thpc-3.0.895/setup.py`

 * *Files identical despite different names*

