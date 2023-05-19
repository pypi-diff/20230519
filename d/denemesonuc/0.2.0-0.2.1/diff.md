# Comparing `tmp/denemesonuc-0.2.0.tar.gz` & `tmp/denemesonuc-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denemesonuc-0.2.0.tar", max compression
+gzip compressed data, was "denemesonuc-0.2.1.tar", max compression
```

## Comparing `denemesonuc-0.2.0.tar` & `denemesonuc-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-05-19 10:54:38.141023 denemesonuc-0.2.0/LICENSE
--rw-r--r--   0        0        0       67 2023-05-19 10:54:38.141023 denemesonuc-0.2.0/README.md
--rw-r--r--   0        0        0     2366 2023-05-19 10:54:38.141023 denemesonuc-0.2.0/denemesonuc/__init__.py
--rw-r--r--   0        0        0     6370 2023-05-19 10:54:38.141023 denemesonuc-0.2.0/denemesonuc/fetchers/karnemiz.py
--rw-r--r--   0        0        0     7544 2023-05-19 10:54:38.141023 denemesonuc-0.2.0/denemesonuc/fetchers/okulizyon.py
--rw-r--r--   0        0        0     6835 2023-05-19 10:54:38.141023 denemesonuc-0.2.0/denemesonuc/models.py
--rw-r--r--   0        0        0      315 2023-05-19 10:54:38.141023 denemesonuc-0.2.0/denemesonuc/utils.py
--rw-r--r--   0        0        0      713 2023-05-19 10:54:38.141023 denemesonuc-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 denemesonuc-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-19 16:32:21.848325 denemesonuc-0.2.1/LICENSE
+-rw-r--r--   0        0        0       67 2023-05-19 16:32:21.848325 denemesonuc-0.2.1/README.md
+-rw-r--r--   0        0        0     2366 2023-05-19 16:32:21.848325 denemesonuc-0.2.1/denemesonuc/__init__.py
+-rw-r--r--   0        0        0     6370 2023-05-19 16:32:21.848325 denemesonuc-0.2.1/denemesonuc/fetchers/karnemiz.py
+-rw-r--r--   0        0        0     7544 2023-05-19 16:32:21.848325 denemesonuc-0.2.1/denemesonuc/fetchers/okulizyon.py
+-rw-r--r--   0        0        0     6877 2023-05-19 16:32:21.848325 denemesonuc-0.2.1/denemesonuc/models.py
+-rw-r--r--   0        0        0      315 2023-05-19 16:32:21.848325 denemesonuc-0.2.1/denemesonuc/utils.py
+-rw-r--r--   0        0        0      713 2023-05-19 16:32:21.848325 denemesonuc-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 denemesonuc-0.2.1/PKG-INFO
```

### Comparing `denemesonuc-0.2.0/LICENSE` & `denemesonuc-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `denemesonuc-0.2.0/denemesonuc/__init__.py` & `denemesonuc-0.2.1/denemesonuc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Denemesonuc: A package for `orbim ölçme değerlendirme` thing.
 
 This package contains tools for fetching and processing deneme results from \
     remote web servers which their frontend is based on `orbim ölçme \
     değerlendirme` thing.
 """
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 from selenium.webdriver.remote.webdriver import WebDriver as __WebDriver
 
 from denemesonuc.models import Denek as __Denek
 
 
 def fetch_deneme(
```

### Comparing `denemesonuc-0.2.0/denemesonuc/fetchers/karnemiz.py` & `denemesonuc-0.2.1/denemesonuc/fetchers/karnemiz.py`

 * *Files identical despite different names*

### Comparing `denemesonuc-0.2.0/denemesonuc/fetchers/okulizyon.py` & `denemesonuc-0.2.1/denemesonuc/fetchers/okulizyon.py`

 * *Files identical despite different names*

### Comparing `denemesonuc-0.2.0/denemesonuc/models.py` & `denemesonuc-0.2.1/denemesonuc/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,17 @@
     grade: str = field(init=False)
     """Grade of the denek"""
 
     def __post_init__(self, grade_):
         """Post init method."""
         if isinstance(grade_, int):
             self.grade = str(grade_) + ".Sınıf"
-        elif not isinstance(grade_, str):
+        elif isinstance(grade_, str):
+            self.grade = grade_
+        else:
             raise TypeError(f"grade must be str or int, not {type(grade_).__name__}")
 
     def add_report(self, report: Report) -> None:
         """Add a report to the denek.
 
         Args:
             report: Report to add.
```

### Comparing `denemesonuc-0.2.0/pyproject.toml` & `denemesonuc-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "denemesonuc"
-version = "0.2.0"
+version = "0.2.1"
 description = "orbim ölçme değerlendirme şeyi için bir modül"
 authors = ["insanolanbiri <erenakgun2007@hotmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com:/insanolanbiri/denemesonuc"
 classifiers = [
     "Operating System :: OS Independent",
```

### Comparing `denemesonuc-0.2.0/PKG-INFO` & `denemesonuc-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denemesonuc
-Version: 0.2.0
+Version: 0.2.1
 Summary: orbim ölçme değerlendirme şeyi için bir modül
 Home-page: https://github.com:/insanolanbiri/denemesonuc
 License: GPL-3.0-only
 Author: insanolanbiri
 Author-email: erenakgun2007@hotmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

