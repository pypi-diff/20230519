# Comparing `tmp/text2phonemesequence-0.0.3.tar.gz` & `tmp/text2phonemesequence-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/text2phonemesequence-0.0.3.tar", last modified: Fri May 19 10:13:58 2023, max compression
+gzip compressed data, was "dist/text2phonemesequence-0.0.4.tar", last modified: Fri May 19 10:17:37 2023, max compression
```

## Comparing `text2phonemesequence-0.0.3.tar` & `text2phonemesequence-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-05-19 10:13:58.000000 text2phonemesequence-0.0.3/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     2640 2023-05-19 10:13:58.000000 text2phonemesequence-0.0.3/PKG-INFO
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     1777 2023-05-19 09:33:26.000000 text2phonemesequence-0.0.3/README.md
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       38 2023-05-19 10:13:58.000000 text2phonemesequence-0.0.3/setup.cfg
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     1291 2023-05-19 08:19:14.000000 text2phonemesequence-0.0.3/setup.py
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-05-19 10:13:58.000000 text2phonemesequence-0.0.3/text2phonemesequence/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)      162 2023-05-19 10:13:56.000000 text2phonemesequence-0.0.3/text2phonemesequence/__init__.py
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     6967 2023-05-19 10:13:35.000000 text2phonemesequence-0.0.3/text2phonemesequence/text2phonemesequence.py
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-05-19 10:13:58.000000 text2phonemesequence-0.0.3/text2phonemesequence.egg-info/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     2640 2023-05-19 10:13:58.000000 text2phonemesequence-0.0.3/text2phonemesequence.egg-info/PKG-INFO
--rw-rw-r--   0 vinai     (1000) vinai     (1000)      315 2023-05-19 10:13:58.000000 text2phonemesequence-0.0.3/text2phonemesequence.egg-info/SOURCES.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)        1 2023-05-19 10:13:58.000000 text2phonemesequence-0.0.3/text2phonemesequence.egg-info/dependency_links.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       27 2023-05-19 10:13:58.000000 text2phonemesequence-0.0.3/text2phonemesequence.egg-info/requires.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       21 2023-05-19 10:13:58.000000 text2phonemesequence-0.0.3/text2phonemesequence.egg-info/top_level.txt
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-05-19 10:17:37.000000 text2phonemesequence-0.0.4/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     2640 2023-05-19 10:17:37.000000 text2phonemesequence-0.0.4/PKG-INFO
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     1777 2023-05-19 09:33:26.000000 text2phonemesequence-0.0.4/README.md
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       38 2023-05-19 10:17:37.000000 text2phonemesequence-0.0.4/setup.cfg
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     1291 2023-05-19 08:19:14.000000 text2phonemesequence-0.0.4/setup.py
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-05-19 10:17:37.000000 text2phonemesequence-0.0.4/text2phonemesequence/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)      162 2023-05-19 10:17:26.000000 text2phonemesequence-0.0.4/text2phonemesequence/__init__.py
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     6978 2023-05-19 10:17:02.000000 text2phonemesequence-0.0.4/text2phonemesequence/text2phonemesequence.py
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-05-19 10:17:37.000000 text2phonemesequence-0.0.4/text2phonemesequence.egg-info/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     2640 2023-05-19 10:17:37.000000 text2phonemesequence-0.0.4/text2phonemesequence.egg-info/PKG-INFO
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)      315 2023-05-19 10:17:37.000000 text2phonemesequence-0.0.4/text2phonemesequence.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)        1 2023-05-19 10:17:37.000000 text2phonemesequence-0.0.4/text2phonemesequence.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       27 2023-05-19 10:17:37.000000 text2phonemesequence-0.0.4/text2phonemesequence.egg-info/requires.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       21 2023-05-19 10:17:37.000000 text2phonemesequence-0.0.4/text2phonemesequence.egg-info/top_level.txt
```

### Comparing `text2phonemesequence-0.0.3/PKG-INFO` & `text2phonemesequence-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2phonemesequence
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python Library to convert text to phoneme sequence used for XPhoneBERT
 Home-page: https://github.com/thelinhbkhn2014/Text2PhonemeSequence
 Author: Linh The Nguyen
 Author-email: toank45sphn@gmail.com
 Maintainer: linhthenguyen
 Maintainer-email: toank45sphn@gmail.com
 License: UNKNOWN
```

### Comparing `text2phonemesequence-0.0.3/README.md` & `text2phonemesequence-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `text2phonemesequence-0.0.3/setup.py` & `text2phonemesequence-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `text2phonemesequence-0.0.3/text2phonemesequence/text2phonemesequence.py` & `text2phonemesequence-0.0.4/text2phonemesequence/text2phonemesequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from transformers import T5ForConditionalGeneration, AutoTokenizer
 from segments import Tokenizer
 import os
 from tqdm import tqdm
 import sys 
-sys.path.append('./')
+sys.path.append('./dicts', './')
 
 
 class Text2PhonemeSequence:
     def __init__(self, pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', language='vie-c', is_cuda=True):
         self.tokenizer = AutoTokenizer.from_pretrained('google/byt5-small')
         self.model = T5ForConditionalGeneration.from_pretrained(pretrained_g2p_model)
         self.is_cuda = is_cuda
```

### Comparing `text2phonemesequence-0.0.3/text2phonemesequence.egg-info/PKG-INFO` & `text2phonemesequence-0.0.4/text2phonemesequence.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2phonemesequence
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python Library to convert text to phoneme sequence used for XPhoneBERT
 Home-page: https://github.com/thelinhbkhn2014/Text2PhonemeSequence
 Author: Linh The Nguyen
 Author-email: toank45sphn@gmail.com
 Maintainer: linhthenguyen
 Maintainer-email: toank45sphn@gmail.com
 License: UNKNOWN
```

