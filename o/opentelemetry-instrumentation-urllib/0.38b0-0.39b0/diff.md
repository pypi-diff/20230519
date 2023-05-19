# Comparing `tmp/opentelemetry_instrumentation_urllib-0.38b0.tar.gz` & `tmp/opentelemetry_instrumentation_urllib-0.39b0.tar.gz`

## Comparing `opentelemetry_instrumentation_urllib-0.38b0.tar` & `opentelemetry_instrumentation_urllib-0.39b0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10300 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.38b0/src/opentelemetry/instrumentation/urllib/__init__.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.38b0/src/opentelemetry/instrumentation/urllib/package.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.38b0/src/opentelemetry/instrumentation/urllib/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.38b0/tests/__init__.py
--rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.38b0/tests/test_metrics_instrumentation.py
--rw-r--r--   0        0        0    12797 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.38b0/tests/test_urllib_integration.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.38b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.38b0/LICENSE
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.38b0/README.rst
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.38b0/pyproject.toml
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.38b0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.39b0/src/opentelemetry/instrumentation/urllib/__init__.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.39b0/src/opentelemetry/instrumentation/urllib/package.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.39b0/src/opentelemetry/instrumentation/urllib/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.39b0/tests/__init__.py
+-rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.39b0/tests/test_metrics_instrumentation.py
+-rw-r--r--   0        0        0    14146 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.39b0/tests/test_urllib_integration.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.39b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.39b0/LICENSE
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.39b0/README.rst
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.39b0/pyproject.toml
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_urllib-0.39b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_urllib-0.38b0/src/opentelemetry/instrumentation/urllib/__init__.py` & `opentelemetry_instrumentation_urllib-0.39b0/src/opentelemetry/instrumentation/urllib/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -52,14 +52,28 @@
     def response_hook(span, request_obj, response)
         pass
 
     URLLibInstrumentor.instrument(
         request_hook=request_hook, response_hook=response_hook)
     )
 
+Exclude lists
+*************
+
+To exclude certain URLs from being tracked, set the environment variable ``OTEL_PYTHON_URLLIB_EXCLUDED_URLS``
+(or ``OTEL_PYTHON_EXCLUDED_URLS`` as fallback) with comma delimited regexes representing which URLs to exclude.
+
+For example,
+
+::
+
+    export OTEL_PYTHON_URLLIB_EXCLUDED_URLS="client/.*/info,healthcheck"
+
+will exclude requests such as ``https://site/client/123/info`` and ``https://site/xyz/healthcheck``.
+
 API
 ---
 """
 
 import functools
 import types
 import typing
@@ -84,15 +98,22 @@
 )
 from opentelemetry.metrics import Histogram, get_meter
 from opentelemetry.propagate import inject
 from opentelemetry.semconv.metrics import MetricInstruments
 from opentelemetry.semconv.trace import SpanAttributes
 from opentelemetry.trace import Span, SpanKind, get_tracer
 from opentelemetry.trace.status import Status
-from opentelemetry.util.http import remove_url_credentials
+from opentelemetry.util.http import (
+    ExcludeList,
+    get_excluded_urls,
+    parse_excluded_urls,
+    remove_url_credentials,
+)
+
+_excluded_urls_from_env = get_excluded_urls("URLLIB")
 
 _RequestHookT = typing.Optional[typing.Callable[[Span, Request], None]]
 _ResponseHookT = typing.Optional[
     typing.Callable[[Span, Request, client.HTTPResponse], None]
 ]
 
 
@@ -108,28 +129,33 @@
         """Instruments urllib module
 
         Args:
             **kwargs: Optional arguments
                 ``tracer_provider``: a TracerProvider, defaults to global
                 ``request_hook``: An optional callback invoked that is invoked right after a span is created.
                 ``response_hook``: An optional callback which is invoked right before the span is finished processing a response
