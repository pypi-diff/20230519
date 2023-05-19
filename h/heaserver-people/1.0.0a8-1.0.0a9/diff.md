# Comparing `tmp/heaserver-people-1.0.0a8.tar.gz` & `tmp/heaserver-people-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-people-1.0.0a8.tar", last modified: Tue Aug 16 20:57:51 2022, max compression
+gzip compressed data, was "heaserver-people-1.0.0a9.tar", last modified: Wed Jan 25 00:30:42 2023, max compression
```

## Comparing `heaserver-people-1.0.0a8.tar` & `heaserver-people-1.0.0a9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2022-08-16 20:57:51.750580 heaserver-people-1.0.0a8/
--rw-rw-rw-   0        0        0      261 2021-11-22 20:19:09.000000 heaserver-people-1.0.0a8/.editorconfig
--rw-rw-rw-   0        0        0      288 2022-08-16 20:54:42.000000 heaserver-people-1.0.0a8/.gitignore
--rw-rw-rw-   0        0        0    11625 2021-11-22 20:19:09.000000 heaserver-people-1.0.0a8/LICENSE
--rw-rw-rw-   0        0        0      243 2022-08-16 20:54:56.000000 heaserver-people-1.0.0a8/MANIFEST.in
--rw-rw-rw-   0        0        0     4906 2022-08-16 20:57:51.749579 heaserver-people-1.0.0a8/PKG-INFO
--rw-rw-rw-   0        0        0     3598 2022-08-16 20:54:56.000000 heaserver-people-1.0.0a8/README.md
--rw-rw-rw-   0        0        0     1908 2022-03-10 19:33:18.000000 heaserver-people-1.0.0a8/RELEASING.md
-drwxrwxrwx   0        0        0        0 2022-08-16 20:57:51.651581 heaserver-people-1.0.0a8/integrationtests/
-drwxrwxrwx   0        0        0        0 2022-08-16 20:57:51.651581 heaserver-people-1.0.0a8/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2022-08-16 20:57:51.705584 heaserver-people-1.0.0a8/integrationtests/heaserver/personintegrationtest/
--rw-rw-rw-   0        0        0        0 2021-11-22 20:19:09.000000 heaserver-people-1.0.0a8/integrationtests/heaserver/personintegrationtest/__init__.py
--rw-rw-rw-   0        0        0     3678 2022-08-16 20:54:56.000000 heaserver-people-1.0.0a8/integrationtests/heaserver/personintegrationtest/permissionstestcase.py
--rw-rw-rw-   0        0        0     4479 2022-08-16 20:54:56.000000 heaserver-people-1.0.0a8/integrationtests/heaserver/personintegrationtest/test_all.py
--rw-rw-rw-   0        0        0     3641 2022-08-16 20:54:56.000000 heaserver-people-1.0.0a8/integrationtests/heaserver/personintegrationtest/testcase.py
--rw-rw-rw-   0        0        0       92 2021-11-22 20:20:40.000000 heaserver-people-1.0.0a8/pytest.ini
--rw-rw-rw-   0        0        0      329 2022-08-16 20:54:56.000000 heaserver-people-1.0.0a8/requirements_dev.txt
--rw-rw-rw-   0        0        0       42 2022-08-16 20:57:51.750580 heaserver-people-1.0.0a8/setup.cfg
--rw-rw-rw-   0        0        0     1811 2022-08-16 20:56:19.000000 heaserver-people-1.0.0a8/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-16 20:57:51.652581 heaserver-people-1.0.0a8/src/
-drwxrwxrwx   0        0        0        0 2022-08-16 20:57:51.652581 heaserver-people-1.0.0a8/src/heaserver/
-drwxrwxrwx   0        0        0        0 2022-08-16 20:57:51.713580 heaserver-people-1.0.0a8/src/heaserver/person/
--rw-rw-rw-   0        0        0        0 2021-11-22 20:19:09.000000 heaserver-people-1.0.0a8/src/heaserver/person/__init__.py
--rw-rw-rw-   0        0        0    12321 2022-08-16 20:54:56.000000 heaserver-people-1.0.0a8/src/heaserver/person/service.py
-drwxrwxrwx   0        0        0        0 2022-08-16 20:57:51.718581 heaserver-people-1.0.0a8/src/heaserver/person/wstl/
--rw-rw-rw-   0        0        0     8397 2022-08-16 20:54:56.000000 heaserver-people-1.0.0a8/src/heaserver/person/wstl/all.json
-drwxrwxrwx   0        0        0        0 2022-08-16 20:57:51.735578 heaserver-people-1.0.0a8/src/heaserver_people.egg-info/
--rw-rw-rw-   0        0        0     4906 2022-08-16 20:57:51.000000 heaserver-people-1.0.0a8/src/heaserver_people.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      896 2022-08-16 20:57:51.000000 heaserver-people-1.0.0a8/src/heaserver_people.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-16 20:57:51.000000 heaserver-people-1.0.0a8/src/heaserver_people.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2022-08-16 20:57:51.000000 heaserver-people-1.0.0a8/src/heaserver_people.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2022-08-16 20:57:51.000000 heaserver-people-1.0.0a8/src/heaserver_people.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-08-16 20:57:51.000000 heaserver-people-1.0.0a8/src/heaserver_people.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-08-16 20:57:51.653580 heaserver-people-1.0.0a8/tests/
-drwxrwxrwx   0        0        0        0 2022-08-16 20:57:51.653580 heaserver-people-1.0.0a8/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2022-08-16 20:57:51.748578 heaserver-people-1.0.0a8/tests/heaserver/persontest/
--rw-rw-rw-   0        0        0        0 2021-11-22 20:19:09.000000 heaserver-people-1.0.0a8/tests/heaserver/persontest/__init__.py
--rw-rw-rw-   0        0        0     3678 2022-08-16 20:54:56.000000 heaserver-people-1.0.0a8/tests/heaserver/persontest/permissionstestcase.py
--rw-rw-rw-   0        0        0     3907 2022-08-16 20:54:56.000000 heaserver-people-1.0.0a8/tests/heaserver/persontest/test_all.py
--rw-rw-rw-   0        0        0     3497 2022-08-16 20:54:56.000000 heaserver-people-1.0.0a8/tests/heaserver/persontest/testcase.py
+drwxrwxrwx   0        0        0        0 2023-01-25 00:30:42.983362 heaserver-people-1.0.0a9/
+-rw-rw-rw-   0        0        0      261 2022-05-12 22:51:16.000000 heaserver-people-1.0.0a9/.editorconfig
+-rw-rw-rw-   0        0        0      288 2022-05-12 22:51:16.000000 heaserver-people-1.0.0a9/.gitignore
+-rw-rw-rw-   0        0        0    11625 2022-05-12 22:51:16.000000 heaserver-people-1.0.0a9/LICENSE
+-rw-rw-rw-   0        0        0      243 2022-06-10 20:41:13.000000 heaserver-people-1.0.0a9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4906 2023-01-25 00:30:42.983362 heaserver-people-1.0.0a9/PKG-INFO
+-rw-rw-rw-   0        0        0     3598 2022-07-01 00:43:50.000000 heaserver-people-1.0.0a9/README.md
+-rw-rw-rw-   0        0        0     1908 2022-05-12 22:51:16.000000 heaserver-people-1.0.0a9/RELEASING.md
+drwxrwxrwx   0        0        0        0 2023-01-25 00:30:42.936484 heaserver-people-1.0.0a9/integrationtests/
+drwxrwxrwx   0        0        0        0 2023-01-25 00:30:42.936484 heaserver-people-1.0.0a9/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2023-01-25 00:30:42.952110 heaserver-people-1.0.0a9/integrationtests/heaserver/personintegrationtest/
+-rw-rw-rw-   0        0        0        0 2022-05-12 22:51:16.000000 heaserver-people-1.0.0a9/integrationtests/heaserver/personintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0     3678 2023-01-23 22:57:17.000000 heaserver-people-1.0.0a9/integrationtests/heaserver/personintegrationtest/permissionstestcase.py
+-rw-rw-rw-   0        0        0     4479 2023-01-23 22:57:17.000000 heaserver-people-1.0.0a9/integrationtests/heaserver/personintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0     3641 2023-01-23 22:57:17.000000 heaserver-people-1.0.0a9/integrationtests/heaserver/personintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0       92 2022-05-12 22:51:16.000000 heaserver-people-1.0.0a9/pytest.ini
+-rw-rw-rw-   0        0        0      241 2023-01-24 23:22:01.000000 heaserver-people-1.0.0a9/requirements_dev.txt
+-rw-rw-rw-   0        0        0       42 2023-01-25 00:30:42.983362 heaserver-people-1.0.0a9/setup.cfg
+-rw-rw-rw-   0        0        0     1811 2023-01-25 00:30:21.000000 heaserver-people-1.0.0a9/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-25 00:30:42.936484 heaserver-people-1.0.0a9/src/
+drwxrwxrwx   0        0        0        0 2023-01-25 00:30:42.936484 heaserver-people-1.0.0a9/src/heaserver/
+drwxrwxrwx   0        0        0        0 2023-01-25 00:30:42.952110 heaserver-people-1.0.0a9/src/heaserver/person/
+-rw-rw-rw-   0        0        0        0 2022-05-12 22:51:16.000000 heaserver-people-1.0.0a9/src/heaserver/person/__init__.py
+-rw-rw-rw-   0        0        0    14209 2023-01-25 00:17:59.000000 heaserver-people-1.0.0a9/src/heaserver/person/service.py
+drwxrwxrwx   0        0        0        0 2023-01-25 00:30:42.952110 heaserver-people-1.0.0a9/src/heaserver/person/wstl/
+-rw-rw-rw-   0        0        0     8686 2023-01-24 00:58:40.000000 heaserver-people-1.0.0a9/src/heaserver/person/wstl/all.json
+drwxrwxrwx   0        0        0        0 2023-01-25 00:30:42.967741 heaserver-people-1.0.0a9/src/heaserver_people.egg-info/
+-rw-rw-rw-   0        0        0     4906 2023-01-25 00:30:42.000000 heaserver-people-1.0.0a9/src/heaserver_people.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      896 2023-01-25 00:30:42.000000 heaserver-people-1.0.0a9/src/heaserver_people.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-25 00:30:42.000000 heaserver-people-1.0.0a9/src/heaserver_people.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-01-25 00:30:42.000000 heaserver-people-1.0.0a9/src/heaserver_people.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2023-01-25 00:30:42.000000 heaserver-people-1.0.0a9/src/heaserver_people.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-01-25 00:30:42.000000 heaserver-people-1.0.0a9/src/heaserver_people.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-01-25 00:30:42.936484 heaserver-people-1.0.0a9/tests/
+drwxrwxrwx   0        0        0        0 2023-01-25 00:30:42.936484 heaserver-people-1.0.0a9/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2023-01-25 00:30:42.967741 heaserver-people-1.0.0a9/tests/heaserver/persontest/
+-rw-rw-rw-   0        0        0        0 2022-05-12 22:51:16.000000 heaserver-people-1.0.0a9/tests/heaserver/persontest/__init__.py
+-rw-rw-rw-   0        0        0     3678 2023-01-23 22:57:17.000000 heaserver-people-1.0.0a9/tests/heaserver/persontest/permissionstestcase.py
+-rw-rw-rw-   0        0        0     3907 2023-01-23 22:57:17.000000 heaserver-people-1.0.0a9/tests/heaserver/persontest/test_all.py
+-rw-rw-rw-   0        0        0     3497 2022-07-01 00:43:50.000000 heaserver-people-1.0.0a9/tests/heaserver/persontest/testcase.py
```

### Comparing `heaserver-people-1.0.0a8/LICENSE` & `heaserver-people-1.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-people-1.0.0a8/PKG-INFO` & `heaserver-people-1.0.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-people
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: A microservice designed to provide CRUD operations for the Person HEA object type
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 License: UNKNOWN
 Keywords: heaserver-people,microservice,healthcare,cancer,research,informatics
 Platform: UNKNOWN
