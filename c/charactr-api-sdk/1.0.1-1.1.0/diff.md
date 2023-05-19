# Comparing `tmp/charactr_api_sdk-1.0.1.tar.gz` & `tmp/charactr_api_sdk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charactr_api_sdk-1.0.1.tar", last modified: Thu Apr 13 10:18:29 2023, max compression
+gzip compressed data, was "charactr_api_sdk-1.1.0.tar", last modified: Fri May 19 10:21:12 2023, max compression
```

## Comparing `charactr_api_sdk-1.0.1.tar` & `charactr_api_sdk-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 wiktormazur   (501) staff       (20)        0 2023-04-13 10:18:29.660997 charactr_api_sdk-1.0.1/
--rw-r--r--   0 wiktormazur   (501) staff       (20)    15061 2023-03-27 13:43:23.000000 charactr_api_sdk-1.0.1/LICENSE.rst
--rw-r--r--   0 wiktormazur   (501) staff       (20)       24 2023-03-30 10:29:57.000000 charactr_api_sdk-1.0.1/MANIFEST.in
--rw-r--r--   0 wiktormazur   (501) staff       (20)     1588 2023-04-13 10:18:29.661122 charactr_api_sdk-1.0.1/PKG-INFO
--rw-r--r--   0 wiktormazur   (501) staff       (20)     1257 2023-04-13 10:11:51.000000 charactr_api_sdk-1.0.1/README.md
-drwxr-xr-x   0 wiktormazur   (501) staff       (20)        0 2023-04-13 10:18:29.653843 charactr_api_sdk-1.0.1/charactr_api/
--rw-r--r--   0 wiktormazur   (501) staff       (20)      119 2023-04-11 10:22:44.000000 charactr_api_sdk-1.0.1/charactr_api/__init__.py
-drwxr-xr-x   0 wiktormazur   (501) staff       (20)        0 2023-04-13 10:18:29.659022 charactr_api_sdk-1.0.1/charactr_api/sdk/
--rw-r--r--   0 wiktormazur   (501) staff       (20)        0 2023-04-05 10:03:54.000000 charactr_api_sdk-1.0.1/charactr_api/sdk/__init__.py
--rw-r--r--   0 wiktormazur   (501) staff       (20)      101 2023-04-13 09:51:59.000000 charactr_api_sdk-1.0.1/charactr_api/sdk/config.py
--rw-r--r--   0 wiktormazur   (501) staff       (20)     1059 2023-04-13 09:51:59.000000 charactr_api_sdk-1.0.1/charactr_api/sdk/conversion_module.py
--rw-r--r--   0 wiktormazur   (501) staff       (20)      692 2023-03-30 10:37:01.000000 charactr_api_sdk-1.0.1/charactr_api/sdk/data_objects.py
--rw-r--r--   0 wiktormazur   (501) staff       (20)     1011 2023-04-06 11:56:16.000000 charactr_api_sdk-1.0.1/charactr_api/sdk/errors.py
--rw-r--r--   0 wiktormazur   (501) staff       (20)      269 2023-03-30 10:29:57.000000 charactr_api_sdk-1.0.1/charactr_api/sdk/sdk.py
--rw-r--r--   0 wiktormazur   (501) staff       (20)     1222 2023-04-13 09:51:59.000000 charactr_api_sdk-1.0.1/charactr_api/sdk/tts.py
--rw-r--r--   0 wiktormazur   (501) staff       (20)     1478 2023-04-13 09:51:59.000000 charactr_api_sdk-1.0.1/charactr_api/sdk/vc.py
-drwxr-xr-x   0 wiktormazur   (501) staff       (20)        0 2023-04-13 10:18:29.660730 charactr_api_sdk-1.0.1/charactr_api_sdk.egg-info/
--rw-r--r--   0 wiktormazur   (501) staff       (20)     1588 2023-04-13 10:18:29.000000 charactr_api_sdk-1.0.1/charactr_api_sdk.egg-info/PKG-INFO
--rw-r--r--   0 wiktormazur   (501) staff       (20)      518 2023-04-13 10:18:29.000000 charactr_api_sdk-1.0.1/charactr_api_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 wiktormazur   (501) staff       (20)        1 2023-04-13 10:18:29.000000 charactr_api_sdk-1.0.1/charactr_api_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 wiktormazur   (501) staff       (20)       57 2023-04-13 10:18:29.000000 charactr_api_sdk-1.0.1/charactr_api_sdk.egg-info/requires.txt
--rw-r--r--   0 wiktormazur   (501) staff       (20)       13 2023-04-13 10:18:29.000000 charactr_api_sdk-1.0.1/charactr_api_sdk.egg-info/top_level.txt
--rw-r--r--   0 wiktormazur   (501) staff       (20)       57 2023-04-13 10:14:01.000000 charactr_api_sdk-1.0.1/requirements.txt
--rw-r--r--   0 wiktormazur   (501) staff       (20)      107 2023-04-13 10:18:29.661586 charactr_api_sdk-1.0.1/setup.cfg
--rw-r--r--   0 wiktormazur   (501) staff       (20)      660 2023-04-13 10:18:01.000000 charactr_api_sdk-1.0.1/setup.py
+drwxr-xr-x   0 wiktormazur   (501) staff       (20)        0 2023-05-19 10:21:12.930270 charactr_api_sdk-1.1.0/
+-rw-r--r--   0 wiktormazur   (501) staff       (20)    15061 2023-05-15 14:22:09.000000 charactr_api_sdk-1.1.0/LICENSE.rst
+-rw-r--r--   0 wiktormazur   (501) staff       (20)       24 2023-05-15 14:22:09.000000 charactr_api_sdk-1.1.0/MANIFEST.in
+-rw-r--r--   0 wiktormazur   (501) staff       (20)     1754 2023-05-19 10:21:12.930381 charactr_api_sdk-1.1.0/PKG-INFO
+-rw-r--r--   0 wiktormazur   (501) staff       (20)     1423 2023-05-17 10:12:53.000000 charactr_api_sdk-1.1.0/README.md
+drwxr-xr-x   0 wiktormazur   (501) staff       (20)        0 2023-05-19 10:21:12.923162 charactr_api_sdk-1.1.0/charactr_api/
+-rw-r--r--   0 wiktormazur   (501) staff       (20)      119 2023-05-15 14:22:09.000000 charactr_api_sdk-1.1.0/charactr_api/__init__.py
+drwxr-xr-x   0 wiktormazur   (501) staff       (20)        0 2023-05-19 10:21:12.928536 charactr_api_sdk-1.1.0/charactr_api/sdk/
+-rw-r--r--   0 wiktormazur   (501) staff       (20)        0 2023-05-15 14:22:09.000000 charactr_api_sdk-1.1.0/charactr_api/sdk/__init__.py
+-rw-r--r--   0 wiktormazur   (501) staff       (20)      133 2023-05-17 10:26:53.000000 charactr_api_sdk-1.1.0/charactr_api/sdk/config.py
+-rw-r--r--   0 wiktormazur   (501) staff       (20)     1059 2023-05-15 14:22:09.000000 charactr_api_sdk-1.1.0/charactr_api/sdk/conversion_module.py
+-rw-r--r--   0 wiktormazur   (501) staff       (20)      780 2023-05-16 11:37:19.000000 charactr_api_sdk-1.1.0/charactr_api/sdk/data_objects.py
+-rw-r--r--   0 wiktormazur   (501) staff       (20)     1135 2023-05-16 11:30:13.000000 charactr_api_sdk-1.1.0/charactr_api/sdk/errors.py
+-rw-r--r--   0 wiktormazur   (501) staff       (20)      269 2023-05-15 14:22:09.000000 charactr_api_sdk-1.1.0/charactr_api/sdk/sdk.py
+-rw-r--r--   0 wiktormazur   (501) staff       (20)     2387 2023-05-19 10:20:27.000000 charactr_api_sdk-1.1.0/charactr_api/sdk/tts.py
+-rw-r--r--   0 wiktormazur   (501) staff       (20)     3983 2023-05-17 10:11:46.000000 charactr_api_sdk-1.1.0/charactr_api/sdk/tts_stream_duplex.py
+-rw-r--r--   0 wiktormazur   (501) staff       (20)     1961 2023-05-17 10:09:40.000000 charactr_api_sdk-1.1.0/charactr_api/sdk/tts_stream_simplex.py
+-rw-r--r--   0 wiktormazur   (501) staff       (20)     1478 2023-05-15 14:22:09.000000 charactr_api_sdk-1.1.0/charactr_api/sdk/vc.py
+drwxr-xr-x   0 wiktormazur   (501) staff       (20)        0 2023-05-19 10:21:12.930018 charactr_api_sdk-1.1.0/charactr_api_sdk.egg-info/
+-rw-r--r--   0 wiktormazur   (501) staff       (20)     1754 2023-05-19 10:21:12.000000 charactr_api_sdk-1.1.0/charactr_api_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 wiktormazur   (501) staff       (20)      595 2023-05-19 10:21:12.000000 charactr_api_sdk-1.1.0/charactr_api_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 wiktormazur   (501) staff       (20)        1 2023-05-19 10:21:12.000000 charactr_api_sdk-1.1.0/charactr_api_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 wiktormazur   (501) staff       (20)       81 2023-05-19 10:21:12.000000 charactr_api_sdk-1.1.0/charactr_api_sdk.egg-info/requires.txt
+-rw-r--r--   0 wiktormazur   (501) staff       (20)       13 2023-05-19 10:21:12.000000 charactr_api_sdk-1.1.0/charactr_api_sdk.egg-info/top_level.txt
+-rw-r--r--   0 wiktormazur   (501) staff       (20)       81 2023-05-17 10:02:16.000000 charactr_api_sdk-1.1.0/requirements.txt
+-rw-r--r--   0 wiktormazur   (501) staff       (20)      107 2023-05-19 10:21:12.930881 charactr_api_sdk-1.1.0/setup.cfg
+-rw-r--r--   0 wiktormazur   (501) staff       (20)      660 2023-05-19 10:21:10.000000 charactr_api_sdk-1.1.0/setup.py
```

### Comparing `charactr_api_sdk-1.0.1/LICENSE.rst` & `charactr_api_sdk-1.1.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `charactr_api_sdk-1.0.1/PKG-INFO` & `charactr_api_sdk-1.1.0/charactr_api_sdk.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: charactr_api_sdk
-Version: 1.0.1
+Name: charactr-api-sdk
+Version: 1.1.0
 Summary: Python SDK to interact with the charactr API.
 Home-page: https://github.com/charactr-platform/charactr-api-sdk-python
 Author: charactr
 Author-email: support@charactr.com
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
@@ -55,11 +55,21 @@
 Open `./examples/credentials.py` and provide your credentials. You can find them in your [Client Panel](https://api.charactr.com) account.
 
 #### Use TTS
 ```bash
 $ python examples/tts.py
 ```
 
+#### Use TTS Simplex Streaming
+```bash
+$ python examples/tts_stream_simplex.py
+```
+
+#### Use TTS Duplex Streaming
+```bash
+$ python examples/tts_stream_duplex.py
+```
+
 #### Use VC
 ```bash
 $ python examples/vc.py
 ```
```

