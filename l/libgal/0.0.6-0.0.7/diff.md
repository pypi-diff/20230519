# Comparing `tmp/libgal-0.0.6.tar.gz` & `tmp/libgal-0.0.7.tar.gz`

## Comparing `libgal-0.0.6.tar` & `libgal-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 libgal-0.0.6/__init__.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 libgal-0.0.6/gitignore
--rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 libgal-0.0.6/libgal.py
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 libgal-0.0.6/libgal.py.bak
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 libgal-0.0.6/pyproject.toml.bak
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 libgal-0.0.6/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libgal-0.0.6/libgal_package/libgal/__init__.py.bak
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 libgal-0.0.6/libgal_package/libgal/libgal.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 libgal-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0    12034 2020-02-02 00:00:00.000000 libgal-0.0.6/README.md
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 libgal-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    13669 2020-02-02 00:00:00.000000 libgal-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 libgal-0.0.7/__init__.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 libgal-0.0.7/gitignore
+-rw-r--r--   0        0        0     5267 2020-02-02 00:00:00.000000 libgal-0.0.7/libgal.py
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 libgal-0.0.7/libgal.py.bak
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 libgal-0.0.7/pyproject.toml.bak
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 libgal-0.0.7/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libgal-0.0.7/libgal_package/libgal/__init__.py.bak
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 libgal-0.0.7/libgal_package/libgal/libgal.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 libgal-0.0.7/LICENSE.txt
+-rw-r--r--   0        0        0    12034 2020-02-02 00:00:00.000000 libgal-0.0.7/README.md
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 libgal-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    13669 2020-02-02 00:00:00.000000 libgal-0.0.7/PKG-INFO
```

### Comparing `libgal-0.0.6/libgal.py` & `libgal-0.0.7/libgal.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         
     from bs4 import BeautifulSoup
 
     #Teradata
     import teradatasql
     
     #Variables de entrono
-    from dotenv import load_dotenv
+    from dotenv import load_dotenv, find_dotenv
 
     #SQLALchemy
     from sqlalchemy import create_engine, Column, Integer, String, text
     from sqlalchemy.orm import sessionmaker
     from sqlalchemy.ext.declarative import declarative_base
     
 except ImportError as imp_err:
@@ -46,15 +46,17 @@
     Parámetro:
     - path_env_file (String): 
     """
     
     if path_env_file:
         load_dotenv(path_env_file)
     else:
-        load_dotenv()
+        path_env=find_dotenv()
+        if path_env:
+            load_dotenv(path_env)
     
     return dict(os.environ)
     
     
 def logger(format_output="JSON", app_name=__name__):
     
     """
```

### Comparing `libgal-0.0.6/libgal.py.bak` & `libgal-0.0.7/libgal.py.bak`

 * *Files identical despite different names*

### Comparing `libgal-0.0.6/pyproject.toml.bak` & `libgal-0.0.7/pyproject.toml.bak`

 * *Files identical despite different names*

### Comparing `libgal-0.0.6/libgal_package/libgal/libgal.py` & `libgal-0.0.7/libgal_package/libgal/libgal.py`

 * *Files identical despite different names*

### Comparing `libgal-0.0.6/LICENSE.txt` & `libgal-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `libgal-0.0.6/README.md` & `libgal-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `libgal-0.0.6/pyproject.toml` & `libgal-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "libgal"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Jean Manuel González Mejía", email="ebrainding@gmail.com" },
 ]
 
 license = { file = "LICENSE.txt" }
 
 description = "Librería para agilizar el desarrollo de nuestros programadores en el Banco Galicia"
```

### Comparing `libgal-0.0.6/PKG-INFO` & `libgal-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libgal
-Version: 0.0.6
+Version: 0.0.7
 Summary: Librería para agilizar el desarrollo de nuestros programadores en el Banco Galicia
 Project-URL: Homepage, https://github.com/Banco-Galicia/libgal
 Project-URL: Bug Tracker, https://github.com/Banco-Galicia/libgal/issues
 Author-email: Jean Manuel González Mejía <ebrainding@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 JEAN MANUEL GONZÁLEZ MEJÍA
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: libgal Version: 0.0.6 Summary: LibrerÃ­a para
+Metadata-Version: 2.1 Name: libgal Version: 0.0.7 Summary: LibrerÃ­a para
 agilizar el desarrollo de nuestros programadores en el Banco Galicia Project-
 URL: Homepage, https://github.com/Banco-Galicia/libgal Project-URL: Bug
 Tracker, https://github.com/Banco-Galicia/libgal/issues Author-email: Jean
 Manuel GonzÃ¡lez MejÃ­a
 gmail.com> License: MIT License Copyright (c) 2022 JEAN MANUEL GONZÃLEZ MEJÃA
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
```

