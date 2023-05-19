# Comparing `tmp/opentelemetry_instrumentation_elasticsearch-0.38b0.tar.gz` & `tmp/opentelemetry_instrumentation_elasticsearch-0.39b0.tar.gz`

## Comparing `opentelemetry_instrumentation_elasticsearch-0.38b0.tar` & `opentelemetry_instrumentation_elasticsearch-0.39b0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     9019 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.38b0/src/opentelemetry/instrumentation/elasticsearch/__init__.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.38b0/src/opentelemetry/instrumentation/elasticsearch/package.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.38b0/src/opentelemetry/instrumentation/elasticsearch/utils.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.38b0/src/opentelemetry/instrumentation/elasticsearch/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.38b0/tests/__init__.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.38b0/tests/helpers_es2.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.38b0/tests/helpers_es5.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.38b0/tests/helpers_es6.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.38b0/tests/helpers_es7.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.38b0/tests/sanitization_queries.py
--rw-r--r--   0        0        0    17489 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.38b0/tests/test_elasticsearch.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.38b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.38b0/LICENSE
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.38b0/README.rst
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.38b0/pyproject.toml
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.38b0/PKG-INFO
+-rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/src/opentelemetry/instrumentation/elasticsearch/__init__.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/src/opentelemetry/instrumentation/elasticsearch/package.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/src/opentelemetry/instrumentation/elasticsearch/utils.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/src/opentelemetry/instrumentation/elasticsearch/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/tests/__init__.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/tests/helpers_es2.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/tests/helpers_es5.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/tests/helpers_es6.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/tests/helpers_es7.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/tests/sanitization_queries.py
+-rw-r--r--   0        0        0    16765 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/tests/test_elasticsearch.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/LICENSE
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/README.rst
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/pyproject.toml
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_elasticsearch-0.39b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_elasticsearch-0.38b0/src/opentelemetry/instrumentation/elasticsearch/__init__.py` & `opentelemetry_instrumentation_elasticsearch-0.39b0/src/opentelemetry/instrumentation/elasticsearch/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 
 .. code-block:: python
 
     ElasticsearchInstrumentor("my-custom-prefix").instrument()
 
 The instrument() method accepts the following keyword args:
 tracer_provider (TracerProvider) - an optional tracer provider
-sanitize_query (bool) - an optional query sanitization flag
 request_hook (Callable) - a function with extra user-defined logic to be performed before performing the request
 this function signature is:
 def request_hook(span: Span, method: str, url: str, kwargs)
 
 response_hook (Callable) - a function with extra user-defined logic to be performed after performing the request
 this function signature is:
 def response_hook(span: Span, response: dict)
@@ -134,21 +133,19 @@
         """
         Instruments Elasticsearch module
         """
         tracer_provider = kwargs.get("tracer_provider")
         tracer = get_tracer(__name__, __version__, tracer_provider)
         request_hook = kwargs.get("request_hook")
         response_hook = kwargs.get("response_hook")
-        sanitize_query = kwargs.get("sanitize_query", False)
         _wrap(
             elasticsearch,
             "Transport.perform_request",
             _wrap_perform_request(
                 tracer,
-                sanitize_query,
                 self._span_name_prefix,
                 request_hook,
                 response_hook,
             ),
         )
 
     def _uninstrument(self, **kwargs):
@@ -159,15 +156,14 @@
 
 # search api https://www.elastic.co/guide/en/elasticsearch/reference/current/search-search.html
 _regex_search_url = re.compile(r"/([^/]+)/_search[/]?")
 
 
 def _wrap_perform_request(
     tracer,
-    sanitize_query,
     span_name_prefix,
     request_hook=None,
     response_hook=None,
 ):
     # pylint: disable=R0912,R0914
     def wrapper(wrapped, _, args, kwargs):
         method = url = None
