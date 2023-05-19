# Comparing `tmp/heist-6.3.0.tar.gz` & `tmp/heist-6.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heist-6.3.0.tar", last modified: Wed May  3 18:22:30 2023, max compression
+gzip compressed data, was "heist-6.3.1.tar", last modified: Fri May 19 14:16:47 2023, max compression
```

## Comparing `heist-6.3.0.tar` & `heist-6.3.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.896367 heist-6.3.0/
--rw-rw-rw-   0 root         (0) root         (0)    11357 2023-05-03 18:22:18.000000 heist-6.3.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-05-03 18:22:18.000000 heist-6.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2804 2023-05-03 18:22:30.894534 heist-6.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2331 2023-05-03 18:22:18.000000 heist-6.3.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.885367 heist-6.3.0/heist/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.878033 heist-6.3.0/heist/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.886283 heist-6.3.0/heist/acct/artifact/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 18:22:18.000000 heist-6.3.0/heist/acct/artifact/jfrog.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.887200 heist-6.3.0/heist/acct/recursive_contracts/
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-05-03 18:22:18.000000 heist-6.3.0/heist/acct/recursive_contracts/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.878950 heist-6.3.0/heist/acct/tunnel/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.888117 heist-6.3.0/heist/acct/tunnel/ssh/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 18:22:18.000000 heist-6.3.0/heist/acct/tunnel/ssh/gssapi.py
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-05-03 18:22:18.000000 heist-6.3.0/heist/acct/tunnel/ssh/pam.py
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-05-03 18:22:18.000000 heist-6.3.0/heist/acct/tunnel/ssh/password.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 18:22:18.000000 heist-6.3.0/heist/acct/tunnel/ssh/public_key.py
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-05-03 18:22:18.000000 heist-6.3.0/heist/acct/tunnel/ssh/secure_id.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.888117 heist-6.3.0/heist/artifact/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.889034 heist-6.3.0/heist/artifact/contracts/
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-05-03 18:22:18.000000 heist-6.3.0/heist/artifact/contracts/init.py
--rw-rw-rw-   0 root         (0) root         (0)    15694 2023-05-03 18:22:18.000000 heist-6.3.0/heist/artifact/init.py
--rw-rw-rw-   0 root         (0) root         (0)     5158 2023-05-03 18:22:18.000000 heist-6.3.0/heist/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.889034 heist-6.3.0/heist/heist/
--rw-rw-rw-   0 root         (0) root         (0)     8876 2023-05-03 18:22:18.000000 heist-6.3.0/heist/heist/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.889950 heist-6.3.0/heist/heist/recursive_contracts/
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-05-03 18:22:18.000000 heist-6.3.0/heist/heist/recursive_contracts/init.py
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-05-03 18:22:18.000000 heist-6.3.0/heist/heist/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.890867 heist-6.3.0/heist/roster/
--rw-rw-rw-   0 root         (0) root         (0)     2221 2023-05-03 18:22:18.000000 heist-6.3.0/heist/roster/clustershell.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.891784 heist-6.3.0/heist/roster/contracts/
--rw-rw-rw-   0 root         (0) root         (0)      276 2023-05-03 18:22:18.000000 heist-6.3.0/heist/roster/contracts/init.py
--rw-rw-rw-   0 root         (0) root         (0)      333 2023-05-03 18:22:18.000000 heist-6.3.0/heist/roster/fernet.py
--rw-rw-rw-   0 root         (0) root         (0)      676 2023-05-03 18:22:18.000000 heist-6.3.0/heist/roster/flat.py
--rw-rw-rw-   0 root         (0) root         (0)     1866 2023-05-03 18:22:18.000000 heist-6.3.0/heist/roster/init.py
--rw-rw-rw-   0 root         (0) root         (0)     1951 2023-05-03 18:22:18.000000 heist-6.3.0/heist/roster/scan.py
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-05-03 18:22:18.000000 heist-6.3.0/heist/scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.892701 heist-6.3.0/heist/service/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.892701 heist-6.3.0/heist/service/contracts/
--rw-rw-rw-   0 root         (0) root         (0)     1100 2023-05-03 18:22:18.000000 heist-6.3.0/heist/service/contracts/init.py
--rw-rw-rw-   0 root         (0) root         (0)     3290 2023-05-03 18:22:18.000000 heist-6.3.0/heist/service/init.py
--rw-rw-rw-   0 root         (0) root         (0)     3236 2023-05-03 18:22:18.000000 heist-6.3.0/heist/service/raw.py
--rw-rw-rw-   0 root         (0) root         (0)     2013 2023-05-03 18:22:18.000000 heist-6.3.0/heist/service/systemd.py
--rw-rw-rw-   0 root         (0) root         (0)     2308 2023-05-03 18:22:18.000000 heist-6.3.0/heist/service/win_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.893617 heist-6.3.0/heist/tool/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-05-03 18:22:18.000000 heist-6.3.0/heist/tool/artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)     3064 2023-05-03 18:22:18.000000 heist-6.3.0/heist/tool/path.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-05-03 18:22:18.000000 heist-6.3.0/heist/tool/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.894534 heist-6.3.0/heist/tunnel/
--rw-rw-rw-   0 root         (0) root         (0)     7861 2023-05-03 18:22:18.000000 heist-6.3.0/heist/tunnel/asyncssh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.894534 heist-6.3.0/heist/tunnel/contracts/
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-05-03 18:22:18.000000 heist-6.3.0/heist/tunnel/contracts/init.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-03 18:22:18.000000 heist-6.3.0/heist/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.886283 heist-6.3.0/heist.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2804 2023-05-03 18:22:30.000000 heist-6.3.0/heist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1065 2023-05-03 18:22:30.000000 heist-6.3.0/heist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 18:22:30.000000 heist-6.3.0/heist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-03 18:22:30.000000 heist-6.3.0/heist.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       92 2023-05-03 18:22:30.000000 heist-6.3.0/heist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-03 18:22:30.000000 heist-6.3.0/heist.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      686 2023-05-03 18:22:18.000000 heist-6.3.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-05-03 18:22:18.000000 heist-6.3.0/requirements-test.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 18:22:30.896367 heist-6.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2031 2023-05-03 18:22:18.000000 heist-6.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:16:47.972847 heist-6.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2023-05-19 14:16:38.000000 heist-6.3.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-05-19 14:16:38.000000 heist-6.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2804 2023-05-19 14:16:47.972847 heist-6.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2331 2023-05-19 14:16:38.000000 heist-6.3.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:16:47.965847 heist-6.3.1/heist/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:16:47.961847 heist-6.3.1/heist/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:16:47.966847 heist-6.3.1/heist/acct/artifact/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 14:16:38.000000 heist-6.3.1/heist/acct/artifact/jfrog.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:16:47.966847 heist-6.3.1/heist/acct/recursive_contracts/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-05-19 14:16:38.000000 heist-6.3.1/heist/acct/recursive_contracts/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:16:47.962847 heist-6.3.1/heist/acct/tunnel/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:16:47.967847 heist-6.3.1/heist/acct/tunnel/ssh/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 14:16:38.000000 heist-6.3.1/heist/acct/tunnel/ssh/gssapi.py
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-05-19 14:16:38.000000 heist-6.3.1/heist/acct/tunnel/ssh/pam.py
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-05-19 14:16:38.000000 heist-6.3.1/heist/acct/tunnel/ssh/password.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-19 14:16:38.000000 heist-6.3.1/heist/acct/tunnel/ssh/public_key.py
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-05-19 14:16:38.000000 heist-6.3.1/heist/acct/tunnel/ssh/secure_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:16:47.967847 heist-6.3.1/heist/artifact/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:16:47.968847 heist-6.3.1/heist/artifact/contracts/
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-05-19 14:16:38.000000 heist-6.3.1/heist/artifact/contracts/init.py
+-rw-rw-rw-   0 root         (0) root         (0)    15694 2023-05-19 14:16:38.000000 heist-6.3.1/heist/artifact/init.py
+-rw-rw-rw-   0 root         (0) root         (0)     5158 2023-05-19 14:16:38.000000 heist-6.3.1/heist/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:16:47.968847 heist-6.3.1/heist/heist/
+-rw-rw-rw-   0 root         (0) root         (0)     8876 2023-05-19 14:16:38.000000 heist-6.3.1/heist/heist/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:16:47.968847 heist-6.3.1/heist/heist/recursive_contracts/
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-05-19 14:16:38.000000 heist-6.3.1/heist/heist/recursive_contracts/init.py
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-05-19 14:16:38.000000 heist-6.3.1/heist/heist/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:16:47.969847 heist-6.3.1/heist/roster/
+-rw-rw-rw-   0 root         (0) root         (0)     2221 2023-05-19 14:16:38.000000 heist-6.3.1/heist/roster/clustershell.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:16:47.970847 heist-6.3.1/heist/roster/contracts/
+-rw-rw-rw-   0 root         (0) root         (0)      276 2023-05-19 14:16:38.000000 heist-6.3.1/heist/roster/contracts/init.py
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-05-19 14:16:38.000000 heist-6.3.1/heist/roster/fernet.py
+-rw-rw-rw-   0 root         (0) root         (0)      676 2023-05-19 14:16:38.000000 heist-6.3.1/heist/roster/flat.py
+-rw-rw-rw-   0 root         (0) root         (0)     1866 2023-05-19 14:16:38.000000 heist-6.3.1/heist/roster/init.py
+-rw-rw-rw-   0 root         (0) root         (0)     1951 2023-05-19 14:16:38.000000 heist-6.3.1/heist/roster/scan.py
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-05-19 14:16:38.000000 heist-6.3.1/heist/scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:16:47.970847 heist-6.3.1/heist/service/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:16:47.970847 heist-6.3.1/heist/service/contracts/
+-rw-rw-rw-   0 root         (0) root         (0)     1100 2023-05-19 14:16:38.000000 heist-6.3.1/heist/service/contracts/init.py
+-rw-rw-rw-   0 root         (0) root         (0)     3290 2023-05-19 14:16:38.000000 heist-6.3.1/heist/service/init.py
+-rw-rw-rw-   0 root         (0) root         (0)     3289 2023-05-19 14:16:38.000000 heist-6.3.1/heist/service/raw.py
+-rw-rw-rw-   0 root         (0) root         (0)     2013 2023-05-19 14:16:38.000000 heist-6.3.1/heist/service/systemd.py
+-rw-rw-rw-   0 root         (0) root         (0)     2308 2023-05-19 14:16:38.000000 heist-6.3.1/heist/service/win_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:16:47.971847 heist-6.3.1/heist/tool/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-05-19 14:16:38.000000 heist-6.3.1/heist/tool/artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)     3064 2023-05-19 14:16:38.000000 heist-6.3.1/heist/tool/path.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-05-19 14:16:38.000000 heist-6.3.1/heist/tool/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:16:47.971847 heist-6.3.1/heist/tunnel/
+-rw-rw-rw-   0 root         (0) root         (0)     8093 2023-05-19 14:16:38.000000 heist-6.3.1/heist/tunnel/asyncssh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:16:47.971847 heist-6.3.1/heist/tunnel/contracts/
+-rw-rw-rw-   0 root         (0) root         (0)      410 2023-05-19 14:16:38.000000 heist-6.3.1/heist/tunnel/contracts/init.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-19 14:16:38.000000 heist-6.3.1/heist/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:16:47.966847 heist-6.3.1/heist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2804 2023-05-19 14:16:47.000000 heist-6.3.1/heist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-05-19 14:16:47.000000 heist-6.3.1/heist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 14:16:47.000000 heist-6.3.1/heist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-19 14:16:47.000000 heist-6.3.1/heist.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2023-05-19 14:16:47.000000 heist-6.3.1/heist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-19 14:16:47.000000 heist-6.3.1/heist.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      686 2023-05-19 14:16:38.000000 heist-6.3.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-05-19 14:16:38.000000 heist-6.3.1/requirements-test.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 14:16:47.972847 heist-6.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2023-05-19 14:16:38.000000 heist-6.3.1/setup.py
```

### Comparing `heist-6.3.0/LICENSE` & `heist-6.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `heist-6.3.0/PKG-INFO` & `heist-6.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heist
-Version: 6.3.0
+Version: 6.3.1
 Summary: Ephemeral software tunneling and delivery system
 Home-page: UNKNOWN
 Author: 
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `heist-6.3.0/README.rst` & `heist-6.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `heist-6.3.0/heist/artifact/init.py` & `heist-6.3.1/heist/artifact/init.py`

 * *Files identical despite different names*

