# Comparing `tmp/opentelemetry_instrumentation_system_metrics-0.38b0.tar.gz` & `tmp/opentelemetry_instrumentation_system_metrics-0.39b0.tar.gz`

## Comparing `opentelemetry_instrumentation_system_metrics-0.38b0.tar` & `opentelemetry_instrumentation_system_metrics-0.39b0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    26415 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.38b0/src/opentelemetry/instrumentation/system_metrics/__init__.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.38b0/src/opentelemetry/instrumentation/system_metrics/package.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.38b0/src/opentelemetry/instrumentation/system_metrics/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.38b0/tests/__init__.py
--rw-r--r--   0        0        0    25876 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.38b0/tests/test_system_metrics.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.38b0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.38b0/LICENSE
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.38b0/README.rst
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.38b0/pyproject.toml
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.38b0/PKG-INFO
+-rw-r--r--   0        0        0    26543 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.39b0/src/opentelemetry/instrumentation/system_metrics/__init__.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.39b0/src/opentelemetry/instrumentation/system_metrics/package.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.39b0/src/opentelemetry/instrumentation/system_metrics/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.39b0/tests/__init__.py
+-rw-r--r--   0        0        0    26038 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.39b0/tests/test_system_metrics.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.39b0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.39b0/LICENSE
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.39b0/README.rst
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.39b0/pyproject.toml
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_system_metrics-0.39b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_system_metrics-0.38b0/src/opentelemetry/instrumentation/system_metrics/__init__.py` & `opentelemetry_instrumentation_system_metrics-0.39b0/src/opentelemetry/instrumentation/system_metrics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,16 @@
         "system.disk.time": ["read", "write"],
         "system.network.dropped.packets": ["transmit", "receive"],
         "system.network.packets": ["transmit", "receive"],
         "system.network.errors": ["transmit", "receive"],
         "system.network.io": ["transmit", "receive"],
         "system.network.connections": ["family", "type"],
         "system.thread_count": None
-        "runtime.memory": ["rss", "vms"],
-        "runtime.cpu.time": ["user", "system"],
+        "process.runtime.memory": ["rss", "vms"],
+        "process.runtime.cpu.time": ["user", "system"],
     }
 
 Usage
 -----
 
 .. code:: python
 
