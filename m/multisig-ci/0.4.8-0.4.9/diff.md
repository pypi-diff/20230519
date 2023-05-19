# Comparing `tmp/multisig_ci-0.4.8.tar.gz` & `tmp/multisig_ci-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multisig_ci-0.4.8.tar", max compression
+gzip compressed data, was "multisig_ci-0.4.9.tar", max compression
```

## Comparing `multisig_ci-0.4.8.tar` & `multisig_ci-0.4.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    34523 2023-05-19 01:15:04.995578 multisig_ci-0.4.8/LICENSE
--rw-r--r--   0        0        0        0 2023-05-19 01:15:04.995578 multisig_ci-0.4.8/multisig_ci/__init__.py
--rw-r--r--   0        0        0      570 2023-05-19 01:15:04.995578 multisig_ci-0.4.8/multisig_ci/__main__.py
--rw-r--r--   0        0        0     7536 2023-05-19 01:15:04.995578 multisig_ci-0.4.8/multisig_ci/ci_override.py
--rw-r--r--   0        0        0     5811 2023-05-19 01:15:04.995578 multisig_ci-0.4.8/multisig_ci/hydrate_ci_cache.py
--rw-r--r--   0        0        0     2033 2023-05-19 01:15:04.995578 multisig_ci-0.4.8/multisig_ci/run_brownie.py
--rw-r--r--   0        0        0      811 2023-05-19 01:15:04.995578 multisig_ci-0.4.8/multisig_ci/safes.py
--rw-r--r--   0        0        0     1492 2023-05-19 01:15:04.995578 multisig_ci-0.4.8/multisig_ci/sign.py
--rw-r--r--   0        0        0     1913 2023-05-19 01:15:04.995578 multisig_ci-0.4.8/multisig_ci/telegram.py
--rwxr-xr-x   0        0        0      651 2023-05-19 01:15:04.995578 multisig_ci-0.4.8/multisig_ci/test_telegram.sh
--rw-r--r--   0        0        0      492 2023-05-19 01:15:04.995578 multisig_ci-0.4.8/pyproject.toml
--rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 multisig_ci-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-19 17:25:06.644107 multisig_ci-0.4.9/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-19 17:25:06.644107 multisig_ci-0.4.9/multisig_ci/__init__.py
+-rw-r--r--   0        0        0      570 2023-05-19 17:25:06.644107 multisig_ci-0.4.9/multisig_ci/__main__.py
+-rw-r--r--   0        0        0     7536 2023-05-19 17:25:06.644107 multisig_ci-0.4.9/multisig_ci/ci_override.py
+-rw-r--r--   0        0        0     5811 2023-05-19 17:25:06.644107 multisig_ci-0.4.9/multisig_ci/hydrate_ci_cache.py
+-rw-r--r--   0        0        0     2033 2023-05-19 17:25:06.644107 multisig_ci-0.4.9/multisig_ci/run_brownie.py
+-rw-r--r--   0        0        0      811 2023-05-19 17:25:06.644107 multisig_ci-0.4.9/multisig_ci/safes.py
+-rw-r--r--   0        0        0     1580 2023-05-19 17:25:06.644107 multisig_ci-0.4.9/multisig_ci/sign.py
+-rw-r--r--   0        0        0     1913 2023-05-19 17:25:06.644107 multisig_ci-0.4.9/multisig_ci/telegram.py
+-rwxr-xr-x   0        0        0      651 2023-05-19 17:25:06.644107 multisig_ci-0.4.9/multisig_ci/test_telegram.sh
+-rw-r--r--   0        0        0      492 2023-05-19 17:25:06.648108 multisig_ci-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 multisig_ci-0.4.9/PKG-INFO
```

### Comparing `multisig_ci-0.4.8/LICENSE` & `multisig_ci-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.4.8/multisig_ci/__main__.py` & `multisig_ci-0.4.9/multisig_ci/__main__.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.4.8/multisig_ci/ci_override.py` & `multisig_ci-0.4.9/multisig_ci/ci_override.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.4.8/multisig_ci/hydrate_ci_cache.py` & `multisig_ci-0.4.9/multisig_ci/hydrate_ci_cache.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.4.8/multisig_ci/run_brownie.py` & `multisig_ci-0.4.9/multisig_ci/run_brownie.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.4.8/multisig_ci/safes.py` & `multisig_ci-0.4.9/multisig_ci/safes.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.4.8/multisig_ci/sign.py` & `multisig_ci-0.4.9/multisig_ci/sign.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from multisig_ci.safes import safe
 
-def _tenderly_fork(safe):
+
+def _tenderly_fork(safe, timeout_seconds):
    import requests
    import brownie
    from brownie import chain
 
    fork_base_url = "https://simulate.yearn.network/fork"
    payload = {"network_id": str(chain.id)}
    resp = requests.post(fork_base_url, headers={}, json=payload)
    fork_id = resp.json()["simulation_fork"]["id"]
    fork_rpc_url = f"https://rpc.tenderly.co/fork/{fork_id}"
    print(fork_rpc_url)
-   tenderly_provider = brownie.web3.HTTPProvider(fork_rpc_url, {"timeout": 600})
+   tenderly_provider = brownie.web3.HTTPProvider(fork_rpc_url, {"timeout": timeout_seconds})
    brownie.web3.provider = tenderly_provider
    safe.w3.provider = tenderly_provider
    print(f"https://dashboard.tenderly.co/yearn/yearn-web/fork/{fork_id}")
 
-def sign(nonce_arg = None, skip_preview = False, post_tx = False, tenderly_fork = False):
+
+def sign(nonce_arg = None, skip_preview = False, post_tx = False, tenderly_fork = False, tenderly_timeout_seconds = 60):
     def _sign(func):
         def wrapper():
             if tenderly_fork:
-                _tenderly_fork(safe)
+                _tenderly_fork(safe, tenderly_timeout_seconds)
             func()
             safe_tx = safe.multisend_from_receipts(safe_nonce=nonce)
             if not skip_preview:
                 safe.preview(safe_tx, call_trace=False)
 
             if not post_tx and not safe.is_ci:
                 print("dry-run finished, run again with @sign(post_tx = True) to sign and submit the tx.")
```

### Comparing `multisig_ci-0.4.8/multisig_ci/telegram.py` & `multisig_ci-0.4.9/multisig_ci/telegram.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.4.8/multisig_ci/test_telegram.sh` & `multisig_ci-0.4.9/multisig_ci/test_telegram.sh`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.4.8/PKG-INFO` & `multisig_ci-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multisig-ci
-Version: 0.4.8
+Version: 0.4.9
 Summary: Gnosis safe ci scripts.
 License: AGPLv3
 Author: kx9x
 Author-email: kx9x@protonmail.com
 Requires-Python: >=3.8,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

