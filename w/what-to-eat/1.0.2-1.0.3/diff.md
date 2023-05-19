# Comparing `tmp/what_to_eat-1.0.2.tar.gz` & `tmp/what_to_eat-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "what_to_eat-1.0.2.tar", max compression
+gzip compressed data, was "what_to_eat-1.0.3.tar", max compression
```

## Comparing `what_to_eat-1.0.2.tar` & `what_to_eat-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1081 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/LICENSE
--rw-r--r--   0        0        0    12739 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/README.md
--rw-r--r--   0        0        0     1375 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      334 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/__init__.py
--rw-r--r--   0        0        0       52 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/__main__.py
--rw-r--r--   0        0        0     4032 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/config.py
--rw-r--r--   0        0        0     2286 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/controllers.py
--rw-r--r--   0        0        0        0 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/gateways/__init__.py
--rw-r--r--   0        0        0      542 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/gateways/location.py
--rw-r--r--   0        0        0     1634 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/gateways/wolt.py
--rw-r--r--   0        0        0     3338 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/main.py
--rw-r--r--   0        0        0      582 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/models/__init__.py
--rw-r--r--   0        0        0      268 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/models/config.py
--rw-r--r--   0        0        0      108 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/models/location.py
--rw-r--r--   0        0        0     4771 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/models/wolt.py
--rw-r--r--   0        0        0        0 2023-05-19 09:47:34.535432 what_to_eat-1.0.2/what_to_eat/services/__init__.py
--rw-r--r--   0        0        0     1969 2023-05-19 09:47:34.539432 what_to_eat-1.0.2/what_to_eat/services/display.py
--rw-r--r--   0        0        0     2641 2023-05-19 09:47:34.539432 what_to_eat-1.0.2/what_to_eat/services/filters.py
--rw-r--r--   0        0        0      912 2023-05-19 09:47:34.539432 what_to_eat-1.0.2/what_to_eat/services/profile.py
--rw-r--r--   0        0        0     2172 2023-05-19 09:47:34.539432 what_to_eat-1.0.2/what_to_eat/services/weights.py
--rw-r--r--   0        0        0        0 2023-05-19 09:47:34.539432 what_to_eat-1.0.2/what_to_eat/utils/__init__.py
--rw-r--r--   0        0        0     1908 2023-05-19 09:47:34.539432 what_to_eat-1.0.2/what_to_eat/utils/cache.py
--rw-r--r--   0        0        0      761 2023-05-19 09:47:34.539432 what_to_eat-1.0.2/what_to_eat/utils/handle.py
--rw-r--r--   0        0        0     1720 2023-05-19 09:47:34.539432 what_to_eat-1.0.2/what_to_eat/utils/prompt.py
--rw-r--r--   0        0        0      555 2023-05-19 09:47:34.539432 what_to_eat-1.0.2/what_to_eat/utils/validators.py
--rw-r--r--   0        0        0    13503 1970-01-01 00:00:00.000000 what_to_eat-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-19 10:19:14.534912 what_to_eat-1.0.3/LICENSE
+-rw-r--r--   0        0        0    12739 2023-05-19 10:19:14.534912 what_to_eat-1.0.3/README.md
+-rw-r--r--   0        0        0     1375 2023-05-19 10:19:14.534912 what_to_eat-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      334 2023-05-19 10:19:14.534912 what_to_eat-1.0.3/what_to_eat/__init__.py
+-rw-r--r--   0        0        0       52 2023-05-19 10:19:14.534912 what_to_eat-1.0.3/what_to_eat/__main__.py
+-rw-r--r--   0        0        0     4032 2023-05-19 10:19:14.534912 what_to_eat-1.0.3/what_to_eat/config.py
+-rw-r--r--   0        0        0     2286 2023-05-19 10:19:14.534912 what_to_eat-1.0.3/what_to_eat/controllers.py
+-rw-r--r--   0        0        0        0 2023-05-19 10:19:14.534912 what_to_eat-1.0.3/what_to_eat/gateways/__init__.py
+-rw-r--r--   0        0        0      542 2023-05-19 10:19:14.534912 what_to_eat-1.0.3/what_to_eat/gateways/location.py
+-rw-r--r--   0        0        0     1634 2023-05-19 10:19:14.534912 what_to_eat-1.0.3/what_to_eat/gateways/wolt.py
+-rw-r--r--   0        0        0     3338 2023-05-19 10:19:14.534912 what_to_eat-1.0.3/what_to_eat/main.py
+-rw-r--r--   0        0        0      810 2023-05-19 10:19:14.534912 what_to_eat-1.0.3/what_to_eat/models/__init__.py
+-rw-r--r--   0        0        0      268 2023-05-19 10:19:14.534912 what_to_eat-1.0.3/what_to_eat/models/config.py
+-rw-r--r--   0        0        0      108 2023-05-19 10:19:14.534912 what_to_eat-1.0.3/what_to_eat/models/location.py
+-rw-r--r--   0        0        0     4771 2023-05-19 10:19:14.534912 what_to_eat-1.0.3/what_to_eat/models/wolt.py
+-rw-r--r--   0        0        0        0 2023-05-19 10:19:14.534912 what_to_eat-1.0.3/what_to_eat/services/__init__.py
+-rw-r--r--   0        0        0     1969 2023-05-19 10:19:14.534912 what_to_eat-1.0.3/what_to_eat/services/display.py
+-rw-r--r--   0        0        0     3747 2023-05-19 10:19:14.534912 what_to_eat-1.0.3/what_to_eat/services/filters.py
+-rw-r--r--   0        0        0      912 2023-05-19 10:19:14.534912 what_to_eat-1.0.3/what_to_eat/services/profile.py
+-rw-r--r--   0        0        0     2172 2023-05-19 10:19:14.534912 what_to_eat-1.0.3/what_to_eat/services/weights.py
+-rw-r--r--   0        0        0        0 2023-05-19 10:19:14.534912 what_to_eat-1.0.3/what_to_eat/utils/__init__.py
+-rw-r--r--   0        0        0     1908 2023-05-19 10:19:14.534912 what_to_eat-1.0.3/what_to_eat/utils/cache.py
+-rw-r--r--   0        0        0      761 2023-05-19 10:19:14.534912 what_to_eat-1.0.3/what_to_eat/utils/handle.py
+-rw-r--r--   0        0        0     1720 2023-05-19 10:19:14.534912 what_to_eat-1.0.3/what_to_eat/utils/prompt.py
+-rw-r--r--   0        0        0      555 2023-05-19 10:19:14.534912 what_to_eat-1.0.3/what_to_eat/utils/validators.py
+-rw-r--r--   0        0        0    13503 1970-01-01 00:00:00.000000 what_to_eat-1.0.3/PKG-INFO
```

### Comparing `what_to_eat-1.0.2/LICENSE` & `what_to_eat-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.2/README.md` & `what_to_eat-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.2/pyproject.toml` & `what_to_eat-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "what-to-eat"
-version = "1.0.2"
+version = "1.0.3"
 description = "What to eat? CLI tool to interaction with Wolt API"
 authors = ["Kamil Woźniak <info@kamilwozniak.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 what-to-eat = "what_to_eat.main:app"
```

### Comparing `what_to_eat-1.0.2/what_to_eat/config.py` & `what_to_eat-1.0.3/what_to_eat/config.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.2/what_to_eat/controllers.py` & `what_to_eat-1.0.3/what_to_eat/controllers.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.2/what_to_eat/gateways/location.py` & `what_to_eat-1.0.3/what_to_eat/gateways/location.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.2/what_to_eat/gateways/wolt.py` & `what_to_eat-1.0.3/what_to_eat/gateways/wolt.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.2/what_to_eat/main.py` & `what_to_eat-1.0.3/what_to_eat/main.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.2/what_to_eat/models/__init__.py` & `what_to_eat-1.0.3/what_to_eat/models/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,19 +7,25 @@
     def __hash__(self) -> int:
         return hash(self.json())
 
 
 class Sort(str, Enum):
     NONE = "none"
     RESTAURANT = "restaurant"
+    INVERTED_RESTAURANT = "-restaurant"
     ADDRESS = "address"
+    INVERTED_ADDRESS = "-address"
     DELIVERY_COST = "delivery_cost"
+    INVERTED_DELIVERY_COST = "-delivery_cost"
     ESTIMATE_TIME = "estimate_time"
+    INVERTED_ESTIMATE_TIME = "-estimate_time"
     RATING = "rating"
+    INVERTED_RATING = "-rating"
     PRICE = "price"
+    INVERTED_PRICE = "-price"
 
     @classmethod
     def choices(cls) -> list[str]:
         return list(cls)
 
 
 class Ordering(str, Enum):
```

### Comparing `what_to_eat-1.0.2/what_to_eat/models/wolt.py` & `what_to_eat-1.0.3/what_to_eat/models/wolt.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.2/what_to_eat/services/display.py` & `what_to_eat-1.0.3/what_to_eat/services/display.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.2/what_to_eat/services/filters.py` & `what_to_eat-1.0.3/what_to_eat/services/filters.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,29 +17,50 @@
 
 @cache.apply()
 def sort_by(items: list[Item], sort: Sort = Sort.NONE, ordering: Ordering = Ordering.ASC) -> list[Item]:
     reverse = ordering == Ordering.DESC.value
     match sort:
         case Sort.RESTAURANT:
             return sorted(items, key=lambda i: i.title, reverse=reverse)
+        case Sort.INVERTED_RESTAURANT:
+            return sorted(items, key=lambda i: i.title, reverse=not reverse)
         case Sort.ADDRESS:
             return sorted(items, key=lambda i: i.venue.address, reverse=reverse)
+        case Sort.INVERTED_ADDRESS:
+            return sorted(items, key=lambda i: i.venue.address, reverse=not reverse)
         case Sort.DELIVERY_COST:
             return sorted(items, key=lambda i: i.venue.estimate_range, reverse=reverse)
+        case Sort.INVERTED_DELIVERY_COST:
+            return sorted(items, key=lambda i: i.venue.estimate_range, reverse=not reverse)
         case Sort.ESTIMATE_TIME:
             return sorted(items, key=lambda i: i.venue.delivery_price_int, reverse=reverse)
+        case Sort.INVERTED_ESTIMATE_TIME:
+            return sorted(items, key=lambda i: i.venue.delivery_price_int, reverse=not reverse)
         case Sort.PRICE:
             return sorted(items, key=lambda i: i.venue.price_range, reverse=reverse)
+        case Sort.INVERTED_PRICE:
+            return sorted(items, key=lambda i: i.venue.price_range, reverse=not reverse)
         case Sort.RATING:
             items_without_rating = list(filter(lambda i: i.venue and not i.venue.rating, items))
             items_with_rating = list(filter(lambda i: i.venue and i.venue.rating, items))
             return (
                 sorted(
                     items_with_rating,
                     key=lambda i: i.venue.rating.score,
+                    reverse=not reverse,
+                )
+                + items_without_rating
+            )
+        case Sort.INVERTED_RATING:
+            items_without_rating = list(filter(lambda i: i.venue and not i.venue.rating, items))
+            items_with_rating = list(filter(lambda i: i.venue and i.venue.rating, items))
+            return (
+                sorted(
+                    items_with_rating,
+                    key=lambda i: i.venue.rating.score,
                     reverse=reverse,
                 )
                 + items_without_rating
             )
         case _:
             return items
```

### Comparing `what_to_eat-1.0.2/what_to_eat/services/profile.py` & `what_to_eat-1.0.3/what_to_eat/services/profile.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.2/what_to_eat/services/weights.py` & `what_to_eat-1.0.3/what_to_eat/services/weights.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.2/what_to_eat/utils/cache.py` & `what_to_eat-1.0.3/what_to_eat/utils/cache.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.2/what_to_eat/utils/handle.py` & `what_to_eat-1.0.3/what_to_eat/utils/handle.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.2/what_to_eat/utils/prompt.py` & `what_to_eat-1.0.3/what_to_eat/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.2/what_to_eat/utils/validators.py` & `what_to_eat-1.0.3/what_to_eat/utils/validators.py`

 * *Files identical despite different names*

### Comparing `what_to_eat-1.0.2/PKG-INFO` & `what_to_eat-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: what-to-eat
-Version: 1.0.2
+Version: 1.0.3
 Summary: What to eat? CLI tool to interaction with Wolt API
 Author: Kamil Woźniak
 Author-email: info@kamilwozniak.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

