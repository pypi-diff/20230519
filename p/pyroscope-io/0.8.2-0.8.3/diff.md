# Comparing `tmp/pyroscope-io-0.8.2.tar.gz` & `tmp/pyroscope-io-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroscope-io-0.8.2.tar", last modified: Thu Apr 27 07:29:02 2023, max compression
+gzip compressed data, was "pyroscope-io-0.8.3.tar", last modified: Fri May 19 14:24:16 2023, max compression
```

## Comparing `pyroscope-io-0.8.2.tar` & `pyroscope-io-0.8.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:29:02.107032 pyroscope-io-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-04-27 07:29:02.107032 pyroscope-io-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:29:02.103032 pyroscope-io-0.8.2/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:29:02.103032 pyroscope-io-0.8.2/lib/.cargo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/lib/.cargo/config
--rw-r--r--   0 runner    (1001) docker     (123)    63646 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/lib/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/lib/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/lib/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/lib/cbindgen.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:29:02.103032 pyroscope-io-0.8.2/lib/include/
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/lib/include/pyroscope_ffi.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:29:02.103032 pyroscope-io-0.8.2/lib/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/lib/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:29:02.103032 pyroscope-io-0.8.2/pyroscope/
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/pyroscope/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:29:02.103032 pyroscope-io-0.8.2/pyroscope_io/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/pyroscope_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:29:02.107032 pyroscope-io-0.8.2/pyroscope_io.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-04-27 07:29:02.000000 pyroscope-io-0.8.2/pyroscope_io.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-27 07:29:02.000000 pyroscope-io-0.8.2/pyroscope_io.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 07:29:02.000000 pyroscope-io-0.8.2/pyroscope_io.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 07:29:02.000000 pyroscope-io-0.8.2/pyroscope_io.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 07:29:02.000000 pyroscope-io-0.8.2/pyroscope_io.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 07:29:02.000000 pyroscope-io-0.8.2/pyroscope_io.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-27 07:29:02.107032 pyroscope-io-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-27 07:28:43.000000 pyroscope-io-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:24:16.728547 pyroscope-io-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-19 14:24:16.728547 pyroscope-io-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:24:16.728547 pyroscope-io-0.8.3/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:24:16.728547 pyroscope-io-0.8.3/lib/.cargo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/lib/.cargo/config
+-rw-r--r--   0 runner    (1001) docker     (123)    63646 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/lib/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/lib/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/lib/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/lib/cbindgen.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:24:16.728547 pyroscope-io-0.8.3/lib/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/lib/include/pyroscope_ffi.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:24:16.728547 pyroscope-io-0.8.3/lib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/lib/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:24:16.728547 pyroscope-io-0.8.3/pyroscope/
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/pyroscope/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:24:16.728547 pyroscope-io-0.8.3/pyroscope_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/pyroscope_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:24:16.728547 pyroscope-io-0.8.3/pyroscope_io.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-19 14:24:16.000000 pyroscope-io-0.8.3/pyroscope_io.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-19 14:24:16.000000 pyroscope-io-0.8.3/pyroscope_io.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 14:24:16.000000 pyroscope-io-0.8.3/pyroscope_io.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 14:24:16.000000 pyroscope-io-0.8.3/pyroscope_io.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 14:24:16.000000 pyroscope-io-0.8.3/pyroscope_io.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 14:24:16.000000 pyroscope-io-0.8.3/pyroscope_io.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-19 14:24:16.732547 pyroscope-io-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/setup.py
```

### Comparing `pyroscope-io-0.8.2/LICENSE` & `pyroscope-io-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroscope-io-0.8.2/PKG-INFO` & `pyroscope-io-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscope-io
-Version: 0.8.2
+Version: 0.8.3
 Summary: Pyroscope Python integration
 Home-page: https://pyroscope.io
 Maintainer: Abid Omar
 Maintainer-email: contact@pyroscope.io
 License: Apache 2.0
 Project-URL: Documentation, https://pyroscope.io
 Project-URL: Bug Tracker, https://pyroscope.io
```

### Comparing `pyroscope-io-0.8.2/README.md` & `pyroscope-io-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `pyroscope-io-0.8.2/lib/Cargo.lock` & `pyroscope-io-0.8.3/lib/Cargo.lock`

 * *Files identical despite different names*

### Comparing `pyroscope-io-0.8.2/lib/cbindgen.toml` & `pyroscope-io-0.8.3/lib/cbindgen.toml`

 * *Files identical despite different names*

