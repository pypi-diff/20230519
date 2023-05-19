# Comparing `tmp/python-amcards-1.2.8.tar.gz` & `tmp/python-amcards-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-amcards-1.2.8.tar", last modified: Thu Nov 17 23:05:22 2022, max compression
+gzip compressed data, was "python-amcards-1.2.9.tar", last modified: Thu Nov 17 23:13:15 2022, max compression
```

## Comparing `python-amcards-1.2.8.tar` & `python-amcards-1.2.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2022-11-17 23:05:22.112162 python-amcards-1.2.8/
--rw-r--r--   0 simonesestili   (501) staff       (20)    11357 2022-11-05 02:56:15.000000 python-amcards-1.2.8/LICENSE
--rw-r--r--   0 simonesestili   (501) staff       (20)     3050 2022-11-17 23:05:22.112014 python-amcards-1.2.8/PKG-INFO
--rw-r--r--   0 simonesestili   (501) staff       (20)     2467 2022-11-05 09:50:39.000000 python-amcards-1.2.8/README.rst
-drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2022-11-17 23:05:22.109410 python-amcards-1.2.8/amcards/
--rw-r--r--   0 simonesestili   (501) staff       (20)     5106 2022-11-08 04:57:10.000000 python-amcards-1.2.8/amcards/__helpers.py
--rw-r--r--   0 simonesestili   (501) staff       (20)       34 2022-11-05 02:56:15.000000 python-amcards-1.2.8/amcards/__init__.py
--rw-r--r--   0 simonesestili   (501) staff       (20)    52468 2022-11-17 07:32:01.000000 python-amcards-1.2.8/amcards/amcards.py
--rw-r--r--   0 simonesestili   (501) staff       (20)     1649 2022-11-12 20:48:33.000000 python-amcards-1.2.8/amcards/exceptions.py
--rw-r--r--   0 simonesestili   (501) staff       (20)    25678 2022-11-17 23:04:07.000000 python-amcards-1.2.8/amcards/models.py
-drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2022-11-17 23:05:22.109559 python-amcards-1.2.8/images/
--rw-r--r--   0 simonesestili   (501) staff       (20)   537836 2022-11-05 09:15:52.000000 python-amcards-1.2.8/images/readthedocs.png
-drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2022-11-17 23:05:22.111777 python-amcards-1.2.8/python_amcards.egg-info/
--rw-r--r--   0 simonesestili   (501) staff       (20)     3050 2022-11-17 23:05:22.000000 python-amcards-1.2.8/python_amcards.egg-info/PKG-INFO
--rw-r--r--   0 simonesestili   (501) staff       (20)      339 2022-11-17 23:05:22.000000 python-amcards-1.2.8/python_amcards.egg-info/SOURCES.txt
--rw-r--r--   0 simonesestili   (501) staff       (20)        1 2022-11-17 23:05:22.000000 python-amcards-1.2.8/python_amcards.egg-info/dependency_links.txt
--rw-r--r--   0 simonesestili   (501) staff       (20)       12 2022-11-17 23:05:22.000000 python-amcards-1.2.8/python_amcards.egg-info/requires.txt
--rw-r--r--   0 simonesestili   (501) staff       (20)        8 2022-11-17 23:05:22.000000 python-amcards-1.2.8/python_amcards.egg-info/top_level.txt
--rw-r--r--   0 simonesestili   (501) staff       (20)       38 2022-11-17 23:05:22.112204 python-amcards-1.2.8/setup.cfg
--rw-r--r--   0 simonesestili   (501) staff       (20)      874 2022-11-17 23:04:45.000000 python-amcards-1.2.8/setup.py
+drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2022-11-17 23:13:15.044571 python-amcards-1.2.9/
+-rw-r--r--   0 simonesestili   (501) staff       (20)    11357 2022-11-05 02:56:15.000000 python-amcards-1.2.9/LICENSE
+-rw-r--r--   0 simonesestili   (501) staff       (20)     3050 2022-11-17 23:13:15.044449 python-amcards-1.2.9/PKG-INFO
+-rw-r--r--   0 simonesestili   (501) staff       (20)     2467 2022-11-05 09:50:39.000000 python-amcards-1.2.9/README.rst
+drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2022-11-17 23:13:15.042783 python-amcards-1.2.9/amcards/
+-rw-r--r--   0 simonesestili   (501) staff       (20)     5106 2022-11-08 04:57:10.000000 python-amcards-1.2.9/amcards/__helpers.py
+-rw-r--r--   0 simonesestili   (501) staff       (20)       34 2022-11-05 02:56:15.000000 python-amcards-1.2.9/amcards/__init__.py
+-rw-r--r--   0 simonesestili   (501) staff       (20)    52468 2022-11-17 07:32:01.000000 python-amcards-1.2.9/amcards/amcards.py
+-rw-r--r--   0 simonesestili   (501) staff       (20)     1649 2022-11-12 20:48:33.000000 python-amcards-1.2.9/amcards/exceptions.py
+-rw-r--r--   0 simonesestili   (501) staff       (20)    25679 2022-11-17 23:12:45.000000 python-amcards-1.2.9/amcards/models.py
+drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2022-11-17 23:13:15.042927 python-amcards-1.2.9/images/
+-rw-r--r--   0 simonesestili   (501) staff       (20)   537836 2022-11-05 09:15:52.000000 python-amcards-1.2.9/images/readthedocs.png
+drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2022-11-17 23:13:15.044273 python-amcards-1.2.9/python_amcards.egg-info/
+-rw-r--r--   0 simonesestili   (501) staff       (20)     3050 2022-11-17 23:13:15.000000 python-amcards-1.2.9/python_amcards.egg-info/PKG-INFO
+-rw-r--r--   0 simonesestili   (501) staff       (20)      339 2022-11-17 23:13:15.000000 python-amcards-1.2.9/python_amcards.egg-info/SOURCES.txt
+-rw-r--r--   0 simonesestili   (501) staff       (20)        1 2022-11-17 23:13:15.000000 python-amcards-1.2.9/python_amcards.egg-info/dependency_links.txt
+-rw-r--r--   0 simonesestili   (501) staff       (20)       12 2022-11-17 23:13:15.000000 python-amcards-1.2.9/python_amcards.egg-info/requires.txt
+-rw-r--r--   0 simonesestili   (501) staff       (20)        8 2022-11-17 23:13:15.000000 python-amcards-1.2.9/python_amcards.egg-info/top_level.txt
+-rw-r--r--   0 simonesestili   (501) staff       (20)       38 2022-11-17 23:13:15.044613 python-amcards-1.2.9/setup.cfg
+-rw-r--r--   0 simonesestili   (501) staff       (20)      874 2022-11-17 23:12:23.000000 python-amcards-1.2.9/setup.py
```

### Comparing `python-amcards-1.2.8/LICENSE` & `python-amcards-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python-amcards-1.2.8/PKG-INFO` & `python-amcards-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-amcards
-Version: 1.2.8
+Version: 1.2.9
 Summary: A wrapper for the AMcards API.
 Home-page: https://github.com/simonesestili/python-amcards
 Author: Simone Sestili
 Author-email: simone.sestili@amcards.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `python-amcards-1.2.8/README.rst` & `python-amcards-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `python-amcards-1.2.8/amcards/__helpers.py` & `python-amcards-1.2.9/amcards/__helpers.py`

 * *Files identical despite different names*

### Comparing `python-amcards-1.2.8/amcards/amcards.py` & `python-amcards-1.2.9/amcards/amcards.py`

 * *Files identical despite different names*

### Comparing `python-amcards-1.2.8/amcards/exceptions.py` & `python-amcards-1.2.9/amcards/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-amcards-1.2.8/amcards/models.py` & `python-amcards-1.2.9/amcards/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     @property
     def credits(self) -> int:
         """User's credit balance in `cents`."""
         return self._credits
 
     @property
