# Comparing `tmp/hyper_requests-0.0.3.tar.gz` & `tmp/hyper_requests-0.0.4.tar.gz`

## Comparing `hyper_requests-0.0.3.tar` & `hyper_requests-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 hyper_requests-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hyper_requests-0.0.3/MANIFEST.in
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 hyper_requests-0.0.3/requirements.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 hyper_requests-0.0.3/setup.cfg
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 hyper_requests-0.0.3/.github/workflows/python-package-conda.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hyper_requests-0.0.3/hyper_requests/__init__.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 hyper_requests-0.0.3/hyper_requests/request_builder.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 hyper_requests-0.0.3/hyper_requests/threader.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 hyper_requests-0.0.3/test/performance/test_performance.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 hyper_requests-0.0.3/test/unit/test_check_request_params.py
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 hyper_requests-0.0.3/test/unit/test_threader.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 hyper_requests-0.0.3/test/unit/test_threader_setup.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 hyper_requests-0.0.3/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 hyper_requests-0.0.3/LICENSE
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 hyper_requests-0.0.3/README.md
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 hyper_requests-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 hyper_requests-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/MANIFEST.in
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/setup.cfg
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/.github/workflows/python-package-conda.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/hyper_requests/__init__.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/hyper_requests/request_builder.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/hyper_requests/threader.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/test/performance/test_performance.py
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/test/unit/test_check_request_params.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/test/unit/test_threader.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/test/unit/test_threader_setup.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/README.md
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/PKG-INFO
```

### Comparing `hyper_requests-0.0.3/.pre-commit-config.yaml` & `hyper_requests-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.3/.github/workflows/python-package-conda.yml` & `hyper_requests-0.0.4/.github/workflows/python-package-conda.yml`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.3/hyper_requests/request_builder.py` & `hyper_requests-0.0.4/hyper_requests/request_builder.py`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.3/hyper_requests/threader.py` & `hyper_requests-0.0.4/hyper_requests/threader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 from concurrent.futures import ThreadPoolExecutor
 
 import nest_asyncio
 import requests
-from src.request_builder import check_request_params
+
+from hyper_requests.request_builder import check_request_params
 
 nest_asyncio.apply()
 
 
 class AsyncRequests:
     """Using asyncio this allows for multithreading of API calls. Pass in a list of URLs and a list of parameters."""
```

### Comparing `hyper_requests-0.0.3/test/performance/test_performance.py` & `hyper_requests-0.0.4/test/performance/test_performance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 import unittest
 
 import requests
 
-from src.threader import AsyncRequests
+from hyper_requests.threader import AsyncRequests
 
 
 class PerformanceTest(unittest.TestCase):
     def test_api_performance(self):
         api_calls = 20
         request_params = [
             {"url": "https://official-joke-api.appspot.com/random_joke"}
```

### Comparing `hyper_requests-0.0.3/test/unit/test_check_request_params.py` & `hyper_requests-0.0.4/test/unit/test_check_request_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from src.request_builder import check_request_params
+from hyper_requests.request_builder import check_request_params
 
 
 class TestCheckRequestParams(unittest.TestCase):
     def test_valid_request_parameters(self):
         request_parameters = [
             {"url": "https://example.com", "method": "GET"},
             {"url": "https://example.org", "headers": "Content-Type: application/json"},
```

### Comparing `hyper_requests-0.0.3/test/unit/test_threader.py` & `hyper_requests-0.0.4/test/unit/test_threader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from src.threader import AsyncRequests
+from hyper_requests.threader import AsyncRequests
 
 
 class TestThreading(unittest.TestCase):
     """Uses the overpass openstreet map api to see if two requests with different parameters can be multithreaded"""
 
     def setUp(self):
         self.request_params1 = [
@@ -41,9 +41,8 @@
         ]
         self.api2 = AsyncRequests(self.request_params2)
 
     def test_run_api1_threads_with_params(self):
         self.assertIsNotNone(self.api1.run_threads())
 
     def test_run_api2_threads_just_url(self):
-        print(self.api2.run_threads())
         self.assertIsNotNone(self.api2.run_threads())
```

### Comparing `hyper_requests-0.0.3/test/unit/test_threader_setup.py` & `hyper_requests-0.0.4/test/unit/test_threader_setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from unittest.mock import MagicMock
 
 import requests
 
-from src.threader import AsyncRequests
+from hyper_requests.threader import AsyncRequests
 
 
 class TestThreadingSetup(unittest.TestCase):
     def setUp(self):
         self.request_params = [
             {"url": "https://api.example.com/endpoint1", "param": "value1"},
             {"url": "https://api.example.com/endpoint2", "param": "value2"},
```

### Comparing `hyper_requests-0.0.3/.gitignore` & `hyper_requests-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.3/LICENSE` & `hyper_requests-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.3/README.md` & `hyper_requests-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.3/PKG-INFO` & `hyper_requests-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hyper-requests
-Version: 0.0.3
-Summary: Concurrent request HTTP execution librar
+Version: 0.0.4
+Summary: Concurrent request HTTP execution library
 Project-URL: Homepage, https://github.com/edjones84/hyper-requests
 Project-URL: Bug Tracker, https://github.com/edjones84/hyper-requests/issues
 Author-email: Ed Jones <ejones84@icloud.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

