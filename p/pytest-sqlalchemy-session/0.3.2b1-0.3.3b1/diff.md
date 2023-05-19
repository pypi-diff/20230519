# Comparing `tmp/pytest-sqlalchemy-session-0.3.2b1.tar.gz` & `tmp/pytest-sqlalchemy-session-0.3.3b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-sqlalchemy-session-0.3.2b1.tar", last modified: Thu May 18 13:38:53 2023, max compression
+gzip compressed data, was "pytest-sqlalchemy-session-0.3.3b1.tar", last modified: Thu May 18 14:31:25 2023, max compression
```

## Comparing `pytest-sqlalchemy-session-0.3.2b1.tar` & `pytest-sqlalchemy-session-0.3.3b1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:38:53.539015 pytest-sqlalchemy-session-0.3.2b1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-18 13:38:42.000000 pytest-sqlalchemy-session-0.3.2b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 13:38:42.000000 pytest-sqlalchemy-session-0.3.2b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-18 13:38:53.539015 pytest-sqlalchemy-session-0.3.2b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-18 13:38:42.000000 pytest-sqlalchemy-session-0.3.2b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-18 13:38:42.000000 pytest-sqlalchemy-session-0.3.2b1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:38:53.535015 pytest-sqlalchemy-session-0.3.2b1/pytest_sqlalchemy_session/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:38:42.000000 pytest-sqlalchemy-session-0.3.2b1/pytest_sqlalchemy_session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-05-18 13:38:42.000000 pytest-sqlalchemy-session-0.3.2b1/pytest_sqlalchemy_session/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-18 13:38:42.000000 pytest-sqlalchemy-session-0.3.2b1/pytest_sqlalchemy_session/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-18 13:38:42.000000 pytest-sqlalchemy-session-0.3.2b1/pytest_sqlalchemy_session/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-18 13:38:42.000000 pytest-sqlalchemy-session-0.3.2b1/pytest_sqlalchemy_session/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:38:53.535015 pytest-sqlalchemy-session-0.3.2b1/pytest_sqlalchemy_session.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-18 13:38:53.000000 pytest-sqlalchemy-session-0.3.2b1/pytest_sqlalchemy_session.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-18 13:38:53.000000 pytest-sqlalchemy-session-0.3.2b1/pytest_sqlalchemy_session.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 13:38:53.000000 pytest-sqlalchemy-session-0.3.2b1/pytest_sqlalchemy_session.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-18 13:38:53.000000 pytest-sqlalchemy-session-0.3.2b1/pytest_sqlalchemy_session.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-18 13:38:53.000000 pytest-sqlalchemy-session-0.3.2b1/pytest_sqlalchemy_session.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-18 13:38:53.000000 pytest-sqlalchemy-session-0.3.2b1/pytest_sqlalchemy_session.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:38:53.535015 pytest-sqlalchemy-session-0.3.2b1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-18 13:38:42.000000 pytest-sqlalchemy-session-0.3.2b1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-18 13:38:53.539015 pytest-sqlalchemy-session-0.3.2b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:38:53.539015 pytest-sqlalchemy-session-0.3.2b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-18 13:38:42.000000 pytest-sqlalchemy-session-0.3.2b1/tests/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-05-18 13:38:42.000000 pytest-sqlalchemy-session-0.3.2b1/tests/test_strict_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:31:25.677037 pytest-sqlalchemy-session-0.3.3b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-18 14:31:12.000000 pytest-sqlalchemy-session-0.3.3b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 14:31:12.000000 pytest-sqlalchemy-session-0.3.3b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-18 14:31:25.677037 pytest-sqlalchemy-session-0.3.3b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-18 14:31:12.000000 pytest-sqlalchemy-session-0.3.3b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-18 14:31:12.000000 pytest-sqlalchemy-session-0.3.3b1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:31:25.677037 pytest-sqlalchemy-session-0.3.3b1/pytest_sqlalchemy_session/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 14:31:12.000000 pytest-sqlalchemy-session-0.3.3b1/pytest_sqlalchemy_session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-18 14:31:12.000000 pytest-sqlalchemy-session-0.3.3b1/pytest_sqlalchemy_session/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-18 14:31:12.000000 pytest-sqlalchemy-session-0.3.3b1/pytest_sqlalchemy_session/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-18 14:31:12.000000 pytest-sqlalchemy-session-0.3.3b1/pytest_sqlalchemy_session/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-18 14:31:12.000000 pytest-sqlalchemy-session-0.3.3b1/pytest_sqlalchemy_session/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:31:25.677037 pytest-sqlalchemy-session-0.3.3b1/pytest_sqlalchemy_session.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-18 14:31:25.000000 pytest-sqlalchemy-session-0.3.3b1/pytest_sqlalchemy_session.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-18 14:31:25.000000 pytest-sqlalchemy-session-0.3.3b1/pytest_sqlalchemy_session.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 14:31:25.000000 pytest-sqlalchemy-session-0.3.3b1/pytest_sqlalchemy_session.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-18 14:31:25.000000 pytest-sqlalchemy-session-0.3.3b1/pytest_sqlalchemy_session.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-18 14:31:25.000000 pytest-sqlalchemy-session-0.3.3b1/pytest_sqlalchemy_session.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-18 14:31:25.000000 pytest-sqlalchemy-session-0.3.3b1/pytest_sqlalchemy_session.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:31:25.677037 pytest-sqlalchemy-session-0.3.3b1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-18 14:31:12.000000 pytest-sqlalchemy-session-0.3.3b1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-18 14:31:25.677037 pytest-sqlalchemy-session-0.3.3b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:31:25.677037 pytest-sqlalchemy-session-0.3.3b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-18 14:31:12.000000 pytest-sqlalchemy-session-0.3.3b1/tests/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-05-18 14:31:12.000000 pytest-sqlalchemy-session-0.3.3b1/tests/test_strict_mode.py
```

### Comparing `pytest-sqlalchemy-session-0.3.2b1/LICENSE` & `pytest-sqlalchemy-session-0.3.3b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-sqlalchemy-session-0.3.2b1/PKG-INFO` & `pytest-sqlalchemy-session-0.3.3b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-sqlalchemy-session
-Version: 0.3.2b1
+Version: 0.3.3b1
 Summary: A pytest plugin for preserving test isolation that use SQLAlchemy.
 Author-email: Stanislav Shkitin <stanislav.shkitin@yandex.ru>
 License: MIT
 Keywords: pytest,sqlalchemy,transaction
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
```

### Comparing `pytest-sqlalchemy-session-0.3.2b1/pyproject.toml` & `pytest-sqlalchemy-session-0.3.3b1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pytest-sqlalchemy-session'
-version = "0.3.2-beta1"
+version = "0.3.3-beta1"
 authors = [
     {name = "Stanislav Shkitin", email = "stanislav.shkitin@yandex.ru"},
 ]
 license = {text = "MIT"}
 description = "A pytest plugin for preserving test isolation that use SQLAlchemy."
 keywords = ["pytest", "sqlalchemy", "transaction"]
 readme = "README.md"
