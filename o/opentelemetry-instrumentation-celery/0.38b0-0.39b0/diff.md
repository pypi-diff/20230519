# Comparing `tmp/opentelemetry_instrumentation_celery-0.38b0.tar.gz` & `tmp/opentelemetry_instrumentation_celery-0.39b0.tar.gz`

## Comparing `opentelemetry_instrumentation_celery-0.38b0.tar` & `opentelemetry_instrumentation_celery-0.39b0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     9069 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.38b0/src/opentelemetry/instrumentation/celery/__init__.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.38b0/src/opentelemetry/instrumentation/celery/package.py
--rw-r--r--   0        0        0     7385 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.38b0/src/opentelemetry/instrumentation/celery/utils.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.38b0/src/opentelemetry/instrumentation/celery/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.38b0/tests/__init__.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.38b0/tests/celery_test_tasks.py
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.38b0/tests/test_getter.py
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.38b0/tests/test_tasks.py
--rw-r--r--   0        0        0    10139 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.38b0/tests/test_utils.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.38b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.38b0/LICENSE
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.38b0/README.rst
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.38b0/pyproject.toml
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.38b0/PKG-INFO
+-rw-r--r--   0        0        0     9372 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/src/opentelemetry/instrumentation/celery/__init__.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/src/opentelemetry/instrumentation/celery/package.py
+-rw-r--r--   0        0        0     7421 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/src/opentelemetry/instrumentation/celery/utils.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/src/opentelemetry/instrumentation/celery/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/tests/__init__.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/tests/celery_test_tasks.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/tests/test_getter.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/tests/test_tasks.py
+-rw-r--r--   0        0        0    10421 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/tests/test_utils.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/LICENSE
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/README.rst
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/pyproject.toml
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_celery-0.38b0/src/opentelemetry/instrumentation/celery/__init__.py` & `opentelemetry_instrumentation_celery-0.39b0/src/opentelemetry/instrumentation/celery/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -179,27 +179,34 @@
         activation.__exit__(None, None, None)
         utils.detach_span(task, task_id)
 
     def _trace_before_publish(self, *args, **kwargs):
         task = utils.retrieve_task_from_sender(kwargs)
         task_id = utils.retrieve_task_id_from_message(kwargs)
 
-        if task is None or task_id is None:
+        if task_id is None:
             return
 
-        operation_name = f"{_TASK_APPLY_ASYNC}/{task.name}"
+        if task is None:
+            # task is an anonymous task send using send_task or using canvas workflow
+            # Signatures() to send to a task not in the current processes dependency
+            # tree
+            task_name = kwargs.get("sender", "unknown")
+        else:
+            task_name = task.name
+        operation_name = f"{_TASK_APPLY_ASYNC}/{task_name}"
         span = self._tracer.start_span(
             operation_name, kind=trace.SpanKind.PRODUCER
         )
 
         # apply some attributes here because most of the data is not available
         if span.is_recording():
             span.set_attribute(_TASK_TAG_KEY, _TASK_APPLY_ASYNC)
             span.set_attribute(SpanAttributes.MESSAGING_MESSAGE_ID, task_id)
-            span.set_attribute(_TASK_NAME_KEY, task.name)
+            span.set_attribute(_TASK_NAME_KEY, task_name)
             utils.set_attributes_from_context(span, kwargs)
 
         activation = trace.use_span(span, end_on_exit=True)
         activation.__enter__()  # pylint: disable=E1101
 
         utils.attach_span(task, task_id, (span, activation), is_publish=True)
