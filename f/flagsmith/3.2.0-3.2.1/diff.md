# Comparing `tmp/flagsmith-3.2.0.tar.gz` & `tmp/flagsmith-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flagsmith-3.2.0.tar", max compression
+gzip compressed data, was "flagsmith-3.2.1.tar", max compression
```

## Comparing `flagsmith-3.2.0.tar` & `flagsmith-3.2.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1476 2023-01-13 10:18:16.559466 flagsmith-3.2.0/LICENSE
--rw-r--r--   0        0        0     1116 2023-01-13 10:18:16.559466 flagsmith-3.2.0/Readme.md
--rw-r--r--   0        0        0       41 2023-01-13 10:18:16.559466 flagsmith-3.2.0/flagsmith/__init__.py
--rw-r--r--   0        0        0     2008 2023-01-13 10:18:16.559466 flagsmith-3.2.0/flagsmith/analytics.py
--rw-r--r--   0        0        0      106 2023-01-13 10:18:16.559466 flagsmith-3.2.0/flagsmith/exceptions.py
--rw-r--r--   0        0        0    11054 2023-01-13 10:18:16.559466 flagsmith-3.2.0/flagsmith/flagsmith.py
--rw-r--r--   0        0        0     4633 2023-01-13 10:18:16.559466 flagsmith-3.2.0/flagsmith/models.py
--rw-r--r--   0        0        0      758 2023-01-13 10:18:16.559466 flagsmith-3.2.0/flagsmith/polling_manager.py
--rw-r--r--   0        0        0        0 2023-01-13 10:18:16.559466 flagsmith-3.2.0/flagsmith/utils/__init__.py
--rw-r--r--   0        0        0      204 2023-01-13 10:18:16.559466 flagsmith-3.2.0/flagsmith/utils/identities.py
--rw-r--r--   0        0        0      724 2023-01-13 10:18:16.559466 flagsmith-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 flagsmith-3.2.0/setup.py
--rw-r--r--   0        0        0     1933 1970-01-01 00:00:00.000000 flagsmith-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1476 2023-05-19 09:21:37.241623 flagsmith-3.2.1/LICENSE
+-rw-r--r--   0        0        0     1118 2023-05-19 09:21:37.241623 flagsmith-3.2.1/Readme.md
+-rw-r--r--   0        0        0       41 2023-05-19 09:21:37.241623 flagsmith-3.2.1/flagsmith/__init__.py
+-rw-r--r--   0        0        0     2008 2023-05-19 09:21:37.241623 flagsmith-3.2.1/flagsmith/analytics.py
+-rw-r--r--   0        0        0      106 2023-05-19 09:21:37.241623 flagsmith-3.2.1/flagsmith/exceptions.py
+-rw-r--r--   0        0        0    11054 2023-05-19 09:21:37.241623 flagsmith-3.2.1/flagsmith/flagsmith.py
+-rw-r--r--   0        0        0     4633 2023-05-19 09:21:37.241623 flagsmith-3.2.1/flagsmith/models.py
+-rw-r--r--   0        0        0      758 2023-05-19 09:21:37.241623 flagsmith-3.2.1/flagsmith/polling_manager.py
+-rw-r--r--   0        0        0        0 2023-05-19 09:21:37.241623 flagsmith-3.2.1/flagsmith/utils/__init__.py
+-rw-r--r--   0        0        0      204 2023-05-19 09:21:37.241623 flagsmith-3.2.1/flagsmith/utils/identities.py
+-rw-r--r--   0        0        0      724 2023-05-19 09:21:37.245623 flagsmith-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1935 1970-01-01 00:00:00.000000 flagsmith-3.2.1/PKG-INFO
```

### Comparing `flagsmith-3.2.0/LICENSE` & `flagsmith-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flagsmith-3.2.0/Readme.md` & `flagsmith-3.2.1/Readme.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 <img width="100%" src="https://github.com/Flagsmith/flagsmith/raw/main/static-files/hero.png"/>
 
 # Flagsmith Python SDK
 
