# Comparing `tmp/tencentcloud-sdk-python-tcss-3.0.894.tar.gz` & `tmp/tencentcloud-sdk-python-tcss-3.0.895.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcss-3.0.894.tar", last modified: Thu May 18 00:38:08 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcss-3.0.895.tar", last modified: Fri May 19 03:01:28 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcss-3.0.894.tar` & `tencentcloud-sdk-python-tcss-3.0.895.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/tcss/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/tcss/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/tcss/v20201101/
--rw-r--r--   0 root         (0) root         (0)   316128 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/tcss/v20201101/tcss_client.py
--rw-r--r--   0 root         (0) root         (0)     3916 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/tcss/v20201101/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/tcss/v20201101/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1015595 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/tcss/v20201101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud_sdk_python_tcss.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud_sdk_python_tcss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud_sdk_python_tcss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/tencentcloud_sdk_python_tcss.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:38:08.000000 tencentcloud-sdk-python-tcss-3.0.894/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:01:28.000000 tencentcloud-sdk-python-tcss-3.0.895/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-19 03:01:28.000000 tencentcloud-sdk-python-tcss-3.0.895/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:01:28.000000 tencentcloud-sdk-python-tcss-3.0.895/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-19 03:01:28.000000 tencentcloud-sdk-python-tcss-3.0.895/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:01:28.000000 tencentcloud-sdk-python-tcss-3.0.895/tencentcloud/tcss/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 03:01:28.000000 tencentcloud-sdk-python-tcss-3.0.895/tencentcloud/tcss/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:01:28.000000 tencentcloud-sdk-python-tcss-3.0.895/tencentcloud/tcss/v20201101/
+-rw-r--r--   0 root         (0) root         (0)   316128 2023-05-19 03:01:28.000000 tencentcloud-sdk-python-tcss-3.0.895/tencentcloud/tcss/v20201101/tcss_client.py
+-rw-r--r--   0 root         (0) root         (0)     3916 2023-05-19 03:01:28.000000 tencentcloud-sdk-python-tcss-3.0.895/tencentcloud/tcss/v20201101/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 03:01:28.000000 tencentcloud-sdk-python-tcss-3.0.895/tencentcloud/tcss/v20201101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1040070 2023-05-19 03:01:28.000000 tencentcloud-sdk-python-tcss-3.0.895/tencentcloud/tcss/v20201101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:01:28.000000 tencentcloud-sdk-python-tcss-3.0.895/tencentcloud_sdk_python_tcss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 03:01:28.000000 tencentcloud-sdk-python-tcss-3.0.895/tencentcloud_sdk_python_tcss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-19 03:01:28.000000 tencentcloud-sdk-python-tcss-3.0.895/tencentcloud_sdk_python_tcss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-19 03:01:28.000000 tencentcloud-sdk-python-tcss-3.0.895/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 03:01:28.000000 tencentcloud-sdk-python-tcss-3.0.895/tencentcloud_sdk_python_tcss.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-19 03:01:28.000000 tencentcloud-sdk-python-tcss-3.0.895/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-19 03:01:28.000000 tencentcloud-sdk-python-tcss-3.0.895/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-19 03:01:28.000000 tencentcloud-sdk-python-tcss-3.0.895/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.894/README.rst` & `tencentcloud-sdk-python-tcss-3.0.895/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcss-3.0.895/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/tcss/v20201101/tcss_client.py` & `tencentcloud-sdk-python-tcss-3.0.895/tencentcloud/tcss/v20201101/tcss_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/tcss/v20201101/errorcodes.py` & `tencentcloud-sdk-python-tcss-3.0.895/tencentcloud/tcss/v20201101/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.894/tencentcloud/tcss/v20201101/models.py` & `tencentcloud-sdk-python-tcss-3.0.895/tencentcloud/tcss/v20201101/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,14 +230,36 @@
 暂停: PAUSED
 停止: STOPPED
 已经创建: CREATED
 已经销毁: DESTROYED
 正在重启中: RESTARTING
 迁移中: REMOVING
         :type ContainerStatus: str
+        :param ClusterID: 集群ID
+        :type ClusterID: str
+        :param NodeType: 节点类型：NORMAL普通节点、SUPER超级节点
+        :type NodeType: str
+        :param PodName: pod 名称
+        :type PodName: str
+        :param PodIP: pod ip
+        :type PodIP: str
+        :param NodeUniqueID: 集群id
+        :type NodeUniqueID: str
+        :param PublicIP: 节点公网ip
+        :type PublicIP: str
+        :param NodeName: 节点名称
+        :type NodeName: str
+        :param NodeID: 节点id
+        :type NodeID: str
+        :param HostID: uuid
+        :type HostID: str
+        :param HostIP: 节点内网ip
+        :type HostIP: str
+        :param ClusterName: 集群名称
+        :type ClusterName: str
         """
         self.ProcessPath = None
         self.EventType = None
         self.MatchRuleName = None
         self.FoundTime = None
         self.ContainerName = None
         self.ImageName = None
@@ -257,14 +279,25 @@
         self.RuleId = None
         self.MatchGroupName = None
         self.MatchRuleLevel = None
         self.ContainerNetStatus = None
         self.ContainerNetSubStatus = None
         self.ContainerIsolateOperationSrc = None
         self.ContainerStatus = None
+        self.ClusterID = None
+        self.NodeType = None
+        self.PodName = None
+        self.PodIP = None
+        self.NodeUniqueID = None
+        self.PublicIP = None
+        self.NodeName = None
+        self.NodeID = None
+        self.HostID = None
+        self.HostIP = None
+        self.ClusterName = None
 
 
     def _deserialize(self, params):
         self.ProcessPath = params.get("ProcessPath")
         self.EventType = params.get("EventType")
         self.MatchRuleName = params.get("MatchRuleName")
         self.FoundTime = params.get("FoundTime")
@@ -286,14 +319,25 @@
         self.RuleId = params.get("RuleId")
         self.MatchGroupName = params.get("MatchGroupName")
         self.MatchRuleLevel = params.get("MatchRuleLevel")
         self.ContainerNetStatus = params.get("ContainerNetStatus")
         self.ContainerNetSubStatus = params.get("ContainerNetSubStatus")
         self.ContainerIsolateOperationSrc = params.get("ContainerIsolateOperationSrc")
         self.ContainerStatus = params.get("ContainerStatus")
+        self.ClusterID = params.get("ClusterID")
+        self.NodeType = params.get("NodeType")
+        self.PodName = params.get("PodName")
+        self.PodIP = params.get("PodIP")
+        self.NodeUniqueID = params.get("NodeUniqueID")
+        self.PublicIP = params.get("PublicIP")
+        self.NodeName = params.get("NodeName")
+        self.NodeID = params.get("NodeID")
+        self.HostID = params.get("HostID")
+        self.HostIP = params.get("HostIP")
+        self.ClusterName = params.get("ClusterName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -641,14 +685,36 @@
 暂停: PAUSED
 停止: STOPPED
 已经创建: CREATED
 已经销毁: DESTROYED
 正在重启中: RESTARTING
 迁移中: REMOVING
         :type ContainerStatus: str
+        :param NodeName: 节点名称：如果是超级节点，展示的实质上是它的node_id
+        :type NodeName: str
+        :param PodName: pod名称
+        :type PodName: str
+        :param PodIP: pod ip
+        :type PodIP: str
+        :param NodeType: 节点类型：NORMAL普通节点、SUPER超级节点
+        :type NodeType: str
+        :param ClusterID: 集群id
+        :type ClusterID: str
+        :param NodeUniqueID: 节点的唯一id，主要是超级节点使用
+        :type NodeUniqueID: str
+        :param PublicIP: 节点公网IP
+        :type PublicIP: str
+        :param NodeID: 节点id
+        :type NodeID: str
+        :param HostID: uuid
+        :type HostID: str
+        :param HostIP: 节点内网ip
+        :type HostIP: str
+        :param ClusterName: 集群名称
+        :type ClusterName: str
         """
         self.ProcessName = None
         self.MatchRuleName = None
         self.FoundTime = None
         self.ContainerName = None
         self.ImageName = None
         self.Behavior = None
@@ -669,14 +735,25 @@
         self.EventCount = None
         self.LatestFoundTime = None
         self.RuleId = None
         self.ContainerNetStatus = None
         self.ContainerNetSubStatus = None
         self.ContainerIsolateOperationSrc = None
         self.ContainerStatus = None
+        self.NodeName = None
+        self.PodName = None
+        self.PodIP = None
+        self.NodeType = None
+        self.ClusterID = None
+        self.NodeUniqueID = None
+        self.PublicIP = None
+        self.NodeID = None
+        self.HostID = None
+        self.HostIP = None
+        self.ClusterName = None
 
 
     def _deserialize(self, params):
         self.ProcessName = params.get("ProcessName")
         self.MatchRuleName = params.get("MatchRuleName")
         self.FoundTime = params.get("FoundTime")
         self.ContainerName = params.get("ContainerName")
@@ -699,14 +776,25 @@
         self.EventCount = params.get("EventCount")
         self.LatestFoundTime = params.get("LatestFoundTime")
         self.RuleId = params.get("RuleId")
         self.ContainerNetStatus = params.get("ContainerNetStatus")
         self.ContainerNetSubStatus = params.get("ContainerNetSubStatus")
         self.ContainerIsolateOperationSrc = params.get("ContainerIsolateOperationSrc")
         self.ContainerStatus = params.get("ContainerStatus")
