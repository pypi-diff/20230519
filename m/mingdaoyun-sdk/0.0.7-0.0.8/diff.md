# Comparing `tmp/mingdaoyun_sdk-0.0.7.tar.gz` & `tmp/mingdaoyun_sdk-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mingdaoyun_sdk-0.0.7.tar", last modified: Tue Apr 18 06:39:47 2023, max compression
+gzip compressed data, was "mingdaoyun_sdk-0.0.8.tar", last modified: Fri May 19 09:38:30 2023, max compression
```

## Comparing `mingdaoyun_sdk-0.0.7.tar` & `mingdaoyun_sdk-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:39:47.499807 mingdaoyun_sdk-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-18 06:39:47.499807 mingdaoyun_sdk-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-18 06:39:36.000000 mingdaoyun_sdk-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:39:47.495808 mingdaoyun_sdk-0.0.7/mingdaoyun_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-18 06:39:36.000000 mingdaoyun_sdk-0.0.7/mingdaoyun_sdk/MingdaoOrg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-04-18 06:39:36.000000 mingdaoyun_sdk-0.0.7/mingdaoyun_sdk/MingdaoYun.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 06:39:36.000000 mingdaoyun_sdk-0.0.7/mingdaoyun_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-18 06:39:36.000000 mingdaoyun_sdk-0.0.7/mingdaoyun_sdk/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:39:47.499807 mingdaoyun_sdk-0.0.7/mingdaoyun_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-18 06:39:47.000000 mingdaoyun_sdk-0.0.7/mingdaoyun_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-18 06:39:47.000000 mingdaoyun_sdk-0.0.7/mingdaoyun_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 06:39:47.000000 mingdaoyun_sdk-0.0.7/mingdaoyun_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-18 06:39:47.000000 mingdaoyun_sdk-0.0.7/mingdaoyun_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 06:39:47.499807 mingdaoyun_sdk-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-18 06:39:36.000000 mingdaoyun_sdk-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:38:30.499823 mingdaoyun_sdk-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-19 09:38:30.499823 mingdaoyun_sdk-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-19 09:38:17.000000 mingdaoyun_sdk-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:38:30.499823 mingdaoyun_sdk-0.0.8/mingdaoyun_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-19 09:38:17.000000 mingdaoyun_sdk-0.0.8/mingdaoyun_sdk/MingdaoOrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-05-19 09:38:17.000000 mingdaoyun_sdk-0.0.8/mingdaoyun_sdk/MingdaoYun.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:38:17.000000 mingdaoyun_sdk-0.0.8/mingdaoyun_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-19 09:38:17.000000 mingdaoyun_sdk-0.0.8/mingdaoyun_sdk/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:38:30.499823 mingdaoyun_sdk-0.0.8/mingdaoyun_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-19 09:38:30.000000 mingdaoyun_sdk-0.0.8/mingdaoyun_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-19 09:38:30.000000 mingdaoyun_sdk-0.0.8/mingdaoyun_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 09:38:30.000000 mingdaoyun_sdk-0.0.8/mingdaoyun_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-19 09:38:30.000000 mingdaoyun_sdk-0.0.8/mingdaoyun_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 09:38:30.499823 mingdaoyun_sdk-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-19 09:38:17.000000 mingdaoyun_sdk-0.0.8/setup.py
```

### Comparing `mingdaoyun_sdk-0.0.7/PKG-INFO` & `mingdaoyun_sdk-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mingdaoyun_sdk
-Version: 0.0.7
+Version: 0.0.8
 Summary: 针对mingdaoyun的API封装的Python-SDK包
 Home-page: https://github.com/ghostlitao/mingdaoyun-python-sdk
 Author: Todd
 Author-email: ghostlitao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mingdaoyun_sdk-0.0.7/mingdaoyun_sdk/MingdaoOrg.py` & `mingdaoyun_sdk-0.0.8/mingdaoyun_sdk/MingdaoOrg.py`

 * *Files identical despite different names*

### Comparing `mingdaoyun_sdk-0.0.7/mingdaoyun_sdk/MingdaoYun.py` & `mingdaoyun_sdk-0.0.8/mingdaoyun_sdk/MingdaoYun.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,22 +46,31 @@
         self.filters = []
         self.worksheetId = ""
         self.view = ""
         if cert_path is not None:
             http.verify = cert_path
         return
 
+    def reset(self):
+        """
+        重置class
+        :return:
+        """
+        self.filters = []
+        self.params = {}
+        self.view = ""
+
     def table(self, table: str):
         """
         设置当前的worksheet
         :param table: 表名
         :return: 自身
         """
+        self.reset()
         self.worksheetId = table
-        self.filters = []
         if not self.worksheetMap.get(self.worksheetId):
             data = self.exec(self.WORKSHEET_MAP_URL)
             map = {}
             for item in data["data"]["controls"]:
                 if "alias" in item and item["alias"]:
                     map[item["alias"]] = item
                 else:
@@ -259,7 +268,18 @@
                 print(f'turn page {len(result["data"]["rows"])}/{result["data"]["total"]}')
                 self.params["pageIndex"] = self.params["pageIndex"] + 1
                 current_result = self.exec(self.GET_RELATIONS_URL)
                 result["data"]["rows"] = result["data"]["rows"] + current_result["data"]["rows"]
             return result
         else:
             return result
+
+    def sort(self, sortId: str, isAsc: bool):
+        """
+        设置排序
+        :param sortId:
+        :param isAsc:
+        :return:
+        """
+        self.params["sortId"] = sortId
+        self.params["isAsc"] = isAsc
+        return self
```

### Comparing `mingdaoyun_sdk-0.0.7/mingdaoyun_sdk/common.py` & `mingdaoyun_sdk-0.0.8/mingdaoyun_sdk/common.py`

 * *Files identical despite different names*

### Comparing `mingdaoyun_sdk-0.0.7/mingdaoyun_sdk.egg-info/PKG-INFO` & `mingdaoyun_sdk-0.0.8/mingdaoyun_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mingdaoyun-sdk
-Version: 0.0.7
+Version: 0.0.8
 Summary: 针对mingdaoyun的API封装的Python-SDK包
 Home-page: https://github.com/ghostlitao/mingdaoyun-python-sdk
 Author: Todd
 Author-email: ghostlitao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mingdaoyun_sdk-0.0.7/setup.py` & `mingdaoyun_sdk-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     # 包的分发名称，使用字母、数字、_、-
     name="mingdaoyun_sdk",
     # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
-    version="0.0.7",
+    version="0.0.8",
     # 作者名
     author="Todd",
     # 作者邮箱
     author_email="ghostlitao@gmail.com",
     # 包的简介描述
     description="针对mingdaoyun的API封装的Python-SDK包",
     # 包的详细介绍(一般通过加载README.md)
```

