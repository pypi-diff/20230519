# Comparing `tmp/gtocclient-0.7.8.tar.gz` & `tmp/gtocclient-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gtocclient-0.7.8.tar", last modified: Thu Mar 31 06:37:43 2022, max compression
+gzip compressed data, was "dist/gtocclient-0.7.9.tar", last modified: Wed Apr  6 02:20:22 2022, max compression
```

## Comparing `gtocclient-0.7.8.tar` & `gtocclient-0.7.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 yebk       (501) staff       (20)        0 2022-03-31 06:37:43.000000 gtocclient-0.7.8/
--rw-r--r--   0 yebk       (501) staff       (20)     4584 2022-03-31 06:37:43.000000 gtocclient-0.7.8/PKG-INFO
-drwxr-xr-x   0 yebk       (501) staff       (20)        0 2022-03-31 06:37:43.000000 gtocclient-0.7.8/gtocclient.egg-info/
--rw-r--r--   0 yebk       (501) staff       (20)     4584 2022-03-31 06:37:43.000000 gtocclient-0.7.8/gtocclient.egg-info/PKG-INFO
--rw-r--r--   0 yebk       (501) staff       (20)      883 2022-03-31 06:37:43.000000 gtocclient-0.7.8/gtocclient.egg-info/SOURCES.txt
--rw-r--r--   0 yebk       (501) staff       (20)       65 2022-03-31 06:37:43.000000 gtocclient-0.7.8/gtocclient.egg-info/entry_points.txt
--rw-r--r--   0 yebk       (501) staff       (20)       54 2022-03-31 06:37:43.000000 gtocclient-0.7.8/gtocclient.egg-info/requires.txt
--rw-r--r--   0 yebk       (501) staff       (20)        9 2022-03-31 06:37:43.000000 gtocclient-0.7.8/gtocclient.egg-info/top_level.txt
--rw-r--r--   0 yebk       (501) staff       (20)        1 2022-03-31 06:37:43.000000 gtocclient-0.7.8/gtocclient.egg-info/dependency_links.txt
--rw-r--r--   0 yebk       (501) staff       (20)        0 2021-03-02 07:55:59.000000 gtocclient-0.7.8/CHANGELOG.md
-drwxr-xr-x   0 yebk       (501) staff       (20)        0 2022-03-31 06:37:43.000000 gtocclient-0.7.8/owncloud/
--rw-r--r--   0 yebk       (501) staff       (20)    13129 2021-04-09 09:05:01.000000 gtocclient-0.7.8/owncloud/config.py
-drwxr-xr-x   0 yebk       (501) staff       (20)        0 2022-03-31 06:37:43.000000 gtocclient-0.7.8/owncloud/test/
--rw-r--r--   0 yebk       (501) staff       (20)      865 2021-06-15 07:00:11.000000 gtocclient-0.7.8/owncloud/test/config.py
--rw-r--r--   0 yebk       (501) staff       (20)      862 2021-01-20 07:34:31.000000 gtocclient-0.7.8/owncloud/test/config.py.sample
--rw-r--r--   0 yebk       (501) staff       (20)        0 2021-01-20 07:34:31.000000 gtocclient-0.7.8/owncloud/test/__init__.py
--rw-r--r--   0 yebk       (501) staff       (20)    59798 2021-09-06 03:01:09.000000 gtocclient-0.7.8/owncloud/test/test.py
--rw-r--r--   0 yebk       (501) staff       (20)     1134 2021-03-02 05:57:59.000000 gtocclient-0.7.8/owncloud/bidir_map.py
--rw-r--r--   0 yebk       (501) staff       (20)     2138 2021-03-02 05:57:59.000000 gtocclient-0.7.8/owncloud/exit_codes.py
--rw-r--r--   0 yebk       (501) staff       (20)       88 2022-03-31 06:29:21.000000 gtocclient-0.7.8/owncloud/__init__.py
--rwxr-xr-x   0 yebk       (501) staff       (20)    44331 2022-03-04 03:12:30.000000 gtocclient-0.7.8/owncloud/occmd.py
--rw-r--r--   0 yebk       (501) staff       (20)     7694 2021-03-11 11:45:57.000000 gtocclient-0.7.8/owncloud/utils.py
--rw-r--r--   0 yebk       (501) staff       (20)     1519 2021-03-10 02:15:16.000000 gtocclient-0.7.8/owncloud/exceptions.py
--rw-r--r--   0 yebk       (501) staff       (20)      214 2022-03-31 06:29:21.000000 gtocclient-0.7.8/owncloud/pkg_info.py
--rw-r--r--   0 yebk       (501) staff       (20)    11201 2022-03-04 09:27:25.000000 gtocclient-0.7.8/owncloud/progress.py
--rw-r--r--   0 yebk       (501) staff       (20)     2626 2021-03-03 09:14:44.000000 gtocclient-0.7.8/owncloud/sorted_dict.py
--rw-r--r--   0 yebk       (501) staff       (20)    81617 2022-03-30 12:13:42.000000 gtocclient-0.7.8/owncloud/oc.py
--rwxr-xr-x   0 yebk       (501) staff       (20)       55 2021-01-20 07:34:31.000000 gtocclient-0.7.8/runtests.sh
--rw-r--r--   0 yebk       (501) staff       (20)       56 2021-01-20 07:34:31.000000 gtocclient-0.7.8/MANIFEST.in
-drwxr-xr-x   0 yebk       (501) staff       (20)        0 2022-03-31 06:37:43.000000 gtocclient-0.7.8/docs/
--rw-r--r--   0 yebk       (501) staff       (20)     6803 2021-01-20 07:34:31.000000 gtocclient-0.7.8/docs/Makefile
-drwxr-xr-x   0 yebk       (501) staff       (20)        0 2022-03-31 06:37:43.000000 gtocclient-0.7.8/docs/source/
--rw-r--r--   0 yebk       (501) staff       (20)      524 2021-01-20 07:34:31.000000 gtocclient-0.7.8/docs/source/index.rst
--rw-r--r--   0 yebk       (501) staff       (20)      133 2021-01-20 07:34:31.000000 gtocclient-0.7.8/docs/source/owncloud.utils.rst
--rw-r--r--   0 yebk       (501) staff       (20)     8434 2021-01-20 07:34:31.000000 gtocclient-0.7.8/docs/source/conf.py
--rw-r--r--   0 yebk       (501) staff       (20)      227 2021-01-20 07:34:31.000000 gtocclient-0.7.8/docs/source/owncloud.rst
--rw-r--r--   0 yebk       (501) staff       (20)       61 2021-01-20 07:34:31.000000 gtocclient-0.7.8/docs/source/modules.rst
--rw-r--r--   0 yebk       (501) staff       (20)      685 2021-01-20 07:34:31.000000 gtocclient-0.7.8/docs/source/CONTRIBUTORS.rst
--rw-r--r--   0 yebk       (501) staff       (20)      142 2021-01-20 07:34:31.000000 gtocclient-0.7.8/docs/source/owncloud.owncloud.rst
--rw-r--r--   0 yebk       (501) staff       (20)     2878 2021-01-20 07:34:31.000000 gtocclient-0.7.8/docs/source/README.rst
--rw-r--r--   0 yebk       (501) staff       (20)     1773 2021-01-20 07:34:31.000000 gtocclient-0.7.8/docs/source/CHANGES.rst
--rw-r--r--   0 yebk       (501) staff       (20)     6726 2021-01-20 07:34:31.000000 gtocclient-0.7.8/docs/make.bat
--rw-r--r--   0 yebk       (501) staff       (20)     1353 2022-03-30 12:24:47.000000 gtocclient-0.7.8/setup.py
--rw-r--r--   0 yebk       (501) staff       (20)      109 2021-03-10 02:36:38.000000 gtocclient-0.7.8/.gitignore
--rw-r--r--   0 yebk       (501) staff       (20)      162 2022-03-31 06:37:43.000000 gtocclient-0.7.8/setup.cfg
--rw-r--r--   0 yebk       (501) staff       (20)     2878 2021-01-20 07:34:31.000000 gtocclient-0.7.8/README.rst
--rw-r--r--   0 yebk       (501) staff       (20)     1104 2021-01-20 07:34:31.000000 gtocclient-0.7.8/LICENSE.txt
+drwxr-xr-x   0 yebk       (501) staff       (20)        0 2022-04-06 02:20:22.000000 gtocclient-0.7.9/
+-rw-r--r--   0 yebk       (501) staff       (20)     4584 2022-04-06 02:20:22.000000 gtocclient-0.7.9/PKG-INFO
+drwxr-xr-x   0 yebk       (501) staff       (20)        0 2022-04-06 02:20:22.000000 gtocclient-0.7.9/gtocclient.egg-info/
+-rw-r--r--   0 yebk       (501) staff       (20)     4584 2022-04-06 02:20:22.000000 gtocclient-0.7.9/gtocclient.egg-info/PKG-INFO
+-rw-r--r--   0 yebk       (501) staff       (20)      883 2022-04-06 02:20:22.000000 gtocclient-0.7.9/gtocclient.egg-info/SOURCES.txt
+-rw-r--r--   0 yebk       (501) staff       (20)       65 2022-04-06 02:20:22.000000 gtocclient-0.7.9/gtocclient.egg-info/entry_points.txt
+-rw-r--r--   0 yebk       (501) staff       (20)       54 2022-04-06 02:20:22.000000 gtocclient-0.7.9/gtocclient.egg-info/requires.txt
+-rw-r--r--   0 yebk       (501) staff       (20)        9 2022-04-06 02:20:22.000000 gtocclient-0.7.9/gtocclient.egg-info/top_level.txt
+-rw-r--r--   0 yebk       (501) staff       (20)        1 2022-04-06 02:20:22.000000 gtocclient-0.7.9/gtocclient.egg-info/dependency_links.txt
+-rw-r--r--   0 yebk       (501) staff       (20)        0 2021-03-02 07:55:59.000000 gtocclient-0.7.9/CHANGELOG.md
+drwxr-xr-x   0 yebk       (501) staff       (20)        0 2022-04-06 02:20:22.000000 gtocclient-0.7.9/owncloud/
+-rw-r--r--   0 yebk       (501) staff       (20)    13129 2021-04-09 09:05:01.000000 gtocclient-0.7.9/owncloud/config.py
+drwxr-xr-x   0 yebk       (501) staff       (20)        0 2022-04-06 02:20:22.000000 gtocclient-0.7.9/owncloud/test/
+-rw-r--r--   0 yebk       (501) staff       (20)      865 2021-06-15 07:00:11.000000 gtocclient-0.7.9/owncloud/test/config.py
+-rw-r--r--   0 yebk       (501) staff       (20)      862 2021-01-20 07:34:31.000000 gtocclient-0.7.9/owncloud/test/config.py.sample
+-rw-r--r--   0 yebk       (501) staff       (20)        0 2021-01-20 07:34:31.000000 gtocclient-0.7.9/owncloud/test/__init__.py
+-rw-r--r--   0 yebk       (501) staff       (20)    59798 2021-09-06 03:01:09.000000 gtocclient-0.7.9/owncloud/test/test.py
+-rw-r--r--   0 yebk       (501) staff       (20)     1134 2021-03-02 05:57:59.000000 gtocclient-0.7.9/owncloud/bidir_map.py
+-rw-r--r--   0 yebk       (501) staff       (20)     2138 2021-03-02 05:57:59.000000 gtocclient-0.7.9/owncloud/exit_codes.py
+-rw-r--r--   0 yebk       (501) staff       (20)       88 2022-03-31 06:29:21.000000 gtocclient-0.7.9/owncloud/__init__.py
+-rwxr-xr-x   0 yebk       (501) staff       (20)    44331 2022-03-04 03:12:30.000000 gtocclient-0.7.9/owncloud/occmd.py
+-rw-r--r--   0 yebk       (501) staff       (20)     7694 2021-03-11 11:45:57.000000 gtocclient-0.7.9/owncloud/utils.py
+-rw-r--r--   0 yebk       (501) staff       (20)     1519 2021-03-10 02:15:16.000000 gtocclient-0.7.9/owncloud/exceptions.py
+-rw-r--r--   0 yebk       (501) staff       (20)      214 2022-04-06 02:20:17.000000 gtocclient-0.7.9/owncloud/pkg_info.py
+-rw-r--r--   0 yebk       (501) staff       (20)    11201 2022-03-04 09:27:25.000000 gtocclient-0.7.9/owncloud/progress.py
+-rw-r--r--   0 yebk       (501) staff       (20)     2626 2021-03-03 09:14:44.000000 gtocclient-0.7.9/owncloud/sorted_dict.py
+-rw-r--r--   0 yebk       (501) staff       (20)    81954 2022-04-06 02:19:50.000000 gtocclient-0.7.9/owncloud/oc.py
+-rwxr-xr-x   0 yebk       (501) staff       (20)       55 2021-01-20 07:34:31.000000 gtocclient-0.7.9/runtests.sh
+-rw-r--r--   0 yebk       (501) staff       (20)       56 2021-01-20 07:34:31.000000 gtocclient-0.7.9/MANIFEST.in
+drwxr-xr-x   0 yebk       (501) staff       (20)        0 2022-04-06 02:20:22.000000 gtocclient-0.7.9/docs/
+-rw-r--r--   0 yebk       (501) staff       (20)     6803 2021-01-20 07:34:31.000000 gtocclient-0.7.9/docs/Makefile
+drwxr-xr-x   0 yebk       (501) staff       (20)        0 2022-04-06 02:20:22.000000 gtocclient-0.7.9/docs/source/
+-rw-r--r--   0 yebk       (501) staff       (20)      524 2021-01-20 07:34:31.000000 gtocclient-0.7.9/docs/source/index.rst
+-rw-r--r--   0 yebk       (501) staff       (20)      133 2021-01-20 07:34:31.000000 gtocclient-0.7.9/docs/source/owncloud.utils.rst
+-rw-r--r--   0 yebk       (501) staff       (20)     8434 2021-01-20 07:34:31.000000 gtocclient-0.7.9/docs/source/conf.py
+-rw-r--r--   0 yebk       (501) staff       (20)      227 2021-01-20 07:34:31.000000 gtocclient-0.7.9/docs/source/owncloud.rst
+-rw-r--r--   0 yebk       (501) staff       (20)       61 2021-01-20 07:34:31.000000 gtocclient-0.7.9/docs/source/modules.rst
+-rw-r--r--   0 yebk       (501) staff       (20)      685 2021-01-20 07:34:31.000000 gtocclient-0.7.9/docs/source/CONTRIBUTORS.rst
+-rw-r--r--   0 yebk       (501) staff       (20)      142 2021-01-20 07:34:31.000000 gtocclient-0.7.9/docs/source/owncloud.owncloud.rst
+-rw-r--r--   0 yebk       (501) staff       (20)     2878 2021-01-20 07:34:31.000000 gtocclient-0.7.9/docs/source/README.rst
+-rw-r--r--   0 yebk       (501) staff       (20)     1773 2021-01-20 07:34:31.000000 gtocclient-0.7.9/docs/source/CHANGES.rst
+-rw-r--r--   0 yebk       (501) staff       (20)     6726 2021-01-20 07:34:31.000000 gtocclient-0.7.9/docs/make.bat
+-rw-r--r--   0 yebk       (501) staff       (20)     1353 2022-03-30 12:24:47.000000 gtocclient-0.7.9/setup.py
+-rw-r--r--   0 yebk       (501) staff       (20)      109 2021-03-10 02:36:38.000000 gtocclient-0.7.9/.gitignore
+-rw-r--r--   0 yebk       (501) staff       (20)      162 2022-04-06 02:20:22.000000 gtocclient-0.7.9/setup.cfg
+-rw-r--r--   0 yebk       (501) staff       (20)     2878 2021-01-20 07:34:31.000000 gtocclient-0.7.9/README.rst
+-rw-r--r--   0 yebk       (501) staff       (20)     1104 2021-01-20 07:34:31.000000 gtocclient-0.7.9/LICENSE.txt
```

### Comparing `gtocclient-0.7.8/PKG-INFO` & `gtocclient-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: gtocclient
-Version: 0.7.8
+Version: 0.7.9
 Summary: Getui Custom-Developed Python client library for ownCloud
 Home-page: https://www.getui.com
 Author: Getui
 Author-email: support@getui.com
 License: LICENSE.txt
 Description: =======================================
         Getui Custom-Developed ownCloud library
