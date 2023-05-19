# Comparing `tmp/pyoverkiz-1.7.8.tar.gz` & `tmp/pyoverkiz-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoverkiz-1.7.8.tar", max compression
+gzip compressed data, was "pyoverkiz-1.7.9.tar", max compression
```

## Comparing `pyoverkiz-1.7.8.tar` & `pyoverkiz-1.7.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1073 2023-05-02 21:47:25.634441 pyoverkiz-1.7.8/LICENSE
--rw-r--r--   0        0        0     3319 2023-05-02 21:47:25.634441 pyoverkiz-1.7.8/README.md
--rw-r--r--   0        0        0        0 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/__init__.py
--rw-r--r--   0        0        0    30963 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/client.py
--rw-r--r--   0        0        0     3917 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/const.py
--rw-r--r--   0        0        0      220 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/enums/__init__.py
--rw-r--r--   0        0        0     8866 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/enums/command.py
--rw-r--r--   0        0        0     1888 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/enums/execution.py
--rw-r--r--   0        0        0     2945 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/enums/gateway.py
--rw-r--r--   0        0        0    17241 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/enums/general.py
--rw-r--r--   0        0        0     2141 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/enums/measured_value_type.py
--rw-r--r--   0        0        0     1052 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/enums/protocol.py
--rw-r--r--   0        0        0    14019 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/enums/state.py
--rw-r--r--   0        0        0    18302 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/enums/ui.py
--rw-r--r--   0        0        0     1642 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/exceptions.py
--rw-r--r--   0        0        0    24495 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/models.py
--rw-r--r--   0        0        0     1727 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/obfuscate.py
--rw-r--r--   0        0        0        0 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/py.typed
--rw-r--r--   0        0        0      518 2023-05-02 21:47:25.646441 pyoverkiz-1.7.8/pyoverkiz/types.py
--rw-r--r--   0        0        0      987 2023-05-02 21:47:47.250689 pyoverkiz-1.7.8/pyproject.toml
--rw-r--r--   0        0        0     4303 1970-01-01 00:00:00.000000 pyoverkiz-1.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-19 12:25:35.025662 pyoverkiz-1.7.9/LICENSE
+-rw-r--r--   0        0        0     3319 2023-05-19 12:25:35.025662 pyoverkiz-1.7.9/README.md
+-rw-r--r--   0        0        0        0 2023-05-19 12:25:35.037662 pyoverkiz-1.7.9/pyoverkiz/__init__.py
+-rw-r--r--   0        0        0    30963 2023-05-19 12:25:35.037662 pyoverkiz-1.7.9/pyoverkiz/client.py
+-rw-r--r--   0        0        0     3917 2023-05-19 12:25:35.037662 pyoverkiz-1.7.9/pyoverkiz/const.py
+-rw-r--r--   0        0        0      220 2023-05-19 12:25:35.037662 pyoverkiz-1.7.9/pyoverkiz/enums/__init__.py
+-rw-r--r--   0        0        0     8866 2023-05-19 12:25:35.037662 pyoverkiz-1.7.9/pyoverkiz/enums/command.py
+-rw-r--r--   0        0        0     1888 2023-05-19 12:25:35.041662 pyoverkiz-1.7.9/pyoverkiz/enums/execution.py
+-rw-r--r--   0        0        0     2945 2023-05-19 12:25:35.041662 pyoverkiz-1.7.9/pyoverkiz/enums/gateway.py
+-rw-r--r--   0        0        0    17241 2023-05-19 12:25:35.041662 pyoverkiz-1.7.9/pyoverkiz/enums/general.py
+-rw-r--r--   0        0        0     2141 2023-05-19 12:25:35.041662 pyoverkiz-1.7.9/pyoverkiz/enums/measured_value_type.py
+-rw-r--r--   0        0        0     1052 2023-05-19 12:25:35.041662 pyoverkiz-1.7.9/pyoverkiz/enums/protocol.py
+-rw-r--r--   0        0        0    14019 2023-05-19 12:25:35.041662 pyoverkiz-1.7.9/pyoverkiz/enums/state.py
+-rw-r--r--   0        0        0    18302 2023-05-19 12:25:35.041662 pyoverkiz-1.7.9/pyoverkiz/enums/ui.py
+-rw-r--r--   0        0        0     1642 2023-05-19 12:25:35.041662 pyoverkiz-1.7.9/pyoverkiz/exceptions.py
+-rw-r--r--   0        0        0    24495 2023-05-19 12:25:35.041662 pyoverkiz-1.7.9/pyoverkiz/models.py
+-rw-r--r--   0        0        0     1869 2023-05-19 12:25:35.041662 pyoverkiz-1.7.9/pyoverkiz/obfuscate.py
+-rw-r--r--   0        0        0        0 2023-05-19 12:25:35.041662 pyoverkiz-1.7.9/pyoverkiz/py.typed
+-rw-r--r--   0        0        0      518 2023-05-19 12:25:35.041662 pyoverkiz-1.7.9/pyoverkiz/types.py
+-rw-r--r--   0        0        0      987 2023-05-19 12:25:52.457677 pyoverkiz-1.7.9/pyproject.toml
+-rw-r--r--   0        0        0     4303 1970-01-01 00:00:00.000000 pyoverkiz-1.7.9/PKG-INFO
```

### Comparing `pyoverkiz-1.7.8/LICENSE` & `pyoverkiz-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.8/README.md` & `pyoverkiz-1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.8/pyoverkiz/client.py` & `pyoverkiz-1.7.9/pyoverkiz/client.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.8/pyoverkiz/const.py` & `pyoverkiz-1.7.9/pyoverkiz/const.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.8/pyoverkiz/enums/command.py` & `pyoverkiz-1.7.9/pyoverkiz/enums/command.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.8/pyoverkiz/enums/execution.py` & `pyoverkiz-1.7.9/pyoverkiz/enums/execution.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.8/pyoverkiz/enums/gateway.py` & `pyoverkiz-1.7.9/pyoverkiz/enums/gateway.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.8/pyoverkiz/enums/general.py` & `pyoverkiz-1.7.9/pyoverkiz/enums/general.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.8/pyoverkiz/enums/measured_value_type.py` & `pyoverkiz-1.7.9/pyoverkiz/enums/measured_value_type.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.8/pyoverkiz/enums/protocol.py` & `pyoverkiz-1.7.9/pyoverkiz/enums/protocol.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.8/pyoverkiz/enums/state.py` & `pyoverkiz-1.7.9/pyoverkiz/enums/state.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.8/pyoverkiz/enums/ui.py` & `pyoverkiz-1.7.9/pyoverkiz/enums/ui.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.8/pyoverkiz/exceptions.py` & `pyoverkiz-1.7.9/pyoverkiz/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.8/pyoverkiz/models.py` & `pyoverkiz-1.7.9/pyoverkiz/models.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.8/pyoverkiz/obfuscate.py` & `pyoverkiz-1.7.9/pyoverkiz/obfuscate.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,13 +52,17 @@
         # Mask homekit:SetupCode and homekit:SetupPayload
         if isinstance(value, dict):
             obfuscate_sensitive_data(value)
         elif isinstance(value, list):
             for val in value:
                 if isinstance(val, str):
                     continue
