# Comparing `tmp/opentelemetry_instrumentation_requests-0.38b0.tar.gz` & `tmp/opentelemetry_instrumentation_requests-0.39b0.tar.gz`

## Comparing `opentelemetry_instrumentation_requests-0.38b0.tar` & `opentelemetry_instrumentation_requests-0.39b0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10722 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.38b0/src/opentelemetry/instrumentation/requests/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.38b0/src/opentelemetry/instrumentation/requests/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.38b0/src/opentelemetry/instrumentation/requests/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.38b0/tests/__init__.py
--rw-r--r--   0        0        0    17436 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.38b0/tests/test_requests_integration.py
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.38b0/tests/test_requests_ip_support.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.38b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.38b0/LICENSE
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.38b0/README.rst
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.38b0/pyproject.toml
--rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.38b0/PKG-INFO
+-rw-r--r--   0        0        0    10727 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.39b0/src/opentelemetry/instrumentation/requests/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.39b0/src/opentelemetry/instrumentation/requests/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.39b0/src/opentelemetry/instrumentation/requests/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.39b0/tests/__init__.py
+-rw-r--r--   0        0        0    17436 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.39b0/tests/test_requests_integration.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.39b0/tests/test_requests_ip_support.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.39b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.39b0/LICENSE
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.39b0/README.rst
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.39b0/pyproject.toml
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_requests-0.39b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_requests-0.38b0/src/opentelemetry/instrumentation/requests/__init__.py` & `opentelemetry_instrumentation_requests-0.39b0/src/opentelemetry/instrumentation/requests/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 API
 ---
 """
 
 import functools
 import types
 from timeit import default_timer
-from typing import Callable, Collection, Iterable, Optional
+from typing import Callable, Collection, Optional
 from urllib.parse import urlparse
 
 from requests.models import PreparedRequest, Response
 from requests.sessions import Session
 from requests.structures import CaseInsensitiveDict
 
 from opentelemetry import context
@@ -73,14 +73,15 @@
 from opentelemetry.propagate import inject
 from opentelemetry.semconv.metrics import MetricInstruments
 from opentelemetry.semconv.trace import SpanAttributes
 from opentelemetry.trace import SpanKind, Tracer, get_tracer
 from opentelemetry.trace.span import Span
 from opentelemetry.trace.status import Status
 from opentelemetry.util.http import (
+    ExcludeList,
     get_excluded_urls,
     parse_excluded_urls,
     remove_url_credentials,
 )
 from opentelemetry.util.http.httplib import set_ip_on_next_http_connection
 
 _excluded_urls_from_env = get_excluded_urls("REQUESTS")
@@ -92,15 +93,15 @@
 # pylint: disable=unused-argument
 # pylint: disable=R0915
 def _instrument(
     tracer: Tracer,
     duration_histogram: Histogram,
     request_hook: _RequestHookT = None,
     response_hook: _ResponseHookT = None,
-    excluded_urls: Iterable[str] = None,
+    excluded_urls: ExcludeList = None,
 ):
     """Enables tracing of all requests calls that go through
     :code:`requests.session.Session.request` (this includes
     :code:`requests.get`, etc.)."""
 
     # Since
     # https://github.com/psf/requests/commit/d72d1162142d1bf8b1b5711c664fbbd674f349d1
```

### Comparing `opentelemetry_instrumentation_requests-0.38b0/src/opentelemetry/instrumentation/requests/package.py` & `opentelemetry_instrumentation_requests-0.39b0/src/opentelemetry/instrumentation/requests/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_requests-0.38b0/src/opentelemetry/instrumentation/requests/version.py` & `opentelemetry_instrumentation_requests-0.39b0/src/opentelemetry/instrumentation/requests/version.py`

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

### Comparing `opentelemetry_instrumentation_requests-0.38b0/tests/test_requests_integration.py` & `opentelemetry_instrumentation_requests-0.39b0/tests/test_requests_integration.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_requests-0.38b0/tests/test_requests_ip_support.py` & `opentelemetry_instrumentation_requests-0.39b0/tests/test_requests_ip_support.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_requests-0.38b0/LICENSE` & `opentelemetry_instrumentation_requests-0.39b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_requests-0.38b0/README.rst` & `opentelemetry_instrumentation_requests-0.39b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_requests-0.38b0/pyproject.toml` & `opentelemetry_instrumentation_requests-0.39b0/pyproject.toml`

 * *Files 5% similar despite different names*

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
-  "opentelemetry-util-http == 0.38b0",
+  "opentelemetry-instrumentation == 0.39b0",
+  "opentelemetry-semantic-conventions == 0.39b0",
+  "opentelemetry-util-http == 0.39b0",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "requests ~= 2.0",
 ]
 test = [
   "opentelemetry-instrumentation-requests[instruments]",
   "httpretty ~= 1.0",
-  "opentelemetry-test-utils == 0.38b0",
+  "opentelemetry-test-utils == 0.39b0",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 requests = "opentelemetry.instrumentation.requests:RequestsInstrumentor"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-requests"
```

### Comparing `opentelemetry_instrumentation_requests-0.38b0/PKG-INFO` & `opentelemetry_instrumentation_requests-0.39b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-requests
-Version: 0.38b0
+Version: 0.39b0
 Summary: OpenTelemetry requests instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-requests
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
-Requires-Dist: opentelemetry-util-http==0.38b0
+Requires-Dist: opentelemetry-instrumentation==0.39b0
+Requires-Dist: opentelemetry-semantic-conventions==0.39b0
+Requires-Dist: opentelemetry-util-http==0.39b0
 Provides-Extra: instruments
 Requires-Dist: requests~=2.0; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: httpretty~=1.0; extra == 'test'
 Requires-Dist: opentelemetry-instrumentation-requests[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.38b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Requests Instrumentation
 ======================================
 
 |pypi|
```

