# Comparing `tmp/betwatch-1.0.4.tar.gz` & `tmp/betwatch-1.0.5.tar.gz`

## Comparing `betwatch-1.0.4.tar` & `betwatch-1.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 betwatch-1.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 betwatch-1.0.4/Makefile
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.0.4/.github/dependabot.yml
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 betwatch-1.0.4/.github/workflows/test.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 betwatch-1.0.4/betwatch/__about__.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 betwatch-1.0.4/betwatch/__init__.py
--rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 betwatch-1.0.4/betwatch/client.py
--rw-r--r--   0        0        0    26499 2020-02-02 00:00:00.000000 betwatch-1.0.4/betwatch/client_async.py
--rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 betwatch-1.0.4/betwatch/queries.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.0.4/betwatch/types/__init__.py
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 betwatch-1.0.4/betwatch/types/bookmakers.py
--rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 betwatch-1.0.4/betwatch/types/filters.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 betwatch-1.0.4/betwatch/types/markets.py
--rw-r--r--   0        0        0    12489 2020-02-02 00:00:00.000000 betwatch-1.0.4/betwatch/types/race.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.0.4/betwatch/types/updates.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 betwatch-1.0.4/examples/get_race_prices.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 betwatch-1.0.4/examples/get_race_prices_async.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 betwatch-1.0.4/examples/get_races.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 betwatch-1.0.4/examples/get_races_async.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 betwatch-1.0.4/examples/subscriptions.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 betwatch-1.0.4/examples/update_rated_prices.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.0.4/tests/__init__.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 betwatch-1.0.4/tests/test_check_last_updated.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 betwatch-1.0.4/tests/test_get_race.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 betwatch-1.0.4/tests/test_get_race_async.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 betwatch-1.0.4/tests/test_get_races.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 betwatch-1.0.4/tests/test_get_races_async.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 betwatch-1.0.4/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.0.4/LICENSE.txt
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.0.4/README.md
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 betwatch-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 betwatch-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 betwatch-1.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 betwatch-1.0.5/Makefile
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.0.5/.github/dependabot.yml
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 betwatch-1.0.5/.github/workflows/test.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 betwatch-1.0.5/betwatch/__about__.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 betwatch-1.0.5/betwatch/__init__.py
+-rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 betwatch-1.0.5/betwatch/client.py
+-rw-r--r--   0        0        0    26499 2020-02-02 00:00:00.000000 betwatch-1.0.5/betwatch/client_async.py
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 betwatch-1.0.5/betwatch/queries.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.0.5/betwatch/types/__init__.py
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 betwatch-1.0.5/betwatch/types/bookmakers.py
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 betwatch-1.0.5/betwatch/types/filters.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 betwatch-1.0.5/betwatch/types/markets.py
+-rw-r--r--   0        0        0    12489 2020-02-02 00:00:00.000000 betwatch-1.0.5/betwatch/types/race.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.0.5/betwatch/types/updates.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 betwatch-1.0.5/examples/get_race_prices.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 betwatch-1.0.5/examples/get_race_prices_async.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 betwatch-1.0.5/examples/get_races.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 betwatch-1.0.5/examples/get_races_async.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 betwatch-1.0.5/examples/subscriptions.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 betwatch-1.0.5/examples/update_rated_prices.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.0.5/tests/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 betwatch-1.0.5/tests/test_check_last_updated.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 betwatch-1.0.5/tests/test_get_race.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 betwatch-1.0.5/tests/test_get_race_async.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 betwatch-1.0.5/tests/test_get_races.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 betwatch-1.0.5/tests/test_get_races_async.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 betwatch-1.0.5/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.0.5/LICENSE.txt
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.0.5/README.md
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 betwatch-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 betwatch-1.0.5/PKG-INFO
```

### Comparing `betwatch-1.0.4/.github/workflows/test.yml` & `betwatch-1.0.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.4/betwatch/__init__.py` & `betwatch-1.0.5/betwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.4/betwatch/client.py` & `betwatch-1.0.5/betwatch/client.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.4/betwatch/client_async.py` & `betwatch-1.0.5/betwatch/client_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.4/betwatch/queries.py` & `betwatch-1.0.5/betwatch/queries.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.4/betwatch/types/bookmakers.py` & `betwatch-1.0.5/betwatch/types/bookmakers.py`

 * *Files 19% similar despite different names*

```diff
@@ -84,7 +84,21 @@
     THUNDERBET = "Thunderbet"
     ESKANDERBET = "EskanderBet"
     SPORTCHAMPS = "SportChamps"
     SURGE = "Surge"
 
     def __str__(self):
         return self.value
+    
+    def __repr__(self):
+        return self.value
+    
+    def __eq__(self, other):
+        if isinstance(other, Bookmaker):
+            return self.value == other.value
+        elif isinstance(other, str):
+            return self.value == other
+        else:
+            return False
+        
+    def __hash__(self):
+        return hash(self.value)
```

### Comparing `betwatch-1.0.4/betwatch/types/filters.py` & `betwatch-1.0.5/betwatch/types/filters.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.4/betwatch/types/markets.py` & `betwatch-1.0.5/betwatch/types/markets.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.4/betwatch/types/race.py` & `betwatch-1.0.5/betwatch/types/race.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.4/examples/get_race_prices.py` & `betwatch-1.0.5/examples/get_race_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.4/examples/get_race_prices_async.py` & `betwatch-1.0.5/examples/get_race_prices_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.4/examples/get_races.py` & `betwatch-1.0.5/examples/get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.4/examples/get_races_async.py` & `betwatch-1.0.5/examples/get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.4/examples/subscriptions.py` & `betwatch-1.0.5/examples/subscriptions.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.4/examples/update_rated_prices.py` & `betwatch-1.0.5/examples/update_rated_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.4/tests/test_get_race.py` & `betwatch-1.0.5/tests/test_get_race.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.4/tests/test_get_race_async.py` & `betwatch-1.0.5/tests/test_get_race_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.4/tests/test_get_races.py` & `betwatch-1.0.5/tests/test_get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.4/tests/test_get_races_async.py` & `betwatch-1.0.5/tests/test_get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.4/.gitignore` & `betwatch-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.4/LICENSE.txt` & `betwatch-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.4/README.md` & `betwatch-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.4/pyproject.toml` & `betwatch-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.4/PKG-INFO` & `betwatch-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betwatch
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python package for interacting with the Betwatch.com API
 Project-URL: Documentation, https://github.com/betwatch/betwatch-sdk-python#readme
 Project-URL: Issues, https://github.com/betwatch/betwatch-sdk-python/issues
 Project-URL: Source, https://github.com/betwatch/betwatch-sdk-python
 Project-URL: Betwatch.com, https://betwatch.com
 Author-email: Jamie Watts <jamie@betwatch.com>
 License-File: LICENSE.txt
```

