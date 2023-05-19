# Comparing `tmp/tomcru_jerry-0.1.2.tar.gz` & `tmp/tomcru_jerry-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomcru_jerry-0.1.2.tar", max compression
+gzip compressed data, was "tomcru_jerry-0.1.3.tar", max compression
```

## Comparing `tomcru_jerry-0.1.2.tar` & `tomcru_jerry-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-04-09 00:51:18.750203 tomcru_jerry-0.1.2/LICENSE
--rw-r--r--   0        0        0      124 2023-04-09 00:51:18.750203 tomcru_jerry-0.1.2/README.md
--rw-r--r--   0        0        0      391 2023-05-09 23:35:50.014590 tomcru_jerry-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1978 2023-04-17 23:54:18.705910 tomcru_jerry-0.1.2/tomcru_jerry/__init__.py
--rw-r--r--   0        0        0     3084 2023-04-25 23:25:52.640719 tomcru_jerry-0.1.2/tomcru_jerry/cli.py
--rw-r--r--   0        0        0     3859 2023-04-23 14:49:50.811637 tomcru_jerry-0.1.2/tomcru_jerry/controllers.py
--rw-r--r--   0        0        0     2422 2023-04-17 23:28:38.922059 tomcru_jerry-0.1.2/tomcru_jerry/flask_jerry.py
--rw-r--r--   0        0        0     3874 2023-04-29 02:48:29.775134 tomcru_jerry-0.1.2/tomcru_jerry/mockapi.py
--rw-r--r--   0        0        0     5556 2023-04-29 16:36:50.609598 tomcru_jerry-0.1.2/tomcru_jerry/static.py
--rw-r--r--   0        0        0     2268 2023-04-24 16:07:40.404928 tomcru_jerry-0.1.2/tomcru_jerry/utils.py
--rw-r--r--   0        0        0      576 1970-01-01 00:00:00.000000 tomcru_jerry-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-09 00:51:18.750203 tomcru_jerry-0.1.3/LICENSE
+-rw-r--r--   0        0        0      124 2023-04-09 00:51:18.750203 tomcru_jerry-0.1.3/README.md
+-rw-r--r--   0        0        0      391 2023-05-19 12:55:09.042827 tomcru_jerry-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1978 2023-04-17 23:54:18.705910 tomcru_jerry-0.1.3/tomcru_jerry/__init__.py
+-rw-r--r--   0        0        0     3084 2023-04-25 23:25:52.640719 tomcru_jerry-0.1.3/tomcru_jerry/cli.py
+-rw-r--r--   0        0        0     3859 2023-04-23 14:49:50.811637 tomcru_jerry-0.1.3/tomcru_jerry/controllers.py
+-rw-r--r--   0        0        0     2502 2023-05-19 12:53:47.282236 tomcru_jerry-0.1.3/tomcru_jerry/flask_jerry.py
+-rw-r--r--   0        0        0     3874 2023-04-29 02:48:29.775134 tomcru_jerry-0.1.3/tomcru_jerry/mockapi.py
+-rw-r--r--   0        0        0     5638 2023-05-14 19:42:11.345044 tomcru_jerry-0.1.3/tomcru_jerry/static.py
+-rw-r--r--   0        0        0     2268 2023-04-24 16:07:40.404928 tomcru_jerry-0.1.3/tomcru_jerry/utils.py
+-rw-r--r--   0        0        0      576 1970-01-01 00:00:00.000000 tomcru_jerry-0.1.3/PKG-INFO
```

### Comparing `tomcru_jerry-0.1.2/LICENSE` & `tomcru_jerry-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tomcru_jerry-0.1.2/tomcru_jerry/__init__.py` & `tomcru_jerry-0.1.3/tomcru_jerry/__init__.py`

 * *Files identical despite different names*

### Comparing `tomcru_jerry-0.1.2/tomcru_jerry/cli.py` & `tomcru_jerry-0.1.3/tomcru_jerry/cli.py`

 * *Files identical despite different names*

### Comparing `tomcru_jerry-0.1.2/tomcru_jerry/controllers.py` & `tomcru_jerry-0.1.3/tomcru_jerry/controllers.py`

 * *Files identical despite different names*

### Comparing `tomcru_jerry-0.1.2/tomcru_jerry/flask_jerry.py` & `tomcru_jerry-0.1.3/tomcru_jerry/flask_jerry.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,29 +16,32 @@
 
     def __init__(self, app: Flask, config: dict, path: str):
         self.custom_routes = defaultdict(set)
         self.module_route = app.module_route if hasattr(app, 'module_route') else ""
         self.mockedapi = None
 
         webconf = config.get('website', {})
