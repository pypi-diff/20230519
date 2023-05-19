# Comparing `tmp/Lshengpackage-0.4.4.tar.gz` & `tmp/Lshengpackage-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lshengpackage-0.4.4.tar", last modified: Thu May 18 16:36:31 2023, max compression
+gzip compressed data, was "Lshengpackage-0.4.5.tar", last modified: Fri May 19 06:23:13 2023, max compression
```

## Comparing `Lshengpackage-0.4.4.tar` & `Lshengpackage-0.4.5.tar`

### file list

```diff
@@ -1,48 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 16:36:31.212079 Lshengpackage-0.4.4/
--rw-rw-rw-   0        0        0     1079 2022-05-04 09:06:22.000000 Lshengpackage-0.4.4/LICENSE
--rw-rw-rw-   0        0        0     1077 2022-05-04 09:06:22.000000 Lshengpackage-0.4.4/License.md
-drwxrwxrwx   0        0        0        0 2023-05-18 16:36:31.140798 Lshengpackage-0.4.4/Lshengpackage/
--rw-rw-rw-   0        0        0      550 2023-05-18 16:33:59.000000 Lshengpackage-0.4.4/Lshengpackage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 16:36:31.157899 Lshengpackage-0.4.4/Lshengpackage/simulate/
--rw-rw-rw-   0        0        0       51 2023-05-18 15:10:46.000000 Lshengpackage-0.4.4/Lshengpackage/simulate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 16:36:31.162900 Lshengpackage-0.4.4/Lshengpackage/simulate/adb/
--rw-rw-rw-   0        0        0     3318 2023-05-17 13:41:00.000000 Lshengpackage-0.4.4/Lshengpackage/simulate/adb/Command_adb.py
--rw-rw-rw-   0        0        0       49 2023-05-18 15:10:46.000000 Lshengpackage-0.4.4/Lshengpackage/simulate/adb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 16:36:31.164901 Lshengpackage-0.4.4/Lshengpackage/simulate/adb/__pycache__/
--rw-rw-rw-   0        0        0      162 2022-10-10 08:45:14.000000 Lshengpackage-0.4.4/Lshengpackage/simulate/adb/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-05-18 16:36:31.171424 Lshengpackage-0.4.4/Lshengpackage/simulate/adb/dingtalk/
--rw-rw-rw-   0        0        0       51 2022-10-10 06:18:05.000000 Lshengpackage-0.4.4/Lshengpackage/simulate/adb/dingtalk/__init__.py
--rw-rw-rw-   0        0        0     7619 2023-05-18 16:25:46.000000 Lshengpackage-0.4.4/Lshengpackage/simulate/adb/dingtalk/dingtalk_api.py
--rw-rw-rw-   0        0        0  3646951 2023-05-17 12:12:22.000000 Lshengpackage-0.4.4/Lshengpackage/simulate/adb/dingtalk/image_data.py
--rw-rw-rw-   0        0        0     1631 2023-05-18 16:25:46.000000 Lshengpackage-0.4.4/Lshengpackage/simulate/adb/re_Pic.py
-drwxrwxrwx   0        0        0        0 2023-05-18 16:36:31.186943 Lshengpackage-0.4.4/Lshengpackage/simulate/dm/
--rw-rw-rw-   0        0        0     4683 2023-05-18 16:25:46.000000 Lshengpackage-0.4.4/Lshengpackage/simulate/dm/Pac_dm.py
--rw-rw-rw-   0        0        0      314 2023-05-14 01:06:32.000000 Lshengpackage-0.4.4/Lshengpackage/simulate/dm/Reg.py
--rw-rw-rw-   0        0        0     9334 2022-05-04 09:06:22.000000 Lshengpackage-0.4.4/Lshengpackage/simulate/dm/Win_dm.py
--rw-rw-rw-   0        0        0       49 2022-10-10 06:18:05.000000 Lshengpackage-0.4.4/Lshengpackage/simulate/dm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 16:36:31.195966 Lshengpackage-0.4.4/Lshengpackage/simulate/dm/__pycache__/
--rw-rw-rw-   0        0        0     4816 2022-10-10 08:45:14.000000 Lshengpackage-0.4.4/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc
--rw-rw-rw-   0        0        0      565 2022-10-10 08:45:14.000000 Lshengpackage-0.4.4/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc
--rw-rw-rw-   0        0        0     1262 2022-10-10 08:45:14.000000 Lshengpackage-0.4.4/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc
--rw-rw-rw-   0        0        0      161 2022-10-10 08:45:14.000000 Lshengpackage-0.4.4/Lshengpackage/simulate/dm/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      286 2023-05-18 05:41:23.000000 Lshengpackage-0.4.4/Lshengpackage/simulate/mock_findFr.py
--rw-rw-rw-   0        0        0     2395 2023-05-18 16:25:46.000000 Lshengpackage-0.4.4/Lshengpackage/simulate/mock_findPic.py
-drwxrwxrwx   0        0        0        0 2023-05-18 16:36:31.210079 Lshengpackage-0.4.4/Lshengpackage/tools/
--rw-rw-rw-   0        0        0     1988 2022-05-26 11:29:53.000000 Lshengpackage-0.4.4/Lshengpackage/tools/ChaoJiYing.py
--rw-rw-rw-   0        0        0      757 2023-05-18 15:10:46.000000 Lshengpackage-0.4.4/Lshengpackage/tools/General.py
--rw-rw-rw-   0        0        0     1687 2023-05-18 16:25:46.000000 Lshengpackage-0.4.4/Lshengpackage/tools/Loading.py
--rw-rw-rw-   0        0        0     3311 2023-05-18 14:57:22.000000 Lshengpackage-0.4.4/Lshengpackage/tools/OperateFile.py
--rw-rw-rw-   0        0        0     2055 2023-05-18 05:41:23.000000 Lshengpackage-0.4.4/Lshengpackage/tools/SearchFile.py
--rw-rw-rw-   0        0        0       49 2023-05-18 16:20:17.000000 Lshengpackage-0.4.4/Lshengpackage/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 16:36:31.150795 Lshengpackage-0.4.4/Lshengpackage.egg-info/
--rw-rw-rw-   0        0        0      858 2023-05-18 16:36:30.000000 Lshengpackage-0.4.4/Lshengpackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1308 2023-05-18 16:36:30.000000 Lshengpackage-0.4.4/Lshengpackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 16:36:30.000000 Lshengpackage-0.4.4/Lshengpackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-05-18 16:36:30.000000 Lshengpackage-0.4.4/Lshengpackage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-18 16:36:30.000000 Lshengpackage-0.4.4/Lshengpackage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      299 2023-05-17 15:14:59.000000 Lshengpackage-0.4.4/MANIFEST.in
--rw-rw-rw-   0        0        0      858 2023-05-18 16:36:31.212079 Lshengpackage-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     3975 2023-05-14 07:50:08.000000 Lshengpackage-0.4.4/README.md
--rw-rw-rw-   0        0        0      350 2023-05-14 03:44:13.000000 Lshengpackage-0.4.4/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-05-18 16:36:31.216078 Lshengpackage-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1987 2023-05-18 16:36:21.000000 Lshengpackage-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.264726 Lshengpackage-0.4.5/
+-rw-rw-rw-   0        0        0     1079 2022-05-04 09:06:22.000000 Lshengpackage-0.4.5/LICENSE
+-rw-rw-rw-   0        0        0     1077 2022-05-04 09:06:22.000000 Lshengpackage-0.4.5/License.md
+drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.206652 Lshengpackage-0.4.5/Lshengpackage/
+-rw-rw-rw-   0        0        0      550 2023-05-18 16:33:59.000000 Lshengpackage-0.4.5/Lshengpackage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.216244 Lshengpackage-0.4.5/Lshengpackage/simulate/
+-rw-rw-rw-   0        0        0       51 2023-05-18 15:10:46.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.221179 Lshengpackage-0.4.5/Lshengpackage/simulate/__pycache__/
+-rw-rw-rw-   0        0        0      162 2023-05-19 03:15:17.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      428 2023-05-19 03:15:17.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/__pycache__/mock_findFr.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1717 2023-05-19 03:26:52.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/__pycache__/mock_findPic.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.223689 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/
+-rw-rw-rw-   0        0        0     3313 2023-05-19 03:03:37.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/Command_adb.py
+-rw-rw-rw-   0        0        0       49 2023-05-18 15:10:46.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.227234 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/__pycache__/
+-rw-rw-rw-   0        0        0     3855 2023-05-19 03:15:18.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/__pycache__/Command_adb.cpython-39.pyc
+-rw-rw-rw-   0        0        0      166 2023-05-19 03:15:18.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2290 2023-05-19 03:16:36.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/__pycache__/re_Pic.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.231221 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/dingtalk/
+-rw-rw-rw-   0        0        0       51 2022-10-10 06:18:05.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/dingtalk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.234221 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/dingtalk/__pycache__/
+-rw-rw-rw-   0        0        0      175 2023-05-19 03:16:36.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/dingtalk/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6503 2023-05-19 03:16:36.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/dingtalk/__pycache__/dingtalk_api.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8853 2023-05-19 05:56:20.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/dingtalk/dingtalk_api.py
+-rw-rw-rw-   0        0        0     3059 2023-05-19 03:37:17.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/re_Pic.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.238533 Lshengpackage-0.4.5/Lshengpackage/simulate/dm/
+-rw-rw-rw-   0        0        0     4683 2023-05-18 16:25:46.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/dm/Pac_dm.py
+-rw-rw-rw-   0        0        0      314 2023-05-14 01:06:32.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/dm/Reg.py
+-rw-rw-rw-   0        0        0     9334 2022-05-04 09:06:22.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/dm/Win_dm.py
+-rw-rw-rw-   0        0        0       49 2022-10-10 06:18:05.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/dm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.244057 Lshengpackage-0.4.5/Lshengpackage/simulate/dm/__pycache__/
+-rw-rw-rw-   0        0        0     4828 2023-05-19 03:16:36.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc
+-rw-rw-rw-   0        0        0      160 2023-05-19 03:16:36.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1262 2022-10-10 08:45:14.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc
+-rw-rw-rw-   0        0        0      161 2022-10-10 08:45:14.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/dm/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      286 2023-05-18 05:41:23.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/mock_findFr.py
+-rw-rw-rw-   0        0        0     2554 2023-05-19 03:34:10.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/mock_findPic.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.257730 Lshengpackage-0.4.5/Lshengpackage/tools/
+-rw-rw-rw-   0        0        0     1988 2022-05-26 11:29:53.000000 Lshengpackage-0.4.5/Lshengpackage/tools/ChaoJiYing.py
+-rw-rw-rw-   0        0        0      757 2023-05-18 15:10:46.000000 Lshengpackage-0.4.5/Lshengpackage/tools/General.py
+-rw-rw-rw-   0        0        0     2019 2023-05-19 03:47:29.000000 Lshengpackage-0.4.5/Lshengpackage/tools/Loading.py
+-rw-rw-rw-   0        0        0     3311 2023-05-18 14:57:22.000000 Lshengpackage-0.4.5/Lshengpackage/tools/OperateFile.py
+-rw-rw-rw-   0        0        0     2055 2023-05-18 05:41:23.000000 Lshengpackage-0.4.5/Lshengpackage/tools/SearchFile.py
+-rw-rw-rw-   0        0        0       49 2023-05-18 16:20:17.000000 Lshengpackage-0.4.5/Lshengpackage/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.264726 Lshengpackage-0.4.5/Lshengpackage/tools/__pycache__/
+-rw-rw-rw-   0        0        0     1982 2023-05-19 03:16:35.000000 Lshengpackage-0.4.5/Lshengpackage/tools/__pycache__/ChaoJiYing.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1167 2023-05-19 03:16:35.000000 Lshengpackage-0.4.5/Lshengpackage/tools/__pycache__/General.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1431 2023-05-19 03:16:35.000000 Lshengpackage-0.4.5/Lshengpackage/tools/__pycache__/Loading.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2530 2023-05-19 03:16:35.000000 Lshengpackage-0.4.5/Lshengpackage/tools/__pycache__/OperateFile.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1282 2023-05-19 03:16:36.000000 Lshengpackage-0.4.5/Lshengpackage/tools/__pycache__/SearchFile.cpython-39.pyc
+-rw-rw-rw-   0        0        0      159 2023-05-19 03:16:35.000000 Lshengpackage-0.4.5/Lshengpackage/tools/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.212662 Lshengpackage-0.4.5/Lshengpackage.egg-info/
+-rw-rw-rw-   0        0        0      858 2023-05-19 06:23:13.000000 Lshengpackage-0.4.5/Lshengpackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2058 2023-05-19 06:23:13.000000 Lshengpackage-0.4.5/Lshengpackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 06:23:13.000000 Lshengpackage-0.4.5/Lshengpackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-05-19 06:23:13.000000 Lshengpackage-0.4.5/Lshengpackage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-19 06:23:13.000000 Lshengpackage-0.4.5/Lshengpackage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      299 2023-05-17 15:14:59.000000 Lshengpackage-0.4.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      858 2023-05-19 06:23:13.264726 Lshengpackage-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3975 2023-05-14 07:50:08.000000 Lshengpackage-0.4.5/README.md
+-rw-rw-rw-   0        0        0      350 2023-05-14 03:44:13.000000 Lshengpackage-0.4.5/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-05-19 06:23:13.267246 Lshengpackage-0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     1987 2023-05-19 05:56:20.000000 Lshengpackage-0.4.5/setup.py
```

### Comparing `Lshengpackage-0.4.4/LICENSE` & `Lshengpackage-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.4/License.md` & `Lshengpackage-0.4.5/License.md`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.4/Lshengpackage/__init__.py` & `Lshengpackage-0.4.5/Lshengpackage/__init__.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.4/Lshengpackage/simulate/adb/Command_adb.py` & `Lshengpackage-0.4.5/Lshengpackage/simulate/adb/Command_adb.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,10 +106,10 @@
         """
         模拟滑动操作
         """
         com = os.system('adb shell input swipe {} {} {} {}'.format(x, y, x2, y2))
         return com
 
     def get_ui(self, path):
-        re = os.popen('adb shell uiautomator dump /sdcard/ui.xml')  # 获得屏幕控件信息
+        os.popen('adb shell uiautomator dump /sdcard/ui.xml')  # 获得屏幕控件信息
         re = os.popen(r'adb pull /sdcard/ui.xml {}+ui.xml'.format(path))  # 获得屏幕控件信息
         return re
```

