# Comparing `tmp/vecs-0.2.3.tar.gz` & `tmp/vecs-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vecs-0.2.3.tar", last modified: Fri May 19 17:43:56 2023, max compression
+gzip compressed data, was "vecs-0.2.4.tar", last modified: Fri May 19 18:41:22 2023, max compression
```

## Comparing `vecs-0.2.3.tar` & `vecs-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-19 17:43:56.857446 vecs-0.2.3/
--rw-r--r--   0 oliverrice   (501) staff       (20)      743 2023-05-19 17:43:56.857327 vecs-0.2.3/PKG-INFO
--rw-r--r--   0 oliverrice   (501) staff       (20)     2349 2023-05-19 14:53:34.000000 vecs-0.2.3/README.md
--rw-r--r--   0 oliverrice   (501) staff       (20)      154 2023-05-12 13:47:40.000000 vecs-0.2.3/pyproject.toml
--rw-r--r--   0 oliverrice   (501) staff       (20)       38 2023-05-19 17:43:56.857487 vecs-0.2.3/setup.cfg
--rw-r--r--   0 oliverrice   (501) staff       (20)     2222 2023-05-19 14:54:31.000000 vecs-0.2.3/setup.py
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-19 17:43:56.855695 vecs-0.2.3/src/
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-19 17:43:56.856629 vecs-0.2.3/src/vecs/
--rw-r--r--   0 oliverrice   (501) staff       (20)      390 2023-05-19 17:43:33.000000 vecs-0.2.3/src/vecs/__init__.py
--rw-r--r--   0 oliverrice   (501) staff       (20)     1686 2023-05-16 19:39:23.000000 vecs-0.2.3/src/vecs/client.py
--rw-r--r--   0 oliverrice   (501) staff       (20)    13532 2023-05-19 17:42:34.000000 vecs-0.2.3/src/vecs/collection.py
--rw-r--r--   0 oliverrice   (501) staff       (20)      491 2023-05-16 18:21:37.000000 vecs-0.2.3/src/vecs/exc.py
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-19 17:43:56.857169 vecs-0.2.3/src/vecs.egg-info/
--rw-r--r--   0 oliverrice   (501) staff       (20)      743 2023-05-19 17:43:56.000000 vecs-0.2.3/src/vecs.egg-info/PKG-INFO
--rw-r--r--   0 oliverrice   (501) staff       (20)      271 2023-05-19 17:43:56.000000 vecs-0.2.3/src/vecs.egg-info/SOURCES.txt
--rw-r--r--   0 oliverrice   (501) staff       (20)        1 2023-05-19 17:43:56.000000 vecs-0.2.3/src/vecs.egg-info/dependency_links.txt
--rw-r--r--   0 oliverrice   (501) staff       (20)      157 2023-05-19 17:43:56.000000 vecs-0.2.3/src/vecs.egg-info/requires.txt
--rw-r--r--   0 oliverrice   (501) staff       (20)        5 2023-05-19 17:43:56.000000 vecs-0.2.3/src/vecs.egg-info/top_level.txt
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-19 18:41:22.924553 vecs-0.2.4/
+-rw-r--r--   0 oliverrice   (501) staff       (20)      743 2023-05-19 18:41:22.924449 vecs-0.2.4/PKG-INFO
+-rw-r--r--   0 oliverrice   (501) staff       (20)     2349 2023-05-19 14:53:34.000000 vecs-0.2.4/README.md
+-rw-r--r--   0 oliverrice   (501) staff       (20)      154 2023-05-12 13:47:40.000000 vecs-0.2.4/pyproject.toml
+-rw-r--r--   0 oliverrice   (501) staff       (20)       38 2023-05-19 18:41:22.924592 vecs-0.2.4/setup.cfg
+-rw-r--r--   0 oliverrice   (501) staff       (20)     2222 2023-05-19 14:54:31.000000 vecs-0.2.4/setup.py
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-19 18:41:22.922859 vecs-0.2.4/src/
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-19 18:41:22.923756 vecs-0.2.4/src/vecs/
+-rw-r--r--   0 oliverrice   (501) staff       (20)      390 2023-05-19 18:40:57.000000 vecs-0.2.4/src/vecs/__init__.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)     1686 2023-05-16 19:39:23.000000 vecs-0.2.4/src/vecs/client.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)    13532 2023-05-19 18:19:01.000000 vecs-0.2.4/src/vecs/collection.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)      491 2023-05-16 18:21:37.000000 vecs-0.2.4/src/vecs/exc.py
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-19 18:41:22.924297 vecs-0.2.4/src/vecs.egg-info/
+-rw-r--r--   0 oliverrice   (501) staff       (20)      743 2023-05-19 18:41:22.000000 vecs-0.2.4/src/vecs.egg-info/PKG-INFO
+-rw-r--r--   0 oliverrice   (501) staff       (20)      271 2023-05-19 18:41:22.000000 vecs-0.2.4/src/vecs.egg-info/SOURCES.txt
+-rw-r--r--   0 oliverrice   (501) staff       (20)        1 2023-05-19 18:41:22.000000 vecs-0.2.4/src/vecs.egg-info/dependency_links.txt
+-rw-r--r--   0 oliverrice   (501) staff       (20)      157 2023-05-19 18:41:22.000000 vecs-0.2.4/src/vecs.egg-info/requires.txt
+-rw-r--r--   0 oliverrice   (501) staff       (20)        5 2023-05-19 18:41:22.000000 vecs-0.2.4/src/vecs.egg-info/top_level.txt
```

### Comparing `vecs-0.2.3/PKG-INFO` & `vecs-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vecs
-Version: 0.2.3
+Version: 0.2.4
 Summary: pgvector client
 Home-page: https://github.com/supabase/vecs
 Author: Oliver Rice
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
```

### Comparing `vecs-0.2.3/README.md` & `vecs-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `vecs-0.2.3/setup.py` & `vecs-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `vecs-0.2.3/src/vecs/client.py` & `vecs-0.2.4/src/vecs/client.py`

 * *Files identical despite different names*

### Comparing `vecs-0.2.3/src/vecs/collection.py` & `vecs-0.2.4/src/vecs/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,15 +296,15 @@
             pass
 
         with self.client.Session() as sess:
             n_records: int = sess.execute(func.count(self.table.c.id)).scalar()  # type: ignore
 
         with self.client.Session() as sess:
             with sess.begin():
-                n_index_seed = min(1500, n_records)
+                n_index_seed = min(5000, n_records)
                 clone_table.create(sess.connection())
                 stmt_seed_table = clone_table.insert().from_select(
                     self.table.c,
                     select(self.table).order_by(func.random()).limit(n_index_seed),
                 )
                 sess.execute(stmt_seed_table)
```

### Comparing `vecs-0.2.3/src/vecs.egg-info/PKG-INFO` & `vecs-0.2.4/src/vecs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vecs
-Version: 0.2.3
+Version: 0.2.4
 Summary: pgvector client
 Home-page: https://github.com/supabase/vecs
 Author: Oliver Rice
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
```

