# Comparing `tmp/CrewCo_API-0.0.4.tar.gz` & `tmp/CrewCo_API-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CrewCo_API-0.0.4.tar", last modified: Fri May 19 05:18:05 2023, max compression
+gzip compressed data, was "CrewCo_API-0.0.5.tar", last modified: Fri May 19 05:22:44 2023, max compression
```

## Comparing `CrewCo_API-0.0.4.tar` & `CrewCo_API-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 05:18:05.512816 CrewCo_API-0.0.4/
--rw-rw-rw-   0        0        0     1083 2023-05-18 17:38:59.000000 CrewCo_API-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      611 2023-05-19 05:18:05.512816 CrewCo_API-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      105 2023-05-18 17:04:55.000000 CrewCo_API-0.0.4/README.md
--rw-rw-rw-   0        0        0      632 2023-05-19 05:17:49.000000 CrewCo_API-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 05:18:05.512816 CrewCo_API-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-19 05:18:05.476815 CrewCo_API-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-19 05:18:05.496814 CrewCo_API-0.0.4/src/CrewCo_API.egg-info/
--rw-rw-rw-   0        0        0      611 2023-05-19 05:18:05.000000 CrewCo_API-0.0.4/src/CrewCo_API.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-05-19 05:18:05.000000 CrewCo_API-0.0.4/src/CrewCo_API.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 05:18:05.000000 CrewCo_API-0.0.4/src/CrewCo_API.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-19 05:18:05.000000 CrewCo_API-0.0.4/src/CrewCo_API.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-19 05:18:05.000000 CrewCo_API-0.0.4/src/CrewCo_API.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-19 05:18:05.511814 CrewCo_API-0.0.4/src/crewco_api/
--rw-rw-rw-   0        0        0        0 2023-05-18 16:30:21.000000 CrewCo_API-0.0.4/src/crewco_api/__init__.py
--rw-rw-rw-   0        0        0     3145 2023-05-19 05:08:04.000000 CrewCo_API-0.0.4/src/crewco_api/api.py
--rw-rw-rw-   0        0        0        2 2023-05-19 05:17:21.000000 CrewCo_API-0.0.4/src/crewco_api/main.py
+drwxrwxrwx   0        0        0        0 2023-05-19 05:22:44.178476 CrewCo_API-0.0.5/
+-rw-rw-rw-   0        0        0     1083 2023-05-18 17:38:59.000000 CrewCo_API-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      611 2023-05-19 05:22:44.177476 CrewCo_API-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      105 2023-05-18 17:04:55.000000 CrewCo_API-0.0.5/README.md
+-rw-rw-rw-   0        0        0      632 2023-05-19 05:22:17.000000 CrewCo_API-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 05:22:44.178476 CrewCo_API-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-19 05:22:44.145475 CrewCo_API-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-19 05:22:44.174475 CrewCo_API-0.0.5/src/CrewCo_API.egg-info/
+-rw-rw-rw-   0        0        0      611 2023-05-19 05:22:44.000000 CrewCo_API-0.0.5/src/CrewCo_API.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-05-19 05:22:44.000000 CrewCo_API-0.0.5/src/CrewCo_API.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 05:22:44.000000 CrewCo_API-0.0.5/src/CrewCo_API.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-19 05:22:44.000000 CrewCo_API-0.0.5/src/CrewCo_API.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-19 05:22:44.000000 CrewCo_API-0.0.5/src/CrewCo_API.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 05:22:44.177476 CrewCo_API-0.0.5/src/crewco_api/
+-rw-rw-rw-   0        0        0        0 2023-05-18 16:30:21.000000 CrewCo_API-0.0.5/src/crewco_api/__init__.py
+-rw-rw-rw-   0        0        0     3179 2023-05-19 05:22:10.000000 CrewCo_API-0.0.5/src/crewco_api/api.py
+-rw-rw-rw-   0        0        0        2 2023-05-19 05:17:21.000000 CrewCo_API-0.0.5/src/crewco_api/main.py
```

### Comparing `CrewCo_API-0.0.4/LICENSE` & `CrewCo_API-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `CrewCo_API-0.0.4/PKG-INFO` & `CrewCo_API-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CrewCo_API
-Version: 0.0.4
+Version: 0.0.5
 Summary: CrewCo's beta API
 Author-email: CrewCo <crewco.99@gmail.com>
 Project-URL: Homepage, https://github.com/Crew-co/CrewCo_API/
 Project-URL: Bug Tracker, https://github.com/Crew-co/CrewCo_API//issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `CrewCo_API-0.0.4/pyproject.toml` & `CrewCo_API-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "CrewCo_API"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="CrewCo", email="crewco.99@gmail.com" },
 ]
 description = "CrewCo's beta API"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `CrewCo_API-0.0.4/src/CrewCo_API.egg-info/PKG-INFO` & `CrewCo_API-0.0.5/src/CrewCo_API.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CrewCo-API
-Version: 0.0.4
+Version: 0.0.5
 Summary: CrewCo's beta API
 Author-email: CrewCo <crewco.99@gmail.com>
 Project-URL: Homepage, https://github.com/Crew-co/CrewCo_API/
 Project-URL: Bug Tracker, https://github.com/Crew-co/CrewCo_API//issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `CrewCo_API-0.0.4/src/crewco_api/api.py` & `CrewCo_API-0.0.5/src/crewco_api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,14 @@
         latitude = data['results'][0]['geometry']['location']['lat']
         longitude = data['results'][0]['geometry']['location']['lng']
         formatted_address = data['results'][0]['formatted_address']
         final = f"Latitude:{latitude},Longitude:{longitude}, Formatted-Address:{formatted_address}"
         return final
 
     def override(self,name,key):
-        endpoint = ""
+        endpoint = "http://127.0.0.1:5000/api/override"
         data = {
             'name':name,
             'key':key
         }
         rq.post(url=endpoint,data=data)
         return rq.status_codes
```