### Comparing `charactr_api_sdk-1.0.1/README.md` & `charactr_api_sdk-1.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -44,11 +44,21 @@
 Open `./examples/credentials.py` and provide your credentials. You can find them in your [Client Panel](https://api.charactr.com) account.
 
 #### Use TTS
 ```bash
 $ python examples/tts.py
 ```
 
+#### Use TTS Simplex Streaming
+```bash
+$ python examples/tts_stream_simplex.py
+```
+
+#### Use TTS Duplex Streaming
+```bash
+$ python examples/tts_stream_duplex.py
+```
+
 #### Use VC
 ```bash
 $ python examples/vc.py
 ```
```

### Comparing `charactr_api_sdk-1.0.1/charactr_api/sdk/conversion_module.py` & `charactr_api_sdk-1.1.0/charactr_api/sdk/conversion_module.py`

 * *Files identical despite different names*

### Comparing `charactr_api_sdk-1.0.1/charactr_api/sdk/data_objects.py` & `charactr_api_sdk-1.1.0/charactr_api/sdk/data_objects.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,7 +31,13 @@
 
 
 class Audio(TypedDict):
     data: bytes
     type: str
     duration_ms: int
     size_bytes: int
+
+
+class TTSMsgType:
+    AUTH = "authApiKey"
+    CONVERT = "convert"
+    CLOSE = "close"
```

### Comparing `charactr_api_sdk-1.0.1/charactr_api/sdk/errors.py` & `charactr_api_sdk-1.1.0/charactr_api/sdk/errors.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 import json
 
 
+class ConnectionClosedError(Exception):
+    def __init__(self):
+        super().__init__("Connection is already closed.")
+
+
 class ClientError(Exception):
     """Exception raised for 4xx http errors"""
 
     def __init__(self, code: int, message: str):
         super().__init__("[{0}] {1}".format(code, message))
```

### Comparing `charactr_api_sdk-1.0.1/charactr_api/sdk/tts.py` & `charactr_api_sdk-1.1.0/charactr_api/sdk/vc.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,47 @@
-import json
 import requests
+from typing import Dict
+from requests_toolbelt.multipart.encoder import MultipartEncoder
 
 from .config import API_URL, ApiVersion
-from .data_objects import Audio, Credentials
+from .data_objects import Credentials
 from .conversion_module import ConversionModule
 from .errors import get_api_error
 
 
-class TTS(ConversionModule):
+class VC(ConversionModule):
     def __init__(self, credentials: Credentials) -> None:
-        super().__init__(credentials, "tts")
+        super().__init__(credentials, "vc")
+
+    def convert(self, voice_id: int, input_audio: bytes) -> Dict:
+        """Convert one voice to another with audio file input."""
+        multipart_data = MultipartEncoder(
+            fields={"file": ("file.wav", input_audio, "audio/wav")}
+        )
 
-    def convert(self, voice_id: int, text: str) -> Audio:
-        """Convert text to speech with the voice of your choice."""
         headers = {
             "X-Client-Key": self.credentials["client_key"],
             "X-API-Key": self.credentials["api_key"],
-            "Content-Type": "application/json",
+            "Content-Type": multipart_data.content_type,
         }
-        data = {"voiceId": voice_id, "text": text}
 
         response = requests.post(
-            API_URL + "/" + ApiVersion.V1.value + "/" + self.module_name + "/convert",
+            API_URL
+            + "/"
+            + ApiVersion.V1.value
+            + "/"
+            + self.module_name
+            + "/convert?voiceId="
+            + str(voice_id),
             headers=headers,
-            data=json.dumps(data),
+            data=multipart_data,
         )
 
         if response.status_code != 200:
             raise get_api_error(response)
 
-        return Audio(
-            data=response.content,
-            type=response.headers["Content-Type"],
-            duration_ms=response.headers["Audio-Duration-Ms"],
-            size_bytes=response.headers["Audio-Size-Bytes"],
-        )
+        return {
+            "data": response.content,
+            "type": response.headers["Content-Type"],
+            "duration_ms": response.headers["Audio-Duration-Ms"],
+            "size_bytes": response.headers["Audio-Size-Bytes"],
+        }
```

### Comparing `charactr_api_sdk-1.0.1/charactr_api_sdk.egg-info/PKG-INFO` & `charactr_api_sdk-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: charactr-api-sdk
-Version: 1.0.1
+Name: charactr_api_sdk
+Version: 1.1.0
 Summary: Python SDK to interact with the charactr API.
 Home-page: https://github.com/charactr-platform/charactr-api-sdk-python
 Author: charactr
 Author-email: support@charactr.com
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
@@ -55,11 +55,21 @@
 Open `./examples/credentials.py` and provide your credentials. You can find them in your [Client Panel](https://api.charactr.com) account.
 
 #### Use TTS
 ```bash
 $ python examples/tts.py
 ```
 
+#### Use TTS Simplex Streaming
+```bash
+$ python examples/tts_stream_simplex.py
+```
+
+#### Use TTS Duplex Streaming
+```bash
+$ python examples/tts_stream_duplex.py
+```
+
 #### Use VC
 ```bash
 $ python examples/vc.py
 ```
```

### Comparing `charactr_api_sdk-1.0.1/charactr_api_sdk.egg-info/SOURCES.txt` & `charactr_api_sdk-1.1.0/charactr_api_sdk.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,13 +8,15 @@
 charactr_api/sdk/__init__.py
 charactr_api/sdk/config.py
 charactr_api/sdk/conversion_module.py
 charactr_api/sdk/data_objects.py
 charactr_api/sdk/errors.py
 charactr_api/sdk/sdk.py
 charactr_api/sdk/tts.py
+charactr_api/sdk/tts_stream_duplex.py
+charactr_api/sdk/tts_stream_simplex.py
 charactr_api/sdk/vc.py
 charactr_api_sdk.egg-info/PKG-INFO
 charactr_api_sdk.egg-info/SOURCES.txt
 charactr_api_sdk.egg-info/dependency_links.txt
 charactr_api_sdk.egg-info/requires.txt
 charactr_api_sdk.egg-info/top_level.txt
```

### Comparing `charactr_api_sdk-1.0.1/setup.py` & `charactr_api_sdk-1.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     requirements = req_f.read().splitlines()
 
 setup(
     name="charactr_api_sdk",
     description="Python SDK to interact with the charactr API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    version="1.0.1",
+    version="1.1.0",
     author="charactr",
     author_email="support@charactr.com",
     url="https://github.com/charactr-platform/charactr-api-sdk-python",
     packages=find_packages(),
     include_package_data=True,
     install_requires=requirements,
     python_requires=">=3.8.0",
```

