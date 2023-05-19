# Comparing `tmp/deep-translator-1.9.2.tar.gz` & `tmp/deep-translator-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep-translator-1.9.2.tar", last modified: Sat Jan 14 23:03:15 2023, max compression
+gzip compressed data, was "deep-translator-1.9.3.tar", last modified: Thu Feb  2 21:39:00 2023, max compression
```

## Comparing `deep-translator-1.9.2.tar` & `deep-translator-1.9.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     1032 2023-01-14 23:01:48.774404 deep-translator-1.9.2/deep_translator/__init__.py
--rw-r--r--   0        0        0      106 2023-01-14 23:01:48.774404 deep-translator-1.9.2/deep_translator/__main__.py
--rw-r--r--   0        0        0     4960 2023-01-14 23:01:48.774404 deep-translator-1.9.2/deep_translator/base.py
--rw-r--r--   0        0        0     3158 2023-01-14 23:01:48.774404 deep-translator-1.9.2/deep_translator/cli.py
--rw-r--r--   0        0        0     6110 2023-01-14 23:01:48.774404 deep-translator-1.9.2/deep_translator/constants.py
--rw-r--r--   0        0        0     3310 2023-01-14 23:01:48.774404 deep-translator-1.9.2/deep_translator/deepl.py
--rw-r--r--   0        0        0     2645 2023-01-14 23:01:48.774404 deep-translator-1.9.2/deep_translator/detection.py
--rw-r--r--   0        0        0      191 2023-01-14 23:01:48.774404 deep-translator-1.9.2/deep_translator/engines.py
--rw-r--r--   0        0        0     4512 2023-01-14 23:01:48.778404 deep-translator-1.9.2/deep_translator/exceptions.py
--rw-r--r--   0        0        0     3945 2023-01-14 23:01:48.778404 deep-translator-1.9.2/deep_translator/google.py
--rw-r--r--   0        0        0     3834 2023-01-14 23:01:48.778404 deep-translator-1.9.2/deep_translator/libre.py
--rw-r--r--   0        0        0     3605 2023-01-14 23:01:48.778404 deep-translator-1.9.2/deep_translator/linguee.py
--rw-r--r--   0        0        0     4617 2023-01-14 23:01:48.778404 deep-translator-1.9.2/deep_translator/microsoft.py
--rw-r--r--   0        0        0     3454 2023-01-14 23:01:48.778404 deep-translator-1.9.2/deep_translator/mymemory.py
--rw-r--r--   0        0        0     3100 2023-01-14 23:01:48.778404 deep-translator-1.9.2/deep_translator/papago.py
--rw-r--r--   0        0        0     3425 2023-01-14 23:01:48.778404 deep-translator-1.9.2/deep_translator/pons.py
--rw-r--r--   0        0        0     3030 2023-01-14 23:01:48.778404 deep-translator-1.9.2/deep_translator/qcri.py
--rw-r--r--   0        0        0      607 2023-01-14 23:01:48.778404 deep-translator-1.9.2/deep_translator/validate.py
--rw-r--r--   0        0        0     4298 2023-01-14 23:01:48.778404 deep-translator-1.9.2/deep_translator/yandex.py
--rw-r--r--   0        0        0    23793 2023-01-14 23:01:48.778404 deep-translator-1.9.2/docs/README.rst
--rw-r--r--   0        0        0     1968 2023-01-14 23:01:48.778404 deep-translator-1.9.2/pyproject.toml
--rw-r--r--   0        0        0    25796 2023-01-14 23:03:15.113227 deep-translator-1.9.2/setup.py
--rw-r--r--   0        0        0    25430 2023-01-14 23:03:15.114277 deep-translator-1.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-02-02 21:37:29.130190 deep-translator-1.9.3/LICENSE
+-rw-r--r--   0        0        0     1086 2023-02-02 21:37:29.134190 deep-translator-1.9.3/deep_translator/__init__.py
+-rw-r--r--   0        0        0      162 2023-02-02 21:37:29.134190 deep-translator-1.9.3/deep_translator/__main__.py
+-rw-r--r--   0        0        0     5014 2023-02-02 21:37:29.134190 deep-translator-1.9.3/deep_translator/base.py
+-rw-r--r--   0        0        0     3213 2023-02-02 21:37:29.134190 deep-translator-1.9.3/deep_translator/cli.py
+-rw-r--r--   0        0        0     6291 2023-02-02 21:37:29.134190 deep-translator-1.9.3/deep_translator/constants.py
+-rw-r--r--   0        0        0     3366 2023-02-02 21:37:29.134190 deep-translator-1.9.3/deep_translator/deepl.py
+-rw-r--r--   0        0        0     2700 2023-02-02 21:37:29.134190 deep-translator-1.9.3/deep_translator/detection.py
+-rw-r--r--   0        0        0      246 2023-02-02 21:37:29.134190 deep-translator-1.9.3/deep_translator/engines.py
+-rw-r--r--   0        0        0     4567 2023-02-02 21:37:29.134190 deep-translator-1.9.3/deep_translator/exceptions.py
+-rw-r--r--   0        0        0     3999 2023-02-02 21:37:29.134190 deep-translator-1.9.3/deep_translator/google.py
+-rw-r--r--   0        0        0     3887 2023-02-02 21:37:29.134190 deep-translator-1.9.3/deep_translator/libre.py
+-rw-r--r--   0        0        0     3667 2023-02-02 21:37:29.134190 deep-translator-1.9.3/deep_translator/linguee.py
+-rw-r--r--   0        0        0     4670 2023-02-02 21:37:29.134190 deep-translator-1.9.3/deep_translator/microsoft.py
+-rw-r--r--   0        0        0     3509 2023-02-02 21:37:29.134190 deep-translator-1.9.3/deep_translator/mymemory.py
+-rw-r--r--   0        0        0     3155 2023-02-02 21:37:29.134190 deep-translator-1.9.3/deep_translator/papago.py
+-rw-r--r--   0        0        0     3480 2023-02-02 21:37:29.134190 deep-translator-1.9.3/deep_translator/pons.py
+-rw-r--r--   0        0        0     3085 2023-02-02 21:37:29.134190 deep-translator-1.9.3/deep_translator/qcri.py
+-rw-r--r--   0        0        0      662 2023-02-02 21:37:29.134190 deep-translator-1.9.3/deep_translator/validate.py
+-rw-r--r--   0        0        0     4353 2023-02-02 21:37:29.134190 deep-translator-1.9.3/deep_translator/yandex.py
+-rw-r--r--   0        0        0    23690 2023-02-02 21:37:29.134190 deep-translator-1.9.3/docs/README.rst
+-rw-r--r--   0        0        0     1968 2023-02-02 21:37:29.138191 deep-translator-1.9.3/pyproject.toml
+-rw-r--r--   0        0        0    25686 2023-02-02 21:39:00.167699 deep-translator-1.9.3/setup.py
+-rw-r--r--   0        0        0    25327 2023-02-02 21:39:00.168872 deep-translator-1.9.3/PKG-INFO
```

### Comparing `deep-translator-1.9.2/deep_translator/__init__.py` & `deep-translator-1.9.3/deep_translator/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Top-level package for Deep Translator"""
 
+__copyright__ = "Copyright (C) 2020 Nidhal Baccouri"
+
 from deep_translator.deepl import DeeplTranslator
 from deep_translator.detection import batch_detection, single_detection
 from deep_translator.google import GoogleTranslator
 from deep_translator.libre import LibreTranslator
 from deep_translator.linguee import LingueeTranslator
 from deep_translator.microsoft import MicrosoftTranslator
 from deep_translator.mymemory import MyMemoryTranslator
```

### Comparing `deep-translator-1.9.2/deep_translator/base.py` & `deep-translator-1.9.3/deep_translator/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """base translator class"""
 
+__copyright__ = "Copyright (C) 2020 Nidhal Baccouri"
+
 from abc import ABC, abstractmethod
 from typing import List, Optional, Union
 
 from deep_translator.constants import GOOGLE_LANGUAGES_TO_CODES
 from deep_translator.exceptions import (
     InvalidSourceOrTargetLanguage,
     LanguageNotSupportedException,
```

### Comparing `deep-translator-1.9.2/deep_translator/cli.py` & `deep-translator-1.9.3/deep_translator/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 """Console script for deep_translator."""
+
+__copyright__ = "Copyright (C) 2020 Nidhal Baccouri"
+
 import argparse
 from typing import Optional
 
 from deep_translator.engines import __engines__
 
 
 class CLI(object):
```

### Comparing `deep-translator-1.9.2/deep_translator/constants.py` & `deep-translator-1.9.3/deep_translator/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+
+__copyright__ = "Copyright (C) 2020 Nidhal Baccouri"
+
+
 BASE_URLS = {
     "GOOGLE_TRANSLATE": "https://translate.google.com/m",
     "PONS": "https://en.pons.com/translate/",
     "YANDEX": "https://translate.yandex.net/api/{version}/tr.json/{endpoint}",
     "LINGUEE": "https://www.linguee.com/",
     "MYMEMORY": "http://api.mymemory.translated.net/get",
     "QCRI": "https://mt.qcri.org/api/v1/{endpoint}?",
@@ -172,41 +176,41 @@
     "es": "spanish",
     "sv": "swedish",
     "tr": "turkish",
     "elv": "elvish",
 }
 
 LINGUEE_LANGUAGES_TO_CODES = {
-    "maltese": "mt",
-    "english": "en",
-    "german": "de",
-    "bulgarian": "bg",
-    "polish": "pl",
-    "portuguese": "pt",
-    "hungarian": "hu",
-    "romanian": "ro",
-    "russian": "ru",
+    "maltese": "maltese",
+    "english": "english",
+    "german": "german",
+    "bulgarian": "bulgarian",
+    "polish": "polish",
+    "portuguese": "portuguese",
+    "hungarian": "hungarian",
+    "romanian": "romanian",
+    "russian": "russian",
     # "serbian": "sr",
-    "dutch": "nl",
-    "slovakian": "sk",
-    "greek": "el",
-    "slovenian": "sl",
-    "danish": "da",
-    "italian": "it",
-    "spanish": "es",
-    "finnish": "fi",
-    "chinese": "zh",
-    "french": "fr",
+    "dutch": "dutch",
+    "slovakian": "slovakian",
+    "greek": "greek",
+    "slovenian": "slovenian",
+    "danish": "danish",
+    "italian": "italian",
+    "spanish": "spanish",
+    "finnish": "finnish",
+    "chinese": "chinese",
+    "french": "french",
     # "croatian": "hr",
-    "czech": "cs",
-    "laotian": "lo",
-    "swedish": "sv",
-    "latvian": "lv",
-    "estonian": "et",
-    "japanese": "ja",
+    "czech": "czech",
+    "laotian": "laotian",
+    "swedish": "swedish",
+    "latvian": "latvian",
+    "estonian": "estonian",
+    "japanese": "japanese",
 }
 
 DEEPL_LANGUAGE_TO_CODE = {
     "bulgarian": "bg",
     "czech": "cs",
     "danish": "da",
     "german": "de",
@@ -228,15 +232,15 @@
     "romanian": "ro",
     "russian": "ru",
     "slovak": "sk",
     "slovenian": "sl",
     "swedish": "sv",
     "turkish": "tr",
     "ukrainian": "uk",
-    "chinese": "zh",    
+    "chinese": "zh",
 }
 
 PAPAGO_LANGUAGE_TO_CODE = {
     "ko": "Korean",
     "en": "English",
     "ja": "Japanese",
     "zh-CN": "Chinese",
```

### Comparing `deep-translator-1.9.2/deep_translator/deepl.py` & `deep-translator-1.9.3/deep_translator/deepl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+
+
+__copyright__ = "Copyright (C) 2020 Nidhal Baccouri"
+
 from typing import List, Optional
 
 import requests
 
 from deep_translator.base import BaseTranslator
 from deep_translator.constants import BASE_URLS, DEEPL_LANGUAGE_TO_CODE
 from deep_translator.exceptions import (
```

### Comparing `deep-translator-1.9.2/deep_translator/detection.py` & `deep-translator-1.9.3/deep_translator/detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """
 language detection API
 """
+
+__copyright__ = "Copyright (C) 2020 Nidhal Baccouri"
+
 from typing import List, Optional, Union
 
 import requests
 from requests.exceptions import HTTPError
 
 # Module global config
 config = {
```

### Comparing `deep-translator-1.9.2/deep_translator/exceptions.py` & `deep-translator-1.9.3/deep_translator/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+
+__copyright__ = "Copyright (C) 2020 Nidhal Baccouri"
+
 class BaseError(Exception):
     """
     base error structure class
     """
 
     def __init__(self, val, message):
         """
