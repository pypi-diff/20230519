# Comparing `tmp/async_adbc-1.0.4.tar.gz` & `tmp/async_adbc-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_adbc-1.0.4.tar", max compression
+gzip compressed data, was "async_adbc-1.0.5.tar", max compression
```

## Comparing `async_adbc-1.0.4.tar` & `async_adbc-1.0.5.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0       70 2023-05-16 06:58:01.167502 async_adbc-1.0.4/async_adbc/__init__.py
--rw-r--r--   0        0        0      998 2023-05-16 06:58:27.465793 async_adbc-1.0.4/async_adbc/adbclient.py
--rw-r--r--   0        0        0     2983 2023-05-16 06:52:10.041298 async_adbc-1.0.4/async_adbc/device.py
--rw-r--r--   0        0        0      601 2023-05-16 06:51:45.869292 async_adbc-1.0.4/async_adbc/plugins/__init__.py
--rw-r--r--   0        0        0      411 2023-05-18 08:06:58.438375 async_adbc-1.0.4/async_adbc/plugins/am.py
--rw-r--r--   0        0        0     2657 2023-05-16 02:32:10.948830 async_adbc-1.0.4/async_adbc/plugins/battery.py
--rw-r--r--   0        0        0    11683 2023-05-18 08:13:49.063412 async_adbc-1.0.4/async_adbc/plugins/cpu.py
--rw-r--r--   0        0        0     1242 2023-05-16 06:51:45.797292 async_adbc-1.0.4/async_adbc/plugins/forward.py
--rw-r--r--   0        0        0     3933 2023-05-16 02:51:02.455214 async_adbc-1.0.4/async_adbc/plugins/fps.py
--rw-r--r--   0        0        0      614 2023-05-15 12:07:09.349059 async_adbc-1.0.4/async_adbc/plugins/gpu.py
--rw-r--r--   0        0        0      393 2023-05-15 12:13:38.890420 async_adbc-1.0.4/async_adbc/plugins/input.py
--rw-r--r--   0        0        0      895 2023-05-16 03:18:01.857216 async_adbc-1.0.4/async_adbc/plugins/logcat.py
--rw-r--r--   0        0        0     2209 2023-05-16 03:26:42.422860 async_adbc-1.0.4/async_adbc/plugins/mem.py
--rw-r--r--   0        0        0     5597 2023-05-16 06:51:45.819291 async_adbc-1.0.4/async_adbc/plugins/pm.py
--rw-r--r--   0        0        0      510 2023-05-15 11:29:29.910308 async_adbc-1.0.4/async_adbc/plugins/prop.py
--rw-r--r--   0        0        0     4615 2023-05-16 04:20:29.957697 async_adbc-1.0.4/async_adbc/plugins/temp.py
--rw-r--r--   0        0        0     2216 2023-05-16 06:51:45.868298 async_adbc-1.0.4/async_adbc/plugins/traffic.py
--rw-r--r--   0        0        0      807 2023-05-15 11:29:32.496380 async_adbc-1.0.4/async_adbc/plugins/utils.py
--rw-r--r--   0        0        0     4481 2023-05-16 07:19:17.701385 async_adbc-1.0.4/async_adbc/protocol.py
--rw-r--r--   0        0        0      796 2023-05-16 06:51:45.874292 async_adbc-1.0.4/async_adbc/service/__init__.py
--rw-r--r--   0        0        0    10228 2023-05-16 06:51:45.939291 async_adbc-1.0.4/async_adbc/service/host.py
--rw-r--r--   0        0        0    10086 2023-05-16 06:51:45.937291 async_adbc-1.0.4/async_adbc/service/local.py
--rw-r--r--   0        0        0     1090 2023-05-16 05:23:42.403245 async_adbc-1.0.4/LICENSE
--rw-r--r--   0        0        0      482 2023-05-18 08:17:52.350303 async_adbc-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      423 2023-05-15 02:24:29.723099 async_adbc-1.0.4/README.md
--rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 async_adbc-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0       70 2023-05-19 14:22:34.448070 async_adbc-1.0.5/async_adbc/__init__.py
+-rw-r--r--   0        0        0      998 2023-05-19 14:22:34.448070 async_adbc-1.0.5/async_adbc/adbclient.py
+-rw-r--r--   0        0        0     3276 2023-05-19 14:22:34.449071 async_adbc-1.0.5/async_adbc/device.py
+-rw-r--r--   0        0        0      601 2023-05-19 14:22:34.449071 async_adbc-1.0.5/async_adbc/plugins/__init__.py
+-rw-r--r--   0        0        0      411 2023-05-19 14:22:34.449071 async_adbc-1.0.5/async_adbc/plugins/am.py
+-rw-r--r--   0        0        0     2657 2023-05-19 14:22:34.449071 async_adbc-1.0.5/async_adbc/plugins/battery.py
+-rw-r--r--   0        0        0    11606 2023-05-19 14:22:34.450070 async_adbc-1.0.5/async_adbc/plugins/cpu.py
+-rw-r--r--   0        0        0     1242 2023-05-19 14:22:34.450070 async_adbc-1.0.5/async_adbc/plugins/forward.py
+-rw-r--r--   0        0        0     3933 2023-05-19 14:22:34.450070 async_adbc-1.0.5/async_adbc/plugins/fps.py
+-rw-r--r--   0        0        0      614 2023-05-19 14:22:34.451071 async_adbc-1.0.5/async_adbc/plugins/gpu.py
+-rw-r--r--   0        0        0      393 2023-05-19 14:22:34.451071 async_adbc-1.0.5/async_adbc/plugins/input.py
+-rw-r--r--   0        0        0      895 2023-05-19 14:22:34.451071 async_adbc-1.0.5/async_adbc/plugins/logcat.py
+-rw-r--r--   0        0        0     2209 2023-05-19 14:22:34.451071 async_adbc-1.0.5/async_adbc/plugins/mem.py
+-rw-r--r--   0        0        0     5597 2023-05-19 14:22:34.451071 async_adbc-1.0.5/async_adbc/plugins/pm.py
+-rw-r--r--   0        0        0      510 2023-05-19 14:22:34.451071 async_adbc-1.0.5/async_adbc/plugins/prop.py
+-rw-r--r--   0        0        0     4615 2023-05-19 14:22:34.452071 async_adbc-1.0.5/async_adbc/plugins/temp.py
+-rw-r--r--   0        0        0     2216 2023-05-19 14:22:34.452071 async_adbc-1.0.5/async_adbc/plugins/traffic.py
+-rw-r--r--   0        0        0      807 2023-05-19 14:22:34.452071 async_adbc-1.0.5/async_adbc/plugins/utils.py
+-rw-r--r--   0        0        0     4481 2023-05-19 14:22:34.453071 async_adbc-1.0.5/async_adbc/protocol.py
+-rw-r--r--   0        0        0      796 2023-05-19 14:22:34.453071 async_adbc-1.0.5/async_adbc/service/__init__.py
+-rw-r--r--   0        0        0    10228 2023-05-19 14:22:34.453071 async_adbc-1.0.5/async_adbc/service/host.py
+-rw-r--r--   0        0        0    10086 2023-05-19 14:22:34.453071 async_adbc-1.0.5/async_adbc/service/local.py
+-rw-r--r--   0        0        0     1090 2023-05-19 14:22:34.448070 async_adbc-1.0.5/LICENSE
+-rw-r--r--   0        0        0      482 2023-05-19 14:22:34.454071 async_adbc-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      423 2023-05-19 14:22:34.448070 async_adbc-1.0.5/README.md
+-rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 async_adbc-1.0.5/setup.py
+-rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 async_adbc-1.0.5/PKG-INFO
```

### Comparing `async_adbc-1.0.4/async_adbc/adbclient.py` & `async_adbc-1.0.5/async_adbc/adbclient.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.4/async_adbc/device.py` & `async_adbc-1.0.5/async_adbc/device.py`

 * *Files 13% similar despite different names*

```diff
@@ -96,14 +96,21 @@
             m = re.match(result_pattern, line)
             if m:
                 properties[m.group(1)] = m.group(2)
 
         return properties
 
     async def get_pid_by_pkgname(self, package_name: str) -> int:
