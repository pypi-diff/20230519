# Comparing `tmp/loquax-0.1.1.tar.gz` & `tmp/loquax-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loquax-0.1.1.tar", last modified: Fri May 19 19:48:07 2023, max compression
+gzip compressed data, was "loquax-0.1.2.tar", last modified: Fri May 19 19:53:40 2023, max compression
```

## Comparing `loquax-0.1.1.tar` & `loquax-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,32 @@
-drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:48:07.034247 loquax-0.1.1/
--rw-r--r--   0 matthieucourt   (501) staff       (20)    35149 2023-02-10 04:45:57.000000 loquax-0.1.1/LICENSE
--rw-r--r--   0 matthieucourt   (501) staff       (20)     2072 2023-05-19 19:48:07.033959 loquax-0.1.1/PKG-INFO
--rw-r--r--   0 matthieucourt   (501) staff       (20)     1520 2023-05-19 19:42:27.000000 loquax-0.1.1/README.md
-drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:48:07.025905 loquax-0.1.1/loquax/
--rw-r--r--   0 matthieucourt   (501) staff       (20)       44 2023-05-19 13:53:25.000000 loquax-0.1.1/loquax/__init__.py
-drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:48:07.030645 loquax-0.1.1/loquax/abstractions/
--rw-r--r--   0 matthieucourt   (501) staff       (20)      191 2023-05-19 13:53:25.000000 loquax-0.1.1/loquax/abstractions/__init__.py
--rw-r--r--   0 matthieucourt   (501) staff       (20)     1637 2023-05-19 13:53:25.000000 loquax-0.1.1/loquax/abstractions/constants.py
--rw-r--r--   0 matthieucourt   (501) staff       (20)     9211 2023-05-19 19:42:43.000000 loquax-0.1.1/loquax/abstractions/linguistic_entities.py
--rw-r--r--   0 matthieucourt   (501) staff       (20)     1080 2023-05-19 13:53:25.000000 loquax-0.1.1/loquax/abstractions/phonology.py
--rw-r--r--   0 matthieucourt   (501) staff       (20)     2526 2023-05-19 13:53:25.000000 loquax-0.1.1/loquax/abstractions/syllabification.py
-drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:48:07.031658 loquax-0.1.1/loquax/languages/
--rw-r--r--   0 matthieucourt   (501) staff       (20)       25 2023-05-19 13:53:25.000000 loquax-0.1.1/loquax/languages/__init__.py
--rw-r--r--   0 matthieucourt   (501) staff       (20)      925 2023-05-19 13:53:25.000000 loquax-0.1.1/loquax/languages/latin.py
-drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:48:07.033226 loquax-0.1.1/loquax/text_processing/
--rw-r--r--   0 matthieucourt   (501) staff       (20)      107 2023-05-19 13:53:25.000000 loquax-0.1.1/loquax/text_processing/__init__.py
--rw-r--r--   0 matthieucourt   (501) staff       (20)     1105 2023-05-19 13:53:25.000000 loquax-0.1.1/loquax/text_processing/commons.py
--rw-r--r--   0 matthieucourt   (501) staff       (20)     2758 2023-05-19 19:37:17.000000 loquax-0.1.1/loquax/text_processing/processing.py
-drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:48:07.027658 loquax-0.1.1/loquax.egg-info/
--rw-r--r--   0 matthieucourt   (501) staff       (20)     2072 2023-05-19 19:48:06.000000 loquax-0.1.1/loquax.egg-info/PKG-INFO
--rw-r--r--   0 matthieucourt   (501) staff       (20)      521 2023-05-19 19:48:06.000000 loquax-0.1.1/loquax.egg-info/SOURCES.txt
--rw-r--r--   0 matthieucourt   (501) staff       (20)        1 2023-05-19 19:48:06.000000 loquax-0.1.1/loquax.egg-info/dependency_links.txt
--rw-r--r--   0 matthieucourt   (501) staff       (20)        7 2023-05-19 19:48:06.000000 loquax-0.1.1/loquax.egg-info/top_level.txt
--rw-r--r--   0 matthieucourt   (501) staff       (20)      183 2023-05-19 13:53:25.000000 loquax-0.1.1/pyproject.toml
--rw-r--r--   0 matthieucourt   (501) staff       (20)       38 2023-05-19 19:48:07.034341 loquax-0.1.1/setup.cfg
--rw-r--r--   0 matthieucourt   (501) staff       (20)      779 2023-05-19 19:47:55.000000 loquax-0.1.1/setup.py
+drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:53:40.222721 loquax-0.1.2/
+-rw-r--r--   0 matthieucourt   (501) staff       (20)    35149 2023-02-10 04:45:57.000000 loquax-0.1.2/LICENSE
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     2072 2023-05-19 19:53:40.222286 loquax-0.1.2/PKG-INFO
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     1520 2023-05-19 19:42:27.000000 loquax-0.1.2/README.md
+drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:53:40.212501 loquax-0.1.2/loquax/
+-rw-r--r--   0 matthieucourt   (501) staff       (20)       44 2023-05-19 13:53:25.000000 loquax-0.1.2/loquax/__init__.py
+drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:53:40.217097 loquax-0.1.2/loquax/abstractions/
+-rw-r--r--   0 matthieucourt   (501) staff       (20)      191 2023-05-19 13:53:25.000000 loquax-0.1.2/loquax/abstractions/__init__.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     1637 2023-05-19 13:53:25.000000 loquax-0.1.2/loquax/abstractions/constants.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     9211 2023-05-19 19:42:43.000000 loquax-0.1.2/loquax/abstractions/linguistic_entities.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     1080 2023-05-19 13:53:25.000000 loquax-0.1.2/loquax/abstractions/phonology.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     2526 2023-05-19 13:53:25.000000 loquax-0.1.2/loquax/abstractions/syllabification.py
+drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:53:40.218335 loquax-0.1.2/loquax/languages/
+-rw-r--r--   0 matthieucourt   (501) staff       (20)       25 2023-05-19 13:53:25.000000 loquax-0.1.2/loquax/languages/__init__.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)      925 2023-05-19 13:53:25.000000 loquax-0.1.2/loquax/languages/latin.py
+drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:53:40.219851 loquax-0.1.2/loquax/languages/latin_conf/
+-rw-r--r--   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:53:03.000000 loquax-0.1.2/loquax/languages/latin_conf/__init__.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     1058 2023-05-19 13:53:25.000000 loquax-0.1.2/loquax/languages/latin_conf/constants.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     3361 2023-05-19 13:53:25.000000 loquax-0.1.2/loquax/languages/latin_conf/rules.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)      574 2023-05-19 13:53:25.000000 loquax-0.1.2/loquax/languages/latin_conf/tokenizer.py
+drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:53:40.221458 loquax-0.1.2/loquax/text_processing/
+-rw-r--r--   0 matthieucourt   (501) staff       (20)      107 2023-05-19 13:53:25.000000 loquax-0.1.2/loquax/text_processing/__init__.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     1105 2023-05-19 13:53:25.000000 loquax-0.1.2/loquax/text_processing/commons.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     2758 2023-05-19 19:37:17.000000 loquax-0.1.2/loquax/text_processing/processing.py
+drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:53:40.214518 loquax-0.1.2/loquax.egg-info/
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     2072 2023-05-19 19:53:40.000000 loquax-0.1.2/loquax.egg-info/PKG-INFO
+-rw-r--r--   0 matthieucourt   (501) staff       (20)      680 2023-05-19 19:53:40.000000 loquax-0.1.2/loquax.egg-info/SOURCES.txt
+-rw-r--r--   0 matthieucourt   (501) staff       (20)        1 2023-05-19 19:53:40.000000 loquax-0.1.2/loquax.egg-info/dependency_links.txt
+-rw-r--r--   0 matthieucourt   (501) staff       (20)        7 2023-05-19 19:53:40.000000 loquax-0.1.2/loquax.egg-info/top_level.txt
+-rw-r--r--   0 matthieucourt   (501) staff       (20)      183 2023-05-19 13:53:25.000000 loquax-0.1.2/pyproject.toml
+-rw-r--r--   0 matthieucourt   (501) staff       (20)       38 2023-05-19 19:53:40.222866 loquax-0.1.2/setup.cfg
+-rw-r--r--   0 matthieucourt   (501) staff       (20)      779 2023-05-19 19:53:33.000000 loquax-0.1.2/setup.py
```

### Comparing `loquax-0.1.1/LICENSE` & `loquax-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `loquax-0.1.1/PKG-INFO` & `loquax-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loquax
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Classical Phonology framework
 Home-page: https://github.com/mattlianje/loquax
 Author: Matthieu Court
 Author-email: matthieu.court@protonmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: loquax Version: 0.1.1 Summary: A Classical
+Metadata-Version: 2.1 Name: loquax Version: 0.1.2 Summary: A Classical
 Phonology framework Home-page: https://github.com/mattlianje/loquax Author:
 Matthieu Court Author-email: matthieu.court@protonmail.com License: UNKNOWN
 Platform: UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
 Python :: 3.10 Requires-Python: >=3.10 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `loquax-0.1.1/README.md` & `loquax-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `loquax-0.1.1/loquax/abstractions/constants.py` & `loquax-0.1.2/loquax/abstractions/constants.py`

 * *Files identical despite different names*

