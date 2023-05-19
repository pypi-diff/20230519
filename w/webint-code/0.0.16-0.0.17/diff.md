# Comparing `tmp/webint_code-0.0.16.tar.gz` & `tmp/webint_code-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webint_code-0.0.16.tar", max compression
+gzip compressed data, was "webint_code-0.0.17.tar", max compression
```

## Comparing `webint_code-0.0.16.tar` & `webint_code-0.0.17.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1131 2023-05-19 00:23:08.588808 webint_code-0.0.16/pyproject.toml
--rw-r--r--   0        0        0    19028 2023-05-19 00:23:07.296788 webint_code-0.0.16/webint_code/__init__.py
--rw-r--r--   0        0        0      474 2023-01-27 00:43:27.567919 webint_code-0.0.16/webint_code/templates/__init__.py
--rw-r--r--   0        0        0      161 2023-02-20 19:30:47.711101 webint_code-0.0.16/webint_code/templates/index.html
--rw-r--r--   0        0        0     1225 2023-01-27 00:43:27.575919 webint_code-0.0.16/webint_code/templates/project/commit.html
--rw-r--r--   0        0        0      651 2023-01-27 00:43:27.567919 webint_code-0.0.16/webint_code/templates/project/commit_log.html
--rw-r--r--   0        0        0      116 2023-01-27 00:43:27.571919 webint_code-0.0.16/webint_code/templates/project/created.html
--rw-r--r--   0        0        0    10118 2023-01-27 00:43:27.571919 webint_code-0.0.16/webint_code/templates/project/index.html
--rw-r--r--   0        0        0      872 2023-01-27 00:43:27.575919 webint_code-0.0.16/webint_code/templates/project/issues.html
--rw-r--r--   0        0        0     2921 2023-01-27 00:43:27.571919 webint_code-0.0.16/webint_code/templates/project/namespace.html
--rw-r--r--   0        0        0      294 2023-01-27 00:43:27.571919 webint_code-0.0.16/webint_code/templates/project/release.html
--rw-r--r--   0        0        0      777 2023-01-27 00:43:27.575919 webint_code-0.0.16/webint_code/templates/project/release_file.html
--rw-r--r--   0        0        0     1063 2023-01-27 00:43:27.571919 webint_code-0.0.16/webint_code/templates/project/repository_file.html
--rw-r--r--   0        0        0      485 2023-01-27 00:43:27.575919 webint_code-0.0.16/webint_code/templates/project/settings.html
--rw-r--r--   0        0        0      373 2023-01-27 00:43:27.579919 webint_code-0.0.16/webint_code/templates/projects.html
--rw-r--r--   0        0        0      136 2023-01-27 00:43:27.579919 webint_code-0.0.16/webint_code/templates/pypi/index.html
--rw-r--r--   0        0        0      227 2023-01-27 00:43:27.579919 webint_code-0.0.16/webint_code/templates/pypi/project.html
--rw-r--r--   0        0        0       87 2023-01-27 00:43:27.579919 webint_code-0.0.16/webint_code/templates/search/index.html
--rw-r--r--   0        0        0     1029 2023-01-27 00:43:27.583919 webint_code-0.0.16/webint_code/templates/search/results.html
--rw-r--r--   0        0        0     4967 2023-05-18 23:21:54.011448 webint_code-0.0.16/webint_code/templates/system.html
--rw-r--r--   0        0        0      149 2023-01-27 00:43:27.567919 webint_code-0.0.16/webint_code/templates/template.html
--rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 webint_code-0.0.16/setup.py
--rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 webint_code-0.0.16/PKG-INFO
+-rw-r--r--   0        0        0     1131 2023-05-19 00:32:17.316836 webint_code-0.0.17/pyproject.toml
+-rw-r--r--   0        0        0    18934 2023-05-19 00:31:33.184194 webint_code-0.0.17/webint_code/__init__.py
+-rw-r--r--   0        0        0      474 2023-01-27 00:43:27.567919 webint_code-0.0.17/webint_code/templates/__init__.py
+-rw-r--r--   0        0        0      161 2023-02-20 19:30:47.711101 webint_code-0.0.17/webint_code/templates/index.html
+-rw-r--r--   0        0        0     1225 2023-01-27 00:43:27.575919 webint_code-0.0.17/webint_code/templates/project/commit.html
+-rw-r--r--   0        0        0      651 2023-01-27 00:43:27.567919 webint_code-0.0.17/webint_code/templates/project/commit_log.html
+-rw-r--r--   0        0        0      116 2023-01-27 00:43:27.571919 webint_code-0.0.17/webint_code/templates/project/created.html
+-rw-r--r--   0        0        0    10118 2023-01-27 00:43:27.571919 webint_code-0.0.17/webint_code/templates/project/index.html
+-rw-r--r--   0        0        0      872 2023-01-27 00:43:27.575919 webint_code-0.0.17/webint_code/templates/project/issues.html
+-rw-r--r--   0        0        0     2921 2023-01-27 00:43:27.571919 webint_code-0.0.17/webint_code/templates/project/namespace.html
+-rw-r--r--   0        0        0      294 2023-01-27 00:43:27.571919 webint_code-0.0.17/webint_code/templates/project/release.html
+-rw-r--r--   0        0        0      777 2023-01-27 00:43:27.575919 webint_code-0.0.17/webint_code/templates/project/release_file.html
+-rw-r--r--   0        0        0     1063 2023-01-27 00:43:27.571919 webint_code-0.0.17/webint_code/templates/project/repository_file.html
+-rw-r--r--   0        0        0      485 2023-01-27 00:43:27.575919 webint_code-0.0.17/webint_code/templates/project/settings.html
+-rw-r--r--   0        0        0      373 2023-01-27 00:43:27.579919 webint_code-0.0.17/webint_code/templates/projects.html
+-rw-r--r--   0        0        0      136 2023-01-27 00:43:27.579919 webint_code-0.0.17/webint_code/templates/pypi/index.html
+-rw-r--r--   0        0        0      227 2023-01-27 00:43:27.579919 webint_code-0.0.17/webint_code/templates/pypi/project.html
+-rw-r--r--   0        0        0       87 2023-01-27 00:43:27.579919 webint_code-0.0.17/webint_code/templates/search/index.html
+-rw-r--r--   0        0        0     1029 2023-01-27 00:43:27.583919 webint_code-0.0.17/webint_code/templates/search/results.html
+-rw-r--r--   0        0        0     4967 2023-05-18 23:21:54.011448 webint_code-0.0.17/webint_code/templates/system.html
+-rw-r--r--   0        0        0      149 2023-01-27 00:43:27.567919 webint_code-0.0.17/webint_code/templates/template.html
+-rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 webint_code-0.0.17/setup.py
+-rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 webint_code-0.0.17/PKG-INFO
```

### Comparing `webint_code-0.0.16/pyproject.toml` & `webint_code-0.0.17/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webint-code"
-version = "0.0.16"
+version = "0.0.17"
 description = "manage code on your website"
 keywords = ["webint", "Git", "PyPI"]
 homepage = "https://ragt.ag/code/projects/webint-code"
 repository = "https://ragt.ag/code/projects/webint-code.git"
 documentation = "https://ragt.ag/code/projects/webint-code/api"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "BSD-2-Clause"
