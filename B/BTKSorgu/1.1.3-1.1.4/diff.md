# Comparing `tmp/BTKSorgu-1.1.3.tar.gz` & `tmp/BTKSorgu-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTKSorgu-1.1.3.tar", last modified: Thu May 18 19:40:51 2023, max compression
+gzip compressed data, was "BTKSorgu-1.1.4.tar", last modified: Thu May 18 19:45:04 2023, max compression
```

## Comparing `BTKSorgu-1.1.3.tar` & `BTKSorgu-1.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:40:51.694258 BTKSorgu-1.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:40:51.694258 BTKSorgu-1.1.3/BTKSorgu/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/BTKSorgu/Erisim_Engeli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/BTKSorgu/KekikGUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/BTKSorgu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/BTKSorgu/arayuz.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/BTKSorgu/konsol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/BTKSorgu/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:40:51.694258 BTKSorgu-1.1.3/BTKSorgu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-05-18 19:40:51.000000 BTKSorgu-1.1.3/BTKSorgu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 19:40:51.000000 BTKSorgu-1.1.3/BTKSorgu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:40:51.000000 BTKSorgu-1.1.3/BTKSorgu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 19:40:51.000000 BTKSorgu-1.1.3/BTKSorgu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-18 19:40:51.000000 BTKSorgu-1.1.3/BTKSorgu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 19:40:51.000000 BTKSorgu-1.1.3/BTKSorgu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-05-18 19:40:51.694258 BTKSorgu-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:40:51.694258 BTKSorgu-1.1.3/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/Shared/org.KekikAkademi.BTKSorgu.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/Shared/org.KekikAkademi.BTKSorgu.svg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 19:40:51.694258 BTKSorgu-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-18 19:40:30.000000 BTKSorgu-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:45:04.643430 BTKSorgu-1.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:45:04.639430 BTKSorgu-1.1.4/BTKSorgu/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/BTKSorgu/Erisim_Engeli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/BTKSorgu/KekikGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/BTKSorgu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/BTKSorgu/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/BTKSorgu/konsol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/BTKSorgu/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:45:04.643430 BTKSorgu-1.1.4/BTKSorgu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-05-18 19:45:04.000000 BTKSorgu-1.1.4/BTKSorgu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 19:45:04.000000 BTKSorgu-1.1.4/BTKSorgu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:45:04.000000 BTKSorgu-1.1.4/BTKSorgu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 19:45:04.000000 BTKSorgu-1.1.4/BTKSorgu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-18 19:45:04.000000 BTKSorgu-1.1.4/BTKSorgu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 19:45:04.000000 BTKSorgu-1.1.4/BTKSorgu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-05-18 19:45:04.643430 BTKSorgu-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:45:04.643430 BTKSorgu-1.1.4/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/Shared/org.KekikAkademi.BTKSorgu.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/Shared/org.KekikAkademi.BTKSorgu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 19:45:04.643430 BTKSorgu-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-18 19:44:41.000000 BTKSorgu-1.1.4/setup.py
```

### Comparing `BTKSorgu-1.1.3/BTKSorgu/Erisim_Engeli.py` & `BTKSorgu-1.1.4/BTKSorgu/Erisim_Engeli.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.3/BTKSorgu/KekikGUI.py` & `BTKSorgu-1.1.4/BTKSorgu/KekikGUI.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.3/BTKSorgu/arayuz.py` & `BTKSorgu-1.1.4/BTKSorgu/arayuz.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.3/BTKSorgu/konsol.py` & `BTKSorgu-1.1.4/BTKSorgu/konsol.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.3/BTKSorgu/logo.png` & `BTKSorgu-1.1.4/BTKSorgu/logo.png`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.3/BTKSorgu.egg-info/PKG-INFO` & `BTKSorgu-1.1.4/BTKSorgu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.1.3
+Version: 1.1.4
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.1.3 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.1.4 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `BTKSorgu-1.1.3/LICENSE` & `BTKSorgu-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.3/PKG-INFO` & `BTKSorgu-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.1.3
+Version: 1.1.4
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.1.3 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.1.4 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `BTKSorgu-1.1.3/README.md` & `BTKSorgu-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.3/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.1.4/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

 * *Files 0% similar despite different names*

#### Comparing `BTKSorgu-1.1.3/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.1.4/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

```diff
@@ -25,15 +25,15 @@
       <image>https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
-    <release version="1.1.3" date="2023-5-18">
+    <release version="1.1.4" date="2023-5-18">
       <description>
         <p>Github aksiyonlarıyla otomatik paketlenme ve yayınlama eklendi..</p>
       </description>
     </release>
     <release version="1.1.2" date="2023-5-18">
       <description>
         <p>Readme Genişletildi ve Manuel Paketleme Aşamaları Eklendi..</p>
```

### Comparing `BTKSorgu-1.1.3/Shared/org.KekikAkademi.BTKSorgu.svg` & `BTKSorgu-1.1.4/Shared/org.KekikAkademi.BTKSorgu.svg`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.3/setup.py` & `BTKSorgu-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "BTKSorgu",
-    version      = "1.1.3",
+    version      = "1.1.4",
     url          = "https://github.com/keyiflerolsun/E-Fatura_Sorgu",
     description  = "Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu",
     keywords     = ["BTKSorgu", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
```