```

### Comparing `heaserver-people-1.0.0a8/README.md` & `heaserver-people-1.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `heaserver-people-1.0.0a8/RELEASING.md` & `heaserver-people-1.0.0a9/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-people-1.0.0a8/integrationtests/heaserver/personintegrationtest/permissionstestcase.py` & `heaserver-people-1.0.0a9/integrationtests/heaserver/personintegrationtest/permissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-people-1.0.0a8/integrationtests/heaserver/personintegrationtest/test_all.py` & `heaserver-people-1.0.0a9/integrationtests/heaserver/personintegrationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-people-1.0.0a8/integrationtests/heaserver/personintegrationtest/testcase.py` & `heaserver-people-1.0.0a9/integrationtests/heaserver/personintegrationtest/testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-people-1.0.0a8/setup.py` & `heaserver-people-1.0.0a9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-people',
-    version='1.0.0a8',
+    version='1.0.0a9',
     description="A microservice designed to provide CRUD operations for the Person HEA object type",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.person'],
     package_data={'heaserver.person': ['wstl/*.json']},
-    install_requires=['heaserver>=1.0.0a76, <1.0.0a77'],
+    install_requires=['heaserver>=1.0.0a87, <1.0.0a88'],
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
         'Environment :: Web Environment',
```

### Comparing `heaserver-people-1.0.0a8/src/heaserver/person/wstl/all.json` & `heaserver-people-1.0.0a9/src/heaserver/person/wstl/all.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9732142857142857%*

 * *Differences: {"'wstl'": '{\'actions\': {3: {\'description\': "View and edit this person\'s properties"}, '*

 * *           "insert: [(2, OrderedDict([('name', 'heaserver-people-person-get-self'), "*

 * *           "('description', 'View this person'), ('type', 'safe'), ('action', 'read'), ('target', "*

 * *           "'item read cj'), ('prompt', 'View')]))]}}"}*

