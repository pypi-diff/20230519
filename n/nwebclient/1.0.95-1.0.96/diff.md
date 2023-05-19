# Comparing `tmp/nwebclient-1.0.95.tar.gz` & `tmp/nwebclient-1.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nwebclient-1.0.95.tar", last modified: Fri May 19 11:17:33 2023, max compression
+gzip compressed data, was "dist/nwebclient-1.0.96.tar", last modified: Fri May 19 11:19:30 2023, max compression
```

## Comparing `nwebclient-1.0.95.tar` & `nwebclient-1.0.96.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-19 11:17:33.848907 nwebclient-1.0.95/
--rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.95/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-19 11:17:33.848907 nwebclient-1.0.95/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.95/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-19 11:17:33.838907 nwebclient-1.0.95/nwebclient/
--rw-r--r--   0 pi        (1000) pi        (1000)     6483 2023-05-12 07:26:49.000000 nwebclient-1.0.95/nwebclient/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.95/nwebclient/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3316 2023-05-09 12:58:28.000000 nwebclient-1.0.95/nwebclient/crypt.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3545 2023-05-14 17:14:29.000000 nwebclient-1.0.95/nwebclient/nlp.py
--rw-r--r--   0 pi        (1000) pi        (1000)    13667 2023-05-19 11:17:14.000000 nwebclient-1.0.95/nwebclient/sd.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6100 2023-05-05 17:05:53.000000 nwebclient-1.0.95/nwebclient/sdb.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.95/nwebclient/ticker.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-19 11:17:33.848907 nwebclient-1.0.95/nwebclient.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-19 11:17:33.000000 nwebclient-1.0.95/nwebclient.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      382 2023-05-19 11:17:33.000000 nwebclient-1.0.95/nwebclient.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-19 11:17:33.000000 nwebclient-1.0.95/nwebclient.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-19 11:17:33.000000 nwebclient-1.0.95/nwebclient.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-19 11:17:33.000000 nwebclient-1.0.95/nwebclient.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-19 11:17:33.000000 nwebclient-1.0.95/nwebclient.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-19 11:17:33.848907 nwebclient-1.0.95/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-19 11:17:31.000000 nwebclient-1.0.95/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-19 11:19:30.487072 nwebclient-1.0.96/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.96/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-19 11:19:30.487072 nwebclient-1.0.96/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.96/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-19 11:19:30.487072 nwebclient-1.0.96/nwebclient/
+-rw-r--r--   0 pi        (1000) pi        (1000)     6483 2023-05-12 07:26:49.000000 nwebclient-1.0.96/nwebclient/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.96/nwebclient/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3316 2023-05-09 12:58:28.000000 nwebclient-1.0.96/nwebclient/crypt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3545 2023-05-14 17:14:29.000000 nwebclient-1.0.96/nwebclient/nlp.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    13673 2023-05-19 11:19:17.000000 nwebclient-1.0.96/nwebclient/sd.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     6100 2023-05-05 17:05:53.000000 nwebclient-1.0.96/nwebclient/sdb.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.96/nwebclient/ticker.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-19 11:19:30.487072 nwebclient-1.0.96/nwebclient.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-19 11:19:30.000000 nwebclient-1.0.96/nwebclient.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      382 2023-05-19 11:19:30.000000 nwebclient-1.0.96/nwebclient.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-19 11:19:30.000000 nwebclient-1.0.96/nwebclient.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-19 11:19:30.000000 nwebclient-1.0.96/nwebclient.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-19 11:19:30.000000 nwebclient-1.0.96/nwebclient.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-19 11:19:30.000000 nwebclient-1.0.96/nwebclient.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-19 11:19:30.487072 nwebclient-1.0.96/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-19 11:19:28.000000 nwebclient-1.0.96/setup.py
```

### Comparing `nwebclient-1.0.95/LICENSE` & `nwebclient-1.0.96/LICENSE`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.95/PKG-INFO` & `nwebclient-1.0.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.95
+Version: 1.0.96
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.95/README.md` & `nwebclient-1.0.96/README.md`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.95/nwebclient/__init__.py` & `nwebclient-1.0.96/nwebclient/__init__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.95/nwebclient/__main__.py` & `nwebclient-1.0.96/nwebclient/__main__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.95/nwebclient/crypt.py` & `nwebclient-1.0.96/nwebclient/crypt.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.95/nwebclient/nlp.py` & `nwebclient-1.0.96/nwebclient/nlp.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.95/nwebclient/sd.py` & `nwebclient-1.0.96/nwebclient/sd.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
     def __repr__(self):
         return f'ImageGen(generator=\'{self.generator}\', model_id=\'{self.model_id}\', prefix=\'{self.prefix}\')'
     def __call__(self, prefix, prompt):
         self.prompt = prompt
         self.prefix = prefix
         self.loop(self.loop_count)
         return "ImageGen"
-    def toSdJob(count:50, file = None):
+    def toSdJob(self, count:50, file = None):
         data = {'prefix':self.prefix, 'prompt':self.prompt, 'count':count, 'height': self.height, 'width':self.width}
         if not file is None:
             text = json.dumps(data)
             with open(self.prefix +'.sdjob', 'w') as f:
                 f.write(text)
         return data
     def p(self, prompt, append = False):
```

### Comparing `nwebclient-1.0.95/nwebclient/sdb.py` & `nwebclient-1.0.96/nwebclient/sdb.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.95/nwebclient/ticker.py` & `nwebclient-1.0.96/nwebclient/ticker.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.95/nwebclient.egg-info/PKG-INFO` & `nwebclient-1.0.96/nwebclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.95
+Version: 1.0.96
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.95/setup.py` & `nwebclient-1.0.96/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nwebclient",
-    version="1.0.95",
+    version="1.0.96",
     author="Bjoern Salgert",
     author_email="bjoern.salgert@hs-duesseldorf.de",
     description="NWebClient via HTTP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bsnx.net/4.0/group/pynwebclient",
     packages=setuptools.find_packages(),
```