-> Flagsmith allows you to manage feature flags and remote config across multiple projects, environments and organisations.
+> Flagsmith allows you to manage feature flags and remote config across multiple projects, environments and
+> organisations.
 
 The SDK for Python applications for [https://www.flagsmith.com/](https://www.flagsmith.com/).
 
 ## Adding to your project
 
-For full documentation visit [https://docs.flagsmith.com/clients/server-side](https://docs.flagsmith.com/clients/server-side).
+For full documentation visit
+[https://docs.flagsmith.com/clients/server-side](https://docs.flagsmith.com/clients/server-side).
 
 ## Contributing
 
-Please read [CONTRIBUTING.md](https://gist.github.com/kyle-ssg/c36a03aebe492e45cbd3eefb21cb0486) for details on our code of conduct, and the process for submitting pull requests
+Please read [CONTRIBUTING.md](https://gist.github.com/kyle-ssg/c36a03aebe492e45cbd3eefb21cb0486) for details on our code
+of conduct, and the process for submitting pull requests
 
 ## Getting Help
 
-If you encounter a bug or feature request we would like to hear about it. Before you submit an issue please search existing issues in order to prevent duplicates.
+If you encounter a bug or feature request we would like to hear about it. Before you submit an issue please search
+existing issues in order to prevent duplicates.
 
 ## Get in touch
 
-If you have any questions about our projects you can email <a href="mailto:support@flagsmith.com">support@flagsmith.com</a>.
+If you have any questions about our projects you can email
+<a href="mailto:support@flagsmith.com">support@flagsmith.com</a>.
 
 ## Useful links
 
 [Website](https://www.flagsmith.com/)
 
 [Documentation](https://docs.flagsmith.com/)
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 [https://github.com/Flagsmith/flagsmith/raw/main/static-files/hero.png] #
 Flagsmith Python SDK > Flagsmith allows you to manage feature flags and remote
-config across multiple projects, environments and organisations. The SDK for
+config across multiple projects, environments and > organisations. The SDK for
 Python applications for [https://www.flagsmith.com/](https://www.flagsmith.com/
 ). ## Adding to your project For full documentation visit [https://
 docs.flagsmith.com/clients/server-side](https://docs.flagsmith.com/clients/
 server-side). ## Contributing Please read [CONTRIBUTING.md](https://
 gist.github.com/kyle-ssg/c36a03aebe492e45cbd3eefb21cb0486) for details on our
 code of conduct, and the process for submitting pull requests ## Getting Help
 If you encounter a bug or feature request we would like to hear about it.
```

### Comparing `flagsmith-3.2.0/flagsmith/analytics.py` & `flagsmith-3.2.1/flagsmith/analytics.py`

 * *Files identical despite different names*

### Comparing `flagsmith-3.2.0/flagsmith/flagsmith.py` & `flagsmith-3.2.1/flagsmith/flagsmith.py`

 * *Files identical despite different names*

### Comparing `flagsmith-3.2.0/flagsmith/models.py` & `flagsmith-3.2.1/flagsmith/models.py`

 * *Files identical despite different names*

### Comparing `flagsmith-3.2.0/flagsmith/polling_manager.py` & `flagsmith-3.2.1/flagsmith/polling_manager.py`

 * *Files identical despite different names*

### Comparing `flagsmith-3.2.0/pyproject.toml` & `flagsmith-3.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flagsmith"
-version = "3.2.0"
+version = "3.2.1"
 description = "Flagsmith Python SDK"
 authors = ["Flagsmith <support@flagsmith.com>"]
 license = "BSD3"
 readme = "Readme.md"
 keywords = ["feature", "flag", "flagsmith", "remote", "config"]
 documentation = "https://docs.flagsmith.com"
 packages = [
```

### Comparing `flagsmith-3.2.0/PKG-INFO` & `flagsmith-3.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flagsmith
-Version: 3.2.0
+Version: 3.2.1
 Summary: Flagsmith Python SDK
 License: BSD3
 Keywords: feature,flag,flagsmith,remote,config
 Author: Flagsmith
 Author-email: support@flagsmith.com
 Requires-Python: >=3.7.0,<4
 Classifier: License :: Other/Proprietary License
@@ -20,33 +20,38 @@
 Project-URL: Documentation, https://docs.flagsmith.com
 Description-Content-Type: text/markdown
 
 <img width="100%" src="https://github.com/Flagsmith/flagsmith/raw/main/static-files/hero.png"/>
 
 # Flagsmith Python SDK
 
-> Flagsmith allows you to manage feature flags and remote config across multiple projects, environments and organisations.
+> Flagsmith allows you to manage feature flags and remote config across multiple projects, environments and
+> organisations.
 
 The SDK for Python applications for [https://www.flagsmith.com/](https://www.flagsmith.com/).
 
 ## Adding to your project
 
-For full documentation visit [https://docs.flagsmith.com/clients/server-side](https://docs.flagsmith.com/clients/server-side).
+For full documentation visit
+[https://docs.flagsmith.com/clients/server-side](https://docs.flagsmith.com/clients/server-side).
 
 ## Contributing
 
-Please read [CONTRIBUTING.md](https://gist.github.com/kyle-ssg/c36a03aebe492e45cbd3eefb21cb0486) for details on our code of conduct, and the process for submitting pull requests
+Please read [CONTRIBUTING.md](https://gist.github.com/kyle-ssg/c36a03aebe492e45cbd3eefb21cb0486) for details on our code
+of conduct, and the process for submitting pull requests
 
 ## Getting Help
 
-If you encounter a bug or feature request we would like to hear about it. Before you submit an issue please search existing issues in order to prevent duplicates.
+If you encounter a bug or feature request we would like to hear about it. Before you submit an issue please search
+existing issues in order to prevent duplicates.
 
 ## Get in touch
 
-If you have any questions about our projects you can email <a href="mailto:support@flagsmith.com">support@flagsmith.com</a>.
+If you have any questions about our projects you can email
+<a href="mailto:support@flagsmith.com">support@flagsmith.com</a>.
 
 ## Useful links
 
 [Website](https://www.flagsmith.com/)
 
 [Documentation](https://docs.flagsmith.com/)
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: flagsmith Version: 3.2.0 Summary: Flagsmith Python
+Metadata-Version: 2.1 Name: flagsmith Version: 3.2.1 Summary: Flagsmith Python
 SDK License: BSD3 Keywords: feature,flag,flagsmith,remote,config Author:
 Flagsmith Author-email: support@flagsmith.com Requires-Python: >=3.7.0,<4
 Classifier: License :: Other/Proprietary License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: flagsmith-
 flag-engine (>=2.3.0,<3.0.0) Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: requests-futures (>=1.0.0,<2.0.0) Project-URL: Documentation,
 https://docs.flagsmith.com Description-Content-Type: text/markdown [https://
 github.com/Flagsmith/flagsmith/raw/main/static-files/hero.png] # Flagsmith
 Python SDK > Flagsmith allows you to manage feature flags and remote config
-across multiple projects, environments and organisations. The SDK for Python
+across multiple projects, environments and > organisations. The SDK for Python
 applications for [https://www.flagsmith.com/](https://www.flagsmith.com/). ##
 Adding to your project For full documentation visit [https://
 docs.flagsmith.com/clients/server-side](https://docs.flagsmith.com/clients/
 server-side). ## Contributing Please read [CONTRIBUTING.md](https://
 gist.github.com/kyle-ssg/c36a03aebe492e45cbd3eefb21cb0486) for details on our
 code of conduct, and the process for submitting pull requests ## Getting Help
 If you encounter a bug or feature request we would like to hear about it.
```