### Comparing `heist-6.3.0/heist/conf.py` & `heist-6.3.1/heist/conf.py`

 * *Files identical despite different names*

### Comparing `heist-6.3.0/heist/heist/init.py` & `heist-6.3.1/heist/heist/init.py`

 * *Files identical despite different names*

### Comparing `heist-6.3.0/heist/heist/recursive_contracts/init.py` & `heist-6.3.1/heist/heist/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `heist-6.3.0/heist/roster/clustershell.py` & `heist-6.3.1/heist/roster/clustershell.py`

 * *Files identical despite different names*

### Comparing `heist-6.3.0/heist/roster/flat.py` & `heist-6.3.1/heist/roster/flat.py`

 * *Files identical despite different names*

### Comparing `heist-6.3.0/heist/roster/init.py` & `heist-6.3.1/heist/roster/init.py`

 * *Files identical despite different names*

### Comparing `heist-6.3.0/heist/roster/scan.py` & `heist-6.3.1/heist/roster/scan.py`

 * *Files identical despite different names*

### Comparing `heist-6.3.0/heist/service/contracts/init.py` & `heist-6.3.1/heist/service/contracts/init.py`

 * *Files identical despite different names*

### Comparing `heist-6.3.0/heist/service/init.py` & `heist-6.3.1/heist/service/init.py`

 * *Files identical despite different names*

