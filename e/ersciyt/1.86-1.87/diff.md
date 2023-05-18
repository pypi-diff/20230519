# Comparing `tmp/ersciyt-1.86.tar.gz` & `tmp/ersciyt-1.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ersciyt-1.86.tar", last modified: Thu May 18 23:40:30 2023, max compression
+gzip compressed data, was "ersciyt-1.87.tar", last modified: Thu May 18 23:46:40 2023, max compression
```

## Comparing `ersciyt-1.86.tar` & `ersciyt-1.87.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:40:30.834965 ersciyt-1.86/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-05-18 23:40:22.000000 ersciyt-1.86/LICENSE
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-18 23:40:22.000000 ersciyt-1.86/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      778 2023-05-18 23:40:30.834965 ersciyt-1.86/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      517 2023-05-18 23:40:22.000000 ersciyt-1.86/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:40:30.832965 ersciyt-1.86/ersciyt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 23:40:22.000000 ersciyt-1.86/ersciyt/__init__.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-18 23:40:22.000000 ersciyt-1.86/ersciyt/admin.py
--rw-r--r--   0 root         (0) root         (0)      146 2023-05-18 23:40:22.000000 ersciyt-1.86/ersciyt/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:40:30.834965 ersciyt-1.86/ersciyt/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 23:40:22.000000 ersciyt-1.86/ersciyt/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2023-05-18 23:40:22.000000 ersciyt-1.86/ersciyt/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:40:30.834965 ersciyt-1.86/ersciyt/static/
--rw-r--r--   0 root         (0) root         (0)    11852 2023-05-18 23:40:22.000000 ersciyt-1.86/ersciyt/static/ersci_viddown_tab2.xpi
--rw-r--r--   0 root         (0) root         (0)       60 2023-05-18 23:40:22.000000 ersciyt-1.86/ersciyt/tests.py
--rw-r--r--   0 root         (0) root         (0)      491 2023-05-18 23:40:22.000000 ersciyt-1.86/ersciyt/urls.py
--rw-r--r--   0 root         (0) root         (0)     8171 2023-05-18 23:40:22.000000 ersciyt-1.86/ersciyt/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:40:30.833965 ersciyt-1.86/ersciyt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      778 2023-05-18 23:40:30.000000 ersciyt-1.86/ersciyt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      392 2023-05-18 23:40:30.000000 ersciyt-1.86/ersciyt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 23:40:30.000000 ersciyt-1.86/ersciyt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-18 23:40:30.000000 ersciyt-1.86/ersciyt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-18 23:40:30.000000 ersciyt-1.86/ersciyt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      665 2023-05-18 23:40:30.835965 ersciyt-1.86/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-18 23:40:22.000000 ersciyt-1.86/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:46:40.046178 ersciyt-1.87/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-05-18 23:46:34.000000 ersciyt-1.87/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       69 2023-05-18 23:46:34.000000 ersciyt-1.87/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      778 2023-05-18 23:46:40.046178 ersciyt-1.87/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      517 2023-05-18 23:46:34.000000 ersciyt-1.87/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:46:40.044178 ersciyt-1.87/ersciyt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 23:46:34.000000 ersciyt-1.87/ersciyt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-18 23:46:34.000000 ersciyt-1.87/ersciyt/admin.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-05-18 23:46:34.000000 ersciyt-1.87/ersciyt/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:46:40.046178 ersciyt-1.87/ersciyt/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 23:46:34.000000 ersciyt-1.87/ersciyt/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       57 2023-05-18 23:46:34.000000 ersciyt-1.87/ersciyt/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:46:40.046178 ersciyt-1.87/ersciyt/static/
+-rw-r--r--   0 root         (0) root         (0)    11852 2023-05-18 23:46:34.000000 ersciyt-1.87/ersciyt/static/ersci_viddown_tab2.xpi
+-rw-r--r--   0 root         (0) root         (0)       60 2023-05-18 23:46:34.000000 ersciyt-1.87/ersciyt/tests.py
+-rw-r--r--   0 root         (0) root         (0)      491 2023-05-18 23:46:34.000000 ersciyt-1.87/ersciyt/urls.py
+-rw-r--r--   0 root         (0) root         (0)     8179 2023-05-18 23:46:34.000000 ersciyt-1.87/ersciyt/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:46:40.045178 ersciyt-1.87/ersciyt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      778 2023-05-18 23:46:39.000000 ersciyt-1.87/ersciyt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      392 2023-05-18 23:46:39.000000 ersciyt-1.87/ersciyt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 23:46:39.000000 ersciyt-1.87/ersciyt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-18 23:46:39.000000 ersciyt-1.87/ersciyt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-18 23:46:39.000000 ersciyt-1.87/ersciyt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      665 2023-05-18 23:46:40.047178 ersciyt-1.87/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-18 23:46:34.000000 ersciyt-1.87/setup.py
```

### Comparing `ersciyt-1.86/LICENSE` & `ersciyt-1.87/LICENSE`

 * *Files identical despite different names*

### Comparing `ersciyt-1.86/PKG-INFO` & `ersciyt-1.87/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.86
+Version: 1.87
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ersciyt-1.86/README.md` & `ersciyt-1.87/README.md`

 * *Files identical despite different names*

### Comparing `ersciyt-1.86/ersciyt/static/ersci_viddown_tab2.xpi` & `ersciyt-1.87/ersciyt/static/ersci_viddown_tab2.xpi`

 * *Files identical despite different names*

### Comparing `ersciyt-1.86/ersciyt/views.py` & `ersciyt-1.87/ersciyt/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 '''
 def ytmp4(request,link):
     try:        
         #os.system('sudo apt-get install -y ffmpeg') 
         if os.path.isfile("/tmp/a.mp4"):
             os.remove("/tmp/a.mp4")
         os.system('yt-dlp  -f 18 -o /tmp/a.mp4 https://www.youtube.com/watch?v={}'.format(link)) 
-        urllink = settings.ERSCIYT_LINK if hasattr(settings, 'ERSCIYT_LINK') and settings.ERSCIYT_LINK
+        urllink = settings.ERSCIYT_LINK if hasattr(settings, 'ERSCIYT_LINK') and settings.ERSCIYT_LINK else ""
         return redirect(urllink)
     except:
         return HttpResponse ('Youtube Url Is Mistake!')
 
 def shqr(request):
     try:
         pic=request.GET['idx']
```

### Comparing `ersciyt-1.86/ersciyt.egg-info/PKG-INFO` & `ersciyt-1.87/ersciyt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.86
+Version: 1.87
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ersciyt-1.86/setup.cfg` & `ersciyt-1.87/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ersciyt
-version = 1.86
+version = 1.87
 description = Youtube Downloader
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/epg900/yt.git
 author = epg
 author_email = epg900@gmail.com
 license = GNU GENERAL PUBLIC LICENSE
```