+                ``excluded_urls``: A string containing a comma-delimited
+                    list of regexes used to exclude URLs from tracking
         """
         tracer_provider = kwargs.get("tracer_provider")
         tracer = get_tracer(__name__, __version__, tracer_provider)
-
+        excluded_urls = kwargs.get("excluded_urls")
         meter_provider = kwargs.get("meter_provider")
         meter = get_meter(__name__, __version__, meter_provider)
 
         histograms = _create_client_histograms(meter)
 
         _instrument(
             tracer,
             histograms,
             request_hook=kwargs.get("request_hook"),
             response_hook=kwargs.get("response_hook"),
+            excluded_urls=_excluded_urls_from_env
+            if excluded_urls is None
+            else parse_excluded_urls(excluded_urls),
         )
 
     def _uninstrument(self, **kwargs):
         _uninstrument()
 
     def uninstrument_opener(
         self, opener: OpenerDirector
@@ -139,14 +165,15 @@
 
 
 def _instrument(
     tracer,
     histograms: Dict[str, Histogram],
     request_hook: _RequestHookT = None,
     response_hook: _ResponseHookT = None,
+    excluded_urls: ExcludeList = None,
 ):
     """Enables tracing of all requests calls that go through
     :code:`urllib.Client._make_request`"""
 
     opener_open = OpenerDirector.open
 
     @functools.wraps(opener_open)
@@ -170,16 +197,19 @@
         _, request, call_wrapped, get_or_create_headers
     ):  # pylint: disable=too-many-locals
         if context.get_value(
             _SUPPRESS_INSTRUMENTATION_KEY
         ) or context.get_value(_SUPPRESS_HTTP_INSTRUMENTATION_KEY):
             return call_wrapped()
 
-        method = request.get_method().upper()
         url = request.full_url
+        if excluded_urls and excluded_urls.url_disabled(url):
+            return call_wrapped()
+
+        method = request.get_method().upper()
 
         span_name = f"HTTP {method}".strip()
 
         url = remove_url_credentials(url)
 
         labels = {
             SpanAttributes.HTTP_METHOD: method,
```

### Comparing `opentelemetry_instrumentation_urllib-0.38b0/src/opentelemetry/instrumentation/urllib/package.py` & `opentelemetry_instrumentation_urllib-0.39b0/src/opentelemetry/instrumentation/urllib/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_urllib-0.38b0/src/opentelemetry/instrumentation/urllib/version.py` & `opentelemetry_instrumentation_urllib-0.39b0/src/opentelemetry/instrumentation/urllib/version.py`

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

### Comparing `opentelemetry_instrumentation_urllib-0.38b0/tests/test_metrics_instrumentation.py` & `opentelemetry_instrumentation_urllib-0.39b0/tests/test_metrics_instrumentation.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_urllib-0.38b0/tests/test_urllib_integration.py` & `opentelemetry_instrumentation_urllib-0.39b0/tests/test_urllib_integration.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,28 +34,44 @@
 from opentelemetry.instrumentation.utils import _SUPPRESS_INSTRUMENTATION_KEY
 from opentelemetry.propagate import get_global_textmap, set_global_textmap
 from opentelemetry.sdk import resources
 from opentelemetry.semconv.trace import SpanAttributes
 from opentelemetry.test.mock_textmap import MockTextMapPropagator
 from opentelemetry.test.test_base import TestBase
 from opentelemetry.trace import StatusCode
+from opentelemetry.util.http import get_excluded_urls
 
 # pylint: disable=too-many-public-methods
 
 
 class RequestsIntegrationTestBase(abc.ABC):
     # pylint: disable=no-member
 
     URL = "http://httpbin.org/status/200"
     URL_TIMEOUT = "http://httpbin.org/timeout/0"
     URL_EXCEPTION = "http://httpbin.org/exception/0"
 
     # pylint: disable=invalid-name
     def setUp(self):
         super().setUp()
+
+        self.env_patch = mock.patch.dict(
+            "os.environ",
+            {
+                "OTEL_PYTHON_URLLIB_EXCLUDED_URLS": "http://localhost/env_excluded_arg/123,env_excluded_noarg"
+            },
+        )
+        self.env_patch.start()
+
+        self.exclude_patch = mock.patch(
+            "opentelemetry.instrumentation.urllib._excluded_urls_from_env",
+            get_excluded_urls("URLLIB"),
+        )
+        self.exclude_patch.start()
+
         URLLibInstrumentor().instrument()
         httpretty.enable()
         httpretty.register_uri(httpretty.GET, self.URL, body=b"Hello!")
         httpretty.register_uri(
             httpretty.GET,
             self.URL_TIMEOUT,
             body=self.timeout_exception_callback,
@@ -121,14 +137,44 @@
 
         self.assertIs(span.status.status_code, trace.StatusCode.UNSET)
 
         self.assertEqualSpanInstrumentationInfo(
             span, opentelemetry.instrumentation.urllib
         )
 
+    def test_excluded_urls_explicit(self):
+        url_201 = "http://httpbin.org/status/201"
+        httpretty.register_uri(
+            httpretty.GET,
+            url_201,
+            status=201,
+        )
+
+        URLLibInstrumentor().uninstrument()
+        URLLibInstrumentor().instrument(excluded_urls=".*/201")
+        self.perform_request(self.URL)
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
+        URLLibInstrumentor().uninstrument()
+        URLLibInstrumentor().instrument()
+        self.perform_request(self.URL)
+        self.perform_request(url)
+
+        self.assert_span(num_spans=1)
+
     def test_not_foundbasic(self):
         url_404 = "http://httpbin.org/status/404/"
         httpretty.register_uri(
             httpretty.GET,
             url_404,
             status=404,
         )
```

### Comparing `opentelemetry_instrumentation_urllib-0.38b0/LICENSE` & `opentelemetry_instrumentation_urllib-0.39b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_urllib-0.38b0/pyproject.toml` & `opentelemetry_instrumentation_urllib-0.39b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,24 +22,24 @@
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
 ]
 
 [project.optional-dependencies]
 instruments = []
 test = [
   "httpretty ~= 1.0",
-  "opentelemetry-test-utils == 0.38b0",
+  "opentelemetry-test-utils == 0.39b0",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 urllib = "opentelemetry.instrumentation.urllib:URLLibInstrumentor"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-urllib"
```