```

### Comparing `deep-translator-1.9.2/deep_translator/google.py` & `deep-translator-1.9.3/deep_translator/google.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 google translator API
 """
 
+__copyright__ = "Copyright (C) 2020 Nidhal Baccouri"
+
 from typing import List, Optional
 
 import requests
 from bs4 import BeautifulSoup
 
 from deep_translator.base import BaseTranslator
 from deep_translator.constants import BASE_URLS
```

### Comparing `deep-translator-1.9.2/deep_translator/libre.py` & `deep-translator-1.9.3/deep_translator/libre.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 LibreTranslate API
 """
+__copyright__ = "Copyright (C) 2020 Nidhal Baccouri"
 
 from typing import List, Optional
 
 import requests
 
 from deep_translator.base import BaseTranslator
 from deep_translator.constants import BASE_URLS, LIBRE_LANGUAGES_TO_CODES
```

### Comparing `deep-translator-1.9.2/deep_translator/linguee.py` & `deep-translator-1.9.3/deep_translator/linguee.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """
 linguee translator API
 """
+
+__copyright__ = "Copyright (C) 2020 Nidhal Baccouri"
+
 from typing import List, Optional, Union
 
 import requests
 from bs4 import BeautifulSoup
 from requests.utils import requote_uri
 
 from deep_translator.base import BaseTranslator
