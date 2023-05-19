# Comparing `tmp/BTKSorgu-1.1.6.tar.gz` & `tmp/BTKSorgu-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTKSorgu-1.1.6.tar", last modified: Fri May 19 10:47:04 2023, max compression
+gzip compressed data, was "BTKSorgu-1.1.7.tar", last modified: Fri May 19 10:54:55 2023, max compression
```

## Comparing `BTKSorgu-1.1.6.tar` & `BTKSorgu-1.1.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:47:04.599213 BTKSorgu-1.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:47:04.595213 BTKSorgu-1.1.6/BTKSorgu/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-19 10:46:42.000000 BTKSorgu-1.1.6/BTKSorgu/Erisim_Engeli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-19 10:46:42.000000 BTKSorgu-1.1.6/BTKSorgu/KekikGUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-19 10:46:42.000000 BTKSorgu-1.1.6/BTKSorgu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-19 10:46:42.000000 BTKSorgu-1.1.6/BTKSorgu/arayuz.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-19 10:46:42.000000 BTKSorgu-1.1.6/BTKSorgu/konsol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-05-19 10:46:42.000000 BTKSorgu-1.1.6/BTKSorgu/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:47:04.599213 BTKSorgu-1.1.6/BTKSorgu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-05-19 10:47:04.000000 BTKSorgu-1.1.6/BTKSorgu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-19 10:47:04.000000 BTKSorgu-1.1.6/BTKSorgu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 10:47:04.000000 BTKSorgu-1.1.6/BTKSorgu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-19 10:47:04.000000 BTKSorgu-1.1.6/BTKSorgu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-19 10:47:04.000000 BTKSorgu-1.1.6/BTKSorgu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-19 10:47:04.000000 BTKSorgu-1.1.6/BTKSorgu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-19 10:46:42.000000 BTKSorgu-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-19 10:46:42.000000 BTKSorgu-1.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-05-19 10:47:04.599213 BTKSorgu-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-05-19 10:46:42.000000 BTKSorgu-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:47:04.599213 BTKSorgu-1.1.6/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-19 10:46:42.000000 BTKSorgu-1.1.6/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-19 10:46:42.000000 BTKSorgu-1.1.6/Shared/org.KekikAkademi.BTKSorgu.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-19 10:46:42.000000 BTKSorgu-1.1.6/Shared/org.KekikAkademi.BTKSorgu.svg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 10:47:04.599213 BTKSorgu-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-19 10:46:42.000000 BTKSorgu-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:54:55.636780 BTKSorgu-1.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:54:55.632780 BTKSorgu-1.1.7/BTKSorgu/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-19 10:54:34.000000 BTKSorgu-1.1.7/BTKSorgu/Erisim_Engeli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-19 10:54:34.000000 BTKSorgu-1.1.7/BTKSorgu/KekikGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-19 10:54:34.000000 BTKSorgu-1.1.7/BTKSorgu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-19 10:54:34.000000 BTKSorgu-1.1.7/BTKSorgu/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-19 10:54:34.000000 BTKSorgu-1.1.7/BTKSorgu/konsol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-05-19 10:54:34.000000 BTKSorgu-1.1.7/BTKSorgu/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:54:55.632780 BTKSorgu-1.1.7/BTKSorgu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-05-19 10:54:55.000000 BTKSorgu-1.1.7/BTKSorgu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-19 10:54:55.000000 BTKSorgu-1.1.7/BTKSorgu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 10:54:55.000000 BTKSorgu-1.1.7/BTKSorgu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-19 10:54:55.000000 BTKSorgu-1.1.7/BTKSorgu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-19 10:54:55.000000 BTKSorgu-1.1.7/BTKSorgu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-19 10:54:55.000000 BTKSorgu-1.1.7/BTKSorgu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-19 10:54:34.000000 BTKSorgu-1.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-19 10:54:34.000000 BTKSorgu-1.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-05-19 10:54:55.632780 BTKSorgu-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-05-19 10:54:34.000000 BTKSorgu-1.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:54:55.632780 BTKSorgu-1.1.7/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-19 10:54:34.000000 BTKSorgu-1.1.7/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-19 10:54:34.000000 BTKSorgu-1.1.7/Shared/org.KekikAkademi.BTKSorgu.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-19 10:54:34.000000 BTKSorgu-1.1.7/Shared/org.KekikAkademi.BTKSorgu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 10:54:55.636780 BTKSorgu-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-19 10:54:34.000000 BTKSorgu-1.1.7/setup.py
```

### Comparing `BTKSorgu-1.1.6/BTKSorgu/Erisim_Engeli.py` & `BTKSorgu-1.1.7/BTKSorgu/Erisim_Engeli.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.6/BTKSorgu/KekikGUI.py` & `BTKSorgu-1.1.7/BTKSorgu/KekikGUI.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.6/BTKSorgu/arayuz.py` & `BTKSorgu-1.1.7/BTKSorgu/arayuz.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.6/BTKSorgu/konsol.py` & `BTKSorgu-1.1.7/BTKSorgu/konsol.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.6/BTKSorgu/logo.png` & `BTKSorgu-1.1.7/BTKSorgu/logo.png`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.6/BTKSorgu.egg-info/PKG-INFO` & `BTKSorgu-1.1.7/BTKSorgu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.1.6
+Version: 1.1.7
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/BTKSorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.1.6 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.1.7 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/BTKSorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `BTKSorgu-1.1.6/LICENSE` & `BTKSorgu-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.6/PKG-INFO` & `BTKSorgu-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.1.6
+Version: 1.1.7
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/BTKSorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.1.6 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.1.7 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/BTKSorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `BTKSorgu-1.1.6/README.md` & `BTKSorgu-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.6/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.1.7/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

 * *Files 0% similar despite different names*

#### Comparing `BTKSorgu-1.1.6/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.1.7/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

```diff
@@ -28,15 +28,15 @@
       <image>https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
-    <release version="1.1.5" date="2023-5-19">
+    <release version="1.1.7" date="2023-5-19">
       <description>
         <p>Çeşitli hatalar giderildi..</p>
       </description>
     </release>
     <release version="1.1.4" date="2023-5-18">
       <description>
         <p>Github aksiyonlarıyla otomatik paketlenme ve yayınlama eklendi..</p>
```

### Comparing `BTKSorgu-1.1.6/Shared/org.KekikAkademi.BTKSorgu.svg` & `BTKSorgu-1.1.7/Shared/org.KekikAkademi.BTKSorgu.svg`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.1.6/setup.py` & `BTKSorgu-1.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "BTKSorgu",
-    version      = "1.1.6",
+    version      = "1.1.7",
     url          = "https://github.com/keyiflerolsun/BTKSorgu",
     description  = "Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu",
     keywords     = ["BTKSorgu", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
```

