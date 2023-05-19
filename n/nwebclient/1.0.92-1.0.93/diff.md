# Comparing `tmp/nwebclient-1.0.92.tar.gz` & `tmp/nwebclient-1.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nwebclient-1.0.92.tar", last modified: Wed May 10 08:35:48 2023, max compression
+gzip compressed data, was "dist/nwebclient-1.0.93.tar", last modified: Fri May 19 11:09:39 2023, max compression
```

## Comparing `nwebclient-1.0.92.tar` & `nwebclient-1.0.93.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-10 08:35:48.409059 nwebclient-1.0.92/
--rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.92/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-10 08:35:48.409059 nwebclient-1.0.92/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.92/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-10 08:35:48.409059 nwebclient-1.0.92/nwebclient/
--rw-r--r--   0 pi        (1000) pi        (1000)     6457 2023-05-09 14:11:24.000000 nwebclient-1.0.92/nwebclient/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.92/nwebclient/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3316 2023-05-09 12:58:28.000000 nwebclient-1.0.92/nwebclient/crypt.py
--rw-r--r--   0 pi        (1000) pi        (1000)    13279 2023-05-10 08:35:36.000000 nwebclient-1.0.92/nwebclient/sd.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6100 2023-05-05 17:05:53.000000 nwebclient-1.0.92/nwebclient/sdb.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.92/nwebclient/ticker.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-10 08:35:48.409059 nwebclient-1.0.92/nwebclient.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-10 08:35:48.000000 nwebclient-1.0.92/nwebclient.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-05-10 08:35:48.000000 nwebclient-1.0.92/nwebclient.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-10 08:35:48.000000 nwebclient-1.0.92/nwebclient.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-10 08:35:48.000000 nwebclient-1.0.92/nwebclient.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-10 08:35:48.000000 nwebclient-1.0.92/nwebclient.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-10 08:35:48.000000 nwebclient-1.0.92/nwebclient.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-10 08:35:48.409059 nwebclient-1.0.92/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-10 08:35:46.000000 nwebclient-1.0.92/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-19 11:09:39.206337 nwebclient-1.0.93/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.93/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-19 11:09:39.206337 nwebclient-1.0.93/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.93/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-19 11:09:39.196337 nwebclient-1.0.93/nwebclient/
+-rw-r--r--   0 pi        (1000) pi        (1000)     6483 2023-05-12 07:26:49.000000 nwebclient-1.0.93/nwebclient/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.93/nwebclient/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3316 2023-05-09 12:58:28.000000 nwebclient-1.0.93/nwebclient/crypt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3545 2023-05-14 17:14:29.000000 nwebclient-1.0.93/nwebclient/nlp.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    14410 2023-05-19 07:18:25.000000 nwebclient-1.0.93/nwebclient/sd.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     6100 2023-05-05 17:05:53.000000 nwebclient-1.0.93/nwebclient/sdb.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.93/nwebclient/ticker.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-19 11:09:39.206337 nwebclient-1.0.93/nwebclient.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-19 11:09:39.000000 nwebclient-1.0.93/nwebclient.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      382 2023-05-19 11:09:39.000000 nwebclient-1.0.93/nwebclient.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-19 11:09:39.000000 nwebclient-1.0.93/nwebclient.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-19 11:09:39.000000 nwebclient-1.0.93/nwebclient.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-19 11:09:39.000000 nwebclient-1.0.93/nwebclient.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-19 11:09:39.000000 nwebclient-1.0.93/nwebclient.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-19 11:09:39.206337 nwebclient-1.0.93/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-19 11:09:34.000000 nwebclient-1.0.93/setup.py
```

### Comparing `nwebclient-1.0.92/LICENSE` & `nwebclient-1.0.93/LICENSE`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.92/PKG-INFO` & `nwebclient-1.0.93/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.92
+Version: 1.0.93
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.92/README.md` & `nwebclient-1.0.93/README.md`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.92/nwebclient/__init__.py` & `nwebclient-1.0.93/nwebclient/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,18 +163,18 @@
     def createFileDoc(self, name, group_id, data):
         """  open('file', 'rb') """
         self.upload("w/group/"+str(group_id)+"/create", {
             "title": name,
             "kind": 'binary'
         }, 'file', data)
     def deleteDoc(self, id):
-        self.req('w/d/'+str(id)+'/delete', {'confirm': 1})
-    def downloadImages(self):
+        return self.req('w/d/'+str(id)+'/delete', {'confirm': 1})
+    def downloadImages(self, limit=1000):
         # https://bsnx.net/4.0/w/api/docs?tag=Untertage
-        docs = self.docs('kind=image&limit=1000')
+        docs = self.docs('kind=image&limit='+str(limit))
         for doc in docs:
            self.reqToFile('image/'+str(doc.id())+'/orginal/web/'+str(doc.id())+'.jpg', str(doc.id())+ '.jpg')
            print("Download Image: " + str(doc.id()))
 
 def metric_val(baseUrl, metricName, val):
     """ baseUrl: string = e.g. https://bsnx.net/metric-endpoint """
     requests.get(url=baseUrl, params= {'metric':metricName, 'val':val})
