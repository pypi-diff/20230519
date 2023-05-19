# Comparing `tmp/edge_logger-0.0.8.tar.gz` & `tmp/edge_logger-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge_logger-0.0.8.tar", max compression
+gzip compressed data, was "edge_logger-0.0.9.tar", max compression
```

## Comparing `edge_logger-0.0.8.tar` & `edge_logger-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-04-16 19:59:55.248252 edge_logger-0.0.8/LICENSE
--rw-r--r--   0        0        0        0 2023-04-17 03:01:06.502367 edge_logger-0.0.8/README.md
--rw-r--r--   0        0        0        0 2023-04-16 20:07:03.564649 edge_logger-0.0.8/edge_logger/__init__.py
--rw-r--r--   0        0        0     6012 2023-05-04 02:30:39.656027 edge_logger-0.0.8/edge_logger/edge_logger.py
--rw-r--r--   0        0        0      380 2023-05-04 02:30:39.651033 edge_logger-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 edge_logger-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-16 19:59:55.248252 edge_logger-0.0.9/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-17 03:01:06.502367 edge_logger-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-04-16 20:07:03.564649 edge_logger-0.0.9/edge_logger/__init__.py
+-rw-r--r--   0        0        0     6025 2023-05-04 02:39:41.285474 edge_logger-0.0.9/edge_logger/edge_logger.py
+-rw-r--r--   0        0        0      380 2023-05-04 02:38:38.852490 edge_logger-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 edge_logger-0.0.9/PKG-INFO
```

### Comparing `edge_logger-0.0.8/LICENSE` & `edge_logger-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edge_logger-0.0.8/edge_logger/edge_logger.py` & `edge_logger-0.0.9/edge_logger/edge_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.session = session = requests.Session()
         session.headers.update({
             'Content-Type': 'application/json'
         })
 
         self.session.mount('https://', HTTPAdapter(
             max_retries=Retry(
-                total=5,
+                total=2,
                 backoff_factor=0.5,
                 status_forcelist=[403, 500]
             ),
             pool_connections=self.MAX_POOLSIZE,
             pool_maxsize=self.MAX_POOLSIZE
         ))
 
@@ -48,18 +48,17 @@
         This function gets called when a log event gets emitted. It receives a
         record, formats it and sends it to the url
         Parameters:
             record: a log record
         """
         json_log = self.format(record)
         with concurrent.futures.ProcessPoolExecutor() as executor:
-            future = executor.submit(emit_entry_process_out, json_log, self.url)
-            ret = future.result()
-            print(ret)
-        # self.emit_process_entry(record)
+            # future = executor.submit(emit_entry_process_out, json_log, self.url)
+            _ = executor.submit(emit_entry_process_out, json_log, self.url)
+            # _ = future.result()
 
 
 def emit_entry_process_out(json_log, url):
     # Send the POST request with the JSON data and headers
     headers = {'Content-Type': 'application/json'}
     response = requests.post(url, data=json_log, headers=headers)
     return response
```

