# Comparing `tmp/opentelemetry_instrumentation_asgi-0.38b0.tar.gz` & `tmp/opentelemetry_instrumentation_asgi-0.39b0.tar.gz`

## Comparing `opentelemetry_instrumentation_asgi-0.38b0.tar` & `opentelemetry_instrumentation_asgi-0.39b0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    24852 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.38b0/src/opentelemetry/instrumentation/asgi/__init__.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.38b0/src/opentelemetry/instrumentation/asgi/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.38b0/src/opentelemetry/instrumentation/asgi/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.38b0/tests/__init__.py
--rw-r--r--   0        0        0    13300 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.38b0/tests/test_asgi_custom_headers.py
--rw-r--r--   0        0        0    30123 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.38b0/tests/test_asgi_middleware.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.38b0/tests/test_getter.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.38b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.38b0/LICENSE
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.38b0/README.rst
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.38b0/pyproject.toml
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.38b0/PKG-INFO
+-rw-r--r--   0        0        0    24887 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.39b0/src/opentelemetry/instrumentation/asgi/__init__.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.39b0/src/opentelemetry/instrumentation/asgi/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.39b0/src/opentelemetry/instrumentation/asgi/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.39b0/tests/__init__.py
+-rw-r--r--   0        0        0    13300 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.39b0/tests/test_asgi_custom_headers.py
+-rw-r--r--   0        0        0    30123 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.39b0/tests/test_asgi_middleware.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.39b0/tests/test_getter.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.39b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.39b0/LICENSE
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.39b0/README.rst
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.39b0/pyproject.toml
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_asgi-0.39b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_asgi-0.38b0/src/opentelemetry/instrumentation/asgi/__init__.py` & `opentelemetry_instrumentation_asgi-0.39b0/src/opentelemetry/instrumentation/asgi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -527,23 +527,24 @@
 
         _, _, url = get_host_port_url_tuple(scope)
         if self.excluded_urls and self.excluded_urls.url_disabled(url):
             return await self.app(scope, receive, send)
 
         span_name, additional_attributes = self.default_span_details(scope)
 
+        attributes = collect_request_attributes(scope)
+        attributes.update(additional_attributes)
         span, token = _start_internal_or_server_span(
             tracer=self.tracer,
             span_name=span_name,
             start_time=None,
             context_carrier=scope,
             context_getter=asgi_getter,
+            attributes=attributes,
         )
-        attributes = collect_request_attributes(scope)
-        attributes.update(additional_attributes)
         active_requests_count_attrs = _parse_active_request_count_attrs(
             attributes
         )
         duration_attrs = _parse_duration_attrs(attributes)
 
         if scope["type"] == "http":
             self.active_requests_counter.add(1, active_requests_count_attrs)
```

### Comparing `opentelemetry_instrumentation_asgi-0.38b0/src/opentelemetry/instrumentation/asgi/package.py` & `opentelemetry_instrumentation_asgi-0.39b0/src/opentelemetry/instrumentation/asgi/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_asgi-0.38b0/src/opentelemetry/instrumentation/asgi/version.py` & `opentelemetry_instrumentation_asgi-0.39b0/src/opentelemetry/instrumentation/asgi/version.py`

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

### Comparing `opentelemetry_instrumentation_asgi-0.38b0/tests/test_asgi_custom_headers.py` & `opentelemetry_instrumentation_asgi-0.39b0/tests/test_asgi_custom_headers.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_asgi-0.38b0/tests/test_asgi_middleware.py` & `opentelemetry_instrumentation_asgi-0.39b0/tests/test_asgi_middleware.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_asgi-0.38b0/tests/test_getter.py` & `opentelemetry_instrumentation_asgi-0.39b0/tests/test_getter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_asgi-0.38b0/LICENSE` & `opentelemetry_instrumentation_asgi-0.39b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_asgi-0.38b0/README.rst` & `opentelemetry_instrumentation_asgi-0.39b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_asgi-0.38b0/pyproject.toml` & `opentelemetry_instrumentation_asgi-0.39b0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -23,26 +23,26 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
   "asgiref ~= 3.0",
   "opentelemetry-api ~= 1.12",
-  "opentelemetry-instrumentation == 0.38b0",
-  "opentelemetry-semantic-conventions == 0.38b0",
-  "opentelemetry-util-http == 0.38b0",
+  "opentelemetry-instrumentation == 0.39b0",
+  "opentelemetry-semantic-conventions == 0.39b0",
+  "opentelemetry-util-http == 0.39b0",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "asgiref ~= 3.0",
 ]
 test = [
   "opentelemetry-instrumentation-asgi[instruments]",
-  "opentelemetry-test-utils == 0.38b0",
+  "opentelemetry-test-utils == 0.39b0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-asgi"
 
 [tool.hatch.version]
 path = "src/opentelemetry/instrumentation/asgi/version.py"
```

### Comparing `opentelemetry_instrumentation_asgi-0.38b0/PKG-INFO` & `opentelemetry_instrumentation_asgi-0.39b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-asgi
-Version: 0.38b0
+Version: 0.39b0
 Summary: ASGI instrumentation for OpenTelemetry
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-asgi
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -15,22 +15,22 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: asgiref~=3.0
 Requires-Dist: opentelemetry-api~=1.12
-Requires-Dist: opentelemetry-instrumentation==0.38b0
-Requires-Dist: opentelemetry-semantic-conventions==0.38b0
-Requires-Dist: opentelemetry-util-http==0.38b0
+Requires-Dist: opentelemetry-instrumentation==0.39b0
+Requires-Dist: opentelemetry-semantic-conventions==0.39b0
+Requires-Dist: opentelemetry-util-http==0.39b0
 Provides-Extra: instruments
 Requires-Dist: asgiref~=3.0; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: opentelemetry-instrumentation-asgi[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.38b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry ASGI Instrumentation
 ==================================
 
 |pypi|
```