```

### Comparing `nwebclient-1.0.92/nwebclient/__main__.py` & `nwebclient-1.0.93/nwebclient/__main__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.92/nwebclient/crypt.py` & `nwebclient-1.0.93/nwebclient/crypt.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.92/nwebclient/sd.py` & `nwebclient-1.0.93/nwebclient/sd.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from nwebclient import sdb
 from nwebclient import ticker
 import json
 import os
 import os.path
 import requests
 import time
+import base64
 
 # Stable Diffusion Imports in ImageGen::__init__
 
 def gen(pipe, prompt='photo', negative_prompt = None, prefix='sd',  guidance_scale = 7.5, num_inference_steps=30, height=800, width=640, num_images=1, dbfile='data.db'):
-    # https://huggingface.co/docs/diffusers/v0.14.0/en/api/pipelines/stable_diffusion/text2img#diffusers.StableDiffusionPipeline.__call__
-    images = pipe(
+    # https://huggingface.co/docs/diffusers/v0.14.0/en/
       prompt,
       height = 800,
       width = 640,
       num_inference_steps = num_inference_steps,      # higher better quali default=45
       guidance_scale = guidance_scale,                # Prioritize creativity  7.5  Prioritize prompt (higher)
       num_images_per_prompt = num_images,
       negative_prompt = negative_prompt,
@@ -48,14 +48,15 @@
     # sdb jpg
     save_mode='sdb'
     loaded_model = None
     gen_count = 0
     api = None
     cn_image = None
     diff_cn = None
+    loop_count = 25
     def __init__(self, model_id="XpucT/Deliberate"):
         self.model_id = model_id
     def load(self):
         if self.loaded_model == self.model_id or self.generator == 'automatic1111':
             return
         self.info("Loading Stable Diffusion Dependencies...");
         from diffusers import PNDMScheduler, DDIMScheduler, LMSDiscreteScheduler, EulerDiscreteScheduler, DPMSolverMultistepScheduler
@@ -97,29 +98,31 @@
             self.genA1111(loop_number)
         elif self.generator == 'diffcn':
             self.genDiffCn(loop_number)
         elif self.generator == 'dummy':
             time.sleep(1)
             print("Dummy Generation; " + str(loop_number))
             self.gen_count = self.gen_count + 1
+        if self.gen_count%100 == 0:
+            self.info("gen_count: " + str(self.gen_count))
     def genDiffCn(self, loop_number=1):
         self.initDiffCn()
         output= self.diff_cn(self.prompt, self.cn_image, negative_prompt=self.negative_prompt, num_inference_steps=25, num_images_per_prompt = 1, height = self.height, width = self.width)
         self.save_image(output[0][0], 0,loop_number)
         self.gen_count = self.gen_count + 1
     def genCnPose1111(self, loop_number=1):
         self.initA1111();
         result = self.api.txt2img(prompt=self.prompt,negative_prompt=self.negative_prompt, height=self.height, width=self.width, controlnet_units=[self.cn_image],cfg_scale=7)
         self.save_image(result.image, 0,loop_number)
         self.gen_count = self.gen_count + 1
     def genA1111(self, loop_number=1):  
         self.initA1111();
         if self.model_id.endswith('.safetensors') and self.model_id != self.loaded_model:
              self.a1111setModel(self.model_id)
-        result = self.api.txt2img(prompt=self.prompt,negative_prompt=self.negative_prompt, height=self.height, width=self.width, cfg_scale=7)
+        result = self.api.txt2img(prompt=self.prompt,negative_prompt=self.negative_prompt, height=self.height, width=self.width, cfg_scale=self.guidance_scale)
         self.save_image(result.image, 0,loop_number)
         self.gen_count = self.gen_count + 1
     def genDiffusers(self, loop_number=1):
         if self.pipe is None:
             self.load()
         images = self.pipe(self.prompt,
             height = self.height,
@@ -135,14 +138,15 @@
             self.save_image(images[i], i, loop_number)
     def save_image(self, image, i, loop_number):
         if self.save_mode == 'sdb':
             sdb.sdb_write_pil(image, self.prompt, self.negative_prompt, self.guidance_scale, self.prefix, self.dbfile)
         if self.save_mode == 'jpg':
             image.save(self.prefix+'_'+str(loop_number)+'_'+str(i)+'.jpg')
     def loop(self, count):
+        self.loop_count = count
         for i in range(count):
             print("Loop "+str(i)+"/"+str(count))
             self.gen(loop_number=i)
     def execute(self, data):
         if "prompt" in data:
             self.prompt = data['prompt']
         if "negative_prompt" in data:
@@ -179,15 +183,15 @@
         jobs = data['jobs']
         i = 0
         for job in jobs:
             self.info("Job " + str(i) + "/" + str(len(jobs)) )
             self.execute(job)
             i=i+1
         result_url = data['result_url']
-        if result_url.startswith('http'):
+        if result_url.startswith('http') and os.path.isfile('data.db'):
             files = {'upload_file': open('data.db', 'rb')}
             params = {'name': data['worker_name'], 'g': data['group_id']}
             res = requests.post(result_url, params=params, files=files)
             print(res.text)
             os.remove('data.db')
         self.info("End: "+time.strftime("%Y-%m-%d, %H:%M:%S", time.localtime()))
         return i
@@ -200,14 +204,19 @@
             self.info(res.text)
             self.info("Error: JSON Decode Error");
             return 0
         i = self.executeJobs(data)
         if i > 0 and askForMore:
             self.info('Asking for more Work')
             i = i + self.executeFromUrl(url, True)
+        elif i == 0 and askForMore:
+            self.info("Nothing to do.");
+            time.sleep(120)
+            self.info("Asking again");
+            i = i + self.executeFromUrl(url, True)
         return i
     def info(self, message):
         print("[INFO] " + message)
     def a1111models(self):
         self.initA1111();
         result = self.api.util_get_model_names()
         return result
@@ -217,18 +226,34 @@
         options['sd_model_checkpoint'] = model # 'model.ckpt [7460a6fa]'
         self.loaded_model = model
         self.api.set_options(options)
     def __str__(self):
         return f'ImageGen {self.generator} {self.model_id} {self.prefix}'
     def __repr__(self):
         return f'ImageGen(generator=\'{self.generator}\', model_id=\'{self.model_id}\', prefix=\'{self.prefix}\')'
-    def toSdJob(count:50):
+    def __call__(self, prefix, prompt):
+        self.prompt = prompt
+        self.prefix = prefix
+        self.loop(self.loop_count)
+        return "ImageGen"
+    def toSdJob(count:50, file = None):
         data = {prefix:self.prefix, prompt:self.prompt, count:count, height: self.height, self.width: width}
+        if not file is None:
+            text = json.dumps(data)
+            with open(self.prefix +'.sdjob', 'w') as f:
+                f.write(text)
         return data
-            
+    def p(self, prompt, append = False):
+        if append:
+            self.prompt = self.prompt + ' ' + prompt
+        else:
+            self.prompt = prompt
+        return self
+    def pb(self, prompt_b, append = False):
+        self.p(base64.b64decode(prompt_b), append)
         
 class ImageGenProcess(ticker.FileExtObserver):
     ext = ".sdjob"
     def __init__(self, generator=None):
         if generator is None:
             generator = ImageGen()
         self.generator = generator
@@ -260,39 +285,46 @@
         fernet = Fernet(self.key)
         with open(file, 'rb') as f:
             original = f.read()
         encrypted = fernet.decrypt(original)
         with open(file, 'wb') as encrypted_file:
             encrypted_file.write(encrypted)
     def download(self, doc):
+        self.log("Start Download")
         file = str(doc.id()) + '.sdjob'
         doc.save(file)
         if not self.key is None:
             self.decrypt(file)
         self.nweb.deleteDoc(doc.id())
+    def log(self, message):
+        print("JobFetch: "+str(message))
 class SdbUpload(ticker.Ticker):
     key = None
+    filename = 'data.db'
     def __init__(self, nwebclient=None, group=None, minSize = None):
         super().__init__("jobfetch",60*60*23) 
         from nwebclient import crypt
         from cryptography.fernet import Fernet
         self.nweb = nwebclient
         self.group = group
         self.minSize = minSize
     def execute(self):
-        filename = 'data.db'
-        if os.path.isfile(filename) and self.isBigEnough(filename):
-            self.upload(filename)
+        self.log("Execute")
+        if os.path.isfile(self.filename) and self.isBigEnough(self.filename):
+            self.upload(self.filename)
+    def log(self, message):
+        print("SdbUpload: "+str(message))
     def isBigEnough(self, file):
         if self.minSize == None:
             return True
         else:
             file_stats = os.stat(file)
             return file_stats.st_size > self.minSize
     def upload(self, file, remove = True):
+        self.log("Uploading")
         if not self.key is None:
             fernet = Fernet(self.key)
             with open(file, 'rb') as f:
                 original = f.read()
             encrypted = fernet.encrypt(original)
             with open(file, 'wb') as encrypted_file:
                 encrypted_file.write(encrypted)
```

### Comparing `nwebclient-1.0.92/nwebclient/sdb.py` & `nwebclient-1.0.93/nwebclient/sdb.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.92/nwebclient/ticker.py` & `nwebclient-1.0.93/nwebclient/ticker.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.92/nwebclient.egg-info/PKG-INFO` & `nwebclient-1.0.93/nwebclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.92
+Version: 1.0.93
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.92/setup.py` & `nwebclient-1.0.93/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nwebclient",
-    version="1.0.92",
+    version="1.0.93",
     author="Bjoern Salgert",
     author_email="bjoern.salgert@hs-duesseldorf.de",
     description="NWebClient via HTTP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bsnx.net/4.0/group/pynwebclient",
     packages=setuptools.find_packages(),
```

