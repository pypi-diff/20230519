# Comparing `tmp/opentelemetry_instrumentation_urllib3-0.38b0.tar.gz` & `tmp/opentelemetry_instrumentation_urllib3-0.39b0.tar.gz`

## Comparing `opentelemetry_instrumentation_urllib3-0.38b0.tar` & `opentelemetry_instrumentation_urllib3-0.39b0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11234 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.38b0/src/opentelemetry/instrumentation/urllib3/__init__.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.38b0/src/opentelemetry/instrumentation/urllib3/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.38b0/src/opentelemetry/instrumentation/urllib3/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.38b0/tests/__init__.py
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.38b0/tests/test_urllib3_integration.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.38b0/tests/test_urllib3_ip_support.py
--rw-r--r--   0        0        0     9400 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.38b0/tests/test_urllib3_metrics.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.38b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.38b0/LICENSE
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.38b0/README.rst
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.38b0/pyproject.toml
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.38b0/PKG-INFO
+-rw-r--r--   0        0        0    12326 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.39b0/src/opentelemetry/instrumentation/urllib3/__init__.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.39b0/src/opentelemetry/instrumentation/urllib3/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.39b0/src/opentelemetry/instrumentation/urllib3/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.39b0/tests/__init__.py
+-rw-r--r--   0        0        0    13753 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.39b0/tests/test_urllib3_integration.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.39b0/tests/test_urllib3_ip_support.py
+-rw-r--r--   0        0        0     9400 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.39b0/tests/test_urllib3_metrics.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.39b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.39b0/LICENSE
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.39b0/README.rst
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.39b0/pyproject.toml
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib3-0.39b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_urllib3-0.38b0/src/opentelemetry/instrumentation/urllib3/__init__.py` & `opentelemetry_instrumentation_urllib3-0.39b0/src/opentelemetry/instrumentation/urllib3/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,14 +56,28 @@
     def response_hook(span, request, response):
         pass
 
     URLLib3Instrumentor.instrument(
         request_hook=request_hook, response_hook=response_hook)
     )
 
+Exclude lists
+*************
+
+To exclude certain URLs from being tracked, set the environment variable ``OTEL_PYTHON_URLLIB3_EXCLUDED_URLS``
+(or ``OTEL_PYTHON_EXCLUDED_URLS`` as fallback) with comma delimited regexes representing which URLs to exclude.
+
+For example,
+
+::
+
+    export OTEL_PYTHON_URLLIB3_EXCLUDED_URLS="client/.*/info,healthcheck"
+
+will exclude requests such as ``https://site/client/123/info`` and ``https://site/xyz/healthcheck``.
+
 API
 ---
 """
 
 import collections.abc
 import contextlib
 import io
@@ -88,16 +102,23 @@
 )
 from opentelemetry.metrics import Histogram, get_meter
 from opentelemetry.propagate import inject
 from opentelemetry.semconv.metrics import MetricInstruments
 from opentelemetry.semconv.trace import SpanAttributes
 from opentelemetry.trace import Span, SpanKind, Tracer, get_tracer
 from opentelemetry.trace.status import Status
+from opentelemetry.util.http import (
+    ExcludeList,
+    get_excluded_urls,
+    parse_excluded_urls,
+)
 from opentelemetry.util.http.httplib import set_ip_on_next_http_connection
 
+_excluded_urls_from_env = get_excluded_urls("URLLIB3")
+
 _UrlFilterT = typing.Optional[typing.Callable[[str], str]]
 _RequestHookT = typing.Optional[
     typing.Callable[
         [
             Span,
             urllib3.connectionpool.HTTPConnectionPool,
             typing.Dict,
@@ -134,18 +155,22 @@
         Args:
             **kwargs: Optional arguments
                 ``tracer_provider``: a TracerProvider, defaults to global.
                 ``request_hook``: An optional callback that is invoked right after a span is created.
                 ``response_hook``: An optional callback which is invoked right before the span is finished processing a response.
                 ``url_filter``: A callback to process the requested URL prior
                     to adding it as a span attribute.
+                ``excluded_urls``: A string containing a comma-delimited
+                    list of regexes used to exclude URLs from tracking
         """
         tracer_provider = kwargs.get("tracer_provider")
         tracer = get_tracer(__name__, __version__, tracer_provider)
 
+        excluded_urls = kwargs.get("excluded_urls")
+
         meter_provider = kwargs.get("meter_provider")
         meter = get_meter(__name__, __version__, meter_provider)
 
         duration_histogram = meter.create_histogram(
             name=MetricInstruments.HTTP_CLIENT_DURATION,
             unit="ms",
             description="measures the duration outbound HTTP requests",
@@ -165,35 +190,42 @@
             tracer,
             duration_histogram,
             request_size_histogram,
             response_size_histogram,
             request_hook=kwargs.get("request_hook"),
             response_hook=kwargs.get("response_hook"),
             url_filter=kwargs.get("url_filter"),
+            excluded_urls=_excluded_urls_from_env
+            if excluded_urls is None
+            else parse_excluded_urls(excluded_urls),
         )
 
     def _uninstrument(self, **kwargs):
         _uninstrument()
 
 
 def _instrument(
     tracer: Tracer,
     duration_histogram: Histogram,
     request_size_histogram: Histogram,
     response_size_histogram: Histogram,
     request_hook: _RequestHookT = None,
     response_hook: _ResponseHookT = None,
     url_filter: _UrlFilterT = None,
+    excluded_urls: ExcludeList = None,
 ):
     def instrumented_urlopen(wrapped, instance, args, kwargs):
         if _is_instrumentation_suppressed():
             return wrapped(*args, **kwargs)
 
