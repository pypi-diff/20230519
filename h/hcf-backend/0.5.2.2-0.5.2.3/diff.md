# Comparing `tmp/hcf-backend-0.5.2.2.tar.gz` & `tmp/hcf-backend-0.5.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcf-backend-0.5.2.2.tar", last modified: Wed Apr 19 11:52:16 2023, max compression
+gzip compressed data, was "hcf-backend-0.5.2.3.tar", last modified: Fri May 19 20:32:05 2023, max compression
```

## Comparing `hcf-backend-0.5.2.2.tar` & `hcf-backend-0.5.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-19 11:52:16.839138 hcf-backend-0.5.2.2/
--rw-r--r--   0 molveyra  (1001) molveyra  (1001)     1478 2019-01-31 18:02:16.000000 hcf-backend-0.5.2.2/LICENSE
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2688 2023-04-19 11:52:16.839138 hcf-backend-0.5.2.2/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2067 2023-04-11 20:57:08.000000 hcf-backend-0.5.2.2/README.md
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-19 11:52:16.835138 hcf-backend-0.5.2.2/hcf_backend/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       48 2023-04-19 11:51:45.000000 hcf-backend-0.5.2.2/hcf_backend/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    14039 2023-04-13 16:11:52.000000 hcf-backend-0.5.2.2/hcf_backend/backend.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4529 2023-04-13 17:18:18.000000 hcf-backend-0.5.2.2/hcf_backend/manager.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-19 11:52:16.839138 hcf-backend-0.5.2.2/hcf_backend/utils/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1566 2023-04-11 21:18:45.000000 hcf-backend-0.5.2.2/hcf_backend/utils/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4003 2023-04-17 02:24:22.000000 hcf-backend-0.5.2.2/hcf_backend/utils/crawlmanager.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    13590 2023-04-19 11:51:04.000000 hcf-backend-0.5.2.2/hcf_backend/utils/hcfpal.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-19 11:52:16.839138 hcf-backend-0.5.2.2/hcf_backend.egg-info/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2688 2023-04-19 11:52:16.000000 hcf-backend-0.5.2.2/hcf_backend.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      377 2023-04-19 11:52:16.000000 hcf-backend-0.5.2.2/hcf_backend.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-04-19 11:52:16.000000 hcf-backend-0.5.2.2/hcf_backend.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      107 2023-04-19 11:52:16.000000 hcf-backend-0.5.2.2/hcf_backend.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       12 2023-04-19 11:52:16.000000 hcf-backend-0.5.2.2/hcf_backend.egg-info/top_level.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2021-07-13 00:16:34.000000 hcf-backend-0.5.2.2/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-04-19 11:52:16.839138 hcf-backend-0.5.2.2/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1014 2023-04-19 11:51:36.000000 hcf-backend-0.5.2.2/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-19 20:32:05.115052 hcf-backend-0.5.2.3/
+-rw-r--r--   0 molveyra  (1001) molveyra  (1001)     1478 2019-01-31 18:02:16.000000 hcf-backend-0.5.2.3/LICENSE
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2688 2023-05-19 20:32:05.115052 hcf-backend-0.5.2.3/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2067 2023-04-11 20:57:08.000000 hcf-backend-0.5.2.3/README.md
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-19 20:32:05.115052 hcf-backend-0.5.2.3/hcf_backend/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       48 2023-05-19 20:31:29.000000 hcf-backend-0.5.2.3/hcf_backend/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    14039 2023-04-13 16:11:52.000000 hcf-backend-0.5.2.3/hcf_backend/backend.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4595 2023-05-12 15:28:48.000000 hcf-backend-0.5.2.3/hcf_backend/manager.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-19 20:32:05.115052 hcf-backend-0.5.2.3/hcf_backend/utils/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1566 2023-04-11 21:18:45.000000 hcf-backend-0.5.2.3/hcf_backend/utils/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3994 2023-05-19 20:29:06.000000 hcf-backend-0.5.2.3/hcf_backend/utils/crawlmanager.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    13590 2023-04-19 11:51:04.000000 hcf-backend-0.5.2.3/hcf_backend/utils/hcfpal.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-19 20:32:05.115052 hcf-backend-0.5.2.3/hcf_backend.egg-info/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2688 2023-05-19 20:32:05.000000 hcf-backend-0.5.2.3/hcf_backend.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      377 2023-05-19 20:32:05.000000 hcf-backend-0.5.2.3/hcf_backend.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-05-19 20:32:05.000000 hcf-backend-0.5.2.3/hcf_backend.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      107 2023-05-19 20:32:05.000000 hcf-backend-0.5.2.3/hcf_backend.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       12 2023-05-19 20:32:05.000000 hcf-backend-0.5.2.3/hcf_backend.egg-info/top_level.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2021-07-13 00:16:34.000000 hcf-backend-0.5.2.3/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-05-19 20:32:05.115052 hcf-backend-0.5.2.3/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1014 2023-05-19 20:31:22.000000 hcf-backend-0.5.2.3/setup.py
```

### Comparing `hcf-backend-0.5.2.2/LICENSE` & `hcf-backend-0.5.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hcf-backend-0.5.2.2/PKG-INFO` & `hcf-backend-0.5.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcf-backend
-Version: 0.5.2.2
+Version: 0.5.2.3
 Summary: ScrapyCloud HubStorage frontier backend for Frontera
 Home-page: https://github.com/scrapinghub/hcf-backend
 Maintainer: Scrapinghub
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `hcf-backend-0.5.2.2/README.md` & `hcf-backend-0.5.2.3/README.md`

 * *Files identical despite different names*

