# Comparing `tmp/psychicapi-0.2.tar.gz` & `tmp/psychicapi-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychicapi-0.2.tar", last modified: Wed May 17 19:15:46 2023, max compression
+gzip compressed data, was "dist/psychicapi-0.3.tar", last modified: Fri May 19 03:36:36 2023, max compression
```

## Comparing `psychicapi-0.2.tar` & `psychicapi-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-05-17 19:15:46.580597 psychicapi-0.2/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      197 2023-05-17 19:15:46.579904 psychicapi-0.2/PKG-INFO
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      154 2023-05-17 05:32:44.000000 psychicapi-0.2/README.md
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-05-17 19:15:46.574425 psychicapi-0.2/psychicapi/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       41 2023-05-17 19:08:44.000000 psychicapi-0.2/psychicapi/__init__.py
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      924 2023-05-17 05:55:51.000000 psychicapi-0.2/psychicapi/psychic.py
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-05-17 19:15:46.579044 psychicapi-0.2/psychicapi.egg-info/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      197 2023-05-17 19:15:46.000000 psychicapi-0.2/psychicapi.egg-info/PKG-INFO
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      232 2023-05-17 19:15:46.000000 psychicapi-0.2/psychicapi.egg-info/SOURCES.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        1 2023-05-17 19:15:46.000000 psychicapi-0.2/psychicapi.egg-info/dependency_links.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        9 2023-05-17 19:15:46.000000 psychicapi-0.2/psychicapi.egg-info/requires.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       11 2023-05-17 19:15:46.000000 psychicapi-0.2/psychicapi.egg-info/top_level.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       38 2023-05-17 19:15:46.581750 psychicapi-0.2/setup.cfg
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      327 2023-05-17 19:15:41.000000 psychicapi-0.2/setup.py
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-05-19 03:36:36.000000 psychicapi-0.3/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      272 2023-05-19 03:36:36.000000 psychicapi-0.3/PKG-INFO
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-05-19 03:36:36.000000 psychicapi-0.3/psychicapi/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       41 2023-05-18 20:09:12.000000 psychicapi-0.3/psychicapi/__init__.py
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     1753 2023-05-18 23:32:28.000000 psychicapi-0.3/psychicapi/psychic.py
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      154 2023-05-17 05:32:44.000000 psychicapi-0.3/README.md
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      327 2023-05-19 03:36:27.000000 psychicapi-0.3/setup.py
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-05-19 03:36:36.000000 psychicapi-0.3/psychicapi.egg-info/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      272 2023-05-19 03:36:36.000000 psychicapi-0.3/psychicapi.egg-info/PKG-INFO
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      232 2023-05-19 03:36:36.000000 psychicapi-0.3/psychicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        9 2023-05-19 03:36:36.000000 psychicapi-0.3/psychicapi.egg-info/requires.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       11 2023-05-19 03:36:36.000000 psychicapi-0.3/psychicapi.egg-info/top_level.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        1 2023-05-19 03:36:36.000000 psychicapi-0.3/psychicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       38 2023-05-19 03:36:36.000000 psychicapi-0.3/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `psychicapi-0.2/psychicapi/psychic.py` & `psychicapi-0.3/psychicapi/psychic.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import requests
 from enum import Enum
+from typing import List, Optional, Dict
 
 class ConnectorId(Enum):
     notion = "notion"
     confluence = "confluence"
     zendesk = "zendesk"
     gdrive = "gdrive"
 
@@ -24,8 +25,32 @@
                 'Accept': 'application/json'
             }
         )
         if response.status_code == 200:
             documents = response.json()["documents"]
             return documents
         else:
+            return None
+        
+    def get_connections(self, connector_id: Optional[ConnectorId] = None, connection_id: Optional[str] = None):
+        filter = {}
+
+        if connector_id is not None:
+            filter["connector_id"] = connector_id.value
+        if connection_id is not None:
+            filter["connection_id"] = connection_id
+
+        response = requests.post(
+            self.api_url + "get-connections",
+            json={
+                "filter": filter,
+            },
+            headers={
+                'Authorization': 'Bearer ' + self.secret_key,
+                'Accept': 'application/json'
+            }
+        )
+        if response.status_code == 200:
+            documents = response.json()["connections"]
+            return documents
+        else:
             return None
```

