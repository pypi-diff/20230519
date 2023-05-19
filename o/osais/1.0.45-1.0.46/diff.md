# Comparing `tmp/osais-1.0.45.tar.gz` & `tmp/osais-1.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-03tn37f_\osais-1.0.45.tar", last modified: Thu May 18 17:02:33 2023, max compression
+gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-hsdvnndl\osais-1.0.46.tar", last modified: Fri May 19 11:37:26 2023, max compression
```

## Comparing `osais-1.0.45.tar` & `osais-1.0.46.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 17:02:33.442157 osais-1.0.45/
--rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.45/LICENSE
--rw-rw-rw-   0        0        0     1172 2023-05-18 17:02:33.441158 osais-1.0.45/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-05-12 12:25:24.000000 osais-1.0.45/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 17:02:33.436149 osais-1.0.45/osais/
--rw-rw-rw-   0        0        0     1006 2023-05-18 17:00:02.000000 osais-1.0.45/osais/__init__.py
--rw-rw-rw-   0        0        0    54406 2023-05-18 16:59:27.000000 osais-1.0.45/osais/osais.py
-drwxrwxrwx   0        0        0        0 2023-05-18 17:02:33.440157 osais-1.0.45/osais.egg-info/
--rw-rw-rw-   0        0        0     1172 2023-05-18 17:02:33.000000 osais-1.0.45/osais.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-05-18 17:02:33.000000 osais-1.0.45/osais.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 17:02:33.000000 osais-1.0.45/osais.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-05-18 17:02:33.000000 osais-1.0.45/osais.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-18 17:02:33.000000 osais-1.0.45/osais.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.45/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-18 17:02:33.442157 osais-1.0.45/setup.cfg
--rw-rw-rw-   0        0        0     1180 2023-05-18 17:00:20.000000 osais-1.0.45/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 11:37:26.466733 osais-1.0.46/
+-rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.46/LICENSE
+-rw-rw-rw-   0        0        0     1172 2023-05-19 11:37:26.466733 osais-1.0.46/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-05-12 12:25:24.000000 osais-1.0.46/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 11:37:26.461733 osais-1.0.46/osais/
+-rw-rw-rw-   0        0        0     1041 2023-05-19 11:36:31.000000 osais-1.0.46/osais/__init__.py
+-rw-rw-rw-   0        0        0    54875 2023-05-19 11:36:03.000000 osais-1.0.46/osais/osais.py
+drwxrwxrwx   0        0        0        0 2023-05-19 11:37:26.465737 osais-1.0.46/osais.egg-info/
+-rw-rw-rw-   0        0        0     1172 2023-05-19 11:37:26.000000 osais-1.0.46/osais.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-05-19 11:37:26.000000 osais-1.0.46/osais.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 11:37:26.000000 osais-1.0.46/osais.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-05-19 11:37:26.000000 osais-1.0.46/osais.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-19 11:37:26.000000 osais-1.0.46/osais.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.46/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 11:37:26.466733 osais-1.0.46/setup.cfg
+-rw-rw-rw-   0        0        0     1180 2023-05-19 11:36:43.000000 osais-1.0.46/setup.py
```

### Comparing `osais-1.0.45/LICENSE` & `osais-1.0.46/LICENSE`

 * *Files identical despite different names*

### Comparing `osais-1.0.45/PKG-INFO` & `osais-1.0.46/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.45
+Version: 1.0.46
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.45/osais/__init__.py` & `osais-1.0.46/osais/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 A package for OSAIS virtual AI.
 """
-__version__="1.0.45"
+__version__="1.0.46"
 __author__ = "incubiq"
 __email__ = "eric@incubiq.com"
 
 from .osais import osais_isDebug
 from .osais import osais_isDocker
 from .osais import osais_isLocal
 from .osais import osais_isVirtualAI
@@ -19,12 +19,13 @@
 from .osais import osais_getInfo
 from .osais import osais_getClientID
 from .osais import osais_resetGateway
 from .osais import osais_authenticateAI
 from .osais import osais_authenticateClient
 from .osais import osais_postRequest
 from .osais import osais_initParser
+from .osais import osais_warmupAI
 from .osais import osais_runAI
 from .osais import osais_notify
 from .osais import osais_onNotifyFileCreated
 from .osais import osais_resetOSAIS
 from .osais import osais_initializeAI
```

### Comparing `osais-1.0.45/osais/osais.py` & `osais-1.0.46/osais/osais.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-__version__="1.0.45"
+__version__="1.0.46"
 
 ## ========================================================================
 ## 
 ##                      Utilities starts here 
 ## 
 ## ========================================================================
 
@@ -15,14 +15,15 @@
 import subprocess as sp
 import pkg_resources
 import os
 import platform
 import ctypes
 import threading
 import boto3
+import asyncio
 
 cuda=0                          ## from cuda import cuda, nvrtc
 gObserver=None
 
 ## ------------------------------------------------------------------------
 #       Observer (check updates in directory)
 ## ------------------------------------------------------------------------
@@ -66,14 +67,17 @@
 def start_notification_thread(fnOnNotify):
     def _run(_fn):
         _fn()
     thread = threading.Thread(target=_run, args=(fnOnNotify))
     thread.start()
     return _run
 
+async def wait_250ms():
+  await asyncio.sleep(0.250)
+
 ## ------------------------------------------------------------------------
 #       Directory utils
 ## ------------------------------------------------------------------------
 
 ## list content of a directory
 def listDirContent(_dir):
     from os.path import isfile, join
@@ -351,25 +355,30 @@
     response = urllib.request.urlopen(url)
     image_data = response.read()
     with open(local_file_path, 'wb') as f:
         f.write(image_data)
 
     return f"{local_filename}{file_extension}"
 
-def osais_uploadFileToS3(_filename, _dirS3): 
+## upload image to S3 and tag it
+def osais_uploadFileToS3(_filename, _dirS3, objTag): 
     global gS3
     global gS3Bucket
     root=getS3BucketRoot()
     if gS3!=None:
         try:
+            from urllib import parse    
             # Filename - File to upload
             # Bucket - Bucket to upload to (the top level directory under AWS S3)
             # Key - S3 object name (can contain subdirectories). If not specified then file_name is used
             _baseName=os.path.basename(_filename)
-            gS3.meta.client.upload_file(Filename=_filename, Bucket=gS3Bucket, Key=_dirS3+_baseName)
+            gS3.meta.client.upload_file(Filename=_filename, Bucket=gS3Bucket, Key=_dirS3+_baseName, ExtraArgs={
+                'ACL':'public-read', 
+                "Tagging": parse.urlencode(objTag)
+            })
             print("=> Uploaded "+_filename+" to S3")
             return root+_dirS3+_baseName
             
         except Exception as err:
             consoleLog({"msg":"Could not upload file to S3"})
             raise err
         
@@ -466,15 +475,14 @@
 gPortLocalOSAIS=3022            ## port where a local OSAIS can be accessed
 
 ## temp cache
 gAProcessed=[]                  ## all token being sent to processing (never call twice for same)
 gIsScheduled=False              ## do we have a scheduled event running?
 
 ## run times
-gIsWarmup=False                 ## True if the request was a warmup one (not a true one from client)
 gIsBusy=False                   ## True if AI busy processing
 gDefaultCost=1000               ## default cost value in ms (will get overriden fast, this value is no big deal)
 gaProcessTime=[]                ## Array of last x (10/20?) time spent for processed requests 
 
 ## processing specifics
 gArgsOSAIS=None                 ## the args passed to the AI which are specific to OSAIS for sending notifications
 
@@ -701,19 +709,17 @@
     global gDefaultCost
     global gaProcessTime
     from array import array
     gaProcessTime=array('f', [gDefaultCost,gDefaultCost,gDefaultCost,gDefaultCost,gDefaultCost,gDefaultCost,gDefaultCost,gDefaultCost,gDefaultCost,gDefaultCost])
 
 # init the dafault cost array
 def _addCost(_cost) :
-    global gIsWarmup
     global gaProcessTime
-    if gIsWarmup==False:
-        gaProcessTime.insert(0, _cost)
-        gaProcessTime.pop()
+    gaProcessTime.insert(0, _cost)
+    gaProcessTime.pop()
 
 # init the dafault cost array
 def _getAverageCost() :
     global gaProcessTime
     average = sum(gaProcessTime) / len(gaProcessTime)
     return average
 
@@ -1041,40 +1047,37 @@
 ## ------------------------------------------------------------------------
 
 ## PUBLIC - parse args for OSAIS (not those for AI)
 def osais_initParser(aArg):
     global gArgsOSAIS
     global gInputDir
     global gOutputDir
-    global gIsWarmup
 
     # Create the parser
     vq_parser = argparse.ArgumentParser(description='Arg parser init by OSAIS')
 
     # Add the AI Gateway / OpenSourceAIs arguments
     vq_parser.add_argument("-orig",  "--origin", type=str, help="Caller's origin", default=None , dest='OSAIS_origin')      ##  this is for comms with AI Gateway
     vq_parser.add_argument("-t",  "--token", type=str, help="OpenSourceAIs token", default="0", dest='tokenAI')             ##  this is for comms with OpenSourceAIs
     vq_parser.add_argument("-u",  "--username", type=str, help="OpenSourceAIs username", default="", dest='username')       ##  this is for comms with OpenSourceAIs
     vq_parser.add_argument("-uid",  "--unique_id", type=int, help="Unique ID of this AI session", default=0, dest='uid')    ##  this is for comms with OpenSourceAIs
     vq_parser.add_argument("-odir", "--outdir", type=str, help="Output directory", default=gOutputDir, dest='outdir')
     vq_parser.add_argument("-idir", "--indir", type=str, help="input directory", default=gInputDir, dest='indir')
     vq_parser.add_argument("-cycle", "--cycle", type=int, help="cycle", default=0, dest='cycle')
     vq_parser.add_argument("-filename", "--filename", type=str, help="filename", default="default", dest='filename')
-    vq_parser.add_argument("-warmup", "--warmup", type=bool, help="warmup", default=False, dest='warmup')
 
     gArgsOSAIS = vq_parser.parse_args(aArg)
-    gIsWarmup=(gArgsOSAIS.warmup==True or gArgsOSAIS.warmup=="True")
     if gArgsOSAIS.OSAIS_origin!=None:
         print("=> origin set to "+gArgsOSAIS.OSAIS_origin)
     else:
         print("=> origin set to None")
     return True
-
-## PUBLIC - run the AI (at least try)
-def osais_runAI(*args):
+    
+## run the AI (at least try)
+def _runAI(isWarmup, *args, ):
     global gIsBusy
     global gAProcessed
     global gName 
     global gLastProcessStart_at
     global gOriginOSAIS
     global gIsLocal
 
@@ -1108,16 +1111,21 @@
             except Exception as err:
                 raise err
         else:
             if not _args["-warmup"]:
                 raise ValueError("CRITICAL: require a upload url in S3 ")
                 
     except Exception as err:
-        consoleLog({"msg":"did not get a -filename or could not process"})
-        raise err
+        print("=> did not get a -filename, we continue")
+        _args["-idir"]=gInputDir
+        _args["-odir"]=gOutputDir
+
+    if isWarmup:
+        _args["-idir"]="./static/"
+        print("=> Warming up...")
 
     ## start time
     gIsBusy=True
     beg_date = datetime.utcnow()
     
     ## reprocess AI args
     aArgForparserAI=_getArgs(_args)
@@ -1136,19 +1144,19 @@
     _localT=gArgsOSAIS.tokenAI
     _localU=gArgsOSAIS.username
     _localUID=gArgsOSAIS.uid
     _localODir=gArgsOSAIS.outdir
     _localIDir=gArgsOSAIS.indir
     _localCycle=gArgsOSAIS.cycle
     _localFilename=gArgsOSAIS.filename
-
     _isGateway=None
-    if gIsWarmup:
-        print("=> Warming up...")
-    else:
+
+    if isWarmup:
+        _localOrig=None
+    else :
         ## req received from a gateway ot OSAIS?
         _isGateway = not (_localOrig == "https://opensourceais.com/" or _localOrig == "https://opensourceais.com" or _localOrig[:5]== "http:")
         print("=> before run: processed args from url: "+str(aArgForparserAI)+"\r\n")
 
     ## notify OSAIS (Req received)
     CredsParam=getCredsParams(_localT, _localU, _isGateway)
     MorphingParam=getMorphingParams(_localUID, _localCycle, _localFilename)
@@ -1187,30 +1195,39 @@
         raise err
 
     ## calculate cost
     gIsBusy=False
     end_date = datetime.utcnow()
     delta=end_date - beg_date
     cost = int(delta.total_seconds()* 1000 + delta.microseconds / 1000)
-    _addCost(cost)
-
-    ## notify end
-    StageParam=getStageParams(AI_PROGRESS_AI_STOPPED, cost)
-    osais_notify(_localOrig, CredsParam, MorphingParam , StageParam)
 
-    if gIsWarmup:
+    if isWarmup:
         _strDelta=str(delta)
         print("\r\n=> AI ready!")
         print("=> Able to process requests in "+_strDelta+" secs\r\n")
+    else:
+        _addCost(cost)
+
+    ## notify end
+    StageParam=getStageParams(AI_PROGRESS_AI_STOPPED, cost)
+    osais_notify(_localOrig, CredsParam, MorphingParam , StageParam)
 
     ## default OK response if the AI does not send any
     if response==None:
         response=True
     return response
 
+### PUBLIC - warmup the AI (at least try)
+def osais_warmupAI(*args):
+    return _runAI(True, *args)
+
+## PUBLIC - run the AI (at least try)
+def osais_runAI(*args):
+    return _runAI(False, *args)
+
 ## ------------------------------------------------------------------------
 #       get formatted params from AI current state
 ## ------------------------------------------------------------------------
 
 def getCredsParams(_token, _username, _isGateway) :
     global gName
     global gArgsOSAIS
@@ -1285,24 +1302,29 @@
 
     api_url=f"{_origin}api/v1/public/upload"        
     payload = json.dumps(objParam)
     response = requests.post(api_url, headers=headers, data=payload )
     objRes=response.json()
     return objRes    
 
-## got notified of file creation (by watch)
-def osais_onNotifyFileCreated(_dir, _filename, _args):
-    ## where is the caller?
+async def _delayed_onNotifyFileCreated(_dir, _filename, _args):
+    ## a small wait
+    await wait_250ms()
+
     _isGateway=None
     _origin=_args.get('-orig')
     if _origin!=None:
         _isGateway = not (_origin == "https://opensourceais.com/" or _origin == "https://opensourceais.com" or _origin[:5]== "http:")
 
-    ## also send to S3
-    _fileS3=osais_uploadFileToS3(_dir+_filename, getS3BucketOutputDir())
+    ## upload image to S3
+    objTag={
+        "uid": _args["-uid"],
+        "username": _args["-u"]
+    }
+    _fileS3=osais_uploadFileToS3(_dir+_filename, getS3BucketOutputDir(), objTag)
 
     # notify
     _cycle=0
     try: 
         if _args["-cycle"]:
             _cycle=_args["-cycle"]
     except:
@@ -1310,14 +1332,18 @@
 
     _stageParam=getStageParams(AI_PROGRESS_DONE_IMAGE, 0)
     _morphingParam=getMorphingParams(_args["-uid"], _cycle, _fileS3)
     _credsParam=getCredsParams(_args["-t"], _args["-u"], _isGateway)
     osais_notify(_origin, _credsParam, _morphingParam, _stageParam)            # OSAIS Notification
     return True
 
+## got notified of file creation (by watch)
+def osais_onNotifyFileCreated(_dir, _filename, _args):
+    asyncio.run(_delayed_onNotifyFileCreated(_dir, _filename, _args))
+
 def _notifyGateway(_origin, objParam):
     headers = {
         "Content-Type": "application/json"
     }
     api_url=f"{_origin}api/v1/public/notify"
     try: 
         response = requests.post(api_url, headers=headers, data=json.dumps(objParam))
@@ -1344,18 +1370,17 @@
 def osais_notify(_origin, CredParam, MorphingParam, StageParam):
     global gIPLocal
     global gPortGateway
     global gIsVirtualAI
     global gIsLocal
     global gVAIAuthToken
     global gLastChecked_at
-    global gIsWarmup
 
     ## no notification of warmup or unknown caller
-    if gIsWarmup or _origin==None:
+    if _origin==None:
         return None
     
     gLastChecked_at = datetime.utcnow()
 
     # notification console log
     merged = dict()
     merged.update(CredParam)
```

### Comparing `osais-1.0.45/osais.egg-info/PKG-INFO` & `osais-1.0.46/osais.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.45
+Version: 1.0.46
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.45/setup.py` & `osais-1.0.46/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='osais',
-    version='1.0.45',
+    version='1.0.46',
     author='incubiq',
     author_email='eric@incubiq.com',
     description='The osais Python lib for connecting AIs to OSAIS cloud',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/incubiq/osais',
     keywords = "osais, opensourceais",
```

