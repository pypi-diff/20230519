# Comparing `tmp/nwebclient-1.0.93.tar.gz` & `tmp/nwebclient-1.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nwebclient-1.0.93.tar", last modified: Fri May 19 11:09:39 2023, max compression
+gzip compressed data, was "dist/nwebclient-1.0.94.tar", last modified: Fri May 19 11:14:44 2023, max compression
```

## Comparing `nwebclient-1.0.93.tar` & `nwebclient-1.0.94.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-19 11:09:39.206337 nwebclient-1.0.93/
--rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.93/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-19 11:09:39.206337 nwebclient-1.0.93/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.93/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-19 11:09:39.196337 nwebclient-1.0.93/nwebclient/
--rw-r--r--   0 pi        (1000) pi        (1000)     6483 2023-05-12 07:26:49.000000 nwebclient-1.0.93/nwebclient/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.93/nwebclient/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3316 2023-05-09 12:58:28.000000 nwebclient-1.0.93/nwebclient/crypt.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3545 2023-05-14 17:14:29.000000 nwebclient-1.0.93/nwebclient/nlp.py
--rw-r--r--   0 pi        (1000) pi        (1000)    14410 2023-05-19 07:18:25.000000 nwebclient-1.0.93/nwebclient/sd.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6100 2023-05-05 17:05:53.000000 nwebclient-1.0.93/nwebclient/sdb.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.93/nwebclient/ticker.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-19 11:09:39.206337 nwebclient-1.0.93/nwebclient.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-19 11:09:39.000000 nwebclient-1.0.93/nwebclient.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      382 2023-05-19 11:09:39.000000 nwebclient-1.0.93/nwebclient.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-19 11:09:39.000000 nwebclient-1.0.93/nwebclient.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-19 11:09:39.000000 nwebclient-1.0.93/nwebclient.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-19 11:09:39.000000 nwebclient-1.0.93/nwebclient.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-19 11:09:39.000000 nwebclient-1.0.93/nwebclient.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-19 11:09:39.206337 nwebclient-1.0.93/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-19 11:09:34.000000 nwebclient-1.0.93/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-19 11:14:44.011574 nwebclient-1.0.94/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.94/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-19 11:14:44.011574 nwebclient-1.0.94/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.94/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-19 11:14:44.011574 nwebclient-1.0.94/nwebclient/
+-rw-r--r--   0 pi        (1000) pi        (1000)     6483 2023-05-12 07:26:49.000000 nwebclient-1.0.94/nwebclient/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.94/nwebclient/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3316 2023-05-09 12:58:28.000000 nwebclient-1.0.94/nwebclient/crypt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3545 2023-05-14 17:14:29.000000 nwebclient-1.0.94/nwebclient/nlp.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    13658 2023-05-19 11:14:32.000000 nwebclient-1.0.94/nwebclient/sd.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     6100 2023-05-05 17:05:53.000000 nwebclient-1.0.94/nwebclient/sdb.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.94/nwebclient/ticker.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-19 11:14:44.011574 nwebclient-1.0.94/nwebclient.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-19 11:14:43.000000 nwebclient-1.0.94/nwebclient.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      382 2023-05-19 11:14:43.000000 nwebclient-1.0.94/nwebclient.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-19 11:14:43.000000 nwebclient-1.0.94/nwebclient.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-19 11:14:43.000000 nwebclient-1.0.94/nwebclient.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-19 11:14:43.000000 nwebclient-1.0.94/nwebclient.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-19 11:14:43.000000 nwebclient-1.0.94/nwebclient.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-19 11:14:44.011574 nwebclient-1.0.94/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-19 11:14:41.000000 nwebclient-1.0.94/setup.py
```

### Comparing `nwebclient-1.0.93/LICENSE` & `nwebclient-1.0.94/LICENSE`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.93/PKG-INFO` & `nwebclient-1.0.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.93
+Version: 1.0.94
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.93/README.md` & `nwebclient-1.0.94/README.md`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.93/nwebclient/__init__.py` & `nwebclient-1.0.94/nwebclient/__init__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.93/nwebclient/__main__.py` & `nwebclient-1.0.94/nwebclient/__main__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.93/nwebclient/crypt.py` & `nwebclient-1.0.94/nwebclient/crypt.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.93/nwebclient/nlp.py` & `nwebclient-1.0.94/nwebclient/nlp.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.93/nwebclient/sd.py` & `nwebclient-1.0.94/nwebclient/sd.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,14 @@
 import os.path
 import requests
 import time
 import base64
 
 # Stable Diffusion Imports in ImageGen::__init__
 
-def gen(pipe, prompt='photo', negative_prompt = None, prefix='sd',  guidance_scale = 7.5, num_inference_steps=30, height=800, width=640, num_images=1, dbfile='data.db'):
-    # https://huggingface.co/docs/diffusers/v0.14.0/en/
-      prompt,
-      height = 800,
-      width = 640,
-      num_inference_steps = num_inference_steps,      # higher better quali default=45
-      guidance_scale = guidance_scale,                # Prioritize creativity  7.5  Prioritize prompt (higher)
-      num_images_per_prompt = num_images,
-      negative_prompt = negative_prompt,
-      ).images
-    for i in range(len(images)):
-        #  images[i].save(prefix+str(i)+".jpg")
-        sdb.sdb_write_pil(images[i], prompt, negative_prompt, guidance_scale, prefix, dbfile)
-
-
 class ImageGen:
     """
     from nwebclient import sd
     ig = sd.ImageGen()
     ig.prompt = "photo"
     ig.loop(5)
```

### Comparing `nwebclient-1.0.93/nwebclient/sdb.py` & `nwebclient-1.0.94/nwebclient/sdb.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.93/nwebclient/ticker.py` & `nwebclient-1.0.94/nwebclient/ticker.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.93/nwebclient.egg-info/PKG-INFO` & `nwebclient-1.0.94/nwebclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.93
+Version: 1.0.94
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.93/setup.py` & `nwebclient-1.0.94/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nwebclient",
-    version="1.0.93",
+    version="1.0.94",
     author="Bjoern Salgert",
     author_email="bjoern.salgert@hs-duesseldorf.de",
     description="NWebClient via HTTP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bsnx.net/4.0/group/pynwebclient",
     packages=setuptools.find_packages(),
```