-    def mail(self) -> str:
+    def email(self) -> str:
         """User's email address."""
         return self._email
 
     @property
     def date_joined(self) -> datetime:
         """Date and time when user created their AMcards account."""
         return self._date_joined
```

### Comparing `python-amcards-1.2.8/images/readthedocs.png` & `python-amcards-1.2.9/images/readthedocs.png`

 * *Files identical despite different names*

### Comparing `python-amcards-1.2.8/python_amcards.egg-info/PKG-INFO` & `python-amcards-1.2.9/python_amcards.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-amcards
-Version: 1.2.8
+Version: 1.2.9
 Summary: A wrapper for the AMcards API.
 Home-page: https://github.com/simonesestili/python-amcards
 Author: Simone Sestili
 Author-email: simone.sestili@amcards.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `python-amcards-1.2.8/setup.py` & `python-amcards-1.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def README():
     with open('README.rst') as f:
         return f.read()
 
 setup(
     name='python-amcards',
-    version='1.2.8',
+    version='1.2.9',
     description='A wrapper for the AMcards API.',
     long_description=README(),
     long_description_content_type='text/x-rst',
     author='Simone Sestili',
     author_email='simone.sestili@amcards.com',
     url='https://github.com/simonesestili/python-amcards',
     packages=['amcards'],
```