@@ -221,18 +217,17 @@
                     SpanAttributes.DB_SYSTEM: "elasticsearch",
                 }
                 if url:
                     attributes["elasticsearch.url"] = url
                 if method:
                     attributes["elasticsearch.method"] = method
                 if body:
-                    statement = str(body)
-                    if sanitize_query:
-                        statement = sanitize_body(body)
-                    attributes[SpanAttributes.DB_STATEMENT] = statement
+                    attributes[SpanAttributes.DB_STATEMENT] = sanitize_body(
+                        body
+                    )
                 if params:
                     attributes["elasticsearch.params"] = str(params)
                 if doc_id:
                     attributes["elasticsearch.id"] = doc_id
                 if search_target:
                     attributes["elasticsearch.target"] = search_target
                 for key, value in attributes.items():
```

### Comparing `opentelemetry_instrumentation_elasticsearch-0.38b0/src/opentelemetry/instrumentation/elasticsearch/package.py` & `opentelemetry_instrumentation_elasticsearch-0.39b0/src/opentelemetry/instrumentation/elasticsearch/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_elasticsearch-0.38b0/src/opentelemetry/instrumentation/elasticsearch/utils.py` & `opentelemetry_instrumentation_elasticsearch-0.39b0/src/opentelemetry/instrumentation/elasticsearch/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
 
 # pylint: disable=C0103
 def _flatten_dict(d, parent_key=""):
     items = []
     for k, v in d.items():
         new_key = parent_key + "." + k if parent_key else k
-        if isinstance(v, dict):
+        # recursive call _flatten_dict for a non-empty dict value
+        if isinstance(v, dict) and v:
             items.extend(_flatten_dict(v, new_key).items())
         else:
             items.append((new_key, v))
     return dict(items)
 
 
 def _unflatten_dict(d):
```

### Comparing `opentelemetry_instrumentation_elasticsearch-0.38b0/src/opentelemetry/instrumentation/elasticsearch/version.py` & `opentelemetry_instrumentation_elasticsearch-0.39b0/src/opentelemetry/instrumentation/elasticsearch/version.py`

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

### Comparing `opentelemetry_instrumentation_elasticsearch-0.38b0/tests/helpers_es2.py` & `opentelemetry_instrumentation_elasticsearch-0.39b0/tests/helpers_es2.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_elasticsearch-0.38b0/tests/helpers_es5.py` & `opentelemetry_instrumentation_elasticsearch-0.39b0/tests/helpers_es5.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_elasticsearch-0.38b0/tests/helpers_es6.py` & `opentelemetry_instrumentation_elasticsearch-0.39b0/tests/helpers_es6.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_elasticsearch-0.38b0/tests/helpers_es7.py` & `opentelemetry_instrumentation_elasticsearch-0.39b0/tests/helpers_es7.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_elasticsearch-0.38b0/tests/sanitization_queries.py` & `opentelemetry_instrumentation_elasticsearch-0.39b0/tests/sanitization_queries.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_elasticsearch-0.38b0/tests/test_elasticsearch.py` & `opentelemetry_instrumentation_elasticsearch-0.39b0/tests/test_elasticsearch.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,17 +54,15 @@
 )
 class TestElasticsearchIntegration(TestBase):
     search_attributes = {
         SpanAttributes.DB_SYSTEM: "elasticsearch",
         "elasticsearch.url": "/test-index/_search",
         "elasticsearch.method": helpers.dsl_search_method,
         "elasticsearch.target": "test-index",
-        SpanAttributes.DB_STATEMENT: str(
-            {"query": {"bool": {"filter": [{"term": {"author": "testing"}}]}}}
-        ),
+        SpanAttributes.DB_STATEMENT: str({"query": {"bool": {"filter": "?"}}}),
     }
 
     create_attributes = {
         SpanAttributes.DB_SYSTEM: "elasticsearch",
         "elasticsearch.url": "/test-index",
         "elasticsearch.method": "HEAD",
     }
