# Comparing `tmp/zappa-0.8.0.tar.gz` & `tmp/zappa-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zappa-0.8.0.tar", last modified: Sat Jan 30 19:41:05 2016, max compression
+gzip compressed data, was "dist/zappa-0.9.0.tar", last modified: Sun Jan 31 20:38:06 2016, max compression
```

## Comparing `zappa-0.8.0.tar` & `zappa-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 rjones   (3629613) 713727123        0 2016-01-30 19:41:05.000000 zappa-0.8.0/
--rw-r--r--   0 rjones   (3629613) 713727123     1077 2016-01-20 21:57:55.000000 zappa-0.8.0/LICENSE
--rw-r--r--   0 rjones   (3629613) 713727123       72 2016-01-26 13:31:42.000000 zappa-0.8.0/MANIFEST.in
--rw-r--r--   0 rjones   (3629613) 713727123     5089 2016-01-30 19:41:05.000000 zappa-0.8.0/PKG-INFO
--rw-r--r--   0 rjones   (3629613) 713727123     3208 2016-01-26 13:30:09.000000 zappa-0.8.0/README.md
--rw-r--r--   0 rjones   (3629613) 713727123      179 2016-01-26 00:12:58.000000 zappa-0.8.0/requirements.txt
--rw-r--r--   0 rjones   (3629613) 713727123       59 2016-01-30 19:41:05.000000 zappa-0.8.0/setup.cfg
--rw-r--r--   0 rjones   (3629613) 713727123     1292 2016-01-30 19:40:45.000000 zappa-0.8.0/setup.py
-drwxr-xr-x   0 rjones   (3629613) 713727123        0 2016-01-30 19:41:05.000000 zappa-0.8.0/zappa/
--rw-r--r--   0 rjones   (3629613) 713727123        0 2016-01-28 15:10:03.000000 zappa-0.8.0/zappa/__init__.py
--rw-r--r--   0 rjones   (3629613) 713727123     5946 2016-01-28 13:11:33.000000 zappa-0.8.0/zappa/sign_request.py
--rw-r--r--   0 rjones   (3629613) 713727123     2327 2016-01-25 19:59:16.000000 zappa-0.8.0/zappa/wsgi.py
--rwxr-xr-x   0 rjones   (3629613) 713727123    21983 2016-01-30 19:36:31.000000 zappa-0.8.0/zappa/zappa.py
-drwxr-xr-x   0 rjones   (3629613) 713727123        0 2016-01-30 19:41:05.000000 zappa-0.8.0/zappa.egg-info/
--rw-r--r--   0 rjones   (3629613) 713727123        1 2016-01-30 19:41:05.000000 zappa-0.8.0/zappa.egg-info/dependency_links.txt
--rw-r--r--   0 rjones   (3629613) 713727123       47 2016-01-30 19:41:05.000000 zappa-0.8.0/zappa.egg-info/pbr.json
--rw-r--r--   0 rjones   (3629613) 713727123     5089 2016-01-30 19:41:05.000000 zappa-0.8.0/zappa.egg-info/PKG-INFO
--rw-r--r--   0 rjones   (3629613) 713727123      179 2016-01-30 19:41:05.000000 zappa-0.8.0/zappa.egg-info/requires.txt
--rw-r--r--   0 rjones   (3629613) 713727123      292 2016-01-30 19:41:05.000000 zappa-0.8.0/zappa.egg-info/SOURCES.txt
--rw-r--r--   0 rjones   (3629613) 713727123        6 2016-01-30 19:41:05.000000 zappa-0.8.0/zappa.egg-info/top_level.txt
+drwxr-xr-x   0 rjones   (3629613) 713727123        0 2016-01-31 20:38:06.000000 zappa-0.9.0/
+-rw-r--r--   0 rjones   (3629613) 713727123     1077 2016-01-20 21:57:55.000000 zappa-0.9.0/LICENSE
+-rw-r--r--   0 rjones   (3629613) 713727123       72 2016-01-26 13:31:42.000000 zappa-0.9.0/MANIFEST.in
+-rw-r--r--   0 rjones   (3629613) 713727123     5089 2016-01-31 20:38:06.000000 zappa-0.9.0/PKG-INFO
+-rw-r--r--   0 rjones   (3629613) 713727123     3208 2016-01-26 13:30:09.000000 zappa-0.9.0/README.md
+-rw-r--r--   0 rjones   (3629613) 713727123      179 2016-01-26 00:12:58.000000 zappa-0.9.0/requirements.txt
+-rw-r--r--   0 rjones   (3629613) 713727123       59 2016-01-31 20:38:06.000000 zappa-0.9.0/setup.cfg
+-rw-r--r--   0 rjones   (3629613) 713727123     1292 2016-01-31 20:35:23.000000 zappa-0.9.0/setup.py
+drwxr-xr-x   0 rjones   (3629613) 713727123        0 2016-01-31 20:38:06.000000 zappa-0.9.0/zappa/
+-rw-r--r--   0 rjones   (3629613) 713727123        0 2016-01-28 15:10:03.000000 zappa-0.9.0/zappa/__init__.py
+-rw-r--r--   0 rjones   (3629613) 713727123     5946 2016-01-28 13:11:33.000000 zappa-0.9.0/zappa/sign_request.py
+-rw-r--r--   0 rjones   (3629613) 713727123     2860 2016-01-31 18:31:17.000000 zappa-0.9.0/zappa/wsgi.py
+-rwxr-xr-x   0 rjones   (3629613) 713727123    22848 2016-01-31 15:59:25.000000 zappa-0.9.0/zappa/zappa.py
+drwxr-xr-x   0 rjones   (3629613) 713727123        0 2016-01-31 20:38:06.000000 zappa-0.9.0/zappa.egg-info/
+-rw-r--r--   0 rjones   (3629613) 713727123        1 2016-01-31 20:38:05.000000 zappa-0.9.0/zappa.egg-info/dependency_links.txt
+-rw-r--r--   0 rjones   (3629613) 713727123       47 2016-01-31 20:38:05.000000 zappa-0.9.0/zappa.egg-info/pbr.json
+-rw-r--r--   0 rjones   (3629613) 713727123     5089 2016-01-31 20:38:05.000000 zappa-0.9.0/zappa.egg-info/PKG-INFO
+-rw-r--r--   0 rjones   (3629613) 713727123      179 2016-01-31 20:38:05.000000 zappa-0.9.0/zappa.egg-info/requires.txt
+-rw-r--r--   0 rjones   (3629613) 713727123      292 2016-01-31 20:38:06.000000 zappa-0.9.0/zappa.egg-info/SOURCES.txt
+-rw-r--r--   0 rjones   (3629613) 713727123        6 2016-01-31 20:38:05.000000 zappa-0.9.0/zappa.egg-info/top_level.txt
```

### Comparing `zappa-0.8.0/LICENSE` & `zappa-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zappa-0.8.0/PKG-INFO` & `zappa-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: zappa
-Version: 0.8.0
+Version: 0.9.0
 Summary: Serverless WSGI With AWS Lambda + API Gateway
 Home-page: https://github.com/Miserlou/Zappa
 Author: Rich Jones
 Author-email: rich@openwatch.net
 License: MIT License
 Description: |Logo placeholder| # Zappa |Build Status| #### Serverless WSGI with AWS
         Lambda + API Gateway
