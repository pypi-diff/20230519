# Comparing `tmp/opentelemetry_instrumentation_sqlalchemy-0.38b0.tar.gz` & `tmp/opentelemetry_instrumentation_sqlalchemy-0.39b0.tar.gz`

## Comparing `opentelemetry_instrumentation_sqlalchemy-0.38b0.tar` & `opentelemetry_instrumentation_sqlalchemy-0.39b0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     6949 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.38b0/src/opentelemetry/instrumentation/sqlalchemy/__init__.py
--rw-r--r--   0        0        0    10446 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.38b0/src/opentelemetry/instrumentation/sqlalchemy/engine.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.38b0/src/opentelemetry/instrumentation/sqlalchemy/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.38b0/src/opentelemetry/instrumentation/sqlalchemy/version.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.38b0/tests/__init__.py
--rw-r--r--   0        0        0    12175 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.38b0/tests/test_sqlalchemy.py
--rw-r--r--   0        0        0     5048 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.38b0/tests/test_sqlalchemy_metrics.py
--rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.38b0/tests/test_sqlcommenter.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.38b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.38b0/LICENSE
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.38b0/README.rst
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.38b0/pyproject.toml
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.38b0/PKG-INFO
+-rw-r--r--   0        0        0     6949 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/src/opentelemetry/instrumentation/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0    10828 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/src/opentelemetry/instrumentation/sqlalchemy/engine.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/src/opentelemetry/instrumentation/sqlalchemy/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/src/opentelemetry/instrumentation/sqlalchemy/version.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/tests/__init__.py
+-rw-r--r--   0        0        0    12175 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/tests/test_sqlalchemy.py
+-rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/tests/test_sqlalchemy_metrics.py
+-rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/tests/test_sqlcommenter.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/LICENSE
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/README.rst
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/pyproject.toml
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_sqlalchemy-0.39b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_sqlalchemy-0.38b0/src/opentelemetry/instrumentation/sqlalchemy/__init__.py` & `opentelemetry_instrumentation_sqlalchemy-0.39b0/src/opentelemetry/instrumentation/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_sqlalchemy-0.38b0/src/opentelemetry/instrumentation/sqlalchemy/engine.py` & `opentelemetry_instrumentation_sqlalchemy-0.39b0/src/opentelemetry/instrumentation/sqlalchemy/engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,16 +114,25 @@
         )
         self._register_event_listener(engine, "handle_error", _handle_error)
         self._register_event_listener(engine, "connect", self._pool_connect)
         self._register_event_listener(engine, "close", self._pool_close)
         self._register_event_listener(engine, "checkin", self._pool_checkin)
         self._register_event_listener(engine, "checkout", self._pool_checkout)
 
+    def _get_connection_string(self):
+        drivername = self.engine.url.drivername or ""
+        host = self.engine.url.host or ""
+        port = self.engine.url.port or ""
+        database = self.engine.url.database or ""
+        return f"{drivername}://{host}:{port}/{database}"
+
     def _get_pool_name(self):
-        return self.engine.pool.logging_name or ""
+        if self.engine.pool.logging_name is not None:
+            return self.engine.pool.logging_name
+        return self._get_connection_string()
 
     def _add_idle_to_connection_usage(self, value):
         self.connections_usage.add(
             value,
             attributes={
                 "pool.name": self._get_pool_name(),
                 "state": "idle",
```

### Comparing `opentelemetry_instrumentation_sqlalchemy-0.38b0/src/opentelemetry/instrumentation/sqlalchemy/package.py` & `opentelemetry_instrumentation_sqlalchemy-0.39b0/src/opentelemetry/instrumentation/sqlalchemy/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_sqlalchemy-0.38b0/src/opentelemetry/instrumentation/sqlalchemy/version.py` & `opentelemetry_instrumentation_sqlalchemy-0.39b0/src/opentelemetry/instrumentation/sqlalchemy/version.py`

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

### Comparing `opentelemetry_instrumentation_sqlalchemy-0.38b0/tests/__init__.py` & `opentelemetry_instrumentation_sqlalchemy-0.39b0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_sqlalchemy-0.38b0/tests/test_sqlalchemy.py` & `opentelemetry_instrumentation_sqlalchemy-0.39b0/tests/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_sqlalchemy-0.38b0/tests/test_sqlalchemy_metrics.py` & `opentelemetry_instrumentation_sqlalchemy-0.39b0/tests/test_sqlalchemy_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,19 +66,20 @@
 
         # After the connection is closed
         self.assert_pool_idle_used_expected(
             pool_name=pool_name, idle=1, used=0
         )
 
     def test_metrics_without_pool_name(self):
-        pool_name = ""
+        pool_name = "pool_test_name"
         engine = sqlalchemy.create_engine(
             "sqlite:///:memory:",
             pool_size=5,
             poolclass=QueuePool,
+            pool_logging_name=pool_name,
         )
 
         metrics = self.get_sorted_metrics()
         self.assertEqual(len(metrics), 0)
 
         with engine.connect():
             self.assert_pool_idle_used_expected(
```

### Comparing `opentelemetry_instrumentation_sqlalchemy-0.38b0/tests/test_sqlcommenter.py` & `opentelemetry_instrumentation_sqlalchemy-0.39b0/tests/test_sqlcommenter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_sqlalchemy-0.38b0/LICENSE` & `opentelemetry_instrumentation_sqlalchemy-0.39b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_sqlalchemy-0.38b0/README.rst` & `opentelemetry_instrumentation_sqlalchemy-0.39b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_sqlalchemy-0.38b0/pyproject.toml` & `opentelemetry_instrumentation_sqlalchemy-0.39b0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,16 @@
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
   "packaging >= 21.0",
   "wrapt >= 1.11.2",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "sqlalchemy",
```

### Comparing `opentelemetry_instrumentation_sqlalchemy-0.38b0/PKG-INFO` & `opentelemetry_instrumentation_sqlalchemy-0.39b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-sqlalchemy
-Version: 0.38b0
+Version: 0.39b0
 Summary: OpenTelemetry SQLAlchemy instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-sqlalchemy
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,16 +14,16 @@
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
 Requires-Dist: packaging>=21.0
 Requires-Dist: wrapt>=1.11.2
 Provides-Extra: instruments
 Requires-Dist: sqlalchemy; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: opentelemetry-instrumentation-sqlalchemy[instruments]; extra == 'test'
 Requires-Dist: opentelemetry-sdk~=1.12; extra == 'test'
```

