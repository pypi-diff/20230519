# Comparing `tmp/ersciyt-1.84.tar.gz` & `tmp/ersciyt-1.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ersciyt-1.84.tar", last modified: Mon May  8 08:00:18 2023, max compression
+gzip compressed data, was "ersciyt-1.85.tar", last modified: Thu May 18 23:16:12 2023, max compression
```

## Comparing `ersciyt-1.84.tar` & `ersciyt-1.85.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:00:18.149937 ersciyt-1.84/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-05-08 08:00:08.000000 ersciyt-1.84/LICENSE
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-08 08:00:08.000000 ersciyt-1.84/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      796 2023-05-08 08:00:18.149937 ersciyt-1.84/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      517 2023-05-08 08:00:08.000000 ersciyt-1.84/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:00:18.147937 ersciyt-1.84/ersciyt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 08:00:08.000000 ersciyt-1.84/ersciyt/__init__.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-08 08:00:08.000000 ersciyt-1.84/ersciyt/admin.py
--rw-r--r--   0 root         (0) root         (0)      146 2023-05-08 08:00:08.000000 ersciyt-1.84/ersciyt/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:00:18.148937 ersciyt-1.84/ersciyt/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 08:00:08.000000 ersciyt-1.84/ersciyt/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2023-05-08 08:00:08.000000 ersciyt-1.84/ersciyt/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:00:18.149937 ersciyt-1.84/ersciyt/static/
--rw-r--r--   0 root         (0) root         (0)    11852 2023-05-08 08:00:08.000000 ersciyt-1.84/ersciyt/static/ersci_viddown_tab2.xpi
--rw-r--r--   0 root         (0) root         (0)       60 2023-05-08 08:00:08.000000 ersciyt-1.84/ersciyt/tests.py
--rw-r--r--   0 root         (0) root         (0)      448 2023-05-08 08:00:08.000000 ersciyt-1.84/ersciyt/urls.py
--rw-r--r--   0 root         (0) root         (0)     7340 2023-05-08 08:00:08.000000 ersciyt-1.84/ersciyt/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:00:18.148937 ersciyt-1.84/ersciyt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      796 2023-05-08 08:00:17.000000 ersciyt-1.84/ersciyt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      392 2023-05-08 08:00:17.000000 ersciyt-1.84/ersciyt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 08:00:17.000000 ersciyt-1.84/ersciyt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-08 08:00:17.000000 ersciyt-1.84/ersciyt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-08 08:00:17.000000 ersciyt-1.84/ersciyt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      665 2023-05-08 08:00:18.150937 ersciyt-1.84/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-08 08:00:08.000000 ersciyt-1.84/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:16:12.948716 ersciyt-1.85/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-05-18 23:16:05.000000 ersciyt-1.85/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       69 2023-05-18 23:16:05.000000 ersciyt-1.85/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      778 2023-05-18 23:16:12.948716 ersciyt-1.85/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      517 2023-05-18 23:16:05.000000 ersciyt-1.85/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:16:12.946715 ersciyt-1.85/ersciyt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 23:16:05.000000 ersciyt-1.85/ersciyt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-18 23:16:05.000000 ersciyt-1.85/ersciyt/admin.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-05-18 23:16:05.000000 ersciyt-1.85/ersciyt/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:16:12.948716 ersciyt-1.85/ersciyt/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 23:16:05.000000 ersciyt-1.85/ersciyt/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       57 2023-05-18 23:16:05.000000 ersciyt-1.85/ersciyt/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:16:12.948716 ersciyt-1.85/ersciyt/static/
+-rw-r--r--   0 root         (0) root         (0)    11852 2023-05-18 23:16:05.000000 ersciyt-1.85/ersciyt/static/ersci_viddown_tab2.xpi
+-rw-r--r--   0 root         (0) root         (0)       60 2023-05-18 23:16:05.000000 ersciyt-1.85/ersciyt/tests.py
+-rw-r--r--   0 root         (0) root         (0)      491 2023-05-18 23:16:05.000000 ersciyt-1.85/ersciyt/urls.py
+-rw-r--r--   0 root         (0) root         (0)     8236 2023-05-18 23:16:05.000000 ersciyt-1.85/ersciyt/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 23:16:12.947716 ersciyt-1.85/ersciyt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      778 2023-05-18 23:16:12.000000 ersciyt-1.85/ersciyt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      392 2023-05-18 23:16:12.000000 ersciyt-1.85/ersciyt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 23:16:12.000000 ersciyt-1.85/ersciyt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-18 23:16:12.000000 ersciyt-1.85/ersciyt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-18 23:16:12.000000 ersciyt-1.85/ersciyt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      665 2023-05-18 23:16:12.949716 ersciyt-1.85/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-18 23:16:05.000000 ersciyt-1.85/setup.py
```

### Comparing `ersciyt-1.84/LICENSE` & `ersciyt-1.85/LICENSE`

 * *Files identical despite different names*

### Comparing `ersciyt-1.84/PKG-INFO` & `ersciyt-1.85/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.84
+Version: 1.85
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Erscipcard
 =========
