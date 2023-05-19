# Comparing `tmp/opentelemetry_instrumentation_redis-0.38b0.tar.gz` & `tmp/opentelemetry_instrumentation_redis-0.39b0.tar.gz`

## Comparing `opentelemetry_instrumentation_redis-0.38b0.tar` & `opentelemetry_instrumentation_redis-0.39b0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11821 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.38b0/src/opentelemetry/instrumentation/redis/__init__.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.38b0/src/opentelemetry/instrumentation/redis/environment_variables.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.38b0/src/opentelemetry/instrumentation/redis/package.py
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.38b0/src/opentelemetry/instrumentation/redis/util.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.38b0/src/opentelemetry/instrumentation/redis/version.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.38b0/tests/__init__.py
--rw-r--r--   0        0        0     7488 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.38b0/tests/test_redis.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.38b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.38b0/LICENSE
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.38b0/README.rst
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.38b0/pyproject.toml
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.38b0/PKG-INFO
+-rw-r--r--   0        0        0    11821 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.39b0/src/opentelemetry/instrumentation/redis/__init__.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.39b0/src/opentelemetry/instrumentation/redis/environment_variables.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.39b0/src/opentelemetry/instrumentation/redis/package.py
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.39b0/src/opentelemetry/instrumentation/redis/util.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.39b0/src/opentelemetry/instrumentation/redis/version.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.39b0/tests/__init__.py
+-rw-r--r--   0        0        0     7488 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.39b0/tests/test_redis.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.39b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.39b0/LICENSE
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.39b0/README.rst
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.39b0/pyproject.toml
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_redis-0.39b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_redis-0.38b0/src/opentelemetry/instrumentation/redis/__init__.py` & `opentelemetry_instrumentation_redis-0.39b0/src/opentelemetry/instrumentation/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_redis-0.38b0/src/opentelemetry/instrumentation/redis/environment_variables.py` & `opentelemetry_instrumentation_redis-0.39b0/src/opentelemetry/instrumentation/redis/environment_variables.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_redis-0.38b0/src/opentelemetry/instrumentation/redis/package.py` & `opentelemetry_instrumentation_redis-0.39b0/src/opentelemetry/instrumentation/redis/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_redis-0.38b0/src/opentelemetry/instrumentation/redis/util.py` & `opentelemetry_instrumentation_redis-0.39b0/src/opentelemetry/instrumentation/redis/util.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_redis-0.38b0/src/opentelemetry/instrumentation/redis/version.py` & `opentelemetry_instrumentation_redis-0.39b0/src/opentelemetry/instrumentation/redis/version.py`

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

### Comparing `opentelemetry_instrumentation_redis-0.38b0/tests/__init__.py` & `opentelemetry_instrumentation_redis-0.39b0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_redis-0.38b0/tests/test_redis.py` & `opentelemetry_instrumentation_redis-0.39b0/tests/test_redis.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_redis-0.38b0/LICENSE` & `opentelemetry_instrumentation_redis-0.39b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_redis-0.38b0/README.rst` & `opentelemetry_instrumentation_redis-0.39b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_redis-0.38b0/pyproject.toml` & `opentelemetry_instrumentation_redis-0.39b0/pyproject.toml`

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
+  "opentelemetry-instrumentation == 0.39b0",
+  "opentelemetry-semantic-conventions == 0.39b0",
   "wrapt >= 1.12.1",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "redis >= 2.6",
 ]
 test = [
   "opentelemetry-instrumentation-redis[instruments]",
   "opentelemetry-sdk ~= 1.3",
-  "opentelemetry-test-utils == 0.38b0",
+  "opentelemetry-test-utils == 0.39b0",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 redis = "opentelemetry.instrumentation.redis:RedisInstrumentor"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-redis"
```

### Comparing `opentelemetry_instrumentation_redis-0.38b0/PKG-INFO` & `opentelemetry_instrumentation_redis-0.39b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-redis
-Version: 0.38b0
+Version: 0.39b0
 Summary: OpenTelemetry Redis instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-redis
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
 Requires-Dist: wrapt>=1.12.1
 Provides-Extra: instruments
 Requires-Dist: redis>=2.6; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: opentelemetry-instrumentation-redis[instruments]; extra == 'test'
 Requires-Dist: opentelemetry-sdk~=1.3; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.38b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Redis Instrumentation
 ===================================
 
 |pypi|
```

