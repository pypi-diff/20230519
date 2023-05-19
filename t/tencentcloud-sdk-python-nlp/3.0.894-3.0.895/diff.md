# Comparing `tmp/tencentcloud-sdk-python-nlp-3.0.894.tar.gz` & `tmp/tencentcloud-sdk-python-nlp-3.0.895.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-nlp-3.0.894.tar", last modified: Thu May 18 00:32:38 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-nlp-3.0.895.tar", last modified: Fri May 19 02:56:15 2023, max compression
```

## Comparing `tencentcloud-sdk-python-nlp-3.0.894.tar` & `tencentcloud-sdk-python-nlp-3.0.895.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:32:38.000000 tencentcloud-sdk-python-nlp-3.0.894/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-18 00:32:38.000000 tencentcloud-sdk-python-nlp-3.0.894/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:32:38.000000 tencentcloud-sdk-python-nlp-3.0.894/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:32:38.000000 tencentcloud-sdk-python-nlp-3.0.894/tencentcloud/nlp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:32:38.000000 tencentcloud-sdk-python-nlp-3.0.894/tencentcloud/nlp/v20190408/
--rw-r--r--   0 root         (0) root         (0)     5906 2023-05-18 00:32:38.000000 tencentcloud-sdk-python-nlp-3.0.894/tencentcloud/nlp/v20190408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    44601 2023-05-18 00:32:38.000000 tencentcloud-sdk-python-nlp-3.0.894/tencentcloud/nlp/v20190408/nlp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:32:38.000000 tencentcloud-sdk-python-nlp-3.0.894/tencentcloud/nlp/v20190408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80999 2023-05-18 00:32:38.000000 tencentcloud-sdk-python-nlp-3.0.894/tencentcloud/nlp/v20190408/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:32:38.000000 tencentcloud-sdk-python-nlp-3.0.894/tencentcloud/nlp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:32:38.000000 tencentcloud-sdk-python-nlp-3.0.894/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:32:38.000000 tencentcloud-sdk-python-nlp-3.0.894/tencentcloud_sdk_python_nlp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:32:38.000000 tencentcloud-sdk-python-nlp-3.0.894/tencentcloud_sdk_python_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-18 00:32:38.000000 tencentcloud-sdk-python-nlp-3.0.894/tencentcloud_sdk_python_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:32:38.000000 tencentcloud-sdk-python-nlp-3.0.894/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:32:38.000000 tencentcloud-sdk-python-nlp-3.0.894/tencentcloud_sdk_python_nlp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:32:38.000000 tencentcloud-sdk-python-nlp-3.0.894/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-18 00:32:38.000000 tencentcloud-sdk-python-nlp-3.0.894/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:32:38.000000 tencentcloud-sdk-python-nlp-3.0.894/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:56:15.000000 tencentcloud-sdk-python-nlp-3.0.895/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-19 02:56:15.000000 tencentcloud-sdk-python-nlp-3.0.895/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:56:15.000000 tencentcloud-sdk-python-nlp-3.0.895/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:56:15.000000 tencentcloud-sdk-python-nlp-3.0.895/tencentcloud/nlp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:56:15.000000 tencentcloud-sdk-python-nlp-3.0.895/tencentcloud/nlp/v20190408/
+-rw-r--r--   0 root         (0) root         (0)     5906 2023-05-19 02:56:15.000000 tencentcloud-sdk-python-nlp-3.0.895/tencentcloud/nlp/v20190408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    44601 2023-05-19 02:56:15.000000 tencentcloud-sdk-python-nlp-3.0.895/tencentcloud/nlp/v20190408/nlp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:56:15.000000 tencentcloud-sdk-python-nlp-3.0.895/tencentcloud/nlp/v20190408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81020 2023-05-19 02:56:15.000000 tencentcloud-sdk-python-nlp-3.0.895/tencentcloud/nlp/v20190408/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:56:15.000000 tencentcloud-sdk-python-nlp-3.0.895/tencentcloud/nlp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-19 02:56:15.000000 tencentcloud-sdk-python-nlp-3.0.895/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:56:15.000000 tencentcloud-sdk-python-nlp-3.0.895/tencentcloud_sdk_python_nlp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 02:56:15.000000 tencentcloud-sdk-python-nlp-3.0.895/tencentcloud_sdk_python_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-19 02:56:15.000000 tencentcloud-sdk-python-nlp-3.0.895/tencentcloud_sdk_python_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 02:56:15.000000 tencentcloud-sdk-python-nlp-3.0.895/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 02:56:15.000000 tencentcloud-sdk-python-nlp-3.0.895/tencentcloud_sdk_python_nlp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 02:56:15.000000 tencentcloud-sdk-python-nlp-3.0.895/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-19 02:56:15.000000 tencentcloud-sdk-python-nlp-3.0.895/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-19 02:56:15.000000 tencentcloud-sdk-python-nlp-3.0.895/setup.cfg
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.894/README.rst` & `tencentcloud-sdk-python-nlp-3.0.895/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-nlp-3.0.894/tencentcloud/nlp/v20190408/errorcodes.py` & `tencentcloud-sdk-python-nlp-3.0.895/tencentcloud/nlp/v20190408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-nlp-3.0.894/tencentcloud/nlp/v20190408/nlp_client.py` & `tencentcloud-sdk-python-nlp-3.0.895/tencentcloud/nlp/v20190408/nlp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-nlp-3.0.894/tencentcloud/nlp/v20190408/models.py` & `tencentcloud-sdk-python-nlp-3.0.895/tencentcloud/nlp/v20190408/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -867,15 +867,15 @@
     """
 
     def __init__(self):
         r"""
         :param Text: 润色后的文本。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Text: str
