# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.894.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.895.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.894.tar", last modified: Thu May 18 00:26:03 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.895.tar", last modified: Fri May 19 02:50:59 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.894.tar` & `tencentcloud-sdk-python-essbasic-3.0.895.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      752 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)    15673 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    50895 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)   230725 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)     5392 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171664 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:26:03.000000 tencentcloud-sdk-python-essbasic-3.0.894/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:50:59.000000 tencentcloud-sdk-python-essbasic-3.0.895/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:50:59.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 02:50:59.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-05-19 02:50:59.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-19 02:50:59.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 02:50:59.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      752 2023-05-19 02:50:58.000000 tencentcloud-sdk-python-essbasic-3.0.895/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:50:59.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-19 02:50:58.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:50:59.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:50:59.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)    15673 2023-05-19 02:50:58.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    50895 2023-05-19 02:50:58.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:50:58.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   230804 2023-05-19 02:50:58.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:50:58.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:50:59.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-05-19 02:50:58.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-05-19 02:50:58.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:50:58.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171664 2023-05-19 02:50:58.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-19 02:50:59.000000 tencentcloud-sdk-python-essbasic-3.0.895/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-05-19 02:50:58.000000 tencentcloud-sdk-python-essbasic-3.0.895/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-19 02:50:59.000000 tencentcloud-sdk-python-essbasic-3.0.895/setup.cfg
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.894/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.895/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2008,15 +2008,16 @@
 TaskEnd        - 任务处理完成
 DownloadFailed - 下载失败
 ProcessFailed  - 转换失败
 ProcessTimeout - 转换文件超时
         :type TaskMessage: str
         :param ResourceId: 资源Id，也是FileId，用于文件发起使用
         :type ResourceId: str
-        :param PreviewUrl: 预览文件Url，有效期30分钟
+        :param PreviewUrl: 预览文件Url，有效期30分钟 
+当前字段返回为空，发起的时候，将ResourceId 放入发起即可
 注意：此字段可能返回 null，表示取不到有效值。
         :type PreviewUrl: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.TaskId = None
         self.TaskStatus = None
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.894/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.894/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.895/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.894/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.895/setup.py`

 * *Files identical despite different names*

