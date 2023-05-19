# Comparing `tmp/multisig_ci-0.4.6.tar.gz` & `tmp/multisig_ci-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multisig_ci-0.4.6.tar", max compression
+gzip compressed data, was "multisig_ci-0.4.7.tar", max compression
```

## Comparing `multisig_ci-0.4.6.tar` & `multisig_ci-0.4.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    34523 2023-03-02 17:37:16.968341 multisig_ci-0.4.6/LICENSE
--rw-r--r--   0        0        0        0 2023-03-02 17:37:16.968341 multisig_ci-0.4.6/multisig_ci/__init__.py
--rw-r--r--   0        0        0      570 2023-03-02 17:37:16.968341 multisig_ci-0.4.6/multisig_ci/__main__.py
--rw-r--r--   0        0        0     7536 2023-03-02 17:37:16.968341 multisig_ci-0.4.6/multisig_ci/ci_override.py
--rw-r--r--   0        0        0     5811 2023-03-02 17:37:16.968341 multisig_ci-0.4.6/multisig_ci/hydrate_ci_cache.py
--rw-r--r--   0        0        0     2033 2023-03-02 17:37:16.968341 multisig_ci-0.4.6/multisig_ci/run_brownie.py
--rw-r--r--   0        0        0      811 2023-03-02 17:37:16.968341 multisig_ci-0.4.6/multisig_ci/safes.py
--rw-r--r--   0        0        0     1492 2023-03-02 17:37:16.968341 multisig_ci-0.4.6/multisig_ci/sign.py
--rw-r--r--   0        0        0     1933 2023-03-02 17:37:16.968341 multisig_ci-0.4.6/multisig_ci/telegram.py
--rwxr-xr-x   0        0        0      651 2023-03-02 17:37:16.968341 multisig_ci-0.4.6/multisig_ci/test_telegram.sh
--rw-r--r--   0        0        0      492 2023-03-02 17:37:16.968341 multisig_ci-0.4.6/pyproject.toml
--rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 multisig_ci-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-19 01:02:35.833555 multisig_ci-0.4.7/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-19 01:02:35.833555 multisig_ci-0.4.7/multisig_ci/__init__.py
+-rw-r--r--   0        0        0      570 2023-05-19 01:02:35.833555 multisig_ci-0.4.7/multisig_ci/__main__.py
+-rw-r--r--   0        0        0     7536 2023-05-19 01:02:35.833555 multisig_ci-0.4.7/multisig_ci/ci_override.py
+-rw-r--r--   0        0        0     5811 2023-05-19 01:02:35.833555 multisig_ci-0.4.7/multisig_ci/hydrate_ci_cache.py
+-rw-r--r--   0        0        0     2033 2023-05-19 01:02:35.833555 multisig_ci-0.4.7/multisig_ci/run_brownie.py
+-rw-r--r--   0        0        0      811 2023-05-19 01:02:35.837556 multisig_ci-0.4.7/multisig_ci/safes.py
+-rw-r--r--   0        0        0     1492 2023-05-19 01:02:35.837556 multisig_ci-0.4.7/multisig_ci/sign.py
+-rw-r--r--   0        0        0     1929 2023-05-19 01:02:35.837556 multisig_ci-0.4.7/multisig_ci/telegram.py
+-rwxr-xr-x   0        0        0      651 2023-05-19 01:02:35.837556 multisig_ci-0.4.7/multisig_ci/test_telegram.sh
+-rw-r--r--   0        0        0      492 2023-05-19 01:02:35.837556 multisig_ci-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 multisig_ci-0.4.7/PKG-INFO
```

### Comparing `multisig_ci-0.4.6/LICENSE` & `multisig_ci-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.4.6/multisig_ci/__main__.py` & `multisig_ci-0.4.7/multisig_ci/__main__.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.4.6/multisig_ci/ci_override.py` & `multisig_ci-0.4.7/multisig_ci/ci_override.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.4.6/multisig_ci/hydrate_ci_cache.py` & `multisig_ci-0.4.7/multisig_ci/hydrate_ci_cache.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.4.6/multisig_ci/run_brownie.py` & `multisig_ci-0.4.7/multisig_ci/run_brownie.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.4.6/multisig_ci/safes.py` & `multisig_ci-0.4.7/multisig_ci/safes.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.4.6/multisig_ci/sign.py` & `multisig_ci-0.4.7/multisig_ci/sign.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.4.6/multisig_ci/telegram.py` & `multisig_ci-0.4.7/multisig_ci/telegram.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,10 +56,10 @@
     if not ok:
         raise Exception("failed to pin")
 
 if __name__ == '__main__':
     if len(sys.argv) > 1 and sys.argv[1] == 'send_and_pin_message':
         try:
             send_and_pin_message(sys.argv[2], sys.argv[3], os.getenv("TELEGRAM_MESSAGE"))
-            exit(0)
         except:
-            exit(1)
+            exit(1)
+        exit(0)
```

### Comparing `multisig_ci-0.4.6/multisig_ci/test_telegram.sh` & `multisig_ci-0.4.7/multisig_ci/test_telegram.sh`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.4.6/PKG-INFO` & `multisig_ci-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multisig-ci
-Version: 0.4.6
+Version: 0.4.7
 Summary: Gnosis safe ci scripts.
 License: AGPLv3
 Author: kx9x
 Author-email: kx9x@protonmail.com
 Requires-Python: >=3.8,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