@@ -57,16 +57,16 @@
     input("...")
 
     # to configure custom metrics
     configuration = {
         "system.memory.usage": ["used", "free", "cached"],
         "system.cpu.time": ["idle", "user", "system", "irq"],
         "system.network.io": ["transmit", "receive"],
-        "runtime.memory": ["rss", "vms"],
-        "runtime.cpu.time": ["user", "system"],
+        "process.runtime.memory": ["rss", "vms"],
+        "process.runtime.cpu.time": ["user", "system"],
     }
     SystemMetricsInstrumentor(config=configuration).instrument()
 
 API
 ---
 """
 
@@ -98,17 +98,17 @@
     "system.disk.time": ["read", "write"],
     "system.network.dropped.packets": ["transmit", "receive"],
     "system.network.packets": ["transmit", "receive"],
     "system.network.errors": ["transmit", "receive"],
     "system.network.io": ["transmit", "receive"],
     "system.network.connections": ["family", "type"],
     "system.thread_count": None,
-    "runtime.memory": ["rss", "vms"],
-    "runtime.cpu.time": ["user", "system"],
-    "runtime.gc_count": None,
+    "process.runtime.memory": ["rss", "vms"],
+    "process.runtime.cpu.time": ["user", "system"],
+    "process.runtime.gc_count": None,
 }
 
 
 class SystemMetricsInstrumentor(BaseInstrumentor):
     def __init__(
         self,
         labels: Optional[Dict[str, str]] = None,
@@ -319,33 +319,33 @@
         if "system.thread_count" in self._config:
             self._meter.create_observable_gauge(
                 name="system.thread_count",
                 callbacks=[self._get_system_thread_count],
                 description="System active threads count",
             )
 
-        if "runtime.memory" in self._config:
-            self._meter.create_observable_counter(
-                name=f"runtime.{self._python_implementation}.memory",
+        if "process.runtime.memory" in self._config:
+            self._meter.create_observable_up_down_counter(
+                name=f"process.runtime.{self._python_implementation}.memory",
                 callbacks=[self._get_runtime_memory],
                 description=f"Runtime {self._python_implementation} memory",
                 unit="bytes",
             )
 
-        if "runtime.cpu.time" in self._config:
+        if "process.runtime.cpu.time" in self._config:
             self._meter.create_observable_counter(
-                name=f"runtime.{self._python_implementation}.cpu_time",
+                name=f"process.runtime.{self._python_implementation}.cpu_time",
                 callbacks=[self._get_runtime_cpu_time],
                 description=f"Runtime {self._python_implementation} CPU time",
                 unit="seconds",
             )
 
-        if "runtime.gc_count" in self._config:
+        if "process.runtime.gc_count" in self._config:
             self._meter.create_observable_counter(
-                name=f"runtime.{self._python_implementation}.gc_count",
+                name=f"process.runtime.{self._python_implementation}.gc_count",
                 callbacks=[self._get_runtime_gc_count],
                 description=f"Runtime {self._python_implementation} GC count",
                 unit="bytes",
             )
 
     def _uninstrument(self, **__):
         pass
@@ -614,28 +614,28 @@
         )
 
     def _get_runtime_memory(
         self, options: CallbackOptions
     ) -> Iterable[Observation]:
         """Observer callback for runtime memory"""
         proc_memory = self._proc.memory_info()
-        for metric in self._config["runtime.memory"]:
+        for metric in self._config["process.runtime.memory"]:
             if hasattr(proc_memory, metric):
                 self._runtime_memory_labels["type"] = metric
                 yield Observation(
                     getattr(proc_memory, metric),
                     self._runtime_memory_labels.copy(),
                 )
 
     def _get_runtime_cpu_time(
         self, options: CallbackOptions
     ) -> Iterable[Observation]:
         """Observer callback for runtime CPU time"""
         proc_cpu = self._proc.cpu_times()
-        for metric in self._config["runtime.cpu.time"]:
+        for metric in self._config["process.runtime.cpu.time"]:
             if hasattr(proc_cpu, metric):
                 self._runtime_cpu_time_labels["type"] = metric
                 yield Observation(
                     getattr(proc_cpu, metric),
                     self._runtime_cpu_time_labels.copy(),
                 )
```

### Comparing `opentelemetry_instrumentation_system_metrics-0.38b0/src/opentelemetry/instrumentation/system_metrics/package.py` & `opentelemetry_instrumentation_system_metrics-0.39b0/src/opentelemetry/instrumentation/system_metrics/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_system_metrics-0.38b0/src/opentelemetry/instrumentation/system_metrics/version.py` & `opentelemetry_instrumentation_system_metrics-0.39b0/src/opentelemetry/instrumentation/system_metrics/version.py`

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

### Comparing `opentelemetry_instrumentation_system_metrics-0.38b0/tests/test_system_metrics.py` & `opentelemetry_instrumentation_system_metrics-0.39b0/tests/test_system_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,28 +110,28 @@
             "system.disk.time",
             "system.network.dropped_packets",
             "system.network.packets",
             "system.network.errors",
             "system.network.io",
             "system.network.connections",
             "system.thread_count",
-            f"runtime.{self.implementation}.memory",
-            f"runtime.{self.implementation}.cpu_time",
-            f"runtime.{self.implementation}.gc_count",
+            f"process.runtime.{self.implementation}.memory",
+            f"process.runtime.{self.implementation}.cpu_time",
+            f"process.runtime.{self.implementation}.gc_count",
         ]
 
         for observer in metric_names:
             self.assertIn(observer, observer_names)
             observer_names.remove(observer)
 
     def test_runtime_metrics_instrument(self):
         runtime_config = {
-            "runtime.memory": ["rss", "vms"],
-            "runtime.cpu.time": ["user", "system"],
-            "runtime.gc_count": None,
+            "process.runtime.memory": ["rss", "vms"],
+            "process.runtime.cpu.time": ["user", "system"],
+            "process.runtime.gc_count": None,
         }
 
         reader = InMemoryMetricReader()
         meter_provider = MeterProvider(metric_readers=[reader])
         runtime_metrics = SystemMetricsInstrumentor(config=runtime_config)
         runtime_metrics.instrument(meter_provider=meter_provider)
 
@@ -139,17 +139,17 @@
         for resource_metrics in reader.get_metrics_data().resource_metrics:
             for scope_metrics in resource_metrics.scope_metrics:
                 for metric in scope_metrics.metrics:
                     metric_names.append(metric.name)
         self.assertEqual(len(metric_names), 3)
 
         observer_names = [
-            f"runtime.{self.implementation}.memory",
-            f"runtime.{self.implementation}.cpu_time",
-            f"runtime.{self.implementation}.gc_count",
+            f"process.runtime.{self.implementation}.memory",
+            f"process.runtime.{self.implementation}.cpu_time",
+            f"process.runtime.{self.implementation}.gc_count",
         ]
 
         for observer in metric_names:
             self.assertIn(observer, observer_names)
             observer_names.remove(observer)
 
     def _assert_metrics(self, observer_name, reader, expected):
@@ -746,33 +746,39 @@
             **{"return_value": PMem(rss=1, vms=2)}
         )
 
         expected = [
             _SystemMetricsResult({"type": "rss"}, 1),
             _SystemMetricsResult({"type": "vms"}, 2),
         ]
-        self._test_metrics(f"runtime.{self.implementation}.memory", expected)
+        self._test_metrics(
+            f"process.runtime.{self.implementation}.memory", expected
+        )
 
     @mock.patch("psutil.Process.cpu_times")
     def test_runtime_cpu_time(self, mock_process_cpu_times):
         PCPUTimes = namedtuple("PCPUTimes", ["user", "system"])
 
         mock_process_cpu_times.configure_mock(
             **{"return_value": PCPUTimes(user=1.1, system=2.2)}
         )
 
         expected = [
             _SystemMetricsResult({"type": "user"}, 1.1),
             _SystemMetricsResult({"type": "system"}, 2.2),
         ]
-        self._test_metrics(f"runtime.{self.implementation}.cpu_time", expected)
+        self._test_metrics(
+            f"process.runtime.{self.implementation}.cpu_time", expected
+        )
 
     @mock.patch("gc.get_count")
     def test_runtime_get_count(self, mock_gc_get_count):
         mock_gc_get_count.configure_mock(**{"return_value": (1, 2, 3)})
 
         expected = [
             _SystemMetricsResult({"count": "0"}, 1),
             _SystemMetricsResult({"count": "1"}, 2),
             _SystemMetricsResult({"count": "2"}, 3),
         ]
-        self._test_metrics(f"runtime.{self.implementation}.gc_count", expected)
+        self._test_metrics(
+            f"process.runtime.{self.implementation}.gc_count", expected
+        )
```

### Comparing `opentelemetry_instrumentation_system_metrics-0.38b0/LICENSE` & `opentelemetry_instrumentation_system_metrics-0.39b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_system_metrics-0.38b0/README.rst` & `opentelemetry_instrumentation_system_metrics-0.39b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_system_metrics-0.38b0/pyproject.toml` & `opentelemetry_instrumentation_system_metrics-0.39b0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 [project.optional-dependencies]
 instruments = [
   "psutil >= 5",
 ]
 test = [
   "opentelemetry-instrumentation-system-metrics[instruments]",
-  "opentelemetry-test-utils == 0.38b0",
+  "opentelemetry-test-utils == 0.39b0",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 system_metrics = "opentelemetry.instrumentation.system_metrics:SystemMetricsInstrumentor"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-system-metrics"
```

### Comparing `opentelemetry_instrumentation_system_metrics-0.38b0/PKG-INFO` & `opentelemetry_instrumentation_system_metrics-0.39b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-system-metrics
-Version: 0.38b0
+Version: 0.39b0
 Summary: OpenTelemetry System Metrics Instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-system-metrics
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 Requires-Dist: opentelemetry-api~=1.11
 Requires-Dist: opentelemetry-sdk~=1.11
 Requires-Dist: psutil~=5.9
 Provides-Extra: instruments
 Requires-Dist: psutil>=5; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: opentelemetry-instrumentation-system-metrics[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.38b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry System Metrics Instrumentation
 ============================================
 
 |pypi|
```