-        method = _get_url_open_arg("method", args, kwargs).upper()
         url = _get_url(instance, args, kwargs, url_filter)
+        if excluded_urls and excluded_urls.url_disabled(url):
+            return wrapped(*args, **kwargs)
+
+        method = _get_url_open_arg("method", args, kwargs).upper()
         headers = _prepare_headers(kwargs)
         body = _get_url_open_arg("body", args, kwargs)
 
         span_name = f"HTTP {method.strip()}"
         span_attributes = {
             SpanAttributes.HTTP_METHOD: method,
             SpanAttributes.HTTP_URL: url,
```

### Comparing `opentelemetry_instrumentation_urllib3-0.38b0/src/opentelemetry/instrumentation/urllib3/package.py` & `opentelemetry_instrumentation_urllib3-0.39b0/src/opentelemetry/instrumentation/urllib3/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_urllib3-0.38b0/src/opentelemetry/instrumentation/urllib3/version.py` & `opentelemetry_instrumentation_urllib3-0.39b0/src/opentelemetry/instrumentation/urllib3/version.py`

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

### Comparing `opentelemetry_instrumentation_urllib3-0.38b0/tests/test_urllib3_integration.py` & `opentelemetry_instrumentation_urllib3-0.39b0/tests/test_urllib3_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,24 +25,40 @@
 from opentelemetry.context import _SUPPRESS_HTTP_INSTRUMENTATION_KEY
 from opentelemetry.instrumentation.urllib3 import URLLib3Instrumentor
 from opentelemetry.instrumentation.utils import _SUPPRESS_INSTRUMENTATION_KEY
 from opentelemetry.propagate import get_global_textmap, set_global_textmap
 from opentelemetry.semconv.trace import SpanAttributes
 from opentelemetry.test.mock_textmap import MockTextMapPropagator
 from opentelemetry.test.test_base import TestBase
+from opentelemetry.util.http import get_excluded_urls
 
 # pylint: disable=too-many-public-methods
 
 
 class TestURLLib3Instrumentor(TestBase):
     HTTP_URL = "http://httpbin.org/status/200"
     HTTPS_URL = "https://httpbin.org/status/200"
 
     def setUp(self):
         super().setUp()
+
+        self.env_patch = mock.patch.dict(
+            "os.environ",
+            {
+                "OTEL_PYTHON_URLLIB3_EXCLUDED_URLS": "http://localhost/env_excluded_arg/123,env_excluded_noarg"
+            },
+        )
+        self.env_patch.start()
+
+        self.exclude_patch = mock.patch(
+            "opentelemetry.instrumentation.urllib3._excluded_urls_from_env",
+            get_excluded_urls("URLLIB3"),
+        )
+        self.exclude_patch.start()
+
         URLLib3Instrumentor().instrument()
 
         httpretty.enable(allow_net_connect=False)
         httpretty.register_uri(httpretty.GET, self.HTTP_URL, body="Hello!")
         httpretty.register_uri(httpretty.GET, self.HTTPS_URL, body="Hello!")
         httpretty.register_uri(httpretty.POST, self.HTTP_URL, body="Hello!")
 
@@ -154,14 +170,44 @@
         url = "http://httpbin.org:666/status/200"
         httpretty.register_uri(httpretty.GET, url, body="Hello!")
         pool = urllib3.HTTPConnectionPool("httpbin.org", port=666)
         response = pool.urlopen(method="GET", url="/status/200")
 
         self.assert_success_span(response, url)
 
+    def test_excluded_urls_explicit(self):
+        url_201 = "http://httpbin.org/status/201"
+        httpretty.register_uri(
+            httpretty.GET,
+            url_201,
+            status=201,
+        )
+
+        URLLib3Instrumentor().uninstrument()
+        URLLib3Instrumentor().instrument(excluded_urls=".*/201")
+        self.perform_request(self.HTTP_URL)
+        self.perform_request(url_201)
+
+        self.assert_span(num_spans=1)
+
+    def test_excluded_urls_from_env(self):
+        url = "http://localhost/env_excluded_arg/123"
+        httpretty.register_uri(
+            httpretty.GET,
+            url,
+            status=200,
+        )
+
+        URLLib3Instrumentor().uninstrument()
+        URLLib3Instrumentor().instrument()
+        self.perform_request(self.HTTP_URL)
+        self.perform_request(url)
+
+        self.assert_span(num_spans=1)
+
     def test_uninstrument(self):
         URLLib3Instrumentor().uninstrument()
 
         response = self.perform_request(self.HTTP_URL)
         self.assertEqual(b"Hello!", response.data)
         self.assert_span(num_spans=0)
         # instrument again to avoid warning message on tearDown
```

### Comparing `opentelemetry_instrumentation_urllib3-0.38b0/tests/test_urllib3_ip_support.py` & `opentelemetry_instrumentation_urllib3-0.39b0/tests/test_urllib3_ip_support.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_urllib3-0.38b0/tests/test_urllib3_metrics.py` & `opentelemetry_instrumentation_urllib3-0.39b0/tests/test_urllib3_metrics.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_urllib3-0.38b0/LICENSE` & `opentelemetry_instrumentation_urllib3-0.39b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_urllib3-0.38b0/README.rst` & `opentelemetry_instrumentation_urllib3-0.39b0/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -38,13 +38,27 @@
     def response_hook(span, request, response):
         pass
 
     URLLib3Instrumentor.instrument(
         request_hook=request_hook, response_hook=response_hook)
     )
 
