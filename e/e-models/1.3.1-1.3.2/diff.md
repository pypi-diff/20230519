# Comparing `tmp/e-models-1.3.1.tar.gz` & `tmp/e-models-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-models-1.3.1.tar", last modified: Tue May  9 19:12:45 2023, max compression
+gzip compressed data, was "e-models-1.3.2.tar", last modified: Fri May 19 18:49:17 2023, max compression
```

## Comparing `e-models-1.3.1.tar` & `e-models-1.3.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-09 19:12:45.085422 e-models-1.3.1/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.3.1/LICENSE
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3270 2023-05-09 19:12:45.085422 e-models-1.3.1/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2730 2023-04-19 14:03:12.000000 e-models-1.3.1/README.md
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-09 19:12:45.081422 e-models-1.3.1/e_models.egg-info/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3270 2023-05-09 19:12:45.000000 e-models-1.3.1/e_models.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      471 2023-05-09 19:12:45.000000 e-models-1.3.1/e_models.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-05-09 19:12:45.000000 e-models-1.3.1/e_models.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        7 2023-05-09 19:12:45.000000 e-models-1.3.1/e_models.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-05-09 19:12:45.000000 e-models-1.3.1/e_models.egg-info/top_level.txt
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-09 19:12:45.085422 e-models-1.3.1/emodels/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       22 2023-05-09 19:11:57.000000 e-models-1.3.1/emodels/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-05-04 18:51:26.000000 e-models-1.3.1/emodels/config.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-09 19:12:45.085422 e-models-1.3.1/emodels/html2text/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    34895 2023-05-04 18:51:26.000000 e-models-1.3.1/emodels/html2text/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.3.1/emodels/html2text/config.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.3.1/emodels/html2text/elements.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.3.1/emodels/html2text/typing.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.3.1/emodels/html2text/utils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.3.1/emodels/py.typed
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6744 2023-05-09 19:10:30.000000 e-models-1.3.1/emodels/scrapyutils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.3.1/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-05-09 19:12:45.085422 e-models-1.3.1/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      907 2023-05-09 19:12:04.000000 e-models-1.3.1/setup.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-09 19:12:45.085422 e-models-1.3.1/tests/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3181 2023-05-04 18:49:39.000000 e-models-1.3.1/tests/test_html2text.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7435 2023-05-04 18:49:39.000000 e-models-1.3.1/tests/test_scrapyutils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-19 18:49:17.846984 e-models-1.3.2/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.3.2/LICENSE
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3270 2023-05-19 18:49:17.846984 e-models-1.3.2/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2730 2023-04-19 14:03:12.000000 e-models-1.3.2/README.md
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-19 18:49:17.842984 e-models-1.3.2/e_models.egg-info/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3270 2023-05-19 18:49:17.000000 e-models-1.3.2/e_models.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      471 2023-05-19 18:49:17.000000 e-models-1.3.2/e_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-05-19 18:49:17.000000 e-models-1.3.2/e_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        7 2023-05-19 18:49:17.000000 e-models-1.3.2/e_models.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-05-19 18:49:17.000000 e-models-1.3.2/e_models.egg-info/top_level.txt
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-19 18:49:17.846984 e-models-1.3.2/emodels/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       22 2023-05-19 18:48:44.000000 e-models-1.3.2/emodels/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-05-04 18:51:26.000000 e-models-1.3.2/emodels/config.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-19 18:49:17.846984 e-models-1.3.2/emodels/html2text/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    34290 2023-05-19 18:47:14.000000 e-models-1.3.2/emodels/html2text/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.3.2/emodels/html2text/config.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.3.2/emodels/html2text/elements.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.3.2/emodels/html2text/typing.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.3.2/emodels/html2text/utils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.3.2/emodels/py.typed
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6744 2023-05-19 17:09:55.000000 e-models-1.3.2/emodels/scrapyutils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.3.2/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-05-19 18:49:17.846984 e-models-1.3.2/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      907 2023-05-19 18:48:49.000000 e-models-1.3.2/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-19 18:49:17.846984 e-models-1.3.2/tests/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3915 2023-05-19 18:19:41.000000 e-models-1.3.2/tests/test_html2text.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7435 2023-05-04 18:49:39.000000 e-models-1.3.2/tests/test_scrapyutils.py
```

### Comparing `e-models-1.3.1/LICENSE` & `e-models-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `e-models-1.3.1/PKG-INFO` & `e-models-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.3.1
+Version: 1.3.2
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.3.1/README.md` & `e-models-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `e-models-1.3.1/e_models.egg-info/PKG-INFO` & `e-models-1.3.2/e_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.3.1
+Version: 1.3.2
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.3.1/emodels/html2text/__init__.py` & `e-models-1.3.2/emodels/html2text/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """html2text: Turn HTML into equivalent Markdown-structured text."""
 
 import html.entities
 import html.parser
