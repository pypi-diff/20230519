# Comparing `tmp/neuri-1.0.0.tar.gz` & `tmp/neuri-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\neuri-1.0.0.tar", last modified: Mon May 15 17:42:08 2023, max compression
+gzip compressed data, was "neuri-1.0.1.tar", last modified: Thu May 18 00:53:14 2023, max compression
```

## Comparing `neuri-1.0.0.tar` & `neuri-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 17:42:08.000000 neuri-1.0.0/
--rw-rw-rw-   0        0        0     1111 2023-05-05 10:28:43.000000 neuri-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     4654 2023-05-15 17:42:08.000000 neuri-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2563 2023-05-15 17:39:55.000000 neuri-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-15 17:42:08.000000 neuri-1.0.0/neuri/
--rw-rw-rw-   0        0        0       37 2023-05-05 10:37:41.000000 neuri-1.0.0/neuri/__init__.py
--rw-rw-rw-   0        0        0     6646 2023-05-15 15:50:37.000000 neuri-1.0.0/neuri/client.py
--rw-rw-rw-   0        0        0      619 2023-05-15 15:48:01.000000 neuri-1.0.0/neuri/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-15 17:42:08.000000 neuri-1.0.0/neuri.egg-info/
--rw-rw-rw-   0        0        0     4654 2023-05-15 17:42:08.000000 neuri-1.0.0/neuri.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-05-15 17:42:08.000000 neuri-1.0.0/neuri.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 17:42:08.000000 neuri-1.0.0/neuri.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-15 17:42:08.000000 neuri-1.0.0/neuri.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-15 17:42:08.000000 neuri-1.0.0/neuri.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 17:42:08.000000 neuri-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1206 2023-05-15 10:43:49.000000 neuri-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 00:53:14.271858 neuri-1.0.1/
+-rw-rw-rw-   0        0        0     1111 2023-05-05 10:28:43.000000 neuri-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     4666 2023-05-18 00:53:14.270859 neuri-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2575 2023-05-18 00:52:32.000000 neuri-1.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-18 00:53:14.245175 neuri-1.0.1/neuri/
+-rw-rw-rw-   0        0        0       37 2023-05-05 10:37:41.000000 neuri-1.0.1/neuri/__init__.py
+-rw-rw-rw-   0        0        0     6561 2023-05-18 00:51:00.000000 neuri-1.0.1/neuri/client.py
+-rw-rw-rw-   0        0        0      619 2023-05-15 15:48:01.000000 neuri-1.0.1/neuri/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-18 00:53:14.268696 neuri-1.0.1/neuri.egg-info/
+-rw-rw-rw-   0        0        0     4666 2023-05-18 00:53:13.000000 neuri-1.0.1/neuri.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-05-18 00:53:14.000000 neuri-1.0.1/neuri.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 00:53:13.000000 neuri-1.0.1/neuri.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-18 00:53:13.000000 neuri-1.0.1/neuri.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-18 00:53:13.000000 neuri-1.0.1/neuri.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 00:53:14.271858 neuri-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1206 2023-05-18 00:51:16.000000 neuri-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `neuri-1.0.0/LICENSE.txt` & `neuri-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `neuri-1.0.0/PKG-INFO` & `neuri-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuri
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python client library for the Neuri API
 Home-page: https://github.com/Neuri-ai/python-client
 Author: Neuri
 Author-email: support@neuri.ai
 License: MIT License
         
         Copyright (c) 2023 Neuri (https://github.com/Neuri-ai)
@@ -52,46 +52,51 @@
 
 To get started with the Neuri Python Client Library, you need to first install the library using pip:
 
 .. code-block:: python
 
   pip install neuri
 
+
+
 +++++
 Import and initialize the library
 +++++
 
 First you have to import the module and set up the client with your API key and service details, as shown below.
+
 .. code-block:: python
 
     import neuri
 
     config = {
         "service": "translate",
         "lang": "en",
         "temperature": 0.5,
         "api_key": "YOUR_API_KEY_HERE",
         "translate_to": "es" # optional
     }
 
     client = neuri.initialize_client(config)
 
+
 +++++
 Import and initialize the library
 +++++
 
 The Neuri Client Library currently supports three services: **audio_file**, **audio_url**, and **text**. Each service has its own set of parameters and returns a JSON containing the results of the processing.
 
 * **neuri.audio_file()**: Audio File.
 * **neuri.audio_url()**: Audio URL.
 * **neuri.text()**: Text
 
 +++++
 Audio File
 +++++
+
 Process audio files stored locally on your system using the audio_file service.
 
 .. code-block:: python
 
     result = client.audio_file(file_path=[
         os.path.join(os.path.dirname(__file__), "examples/girl_phone_call.wav"),
         os.path.join(os.path.dirname(__file__), "examples/noise_man_question.wav")
@@ -110,14 +115,15 @@
     result = client.audio_url(url="https://neuri-storage.s3.amazonaws.com/public_data/girl_phone_call.wav?AWSAccessKeyId=AKIAQFECGXRQOTIJ2FUV&Signature=GjrMz1NkMtQgFd0etJUCiQg4WNI%3D&Expires=1995267608")
 
 Replace the file paths in the url list with the actual paths to your audio files. The audio_url service will process the audio files and return the results in a JSON format.
 
 +++++
 Text
 +++++
+
 Process text using the text service.
 
 .. code-block:: python
 
     result = client.text(text="Hello, how are you?")
 
 Replace the text in the text parameter with the actual text you want to process. The text service will process the text and return the results in a JSON format.
```

### Comparing `neuri-1.0.0/README.rst` & `neuri-1.0.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,46 +10,51 @@
 
 To get started with the Neuri Python Client Library, you need to first install the library using pip:
 
 .. code-block:: python
 
   pip install neuri
 
+
+
 +++++
 Import and initialize the library
 +++++
 
 First you have to import the module and set up the client with your API key and service details, as shown below.
+
 .. code-block:: python
 
     import neuri
 
     config = {
         "service": "translate",
         "lang": "en",
         "temperature": 0.5,
         "api_key": "YOUR_API_KEY_HERE",
         "translate_to": "es" # optional
     }
 
     client = neuri.initialize_client(config)
 
+
 +++++
 Import and initialize the library
 +++++
 
 The Neuri Client Library currently supports three services: **audio_file**, **audio_url**, and **text**. Each service has its own set of parameters and returns a JSON containing the results of the processing.
 
 * **neuri.audio_file()**: Audio File.
 * **neuri.audio_url()**: Audio URL.
 * **neuri.text()**: Text
 
 +++++
 Audio File
 +++++
+
 Process audio files stored locally on your system using the audio_file service.
 
 .. code-block:: python
 
     result = client.audio_file(file_path=[
         os.path.join(os.path.dirname(__file__), "examples/girl_phone_call.wav"),
         os.path.join(os.path.dirname(__file__), "examples/noise_man_question.wav")
@@ -68,14 +73,15 @@
     result = client.audio_url(url="https://neuri-storage.s3.amazonaws.com/public_data/girl_phone_call.wav?AWSAccessKeyId=AKIAQFECGXRQOTIJ2FUV&Signature=GjrMz1NkMtQgFd0etJUCiQg4WNI%3D&Expires=1995267608")
 
 Replace the file paths in the url list with the actual paths to your audio files. The audio_url service will process the audio files and return the results in a JSON format.
 
 +++++
 Text
 +++++
+
 Process text using the text service.
 
 .. code-block:: python
 
     result = client.text(text="Hello, how are you?")
 
 Replace the text in the text parameter with the actual text you want to process. The text service will process the text and return the results in a JSON format.
```

### Comparing `neuri-1.0.0/neuri/client.py` & `neuri-1.0.1/neuri/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,17 +124,14 @@
 			files.append(
 				('files', (file_path.split('/')[-1], open(file_path, 'rb'), 'audio/wav')))
 		else:
 			for file in file_path:
 				files.append(
 					('files', (file.split('/')[-1], open(file, 'rb'), 'audio/wav')))
 
-		headers = {
-			'Authorization': 'Bearer s21FZ-ffdMbqfY3EAS6-vKOrHLI52dnZPw'
-		}
 		response = requests.request(
 			"POST", self.__URL, headers=headers, files=files)
 		try:
 			return json.loads(response.text)
 		except Exception as e:
 			return "Something went wrong. Please try again later."
```

### Comparing `neuri-1.0.0/neuri/exceptions.py` & `neuri-1.0.1/neuri/exceptions.py`

 * *Files identical despite different names*

### Comparing `neuri-1.0.0/neuri.egg-info/PKG-INFO` & `neuri-1.0.1/neuri.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuri
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python client library for the Neuri API
 Home-page: https://github.com/Neuri-ai/python-client
 Author: Neuri
 Author-email: support@neuri.ai
 License: MIT License
         
         Copyright (c) 2023 Neuri (https://github.com/Neuri-ai)
@@ -52,46 +52,51 @@
 
 To get started with the Neuri Python Client Library, you need to first install the library using pip:
 
 .. code-block:: python
 
   pip install neuri
 
+
+
 +++++
 Import and initialize the library
 +++++
 
 First you have to import the module and set up the client with your API key and service details, as shown below.
+
 .. code-block:: python
 
     import neuri
 
     config = {
         "service": "translate",
         "lang": "en",
         "temperature": 0.5,
         "api_key": "YOUR_API_KEY_HERE",
         "translate_to": "es" # optional
     }
 
     client = neuri.initialize_client(config)
 
+
 +++++
 Import and initialize the library
 +++++
 
 The Neuri Client Library currently supports three services: **audio_file**, **audio_url**, and **text**. Each service has its own set of parameters and returns a JSON containing the results of the processing.
 
 * **neuri.audio_file()**: Audio File.
 * **neuri.audio_url()**: Audio URL.
 * **neuri.text()**: Text
 
 +++++
 Audio File
 +++++
+
 Process audio files stored locally on your system using the audio_file service.
 
 .. code-block:: python
 
     result = client.audio_file(file_path=[
         os.path.join(os.path.dirname(__file__), "examples/girl_phone_call.wav"),
         os.path.join(os.path.dirname(__file__), "examples/noise_man_question.wav")
@@ -110,14 +115,15 @@
     result = client.audio_url(url="https://neuri-storage.s3.amazonaws.com/public_data/girl_phone_call.wav?AWSAccessKeyId=AKIAQFECGXRQOTIJ2FUV&Signature=GjrMz1NkMtQgFd0etJUCiQg4WNI%3D&Expires=1995267608")
 
 Replace the file paths in the url list with the actual paths to your audio files. The audio_url service will process the audio files and return the results in a JSON format.
 
 +++++
 Text
 +++++
+
 Process text using the text service.
 
 .. code-block:: python
 
     result = client.text(text="Hello, how are you?")
 
 Replace the text in the text parameter with the actual text you want to process. The text service will process the text and return the results in a JSON format.
```

### Comparing `neuri-1.0.0/setup.py` & `neuri-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def open_file(fname):
     return open(os.path.join(os.path.dirname(__file__), fname))
 
 setup(
   name = 'neuri',
   packages = ['neuri'],
-  version = '1.0.0',
+  version = '1.0.1',
   license=open('LICENSE.txt').read(),
   description = 'Python client library for the Neuri API',
   author = 'Neuri',
   author_email = 'support@neuri.ai',
   url = 'https://github.com/Neuri-ai/python-client',  # use the URL to the github repo
   keywords = ["api client", "neuri", "neuri.ai", "neuri api"],
   classifiers = [
```

