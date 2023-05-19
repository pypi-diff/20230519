# Comparing `tmp/vecs-0.2.2.tar.gz` & `tmp/vecs-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vecs-0.2.2.tar", last modified: Wed May 17 23:24:14 2023, max compression
+gzip compressed data, was "vecs-0.2.3.tar", last modified: Fri May 19 17:43:56 2023, max compression
```

## Comparing `vecs-0.2.2.tar` & `vecs-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-17 23:24:14.207342 vecs-0.2.2/
--rw-r--r--   0 oliverrice   (501) staff       (20)      742 2023-05-17 23:24:14.207219 vecs-0.2.2/PKG-INFO
--rw-r--r--   0 oliverrice   (501) staff       (20)     6013 2023-05-17 19:24:32.000000 vecs-0.2.2/README.md
--rw-r--r--   0 oliverrice   (501) staff       (20)      154 2023-05-12 13:47:40.000000 vecs-0.2.2/pyproject.toml
--rw-r--r--   0 oliverrice   (501) staff       (20)       38 2023-05-17 23:24:14.207394 vecs-0.2.2/setup.cfg
--rw-r--r--   0 oliverrice   (501) staff       (20)     2221 2023-05-17 23:23:18.000000 vecs-0.2.2/setup.py
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-17 23:24:14.204907 vecs-0.2.2/src/
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-17 23:24:14.206354 vecs-0.2.2/src/vecs/
--rw-r--r--   0 oliverrice   (501) staff       (20)      390 2023-05-17 23:23:39.000000 vecs-0.2.2/src/vecs/__init__.py
--rw-r--r--   0 oliverrice   (501) staff       (20)     1686 2023-05-16 19:39:23.000000 vecs-0.2.2/src/vecs/client.py
--rw-r--r--   0 oliverrice   (501) staff       (20)    13522 2023-05-17 19:04:04.000000 vecs-0.2.2/src/vecs/collection.py
--rw-r--r--   0 oliverrice   (501) staff       (20)      491 2023-05-16 18:21:37.000000 vecs-0.2.2/src/vecs/exc.py
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-17 23:24:14.207053 vecs-0.2.2/src/vecs.egg-info/
--rw-r--r--   0 oliverrice   (501) staff       (20)      742 2023-05-17 23:24:14.000000 vecs-0.2.2/src/vecs.egg-info/PKG-INFO
--rw-r--r--   0 oliverrice   (501) staff       (20)      271 2023-05-17 23:24:14.000000 vecs-0.2.2/src/vecs.egg-info/SOURCES.txt
--rw-r--r--   0 oliverrice   (501) staff       (20)        1 2023-05-17 23:24:14.000000 vecs-0.2.2/src/vecs.egg-info/dependency_links.txt
--rw-r--r--   0 oliverrice   (501) staff       (20)      157 2023-05-17 23:24:14.000000 vecs-0.2.2/src/vecs.egg-info/requires.txt
--rw-r--r--   0 oliverrice   (501) staff       (20)        5 2023-05-17 23:24:14.000000 vecs-0.2.2/src/vecs.egg-info/top_level.txt
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-19 17:43:56.857446 vecs-0.2.3/
+-rw-r--r--   0 oliverrice   (501) staff       (20)      743 2023-05-19 17:43:56.857327 vecs-0.2.3/PKG-INFO
+-rw-r--r--   0 oliverrice   (501) staff       (20)     2349 2023-05-19 14:53:34.000000 vecs-0.2.3/README.md
+-rw-r--r--   0 oliverrice   (501) staff       (20)      154 2023-05-12 13:47:40.000000 vecs-0.2.3/pyproject.toml
+-rw-r--r--   0 oliverrice   (501) staff       (20)       38 2023-05-19 17:43:56.857487 vecs-0.2.3/setup.cfg
+-rw-r--r--   0 oliverrice   (501) staff       (20)     2222 2023-05-19 14:54:31.000000 vecs-0.2.3/setup.py
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-19 17:43:56.855695 vecs-0.2.3/src/
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-19 17:43:56.856629 vecs-0.2.3/src/vecs/
+-rw-r--r--   0 oliverrice   (501) staff       (20)      390 2023-05-19 17:43:33.000000 vecs-0.2.3/src/vecs/__init__.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)     1686 2023-05-16 19:39:23.000000 vecs-0.2.3/src/vecs/client.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)    13532 2023-05-19 17:42:34.000000 vecs-0.2.3/src/vecs/collection.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)      491 2023-05-16 18:21:37.000000 vecs-0.2.3/src/vecs/exc.py
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-19 17:43:56.857169 vecs-0.2.3/src/vecs.egg-info/
+-rw-r--r--   0 oliverrice   (501) staff       (20)      743 2023-05-19 17:43:56.000000 vecs-0.2.3/src/vecs.egg-info/PKG-INFO
+-rw-r--r--   0 oliverrice   (501) staff       (20)      271 2023-05-19 17:43:56.000000 vecs-0.2.3/src/vecs.egg-info/SOURCES.txt
+-rw-r--r--   0 oliverrice   (501) staff       (20)        1 2023-05-19 17:43:56.000000 vecs-0.2.3/src/vecs.egg-info/dependency_links.txt
+-rw-r--r--   0 oliverrice   (501) staff       (20)      157 2023-05-19 17:43:56.000000 vecs-0.2.3/src/vecs.egg-info/requires.txt
+-rw-r--r--   0 oliverrice   (501) staff       (20)        5 2023-05-19 17:43:56.000000 vecs-0.2.3/src/vecs.egg-info/top_level.txt
```

### Comparing `vecs-0.2.2/PKG-INFO` & `vecs-0.2.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: vecs
-Version: 0.2.2
+Version: 0.2.3
 Summary: pgvector client
