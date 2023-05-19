# Comparing `tmp/FileInfo_Video_Audio-0.1.1.tar.gz` & `tmp/FileInfo_Video_Audio-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FileInfo_Video_Audio-0.1.1.tar", last modified: Wed May 17 14:16:55 2023, max compression
+gzip compressed data, was "FileInfo_Video_Audio-0.1.2.tar", last modified: Fri May 19 13:46:31 2023, max compression
```

## Comparing `FileInfo_Video_Audio-0.1.1.tar` & `FileInfo_Video_Audio-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-17 14:16:55.188400 FileInfo_Video_Audio-0.1.1/
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-17 14:16:55.188400 FileInfo_Video_Audio-0.1.1/FileInfo_Video_Audio.egg-info/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1498 2023-05-17 14:16:55.000000 FileInfo_Video_Audio-0.1.1/FileInfo_Video_Audio.egg-info/PKG-INFO
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      321 2023-05-17 14:16:55.000000 FileInfo_Video_Audio-0.1.1/FileInfo_Video_Audio.egg-info/SOURCES.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-05-17 14:16:55.000000 FileInfo_Video_Audio-0.1.1/FileInfo_Video_Audio.egg-info/dependency_links.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       62 2023-05-17 14:16:55.000000 FileInfo_Video_Audio-0.1.1/FileInfo_Video_Audio.egg-info/entry_points.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        7 2023-05-17 14:16:55.000000 FileInfo_Video_Audio-0.1.1/FileInfo_Video_Audio.egg-info/top_level.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1498 2023-05-17 14:16:55.188400 FileInfo_Video_Audio-0.1.1/PKG-INFO
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1127 2023-05-17 10:56:40.000000 FileInfo_Video_Audio-0.1.1/README.md
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-05-17 14:16:55.188400 FileInfo_Video_Audio-0.1.1/setup.cfg
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      816 2023-05-17 14:16:31.000000 FileInfo_Video_Audio-0.1.1/setup.py
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-17 14:16:55.188400 FileInfo_Video_Audio-0.1.1/source/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-14 18:26:11.000000 FileInfo_Video_Audio-0.1.1/source/__init__.py
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-17 14:16:55.188400 FileInfo_Video_Audio-0.1.1/source/lib/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1272 2023-05-14 14:25:10.000000 FileInfo_Video_Audio-0.1.1/source/lib/Argument.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       36 2023-05-14 14:25:10.000000 FileInfo_Video_Audio-0.1.1/source/lib/__init__.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     3875 2023-05-17 13:59:03.000000 FileInfo_Video_Audio-0.1.1/source/main.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-19 13:46:31.304569 FileInfo_Video_Audio-0.1.2/
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-19 13:46:31.300569 FileInfo_Video_Audio-0.1.2/FileInfo_Video_Audio.egg-info/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1496 2023-05-19 13:46:31.000000 FileInfo_Video_Audio-0.1.2/FileInfo_Video_Audio.egg-info/PKG-INFO
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      321 2023-05-19 13:46:31.000000 FileInfo_Video_Audio-0.1.2/FileInfo_Video_Audio.egg-info/SOURCES.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-05-19 13:46:31.000000 FileInfo_Video_Audio-0.1.2/FileInfo_Video_Audio.egg-info/dependency_links.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       62 2023-05-19 13:46:31.000000 FileInfo_Video_Audio-0.1.2/FileInfo_Video_Audio.egg-info/entry_points.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        7 2023-05-19 13:46:31.000000 FileInfo_Video_Audio-0.1.2/FileInfo_Video_Audio.egg-info/top_level.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1496 2023-05-19 13:46:31.300569 FileInfo_Video_Audio-0.1.2/PKG-INFO
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1125 2023-05-19 13:36:10.000000 FileInfo_Video_Audio-0.1.2/README.md
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-05-19 13:46:31.304569 FileInfo_Video_Audio-0.1.2/setup.cfg
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      815 2023-05-19 13:46:10.000000 FileInfo_Video_Audio-0.1.2/setup.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-19 13:46:31.300569 FileInfo_Video_Audio-0.1.2/source/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-19 13:31:53.000000 FileInfo_Video_Audio-0.1.2/source/__init__.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-19 13:46:31.300569 FileInfo_Video_Audio-0.1.2/source/lib/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1272 2023-05-19 13:31:53.000000 FileInfo_Video_Audio-0.1.2/source/lib/Argument.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       36 2023-05-19 13:31:53.000000 FileInfo_Video_Audio-0.1.2/source/lib/__init__.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     3875 2023-05-19 13:31:53.000000 FileInfo_Video_Audio-0.1.2/source/main.py
```

### Comparing `FileInfo_Video_Audio-0.1.1/FileInfo_Video_Audio.egg-info/PKG-INFO` & `FileInfo_Video_Audio-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: FileInfo-Video-Audio
-Version: 0.1.1
+Name: FileInfo_Video_Audio
+Version: 0.1.2
 Summary: In this tool is help to get the properties of the Audio and Video files
 Home-page: https://git.selfmade.ninja/SRIDHARDSCV/collage_sem_4_python_project_cli_file_details
 Author: Sridhar
 Author-email: dcsvsridhar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -29,19 +29,19 @@
 
 #### Usage
 ##### To get the Information about the Video file
 
 To get all available info about a particular track of the  video file. It works with all media types.
 
 ```
-GetFileinfo_Audio_Video --file="some_video.mp4" --type={General/Audio/Video} --list_All_keys 
+GetFileinfo_Audio_Video -file="some_video.mp4" --type={General/Audio/Video} --list_All_keys 
 
 (or)
 
-GetFileinfo_Audio_Video --file="some_video.mp4" --type={General/Audio/Video} -l
+GetFileinfo_Audio_Video -file="some_video.mp4" --type={General/Audio/Video} -l
 
 ```
 
 To get all available  tracks of the  video file.
 
 ```
 GetFileinfo_Audio_Video -file=test.mp4 --type -h
```