### Comparing `heist-6.3.0/heist/service/raw.py` & `heist-6.3.1/heist/service/raw.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     hub,
     target_name,
     tunnel_plugin,
     service,
     run_cmd=None,
     target_os="linux",
     run_dir=None,
+    background=False,
     **kwargs,
 ):
     """
     Start the service in the background
     """
     # each heist manager will need to have a function
     # that validates the run_cmd input
@@ -28,15 +29,15 @@
         hub.log.error(
             f"The run command is not valid. Not starting the service {service}"
         )
         return False
     cmd = [f"{run_cmd}"]
     hub.log.info(f"Starting the service {service}")
     ret = await hub.tunnel[tunnel_plugin].cmd(
-        target_name, " ".join(cmd), background=True, target_os=target_os
+        target_name, " ".join(cmd), background=background, target_os=target_os
     )
     if ret.returncode != 0:
         hub.log.error(ret.stderr)
         return False
     return True
 
 
@@ -108,14 +109,14 @@
 
 
 async def status(hub, target_name, tunnel_plugin, service, target_os="linux", **kwargs):
     cmd = [f"pgrep -f {service}"]
     if target_os == "windows":
         cmd = [f'powershell -command "get-process {service}"']
     ret = await hub.tunnel[tunnel_plugin].cmd(
-        target_name, " ".join(cmd), target_os=target_os
+        target_name, " ".join(cmd), target_os=target_os, sudo=kwargs.get("sudo")
     )
     if ret.returncode != 0:
         hub.log.info(f"The service {service} is not running")
         return False
     hub.log.info(f"The service {service} is running")
     return True
