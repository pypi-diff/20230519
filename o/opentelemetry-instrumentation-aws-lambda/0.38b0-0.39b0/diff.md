# Comparing `tmp/opentelemetry_instrumentation_aws_lambda-0.38b0.tar.gz` & `tmp/opentelemetry_instrumentation_aws_lambda-0.39b0.tar.gz`

## Comparing `opentelemetry_instrumentation_aws_lambda-0.38b0.tar` & `opentelemetry_instrumentation_aws_lambda-0.39b0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    17400 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.38b0/src/opentelemetry/instrumentation/aws_lambda/__init__.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.38b0/src/opentelemetry/instrumentation/aws_lambda/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.38b0/src/opentelemetry/instrumentation/aws_lambda/version.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.38b0/tests/test_aws_lambda_instrumentation.py
--rw-r--r--   0        0        0    16522 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.38b0/tests/test_aws_lambda_instrumentation_manual.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.38b0/tests/mocks/api_gateway_http_api_event.py
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.38b0/tests/mocks/api_gateway_proxy_event.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.38b0/tests/mocks/lambda_function.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.38b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.38b0/LICENSE
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.38b0/README.rst
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.38b0/pyproject.toml
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.38b0/PKG-INFO
+-rw-r--r--   0        0        0    17448 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/src/opentelemetry/instrumentation/aws_lambda/__init__.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/src/opentelemetry/instrumentation/aws_lambda/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/src/opentelemetry/instrumentation/aws_lambda/version.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/tests/test_aws_lambda_instrumentation.py
+-rw-r--r--   0        0        0    16747 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/tests/test_aws_lambda_instrumentation_manual.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/tests/mocks/api_gateway_http_api_event.py
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/tests/mocks/api_gateway_proxy_event.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/tests/mocks/lambda_function.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/LICENSE
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/README.rst
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/pyproject.toml
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_aws_lambda-0.39b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_aws_lambda-0.38b0/src/opentelemetry/instrumentation/aws_lambda/__init__.py` & `opentelemetry_instrumentation_aws_lambda-0.39b0/src/opentelemetry/instrumentation/aws_lambda/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,15 +338,17 @@
                 )
 
             result = call_wrapped(*args, **kwargs)
 
             # If the request came from an API Gateway, extract http attributes from the event
             # https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/trace/semantic_conventions/instrumentation/aws-lambda.md#api-gateway
             # https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/trace/semantic_conventions/http.md#http-server-semantic-conventions
-            if lambda_event and lambda_event.get("requestContext"):
+            if isinstance(lambda_event, dict) and lambda_event.get(
+                "requestContext"
+            ):
                 span.set_attribute(SpanAttributes.FAAS_TRIGGER, "http")
 
                 if lambda_event.get("version") == "2.0":
                     _set_api_gateway_v2_proxy_attributes(lambda_event, span)
                 else:
                     _set_api_gateway_v1_proxy_attributes(lambda_event, span)
```

### Comparing `opentelemetry_instrumentation_aws_lambda-0.38b0/src/opentelemetry/instrumentation/aws_lambda/package.py` & `opentelemetry_instrumentation_aws_lambda-0.39b0/src/opentelemetry/instrumentation/aws_lambda/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aws_lambda-0.38b0/src/opentelemetry/instrumentation/aws_lambda/version.py` & `opentelemetry_instrumentation_aws_lambda-0.39b0/src/opentelemetry/instrumentation/aws_lambda/version.py`

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

### Comparing `opentelemetry_instrumentation_aws_lambda-0.38b0/tests/test_aws_lambda_instrumentation.py` & `opentelemetry_instrumentation_aws_lambda-0.39b0/tests/test_aws_lambda_instrumentation.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aws_lambda-0.38b0/tests/test_aws_lambda_instrumentation_manual.py` & `opentelemetry_instrumentation_aws_lambda-0.39b0/tests/test_aws_lambda_instrumentation_manual.py`

 * *Files 2% similar despite different names*

```diff
@@ -395,14 +395,23 @@
                 SpanAttributes.HTTP_ROUTE: "/path/to/resource",
                 SpanAttributes.HTTP_TARGET: "/path/to/resource?parameter1=value1&parameter1=value2&parameter2=value",
                 SpanAttributes.NET_HOST_NAME: "id.execute-api.us-east-1.amazonaws.com",
                 SpanAttributes.HTTP_USER_AGENT: "agent",
             },
         )
 
+    def test_lambda_handles_list_event(self):
+        AwsLambdaInstrumentor().instrument()
+
+        mock_execute_lambda([{"message": "test"}])
+
+        spans = self.memory_exporter.get_finished_spans()
+
+        assert spans
+
     def test_uninstrument(self):
         AwsLambdaInstrumentor().instrument()
 
         mock_execute_lambda(MOCK_LAMBDA_API_GATEWAY_HTTP_API_EVENT)
 
         spans = self.memory_exporter.get_finished_spans()
         self.assertEqual(len(spans), 1)
```

### Comparing `opentelemetry_instrumentation_aws_lambda-0.38b0/tests/mocks/api_gateway_http_api_event.py` & `opentelemetry_instrumentation_aws_lambda-0.39b0/tests/mocks/api_gateway_http_api_event.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aws_lambda-0.38b0/tests/mocks/api_gateway_proxy_event.py` & `opentelemetry_instrumentation_aws_lambda-0.39b0/tests/mocks/api_gateway_proxy_event.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aws_lambda-0.38b0/tests/mocks/lambda_function.py` & `opentelemetry_instrumentation_aws_lambda-0.39b0/tests/mocks/lambda_function.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aws_lambda-0.38b0/LICENSE` & `opentelemetry_instrumentation_aws_lambda-0.39b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aws_lambda-0.38b0/README.rst` & `opentelemetry_instrumentation_aws_lambda-0.39b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_aws_lambda-0.38b0/pyproject.toml` & `opentelemetry_instrumentation_aws_lambda-0.39b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,23 +18,23 @@
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
 ]
 dependencies = [
-  "opentelemetry-instrumentation == 0.38b0",
+  "opentelemetry-instrumentation == 0.39b0",
   "opentelemetry-propagator-aws-xray == 1.0.1",
-  "opentelemetry-semantic-conventions == 0.38b0",
+  "opentelemetry-semantic-conventions == 0.39b0",
 ]
 
 [project.optional-dependencies]
 instruments = []
 test = [
-  "opentelemetry-test-utils == 0.38b0",
+  "opentelemetry-test-utils == 0.39b0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-aws-lambda"
 
 [tool.hatch.version]
 path = "src/opentelemetry/instrumentation/aws_lambda/version.py"
```

### Comparing `opentelemetry_instrumentation_aws_lambda-0.38b0/PKG-INFO` & `opentelemetry_instrumentation_aws_lambda-0.39b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-aws-lambda
-Version: 0.38b0
+Version: 0.39b0
 Summary: OpenTelemetry AWS Lambda instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-aws-lambda
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
-Requires-Dist: opentelemetry-instrumentation==0.38b0
+Requires-Dist: opentelemetry-instrumentation==0.39b0
 Requires-Dist: opentelemetry-propagator-aws-xray==1.0.1
-Requires-Dist: opentelemetry-semantic-conventions==0.38b0
+Requires-Dist: opentelemetry-semantic-conventions==0.39b0
 Provides-Extra: instruments
 Provides-Extra: test
-Requires-Dist: opentelemetry-test-utils==0.38b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry AWS Lambda Tracing
 ================================
 
 |pypi|
```

