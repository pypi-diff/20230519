# Comparing `tmp/opentelemetry_instrumentation_flask-0.38b0.tar.gz` & `tmp/opentelemetry_instrumentation_flask-0.39b0.tar.gz`

## Comparing `opentelemetry_instrumentation_flask-0.38b0.tar` & `opentelemetry_instrumentation_flask-0.39b0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    24568 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.38b0/src/opentelemetry/instrumentation/flask/__init__.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.38b0/src/opentelemetry/instrumentation/flask/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.38b0/src/opentelemetry/instrumentation/flask/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.38b0/tests/__init__.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.38b0/tests/base_test.py
--rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.38b0/tests/test_automatic.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.38b0/tests/test_multithreading.py
--rw-r--r--   0        0        0    26898 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.38b0/tests/test_programmatic.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.38b0/tests/test_sqlcommenter.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.38b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.38b0/LICENSE
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.38b0/README.rst
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.38b0/pyproject.toml
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.38b0/PKG-INFO
+-rw-r--r--   0        0        0    24568 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/src/opentelemetry/instrumentation/flask/__init__.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/src/opentelemetry/instrumentation/flask/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/src/opentelemetry/instrumentation/flask/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/tests/__init__.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/tests/base_test.py
+-rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/tests/test_automatic.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/tests/test_multithreading.py
+-rw-r--r--   0        0        0    26898 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/tests/test_programmatic.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/tests/test_sqlcommenter.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/LICENSE
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/README.rst
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/pyproject.toml
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_flask-0.39b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_flask-0.38b0/src/opentelemetry/instrumentation/flask/__init__.py` & `opentelemetry_instrumentation_flask-0.39b0/src/opentelemetry/instrumentation/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_flask-0.38b0/src/opentelemetry/instrumentation/flask/package.py` & `opentelemetry_instrumentation_flask-0.39b0/src/opentelemetry/instrumentation/flask/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_flask-0.38b0/src/opentelemetry/instrumentation/flask/version.py` & `opentelemetry_instrumentation_flask-0.39b0/src/opentelemetry/instrumentation/flask/version.py`

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

### Comparing `opentelemetry_instrumentation_flask-0.38b0/tests/base_test.py` & `opentelemetry_instrumentation_flask-0.39b0/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_flask-0.38b0/tests/test_automatic.py` & `opentelemetry_instrumentation_flask-0.39b0/tests/test_automatic.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_flask-0.38b0/tests/test_multithreading.py` & `opentelemetry_instrumentation_flask-0.39b0/tests/test_multithreading.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_flask-0.38b0/tests/test_programmatic.py` & `opentelemetry_instrumentation_flask-0.39b0/tests/test_programmatic.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_flask-0.38b0/tests/test_sqlcommenter.py` & `opentelemetry_instrumentation_flask-0.39b0/tests/test_sqlcommenter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_flask-0.38b0/LICENSE` & `opentelemetry_instrumentation_flask-0.39b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_flask-0.38b0/README.rst` & `opentelemetry_instrumentation_flask-0.39b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_flask-0.38b0/pyproject.toml` & `opentelemetry_instrumentation_flask-0.39b0/pyproject.toml`

 * *Files 5% similar despite different names*

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
 ]
 
 [project.optional-dependencies]
 instruments = [
   "flask >= 1.0, < 3.0",
 ]
 test = [
   "opentelemetry-instrumentation-flask[instruments]",
   "markupsafe==2.0.1",
-  "opentelemetry-test-utils == 0.38b0",
+  "opentelemetry-test-utils == 0.39b0",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 flask = "opentelemetry.instrumentation.flask:FlaskInstrumentor"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-flask"
```

### Comparing `opentelemetry_instrumentation_flask-0.38b0/PKG-INFO` & `opentelemetry_instrumentation_flask-0.39b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-flask
-Version: 0.38b0
+Version: 0.39b0
 Summary: Flask instrumentation for OpenTelemetry
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-flask
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
 Provides-Extra: instruments
 Requires-Dist: flask<3.0,>=1.0; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: markupsafe==2.0.1; extra == 'test'
 Requires-Dist: opentelemetry-instrumentation-flask[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.38b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Flask Tracing
 ===========================
 
 |pypi|
```

