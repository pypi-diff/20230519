# Comparing `tmp/t2d2-sdk-0.0.1.tar.gz` & `tmp/t2d2-sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t2d2-sdk-0.0.1.tar", last modified: Fri May 19 00:17:00 2023, max compression
+gzip compressed data, was "t2d2-sdk-0.0.2.tar", last modified: Fri May 19 00:21:42 2023, max compression
```

## Comparing `t2d2-sdk-0.0.1.tar` & `t2d2-sdk-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 00:17:00.764173 t2d2-sdk-0.0.1/
--rw-rw-rw-   0        0        0     1084 2023-05-18 20:04:58.000000 t2d2-sdk-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1619 2023-05-19 00:17:00.762193 t2d2-sdk-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1135 2023-05-18 23:51:43.000000 t2d2-sdk-0.0.1/README.md
--rw-rw-rw-   0        0        0      564 2023-05-19 00:13:08.000000 t2d2-sdk-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 00:17:00.765147 t2d2-sdk-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-19 00:17:00.731734 t2d2-sdk-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-19 00:17:00.759138 t2d2-sdk-0.0.1/src/t2d2_sdk.egg-info/
--rw-rw-rw-   0        0        0     1619 2023-05-19 00:17:00.000000 t2d2-sdk-0.0.1/src/t2d2_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-05-19 00:17:00.000000 t2d2-sdk-0.0.1/src/t2d2_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 00:17:00.000000 t2d2-sdk-0.0.1/src/t2d2_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-19 00:17:00.000000 t2d2-sdk-0.0.1/src/t2d2_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:21:42.515743 t2d2-sdk-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-19 00:21:32.000000 t2d2-sdk-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-19 00:21:42.515743 t2d2-sdk-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-19 00:21:32.000000 t2d2-sdk-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-19 00:21:32.000000 t2d2-sdk-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 00:21:42.515743 t2d2-sdk-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:21:42.515743 t2d2-sdk-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:21:42.515743 t2d2-sdk-0.0.2/src/t2d2_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-19 00:21:42.000000 t2d2-sdk-0.0.2/src/t2d2_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-19 00:21:42.000000 t2d2-sdk-0.0.2/src/t2d2_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 00:21:42.000000 t2d2-sdk-0.0.2/src/t2d2_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 00:21:42.000000 t2d2-sdk-0.0.2/src/t2d2_sdk.egg-info/top_level.txt
```

### Comparing `t2d2-sdk-0.0.1/LICENSE` & `t2d2-sdk-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# MIT License
-
-Copyright (c) 2022 T2D2
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+# MIT License
+
+Copyright (c) 2022 T2D2
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `t2d2-sdk-0.0.1/PKG-INFO` & `t2d2-sdk-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,42 @@
-Metadata-Version: 2.1
-Name: t2d2-sdk
-Version: 0.0.1
-Summary: T2D2 SDK
-Author-email: Badri Hiriyur <badri@t2d2.ai>
-Project-URL: Homepage, https://github.com/t2d2-ai/py-sdk
-Project-URL: Bug Tracker, https://github.com/t2d2-ai/py-sdk/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# T2D2
-
-T2D2 api class
-
-```python
-T = T2D2(credentials)
-```
-
-- users                 create, get, update, delete
---  api_keys            create, get, update, delete
---  notifications       create, get, update, delete
---  tasks               create, get, update, delete
-- organizations         create, get, update, delete, add_user, update_user, remove_user
---  licenses            create, get, update, delete
-- projects              create, get, update, delete, add_user, update_user, remove_user
---  images              create, get, update, delete, upload
---  orthomosaics        create, get, update, delete, upload
---  videos              create, get, update, delete, upload
---  drawings            create, get, update, delete, upload
---  3dmodels            create, get, update, delete, upload
---  annotations         create, get, update, delete
---  geotags             create, get, update, delete
---  filters             create, get, update, delete
---  tags                create, get, update, delete
---  tools               create, get, update, delete
---  labels              create, get, update, delete
+Metadata-Version: 2.1
+Name: t2d2-sdk
+Version: 0.0.2
+Summary: T2D2 SDK
+Author-email: Badri Hiriyur <badri@t2d2.ai>
+Project-URL: Homepage, https://github.com/t2d2-ai/py-sdk
+Project-URL: Bug Tracker, https://github.com/t2d2-ai/py-sdk/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# T2D2
+
+T2D2 api class
+
+```python
+T = T2D2(credentials)
+```
+
+- users                 create, get, update, delete
+--  api_keys            create, get, update, delete
+--  notifications       create, get, update, delete
+--  tasks               create, get, update, delete
+
+- organizations         create, get, update, delete, add_user, update_user, remove_user
+--  licenses            create, get, update, delete
+
+- projects              create, get, update, delete, add_user, update_user, remove_user
+--  images              create, get, update, delete, upload
+--  orthomosaics        create, get, update, delete, upload
+--  videos              create, get, update, delete, upload
+--  drawings            create, get, update, delete, upload
+--  3dmodels            create, get, update, delete, upload
+--  annotations         create, get, update, delete
+--  geotags             create, get, update, delete
+--  filters             create, get, update, delete
+--  tags                create, get, update, delete
+--  tools               create, get, update, delete
+--  labels              create, get, update, delete
```

