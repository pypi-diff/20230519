# Comparing `tmp/ats_case-0.7.4.tar.gz` & `tmp/ats_case-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.7.4.tar", last modified: Thu May 18 05:26:22 2023, max compression
+gzip compressed data, was "ats_case-0.7.5.tar", last modified: Fri May 19 08:22:35 2023, max compression
```

## Comparing `ats_case-0.7.4.tar` & `ats_case-0.7.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 05:26:22.703630 ats_case-0.7.4/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.7.4/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.7.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-05-18 05:26:22.701635 ats_case-0.7.4/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.7.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 05:26:22.231452 ats_case-0.7.4/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.7.4/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 05:26:22.519102 ats_case-0.7.4/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.7.4/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    17907 2023-05-18 03:07:32.000000 ats_case-0.7.4/ats_case/case/command.py
--rw-rw-rw-   0        0        0    11101 2023-05-18 05:15:05.000000 ats_case-0.7.4/ats_case/case/context.py
--rw-rw-rw-   0        0        0     7500 2023-04-26 02:52:46.000000 ats_case-0.7.4/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5548 2023-05-04 06:36:02.000000 ats_case-0.7.4/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-05-18 05:26:22.590910 ats_case-0.7.4/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.7.4/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.7.4/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.7.4/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-05-18 05:26:22.655738 ats_case-0.7.4/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.7.4/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.7.4/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     3611 2023-04-26 05:44:37.000000 ats_case-0.7.4/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-05-18 05:26:22.693654 ats_case-0.7.4/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.7.4/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2473 2023-05-18 05:24:57.000000 ats_case-0.7.4/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-05-18 05:26:22.368106 ats_case-0.7.4/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-05-18 05:26:21.000000 ats_case-0.7.4/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-05-18 05:26:21.000000 ats_case-0.7.4/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 05:26:21.000000 ats_case-0.7.4/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-18 05:26:21.000000 ats_case-0.7.4/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-18 05:26:21.000000 ats_case-0.7.4/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 05:26:22.704628 ats_case-0.7.4/setup.cfg
--rw-rw-rw-   0        0        0      945 2023-05-17 05:57:29.000000 ats_case-0.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:22:35.262507 ats_case-0.7.5/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.7.5/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.7.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-05-19 08:22:35.260512 ats_case-0.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.7.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 08:22:34.876990 ats_case-0.7.5/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.7.5/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:22:35.083505 ats_case-0.7.5/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.7.5/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    17903 2023-05-19 08:22:21.000000 ats_case-0.7.5/ats_case/case/command.py
+-rw-rw-rw-   0        0        0    11101 2023-05-18 05:15:05.000000 ats_case-0.7.5/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     7500 2023-04-26 02:52:46.000000 ats_case-0.7.5/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5548 2023-05-04 06:36:02.000000 ats_case-0.7.5/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:22:35.151282 ats_case-0.7.5/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.7.5/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.7.5/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.7.5/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:22:35.214631 ats_case-0.7.5/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.7.5/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.7.5/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     3611 2023-04-26 05:44:37.000000 ats_case-0.7.5/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:22:35.248544 ats_case-0.7.5/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.7.5/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2473 2023-05-18 05:24:57.000000 ats_case-0.7.5/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-05-19 08:22:34.972347 ats_case-0.7.5/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-05-19 08:22:34.000000 ats_case-0.7.5/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-05-19 08:22:34.000000 ats_case-0.7.5/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 08:22:34.000000 ats_case-0.7.5/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-19 08:22:34.000000 ats_case-0.7.5/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-19 08:22:34.000000 ats_case-0.7.5/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 08:22:35.262507 ats_case-0.7.5/setup.cfg
+-rw-rw-rw-   0        0        0      945 2023-05-19 08:22:21.000000 ats_case-0.7.5/setup.py
```

### Comparing `ats_case-0.7.4/PKG-INFO` & `ats_case-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.7.4
+Version: 0.7.5
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.7.4/README.md` & `ats_case-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.7.4/ats_case/case/command.py` & `ats_case-0.7.5/ats_case/case/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,15 +273,15 @@
         if self._func is not None:
             if type(self._func_parameter) is dict:
                 self._func_parameter = _replace(context, self._func_parameter)
             try:
                 if self._expect_result is None:
                     expect_result = context.runtime.steps[context.runtime.step - 1]
                 else:
-                    expect_result = context.runtime.steps[int(self._expect_result) - 1]
+                    expect_result = context.runtime.steps[int(self._expect_result)]
             except:
                 expect_result = None
             data = func.to_dict(result=self._parse, expect_result=expect_result, parameter=self._func_parameter)
 
             logger.info('~ @ACD-> module:{} function:{} parameter:{}'.format(
                 self._func_module, self._func, self._func_parameter))
             result = udm.handle(module='meter.{}'.format(self._func_module), function=self._func
```

### Comparing `ats_case-0.7.4/ats_case/case/context.py` & `ats_case-0.7.5/ats_case/case/context.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.7.4/ats_case/case/executor.py` & `ats_case-0.7.5/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.7.4/ats_case/case/translator.py` & `ats_case-0.7.5/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.7.4/ats_case/common/error.py` & `ats_case-0.7.5/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.7.4/ats_case/manage/core.py` & `ats_case-0.7.5/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.7.4/ats_case/manage/start.py` & `ats_case-0.7.5/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.7.4/ats_case/template/testcase_v1.tmp` & `ats_case-0.7.5/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.7.4/ats_case.egg-info/PKG-INFO` & `ats_case-0.7.5/ats_case.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.7.4
+Version: 0.7.5
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.7.4/ats_case.egg-info/SOURCES.txt` & `ats_case-0.7.5/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.7.4/setup.py` & `ats_case-0.7.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.7.4",
+    version="0.7.5",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

