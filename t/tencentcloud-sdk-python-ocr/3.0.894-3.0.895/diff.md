# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.894.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.895.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.894.tar", last modified: Thu May 18 00:32:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.895.tar", last modified: Fri May 19 02:56:38 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.894.tar` & `tencentcloud-sdk-python-ocr-3.0.895.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/ocr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)   113504 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)     5764 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)   505442 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/ocr/v20181119/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/ocr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:32:57.000000 tencentcloud-sdk-python-ocr-3.0.894/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:56:38.000000 tencentcloud-sdk-python-ocr-3.0.895/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:56:38.000000 tencentcloud-sdk-python-ocr-3.0.895/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 02:56:38.000000 tencentcloud-sdk-python-ocr-3.0.895/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-19 02:56:38.000000 tencentcloud-sdk-python-ocr-3.0.895/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 02:56:38.000000 tencentcloud-sdk-python-ocr-3.0.895/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 02:56:38.000000 tencentcloud-sdk-python-ocr-3.0.895/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-19 02:56:38.000000 tencentcloud-sdk-python-ocr-3.0.895/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:56:38.000000 tencentcloud-sdk-python-ocr-3.0.895/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:56:38.000000 tencentcloud-sdk-python-ocr-3.0.895/tencentcloud/ocr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:56:38.000000 tencentcloud-sdk-python-ocr-3.0.895/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)   113504 2023-05-19 02:56:38.000000 tencentcloud-sdk-python-ocr-3.0.895/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)     5764 2023-05-19 02:56:38.000000 tencentcloud-sdk-python-ocr-3.0.895/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:56:38.000000 tencentcloud-sdk-python-ocr-3.0.895/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   505665 2023-05-19 02:56:38.000000 tencentcloud-sdk-python-ocr-3.0.895/tencentcloud/ocr/v20181119/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:56:38.000000 tencentcloud-sdk-python-ocr-3.0.895/tencentcloud/ocr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-19 02:56:38.000000 tencentcloud-sdk-python-ocr-3.0.895/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 02:56:38.000000 tencentcloud-sdk-python-ocr-3.0.895/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-19 02:56:38.000000 tencentcloud-sdk-python-ocr-3.0.895/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-19 02:56:38.000000 tencentcloud-sdk-python-ocr-3.0.895/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.894/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.895/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.894/README.rst` & `tencentcloud-sdk-python-ocr-3.0.895/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.895/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.895/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.895/tencentcloud/ocr/v20181119/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -9886,38 +9886,43 @@
         :type Marks: str
         :param Record: 检验记录
 注意：此字段可能返回 null，表示取不到有效值。
         :type Record: str
         :param TotalQuasiMass: 准牵引总质量
 注意：此字段可能返回 null，表示取不到有效值。
         :type TotalQuasiMass: str
+        :param SubPageCode: 副页编码
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SubPageCode: str
         """
         self.PlateNo = None
         self.FileNo = None
         self.AllowNum = None
         self.TotalMass = None
         self.CurbWeight = None
         self.LoadQuality = None
         self.ExternalSize = None
         self.Marks = None
         self.Record = None
         self.TotalQuasiMass = None
+        self.SubPageCode = None
 
 
     def _deserialize(self, params):
         self.PlateNo = params.get("PlateNo")
         self.FileNo = params.get("FileNo")
         self.AllowNum = params.get("AllowNum")
         self.TotalMass = params.get("TotalMass")
         self.CurbWeight = params.get("CurbWeight")
         self.LoadQuality = params.get("LoadQuality")
         self.ExternalSize = params.get("ExternalSize")
         self.Marks = params.get("Marks")
         self.Record = params.get("Record")
         self.TotalQuasiMass = params.get("TotalQuasiMass")
+        self.SubPageCode = params.get("SubPageCode")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.894/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.895/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.894/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.895/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.894/setup.py` & `tencentcloud-sdk-python-ocr-3.0.895/setup.py`

 * *Files identical despite different names*

