# Comparing `tmp/opentelemetry_instrumentation_logging-0.38b0.tar.gz` & `tmp/opentelemetry_instrumentation_logging-0.39b0.tar.gz`

## Comparing `opentelemetry_instrumentation_logging-0.38b0.tar` & `opentelemetry_instrumentation_logging-0.39b0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_logging-0.38b0/src/opentelemetry/instrumentation/logging/__init__.py
--rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_logging-0.38b0/src/opentelemetry/instrumentation/logging/constants.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_logging-0.38b0/src/opentelemetry/instrumentation/logging/environment_variables.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_logging-0.38b0/src/opentelemetry/instrumentation/logging/package.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_logging-0.38b0/src/opentelemetry/instrumentation/logging/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_logging-0.38b0/tests/__init__.py
--rw-r--r--   0        0        0     7613 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_logging-0.38b0/tests/test_logging.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_logging-0.38b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_logging-0.38b0/LICENSE
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_logging-0.38b0/README.rst
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_logging-0.38b0/pyproject.toml
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_logging-0.38b0/PKG-INFO
+-rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_logging-0.39b0/src/opentelemetry/instrumentation/logging/__init__.py
+-rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_logging-0.39b0/src/opentelemetry/instrumentation/logging/constants.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_logging-0.39b0/src/opentelemetry/instrumentation/logging/environment_variables.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_logging-0.39b0/src/opentelemetry/instrumentation/logging/package.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_logging-0.39b0/src/opentelemetry/instrumentation/logging/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_logging-0.39b0/tests/__init__.py
+-rw-r--r--   0        0        0     8286 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_logging-0.39b0/tests/test_logging.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_logging-0.39b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_logging-0.39b0/LICENSE
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_logging-0.39b0/README.rst
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_logging-0.39b0/pyproject.toml
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_logging-0.39b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_logging-0.38b0/src/opentelemetry/instrumentation/logging/__init__.py` & `opentelemetry_instrumentation_logging-0.39b0/src/opentelemetry/instrumentation/logging/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,14 +90,15 @@
         service_name = None
 
         def record_factory(*args, **kwargs):
             record = old_factory(*args, **kwargs)
 
             record.otelSpanID = "0"
             record.otelTraceID = "0"