### Comparing `Lshengpackage-0.4.4/Lshengpackage/simulate/adb/dingtalk/dingtalk_api.py` & `Lshengpackage-0.4.5/Lshengpackage/simulate/adb/dingtalk/dingtalk_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # -*- coding: UTF-8 -*-
 import os
+import pickle
+import sys
 from time import sleep
 
 from Lshengpackage.simulate.adb.Command_adb import command
-from Lshengpackage.simulate.adb.re_Pic import refind_image, refiinsclick_image, refiloadclick_image, refiload_image
+from Lshengpackage.simulate.adb.re_Pic import refind_image, refiinsclick_image, refiload_image, refiloadclick_image
 
 
 # 检测当前连接状态
 def connect_status_api():
     state = os.popen('adb get-state').read()  # ddddddddddd
     if state[0:7] == 'unknown':
         print('未检测到连接设备')
@@ -31,127 +33,136 @@
 # 检测dingding当前界面
 def ding_current_api(fol_path, path, _system):
     # Lshengpackage.simulate.adb.Command_adb.command().tap_work(419,953)
     sleep(0.1)
     if refind_image(fol_path, path, 'is_msg', _system) is not None:
         print('******当前页面为消息页******')
         return '消息页'
-    elif refind_image(fol_path, path, 'is_tooge', _system) is not None:
+    elif refind_image(fol_path, path, 'is_tooge', _system, screenshot=False) is not None:
         print('******当前页面为协作页******')
         return '协作页'
-    elif refind_image(fol_path, path, 'is_work', _system) is not None:
+    elif refind_image(fol_path, path, 'is_work', _system, screenshot=False) is not None:
         print('******当前页面为办公页******')
         return '办公页'
-    elif refind_image(fol_path, path, 'is_iph', _system) is not None:
+    elif refind_image(fol_path, path, 'is_iph', _system, screenshot=False) is not None:
         print('******当前页面为通讯页******')
         return '通讯页'
-    elif refind_image(fol_path, path, 'is_my', _system) is not None:
+    elif refind_image(fol_path, path, 'is_my', _system, screenshot=False) is not None:
         print('******当前页面为个人页******')
         return '个人页'
-    elif refind_image(fol_path, path, 'is_exa', _system) is not None:
+    elif refind_image(fol_path, path, 'is_exa', _system, screenshot=False) is not None:
         print('******当前页面为自查页,立即返回主程序******')
 
-        refiinsclick_image(fol_path, path, 'tureok', _system)
-        refiinsclick_image(fol_path, path, 'exit', _system)
+        refiinsclick_image(fol_path, path, 'tureok', _system, screenshot=False)
+        refiinsclick_image(fol_path, path, 'exit', _system,screenshot=False)
         sleep(0.1)
         ding_current_api(fol_path, path, _system)
-    elif refind_image(fol_path, path, 'is_answer', _system) is not None:
+    elif refind_image(fol_path, path, 'is_answer', _system, screenshot=False) is not None:
         print('******当前页面为答题页,立即返回主程序******')
-        refiinsclick_image(fol_path, path, 'tureok', _system)
-        refiloadclick_image(fol_path, path, 'exit', _system)
+        refiinsclick_image(fol_path, path, 'tureok', _system,screenshot=False)
+        refiinsclick_image(fol_path, path, 'exit', _system,screenshot=False)
         sleep(0.1)
         ding_current_api(fol_path, path, _system)
 
 
 # 打开应用接口 #答题 op_answer.png 自查 op_exaself.png
 def open_app_api(fol_path, path, _system, op_name):  # op_name op的名
-    xy = refiinsclick_image(fol_path, path, 'is_work', _system)
-    if xy is False:
-        refiinsclick_image(fol_path, path, 'work', _system)
+    xy = refind_image(fol_path, path, 'is_work', _system)
+    if xy is None:
+        refiinsclick_image(fol_path, path, 'work', _system, screenshot=False)
     else:
         pass
     refiload_image(fol_path, path, 'op_answer', _system)
-    op_answer = refiinsclick_image(fol_path, path, op_name, _system)
+    sleep(1)
+    op_answer = refiinsclick_image(fol_path, path, op_name, _system, screenshot=False)
 
     if op_answer is False:
-        is_work = refind_image(fol_path, path, 'is_work', _system)
+        is_work = refind_image(fol_path, path, 'is_work', _system, screenshot=False)
         if is_work is not None:
             command().swip_work(int(is_work[0]), int(is_work[1] - 400), int(is_work[0]), int(is_work[1]))
     else:
         print('{}页已打开,持续更近中'.format(op_name))
         return True
-    for i in range(2):
+    for i in range(3):
         op_answer = refind_image(fol_path, path, op_name, _system)
         if op_answer is None:
             sleep(0.1)
-            is_work = refind_image(fol_path, path, 'is_work', _system)
             command().swip_work(int(is_work[0]), int(is_work[1] - 200), int(is_work[0]), int(is_work[1] - 500))
         else:
-            op_answer = refiinsclick_image(fol_path, path, op_name, _system)
+            op_answer = refiinsclick_image(fol_path, path, op_name, _system, screenshot=False)
             print('{}页已打开,持续更近中'.format(op_name))
             return True
+    print('找不到应用，退出程序')
+    sys.exit()
 
 
 # 安全答题程序执行程序接口
-def do_answer_api(fol_path, path, _system):
+def do_answer_api(fol_path, path, _system, int_x=0, int_y=540, width=1920, high=540, sw_high=100, sw_highA=40):
     refiload_image(fol_path, path, 'do_answer', _system)
-    sleep(0.5)
-
-    do_fi_answer = refind_image(fol_path, path, 'do_fi_answer', _system)
+    do_fi_answer = refind_image(fol_path, path, 'do_fi_answer', _system, screenshot=False)
     if do_fi_answer is not None:  # 处理上次记忆时间
         pass
     else:
         refiloadclick_image(fol_path, path, 'do_answer', _system)
     refiinsclick_image(fol_path, path, 'do_fi_answer', _system)
     sleep(0.1)
 
     lo = refiload_image(fol_path, path, 'do_fi_ti_answer', _system)  # 加载
+    sleep(0.5)
     v = 0
     for i in range(5):
         v += 1
-        refiinsclick_image(fol_path, path, 'push', _system)  # 加载
+        refiinsclick_image(fol_path, path, 'push', _system, screenshot=False)  # 加载
 
-        _upup(fol_path, path, _system, a=v)
+        _upup(fol_path, path, _system, sw_high, a=v)
 
-        answer(fol_path, path, _system)
+        answer(fol_path, path, _system, int_x, int_y, width, high, sw_highA)
     refiloadclick_image(fol_path, path, 'update', _system)
-    refiload_image(fol_path, path, 'answer_over', _system)
-    print('答题成功！！！')
-    refiinsclick_image(fol_path, path, 'exit', _system)  # 加载
-    refiloadclick_image(fol_path, path, 'ose', _system)
+    while True:
+        already = refind_image(fol_path, path, 'answer_already', _system)
+        if already is not None:
+            print('重复答题,退出')
+            refiinsclick_image(fol_path, path, 'exit', _system, screenshot=False)  # 加载
+            refiloadclick_image(fol_path, path, 'ose', _system)
+            break
+        else:
+            answer_over = refind_image(fol_path, path, 'answer_over', _system, screenshot=False)
+            if answer_over is not None:
+                print('答题任务完成！！！')
+                refiinsclick_image(fol_path, path, 'exit', _system)  # 加载
+                break
+            else:
+                sleep(1)
 
 
-def _upup(fol_path, path, _system, a):
+def _upup(fol_path, path, _system, sw_high, a):
     while True:
 
         sh = refiload_image(fol_path, path, 'shouqi', _system)  # 加载
         print(sh)
