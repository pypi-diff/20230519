# Comparing `tmp/CrewCo_API-0.0.1.tar.gz` & `tmp/CrewCo_API-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CrewCo_API-0.0.1.tar", last modified: Thu May 18 17:20:29 2023, max compression
+gzip compressed data, was "CrewCo_API-0.0.3.tar", last modified: Fri May 19 04:18:12 2023, max compression
```

## Comparing `CrewCo_API-0.0.1.tar` & `CrewCo_API-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 17:20:29.875604 CrewCo_API-0.0.1/
--rw-rw-rw-   0        0        0     1083 2023-05-18 17:01:47.000000 CrewCo_API-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      611 2023-05-18 17:20:29.875604 CrewCo_API-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      105 2023-05-18 17:04:55.000000 CrewCo_API-0.0.1/README.md
--rw-rw-rw-   0        0        0      586 2023-05-18 17:19:43.000000 CrewCo_API-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-18 17:20:29.875604 CrewCo_API-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-18 17:20:29.860602 CrewCo_API-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-18 17:20:29.871604 CrewCo_API-0.0.1/src/CrewCo_API.egg-info/
--rw-rw-rw-   0        0        0      611 2023-05-18 17:20:29.000000 CrewCo_API-0.0.1/src/CrewCo_API.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-05-18 17:20:29.000000 CrewCo_API-0.0.1/src/CrewCo_API.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 17:20:29.000000 CrewCo_API-0.0.1/src/CrewCo_API.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-18 17:20:29.000000 CrewCo_API-0.0.1/src/CrewCo_API.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 17:20:29.874603 CrewCo_API-0.0.1/src/crewco_api/
--rw-rw-rw-   0        0        0        0 2023-05-18 16:30:21.000000 CrewCo_API-0.0.1/src/crewco_api/__init__.py
--rw-rw-rw-   0        0        0     2023 2023-05-18 16:21:54.000000 CrewCo_API-0.0.1/src/crewco_api/api.py
--rw-rw-rw-   0        0        0       83 2023-05-18 17:01:00.000000 CrewCo_API-0.0.1/src/crewco_api/main.py
+drwxrwxrwx   0        0        0        0 2023-05-19 04:18:12.838521 CrewCo_API-0.0.3/
+-rw-rw-rw-   0        0        0     1083 2023-05-18 17:38:59.000000 CrewCo_API-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      611 2023-05-19 04:18:12.838521 CrewCo_API-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      105 2023-05-18 17:04:55.000000 CrewCo_API-0.0.3/README.md
+-rw-rw-rw-   0        0        0      621 2023-05-19 04:17:56.000000 CrewCo_API-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 04:18:12.838521 CrewCo_API-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-19 04:18:12.816519 CrewCo_API-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-19 04:18:12.835519 CrewCo_API-0.0.3/src/CrewCo_API.egg-info/
+-rw-rw-rw-   0        0        0      611 2023-05-19 04:18:12.000000 CrewCo_API-0.0.3/src/CrewCo_API.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-05-19 04:18:12.000000 CrewCo_API-0.0.3/src/CrewCo_API.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 04:18:12.000000 CrewCo_API-0.0.3/src/CrewCo_API.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-19 04:18:12.000000 CrewCo_API-0.0.3/src/CrewCo_API.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-19 04:18:12.000000 CrewCo_API-0.0.3/src/CrewCo_API.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 04:18:12.837519 CrewCo_API-0.0.3/src/crewco_api/
+-rw-rw-rw-   0        0        0        0 2023-05-18 16:30:21.000000 CrewCo_API-0.0.3/src/crewco_api/__init__.py
+-rw-rw-rw-   0        0        0     2023 2023-05-18 16:21:54.000000 CrewCo_API-0.0.3/src/crewco_api/api.py
+-rw-rw-rw-   0        0        0       83 2023-05-18 17:01:00.000000 CrewCo_API-0.0.3/src/crewco_api/main.py
```

### Comparing `CrewCo_API-0.0.1/LICENSE` & `CrewCo_API-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CrewCo_API-0.0.1/PKG-INFO` & `CrewCo_API-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CrewCo_API
-Version: 0.0.1
+Version: 0.0.3
 Summary: CrewCo's beta API
 Author-email: CrewCo <crewco.99@gmail.com>
 Project-URL: Homepage, https://github.com/Crew-co/CrewCo_API/
 Project-URL: Bug Tracker, https://github.com/Crew-co/CrewCo_API//issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `CrewCo_API-0.0.1/pyproject.toml` & `CrewCo_API-0.0.3/src/CrewCo_API.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-[project]
-name = "CrewCo_API"
-version = "0.0.1"
-authors = [
-  { name="CrewCo", email="crewco.99@gmail.com" },
-]
-description = "CrewCo's beta API"
-readme = "README.md"
-requires-python = ">=3.9"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
+Metadata-Version: 2.1
+Name: CrewCo-API
+Version: 0.0.3
+Summary: CrewCo's beta API
+Author-email: CrewCo <crewco.99@gmail.com>
+Project-URL: Homepage, https://github.com/Crew-co/CrewCo_API/
+Project-URL: Bug Tracker, https://github.com/Crew-co/CrewCo_API//issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-[project.urls]
-"Homepage" = "https://github.com/Crew-co/CrewCo_API/"
-"Bug Tracker" = "https://github.com/Crew-co/CrewCo_API//issues"
+# CrewCo API
 
-
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
+You can use
+[CrewCo-API](https://github.com/Crew-co/CrewCo_API/)
+to write your content.
```

### Comparing `CrewCo_API-0.0.1/src/crewco_api/api.py` & `CrewCo_API-0.0.3/src/crewco_api/api.py`

 * *Files identical despite different names*

