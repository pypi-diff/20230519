# Comparing `tmp/opentelemetry_instrumentation_confluent_kafka-0.38b0.tar.gz` & `tmp/opentelemetry_instrumentation_confluent_kafka-0.39b0.tar.gz`

## Comparing `opentelemetry_instrumentation_confluent_kafka-0.38b0.tar` & `opentelemetry_instrumentation_confluent_kafka-0.39b0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    12300 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.38b0/src/opentelemetry/instrumentation/confluent_kafka/__init__.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.38b0/src/opentelemetry/instrumentation/confluent_kafka/package.py
--rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.38b0/src/opentelemetry/instrumentation/confluent_kafka/utils.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.38b0/src/opentelemetry/instrumentation/confluent_kafka/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.38b0/tests/__init__.py
--rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.38b0/tests/test_instrumentation.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.38b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.38b0/LICENSE
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.38b0/README.rst
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.38b0/pyproject.toml
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.38b0/PKG-INFO
+-rw-r--r--   0        0        0    12300 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.39b0/src/opentelemetry/instrumentation/confluent_kafka/__init__.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.39b0/src/opentelemetry/instrumentation/confluent_kafka/package.py
+-rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.39b0/src/opentelemetry/instrumentation/confluent_kafka/utils.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.39b0/src/opentelemetry/instrumentation/confluent_kafka/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.39b0/tests/__init__.py
+-rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.39b0/tests/test_instrumentation.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.39b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.39b0/LICENSE
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.39b0/README.rst
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.39b0/pyproject.toml
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_confluent_kafka-0.39b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_confluent_kafka-0.38b0/src/opentelemetry/instrumentation/confluent_kafka/__init__.py` & `opentelemetry_instrumentation_confluent_kafka-0.39b0/src/opentelemetry/instrumentation/confluent_kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_confluent_kafka-0.38b0/src/opentelemetry/instrumentation/confluent_kafka/package.py` & `opentelemetry_instrumentation_confluent_kafka-0.39b0/src/opentelemetry/instrumentation/confluent_kafka/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_confluent_kafka-0.38b0/src/opentelemetry/instrumentation/confluent_kafka/utils.py` & `opentelemetry_instrumentation_confluent_kafka-0.39b0/src/opentelemetry/instrumentation/confluent_kafka/utils.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_confluent_kafka-0.38b0/src/opentelemetry/instrumentation/confluent_kafka/version.py` & `opentelemetry_instrumentation_confluent_kafka-0.39b0/src/opentelemetry/instrumentation/confluent_kafka/version.py`

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

### Comparing `opentelemetry_instrumentation_confluent_kafka-0.38b0/tests/test_instrumentation.py` & `opentelemetry_instrumentation_confluent_kafka-0.39b0/tests/test_instrumentation.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_confluent_kafka-0.38b0/LICENSE` & `opentelemetry_instrumentation_confluent_kafka-0.39b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_confluent_kafka-0.38b0/README.rst` & `opentelemetry_instrumentation_confluent_kafka-0.39b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_confluent_kafka-0.38b0/pyproject.toml` & `opentelemetry_instrumentation_confluent_kafka-0.39b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_confluent_kafka-0.38b0/PKG-INFO` & `opentelemetry_instrumentation_confluent_kafka-0.39b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-confluent-kafka
-Version: 0.38b0
+Version: 0.39b0
 Summary: OpenTelemetry Confluent Kafka instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-confluent-kafka
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

