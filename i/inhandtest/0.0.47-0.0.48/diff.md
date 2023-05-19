# Comparing `tmp/inhandtest-0.0.47.tar.gz` & `tmp/inhandtest-0.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.47.tar", last modified: Fri May 19 01:02:56 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.48.tar", last modified: Fri May 19 01:12:37 2023, max compression
```

## Comparing `inhandtest-0.0.47.tar` & `inhandtest-0.0.48.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 01:02:56.000000 inhandtest-0.0.47/
--rw-rw-rw-   0        0        0      535 2023-05-19 01:02:56.000000 inhandtest-0.0.47/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.47/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 01:02:56.000000 inhandtest-0.0.47/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.47/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:02:56.000000 inhandtest-0.0.47/inhandtest/base_page/
--rw-rw-rw-   0        0        0      134 2023-03-15 06:05:35.000000 inhandtest-0.0.47/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    39712 2023-05-16 03:23:36.000000 inhandtest-0.0.47/inhandtest/base_page/_ig_contents_locators.py
--rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.47/inhandtest/base_page/_ir3XX_contents_locators.py
--rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.47/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    52406 2023-05-18 09:41:02.000000 inhandtest-0.0.47/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0    15461 2023-05-17 09:10:24.000000 inhandtest-0.0.47/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.47/inhandtest/exception.py
--rw-rw-rw-   0        0        0     3890 2023-03-30 10:08:49.000000 inhandtest-0.0.47/inhandtest/file.py
--rw-rw-rw-   0        0        0    11861 2023-05-06 01:56:01.000000 inhandtest-0.0.47/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.47/inhandtest/inmongodb.py
--rw-rw-rw-   0        0        0    22049 2023-03-30 10:08:49.000000 inhandtest-0.0.47/inhandtest/inmqtt.py
--rw-rw-rw-   0        0        0    51883 2023-05-16 09:03:39.000000 inhandtest-0.0.47/inhandtest/inrequest.py
--rw-rw-rw-   0        0        0     7583 2023-05-06 07:36:44.000000 inhandtest-0.0.47/inhandtest/inserial.py
--rw-rw-rw-   0        0        0    12335 2023-04-06 06:40:29.000000 inhandtest-0.0.47/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     6847 2023-05-18 06:06:23.000000 inhandtest-0.0.47/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     1144 2023-03-30 10:18:47.000000 inhandtest-0.0.47/inhandtest/ip.py
--rw-rw-rw-   0        0        0    11620 2023-05-08 10:30:07.000000 inhandtest-0.0.47/inhandtest/mail.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:02:56.000000 inhandtest-0.0.47/inhandtest/pages/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.47/inhandtest/pages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:02:56.000000 inhandtest-0.0.47/inhandtest/pages/ingateway/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:38:25.000000 inhandtest-0.0.47/inhandtest/pages/ingateway/__init__.py
--rw-rw-rw-   0        0        0     5307 2023-05-18 09:51:01.000000 inhandtest-0.0.47/inhandtest/pages/ingateway/ingateway.py
--rw-rw-rw-   0        0        0      593 2023-05-18 07:02:23.000000 inhandtest-0.0.47/inhandtest/pages/ingateway/locators.py
--rw-rw-rw-   0        0        0      303 2023-05-15 09:37:04.000000 inhandtest-0.0.47/inhandtest/pages/locale.py
--rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.47/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0    32773 2023-05-16 10:13:54.000000 inhandtest-0.0.47/inhandtest/telnet.py
--rw-rw-rw-   0        0        0    25281 2023-05-12 08:18:46.000000 inhandtest-0.0.47/inhandtest/tools.py
--rw-rw-rw-   0        0        0      137 2023-05-15 07:42:26.000000 inhandtest-0.0.47/requirements.txt
--rw-rw-rw-   0        0        0     1544 2023-05-19 01:02:26.000000 inhandtest-0.0.47/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 01:12:37.000000 inhandtest-0.0.48/
+-rw-rw-rw-   0        0        0      535 2023-05-19 01:12:37.000000 inhandtest-0.0.48/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.48/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 01:12:37.000000 inhandtest-0.0.48/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.48/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 01:12:37.000000 inhandtest-0.0.48/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      134 2023-03-15 06:05:35.000000 inhandtest-0.0.48/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    39712 2023-05-16 03:23:36.000000 inhandtest-0.0.48/inhandtest/base_page/_ig_contents_locators.py
+-rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.48/inhandtest/base_page/_ir3XX_contents_locators.py
+-rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.48/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    52406 2023-05-18 09:41:02.000000 inhandtest-0.0.48/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0    15461 2023-05-17 09:10:24.000000 inhandtest-0.0.48/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.48/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     3890 2023-03-30 10:08:49.000000 inhandtest-0.0.48/inhandtest/file.py
+-rw-rw-rw-   0        0        0    11861 2023-05-06 01:56:01.000000 inhandtest-0.0.48/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.48/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22049 2023-03-30 10:08:49.000000 inhandtest-0.0.48/inhandtest/inmqtt.py
+-rw-rw-rw-   0        0        0    51883 2023-05-16 09:03:39.000000 inhandtest-0.0.48/inhandtest/inrequest.py
+-rw-rw-rw-   0        0        0     7583 2023-05-06 07:36:44.000000 inhandtest-0.0.48/inhandtest/inserial.py
+-rw-rw-rw-   0        0        0    12335 2023-04-06 06:40:29.000000 inhandtest-0.0.48/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     6847 2023-05-18 06:06:23.000000 inhandtest-0.0.48/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     1144 2023-03-30 10:18:47.000000 inhandtest-0.0.48/inhandtest/ip.py
+-rw-rw-rw-   0        0        0    11620 2023-05-08 10:30:07.000000 inhandtest-0.0.48/inhandtest/mail.py
+drwxrwxrwx   0        0        0        0 2023-05-19 01:12:37.000000 inhandtest-0.0.48/inhandtest/pages/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.48/inhandtest/pages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 01:12:37.000000 inhandtest-0.0.48/inhandtest/pages/ingateway/
+-rw-rw-rw-   0        0        0     5307 2023-05-18 09:51:01.000000 inhandtest-0.0.48/inhandtest/pages/ingateway/ingateway.py
+-rw-rw-rw-   0        0        0     2125 2023-05-18 09:47:36.000000 inhandtest-0.0.48/inhandtest/pages/ingateway/locale.yml
+-rw-rw-rw-   0        0        0      593 2023-05-18 07:02:23.000000 inhandtest-0.0.48/inhandtest/pages/ingateway/locators.py
+-rw-rw-rw-   0        0        0      303 2023-05-15 09:37:04.000000 inhandtest-0.0.48/inhandtest/pages/locale.py
+-rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.48/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0    32773 2023-05-16 10:13:54.000000 inhandtest-0.0.48/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0    25281 2023-05-12 08:18:46.000000 inhandtest-0.0.48/inhandtest/tools.py
+-rw-rw-rw-   0        0        0      137 2023-05-15 07:42:26.000000 inhandtest-0.0.48/requirements.txt
+-rw-rw-rw-   0        0        0     1543 2023-05-19 01:12:26.000000 inhandtest-0.0.48/setup.py
```

### Comparing `inhandtest-0.0.47/README.md` & `inhandtest-0.0.48/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.47/inhandtest/base_page/_ig_contents_locators.py` & `inhandtest-0.0.48/inhandtest/base_page/_ig_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.47/inhandtest/base_page/_ir3XX_contents_locators.py` & `inhandtest-0.0.48/inhandtest/base_page/_ir3XX_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.47/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.48/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.47/inhandtest/base_page/base_page.py` & `inhandtest-0.0.48/inhandtest/base_page/base_page.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.47/inhandtest/base_page/table_tr.py` & `inhandtest-0.0.48/inhandtest/base_page/table_tr.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.47/inhandtest/exception.py` & `inhandtest-0.0.48/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.47/inhandtest/file.py` & `inhandtest-0.0.48/inhandtest/file.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.47/inhandtest/inmodbus.py` & `inhandtest-0.0.48/inhandtest/inmodbus.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.47/inhandtest/inmongodb.py` & `inhandtest-0.0.48/inhandtest/inmongodb.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.47/inhandtest/inmqtt.py` & `inhandtest-0.0.48/inhandtest/inmqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.47/inhandtest/inrequest.py` & `inhandtest-0.0.48/inhandtest/inrequest.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.47/inhandtest/inserial.py` & `inhandtest-0.0.48/inhandtest/inserial.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.47/inhandtest/insocket.py` & `inhandtest-0.0.48/inhandtest/insocket.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.47/inhandtest/inssh.py` & `inhandtest-0.0.48/inhandtest/inssh.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.47/inhandtest/ip.py` & `inhandtest-0.0.48/inhandtest/ip.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.47/inhandtest/mail.py` & `inhandtest-0.0.48/inhandtest/mail.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.47/inhandtest/pages/ingateway/ingateway.py` & `inhandtest-0.0.48/inhandtest/pages/ingateway/ingateway.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.47/inhandtest/pages/ingateway/locators.py` & `inhandtest-0.0.48/inhandtest/pages/ingateway/locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.47/inhandtest/pytest_email.html` & `inhandtest-0.0.48/inhandtest/pytest_email.html`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.47/inhandtest/telnet.py` & `inhandtest-0.0.48/inhandtest/telnet.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.47/inhandtest/tools.py` & `inhandtest-0.0.48/inhandtest/tools.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.47/setup.py` & `inhandtest-0.0.48/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 setup
 
 """
 from distutils.core import setup
 
 setup(
     name='inhandtest',
-    version='0.0.47',
+    version='0.0.48',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
     packages=['inhandtest', 'inhandtest.base_page', 'inhandtest.pages', 'inhandtest.pages.ingateway', ],
-    package_data={'inhandtest': ['pytest_email.html'], 'inhandtest.pages.ingateway': ['*.yaml']},
+    package_data={'inhandtest': ['pytest_email.html'], 'inhandtest.pages.ingateway': ['*.yml']},
     url='https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》',
     long_description='方便inhand测试同事在自动化测试时，对通用协议或者常用工具及方法做封装，需要使用时即在线安装；\n映翰通出品，追尾必究！',
     classifiers=[
         "Programming Language :: Python :: 3.7",
     ],
     install_requires=['pytz', 'requests', 'playwright', 'pyserial', 'modbus-tk', 'paho-mqtt', 'urllib3', 'paramiko',
                       'emails', 'Jinja2', 'pymongo', 'psutil', 'lxml', 'dynaconf'
```

