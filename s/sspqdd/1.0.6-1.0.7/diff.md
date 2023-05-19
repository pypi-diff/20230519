# Comparing `tmp/sspqdd-1.0.6.tar.gz` & `tmp/sspqdd-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sspqdd-1.0.6.tar", last modified: Wed May 17 15:22:06 2023, max compression
+gzip compressed data, was "sspqdd-1.0.7.tar", last modified: Wed May 17 15:26:45 2023, max compression
```

## Comparing `sspqdd-1.0.6.tar` & `sspqdd-1.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 15:22:06.978876 sspqdd-1.0.6/
--rw-rw-rw-   0        0        0     1088 2023-05-17 15:22:06.977872 sspqdd-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     6293 2023-04-14 13:52:05.000000 sspqdd-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-17 15:22:06.979889 sspqdd-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     2358 2023-05-17 15:21:59.000000 sspqdd-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 15:22:06.963714 sspqdd-1.0.6/sspqdd/
--rw-rw-rw-   0        0        0        0 2023-05-17 10:19:04.000000 sspqdd-1.0.6/sspqdd/__init__.py
--rw-rw-rw-   0        0        0     3809 2023-05-17 11:25:56.000000 sspqdd-1.0.6/sspqdd/sspqdd_pkg.py
-drwxrwxrwx   0        0        0        0 2023-05-17 15:22:06.975352 sspqdd-1.0.6/sspqdd.egg-info/
--rw-rw-rw-   0        0        0     1088 2023-05-17 15:22:06.000000 sspqdd-1.0.6/sspqdd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-05-17 15:22:06.000000 sspqdd-1.0.6/sspqdd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 15:22:06.000000 sspqdd-1.0.6/sspqdd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-17 15:22:06.000000 sspqdd-1.0.6/sspqdd.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 15:26:45.981384 sspqdd-1.0.7/
+-rw-rw-rw-   0        0        0     1088 2023-05-17 15:26:45.981384 sspqdd-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6293 2023-04-14 13:52:05.000000 sspqdd-1.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-17 15:26:45.981384 sspqdd-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     2358 2023-05-17 15:26:38.000000 sspqdd-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 15:26:45.964506 sspqdd-1.0.7/sspqdd/
+-rw-rw-rw-   0        0        0        0 2023-05-17 10:19:04.000000 sspqdd-1.0.7/sspqdd/__init__.py
+-rw-rw-rw-   0        0        0     3809 2023-05-17 11:25:56.000000 sspqdd-1.0.7/sspqdd/sspqdd_pkg.py
+drwxrwxrwx   0        0        0        0 2023-05-17 15:26:45.978912 sspqdd-1.0.7/sspqdd.egg-info/
+-rw-rw-rw-   0        0        0     1088 2023-05-17 15:26:45.000000 sspqdd-1.0.7/sspqdd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-05-17 15:26:45.000000 sspqdd-1.0.7/sspqdd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 15:26:45.000000 sspqdd-1.0.7/sspqdd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-17 15:26:45.000000 sspqdd-1.0.7/sspqdd.egg-info/top_level.txt
```

### Comparing `sspqdd-1.0.6/PKG-INFO` & `sspqdd-1.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sspqdd
-Version: 1.0.6
+Version: 1.0.7
 Summary: Single-Shot-Power-Quality-Disturbance-Detector
 Home-page: UNKNOWN
 Author: Carlos Iturrino-García
 Author-email: carlos.iturrino.garcia@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `sspqdd-1.0.6/README.md` & `sspqdd-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sspqdd-1.0.6/setup.py` & `sspqdd-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup
 
 setup(
     name="sspqdd",
-    version="1.0.6",
+    version="1.0.7",
     description="Single-Shot-Power-Quality-Disturbance-Detector",
     author="Carlos Iturrino-García",
     author_email="carlos.iturrino.garcia@gmail.com",
     packages=["sspqdd"],
     long_description = "Single-Shot-Power-Quality-Disturbance-Detector (SSPQDD) is a Python package that provides a "
                        "comprehensive solution for detection and"
                        " classification of power quality disturbances. It utilizes state-of-the-art deep learning "
                        "algorithms to analyze power signals and identify various types of disturbances, such as voltage"
                        "sags, swells, harmonics, transients, notch and interruptions. The SSPQDD is designed to empower"
                        " engineers and researchers working in the field of power quality analysis. By leveraging "
                        "deep learning techniques, it offers an efficient and accurate approach to automatically detect "
                        "and classify power disturbances, saving time and effort compared to manual inspection. "
                        "With the SSPQDD, users can gain valuable insights into power quality issues and make informed "
                        "decisions for optimal system performance and reliability.",
-    Features = "\n - Detection and classification of power quality disturbances: SSPQDD provides an extensive library of "
+    features = "\n - Detection and classification of power quality disturbances: SSPQDD provides an extensive library of "
                "pre-trained deep learning models capable of identifying various power disturbances with high precision. "
                "\n - Real-time monitoring: It enables real-time analysis of power signals,"
                "allowing for immediate detection and notification of disturbances as they occur."
                "\n - Customizability: Users have the flexibility to fine-tune or retrain the models with their "
                "own datasets to cater to specific power quality analysis requirements. "
                "\n -Visualization and reporting: PowerQDetect offers interactive visualization "
                "tools and comprehensive reporting capabilities to help users interpret the detected disturbances "
```

### Comparing `sspqdd-1.0.6/sspqdd/sspqdd_pkg.py` & `sspqdd-1.0.7/sspqdd/sspqdd_pkg.py`

 * *Files identical despite different names*

### Comparing `sspqdd-1.0.6/sspqdd.egg-info/PKG-INFO` & `sspqdd-1.0.7/sspqdd.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sspqdd
-Version: 1.0.6
+Version: 1.0.7
 Summary: Single-Shot-Power-Quality-Disturbance-Detector
 Home-page: UNKNOWN
 Author: Carlos Iturrino-García
 Author-email: carlos.iturrino.garcia@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
```

