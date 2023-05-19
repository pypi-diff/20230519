# Comparing `tmp/hyper_requests-0.0.4.tar.gz` & `tmp/hyper_requests-0.0.5.tar.gz`

## Comparing `hyper_requests-0.0.4.tar` & `hyper_requests-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/MANIFEST.in
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/requirements.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/setup.cfg
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/.github/workflows/python-package-conda.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/hyper_requests/__init__.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/hyper_requests/request_builder.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/hyper_requests/threader.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/test/performance/test_performance.py
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/test/unit/test_check_request_params.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/test/unit/test_threader.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/test/unit/test_threader_setup.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/LICENSE
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/README.md
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 hyper_requests-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/MANIFEST.in
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/setup.cfg
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/.github/workflows/python-package-conda.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/hyper_requests/__init__.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/hyper_requests/request_builder.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/hyper_requests/threader.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/test/performance/test_performance.py
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/test/unit/test_check_request_params.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/test/unit/test_threader.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/test/unit/test_threader_setup.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/README.md
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/PKG-INFO
```

### Comparing `hyper_requests-0.0.4/.pre-commit-config.yaml` & `hyper_requests-0.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.4/.github/workflows/python-package-conda.yml` & `hyper_requests-0.0.5/.github/workflows/python-package-conda.yml`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.4/hyper_requests/request_builder.py` & `hyper_requests-0.0.5/hyper_requests/request_builder.py`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.4/hyper_requests/threader.py` & `hyper_requests-0.0.5/hyper_requests/threader.py`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.4/test/performance/test_performance.py` & `hyper_requests-0.0.5/test/performance/test_performance.py`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.4/test/unit/test_check_request_params.py` & `hyper_requests-0.0.5/test/unit/test_check_request_params.py`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.4/test/unit/test_threader.py` & `hyper_requests-0.0.5/test/unit/test_threader.py`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.4/test/unit/test_threader_setup.py` & `hyper_requests-0.0.5/test/unit/test_threader_setup.py`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.4/.gitignore` & `hyper_requests-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.4/LICENSE` & `hyper_requests-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.4/pyproject.toml` & `hyper_requests-0.0.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "hyper-requests"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Ed Jones", email="ejones84@icloud.com" },
 ]
 description = "Concurrent request HTTP execution library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "requests ~= 2.28.1",
+    "nest-asyncio ~=1.5.6",
+]
 
 [project.urls]
 "Homepage" = "https://github.com/edjones84/hyper-requests"
 "Bug Tracker" = "https://github.com/edjones84/hyper-requests/issues"
-
-[tool.hatchling.requires]
-python = ">=3.7"
-requests = "~=2.28.1"
-nest-asyncio = "~=1.5.6"
```

