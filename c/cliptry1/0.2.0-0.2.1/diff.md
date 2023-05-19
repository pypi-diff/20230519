# Comparing `tmp/cliptry1-0.2.0.tar.gz` & `tmp/cliptry1-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliptry1-0.2.0.tar", last modified: Thu May 18 10:14:12 2023, max compression
+gzip compressed data, was "cliptry1-0.2.1.tar", last modified: Fri May 19 10:29:01 2023, max compression
```

## Comparing `cliptry1-0.2.0.tar` & `cliptry1-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 10:14:12.292734 cliptry1-0.2.0/
--rw-rw-rw-   0        0        0       25 2020-04-19 14:59:35.000000 cliptry1-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      236 2023-05-18 10:14:12.289734 cliptry1-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      106 2020-04-19 14:58:18.000000 cliptry1-0.2.0/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 10:14:12.272734 cliptry1-0.2.0/cliptry1.egg-info/
--rw-rw-rw-   0        0        0      236 2023-05-18 10:14:11.000000 cliptry1-0.2.0/cliptry1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-05-18 10:14:11.000000 cliptry1-0.2.0/cliptry1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      124 2023-05-18 10:14:11.000000 cliptry1-0.2.0/cliptry1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-18 10:14:11.000000 cliptry1-0.2.0/cliptry1.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-18 10:14:11.000000 cliptry1-0.2.0/cliptry1.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 10:14:12.279734 cliptry1-0.2.0/jaical/
--rw-rw-rw-   0        0        0     1799 2023-05-18 10:13:51.000000 cliptry1-0.2.0/jaical/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-18 10:14:12.294732 cliptry1-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      526 2023-05-18 10:14:01.000000 cliptry1-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 10:29:01.139002 cliptry1-0.2.1/
+-rw-rw-rw-   0        0        0       25 2020-04-19 14:59:35.000000 cliptry1-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      228 2023-05-19 10:29:01.134002 cliptry1-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      106 2020-04-19 14:58:18.000000 cliptry1-0.2.1/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 10:29:01.054154 cliptry1-0.2.1/cliptry1.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-05-19 10:28:58.000000 cliptry1-0.2.1/cliptry1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-05-19 10:28:58.000000 cliptry1-0.2.1/cliptry1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      124 2023-05-19 10:28:58.000000 cliptry1-0.2.1/cliptry1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-19 10:28:58.000000 cliptry1-0.2.1/cliptry1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-19 10:28:58.000000 cliptry1-0.2.1/cliptry1.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 10:29:01.121003 cliptry1-0.2.1/jaical/
+-rw-rw-rw-   0        0        0     2095 2023-05-19 10:28:12.000000 cliptry1-0.2.1/jaical/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-19 10:29:01.143001 cliptry1-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      518 2023-05-19 10:28:15.000000 cliptry1-0.2.1/setup.py
```

### Comparing `cliptry1-0.2.0/jaical/__init__.py` & `cliptry1-0.2.1/jaical/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import clip
 import os
 import torch
 import PIL.Image as Image
 device ="cpu"
-model, preprocess = clip.load('ViT-B/32', device)
+model, preprocess = clip.load('ViT-L/14', device)
 img_featureslist=[]
 def read_folder(path):
     pair_dir={}
     result=[]
     for roots, dirs, files in os.walk(path):
           for dirs in files:
                 result.append(os.path.join(roots, dirs))
@@ -27,27 +27,34 @@
     text_features /= text_features.norm(dim=-1, keepdim=True)
     return text_features
 def get_imagefeatures(path,pair_dir):
     #result = get_image_path(path)
     for i in range(0,len(pair_dir)):
         img_featureslist.append(image_feature_extract(pair_dir[i]))
 def similar_F(path,txt):
+    result_dir={}
     end_result=[]
     pair_dir={}
+    txt_len = len(txt.split())
+    if(txt_len<3):
+        threshold=34-(1*txt_len)
+    else:
+        threshold =30+(1*txt_len) 
     text_answer = extract_textfeatures(txt)
     pair_dir = read_folder(path)
     if(len(img_featureslist) == 0):
-        get_imagefeatures(path,pair_dir)
-    else:
-        x = len(img_featureslist)
-        print(x)
+            get_imagefeatures(path,pair_dir)
     with torch.no_grad():
         for k in range(0, len(img_featureslist)):
             ans = (10* img_featureslist[k] @ text_answer[0])
-            #print(ans)
-            if(ans >25):
-                #print(ans)
-                #print(k)
-                if k in pair_dir:
-                    i = pair_dir[k]
-                    end_result.append(i)
-    return (end_result)
+            if(ans>threshold):
+                result_dir[k]=ans
+        result_dir = dict(sorted(result_dir.items(), key=lambda item: item[1],reverse =True))
+        #print(result_dir)
+        for i in result_dir:
+            if i in pair_dir:
+                j = pair_dir[i]
+                end_result.append(j)
+    return(end_result)
+
+x = similar_F(r"C:\Users\jkaushal\Desktop\testfolder\allimages",r"boy studying on laptop")
+print(x)
```