```

### Comparing `heist-6.3.0/heist/service/systemd.py` & `heist-6.3.1/heist/service/systemd.py`

 * *Files identical despite different names*

### Comparing `heist-6.3.0/heist/service/win_service.py` & `heist-6.3.1/heist/service/win_service.py`

 * *Files identical despite different names*

### Comparing `heist-6.3.0/heist/tool/artifacts.py` & `heist-6.3.1/heist/tool/artifacts.py`

 * *Files identical despite different names*

### Comparing `heist-6.3.0/heist/tool/path.py` & `heist-6.3.1/heist/tool/path.py`

 * *Files identical despite different names*

### Comparing `heist-6.3.0/heist/tool/system.py` & `heist-6.3.1/heist/tool/system.py`

 * *Files identical despite different names*

### Comparing `heist-6.3.0/heist/tunnel/asyncssh.py` & `heist-6.3.1/heist/tunnel/asyncssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,20 +118,29 @@
     Take the file located on the remote system and copy it locally
     """
     sftp = hub.tunnel.asyncssh.CONS[name]["sftp"]
     await sftp.get(source, dest)
 
 
 async def cmd(
-    hub, name: str, command: str, background=False, target_os="linux", **kwargs
+    hub,
+    name: str,
+    command: str,
+    background=False,
+    target_os="linux",
+    sudo=None,
+    **kwargs,
 ):
     """
     Execute the given command on the machine associated with the named connection
     """
-    sudo = hub.tunnel.asyncssh.CONS[name].get("sudo")
+    # Allow us to bypass sudo settings in roster for commands
+    # that do not require sudo via kwargs
+    if sudo is None:
+        sudo = hub.tunnel.asyncssh.CONS[name].get("sudo")
     sudo_password = re.compile(r"(?:.*)[Pp]assword(?: for .*)?:", re.M)
     con: asyncssh.SSHClientConnection = hub.tunnel.asyncssh.CONS[name]["con"]
     if target_os == "windows":
         win_background_cmd = command
         arg_list = win_background_cmd.split()
         win_background_cmd = arg_list.pop(0)
         arg_list = " ".join(arg_list)
@@ -182,15 +191,17 @@
         async with con.create_process(command, **kwargs) as process:
             while not process.stdout.at_eof():
                 output = await process.stdout.read(1024)
                 if sudo_password.search(output):
                     process.stdin.write(
                         hub.tunnel.asyncssh.CONS[name].get("password") + "\n"
                     )
-                stdout = await process.stdout.read()
+                stdout = output
+                if not stdout:
+                    stdout = await process.stdout.read()
                 stderr = await process.stderr.readline()
                 result = NamespaceDict(
                     stdout=stdout,
                     stderr=stderr,
                     returncode=process.returncode,
                     exit_status=process.returncode,
                 )
```

### Comparing `heist-6.3.0/heist.egg-info/PKG-INFO` & `heist-6.3.1/heist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heist
-Version: 6.3.0
+Version: 6.3.1
 Summary: Ephemeral software tunneling and delivery system
 Home-page: UNKNOWN
 Author: 
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `heist-6.3.0/heist.egg-info/SOURCES.txt` & `heist-6.3.1/heist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heist-6.3.0/pyproject.toml` & `heist-6.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `heist-6.3.0/setup.py` & `heist-6.3.1/setup.py`

 * *Files identical despite different names*