### Comparing `pyroscope-io-0.8.2/lib/include/pyroscope_ffi.h` & `pyroscope-io-0.8.3/lib/include/pyroscope_ffi.h`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
                       bool oncpu,
                       bool native,
                       bool gil_only,
                       bool report_pid,
                       bool report_thread_id,
                       bool report_thread_name,
                       const char *tags,
-                      const char *scope_org_id,
+                      const char *tenant_id,
                       const char *http_headers_json);
 
 bool drop_agent(void);
 
 bool add_thread_tag(uint64_t thread_id, const char *key, const char *value);
 
 bool remove_thread_tag(uint64_t thread_id, const char *key, const char *value);
```

### Comparing `pyroscope-io-0.8.2/lib/src/lib.rs` & `pyroscope-io-0.8.3/lib/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     oncpu: bool,
     native: bool,
     gil_only: bool,
     report_pid: bool,
     report_thread_id: bool,
     report_thread_name: bool,
     tags: *const c_char,
-    scope_org_id: *const c_char,
+    tenant_id: *const c_char,
     http_headers_json: *const c_char,
 ) -> bool {
     // Initialize FFIKit
     let recv = ffikit::initialize_ffi().unwrap();
 
     // application_name
     let application_name = unsafe { CStr::from_ptr(application_name) }
@@ -89,15 +89,15 @@
 
     // tags
     let tags_string = unsafe { CStr::from_ptr(tags) }
         .to_str()
         .unwrap()
         .to_string();
 
-    let scope_org_id = unsafe { CStr::from_ptr(scope_org_id) }
+    let tenant_id = unsafe { CStr::from_ptr(tenant_id) }
         .to_str()
         .unwrap()
         .to_string();
 
     let http_headers_json = unsafe { CStr::from_ptr(http_headers_json) }
         .to_str()
         .unwrap()
@@ -143,16 +143,16 @@
 
     // Add the auth token if it is not empty.
     if auth_token != "" {
         agent_builder = agent_builder.auth_token(auth_token);
     } else if basic_auth_username != "" && basic_auth_password != "" {
         agent_builder = agent_builder.basic_auth(basic_auth_username, basic_auth_password);
     }
-    if scope_org_id != "" {
-        agent_builder = agent_builder.scope_org_id(scope_org_id);
+    if tenant_id != "" {
+        agent_builder = agent_builder.tenant_id(tenant_id);
     }
 
     let http_headers = pyroscope::pyroscope::parse_http_headers_json(http_headers_json);
     match http_headers {
         Ok(http_headers) => {
             agent_builder = agent_builder.http_headers(http_headers);
         }
```

### Comparing `pyroscope-io-0.8.2/pyroscope/__init__.py` & `pyroscope-io-0.8.3/pyroscope/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         oncpu=True,
         native=False,
         gil_only=True,
         report_pid=False,
         report_thread_id=False,
         report_thread_name=False,
         tags=None,
-        scope_org_id="",
+        tenant_id="",
         http_headers=None,
 ):
 
     if app_name is not None:
         warnings.warn("app_name is deprecated, use application_name", DeprecationWarning)
         application_name = app_name
 
@@ -48,15 +48,15 @@
         oncpu,
         native,
         gil_only,
         report_pid,
         report_thread_id,
         report_thread_name,
         tags_to_string(tags).encode("UTF-8"),
-        (scope_org_id or "").encode("UTF-8"),
+        (tenant_id or "").encode("UTF-8"),
         http_headers_to_json(http_headers).encode("UTF-8"),
 )
 
 def shutdown():
     drop = lib.drop_agent()
 
     if drop:
```

### Comparing `pyroscope-io-0.8.2/pyroscope_io.egg-info/PKG-INFO` & `pyroscope-io-0.8.3/pyroscope_io.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscope-io
-Version: 0.8.2
+Version: 0.8.3
 Summary: Pyroscope Python integration
 Home-page: https://pyroscope.io
 Maintainer: Abid Omar
 Maintainer-email: contact@pyroscope.io
 License: Apache 2.0
 Project-URL: Documentation, https://pyroscope.io
 Project-URL: Bug Tracker, https://pyroscope.io
```

### Comparing `pyroscope-io-0.8.2/setup.cfg` & `pyroscope-io-0.8.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyroscope-io
-version = 0.8.2
+version = 0.8.3
 description = Pyroscope Python integration
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://pyroscope.io
 maintainer = Abid Omar
 maintainer_email = contact@pyroscope.io
 license = Apache 2.0
```

### Comparing `pyroscope-io-0.8.2/setup.py` & `pyroscope-io-0.8.3/setup.py`

 * *Files identical despite different names*