-        command().swip_work(int(sh[0]), int(sh[1]), int(sh[0]), int(sh[1] - 100))
+        command().swip_work(int(sh[0]), int(sh[1]), int(sh[0]), int(sh[1] - sw_high))
 
         pu = refind_image(fol_path, path, 'push', _system)  # 加载
         print(pu)
         if pu is not None:
             return True
         else:
             if a == 5:
                 command().swip_work(int(sh[0]), int(sh[1]), int(sh[0]), int(sh[1] - 500))
                 return True
 
 
-def answer(fol_path, path, _system):
+def answer(fol_path, path, _system, int_x, int_y, width, high, sw_high):
     for i in ['A', 'B', 'C', 'D']:
 
-        select = refind_image(fol_path, path, 'select', _system, int_x1=0, int_y1=540, int_x2=1920,
-                              int_y2=1080)
-        command().tap_work(int(select[0]), int(select[1] + 40))
+        select = refind_image(fol_path, path, 'select', _system, int_x, int_y, width, high)
+        command().tap_work(int(select[0]), int(select[1] + sw_high))
         refiloadclick_image(fol_path, path, '{}'.format(i), _system)  # 加载
         sleep(0.2)
-
-        yesok = refind_image(fol_path, path, 'yesok', _system, int_x1=0, int_y1=540, int_x2=1920,
-                             int_y2=1080)
+        yesok = refind_image(fol_path, path, 'yesok', _system, int_x, int_y, width, high)
         if yesok is not None:
             return True
 
 
 # 每日安全自查程序接口
 def do_checkself_api(fol_path, path, _system):
     sleep(0.3)
@@ -187,11 +198,22 @@
             if ye is False:
                 break
         sleep(0.1)
 
         ye = refind_image(fol_path, path, 'saferope', _system)
         if ye is not None:
             break
-    refiloadclick_image(fol_path, path, 'update', _system)
-    refiload_image(fol_path, path, 'selfsafe_over', _system)
-    print('自查成功！！！')
+    refiloadclick_image(fol_path, path, 'update', _system,screenshot=False)
+    while True:
+        already = refind_image(fol_path, path, 'self_already', _system)
+        if already is not None:
+            print('重复自查,退出')
+            break
+        else:
+            selfsafe_over = refind_image(fol_path, path, 'selfsafe_over', _system, screenshot=False)
+            if selfsafe_over is not None:
+                print('自查任务完成！！！')
+                break
+            else:
+                sleep(1)
+
     refiinsclick_image(fol_path, path, 'exit', _system)
```

### Comparing `Lshengpackage-0.4.4/Lshengpackage/simulate/dm/Pac_dm.py` & `Lshengpackage-0.4.5/Lshengpackage/simulate/dm/Pac_dm.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.4/Lshengpackage/simulate/dm/Win_dm.py` & `Lshengpackage-0.4.5/Lshengpackage/simulate/dm/Win_dm.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.4/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc` & `Lshengpackage-0.4.5/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed May  4 09:06:22 2022 UTC, .py size: 4677 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 0e42 7262 4512 0000  a........BrbE...
+00000000: 610d 0d0a 0000 0000 8a51 6664 4b12 0000  a........QfdK...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 8302 5a02 4700 6404 6405 8400  ..d...Z.G.d.d...
 00000050: 6405 8302 5a03 4700 6406 6407 8400 6407  d...Z.G.d.d...d.
 00000060: 8302 5a04 4700 6408 6409 8400 6409 8302  ..Z.G.d.d...d...
 00000070: 5a05 640a 5300 290b e900 0000 0029 01da  Z.d.S.)......)..
@@ -17,285 +17,286 @@
 00000100: 0000 0400 0000 0200 0000 4300 0000 7316  ..........C...s.
 00000110: 0000 007c 017c 005f 007c 027c 005f 017c  ...|.|._.|.|._.|
 00000120: 037c 005f 0264 0053 00a9 014e 2903 da0e  .|._.d.S...N)...
 00000130: 5f6d 6f75 7365 5f5f 646d 5f6f 626a da0a  _mouse__dm_obj..
 00000140: 7374 6172 745f 7469 6d65 da08 656e 645f  start_time..end_
 00000150: 7469 6d65 2904 da04 7365 6c66 da06 646d  time)...self..dm
 00000160: 5f6f 626a 7208 0000 0072 0900 0000 a900  _objr....r......