```diff
@@ -10,16 +10,24 @@
             {
                 "name": "heaserver-people-person-open",
                 "prompt": "Open",
                 "target": "item",
                 "type": "safe"
             },
             {
+                "action": "read",
+                "description": "View this person",
+                "name": "heaserver-people-person-get-self",
+                "prompt": "View",
+                "target": "item read cj",
+                "type": "safe"
+            },
+            {
                 "action": "update",
-                "description": "View and edit this Person's properties",
+                "description": "View and edit this person's properties",
                 "inputs": [
                     {
                         "name": "id",
                         "prompt": "Id",
                         "readOnly": true
                     },
                     {
```

### Comparing `heaserver-people-1.0.0a8/src/heaserver_people.egg-info/PKG-INFO` & `heaserver-people-1.0.0a9/src/heaserver_people.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-people
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: A microservice designed to provide CRUD operations for the Person HEA object type
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 License: UNKNOWN
 Keywords: heaserver-people,microservice,healthcare,cancer,research,informatics
 Platform: UNKNOWN
```

### Comparing `heaserver-people-1.0.0a8/src/heaserver_people.egg-info/SOURCES.txt` & `heaserver-people-1.0.0a9/src/heaserver_people.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-people-1.0.0a8/tests/heaserver/persontest/permissionstestcase.py` & `heaserver-people-1.0.0a9/tests/heaserver/persontest/permissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-people-1.0.0a8/tests/heaserver/persontest/test_all.py` & `heaserver-people-1.0.0a9/tests/heaserver/persontest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-people-1.0.0a8/tests/heaserver/persontest/testcase.py` & `heaserver-people-1.0.0a9/tests/heaserver/persontest/testcase.py`

 * *Files identical despite different names*

