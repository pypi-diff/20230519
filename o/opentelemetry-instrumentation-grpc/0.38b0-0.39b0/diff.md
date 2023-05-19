# Comparing `tmp/opentelemetry_instrumentation_grpc-0.38b0.tar.gz` & `tmp/opentelemetry_instrumentation_grpc-0.39b0.tar.gz`

## Comparing `opentelemetry_instrumentation_grpc-0.38b0.tar` & `opentelemetry_instrumentation_grpc-0.39b0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0    19630 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/src/opentelemetry/instrumentation/grpc/__init__.py
--rw-r--r--   0        0        0     7445 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/src/opentelemetry/instrumentation/grpc/_aio_client.py
--rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/src/opentelemetry/instrumentation/grpc/_aio_server.py
--rw-r--r--   0        0        0     7428 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/src/opentelemetry/instrumentation/grpc/_client.py
--rw-r--r--   0        0        0    12086 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/src/opentelemetry/instrumentation/grpc/_server.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/src/opentelemetry/instrumentation/grpc/_utilities.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/src/opentelemetry/instrumentation/grpc/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/src/opentelemetry/instrumentation/grpc/version.py
--rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/src/opentelemetry/instrumentation/grpc/filters/__init__.py
--rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/src/opentelemetry/instrumentation/grpc/grpcext/__init__.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/src/opentelemetry/instrumentation/grpc/grpcext/_interceptor.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/tests/__init__.py
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/tests/_aio_client.py
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/tests/_client.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/tests/_server.py
--rw-r--r--   0        0        0    12603 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/tests/test_aio_client_interceptor.py
--rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/tests/test_aio_client_interceptor_filter.py
--rw-r--r--   0        0        0    20580 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/tests/test_aio_server_interceptor.py
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/tests/test_aio_server_interceptor_filter.py
--rw-r--r--   0        0        0    11954 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/tests/test_client_interceptor.py
--rw-r--r--   0        0        0    23591 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/tests/test_client_interceptor_filter.py
--rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/tests/test_filters.py
--rw-r--r--   0        0        0    23841 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/tests/test_server_interceptor.py
--rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/tests/test_server_interceptor_filter.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/tests/protobuf/test_server.proto
--rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/tests/protobuf/test_server_pb2.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/tests/protobuf/test_server_pb2_grpc.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/LICENSE
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/README.rst
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/pyproject.toml
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.38b0/PKG-INFO
+-rw-r--r--   0        0        0    21061 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/__init__.py
+-rw-r--r--   0        0        0     7930 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/_aio_client.py
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/_aio_server.py
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/_client.py
+-rw-r--r--   0        0        0    12086 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/_server.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/_utilities.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/version.py
+-rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/filters/__init__.py
+-rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/grpcext/__init__.py
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/grpcext/_interceptor.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/__init__.py
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/_aio_client.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/_client.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/_server.py
+-rw-r--r--   0        0        0    12603 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/test_aio_client_interceptor.py
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/test_aio_client_interceptor_filter.py
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/test_aio_client_interceptor_hooks.py
+-rw-r--r--   0        0        0    20580 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/test_aio_server_interceptor.py
+-rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/test_aio_server_interceptor_filter.py
+-rw-r--r--   0        0        0    11954 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/test_client_interceptor.py
+-rw-r--r--   0        0        0    23591 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/test_client_interceptor_filter.py
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/test_client_interceptor_hooks.py
+-rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/test_filters.py
+-rw-r--r--   0        0        0    23841 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/test_server_interceptor.py
+-rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/test_server_interceptor_filter.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/protobuf/test_server.proto
+-rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/protobuf/test_server_pb2.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/tests/protobuf/test_server_pb2_grpc.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/LICENSE
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/README.rst
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/pyproject.toml
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_grpc-0.39b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/src/opentelemetry/instrumentation/grpc/__init__.py` & `opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -430,14 +430,16 @@
         excluded_service_filter = _excluded_service_filter()
         if excluded_service_filter is not None:
             if filter_ is None:
                 filter_ = excluded_service_filter
             else:
                 filter_ = any_of(filter_, excluded_service_filter)
         self._filter = filter_
