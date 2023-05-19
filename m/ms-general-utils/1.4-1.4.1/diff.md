# Comparing `tmp/ms_general_utils-1.4.tar.gz` & `tmp/ms_general_utils-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_general_utils-1.4.tar", last modified: Wed May 17 12:42:40 2023, max compression
+gzip compressed data, was "ms_general_utils-1.4.1.tar", last modified: Fri May 19 16:20:00 2023, max compression
```

## Comparing `ms_general_utils-1.4.tar` & `ms_general_utils-1.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 12:42:40.457096 ms_general_utils-1.4/
--rw-rw-rw-   0        0        0     1073 2023-03-14 11:56:37.000000 ms_general_utils-1.4/LICENSE.txt
--rw-rw-rw-   0        0        0      352 2023-05-17 12:42:40.454104 ms_general_utils-1.4/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-03-14 15:40:50.000000 ms_general_utils-1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 12:42:40.381559 ms_general_utils-1.4/ms_general_utils.egg-info/
--rw-rw-rw-   0        0        0      352 2023-05-17 12:42:40.000000 ms_general_utils-1.4/ms_general_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-05-17 12:42:40.000000 ms_general_utils-1.4/ms_general_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 12:42:40.000000 ms_general_utils-1.4/ms_general_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-17 12:42:40.000000 ms_general_utils-1.4/ms_general_utils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-17 12:42:40.449102 ms_general_utils-1.4/ms_utils/
--rw-rw-rw-   0        0        0      555 2023-03-27 15:14:21.000000 ms_general_utils-1.4/ms_utils/__init__.py
--rw-rw-rw-   0        0        0      386 2023-03-17 12:23:38.000000 ms_general_utils-1.4/ms_utils/abstract_model.py
--rw-rw-rw-   0        0        0     1034 2023-03-17 11:27:17.000000 ms_general_utils-1.4/ms_utils/binary_uuid.py
--rw-rw-rw-   0        0        0      695 2023-03-17 08:52:55.000000 ms_general_utils-1.4/ms_utils/func_date.py
--rw-rw-rw-   0        0        0     2570 2023-04-03 15:04:19.000000 ms_general_utils-1.4/ms_utils/generic_crud_class.py
--rw-rw-rw-   0        0        0      706 2023-03-17 08:52:56.000000 ms_general_utils-1.4/ms_utils/generic_pagination.py
--rw-rw-rw-   0        0        0     1527 2023-04-03 17:16:10.000000 ms_general_utils-1.4/ms_utils/model_utils.py
--rw-rw-rw-   0        0        0      341 2023-03-17 08:52:56.000000 ms_general_utils-1.4/ms_utils/prepare_json_response.py
--rw-rw-rw-   0        0        0      466 2023-04-03 14:47:57.000000 ms_general_utils-1.4/ms_utils/validation_utils.py
--rw-rw-rw-   0        0        0     4228 2023-05-17 12:41:26.000000 ms_general_utils-1.4/ms_utils/view_utils.py
--rw-rw-rw-   0        0        0       42 2023-05-17 12:42:40.457096 ms_general_utils-1.4/setup.cfg
--rw-rw-rw-   0        0        0      674 2023-05-17 12:41:47.000000 ms_general_utils-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 16:20:00.447266 ms_general_utils-1.4.1/
+-rw-rw-rw-   0        0        0     1073 2023-03-14 11:56:37.000000 ms_general_utils-1.4.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      354 2023-05-19 16:20:00.441265 ms_general_utils-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-03-14 15:40:50.000000 ms_general_utils-1.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 16:20:00.243964 ms_general_utils-1.4.1/ms_general_utils.egg-info/
+-rw-rw-rw-   0        0        0      354 2023-05-19 16:20:00.000000 ms_general_utils-1.4.1/ms_general_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-05-19 16:20:00.000000 ms_general_utils-1.4.1/ms_general_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 16:20:00.000000 ms_general_utils-1.4.1/ms_general_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-19 16:20:00.000000 ms_general_utils-1.4.1/ms_general_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 16:20:00.430736 ms_general_utils-1.4.1/ms_utils/
+-rw-rw-rw-   0        0        0      555 2023-03-27 15:14:21.000000 ms_general_utils-1.4.1/ms_utils/__init__.py
+-rw-rw-rw-   0        0        0      386 2023-03-17 12:23:38.000000 ms_general_utils-1.4.1/ms_utils/abstract_model.py
+-rw-rw-rw-   0        0        0     1034 2023-03-17 11:27:17.000000 ms_general_utils-1.4.1/ms_utils/binary_uuid.py
+-rw-rw-rw-   0        0        0      695 2023-03-17 08:52:55.000000 ms_general_utils-1.4.1/ms_utils/func_date.py
+-rw-rw-rw-   0        0        0     2570 2023-04-03 15:04:19.000000 ms_general_utils-1.4.1/ms_utils/generic_crud_class.py
+-rw-rw-rw-   0        0        0      706 2023-03-17 08:52:56.000000 ms_general_utils-1.4.1/ms_utils/generic_pagination.py
+-rw-rw-rw-   0        0        0     1527 2023-04-03 17:16:10.000000 ms_general_utils-1.4.1/ms_utils/model_utils.py
+-rw-rw-rw-   0        0        0      341 2023-03-17 08:52:56.000000 ms_general_utils-1.4.1/ms_utils/prepare_json_response.py
+-rw-rw-rw-   0        0        0      622 2023-05-19 16:18:44.000000 ms_general_utils-1.4.1/ms_utils/validation_utils.py
+-rw-rw-rw-   0        0        0     4472 2023-05-19 16:16:18.000000 ms_general_utils-1.4.1/ms_utils/view_utils.py
+-rw-rw-rw-   0        0        0       42 2023-05-19 16:20:00.457261 ms_general_utils-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      676 2023-05-19 16:19:26.000000 ms_general_utils-1.4.1/setup.py
```

### Comparing `ms_general_utils-1.4/LICENSE.txt` & `ms_general_utils-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4/ms_utils/__init__.py` & `ms_general_utils-1.4.1/ms_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4/ms_utils/binary_uuid.py` & `ms_general_utils-1.4.1/ms_utils/binary_uuid.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4/ms_utils/func_date.py` & `ms_general_utils-1.4.1/ms_utils/func_date.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4/ms_utils/generic_crud_class.py` & `ms_general_utils-1.4.1/ms_utils/generic_crud_class.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4/ms_utils/generic_pagination.py` & `ms_general_utils-1.4.1/ms_utils/generic_pagination.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4/ms_utils/model_utils.py` & `ms_general_utils-1.4.1/ms_utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4/ms_utils/view_utils.py` & `ms_general_utils-1.4.1/ms_utils/view_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,15 +79,20 @@
     def generic_update(model_object, data):
         """
         Generic Update method
         :param data:
         :param model_object:
         :return:
         """
-        model_object.query.filter_by(id=model_object.id).update(data)
+        for key, value in data.items():
+            if hasattr(model_object, key):
+                attribute = getattr(model_object, key)
+                if not hasattr(attribute, '__tablename__'):
+                    # Si el atributo no es una relación
+                    setattr(model_object, key, value)
 
     def generic_details(self, model, schema, object_id):
         """
         Generic details method
         :param schema:
         :param model:
         :param object_id:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ms_general_utils-1.4/setup.py` & `ms_general_utils-1.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ms_general_utils',
     packages=find_packages(),
     include_package_data=True,
-    version='1.4',
+    version='1.4.1',
     description='General functions for the implementation of microservices.',
     authors=[
         {"name": "Alejandro A. Serrano Correa", "email": "alejandroasc93@gmail.com"},
         {"name": "Rene Gonzalez Ramos", "email": "rgramos9310@gmail.com"}
     ],
     license="GPLv3",
     url="https://github.com/rgramos/ms-utils.git",
```