+        self.NodeName = params.get("NodeName")
+        self.PodName = params.get("PodName")
+        self.PodIP = params.get("PodIP")
+        self.NodeType = params.get("NodeType")
+        self.ClusterID = params.get("ClusterID")
+        self.NodeUniqueID = params.get("NodeUniqueID")
+        self.PublicIP = params.get("PublicIP")
+        self.NodeID = params.get("NodeID")
+        self.HostID = params.get("HostID")
+        self.HostIP = params.get("HostIP")
+        self.ClusterName = params.get("ClusterName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1769,36 +1857,40 @@
         :type ClusterVersion: str
         :param ContainerRuntime: 运行时组件,docker或者containerd
         :type ContainerRuntime: str
         :param Region: 区域
         :type Region: str
         :param VerifyInfo: 检查结果的验证信息
         :type VerifyInfo: str
+        :param NodeName: 节点名称
+        :type NodeName: str
         """
         self.ClusterId = None
         self.ClusterName = None
         self.InstanceId = None
         self.PrivateIpAddresses = None
         self.InstanceRole = None
         self.ClusterVersion = None
         self.ContainerRuntime = None
         self.Region = None
         self.VerifyInfo = None
+        self.NodeName = None
 
 
     def _deserialize(self, params):
         self.ClusterId = params.get("ClusterId")
         self.ClusterName = params.get("ClusterName")
         self.InstanceId = params.get("InstanceId")
         self.PrivateIpAddresses = params.get("PrivateIpAddresses")
         self.InstanceRole = params.get("InstanceRole")
         self.ClusterVersion = params.get("ClusterVersion")
         self.ContainerRuntime = params.get("ContainerRuntime")
         self.Region = params.get("Region")
         self.VerifyInfo = params.get("VerifyInfo")
+        self.NodeName = params.get("NodeName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1863,31 +1955,44 @@
 CSR_RUNNING: 运行中
 CSR_EXCEPTION:异常
 CSR_DEL:已经删除
         :type Status: str
         :param BindRuleName: 绑定规则名称
         :type BindRuleName: str
         :param ClusterType: 集群类型:
-CT_TKE: TKE集群
-CT_USER_CREATE: 用户自建集群
+CT_TKE:TKE集群;
+CT_USER_CREATE:用户自建集群;
+CT_TKE_SERVERLESS:TKE Serverless集群;
         :type ClusterType: str
+        :param ClusterVersion: 集群版本
+        :type ClusterVersion: str
+        :param MemLimit: 内存量
+        :type MemLimit: int
+        :param CpuLimit: cpu
+        :type CpuLimit: int
         """
         self.ClusterID = None
         self.ClusterName = None
         self.Status = None
         self.BindRuleName = None
         self.ClusterType = None
+        self.ClusterVersion = None
+        self.MemLimit = None
+        self.CpuLimit = None
 
 
     def _deserialize(self, params):
         self.ClusterID = params.get("ClusterID")
         self.ClusterName = params.get("ClusterName")
         self.Status = params.get("Status")
         self.BindRuleName = params.get("BindRuleName")
         self.ClusterType = params.get("ClusterType")
+        self.ClusterVersion = params.get("ClusterVersion")
+        self.MemLimit = params.get("MemLimit")
+        self.CpuLimit = params.get("CpuLimit")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3885,14 +3990,28 @@
         :type NetSubStatus: str
         :param IsolateSource: 隔离来源
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsolateSource: str
         :param IsolateTime: 隔离时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsolateTime: str
+        :param NodeID: 超级节点id
+        :type NodeID: str
+        :param PodIP: podip
+        :type PodIP: str
+        :param PodName: pod名称
+        :type PodName: str
+        :param NodeType: 节点类型:节点类型：NORMAL普通节点、SUPER超级节点
+        :type NodeType: str
+        :param NodeUniqueID: 超级节点唯一id
+        :type NodeUniqueID: str
+        :param PodCpu: 所属Pod的CPU
+        :type PodCpu: int
+        :param PodMem: 所属Pod的内存
+        :type PodMem: int
         """
         self.ContainerID = None
         self.ContainerName = None
         self.Status = None
         self.CreateTime = None
         self.RunAs = None
         self.Cmd = None
@@ -3906,14 +4025,21 @@
         self.UpdateTime = None
         self.HostName = None
         self.PublicIp = None
         self.NetStatus = None
         self.NetSubStatus = None
         self.IsolateSource = None
         self.IsolateTime = None
+        self.NodeID = None
+        self.PodIP = None
+        self.PodName = None
+        self.NodeType = None
+        self.NodeUniqueID = None
+        self.PodCpu = None
+        self.PodMem = None
 
 
     def _deserialize(self, params):
         self.ContainerID = params.get("ContainerID")
         self.ContainerName = params.get("ContainerName")
         self.Status = params.get("Status")
         self.CreateTime = params.get("CreateTime")
@@ -3929,14 +4055,21 @@
         self.UpdateTime = params.get("UpdateTime")
         self.HostName = params.get("HostName")
         self.PublicIp = params.get("PublicIp")
         self.NetStatus = params.get("NetStatus")
         self.NetSubStatus = params.get("NetSubStatus")
         self.IsolateSource = params.get("IsolateSource")
         self.IsolateTime = params.get("IsolateTime")
+        self.NodeID = params.get("NodeID")
+        self.PodIP = params.get("PodIP")
+        self.PodName = params.get("PodName")
+        self.NodeType = params.get("NodeType")
+        self.NodeUniqueID = params.get("NodeUniqueID")
+        self.PodCpu = params.get("PodCpu")
+        self.PodMem = params.get("PodMem")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -8913,14 +9046,40 @@
         :type NetSubStatus: str
         :param IsolateSource: 隔离来源
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsolateSource: str
         :param IsolateTime: 隔离时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsolateTime: str
+        :param NodeID: 节点ID
+        :type NodeID: str
+        :param NodeName: 节点名称
+        :type NodeName: str
+        :param NodeSubNetID: 节点子网ID
+        :type NodeSubNetID: str
+        :param NodeSubNetName: 节点子网名称
+        :type NodeSubNetName: str
+        :param NodeSubNetCIDR: 节点子网网段
+        :type NodeSubNetCIDR: str
+        :param PodName: pod名称
+        :type PodName: str
+        :param PodIP: pod ip
+        :type PodIP: str
+        :param PodStatus: pod状态
+        :type PodStatus: str
+        :param ClusterID: 集群ID
+        :type ClusterID: str
+        :param ClusterName: 集群名称
+        :type ClusterName: str
+        :param NodeType: 节点类型:NORMAL: 普通节点(默认值) SUPER: 超级节点
+        :type NodeType: str
+        :param NodeUniqueID: 超级节点唯一id
+        :type NodeUniqueID: str
+        :param PublicIP: 外网ip
+        :type PublicIP: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.HostID = None
         self.HostIP = None
         self.ContainerName = None
         self.Status = None
@@ -8943,14 +9102,27 @@
         self.ImageCreateTime = None
         self.ImageSize = None
         self.HostStatus = None
         self.NetStatus = None
         self.NetSubStatus = None
         self.IsolateSource = None
         self.IsolateTime = None
+        self.NodeID = None
+        self.NodeName = None
+        self.NodeSubNetID = None
+        self.NodeSubNetName = None
+        self.NodeSubNetCIDR = None
+        self.PodName = None
+        self.PodIP = None
+        self.PodStatus = None
+        self.ClusterID = None
+        self.ClusterName = None
+        self.NodeType = None
+        self.NodeUniqueID = None
+        self.PublicIP = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.HostID = params.get("HostID")
         self.HostIP = params.get("HostIP")
         self.ContainerName = params.get("ContainerName")
@@ -8981,14 +9153,27 @@
         self.ImageCreateTime = params.get("ImageCreateTime")
         self.ImageSize = params.get("ImageSize")
         self.HostStatus = params.get("HostStatus")
         self.NetStatus = params.get("NetStatus")
         self.NetSubStatus = params.get("NetSubStatus")
         self.IsolateSource = params.get("IsolateSource")
         self.IsolateTime = params.get("IsolateTime")
+        self.NodeID = params.get("NodeID")
+        self.NodeName = params.get("NodeName")
+        self.NodeSubNetID = params.get("NodeSubNetID")
+        self.NodeSubNetName = params.get("NodeSubNetName")
+        self.NodeSubNetCIDR = params.get("NodeSubNetCIDR")
+        self.PodName = params.get("PodName")
+        self.PodIP = params.get("PodIP")
+        self.PodStatus = params.get("PodStatus")
+        self.ClusterID = params.get("ClusterID")
+        self.ClusterName = params.get("ClusterName")
+        self.NodeType = params.get("NodeType")
+        self.NodeUniqueID = params.get("NodeUniqueID")
+        self.PublicIP = params.get("PublicIP")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeAssetContainerListRequest(AbstractModel):
     """DescribeAssetContainerList请求参数结构体
 
     """
@@ -9003,14 +9188,19 @@
 <li>ContainerName - String - 是否必填：否 - 容器名称模糊搜索</li>
 <li>Status - String - 是否必填：否 - 容器运行状态筛选，0："created",1："running", 2："paused", 3："restarting", 4："removing", 5："exited", 6："dead" </li>
 <li>Runas - String - 是否必填：否 - 运行用户筛选</li>
 <li>ImageName- String - 是否必填：否 - 镜像名称搜索</li>
 <li>HostIP- string - 是否必填：否 - 主机ip搜索</li>
 <li>OrderBy - String 是否必填：否 -排序字段，支持：cpu_usage, mem_usage的动态排序 ["cpu_usage","+"]  '+'升序、'-'降序</li>
 <li>NetStatus - String -是否必填: 否 -  容器网络状态筛选 normal isolated isolating isolate_failed restoring restore_failed</li>
+<li>PodID - String -是否必填: 否 - PodID筛选</li>
+<li>NodeUniqueID - String -是否必填: 否 - SuperNode筛选</li>
+<li>PodUid - String -是否必填: 否 - Pod筛选</li>
+<li>PodIP - String -是否必填: 否 - PodIP筛选</li>
+<li>NodeType - String -是否必填: 否 - 节点类型筛选:NORMAL:普通节点;SUPER:超级节点</li>
         :type Filters: list of AssetFilters
         :param By: 排序字段
         :type By: str
         :param Order: 排序方式 asc,desc
         :type Order: str
         """
         self.Limit = None
@@ -11801,14 +11991,18 @@
         :type WebServiceCnt: int
         :param LatestImageScanTime: 最近镜像扫描时间
         :type LatestImageScanTime: str
         :param ImageUnsafeCnt: 风险镜像个数
         :type ImageUnsafeCnt: int
         :param HostUnInstallCnt: 主机未安装agent数量
         :type HostUnInstallCnt: int
+        :param SuperNodeCnt: 超级节点个数
+        :type SuperNodeCnt: int
+        :param SuperNodeRunningCnt: 超级节点运行个数
+        :type SuperNodeRunningCnt: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.AppCnt = None
         self.ContainerCnt = None
         self.ContainerPause = None
         self.ContainerRunning = None
@@ -11824,14 +12018,16 @@
         self.ImageUntrustCnt = None
         self.ListenPortCnt = None
         self.ProcessCnt = None
         self.WebServiceCnt = None
         self.LatestImageScanTime = None
         self.ImageUnsafeCnt = None
         self.HostUnInstallCnt = None
+        self.SuperNodeCnt = None
+        self.SuperNodeRunningCnt = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.AppCnt = params.get("AppCnt")
         self.ContainerCnt = params.get("ContainerCnt")
         self.ContainerPause = params.get("ContainerPause")
@@ -11848,14 +12044,16 @@
         self.ImageUntrustCnt = params.get("ImageUntrustCnt")
         self.ListenPortCnt = params.get("ListenPortCnt")
         self.ProcessCnt = params.get("ProcessCnt")
         self.WebServiceCnt = params.get("WebServiceCnt")
         self.LatestImageScanTime = params.get("LatestImageScanTime")
         self.ImageUnsafeCnt = params.get("ImageUnsafeCnt")
         self.HostUnInstallCnt = params.get("HostUnInstallCnt")
+        self.SuperNodeCnt = params.get("SuperNodeCnt")
+        self.SuperNodeRunningCnt = params.get("SuperNodeRunningCnt")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeAssetSyncLastTimeRequest(AbstractModel):
     """DescribeAssetSyncLastTime请求参数结构体
 
     """
@@ -12264,28 +12462,31 @@
         :type AutoCheckClusterCount: int
         :param ManualCheckClusterCount: 手动检查集群数
         :type ManualCheckClusterCount: int
         :param FailedClusterCount: 检查失败集群数
         :type FailedClusterCount: int
         :param NotImportedClusterCount: 未导入的集群数量
         :type NotImportedClusterCount: int
+        :param ServerlessClusterCount: eks集群数量
+        :type ServerlessClusterCount: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.TotalCount = None
         self.RiskClusterCount = None
         self.UncheckClusterCount = None
         self.ManagedClusterCount = None
         self.IndependentClusterCount = None
         self.NoRiskClusterCount = None
         self.CheckedClusterCount = None
         self.AutoCheckClusterCount = None
         self.ManualCheckClusterCount = None
         self.FailedClusterCount = None
         self.NotImportedClusterCount = None
+        self.ServerlessClusterCount = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.TotalCount = params.get("TotalCount")
         self.RiskClusterCount = params.get("RiskClusterCount")
         self.UncheckClusterCount = params.get("UncheckClusterCount")
@@ -12293,14 +12494,15 @@
         self.IndependentClusterCount = params.get("IndependentClusterCount")
         self.NoRiskClusterCount = params.get("NoRiskClusterCount")
         self.CheckedClusterCount = params.get("CheckedClusterCount")
         self.AutoCheckClusterCount = params.get("AutoCheckClusterCount")
         self.ManualCheckClusterCount = params.get("ManualCheckClusterCount")
         self.FailedClusterCount = params.get("FailedClusterCount")
         self.NotImportedClusterCount = params.get("NotImportedClusterCount")
+        self.ServerlessClusterCount = params.get("ServerlessClusterCount")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeComplianceAssetDetailInfoRequest(AbstractModel):
     """DescribeComplianceAssetDetailInfo请求参数结构体
 
     """
@@ -13040,28 +13242,31 @@
         :type HostOfflineCnt: int
         :param ImageRegistryCnt: 镜像仓库数量
         :type ImageRegistryCnt: int
         :param ImageTotalCnt: 镜像总数
         :type ImageTotalCnt: int
         :param HostUnInstallCnt: 主机未安装agent数量
         :type HostUnInstallCnt: int
+        :param HostSuperNodeCnt: 超级节点个数
+        :type HostSuperNodeCnt: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.ContainerTotalCnt = None
         self.ContainerRunningCnt = None
         self.ContainerPauseCnt = None
         self.ContainerStopped = None
         self.ImageCnt = None
         self.HostCnt = None
         self.HostRunningCnt = None
         self.HostOfflineCnt = None
         self.ImageRegistryCnt = None
         self.ImageTotalCnt = None
         self.HostUnInstallCnt = None
+        self.HostSuperNodeCnt = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.ContainerTotalCnt = params.get("ContainerTotalCnt")
         self.ContainerRunningCnt = params.get("ContainerRunningCnt")
         self.ContainerPauseCnt = params.get("ContainerPauseCnt")
@@ -13069,14 +13274,15 @@
         self.ImageCnt = params.get("ImageCnt")
         self.HostCnt = params.get("HostCnt")
         self.HostRunningCnt = params.get("HostRunningCnt")
         self.HostOfflineCnt = params.get("HostOfflineCnt")
         self.ImageRegistryCnt = params.get("ImageRegistryCnt")
         self.ImageTotalCnt = params.get("ImageTotalCnt")
         self.HostUnInstallCnt = params.get("HostUnInstallCnt")
+        self.HostSuperNodeCnt = params.get("HostSuperNodeCnt")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeContainerSecEventSummaryRequest(AbstractModel):
     """DescribeContainerSecEventSummary请求参数结构体
 
     """
@@ -18639,17 +18845,14 @@
         :type ProcessStartAccount: str
         :param ProcessFileAuthority: 进程文件权限
 注意：此字段可能返回 null，表示取不到有效值。
         :type ProcessFileAuthority: str
         :param SourceType: 来源：0：一键扫描， 1：定时扫描 2：实时监控
 注意：此字段可能返回 null，表示取不到有效值。
         :type SourceType: int
-        :param PodName: 集群名称
-注意：此字段可能返回 null，表示取不到有效值。
-        :type PodName: str
         :param Tags: 标签
 注意：此字段可能返回 null，表示取不到有效值。
         :type Tags: list of str
         :param HarmDescribe: 事件描述
 注意：此字段可能返回 null，表示取不到有效值。
         :type HarmDescribe: str
         :param SuggestScheme: 建议方案
@@ -18663,14 +18866,17 @@
         :type FileName: str
         :param FileMd5: 文件MD5
 注意：此字段可能返回 null，表示取不到有效值。
         :type FileMd5: str
         :param EventType: 事件类型
 注意：此字段可能返回 null，表示取不到有效值。
         :type EventType: str
+        :param PodName: 集群名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PodName: str
         :param Status: DEAL_NONE:文件待处理
 DEAL_IGNORE:已经忽略
 DEAL_ADD_WHITELIST:加白
 DEAL_DEL:文件已经删除
 DEAL_ISOLATE:已经隔离
 DEAL_ISOLATING:隔离中
 DEAL_ISOLATE_FAILED:隔离失败
@@ -18739,14 +18945,34 @@
         :type CheckPlatform: list of str
         :param FileAccessTime: 文件访问时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type FileAccessTime: str
         :param FileModifyTime: 文件修改时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type FileModifyTime: str
+        :param NodeSubNetID: 节点子网ID
+        :type NodeSubNetID: str
+        :param NodeSubNetName: 节点子网名称
+        :type NodeSubNetName: str
+        :param NodeSubNetCIDR: 节点子网网段
+        :type NodeSubNetCIDR: str
+        :param ClusterID: 集群id
+        :type ClusterID: str
+        :param PodIP: pod ip
+        :type PodIP: str
+        :param PodStatus: pod状态
+        :type PodStatus: str
+        :param NodeUniqueID: 节点唯一ID
+        :type NodeUniqueID: str
+        :param NodeType: 节点类型：NORMAL普通节点、SUPER超级节点
+        :type NodeType: str
+        :param NodeID: 节点ID
+        :type NodeID: str
+        :param ClusterName: 集群名称
+        :type ClusterName: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.ImageId = None
         self.ImageName = None
         self.CreateTime = None
         self.Size = None
@@ -18764,22 +18990,22 @@
         self.ProcessId = None
         self.ProcessArgv = None
         self.ProcessChan = None
         self.ProcessAccountGroup = None
         self.ProcessStartAccount = None
         self.ProcessFileAuthority = None
         self.SourceType = None
-        self.PodName = None
         self.Tags = None
         self.HarmDescribe = None
         self.SuggestScheme = None
         self.Mark = None
         self.FileName = None
         self.FileMd5 = None
         self.EventType = None
+        self.PodName = None
         self.Status = None
         self.SubStatus = None
         self.HostIP = None
         self.ClientIP = None
         self.PProcessStartUser = None
         self.PProcessUserGroup = None
         self.PProcessPath = None
@@ -18791,14 +19017,24 @@
         self.OperationTime = None
         self.ContainerNetStatus = None
         self.ContainerNetSubStatus = None
         self.ContainerIsolateOperationSrc = None
         self.CheckPlatform = None
         self.FileAccessTime = None
         self.FileModifyTime = None
+        self.NodeSubNetID = None
+        self.NodeSubNetName = None
+        self.NodeSubNetCIDR = None
+        self.ClusterID = None
+        self.PodIP = None
+        self.PodStatus = None
+        self.NodeUniqueID = None
+        self.NodeType = None
+        self.NodeID = None
+        self.ClusterName = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.ImageId = params.get("ImageId")
         self.ImageName = params.get("ImageName")
         self.CreateTime = params.get("CreateTime")
@@ -18817,22 +19053,22 @@
         self.ProcessId = params.get("ProcessId")
         self.ProcessArgv = params.get("ProcessArgv")
         self.ProcessChan = params.get("ProcessChan")
         self.ProcessAccountGroup = params.get("ProcessAccountGroup")
         self.ProcessStartAccount = params.get("ProcessStartAccount")
         self.ProcessFileAuthority = params.get("ProcessFileAuthority")
         self.SourceType = params.get("SourceType")
-        self.PodName = params.get("PodName")
         self.Tags = params.get("Tags")
         self.HarmDescribe = params.get("HarmDescribe")
         self.SuggestScheme = params.get("SuggestScheme")
         self.Mark = params.get("Mark")
         self.FileName = params.get("FileName")
         self.FileMd5 = params.get("FileMd5")
         self.EventType = params.get("EventType")
+        self.PodName = params.get("PodName")
         self.Status = params.get("Status")
         self.SubStatus = params.get("SubStatus")
         self.HostIP = params.get("HostIP")
         self.ClientIP = params.get("ClientIP")
         self.PProcessStartUser = params.get("PProcessStartUser")
         self.PProcessUserGroup = params.get("PProcessUserGroup")
         self.PProcessPath = params.get("PProcessPath")
@@ -18844,14 +19080,24 @@
         self.OperationTime = params.get("OperationTime")
         self.ContainerNetStatus = params.get("ContainerNetStatus")
         self.ContainerNetSubStatus = params.get("ContainerNetSubStatus")
         self.ContainerIsolateOperationSrc = params.get("ContainerIsolateOperationSrc")
         self.CheckPlatform = params.get("CheckPlatform")
         self.FileAccessTime = params.get("FileAccessTime")
         self.FileModifyTime = params.get("FileModifyTime")
+        self.NodeSubNetID = params.get("NodeSubNetID")
+        self.NodeSubNetName = params.get("NodeSubNetName")
+        self.NodeSubNetCIDR = params.get("NodeSubNetCIDR")
+        self.ClusterID = params.get("ClusterID")
+        self.PodIP = params.get("PodIP")
+        self.PodStatus = params.get("PodStatus")
+        self.NodeUniqueID = params.get("NodeUniqueID")
+        self.NodeType = params.get("NodeType")
+        self.NodeID = params.get("NodeID")
+        self.ClusterName = params.get("ClusterName")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeVirusEventTendencyRequest(AbstractModel):
     """DescribeVirusEventTendency请求参数结构体
 
     """
@@ -19777,15 +20023,19 @@
 
     """
 
     def __init__(self):
         r"""
         :param Filters: 过滤条件。
 <li>Status- String - 是否必填：否 - 插件状态，正常：SUCCESS，异常：FAIL， NO_DEFENCE:未防御</li>
-<li>KeyWords- string - 是否必填：否 - 主机名称/IP。</li>
+<li>HostName- String - 是否必填：否 - 主机名称/超级节点名称</li>
+<li>HostIP- String - 是否必填：否 - 主机IP</li>
+<li>NodeType- String - 是否必填：否 - 节点类型</li>
+<li>HostName- String - 是否必填：否 - 超级节点名称</li>
+<li>NodeSubNetCIDR- String - 是否必填：否 - 超级节点CIDR</li>
         :type Filters: list of RunTimeFilters
         :param Limit: 需要返回的数量，默认为10，最大值为100
         :type Limit: int
         :param Offset: 偏移量，默认为0。
         :type Offset: int
         :param Order: 排序方式：asc/desc
         :type Order: str
@@ -19852,22 +20102,24 @@
 class DescribeVulDefencePluginRequest(AbstractModel):
     """DescribeVulDefencePlugin请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param HostID: 主机HostID即quuid
+        :param HostID: 主机HostID或超级节点UniqueId
         :type HostID: str
         :param Limit: 需要返回的数量，默认为10，最大值为100
         :type Limit: int
         :param Offset: 偏移量，默认为0。
         :type Offset: int
         :param Filters: 过滤条件。
-<li>Status- String - 是否必填：否 -插件运行状态：注入中:INJECTING，注入成功：SUCCESS，注入失败：FAIL，插件超时：TIMEOUT，插件退出：QUIT</li>
+<li>
+Status- String - 是否必填：否 -插件运行状态：注入中:INJECTING，注入成功：SUCCESS，注入失败：FAIL，插件超时：TIMEOUT，插件退出：QUIT
+</li>
         :type Filters: list of RunTimeFilters
         """
         self.HostID = None
         self.Limit = None
         self.Offset = None
         self.Filters = None
 
@@ -19947,35 +20199,55 @@
         :type HostIDs: list of str
         :param HostTotalCount: 开通容器安全的主机总数
 注意：此字段可能返回 null，表示取不到有效值。
         :type HostTotalCount: int
         :param SupportDefenseVulCount: 支持防御的漏洞数
 注意：此字段可能返回 null，表示取不到有效值。
         :type SupportDefenseVulCount: int
+        :param HostNodeCount: 普通节点个数
+        :type HostNodeCount: int
+        :param SuperScope: 超级节点范围
+        :type SuperScope: int
+        :param SuperNodeCount: 超级节点个数
+        :type SuperNodeCount: int
+        :param SuperNodeIds: 超级节点Id列表
+        :type SuperNodeIds: list of str
+        :param NodeTotalCount: 开通容器安全的超级结点总数
+        :type NodeTotalCount: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.IsEnabled = None
         self.Scope = None
         self.HostCount = None
         self.ExceptionHostCount = None
         self.HostIDs = None
         self.HostTotalCount = None
         self.SupportDefenseVulCount = None
+        self.HostNodeCount = None
+        self.SuperScope = None
+        self.SuperNodeCount = None
+        self.SuperNodeIds = None
+        self.NodeTotalCount = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.IsEnabled = params.get("IsEnabled")
         self.Scope = params.get("Scope")
         self.HostCount = params.get("HostCount")
         self.ExceptionHostCount = params.get("ExceptionHostCount")
         self.HostIDs = params.get("HostIDs")
         self.HostTotalCount = params.get("HostTotalCount")
         self.SupportDefenseVulCount = params.get("SupportDefenseVulCount")
+        self.HostNodeCount = params.get("HostNodeCount")
+        self.SuperScope = params.get("SuperScope")
+        self.SuperNodeCount = params.get("SuperNodeCount")
+        self.SuperNodeIds = params.get("SuperNodeIds")
+        self.NodeTotalCount = params.get("NodeTotalCount")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeVulDetailRequest(AbstractModel):
     """DescribeVulDetail请求参数结构体
 
     """
@@ -21087,20 +21359,21 @@
     """容器逃逸事件列表
 
     """
 
     def __init__(self):
         r"""
         :param EventType: 事件类型
-   ESCAPE_HOST_ACESS_FILE:宿主机文件访问逃逸
-   ESCAPE_MOUNT_NAMESPACE:MountNamespace逃逸
-   ESCAPE_PRIVILEDGE:程序提权逃逸
-   ESCAPE_PRIVILEDGE_CONTAINER_START:特权容器启动逃逸
-   ESCAPE_MOUNT_SENSITIVE_PTAH:敏感路径挂载
-   ESCAPE_SYSCALL:Syscall逃逸
+   ESCAPE_CGROUPS：利用cgroup机制逃逸
+   ESCAPE_TAMPER_SENSITIVE_FILE：篡改敏感文件逃逸
+   ESCAPE_DOCKER_API：访问Docker API接口逃逸
+   ESCAPE_VUL_OCCURRED：逃逸漏洞利用
+   MOUNT_SENSITIVE_PTAH：敏感路径挂载
+   PRIVILEGE_CONTAINER_START：特权容器
+   PRIVILEGE：程序提权逃逸
         :type EventType: str
         :param ContainerName: 容器名
         :type ContainerName: str
         :param ImageName: 镜像名
         :type ImageName: str
         :param Status: 状态，EVENT_UNDEAL:未处理，EVENT_DEALED:已处理，EVENT_INGNORE:忽略
         :type Status: str
@@ -21165,14 +21438,30 @@
 暂停: PAUSED
 停止: STOPPED
 已经创建: CREATED
 已经销毁: DESTROYED
 正在重启中: RESTARTING
 迁移中: REMOVING
         :type ContainerStatus: str
+        :param ClusterID: 节点所属集群ID
+        :type ClusterID: str
+        :param NodeType: 节点类型：NORMAL普通节点、SUPER超级节点
+        :type NodeType: str
+        :param PodIP: pod ip
+        :type PodIP: str
+        :param NodeUniqueID: 节点唯一id
+        :type NodeUniqueID: str
+        :param PublicIP: 节点公网ip
+        :type PublicIP: str
+        :param NodeID: 节点id
+        :type NodeID: str
+        :param HostIP: 节点内网ip
+        :type HostIP: str
+        :param ClusterName: 集群名称
+        :type ClusterName: str
         """
         self.EventType = None
         self.ContainerName = None
         self.ImageName = None
         self.Status = None
         self.EventId = None
         self.NodeName = None
@@ -21187,14 +21476,22 @@
         self.LatestFoundTime = None
         self.NodeIP = None
         self.HostID = None
         self.ContainerNetStatus = None
         self.ContainerNetSubStatus = None
         self.ContainerIsolateOperationSrc = None
         self.ContainerStatus = None
+        self.ClusterID = None
+        self.NodeType = None
+        self.PodIP = None
+        self.NodeUniqueID = None
+        self.PublicIP = None
+        self.NodeID = None
+        self.HostIP = None
+        self.ClusterName = None
 
 
     def _deserialize(self, params):
         self.EventType = params.get("EventType")
         self.ContainerName = params.get("ContainerName")
         self.ImageName = params.get("ImageName")
         self.Status = params.get("Status")
@@ -21211,14 +21508,22 @@
         self.LatestFoundTime = params.get("LatestFoundTime")
         self.NodeIP = params.get("NodeIP")
         self.HostID = params.get("HostID")
         self.ContainerNetStatus = params.get("ContainerNetStatus")
         self.ContainerNetSubStatus = params.get("ContainerNetSubStatus")
         self.ContainerIsolateOperationSrc = params.get("ContainerIsolateOperationSrc")
         self.ContainerStatus = params.get("ContainerStatus")
+        self.ClusterID = params.get("ClusterID")
+        self.NodeType = params.get("NodeType")
+        self.PodIP = params.get("PodIP")
+        self.NodeUniqueID = params.get("NodeUniqueID")
+        self.PublicIP = params.get("PublicIP")
+        self.NodeID = params.get("NodeID")
+        self.HostIP = params.get("HostIP")
+        self.ClusterName = params.get("ClusterName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -24499,24 +24804,31 @@
 容器启动: container_launch
 k8sApi: k8s_api
         :type LogType: str
         :param BindList: 绑定主机quuid列表
         :type BindList: list of str
         :param UnBindList: 待解绑主机quuid列表
         :type UnBindList: list of str
+        :param NodeType: 节点类型:
+NORMAL: 普通节点(默认值)
+SUPER: 超级节点
+
+        :type NodeType: str
         """
         self.LogType = None
         self.BindList = None
         self.UnBindList = None
+        self.NodeType = None
 
 
     def _deserialize(self, params):
         self.LogType = params.get("LogType")
         self.BindList = params.get("BindList")
         self.UnBindList = params.get("UnBindList")
+        self.NodeType = params.get("NodeType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -25024,28 +25336,36 @@
 
     """
 
     def __init__(self):
         r"""
         :param IsEnabled: 是否开启:0: 关闭 1:开启
         :type IsEnabled: int
-        :param Scope: 漏洞防御主机范围:0：自选 1: 全部主机。IsEnabled为1时必填
+        :param Scope: 漏洞防御主机范围:0：自选 1: 全部主机
         :type Scope: int
-        :param HostIDs: 自选漏洞防御主机,Scope为0时必填
+        :param HostIDs: 自选漏洞防御主机
         :type HostIDs: list of str
+        :param SuperScope: 漏洞防御超级节点范围:0：自选 1: 全部
+        :type SuperScope: int
+        :param NodeIds: 超级节点Id列表
+        :type NodeIds: list of str
         """
         self.IsEnabled = None
         self.Scope = None
         self.HostIDs = None
+        self.SuperScope = None
+        self.NodeIds = None
 
 
     def _deserialize(self, params):
         self.IsEnabled = params.get("IsEnabled")
         self.Scope = params.get("Scope")
         self.HostIDs = params.get("HostIDs")
+        self.SuperScope = params.get("SuperScope")
+        self.NodeIds = params.get("NodeIds")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -25586,14 +25906,24 @@
         :type ListenHost: str
         :param RunAs: 运行账号
         :type RunAs: str
         :param HostName: 主机名称
         :type HostName: str
         :param PublicIp: 外网ip
         :type PublicIp: str
+        :param NodeID: 节点id
+        :type NodeID: str
+        :param PodIP: podip
+        :type PodIP: str
+        :param PodName: pod名称
+        :type PodName: str
+        :param NodeType: 节点类型
+        :type NodeType: str
+        :param NodeUniqueID: 超级节点唯一id
+        :type NodeUniqueID: str
         """
         self.Type = None
         self.PublicIP = None
         self.PublicPort = None
         self.ContainerPort = None
         self.ContainerPID = None
         self.ContainerName = None
@@ -25601,14 +25931,19 @@
         self.HostIP = None
         self.ProcessName = None
         self.ListenContainer = None
         self.ListenHost = None
         self.RunAs = None
         self.HostName = None
         self.PublicIp = None
+        self.NodeID = None
+        self.PodIP = None
+        self.PodName = None
+        self.NodeType = None
+        self.NodeUniqueID = None
 
 
     def _deserialize(self, params):
         self.Type = params.get("Type")
         self.PublicIP = params.get("PublicIP")
         self.PublicPort = params.get("PublicPort")
         self.ContainerPort = params.get("ContainerPort")
@@ -25618,14 +25953,19 @@
         self.HostIP = params.get("HostIP")
         self.ProcessName = params.get("ProcessName")
         self.ListenContainer = params.get("ListenContainer")
         self.ListenHost = params.get("ListenHost")
         self.RunAs = params.get("RunAs")
         self.HostName = params.get("HostName")
         self.PublicIp = params.get("PublicIp")
+        self.NodeID = params.get("NodeID")
+        self.PodIP = params.get("PodIP")
+        self.PodName = params.get("PodName")
+        self.NodeType = params.get("NodeType")
+        self.NodeUniqueID = params.get("NodeUniqueID")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -25798,27 +26138,42 @@
         :type HostIP: str
         :param ProcessName: 进程名称
         :type ProcessName: str
         :param HostName: 主机名称
         :type HostName: str
         :param PublicIp: 外网ip
         :type PublicIp: str
+        :param NodeID: 节点id
+        :type NodeID: str
+        :param PodIP: podip
+        :type PodIP: str
+        :param PodName: pod名称
+        :type PodName: str
+        :param NodeType: 节点类型
+        :type NodeType: str
+        :param NodeUniqueID: 超级节点唯一id
+        :type NodeUniqueID: str
         """
         self.StartTime = None
         self.RunAs = None
         self.CmdLine = None
         self.Exe = None
         self.PID = None
         self.ContainerPID = None
         self.ContainerName = None
         self.HostID = None
         self.HostIP = None
         self.ProcessName = None
         self.HostName = None
         self.PublicIp = None
+        self.NodeID = None
+        self.PodIP = None
+        self.PodName = None
+        self.NodeType = None
+        self.NodeUniqueID = None
 
 
     def _deserialize(self, params):
         self.StartTime = params.get("StartTime")
         self.RunAs = params.get("RunAs")
         self.CmdLine = params.get("CmdLine")
         self.Exe = params.get("Exe")
@@ -25826,14 +26181,19 @@
         self.ContainerPID = params.get("ContainerPID")
         self.ContainerName = params.get("ContainerName")
         self.HostID = params.get("HostID")
         self.HostIP = params.get("HostIP")
         self.ProcessName = params.get("ProcessName")
         self.HostName = params.get("HostName")
         self.PublicIp = params.get("PublicIp")
+        self.NodeID = params.get("NodeID")
+        self.PodIP = params.get("PodIP")
+        self.PodName = params.get("PodName")
+        self.NodeType = params.get("NodeType")
+        self.NodeUniqueID = params.get("NodeUniqueID")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -26463,14 +26823,32 @@
 暂停: PAUSED
 停止: STOPPED
 已经创建: CREATED
 已经销毁: DESTROYED
 正在重启中: RESTARTING
 迁移中: REMOVING
         :type ContainerStatus: str
+        :param NodeType: 节点类型：NORMAL普通节点、SUPER超级节点
+        :type NodeType: str
+        :param ClusterID: 集群I'D
+        :type ClusterID: str
+        :param PodIP: pod ip
+        :type PodIP: str
+        :param NodeUniqueID: 节点唯一id
+        :type NodeUniqueID: str
+        :param PublicIP: 节点公网ip
+        :type PublicIP: str
+        :param NodeID: 节点id
+        :type NodeID: str
+        :param HostID: uuid
+        :type HostID: str
+        :param HostIP: 节点内网ip
+        :type HostIP: str
+        :param ClusterName: 集群名称
+        :type ClusterName: str
         """
         self.ProcessName = None
         self.ProcessPath = None
         self.ImageId = None
         self.ContainerId = None
         self.ImageName = None
         self.ContainerName = None
@@ -26486,14 +26864,23 @@
         self.RuleExist = None
         self.EventCount = None
         self.LatestFoundTime = None
         self.ContainerNetStatus = None
         self.ContainerNetSubStatus = None
         self.ContainerIsolateOperationSrc = None
         self.ContainerStatus = None
+        self.NodeType = None
+        self.ClusterID = None
+        self.PodIP = None
+        self.NodeUniqueID = None
+        self.PublicIP = None
+        self.NodeID = None
+        self.HostID = None
+        self.HostIP = None
+        self.ClusterName = None
 
 
     def _deserialize(self, params):
         self.ProcessName = params.get("ProcessName")
         self.ProcessPath = params.get("ProcessPath")
         self.ImageId = params.get("ImageId")
         self.ContainerId = params.get("ContainerId")
@@ -26511,14 +26898,23 @@
         self.RuleExist = params.get("RuleExist")
         self.EventCount = params.get("EventCount")
         self.LatestFoundTime = params.get("LatestFoundTime")
         self.ContainerNetStatus = params.get("ContainerNetStatus")
         self.ContainerNetSubStatus = params.get("ContainerNetSubStatus")
         self.ContainerIsolateOperationSrc = params.get("ContainerIsolateOperationSrc")
         self.ContainerStatus = params.get("ContainerStatus")
+        self.NodeType = params.get("NodeType")
+        self.ClusterID = params.get("ClusterID")
+        self.PodIP = params.get("PodIP")
+        self.NodeUniqueID = params.get("NodeUniqueID")
+        self.PublicIP = params.get("PublicIP")
+        self.NodeID = params.get("NodeID")
+        self.HostID = params.get("HostID")
+        self.HostIP = params.get("HostIP")
+        self.ClusterName = params.get("ClusterName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -26678,16 +27074,14 @@
         :type ContainerName: str
         :param ImageId: 镜像id
         :type ImageId: str
         :param ImageName: 镜像名称
         :type ImageName: str
         :param NodeName: 节点名称
         :type NodeName: str
-        :param PodName: Pod名称
-        :type PodName: str
         :param Status: 状态， “EVENT_UNDEAL”:事件未处理
     "EVENT_DEALED":事件已经处理
     "EVENT_INGNORE"：事件已经忽略
         :type Status: str
         :param EventName: 事件名称：
 宿主机文件访问逃逸、
 Syscall逃逸、
@@ -26734,54 +27128,100 @@
 "RESOURCE_LIMIT"      //隔离操作资源超限
 "UNKNOW"              // 原因未知
 注意：此字段可能返回 null，表示取不到有效值。
         :type ContainerNetSubStatus: str
         :param ContainerIsolateOperationSrc: 容器隔离操作来源
 注意：此字段可能返回 null，表示取不到有效值。
         :type ContainerIsolateOperationSrc: str
+        :param NodeID: 节点ID
+        :type NodeID: str
+        :param NodeType: 节点类型:NORMAL:普通节点;SUPER:超级节点
+        :type NodeType: str
+        :param NodeSubNetID: 节点子网ID
+        :type NodeSubNetID: str
+        :param NodeSubNetName: 节点子网名称
+        :type NodeSubNetName: str
+        :param NodeSubNetCIDR: 节点子网网段
+        :type NodeSubNetCIDR: str
+        :param PodName: pod名称
+        :type PodName: str
+        :param PodIP: podIP
+        :type PodIP: str
+        :param PodStatus: pod状态
+        :type PodStatus: str
+        :param ClusterID: 集群id
+        :type ClusterID: str
+        :param ClusterName: 集群名称
+        :type ClusterName: str
+        :param NodeUniqueID: 节点唯一id
+        :type NodeUniqueID: str
+        :param HostID: uuid
+        :type HostID: str
         """
         self.EventId = None
         self.FoundTime = None
         self.ContainerId = None
         self.ContainerName = None
         self.ImageId = None
         self.ImageName = None
         self.NodeName = None
-        self.PodName = None
         self.Status = None
         self.EventName = None
         self.EventType = None
         self.EventCount = None
         self.LatestFoundTime = None
         self.HostIP = None
         self.ClientIP = None
         self.ContainerNetStatus = None
         self.ContainerNetSubStatus = None
         self.ContainerIsolateOperationSrc = None
+        self.NodeID = None
+        self.NodeType = None
+        self.NodeSubNetID = None
+        self.NodeSubNetName = None
+        self.NodeSubNetCIDR = None
+        self.PodName = None
+        self.PodIP = None
+        self.PodStatus = None
+        self.ClusterID = None
+        self.ClusterName = None
+        self.NodeUniqueID = None
+        self.HostID = None
 
 
     def _deserialize(self, params):
         self.EventId = params.get("EventId")
         self.FoundTime = params.get("FoundTime")
         self.ContainerId = params.get("ContainerId")
         self.ContainerName = params.get("ContainerName")
         self.ImageId = params.get("ImageId")
         self.ImageName = params.get("ImageName")
         self.NodeName = params.get("NodeName")
-        self.PodName = params.get("PodName")
         self.Status = params.get("Status")
         self.EventName = params.get("EventName")
         self.EventType = params.get("EventType")
         self.EventCount = params.get("EventCount")
         self.LatestFoundTime = params.get("LatestFoundTime")
         self.HostIP = params.get("HostIP")
         self.ClientIP = params.get("ClientIP")
         self.ContainerNetStatus = params.get("ContainerNetStatus")
         self.ContainerNetSubStatus = params.get("ContainerNetSubStatus")
         self.ContainerIsolateOperationSrc = params.get("ContainerIsolateOperationSrc")
+        self.NodeID = params.get("NodeID")
+        self.NodeType = params.get("NodeType")
+        self.NodeSubNetID = params.get("NodeSubNetID")
+        self.NodeSubNetName = params.get("NodeSubNetName")
+        self.NodeSubNetCIDR = params.get("NodeSubNetCIDR")
+        self.PodName = params.get("PodName")
+        self.PodIP = params.get("PodIP")
+        self.PodStatus = params.get("PodStatus")
+        self.ClusterID = params.get("ClusterID")
+        self.ClusterName = params.get("ClusterName")
+        self.NodeUniqueID = params.get("NodeUniqueID")
+        self.HostID = params.get("HostID")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -27288,32 +27728,36 @@
 class SecLogJoinInfo(AbstractModel):
     """安全日志接入详情
 
     """
 
     def __init__(self):
         r"""
-        :param Count: 已接入数量
+        :param Count: 已接入普通主机数量
         :type Count: int
+        :param SuperNodeCount: 已接入超级节点数量
+        :type SuperNodeCount: int
         :param IsJoined: 是否已接入(true:已接入 false:未接入)
         :type IsJoined: bool
         :param LogType: 日志类型(
 容器bash:  "container_bash"
 容器启动: "container_launch"
 k8sApi: "k8s_api"
 )
         :type LogType: str
         """
         self.Count = None
+        self.SuperNodeCount = None
         self.IsJoined = None
         self.LogType = None
 
 
     def _deserialize(self, params):
         self.Count = params.get("Count")
+        self.SuperNodeCount = params.get("SuperNodeCount")
         self.IsJoined = params.get("IsJoined")
         self.LogType = params.get("LogType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
@@ -27472,14 +27916,24 @@
         :type Parameter: str
         :param ContainerId: 容器id
         :type ContainerId: str
         :param HostName: 主机名称
         :type HostName: str
         :param PublicIp: 外网ip
         :type PublicIp: str
+        :param NodeID: 节点id
+        :type NodeID: str
+        :param PodIP: podip
+        :type PodIP: str
+        :param PodName: pod名称
+        :type PodName: str
+        :param NodeType: 节点类型
+        :type NodeType: str
+        :param NodeUniqueID: 超级节点唯一id
+        :type NodeUniqueID: str
         """
         self.ServiceID = None
         self.HostID = None
         self.HostIP = None
         self.ContainerName = None
         self.Type = None
         self.Version = None
@@ -27494,14 +27948,19 @@
         self.Pids = None
         self.MainType = None
         self.Exe = None
         self.Parameter = None
         self.ContainerId = None
         self.HostName = None
         self.PublicIp = None
+        self.NodeID = None
+        self.PodIP = None
+        self.PodName = None
+        self.NodeType = None
+        self.NodeUniqueID = None
 
 
     def _deserialize(self, params):
         self.ServiceID = params.get("ServiceID")
         self.HostID = params.get("HostID")
         self.HostIP = params.get("HostIP")
         self.ContainerName = params.get("ContainerName")
@@ -27518,14 +27977,19 @@
         self.Pids = params.get("Pids")
         self.MainType = params.get("MainType")
         self.Exe = params.get("Exe")
         self.Parameter = params.get("Parameter")
         self.ContainerId = params.get("ContainerId")
         self.HostName = params.get("HostName")
         self.PublicIp = params.get("PublicIp")
+        self.NodeID = params.get("NodeID")
+        self.PodIP = params.get("PodIP")
+        self.PodName = params.get("PodName")
+        self.NodeType = params.get("NodeType")
+        self.NodeUniqueID = params.get("NodeUniqueID")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -28486,14 +28950,36 @@
 1: 云查杀引擎
 2: tav
 3: binaryAi
 4: 异常行为
 5: 威胁情报
 注意：此字段可能返回 null，表示取不到有效值。
         :type CheckPlatform: list of str
+        :param NodeID: 节点ID
+        :type NodeID: str
+        :param NodeName: 节点名称
+        :type NodeName: str
+        :param PodIP: pod ip
+        :type PodIP: str
+        :param PodName: pod(实例)的名字
+        :type PodName: str
+        :param ClusterID: 节点所属集群ID
+        :type ClusterID: str
+        :param NodeType: 节点类型：NORMAL普通节点、SUPER超级节点
+        :type NodeType: str
+        :param PublicIP: 节点外网IP
+        :type PublicIP: str
+        :param InnerIP: 节点内网IP
+        :type InnerIP: str
+        :param NodeUniqueID: 节点唯一ID
+        :type NodeUniqueID: str
+        :param HostID: 普通节点ID
+        :type HostID: str
+        :param ClusterName: 集群名称
+        :type ClusterName: str
         """
         self.FileName = None
         self.FilePath = None
         self.VirusName = None
         self.CreateTime = None
         self.ModifyTime = None
         self.ContainerName = None
@@ -28508,14 +28994,25 @@
         self.SubStatus = None
         self.ContainerNetStatus = None
         self.ContainerNetSubStatus = None
         self.ContainerIsolateOperationSrc = None
         self.MD5 = None
         self.RiskLevel = None
         self.CheckPlatform = None
+        self.NodeID = None
+        self.NodeName = None
+        self.PodIP = None
+        self.PodName = None
+        self.ClusterID = None
+        self.NodeType = None
+        self.PublicIP = None
+        self.InnerIP = None
+        self.NodeUniqueID = None
+        self.HostID = None
+        self.ClusterName = None
 
 
     def _deserialize(self, params):
         self.FileName = params.get("FileName")
         self.FilePath = params.get("FilePath")
         self.VirusName = params.get("VirusName")
         self.CreateTime = params.get("CreateTime")
@@ -28532,14 +29029,25 @@
         self.SubStatus = params.get("SubStatus")
         self.ContainerNetStatus = params.get("ContainerNetStatus")
         self.ContainerNetSubStatus = params.get("ContainerNetSubStatus")
         self.ContainerIsolateOperationSrc = params.get("ContainerIsolateOperationSrc")
         self.MD5 = params.get("MD5")
         self.RiskLevel = params.get("RiskLevel")
         self.CheckPlatform = params.get("CheckPlatform")
+        self.NodeID = params.get("NodeID")
+        self.NodeName = params.get("NodeName")
+        self.PodIP = params.get("PodIP")
+        self.PodName = params.get("PodName")
+        self.ClusterID = params.get("ClusterID")
+        self.NodeType = params.get("NodeType")
+        self.PublicIP = params.get("PublicIP")
+        self.InnerIP = params.get("InnerIP")
+        self.NodeUniqueID = params.get("NodeUniqueID")
+        self.HostID = params.get("HostID")
+        self.ClusterName = params.get("ClusterName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -28556,17 +29064,17 @@
         :type ContainerName: str
         :param ContainerId: 容器id
         :type ContainerId: str
         :param ImageName: 镜像名称
         :type ImageName: str
         :param ImageId: 镜像Id
         :type ImageId: str
-        :param HostName: 主机名称
+        :param HostName: 节点名
         :type HostName: str
-        :param HostIp: 主机ip
+        :param HostIp: 节点内网ip
         :type HostIp: str
         :param Status: 扫描状态：
 WAIT: 等待扫描
 FAILED: 失败
 SCANNING: 扫描中
 FINISHED: 结束
 CANCELING: 取消中
@@ -28592,27 +29100,36 @@
 TOO_MANY: 任务过多
 VALIDATION: 参数非法
 INTERNAL: 服务内部错误
 MISC: 其他错误
 UNAUTH: 所在镜像未授权
 SEND_CANCEL_SUCCESSED:下发成功
         :type ErrorMsg: str
+        :param NodeType: 节点类型：NORMAL普通节点、SUPER超级节点
+        :type NodeType: str
+        :param PublicIP: 节点外网IP
+        :type PublicIP: str
+        :param NodeID: 节点ID
+        :type NodeID: str
         """
         self.ContainerName = None
         self.ContainerId = None
         self.ImageName = None
         self.ImageId = None
         self.HostName = None
         self.HostIp = None
         self.Status = None
         self.StartTime = None
         self.EndTime = None
         self.RiskCnt = None
         self.Id = None
         self.ErrorMsg = None
+        self.NodeType = None
+        self.PublicIP = None
+        self.NodeID = None
 
 
     def _deserialize(self, params):
         self.ContainerName = params.get("ContainerName")
         self.ContainerId = params.get("ContainerId")
         self.ImageName = params.get("ImageName")
         self.ImageId = params.get("ImageId")
@@ -28620,14 +29137,17 @@
         self.HostIp = params.get("HostIp")
         self.Status = params.get("Status")
         self.StartTime = params.get("StartTime")
         self.EndTime = params.get("EndTime")
         self.RiskCnt = params.get("RiskCnt")
         self.Id = params.get("Id")
         self.ErrorMsg = params.get("ErrorMsg")
+        self.NodeType = params.get("NodeType")
+        self.PublicIP = params.get("PublicIP")
+        self.NodeID = params.get("NodeID")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -28727,34 +29247,58 @@
         :type PodIP: str
         :param HostName: 主机名称
         :type HostName: str
         :param HostID: 主机ID
         :type HostID: str
         :param PublicIP: 外网IP
         :type PublicIP: str
+        :param ClusterID: 集群ID
+        :type ClusterID: str
+        :param ClusterName: 集群名称
+        :type ClusterName: str
+        :param NodeType: 节点类型[NORMAL:普通节点|SUPER:超级节点]
+        :type NodeType: str
+        :param NodeUniqueID: 超级节点唯一ID
+        :type NodeUniqueID: str
+        :param NodeID: 超级节点ID
+        :type NodeID: str
+        :param NodeName: 超级节点名称
+        :type NodeName: str
         """
         self.HostIP = None
         self.ContainerID = None
         self.ContainerName = None
         self.PodName = None
         self.PodIP = None
         self.HostName = None
         self.HostID = None
         self.PublicIP = None
+        self.ClusterID = None
+        self.ClusterName = None
+        self.NodeType = None
+        self.NodeUniqueID = None
+        self.NodeID = None
+        self.NodeName = None
 
 
     def _deserialize(self, params):
         self.HostIP = params.get("HostIP")
         self.ContainerID = params.get("ContainerID")
         self.ContainerName = params.get("ContainerName")
         self.PodName = params.get("PodName")
         self.PodIP = params.get("PodIP")
         self.HostName = params.get("HostName")
         self.HostID = params.get("HostID")
         self.PublicIP = params.get("PublicIP")
+        self.ClusterID = params.get("ClusterID")
+        self.ClusterName = params.get("ClusterName")
+        self.NodeType = params.get("NodeType")
+        self.NodeUniqueID = params.get("NodeUniqueID")
+        self.NodeID = params.get("NodeID")
+        self.NodeName = params.get("NodeName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -28911,23 +29455,35 @@
 	"RESOURCE_LIMIT"      //隔离操作资源超限
 	"UNKNOW"              // 原因未知
 注意：此字段可能返回 null，表示取不到有效值。
         :type ContainerNetSubStatus: str
         :param ContainerIsolateOperationSrc: 容器隔离操作来源
 注意：此字段可能返回 null，表示取不到有效值。
         :type ContainerIsolateOperationSrc: str
-        :param QUUID: 主机QUUID
+        :param QUUID: 主机QUUID/超级节点ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type QUUID: str
         :param HostIP: 主机内网IP
 注意：此字段可能返回 null，表示取不到有效值。
         :type HostIP: str
-        :param HostName: 主机名称
+        :param HostName: 主机名称/超级节点名称
 注意：此字段可能返回 null，表示取不到有效值。
         :type HostName: str
+        :param NodeType: 节点类型[NORMAL:普通节点|SUPER:超级节点]
+        :type NodeType: str
+        :param PublicIP: 外网IP
+        :type PublicIP: str
+        :param NodeUniqueID: 超级节点唯一ID
+        :type NodeUniqueID: str
+        :param NodeID: 超级节点ID
+        :type NodeID: str
+        :param ClusterID: 集群ID
+        :type ClusterID: str
+        :param ClusterName: 集群名称
+        :type ClusterName: str
         """
         self.CVEID = None
         self.VulName = None
         self.PocID = None
         self.EventType = None
         self.SourceIP = None
         self.City = None
@@ -28943,14 +29499,20 @@
         self.MergeTime = None
         self.ContainerStatus = None
         self.ContainerNetSubStatus = None
         self.ContainerIsolateOperationSrc = None
         self.QUUID = None
         self.HostIP = None
         self.HostName = None
+        self.NodeType = None
+        self.PublicIP = None
+        self.NodeUniqueID = None
+        self.NodeID = None
+        self.ClusterID = None
+        self.ClusterName = None
 
 
     def _deserialize(self, params):
         self.CVEID = params.get("CVEID")
         self.VulName = params.get("VulName")
         self.PocID = params.get("PocID")
         self.EventType = params.get("EventType")
@@ -28968,14 +29530,20 @@
         self.MergeTime = params.get("MergeTime")
         self.ContainerStatus = params.get("ContainerStatus")
         self.ContainerNetSubStatus = params.get("ContainerNetSubStatus")
         self.ContainerIsolateOperationSrc = params.get("ContainerIsolateOperationSrc")
         self.QUUID = params.get("QUUID")
         self.HostIP = params.get("HostIP")
         self.HostName = params.get("HostName")
+        self.NodeType = params.get("NodeType")
+        self.PublicIP = params.get("PublicIP")
+        self.NodeUniqueID = params.get("NodeUniqueID")
+        self.NodeID = params.get("NodeID")
+        self.ClusterID = params.get("ClusterID")
+        self.ClusterName = params.get("ClusterName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -29012,15 +29580,15 @@
         :type ImageName: str
         :param Status: 处理状态
         :type Status: str
         :param SourcePort: 攻击源端口
         :type SourcePort: list of str
         :param EventID: 事件ID
         :type EventID: int
-        :param HostName: 主机名称
+        :param HostName: 主机名称/超级节点名称
         :type HostName: str
         :param HostIP: 主机内网IP
         :type HostIP: str
         :param PublicIP: 主机外网IP
         :type PublicIP: str
         :param PodName: Pod名称
         :type PodName: str
@@ -29047,15 +29615,15 @@
         :type ServerPort: str
         :param ServerExe: 进程路径
 注意：此字段可能返回 null，表示取不到有效值。
         :type ServerExe: str
         :param ServerArg: 进程命令行参数
 注意：此字段可能返回 null，表示取不到有效值。
         :type ServerArg: str
-        :param QUUID: 主机QUUID
+        :param QUUID: 主机QUUID/超级节点ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type QUUID: str
         :param ContainerNetStatus: 隔离状态
 未隔离  	NORMAL
 已隔离		ISOLATED
 隔离中		ISOLATING
 隔离失败	ISOLATE_FAILED
@@ -29088,14 +29656,32 @@
         :type ContainerStatus: str
         :param JNDIUrl: 接口Url
 注意：此字段可能返回 null，表示取不到有效值。
         :type JNDIUrl: str
         :param RaspDetail: rasp detail
 注意：此字段可能返回 null，表示取不到有效值。
         :type RaspDetail: list of RaspInfo
+        :param NodeSubNetName: 超级节点子网名称
+        :type NodeSubNetName: str
+        :param NodeSubNetCIDR: 超级节点子网网段
+        :type NodeSubNetCIDR: str
+        :param PodIP: pod ip
+        :type PodIP: str
+        :param NodeType: 节点类型[NORMAL:普通节点|SUPER:超级节点]
+        :type NodeType: str
+        :param NodeID: 超级节点ID
+        :type NodeID: str
+        :param NodeUniqueID: 超级节点唯一ID
+        :type NodeUniqueID: str
+        :param NodeSubNetID: 超级节点子网ID
+        :type NodeSubNetID: str
+        :param ClusterID: 集群ID
+        :type ClusterID: str
+        :param ClusterName: 集群名称
+        :type ClusterName: str
         """
         self.CVEID = None
         self.VulName = None
         self.PocID = None
         self.EventType = None
         self.SourceIP = None
         self.City = None
@@ -29124,14 +29710,23 @@
         self.QUUID = None
         self.ContainerNetStatus = None
         self.ContainerNetSubStatus = None
         self.ContainerIsolateOperationSrc = None
         self.ContainerStatus = None
         self.JNDIUrl = None
         self.RaspDetail = None
+        self.NodeSubNetName = None
+        self.NodeSubNetCIDR = None
+        self.PodIP = None
+        self.NodeType = None
+        self.NodeID = None
+        self.NodeUniqueID = None
+        self.NodeSubNetID = None
+        self.ClusterID = None
+        self.ClusterName = None
 
 
     def _deserialize(self, params):
         self.CVEID = params.get("CVEID")
         self.VulName = params.get("VulName")
         self.PocID = params.get("PocID")
         self.EventType = params.get("EventType")
@@ -29167,14 +29762,23 @@
         self.JNDIUrl = params.get("JNDIUrl")
         if params.get("RaspDetail") is not None:
             self.RaspDetail = []
             for item in params.get("RaspDetail"):
                 obj = RaspInfo()
                 obj._deserialize(item)
                 self.RaspDetail.append(obj)
+        self.NodeSubNetName = params.get("NodeSubNetName")
+        self.NodeSubNetCIDR = params.get("NodeSubNetCIDR")
+        self.PodIP = params.get("PodIP")
+        self.NodeType = params.get("NodeType")
+        self.NodeID = params.get("NodeID")
+        self.NodeUniqueID = params.get("NodeUniqueID")
+        self.NodeSubNetID = params.get("NodeSubNetID")
+        self.ClusterID = params.get("ClusterID")
+        self.ClusterName = params.get("ClusterName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -29211,46 +29815,78 @@
 class VulDefenceHost(AbstractModel):
     """漏洞防御的主机信息
 
     """
 
     def __init__(self):
         r"""
-        :param HostName: 主机名称
+        :param HostName: 主机名称/超级节点名称
         :type HostName: str
         :param HostIP: 主机ip即内网ip
         :type HostIP: str
-        :param HostID: 主机QUUID
+        :param HostID: 主机QUUID/超级节点ID
         :type HostID: str
         :param Status: 插件状态，正常：SUCCESS，异常：FAIL， NO_DEFENDED:未防御
         :type Status: str
         :param PublicIP: 外网ip
         :type PublicIP: str
         :param CreateTime: 首次开启时间
         :type CreateTime: str
         :param ModifyTime: 更新时间
         :type ModifyTime: str
+        :param NodeType: 节点类型[NORMAL:普通节点|SUPER:超级节点]
+        :type NodeType: str
+        :param NodeSubNetName: 超级节点子网名称
+        :type NodeSubNetName: str
+        :param NodeSubNetCIDR: 超级节点子网网段
+        :type NodeSubNetCIDR: str
+        :param NodeSubNetID: 超级节点子网ID
+        :type NodeSubNetID: str
+        :param NodeUniqueID: 超级节点唯一ID
+        :type NodeUniqueID: str
+        :param NodeID: 超级节点ID
+        :type NodeID: str
+        :param PodIP: Pod Ip
+        :type PodIP: str
+        :param PodName: Pod 名称
+        :type PodName: str
         """
         self.HostName = None
         self.HostIP = None
         self.HostID = None
         self.Status = None
         self.PublicIP = None
         self.CreateTime = None
         self.ModifyTime = None
+        self.NodeType = None
+        self.NodeSubNetName = None
+        self.NodeSubNetCIDR = None
+        self.NodeSubNetID = None
+        self.NodeUniqueID = None
+        self.NodeID = None
+        self.PodIP = None
+        self.PodName = None
 
 
     def _deserialize(self, params):
         self.HostName = params.get("HostName")
         self.HostIP = params.get("HostIP")
         self.HostID = params.get("HostID")
         self.Status = params.get("Status")
         self.PublicIP = params.get("PublicIP")
         self.CreateTime = params.get("CreateTime")
         self.ModifyTime = params.get("ModifyTime")
+        self.NodeType = params.get("NodeType")
+        self.NodeSubNetName = params.get("NodeSubNetName")
+        self.NodeSubNetCIDR = params.get("NodeSubNetCIDR")
+        self.NodeSubNetID = params.get("NodeSubNetID")
+        self.NodeUniqueID = params.get("NodeUniqueID")
+        self.NodeID = params.get("NodeID")
+        self.PodIP = params.get("PodIP")
+        self.PodName = params.get("PodName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.894/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcss-3.0.895/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcss
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Tcss SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.894/PKG-INFO` & `tencentcloud-sdk-python-tcss-3.0.895/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcss
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Tcss SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.894/setup.py` & `tencentcloud-sdk-python-tcss-3.0.895/setup.py`

 * *Files identical despite different names*

