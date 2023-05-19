# Comparing `tmp/opentelemetry_instrumentation_falcon-0.38b0.tar.gz` & `tmp/opentelemetry_instrumentation_falcon-0.39b0.tar.gz`

## Comparing `opentelemetry_instrumentation_falcon-0.38b0.tar` & `opentelemetry_instrumentation_falcon-0.39b0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    20291 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.38b0/src/opentelemetry/instrumentation/falcon/__init__.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.38b0/src/opentelemetry/instrumentation/falcon/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.38b0/src/opentelemetry/instrumentation/falcon/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.38b0/tests/__init__.py
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.38b0/tests/app.py
--rw-r--r--   0        0        0    23387 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.38b0/tests/test_falcon.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.38b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.38b0/LICENSE
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.38b0/README.rst
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.38b0/pyproject.toml
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.38b0/PKG-INFO
+-rw-r--r--   0        0        0    20375 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.39b0/src/opentelemetry/instrumentation/falcon/__init__.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.39b0/src/opentelemetry/instrumentation/falcon/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.39b0/src/opentelemetry/instrumentation/falcon/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.39b0/tests/__init__.py
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.39b0/tests/app.py
+-rw-r--r--   0        0        0    23387 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.39b0/tests/test_falcon.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.39b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.39b0/LICENSE
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.39b0/README.rst
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.39b0/pyproject.toml
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_falcon-0.39b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_falcon-0.38b0/src/opentelemetry/instrumentation/falcon/__init__.py` & `opentelemetry_instrumentation_falcon-0.39b0/src/opentelemetry/instrumentation/falcon/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,14 +241,17 @@
     _instrumented_falcon_apps = set()
 
     def __init__(self, *args, **kwargs):
         otel_opts = kwargs.pop("_otel_opts", {})
 
         # inject trace middleware
         self._middlewares_list = kwargs.pop("middleware", [])
+        if self._middlewares_list is None:
+            self._middlewares_list = []
+
         tracer_provider = otel_opts.pop("tracer_provider", None)
         meter_provider = otel_opts.pop("meter_provider", None)
         if not isinstance(self._middlewares_list, (list, tuple)):
             self._middlewares_list = [self._middlewares_list]
 
         self._otel_tracer = trace.get_tracer(
             __name__, __version__, tracer_provider
```

### Comparing `opentelemetry_instrumentation_falcon-0.38b0/src/opentelemetry/instrumentation/falcon/package.py` & `opentelemetry_instrumentation_falcon-0.39b0/src/opentelemetry/instrumentation/falcon/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_falcon-0.38b0/src/opentelemetry/instrumentation/falcon/version.py` & `opentelemetry_instrumentation_falcon-0.39b0/src/opentelemetry/instrumentation/falcon/version.py`

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

### Comparing `opentelemetry_instrumentation_falcon-0.38b0/tests/app.py` & `opentelemetry_instrumentation_falcon-0.39b0/tests/app.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_falcon-0.38b0/tests/test_falcon.py` & `opentelemetry_instrumentation_falcon-0.39b0/tests/test_falcon.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_falcon-0.38b0/LICENSE` & `opentelemetry_instrumentation_falcon-0.39b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_falcon-0.38b0/README.rst` & `opentelemetry_instrumentation_falcon-0.39b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_falcon-0.38b0/pyproject.toml` & `opentelemetry_instrumentation_falcon-0.39b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,28 +22,28 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
   "opentelemetry-api ~= 1.12",
-  "opentelemetry-instrumentation == 0.38b0",
-  "opentelemetry-instrumentation-wsgi == 0.38b0",
-  "opentelemetry-semantic-conventions == 0.38b0",
-  "opentelemetry-util-http == 0.38b0",
+  "opentelemetry-instrumentation == 0.39b0",
+  "opentelemetry-instrumentation-wsgi == 0.39b0",
+  "opentelemetry-semantic-conventions == 0.39b0",
+  "opentelemetry-util-http == 0.39b0",
   "packaging >= 20.0",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "falcon >= 1.4.1, < 4.0.0",
 ]
 test = [
   "opentelemetry-instrumentation-falcon[instruments]",
-  "opentelemetry-test-utils == 0.38b0",
+  "opentelemetry-test-utils == 0.39b0",
   "parameterized == 0.7.4",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 falcon = "opentelemetry.instrumentation.falcon:FalconInstrumentor"
 
 [project.urls]
```

### Comparing `opentelemetry_instrumentation_falcon-0.38b0/PKG-INFO` & `opentelemetry_instrumentation_falcon-0.39b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-falcon
-Version: 0.38b0
+Version: 0.39b0
 Summary: Falcon instrumentation for OpenTelemetry
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-falcon
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
-Requires-Dist: opentelemetry-instrumentation-wsgi==0.38b0
-Requires-Dist: opentelemetry-instrumentation==0.38b0
-Requires-Dist: opentelemetry-semantic-conventions==0.38b0
-Requires-Dist: opentelemetry-util-http==0.38b0
+Requires-Dist: opentelemetry-instrumentation-wsgi==0.39b0
+Requires-Dist: opentelemetry-instrumentation==0.39b0
+Requires-Dist: opentelemetry-semantic-conventions==0.39b0
+Requires-Dist: opentelemetry-util-http==0.39b0
 Requires-Dist: packaging>=20.0
 Provides-Extra: instruments
 Requires-Dist: falcon<4.0.0,>=1.4.1; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: opentelemetry-instrumentation-falcon[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.38b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
 Requires-Dist: parameterized==0.7.4; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Falcon Tracing
 ============================
 
 |pypi|
```