-Home-page: https://github.com/olirice/vecs
+Home-page: https://github.com/supabase/vecs
 Author: Oliver Rice
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `vecs-0.2.2/setup.py` & `vecs-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 ]
 
 
 setuptools.setup(
     name=read_package_variable("__project__"),
     version=read_package_variable("__version__"),
     description="pgvector client",
-    url="https://github.com/olirice/vecs",
+    url="https://github.com/supabase/vecs",
     author="Oliver Rice",
     packages=setuptools.find_packages("src", exclude="tests"),
     package_dir={"": "src"},
     package_data={"": ["py.typed"]},
     tests_require=["pytest"],
     license="MIT",
     classifiers=[
```

### Comparing `vecs-0.2.2/src/vecs/client.py` & `vecs-0.2.3/src/vecs/client.py`

 * *Files identical despite different names*

### Comparing `vecs-0.2.2/src/vecs/collection.py` & `vecs-0.2.3/src/vecs/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,17 +305,17 @@
                 stmt_seed_table = clone_table.insert().from_select(
                     self.table.c,
                     select(self.table).order_by(func.random()).limit(n_index_seed),
                 )
                 sess.execute(stmt_seed_table)
 
                 n_lists = (
-                    max(n_records / 1000, 30)
+                    int(max(n_records / 1000, 30))
                     if n_records < 1_000_000
-                    else math.sqrt(n_records)
+                    else int(math.sqrt(n_records))
                 )
 
                 unique_string = str(uuid.uuid4()).replace("-", "_")[0:7]
 
                 sess.execute(
                     text(
                         f"""
```

### Comparing `vecs-0.2.2/src/vecs.egg-info/PKG-INFO` & `vecs-0.2.3/src/vecs.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: vecs
-Version: 0.2.2
+Version: 0.2.3
 Summary: pgvector client
-Home-page: https://github.com/olirice/vecs
+Home-page: https://github.com/supabase/vecs
 Author: Oliver Rice
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

