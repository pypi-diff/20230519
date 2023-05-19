# Comparing `tmp/upstash_py-0.4.0.tar.gz` & `tmp/upstash_py-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_py-0.4.0.tar", max compression
+gzip compressed data, was "upstash_py-0.5.0.tar", max compression
```

## Comparing `upstash_py-0.4.0.tar` & `upstash_py-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,29 @@
--rw-r--r--   0        0        0       37 2023-03-04 10:43:41.243570 upstash_py-0.4.0/README.md
--rw-r--r--   0        0        0      379 2023-05-18 16:55:54.788352 upstash_py-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-04 11:23:56.540070 upstash_py-0.4.0/upstash_py/__init__.py
--rw-r--r--   0        0        0    87469 2023-05-16 16:11:10.452567 upstash_py-0.4.0/upstash_py/client.py
--rw-r--r--   0        0        0      308 2023-05-16 14:24:46.481207 upstash_py-0.4.0/upstash_py/config.py
--rw-r--r--   0        0        0       44 2023-03-08 07:44:02.265644 upstash_py-0.4.0/upstash_py/exception.py
--rw-r--r--   0        0        0      755 2023-05-04 15:53:00.952164 upstash_py-0.4.0/upstash_py/http/decode.py
--rw-r--r--   0        0        0     2445 2023-05-16 14:52:47.823004 upstash_py-0.4.0/upstash_py/http/execute.py
--rw-r--r--   0        0        0     1030 2023-05-04 15:39:39.039487 upstash_py-0.4.0/upstash_py/play.py
--rw-r--r--   0        0        0       65 2023-05-16 14:51:29.801586 upstash_py-0.4.0/upstash_py/play2.py
--rw-r--r--   0        0        0      409 2023-04-14 12:17:17.899972 upstash_py-0.4.0/upstash_py/schema/commands/parameters.py
--rw-r--r--   0        0        0     1119 2023-05-13 16:00:21.639249 upstash_py-0.4.0/upstash_py/schema/commands/returns.py
--rw-r--r--   0        0        0      761 2023-04-13 15:35:06.241703 upstash_py-0.4.0/upstash_py/schema/http.py
--rw-r--r--   0        0        0      188 2023-05-15 17:17:17.515782 upstash_py-0.4.0/upstash_py/schema/telemetry.py
--rw-r--r--   0        0        0      107 2023-04-13 16:18:51.335437 upstash_py-0.4.0/upstash_py/utils/base.py
--rw-r--r--   0        0        0      242 2023-04-14 14:58:16.064260 upstash_py-0.4.0/upstash_py/utils/comparison.py
--rw-r--r--   0        0        0     3333 2023-05-04 07:39:00.163434 upstash_py-0.4.0/upstash_py/utils/exception.py
--rw-r--r--   0        0        0     4088 2023-05-04 15:26:27.420397 upstash_py-0.4.0/upstash_py/utils/format.py
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 upstash_py-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       37 2023-03-04 10:43:41.243570 upstash_py-0.5.0/README.md
+-rw-r--r--   0        0        0      379 2023-05-19 12:00:59.470402 upstash_py-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-04 11:23:56.540070 upstash_py-0.5.0/upstash_py/__init__.py
+-rw-r--r--   0        0        0    87469 2023-05-16 16:11:10.452567 upstash_py-0.5.0/upstash_py/client.py
+-rw-r--r--   0        0        0      308 2023-05-16 14:24:46.481207 upstash_py-0.5.0/upstash_py/config.py
+-rw-r--r--   0        0        0       44 2023-03-08 07:44:02.265644 upstash_py-0.5.0/upstash_py/exception.py
+-rw-r--r--   0        0        0     1477 2023-05-04 15:53:50.306646 upstash_py-0.5.0/upstash_py/http/__pycache__/decode.cpython-311.pyc
+-rw-r--r--   0        0        0     3593 2023-05-19 11:57:45.592151 upstash_py-0.5.0/upstash_py/http/__pycache__/execute.cpython-311.pyc
+-rw-r--r--   0        0        0      755 2023-05-04 15:53:00.952164 upstash_py-0.5.0/upstash_py/http/decode.py
+-rw-r--r--   0        0        0     2596 2023-05-19 11:57:33.889831 upstash_py-0.5.0/upstash_py/http/execute.py
+-rw-r--r--   0        0        0     1030 2023-05-04 15:39:39.039487 upstash_py-0.5.0/upstash_py/play.py
+-rw-r--r--   0        0        0       61 2023-05-19 11:53:59.079435 upstash_py-0.5.0/upstash_py/play2.py
+-rw-r--r--   0        0        0      955 2023-04-13 15:52:55.302528 upstash_py-0.5.0/upstash_py/schema/__pycache__/http.cpython-311.pyc
+-rw-r--r--   0        0        0      594 2023-05-19 11:56:26.231398 upstash_py-0.5.0/upstash_py/schema/__pycache__/telemetry.cpython-311.pyc
+-rw-r--r--   0        0        0      787 2023-04-14 12:24:16.330346 upstash_py-0.5.0/upstash_py/schema/commands/__pycache__/parameters.cpython-311.pyc
+-rw-r--r--   0        0        0     1035 2023-05-13 16:12:40.737259 upstash_py-0.5.0/upstash_py/schema/commands/__pycache__/returns.cpython-311.pyc
+-rw-r--r--   0        0        0      409 2023-04-14 12:17:17.899972 upstash_py-0.5.0/upstash_py/schema/commands/parameters.py
+-rw-r--r--   0        0        0     1119 2023-05-13 16:00:21.639249 upstash_py-0.5.0/upstash_py/schema/commands/returns.py
+-rw-r--r--   0        0        0      761 2023-04-13 15:35:06.241703 upstash_py-0.5.0/upstash_py/schema/http.py
+-rw-r--r--   0        0        0      154 2023-05-19 11:45:14.791080 upstash_py-0.5.0/upstash_py/schema/telemetry.py
+-rw-r--r--   0        0        0      498 2023-04-13 16:21:42.465103 upstash_py-0.5.0/upstash_py/utils/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0      806 2023-04-14 15:10:31.968199 upstash_py-0.5.0/upstash_py/utils/__pycache__/comparison.cpython-311.pyc
+-rw-r--r--   0        0        0     4592 2023-05-04 09:53:23.644989 upstash_py-0.5.0/upstash_py/utils/__pycache__/exception.cpython-311.pyc
+-rw-r--r--   0        0        0     6553 2023-05-04 15:29:10.957427 upstash_py-0.5.0/upstash_py/utils/__pycache__/format.cpython-311.pyc
+-rw-r--r--   0        0        0      107 2023-04-13 16:18:51.335437 upstash_py-0.5.0/upstash_py/utils/base.py
+-rw-r--r--   0        0        0      242 2023-04-14 14:58:16.064260 upstash_py-0.5.0/upstash_py/utils/comparison.py
+-rw-r--r--   0        0        0     3333 2023-05-04 07:39:00.163434 upstash_py-0.5.0/upstash_py/utils/exception.py
+-rw-r--r--   0        0        0     4088 2023-05-04 15:26:27.420397 upstash_py-0.5.0/upstash_py/utils/format.py
+-rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 upstash_py-0.5.0/PKG-INFO
```

### Comparing `upstash_py-0.4.0/upstash_py/client.py` & `upstash_py-0.5.0/upstash_py/client.py`

 * *Files identical despite different names*

### Comparing `upstash_py-0.4.0/upstash_py/http/decode.py` & `upstash_py-0.5.0/upstash_py/http/decode.py`

 * *Files identical despite different names*

### Comparing `upstash_py-0.4.0/upstash_py/http/execute.py` & `upstash_py-0.5.0/upstash_py/http/execute.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,23 +34,27 @@
 
     for i in range(retries + 1):
         try:
             headers: dict[str, str] = {"Authorization": f'Bearer {token}'}
 
             if allow_telemetry:
                 if telemetry_data:
