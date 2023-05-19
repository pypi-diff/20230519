# Comparing `tmp/opentelemetry_instrumentation_botocore-0.38b0.tar.gz` & `tmp/opentelemetry_instrumentation_botocore-0.39b0.tar.gz`

## Comparing `opentelemetry_instrumentation_botocore-0.38b0.tar` & `opentelemetry_instrumentation_botocore-0.39b0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    10015 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.38b0/src/opentelemetry/instrumentation/botocore/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.38b0/src/opentelemetry/instrumentation/botocore/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.38b0/src/opentelemetry/instrumentation/botocore/version.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.38b0/src/opentelemetry/instrumentation/botocore/extensions/__init__.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.38b0/src/opentelemetry/instrumentation/botocore/extensions/_messaging.py
--rw-r--r--   0        0        0    13523 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.38b0/src/opentelemetry/instrumentation/botocore/extensions/dynamodb.py
--rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.38b0/src/opentelemetry/instrumentation/botocore/extensions/lmbd.py
--rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.38b0/src/opentelemetry/instrumentation/botocore/extensions/sns.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.38b0/src/opentelemetry/instrumentation/botocore/extensions/sqs.py
--rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.38b0/src/opentelemetry/instrumentation/botocore/extensions/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.38b0/tests/__init__.py
--rw-r--r--   0        0        0    17989 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.38b0/tests/test_botocore_dynamodb.py
--rw-r--r--   0        0        0    14026 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.38b0/tests/test_botocore_instrumentation.py
--rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.38b0/tests/test_botocore_lambda.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.38b0/tests/test_botocore_messaging.py
--rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.38b0/tests/test_botocore_sns.py
--rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.38b0/tests/test_botocore_sqs.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.38b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.38b0/LICENSE
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.38b0/README.rst
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.38b0/pyproject.toml
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.38b0/PKG-INFO
+-rw-r--r--   0        0        0    10015 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/version.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/__init__.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/_messaging.py
+-rw-r--r--   0        0        0    13523 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/dynamodb.py
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/lmbd.py
+-rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/sns.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/sqs.py
+-rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/tests/__init__.py
+-rw-r--r--   0        0        0    17989 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/tests/test_botocore_dynamodb.py
+-rw-r--r--   0        0        0    14026 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/tests/test_botocore_instrumentation.py
+-rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/tests/test_botocore_lambda.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/tests/test_botocore_messaging.py
+-rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/tests/test_botocore_sns.py
+-rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/tests/test_botocore_sqs.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/LICENSE
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/README.rst
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/pyproject.toml
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_botocore-0.39b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_botocore-0.38b0/src/opentelemetry/instrumentation/botocore/__init__.py` & `opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.38b0/src/opentelemetry/instrumentation/botocore/package.py` & `opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.38b0/src/opentelemetry/instrumentation/botocore/version.py` & `opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/version.py`

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

### Comparing `opentelemetry_instrumentation_botocore-0.38b0/src/opentelemetry/instrumentation/botocore/extensions/__init__.py` & `opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.38b0/src/opentelemetry/instrumentation/botocore/extensions/_messaging.py` & `opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/_messaging.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.38b0/src/opentelemetry/instrumentation/botocore/extensions/dynamodb.py` & `opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/dynamodb.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.38b0/src/opentelemetry/instrumentation/botocore/extensions/lmbd.py` & `opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/lmbd.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.38b0/src/opentelemetry/instrumentation/botocore/extensions/sns.py` & `opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/sns.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.38b0/src/opentelemetry/instrumentation/botocore/extensions/sqs.py` & `opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/sqs.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.38b0/src/opentelemetry/instrumentation/botocore/extensions/types.py` & `opentelemetry_instrumentation_botocore-0.39b0/src/opentelemetry/instrumentation/botocore/extensions/types.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.38b0/tests/test_botocore_dynamodb.py` & `opentelemetry_instrumentation_botocore-0.39b0/tests/test_botocore_dynamodb.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.38b0/tests/test_botocore_instrumentation.py` & `opentelemetry_instrumentation_botocore-0.39b0/tests/test_botocore_instrumentation.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.38b0/tests/test_botocore_lambda.py` & `opentelemetry_instrumentation_botocore-0.39b0/tests/test_botocore_lambda.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.38b0/tests/test_botocore_messaging.py` & `opentelemetry_instrumentation_botocore-0.39b0/tests/test_botocore_messaging.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.38b0/tests/test_botocore_sns.py` & `opentelemetry_instrumentation_botocore-0.39b0/tests/test_botocore_sns.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.38b0/tests/test_botocore_sqs.py` & `opentelemetry_instrumentation_botocore-0.39b0/tests/test_botocore_sqs.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.38b0/LICENSE` & `opentelemetry_instrumentation_botocore-0.39b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.38b0/README.rst` & `opentelemetry_instrumentation_botocore-0.39b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_botocore-0.38b0/pyproject.toml` & `opentelemetry_instrumentation_botocore-0.39b0/pyproject.toml`

 * *Files 0% similar despite different names*

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
 ]
 
 [project.optional-dependencies]
 instruments = [
   "botocore ~= 1.0",
 ]
 test = [
   "opentelemetry-instrumentation-botocore[instruments]",
   "markupsafe==2.0.1",
   "moto[all] ~= 2.2.6",
-  "opentelemetry-test-utils == 0.38b0",
+  "opentelemetry-test-utils == 0.39b0",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 botocore = "opentelemetry.instrumentation.botocore:BotocoreInstrumentor"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-botocore"
```

### Comparing `opentelemetry_instrumentation_botocore-0.38b0/PKG-INFO` & `opentelemetry_instrumentation_botocore-0.39b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-botocore
-Version: 0.38b0
+Version: 0.39b0
 Summary: OpenTelemetry Botocore instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-botocore
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
 Provides-Extra: instruments
 Requires-Dist: botocore~=1.0; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: markupsafe==2.0.1; extra == 'test'
 Requires-Dist: moto[all]~=2.2.6; extra == 'test'
 Requires-Dist: opentelemetry-instrumentation-botocore[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.38b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Botocore Tracing
 ==============================
 
 |pypi|
```