```

### Comparing `pytest-sqlalchemy-session-0.3.2b1/pytest_sqlalchemy_session/fixtures.py` & `pytest-sqlalchemy-session-0.3.3b1/pytest_sqlalchemy_session/fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,21 +40,22 @@
     def close() -> None:
         session.rollback()
 
     session.close = close
 
     # Begin a nested transaction (any new transactions created in the codebase
     # will be held until this outer transaction is committed or closed)
-    session.begin_nested()
+    main_nested_transaction = session.begin_nested()
 
     # Each time the SAVEPOINT for the nested transaction ends, reopen it
     @event.listens_for(session, "after_transaction_end")
     def restart_savepoint(session: Session, trans: SessionTransaction) -> None:
         if root_transaction.is_active and (
             getattr(trans, "fake_nested", None)
+            or (trans.nested and trans.parent == main_nested_transaction)
             or (trans.nested and not trans.parent.nested)
         ):
             # ensure that state is expired the way
             # session.commit() at the top level normally does
             session.expire_all()
 
             if (
```

### Comparing `pytest-sqlalchemy-session-0.3.2b1/pytest_sqlalchemy_session/plugin.py` & `pytest-sqlalchemy-session-0.3.3b1/pytest_sqlalchemy_session/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-sqlalchemy-session-0.3.2b1/pytest_sqlalchemy_session/session.py` & `pytest-sqlalchemy-session-0.3.3b1/pytest_sqlalchemy_session/session.py`

 * *Files identical despite different names*

### Comparing `pytest-sqlalchemy-session-0.3.2b1/pytest_sqlalchemy_session/version.py` & `pytest-sqlalchemy-session-0.3.3b1/pytest_sqlalchemy_session/version.py`

 * *Files identical despite different names*

### Comparing `pytest-sqlalchemy-session-0.3.2b1/pytest_sqlalchemy_session.egg-info/PKG-INFO` & `pytest-sqlalchemy-session-0.3.3b1/pytest_sqlalchemy_session.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-sqlalchemy-session
-Version: 0.3.2b1
+Version: 0.3.3b1
 Summary: A pytest plugin for preserving test isolation that use SQLAlchemy.
 Author-email: Stanislav Shkitin <stanislav.shkitin@yandex.ru>
 License: MIT
 Keywords: pytest,sqlalchemy,transaction
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
```

### Comparing `pytest-sqlalchemy-session-0.3.2b1/pytest_sqlalchemy_session.egg-info/SOURCES.txt` & `pytest-sqlalchemy-session-0.3.3b1/pytest_sqlalchemy_session.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-sqlalchemy-session-0.3.2b1/setup.cfg` & `pytest-sqlalchemy-session-0.3.3b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-sqlalchemy-session-0.3.2b1/tests/test_configs.py` & `pytest-sqlalchemy-session-0.3.3b1/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `pytest-sqlalchemy-session-0.3.2b1/tests/test_strict_mode.py` & `pytest-sqlalchemy-session-0.3.3b1/tests/test_strict_mode.py`

 * *Files identical despite different names*

