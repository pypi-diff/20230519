# Comparing `tmp/ersciyt-1.85.tar.gz` & `tmp/ersciyt-1.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ersciyt-1.85.tar", last modified: Thu May 18 23:16:12 2023, max compression
+gzip compressed data, was "ersciyt-1.86.tar", last modified: Thu May 18 23:40:30 2023, max compression
```

## Comparing `ersciyt-1.85.tar` & `ersciyt-1.86.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:16:12.948716 ersciyt-1.85/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-05-18 23:16:05.000000 ersciyt-1.85/LICENSE
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-18 23:16:05.000000 ersciyt-1.85/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      778 2023-05-18 23:16:12.948716 ersciyt-1.85/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      517 2023-05-18 23:16:05.000000 ersciyt-1.85/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:16:12.946715 ersciyt-1.85/ersciyt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 23:16:05.000000 ersciyt-1.85/ersciyt/__init__.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-18 23:16:05.000000 ersciyt-1.85/ersciyt/admin.py
--rw-r--r--   0 root         (0) root         (0)      146 2023-05-18 23:16:05.000000 ersciyt-1.85/ersciyt/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:16:12.948716 ersciyt-1.85/ersciyt/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 23:16:05.000000 ersciyt-1.85/ersciyt/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2023-05-18 23:16:05.000000 ersciyt-1.85/ersciyt/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:16:12.948716 ersciyt-1.85/ersciyt/static/
--rw-r--r--   0 root         (0) root         (0)    11852 2023-05-18 23:16:05.000000 ersciyt-1.85/ersciyt/static/ersci_viddown_tab2.xpi
--rw-r--r--   0 root         (0) root         (0)       60 2023-05-18 23:16:05.000000 ersciyt-1.85/ersciyt/tests.py
--rw-r--r--   0 root         (0) root         (0)      491 2023-05-18 23:16:05.000000 ersciyt-1.85/ersciyt/urls.py
--rw-r--r--   0 root         (0) root         (0)     8236 2023-05-18 23:16:05.000000 ersciyt-1.85/ersciyt/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:16:12.947716 ersciyt-1.85/ersciyt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      778 2023-05-18 23:16:12.000000 ersciyt-1.85/ersciyt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      392 2023-05-18 23:16:12.000000 ersciyt-1.85/ersciyt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 23:16:12.000000 ersciyt-1.85/ersciyt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-18 23:16:12.000000 ersciyt-1.85/ersciyt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-18 23:16:12.000000 ersciyt-1.85/ersciyt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      665 2023-05-18 23:16:12.949716 ersciyt-1.85/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-18 23:16:05.000000 ersciyt-1.85/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:40:30.834965 ersciyt-1.86/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-05-18 23:40:22.000000 ersciyt-1.86/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       69 2023-05-18 23:40:22.000000 ersciyt-1.86/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      778 2023-05-18 23:40:30.834965 ersciyt-1.86/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      517 2023-05-18 23:40:22.000000 ersciyt-1.86/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:40:30.832965 ersciyt-1.86/ersciyt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 23:40:22.000000 ersciyt-1.86/ersciyt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-18 23:40:22.000000 ersciyt-1.86/ersciyt/admin.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-05-18 23:40:22.000000 ersciyt-1.86/ersciyt/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:40:30.834965 ersciyt-1.86/ersciyt/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 23:40:22.000000 ersciyt-1.86/ersciyt/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       57 2023-05-18 23:40:22.000000 ersciyt-1.86/ersciyt/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:40:30.834965 ersciyt-1.86/ersciyt/static/
+-rw-r--r--   0 root         (0) root         (0)    11852 2023-05-18 23:40:22.000000 ersciyt-1.86/ersciyt/static/ersci_viddown_tab2.xpi
+-rw-r--r--   0 root         (0) root         (0)       60 2023-05-18 23:40:22.000000 ersciyt-1.86/ersciyt/tests.py
+-rw-r--r--   0 root         (0) root         (0)      491 2023-05-18 23:40:22.000000 ersciyt-1.86/ersciyt/urls.py
+-rw-r--r--   0 root         (0) root         (0)     8171 2023-05-18 23:40:22.000000 ersciyt-1.86/ersciyt/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:40:30.833965 ersciyt-1.86/ersciyt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      778 2023-05-18 23:40:30.000000 ersciyt-1.86/ersciyt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      392 2023-05-18 23:40:30.000000 ersciyt-1.86/ersciyt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 23:40:30.000000 ersciyt-1.86/ersciyt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-18 23:40:30.000000 ersciyt-1.86/ersciyt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-18 23:40:30.000000 ersciyt-1.86/ersciyt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      665 2023-05-18 23:40:30.835965 ersciyt-1.86/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-18 23:40:22.000000 ersciyt-1.86/setup.py
```

### Comparing `ersciyt-1.85/LICENSE` & `ersciyt-1.86/LICENSE`

 * *Files identical despite different names*

### Comparing `ersciyt-1.85/PKG-INFO` & `ersciyt-1.86/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.85
+Version: 1.86
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ersciyt-1.85/README.md` & `ersciyt-1.86/README.md`

 * *Files identical despite different names*

### Comparing `ersciyt-1.85/ersciyt/static/ersci_viddown_tab2.xpi` & `ersciyt-1.86/ersciyt/static/ersci_viddown_tab2.xpi`

 * *Files identical despite different names*

### Comparing `ersciyt-1.85/ersciyt/views.py` & `ersciyt-1.86/ersciyt/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,18 +146,18 @@
         return response
     except:
         return HttpResponse (video.description)
 '''
 def ytmp4(request,link):
     try:        
         #os.system('sudo apt-get install -y ffmpeg') 
-        if os.path.isfile("~/a.mp4"):
-            os.remove("~/a.mp4")
-        os.system('yt-dlp  -f 18 -o ~/a.mp4 https://www.youtube.com/watch?v={}'.format(link)) 
-        urllink = settings.ERSCIYT_LINK if hasattr(settings, 'ERSCIYT_LINK') and settings.ERSCIYT_LINK else "https://80-cs-751095881778-default.cs-us-central1-pits.cloudshell.dev/"
+        if os.path.isfile("/tmp/a.mp4"):
+            os.remove("/tmp/a.mp4")
+        os.system('yt-dlp  -f 18 -o /tmp/a.mp4 https://www.youtube.com/watch?v={}'.format(link)) 
+        urllink = settings.ERSCIYT_LINK if hasattr(settings, 'ERSCIYT_LINK') and settings.ERSCIYT_LINK
         return redirect(urllink)
     except:
         return HttpResponse ('Youtube Url Is Mistake!')
 
 def shqr(request):
     try:
         pic=request.GET['idx']
@@ -169,15 +169,15 @@
         return HttpResponse (imgdata)
     except:
         return HttpResponse ('Youtube Url Is Mistake!!!!')
         
 def helping(request):
     try:
         os.system('sudo apt install -y nginx')
-        os.system('sudo sed -i "s/root \/var\/www\/html/root ~/" /etc/nginx/sites-enabled/default')
+        os.system('sudo sed -i "s/root \/var\/www\/html/root \/tmp/" /etc/nginx/sites-enabled/default')
         os.system('sudo sed -i "s/index index.html/index a.mp4 index.html/" /etc/nginx/sites-enabled/default')
         os.system('sudo service nginx restart')
         return HttpResponse ('''<!Doctype html><html><head></head><body>
         <p>Use address of youtube after watch like - for download video -  :<br>
         <b> YourSiteName/ytlink?url=<any video site link></b><br>
         or<br>
         enter Youtube ID after YourSiteName address - for play in firefox -  : <br>
```

### Comparing `ersciyt-1.85/ersciyt.egg-info/PKG-INFO` & `ersciyt-1.86/ersciyt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.85
+Version: 1.86
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ersciyt-1.85/setup.cfg` & `ersciyt-1.86/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ersciyt
-version = 1.85
+version = 1.86
 description = Youtube Downloader
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/epg900/yt.git
 author = epg
 author_email = epg900@gmail.com
 license = GNU GENERAL PUBLIC LICENSE
```

