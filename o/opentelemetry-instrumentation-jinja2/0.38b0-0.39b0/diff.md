# Comparing `tmp/opentelemetry_instrumentation_jinja2-0.38b0.tar.gz` & `tmp/opentelemetry_instrumentation_jinja2-0.39b0.tar.gz`

## Comparing `opentelemetry_instrumentation_jinja2-0.38b0.tar` & `opentelemetry_instrumentation_jinja2-0.39b0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_jinja2-0.38b0/src/opentelemetry/instrumentation/jinja2/__init__.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_jinja2-0.38b0/src/opentelemetry/instrumentation/jinja2/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_jinja2-0.38b0/src/opentelemetry/instrumentation/jinja2/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_jinja2-0.38b0/tests/__init__.py
--rw-r--r--   0        0        0     8180 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_jinja2-0.38b0/tests/test_jinja2.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_jinja2-0.38b0/tests/templates/base.html
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_jinja2-0.38b0/tests/templates/template.html
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_jinja2-0.38b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_jinja2-0.38b0/LICENSE
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_jinja2-0.38b0/README.rst
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_jinja2-0.38b0/pyproject.toml
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_jinja2-0.38b0/PKG-INFO
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_jinja2-0.39b0/src/opentelemetry/instrumentation/jinja2/__init__.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_jinja2-0.39b0/src/opentelemetry/instrumentation/jinja2/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_jinja2-0.39b0/src/opentelemetry/instrumentation/jinja2/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_jinja2-0.39b0/tests/__init__.py
+-rw-r--r--   0        0        0     8180 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_jinja2-0.39b0/tests/test_jinja2.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_jinja2-0.39b0/tests/templates/base.html
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_jinja2-0.39b0/tests/templates/template.html
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_jinja2-0.39b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_jinja2-0.39b0/LICENSE
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_jinja2-0.39b0/README.rst
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_jinja2-0.39b0/pyproject.toml
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_jinja2-0.39b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_jinja2-0.38b0/src/opentelemetry/instrumentation/jinja2/__init__.py` & `opentelemetry_instrumentation_jinja2-0.39b0/src/opentelemetry/instrumentation/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_jinja2-0.38b0/src/opentelemetry/instrumentation/jinja2/package.py` & `opentelemetry_instrumentation_jinja2-0.39b0/src/opentelemetry/instrumentation/jinja2/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_jinja2-0.38b0/src/opentelemetry/instrumentation/jinja2/version.py` & `opentelemetry_instrumentation_jinja2-0.39b0/src/opentelemetry/instrumentation/jinja2/version.py`

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

### Comparing `opentelemetry_instrumentation_jinja2-0.38b0/tests/test_jinja2.py` & `opentelemetry_instrumentation_jinja2-0.39b0/tests/test_jinja2.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_jinja2-0.38b0/LICENSE` & `opentelemetry_instrumentation_jinja2-0.39b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_jinja2-0.38b0/README.rst` & `opentelemetry_instrumentation_jinja2-0.39b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_jinja2-0.38b0/pyproject.toml` & `opentelemetry_instrumentation_jinja2-0.39b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,26 +21,26 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
   "opentelemetry-api ~= 1.12",
-  "opentelemetry-instrumentation == 0.38b0",
+  "opentelemetry-instrumentation == 0.39b0",
   "wrapt >= 1.0.0, < 2.0.0",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "jinja2 >= 2.7, < 4.0",
 ]
 test = [
   "opentelemetry-instrumentation-jinja2[instruments]",
   "markupsafe==2.0.1",
-  "opentelemetry-test-utils == 0.38b0",
+  "opentelemetry-test-utils == 0.39b0",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 jinja2 = "opentelemetry.instrumentation.jinja2:Jinja2Instrumentor"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-jinja2"
```

### Comparing `opentelemetry_instrumentation_jinja2-0.38b0/PKG-INFO` & `opentelemetry_instrumentation_jinja2-0.39b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-jinja2
-Version: 0.38b0
+Version: 0.39b0
 Summary: OpenTelemetry jinja2 instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-jinja2
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -13,22 +13,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: opentelemetry-api~=1.12
-Requires-Dist: opentelemetry-instrumentation==0.38b0
+Requires-Dist: opentelemetry-instrumentation==0.39b0
 Requires-Dist: wrapt<2.0.0,>=1.0.0
 Provides-Extra: instruments
 Requires-Dist: jinja2<4.0,>=2.7; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: markupsafe==2.0.1; extra == 'test'
 Requires-Dist: opentelemetry-instrumentation-jinja2[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.38b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry jinja2 integration
 ================================
 
 |pypi|
```

