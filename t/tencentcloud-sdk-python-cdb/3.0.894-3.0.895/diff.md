# Comparing `tmp/tencentcloud-sdk-python-cdb-3.0.894.tar.gz` & `tmp/tencentcloud-sdk-python-cdb-3.0.895.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.894.tar", last modified: Thu May 18 00:19:21 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.895.tar", last modified: Fri May 19 02:44:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdb-3.0.894.tar` & `tencentcloud-sdk-python-cdb-3.0.895.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/cdb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/cdb/v20170320/
--rw-r--r--   0 root         (0) root         (0)   151787 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/cdb/v20170320/cdb_client.py
--rw-r--r--   0 root         (0) root         (0)    18943 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/cdb/v20170320/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/cdb/v20170320/__init__.py
--rw-r--r--   0 root         (0) root         (0)   529181 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/cdb/v20170320/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/cdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud_sdk_python_cdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.894/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/cdb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/cdb/v20170320/
+-rw-r--r--   0 root         (0) root         (0)   151870 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/cdb/v20170320/cdb_client.py
+-rw-r--r--   0 root         (0) root         (0)    18943 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/cdb/v20170320/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/cdb/v20170320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   529193 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/cdb/v20170320/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/cdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud_sdk_python_cdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.894/README.rst` & `tencentcloud-sdk-python-cdb-3.0.895/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/cdb/v20170320/cdb_client.py` & `tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/cdb/v20170320/cdb_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -939,15 +939,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeBackupDatabases(self, request):
-        """本接口(DescribeBackupDatabases)用于查询备份文件包含的库 (已废弃)。
+        """接口已废弃，需要下线
+
+        本接口(DescribeBackupDatabases)用于查询备份文件包含的库 (已废弃)。
         旧版本支持全量备份后，用户如果分库表下载逻辑备份文件，需要用到此接口。
         新版本支持(CreateBackup)创建逻辑备份的时候，直接发起指定库表备份，用户直接下载该备份文件即可。
 
         :param request: Request instance for DescribeBackupDatabases.
         :type request: :class:`tencentcloud.cdb.v20170320.models.DescribeBackupDatabasesRequest`
         :rtype: :class:`tencentcloud.cdb.v20170320.models.DescribeBackupDatabasesResponse`
 
@@ -1079,15 +1081,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeBackupTables(self, request):
-        """本接口(DescribeBackupTables)用于查询指定的数据库的备份数据表名 (已废弃)。
+        """该接口已废弃，需要下线
+
+        本接口(DescribeBackupTables)用于查询指定的数据库的备份数据表名 (已废弃)。
         旧版本支持全量备份后，用户如果分库表下载逻辑备份文件，需要用到此接口。
         新版本支持(CreateBackup)创建逻辑备份的时候，直接发起指定库表备份，用户直接下载该备份文件即可。
 
         :param request: Request instance for DescribeBackupTables.
         :type request: :class:`tencentcloud.cdb.v20170320.models.DescribeBackupTablesRequest`
         :rtype: :class:`tencentcloud.cdb.v20170320.models.DescribeBackupTablesResponse`
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/cdb/v20170320/errorcodes.py` & `tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/cdb/v20170320/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/cdb/v20170320/models.py` & `tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/cdb/v20170320/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5992,15 +5992,15 @@
         :type Volume: int
         :param InstanceRole: 实例类型，默认为 master，支持值包括：master - 表示主实例，ro - 表示只读实例，dr - 表示灾备实例。InstanceId为空时该参数为必填项。
         :type InstanceRole: str
         :param PayType: 付费类型，支持值包括：PRE_PAID - 包年包月，HOUR_PAID - 按量计费。InstanceId为空时该参数为必填项。
         :type PayType: str
         :param ProtectMode: 数据复制方式，默认为 0，支持值包括：0 - 表示异步复制，1 - 表示半同步复制，2 - 表示强同步复制。
         :type ProtectMode: int
-        :param DeviceType: 实例隔离类型。支持值包括： "UNIVERSAL" - 通用型实例， "EXCLUSIVE" - 独享型实例， "BASIC" - 基础版实例。 不指定则默认为通用型实例。
+        :param DeviceType: 实例隔离类型。支持值包括： "UNIVERSAL" - 通用型实例， "EXCLUSIVE" - 独享型实例， "BASIC_V2" - 单节点云盘版实例。 不指定则默认为通用型实例。
         :type DeviceType: str
         :param InstanceNodes: 实例节点数。对于 RO 和 基础版实例， 该值默认为1。 如果需要询价三节点实例， 请将该值设置为3。其余主实例该值默认为2。
         :type InstanceNodes: int
         :param Cpu: 询价实例的CPU核心数目，单位：核，为保证传入 CPU 值有效，请使用 [获取云数据库可售卖规格](https://cloud.tencent.com/document/product/236/17229) 接口获取可售卖的核心数目，当未指定该值时，将按照 Memory 大小补全一个默认值。
         :type Cpu: int
         :param InstanceId: 询价续费实例ID。如需查询实例续费价格，填写InstanceId和Period即可。
         :type InstanceId: str
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.894/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdb-3.0.894/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.895/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.894/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.895/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.894/setup.py` & `tencentcloud-sdk-python-cdb-3.0.895/setup.py`

 * *Files identical despite different names*

