# Comparing `tmp/ebeer-0.0.6.tar.gz` & `tmp/ebeer-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebeer-0.0.6.tar", last modified: Fri May 19 00:37:42 2023, max compression
+gzip compressed data, was "ebeer-0.0.8.tar", last modified: Fri May 19 18:12:15 2023, max compression
```

## Comparing `ebeer-0.0.6.tar` & `ebeer-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:37:42.803117 ebeer-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-19 00:37:42.803117 ebeer-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-19 00:36:33.000000 ebeer-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-19 00:36:33.000000 ebeer-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 00:37:42.803117 ebeer-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:37:42.803117 ebeer-0.0.6/src/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-19 00:36:33.000000 ebeer-0.0.6/src/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-19 00:36:33.000000 ebeer-0.0.6/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:37:42.803117 ebeer-0.0.6/src/ebeer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-19 00:36:33.000000 ebeer-0.0.6/src/ebeer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-19 00:36:33.000000 ebeer-0.0.6/src/ebeer/beer_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12718 2023-05-19 00:36:33.000000 ebeer-0.0.6/src/ebeer/label_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:37:42.803117 ebeer-0.0.6/src/ebeer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-19 00:37:42.000000 ebeer-0.0.6/src/ebeer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-19 00:37:42.000000 ebeer-0.0.6/src/ebeer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 00:37:42.000000 ebeer-0.0.6/src/ebeer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-19 00:37:42.000000 ebeer-0.0.6/src/ebeer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:37:42.803117 ebeer-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-19 00:36:33.000000 ebeer-0.0.6/tests/test_classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:15.924611 ebeer-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-19 18:12:15.924611 ebeer-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-19 18:11:08.000000 ebeer-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-19 18:11:08.000000 ebeer-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 18:12:15.924611 ebeer-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:15.924611 ebeer-0.0.8/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-19 18:11:08.000000 ebeer-0.0.8/src/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-19 18:11:08.000000 ebeer-0.0.8/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:15.924611 ebeer-0.0.8/src/ebeer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-19 18:11:08.000000 ebeer-0.0.8/src/ebeer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-19 18:11:08.000000 ebeer-0.0.8/src/ebeer/beer_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12718 2023-05-19 18:11:08.000000 ebeer-0.0.8/src/ebeer/label_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:15.924611 ebeer-0.0.8/src/ebeer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-19 18:12:15.000000 ebeer-0.0.8/src/ebeer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-19 18:12:15.000000 ebeer-0.0.8/src/ebeer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:12:15.000000 ebeer-0.0.8/src/ebeer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-19 18:12:15.000000 ebeer-0.0.8/src/ebeer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:12:15.924611 ebeer-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-19 18:11:08.000000 ebeer-0.0.8/tests/test_classify.py
```

### Comparing `ebeer-0.0.6/src/ebeer/beer_classifier.py` & `ebeer-0.0.8/src/ebeer/beer_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class BeerClassifier:
 
     def __init__(self) -> None:
         pass
 
-    def predict(self, img_path):
+    def predict(self, path_img):
 
         width = 128
         height = 128
         size = (width, height)
         channels = 3
         n_neuronios_saida = 20
         learning_rate = 1e-4
@@ -52,19 +52,18 @@
             metrics=[
                 'accuracy',
                 tf.keras.metrics.Precision(),
                 tf.keras.metrics.Recall()
             ]
         )
 
-        # model = keras.models.load_model("trained_model.h5")
         model = keras.models.load_model("src/trained_model/trained_model.h5")
 
         image_original = tf.keras.utils.load_img(
-            img_path,
+            path_img,
             grayscale=False,
             color_mode="rgb",
             target_size=None,
             interpolation="nearest"
         )
 
         image_resized = image_original.resize(size)
```

### Comparing `ebeer-0.0.6/src/ebeer/label_index.py` & `ebeer-0.0.8/src/ebeer/label_index.py`

 * *Files identical despite different names*