-00000170: 720c 0000 00f5 4100 0000 433a 5ce7 bc96  r.....A...C:\...
-00000180: e7a8 8be9 a1b9 e79b ae5c 4c53 6865 6e67  .........\LSheng
-00000190: 7061 636b 6167 655c 4c73 6865 6e67 7061  package\Lshengpa
-000001a0: 636b 6167 655c 7369 6d75 6c61 7465 5c64  ckage\simulate\d
-000001b0: 6d5c 5061 635f 646d 2e70 79da 085f 5f69  m\Pac_dm.py..__i
-000001c0: 6e69 745f 5f07 0000 0073 0600 0000 0001  nit__....s......
-000001d0: 0601 0601 7a0e 6d6f 7573 652e 5f5f 696e  ....z.mouse.__in
-000001e0: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
-000001f0: 0001 0000 0004 0000 0043 0000 0073 1e00  .........C...s..
-00000200: 0000 7400 a001 7c00 6a02 7c00 6a03 a102  ..t...|.j.|.j...
-00000210: 0100 7c00 6a04 a005 a100 0100 6401 5300  ..|.j.......d.S.
-00000220: 2902 751e 0000 000a 2020 2020 2020 2020  ).u.....        
-00000230: e5b7 a6e9 94ae e782 b9e5 87bb 0a20 2020  .............   
-00000240: 2020 2020 204e 2906 7202 0000 00da 0564       N).r......d
-00000250: 656c 6179 7208 0000 0072 0900 0000 7207  elayr....r....r.
-00000260: 0000 005a 094c 6566 7443 6c69 636b a901  ...Z.LeftClick..
-00000270: 720a 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
-00000280: 0d00 0000 da06 6c43 6c69 636b 0c00 0000  ......lClick....
-00000290: 7304 0000 0000 0410 017a 0c6d 6f75 7365  s........z.mouse
-000002a0: 2e6c 436c 6963 6b63 0100 0000 0000 0000  .lClickc........
-000002b0: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
-000002c0: 731e 0000 0074 00a0 017c 006a 027c 006a  s....t...|.j.|.j
-000002d0: 03a1 0201 007c 006a 04a0 05a1 0001 0064  .....|.j.......d
-000002e0: 0153 0029 0275 1e00 0000 0a20 2020 2020  .S.).u.....     
-000002f0: 2020 20e5 8fb3 e994 aee7 82b9 e587 bb0a     .............
-00000300: 2020 2020 2020 2020 4e29 0672 0200 0000          N).r....
-00000310: 720f 0000 0072 0800 0000 7209 0000 0072  r....r....r....r
-00000320: 0700 0000 5a0a 5269 6768 7443 6c69 636b  ....Z.RightClick
-00000330: 7210 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
-00000340: 0d00 0000 da06 7243 6c69 636b 1300 0000  ......rClick....
-00000350: 7304 0000 0000 0410 017a 0c6d 6f75 7365  s........z.mouse
-00000360: 2e72 436c 6963 6b63 0300 0000 0000 0000  .rClickc........
-00000370: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
-00000380: 732a 0000 007c 006a 00a0 017c 017c 02a1  s*...|.j...|.|..
-00000390: 0201 0074 02a0 037c 006a 047c 006a 05a1  ...t...|.j.|.j..
-000003a0: 0201 007c 00a0 06a1 0001 0064 0153 0029  ...|.......d.S.)
-000003b0: 0275 2100 0000 0a20 2020 2020 2020 20e7  .u!....        .
-000003c0: a7bb e58a a8e5 b9b6 e782 b9e5 87bb 0a20  ............... 
-000003d0: 2020 2020 2020 204e 2907 7207 0000 00da         N).r.....
-000003e0: 064d 6f76 6554 6f72 0200 0000 720f 0000  .MoveTor....r...
-000003f0: 0072 0800 0000 7209 0000 0072 1100 0000  .r....r....r....
-00000400: a903 720a 0000 00da 0569 6e74 5f78 da05  ..r......int_x..
-00000410: 696e 745f 7972 0c00 0000 720c 0000 0072  int_yr....r....r
-00000420: 0d00 0000 da0b 6d6f 7665 5f6c 436c 6963  ......move_lClic
-00000430: 6b1a 0000 0073 0600 0000 0004 0e01 1001  k....s..........
-00000440: 7a11 6d6f 7573 652e 6d6f 7665 5f6c 436c  z.mouse.move_lCl
-00000450: 6963 6b63 0300 0000 0000 0000 0000 0000  ickc............
-00000460: 0300 0000 0400 0000 4300 0000 732c 0000  ........C...s,..
-00000470: 007c 006a 00a0 017c 017c 02a1 0201 0074  .|.j...|.|.....t
-00000480: 02a0 037c 006a 047c 006a 05a1 0201 007c  ...|.j.|.j.....|
-00000490: 006a 00a0 06a1 0001 0064 0153 0029 0275  .j.......d.S.).u
-000004a0: 2100 0000 0a20 2020 2020 2020 20e7 a7bb  !....        ...
-000004b0: e58a a8e5 b9b6 e58f 8ce5 87bb 0a20 2020  .............   
-000004c0: 2020 2020 204e 2907 7207 0000 0072 1300       N).r....r..
-000004d0: 0000 7202 0000 0072 0f00 0000 7208 0000  ..r....r....r...
-000004e0: 0072 0900 0000 5a0f 4c65 6674 446f 7562  .r....Z.LeftDoub
-000004f0: 6c65 436c 6963 6b72 1400 0000 720c 0000  leClickr....r...
-00000500: 0072 0c00 0000 720d 0000 00da 116d 6f76  .r....r......mov
-00000510: 655f 646f 7562 6c65 5f63 6c69 636b 2200  e_double_click".
-00000520: 0000 7306 0000 0000 040e 0110 017a 176d  ..s..........z.m
-00000530: 6f75 7365 2e6d 6f76 655f 646f 7562 6c65  ouse.move_double
-00000540: 5f63 6c69 636b 4e29 0272 0400 0000 7205  _clickN).r....r.
-00000550: 0000 0029 08da 085f 5f6e 616d 655f 5fda  ...)...__name__.
-00000560: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00000570: 7561 6c6e 616d 655f 5f72 0e00 0000 7211  ualname__r....r.
-00000580: 0000 0072 1200 0000 7217 0000 0072 1800  ...r....r....r..
-00000590: 0000 720c 0000 0072 0c00 0000 720c 0000  ..r....r....r...
-000005a0: 0072 0d00 0000 7203 0000 0006 0000 0073  .r....r........s
-000005b0: 0a00 0000 0801 0a05 0807 0807 0808 7203  ..............r.
-000005c0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000005d0: 0000 0000 0300 0000 4000 0000 7328 0000  ........@...s(..
-000005e0: 0065 005a 0164 005a 0264 0164 0284 005a  .e.Z.d.Z.d.d...Z
-000005f0: 0364 0a64 0564 0684 015a 0464 0b64 0764  .d.d.d...Z.d.d.d
-00000600: 0884 015a 0564 0953 0029 0cda 0563 6f6c  ...Z.d.S.)...col
-00000610: 6f72 6302 0000 0000 0000 0000 0000 0002  orc.............
-00000620: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
-00000630: 7c01 7c00 5f00 6400 5300 7206 0000 0029  |.|._.d.S.r....)
-00000640: 01da 0e5f 636f 6c6f 725f 5f64 6d5f 6f62  ..._color__dm_ob
-00000650: 6aa9 0272 0a00 0000 720b 0000 0072 0c00  j..r....r....r..
-00000660: 0000 720c 0000 0072 0d00 0000 720e 0000  ..r....r....r...
-00000670: 002c 0000 0073 0200 0000 0001 7a0e 636f  .,...s......z.co
-00000680: 6c6f 722e 5f5f 696e 6974 5f5f e7cd cccc  lor.__init__....
-00000690: cccc ccec 3f72 0100 0000 6308 0000 0000  ....?r....c.....
-000006a0: 0000 0000 0000 0009 0000 0009 0000 0043  ...............C
-000006b0: 0000 0073 1c00 0000 7c00 6a00 a001 7c01  ...s....|.j...|.
-000006c0: 7c02 7c03 7c04 7c05 7c06 7c07 a107 7d08  |.|.|.|.|.|...}.
-000006d0: 7c08 5300 7206 0000 0029 0272 1d00 0000  |.S.r....).r....
-000006e0: da09 4669 6e64 436f 6c6f 7229 0972 0a00  ..FindColor).r..
-000006f0: 0000 da06 696e 745f 7831 da06 696e 745f  ....int_x1..int_
-00000700: 7931 da06 696e 745f 7832 da06 696e 745f  y1..int_x2..int_
-00000710: 7932 721c 0000 00da 0373 696d da06 6469  y2r......sim..di
-00000720: 7265 6374 da06 646d 5f72 6574 720c 0000  rect..dm_retr...
-00000730: 0072 0c00 0000 720d 0000 00da 0a66 696e  .r....r......fin
-00000740: 645f 636f 6c6f 722f 0000 0073 0400 0000  d_color/...s....
-00000750: 000a 1801 7a10 636f 6c6f 722e 6669 6e64  ....z.color.find
-00000760: 5f63 6f6c 6f72 6308 0000 0000 0000 0000  _colorc.........
-00000770: 0000 000b 0000 0009 0000 0043 0000 0073  ...........C...s
-00000780: 5200 0000 7c00 6a00 a001 7c01 7c02 7c03  R...|.j...|.|.|.
-00000790: 7c04 7c05 7c06 7c07 a107 7d08 7c08 6401  |.|.|.|...}.|.d.
-000007a0: 1900 6401 6b02 7228 6402 5300 7c08 6403  ..d.k.r(d.S.|.d.
-000007b0: 1900 7d09 7c08 6404 1900 7d0a 7402 7c00  ..}.|.d...}.t.|.
-000007c0: 6a00 8301 a003 7c09 7c0a a102 0100 6404  j.....|.|.....d.
-000007d0: 5300 6402 5300 2905 75f1 0000 000a 2020  S.d.S.).u.....  
-000007e0: 2020 2020 2020 e689 bee8 89b2 20e5 b9b6        ...... ...
-000007f0: 20e7 82b9 e587 bb0a 2020 2020 2020 2020   .......        
-00000800: 3a70 6172 616d 2069 6e74 5f78 313a 0a20  :param int_x1:. 
-00000810: 2020 2020 2020 203a 7061 7261 6d20 696e         :param in
-00000820: 745f 7931 3a0a 2020 2020 2020 2020 3a70  t_y1:.        :p
-00000830: 6172 616d 2069 6e74 5f78 323a 0a20 2020  aram int_x2:.   
-00000840: 2020 2020 203a 7061 7261 6d20 696e 745f       :param int_
-00000850: 7932 3a0a 2020 2020 2020 2020 3a70 6172  y2:.        :par
-00000860: 616d 2063 6f6c 6f72 3a20 e889 b2e5 bda9  am color: ......
-00000870: e6a0 bce5 bc8f 0a20 2020 2020 2020 203a  .......        :
-00000880: 7061 7261 6d20 7369 6d3a 0a20 2020 2020  param sim:.     
-00000890: 2020 203a 7061 7261 6d20 6469 7265 6374     :param direct
-000008a0: 3a0a 2020 2020 2020 2020 3a72 6574 7572  :.        :retur
-000008b0: 6e3a 20e6 8890 e58a 9f20 312c 20e5 a4b1  n: ...... 1, ...
-000008c0: e8b4 a520 300a 2020 2020 2020 2020 e9ff  ... 0.        ..
-000008d0: ffff ff4e 7201 0000 00e9 0100 0000 2904  ...Nr.........).
-000008e0: 721d 0000 0072 2000 0000 7203 0000 0072  r....r ...r....r
-000008f0: 1700 0000 290b 720a 0000 0072 2100 0000  ....).r....r!...
-00000900: 7222 0000 0072 2300 0000 7224 0000 0072  r"...r#...r$...r
-00000910: 1c00 0000 7225 0000 0072 2600 0000 7227  ....r%...r&...r'
-00000920: 0000 0072 1500 0000 7216 0000 0072 0c00  ...r....r....r..
-00000930: 0000 720c 0000 0072 0d00 0000 da10 6669  ..r....r......fi
-00000940: 6e64 5f63 6f6c 6f72 5f63 6c69 636b 3c00  nd_color_click<.
-00000950: 0000 730e 0000 0000 0c18 010c 0104 0208  ..s.............
-00000960: 0108 0112 017a 1663 6f6c 6f72 2e66 696e  .....z.color.fin
-00000970: 645f 636f 6c6f 725f 636c 6963 6b4e 2902  d_color_clickN).
-00000980: 721f 0000 0072 0100 0000 2902 721f 0000  r....r....).r...
-00000990: 0072 0100 0000 2906 7219 0000 0072 1a00  .r....).r....r..
-000009a0: 0000 721b 0000 0072 0e00 0000 7228 0000  ..r....r....r(..
-000009b0: 0072 2b00 0000 720c 0000 0072 0c00 0000  .r+...r....r....
-000009c0: 720c 0000 0072 0d00 0000 721c 0000 002b  r....r....r....+
-000009d0: 0000 0073 0600 0000 0801 0803 0a0d 721c  ...s..........r.
-000009e0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000009f0: 0000 0000 0300 0000 4000 0000 7328 0000  ........@...s(..
-00000a00: 0065 005a 0164 005a 0264 0164 0284 005a  .e.Z.d.Z.d.d...Z
-00000a10: 0364 0b64 0664 0784 015a 0464 0c64 0864  .d.d.d...Z.d.d.d
-00000a20: 0984 015a 0564 0a53 0029 0dda 0370 6963  ...Z.d.S.)...pic
-00000a30: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000a40: 0002 0000 0043 0000 0073 0a00 0000 7c01  .....C...s....|.
-00000a50: 7c00 5f00 6400 5300 7206 0000 0029 01da  |._.d.S.r....)..
-00000a60: 0c5f 7069 635f 5f64 6d5f 6f62 6a72 1e00  ._pic__dm_objr..
-00000a70: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
-00000a80: 0072 0e00 0000 5300 0000 7302 0000 0000  .r....S...s.....
-00000a90: 017a 0c70 6963 2e5f 5f69 6e69 745f 5fda  .z.pic.__init__.
-00000aa0: 0630 3030 3030 3072 1f00 0000 7201 0000  .000000r....r...
-00000ab0: 0063 0900 0000 0000 0000 0000 0000 0a00  .c..............
-00000ac0: 0000 0a00 0000 4300 0000 731e 0000 007c  ......C...s....|
-00000ad0: 006a 00a0 017c 017c 027c 037c 047c 057c  .j...|.|.|.|.|.|
-00000ae0: 067c 077c 08a1 087d 097c 0953 0029 0175  .|.|...}.|.S.).u
-00000af0: 0c01 0000 0a20 2020 2020 2020 20e6 89be  .....        ...
-00000b00: e59b be0a 2020 2020 2020 2020 3a70 6172  ....        :par
-00000b10: 616d 2069 6e74 5f78 313a 0a20 2020 2020  am int_x1:.     
-00000b20: 2020 203a 7061 7261 6d20 696e 745f 7931     :param int_y1
-00000b30: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
-00000b40: 2069 6e74 5f78 323a 0a20 2020 2020 2020   int_x2:.       
-00000b50: 203a 7061 7261 6d20 696e 745f 7932 3a0a   :param int_y2:.
-00000b60: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
-00000b70: 6963 5f6e 616d 653a 0a20 2020 2020 2020  ic_name:.       
-00000b80: 203a 7061 7261 6d20 6465 6c74 615f 636f   :param delta_co
-00000b90: 6c6f 723a 0a20 2020 2020 2020 203a 7061  lor:.        :pa
-00000ba0: 7261 6d20 7369 6d3a 0a20 2020 2020 2020  ram sim:.       
-00000bb0: 203a 7061 7261 6d20 6469 7265 6374 3a0a   :param direct:.
-00000bc0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00000bd0: 20e6 8890 e58a 9f20 e8bf 94e5 9b9e e59d   ...... ........
-00000be0: 90e6 a087 2c20 e5a4 b1e8 b4a5 202d 312c  ...., ...... -1,
-00000bf0: 202d 312c 202d 310a 2020 2020 2020 2020   -1, -1.        
-00000c00: 2902 722d 0000 00da 0846 696e 6450 6963  ).r-.....FindPic
-00000c10: 4529 0a72 0a00 0000 7221 0000 0072 2200  E).r....r!...r".
-00000c20: 0000 7223 0000 0072 2400 0000 da08 7069  ..r#...r$.....pi
-00000c30: 635f 6e61 6d65 da0b 6465 6c74 615f 636f  c_name..delta_co
-00000c40: 6c6f 7272 2500 0000 7226 0000 0072 2700  lorr%...r&...r'.
-00000c50: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
-00000c60: 00da 0866 696e 645f 7069 6356 0000 0073  ...find_picV...s
-00000c70: 0400 0000 000e 1a01 7a0c 7069 632e 6669  ........z.pic.fi
-00000c80: 6e64 5f70 6963 6309 0000 0000 0000 0000  nd_picc.........
-00000c90: 0000 000c 0000 000a 0000 0043 0000 0073  ...........C...s
-00000ca0: 5400 0000 7c00 6a00 a001 7c01 7c02 7c03  T...|.j...|.|.|.
-00000cb0: 7c04 7c05 7c06 7c07 7c08 a108 7d09 7c09  |.|.|.|.|...}.|.
-00000cc0: 6401 1900 6401 6b02 722a 6402 5300 7c09  d...d.k.r*d.S.|.
-00000cd0: 6403 1900 7d0a 7c09 6401 1900 7d0b 7402  d...}.|.d...}.t.
-00000ce0: 7c00 6a00 8301 a003 7c0a 7c0b a102 0100  |.j.....|.|.....
-00000cf0: 6403 5300 6402 5300 2904 7545 0000 000a  d.S.d.S.).uE....
-00000d00: 2020 2020 2020 2020 e689 bee5 9bbe e5b9          ........
-00000d10: b6e7 82b9 e587 bb0a 2020 2020 2020 2020  ........        
-00000d20: 3a72 6574 7572 6e3a 20e6 8890 e58a 9f20  :return: ...... 
-00000d30: 312c 20e5 a4b1 e8b4 a520 300a 2020 2020  1, ...... 0.    
-00000d40: 2020 2020 7229 0000 004e 722a 0000 0029      r)...Nr*...)
-00000d50: 0472 2d00 0000 722f 0000 0072 0300 0000  .r-...r/...r....
-00000d60: 7217 0000 0029 0c72 0a00 0000 7221 0000  r....).r....r!..
-00000d70: 0072 2200 0000 7223 0000 0072 2400 0000  .r"...r#...r$...
-00000d80: 7230 0000 0072 3100 0000 7225 0000 0072  r0...r1...r%...r
-00000d90: 2600 0000 7227 0000 0072 1500 0000 7216  &...r'...r....r.
-00000da0: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
-00000db0: 0000 da0e 6669 6e64 5f70 6963 5f63 6c69  ....find_pic_cli
-00000dc0: 636b 6700 0000 730e 0000 0000 051a 010c  ckg...s.........
-00000dd0: 0104 0208 0108 0112 017a 1270 6963 2e66  .........z.pic.f
-00000de0: 696e 645f 7069 635f 636c 6963 6b4e 2903  ind_pic_clickN).
-00000df0: 722e 0000 0072 1f00 0000 7201 0000 0029  r....r....r....)
-00000e00: 0372 2e00 0000 721f 0000 0072 0100 0000  .r....r....r....
-00000e10: 2906 7219 0000 0072 1a00 0000 721b 0000  ).r....r....r...
-00000e20: 0072 0e00 0000 7232 0000 0072 3300 0000  .r....r2...r3...
-00000e30: 720c 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
-00000e40: 0d00 0000 722c 0000 0052 0000 0073 0600  ....r,...R...s..
-00000e50: 0000 0801 0803 0a11 722c 0000 0063 0000  ........r,...c..
-00000e60: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-00000e70: 0000 4000 0000 7328 0000 0065 005a 0164  ..@...s(...e.Z.d
-00000e80: 005a 0264 0164 0284 005a 0364 0964 0464  .Z.d.d...Z.d.d.d
-00000e90: 0584 015a 0464 0a64 0664 0784 015a 0564  ...Z.d.d.d...Z.d
-00000ea0: 0853 0029 0bda 0477 6f72 6463 0200 0000  .S.)...wordc....
-00000eb0: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-00000ec0: 4300 0000 730a 0000 007c 017c 005f 0064  C...s....|.|._.d
-00000ed0: 0053 0072 0600 0000 2901 da0d 5f77 6f72  .S.r....)..._wor
-00000ee0: 645f 5f64 6d5f 6f62 6a72 1e00 0000 720c  d__dm_objr....r.
-00000ef0: 0000 0072 0c00 0000 720d 0000 0072 0e00  ...r....r....r..
-00000f00: 0000 7700 0000 7302 0000 0000 017a 0d77  ..w...s......z.w
-00000f10: 6f72 642e 5f5f 696e 6974 5f5f e79a 9999  ord.__init__....
-00000f20: 9999 99e9 3f63 0800 0000 0000 0000 0000  ....?c..........
-00000f30: 0000 0900 0000 0900 0000 4300 0000 731c  ..........C...s.
-00000f40: 0000 007c 006a 00a0 017c 017c 027c 037c  ...|.j...|.|.|.|
-00000f50: 047c 057c 067c 07a1 077d 087c 0853 0029  .|.|.|...}.|.S.)
-00000f60: 0175 1800 0000 0a20 2020 2020 2020 20e6  .u.....        .
-00000f70: 89be e5ad 970a 2020 2020 2020 2020 2902  ......        ).
-00000f80: 7235 0000 00da 0b46 696e 6453 7472 4661  r5.....FindStrFa
-00000f90: 7374 2909 720a 0000 0072 2100 0000 7222  st).r....r!...r"
-00000fa0: 0000 0072 2300 0000 7224 0000 00da 0873  ...r#...r$.....s
-00000fb0: 7472 5f6e 616d 65da 0c63 6f6c 6f72 5f66  tr_name..color_f
-00000fc0: 6f72 6d61 7472 2500 0000 7227 0000 0072  ormatr%...r'...r
-00000fd0: 0c00 0000 720c 0000 0072 0d00 0000 da09  ....r....r......
-00000fe0: 6669 6e64 5f77 6f72 647a 0000 0073 0400  find_wordz...s..
-00000ff0: 0000 0004 1801 7a0e 776f 7264 2e66 696e  ......z.word.fin
-00001000: 645f 776f 7264 6308 0000 0000 0000 0000  d_wordc.........
-00001010: 0000 000b 0000 0009 0000 0043 0000 0073  ...........C...s
-00001020: 5200 0000 7c00 6a00 a001 7c01 7c02 7c03  R...|.j...|.|.|.
-00001030: 7c04 7c05 7c06 7c07 a107 7d08 7c08 6401  |.|.|.|...}.|.d.
-00001040: 1900 6401 6b02 7228 6402 5300 7c08 6403  ..d.k.r(d.S.|.d.
-00001050: 1900 7d09 7c08 6404 1900 7d0a 7402 7c00  ..}.|.d...}.t.|.
-00001060: 6a00 8301 a003 7c09 7c0a a102 0100 6404  j.....|.|.....d.
-00001070: 5300 6402 5300 2905 75eb 0000 000a 2020  S.d.S.).u.....  
-00001080: 2020 2020 2020 e689 bee5 ad97 e5b9 b6e7        ..........
-00001090: 82b9 e587 bb0a 2020 2020 2020 2020 3a70  ......        :p
-000010a0: 6172 616d 2069 6e74 5f78 313a 0a20 2020  aram int_x1:.   
-000010b0: 2020 2020 203a 7061 7261 6d20 696e 745f       :param int_
-000010c0: 7931 3a0a 2020 2020 2020 2020 3a70 6172  y1:.        :par
-000010d0: 616d 2069 6e74 5f78 323a 0a20 2020 2020  am int_x2:.     
-000010e0: 2020 203a 7061 7261 6d20 696e 745f 7932     :param int_y2
-000010f0: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
-00001100: 2073 7472 5f6e 616d 653a 0a20 2020 2020   str_name:.     
-00001110: 2020 203a 7061 7261 6d20 636f 6c6f 725f     :param color_
-00001120: 666f 726d 6174 3a0a 2020 2020 2020 2020  format:.        
-00001130: 3a70 6172 616d 2073 696d 3a0a 2020 2020  :param sim:.    
-00001140: 2020 2020 3a72 6574 7572 6e3a 20e6 8890      :return: ...
-00001150: e58a 9f20 312c 20e5 a4b1 e8b4 a520 300a  ... 1, ...... 0.
-00001160: 2020 2020 2020 2020 7229 0000 004e 7201          r)...Nr.
-00001170: 0000 0072 2a00 0000 2904 7235 0000 0072  ...r*...).r5...r
-00001180: 3700 0000 7203 0000 0072 1700 0000 290b  7...r....r....).
-00001190: 720a 0000 0072 2100 0000 7222 0000 0072  r....r!...r"...r
-000011a0: 2300 0000 7224 0000 0072 3800 0000 7239  #...r$...r8...r9
-000011b0: 0000 0072 2500 0000 7227 0000 0072 1500  ...r%...r'...r..
-000011c0: 0000 7216 0000 0072 0c00 0000 720c 0000  ..r....r....r...
-000011d0: 0072 0d00 0000 da0f 6669 6e64 5f77 6f72  .r......find_wor
-000011e0: 645f 636c 6963 6b81 0000 0073 0e00 0000  d_click....s....
-000011f0: 000c 1801 0c01 0402 0801 0801 1201 7a14  ..............z.
-00001200: 776f 7264 2e66 696e 645f 776f 7264 5f63  word.find_word_c
-00001210: 6c69 636b 4e29 0172 3600 0000 2901 7236  lickN).r6...).r6
-00001220: 0000 0029 0672 1900 0000 721a 0000 0072  ...).r....r....r
-00001230: 1b00 0000 720e 0000 0072 3a00 0000 723b  ....r....r:...r;
-00001240: 0000 0072 0c00 0000 720c 0000 0072 0c00  ...r....r....r..
-00001250: 0000 720d 0000 0072 3400 0000 7600 0000  ..r....r4...v...
-00001260: 7306 0000 0008 0108 030a 0772 3400 0000  s..........r4...
-00001270: 4e29 06da 134c 7368 656e 6770 6163 6b61  N)...Lshengpacka
-00001280: 6765 2e44 656c 6179 7202 0000 0072 0300  ge.Delayr....r..
-00001290: 0000 721c 0000 0072 2c00 0000 7234 0000  ..r....r,...r4..
-000012a0: 0072 0c00 0000 720c 0000 0072 0c00 0000  .r....r....r....
-000012b0: 720d 0000 00da 083c 6d6f 6475 6c65 3e03  r......<module>.
-000012c0: 0000 0073 0800 0000 0c03 0e25 0e27 0e24  ...s.......%.'.$
+00000170: 720c 0000 00fa 4843 3a5c 5072 6f67 7261  r.....HC:\Progra
+00000180: 6d6d 696e 675f 7072 6f6a 6563 745c 4c53  mming_project\LS
+00000190: 6865 6e67 7061 636b 6167 655c 4c73 6865  hengpackage\Lshe
+000001a0: 6e67 7061 636b 6167 655c 7369 6d75 6c61  ngpackage\simula
+000001b0: 7465 5c64 6d5c 5061 635f 646d 2e70 79da  te\dm\Pac_dm.py.
+000001c0: 085f 5f69 6e69 745f 5f06 0000 0073 0600  .__init__....s..
+000001d0: 0000 0001 0601 0601 7a0e 6d6f 7573 652e  ........z.mouse.
+000001e0: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
+000001f0: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
+00000200: 0073 1e00 0000 7400 a001 7c00 6a02 7c00  .s....t...|.j.|.
+00000210: 6a03 a102 0100 7c00 6a04 a005 a100 0100  j.....|.j.......
+00000220: 6401 5300 2902 751e 0000 000a 2020 2020  d.S.).u.....    
+00000230: 2020 2020 e5b7 a6e9 94ae e782 b9e5 87bb      ............
+00000240: 0a20 2020 2020 2020 204e 2906 7202 0000  .        N).r...
+00000250: 00da 0564 656c 6179 7208 0000 0072 0900  ...delayr....r..
+00000260: 0000 7207 0000 005a 094c 6566 7443 6c69  ..r....Z.LeftCli
+00000270: 636b a901 720a 0000 0072 0c00 0000 720c  ck..r....r....r.
+00000280: 0000 0072 0d00 0000 da06 6c43 6c69 636b  ...r......lClick
+00000290: 0b00 0000 7304 0000 0000 0410 017a 0c6d  ....s........z.m
+000002a0: 6f75 7365 2e6c 436c 6963 6b63 0100 0000  ouse.lClickc....
+000002b0: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+000002c0: 4300 0000 731e 0000 0074 00a0 017c 006a  C...s....t...|.j
+000002d0: 027c 006a 03a1 0201 007c 006a 04a0 05a1  .|.j.....|.j....
+000002e0: 0001 0064 0153 0029 0275 1e00 0000 0a20  ...d.S.).u..... 
+000002f0: 2020 2020 2020 20e5 8fb3 e994 aee7 82b9         .........
+00000300: e587 bb0a 2020 2020 2020 2020 4e29 0672  ....        N).r
+00000310: 0200 0000 720f 0000 0072 0800 0000 7209  ....r....r....r.
+00000320: 0000 0072 0700 0000 5a0a 5269 6768 7443  ...r....Z.RightC
+00000330: 6c69 636b 7210 0000 0072 0c00 0000 720c  lickr....r....r.
+00000340: 0000 0072 0d00 0000 da06 7243 6c69 636b  ...r......rClick
+00000350: 1200 0000 7304 0000 0000 0410 017a 0c6d  ....s........z.m
+00000360: 6f75 7365 2e72 436c 6963 6b63 0300 0000  ouse.rClickc....
+00000370: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00000380: 4300 0000 732a 0000 007c 006a 00a0 017c  C...s*...|.j...|
+00000390: 017c 02a1 0201 0074 02a0 037c 006a 047c  .|.....t...|.j.|
+000003a0: 006a 05a1 0201 007c 00a0 06a1 0001 0064  .j.....|.......d
+000003b0: 0153 0029 0275 2100 0000 0a20 2020 2020  .S.).u!....     
+000003c0: 2020 20e7 a7bb e58a a8e5 b9b6 e782 b9e5     .............
+000003d0: 87bb 0a20 2020 2020 2020 204e 2907 7207  ...        N).r.
+000003e0: 0000 00da 064d 6f76 6554 6f72 0200 0000  .....MoveTor....
+000003f0: 720f 0000 0072 0800 0000 7209 0000 0072  r....r....r....r
+00000400: 1100 0000 a903 720a 0000 00da 0569 6e74  ......r......int
+00000410: 5f78 da05 696e 745f 7972 0c00 0000 720c  _x..int_yr....r.
+00000420: 0000 0072 0d00 0000 da0b 6d6f 7665 5f6c  ...r......move_l
+00000430: 436c 6963 6b19 0000 0073 0600 0000 0004  Click....s......
+00000440: 0e01 1001 7a11 6d6f 7573 652e 6d6f 7665  ....z.mouse.move
+00000450: 5f6c 436c 6963 6b63 0300 0000 0000 0000  _lClickc........
+00000460: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
+00000470: 732c 0000 007c 006a 00a0 017c 017c 02a1  s,...|.j...|.|..
+00000480: 0201 0074 02a0 037c 006a 047c 006a 05a1  ...t...|.j.|.j..
+00000490: 0201 007c 006a 00a0 06a1 0001 0064 0153  ...|.j.......d.S
+000004a0: 0029 0275 2100 0000 0a20 2020 2020 2020  .).u!....       
+000004b0: 20e7 a7bb e58a a8e5 b9b6 e58f 8ce5 87bb   ...............
+000004c0: 0a20 2020 2020 2020 204e 2907 7207 0000  .        N).r...
+000004d0: 0072 1300 0000 7202 0000 0072 0f00 0000  .r....r....r....
+000004e0: 7208 0000 0072 0900 0000 5a0f 4c65 6674  r....r....Z.Left
+000004f0: 446f 7562 6c65 436c 6963 6b72 1400 0000  DoubleClickr....
+00000500: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
+00000510: 116d 6f76 655f 646f 7562 6c65 5f63 6c69  .move_double_cli
+00000520: 636b 2100 0000 7306 0000 0000 040e 0110  ck!...s.........
+00000530: 017a 176d 6f75 7365 2e6d 6f76 655f 646f  .z.mouse.move_do
+00000540: 7562 6c65 5f63 6c69 636b 4e29 0272 0400  uble_clickN).r..
+00000550: 0000 7205 0000 0029 08da 085f 5f6e 616d  ..r....)...__nam
+00000560: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000570: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0e00  .__qualname__r..
+00000580: 0000 7211 0000 0072 1200 0000 7217 0000  ..r....r....r...
+00000590: 0072 1800 0000 720c 0000 0072 0c00 0000  .r....r....r....
+000005a0: 720c 0000 0072 0d00 0000 7203 0000 0005  r....r....r.....
+000005b0: 0000 0073 0a00 0000 0801 0a05 0807 0807  ...s............
+000005c0: 0808 7203 0000 0063 0000 0000 0000 0000  ..r....c........
+000005d0: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+000005e0: 7328 0000 0065 005a 0164 005a 0264 0164  s(...e.Z.d.Z.d.d
+000005f0: 0284 005a 0364 0a64 0564 0684 015a 0464  ...Z.d.d.d...Z.d
+00000600: 0b64 0764 0884 015a 0564 0953 0029 0cda  .d.d...Z.d.S.)..
+00000610: 0563 6f6c 6f72 6302 0000 0000 0000 0000  .colorc.........
+00000620: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
+00000630: 0a00 0000 7c01 7c00 5f00 6400 5300 7206  ....|.|._.d.S.r.
+00000640: 0000 0029 01da 0e5f 636f 6c6f 725f 5f64  ...)..._color__d
+00000650: 6d5f 6f62 6aa9 0272 0a00 0000 720b 0000  m_obj..r....r...
+00000660: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000670: 720e 0000 002b 0000 0073 0200 0000 0001  r....+...s......
+00000680: 7a0e 636f 6c6f 722e 5f5f 696e 6974 5f5f  z.color.__init__
+00000690: e7cd cccc cccc ccec 3f72 0100 0000 6308  ........?r....c.
+000006a0: 0000 0000 0000 0000 0000 0009 0000 0009  ................
+000006b0: 0000 0043 0000 0073 1c00 0000 7c00 6a00  ...C...s....|.j.
+000006c0: a001 7c01 7c02 7c03 7c04 7c05 7c06 7c07  ..|.|.|.|.|.|.|.
+000006d0: a107 7d08 7c08 5300 7206 0000 0029 0272  ..}.|.S.r....).r
+000006e0: 1d00 0000 da09 4669 6e64 436f 6c6f 7229  ......FindColor)
+000006f0: 0972 0a00 0000 da06 696e 745f 7831 da06  .r......int_x1..
+00000700: 696e 745f 7931 da06 696e 745f 7832 da06  int_y1..int_x2..
+00000710: 696e 745f 7932 721c 0000 00da 0373 696d  int_y2r......sim
+00000720: da06 6469 7265 6374 da06 646d 5f72 6574  ..direct..dm_ret
+00000730: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
+00000740: 0a66 696e 645f 636f 6c6f 722e 0000 0073  .find_color....s
+00000750: 0400 0000 000a 1801 7a10 636f 6c6f 722e  ........z.color.
+00000760: 6669 6e64 5f63 6f6c 6f72 6308 0000 0000  find_colorc.....
+00000770: 0000 0000 0000 000b 0000 0009 0000 0043  ...............C
+00000780: 0000 0073 5200 0000 7c00 6a00 a001 7c01  ...sR...|.j...|.
+00000790: 7c02 7c03 7c04 7c05 7c06 7c07 a107 7d08  |.|.|.|.|.|...}.
+000007a0: 7c08 6401 1900 6401 6b02 7228 6402 5300  |.d...d.k.r(d.S.
+000007b0: 7c08 6403 1900 7d09 7c08 6404 1900 7d0a  |.d...}.|.d...}.
+000007c0: 7402 7c00 6a00 8301 a003 7c09 7c0a a102  t.|.j.....|.|...
+000007d0: 0100 6404 5300 6402 5300 2905 75f1 0000  ..d.S.d.S.).u...
+000007e0: 000a 2020 2020 2020 2020 e689 bee8 89b2  ..        ......
+000007f0: 20e5 b9b6 20e7 82b9 e587 bb0a 2020 2020   ... .......    
+00000800: 2020 2020 3a70 6172 616d 2069 6e74 5f78      :param int_x
+00000810: 313a 0a20 2020 2020 2020 203a 7061 7261  1:.        :para
+00000820: 6d20 696e 745f 7931 3a0a 2020 2020 2020  m int_y1:.      
+00000830: 2020 3a70 6172 616d 2069 6e74 5f78 323a    :param int_x2:
+00000840: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00000850: 696e 745f 7932 3a0a 2020 2020 2020 2020  int_y2:.        
+00000860: 3a70 6172 616d 2063 6f6c 6f72 3a20 e889  :param color: ..
+00000870: b2e5 bda9 e6a0 bce5 bc8f 0a20 2020 2020  ...........     
+00000880: 2020 203a 7061 7261 6d20 7369 6d3a 0a20     :param sim:. 
+00000890: 2020 2020 2020 203a 7061 7261 6d20 6469         :param di
+000008a0: 7265 6374 3a0a 2020 2020 2020 2020 3a72  rect:.        :r
+000008b0: 6574 7572 6e3a 20e6 8890 e58a 9f20 312c  eturn: ...... 1,
+000008c0: 20e5 a4b1 e8b4 a520 300a 2020 2020 2020   ...... 0.      
+000008d0: 2020 e9ff ffff ff4e 7201 0000 00e9 0100    .....Nr.......
+000008e0: 0000 2904 721d 0000 0072 2000 0000 7203  ..).r....r ...r.
+000008f0: 0000 0072 1700 0000 290b 720a 0000 0072  ...r....).r....r
+00000900: 2100 0000 7222 0000 0072 2300 0000 7224  !...r"...r#...r$
+00000910: 0000 0072 1c00 0000 7225 0000 0072 2600  ...r....r%...r&.
+00000920: 0000 7227 0000 0072 1500 0000 7216 0000  ..r'...r....r...
+00000930: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000940: da10 6669 6e64 5f63 6f6c 6f72 5f63 6c69  ..find_color_cli
+00000950: 636b 3b00 0000 730e 0000 0000 0c18 010c  ck;...s.........
+00000960: 0104 0208 0108 0112 017a 1663 6f6c 6f72  .........z.color
+00000970: 2e66 696e 645f 636f 6c6f 725f 636c 6963  .find_color_clic
+00000980: 6b4e 2902 721f 0000 0072 0100 0000 2902  kN).r....r....).
+00000990: 721f 0000 0072 0100 0000 2906 7219 0000  r....r....).r...
+000009a0: 0072 1a00 0000 721b 0000 0072 0e00 0000  .r....r....r....
+000009b0: 7228 0000 0072 2b00 0000 720c 0000 0072  r(...r+...r....r
+000009c0: 0c00 0000 720c 0000 0072 0d00 0000 721c  ....r....r....r.
+000009d0: 0000 002a 0000 0073 0600 0000 0801 0803  ...*...s........
+000009e0: 0a0d 721c 0000 0063 0000 0000 0000 0000  ..r....c........
+000009f0: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+00000a00: 7328 0000 0065 005a 0164 005a 0264 0164  s(...e.Z.d.Z.d.d
+00000a10: 0284 005a 0364 0b64 0664 0784 015a 0464  ...Z.d.d.d...Z.d
+00000a20: 0c64 0864 0984 015a 0564 0a53 0029 0dda  .d.d...Z.d.S.)..
+00000a30: 0370 6963 6302 0000 0000 0000 0000 0000  .picc...........
+00000a40: 0002 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
+00000a50: 0000 7c01 7c00 5f00 6400 5300 7206 0000  ..|.|._.d.S.r...
+00000a60: 0029 01da 0c5f 7069 635f 5f64 6d5f 6f62  .)..._pic__dm_ob
+00000a70: 6a72 1e00 0000 720c 0000 0072 0c00 0000  jr....r....r....
+00000a80: 720d 0000 0072 0e00 0000 5200 0000 7302  r....r....R...s.
+00000a90: 0000 0000 017a 0c70 6963 2e5f 5f69 6e69  .....z.pic.__ini
+00000aa0: 745f 5fda 0630 3030 3030 3072 1f00 0000  t__..000000r....
+00000ab0: 7201 0000 0063 0900 0000 0000 0000 0000  r....c..........
+00000ac0: 0000 0a00 0000 0a00 0000 4300 0000 731e  ..........C...s.
+00000ad0: 0000 007c 006a 00a0 017c 017c 027c 037c  ...|.j...|.|.|.|
+00000ae0: 047c 057c 067c 077c 08a1 087d 097c 0953  .|.|.|.|...}.|.S
+00000af0: 0029 0175 0c01 0000 0a20 2020 2020 2020  .).u.....       
+00000b00: 20e6 89be e59b be0a 2020 2020 2020 2020   .......        
+00000b10: 3a70 6172 616d 2069 6e74 5f78 313a 0a20  :param int_x1:. 
+00000b20: 2020 2020 2020 203a 7061 7261 6d20 696e         :param in
+00000b30: 745f 7931 3a0a 2020 2020 2020 2020 3a70  t_y1:.        :p
+00000b40: 6172 616d 2069 6e74 5f78 323a 0a20 2020  aram int_x2:.   
+00000b50: 2020 2020 203a 7061 7261 6d20 696e 745f       :param int_
+00000b60: 7932 3a0a 2020 2020 2020 2020 3a70 6172  y2:.        :par
+00000b70: 616d 2070 6963 5f6e 616d 653a 0a20 2020  am pic_name:.   
+00000b80: 2020 2020 203a 7061 7261 6d20 6465 6c74       :param delt
+00000b90: 615f 636f 6c6f 723a 0a20 2020 2020 2020  a_color:.       
+00000ba0: 203a 7061 7261 6d20 7369 6d3a 0a20 2020   :param sim:.   
+00000bb0: 2020 2020 203a 7061 7261 6d20 6469 7265       :param dire
+00000bc0: 6374 3a0a 2020 2020 2020 2020 3a72 6574  ct:.        :ret
+00000bd0: 7572 6e3a 20e6 8890 e58a 9f20 e8bf 94e5  urn: ...... ....
+00000be0: 9b9e e59d 90e6 a087 2c20 e5a4 b1e8 b4a5  ........, ......
+00000bf0: 202d 312c 202d 312c 202d 310a 2020 2020   -1, -1, -1.    
+00000c00: 2020 2020 2902 722d 0000 00da 0846 696e      ).r-.....Fin
+00000c10: 6450 6963 4529 0a72 0a00 0000 7221 0000  dPicE).r....r!..
+00000c20: 0072 2200 0000 7223 0000 0072 2400 0000  .r"...r#...r$...
+00000c30: da08 7069 635f 6e61 6d65 da0b 6465 6c74  ..pic_name..delt
+00000c40: 615f 636f 6c6f 7272 2500 0000 7226 0000  a_colorr%...r&..
+00000c50: 0072 2700 0000 720c 0000 0072 0c00 0000  .r'...r....r....
+00000c60: 720d 0000 00da 0866 696e 645f 7069 6355  r......find_picU
+00000c70: 0000 0073 0400 0000 000e 1a01 7a0c 7069  ...s........z.pi
+00000c80: 632e 6669 6e64 5f70 6963 6309 0000 0000  c.find_picc.....
+00000c90: 0000 0000 0000 000c 0000 000a 0000 0043  ...............C
+00000ca0: 0000 0073 5400 0000 7c00 6a00 a001 7c01  ...sT...|.j...|.
+00000cb0: 7c02 7c03 7c04 7c05 7c06 7c07 7c08 a108  |.|.|.|.|.|.|...
+00000cc0: 7d09 7c09 6401 1900 6401 6b02 722a 6402  }.|.d...d.k.r*d.
+00000cd0: 5300 7c09 6403 1900 7d0a 7c09 6401 1900  S.|.d...}.|.d...
+00000ce0: 7d0b 7402 7c00 6a00 8301 a003 7c0a 7c0b  }.t.|.j.....|.|.
+00000cf0: a102 0100 6403 5300 6402 5300 2904 7545  ....d.S.d.S.).uE
+00000d00: 0000 000a 2020 2020 2020 2020 e689 bee5  ....        ....
+00000d10: 9bbe e5b9 b6e7 82b9 e587 bb0a 2020 2020  ............    
+00000d20: 2020 2020 3a72 6574 7572 6e3a 20e6 8890      :return: ...
+00000d30: e58a 9f20 312c 20e5 a4b1 e8b4 a520 300a  ... 1, ...... 0.
+00000d40: 2020 2020 2020 2020 7229 0000 004e 722a          r)...Nr*
+00000d50: 0000 0029 0472 2d00 0000 722f 0000 0072  ...).r-...r/...r
+00000d60: 0300 0000 7217 0000 0029 0c72 0a00 0000  ....r....).r....
+00000d70: 7221 0000 0072 2200 0000 7223 0000 0072  r!...r"...r#...r
+00000d80: 2400 0000 7230 0000 0072 3100 0000 7225  $...r0...r1...r%
+00000d90: 0000 0072 2600 0000 7227 0000 0072 1500  ...r&...r'...r..
+00000da0: 0000 7216 0000 0072 0c00 0000 720c 0000  ..r....r....r...
+00000db0: 0072 0d00 0000 da0e 6669 6e64 5f70 6963  .r......find_pic
+00000dc0: 5f63 6c69 636b 6600 0000 730e 0000 0000  _clickf...s.....
+00000dd0: 051a 010c 0104 0208 0108 0112 017a 1270  .............z.p
+00000de0: 6963 2e66 696e 645f 7069 635f 636c 6963  ic.find_pic_clic
+00000df0: 6b4e 2903 722e 0000 0072 1f00 0000 7201  kN).r....r....r.
+00000e00: 0000 0029 0372 2e00 0000 721f 0000 0072  ...).r....r....r
+00000e10: 0100 0000 2906 7219 0000 0072 1a00 0000  ....).r....r....
+00000e20: 721b 0000 0072 0e00 0000 7232 0000 0072  r....r....r2...r
+00000e30: 3300 0000 720c 0000 0072 0c00 0000 720c  3...r....r....r.
+00000e40: 0000 0072 0d00 0000 722c 0000 0051 0000  ...r....r,...Q..
+00000e50: 0073 0600 0000 0801 0803 0a11 722c 0000  .s..........r,..
+00000e60: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000e70: 0000 0300 0000 4000 0000 7328 0000 0065  ......@...s(...e
+00000e80: 005a 0164 005a 0264 0164 0284 005a 0364  .Z.d.Z.d.d...Z.d
+00000e90: 0964 0464 0584 015a 0464 0a64 0664 0784  .d.d...Z.d.d.d..
+00000ea0: 015a 0564 0853 0029 0bda 0477 6f72 6463  .Z.d.S.)...wordc
+00000eb0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000ec0: 0200 0000 4300 0000 730a 0000 007c 017c  ....C...s....|.|
+00000ed0: 005f 0064 0053 0072 0600 0000 2901 da0d  ._.d.S.r....)...
+00000ee0: 5f77 6f72 645f 5f64 6d5f 6f62 6a72 1e00  _word__dm_objr..
+00000ef0: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+00000f00: 0072 0e00 0000 7600 0000 7302 0000 0000  .r....v...s.....
+00000f10: 017a 0d77 6f72 642e 5f5f 696e 6974 5f5f  .z.word.__init__
+00000f20: e79a 9999 9999 99e9 3f63 0800 0000 0000  ........?c......
+00000f30: 0000 0000 0000 0900 0000 0900 0000 4300  ..............C.
+00000f40: 0000 731c 0000 007c 006a 00a0 017c 017c  ..s....|.j...|.|
+00000f50: 027c 037c 047c 057c 067c 07a1 077d 087c  .|.|.|.|.|...}.|
+00000f60: 0853 0029 0175 1800 0000 0a20 2020 2020  .S.).u.....     
+00000f70: 2020 20e6 89be e5ad 970a 2020 2020 2020     .......      
+00000f80: 2020 2902 7235 0000 00da 0b46 696e 6453    ).r5.....FindS
+00000f90: 7472 4661 7374 2909 720a 0000 0072 2100  trFast).r....r!.
+00000fa0: 0000 7222 0000 0072 2300 0000 7224 0000  ..r"...r#...r$..
+00000fb0: 00da 0873 7472 5f6e 616d 65da 0c63 6f6c  ...str_name..col
+00000fc0: 6f72 5f66 6f72 6d61 7472 2500 0000 7227  or_formatr%...r'
+00000fd0: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
+00000fe0: 0000 da09 6669 6e64 5f77 6f72 6479 0000  ....find_wordy..
+00000ff0: 0073 0400 0000 0004 1801 7a0e 776f 7264  .s........z.word
+00001000: 2e66 696e 645f 776f 7264 6308 0000 0000  .find_wordc.....
+00001010: 0000 0000 0000 000b 0000 0009 0000 0043  ...............C
+00001020: 0000 0073 5200 0000 7c00 6a00 a001 7c01  ...sR...|.j...|.
+00001030: 7c02 7c03 7c04 7c05 7c06 7c07 a107 7d08  |.|.|.|.|.|...}.
+00001040: 7c08 6401 1900 6401 6b02 7228 6402 5300  |.d...d.k.r(d.S.
+00001050: 7c08 6403 1900 7d09 7c08 6404 1900 7d0a  |.d...}.|.d...}.
+00001060: 7402 7c00 6a00 8301 a003 7c09 7c0a a102  t.|.j.....|.|...
+00001070: 0100 6404 5300 6402 5300 2905 75eb 0000  ..d.S.d.S.).u...
+00001080: 000a 2020 2020 2020 2020 e689 bee5 ad97  ..        ......
+00001090: e5b9 b6e7 82b9 e587 bb0a 2020 2020 2020  ..........      
+000010a0: 2020 3a70 6172 616d 2069 6e74 5f78 313a    :param int_x1:
+000010b0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000010c0: 696e 745f 7931 3a0a 2020 2020 2020 2020  int_y1:.        
+000010d0: 3a70 6172 616d 2069 6e74 5f78 323a 0a20  :param int_x2:. 
+000010e0: 2020 2020 2020 203a 7061 7261 6d20 696e         :param in
+000010f0: 745f 7932 3a0a 2020 2020 2020 2020 3a70  t_y2:.        :p
+00001100: 6172 616d 2073 7472 5f6e 616d 653a 0a20  aram str_name:. 
+00001110: 2020 2020 2020 203a 7061 7261 6d20 636f         :param co
+00001120: 6c6f 725f 666f 726d 6174 3a0a 2020 2020  lor_format:.    
+00001130: 2020 2020 3a70 6172 616d 2073 696d 3a0a      :param sim:.
+00001140: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00001150: 20e6 8890 e58a 9f20 312c 20e5 a4b1 e8b4   ...... 1, .....
+00001160: a520 300a 2020 2020 2020 2020 7229 0000  . 0.        r)..
+00001170: 004e 7201 0000 0072 2a00 0000 2904 7235  .Nr....r*...).r5
+00001180: 0000 0072 3700 0000 7203 0000 0072 1700  ...r7...r....r..
+00001190: 0000 290b 720a 0000 0072 2100 0000 7222  ..).r....r!...r"
+000011a0: 0000 0072 2300 0000 7224 0000 0072 3800  ...r#...r$...r8.
+000011b0: 0000 7239 0000 0072 2500 0000 7227 0000  ..r9...r%...r'..
+000011c0: 0072 1500 0000 7216 0000 0072 0c00 0000  .r....r....r....
+000011d0: 720c 0000 0072 0d00 0000 da0f 6669 6e64  r....r......find
+000011e0: 5f77 6f72 645f 636c 6963 6b80 0000 0073  _word_click....s
+000011f0: 0e00 0000 000c 1801 0c01 0402 0801 0801  ................
+00001200: 1201 7a14 776f 7264 2e66 696e 645f 776f  ..z.word.find_wo
+00001210: 7264 5f63 6c69 636b 4e29 0172 3600 0000  rd_clickN).r6...
+00001220: 2901 7236 0000 0029 0672 1900 0000 721a  ).r6...).r....r.
+00001230: 0000 0072 1b00 0000 720e 0000 0072 3a00  ...r....r....r:.
+00001240: 0000 723b 0000 0072 0c00 0000 720c 0000  ..r;...r....r...
+00001250: 0072 0c00 0000 720d 0000 0072 3400 0000  .r....r....r4...
+00001260: 7500 0000 7306 0000 0008 0108 030a 0772  u...s..........r
+00001270: 3400 0000 4e29 065a 1b4c 7368 656e 6770  4...N).Z.Lshengp
+00001280: 6163 6b61 6765 2e74 6f6f 6c73 2e47 656e  ackage.tools.Gen
+00001290: 6572 616c 7202 0000 0072 0300 0000 721c  eralr....r....r.
+000012a0: 0000 0072 2c00 0000 7234 0000 0072 0c00  ...r,...r4...r..
+000012b0: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+000012c0: 00da 083c 6d6f 6475 6c65 3e02 0000 0073  ...<module>....s
+000012d0: 0800 0000 0c03 0e25 0e27 0e24            .......%.'.$
```

### Comparing `Lshengpackage-0.4.4/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc` & `Lshengpackage-0.4.5/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.4/Lshengpackage/simulate/mock_findPic.py` & `Lshengpackage-0.4.5/Lshengpackage/simulate/mock_findPic.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,37 +10,40 @@
 
 # 截图
 def screen_shot(fol_path):
     sleep(0.1)
     pyautogui.screenshot(fol_path)
 
 
