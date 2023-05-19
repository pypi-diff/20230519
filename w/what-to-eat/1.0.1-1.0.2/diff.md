# Comparing `tmp/what_to_eat-1.0.1.tar.gz` & `tmp/what_to_eat-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "what_to_eat-1.0.1.tar", max compression
+gzip compressed data, was "what_to_eat-1.0.2.tar", max compression
```

## Comparing `what_to_eat-1.0.1.tar` & `what_to_eat-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1081 2023-03-29 20:02:20.504670 what_to_eat-1.0.1/LICENSE
--rw-r--r--   0        0        0    12739 2023-03-29 20:02:20.504670 what_to_eat-1.0.1/README.md
--rw-r--r--   0        0        0     1375 2023-03-29 20:02:20.508670 what_to_eat-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      334 2023-03-29 20:02:20.508670 what_to_eat-1.0.1/what_to_eat/__init__.py
--rw-r--r--   0        0        0       52 2023-03-29 20:02:20.508670 what_to_eat-1.0.1/what_to_eat/__main__.py
--rw-r--r--   0        0        0     4032 2023-03-29 20:02:20.508670 what_to_eat-1.0.1/what_to_eat/config.py
--rw-r--r--   0        0        0     2286 2023-03-29 20:02:20.508670 what_to_eat-1.0.1/what_to_eat/controllers.py
--rw-r--r--   0        0        0        0 2023-03-29 20:02:20.508670 what_to_eat-1.0.1/what_to_eat/gateways/__init__.py
--rw-r--r--   0        0        0      542 2023-03-29 20:02:20.508670 what_to_eat-1.0.1/what_to_eat/gateways/location.py
--rw-r--r--   0        0        0     1634 2023-03-29 20:02:20.508670 what_to_eat-1.0.1/what_to_eat/gateways/wolt.py
--rw-r--r--   0        0        0     3338 2023-03-29 20:02:20.508670 what_to_eat-1.0.1/what_to_eat/main.py
--rw-r--r--   0        0        0      582 2023-03-29 20:02:20.508670 what_to_eat-1.0.1/what_to_eat/models/__init__.py
--rw-r--r--   0        0        0      268 2023-03-29 20:02:20.508670 what_to_eat-1.0.1/what_to_eat/models/config.py
--rw-r--r--   0        0        0      108 2023-03-29 20:02:20.508670 what_to_eat-1.0.1/what_to_eat/models/location.py
--rw-r--r--   0        0        0     4764 2023-03-29 20:02:20.508670 what_to_eat-1.0.1/what_to_eat/models/wolt.py
--rw-r--r--   0        0        0        0 2023-03-29 20:02:20.508670 what_to_eat-1.0.1/what_to_eat/services/__init__.py
--rw-r--r--   0        0        0     1969 2023-03-29 20:02:20.508670 what_to_eat-1.0.1/what_to_eat/services/display.py
--rw-r--r--   0        0        0     2641 2023-03-29 20:02:20.508670 what_to_eat-1.0.1/what_to_eat/services/filters.py
--rw-r--r--   0        0        0      912 2023-03-29 20:02:20.508670 what_to_eat-1.0.1/what_to_eat/services/profile.py
--rw-r--r--   0        0        0     2172 2023-03-29 20:02:20.508670 what_to_eat-1.0.1/what_to_eat/services/weights.py
--rw-r--r--   0        0        0        0 2023-03-29 20:02:20.508670 what_to_eat-1.0.1/what_to_eat/utils/__init__.py
--rw-r--r--   0        0        0     1908 2023-03-29 20:02:20.508670 what_to_eat-1.0.1/what_to_eat/utils/cache.py
--rw-r--r--   0        0        0      750 2023-03-29 20:02:20.508670 what_to_eat-1.0.1/what_to_eat/utils/handle.py
--rw-r--r--   0        0        0     1720 2023-03-29 20:02:20.508670 what_to_eat-1.0.1/what_to_eat/utils/prompt.py
--rw-r--r--   0        0        0      555 2023-03-29 20:02:20.508670 what_to_eat-1.0.1/what_to_eat/utils/validators.py
--rw-r--r--   0        0        0    13503 1970-01-01 00:00:00.000000 what_to_eat-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/LICENSE
+-rw-r--r--   0        0        0    12739 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/README.md
+-rw-r--r--   0        0        0     1375 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      334 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/__init__.py
+-rw-r--r--   0        0        0       52 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/__main__.py
+-rw-r--r--   0        0        0     4032 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/config.py
+-rw-r--r--   0        0        0     2286 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/controllers.py
+-rw-r--r--   0        0        0        0 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/gateways/__init__.py
+-rw-r--r--   0        0        0      542 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/gateways/location.py
+-rw-r--r--   0        0        0     1634 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/gateways/wolt.py
+-rw-r--r--   0        0        0     3338 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/main.py
+-rw-r--r--   0        0        0      582 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/models/__init__.py
+-rw-r--r--   0        0        0      268 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/models/config.py
+-rw-r--r--   0        0        0      108 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/models/location.py
+-rw-r--r--   0        0        0     4771 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/models/wolt.py
+-rw-r--r--   0        0        0        0 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/services/__init__.py
+-rw-r--r--   0        0        0     1969 2023-05-19 09:47:34.539432 what_to_eat-1.0.2/what_to_eat/services/display.py
+-rw-r--r--   0        0        0     2641 2023-05-19 09:47:34.539432 what_to_eat-1.0.2/what_to_eat/services/filters.py
+-rw-r--r--   0        0        0      912 2023-05-19 09:47:34.539432 what_to_eat-1.0.2/what_to_eat/services/profile.py
+-rw-r--r--   0        0        0     2172 2023-05-19 09:47:34.539432 what_to_eat-1.0.2/what_to_eat/services/weights.py
+-rw-r--r--   0        0        0        0 2023-05-19 09:47:34.539432 what_to_eat-1.0.2/what_to_eat/utils/__init__.py
+-rw-r--r--   0        0        0     1908 2023-05-19 09:47:34.539432 what_to_eat-1.0.2/what_to_eat/utils/cache.py
+-rw-r--r--   0        0        0      761 2023-05-19 09:47:34.539432 what_to_eat-1.0.2/what_to_eat/utils/handle.py
+-rw-r--r--   0        0        0     1720 2023-05-19 09:47:34.539432 what_to_eat-1.0.2/what_to_eat/utils/prompt.py
+-rw-r--r--   0        0        0      555 2023-05-19 09:47:34.539432 what_to_eat-1.0.2/what_to_eat/utils/validators.py
+-rw-r--r--   0        0        0    13503 1970-01-01 00:00:00.000000 what_to_eat-1.0.2/PKG-INFO
```

### Comparing `what_to_eat-1.0.1/LICENSE` & `what_to_eat-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.1/README.md` & `what_to_eat-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.1/pyproject.toml` & `what_to_eat-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "what-to-eat"
-version = "1.0.1"
+version = "1.0.2"
 description = "What to eat? CLI tool to interaction with Wolt API"
 authors = ["Kamil Woźniak <info@kamilwozniak.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 what-to-eat = "what_to_eat.main:app"
```

### Comparing `what_to_eat-1.0.1/what_to_eat/config.py` & `what_to_eat-1.0.2/what_to_eat/config.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.1/what_to_eat/controllers.py` & `what_to_eat-1.0.2/what_to_eat/controllers.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.1/what_to_eat/gateways/location.py` & `what_to_eat-1.0.2/what_to_eat/gateways/location.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.1/what_to_eat/gateways/wolt.py` & `what_to_eat-1.0.2/what_to_eat/gateways/wolt.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.1/what_to_eat/main.py` & `what_to_eat-1.0.2/what_to_eat/main.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.1/what_to_eat/models/__init__.py` & `what_to_eat-1.0.2/what_to_eat/models/__init__.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.1/what_to_eat/models/wolt.py` & `what_to_eat-1.0.2/what_to_eat/models/wolt.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 class Venue(HashableModel):
     name: str
     address: str
     country: str
     currency: str
     delivery_price_int: int
-    estimate_range: str
+    estimate_range: str | None
     estimate: float
     delivers: bool
     short_description: str | None
     tags: list[str]
     rating: Rating | None
     price_range: int
```

### Comparing `what_to_eat-1.0.1/what_to_eat/services/display.py` & `what_to_eat-1.0.2/what_to_eat/services/display.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.1/what_to_eat/services/filters.py` & `what_to_eat-1.0.2/what_to_eat/services/filters.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.1/what_to_eat/services/profile.py` & `what_to_eat-1.0.2/what_to_eat/services/profile.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.1/what_to_eat/services/weights.py` & `what_to_eat-1.0.2/what_to_eat/services/weights.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.1/what_to_eat/utils/cache.py` & `what_to_eat-1.0.2/what_to_eat/utils/cache.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.1/what_to_eat/utils/prompt.py` & `what_to_eat-1.0.2/what_to_eat/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.1/what_to_eat/utils/validators.py` & `what_to_eat-1.0.2/what_to_eat/utils/validators.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.1/PKG-INFO` & `what_to_eat-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: what-to-eat
-Version: 1.0.1
+Version: 1.0.2
 Summary: What to eat? CLI tool to interaction with Wolt API
 Author: Kamil Woźniak
 Author-email: info@kamilwozniak.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