+            record.otelTraceSampled = False
 
             nonlocal service_name
             if service_name is None:
                 resource = getattr(provider, "resource", None)
                 if resource:
                     service_name = (
                         resource.attributes.get("service.name") or ""
@@ -109,14 +110,15 @@
 
             span = get_current_span()
             if span != INVALID_SPAN:
                 ctx = span.get_span_context()
                 if ctx != INVALID_SPAN_CONTEXT:
                     record.otelSpanID = format(ctx.span_id, "016x")
                     record.otelTraceID = format(ctx.trace_id, "032x")
+                    record.otelTraceSampled = ctx.trace_flags.sampled
                     if callable(LoggingInstrumentor._log_hook):
                         try:
                             LoggingInstrumentor._log_hook(  # pylint: disable=E1102
                                 span, record
                             )
                         except Exception:  # pylint: disable=W0703
                             pass
```

### Comparing `opentelemetry_instrumentation_logging-0.38b0/src/opentelemetry/instrumentation/logging/constants.py` & `opentelemetry_instrumentation_logging-0.39b0/src/opentelemetry/instrumentation/logging/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,29 +8,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-DEFAULT_LOGGING_FORMAT = "%(asctime)s %(levelname)s [%(name)s] [%(filename)s:%(lineno)d] [trace_id=%(otelTraceID)s span_id=%(otelSpanID)s resource.service.name=%(otelServiceName)s] - %(message)s"
+DEFAULT_LOGGING_FORMAT = "%(asctime)s %(levelname)s [%(name)s] [%(filename)s:%(lineno)d] [trace_id=%(otelTraceID)s span_id=%(otelSpanID)s resource.service.name=%(otelServiceName)s trace_sampled=%(otelTraceSampled)s] - %(message)s"
 
 
 _MODULE_DOC = """
 The OpenTelemetry ``logging`` integration automatically injects tracing context into log statements.
 
 The integration registers a custom log record factory with the the standard library logging module that automatically inject
 tracing context into log record objects. Optionally, the integration can also call ``logging.basicConfig()`` to set a logging
 format with placeholders for span ID, trace ID and service name.
 
 The following keys are injected into log record objects by the factory:
 
 - ``otelSpanID``
 - ``otelTraceID``
 - ``otelServiceName``
+- ``otelTraceSampled``
 
 The integration uses the following logging format by default:
 
 .. code-block::
 
     {default_logging_format}
 
@@ -109,15 +110,15 @@
 If you code or some other library/framework you are using calls logging.basicConfig before this integration is enabled, then this integration's logging
 format will not be used and log statements will not contain tracing context. For this reason, you'll need to make sure this integration is enabled as early
 as possible in the service lifecycle or your framework is configured to use a logging format with placeholders for tracing context. This can be achieved by
 adding the following placeholders to your logging format:
 
 .. code-block::
 
-    %(otelSpanID)s %(otelTraceID)s %(otelServiceName)s
+    %(otelSpanID)s %(otelTraceID)s %(otelServiceName)s %(otelTraceSampled)s
 
 
 
 API
 -----
 
 .. code-block:: python
```

### Comparing `opentelemetry_instrumentation_logging-0.38b0/src/opentelemetry/instrumentation/logging/environment_variables.py` & `opentelemetry_instrumentation_logging-0.39b0/src/opentelemetry/instrumentation/logging/environment_variables.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_logging-0.38b0/src/opentelemetry/instrumentation/logging/package.py` & `opentelemetry_instrumentation_logging-0.39b0/src/opentelemetry/instrumentation/logging/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_logging-0.38b0/src/opentelemetry/instrumentation/logging/version.py` & `opentelemetry_instrumentation_logging-0.39b0/src/opentelemetry/instrumentation/logging/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.38b0"
+__version__ = "0.39b0"
 
 _instruments = tuple()
```

### Comparing `opentelemetry_instrumentation_logging-0.38b0/tests/test_logging.py` & `opentelemetry_instrumentation_logging-0.39b0/tests/test_logging.py`

 * *Files 12% similar despite different names*

```diff
@@ -58,14 +58,15 @@
             logger = logging.getLogger("test logger")
             logger.info("hello")
             self.assertEqual(len(self.caplog.records), 1)
             record = self.caplog.records[0]
             self.assertEqual(record.otelSpanID, "0")
             self.assertEqual(record.otelTraceID, "0")
             self.assertEqual(record.otelServiceName, "")
+            self.assertEqual(record.otelTraceSampled, False)
 
 
 def log_hook(span, record):
     record.custom_user_attribute_from_log_hook = "some-value"
 
 
 class TestLoggingInstrumentor(TestBase):
@@ -78,32 +79,36 @@
         LoggingInstrumentor().instrument()
         self.tracer = get_tracer(__name__)
 
     def tearDown(self):
         super().tearDown()
         LoggingInstrumentor().uninstrument()
 
-    def assert_trace_context_injected(self, span_id, trace_id):
+    def assert_trace_context_injected(self, span_id, trace_id, trace_sampled):
         with self.caplog.at_level(level=logging.INFO):
             logger = logging.getLogger("test logger")
             logger.info("hello")
             self.assertEqual(len(self.caplog.records), 1)
             record = self.caplog.records[0]
             self.assertEqual(record.otelSpanID, span_id)
             self.assertEqual(record.otelTraceID, trace_id)
+            self.assertEqual(record.otelTraceSampled, trace_sampled)
             self.assertEqual(record.otelServiceName, "unknown_service")
 
     def test_trace_context_injection(self):
         with self.tracer.start_as_current_span("s1") as span:
             span_id = format(span.get_span_context().span_id, "016x")
             trace_id = format(span.get_span_context().trace_id, "032x")
-            self.assert_trace_context_injected(span_id, trace_id)
+            trace_sampled = span.get_span_context().trace_flags.sampled
+            self.assert_trace_context_injected(
+                span_id, trace_id, trace_sampled
+            )
 
     def test_trace_context_injection_without_span(self):
-        self.assert_trace_context_injected("0", "0")
+        self.assert_trace_context_injected("0", "0", False)
 
     @mock.patch("logging.basicConfig")
     def test_basic_config_called(self, basic_config_mock):
         LoggingInstrumentor().uninstrument()
         LoggingInstrumentor().instrument()
         self.assertFalse(basic_config_mock.called)
         LoggingInstrumentor().uninstrument()
@@ -159,39 +164,46 @@
         LoggingInstrumentor().instrument(
             set_logging_format=True,
             log_hook=log_hook,
         )
         with self.tracer.start_as_current_span("s1") as span:
             span_id = format(span.get_span_context().span_id, "016x")
             trace_id = format(span.get_span_context().trace_id, "032x")
+            trace_sampled = span.get_span_context().trace_flags.sampled
             with self.caplog.at_level(level=logging.INFO):
                 logger = logging.getLogger("test logger")
                 logger.info("hello")
                 self.assertEqual(len(self.caplog.records), 1)
                 record = self.caplog.records[0]
                 self.assertEqual(record.otelSpanID, span_id)
                 self.assertEqual(record.otelTraceID, trace_id)
                 self.assertEqual(record.otelServiceName, "unknown_service")
+                self.assertEqual(record.otelTraceSampled, trace_sampled)
                 self.assertEqual(
                     record.custom_user_attribute_from_log_hook, "some-value"
                 )
 
     def test_uninstrumented(self):
         with self.tracer.start_as_current_span("s1") as span:
             span_id = format(span.get_span_context().span_id, "016x")
             trace_id = format(span.get_span_context().trace_id, "032x")
-            self.assert_trace_context_injected(span_id, trace_id)
+            trace_sampled = span.get_span_context().trace_flags.sampled
+            self.assert_trace_context_injected(
+                span_id, trace_id, trace_sampled
+            )
 
         LoggingInstrumentor().uninstrument()
 
         self.caplog.clear()
         with self.tracer.start_as_current_span("s1") as span:
             span_id = format(span.get_span_context().span_id, "016x")
             trace_id = format(span.get_span_context().trace_id, "032x")
+            trace_sampled = span.get_span_context().trace_flags.sampled
             with self.caplog.at_level(level=logging.INFO):
                 logger = logging.getLogger("test logger")
                 logger.info("hello")
                 self.assertEqual(len(self.caplog.records), 1)
                 record = self.caplog.records[0]
                 self.assertFalse(hasattr(record, "otelSpanID"))
                 self.assertFalse(hasattr(record, "otelTraceID"))
                 self.assertFalse(hasattr(record, "otelServiceName"))
+                self.assertFalse(hasattr(record, "otelTraceSampled"))
```

### Comparing `opentelemetry_instrumentation_logging-0.38b0/LICENSE` & `opentelemetry_instrumentation_logging-0.39b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_logging-0.38b0/README.rst` & `opentelemetry_instrumentation_logging-0.39b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_logging-0.38b0/pyproject.toml` & `opentelemetry_instrumentation_logging-0.39b0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,21 +21,21 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
   "opentelemetry-api ~= 1.12",
-  "opentelemetry-instrumentation == 0.38b0",
+  "opentelemetry-instrumentation == 0.39b0",
 ]
 
 [project.optional-dependencies]
 instruments = []
 test = [
-  "opentelemetry-test-utils == 0.38b0",
+  "opentelemetry-test-utils == 0.39b0",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 logging = "opentelemetry.instrumentation.logging:LoggingInstrumentor"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-logging"
```

### Comparing `opentelemetry_instrumentation_logging-0.38b0/PKG-INFO` & `opentelemetry_instrumentation_logging-0.39b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-logging
-Version: 0.38b0
+Version: 0.39b0
 Summary: OpenTelemetry Logging instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-logging
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -13,18 +13,18 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: opentelemetry-api~=1.12
-Requires-Dist: opentelemetry-instrumentation==0.38b0
+Requires-Dist: opentelemetry-instrumentation==0.39b0
 Provides-Extra: instruments
 Provides-Extra: test
-Requires-Dist: opentelemetry-test-utils==0.38b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry logging integration
 =================================
 
 |pypi|
```

