# Comparing `tmp/CrewCo_API-0.0.3.tar.gz` & `tmp/CrewCo_API-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CrewCo_API-0.0.3.tar", last modified: Fri May 19 04:18:12 2023, max compression
+gzip compressed data, was "CrewCo_API-0.0.4.tar", last modified: Fri May 19 05:18:05 2023, max compression
```

## Comparing `CrewCo_API-0.0.3.tar` & `CrewCo_API-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 04:18:12.838521 CrewCo_API-0.0.3/
--rw-rw-rw-   0        0        0     1083 2023-05-18 17:38:59.000000 CrewCo_API-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      611 2023-05-19 04:18:12.838521 CrewCo_API-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      105 2023-05-18 17:04:55.000000 CrewCo_API-0.0.3/README.md
--rw-rw-rw-   0        0        0      621 2023-05-19 04:17:56.000000 CrewCo_API-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 04:18:12.838521 CrewCo_API-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-19 04:18:12.816519 CrewCo_API-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-19 04:18:12.835519 CrewCo_API-0.0.3/src/CrewCo_API.egg-info/
--rw-rw-rw-   0        0        0      611 2023-05-19 04:18:12.000000 CrewCo_API-0.0.3/src/CrewCo_API.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-05-19 04:18:12.000000 CrewCo_API-0.0.3/src/CrewCo_API.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 04:18:12.000000 CrewCo_API-0.0.3/src/CrewCo_API.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-19 04:18:12.000000 CrewCo_API-0.0.3/src/CrewCo_API.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-19 04:18:12.000000 CrewCo_API-0.0.3/src/CrewCo_API.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-19 04:18:12.837519 CrewCo_API-0.0.3/src/crewco_api/
--rw-rw-rw-   0        0        0        0 2023-05-18 16:30:21.000000 CrewCo_API-0.0.3/src/crewco_api/__init__.py
--rw-rw-rw-   0        0        0     2023 2023-05-18 16:21:54.000000 CrewCo_API-0.0.3/src/crewco_api/api.py
--rw-rw-rw-   0        0        0       83 2023-05-18 17:01:00.000000 CrewCo_API-0.0.3/src/crewco_api/main.py
+drwxrwxrwx   0        0        0        0 2023-05-19 05:18:05.512816 CrewCo_API-0.0.4/
+-rw-rw-rw-   0        0        0     1083 2023-05-18 17:38:59.000000 CrewCo_API-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      611 2023-05-19 05:18:05.512816 CrewCo_API-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      105 2023-05-18 17:04:55.000000 CrewCo_API-0.0.4/README.md
+-rw-rw-rw-   0        0        0      632 2023-05-19 05:17:49.000000 CrewCo_API-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 05:18:05.512816 CrewCo_API-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-19 05:18:05.476815 CrewCo_API-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-19 05:18:05.496814 CrewCo_API-0.0.4/src/CrewCo_API.egg-info/
+-rw-rw-rw-   0        0        0      611 2023-05-19 05:18:05.000000 CrewCo_API-0.0.4/src/CrewCo_API.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-05-19 05:18:05.000000 CrewCo_API-0.0.4/src/CrewCo_API.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 05:18:05.000000 CrewCo_API-0.0.4/src/CrewCo_API.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-19 05:18:05.000000 CrewCo_API-0.0.4/src/CrewCo_API.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-19 05:18:05.000000 CrewCo_API-0.0.4/src/CrewCo_API.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 05:18:05.511814 CrewCo_API-0.0.4/src/crewco_api/
+-rw-rw-rw-   0        0        0        0 2023-05-18 16:30:21.000000 CrewCo_API-0.0.4/src/crewco_api/__init__.py
+-rw-rw-rw-   0        0        0     3145 2023-05-19 05:08:04.000000 CrewCo_API-0.0.4/src/crewco_api/api.py
+-rw-rw-rw-   0        0        0        2 2023-05-19 05:17:21.000000 CrewCo_API-0.0.4/src/crewco_api/main.py
```

### Comparing `CrewCo_API-0.0.3/LICENSE` & `CrewCo_API-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CrewCo_API-0.0.3/PKG-INFO` & `CrewCo_API-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CrewCo_API
-Version: 0.0.3
+Version: 0.0.4
 Summary: CrewCo's beta API
 Author-email: CrewCo <crewco.99@gmail.com>
 Project-URL: Homepage, https://github.com/Crew-co/CrewCo_API/
 Project-URL: Bug Tracker, https://github.com/Crew-co/CrewCo_API//issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `CrewCo_API-0.0.3/pyproject.toml` & `CrewCo_API-0.0.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = "CrewCo_API"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="CrewCo", email="crewco.99@gmail.com" },
 ]
 description = "CrewCo's beta API"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
-dependencies = ["pycryptodome"]
+dependencies = ["pycryptodome","requests"]
 
 [project.urls]
 "Homepage" = "https://github.com/Crew-co/CrewCo_API/"
 "Bug Tracker" = "https://github.com/Crew-co/CrewCo_API//issues"
 
 
 [build-system]
```

### Comparing `CrewCo_API-0.0.3/src/CrewCo_API.egg-info/PKG-INFO` & `CrewCo_API-0.0.4/src/CrewCo_API.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CrewCo-API
-Version: 0.0.3
+Version: 0.0.4
 Summary: CrewCo's beta API
 Author-email: CrewCo <crewco.99@gmail.com>
 Project-URL: Homepage, https://github.com/Crew-co/CrewCo_API/
 Project-URL: Bug Tracker, https://github.com/Crew-co/CrewCo_API//issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