-        result = await self.shell(f"ps| grep -i {package_name}")
-
+        result = await self.shell(f"ps -ef| grep {package_name}")
         if result:
-            return int(result.split()[1])
+            lines = [
+                line.split()
+                for line in result.splitlines()
+                if not line.startswith("shell")
+            ]
+            process_list = [(seq[1], seq[7]) for seq in lines]
+            process_list.sort(key=lambda v: v[1], reverse=False)
+
+            return process_list[0][0]
 
         else:
             raise ValueError(f"{package_name} 应用没有运行")
```

### Comparing `async_adbc-1.0.4/async_adbc/plugins/__init__.py` & `async_adbc-1.0.5/async_adbc/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.4/async_adbc/plugins/battery.py` & `async_adbc-1.0.5/async_adbc/plugins/battery.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.4/async_adbc/plugins/cpu.py` & `async_adbc-1.0.5/async_adbc/plugins/cpu.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     def usage(self) -> float:
         """
         获取占用率，单位%
 
         Returns:
             float: 占用率
         """
-        return (self.user + self.system) / self.total * 100
+        return 100 * (self.user + self.system) / self.total
 
     def __add__(self, other: "CPUStat"):
         summary = CPUStat()
 
         summary.user = self.user + other.user
         summary.nice = self.nice + other.nice
         summary.system = self.system + other.system