+        self._request_hook = None
+        self._response_hook = None
 
     # Figures out which channel type we need to wrap
     def _which_channel(self, kwargs):
         # handle legacy argument
         if "channel_type" in kwargs:
             if kwargs.get("channel_type") == "secure":
                 return ("secure_channel",)
@@ -451,33 +453,39 @@
 
         return tuple(types)
 
     def instrumentation_dependencies(self) -> Collection[str]:
         return _instruments
 
     def _instrument(self, **kwargs):
+        self._request_hook = kwargs.get("request_hook")
+        self._response_hook = kwargs.get("response_hook")
         for ctype in self._which_channel(kwargs):
             _wrap(
                 "grpc",
                 ctype,
                 self.wrapper_fn,
             )
 
     def _uninstrument(self, **kwargs):
         for ctype in self._which_channel(kwargs):
             unwrap(grpc, ctype)
 
     def wrapper_fn(self, original_func, instance, args, kwargs):
         channel = original_func(*args, **kwargs)
         tracer_provider = kwargs.get("tracer_provider")
+        request_hook = self._request_hook
+        response_hook = self._response_hook
         return intercept_channel(
             channel,
             client_interceptor(
                 tracer_provider=tracer_provider,
                 filter_=self._filter,
+                request_hook=request_hook,
+                response_hook=response_hook,
             ),
         )
 
 
 class GrpcAioInstrumentorClient(BaseInstrumentor):
     """
     Globally instrument the grpc.aio client.
@@ -495,36 +503,46 @@
         excluded_service_filter = _excluded_service_filter()
         if excluded_service_filter is not None:
             if filter_ is None:
                 filter_ = excluded_service_filter
             else:
                 filter_ = any_of(filter_, excluded_service_filter)
         self._filter = filter_
+        self._request_hook = None
+        self._response_hook = None
 
     def instrumentation_dependencies(self) -> Collection[str]:
         return _instruments
 
     def _add_interceptors(self, tracer_provider, kwargs):
         if "interceptors" in kwargs and kwargs["interceptors"]:
             kwargs["interceptors"] = (
                 aio_client_interceptors(
-                    tracer_provider=tracer_provider, filter_=self._filter
+                    tracer_provider=tracer_provider,
+                    filter_=self._filter,
+                    request_hook=self._request_hook,
+                    response_hook=self._response_hook,
                 )
                 + kwargs["interceptors"]
             )
         else:
             kwargs["interceptors"] = aio_client_interceptors(
-                tracer_provider=tracer_provider, filter_=self._filter
+                tracer_provider=tracer_provider,
+                filter_=self._filter,
+                request_hook=self._request_hook,
+                response_hook=self._response_hook,
             )
 
         return kwargs
 
     def _instrument(self, **kwargs):
         self._original_insecure = grpc.aio.insecure_channel
         self._original_secure = grpc.aio.secure_channel
+        self._request_hook = kwargs.get("request_hook")
+        self._response_hook = kwargs.get("response_hook")
         tracer_provider = kwargs.get("tracer_provider")
 
         def insecure(*args, **kwargs):
             kwargs = self._add_interceptors(tracer_provider, kwargs)
 
             return self._original_insecure(*args, **kwargs)
 
@@ -537,15 +555,17 @@
         grpc.aio.secure_channel = secure
 
     def _uninstrument(self, **kwargs):
         grpc.aio.insecure_channel = self._original_insecure
         grpc.aio.secure_channel = self._original_secure
 
 
-def client_interceptor(tracer_provider=None, filter_=None):
+def client_interceptor(
+    tracer_provider=None, filter_=None, request_hook=None, response_hook=None
+):
     """Create a gRPC client channel interceptor.
 
     Args:
         tracer: The tracer to use to create client-side spans.
 
         filter_: filter function that returns True if gRPC requests
                  matches the condition. Default is None and intercept