```

### Comparing `zappa-0.8.0/README.md` & `zappa-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `zappa-0.8.0/setup.py` & `zappa-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     README = open(os.path.join(os.path.dirname(__file__), 'README.md')).read()
 
 with open(os.path.join(os.path.dirname(__file__), 'requirements.txt')) as f:
     required = f.read().splitlines()
 
 setup(
     name='zappa',
-    version='0.8.0',
+    version='0.9.0',
     packages=['zappa'],
     install_requires=required,  
     include_package_data=True,
     license='MIT License',
     description='Serverless WSGI With AWS Lambda + API Gateway',
     long_description=README,
     url='https://github.com/Miserlou/Zappa',
```

### Comparing `zappa-0.8.0/zappa/sign_request.py` & `zappa-0.9.0/zappa/sign_request.py`

 * *Files identical despite different names*

### Comparing `zappa-0.8.0/zappa/wsgi.py` & `zappa-0.9.0/zappa/wsgi.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from urllib import urlencode
+from StringIO import StringIO
 
 # Event format:
 # event = {
 #     "body": {},
 #     "headers": {
 #         "Via": "1.1 e604e934e9195aaf3e36195adbcb3e18.cloudfront.net (CloudFront)",
 #         "Accept-Language": "en-US,en;q=0.5",
@@ -25,22 +26,22 @@
 #     },
 #     "method": "GET",
 #     "query": { 
 #         "dead": "beef" 
 #     }
 # }
 
-def create_wsgi_request(event_info, server_name='zappa'):
+def create_wsgi_request(event_info, server_name='zappa', script_name=None):
         """
         Given some event_info,
         create and return a valid WSGI request environ.
         """
 
         method = event_info['method']
-        body = event_info['body']
+        body = str(event_info['body'])
         params = event_info['params']
         query = event_info['query']
 
         path = "/"
         for key in sorted(params.keys()):
             path = path + params[key] + "/"
 