```

### Comparing `ersciyt-1.84/README.md` & `ersciyt-1.85/README.md`

 * *Files identical despite different names*

### Comparing `ersciyt-1.84/ersciyt/static/ersci_viddown_tab2.xpi` & `ersciyt-1.85/ersciyt/static/ersci_viddown_tab2.xpi`

 * *Files identical despite different names*

### Comparing `ersciyt-1.84/ersciyt/views.py` & `ersciyt-1.85/ersciyt/views.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from django.shortcuts import render
+from django.shortcuts import render,redirect
 from django.conf import settings
 #from pytube import YouTube
 import pyqrcode
 import os,subprocess
 from django.http import HttpResponse,FileResponse
 #from youtube_transcript_api import YouTubeTranscriptApi
 #from youtube_transcript_api.formatters import WebVTTFormatter
 #pip install googletrans==4.0.0-rc1
 #from googletrans import Translator
 import re,base64
 from django.contrib.staticfiles import finders
-
+from django.conf import settings
 
 def ytdwn(request,link):
     try:        
         #os.system('sudo apt-get install -y ffmpeg') 
         os.system('yt-dlp  -f 18 -o a.mp4 https://www.youtube.com/watch?v={}'.format(link))        
         tmp4=open('a.mp4' , 'rb')
         tmp5=tmp4.read()
@@ -143,39 +143,54 @@
         response['Content-Disposition'] = 'attachment; filename=%s' % fn
         os.remove(media_dir + '/' + file)
         os.remove(media_dir + '/m1.mp3')
         return response
     except:
         return HttpResponse (video.description)
 '''
+def ytmp4(request,link):
+    try:        
+        #os.system('sudo apt-get install -y ffmpeg') 
+        if os.path.isfile("~/a.mp4"):
+            os.remove("~/a.mp4")
+        os.system('yt-dlp  -f 18 -o ~/a.mp4 https://www.youtube.com/watch?v={}'.format(link)) 
+        urllink = settings.ERSCIYT_LINK if hasattr(settings, 'ERSCIYT_LINK') and settings.ERSCIYT_LINK else "https://80-cs-751095881778-default.cs-us-central1-pits.cloudshell.dev/"
+        return redirect(urllink)
+    except:
+        return HttpResponse ('Youtube Url Is Mistake!')
+
 def shqr(request):
     try:
         pic=request.GET['idx']
         qr_code = pyqrcode.create(pic)#request.headers['HTTP_REFERER'])
         qr_code.svg('a.svg', scale=6)
         img=open('a.svg', "r")
         #image_data = base64.b64encode(img.read()).decode('utf-8')
         imgdata = "{}".format(img.read())
         return HttpResponse (imgdata)
     except:
         return HttpResponse ('Youtube Url Is Mistake!!!!')
         
 def helping(request):
     try:
+        os.system('sudo apt install -y nginx')
+        os.system('sudo sed -i "s/root \/var\/www\/html/root ~/" /etc/nginx/sites-enabled/default')
+        os.system('sudo sed -i "s/index index.html/index a.mp4 index.html/" /etc/nginx/sites-enabled/default')
+        os.system('sudo service nginx restart')
         return HttpResponse ('''<!Doctype html><html><head></head><body>
         <p>Use address of youtube after watch like - for download video -  :<br>
         <b> YourSiteName/ytlink?url=<any video site link></b><br>
         or<br>
         enter Youtube ID after YourSiteName address - for play in firefox -  : <br>
         <b>YourSiteName/xazlZh1lTpM</b><br>        
         <a href="/static/ersci_viddown_tab2.xpi">Video download firefox Addon direct link</a><br>
         or<br>
         <a href="https://addons.mozilla.org/en-US/firefox/addon/ersci_viddown_tab2">video download firefox Addon mozilla site link</a>
         <br>
         <br>
-        <a href="" onclick="window.open('/shqr?idx=' + window.location.href);">show QR Code for this site </a>
+        <a href="#" onclick="window.open('/yt/shqr?idx=' + window.location.href);">show QR Code for this site </a>
         <br>
         </p>
         </body></html>
         ''')
     except:
         return HttpResponse ('Youtube Url Is Mistake!!!')
```

### Comparing `ersciyt-1.84/ersciyt.egg-info/PKG-INFO` & `ersciyt-1.85/ersciyt.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.84
+Version: 1.85
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Erscipcard
 =========
```