### Comparing `loquax-0.1.1/loquax/abstractions/linguistic_entities.py` & `loquax-0.1.2/loquax/abstractions/linguistic_entities.py`

 * *Files identical despite different names*

### Comparing `loquax-0.1.1/loquax/abstractions/phonology.py` & `loquax-0.1.2/loquax/abstractions/phonology.py`

 * *Files identical despite different names*

### Comparing `loquax-0.1.1/loquax/abstractions/syllabification.py` & `loquax-0.1.2/loquax/abstractions/syllabification.py`

 * *Files identical despite different names*

### Comparing `loquax-0.1.1/loquax/languages/latin.py` & `loquax-0.1.2/loquax/languages/latin.py`

 * *Files identical despite different names*

### Comparing `loquax-0.1.1/loquax/text_processing/commons.py` & `loquax-0.1.2/loquax/text_processing/commons.py`

 * *Files identical despite different names*

### Comparing `loquax-0.1.1/loquax/text_processing/processing.py` & `loquax-0.1.2/loquax/text_processing/processing.py`

 * *Files identical despite different names*

### Comparing `loquax-0.1.1/loquax.egg-info/PKG-INFO` & `loquax-0.1.2/loquax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loquax
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Classical Phonology framework
 Home-page: https://github.com/mattlianje/loquax
 Author: Matthieu Court
 Author-email: matthieu.court@protonmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: loquax Version: 0.1.1 Summary: A Classical