### Comparing `t2d2-sdk-0.0.1/README.md` & `t2d2-sdk-0.0.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-# T2D2
-
-T2D2 api class
-
-```python
-T = T2D2(credentials)
-```
-
-- users                 create, get, update, delete
---  api_keys            create, get, update, delete
---  notifications       create, get, update, delete
---  tasks               create, get, update, delete
-- organizations         create, get, update, delete, add_user, update_user, remove_user
---  licenses            create, get, update, delete
-- projects              create, get, update, delete, add_user, update_user, remove_user
---  images              create, get, update, delete, upload
---  orthomosaics        create, get, update, delete, upload
---  videos              create, get, update, delete, upload
---  drawings            create, get, update, delete, upload
---  3dmodels            create, get, update, delete, upload
---  annotations         create, get, update, delete
---  geotags             create, get, update, delete
---  filters             create, get, update, delete
---  tags                create, get, update, delete
---  tools               create, get, update, delete
---  labels              create, get, update, delete
+# T2D2
+
+T2D2 api class
+
+```python
+T = T2D2(credentials)
+```
+
+- users                 create, get, update, delete
+--  api_keys            create, get, update, delete
+--  notifications       create, get, update, delete
+--  tasks               create, get, update, delete
+
+- organizations         create, get, update, delete, add_user, update_user, remove_user
+--  licenses            create, get, update, delete
+
+- projects              create, get, update, delete, add_user, update_user, remove_user
+--  images              create, get, update, delete, upload
+--  orthomosaics        create, get, update, delete, upload
+--  videos              create, get, update, delete, upload
+--  drawings            create, get, update, delete, upload
+--  3dmodels            create, get, update, delete, upload
+--  annotations         create, get, update, delete
+--  geotags             create, get, update, delete
+--  filters             create, get, update, delete
+--  tags                create, get, update, delete
+--  tools               create, get, update, delete
+--  labels              create, get, update, delete
```

### Comparing `t2d2-sdk-0.0.1/pyproject.toml` & `t2d2-sdk-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "t2d2-sdk"
-version = "0.0.1"
-authors = [
-  { name="Badri Hiriyur", email="badri@t2d2.ai" },
-]
-description = "T2D2 SDK"
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/t2d2-ai/py-sdk"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "t2d2-sdk"
+version = "0.0.2"
+authors = [
+  { name="Badri Hiriyur", email="badri@t2d2.ai" },
+]
+description = "T2D2 SDK"
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/t2d2-ai/py-sdk"
 "Bug Tracker" = "https://github.com/t2d2-ai/py-sdk/issues"
```

### Comparing `t2d2-sdk-0.0.1/src/t2d2_sdk.egg-info/PKG-INFO` & `t2d2-sdk-0.0.2/src/t2d2_sdk.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,42 @@
-Metadata-Version: 2.1
-Name: t2d2-sdk
-Version: 0.0.1
-Summary: T2D2 SDK
-Author-email: Badri Hiriyur <badri@t2d2.ai>
-Project-URL: Homepage, https://github.com/t2d2-ai/py-sdk
-Project-URL: Bug Tracker, https://github.com/t2d2-ai/py-sdk/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# T2D2
-
-T2D2 api class
-
-```python
-T = T2D2(credentials)
-```
-
-- users                 create, get, update, delete
---  api_keys            create, get, update, delete
---  notifications       create, get, update, delete
---  tasks               create, get, update, delete
-- organizations         create, get, update, delete, add_user, update_user, remove_user
---  licenses            create, get, update, delete
-- projects              create, get, update, delete, add_user, update_user, remove_user
---  images              create, get, update, delete, upload
---  orthomosaics        create, get, update, delete, upload
---  videos              create, get, update, delete, upload
---  drawings            create, get, update, delete, upload
---  3dmodels            create, get, update, delete, upload
---  annotations         create, get, update, delete
---  geotags             create, get, update, delete
---  filters             create, get, update, delete
---  tags                create, get, update, delete
---  tools               create, get, update, delete
---  labels              create, get, update, delete
+Metadata-Version: 2.1
+Name: t2d2-sdk
+Version: 0.0.2
+Summary: T2D2 SDK
+Author-email: Badri Hiriyur <badri@t2d2.ai>
+Project-URL: Homepage, https://github.com/t2d2-ai/py-sdk
+Project-URL: Bug Tracker, https://github.com/t2d2-ai/py-sdk/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# T2D2
+
+T2D2 api class
+
+```python
+T = T2D2(credentials)
+```
+
+- users                 create, get, update, delete
+--  api_keys            create, get, update, delete
+--  notifications       create, get, update, delete
+--  tasks               create, get, update, delete
+
+- organizations         create, get, update, delete, add_user, update_user, remove_user
+--  licenses            create, get, update, delete
+
+- projects              create, get, update, delete, add_user, update_user, remove_user
+--  images              create, get, update, delete, upload
+--  orthomosaics        create, get, update, delete, upload
+--  videos              create, get, update, delete, upload
+--  drawings            create, get, update, delete, upload
+--  3dmodels            create, get, update, delete, upload
+--  annotations         create, get, update, delete
+--  geotags             create, get, update, delete
+--  filters             create, get, update, delete
+--  tags                create, get, update, delete
+--  tools               create, get, update, delete
+--  labels              create, get, update, delete
```