+Exclude lists
+*************
+
+To exclude certain URLs from being tracked, set the environment variable ``OTEL_PYTHON_URLLIB3_EXCLUDED_URLS``
+(or ``OTEL_PYTHON_EXCLUDED_URLS`` as fallback) with comma delimited regexes representing which URLs to exclude.
+
+For example,
+
+::
+
+    export OTEL_PYTHON_URLLIB3_EXCLUDED_URLS="client/.*/info,healthcheck"
+
+will exclude requests such as ``https://site/client/123/info`` and ``https://site/xyz/healthcheck``.
+
 References
 ----------
 
 * `OpenTelemetry urllib3 Instrumentation <https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/urllib3/urllib3.html>`_
 * `OpenTelemetry Project <https://opentelemetry.io/>`_
 * `OpenTelemetry Python Examples <https://github.com/open-telemetry/opentelemetry-python/tree/main/docs/examples>`_
```

### Comparing `opentelemetry_instrumentation_urllib3-0.38b0/pyproject.toml` & `opentelemetry_instrumentation_urllib3-0.39b0/pyproject.toml`

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
-  "opentelemetry-semantic-conventions == 0.38b0",
-  "opentelemetry-util-http == 0.38b0",
+  "opentelemetry-instrumentation == 0.39b0",
+  "opentelemetry-semantic-conventions == 0.39b0",
+  "opentelemetry-util-http == 0.39b0",
   "wrapt >= 1.0.0, < 2.0.0",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "urllib3 >= 1.0.0, < 2.0.0",
 ]
 test = [
   "opentelemetry-instrumentation-urllib3[instruments]",
   "httpretty ~= 1.0",
-  "opentelemetry-test-utils == 0.38b0",
+  "opentelemetry-test-utils == 0.39b0",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 urllib3 = "opentelemetry.instrumentation.urllib3:URLLib3Instrumentor"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-urllib3"
```

### Comparing `opentelemetry_instrumentation_urllib3-0.38b0/PKG-INFO` & `opentelemetry_instrumentation_urllib3-0.39b0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-urllib3
-Version: 0.38b0
+Version: 0.39b0
 Summary: OpenTelemetry urllib3 instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-urllib3
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
-Requires-Dist: opentelemetry-instrumentation==0.38b0
-Requires-Dist: opentelemetry-semantic-conventions==0.38b0
-Requires-Dist: opentelemetry-util-http==0.38b0
+Requires-Dist: opentelemetry-instrumentation==0.39b0
+Requires-Dist: opentelemetry-semantic-conventions==0.39b0
+Requires-Dist: opentelemetry-util-http==0.39b0
 Requires-Dist: wrapt<2.0.0,>=1.0.0
 Provides-Extra: instruments
 Requires-Dist: urllib3<2.0.0,>=1.0.0; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: httpretty~=1.0; extra == 'test'
 Requires-Dist: opentelemetry-instrumentation-urllib3[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.38b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry urllib3 Instrumentation
 ======================================
 
 |pypi|
 
@@ -70,13 +70,27 @@
     def response_hook(span, request, response):
         pass
 
     URLLib3Instrumentor.instrument(
         request_hook=request_hook, response_hook=response_hook)
     )
 
+Exclude lists
+*************
+
+To exclude certain URLs from being tracked, set the environment variable ``OTEL_PYTHON_URLLIB3_EXCLUDED_URLS``
+(or ``OTEL_PYTHON_EXCLUDED_URLS`` as fallback) with comma delimited regexes representing which URLs to exclude.
+
+For example,
+
+::
+
+    export OTEL_PYTHON_URLLIB3_EXCLUDED_URLS="client/.*/info,healthcheck"
+
+will exclude requests such as ``https://site/client/123/info`` and ``https://site/xyz/healthcheck``.
+
 References
 ----------
 
 * `OpenTelemetry urllib3 Instrumentation <https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/urllib3/urllib3.html>`_
 * `OpenTelemetry Project <https://opentelemetry.io/>`_
 * `OpenTelemetry Python Examples <https://github.com/open-telemetry/opentelemetry-python/tree/main/docs/examples>`_
```