+from html import unescape as html_unescape
 import re
 import urllib.parse as urlparse
 from textwrap import wrap
 from typing import Dict, List, Optional, Tuple, Union
+from unicodedata import normalize as unormalize
 
 from . import config
 from .elements import AnchorElement, ListElement
 from .typing import OutCallback
 from .utils import (
     dumb_css_parser,
     element_style,
@@ -177,24 +179,17 @@
 
         return outtext
 
     def handle_charref(self, c: str) -> None:
         self.handle_data(self.charref(c), True)
 
     def handle_entityref(self, c: str) -> None:
-        ref = self.entityref(c)
-
-        # ref may be an empty string (e.g. for &lrm;/&rlm; markers that should
-        # not contribute to the final output).
-        # self.handle_data cannot handle a zero-length string right after a
-        # stressed tag or mid-text within a stressed tag (text get split and
-        # self.stressed/self.preceding_stressed gets switched after the first
-        # part of that text).
-        if ref:
-            self.handle_data(ref, True)
+        result = unormalize("NFKC", html_unescape("&" + c))
+        if result:
+            return self.handle_data(result, True)
 
     def handle_starttag(self, tag: str, attrs: List[Tuple[str, Optional[str]]]) -> None:
         attrid = dict(attrs).get("itemprop", "")
         if not attrid:
             attrid = dict(attrs).get("id", "")
         self.current_id.append(attrid)
 
@@ -704,15 +699,14 @@
                     data = lstripped_data
                 if lstripped_data != "":
                     self.drop_white_space = 0
 
             if puredata and not self.pre:
                 # This is a very dangerous call ... it could mess up
                 # all handling of &nbsp; when not handled properly
-                # (see entityref)
                 data = re.sub(r"\s+", r" ", data)
                 if data and data[0] == " ":
                     self.space = True
                     data = data[1:]
             if not data and not force:
                 return
 
@@ -852,23 +846,14 @@
             return unifiable_n[c]
         else:
             try:
                 return chr(c)
             except ValueError:  # invalid unicode
                 return ""
 
-    def entityref(self, c: str) -> str:
-        if not self.unicode_snob and c in config.UNIFIABLE:
-            return config.UNIFIABLE[c]
-        try:
-            ch = html.entities.html5[c + ";"]
-        except KeyError:
-            return "&" + c + ";"
-        return config.UNIFIABLE[c] if c == "nbsp" else ch
-
     def google_nest_count(self, style: Dict[str, str]) -> int:
         """
         Calculate the nesting count of google doc lists
 
         :type style: dict
 
         :rtype: int
```

### Comparing `e-models-1.3.1/emodels/html2text/config.py` & `e-models-1.3.2/emodels/html2text/config.py`

 * *Files identical despite different names*

### Comparing `e-models-1.3.1/emodels/html2text/utils.py` & `e-models-1.3.2/emodels/html2text/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.3.1/emodels/scrapyutils.py` & `e-models-1.3.2/emodels/scrapyutils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.3.1/setup.py` & `e-models-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name         = 'e-models',
-    version      = '1.3.1',
+    version      = '1.3.2',
     description  = 'Tools for helping build of extraction models with scrapy spiders.',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     license      = 'BSD',
     author       = 'Martin Olveyra',
     author_email = 'molveyra@gmail.com',
     url          = 'https://github.com/kalessin/emodels',
```

### Comparing `e-models-1.3.1/tests/test_html2text.py` & `e-models-1.3.2/tests/test_html2text.py`

 * *Files 14% similar despite different names*

```diff
@@ -107,7 +107,22 @@
 
 Data 6
 
 |
 | Data 7| Data 8|
 """
         self.assertEqual(response.markdown, expected)
+
+    def test_entities(self):
+        html = b"""<div>There&nbsp;are&nbsp;spaces</div>"""
+        response = ExtractTextResponse(url="http://example.com/example2.html", status=200, body=html)
+        self.assertEqual(response.markdown, "There are spaces\n")
+
+        html = b"""<div>There&amp;nbsp;are&amp;nbsp;spaces</div>"""
+        response = ExtractTextResponse(url="http://example.com/example2.html", status=200, body=html)
+        self.assertEqual(response.markdown, "There&nbsp;are&nbsp;spaces\n")
+
+        html = b"""<div>There&nbspare&nbspspaces</div>"""
+        response = ExtractTextResponse(url="http://example.com/example2.html", status=200, body=html)
+        self.assertEqual(response.markdown, "There are spaces\n")
+
+
```

### Comparing `e-models-1.3.1/tests/test_scrapyutils.py` & `e-models-1.3.2/tests/test_scrapyutils.py`

 * *Files identical despite different names*