-# 当前页面找图,找到匹配对象位置中心点
-def find_image(fol_path, target_path, _system=None, int_x1=0, int_y1=None, int_x2=None, int_y2=None):
+# 当前页面找图,找到匹配对象位置中心点 # 自定义int_x1 不能等于0
+def find_image(fol_path, target_path, _system=None, int_x=None, int_y=None, width= 0, high = None,screenshot = True):
     """
     在当前页面上找目标图片坐在坐标，返回中心坐标 (x,y)
     :param path:
     :param target: 例：../img/test.png
     :return:
     """
-    if _system == 'hwnd':  # hwnd暂时没更新进来
+    if screenshot is True:
+        if _system == 'hwnd':  # hwnd暂时没更新进来
+            pass
+        elif _system == 'adb':  # android adb 截图
+            cut = command()
+            # print(fol_path.split('\\')[-1])
+            cut.cut_scr(fol_path)
+        elif _system is None:  # pyautogui 截图
+            screen_shot(fol_path)
+    elif screenshot is False:
         pass
-    elif _system == 'adb':  # android adb 截图
-        cut = command()
-        # print(fol_path.split('\\')[-1])
-        cut.cut_scr(fol_path)
-    elif _system is None:  # pyautogui 截图
-        screen_shot(fol_path)
     # 获取当前页面的截图
     source_path = os.path.join(fol_path)