@@ -55,28 +58,28 @@
         """
         if self._same_source_target() or is_empty(word):
             return word
 
         if is_input_valid(word, max_chars=50):
             # %s-%s/translation/%s.html
             url = (
-                f"{self._base_url}{self._source}-{self._target}/translation/{word}.html"
+                f"{self._base_url}{self._source}-{self._target}/search/?source={self._source}&query={word}"
             )
             url = requote_uri(url)
             response = requests.get(url, proxies=self.proxies)
 
             if response.status_code == 429:
                 raise TooManyRequests()
 
             if response.status_code != 200:
                 raise RequestError()
             soup = BeautifulSoup(response.text, "html.parser")
             elements = soup.find_all(self._element_tag, self._element_query)
             response.close()
-            
+
             if not elements:
                 raise ElementNotFoundInGetRequest(elements)
 
             filtered_elements = []
             for el in elements:
                 try:
                     pronoun = el.find("span", {"class": "placeholder"}).get_text(
```

### Comparing `deep-translator-1.9.2/deep_translator/microsoft.py` & `deep-translator-1.9.3/deep_translator/microsoft.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # -*- coding: utf-8 -*-
 
+__copyright__ = "Copyright (C) 2020 Nidhal Baccouri"
+
 import logging
 import sys
 from typing import List, Optional
 
 import requests
 
 from deep_translator.base import BaseTranslator
@@ -37,15 +39,15 @@
 
         self.api_key = api_key
         self.proxies = proxies
         self.headers = {
             "Ocp-Apim-Subscription-Key": self.api_key,
             "Content-type": "application/json",
         }
-        # region is not required but very common and goes to headers if passed
+        #region is not required but very common and goes to headers if passed
         if region:
             self.region = region
             self.headers["Ocp-Apim-Subscription-Region"] = self.region
         super().__init__(
             base_url=BASE_URLS.get("MICROSOFT_TRANSLATE"),
             source=source,
             target=target,
```

### Comparing `deep-translator-1.9.2/deep_translator/mymemory.py` & `deep-translator-1.9.3/deep_translator/mymemory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """
 mymemory translator API
 """
+
+__copyright__ = "Copyright (C) 2020 Nidhal Baccouri"
+
 from typing import List, Optional, Union
 
 import requests
 
 from deep_translator.base import BaseTranslator
 from deep_translator.constants import BASE_URLS
 from deep_translator.exceptions import (
```

### Comparing `deep-translator-1.9.2/deep_translator/papago.py` & `deep-translator-1.9.3/deep_translator/papago.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """
-google translator API
+papago translator API
 """
+
+__copyright__ = "Copyright (C) 2020 Nidhal Baccouri"
+
 import json
 from typing import List, Optional
 
 import requests
 
 from deep_translator.base import BaseTranslator
 from deep_translator.constants import BASE_URLS, PAPAGO_LANGUAGE_TO_CODE
```

### Comparing `deep-translator-1.9.2/deep_translator/pons.py` & `deep-translator-1.9.3/deep_translator/pons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """
 pons translator API
 """
+
+__copyright__ = "Copyright (C) 2020 Nidhal Baccouri"
+
 from typing import List, Optional, Union
 
 import requests
 from bs4 import BeautifulSoup
 from requests.utils import requote_uri
 
 from deep_translator.base import BaseTranslator
```

### Comparing `deep-translator-1.9.2/deep_translator/qcri.py` & `deep-translator-1.9.3/deep_translator/qcri.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+
+__copyright__ = "Copyright (C) 2020 Nidhal Baccouri"
+
 from typing import List, Optional
 
 import requests
 
 from deep_translator.base import BaseTranslator
 from deep_translator.constants import BASE_URLS, QCRI_LANGUAGE_TO_CODE
 from deep_translator.exceptions import ServerException, TranslationNotFound
```

### Comparing `deep-translator-1.9.2/deep_translator/validate.py` & `deep-translator-1.9.3/deep_translator/validate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+
+__copyright__ = "Copyright (C) 2020 Nidhal Baccouri"
+
 from deep_translator.exceptions import NotValidLength, NotValidPayload
 
 
 def is_empty(text: str) -> bool:
     return text == ""
```

### Comparing `deep-translator-1.9.2/deep_translator/yandex.py` & `deep-translator-1.9.3/deep_translator/yandex.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """
 Yandex translator API
 """
+
+__copyright__ = "Copyright (C) 2020 Nidhal Baccouri"
+
 from typing import List, Optional
 
 import requests
 
 from deep_translator.base import BaseTranslator
 from deep_translator.constants import BASE_URLS
 from deep_translator.exceptions import (
```

### Comparing `deep-translator-1.9.2/docs/README.rst` & `deep-translator-1.9.3/docs/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -403,17 +403,14 @@
 
 - Simple Translation
 
 .. code-block:: python
 
     translated_word = LingueeTranslator(source='english', target='french').translate(word)
 
-    # pass language by their abbreviation
-    translated_word = LingueeTranslator(source='en', target='fr').translate(word)
-
 - Return all synonyms or words that match
 
 .. code-block:: python
 
     # set the argument return_all to True if you want to get all synonyms of the word to translate
     translated_word = LingueeTranslator(source='english', target='french').translate(word, return_all=True)
 
@@ -652,15 +649,15 @@
 
     $ deep-translator languages google
 
 ======
 Tests
 ======
 
-Developers can install the development version of deep-translator and execute unit tests to verify functionality. For more information on doing this, see `the contribution guidelines <https://deep-translator.readthedocs.io/en/latest/contributing.html/>`_
+Developers can install the development version of deep-translator and execute unit tests to verify functionality. For more information on doing this, see `the contribution guidelines <https://deep-translator.readthedocs.io/en/latest/contributing.html#get-started>`_
 
 ========
 Links
 ========
 Check this article on medium to know why you should use the deep-translator package and how to translate text using python.
 https://medium.com/@nidhalbacc/how-to-translate-text-with-python-9d203139dcf5
 
@@ -684,15 +681,15 @@
 
 ===========
 Next Steps
 ===========
 
 Take a look in the examples folder for more :)
 Contributions are always welcome.
-Read the Contribution guidelines `Here <https://deep-translator.readthedocs.io/en/latest/contributing.html/>`_
+Read the Contribution guidelines `Here <https://deep-translator.readthedocs.io/en/latest/contributing.html#get-started>`_
 
 ==========
 Credits
 ==========
 
 Many thanks to @KirillSklyarenko for his work on integrating the microsoft translator
```

### Comparing `deep-translator-1.9.2/pyproject.toml` & `deep-translator-1.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deep-translator"
-version = "1.9.2"
+version = "1.9.3"
 description = "A flexible free and unlimited python tool to translate between different languages in a simple way using multiple translators"
 license = "MIT"
 authors = ["Nidhal Baccouri <nidhalbacc@gmail.com>"]
 maintainers = ["Nidhal Baccouri <nidhalbacc@gmail.com>", "Chris Trenthem <trenthemc@gmail.com>"]
 readme = "docs/README.rst"
 homepage = "https://github.com/nidhaloff/deep_translator"
 repository = "https://github.com/nidhaloff/deep_translator"
```

### Comparing `deep-translator-1.9.2/setup.py` & `deep-translator-1.9.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 entry_points = \
 {'console_scripts': ['deep-translator = deep_translator.__main__:main',
                      'dt = deep_translator.__main__:main']}
 
 setup_kwargs = {
     'name': 'deep-translator',
-    'version': '1.9.2',
+    'version': '1.9.3',
     'description': 'A flexible free and unlimited python tool to translate between different languages in a simple way using multiple translators',
-    'long_description': '##################\ndeep-translator\n##################\n\n.. image:: ../assets/icon.jpg\n    :width: 100\n    :align: center\n    :alt: deep-translator-icon\n\n|\n\n\n.. image:: https://img.shields.io/pypi/v/deep-translator.svg\n        :target: https://pypi.python.org/pypi/deep-translator\n.. image:: https://img.shields.io/travis/nidhaloff/deep-translator.svg\n        :target: https://github.com/nidhaloff/deep-translator/actions/workflows/build.yml\n.. image:: https://readthedocs.org/projects/deep-translator/badge/?version=latest\n        :target: https://deep-translator.readthedocs.io/en/latest/?badge=latest\n        :alt: Documentation Status\n.. image:: https://img.shields.io/pypi/l/deep-translator\n        :target: https://pypi.python.org/pypi/deep-translator\n\n.. image:: https://img.shields.io/pypi/status/deep-translator\n        :target: https://pypi.python.org/pypi/deep-translator\n\n.. image:: https://pepy.tech/badge/deep-translator\n    :target: https://pepy.tech/project/deep-translator\n\n\n.. image:: https://img.shields.io/pypi/wheel/deep-translator\n        :target: https://pypi.python.org/pypi/deep-translator\n\n.. image:: https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2FNidhalBaccouri\n        :alt: Twitter URL\n        :target: https://twitter.com/NidhalBaccouri\n\n\n=======================\nTranslation for humans\n=======================\n\nA flexible **FREE** and **UNLIMITED** tool to translate between different languages in a simple way using multiple translators.\n\n\n* Free software: MIT license\n* Documentation: https://deep-translator.readthedocs.io.\n* Swagger API: https://deep-translator-api.azurewebsites.net/docs.\n\n|\n|\n\n.. contents:: Table of Contents\n    :depth: 3\n\n|\n|\n\n\n==========\nMotivation\n==========\n\nI needed to translate a text using python. It was hard to find a simple way to do it.\nThere are other libraries that can be used for this task, but most of them\nare **buggy, not free, limited, not supported anymore or complex to use.**\n\nTherefore, I decided to build this simple tool. It is 100% free, unlimited, easy to use and provides\nsupport for all languages.\n\nBasically, my goal was to integrate support for multiple famous translators\nin this tool.\n\n======================\nWhen you should use it\n======================\n\n- If you want to translate text using python\n- If you want to translate from a file\n- If you want to get translations from many sources and not only one\n- If you want to automate translations\n- If you want to compare different translations\n- If you want to detect language automatically\n\n======================\nWhy you should use it\n======================\n\n- It\'s the only python tool that integrates many translators\n- Multi language support\n- Supports batch translation\n- High level of abstraction\n- Automatic language detection\n- Easy to use and extend\n- Support for most famous universal translators\n- Stable and maintained regularly\n- The API is very easy to use\n- Proxy integration is supported\n\n========\nFeatures\n========\n\n* Support for `google translate <https://translate.google.com/>`_\n* Support for the `microsoft translator <https://www.microsoft.com/en-us/translator//>`_ (version >= 1.3.5)\n* Support for `Pons translator <https://de.pons.com/>`_\n* Support for the `Linguee translator <https://www.linguee.com/>`_\n* Support for the `Mymemory translator <https://mymemory.translated.net/>`_\n* Support for the `Yandex translator <https://yandex.com/>`_ (version >= 1.2.1)\n* Support for the `QcriTranslator translator <https://mt.qcri.org/api/>`_ (version >= 1.2.4)\n* Support for the `DeeplTranslator translator <https://www.deepl.com/en/translator/>`_ (version >= 1.2.5)\n* Support for the `Papago translator <https://papago.naver.com/>`_ (version >= 1.4.4)\n* Support for the `Libre translator <https://libretranslate.com/>`_\n* Support for proxy usage\n* Automatic single language detection\n* Batch language detection\n* Translate directly from a text file\n* Get multiple translation for a word\n* Automate the translation of different paragraphs in different languages\n* Translate directly from terminal (version >= 1.1.0)\n\n=============\nInstallation\n=============\n\nInstall the stable release:\n\n.. code-block:: console\n\n    $ pip install -U deep-translator\n\ntake a look at the docs if you want to install from source.\n\n============\nQuick Start\n============\n\n.. code-block:: python\n\n    from deep_translator import GoogleTranslator\n    translated = GoogleTranslator(source=\'auto\', target=\'de\').translate("keep it up, you are awesome")  # output -> Weiter so, du bist großartig\n\nor using proxies:\n\n.. code-block:: python\n\n    from deep_translator import GoogleTranslator\n\n    proxies_example = {\n        "https": "34.195.196.27:8080",\n        "http": "34.195.196.27:8080"\n    }\n    translated = GoogleTranslator(source=\'auto\', target=\'de\', proxies=proxies_example).translate("keep it up, you are awesome")  # output -> Weiter so, du bist großartig\n\n\nor even directly from terminal:\n\n.. code-block:: console\n\n    $ deep-translator --source "en" --target "de" --text "hello world"\n\n    or shorter\n\n    $ dt -tg de -txt "hello world"\n\n\n=====\nUsage\n=====\n\nIn this section, demos on how to use all different integrated translators in this tool are provided.\n\n.. note::\n\n    You can always pass the languages by the name or by abbreviation.\n\n    *Example*: If you want to use english as a source or target language, you can pass **english** or **en** as an argument\n\nImports\n--------\n\n.. code-block:: python\n\n    from deep_translator import (GoogleTranslator,\n                                 MicrosoftTranslator,\n                                 PonsTranslator,\n                                 LingueeTranslator,\n                                 MyMemoryTranslator,\n                                 YandexTranslator,\n                                 PapagoTranslator,\n                                 DeeplTranslator,\n                                 QcriTranslator,\n                                 single_detection,\n                                 batch_detection)\n\n\nCheck Supported Languages\n---------------------------\n\n.. note::\n\n    You can check the supported languages of each translator by calling the\n    get_supported_languages function.\n\n.. code-block:: python\n\n    # default return type is a list\n    langs_list = GoogleTranslator().get_supported_languages()  # output: [arabic, french, english etc...]\n\n    # alternatively, you can the dictionary containing languages mapped to their abbreviation\n    langs_dict = GoogleTranslator().get_supported_languages(as_dict=True)  # output: {arabic: ar, french: fr, english:en etc...}\n\nLanguage Detection\n------------------\n\n.. note::\n\n    You can also detect language automatically. Notice that this package is free and my goal is to keep it free.\n    Therefore, you will need to get your own api_key if you want to use the language detection function.\n    I figured out you can get one for free here: https://detectlanguage.com/documentation\n\n- Single Text Detection\n\n.. code-block:: python\n\n    lang = single_detection(\'bonjour la vie\', api_key=\'your_api_key\')\n    print(lang) # output: fr\n\n- Batch Detection\n\n.. code-block:: python\n\n    lang = batch_detection([\'bonjour la vie\', \'hello world\'], api_key=\'your_api_key\')\n    print(lang) # output: [fr, en]\n\n\n\nGoogle Translate\n-----------------\n\n.. code-block:: python\n\n    text = \'happy coding\'\n\n- You can use automatic language detection to detect the source language:\n\n.. code-block:: python\n\n    translated = GoogleTranslator(source=\'auto\', target=\'de\').translate(text=text)\n\n- You can pass languages by name or by abbreviation:\n\n.. code-block:: python\n\n    translated = GoogleTranslator(source=\'auto\', target=\'german\').translate(text=text)\n\n    # Alternatively, you can pass languages by their abbreviation:\n    translated = GoogleTranslator(source=\'en\', target=\'de\').translate(text=text)\n\n- You can also reuse the Translator class and change/update its properties.\n\n(Notice that this is important for performance too, since instantiating new objects is expensive)\n\n\n.. code-block:: python\n\n    # let\'s say first you need to translate from auto to german\n    my_translator = GoogleTranslator(source=\'auto\', target=\'german\')\n    result = my_translator.translate(text=text)\n    print(f"Translation using source = {my_translator.source} and target = {my_translator.target} -> {result}")\n\n    # let\'s say later you want to reuse the class but your target is french now\n    # This is the best practice and how you should use deep-translator.\n    # Please don\'t over-instantiate translator objects without a good reason, otherwise you will run into performance issues\n    my_translator.target = \'fr\'  # this will override the target \'german\' passed previously\n    result = my_translator.translate(text=text)\n    print(f"Translation using source = {my_translator.source} and target = {my_translator.target} -> {result}")\n\n    # you can also update the source language as well\n    my_translator.source = \'en\'  # this will override the source \'auto\' passed previously\n    result = my_translator.translate(text=text)\n    print(f"Translation using source = {my_translator.source} and target = {my_translator.target} -> {result}")\n\n\n- Translate batch of texts\n\n.. code-block:: python\n\n    texts = ["hallo welt", "guten morgen"]\n\n    # the translate_sentences function is deprecated, use the translate_batch function instead\n    translated = GoogleTranslator(\'de\', \'en\').translate_batch(texts)\n\n- Translate from a file:\n\n.. code-block:: python\n\n    translated = GoogleTranslator(source=\'auto\', target=\'german\').translate_file(\'path/to/file\')\n\nMymemory Translator\n--------------------\n\n.. note::\n\n    As in google translate, you can use the automatic language detection with mymemory by using "auto" as an\n    argument for the source language. However, this feature in the mymemory translator is not so powerful as\n    in google translate.\n\n- Simple translation\n\n.. code-block:: python\n\n    text = \'Keep it up. You are awesome\'\n\n    translated = MyMemoryTranslator(source=\'auto\', target=\'french\').translate(text)\n\n- Translate batch of texts\n\n.. code-block:: python\n\n    texts = ["hallo welt", "guten morgen"]\n\n    # the translate_sentences function is deprecated, use the translate_batch function instead\n    translated = MyMemoryTranslator(\'de\', \'en\').translate_batch(texts)\n\n- Translate from file\n\n.. code-block:: python\n\n    path = "your_file.txt"\n\n    translated = MyMemoryTranslator(source=\'en\', target=\'fr\').translate_file(path)\n\n\nDeeplTranslator\n-----------------\n\n.. note::\n\n    In order to use the DeeplTranslator translator, you need to generate an api key. Deepl offers a Pro and a free API.\n    deep-translator supports both Pro and free APIs. Just check the examples below.\n    Visit https://www.deepl.com/en/docs-api/ for more information on how to generate your Deepl api key\n\n- Simple translation\n\n.. code-block:: python\n\n    text = \'Keep it up. You are awesome\'\n\n    translated = DeeplTranslator(api_key="your_api_key", source="en", target="en", use_free_api=True).translate(text)\n\n.. note::\n        deep-translator uses free deepl api by default. If you have the pro version then simply set the use_free_api to false.\n\n\n- Translate batch of texts\n\n.. code-block:: python\n\n    texts = ["hallo welt", "guten morgen"]\n\n    # the translate_sentences function is deprecated, use the translate_batch function instead\n    translated = DeeplTranslator("your_api_key").translate_batch(texts)\n\nQcriTranslator\n--------------------\n\n.. note::\n\n    In order to use the QcriTranslator translator, you need to generate a free api key. Visit https://mt.qcri.org/api/\n    for more information\n\n- Check languages\n\n.. code-block:: python\n\n    # as a property\n    print("language pairs: ", QcriTranslator("your_api_key").languages)\n\n- Check domains\n\n.. code-block:: python\n\n    # as a property\n    print("domains: ", QcriTranslator("your_api_key").domains)\n\n- Text translation\n\n.. code-block:: python\n\n    text = \'Education is great\'\n\n    translated = QcriTranslator("your_api_key").translate(source=\'en\', target=\'ar\', domain="news", text=text)\n    # output -> التعليم هو عظيم\n\n    # see docs for batch translation and more.\n\nLinguee Translator\n-------------------\n\n.. code-block:: python\n\n    word = \'good\'\n\n- Simple Translation\n\n.. code-block:: python\n\n    translated_word = LingueeTranslator(source=\'english\', target=\'french\').translate(word)\n\n    # pass language by their abbreviation\n    translated_word = LingueeTranslator(source=\'en\', target=\'fr\').translate(word)\n\n- Return all synonyms or words that match\n\n.. code-block:: python\n\n    # set the argument return_all to True if you want to get all synonyms of the word to translate\n    translated_word = LingueeTranslator(source=\'english\', target=\'french\').translate(word, return_all=True)\n\n- Translate a batch of words\n\n.. code-block:: python\n\n    translated_words = LingueeTranslator(source=\'english\', target=\'french\').translate_words(["good", "awesome"])\n\nPONS Translator\n----------------\n\n.. note::\n\n    You can pass the languages by the name or by abbreviation just like\n    previous examples using GoogleTranslate\n\n.. code-block:: python\n\n    word = \'awesome\'\n\n- Simple Translation\n\n.. code-block:: python\n\n    translated_word = PonsTranslator(source=\'english\', target=\'french\').translate(word)\n\n    # pass language by their abbreviation\n    translated_word = PonsTranslator(source=\'en\', target=\'fr\').translate(word)\n\n- Return all synonyms or words that match\n\n.. code-block:: python\n\n    # set the argument return_all to True if you want to get all synonyms of the word to translate\n    translated_word = PonsTranslator(source=\'english\', target=\'french\').translate(word, return_all=True)\n\n- Translate a batch of words\n\n.. code-block:: python\n\n    translated_words = LingueeTranslator(source=\'english\', target=\'french\').translate_words(["good", "awesome"])\n\nYandex Translator\n------------------\n\n.. note::\n\n    You need to require a **private api key** if you want to use the yandex translator.\n    Visit the official website for more information about how to get one\n\n- Language detection\n\n.. code-block:: python\n\n    lang = YandexTranslator(\'your_api_key\').detect(\'Hallo, Welt\')\n    print(f"language detected: {lang}")  # output -> language detected: \'de\'\n\n- Text translation\n\n.. code-block:: python\n\n    # with auto detection | meaning provide only the target language and let yandex detect the source\n    translated = YandexTranslator(\'your_api_key\').translate(source="auto", target="en", text=\'Hallo, Welt\')\n    print(f"translated text: {translated}")  # output -> translated text: Hello world\n\n    # provide source and target language explicitly\n    translated = YandexTranslator(\'your_api_key\').translate(source="de", target="en", text=\'Hallo, Welt\')\n    print(f"translated text: {translated}")  # output -> translated text: Hello world\n\n- File translation\n\n.. code-block:: python\n\n    translated = YandexTranslator(\'your_api_key\').translate_file(source="auto", target="en", path="path_to_your_file")\n\n- Batch translation\n\n.. code-block:: python\n\n    translated = YandexTranslator(\'your_api_key\').translate_batch(source="auto", target="de", batch=["hello world", "happy coding"])\n\n\nMicrosoft Translator\n---------------------\n\n.. note::\n\n    You need to require an **api key** if you want to use the microsoft translator.\n    Visit the official website for more information about how to get one.\n    Microsoft offers a free tier 0 subscription (2 million characters per month).\n\n- Required and optional attributes\n\n    There are two required attributes, namely "api_key" (string) and "target" (string or list).\n    Attribute "source" is optional.\n    Also, Microsoft API accepts a number of other optional attributes, you can find them here:  https://docs.microsoft.com/azure/cognitive-services/translator/reference/v3-0-translate\n    You can simply add them after the required attributes, see the example.\n\n.. code-block:: python\n\n    text = \'happy coding\'\n    translated = MicrosoftTranslator(api_key=\'some-key\', target=\'de\').translate(text=text)\n    translated_two_targets = MicrosoftTranslator(api_key=\'some-key\', target=[\'de\', \'ru\']).translate(text=text)\n    translated_with_optional_attr = MicrosoftTranslator(api_key=\'some-key\', target=\'de\', textType=\'html\']).translate(text=text)\n\n- You can pass languages by name or by abbreviation:\n\n.. code-block:: python\n\n    translated = MicrosoftTranslator(api_key=\'some-key\', target=\'german\').translate(text=text)\n\n    # Alternatively, you can pass languages by their abbreviation:\n    translated = MicrosoftTranslator(api_key=\'some-key\', target=\'de\').translate(text=text)\n\n- Translate batch of texts\n\n.. code-block:: python\n\n    texts = ["hallo welt", "guten morgen"]\n    translated = MicrosoftTranslator(api_key=\'some-key\', target=\'english\').translate_batch(texts)\n\n- Translate from a file:\n\n.. code-block:: python\n\n    translated = MicrosoftTranslator(api_key=\'some-key\', target=\'german\').translate_file(\'path/to/file\')\n\n\nPapago Translator\n---------------------\n\n.. note::\n\n    You need to require a **client id** and **client secret key** if you want to use the papago translator.\n    Visit the official website for more information about how to get one.\n\n.. code-block:: python\n\n    text = \'happy coding\'\n    translated = PapagoTranslator(client_id=\'your_client_id\', secret_key=\'your_secret_key\', source=\'en\', target=\'ko\').translate(text=text)  # output: 행복한 부호화\n\n\nLibre Translator\n---------------------\n\n.. note::\n\n    Libre translate has multiple  `mirrors <https://github.com/LibreTranslate/LibreTranslate#mirrors>`_ which can be used for the API endpoint.\n    Some require an API key to be used. By default the base url is set to `libretranslate.de <https://libretranslate.de/>`_ .\n    This can be set using the "base_url" input parameter.\n\n.. code-block:: python\n\n    text = \'laufen\'\n    translated = LibreTranslator(source=\'auto\', target=\'en\', base_url = \'https://libretranslate.com/\', api_key = \'your_api_key\').translate(text=text)  # output: run\n\n\n- You can pass languages by name or by abbreviation:\n\n.. code-block:: python\n\n    translated = LibreTranslator(source=\'german\', target=\'english\').translate(text=text)\n\n    # Alternatively, you can pass languages by their abbreviation:\n    translated = LibreTranslator(source=\'de\', target=\'en\').translate(text=text)\n\n\n- Translate batch of texts\n\n.. code-block:: python\n\n    texts = ["hallo welt", "guten morgen"]\n    translated = LibreTranslator(source=\'auto\', target=\'en\').translate_batch(texts)\n\n- Translate from a file:\n\n.. code-block:: python\n\n    translated = LibreTranslator(source=\'auto\', target=\'en\').translate_file(\'path/to/file\')\n\n\n\nProxy usage\n-------------\n\ndeep-translator provides out of the box usage of proxies. Just define your proxies config as a dictionary\nand pass it to the corresponding translator. Below is an example using the GoogleTranslator, but this feature\ncan be used with all supported translators.\n\n.. code-block:: python\n\n    from deep_translator import GoogleTranslator\n\n    # define your proxy configs:\n    proxies_example = {\n        "https": "your https proxy",  # example: 34.195.196.27:8080\n        "http": "your http proxy if available"\n    }\n    translated = GoogleTranslator(source=\'auto\', target=\'de\', proxies=proxies_example).translate("this package is awesome")\n\n\n\n\nUsage from Terminal\n--------------------\n\nDeep-translator supports a series of command line arguments for quick and simple access to the translators directly in your console.\n\n.. note::\n\n    The program accepts ``deep-translator`` or ``dt`` as a command, feel free to substitute whichever you prefer.\n\nFor a list of available translators:\n\n.. code-block:: console\n\n    $ deep-translator list\n\nTo translate a string or line of text:\n\n.. code-block:: console\n\n    $ deep_translator google --source "english" --target "german" --text "happy coding"\n\nAlternate short option names, along with using language abbreviations:\n\n.. code-block:: console\n\n    $ deep_translator google -src "en" -tgt "de" -txt "happy coding"\n\n\nFinally, to retrieve a list of available languages for a given translator:\n\n.. code-block:: console\n\n    $ deep-translator languages google\n\n======\nTests\n======\n\nDevelopers can install the development version of deep-translator and execute unit tests to verify functionality. For more information on doing this, see `the contribution guidelines <https://deep-translator.readthedocs.io/en/latest/contributing.html/>`_\n\n========\nLinks\n========\nCheck this article on medium to know why you should use the deep-translator package and how to translate text using python.\nhttps://medium.com/@nidhalbacc/how-to-translate-text-with-python-9d203139dcf5\n\n======\nHelp\n======\n\nIf you are facing any problems, please feel free to open an issue.\nAdditionally, you can make contact with the author for further information/questions.\n\nDo you like deep-translator?\nYou can always help the development of this project by:\n\n- Following on github and/or twitter\n- Promote the project (ex: by giving it a star on github)\n- Watch the github repo for new releases\n- Tweet about the package\n- Help others with issues on github\n- Create issues and pull requests\n- Sponsor the project\n\n===========\nNext Steps\n===========\n\nTake a look in the examples folder for more :)\nContributions are always welcome.\nRead the Contribution guidelines `Here <https://deep-translator.readthedocs.io/en/latest/contributing.html/>`_\n\n==========\nCredits\n==========\n\nMany thanks to @KirillSklyarenko for his work on integrating the microsoft translator\n\n==========\nLicense\n==========\n\nMIT license\n\nCopyright (c) 2020-present, Nidhal Baccouri\n\n===========\nSwagger UI\n===========\n\ndeep-translator offers an api server for easy integration with other applications. Non python applications\ncan communicate with the api directly and leverage the features of deep-translator\n\nAccess the api here: https://deep-translator-api.azurewebsites.net/docs\n\n\n\n===========================\nThe Translator++ mobile app\n===========================\n\n.. image:: ../assets/app-icon.png\n    :width: 100\n    :alt: Icon of the app\n\nYou can download and try the app on play store https://play.google.com/store/apps/details?id=org.translator.translator&hl=en_US&gl=US\n\nAfter developing the deep-translator, I realized how cool this would be if I can use it as an app on my mobile phone.\nSure, there is google translate, pons and linguee apps etc.. but isn\'t it cooler to make an app where all these\ntranslators are integrated?\n\nLong story short, I started working on the app. I decided to use the `kivy framework <https://kivy.org/#home/>`_ since\nI wanted to code in python and to develop a cross platform app.\nI open sourced the `Translator++ app <https://github.com/nidhaloff/deep-translator-app/>`_ on my github too.\nFeel free to take a look at the code or make a pull request ;)\n\n.. note::\n    The Translator++ app is based on the deep-translator package. I just built the app to prove the capabilities\n    of the deep-translator package ;)\n\nI published the first release on google play store on 02-08-2020\n\nHere are some screenshots:\n\n- Phone\n\n.. image:: ../assets/translator1.jpg\n    :width: 30%\n    :height: 200\n    :alt: screenshot1\n.. image:: ../assets/translator2.jpg\n    :width: 30%\n    :height: 200\n    :alt: screenshot2\n.. image:: ../assets/spinner.jpg\n    :width: 30%\n    :height: 200\n    :alt: spinner\n\n- Tablet:\n\n.. image:: ../assets/hz_view.png\n    :width: 100%\n    :height: 300\n    :alt: screenshot3\n\n===========================\nWebsite & Desktop app\n===========================\n\nCurrently, there are propositions for a website and/or desktop app based on deep-translator.\nYou can follow the issue here: https://github.com/nidhaloff/deep-translator/issues/144\n',
+    'long_description': '##################\ndeep-translator\n##################\n\n.. image:: ../assets/icon.jpg\n    :width: 100\n    :align: center\n    :alt: deep-translator-icon\n\n|\n\n\n.. image:: https://img.shields.io/pypi/v/deep-translator.svg\n        :target: https://pypi.python.org/pypi/deep-translator\n.. image:: https://img.shields.io/travis/nidhaloff/deep-translator.svg\n        :target: https://github.com/nidhaloff/deep-translator/actions/workflows/build.yml\n.. image:: https://readthedocs.org/projects/deep-translator/badge/?version=latest\n        :target: https://deep-translator.readthedocs.io/en/latest/?badge=latest\n        :alt: Documentation Status\n.. image:: https://img.shields.io/pypi/l/deep-translator\n        :target: https://pypi.python.org/pypi/deep-translator\n\n.. image:: https://img.shields.io/pypi/status/deep-translator\n        :target: https://pypi.python.org/pypi/deep-translator\n\n.. image:: https://pepy.tech/badge/deep-translator\n    :target: https://pepy.tech/project/deep-translator\n\n\n.. image:: https://img.shields.io/pypi/wheel/deep-translator\n        :target: https://pypi.python.org/pypi/deep-translator\n\n.. image:: https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2FNidhalBaccouri\n        :alt: Twitter URL\n        :target: https://twitter.com/NidhalBaccouri\n\n\n=======================\nTranslation for humans\n=======================\n\nA flexible **FREE** and **UNLIMITED** tool to translate between different languages in a simple way using multiple translators.\n\n\n* Free software: MIT license\n* Documentation: https://deep-translator.readthedocs.io.\n* Swagger API: https://deep-translator-api.azurewebsites.net/docs.\n\n|\n|\n\n.. contents:: Table of Contents\n    :depth: 3\n\n|\n|\n\n\n==========\nMotivation\n==========\n\nI needed to translate a text using python. It was hard to find a simple way to do it.\nThere are other libraries that can be used for this task, but most of them\nare **buggy, not free, limited, not supported anymore or complex to use.**\n\nTherefore, I decided to build this simple tool. It is 100% free, unlimited, easy to use and provides\nsupport for all languages.\n\nBasically, my goal was to integrate support for multiple famous translators\nin this tool.\n\n======================\nWhen you should use it\n======================\n\n- If you want to translate text using python\n- If you want to translate from a file\n- If you want to get translations from many sources and not only one\n- If you want to automate translations\n- If you want to compare different translations\n- If you want to detect language automatically\n\n======================\nWhy you should use it\n======================\n\n- It\'s the only python tool that integrates many translators\n- Multi language support\n- Supports batch translation\n- High level of abstraction\n- Automatic language detection\n- Easy to use and extend\n- Support for most famous universal translators\n- Stable and maintained regularly\n- The API is very easy to use\n- Proxy integration is supported\n\n========\nFeatures\n========\n\n* Support for `google translate <https://translate.google.com/>`_\n* Support for the `microsoft translator <https://www.microsoft.com/en-us/translator//>`_ (version >= 1.3.5)\n* Support for `Pons translator <https://de.pons.com/>`_\n* Support for the `Linguee translator <https://www.linguee.com/>`_\n* Support for the `Mymemory translator <https://mymemory.translated.net/>`_\n* Support for the `Yandex translator <https://yandex.com/>`_ (version >= 1.2.1)\n* Support for the `QcriTranslator translator <https://mt.qcri.org/api/>`_ (version >= 1.2.4)\n* Support for the `DeeplTranslator translator <https://www.deepl.com/en/translator/>`_ (version >= 1.2.5)\n* Support for the `Papago translator <https://papago.naver.com/>`_ (version >= 1.4.4)\n* Support for the `Libre translator <https://libretranslate.com/>`_\n* Support for proxy usage\n* Automatic single language detection\n* Batch language detection\n* Translate directly from a text file\n* Get multiple translation for a word\n* Automate the translation of different paragraphs in different languages\n* Translate directly from terminal (version >= 1.1.0)\n\n=============\nInstallation\n=============\n\nInstall the stable release:\n\n.. code-block:: console\n\n    $ pip install -U deep-translator\n\ntake a look at the docs if you want to install from source.\n\n============\nQuick Start\n============\n\n.. code-block:: python\n\n    from deep_translator import GoogleTranslator\n    translated = GoogleTranslator(source=\'auto\', target=\'de\').translate("keep it up, you are awesome")  # output -> Weiter so, du bist großartig\n\nor using proxies:\n\n.. code-block:: python\n\n    from deep_translator import GoogleTranslator\n\n    proxies_example = {\n        "https": "34.195.196.27:8080",\n        "http": "34.195.196.27:8080"\n    }\n    translated = GoogleTranslator(source=\'auto\', target=\'de\', proxies=proxies_example).translate("keep it up, you are awesome")  # output -> Weiter so, du bist großartig\n\n\nor even directly from terminal:\n\n.. code-block:: console\n\n    $ deep-translator --source "en" --target "de" --text "hello world"\n\n    or shorter\n\n    $ dt -tg de -txt "hello world"\n\n\n=====\nUsage\n=====\n\nIn this section, demos on how to use all different integrated translators in this tool are provided.\n\n.. note::\n\n    You can always pass the languages by the name or by abbreviation.\n\n    *Example*: If you want to use english as a source or target language, you can pass **english** or **en** as an argument\n\nImports\n--------\n\n.. code-block:: python\n\n    from deep_translator import (GoogleTranslator,\n                                 MicrosoftTranslator,\n                                 PonsTranslator,\n                                 LingueeTranslator,\n                                 MyMemoryTranslator,\n                                 YandexTranslator,\n                                 PapagoTranslator,\n                                 DeeplTranslator,\n                                 QcriTranslator,\n                                 single_detection,\n                                 batch_detection)\n\n\nCheck Supported Languages\n---------------------------\n\n.. note::\n\n    You can check the supported languages of each translator by calling the\n    get_supported_languages function.\n\n.. code-block:: python\n\n    # default return type is a list\n    langs_list = GoogleTranslator().get_supported_languages()  # output: [arabic, french, english etc...]\n\n    # alternatively, you can the dictionary containing languages mapped to their abbreviation\n    langs_dict = GoogleTranslator().get_supported_languages(as_dict=True)  # output: {arabic: ar, french: fr, english:en etc...}\n\nLanguage Detection\n------------------\n\n.. note::\n\n    You can also detect language automatically. Notice that this package is free and my goal is to keep it free.\n    Therefore, you will need to get your own api_key if you want to use the language detection function.\n    I figured out you can get one for free here: https://detectlanguage.com/documentation\n\n- Single Text Detection\n\n.. code-block:: python\n\n    lang = single_detection(\'bonjour la vie\', api_key=\'your_api_key\')\n    print(lang) # output: fr\n\n- Batch Detection\n\n.. code-block:: python\n\n    lang = batch_detection([\'bonjour la vie\', \'hello world\'], api_key=\'your_api_key\')\n    print(lang) # output: [fr, en]\n\n\n\nGoogle Translate\n-----------------\n\n.. code-block:: python\n\n    text = \'happy coding\'\n\n- You can use automatic language detection to detect the source language:\n\n.. code-block:: python\n\n    translated = GoogleTranslator(source=\'auto\', target=\'de\').translate(text=text)\n\n- You can pass languages by name or by abbreviation:\n\n.. code-block:: python\n\n    translated = GoogleTranslator(source=\'auto\', target=\'german\').translate(text=text)\n\n    # Alternatively, you can pass languages by their abbreviation:\n    translated = GoogleTranslator(source=\'en\', target=\'de\').translate(text=text)\n\n- You can also reuse the Translator class and change/update its properties.\n\n(Notice that this is important for performance too, since instantiating new objects is expensive)\n\n\n.. code-block:: python\n\n    # let\'s say first you need to translate from auto to german\n    my_translator = GoogleTranslator(source=\'auto\', target=\'german\')\n    result = my_translator.translate(text=text)\n    print(f"Translation using source = {my_translator.source} and target = {my_translator.target} -> {result}")\n\n    # let\'s say later you want to reuse the class but your target is french now\n    # This is the best practice and how you should use deep-translator.\n    # Please don\'t over-instantiate translator objects without a good reason, otherwise you will run into performance issues\n    my_translator.target = \'fr\'  # this will override the target \'german\' passed previously\n    result = my_translator.translate(text=text)\n    print(f"Translation using source = {my_translator.source} and target = {my_translator.target} -> {result}")\n\n    # you can also update the source language as well\n    my_translator.source = \'en\'  # this will override the source \'auto\' passed previously\n    result = my_translator.translate(text=text)\n    print(f"Translation using source = {my_translator.source} and target = {my_translator.target} -> {result}")\n\n\n- Translate batch of texts\n\n.. code-block:: python\n\n    texts = ["hallo welt", "guten morgen"]\n\n    # the translate_sentences function is deprecated, use the translate_batch function instead\n    translated = GoogleTranslator(\'de\', \'en\').translate_batch(texts)\n\n- Translate from a file:\n\n.. code-block:: python\n\n    translated = GoogleTranslator(source=\'auto\', target=\'german\').translate_file(\'path/to/file\')\n\nMymemory Translator\n--------------------\n\n.. note::\n\n    As in google translate, you can use the automatic language detection with mymemory by using "auto" as an\n    argument for the source language. However, this feature in the mymemory translator is not so powerful as\n    in google translate.\n\n- Simple translation\n\n.. code-block:: python\n\n    text = \'Keep it up. You are awesome\'\n\n    translated = MyMemoryTranslator(source=\'auto\', target=\'french\').translate(text)\n\n- Translate batch of texts\n\n.. code-block:: python\n\n    texts = ["hallo welt", "guten morgen"]\n\n    # the translate_sentences function is deprecated, use the translate_batch function instead\n    translated = MyMemoryTranslator(\'de\', \'en\').translate_batch(texts)\n\n- Translate from file\n\n.. code-block:: python\n\n    path = "your_file.txt"\n\n    translated = MyMemoryTranslator(source=\'en\', target=\'fr\').translate_file(path)\n\n\nDeeplTranslator\n-----------------\n\n.. note::\n\n    In order to use the DeeplTranslator translator, you need to generate an api key. Deepl offers a Pro and a free API.\n    deep-translator supports both Pro and free APIs. Just check the examples below.\n    Visit https://www.deepl.com/en/docs-api/ for more information on how to generate your Deepl api key\n\n- Simple translation\n\n.. code-block:: python\n\n    text = \'Keep it up. You are awesome\'\n\n    translated = DeeplTranslator(api_key="your_api_key", source="en", target="en", use_free_api=True).translate(text)\n\n.. note::\n        deep-translator uses free deepl api by default. If you have the pro version then simply set the use_free_api to false.\n\n\n- Translate batch of texts\n\n.. code-block:: python\n\n    texts = ["hallo welt", "guten morgen"]\n\n    # the translate_sentences function is deprecated, use the translate_batch function instead\n    translated = DeeplTranslator("your_api_key").translate_batch(texts)\n\nQcriTranslator\n--------------------\n\n.. note::\n\n    In order to use the QcriTranslator translator, you need to generate a free api key. Visit https://mt.qcri.org/api/\n    for more information\n\n- Check languages\n\n.. code-block:: python\n\n    # as a property\n    print("language pairs: ", QcriTranslator("your_api_key").languages)\n\n- Check domains\n\n.. code-block:: python\n\n    # as a property\n    print("domains: ", QcriTranslator("your_api_key").domains)\n\n- Text translation\n\n.. code-block:: python\n\n    text = \'Education is great\'\n\n    translated = QcriTranslator("your_api_key").translate(source=\'en\', target=\'ar\', domain="news", text=text)\n    # output -> التعليم هو عظيم\n\n    # see docs for batch translation and more.\n\nLinguee Translator\n-------------------\n\n.. code-block:: python\n\n    word = \'good\'\n\n- Simple Translation\n\n.. code-block:: python\n\n    translated_word = LingueeTranslator(source=\'english\', target=\'french\').translate(word)\n\n- Return all synonyms or words that match\n\n.. code-block:: python\n\n    # set the argument return_all to True if you want to get all synonyms of the word to translate\n    translated_word = LingueeTranslator(source=\'english\', target=\'french\').translate(word, return_all=True)\n\n- Translate a batch of words\n\n.. code-block:: python\n\n    translated_words = LingueeTranslator(source=\'english\', target=\'french\').translate_words(["good", "awesome"])\n\nPONS Translator\n----------------\n\n.. note::\n\n    You can pass the languages by the name or by abbreviation just like\n    previous examples using GoogleTranslate\n\n.. code-block:: python\n\n    word = \'awesome\'\n\n- Simple Translation\n\n.. code-block:: python\n\n    translated_word = PonsTranslator(source=\'english\', target=\'french\').translate(word)\n\n    # pass language by their abbreviation\n    translated_word = PonsTranslator(source=\'en\', target=\'fr\').translate(word)\n\n- Return all synonyms or words that match\n\n.. code-block:: python\n\n    # set the argument return_all to True if you want to get all synonyms of the word to translate\n    translated_word = PonsTranslator(source=\'english\', target=\'french\').translate(word, return_all=True)\n\n- Translate a batch of words\n\n.. code-block:: python\n\n    translated_words = LingueeTranslator(source=\'english\', target=\'french\').translate_words(["good", "awesome"])\n\nYandex Translator\n------------------\n\n.. note::\n\n    You need to require a **private api key** if you want to use the yandex translator.\n    Visit the official website for more information about how to get one\n\n- Language detection\n\n.. code-block:: python\n\n    lang = YandexTranslator(\'your_api_key\').detect(\'Hallo, Welt\')\n    print(f"language detected: {lang}")  # output -> language detected: \'de\'\n\n- Text translation\n\n.. code-block:: python\n\n    # with auto detection | meaning provide only the target language and let yandex detect the source\n    translated = YandexTranslator(\'your_api_key\').translate(source="auto", target="en", text=\'Hallo, Welt\')\n    print(f"translated text: {translated}")  # output -> translated text: Hello world\n\n    # provide source and target language explicitly\n    translated = YandexTranslator(\'your_api_key\').translate(source="de", target="en", text=\'Hallo, Welt\')\n    print(f"translated text: {translated}")  # output -> translated text: Hello world\n\n- File translation\n\n.. code-block:: python\n\n    translated = YandexTranslator(\'your_api_key\').translate_file(source="auto", target="en", path="path_to_your_file")\n\n- Batch translation\n\n.. code-block:: python\n\n    translated = YandexTranslator(\'your_api_key\').translate_batch(source="auto", target="de", batch=["hello world", "happy coding"])\n\n\nMicrosoft Translator\n---------------------\n\n.. note::\n\n    You need to require an **api key** if you want to use the microsoft translator.\n    Visit the official website for more information about how to get one.\n    Microsoft offers a free tier 0 subscription (2 million characters per month).\n\n- Required and optional attributes\n\n    There are two required attributes, namely "api_key" (string) and "target" (string or list).\n    Attribute "source" is optional.\n    Also, Microsoft API accepts a number of other optional attributes, you can find them here:  https://docs.microsoft.com/azure/cognitive-services/translator/reference/v3-0-translate\n    You can simply add them after the required attributes, see the example.\n\n.. code-block:: python\n\n    text = \'happy coding\'\n    translated = MicrosoftTranslator(api_key=\'some-key\', target=\'de\').translate(text=text)\n    translated_two_targets = MicrosoftTranslator(api_key=\'some-key\', target=[\'de\', \'ru\']).translate(text=text)\n    translated_with_optional_attr = MicrosoftTranslator(api_key=\'some-key\', target=\'de\', textType=\'html\']).translate(text=text)\n\n- You can pass languages by name or by abbreviation:\n\n.. code-block:: python\n\n    translated = MicrosoftTranslator(api_key=\'some-key\', target=\'german\').translate(text=text)\n\n    # Alternatively, you can pass languages by their abbreviation:\n    translated = MicrosoftTranslator(api_key=\'some-key\', target=\'de\').translate(text=text)\n\n- Translate batch of texts\n\n.. code-block:: python\n\n    texts = ["hallo welt", "guten morgen"]\n    translated = MicrosoftTranslator(api_key=\'some-key\', target=\'english\').translate_batch(texts)\n\n- Translate from a file:\n\n.. code-block:: python\n\n    translated = MicrosoftTranslator(api_key=\'some-key\', target=\'german\').translate_file(\'path/to/file\')\n\n\nPapago Translator\n---------------------\n\n.. note::\n\n    You need to require a **client id** and **client secret key** if you want to use the papago translator.\n    Visit the official website for more information about how to get one.\n\n.. code-block:: python\n\n    text = \'happy coding\'\n    translated = PapagoTranslator(client_id=\'your_client_id\', secret_key=\'your_secret_key\', source=\'en\', target=\'ko\').translate(text=text)  # output: 행복한 부호화\n\n\nLibre Translator\n---------------------\n\n.. note::\n\n    Libre translate has multiple  `mirrors <https://github.com/LibreTranslate/LibreTranslate#mirrors>`_ which can be used for the API endpoint.\n    Some require an API key to be used. By default the base url is set to `libretranslate.de <https://libretranslate.de/>`_ .\n    This can be set using the "base_url" input parameter.\n\n.. code-block:: python\n\n    text = \'laufen\'\n    translated = LibreTranslator(source=\'auto\', target=\'en\', base_url = \'https://libretranslate.com/\', api_key = \'your_api_key\').translate(text=text)  # output: run\n\n\n- You can pass languages by name or by abbreviation:\n\n.. code-block:: python\n\n    translated = LibreTranslator(source=\'german\', target=\'english\').translate(text=text)\n\n    # Alternatively, you can pass languages by their abbreviation:\n    translated = LibreTranslator(source=\'de\', target=\'en\').translate(text=text)\n\n\n- Translate batch of texts\n\n.. code-block:: python\n\n    texts = ["hallo welt", "guten morgen"]\n    translated = LibreTranslator(source=\'auto\', target=\'en\').translate_batch(texts)\n\n- Translate from a file:\n\n.. code-block:: python\n\n    translated = LibreTranslator(source=\'auto\', target=\'en\').translate_file(\'path/to/file\')\n\n\n\nProxy usage\n-------------\n\ndeep-translator provides out of the box usage of proxies. Just define your proxies config as a dictionary\nand pass it to the corresponding translator. Below is an example using the GoogleTranslator, but this feature\ncan be used with all supported translators.\n\n.. code-block:: python\n\n    from deep_translator import GoogleTranslator\n\n    # define your proxy configs:\n    proxies_example = {\n        "https": "your https proxy",  # example: 34.195.196.27:8080\n        "http": "your http proxy if available"\n    }\n    translated = GoogleTranslator(source=\'auto\', target=\'de\', proxies=proxies_example).translate("this package is awesome")\n\n\n\n\nUsage from Terminal\n--------------------\n\nDeep-translator supports a series of command line arguments for quick and simple access to the translators directly in your console.\n\n.. note::\n\n    The program accepts ``deep-translator`` or ``dt`` as a command, feel free to substitute whichever you prefer.\n\nFor a list of available translators:\n\n.. code-block:: console\n\n    $ deep-translator list\n\nTo translate a string or line of text:\n\n.. code-block:: console\n\n    $ deep_translator google --source "english" --target "german" --text "happy coding"\n\nAlternate short option names, along with using language abbreviations:\n\n.. code-block:: console\n\n    $ deep_translator google -src "en" -tgt "de" -txt "happy coding"\n\n\nFinally, to retrieve a list of available languages for a given translator:\n\n.. code-block:: console\n\n    $ deep-translator languages google\n\n======\nTests\n======\n\nDevelopers can install the development version of deep-translator and execute unit tests to verify functionality. For more information on doing this, see `the contribution guidelines <https://deep-translator.readthedocs.io/en/latest/contributing.html#get-started>`_\n\n========\nLinks\n========\nCheck this article on medium to know why you should use the deep-translator package and how to translate text using python.\nhttps://medium.com/@nidhalbacc/how-to-translate-text-with-python-9d203139dcf5\n\n======\nHelp\n======\n\nIf you are facing any problems, please feel free to open an issue.\nAdditionally, you can make contact with the author for further information/questions.\n\nDo you like deep-translator?\nYou can always help the development of this project by:\n\n- Following on github and/or twitter\n- Promote the project (ex: by giving it a star on github)\n- Watch the github repo for new releases\n- Tweet about the package\n- Help others with issues on github\n- Create issues and pull requests\n- Sponsor the project\n\n===========\nNext Steps\n===========\n\nTake a look in the examples folder for more :)\nContributions are always welcome.\nRead the Contribution guidelines `Here <https://deep-translator.readthedocs.io/en/latest/contributing.html#get-started>`_\n\n==========\nCredits\n==========\n\nMany thanks to @KirillSklyarenko for his work on integrating the microsoft translator\n\n==========\nLicense\n==========\n\nMIT license\n\nCopyright (c) 2020-present, Nidhal Baccouri\n\n===========\nSwagger UI\n===========\n\ndeep-translator offers an api server for easy integration with other applications. Non python applications\ncan communicate with the api directly and leverage the features of deep-translator\n\nAccess the api here: https://deep-translator-api.azurewebsites.net/docs\n\n\n\n===========================\nThe Translator++ mobile app\n===========================\n\n.. image:: ../assets/app-icon.png\n    :width: 100\n    :alt: Icon of the app\n\nYou can download and try the app on play store https://play.google.com/store/apps/details?id=org.translator.translator&hl=en_US&gl=US\n\nAfter developing the deep-translator, I realized how cool this would be if I can use it as an app on my mobile phone.\nSure, there is google translate, pons and linguee apps etc.. but isn\'t it cooler to make an app where all these\ntranslators are integrated?\n\nLong story short, I started working on the app. I decided to use the `kivy framework <https://kivy.org/#home/>`_ since\nI wanted to code in python and to develop a cross platform app.\nI open sourced the `Translator++ app <https://github.com/nidhaloff/deep-translator-app/>`_ on my github too.\nFeel free to take a look at the code or make a pull request ;)\n\n.. note::\n    The Translator++ app is based on the deep-translator package. I just built the app to prove the capabilities\n    of the deep-translator package ;)\n\nI published the first release on google play store on 02-08-2020\n\nHere are some screenshots:\n\n- Phone\n\n.. image:: ../assets/translator1.jpg\n    :width: 30%\n    :height: 200\n    :alt: screenshot1\n.. image:: ../assets/translator2.jpg\n    :width: 30%\n    :height: 200\n    :alt: screenshot2\n.. image:: ../assets/spinner.jpg\n    :width: 30%\n    :height: 200\n    :alt: spinner\n\n- Tablet:\n\n.. image:: ../assets/hz_view.png\n    :width: 100%\n    :height: 300\n    :alt: screenshot3\n\n===========================\nWebsite & Desktop app\n===========================\n\nCurrently, there are propositions for a website and/or desktop app based on deep-translator.\nYou can follow the issue here: https://github.com/nidhaloff/deep-translator/issues/144\n',
     'author': 'Nidhal Baccouri',
     'author_email': 'nidhalbacc@gmail.com',
     'maintainer': 'Nidhal Baccouri',
     'maintainer_email': 'nidhalbacc@gmail.com',
     'url': 'https://github.com/nidhaloff/deep_translator',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `deep-translator-1.9.2/PKG-INFO` & `deep-translator-1.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep-translator
-Version: 1.9.2
+Version: 1.9.3
 Summary: A flexible free and unlimited python tool to translate between different languages in a simple way using multiple translators
 Home-page: https://github.com/nidhaloff/deep_translator
 License: MIT
 Keywords: deep_translator,deepL,DeeplTranslator,translator,translation,automation,web scraping,google translator,google translation,google trans,PONS,YANDEX,MyMemory translator,Linguee,QcriTranslator,Language,Language detection,detect language,free translation,unlimited translation,translate for free
 Author: Nidhal Baccouri
 Author-email: nidhalbacc@gmail.com
 Maintainer: Nidhal Baccouri
@@ -435,17 +435,14 @@
 
 - Simple Translation
 
 .. code-block:: python
 
     translated_word = LingueeTranslator(source='english', target='french').translate(word)
 
-    # pass language by their abbreviation
-    translated_word = LingueeTranslator(source='en', target='fr').translate(word)
-
 - Return all synonyms or words that match
 
 .. code-block:: python
 
     # set the argument return_all to True if you want to get all synonyms of the word to translate
     translated_word = LingueeTranslator(source='english', target='french').translate(word, return_all=True)
 
@@ -684,15 +681,15 @@
 
     $ deep-translator languages google
 
 ======
 Tests
 ======
 
-Developers can install the development version of deep-translator and execute unit tests to verify functionality. For more information on doing this, see `the contribution guidelines <https://deep-translator.readthedocs.io/en/latest/contributing.html/>`_
+Developers can install the development version of deep-translator and execute unit tests to verify functionality. For more information on doing this, see `the contribution guidelines <https://deep-translator.readthedocs.io/en/latest/contributing.html#get-started>`_
 
 ========
 Links
 ========
 Check this article on medium to know why you should use the deep-translator package and how to translate text using python.
 https://medium.com/@nidhalbacc/how-to-translate-text-with-python-9d203139dcf5
 
@@ -716,15 +713,15 @@
 
 ===========
 Next Steps
 ===========
 
 Take a look in the examples folder for more :)
 Contributions are always welcome.
-Read the Contribution guidelines `Here <https://deep-translator.readthedocs.io/en/latest/contributing.html/>`_
+Read the Contribution guidelines `Here <https://deep-translator.readthedocs.io/en/latest/contributing.html#get-started>`_
 
 ==========
 Credits
 ==========
 
 Many thanks to @KirillSklyarenko for his work on integrating the microsoft translator
```