@@ -260,40 +258,28 @@
         self.assertIsNotNone(span.end_time)
         self.assertEqual(
             span.attributes,
             self.search_attributes,
         )
 
     def test_dsl_search_sanitized(self, request_mock):
-        # Reset instrumentation to use sanitized query (default)
-        ElasticsearchInstrumentor().uninstrument()
-        ElasticsearchInstrumentor().instrument(sanitize_query=True)
-
-        # update expected attributes to match sanitized query
-        sanitized_search_attributes = self.search_attributes.copy()
-        sanitized_search_attributes.update(
-            {
-                SpanAttributes.DB_STATEMENT: "{'query': {'bool': {'filter': '?'}}}"
-            }
-        )
-
         request_mock.return_value = (1, {}, '{"hits": {"hits": []}}')
         client = Elasticsearch()
         search = Search(using=client, index="test-index").filter(
             "term", author="testing"
         )
         search.execute()
         spans = self.get_finished_spans()
         span = spans[0]
         self.assertEqual(1, len(spans))
         self.assertEqual(span.name, "Elasticsearch/<target>/_search")
         self.assertIsNotNone(span.end_time)
         self.assertEqual(
             span.attributes,
-            sanitized_search_attributes,
+            self.search_attributes,
         )
 
     def test_dsl_create(self, request_mock):
         request_mock.return_value = (1, {}, {})
         client = Elasticsearch()
         Article.init(using=client)
 
@@ -316,17 +302,14 @@
         self.assertSpanHasAttributes(span2, attributes)
         self.assertEqual(
             literal_eval(span2.attributes[SpanAttributes.DB_STATEMENT]),
             helpers.dsl_create_statement,
         )
 
     def test_dsl_create_sanitized(self, request_mock):
-        # Reset instrumentation to explicitly use sanitized query
-        ElasticsearchInstrumentor().uninstrument()
-        ElasticsearchInstrumentor().instrument(sanitize_query=True)
         request_mock.return_value = (1, {}, {})
         client = Elasticsearch()
         Article.init(using=client)
 
         spans = self.get_finished_spans()
         assert spans
```

### Comparing `opentelemetry_instrumentation_elasticsearch-0.38b0/LICENSE` & `opentelemetry_instrumentation_elasticsearch-0.39b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_elasticsearch-0.38b0/README.rst` & `opentelemetry_instrumentation_elasticsearch-0.39b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_elasticsearch-0.38b0/pyproject.toml` & `opentelemetry_instrumentation_elasticsearch-0.39b0/pyproject.toml`

 * *Files 8% similar despite different names*

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
-  "opentelemetry-semantic-conventions == 0.38b0",
+  "opentelemetry-instrumentation == 0.39b0",
+  "opentelemetry-semantic-conventions == 0.39b0",
   "wrapt >= 1.0.0, < 2.0.0",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "elasticsearch >= 2.0",
 ]
 test = [
   "opentelemetry-instrumentation-elasticsearch[instruments]",
   "elasticsearch-dsl >= 2.0",
-  "opentelemetry-test-utils == 0.38b0",
+  "opentelemetry-test-utils == 0.39b0",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 elasticsearch = "opentelemetry.instrumentation.elasticsearch:ElasticsearchInstrumentor"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-elasticsearch"
```

### Comparing `opentelemetry_instrumentation_elasticsearch-0.38b0/PKG-INFO` & `opentelemetry_instrumentation_elasticsearch-0.39b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-elasticsearch
-Version: 0.38b0
+Version: 0.39b0
 Summary: OpenTelemetry elasticsearch instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-elasticsearch
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,23 +14,23 @@
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
 Requires-Dist: wrapt<2.0.0,>=1.0.0
 Provides-Extra: instruments
 Requires-Dist: elasticsearch>=2.0; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: elasticsearch-dsl>=2.0; extra == 'test'
 Requires-Dist: opentelemetry-instrumentation-elasticsearch[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.38b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry elasticsearch Integration
 ========================================
 
 |pypi|
```