-    if int_x1 == 0:
+    if width == 0:
         pass
     else:
         img = Image.open(source_path)
-        code_image = img.crop((int_x1, int_y1, int_x2, int_y2))
+        code_image = img.crop((int_x, int_y, (int_x+width), (int_y + high)))
         code_image.save(source_path)  # 原地址重写
 
     # 获取目标图片的存放路径
     target_path = os.path.join(target_path)
     # print(source_path)
     # print(target_path)
 
@@ -56,20 +59,20 @@
     if match_result[1] > 0.9:  # 匹配度大于90%，视为匹配成功
         pos_start = cv2.minMaxLoc(result)[3]  # 获取匹配成功后的起始坐标
 
         # 计算匹配对象的中心位置坐标
         x = int(pos_start[0]) + int(target_image.shape[1]) / 2
         y = int(pos_start[1]) + int(target_image.shape[0]) / 2
         if sys.platform == 'darwin':
-            if int_x1 == 0:
+            if width == 0:
                 return x / 2, y / 2
             else:
-                return (x + int_x1) / 2, (y + int_y1) / 2
+                return (x + int_x) / 2, (y + int_y) / 2
         else:
-            if int_x1 == 0:
+            if width == 0:
                 return x, y
             else:
-                return (x + int_x1), (y + int_y1)
+                return (x + int_x), (y + int_y)
     else:
         return None