### Comparing `hcf-backend-0.5.2.2/hcf_backend/backend.py` & `hcf-backend-0.5.2.3/hcf_backend/backend.py`

 * *Files identical despite different names*

### Comparing `hcf-backend-0.5.2.2/hcf_backend/manager.py` & `hcf-backend-0.5.2.3/hcf_backend/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,17 @@
         self._hcf = self._client.get_project(project_id).frontiers
         self._frontier = self._hcf.get(frontier)
         self._links_count: Dict[str, int] = defaultdict(int)
         self._links_to_flush_count: Dict[str, int] = defaultdict(int)
         self._batch_size = batch_size
         self._hcf_retries = 10
 
+    def new_links_count(self):
+        return self._hcf.newcount
+
     def add_request(self, slot: str, request):
         self._frontier.get(slot).q.add([request])
         self._links_count[slot] += 1
         self._links_to_flush_count[slot] += 1
         if self._batch_size and self._links_to_flush_count[slot] >= self._batch_size:
             return self.flush(slot)
         return 0
```

### Comparing `hcf-backend-0.5.2.2/hcf_backend/utils/__init__.py` & `hcf-backend-0.5.2.3/hcf_backend/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hcf-backend-0.5.2.2/hcf_backend/utils/crawlmanager.py` & `hcf-backend-0.5.2.3/hcf_backend/utils/crawlmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     def workflow_loop(self):
         available_slots = self.print_frontier_status()
 
         running_jobs = 0
         states = "running", "pending"
         for state in states:
-            for job in self.get_project().jobs.list(
+            for job in self.get_owned_jobs(
                 spider=self.args.spider, state=state, meta="spider_args"
             ):
                 frontera_settings_json = json.loads(
                     job["spider_args"].get("frontera_settings_json", "{}")
                 )
                 if "HCF_CONSUMER_SLOT" in frontera_settings_json:
                     slot = frontera_settings_json["HCF_CONSUMER_SLOT"]
```

### Comparing `hcf-backend-0.5.2.2/hcf_backend/utils/hcfpal.py` & `hcf-backend-0.5.2.3/hcf_backend/utils/hcfpal.py`

 * *Files identical despite different names*

### Comparing `hcf-backend-0.5.2.2/hcf_backend.egg-info/PKG-INFO` & `hcf-backend-0.5.2.3/hcf_backend.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcf-backend
-Version: 0.5.2.2
+Version: 0.5.2.3
 Summary: ScrapyCloud HubStorage frontier backend for Frontera
 Home-page: https://github.com/scrapinghub/hcf-backend
 Maintainer: Scrapinghub
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `hcf-backend-0.5.2.2/setup.py` & `hcf-backend-0.5.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name="hcf-backend",
-    version="0.5.2.2",
+    version="0.5.2.3",
     description="ScrapyCloud HubStorage frontier backend for Frontera",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="BSD",
     url="https://github.com/scrapinghub/hcf-backend",
     maintainer="Scrapinghub",
     packages=find_packages(),
```