+                if isinstance(val, int):
+                    continue
+                if isinstance(val, float):
+                    continue
                 if isinstance(val, list):
                     continue
 
                 obfuscate_sensitive_data(val)
 
     return data
```

### Comparing `pyoverkiz-1.7.8/pyoverkiz/types.py` & `pyoverkiz-1.7.9/pyoverkiz/types.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.7.8/pyproject.toml` & `pyoverkiz-1.7.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyoverkiz"
-version = "1.7.8"
+version = "1.7.9"
 description = "Async Python client to interact with internal OverKiz API (e.g. used by Somfy TaHoma)."
 authors = ["Mick Vleeshouwer", "Vincent Le Bourlot", "Thibaut Etienne"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/iMicknl/python-overkiz-api"
 repository = "https://github.com/iMicknl/python-overkiz-api"
 packages = [
@@ -25,15 +25,15 @@
 tox = "^3.28"
 pytest = "^7.3"
 pytest-cov = "^4.0.0"
 pre-commit = "^2.21"
 black = {version = "^22.12", allow-prereleases = true}
 pylint = "^2.13.9"
 isort = "^5.11.5"
-mypy = "^1.2"
+mypy = "^1.3"
 flake8 = "^5.0.4"
 pyupgrade = "^3.3.2"
 pytest-asyncio = "^0.21.0"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `pyoverkiz-1.7.8/PKG-INFO` & `pyoverkiz-1.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoverkiz
-Version: 1.7.8
+Version: 1.7.9
 Summary: Async Python client to interact with internal OverKiz API (e.g. used by Somfy TaHoma).
 Home-page: https://github.com/iMicknl/python-overkiz-api
 License: MIT
 Author: Mick Vleeshouwer
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyoverkiz Version: 1.7.8 Summary: Async Python
+Metadata-Version: 2.1 Name: pyoverkiz Version: 1.7.9 Summary: Async Python
 client to interact with internal OverKiz API (e.g. used by Somfy TaHoma). Home-
 page: https://github.com/iMicknl/python-overkiz-api License: MIT Author: Mick
 Vleeshouwer Requires-Python: >=3.7,<4.0 Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