```

### Comparing `opentelemetry_instrumentation_celery-0.38b0/src/opentelemetry/instrumentation/celery/package.py` & `opentelemetry_instrumentation_celery-0.39b0/src/opentelemetry/instrumentation/celery/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_celery-0.38b0/src/opentelemetry/instrumentation/celery/utils.py` & `opentelemetry_instrumentation_celery-0.39b0/src/opentelemetry/instrumentation/celery/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,16 @@
     to publish a task with the same id as the task currently running.
 
     Previously publishing the new task would overwrite the existing `celery.run` span
     in the `dict` causing that span to be forgotten and never finished
     NOTE: We cannot test for this well yet, because we do not run a celery worker,
     and cannot run `task.apply_async()`
     """
+    if task is None:
+        return
     span_dict = getattr(task, CTX_KEY, None)
     if span_dict is None:
         span_dict = {}
         setattr(task, CTX_KEY, span_dict)
 
     span_dict[(task_id, is_publish)] = span
```

### Comparing `opentelemetry_instrumentation_celery-0.38b0/src/opentelemetry/instrumentation/celery/version.py` & `opentelemetry_instrumentation_celery-0.39b0/src/opentelemetry/instrumentation/celery/version.py`

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

### Comparing `opentelemetry_instrumentation_celery-0.38b0/tests/celery_test_tasks.py` & `opentelemetry_instrumentation_celery-0.39b0/tests/celery_test_tasks.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_celery-0.38b0/tests/test_getter.py` & `opentelemetry_instrumentation_celery-0.39b0/tests/test_getter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_celery-0.38b0/tests/test_tasks.py` & `opentelemetry_instrumentation_celery-0.39b0/tests/test_tasks.py`

 * *Files 23% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         self._thread.start()
 
     def tearDown(self):
         super().tearDown()
         CeleryInstrumentor().uninstrument()
         self._worker.stop()
         self._thread.join()
+        CeleryInstrumentor().uninstrument()
 
     def test_task(self):
         CeleryInstrumentor().instrument()
 
         result = task_add.delay(1, 2)
 
         timeout = time.time() + 60 * 1  # 1 minutes from now
@@ -93,7 +94,56 @@
         while not result.ready():
             if time.time() > timeout:
                 break
             time.sleep(0.05)
 
         spans = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(spans), 0)
+
+
+class TestCelerySignatureTask(TestBase):
+    def setUp(self):
+        super().setUp()
+
+        def start_app(*args, **kwargs):
+            # Add an additional task that will not be registered with parent thread
+            @app.task
+            def hidden_task(num_a):
+                return num_a * 2
+
+            self._worker = app.Worker(app=app, pool="solo", concurrency=1)
+            return self._worker.start(*args, **kwargs)
+
+        self._thread = threading.Thread(target=start_app)
+        self._worker = app.Worker(app=app, pool="solo", concurrency=1)
+        self._thread.daemon = True
+        self._thread.start()
+
+    def tearDown(self):
+        super().tearDown()
+        self._worker.stop()
+        self._thread.join()
+        CeleryInstrumentor().uninstrument()
+
+    def test_hidden_task(self):
+        # no-op since already instrumented
+        CeleryInstrumentor().instrument()
+
+        res = app.signature("tests.test_tasks.hidden_task", (2,)).apply_async()
+        while not res.ready():
+            time.sleep(0.05)
+        spans = self.sorted_spans(self.memory_exporter.get_finished_spans())
+        self.assertEqual(len(spans), 2)
+
+        consumer, producer = spans
+
+        self.assertEqual(consumer.name, "run/tests.test_tasks.hidden_task")
+        self.assertEqual(consumer.kind, SpanKind.CONSUMER)
+
+        self.assertEqual(
+            producer.name, "apply_async/tests.test_tasks.hidden_task"
+        )
+        self.assertEqual(producer.kind, SpanKind.PRODUCER)
+
+        self.assertNotEqual(consumer.parent, producer.context)
+        self.assertEqual(consumer.parent.span_id, producer.context.span_id)
+        self.assertEqual(consumer.context.trace_id, producer.context.trace_id)
```

### Comparing `opentelemetry_instrumentation_celery-0.38b0/tests/test_utils.py` & `opentelemetry_instrumentation_celery-0.39b0/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,21 @@
         task_id = "7c6731af-9533-40c3-83a9-25b58f0d837f"
         span = trace._Span("name", mock.Mock(spec=trace_api.SpanContext))
         utils.attach_span(fn_task, task_id, span)
         # delete the Span
         utils.detach_span(fn_task, task_id)
         self.assertEqual(utils.retrieve_span(fn_task, task_id), (None, None))
 
+    def test_optional_task_span_attach(self):
+        task_id = "7c6731af-9533-40c3-83a9-25b58f0d837f"
+        span = trace._Span("name", mock.Mock(spec=trace_api.SpanContext))
+
+        # assert this is is a no-aop
+        self.assertIsNone(utils.attach_span(None, task_id, span))
+
     def test_span_delete_empty(self):
         # ensure detach_span doesn't raise an exception if span is not present
         @self.app.task
         def fn_task():
             return 42
 
         # delete the Span
```

### Comparing `opentelemetry_instrumentation_celery-0.38b0/LICENSE` & `opentelemetry_instrumentation_celery-0.39b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_celery-0.38b0/README.rst` & `opentelemetry_instrumentation_celery-0.39b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_celery-0.38b0/pyproject.toml` & `opentelemetry_instrumentation_celery-0.39b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,25 +22,25 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
   "opentelemetry-api ~= 1.12",
-  "opentelemetry-instrumentation == 0.38b0",
-  "opentelemetry-semantic-conventions == 0.38b0",
+  "opentelemetry-instrumentation == 0.39b0",
+  "opentelemetry-semantic-conventions == 0.39b0",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "celery >= 4.0, < 6.0",
 ]
 test = [
   "opentelemetry-instrumentation-celery[instruments]",
-  "opentelemetry-test-utils == 0.38b0",
+  "opentelemetry-test-utils == 0.39b0",
   "pytest",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 celery = "opentelemetry.instrumentation.celery:CeleryInstrumentor"
 
 [project.urls]
```

### Comparing `opentelemetry_instrumentation_celery-0.38b0/PKG-INFO` & `opentelemetry_instrumentation_celery-0.39b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-celery
-Version: 0.38b0
+Version: 0.39b0
 Summary: OpenTelemetry Celery Instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-celery
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,21 +14,21 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: opentelemetry-api~=1.12
-Requires-Dist: opentelemetry-instrumentation==0.38b0
-Requires-Dist: opentelemetry-semantic-conventions==0.38b0
+Requires-Dist: opentelemetry-instrumentation==0.39b0
+Requires-Dist: opentelemetry-semantic-conventions==0.39b0
 Provides-Extra: instruments
 Requires-Dist: celery<6.0,>=4.0; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: opentelemetry-instrumentation-celery[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.38b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Celery Instrumentation
 ====================================
 
 |pypi|
```

