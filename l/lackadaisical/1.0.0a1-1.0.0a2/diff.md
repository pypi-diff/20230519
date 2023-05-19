# Comparing `tmp/lackadaisical-1.0.0a1-py3-none-any.whl.zip` & `tmp/lackadaisical-1.0.0a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 4276 bytes, number of entries: 11
--rw-r--r--  2.0 unx        8 b- defN 23-May-17 16:46 lackadaisical/VERSION
--rw-r--r--  2.0 unx     1167 b- defN 23-May-17 16:46 lackadaisical/__init__.py
--rw-r--r--  2.0 unx      359 b- defN 23-May-17 16:46 lackadaisical/faster_than.py
--rw-r--r--  2.0 unx       67 b- defN 23-May-17 16:46 lackadaisical/logging.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-17 16:46 lackadaisical/py.typed
--rw-r--r--  2.0 unx      368 b- defN 23-May-17 16:46 lackadaisical/too_slow.py
--rw-r--r--  2.0 unx     1073 b- defN 23-May-17 16:46 lackadaisical-1.0.0a1.dist-info/LICENSE
--rw-r--r--  2.0 unx      880 b- defN 23-May-17 16:46 lackadaisical-1.0.0a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-17 16:46 lackadaisical-1.0.0a1.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-May-17 16:46 lackadaisical-1.0.0a1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      902 b- defN 23-May-17 16:46 lackadaisical-1.0.0a1.dist-info/RECORD
+-rw-r--r--  2.0 unx        8 b- defN 23-May-18 08:08 lackadaisical/VERSION
+-rw-r--r--  2.0 unx     1167 b- defN 23-May-18 08:08 lackadaisical/__init__.py
+-rw-r--r--  2.0 unx      359 b- defN 23-May-18 08:08 lackadaisical/faster_than.py
+-rw-r--r--  2.0 unx       67 b- defN 23-May-18 08:08 lackadaisical/logging.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-18 08:08 lackadaisical/py.typed
+-rw-r--r--  2.0 unx      368 b- defN 23-May-18 08:08 lackadaisical/too_slow.py
+-rw-r--r--  2.0 unx     1073 b- defN 23-May-18 08:08 lackadaisical-1.0.0a2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      880 b- defN 23-May-18 08:08 lackadaisical-1.0.0a2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-18 08:08 lackadaisical-1.0.0a2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-May-18 08:08 lackadaisical-1.0.0a2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      902 b- defN 23-May-18 08:08 lackadaisical-1.0.0a2.dist-info/RECORD
 11 files, 4930 bytes uncompressed, 2730 bytes compressed:  44.6%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: lackadaisical/py.typed
 Comment: 
 
 Filename: lackadaisical/too_slow.py
 Comment: 
 
-Filename: lackadaisical-1.0.0a1.dist-info/LICENSE
+Filename: lackadaisical-1.0.0a2.dist-info/LICENSE
 Comment: 
 
-Filename: lackadaisical-1.0.0a1.dist-info/METADATA
+Filename: lackadaisical-1.0.0a2.dist-info/METADATA
 Comment: 
 
-Filename: lackadaisical-1.0.0a1.dist-info/WHEEL
+Filename: lackadaisical-1.0.0a2.dist-info/WHEEL
 Comment: 
 
-Filename: lackadaisical-1.0.0a1.dist-info/top_level.txt
+Filename: lackadaisical-1.0.0a2.dist-info/top_level.txt
 Comment: 
 
-Filename: lackadaisical-1.0.0a1.dist-info/RECORD
+Filename: lackadaisical-1.0.0a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lackadaisical/VERSION

```diff
@@ -1 +1 @@
-1.0.0a1
+1.0.0a2
```

## Comparing `lackadaisical-1.0.0a1.dist-info/LICENSE` & `lackadaisical-1.0.0a2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `lackadaisical-1.0.0a1.dist-info/METADATA` & `lackadaisical-1.0.0a2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lackadaisical
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Keeps an eye on slow tests
 Author: Cariad Eccleston
 Author-email: cariad@cariad.earth
 License: MIT
 Project-URL: Documentation, https://cariad.github.io/lackadaisical/lackadaisical.html
 Project-URL: Source, https://github.com/cariad/lackadaisical
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `lackadaisical-1.0.0a1.dist-info/RECORD` & `lackadaisical-1.0.0a2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-lackadaisical/VERSION,sha256=AenaELWTGI1sRzTLSXUhGM9eVEZ_jM3fw0ZRlN1Yzsc,8
+lackadaisical/VERSION,sha256=LXUCGsKHGGt0wefNXJd79GwVqjrn4sseR1ce6an5XIY,8
 lackadaisical/__init__.py,sha256=97kd_ckRTm4dZrW1btjjsIpsMxugkEtWzc8kgR6Qc7s,1167
 lackadaisical/faster_than.py,sha256=MiX8eXyel7D_jM7P7vlRwhX2ucOrBGiYbCbUSSM3m8I,359
 lackadaisical/logging.py,sha256=sNW5CzWbjJq_QFfvS8UjrjNZrYwpa5O6VoNJ3CWmYEo,67
 lackadaisical/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lackadaisical/too_slow.py,sha256=KYqSJjSi91L8Yh4G8zJd3691-h5gl6bAk2diUbhhEew,368
-lackadaisical-1.0.0a1.dist-info/LICENSE,sha256=jXz8xZq3cMjXXQ2Hb9sj6RNKFigwHmut-OnbWc-uHOU,1073
-lackadaisical-1.0.0a1.dist-info/METADATA,sha256=1JXw1kfCu0ETG7lMYtlqNQ0vRTsbxfmjLhXzR-7zEzQ,880
-lackadaisical-1.0.0a1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-lackadaisical-1.0.0a1.dist-info/top_level.txt,sha256=Rf4_1coYZpMJ35dacwQtLPJLW16DM98lWHwuEQ5nmRw,14
-lackadaisical-1.0.0a1.dist-info/RECORD,,
+lackadaisical-1.0.0a2.dist-info/LICENSE,sha256=jXz8xZq3cMjXXQ2Hb9sj6RNKFigwHmut-OnbWc-uHOU,1073
+lackadaisical-1.0.0a2.dist-info/METADATA,sha256=Cu1JgNkWBDaLlIFocscibKfsUXLNY4oq42KvgwjrJUI,880
+lackadaisical-1.0.0a2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+lackadaisical-1.0.0a2.dist-info/top_level.txt,sha256=Rf4_1coYZpMJ35dacwQtLPJLW16DM98lWHwuEQ5nmRw,14
+lackadaisical-1.0.0a2.dist-info/RECORD,,
```

