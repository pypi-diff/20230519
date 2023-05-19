# Comparing `tmp/webint_code-0.0.15.tar.gz` & `tmp/webint_code-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webint_code-0.0.15.tar", max compression
+gzip compressed data, was "webint_code-0.0.16.tar", max compression
```

## Comparing `webint_code-0.0.15.tar` & `webint_code-0.0.16.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1131 2023-05-18 23:12:02.565916 webint_code-0.0.15/pyproject.toml
--rw-r--r--   0        0        0    18967 2023-05-18 22:36:21.174177 webint_code-0.0.15/webint_code/__init__.py
--rw-r--r--   0        0        0      474 2023-01-27 00:43:27.567919 webint_code-0.0.15/webint_code/templates/__init__.py
--rw-r--r--   0        0        0      161 2023-02-20 19:30:47.711101 webint_code-0.0.15/webint_code/templates/index.html
--rw-r--r--   0        0        0     1225 2023-01-27 00:43:27.575919 webint_code-0.0.15/webint_code/templates/project/commit.html
--rw-r--r--   0        0        0      651 2023-01-27 00:43:27.567919 webint_code-0.0.15/webint_code/templates/project/commit_log.html
--rw-r--r--   0        0        0      116 2023-01-27 00:43:27.571919 webint_code-0.0.15/webint_code/templates/project/created.html
--rw-r--r--   0        0        0    10118 2023-01-27 00:43:27.571919 webint_code-0.0.15/webint_code/templates/project/index.html
--rw-r--r--   0        0        0      872 2023-01-27 00:43:27.575919 webint_code-0.0.15/webint_code/templates/project/issues.html
--rw-r--r--   0        0        0     2921 2023-01-27 00:43:27.571919 webint_code-0.0.15/webint_code/templates/project/namespace.html
--rw-r--r--   0        0        0      294 2023-01-27 00:43:27.571919 webint_code-0.0.15/webint_code/templates/project/release.html
--rw-r--r--   0        0        0      777 2023-01-27 00:43:27.575919 webint_code-0.0.15/webint_code/templates/project/release_file.html
--rw-r--r--   0        0        0     1063 2023-01-27 00:43:27.571919 webint_code-0.0.15/webint_code/templates/project/repository_file.html
--rw-r--r--   0        0        0      485 2023-01-27 00:43:27.575919 webint_code-0.0.15/webint_code/templates/project/settings.html
--rw-r--r--   0        0        0      373 2023-01-27 00:43:27.579919 webint_code-0.0.15/webint_code/templates/projects.html
--rw-r--r--   0        0        0      136 2023-01-27 00:43:27.579919 webint_code-0.0.15/webint_code/templates/pypi/index.html
--rw-r--r--   0        0        0      227 2023-01-27 00:43:27.579919 webint_code-0.0.15/webint_code/templates/pypi/project.html
--rw-r--r--   0        0        0       87 2023-01-27 00:43:27.579919 webint_code-0.0.15/webint_code/templates/search/index.html
--rw-r--r--   0        0        0     1029 2023-01-27 00:43:27.583919 webint_code-0.0.15/webint_code/templates/search/results.html
--rw-r--r--   0        0        0     4967 2023-02-19 06:49:46.337101 webint_code-0.0.15/webint_code/templates/system.html
--rw-r--r--   0        0        0      149 2023-01-27 00:43:27.567919 webint_code-0.0.15/webint_code/templates/template.html
--rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 webint_code-0.0.15/setup.py
--rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 webint_code-0.0.15/PKG-INFO
+-rw-r--r--   0        0        0     1131 2023-05-19 00:23:08.588808 webint_code-0.0.16/pyproject.toml
+-rw-r--r--   0        0        0    19028 2023-05-19 00:23:07.296788 webint_code-0.0.16/webint_code/__init__.py
+-rw-r--r--   0        0        0      474 2023-01-27 00:43:27.567919 webint_code-0.0.16/webint_code/templates/__init__.py
+-rw-r--r--   0        0        0      161 2023-02-20 19:30:47.711101 webint_code-0.0.16/webint_code/templates/index.html
+-rw-r--r--   0        0        0     1225 2023-01-27 00:43:27.575919 webint_code-0.0.16/webint_code/templates/project/commit.html
+-rw-r--r--   0        0        0      651 2023-01-27 00:43:27.567919 webint_code-0.0.16/webint_code/templates/project/commit_log.html
+-rw-r--r--   0        0        0      116 2023-01-27 00:43:27.571919 webint_code-0.0.16/webint_code/templates/project/created.html
+-rw-r--r--   0        0        0    10118 2023-01-27 00:43:27.571919 webint_code-0.0.16/webint_code/templates/project/index.html
+-rw-r--r--   0        0        0      872 2023-01-27 00:43:27.575919 webint_code-0.0.16/webint_code/templates/project/issues.html
+-rw-r--r--   0        0        0     2921 2023-01-27 00:43:27.571919 webint_code-0.0.16/webint_code/templates/project/namespace.html
+-rw-r--r--   0        0        0      294 2023-01-27 00:43:27.571919 webint_code-0.0.16/webint_code/templates/project/release.html
+-rw-r--r--   0        0        0      777 2023-01-27 00:43:27.575919 webint_code-0.0.16/webint_code/templates/project/release_file.html
+-rw-r--r--   0        0        0     1063 2023-01-27 00:43:27.571919 webint_code-0.0.16/webint_code/templates/project/repository_file.html
+-rw-r--r--   0        0        0      485 2023-01-27 00:43:27.575919 webint_code-0.0.16/webint_code/templates/project/settings.html
+-rw-r--r--   0        0        0      373 2023-01-27 00:43:27.579919 webint_code-0.0.16/webint_code/templates/projects.html
+-rw-r--r--   0        0        0      136 2023-01-27 00:43:27.579919 webint_code-0.0.16/webint_code/templates/pypi/index.html
+-rw-r--r--   0        0        0      227 2023-01-27 00:43:27.579919 webint_code-0.0.16/webint_code/templates/pypi/project.html
+-rw-r--r--   0        0        0       87 2023-01-27 00:43:27.579919 webint_code-0.0.16/webint_code/templates/search/index.html
+-rw-r--r--   0        0        0     1029 2023-01-27 00:43:27.583919 webint_code-0.0.16/webint_code/templates/search/results.html
+-rw-r--r--   0        0        0     4967 2023-05-18 23:21:54.011448 webint_code-0.0.16/webint_code/templates/system.html
+-rw-r--r--   0        0        0      149 2023-01-27 00:43:27.567919 webint_code-0.0.16/webint_code/templates/template.html
+-rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 webint_code-0.0.16/setup.py
+-rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 webint_code-0.0.16/PKG-INFO
```

### Comparing `webint_code-0.0.15/pyproject.toml` & `webint_code-0.0.16/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webint-code"
-version = "0.0.15"
+version = "0.0.16"
 description = "manage code on your website"
 keywords = ["webint", "Git", "PyPI"]
 homepage = "https://ragt.ag/code/projects/webint-code"
 repository = "https://ragt.ag/code/projects/webint-code.git"
 documentation = "https://ragt.ag/code/projects/webint-code/api"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "BSD-2-Clause"
