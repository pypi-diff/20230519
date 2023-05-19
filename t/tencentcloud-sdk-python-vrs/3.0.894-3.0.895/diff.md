# Comparing `tmp/tencentcloud-sdk-python-vrs-3.0.894.tar.gz` & `tmp/tencentcloud-sdk-python-vrs-3.0.895.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vrs-3.0.894.tar", last modified: Thu May 18 00:42:03 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vrs-3.0.895.tar", last modified: Fri May 19 03:05:30 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vrs-3.0.894.tar` & `tencentcloud-sdk-python-vrs-3.0.895.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:42:03.000000 tencentcloud-sdk-python-vrs-3.0.894/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-18 00:42:03.000000 tencentcloud-sdk-python-vrs-3.0.894/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:42:03.000000 tencentcloud-sdk-python-vrs-3.0.894/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:42:03.000000 tencentcloud-sdk-python-vrs-3.0.894/tencentcloud/vrs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:42:03.000000 tencentcloud-sdk-python-vrs-3.0.894/tencentcloud/vrs/v20200824/
--rw-r--r--   0 root         (0) root         (0)     5710 2023-05-18 00:42:03.000000 tencentcloud-sdk-python-vrs-3.0.894/tencentcloud/vrs/v20200824/vrs_client.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-05-18 00:42:03.000000 tencentcloud-sdk-python-vrs-3.0.894/tencentcloud/vrs/v20200824/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:42:03.000000 tencentcloud-sdk-python-vrs-3.0.894/tencentcloud/vrs/v20200824/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15471 2023-05-18 00:42:03.000000 tencentcloud-sdk-python-vrs-3.0.894/tencentcloud/vrs/v20200824/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:42:03.000000 tencentcloud-sdk-python-vrs-3.0.894/tencentcloud/vrs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:42:03.000000 tencentcloud-sdk-python-vrs-3.0.894/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:42:03.000000 tencentcloud-sdk-python-vrs-3.0.894/tencentcloud_sdk_python_vrs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:42:03.000000 tencentcloud-sdk-python-vrs-3.0.894/tencentcloud_sdk_python_vrs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-18 00:42:03.000000 tencentcloud-sdk-python-vrs-3.0.894/tencentcloud_sdk_python_vrs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:42:03.000000 tencentcloud-sdk-python-vrs-3.0.894/tencentcloud_sdk_python_vrs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:42:03.000000 tencentcloud-sdk-python-vrs-3.0.894/tencentcloud_sdk_python_vrs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:42:03.000000 tencentcloud-sdk-python-vrs-3.0.894/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-18 00:42:03.000000 tencentcloud-sdk-python-vrs-3.0.894/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:42:03.000000 tencentcloud-sdk-python-vrs-3.0.894/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:05:30.000000 tencentcloud-sdk-python-vrs-3.0.895/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-19 03:05:30.000000 tencentcloud-sdk-python-vrs-3.0.895/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:05:30.000000 tencentcloud-sdk-python-vrs-3.0.895/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:05:30.000000 tencentcloud-sdk-python-vrs-3.0.895/tencentcloud/vrs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:05:30.000000 tencentcloud-sdk-python-vrs-3.0.895/tencentcloud/vrs/v20200824/
+-rw-r--r--   0 root         (0) root         (0)     5710 2023-05-19 03:05:30.000000 tencentcloud-sdk-python-vrs-3.0.895/tencentcloud/vrs/v20200824/vrs_client.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-05-19 03:05:30.000000 tencentcloud-sdk-python-vrs-3.0.895/tencentcloud/vrs/v20200824/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 03:05:30.000000 tencentcloud-sdk-python-vrs-3.0.895/tencentcloud/vrs/v20200824/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15425 2023-05-19 03:05:30.000000 tencentcloud-sdk-python-vrs-3.0.895/tencentcloud/vrs/v20200824/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 03:05:30.000000 tencentcloud-sdk-python-vrs-3.0.895/tencentcloud/vrs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-19 03:05:30.000000 tencentcloud-sdk-python-vrs-3.0.895/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:05:30.000000 tencentcloud-sdk-python-vrs-3.0.895/tencentcloud_sdk_python_vrs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 03:05:30.000000 tencentcloud-sdk-python-vrs-3.0.895/tencentcloud_sdk_python_vrs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-19 03:05:30.000000 tencentcloud-sdk-python-vrs-3.0.895/tencentcloud_sdk_python_vrs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 03:05:30.000000 tencentcloud-sdk-python-vrs-3.0.895/tencentcloud_sdk_python_vrs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 03:05:30.000000 tencentcloud-sdk-python-vrs-3.0.895/tencentcloud_sdk_python_vrs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 03:05:30.000000 tencentcloud-sdk-python-vrs-3.0.895/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-19 03:05:30.000000 tencentcloud-sdk-python-vrs-3.0.895/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-19 03:05:30.000000 tencentcloud-sdk-python-vrs-3.0.895/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.894/README.rst` & `tencentcloud-sdk-python-vrs-3.0.895/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vrs-3.0.894/tencentcloud/vrs/v20200824/vrs_client.py` & `tencentcloud-sdk-python-vrs-3.0.895/tencentcloud/vrs/v20200824/vrs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vrs-3.0.894/tencentcloud/vrs/v20200824/errorcodes.py` & `tencentcloud-sdk-python-vrs-3.0.895/tencentcloud/vrs/v20200824/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vrs-3.0.894/tencentcloud/vrs/v20200824/models.py` & `tencentcloud-sdk-python-vrs-3.0.895/tencentcloud/vrs/v20200824/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 1-中文
         :type VoiceLanguage: int
         :param Codec: 音频格式，音频类型(wav,mp3,aac,m4a)
         :type Codec: str
         :param AudioIdList: 音频ID集合
         :type AudioIdList: list of str
         :param CallbackUrl: 回调 URL，用户自行搭建的用于接收结果的服务URL。如果用户使用轮询方式获取识别结果，则无需提交该参数。
-回调采用POST请求方式，Content-Type为application/x-www-form-urlencoded，回调数据格式如下:callback_body=checksum=&data={"TaskId":"xxxxxxxxxxxxxx","Status":2,"StatusStr":"success","VoiceType":xxxxx,"ErrorMsg":""}
+回调采用POST请求方式，Content-Type为application/json，回调数据格式如下:{"TaskId":"xxxxxxxxxxxxxx","Status":2,"StatusStr":"success","VoiceType":xxxxx,"ErrorMsg":""}
         :type CallbackUrl: str
         """
         self.SessionId = None
         self.VoiceName = None
         self.SampleRate = None
         self.VoiceGender = None
         self.VoiceLanguage = None
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.894/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vrs-3.0.895/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vrs-3.0.894/tencentcloud_sdk_python_vrs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vrs-3.0.895/tencentcloud_sdk_python_vrs.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vrs
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Vrs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.894/PKG-INFO` & `tencentcloud-sdk-python-vrs-3.0.895/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vrs
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Vrs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.894/setup.py` & `tencentcloud-sdk-python-vrs-3.0.895/setup.py`

 * *Files identical despite different names*