-        :param EmbellishType: 润色类型。类型列表
+        :param EmbellishType: 润色类型。类型如下：
 expansion：扩写
 rewriting：改写
 translation_m2a：从现代文改写为古文
 translation_a2m：从古文改写为现代文
 
 
 注意：此字段可能返回 null，表示取不到有效值。
@@ -1103,15 +1103,15 @@
     def __init__(self):
         r"""
         :param WordList: 生成句子的关键词，关键词个数需不超过4个，中文关键词长度应不超过10字符，英文关键词长度不超过3个单词。关键词中不可包含标点符号。
         :type WordList: list of str
         :param Number: 返回生成句子的个数。数量需>=1且<=5。
 （注意实际结果可能小于指定个数）
         :type Number: int
-        :param Domain: 指定生成句子的领域，支持领域列表
+        :param Domain: 指定生成句子的领域，支持领域如下：
 general：通用领域，支持中英文
 academic：学术领域，仅支持英文
 默认为general（通用领域）。
         :type Domain: str
         """
         self.WordList = None
         self.Number = None
@@ -2138,22 +2138,22 @@
 
     """
 
     def __init__(self):
         r"""
         :param Text: 待润色的文本。中文文本长度需<=50字符；英文文本长度需<=30个单词。
         :type Text: str
-        :param SourceLang: 待润色文本的语言类型，支持语言列表
+        :param SourceLang: 待润色文本的语言类型，支持语言如下：
 zh：中文
 en：英文
         :type SourceLang: str
         :param Number: 返回润色结果的个数。数量需>=1且<=5。
 （注意实际结果可能小于指定个数）
         :type Number: int
-        :param Style: 控制润色类型，类型列表
+        :param Style: 控制润色类型，类型如下：
 both：同时返回改写和扩写
 expansion：扩写
 rewriting：改写
 m2a：从现代文改写为古文
 a2m：从古文改写为现代文
 默认为both。
         :type Style: str
@@ -2317,27 +2317,27 @@
 
     """
 
     def __init__(self):
         r"""
         :param Text: 待续写的句子，文本统一使用utf-8格式编码，长度不超过200字符。
         :type Text: str
-        :param SourceLang: 待续写文本的语言类型，支持语言列表
+        :param SourceLang: 待续写文本的语言类型，支持语言如下：
 zh：中文
 en：英文
         :type SourceLang: str
         :param Number: 返回续写结果的个数。数量需>=1且<=5。
 （注意实际结果可能小于指定个数）
         :type Number: int
-        :param Domain: 指定续写领域，支持领域列表
+        :param Domain: 指定续写领域，支持领域如下：
 general：通用领域，支持中英文补全
 academic：学术领域，仅支持英文补全
 默认为general（通用领域）。
         :type Domain: str
-        :param Style: 指定续写风格，支持风格列表
+        :param Style: 指定续写风格，支持风格如下：
 science_fiction：科幻
 military_history：军事
 xuanhuan_wuxia：武侠
 urban_officialdom：职场
 默认为xuanhuan_wuxia（武侠）。
         :type Style: str
         """
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.894/tencentcloud/__init__.py` & `tencentcloud-sdk-python-nlp-3.0.895/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-nlp-3.0.894/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-nlp-3.0.895/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-nlp
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Nlp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.894/PKG-INFO` & `tencentcloud-sdk-python-nlp-3.0.895/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-nlp
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Nlp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.894/setup.py` & `tencentcloud-sdk-python-nlp-3.0.895/setup.py`

 * *Files identical despite different names*