```

### Comparing `webint_code-0.0.16/webint_code/__init__.py` & `webint_code-0.0.17/webint_code/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,28 +82,29 @@
     """
     project_dir = meta_dir / project
     testing_dir = project_dir / "testing"
     shutil.rmtree(testing_dir, ignore_errors=True)
     gmpg.clone_repo(project_dir / "source.git", testing_dir)
     time.sleep(5)
     gmpg.strip_local_dev_deps(testing_dir)
-    poetry_binary = "/home/admin/.local/bin/poetry"  # XXX "/srv/poetry/bin/poetry"
-    print(
-        subprocess.run(
-            [poetry_binary, "install"],
+
+    def run_poetry(*command, capture_output=False):
+        return subprocess.run(
+            ["/home/admin/.local/bin/poetry", *command],
             cwd=testing_dir,
-            capture_output=True,
+            capture_output=capture_output,
         )
-    )
+
+    print(run_poetry("install"))
     print("installation complete")
-    subprocess.run([poetry_binary, "run", "gmpg", "test"], cwd=testing_dir)
+    run_poetry("run", "gmpg", "test")
     print("testing complete")
-    subprocess.run([poetry_binary, "run", "gmpg", "analyze"], cwd=testing_dir)
+    run_poetry("run", "gmpg", "analyze")
     print("API analysis complete")
-    subprocess.run([poetry_binary, "run", "gmpg", "graph"], cwd=testing_dir)
+    run_poetry("run", "gmpg", "graph")
     print("dependency visualization complete")
 
 
 @app.query
 def search(db, query):
     """Search for `query` in commited code."""
     files = {}
```

### Comparing `webint_code-0.0.16/webint_code/templates/project/commit.html` & `webint_code-0.0.17/webint_code/templates/project/commit.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.16/webint_code/templates/project/commit_log.html` & `webint_code-0.0.17/webint_code/templates/project/commit_log.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.16/webint_code/templates/project/index.html` & `webint_code-0.0.17/webint_code/templates/project/index.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.16/webint_code/templates/project/issues.html` & `webint_code-0.0.17/webint_code/templates/project/issues.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.16/webint_code/templates/project/namespace.html` & `webint_code-0.0.17/webint_code/templates/project/namespace.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.16/webint_code/templates/project/release_file.html` & `webint_code-0.0.17/webint_code/templates/project/release_file.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.16/webint_code/templates/project/repository_file.html` & `webint_code-0.0.17/webint_code/templates/project/repository_file.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.16/webint_code/templates/search/results.html` & `webint_code-0.0.17/webint_code/templates/search/results.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.16/webint_code/templates/system.html` & `webint_code-0.0.17/webint_code/templates/system.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.16/setup.py` & `webint_code-0.0.17/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'webint>=0.0']
 
 entry_points = \
 {'webapps': ['code = webint_code:app']}
 
 setup_kwargs = {
     'name': 'webint-code',
-    'version': '0.0.16',
+    'version': '0.0.17',
     'description': 'manage code on your website',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://ragt.ag/code/projects/webint-code',
```

### Comparing `webint_code-0.0.16/PKG-INFO` & `webint_code-0.0.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webint-code
-Version: 0.0.16
+Version: 0.0.17
 Summary: manage code on your website
 Home-page: https://ragt.ag/code/projects/webint-code
 License: BSD-2-Clause
 Keywords: webint,Git,PyPI
 Author: Angelo Gladding
 Author-email: angelo@ragt.ag
 Requires-Python: >=3.10,<3.11
```

