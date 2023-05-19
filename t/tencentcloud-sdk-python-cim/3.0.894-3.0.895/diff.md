# Comparing `tmp/tencentcloud-sdk-python-cim-3.0.894.tar.gz` & `tmp/tencentcloud-sdk-python-cim-3.0.895.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cim-3.0.894.tar", last modified: Thu May 18 00:20:54 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cim-3.0.895.tar", last modified: Fri May 19 02:46:17 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cim-3.0.894.tar` & `tencentcloud-sdk-python-cim-3.0.895.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:20:54.000000 tencentcloud-sdk-python-cim-3.0.894/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-18 00:20:54.000000 tencentcloud-sdk-python-cim-3.0.894/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:20:54.000000 tencentcloud-sdk-python-cim-3.0.894/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:20:54.000000 tencentcloud-sdk-python-cim-3.0.894/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:20:54.000000 tencentcloud-sdk-python-cim-3.0.894/tencentcloud/cim/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:20:54.000000 tencentcloud-sdk-python-cim-3.0.894/tencentcloud/cim/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:20:54.000000 tencentcloud-sdk-python-cim-3.0.894/tencentcloud/cim/v20190318/
--rw-r--r--   0 root         (0) root         (0)      827 2023-05-18 00:20:54.000000 tencentcloud-sdk-python-cim-3.0.894/tencentcloud/cim/v20190318/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:20:54.000000 tencentcloud-sdk-python-cim-3.0.894/tencentcloud/cim/v20190318/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1441 2023-05-18 00:20:54.000000 tencentcloud-sdk-python-cim-3.0.894/tencentcloud/cim/v20190318/models.py
--rw-r--r--   0 root         (0) root         (0)     1890 2023-05-18 00:20:54.000000 tencentcloud-sdk-python-cim-3.0.894/tencentcloud/cim/v20190318/cim_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:20:54.000000 tencentcloud-sdk-python-cim-3.0.894/tencentcloud_sdk_python_cim.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:20:54.000000 tencentcloud-sdk-python-cim-3.0.894/tencentcloud_sdk_python_cim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-18 00:20:54.000000 tencentcloud-sdk-python-cim-3.0.894/tencentcloud_sdk_python_cim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:20:54.000000 tencentcloud-sdk-python-cim-3.0.894/tencentcloud_sdk_python_cim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:20:54.000000 tencentcloud-sdk-python-cim-3.0.894/tencentcloud_sdk_python_cim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:20:54.000000 tencentcloud-sdk-python-cim-3.0.894/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-18 00:20:54.000000 tencentcloud-sdk-python-cim-3.0.894/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:20:54.000000 tencentcloud-sdk-python-cim-3.0.894/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:46:17.000000 tencentcloud-sdk-python-cim-3.0.895/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-19 02:46:17.000000 tencentcloud-sdk-python-cim-3.0.895/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:46:17.000000 tencentcloud-sdk-python-cim-3.0.895/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-19 02:46:17.000000 tencentcloud-sdk-python-cim-3.0.895/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:46:17.000000 tencentcloud-sdk-python-cim-3.0.895/tencentcloud/cim/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:46:17.000000 tencentcloud-sdk-python-cim-3.0.895/tencentcloud/cim/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:46:17.000000 tencentcloud-sdk-python-cim-3.0.895/tencentcloud/cim/v20190318/
+-rw-r--r--   0 root         (0) root         (0)      827 2023-05-19 02:46:17.000000 tencentcloud-sdk-python-cim-3.0.895/tencentcloud/cim/v20190318/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:46:17.000000 tencentcloud-sdk-python-cim-3.0.895/tencentcloud/cim/v20190318/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2023-05-19 02:46:17.000000 tencentcloud-sdk-python-cim-3.0.895/tencentcloud/cim/v20190318/models.py
+-rw-r--r--   0 root         (0) root         (0)     1890 2023-05-19 02:46:17.000000 tencentcloud-sdk-python-cim-3.0.895/tencentcloud/cim/v20190318/cim_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:46:17.000000 tencentcloud-sdk-python-cim-3.0.895/tencentcloud_sdk_python_cim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 02:46:17.000000 tencentcloud-sdk-python-cim-3.0.895/tencentcloud_sdk_python_cim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-19 02:46:17.000000 tencentcloud-sdk-python-cim-3.0.895/tencentcloud_sdk_python_cim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 02:46:17.000000 tencentcloud-sdk-python-cim-3.0.895/tencentcloud_sdk_python_cim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 02:46:17.000000 tencentcloud-sdk-python-cim-3.0.895/tencentcloud_sdk_python_cim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 02:46:17.000000 tencentcloud-sdk-python-cim-3.0.895/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-19 02:46:17.000000 tencentcloud-sdk-python-cim-3.0.895/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-19 02:46:17.000000 tencentcloud-sdk-python-cim-3.0.895/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cim-3.0.894/README.rst` & `tencentcloud-sdk-python-cim-3.0.895/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cim-3.0.894/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cim-3.0.895/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cim-3.0.894/tencentcloud/cim/v20190318/errorcodes.py` & `tencentcloud-sdk-python-cim-3.0.895/tencentcloud/cim/v20190318/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cim-3.0.894/tencentcloud/cim/v20190318/models.py` & `tencentcloud-sdk-python-cim-3.0.895/tencentcloud/cim/v20190318/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cim-3.0.894/tencentcloud/cim/v20190318/cim_client.py` & `tencentcloud-sdk-python-cim-3.0.895/tencentcloud/cim/v20190318/cim_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cim-3.0.894/tencentcloud_sdk_python_cim.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cim-3.0.895/tencentcloud_sdk_python_cim.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cim
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Cim SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cim-3.0.894/PKG-INFO` & `tencentcloud-sdk-python-cim-3.0.895/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cim
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Cim SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cim-3.0.894/setup.py` & `tencentcloud-sdk-python-cim-3.0.895/setup.py`

 * *Files identical despite different names*