```

### Comparing `Lshengpackage-0.4.4/Lshengpackage/tools/ChaoJiYing.py` & `Lshengpackage-0.4.5/Lshengpackage/tools/ChaoJiYing.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.4/Lshengpackage/tools/General.py` & `Lshengpackage-0.4.5/Lshengpackage/tools/General.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.4/Lshengpackage/tools/OperateFile.py` & `Lshengpackage-0.4.5/Lshengpackage/tools/OperateFile.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.4/Lshengpackage/tools/SearchFile.py` & `Lshengpackage-0.4.5/Lshengpackage/tools/SearchFile.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.4/Lshengpackage.egg-info/PKG-INFO` & `Lshengpackage-0.4.5/Lshengpackage.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lshengpackage
-Version: 0.4.4
+Version: 0.4.5
 Summary: 个人自动化爬虫开源学习
 Home-page: https://lsheng0-0.github.io/
 Download-URL: https://github.com/Lsheng0-0/package
 Author: Lsheng0-0
 Author-email: 1522833718@qq.com
 License: MIT
 Keywords: 游戏,办公,自动化,爬虫
```

### Comparing `Lshengpackage-0.4.4/Lshengpackage.egg-info/SOURCES.txt` & `Lshengpackage-0.4.5/Lshengpackage.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -10,28 +10,40 @@
 Lshengpackage.egg-info/SOURCES.txt
 Lshengpackage.egg-info/dependency_links.txt
 Lshengpackage.egg-info/requires.txt
 Lshengpackage.egg-info/top_level.txt
 Lshengpackage/simulate/__init__.py
 Lshengpackage/simulate/mock_findFr.py
 Lshengpackage/simulate/mock_findPic.py
