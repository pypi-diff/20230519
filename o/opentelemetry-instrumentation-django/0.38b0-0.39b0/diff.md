# Comparing `tmp/opentelemetry_instrumentation_django-0.38b0.tar.gz` & `tmp/opentelemetry_instrumentation_django-0.39b0.tar.gz`

## Comparing `opentelemetry_instrumentation_django-0.38b0.tar` & `opentelemetry_instrumentation_django-0.39b0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    14520 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.38b0/src/opentelemetry/instrumentation/django/__init__.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.38b0/src/opentelemetry/instrumentation/django/environment_variables.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.38b0/src/opentelemetry/instrumentation/django/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.38b0/src/opentelemetry/instrumentation/django/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.38b0/src/opentelemetry/instrumentation/django/middleware/__init__.py
--rw-r--r--   0        0        0    14767 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.38b0/src/opentelemetry/instrumentation/django/middleware/otel_middleware.py
--rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.38b0/src/opentelemetry/instrumentation/django/middleware/sqlcommenter_middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.38b0/tests/__init__.py
--rw-r--r--   0        0        0    24755 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.38b0/tests/test_middleware.py
--rw-r--r--   0        0        0    20582 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.38b0/tests/test_middleware_asgi.py
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.38b0/tests/test_sqlcommenter.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.38b0/tests/views.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.38b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.38b0/LICENSE
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.38b0/README.rst
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.38b0/pyproject.toml
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.38b0/PKG-INFO
+-rw-r--r--   0        0        0    14520 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/__init__.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/environment_variables.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/middleware/__init__.py
+-rw-r--r--   0        0        0    14802 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/middleware/otel_middleware.py
+-rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/middleware/sqlcommenter_middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/tests/__init__.py
+-rw-r--r--   0        0        0    24755 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/tests/test_middleware.py
+-rw-r--r--   0        0        0    20582 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/tests/test_middleware_asgi.py
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/tests/test_sqlcommenter.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/tests/views.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/LICENSE
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/README.rst
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/pyproject.toml
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_django-0.39b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_django-0.38b0/src/opentelemetry/instrumentation/django/__init__.py` & `opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_django-0.38b0/src/opentelemetry/instrumentation/django/environment_variables.py` & `opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/environment_variables.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_django-0.38b0/src/opentelemetry/instrumentation/django/package.py` & `opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_django-0.38b0/src/opentelemetry/instrumentation/django/version.py` & `opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/version.py`

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

### Comparing `opentelemetry_instrumentation_django-0.38b0/src/opentelemetry/instrumentation/django/middleware/otel_middleware.py` & `opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/middleware/otel_middleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,25 +208,26 @@
             carrier_getter = asgi_getter
             collect_request_attributes = asgi_collect_request_attributes
         else:
             carrier = request_meta
             carrier_getter = wsgi_getter
             collect_request_attributes = wsgi_collect_request_attributes
 
+        attributes = collect_request_attributes(carrier)
         span, token = _start_internal_or_server_span(
             tracer=self._tracer,
             span_name=self._get_span_name(request),
             start_time=request_meta.get(
                 "opentelemetry-instrumentor-django.starttime_key"
             ),
             context_carrier=carrier,
             context_getter=carrier_getter,
+            attributes=attributes,
         )
 
-        attributes = collect_request_attributes(carrier)
         active_requests_count_attrs = _parse_active_request_count_attrs(
             attributes
         )
         duration_attrs = _parse_duration_attrs(attributes)
 
         request.META[
             self._environ_active_request_attr_key
```

### Comparing `opentelemetry_instrumentation_django-0.38b0/src/opentelemetry/instrumentation/django/middleware/sqlcommenter_middleware.py` & `opentelemetry_instrumentation_django-0.39b0/src/opentelemetry/instrumentation/django/middleware/sqlcommenter_middleware.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_django-0.38b0/tests/test_middleware.py` & `opentelemetry_instrumentation_django-0.39b0/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_django-0.38b0/tests/test_middleware_asgi.py` & `opentelemetry_instrumentation_django-0.39b0/tests/test_middleware_asgi.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_django-0.38b0/tests/test_sqlcommenter.py` & `opentelemetry_instrumentation_django-0.39b0/tests/test_sqlcommenter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_django-0.38b0/tests/views.py` & `opentelemetry_instrumentation_django-0.39b0/tests/views.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_django-0.38b0/LICENSE` & `opentelemetry_instrumentation_django-0.39b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_django-0.38b0/README.rst` & `opentelemetry_instrumentation_django-0.39b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_django-0.38b0/pyproject.toml` & `opentelemetry_instrumentation_django-0.39b0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -22,30 +22,30 @@
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
 asgi = [
-  "opentelemetry-instrumentation-asgi == 0.38b0",
+  "opentelemetry-instrumentation-asgi == 0.39b0",
 ]
 instruments = [
   "django >= 1.10",
 ]
 test = [
   "opentelemetry-instrumentation-django[instruments]",
-  "opentelemetry-test-utils == 0.38b0",
+  "opentelemetry-test-utils == 0.39b0",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 django = "opentelemetry.instrumentation.django:DjangoInstrumentor"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-django"
```

### Comparing `opentelemetry_instrumentation_django-0.38b0/PKG-INFO` & `opentelemetry_instrumentation_django-0.39b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-django
-Version: 0.38b0
+Version: 0.39b0
 Summary: OpenTelemetry Instrumentation for Django
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-django
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,25 +14,25 @@
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
 Provides-Extra: asgi
-Requires-Dist: opentelemetry-instrumentation-asgi==0.38b0; extra == 'asgi'
+Requires-Dist: opentelemetry-instrumentation-asgi==0.39b0; extra == 'asgi'
 Provides-Extra: instruments
 Requires-Dist: django>=1.10; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: opentelemetry-instrumentation-django[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.38b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Django Tracing
 ============================
 
 |pypi|
```