-                    headers["Upstash-Telemetry-Runtime"] = telemetry_data["runtime"]
-                    headers["Upstash-Telemetry-Sdk"] = telemetry_data["sdk"]
-
                     # Avoid the [] syntax to prevent KeyError from being raised.
+                    if telemetry_data.get("runtime"):
+                        headers["Upstash-Telemetry-Runtime"] = telemetry_data["runtime"]
+                    else:
+                        headers["Upstash-Telemetry-Runtime"] = f'python@v{python_version()}'
+
+                    if telemetry_data.get("sdk"):
+                        headers["Upstash-Telemetry-Sdk"] = telemetry_data["sdk"]
+                    else:
+                        headers["Upstash-Telemetry-Sdk"] = "upstash-py@development"
+
                     if telemetry_data.get("platform"):
                         headers["Upstash-Telemetry-Platform"] = telemetry_data["platform"]
-                else:
-                    headers["Upstash-Telemetry-Runtime"] = f'python@v{python_version()}'
-                    headers["Upstash-Telemetry-Sdk"] = "upstash-py@development"
 
             if encoding:
                 headers["Upstash-Encoding"] = encoding
 
             async with session.post(url, headers=headers, json=command) as response:
                 body: RESTResponse[RESTResult] = await response.json()
```

### Comparing `upstash_py-0.4.0/upstash_py/play.py` & `upstash_py-0.5.0/upstash_py/play.py`

 * *Files identical despite different names*

### Comparing `upstash_py-0.4.0/upstash_py/schema/commands/returns.py` & `upstash_py-0.5.0/upstash_py/schema/commands/returns.py`

 * *Files identical despite different names*

### Comparing `upstash_py-0.4.0/upstash_py/schema/http.py` & `upstash_py-0.5.0/upstash_py/schema/http.py`

 * *Files identical despite different names*

### Comparing `upstash_py-0.4.0/upstash_py/utils/exception.py` & `upstash_py-0.5.0/upstash_py/utils/exception.py`

 * *Files identical despite different names*

### Comparing `upstash_py-0.4.0/upstash_py/utils/format.py` & `upstash_py-0.5.0/upstash_py/utils/format.py`

 * *Files identical despite different names*

