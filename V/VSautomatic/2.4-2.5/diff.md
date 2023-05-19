# Comparing `tmp/VSautomatic-2.4.tar.gz` & `tmp/VSautomatic-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VSautomatic-2.4.tar", last modified: Thu May 18 07:43:10 2023, max compression
+gzip compressed data, was "VSautomatic-2.5.tar", last modified: Thu May 18 08:02:43 2023, max compression
```

## Comparing `VSautomatic-2.4.tar` & `VSautomatic-2.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 07:43:10.656377 VSautomatic-2.4/
--rw-rw-rw-   0        0        0      259 2023-05-18 07:43:10.656377 VSautomatic-2.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 07:43:10.636392 VSautomatic-2.4/VSautomatic/
--rw-rw-rw-   0        0        0       10 2023-05-15 06:47:27.000000 VSautomatic-2.4/VSautomatic/Auth_Token.txt
--rw-rw-rw-   0        0        0   432646 2016-06-02 01:39:06.000000 VSautomatic-2.4/VSautomatic/DeviceDB.xml
--rw-rw-rw-   0        0        0    24737 2022-10-28 06:26:28.000000 VSautomatic-2.4/VSautomatic/Dictionary.txt
--rw-rw-rw-   0        0        0     3326 2018-08-08 06:11:30.000000 VSautomatic-2.4/VSautomatic/IR_Remote.xml
--rw-rw-rw-   0        0        0   302689 2018-11-23 08:40:34.000000 VSautomatic-2.4/VSautomatic/MacroList.xml
--rw-rw-rw-   0        0        0     2708 2023-05-16 06:09:22.000000 VSautomatic-2.4/VSautomatic/MyCamera.py
--rw-rw-rw-   0        0        0     1460 2023-05-15 09:48:39.000000 VSautomatic-2.4/VSautomatic/MyRedRat.py
--rw-rw-rw-   0        0        0     8124 2023-05-18 07:19:14.000000 VSautomatic-2.4/VSautomatic/MyTools.py
--rw-rw-rw-   0        0        0     1481 2018-03-09 10:13:06.000000 VSautomatic-2.4/VSautomatic/NLog.config
--rw-rw-rw-   0        0        0   612864 2018-02-27 16:35:06.000000 VSautomatic-2.4/VSautomatic/NLog.dll
--rw-rw-rw-   0        0        0    18705 2023-05-15 09:48:39.000000 VSautomatic-2.4/VSautomatic/ReSTTerminal.py
--rw-rw-rw-   0        0        0   842240 2018-07-25 04:16:14.000000 VSautomatic-2.4/VSautomatic/RedRat.dll
--rw-rw-rw-   0        0        0    10752 2018-07-25 04:16:10.000000 VSautomatic-2.4/VSautomatic/RedRatHub.Connection.dll
--rw-rw-rw-   0        0        0     1768 2023-05-15 09:48:39.000000 VSautomatic-2.4/VSautomatic/RedRatHub.py
--rwxrwxrwx   0        0        0    14336 2018-07-25 04:16:16.000000 VSautomatic-2.4/VSautomatic/RedRatHubCmd.exe
--rw-rw-rw-   0        0        0      146 2018-03-09 10:13:06.000000 VSautomatic-2.4/VSautomatic/RedRatHubCmd.exe.config
--rw-rw-rw-   0        0        0    48640 2018-07-25 04:16:14.000000 VSautomatic-2.4/VSautomatic/RedRatHubCore.dll
--rw-rw-rw-   0        0        0     1052 2023-05-16 05:16:48.000000 VSautomatic-2.4/VSautomatic/RedRatHubS.py
--rw-rw-rw-   0        0        0     2522 2023-05-15 09:48:39.000000 VSautomatic-2.4/VSautomatic/TestCfgParse.py
--rw-rw-rw-   0        0        0    48335 2018-11-01 05:37:28.000000 VSautomatic-2.4/VSautomatic/Vizio.xml
--rw-rw-rw-   0        0        0    14450 2022-03-17 01:56:03.000000 VSautomatic-2.4/VSautomatic/Vizio_IR.xml
--rw-rw-rw-   0        0        0      154 2023-05-15 09:48:39.000000 VSautomatic-2.4/VSautomatic/__init__.py
--rw-rw-rw-   0        0        0     1121 2023-05-15 09:48:39.000000 VSautomatic-2.4/VSautomatic/deco.py
--rw-rw-rw-   0        0        0     3230 2023-05-15 09:48:39.000000 VSautomatic-2.4/VSautomatic/my_serial.py
--rw-rw-rw-   0        0        0       81 2023-05-15 06:49:02.000000 VSautomatic-2.4/VSautomatic/restlog.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 07:43:10.646378 VSautomatic-2.4/VSautomatic.egg-info/
--rw-rw-rw-   0        0        0      259 2023-05-18 07:43:10.000000 VSautomatic-2.4/VSautomatic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      831 2023-05-18 07:43:10.000000 VSautomatic-2.4/VSautomatic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 07:43:10.000000 VSautomatic-2.4/VSautomatic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-05-18 07:43:10.000000 VSautomatic-2.4/VSautomatic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-18 07:43:10.000000 VSautomatic-2.4/VSautomatic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 07:43:10.656377 VSautomatic-2.4/setup.cfg
--rw-rw-rw-   0        0        0     1111 2023-05-18 07:42:47.000000 VSautomatic-2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:02:43.315146 VSautomatic-2.5/
+-rw-rw-rw-   0        0        0      259 2023-05-18 08:02:43.315146 VSautomatic-2.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 08:02:43.285137 VSautomatic-2.5/VSautomatic/
+-rw-rw-rw-   0        0        0       10 2023-05-15 06:47:27.000000 VSautomatic-2.5/VSautomatic/Auth_Token.txt
+-rw-rw-rw-   0        0        0   432646 2016-06-02 01:39:06.000000 VSautomatic-2.5/VSautomatic/DeviceDB.xml
+-rw-rw-rw-   0        0        0    24737 2022-10-28 06:26:28.000000 VSautomatic-2.5/VSautomatic/Dictionary.txt
+-rw-rw-rw-   0        0        0     3326 2018-08-08 06:11:30.000000 VSautomatic-2.5/VSautomatic/IR_Remote.xml
+-rw-rw-rw-   0        0        0   302689 2018-11-23 08:40:34.000000 VSautomatic-2.5/VSautomatic/MacroList.xml
+-rw-rw-rw-   0        0        0     2708 2023-05-16 06:09:22.000000 VSautomatic-2.5/VSautomatic/MyCamera.py
+-rw-rw-rw-   0        0        0     1460 2023-05-15 09:48:39.000000 VSautomatic-2.5/VSautomatic/MyRedRat.py
+-rw-rw-rw-   0        0        0     8124 2023-05-18 07:19:14.000000 VSautomatic-2.5/VSautomatic/MyTools.py
+-rw-rw-rw-   0        0        0     1481 2018-03-09 10:13:06.000000 VSautomatic-2.5/VSautomatic/NLog.config
+-rw-rw-rw-   0        0        0   612864 2018-02-27 16:35:06.000000 VSautomatic-2.5/VSautomatic/NLog.dll
+-rw-rw-rw-   0        0        0    18705 2023-05-15 09:48:39.000000 VSautomatic-2.5/VSautomatic/ReSTTerminal.py
+-rw-rw-rw-   0        0        0   842240 2018-07-25 04:16:14.000000 VSautomatic-2.5/VSautomatic/RedRat.dll
+-rw-rw-rw-   0        0        0    10752 2018-07-25 04:16:10.000000 VSautomatic-2.5/VSautomatic/RedRatHub.Connection.dll
+-rw-rw-rw-   0        0        0     1768 2023-05-15 09:48:39.000000 VSautomatic-2.5/VSautomatic/RedRatHub.py
+-rwxrwxrwx   0        0        0    14336 2018-07-25 04:16:16.000000 VSautomatic-2.5/VSautomatic/RedRatHubCmd.exe
+-rw-rw-rw-   0        0        0      146 2018-03-09 10:13:06.000000 VSautomatic-2.5/VSautomatic/RedRatHubCmd.exe.config
+-rw-rw-rw-   0        0        0    48640 2018-07-25 04:16:14.000000 VSautomatic-2.5/VSautomatic/RedRatHubCore.dll
+-rw-rw-rw-   0        0        0     1052 2023-05-16 05:16:48.000000 VSautomatic-2.5/VSautomatic/RedRatHubS.py
+-rw-rw-rw-   0        0        0     2522 2023-05-15 09:48:39.000000 VSautomatic-2.5/VSautomatic/TestCfgParse.py
+-rw-rw-rw-   0        0        0    48335 2018-11-01 05:37:28.000000 VSautomatic-2.5/VSautomatic/Vizio.xml
+-rw-rw-rw-   0        0        0    14450 2022-03-17 01:56:03.000000 VSautomatic-2.5/VSautomatic/Vizio_IR.xml
+-rw-rw-rw-   0        0        0      154 2023-05-15 09:48:39.000000 VSautomatic-2.5/VSautomatic/__init__.py
+-rw-rw-rw-   0        0        0     1121 2023-05-15 09:48:39.000000 VSautomatic-2.5/VSautomatic/deco.py
+-rw-rw-rw-   0        0        0     3230 2023-05-15 09:48:39.000000 VSautomatic-2.5/VSautomatic/my_serial.py
+-rw-rw-rw-   0        0        0       81 2023-05-15 06:49:02.000000 VSautomatic-2.5/VSautomatic/restlog.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 08:02:43.315146 VSautomatic-2.5/VSautomatic.egg-info/
+-rw-rw-rw-   0        0        0      259 2023-05-18 08:02:42.000000 VSautomatic-2.5/VSautomatic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      831 2023-05-18 08:02:42.000000 VSautomatic-2.5/VSautomatic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 08:02:42.000000 VSautomatic-2.5/VSautomatic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-05-18 08:02:42.000000 VSautomatic-2.5/VSautomatic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-18 08:02:42.000000 VSautomatic-2.5/VSautomatic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 08:02:43.315146 VSautomatic-2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1111 2023-05-18 08:02:34.000000 VSautomatic-2.5/setup.py
```

### Comparing `VSautomatic-2.4/VSautomatic/DeviceDB.xml` & `VSautomatic-2.5/VSautomatic/DeviceDB.xml`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.4/VSautomatic/Dictionary.txt` & `VSautomatic-2.5/VSautomatic/Dictionary.txt`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.4/VSautomatic/IR_Remote.xml` & `VSautomatic-2.5/VSautomatic/IR_Remote.xml`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.4/VSautomatic/MacroList.xml` & `VSautomatic-2.5/VSautomatic/MacroList.xml`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.4/VSautomatic/MyCamera.py` & `VSautomatic-2.5/VSautomatic/MyCamera.py`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.4/VSautomatic/MyRedRat.py` & `VSautomatic-2.5/VSautomatic/MyRedRat.py`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.4/VSautomatic/MyTools.py` & `VSautomatic-2.5/VSautomatic/MyTools.py`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.4/VSautomatic/NLog.config` & `VSautomatic-2.5/VSautomatic/NLog.config`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.4/VSautomatic/NLog.dll` & `VSautomatic-2.5/VSautomatic/NLog.dll`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.4/VSautomatic/ReSTTerminal.py` & `VSautomatic-2.5/VSautomatic/ReSTTerminal.py`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.4/VSautomatic/RedRat.dll` & `VSautomatic-2.5/VSautomatic/RedRat.dll`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.4/VSautomatic/RedRatHub.Connection.dll` & `VSautomatic-2.5/VSautomatic/RedRatHub.Connection.dll`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.4/VSautomatic/RedRatHub.py` & `VSautomatic-2.5/VSautomatic/RedRatHub.py`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.4/VSautomatic/RedRatHubCmd.exe` & `VSautomatic-2.5/VSautomatic/RedRatHubCmd.exe`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.4/VSautomatic/RedRatHubCore.dll` & `VSautomatic-2.5/VSautomatic/RedRatHubCore.dll`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.4/VSautomatic/RedRatHubS.py` & `VSautomatic-2.5/VSautomatic/RedRatHubS.py`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.4/VSautomatic/TestCfgParse.py` & `VSautomatic-2.5/VSautomatic/TestCfgParse.py`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.4/VSautomatic/Vizio.xml` & `VSautomatic-2.5/VSautomatic/Vizio.xml`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.4/VSautomatic/Vizio_IR.xml` & `VSautomatic-2.5/VSautomatic/Vizio_IR.xml`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.4/VSautomatic/deco.py` & `VSautomatic-2.5/VSautomatic/deco.py`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.4/VSautomatic/my_serial.py` & `VSautomatic-2.5/VSautomatic/my_serial.py`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.4/VSautomatic.egg-info/SOURCES.txt` & `VSautomatic-2.5/VSautomatic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.4/setup.py` & `VSautomatic-2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
  
 # requirements = ['numpy']       # 自定义工具中需要的依赖包
  
 setuptools.setup(
     name="VSautomatic",       # 自定义工具包的名字
-    version="2.4",             # 版本号
+    version="2.5",             # 版本号
     author="jasonliu",           # 作者名字
     author_email="batianhu4444@gmail.com",  # 作者邮箱
     description="VS Automatic Tools", # 自定义工具包的简介
     license='MIT-0',           # 许可协议
     url="https://pypi.org/manage/projects/",              # 项目开源地址
     packages=setuptools.find_packages(),  # 自动发现自定义工具包中的所有包和子包
     install_requires=['robotframework','robotframework-ride','robotframework-sshlibrary','robotframework-seriallibrary'],  # 安装自定义工具包需要依赖的包
```