```

### Comparing `webint_code-0.0.15/webint_code/__init__.py` & `webint_code-0.0.16/webint_code/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,25 +56,25 @@
             "version": "TEXT",
         },
     },
 )
 
 code_dir = pathlib.Path("code")
 meta_dir = code_dir / "meta"
-working_dir = code_dir / "working"
+# XXX working_dir = code_dir / "working"
 
 
-def update_system():
-    print(
-        subprocess.run(
-            ["poetry", "update"],
-            cwd=working_dir / "ragt.ag",
-            capture_output=True,
-        )
-    )
+# XXX def update_system():
+# XXX     print(
+# XXX         subprocess.run(
+# XXX             ["poetry", "update"],
+# XXX             cwd=working_dir / "ragt.ag",
+# XXX             capture_output=True,
+# XXX         )
+# XXX     )
 
 
 def run_ci(project):
     """
     Run continuous integration pipeline.
 
     Execute tests.
@@ -82,34 +82,28 @@
     """
     project_dir = meta_dir / project
     testing_dir = project_dir / "testing"
     shutil.rmtree(testing_dir, ignore_errors=True)
     gmpg.clone_repo(project_dir / "source.git", testing_dir)
     time.sleep(5)
     gmpg.strip_local_dev_deps(testing_dir)
+    poetry_binary = "/home/admin/.local/bin/poetry"  # XXX "/srv/poetry/bin/poetry"
     print(
         subprocess.run(
-            ["/srv/poetry/bin/poetry", "install"],
+            [poetry_binary, "install"],
             cwd=testing_dir,
             capture_output=True,
         )
     )
     print("installation complete")
-    # XXX print(
-    # XXX     subprocess.run(
-    # XXX         ["/srv/poetry/bin/poetry", "run", "which", "gmpg"], cwd=testing_dir
-    # XXX     )
-    # XXX )
-    subprocess.run(["/srv/poetry/bin/poetry", "run", "gmpg", "test"], cwd=testing_dir)
+    subprocess.run([poetry_binary, "run", "gmpg", "test"], cwd=testing_dir)
     print("testing complete")
-    subprocess.run(
-        ["/srv/poetry/bin/poetry", "run", "gmpg", "analyze"], cwd=testing_dir
-    )
+    subprocess.run([poetry_binary, "run", "gmpg", "analyze"], cwd=testing_dir)
     print("API analysis complete")