@@ -53,19 +54,31 @@
             'REQUEST_METHOD': method,
             'SCRIPT_NAME': str(''),
             'SERVER_NAME': str(server_name),
             'SERVER_PORT': str('80'),
             'SERVER_PROTOCOL': str('HTTP/1.1'),
             'wsgi.version': (1, 0),
             'wsgi.url_scheme': str('http'),
-            'wsgi.input': str(body),
+            'wsgi.input': body,
             'wsgi.errors': str(''),
             'wsgi.multiprocess': False,
             'wsgi.multithread': False,
             'wsgi.run_once': False,
         }
 
+        # Input processing
+        if method == "POST":
+            environ['wsgi.input'] = StringIO(body)
+            environ['CONTENT_TYPE'] = event_info["headers"]['Content-Type']
+            environ['CONTENT_LENGTH'] = str(len(body))
+
         for header in event_info["headers"]:
             wsgi_name = "HTTP_" + header.upper().replace('-', '_')
-            environ[wsgi_name] = event_info["headers"][header]
+            environ[wsgi_name] = str(event_info["headers"][header])
+
+        if script_name:
+            environ['SCRIPT_NAME'] = script_name
+            path_info = environ['PATH_INFO']
+            # if path_info.startswith(script_name):
+            #     environ['PATH_INFO'] = path_info[len(script_name):]
 
         return environ
```

### Comparing `zappa-0.8.0/zappa/zappa.py` & `zappa-0.9.0/zappa/zappa.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,14 +39,38 @@
     #foreach($queryParam in $input.params().querystring.keySet())
     "$queryParam": "$util.escapeJavaScript($input.params().querystring.get($queryParam))" #if($foreach.hasNext),#end
     
     #end
   }  
 }"""
 
+POST_TEMPLATE_MAPPING = """#set($rawPostData = $input.path('$'))
+{
+  "body" : "$rawPostData",
+  "headers": {
+    #foreach($header in $input.params().header.keySet())
+    "$header": "$util.escapeJavaScript($input.params().header.get($header))" #if($foreach.hasNext),#end
+    
+    #end
+  },
+  "method": "$context.httpMethod",
+  "params": {
+    #foreach($param in $input.params().path.keySet())
+    "$param": "$util.escapeJavaScript($input.params().path.get($param))" #if($foreach.hasNext),#end
+    
+    #end
+  },
+  "query": {
+    #foreach($queryParam in $input.params().querystring.keySet())
+    "$queryParam": "$util.escapeJavaScript($input.params().querystring.get($queryParam))" #if($foreach.hasNext),#end
+    
+    #end
+  }  
+}"""
+
 ASSUME_POLICY = """{
   "Version": "2012-10-17",
   "Statement": [
     {
       "Sid": "",
       "Effect": "Allow",
       "Principal": {
@@ -107,15 +131,15 @@
         'GET',
         'HEAD',
         'OPTIONS',
         'PATCH',
         'POST'
     ]
     parameter_depth = 5
-    integration_response_codes = [200, 301, 400, 404, 500]
+    integration_response_codes = [200, 301, 400, 401, 403, 404, 500]
     integration_content_types = [
         'text/html',
         # 'application/atom+xml',
         # 'application/json',
         # 'application/jwt',
         # 'application/xml',
     ]
@@ -470,15 +494,16 @@
                     httpMethod=method,
                     authorizationType='none',
                     apiKeyRequired=False
                 )
 
                 # Gotta do this one dirty.. thanks Boto..
                 template_mapping = TEMPLATE_MAPPING
-                content_mapping_templates = {'application/json': template_mapping}
+                post_template_mapping = POST_TEMPLATE_MAPPING
+                content_mapping_templates = {'application/json': template_mapping, 'application/x-www-form-urlencoded': post_template_mapping}
                 credentials = self.credentials_arn # This must be a Role ARN
                 uri='arn:aws:apigateway:' + self.aws_region + ':lambda:path/2015-03-31/functions/' + lambda_arn + '/invocations'
                 url = "/restapis/{0}/resources/{1}/methods/{2}/integration".format(
                     api_id,
                     resource_id,
                     method.upper()
                 )
```

### Comparing `zappa-0.8.0/zappa.egg-info/PKG-INFO` & `zappa-0.9.0/zappa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: zappa
-Version: 0.8.0
+Version: 0.9.0
 Summary: Serverless WSGI With AWS Lambda + API Gateway
 Home-page: https://github.com/Miserlou/Zappa
 Author: Rich Jones
 Author-email: rich@openwatch.net
 License: MIT License
 Description: |Logo placeholder| # Zappa |Build Status| #### Serverless WSGI with AWS
         Lambda + API Gateway
```