@@ -311,19 +311,18 @@
 
         # 用sleep来间隔采样
         await asyncio.sleep(1)
 
         total_cpu_stat = await self.total_cpu_stat
         diff = total_cpu_stat - last_total_cpu_stat
 
-        usage = round(diff.usage, 2)
         normalize_factor = await self.normalize_factor
-        normalized = usage * normalize_factor
+        normalized = diff.usage * normalize_factor
 
-        return CPUUsage(usage, normalized)
+        return CPUUsage(diff.usage, normalized)
 
     async def get_pid_cpu_stat(self, pid: int) -> ProcessCPUStat:
         """以pid获取进程cpu状态
 
         Args:
             pid (int): 进程pid
 
@@ -333,30 +332,29 @@
         result = await self._device.shell(f"cat /proc/{pid}/stat")
 
         if "No such file or directory" in result:
             return ProcessCPUStat()
         else:
             items = result.split()
             return ProcessCPUStat(
-                items[1], int(items[13]), int(items[14], int(items[15], int(items[16])))
+                items[1], int(items[13]), int(items[14]), int(items[15]), int(items[16])
             )
 
     async def get_pid_cpu_usage(self, pid: int) -> CPUUsage:
         normalize_factor = await self.normalize_factor
 
         last_pid_cpu_stat = await self.get_pid_cpu_stat(pid)
         last_total_cpu_stat = await self.total_cpu_stat
         await asyncio.sleep(1)
         pid_stat = await self.get_pid_cpu_stat(pid)
         total_cpu_stat = await self.total_cpu_stat
         pid_diff = pid_stat - last_pid_cpu_stat
         cpu_diff = total_cpu_stat - last_total_cpu_stat
 
         app_cpu_usage = pid_diff.total / cpu_diff.total * 100
-        app_cpu_usage = round(app_cpu_usage, 2)
 
         normalized = app_cpu_usage * normalize_factor
         return CPUUsage(app_cpu_usage, normalized)
 
     @property
     async def cpu_name(self) -> str:
         """
```

### Comparing `async_adbc-1.0.4/async_adbc/plugins/forward.py` & `async_adbc-1.0.5/async_adbc/plugins/forward.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.4/async_adbc/plugins/fps.py` & `async_adbc-1.0.5/async_adbc/plugins/fps.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.4/async_adbc/plugins/gpu.py` & `async_adbc-1.0.5/async_adbc/plugins/gpu.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.4/async_adbc/plugins/logcat.py` & `async_adbc-1.0.5/async_adbc/plugins/logcat.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.4/async_adbc/plugins/mem.py` & `async_adbc-1.0.5/async_adbc/plugins/mem.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.4/async_adbc/plugins/pm.py` & `async_adbc-1.0.5/async_adbc/plugins/pm.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.4/async_adbc/plugins/temp.py` & `async_adbc-1.0.5/async_adbc/plugins/temp.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.4/async_adbc/plugins/traffic.py` & `async_adbc-1.0.5/async_adbc/plugins/traffic.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.4/async_adbc/plugins/utils.py` & `async_adbc-1.0.5/async_adbc/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.4/async_adbc/protocol.py` & `async_adbc-1.0.5/async_adbc/protocol.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.4/async_adbc/service/__init__.py` & `async_adbc-1.0.5/async_adbc/service/__init__.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.4/async_adbc/service/host.py` & `async_adbc-1.0.5/async_adbc/service/host.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.4/async_adbc/service/local.py` & `async_adbc-1.0.5/async_adbc/service/local.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.4/LICENSE` & `async_adbc-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.4/PKG-INFO` & `async_adbc-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-adbc
-Version: 1.0.4
+Version: 1.0.5
 Summary: 
 Author: kaluluosi
 Author-email: kaluluosi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