+Metadata-Version: 2.1 Name: loquax Version: 0.1.2 Summary: A Classical
 Phonology framework Home-page: https://github.com/mattlianje/loquax Author:
 Matthieu Court Author-email: matthieu.court@protonmail.com License: UNKNOWN
 Platform: UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
 Python :: 3.10 Requires-Python: >=3.10 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `loquax-0.1.1/loquax.egg-info/SOURCES.txt` & `loquax-0.1.2/loquax.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -10,10 +10,14 @@
 loquax/abstractions/__init__.py
 loquax/abstractions/constants.py
 loquax/abstractions/linguistic_entities.py
 loquax/abstractions/phonology.py
 loquax/abstractions/syllabification.py
 loquax/languages/__init__.py
 loquax/languages/latin.py
+loquax/languages/latin_conf/__init__.py
+loquax/languages/latin_conf/constants.py
+loquax/languages/latin_conf/rules.py
+loquax/languages/latin_conf/tokenizer.py
 loquax/text_processing/__init__.py
 loquax/text_processing/commons.py
 loquax/text_processing/processing.py
```

### Comparing `loquax-0.1.1/setup.py` & `loquax-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="loquax",
-    version="0.1.1",
+    version="0.1.2",
     author="Matthieu Court",
     author_email="matthieu.court@protonmail.com",
     description="A Classical Phonology framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mattlianje/loquax",
     packages=find_packages(exclude=['tests', 'tests.*']),
```

