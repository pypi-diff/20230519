# Comparing `tmp/hive-archeology-bot-0.1.1.tar.gz` & `tmp/hive-archeology-bot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hive-archeology-bot-0.1.1.tar", last modified: Fri May 19 18:53:43 2023, max compression
+gzip compressed data, was "hive-archeology-bot-0.1.2.tar", last modified: Fri May 19 18:59:16 2023, max compression
```

## Comparing `hive-archeology-bot-0.1.1.tar` & `hive-archeology-bot-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-19 18:53:43.449216 hive-archeology-bot-0.1.1/
--rw-rw-r--   0 rob       (1000) rob       (1000)     1499 2023-05-19 18:51:54.000000 hive-archeology-bot-0.1.1/LICENSE
--rw-rw-r--   0 rob       (1000) rob       (1000)      754 2023-05-19 18:53:43.449216 hive-archeology-bot-0.1.1/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)       98 2023-05-19 18:51:54.000000 hive-archeology-bot-0.1.1/README.md
--rwxr-xr-x   0 rob       (1000) rob       (1000)    14371 2023-05-19 18:48:46.000000 hive-archeology-bot-0.1.1/hive_archeology.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-19 18:53:43.449216 hive-archeology-bot-0.1.1/hive_archeology_bot.egg-info/
--rw-rw-r--   0 rob       (1000) rob       (1000)      754 2023-05-19 18:53:43.000000 hive-archeology-bot-0.1.1/hive_archeology_bot.egg-info/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)      347 2023-05-19 18:53:43.000000 hive-archeology-bot-0.1.1/hive_archeology_bot.egg-info/SOURCES.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-19 18:53:43.000000 hive-archeology-bot-0.1.1/hive_archeology_bot.egg-info/dependency_links.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       62 2023-05-19 18:53:43.000000 hive-archeology-bot-0.1.1/hive_archeology_bot.egg-info/entry_points.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-19 18:53:43.000000 hive-archeology-bot-0.1.1/hive_archeology_bot.egg-info/not-zip-safe
--rw-rw-r--   0 rob       (1000) rob       (1000)       43 2023-05-19 18:53:43.000000 hive-archeology-bot-0.1.1/hive_archeology_bot.egg-info/requires.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       16 2023-05-19 18:53:43.000000 hive-archeology-bot-0.1.1/hive_archeology_bot.egg-info/top_level.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-19 18:53:43.449216 hive-archeology-bot-0.1.1/setup.cfg
--rwxr-xr-x   0 rob       (1000) rob       (1000)     1128 2023-05-19 18:53:41.000000 hive-archeology-bot-0.1.1/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-19 18:59:16.858200 hive-archeology-bot-0.1.2/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1499 2023-05-19 18:51:54.000000 hive-archeology-bot-0.1.2/LICENSE
+-rw-rw-r--   0 rob       (1000) rob       (1000)      754 2023-05-19 18:59:16.858200 hive-archeology-bot-0.1.2/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)       98 2023-05-19 18:51:54.000000 hive-archeology-bot-0.1.2/README.md
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    14371 2023-05-19 18:48:46.000000 hive-archeology-bot-0.1.2/hive_archeology.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-19 18:59:16.858200 hive-archeology-bot-0.1.2/hive_archeology_bot.egg-info/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      754 2023-05-19 18:59:16.000000 hive-archeology-bot-0.1.2/hive_archeology_bot.egg-info/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)      347 2023-05-19 18:59:16.000000 hive-archeology-bot-0.1.2/hive_archeology_bot.egg-info/SOURCES.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-19 18:59:16.000000 hive-archeology-bot-0.1.2/hive_archeology_bot.egg-info/dependency_links.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       62 2023-05-19 18:59:16.000000 hive-archeology-bot-0.1.2/hive_archeology_bot.egg-info/entry_points.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-19 18:53:43.000000 hive-archeology-bot-0.1.2/hive_archeology_bot.egg-info/not-zip-safe
+-rw-rw-r--   0 rob       (1000) rob       (1000)       10 2023-05-19 18:59:16.000000 hive-archeology-bot-0.1.2/hive_archeology_bot.egg-info/requires.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       16 2023-05-19 18:59:16.000000 hive-archeology-bot-0.1.2/hive_archeology_bot.egg-info/top_level.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-19 18:59:16.858200 hive-archeology-bot-0.1.2/setup.cfg
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     1089 2023-05-19 18:58:33.000000 hive-archeology-bot-0.1.2/setup.py
```

### Comparing `hive-archeology-bot-0.1.1/LICENSE` & `hive-archeology-bot-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hive-archeology-bot-0.1.1/PKG-INFO` & `hive-archeology-bot-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hive-archeology-bot
-Version: 0.1.1
+Version: 0.1.2
 Summary: Hive Archeology Bot
 Home-page: https://github.com/pibara/hive-archeology
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: hive web3 bot
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hive-archeology-bot-0.1.1/hive_archeology.py` & `hive-archeology-bot-0.1.2/hive_archeology.py`

 * *Files identical despite different names*

### Comparing `hive-archeology-bot-0.1.1/hive_archeology_bot.egg-info/PKG-INFO` & `hive-archeology-bot-0.1.2/hive_archeology_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hive-archeology-bot
-Version: 0.1.1
+Version: 0.1.2
 Summary: Hive Archeology Bot
 Home-page: https://github.com/pibara/hive-archeology
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: hive web3 bot
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hive-archeology-bot-0.1.1/setup.py` & `hive-archeology-bot-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='hive-archeology-bot',
-    version="0.1.1",
+    version="0.1.2",
     description="Hive Archeology Bot",
     long_description="Simple HIVE bot that allows its owner to up-vote valuable timeless HIVE posts.",
     author='Rob Meijer',
     author_email='pibara@gmail.com',
     url='https://github.com/pibara/hive-archeology',
     license='BSD',
     py_modules=['hive_archeology'],
@@ -25,9 +25,9 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
-    install_requires=["base58", "aioflureedb>=0.6.4", "requests<=2.28.1"],
+    install_requires=["lighthive"],
 )
```