```

### Comparing `gtocclient-0.7.8/gtocclient.egg-info/PKG-INFO` & `gtocclient-0.7.9/gtocclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: gtocclient
-Version: 0.7.8
+Version: 0.7.9
 Summary: Getui Custom-Developed Python client library for ownCloud
 Home-page: https://www.getui.com
 Author: Getui
 Author-email: support@getui.com
 License: LICENSE.txt
 Description: =======================================
         Getui Custom-Developed ownCloud library
```

### Comparing `gtocclient-0.7.8/gtocclient.egg-info/SOURCES.txt` & `gtocclient-0.7.9/gtocclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gtocclient-0.7.8/owncloud/config.py` & `gtocclient-0.7.9/owncloud/config.py`

 * *Files identical despite different names*

### Comparing `gtocclient-0.7.8/owncloud/test/config.py` & `gtocclient-0.7.9/owncloud/test/config.py`

 * *Files identical despite different names*

### Comparing `gtocclient-0.7.8/owncloud/test/config.py.sample` & `gtocclient-0.7.9/owncloud/test/config.py.sample`

 * *Files identical despite different names*

### Comparing `gtocclient-0.7.8/owncloud/test/test.py` & `gtocclient-0.7.9/owncloud/test/test.py`

 * *Files identical despite different names*

### Comparing `gtocclient-0.7.8/owncloud/bidir_map.py` & `gtocclient-0.7.9/owncloud/bidir_map.py`

 * *Files identical despite different names*

### Comparing `gtocclient-0.7.8/owncloud/exit_codes.py` & `gtocclient-0.7.9/owncloud/exit_codes.py`

 * *Files identical despite different names*

### Comparing `gtocclient-0.7.8/owncloud/occmd.py` & `gtocclient-0.7.9/owncloud/occmd.py`

 * *Files identical despite different names*

### Comparing `gtocclient-0.7.8/owncloud/utils.py` & `gtocclient-0.7.9/owncloud/utils.py`

 * *Files identical despite different names*

### Comparing `gtocclient-0.7.8/owncloud/exceptions.py` & `gtocclient-0.7.9/owncloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `gtocclient-0.7.8/owncloud/progress.py` & `gtocclient-0.7.9/owncloud/progress.py`

 * *Files identical despite different names*