@@ -554,15 +574,20 @@
     Returns:
         An invocation-side interceptor object.
     """
     from . import _client
 
     tracer = trace.get_tracer(__name__, __version__, tracer_provider)
 
-    return _client.OpenTelemetryClientInterceptor(tracer, filter_=filter_)
+    return _client.OpenTelemetryClientInterceptor(
+        tracer,
+        filter_=filter_,
+        request_hook=request_hook,
+        response_hook=response_hook,
+    )
 
 
 def server_interceptor(tracer_provider=None, filter_=None):
     """Create a gRPC server interceptor.
 
     Args:
         tracer: The tracer to use to create server-side spans.
@@ -577,32 +602,54 @@
     from . import _server
 
     tracer = trace.get_tracer(__name__, __version__, tracer_provider)
 
     return _server.OpenTelemetryServerInterceptor(tracer, filter_=filter_)
 
 
-def aio_client_interceptors(tracer_provider=None, filter_=None):
+def aio_client_interceptors(
+    tracer_provider=None, filter_=None, request_hook=None, response_hook=None
+):
     """Create a gRPC client channel interceptor.
 
     Args:
         tracer: The tracer to use to create client-side spans.
 
     Returns:
         An invocation-side interceptor object.
     """
     from . import _aio_client
 
     tracer = trace.get_tracer(__name__, __version__, tracer_provider)
 
     return [
-        _aio_client.UnaryUnaryAioClientInterceptor(tracer, filter_=filter_),
-        _aio_client.UnaryStreamAioClientInterceptor(tracer, filter_=filter_),
-        _aio_client.StreamUnaryAioClientInterceptor(tracer, filter_=filter_),
-        _aio_client.StreamStreamAioClientInterceptor(tracer, filter_=filter_),
+        _aio_client.UnaryUnaryAioClientInterceptor(
+            tracer,
+            filter_=filter_,
+            request_hook=request_hook,
+            response_hook=response_hook,
+        ),
+        _aio_client.UnaryStreamAioClientInterceptor(
+            tracer,
+            filter_=filter_,
+            request_hook=request_hook,
+            response_hook=response_hook,
+        ),
+        _aio_client.StreamUnaryAioClientInterceptor(
+            tracer,
+            filter_=filter_,
+            request_hook=request_hook,
+            response_hook=response_hook,
+        ),
+        _aio_client.StreamStreamAioClientInterceptor(
+            tracer,
+            filter_=filter_,
+            request_hook=request_hook,
+            response_hook=response_hook,
+        ),
     ]
 
 
 def aio_server_interceptor(tracer_provider=None, filter_=None):
     """Create a gRPC aio server interceptor.
 
     Args:
```

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/src/opentelemetry/instrumentation/grpc/_aio_client.py` & `opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/_aio_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import functools
+import logging
 from collections import OrderedDict
 
 import grpc
 from grpc.aio import ClientCallDetails
 
 from opentelemetry import context
 from opentelemetry.instrumentation.grpc._client import (
@@ -24,29 +25,33 @@
     _carrier_setter,
 )
 from opentelemetry.instrumentation.utils import _SUPPRESS_INSTRUMENTATION_KEY
 from opentelemetry.propagate import inject
 from opentelemetry.semconv.trace import SpanAttributes
 from opentelemetry.trace.status import Status, StatusCode
 
+logger = logging.getLogger(__name__)
 
-def _unary_done_callback(span, code, details):
+
+def _unary_done_callback(span, code, details, response_hook):
     def callback(call):
         try:
             span.set_attribute(
                 SpanAttributes.RPC_GRPC_STATUS_CODE,
                 code.value[0],
             )
             if code != grpc.StatusCode.OK:
                 span.set_status(
                     Status(
                         status_code=StatusCode.ERROR,
                         description=details,
                     )
                 )
+            response_hook(span, details)
+
         finally:
             span.end()
 
     return callback
 
 
 class _BaseAioClientInterceptor(OpenTelemetryClientInterceptor):
@@ -106,24 +111,30 @@
             # code and details are both coroutines that need to be await-ed,
             # the callbacks added with add_done_callback do not allow async
             # code so we need to get the code and details here then pass them
             # to the callback.
             code = await call.code()
             details = await call.details()
 
-            call.add_done_callback(_unary_done_callback(span, code, details))
+            call.add_done_callback(
+                _unary_done_callback(
+                    span, code, details, self._call_response_hook
+                )
+            )
 
             return call
         except grpc.aio.AioRpcError as exc:
             self.add_error_details_to_span(span, exc)
             raise exc
 
     async def _wrap_stream_response(self, span, call):
         try:
             async for response in call:
+                if self._response_hook:
+                    self._call_response_hook(span, response)
                 yield response
         except Exception as exc:
             self.add_error_details_to_span(span, exc)
             raise exc
         finally:
             span.end()
 
@@ -147,14 +158,17 @@
             return await continuation(client_call_details, request)
 
         with self._start_interceptor_span(
             client_call_details.method,
         ) as span:
             new_details = self.propagate_trace_in_details(client_call_details)
 
+            if self._request_hook:
+                self._call_request_hook(span, request)
+
             continuation_with_args = functools.partial(
                 continuation, new_details, request
             )
             return await self._wrap_unary_response(
                 continuation_with_args, span
             )
 
@@ -171,15 +185,16 @@
 
         with self._start_interceptor_span(
             client_call_details.method,
         ) as span:
             new_details = self.propagate_trace_in_details(client_call_details)
 
             resp = await continuation(new_details, request)
-
+            if self._request_hook:
+                self._call_request_hook(span, request)
             return self._wrap_stream_response(span, resp)
 
 
 class StreamUnaryAioClientInterceptor(
     grpc.aio.StreamUnaryClientInterceptor,
     _BaseAioClientInterceptor,
 ):
```

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/src/opentelemetry/instrumentation/grpc/_aio_server.py` & `opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/_aio_server.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/src/opentelemetry/instrumentation/grpc/_client.py` & `opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,28 +15,31 @@
 # pylint:disable=relative-beyond-top-level
 # pylint:disable=arguments-differ
 # pylint:disable=no-member
 # pylint:disable=signature-differs
 
 """Implementation of the invocation-side open-telemetry interceptor."""
 
+import logging
 from collections import OrderedDict
-from typing import MutableMapping
+from typing import Callable, MutableMapping
 
 import grpc
 
 from opentelemetry import context, trace
 from opentelemetry.instrumentation.grpc import grpcext
 from opentelemetry.instrumentation.grpc._utilities import RpcInfo
 from opentelemetry.instrumentation.utils import _SUPPRESS_INSTRUMENTATION_KEY
 from opentelemetry.propagate import inject
 from opentelemetry.propagators.textmap import Setter
 from opentelemetry.semconv.trace import SpanAttributes
 from opentelemetry.trace.status import Status, StatusCode
 
+logger = logging.getLogger(__name__)
+
 
 class _CarrierSetter(Setter):
     """We use a custom setter in order to be able to lower case
     keys as is required by grpc.
     """
 
     def set(self, carrier: MutableMapping[str, str], key: str, value: str):
@@ -55,20 +58,35 @@
                 return
             response = response_future.result()
             rpc_info.response = response
 
     return callback
 
 
+def _safe_invoke(function: Callable, *args):
+    function_name = "<unknown>"
+    try:
+        function_name = function.__name__
+        function(*args)
+    except Exception as ex:  # pylint:disable=broad-except
+        logger.error(
+            "Error when invoking function '%s'", function_name, exc_info=ex
+        )
+
+
 class OpenTelemetryClientInterceptor(
     grpcext.UnaryClientInterceptor, grpcext.StreamClientInterceptor
 ):
-    def __init__(self, tracer, filter_=None):
+    def __init__(
+        self, tracer, filter_=None, request_hook=None, response_hook=None
+    ):
         self._tracer = tracer
         self._filter = filter_
+        self._request_hook = request_hook
+        self._response_hook = response_hook
 
     def _start_span(self, method, **kwargs):
         service, meth = method.lstrip("/").split("/", 1)
         attributes = {
             SpanAttributes.RPC_SYSTEM: "grpc",
             SpanAttributes.RPC_GRPC_STATUS_CODE: grpc.StatusCode.OK.value[0],
             SpanAttributes.RPC_METHOD: meth,
@@ -95,14 +113,16 @@
         # Handle the case when the RPC is initiated via the with_call
         # method and the result is a tuple with the first element as the
         # response.
         # http://www.grpc.io/grpc/python/grpc.html#grpc.UnaryUnaryMultiCallable.with_call
         if isinstance(result, tuple):
             response = result[0]
         rpc_info.response = response
+        if self._response_hook:
+            self._call_response_hook(span, response)
         span.end()
         return result
 
     def _intercept(self, request, metadata, client_info, invoker):
         if context.get_value(_SUPPRESS_INSTRUMENTATION_KEY):
             return invoker(request, metadata)
 
@@ -123,15 +143,16 @@
 
                 rpc_info = RpcInfo(
                     full_method=client_info.full_method,
                     metadata=metadata,
                     timeout=client_info.timeout,
                     request=request,
                 )
-
+                if self._request_hook:
+                    self._call_request_hook(span, request)
                 result = invoker(request, metadata)
             except Exception as exc:
                 if isinstance(exc, grpc.RpcError):
                     span.set_attribute(
                         SpanAttributes.RPC_GRPC_STATUS_CODE,
                         exc.code().value[0],
                     )
@@ -144,14 +165,24 @@
                 span.record_exception(exc)
                 raise exc
             finally:
                 if not result:
                     span.end()
         return self._trace_result(span, rpc_info, result)
 
+    def _call_request_hook(self, span, request):
+        if not callable(self._request_hook):
+            return
+        _safe_invoke(self._request_hook, span, request)
+
+    def _call_response_hook(self, span, response):
+        if not callable(self._response_hook):
+            return
+        _safe_invoke(self._response_hook, span, response)
+
     def intercept_unary(self, request, metadata, client_info, invoker):
         if self._filter is not None and not self._filter(client_info):
             return invoker(request, metadata)
         return self._intercept(request, metadata, client_info, invoker)
 
     # For RPCs that stream responses, the result can be a generator. To record
     # the span across the generated responses and detect any errors, we wrap
```

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/src/opentelemetry/instrumentation/grpc/_server.py` & `opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/_server.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/src/opentelemetry/instrumentation/grpc/_utilities.py` & `opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/_utilities.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/src/opentelemetry/instrumentation/grpc/package.py` & `opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/src/opentelemetry/instrumentation/grpc/version.py` & `opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/version.py`

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

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/src/opentelemetry/instrumentation/grpc/filters/__init__.py` & `opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/src/opentelemetry/instrumentation/grpc/grpcext/__init__.py` & `opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/grpcext/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/src/opentelemetry/instrumentation/grpc/grpcext/_interceptor.py` & `opentelemetry_instrumentation_grpc-0.39b0/src/opentelemetry/instrumentation/grpc/grpcext/_interceptor.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/tests/__init__.py` & `opentelemetry_instrumentation_grpc-0.39b0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/tests/_aio_client.py` & `opentelemetry_instrumentation_grpc-0.39b0/tests/_aio_client.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/tests/_client.py` & `opentelemetry_instrumentation_grpc-0.39b0/tests/_client.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/tests/_server.py` & `opentelemetry_instrumentation_grpc-0.39b0/tests/_server.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/tests/test_aio_client_interceptor.py` & `opentelemetry_instrumentation_grpc-0.39b0/tests/test_aio_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/tests/test_aio_client_interceptor_filter.py` & `opentelemetry_instrumentation_grpc-0.39b0/tests/test_aio_client_interceptor_filter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/tests/test_aio_server_interceptor.py` & `opentelemetry_instrumentation_grpc-0.39b0/tests/test_aio_server_interceptor.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/tests/test_aio_server_interceptor_filter.py` & `opentelemetry_instrumentation_grpc-0.39b0/tests/test_aio_server_interceptor_filter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/tests/test_client_interceptor.py` & `opentelemetry_instrumentation_grpc-0.39b0/tests/test_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/tests/test_client_interceptor_filter.py` & `opentelemetry_instrumentation_grpc-0.39b0/tests/test_client_interceptor_filter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/tests/test_filters.py` & `opentelemetry_instrumentation_grpc-0.39b0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/tests/test_server_interceptor.py` & `opentelemetry_instrumentation_grpc-0.39b0/tests/test_server_interceptor.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/tests/test_server_interceptor_filter.py` & `opentelemetry_instrumentation_grpc-0.39b0/tests/test_server_interceptor_filter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/tests/protobuf/test_server.proto` & `opentelemetry_instrumentation_grpc-0.39b0/tests/protobuf/test_server.proto`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/tests/protobuf/test_server_pb2.py` & `opentelemetry_instrumentation_grpc-0.39b0/tests/protobuf/test_server_pb2.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/tests/protobuf/test_server_pb2_grpc.py` & `opentelemetry_instrumentation_grpc-0.39b0/tests/protobuf/test_server_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/LICENSE` & `opentelemetry_instrumentation_grpc-0.39b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/README.rst` & `opentelemetry_instrumentation_grpc-0.39b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/pyproject.toml` & `opentelemetry_instrumentation_grpc-0.39b0/pyproject.toml`

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
+  "opentelemetry-instrumentation == 0.39b0",
   "opentelemetry-sdk ~= 1.12",
-  "opentelemetry-semantic-conventions == 0.38b0",
+  "opentelemetry-semantic-conventions == 0.39b0",
   "wrapt >= 1.0.0, < 2.0.0",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "grpcio ~= 1.27",
 ]
 test = [
   "opentelemetry-instrumentation-grpc[instruments]",
   "opentelemetry-sdk ~= 1.12",
-  "opentelemetry-test-utils == 0.38b0",
+  "opentelemetry-test-utils == 0.39b0",
   "protobuf ~= 3.13",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 grpc_client = "opentelemetry.instrumentation.grpc:GrpcInstrumentorClient"
 grpc_server = "opentelemetry.instrumentation.grpc:GrpcInstrumentorServer"
 grpc_aio_client = "opentelemetry.instrumentation.grpc:GrpcAioInstrumentorClient"
```

### Comparing `opentelemetry_instrumentation_grpc-0.38b0/PKG-INFO` & `opentelemetry_instrumentation_grpc-0.39b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-grpc
-Version: 0.38b0
+Version: 0.39b0
 Summary: OpenTelemetry gRPC instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-grpc
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
+Requires-Dist: opentelemetry-instrumentation==0.39b0
 Requires-Dist: opentelemetry-sdk~=1.12
-Requires-Dist: opentelemetry-semantic-conventions==0.38b0
+Requires-Dist: opentelemetry-semantic-conventions==0.39b0
 Requires-Dist: wrapt<2.0.0,>=1.0.0
 Provides-Extra: instruments
 Requires-Dist: grpcio~=1.27; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: opentelemetry-instrumentation-grpc[instruments]; extra == 'test'
 Requires-Dist: opentelemetry-sdk~=1.12; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.38b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
 Requires-Dist: protobuf~=3.13; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry gRPC Integration
 ==============================
 
 |pypi|
```

