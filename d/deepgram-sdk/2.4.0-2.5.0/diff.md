# Comparing `tmp/deepgram-sdk-2.4.0.tar.gz` & `tmp/deepgram-sdk-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepgram-sdk-2.4.0.tar", last modified: Wed Apr 12 15:19:21 2023, max compression
+gzip compressed data, was "deepgram-sdk-2.5.0.tar", last modified: Thu May 18 22:22:10 2023, max compression
```

## Comparing `deepgram-sdk-2.4.0.tar` & `deepgram-sdk-2.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:19:21.524349 deepgram-sdk-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-04-12 15:19:21.520349 deepgram-sdk-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:19:21.520349 deepgram-sdk-2.4.0/deepgram/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/billing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/invitations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14159 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/transcription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/usage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:19:21.520349 deepgram-sdk-2.4.0/deepgram_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-04-12 15:19:21.000000 deepgram-sdk-2.4.0/deepgram_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-12 15:19:21.000000 deepgram-sdk-2.4.0/deepgram_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:19:21.000000 deepgram-sdk-2.4.0/deepgram_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 15:19:21.000000 deepgram-sdk-2.4.0/deepgram_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 15:19:21.000000 deepgram-sdk-2.4.0/deepgram_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 15:19:21.524349 deepgram-sdk-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:22:10.513366 deepgram-sdk-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-05-18 22:22:10.513366 deepgram-sdk-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:22:10.513366 deepgram-sdk-2.5.0/deepgram/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/invitations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14159 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/transcription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/usage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:22:10.513366 deepgram-sdk-2.5.0/deepgram_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-05-18 22:22:10.000000 deepgram-sdk-2.5.0/deepgram_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-18 22:22:10.000000 deepgram-sdk-2.5.0/deepgram_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 22:22:10.000000 deepgram-sdk-2.5.0/deepgram_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-18 22:22:10.000000 deepgram-sdk-2.5.0/deepgram_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 22:22:10.000000 deepgram-sdk-2.5.0/deepgram_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 22:22:10.513366 deepgram-sdk-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/setup.py
```

### Comparing `deepgram-sdk-2.4.0/LICENSE` & `deepgram-sdk-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.4.0/PKG-INFO` & `deepgram-sdk-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepgram-sdk
-Version: 2.4.0
+Version: 2.5.0
 Summary: The official Python SDK for the Deepgram automated speech recognition platform.
 Home-page: https://github.com/deepgram/deepgram-python-sdk
 Author: Luca Todd
 Author-email: luca.todd@deepgram.com
 License: MIT
 Keywords: deepgram speech-to-text
 Classifier: Intended Audience :: Developers
```

### Comparing `deepgram-sdk-2.4.0/README.md` & `deepgram-sdk-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.4.0/deepgram/__init__.py` & `deepgram-sdk-2.5.0/deepgram/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.4.0/deepgram/_types.py` & `deepgram-sdk-2.5.0/deepgram/_types.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.4.0/deepgram/_utils.py` & `deepgram-sdk-2.5.0/deepgram/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,16 +140,16 @@
                 content = resp.read().strip()
                 if not content:
                     return None
                 body = json.loads(content)
                 if body.get('error'):
                     raise Exception(f'DG: {content}')
                 return body
-        except urllib.error.URLError as exc:
-            raise (Exception(f'DG: {exc}') if exc.status < 500 else exc)
+        except urllib.error.HTTPError as exc:
+            raise (Exception(f'DG: {exc}') if exc.code < 500 else exc)
 
     tries = RETRY_COUNT
     while tries > 0:
         try:
             return attempt()
         except urllib.error.URLError as exc:
             if isinstance(payload, io.IOBase):
```

### Comparing `deepgram-sdk-2.4.0/deepgram/billing.py` & `deepgram-sdk-2.5.0/deepgram/billing.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.4.0/deepgram/invitations.py` & `deepgram-sdk-2.5.0/deepgram/invitations.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.4.0/deepgram/keys.py` & `deepgram-sdk-2.5.0/deepgram/keys.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.4.0/deepgram/members.py` & `deepgram-sdk-2.5.0/deepgram/members.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.4.0/deepgram/projects.py` & `deepgram-sdk-2.5.0/deepgram/projects.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.4.0/deepgram/scopes.py` & `deepgram-sdk-2.5.0/deepgram/scopes.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.4.0/deepgram/transcription.py` & `deepgram-sdk-2.5.0/deepgram/transcription.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.4.0/deepgram/usage.py` & `deepgram-sdk-2.5.0/deepgram/usage.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.4.0/deepgram_sdk.egg-info/PKG-INFO` & `deepgram-sdk-2.5.0/deepgram_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepgram-sdk
-Version: 2.4.0
+Version: 2.5.0
 Summary: The official Python SDK for the Deepgram automated speech recognition platform.
 Home-page: https://github.com/deepgram/deepgram-python-sdk
 Author: Luca Todd
 Author-email: luca.todd@deepgram.com
 License: MIT
 Keywords: deepgram speech-to-text
 Classifier: Intended Audience :: Developers
```

### Comparing `deepgram-sdk-2.4.0/setup.py` & `deepgram-sdk-2.5.0/setup.py`

 * *Files identical despite different names*

