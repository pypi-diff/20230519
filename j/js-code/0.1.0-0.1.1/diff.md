# Comparing `tmp/js_code-0.1.0.tar.gz` & `tmp/js_code-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "js_code-0.1.0.tar", last modified: Thu May 18 01:42:46 2023, max compression
+gzip compressed data, was "js_code-0.1.1.tar", last modified: Fri May 19 00:12:53 2023, max compression
```

## Comparing `js_code-0.1.0.tar` & `js_code-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 01:42:46.244468 js_code-0.1.0/
--rw-rw-rw-   0        0        0     1094 2023-04-12 08:29:30.000000 js_code-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      330 2023-05-18 01:42:46.244468 js_code-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 01:42:46.227514 js_code-0.1.0/js_code/
--rw-rw-rw-   0        0        0        0 2023-04-12 06:50:12.000000 js_code-0.1.0/js_code/__init__.py
--rw-rw-rw-   0        0        0     1107 2023-05-18 01:33:41.000000 js_code-0.1.0/js_code/js_open.py
-drwxrwxrwx   0        0        0        0 2023-05-18 01:42:46.243474 js_code-0.1.0/js_code.egg-info/
--rw-rw-rw-   0        0        0      330 2023-05-18 01:42:46.000000 js_code-0.1.0/js_code.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-05-18 01:42:46.000000 js_code-0.1.0/js_code.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 01:42:46.000000 js_code-0.1.0/js_code.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-18 01:42:46.000000 js_code-0.1.0/js_code.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-18 01:42:46.000000 js_code-0.1.0/js_code.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 01:42:46.244468 js_code-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      490 2023-05-18 01:42:19.000000 js_code-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 00:12:53.205357 js_code-0.1.1/
+-rw-rw-rw-   0        0        0     1094 2023-04-12 08:29:30.000000 js_code-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      306 2023-05-19 00:12:53.205357 js_code-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-19 00:12:53.189729 js_code-0.1.1/js_code/
+-rw-rw-rw-   0        0        0        0 2023-04-12 06:50:12.000000 js_code-0.1.1/js_code/__init__.py
+-rw-rw-rw-   0        0        0     1130 2023-05-19 00:11:10.000000 js_code-0.1.1/js_code/js_open.py
+drwxrwxrwx   0        0        0        0 2023-05-19 00:12:53.205357 js_code-0.1.1/js_code.egg-info/
+-rw-rw-rw-   0        0        0      306 2023-05-19 00:12:53.000000 js_code-0.1.1/js_code.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-05-19 00:12:53.000000 js_code-0.1.1/js_code.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 00:12:53.000000 js_code-0.1.1/js_code.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-19 00:12:53.000000 js_code-0.1.1/js_code.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-19 00:12:53.000000 js_code-0.1.1/js_code.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 00:12:53.205357 js_code-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      460 2023-05-19 00:12:21.000000 js_code-0.1.1/setup.py
```

### Comparing `js_code-0.1.0/LICENSE` & `js_code-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `js_code-0.1.0/js_code/js_open.py` & `js_code-0.1.1/js_code/js_open.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import subprocess
 
 # 防止乱码
 subprocess.Popen = partial(subprocess.Popen, encoding="utf-8")
 import execjs
 
 
-def js_lead_into(file, code=None, encoding="utf-8"):
+def js_lead_into(file=None, code=None, encoding="utf-8"):
     """
     :param code:需要添加在文件开头  javascript 代码  示例 code = "var a = 10;\n"
     :param file: 需要手动添加文件路径，或者javascript的代码格式(function fn(){return xxx;};
     有条件判断增加相应的条件判断，或者循环)
     :param mode: 只读模式
     :param encoding: 默认utf-8
     """
@@ -20,13 +20,16 @@
             if code:
                 js_code = code + f.read()
             else:
                 js_code = f.read()
             # 加载 javascript 代码
         js = execjs.compile(js_code)
     except:
-        try:
-            # 做一个适配同时兼容 javascript 代码 不用读出javascript代码文件
+        # 做一个适配同时兼容 javascript 代码 不用读出javascript代码文件
+        if code:
+            js = execjs.compile(f"{code}{file}")
+        else:
             js = execjs.compile(file)
-        except:
-            js = execjs.eval(file)
     return js
+
+
+
```