### Comparing `FileInfo_Video_Audio-0.1.1/PKG-INFO` & `FileInfo_Video_Audio-0.1.2/FileInfo_Video_Audio.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: FileInfo_Video_Audio
-Version: 0.1.1
+Name: FileInfo-Video-Audio
+Version: 0.1.2
 Summary: In this tool is help to get the properties of the Audio and Video files
 Home-page: https://git.selfmade.ninja/SRIDHARDSCV/collage_sem_4_python_project_cli_file_details
 Author: Sridhar
 Author-email: dcsvsridhar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -29,19 +29,19 @@
 
 #### Usage
 ##### To get the Information about the Video file
 
 To get all available info about a particular track of the  video file. It works with all media types.
 
 ```
-GetFileinfo_Audio_Video --file="some_video.mp4" --type={General/Audio/Video} --list_All_keys 
+GetFileinfo_Audio_Video -file="some_video.mp4" --type={General/Audio/Video} --list_All_keys 
 
 (or)
 
-GetFileinfo_Audio_Video --file="some_video.mp4" --type={General/Audio/Video} -l
+GetFileinfo_Audio_Video -file="some_video.mp4" --type={General/Audio/Video} -l
 
 ```
 
 To get all available  tracks of the  video file.
 
 ```
 GetFileinfo_Audio_Video -file=test.mp4 --type -h
```

### Comparing `FileInfo_Video_Audio-0.1.1/README.md` & `FileInfo_Video_Audio-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 
 #### Usage
 ##### To get the Information about the Video file
 
 To get all available info about a particular track of the  video file. It works with all media types.
 
 ```
-GetFileinfo_Audio_Video --file="some_video.mp4" --type={General/Audio/Video} --list_All_keys 
+GetFileinfo_Audio_Video -file="some_video.mp4" --type={General/Audio/Video} --list_All_keys 
 
 (or)
 
-GetFileinfo_Audio_Video --file="some_video.mp4" --type={General/Audio/Video} -l
+GetFileinfo_Audio_Video -file="some_video.mp4" --type={General/Audio/Video} -l
 
 ```
 
 To get all available  tracks of the  video file.
 
 ```
 GetFileinfo_Audio_Video -file=test.mp4 --type -h
```

### Comparing `FileInfo_Video_Audio-0.1.1/setup.py` & `FileInfo_Video_Audio-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 requirements = os.popen("/usr/local/bin/pipreqs main --print").read().splitlines()
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='FileInfo_Video_Audio',
-    version='0.1.1',
+    version='0.1.2',
     author='Sridhar',
     author_email='dcsvsridhar@gmail.com',
     description="In this tool is help to get the properties of the Audio and Video files",
     packages=find_packages(),
     url='https://git.selfmade.ninja/SRIDHARDSCV/collage_sem_4_python_project_cli_file_details',
     install_requires=requirements,
     long_description=long_description,
     long_description_content_type='text/markdown',
     entry_points={
         'console_scripts': [
             'GetFileinfo_Audio_Video=source.main:main',
         ],
     },
-)
+)
```

### Comparing `FileInfo_Video_Audio-0.1.1/source/lib/Argument.py` & `FileInfo_Video_Audio-0.1.2/source/lib/Argument.py`

 * *Files identical despite different names*

### Comparing `FileInfo_Video_Audio-0.1.1/source/main.py` & `FileInfo_Video_Audio-0.1.2/source/main.py`

 * *Files identical despite different names*