-    subprocess.run(["/srv/poetry/bin/poetry", "run", "gmpg", "graph"], cwd=testing_dir)
+    subprocess.run([poetry_binary, "run", "gmpg", "graph"], cwd=testing_dir)
     print("dependency visualization complete")
 
 
 @app.query
 def search(db, query):
     """Search for `query` in commited code."""
     files = {}
@@ -141,18 +135,18 @@
                 [line.partition(":")[2] for line in block_text.splitlines()]
             )
             blocks[starting_line] = block
         files[filename.lstrip(":").partition("/working/")[::2]] = blocks
     return files
 
 
-@app.wrap
-def set_working_dir(handler, main_app):
-    web.tx.host.working_dir = working_dir
-    yield
+# XXX @app.wrap
+# XXX def set_working_dir(handler, main_app):
+# XXX     web.tx.host.working_dir = working_dir
+# XXX     yield
 
 
 @app.query
 def create_project(db, name):
     """Create a project."""
     db.insert("projects", name=name, pypi=name, visibility="public")
     project_dir = meta_dir / name
@@ -177,18 +171,20 @@
     subprocess.run(["chgrp", "www-data", bare_repo, working_repo, "-R"])
     subprocess.run(["chmod", "g+w", bare_repo, working_repo, "-R"])
     if not (meta_dir / "gitpasswd").exists():
         token = web.application("webint_auth").model.generate_local_token(
             "/code", "webint_code", "git_owner"
         )
         subprocess.run(["htpasswd", "-cb", meta_dir / "gitpasswd", "owner", token])
+
     # XXX subprocess.run(["sudo", "service", "nginx", "restart"])
-    gmpg.clone_repo(
-        f"{web.tx.origin}/code/projects/{name}.git", f"{working_dir}/{name}"
-    )
+
+    # XXX gmpg.clone_repo(
+    # XXX     f"{web.tx.origin}/code/projects/{name}.git", f"{working_dir}/{name}"
+    # XXX )
 
 
 @app.query
 def get_projects(db):
     """Return a list of project names."""
     visibility_wheres = ["public"]
     if web.tx.user.is_owner:
@@ -610,24 +606,24 @@
         try:
             query = web.form("q").q
         except web.BadRequest:
             return app.view.search.index()
         return app.view.search.results(query, app.model.search(query))
 
 
-@app.control("system")
-class System:
-    """System code."""
-
-    def get(self):
-        """"""
-        return app.view.system(web.tx.app)
-
-
-@app.control("system/update")
-class SystemUpdate:
-    """Update the system."""
-
-    def post(self):
-        """"""
-        web.enqueue(update_system)
-        return "update has been started"
+# XXX @app.control("system")
+# XXX class System:
+# XXX     """System code."""
+# XXX
+# XXX     def get(self):
+# XXX         """"""
+# XXX         return app.view.system(web.tx.app)
+# XXX
+# XXX
+# XXX @app.control("system/update")
+# XXX class SystemUpdate:
+# XXX     """Update the system."""
+# XXX
+# XXX     def post(self):
+# XXX         """"""
+# XXX         web.enqueue(update_system)
+# XXX         return "update has been started"
```

### Comparing `webint_code-0.0.15/webint_code/templates/project/commit.html` & `webint_code-0.0.16/webint_code/templates/project/commit.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.15/webint_code/templates/project/commit_log.html` & `webint_code-0.0.16/webint_code/templates/project/commit_log.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.15/webint_code/templates/project/index.html` & `webint_code-0.0.16/webint_code/templates/project/index.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.15/webint_code/templates/project/issues.html` & `webint_code-0.0.16/webint_code/templates/project/issues.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.15/webint_code/templates/project/namespace.html` & `webint_code-0.0.16/webint_code/templates/project/namespace.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.15/webint_code/templates/project/release_file.html` & `webint_code-0.0.16/webint_code/templates/project/release_file.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.15/webint_code/templates/project/repository_file.html` & `webint_code-0.0.16/webint_code/templates/project/repository_file.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.15/webint_code/templates/search/results.html` & `webint_code-0.0.16/webint_code/templates/search/results.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.15/webint_code/templates/system.html` & `webint_code-0.0.16/webint_code/templates/system.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.15/setup.py` & `webint_code-0.0.16/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'webint>=0.0']
 
 entry_points = \
 {'webapps': ['code = webint_code:app']}
 
 setup_kwargs = {
     'name': 'webint-code',
-    'version': '0.0.15',
+    'version': '0.0.16',
     'description': 'manage code on your website',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://ragt.ag/code/projects/webint-code',
```

### Comparing `webint_code-0.0.15/PKG-INFO` & `webint_code-0.0.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webint-code
-Version: 0.0.15
+Version: 0.0.16
 Summary: manage code on your website
 Home-page: https://ragt.ag/code/projects/webint-code
 License: BSD-2-Clause
 Keywords: webint,Git,PyPI
 Author: Angelo Gladding
 Author-email: angelo@ragt.ag
 Requires-Python: >=3.10,<3.11
```

