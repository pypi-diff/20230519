# Comparing `tmp/Pydule-3.3.3.tar.gz` & `tmp/Pydule-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pydule-3.3.3.tar", last modified: Thu May 11 15:17:16 2023, max compression
+gzip compressed data, was "Pydule-3.3.4.tar", last modified: Fri May 19 06:17:48 2023, max compression
```

## Comparing `Pydule-3.3.3.tar` & `Pydule-3.3.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 15:17:16.402519 Pydule-3.3.3/
--rw-rw-rw-   0        0        0     2662 2023-05-11 15:17:16.382758 Pydule-3.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     1898 2023-05-11 15:13:44.000000 Pydule-3.3.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-11 15:17:16.402519 Pydule-3.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1428 2023-05-11 15:14:23.000000 Pydule-3.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:17:16.333357 Pydule-3.3.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-11 15:17:16.382758 Pydule-3.3.3/src/Pydule.egg-info/
--rw-rw-rw-   0        0        0     2662 2023-05-11 15:17:15.000000 Pydule-3.3.3/src/Pydule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-05-11 15:17:15.000000 Pydule-3.3.3/src/Pydule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 15:17:15.000000 Pydule-3.3.3/src/Pydule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      209 2023-05-11 15:17:15.000000 Pydule-3.3.3/src/Pydule.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-11 15:17:15.000000 Pydule-3.3.3/src/Pydule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    16000 2023-05-11 15:12:34.000000 Pydule-3.3.3/src/Pydule.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:17:48.684229 Pydule-3.3.4/
+-rw-rw-rw-   0        0        0     2547 2023-05-19 06:17:48.653219 Pydule-3.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1783 2023-05-19 06:08:01.000000 Pydule-3.3.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-19 06:17:48.684229 Pydule-3.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1474 2023-05-19 06:07:38.000000 Pydule-3.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:17:48.434976 Pydule-3.3.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-19 06:17:48.637382 Pydule-3.3.4/src/Pydule.egg-info/
+-rw-rw-rw-   0        0        0     2547 2023-05-19 06:17:47.000000 Pydule-3.3.4/src/Pydule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-05-19 06:17:47.000000 Pydule-3.3.4/src/Pydule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 06:17:47.000000 Pydule-3.3.4/src/Pydule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      237 2023-05-19 06:17:47.000000 Pydule-3.3.4/src/Pydule.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-19 06:17:47.000000 Pydule-3.3.4/src/Pydule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    21890 2023-05-19 06:13:53.000000 Pydule-3.3.4/src/Pydule.py
```

### Comparing `Pydule-3.3.3/PKG-INFO` & `Pydule-3.3.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pydule
-Version: 3.3.3
+Version: 3.3.4
 Summary: Access ChatGPT,Track Location,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..
 Author: D.Tamil Mutharasan
 Keywords: python,PyDule,Module,Pydule,pydule,matrix,qrcode,youtube,weather,list,tuple,set,dictionary,clear,color,pick_color,open,app,search,play,mp3,song,restart,system,shutdown,date,time,text_to_speech,text,speech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -15,34 +15,33 @@
 # Pydule-TM
 
 [![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)                 
 [![Python 3.6](https://img.shields.io/badge/python-3.10.7-blue.svg)](https://www.python.org/downloads/release/python-3107/)   
 
 ## Functionality of Pydule
 
+- Get Battery Percentage
 - Access ChatGPT
 - Get Any Website HTML
-- Encode and Decode a String
+- Encrypt and Decrypt a String
 - Record Screen,Internal Audio and Microphone
 - Seperate String
-- Swap Dictionary's Key to Values and Values to Key
 - Insert Elements in Tuple & String
 - Generate Qrcode
 - Copy Text
-- Text Translation
+- Language Translation
 - Edit JSON Files
 - Replace Letters in String
-- Replace Elements in List and Tuple
 - Check Weather of any City
 - Open any File
 - Play Songs
 - Get Hex of any Color
 - Convert Text to Speech
 - Convert Speech to Text
-- Restart or Shutdown Your System
+- Restart and Shutdown Your System
 - Search on Browser
 - +40 more Functions
 
 ## Usage
 
 - Make sure you have Python installed in your system.
 - Run Following command in the CMD.
@@ -51,48 +50,45 @@
   ```
 ## Example
 
  ```
 # test.py
 import Pydule as py
 
+# to Find the Remaining Battery Percentage
+battery=py.aboutbattery('percentage')
+print(battery)
+
 # to Search 
 py.search('Youtube')
 
-# to Swap Dictionary
-d={1:2,2:3,3:4}
-print(py.swapdict(d))
-
-# to Encode String
-string,Key=py.codestr('Hello World')
-
-# to Code the String
-x,y=py.codestr('Hi') #This Converts Hi to @^&-+*^+^=##&*
-
-# to Decode the String
-print(py.dcodestr(x,py.swapdict(y)))
-
 # to Get Any Website HTML
-print(py.GetWebHTML('URL'))
+html=py.GetWebHTML('URL')
+print(html)
 
 # to Create Qrcode
 text,filename='Hello World','Hello.png'
 py.cqrcode(text,filename)
 
+# to get the Location of the Selected File
+path=py.askfile()
+print(path)
+
 # to Get all Available Functions
 py.functions() 
 
 # to Open Calculator
 py.openapp('calculator')
 
 # to Copy Text
 py.copytext('Hello World')
 
 # to play mp3
 py.playmusic('PATH')
 
 # to Access ChatGPT
-print(py.ChatGPT('Hi There','Your API Key'))
+from Pydule import AI
+print(AI.ChatGPT('Hi There','Your API Key'))
 
 # to Track the Location
 print(py.TrackLocation('Your Phone Number')) #Example +911234567890
   ```
```

### Comparing `Pydule-3.3.3/README.md` & `Pydule-3.3.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 # Pydule-TM
 
 [![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)                 
 [![Python 3.6](https://img.shields.io/badge/python-3.10.7-blue.svg)](https://www.python.org/downloads/release/python-3107/)   
 
 ## Functionality of Pydule
 
+- Get Battery Percentage
 - Access ChatGPT
 - Get Any Website HTML
-- Encode and Decode a String
+- Encrypt and Decrypt a String
 - Record Screen,Internal Audio and Microphone
 - Seperate String
-- Swap Dictionary's Key to Values and Values to Key
 - Insert Elements in Tuple & String
 - Generate Qrcode
 - Copy Text
-- Text Translation
+- Language Translation
 - Edit JSON Files
 - Replace Letters in String
-- Replace Elements in List and Tuple
 - Check Weather of any City
 - Open any File
 - Play Songs
 - Get Hex of any Color
 - Convert Text to Speech
 - Convert Speech to Text
-- Restart or Shutdown Your System
+- Restart and Shutdown Your System
 - Search on Browser
 - +40 more Functions
 
 ## Usage
 
 - Make sure you have Python installed in your system.
 - Run Following command in the CMD.
@@ -37,48 +36,45 @@
   ```
 ## Example
 
  ```
 # test.py
 import Pydule as py
 
+# to Find the Remaining Battery Percentage
+battery=py.aboutbattery('percentage')
+print(battery)
+
 # to Search 
 py.search('Youtube')
 
-# to Swap Dictionary
-d={1:2,2:3,3:4}
-print(py.swapdict(d))
-
-# to Encode String
-string,Key=py.codestr('Hello World')
-
-# to Code the String
-x,y=py.codestr('Hi') #This Converts Hi to @^&-+*^+^=##&*
-
-# to Decode the String
-print(py.dcodestr(x,py.swapdict(y)))
-
 # to Get Any Website HTML
-print(py.GetWebHTML('URL'))
+html=py.GetWebHTML('URL')
+print(html)
 
 # to Create Qrcode
 text,filename='Hello World','Hello.png'
 py.cqrcode(text,filename)
 
+# to get the Location of the Selected File
+path=py.askfile()
+print(path)
+
 # to Get all Available Functions
 py.functions() 
 
 # to Open Calculator
 py.openapp('calculator')
 
 # to Copy Text
 py.copytext('Hello World')
 
 # to play mp3
 py.playmusic('PATH')
 
 # to Access ChatGPT
-print(py.ChatGPT('Hi There','Your API Key'))
+from Pydule import AI
+print(AI.ChatGPT('Hi There','Your API Key'))
 
 # to Track the Location
 print(py.TrackLocation('Your Phone Number')) #Example +911234567890
   ```
```

### Comparing `Pydule-3.3.3/setup.py` & `Pydule-3.3.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open('README.md','r') as fh:
 	long_description = fh.read()
 
 setup(
 	name='Pydule',
-	version='3.3.3',
+	version='3.3.4',
 	description="Access ChatGPT,Track Location,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..",
 	author='D.Tamil Mutharasan',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	packages=setuptools.find_packages(),
 	keywords=['python','PyDule','Module','Pydule','pydule','matrix','qrcode','youtube','weather','list','tuple','set','dictionary','clear','color','pick_color','open','app','search','play','mp3','song','restart','system','shutdown','date','time','text_to_speech','text','speech'],
 	classifiers=[
@@ -26,25 +26,28 @@
 	install_requires=[
 		'beautifulsoup4',
 		'pyttsx3',
 		'pywhatkit',
 		'pyglet',
 		'datetime',
 		'requests',
+		'psutil',
 		'AppOpener',
 		'deep_translator',
 		'qrcode',
 		'numpy',
 		'pyperclip',
 		'soundfile',
 		'soundcard',
 		'pyautogui',
 		'pyaudio',
 		'wave',
 		'opencv-python',
 		'openai',
 		'phonenumbers',
 		'SpeechRecognition',
-		'Pillow'
+		'Pillow',
+		'pyinstaller',
+		'pyfiglet'
 	]
 
 )
```

### Comparing `Pydule-3.3.3/src/Pydule.egg-info/PKG-INFO` & `Pydule-3.3.4/src/Pydule.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pydule
-Version: 3.3.3
+Version: 3.3.4
 Summary: Access ChatGPT,Track Location,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..
 Author: D.Tamil Mutharasan
 Keywords: python,PyDule,Module,Pydule,pydule,matrix,qrcode,youtube,weather,list,tuple,set,dictionary,clear,color,pick_color,open,app,search,play,mp3,song,restart,system,shutdown,date,time,text_to_speech,text,speech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -15,34 +15,33 @@
 # Pydule-TM
 
 [![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)                 
 [![Python 3.6](https://img.shields.io/badge/python-3.10.7-blue.svg)](https://www.python.org/downloads/release/python-3107/)   
 
 ## Functionality of Pydule
 
+- Get Battery Percentage
 - Access ChatGPT
 - Get Any Website HTML
-- Encode and Decode a String
+- Encrypt and Decrypt a String
 - Record Screen,Internal Audio and Microphone
 - Seperate String
-- Swap Dictionary's Key to Values and Values to Key
 - Insert Elements in Tuple & String
 - Generate Qrcode
 - Copy Text
-- Text Translation
+- Language Translation
 - Edit JSON Files
 - Replace Letters in String
-- Replace Elements in List and Tuple
 - Check Weather of any City
 - Open any File
 - Play Songs
 - Get Hex of any Color
 - Convert Text to Speech
 - Convert Speech to Text
-- Restart or Shutdown Your System
+- Restart and Shutdown Your System
 - Search on Browser
 - +40 more Functions
 
 ## Usage
 
 - Make sure you have Python installed in your system.
 - Run Following command in the CMD.
@@ -51,48 +50,45 @@
   ```
 ## Example
 
  ```
 # test.py
 import Pydule as py
 
+# to Find the Remaining Battery Percentage
+battery=py.aboutbattery('percentage')
+print(battery)
+
 # to Search 
 py.search('Youtube')
 
-# to Swap Dictionary
-d={1:2,2:3,3:4}
-print(py.swapdict(d))
-
-# to Encode String
-string,Key=py.codestr('Hello World')
-
-# to Code the String
-x,y=py.codestr('Hi') #This Converts Hi to @^&-+*^+^=##&*
-
-# to Decode the String
-print(py.dcodestr(x,py.swapdict(y)))
-
 # to Get Any Website HTML
-print(py.GetWebHTML('URL'))
+html=py.GetWebHTML('URL')
+print(html)
 
 # to Create Qrcode
 text,filename='Hello World','Hello.png'
 py.cqrcode(text,filename)
 
+# to get the Location of the Selected File
+path=py.askfile()
+print(path)
+
 # to Get all Available Functions
 py.functions() 
 
 # to Open Calculator
 py.openapp('calculator')
 
 # to Copy Text
 py.copytext('Hello World')
 
 # to play mp3
 py.playmusic('PATH')
 
 # to Access ChatGPT
-print(py.ChatGPT('Hi There','Your API Key'))
+from Pydule import AI
+print(AI.ChatGPT('Hi There','Your API Key'))
 
 # to Track the Location
 print(py.TrackLocation('Your Phone Number')) #Example +911234567890
   ```
```

