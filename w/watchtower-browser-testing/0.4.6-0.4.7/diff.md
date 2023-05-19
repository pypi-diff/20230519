# Comparing `tmp/watchtower_browser_testing-0.4.6.tar.gz` & `tmp/watchtower_browser_testing-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.4.6.tar", last modified: Fri May 12 10:58:46 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.4.7.tar", last modified: Fri May 19 18:02:54 2023, max compression
```

## Comparing `watchtower_browser_testing-0.4.6.tar` & `watchtower_browser_testing-0.4.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 10:58:46.138528 watchtower_browser_testing-0.4.6/
--rw-rw-rw-   0        0        0      310 2023-05-12 10:58:46.138528 watchtower_browser_testing-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.4.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-12 10:58:46.138528 watchtower_browser_testing-0.4.6/setup.cfg
--rw-rw-rw-   0        0        0     1135 2023-04-17 17:34:58.000000 watchtower_browser_testing-0.4.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-12 10:58:46.122903 watchtower_browser_testing-0.4.6/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      945 2023-04-18 07:07:32.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing/helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-12 10:58:46.138528 watchtower_browser_testing-0.4.6/watchtower_browser_testing/templates/
--rw-rw-rw-   0        0        0     6195 2023-04-25 13:45:16.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing/templates/measurement_plan.html
--rw-rw-rw-   0        0        0    17927 2023-05-02 09:55:35.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     7743 2023-04-17 17:27:01.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0       21 2023-05-12 10:58:03.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-05-12 10:58:46.138528 watchtower_browser_testing-0.4.6/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-05-12 10:58:45.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      609 2023-05-12 10:58:45.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 10:58:45.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-05-12 10:58:45.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-05-12 10:58:45.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 18:02:54.357083 watchtower_browser_testing-0.4.7/
+-rw-rw-rw-   0        0        0      310 2023-05-19 18:02:54.357083 watchtower_browser_testing-0.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.4.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-19 18:02:54.357083 watchtower_browser_testing-0.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     1135 2023-04-17 17:34:58.000000 watchtower_browser_testing-0.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 18:02:54.345828 watchtower_browser_testing-0.4.7/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.4.7/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      945 2023-04-18 07:07:32.000000 watchtower_browser_testing-0.4.7/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.4.7/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.4.7/watchtower_browser_testing/helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-19 18:02:54.356216 watchtower_browser_testing-0.4.7/watchtower_browser_testing/templates/
+-rw-rw-rw-   0        0        0     6195 2023-04-25 13:45:16.000000 watchtower_browser_testing-0.4.7/watchtower_browser_testing/templates/measurement_plan.html
+-rw-rw-rw-   0        0        0    17926 2023-05-19 12:18:04.000000 watchtower_browser_testing-0.4.7/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     7861 2023-05-19 18:02:13.000000 watchtower_browser_testing-0.4.7/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0       21 2023-05-19 18:02:13.000000 watchtower_browser_testing-0.4.7/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-05-19 18:02:54.354106 watchtower_browser_testing-0.4.7/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-05-19 18:02:54.000000 watchtower_browser_testing-0.4.7/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2023-05-19 18:02:54.000000 watchtower_browser_testing-0.4.7/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 18:02:54.000000 watchtower_browser_testing-0.4.7/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-05-19 18:02:54.000000 watchtower_browser_testing-0.4.7/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-05-19 18:02:54.000000 watchtower_browser_testing-0.4.7/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.4.6/setup.py` & `watchtower_browser_testing-0.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.6/watchtower_browser_testing/config.py` & `watchtower_browser_testing-0.4.7/watchtower_browser_testing/config.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.6/watchtower_browser_testing/helpers.py` & `watchtower_browser_testing-0.4.7/watchtower_browser_testing/helpers.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.6/watchtower_browser_testing/templates/measurement_plan.html` & `watchtower_browser_testing-0.4.7/watchtower_browser_testing/templates/measurement_plan.html`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.6/watchtower_browser_testing/testsuite.py` & `watchtower_browser_testing-0.4.7/watchtower_browser_testing/testsuite.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
                       tag_assistant_path=None,
                       headless=False):
 
         self.app = getattr(playwright, browser)
 
         if gtm_web_preview_link and re.match(config.GTM_WEB_PREVIEW_LINK_REGEX, gtm_web_preview_link):
             self.browser = None
-            tag_assistant_path is tag_assistant_path or config.DEFAULT_PATH_TO_TAG_ASSISTANT_EXTENSION
+            tag_assistant_path = tag_assistant_path or config.DEFAULT_PATH_TO_TAG_ASSISTANT_EXTENSION
             args = [
                 f'--disable-extensions-except={tag_assistant_path}',
                 f'--load-extension={tag_assistant_path}']
             if headless:
                 args.append('--headless=new')
             self.context = self.app.launch_persistent_context(
                 '',
```

### Comparing `watchtower_browser_testing-0.4.6/watchtower_browser_testing/tracking_validation.py` & `watchtower_browser_testing-0.4.7/watchtower_browser_testing/tracking_validation.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         elif not self.post_data_json is None and config.OLD_HARVEST_USER_ID_KEY in self.post_data_json:
             return self.post_data_json[config.OLD_HARVEST_USER_ID_KEY]
 
         return None
 
     @property
     def frame_url(self):
-        return self.request.frame.url
+        return self.request.wt_frame_url
 
     @property
     def method(self):
         return self.request.method
 
     @property
     def post_data_json(self):
@@ -258,14 +258,18 @@
                  url_patterns):
 
         self.url_patterns = url_patterns
         self.requests = []
 
     def register(self, request):
 
+        # record the frame url
+        frame_url = request.frame.url
+        request.wt_frame_url = frame_url
+
         if self.registration_filter(request):
             self.requests.append(request)
 
     def registration_filter(self, request):
 
         if not any(re.match(url_pattern, request.url) for url_pattern in self.url_patterns):
             return False
```

### Comparing `watchtower_browser_testing-0.4.6/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.4.7/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

