# Comparing `tmp/emailvalidationio-0.1.tar.gz` & `tmp/emailvalidationio-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/emailvalidationio-0.1.tar", last modified: Fri May 19 07:53:25 2023, max compression
+gzip compressed data, was "dist/emailvalidationio-0.2.tar", last modified: Fri May 19 07:58:15 2023, max compression
```

## Comparing `emailvalidationio-0.1.tar` & `emailvalidationio-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 andreasaltheimer   (501) staff       (20)        0 2023-05-19 07:53:25.000000 emailvalidationio-0.1/
--rw-r--r--   0 andreasaltheimer   (501) staff       (20)     2556 2023-05-19 07:53:25.000000 emailvalidationio-0.1/PKG-INFO
-drwxr-xr-x   0 andreasaltheimer   (501) staff       (20)        0 2023-05-19 07:53:25.000000 emailvalidationio-0.1/emailvalidationio.egg-info/
--rw-r--r--   0 andreasaltheimer   (501) staff       (20)     2556 2023-05-19 07:53:25.000000 emailvalidationio-0.1/emailvalidationio.egg-info/PKG-INFO
--rw-r--r--   0 andreasaltheimer   (501) staff       (20)      280 2023-05-19 07:53:25.000000 emailvalidationio-0.1/emailvalidationio.egg-info/SOURCES.txt
--rw-r--r--   0 andreasaltheimer   (501) staff       (20)       17 2023-05-19 07:53:25.000000 emailvalidationio-0.1/emailvalidationio.egg-info/requires.txt
--rw-r--r--   0 andreasaltheimer   (501) staff       (20)       18 2023-05-19 07:53:25.000000 emailvalidationio-0.1/emailvalidationio.egg-info/top_level.txt
--rw-r--r--   0 andreasaltheimer   (501) staff       (20)        1 2023-05-19 07:53:25.000000 emailvalidationio-0.1/emailvalidationio.egg-info/dependency_links.txt
--rw-r--r--   0 andreasaltheimer   (501) staff       (20)     1128 2023-05-19 07:22:24.000000 emailvalidationio-0.1/README.md
--rw-r--r--   0 andreasaltheimer   (501) staff       (20)     1460 2023-05-19 07:52:57.000000 emailvalidationio-0.1/setup.py
-drwxr-xr-x   0 andreasaltheimer   (501) staff       (20)        0 2023-05-19 07:53:25.000000 emailvalidationio-0.1/emailvalidationio/
--rw-r--r--   0 andreasaltheimer   (501) staff       (20)      404 2023-05-19 07:23:58.000000 emailvalidationio-0.1/emailvalidationio/client.py
--rw-r--r--   0 andreasaltheimer   (501) staff       (20)       58 2023-05-19 07:53:18.000000 emailvalidationio-0.1/emailvalidationio/__init__.py
--rw-r--r--   0 andreasaltheimer   (501) staff       (20)       38 2023-05-19 07:53:25.000000 emailvalidationio-0.1/setup.cfg
+drwxr-xr-x   0 andreasaltheimer   (501) staff       (20)        0 2023-05-19 07:58:15.000000 emailvalidationio-0.2/
+-rw-r--r--   0 andreasaltheimer   (501) staff       (20)     2564 2023-05-19 07:58:15.000000 emailvalidationio-0.2/PKG-INFO
+drwxr-xr-x   0 andreasaltheimer   (501) staff       (20)        0 2023-05-19 07:58:15.000000 emailvalidationio-0.2/emailvalidationio.egg-info/
+-rw-r--r--   0 andreasaltheimer   (501) staff       (20)     2564 2023-05-19 07:58:15.000000 emailvalidationio-0.2/emailvalidationio.egg-info/PKG-INFO
+-rw-r--r--   0 andreasaltheimer   (501) staff       (20)      280 2023-05-19 07:58:15.000000 emailvalidationio-0.2/emailvalidationio.egg-info/SOURCES.txt
+-rw-r--r--   0 andreasaltheimer   (501) staff       (20)       17 2023-05-19 07:58:15.000000 emailvalidationio-0.2/emailvalidationio.egg-info/requires.txt
+-rw-r--r--   0 andreasaltheimer   (501) staff       (20)       18 2023-05-19 07:58:15.000000 emailvalidationio-0.2/emailvalidationio.egg-info/top_level.txt
+-rw-r--r--   0 andreasaltheimer   (501) staff       (20)        1 2023-05-19 07:58:15.000000 emailvalidationio-0.2/emailvalidationio.egg-info/dependency_links.txt
+-rw-r--r--   0 andreasaltheimer   (501) staff       (20)     1136 2023-05-19 07:57:15.000000 emailvalidationio-0.2/README.md
+-rw-r--r--   0 andreasaltheimer   (501) staff       (20)     1460 2023-05-19 07:58:12.000000 emailvalidationio-0.2/setup.py
+drwxr-xr-x   0 andreasaltheimer   (501) staff       (20)        0 2023-05-19 07:58:15.000000 emailvalidationio-0.2/emailvalidationio/
+-rw-r--r--   0 andreasaltheimer   (501) staff       (20)      404 2023-05-19 07:23:58.000000 emailvalidationio-0.2/emailvalidationio/client.py
+-rw-r--r--   0 andreasaltheimer   (501) staff       (20)       58 2023-05-19 07:53:18.000000 emailvalidationio-0.2/emailvalidationio/__init__.py
+-rw-r--r--   0 andreasaltheimer   (501) staff       (20)       38 2023-05-19 07:58:15.000000 emailvalidationio-0.2/setup.cfg
```

### Comparing `emailvalidationio-0.1/PKG-INFO` & `emailvalidationio-0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: emailvalidationio
-Version: 0.1
+Version: 0.2
 Summary: Emailvalidation Python Client
 Home-page: https://github.com/everapihq/emailvalidation-python
 Author: Everapi
 Author-email: office@everapi.com
 License: MIT
 Description: # Emailvalidation Python Client #
         
         Emailvalidation Python Client is the official Python Wrapper around the Emailvalidation [API](https://emailvalidation.io/).
         
         ## Installation
         
         Install from pip:
         ````sh
-        pip install emailvalidation
+        pip install emailvalidationio
         ````
         
         Install from code:
         ````sh
         pip install git+https://github.com/everapihq/emailvalidation-python.git
         ````
         
         ## Usage
         
         All emailvalidation API requests are made using the `Client` class. This class must be initialized with your API access key string. [Where is my API access key?](https://app.emailvalidation.io/dashboard)
         
-        In your Python application, import `emailvalidation` and pass authentication information to initialize it:
+        In your Python application, import `emailvalidationio` and pass authentication information to initialize it:
         
         ````python
-        import emailvalidation
-        client = emailvalidation.Client('API_KEY')
+        import emailvalidationio
+        client = emailvalidationio.Client('API_KEY')
         ````
         
         ### Retrieve Status
         
         ```python
         
         print(client.status())
```

### Comparing `emailvalidationio-0.1/emailvalidationio.egg-info/PKG-INFO` & `emailvalidationio-0.2/emailvalidationio.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: emailvalidationio
-Version: 0.1
+Version: 0.2
 Summary: Emailvalidation Python Client
 Home-page: https://github.com/everapihq/emailvalidation-python
 Author: Everapi
 Author-email: office@everapi.com
 License: MIT
 Description: # Emailvalidation Python Client #
         
         Emailvalidation Python Client is the official Python Wrapper around the Emailvalidation [API](https://emailvalidation.io/).
         
         ## Installation
         
         Install from pip:
         ````sh
-        pip install emailvalidation
+        pip install emailvalidationio
         ````
         
         Install from code:
         ````sh
         pip install git+https://github.com/everapihq/emailvalidation-python.git
         ````
         
         ## Usage
         
         All emailvalidation API requests are made using the `Client` class. This class must be initialized with your API access key string. [Where is my API access key?](https://app.emailvalidation.io/dashboard)
         
-        In your Python application, import `emailvalidation` and pass authentication information to initialize it:
+        In your Python application, import `emailvalidationio` and pass authentication information to initialize it:
         
         ````python
-        import emailvalidation
-        client = emailvalidation.Client('API_KEY')
+        import emailvalidationio
+        client = emailvalidationio.Client('API_KEY')
         ````
         
         ### Retrieve Status
         
         ```python
         
         print(client.status())
```

### Comparing `emailvalidationio-0.1/README.md` & `emailvalidationio-0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 
 Emailvalidation Python Client is the official Python Wrapper around the Emailvalidation [API](https://emailvalidation.io/).
 
 ## Installation
 
 Install from pip:
 ````sh
-pip install emailvalidation
+pip install emailvalidationio
 ````
 
 Install from code:
 ````sh
 pip install git+https://github.com/everapihq/emailvalidation-python.git
 ````
 
 ## Usage
 
 All emailvalidation API requests are made using the `Client` class. This class must be initialized with your API access key string. [Where is my API access key?](https://app.emailvalidation.io/dashboard)
 
-In your Python application, import `emailvalidation` and pass authentication information to initialize it:
+In your Python application, import `emailvalidationio` and pass authentication information to initialize it:
 
 ````python
-import emailvalidation
-client = emailvalidation.Client('API_KEY')
+import emailvalidationio
+client = emailvalidationio.Client('API_KEY')
 ````
 
 ### Retrieve Status
 
 ```python
 
 print(client.status())
```

### Comparing `emailvalidationio-0.1/setup.py` & `emailvalidationio-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name='emailvalidationio',
-    version='0.1',
+    version='0.2',
     packages=['emailvalidationio'],
     url='https://github.com/everapihq/emailvalidation-python',
     license='MIT',
     author='Everapi',
     author_email='office@everapi.com',
     description='Emailvalidation Python Client',
     classifiers=[
```

