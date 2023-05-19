# Comparing `tmp/opentelemetry_instrumentation_fastapi-0.38b0.tar.gz` & `tmp/opentelemetry_instrumentation_fastapi-0.39b0.tar.gz`

## Comparing `opentelemetry_instrumentation_fastapi-0.38b0.tar` & `opentelemetry_instrumentation_fastapi-0.39b0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    13375 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.38b0/src/opentelemetry/instrumentation/fastapi/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.38b0/src/opentelemetry/instrumentation/fastapi/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.38b0/src/opentelemetry/instrumentation/fastapi/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.38b0/tests/__init__.py
--rw-r--r--   0        0        0    33406 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.38b0/tests/test_fastapi_instrumentation.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.38b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.38b0/LICENSE
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.38b0/README.rst
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.38b0/pyproject.toml
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.38b0/PKG-INFO
+-rw-r--r--   0        0        0    13375 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.39b0/src/opentelemetry/instrumentation/fastapi/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.39b0/src/opentelemetry/instrumentation/fastapi/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.39b0/src/opentelemetry/instrumentation/fastapi/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.39b0/tests/__init__.py
+-rw-r--r--   0        0        0    33406 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.39b0/tests/test_fastapi_instrumentation.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.39b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.39b0/LICENSE
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.39b0/README.rst
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.39b0/pyproject.toml
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_fastapi-0.39b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_fastapi-0.38b0/src/opentelemetry/instrumentation/fastapi/__init__.py` & `opentelemetry_instrumentation_fastapi-0.39b0/src/opentelemetry/instrumentation/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_fastapi-0.38b0/src/opentelemetry/instrumentation/fastapi/package.py` & `opentelemetry_instrumentation_fastapi-0.39b0/src/opentelemetry/instrumentation/fastapi/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_fastapi-0.38b0/src/opentelemetry/instrumentation/fastapi/version.py` & `opentelemetry_instrumentation_fastapi-0.39b0/src/opentelemetry/instrumentation/fastapi/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.38b0"
+__version__ = "0.39b0"
```

### Comparing `opentelemetry_instrumentation_fastapi-0.38b0/tests/test_fastapi_instrumentation.py` & `opentelemetry_instrumentation_fastapi-0.39b0/tests/test_fastapi_instrumentation.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_fastapi-0.38b0/LICENSE` & `opentelemetry_instrumentation_fastapi-0.39b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_fastapi-0.38b0/README.rst` & `opentelemetry_instrumentation_fastapi-0.39b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_fastapi-0.38b0/pyproject.toml` & `opentelemetry_instrumentation_fastapi-0.39b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,27 +22,27 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
   "opentelemetry-api ~= 1.12",
-  "opentelemetry-instrumentation == 0.38b0",
-  "opentelemetry-instrumentation-asgi == 0.38b0",
-  "opentelemetry-semantic-conventions == 0.38b0",
-  "opentelemetry-util-http == 0.38b0",
+  "opentelemetry-instrumentation == 0.39b0",
+  "opentelemetry-instrumentation-asgi == 0.39b0",
+  "opentelemetry-semantic-conventions == 0.39b0",
+  "opentelemetry-util-http == 0.39b0",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "fastapi ~= 0.58",
 ]
 test = [
   "opentelemetry-instrumentation-fastapi[instruments]",
-  "opentelemetry-test-utils == 0.38b0",
+  "opentelemetry-test-utils == 0.39b0",
   "requests ~= 2.23", # needed for testclient
   "httpx ~= 0.22", # needed for testclient
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 fastapi = "opentelemetry.instrumentation.fastapi:FastAPIInstrumentor"
```

### Comparing `opentelemetry_instrumentation_fastapi-0.38b0/PKG-INFO` & `opentelemetry_instrumentation_fastapi-0.39b0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-fastapi
-Version: 0.38b0
+Version: 0.39b0
 Summary: OpenTelemetry FastAPI Instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-fastapi
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,24 +14,24 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: opentelemetry-api~=1.12
-Requires-Dist: opentelemetry-instrumentation-asgi==0.38b0
-Requires-Dist: opentelemetry-instrumentation==0.38b0
-Requires-Dist: opentelemetry-semantic-conventions==0.38b0
-Requires-Dist: opentelemetry-util-http==0.38b0
+Requires-Dist: opentelemetry-instrumentation-asgi==0.39b0
+Requires-Dist: opentelemetry-instrumentation==0.39b0
+Requires-Dist: opentelemetry-semantic-conventions==0.39b0
+Requires-Dist: opentelemetry-util-http==0.39b0
 Provides-Extra: instruments
 Requires-Dist: fastapi~=0.58; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: httpx~=0.22; extra == 'test'
 Requires-Dist: opentelemetry-instrumentation-fastapi[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.38b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
 Requires-Dist: requests~=2.23; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry FastAPI Instrumentation
 =======================================
 
 |pypi|
```