+Lshengpackage/simulate/__pycache__/__init__.cpython-39.pyc
+Lshengpackage/simulate/__pycache__/mock_findFr.cpython-39.pyc
+Lshengpackage/simulate/__pycache__/mock_findPic.cpython-39.pyc
 Lshengpackage/simulate/adb/Command_adb.py
 Lshengpackage/simulate/adb/__init__.py
 Lshengpackage/simulate/adb/re_Pic.py
+Lshengpackage/simulate/adb/__pycache__/Command_adb.cpython-39.pyc
 Lshengpackage/simulate/adb/__pycache__/__init__.cpython-39.pyc
+Lshengpackage/simulate/adb/__pycache__/re_Pic.cpython-39.pyc
 Lshengpackage/simulate/adb/dingtalk/__init__.py
 Lshengpackage/simulate/adb/dingtalk/dingtalk_api.py
-Lshengpackage/simulate/adb/dingtalk/image_data.py
+Lshengpackage/simulate/adb/dingtalk/__pycache__/__init__.cpython-39.pyc
+Lshengpackage/simulate/adb/dingtalk/__pycache__/dingtalk_api.cpython-39.pyc
 Lshengpackage/simulate/dm/Pac_dm.py
 Lshengpackage/simulate/dm/Reg.py
 Lshengpackage/simulate/dm/Win_dm.py
 Lshengpackage/simulate/dm/__init__.py
 Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc
 Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc
 Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc
 Lshengpackage/simulate/dm/__pycache__/__init__.cpython-39.pyc
 Lshengpackage/tools/ChaoJiYing.py
 Lshengpackage/tools/General.py
 Lshengpackage/tools/Loading.py
 Lshengpackage/tools/OperateFile.py
 Lshengpackage/tools/SearchFile.py
-Lshengpackage/tools/__init__.py
+Lshengpackage/tools/__init__.py
+Lshengpackage/tools/__pycache__/ChaoJiYing.cpython-39.pyc
+Lshengpackage/tools/__pycache__/General.cpython-39.pyc
+Lshengpackage/tools/__pycache__/Loading.cpython-39.pyc
+Lshengpackage/tools/__pycache__/OperateFile.cpython-39.pyc
+Lshengpackage/tools/__pycache__/SearchFile.cpython-39.pyc
+Lshengpackage/tools/__pycache__/__init__.cpython-39.pyc
```

### Comparing `Lshengpackage-0.4.4/PKG-INFO` & `Lshengpackage-0.4.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lshengpackage
-Version: 0.4.4
+Version: 0.4.5
 Summary: 个人自动化爬虫开源学习
 Home-page: https://lsheng0-0.github.io/
 Download-URL: https://github.com/Lsheng0-0/package
 Author: Lsheng0-0
 Author-email: 1522833718@qq.com
 License: MIT
 Keywords: 游戏,办公,自动化,爬虫
```

### Comparing `Lshengpackage-0.4.4/README.md` & `Lshengpackage-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.4/setup.py` & `Lshengpackage-0.4.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='Lshengpackage',  # How you named your package folder (MyLib)
     packages=['Lshengpackage'],  # Chose the same as "name"
-    version='0.4.4',  # Start with a small number and increase it with every change you make
+    version='0.4.5',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='个人自动化爬虫开源学习',  # Give a short description about your library
     # long_description=open('README.md', 'r', encoding='utf-8').read(),
     author='Lsheng0-0',  # Type in your name
     author_email='1522833718@qq.com',  # Type in your E-Mail
     url='https://lsheng0-0.github.io/',  # Provide either the link to your github or to your website
     download_url='https://github.com/Lsheng0-0/package',  # I explain this later on
```