### Comparing `gtocclient-0.7.8/owncloud/sorted_dict.py` & `gtocclient-0.7.9/owncloud/sorted_dict.py`

 * *Files identical despite different names*

### Comparing `gtocclient-0.7.8/owncloud/oc.py` & `gtocclient-0.7.9/owncloud/oc.py`

 * *Files 1% similar despite different names*

```diff
@@ -721,15 +721,19 @@
             return self._put_file_chunked(
                 remote_path,
                 local_source_file,
                 **kwargs
             )
 
         stat_result = os.stat(local_source_file)
-
+        if stat_result.st_size > 30*1024*1024*1024:
+            print("Error: Uploading files larger than 30G is not allowed.")
+            return
+        if stat_result.st_size > 20*1024*1024*1024:
+            print("Warn: Uploading files larger than 20G is not guaranteed to be stable. Please split it into a number of smaller files.")
         headers = {}
         mime_type = magic.from_file(local_source_file, mime=True)
         headers['Content-Type'] = mime_type
         if kwargs.get('keep_mtime', True):
             headers['X-OC-MTIME'] = str(int(stat_result.st_mtime))
 
         file_handle = open(local_source_file, 'rb', 8192)
```

### Comparing `gtocclient-0.7.8/docs/Makefile` & `gtocclient-0.7.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gtocclient-0.7.8/docs/source/index.rst` & `gtocclient-0.7.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `gtocclient-0.7.8/docs/source/conf.py` & `gtocclient-0.7.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gtocclient-0.7.8/docs/source/CONTRIBUTORS.rst` & `gtocclient-0.7.9/docs/source/CONTRIBUTORS.rst`

 * *Files identical despite different names*

### Comparing `gtocclient-0.7.8/docs/source/README.rst` & `gtocclient-0.7.9/docs/source/README.rst`

 * *Files identical despite different names*

### Comparing `gtocclient-0.7.8/docs/source/CHANGES.rst` & `gtocclient-0.7.9/docs/source/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `gtocclient-0.7.8/docs/make.bat` & `gtocclient-0.7.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gtocclient-0.7.8/setup.py` & `gtocclient-0.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `gtocclient-0.7.8/README.rst` & `gtocclient-0.7.9/README.rst`

 * *Files identical despite different names*

### Comparing `gtocclient-0.7.8/LICENSE.txt` & `gtocclient-0.7.9/LICENSE.txt`

 * *Files identical despite different names*

