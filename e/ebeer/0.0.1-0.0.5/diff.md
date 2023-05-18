# Comparing `tmp/ebeer-0.0.1.tar.gz` & `tmp/ebeer-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebeer-0.0.1.tar", last modified: Thu May 18 15:46:37 2023, max compression
+gzip compressed data, was "ebeer-0.0.5.tar", last modified: Thu May 18 22:01:50 2023, max compression
```

## Comparing `ebeer-0.0.1.tar` & `ebeer-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mal       (1000) mal       (1001)        0 2023-05-18 15:46:37.769154 ebeer-0.0.1/
--rw-r--r--   0 mal       (1000) mal       (1001)      462 2023-05-18 15:46:37.769154 ebeer-0.0.1/PKG-INFO
--rw-r--r--   0 mal       (1000) mal       (1001)      211 2023-05-18 12:45:39.000000 ebeer-0.0.1/README.md
--rw-r--r--   0 mal       (1000) mal       (1001)      493 2023-05-18 13:05:19.000000 ebeer-0.0.1/pyproject.toml
--rw-r--r--   0 mal       (1000) mal       (1001)       38 2023-05-18 15:46:37.769154 ebeer-0.0.1/setup.cfg
-drwxr-xr-x   0 mal       (1000) mal       (1001)        0 2023-05-18 15:46:37.769154 ebeer-0.0.1/src/
--rw-r--r--   0 mal       (1000) mal       (1001)       65 2023-05-18 12:50:43.000000 ebeer-0.0.1/src/README.md
--rw-r--r--   0 mal       (1000) mal       (1001)       34 2023-05-18 13:15:01.000000 ebeer-0.0.1/src/__init__.py
-drwxr-xr-x   0 mal       (1000) mal       (1001)        0 2023-05-18 15:46:37.769154 ebeer-0.0.1/src/ebeer/
--rw-r--r--   0 mal       (1000) mal       (1001)       34 2023-05-18 13:11:31.000000 ebeer-0.0.1/src/ebeer/__init__.py
--rw-r--r--   0 mal       (1000) mal       (1001)     2247 2023-05-18 15:41:26.000000 ebeer-0.0.1/src/ebeer/beer_classifier.py
--rw-r--r--   0 mal       (1000) mal       (1001)    12718 2023-05-18 13:14:28.000000 ebeer-0.0.1/src/ebeer/label_index.py
-drwxr-xr-x   0 mal       (1000) mal       (1001)        0 2023-05-18 15:46:37.769154 ebeer-0.0.1/src/ebeer.egg-info/
--rw-r--r--   0 mal       (1000) mal       (1001)      462 2023-05-18 15:46:37.000000 ebeer-0.0.1/src/ebeer.egg-info/PKG-INFO
--rw-r--r--   0 mal       (1000) mal       (1001)      285 2023-05-18 15:46:37.000000 ebeer-0.0.1/src/ebeer.egg-info/SOURCES.txt
--rw-r--r--   0 mal       (1000) mal       (1001)        1 2023-05-18 15:46:37.000000 ebeer-0.0.1/src/ebeer.egg-info/dependency_links.txt
--rw-r--r--   0 mal       (1000) mal       (1001)       29 2023-05-18 15:46:37.000000 ebeer-0.0.1/src/ebeer.egg-info/top_level.txt
-drwxr-xr-x   0 mal       (1000) mal       (1001)        0 2023-05-18 15:46:37.769154 ebeer-0.0.1/tests/
--rw-r--r--   0 mal       (1000) mal       (1001)      381 2023-05-18 15:43:35.000000 ebeer-0.0.1/tests/test_classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:01:50.282068 ebeer-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-18 22:01:50.282068 ebeer-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-18 22:00:33.000000 ebeer-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-18 22:00:33.000000 ebeer-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 22:01:50.282068 ebeer-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:01:50.282068 ebeer-0.0.5/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-18 22:00:33.000000 ebeer-0.0.5/src/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-18 22:00:33.000000 ebeer-0.0.5/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:01:50.282068 ebeer-0.0.5/src/ebeer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-18 22:00:33.000000 ebeer-0.0.5/src/ebeer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-18 22:00:33.000000 ebeer-0.0.5/src/ebeer/beer_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12718 2023-05-18 22:00:33.000000 ebeer-0.0.5/src/ebeer/label_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:01:50.282068 ebeer-0.0.5/src/ebeer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-18 22:01:50.000000 ebeer-0.0.5/src/ebeer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-18 22:01:50.000000 ebeer-0.0.5/src/ebeer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 22:01:50.000000 ebeer-0.0.5/src/ebeer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-18 22:01:50.000000 ebeer-0.0.5/src/ebeer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:01:50.282068 ebeer-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-18 22:00:33.000000 ebeer-0.0.5/tests/test_classify.py
```

### Comparing `ebeer-0.0.1/src/ebeer/beer_classifier.py` & `ebeer-0.0.5/src/ebeer/beer_classifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,16 @@
             metrics=[
                 'accuracy',
                 tf.keras.metrics.Precision(),
                 tf.keras.metrics.Recall()
             ]
         )
 
-        model = keras.models.load_model('src/trained_model/trained_model.h5')
+        # model = keras.models.load_model("trained_model.h5")
+        model = keras.models.load_model("src/trained_model/trained_model.h5")
 
         image_original = tf.keras.utils.load_img(
             img_path,
             grayscale=False,
             color_mode="rgb",
             target_size=None,
             interpolation="nearest"
@@ -71,12 +72,7 @@
         image_prepared = np.expand_dims(image_resized, axis=0)
 
         predicted = model.predict(image_prepared)
 
         n_pos = predicted.argmax(axis=-1)[0]
 
         return n_pos
-
-        # print("n_pos:", n_pos)
-
-        # print("n_pos:", n_pos, " - label:",
-        #       labels_index[n_pos]["name"], "\n\n")
```

### Comparing `ebeer-0.0.1/src/ebeer/label_index.py` & `ebeer-0.0.5/src/ebeer/label_index.py`

 * *Files identical despite different names*