-        web_type = webconf.get('type', None)
+        tags = webconf.get('tags', set())
 
         app.host = webconf.get('host', '0.0.0.0')
         app.port = webconf.get('port', '5000')
         app.debug = self.debug = webconf.get('debug', False)
         app.threaded = webconf.get('threaded', True)
 
-        self.http_verbs = webconf.get('methods', ["GET","HEAD","OPTIONS","POST","PUT","PATCH","DELETE"])
-        headers = config.get('headers', {
-            "Access-Control-Allow-Methods":  ",".join(self.http_verbs),
-            "Access-Control-Allow-Origin": "*",
-            "Access-Control-Allow-Headers": "Origin, Accept, X-Requested-With, Content-Type, Authorization"
-        })
+        headers = config.get('headers', {})
+        if 'cors' in tags:
+            self.http_verbs = webconf.get('methods', ["GET","HEAD","OPTIONS","POST","PUT","PATCH","DELETE"])
+
+            headers.update({
+                "Access-Control-Allow-Methods":  ",".join(self.http_verbs),
+                "Access-Control-Allow-Origin": "*",
+                "Access-Control-Allow-Headers": "Origin, Accept, X-Requested-With, Content-Type, Authorization"
+            })
 
-        if web_type in ('webapi', 'api'):
+        if 'webapi' in tags or 'api' in tags:
             if 'Content-Type' not in headers:
                 headers['Content-Type'] = 'application/json'
                 headers['Referrer-Policy'] = 'no-referrer-when-downgrade'
 
         if path:
             app.template_folder = os.path.join(path, webconf.get('template_folder', 'templates'))
             app.static_folder = os.path.join(path, webconf.get('static_folder', 'public'))
```

### Comparing `tomcru_jerry-0.1.2/tomcru_jerry/mockapi.py` & `tomcru_jerry-0.1.3/tomcru_jerry/mockapi.py`

 * *Files identical despite different names*

### Comparing `tomcru_jerry-0.1.2/tomcru_jerry/static.py` & `tomcru_jerry-0.1.3/tomcru_jerry/static.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import jinja2
 import pynliner
 import htmlmin
 from bs4 import BeautifulSoup
 from flask import Flask, render_template, request, send_from_directory
 from werkzeug.routing import BaseConverter
 
+
 class RegexConverter(BaseConverter):
     def __init__(self, url_map, *items):
         super(RegexConverter, self).__init__(url_map)
         self.regex = items[0]
 
 
 class StaticWebsite:
@@ -98,14 +99,16 @@
         i = 0
 
         for _link_css in soup.find_all("link"):
             el = _link_css.extract()
 
             # read in CSS content
             css_file = el['href']
+            if css_file.startswith('/'):
+                css_file = css_file[1:]
             with open(os.path.join(self.static_folder, css_file)) as fh:
                 css = fh.read()
 
             # fate of external CSS is either becoming internal or inline:
             if 'as-internal' in el.attrs:
                 # internal: re-added later
                 self.kept_styles[el.get('as-internal', i)].append(css)
```

### Comparing `tomcru_jerry-0.1.2/tomcru_jerry/utils.py` & `tomcru_jerry-0.1.3/tomcru_jerry/utils.py`

 * *Files identical despite different names*

### Comparing `tomcru_jerry-0.1.2/PKG-INFO` & `tomcru_jerry-0.1.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomcru-jerry
-Version: 0.1.2
+Version: 0.1.3
 Summary: General purpose web library
 Author: Rajmund Csombordi
 Author-email: rajmund.csombordi@hotmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

