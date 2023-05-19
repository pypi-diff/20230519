# Comparing `tmp/quorum_fullnode_py-1.2.0.tar.gz` & `tmp/quorum_fullnode_py-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quorum_fullnode_py-1.2.0.tar", last modified: Thu Apr  6 03:59:40 2023, max compression
+gzip compressed data, was "quorum_fullnode_py-1.3.0.tar", last modified: Fri May 19 12:27:53 2023, max compression
```

## Comparing `quorum_fullnode_py-1.2.0.tar` & `quorum_fullnode_py-1.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 03:59:40.473512 quorum_fullnode_py-1.2.0/
--rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:18.000000 quorum_fullnode_py-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     2522 2023-04-06 03:59:40.472516 quorum_fullnode_py-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1566 2023-04-03 04:33:04.000000 quorum_fullnode_py-1.2.0/README.md
--rw-rw-rw-   0        0        0      169 2023-02-23 03:21:16.000000 quorum_fullnode_py-1.2.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-06 03:59:40.407095 quorum_fullnode_py-1.2.0/quorum_fullnode_py/
--rw-rw-rw-   0        0        0      329 2023-04-06 03:57:27.000000 quorum_fullnode_py-1.2.0/quorum_fullnode_py/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 03:59:40.462542 quorum_fullnode_py-1.2.0/quorum_fullnode_py/api/
--rw-rw-rw-   0        0        0      164 2023-02-24 06:37:34.000000 quorum_fullnode_py-1.2.0/quorum_fullnode_py/api/__init__.py
--rw-rw-rw-   0        0        0     6061 2023-04-06 03:44:23.000000 quorum_fullnode_py-1.2.0/quorum_fullnode_py/api/base.py
--rw-rw-rw-   0        0        0    20338 2023-04-06 03:55:34.000000 quorum_fullnode_py-1.2.0/quorum_fullnode_py/api/fullnode.py
-drwxrwxrwx   0        0        0        0 2023-04-06 03:59:40.468527 quorum_fullnode_py-1.2.0/quorum_fullnode_py/client/
--rw-rw-rw-   0        0        0      114 2023-02-24 06:37:34.000000 quorum_fullnode_py-1.2.0/quorum_fullnode_py/client/__init__.py
--rw-rw-rw-   0        0        0     1460 2023-04-06 03:32:26.000000 quorum_fullnode_py-1.2.0/quorum_fullnode_py/client/_http.py
--rw-rw-rw-   0        0        0      871 2023-02-24 06:37:34.000000 quorum_fullnode_py-1.2.0/quorum_fullnode_py/client/fullnode.py
--rw-rw-rw-   0        0        0     1490 2023-02-24 06:37:34.000000 quorum_fullnode_py-1.2.0/quorum_fullnode_py/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-06 03:59:40.456560 quorum_fullnode_py-1.2.0/quorum_fullnode_py.egg-info/
--rw-rw-rw-   0        0        0     2522 2023-04-06 03:59:40.000000 quorum_fullnode_py-1.2.0/quorum_fullnode_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-04-06 03:59:40.000000 quorum_fullnode_py-1.2.0/quorum_fullnode_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 03:59:40.000000 quorum_fullnode_py-1.2.0/quorum_fullnode_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-06 03:59:40.000000 quorum_fullnode_py-1.2.0/quorum_fullnode_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-06 03:59:40.000000 quorum_fullnode_py-1.2.0/quorum_fullnode_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 03:59:40.473512 quorum_fullnode_py-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1306 2023-04-06 03:57:27.000000 quorum_fullnode_py-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-06 03:59:40.470521 quorum_fullnode_py-1.2.0/tests/
--rw-rw-rw-   0        0        0     2847 2023-03-27 06:09:37.000000 quorum_fullnode_py-1.2.0/tests/test_fullnode.py
+drwxrwxrwx   0        0        0        0 2023-05-19 12:27:53.627620 quorum_fullnode_py-1.3.0/
+-rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:18.000000 quorum_fullnode_py-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     2522 2023-05-19 12:27:53.606482 quorum_fullnode_py-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1566 2023-04-03 04:33:04.000000 quorum_fullnode_py-1.3.0/README.md
+-rw-rw-rw-   0        0        0      169 2023-02-23 03:21:16.000000 quorum_fullnode_py-1.3.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-19 12:27:53.572947 quorum_fullnode_py-1.3.0/quorum_fullnode_py/
+-rw-rw-rw-   0        0        0      329 2023-05-19 08:07:50.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 12:27:53.595146 quorum_fullnode_py-1.3.0/quorum_fullnode_py/api/
+-rw-rw-rw-   0        0        0      164 2023-02-24 06:37:34.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py/api/__init__.py
+-rw-rw-rw-   0        0        0     6762 2023-05-19 08:38:21.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py/api/base.py
+-rw-rw-rw-   0        0        0    23454 2023-05-19 08:49:31.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py/api/fullnode.py
+drwxrwxrwx   0        0        0        0 2023-05-19 12:27:53.601129 quorum_fullnode_py-1.3.0/quorum_fullnode_py/client/
+-rw-rw-rw-   0        0        0      114 2023-02-24 06:37:34.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py/client/__init__.py
+-rw-rw-rw-   0        0        0     1460 2023-04-06 03:32:26.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py/client/_http.py
+-rw-rw-rw-   0        0        0      871 2023-02-24 06:37:34.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py/client/fullnode.py
+-rw-rw-rw-   0        0        0     1490 2023-02-24 06:37:34.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-19 12:27:53.584914 quorum_fullnode_py-1.3.0/quorum_fullnode_py.egg-info/
+-rw-rw-rw-   0        0        0     2522 2023-05-19 12:27:53.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      549 2023-05-19 12:27:53.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 12:27:53.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-19 12:27:53.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-19 12:27:53.000000 quorum_fullnode_py-1.3.0/quorum_fullnode_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 12:27:53.627620 quorum_fullnode_py-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1306 2023-05-19 12:27:40.000000 quorum_fullnode_py-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 12:27:53.603124 quorum_fullnode_py-1.3.0/tests/
+-rw-rw-rw-   0        0        0     2847 2023-03-27 06:09:37.000000 quorum_fullnode_py-1.3.0/tests/test_fullnode.py
```

### Comparing `quorum_fullnode_py-1.2.0/LICENSE` & `quorum_fullnode_py-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quorum_fullnode_py-1.2.0/PKG-INFO` & `quorum_fullnode_py-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum_fullnode_py
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python SDK for FullNode of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_fullnode_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_fullnode_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_fullnode_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_fullnode_py-1.2.0/README.md` & `quorum_fullnode_py-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `quorum_fullnode_py-1.2.0/quorum_fullnode_py/api/base.py` & `quorum_fullnode_py-1.3.0/quorum_fullnode_py/api/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -142,18 +142,33 @@
 
     def _get_announced_users(self, group_id: str = None):
         return self._get(f"/api/v1/group/{group_id}/announced/users")
 
     def _get_announced_user(self, group_id: str = None, pubkey=None):
         return self._get(f"/api/v1/group/{group_id}/announced/user/{pubkey}")
 
-    def _get_producers(self, group_id: str = None):
-        return self._get(f"/api/v1/group/{group_id}/producers")
-
     def _get_announced_producers(self, group_id: str = None):
         return self._get(f"/api/v1/group/{group_id}/announced/producers")
 
     def _post_user(self, payload: dict = None):
         return self._post("/api/v1/group/user", payload)
 
-    def _post_producer(self, payload: dict = None):
-        return self._post("/api/v1/group/producer", payload)
+    def _get_consensus(self, group_id: str = None):
+        return self._get(f"/api/v1/group/{group_id}/consensus/")
+
+    def _get_consensus_req(self, group_id: str = None, req_id: str = None):
+        return self._get(f"/api/v1/group/{group_id}/consensus/proof/{req_id}")
+
+    def _get_consensus_last(self, group_id: str = None):
+        return self._get(f"/api/v1/group/{group_id}/consensus/proof/last")
+
+    def _get_consensus_history(self, group_id: str = None):
+        return self._get(f"/api/v1/group/{group_id}/consensus/proof/history")
+
+    def _get_consensus_current(self, group_id: str = None):
+        return self._get(f"/api/v1/group/{group_id}/consensus/proof/current")
+
+    def _update_consensus(self, payload: dict = None):
+        return self._post("/api/v1/group/updconsensus", payload)
+
+    def _update_user(self, payload: dict = None):
+        return self._post("/api/v1/group/upduser", payload)
```

### Comparing `quorum_fullnode_py-1.2.0/quorum_fullnode_py/api/fullnode.py` & `quorum_fullnode_py-1.3.0/quorum_fullnode_py/api/fullnode.py`

 * *Files 10% similar despite different names*

```diff
@@ -101,16 +101,18 @@
     def create_token(
         self,
         role: str = None,
         name: str = None,
         group_id: str = None,
         expires_at: str = None,
     ):
-        """Create a new auth token, only allow access from localhost
-        expires_at: ISO time 2027-04-28T08:10:36.675204+00:00"""
+        """
+        Create a new auth token, only allow access from localhost
+        expires_at: ISO time 2027-04-28T08:10:36.675204+00:00
+        """
 
         role = role or "node"
         if role not in ("node", "chain"):
             raise ParamValueError("role must be one of ['node','chain']")
         if role == "chain":
             group_id = None
             name = name or "allow-chain"
@@ -124,27 +126,32 @@
             "role": role,
             "group_id": group_id,
             "expires_at": expires_at,
         }
         return super()._create_token(payload)
 
     def refresh_token(self):
-        """refresh auth token.
-        For example, when the token is about to expire, they can use this interface to obtain a new token.
+        """
+        refresh auth token.
+        For example, when the token is about to expire,
+        they can use this interface to obtain a new token.
         """
         return super()._refresh_token()
 
     def list_token(self):
         """list all jwt tokens"""
         return super()._get_token_list()
 
     def revoke_token(
         self, token: str = None, role: str = None, group_id: str = None
     ):
-        """to revoke a usable token and make it unusable, then add it to the "revoke list" in the config file."""
+        """
+        to revoke a usable token and make it unusable,
+        then add it to the "revoke list" in the config file.
+        """
         role = role or "node"
         if role not in ("node", "chain"):
             raise ParamValueError("role must be one of ['node','chain']")
         if role == "chain":
             group_id = None
         else:
             group_id = self._check_group_id_as_required(group_id)
@@ -475,40 +482,40 @@
             memo="remove deny list",
             action="remove",
             trx_types=trx_types,
             group_id=group_id,
         )
 
     def producers(self, group_id: str = None):
-        """get the producers of the group"""
-        group_id = self._check_group_id_as_required(group_id)
-        return super()._get_producers(group_id)
+        """get the producers pubkey list of the group"""
+        bps = self.get_consensus(group_id).get("producers", [])
+        return [bp["ProducerPubkey"] for bp in bps]
 
     def get_announced_producers(self, group_id: str = None):
         """get the announced producers to be approved"""
         group_id = self._check_group_id_as_required(group_id)
         return super()._get_announced_producers(group_id)
 
     def add_producer(self, pubkeys: list, group_id: str = None):
         """add pubkey as group producer to the group"""
         payload = {
             "producer_pubkey": pubkeys,
             "group_id": group_id,
             "action": "add",
         }
-        return super()._post_producer(payload)
+        return super()._update_consensus(payload)
 
     def remove_producer(self, pubkeys: list, group_id: str = None):
         """remove pubkey as group producer from the group"""
         payload = {
             "producer_pubkey": pubkeys,
             "group_id": group_id,
             "action": "remove",
         }
-        return super()._post_producer(payload)
+        return super()._update_consensus(payload)
 
     def announce_as_producer(self, group_id: str = None, memo: str = None):
         """announce fullnode self as producer"""
         group_id = self._check_group_id_as_required(group_id)
         payload = {
             "group_id": group_id,
             "action": "add",
@@ -526,14 +533,83 @@
             "group_id": group_id,
             "action": "remove",
             "type": "producer",
             "memo": memo or "announce self as producer to remove",
         }
         return super()._announce(payload)
 
+    def get_consensus(self, group_id: str = None):
+        group_id = self._check_group_id_as_required(group_id)
+        return super()._get_consensus(group_id)
+
+    def get_consensus_req(self, req_id: str, group_id: str = None):
+        group_id = self._check_group_id_as_required(group_id)
+        return super()._get_consensus_req(group_id, req_id)
+
+    def get_consensus_last(self, group_id: str = None):
+        group_id = self._check_group_id_as_required(group_id)
+        return super()._get_consensus_last(group_id)
+
+    def get_consensus_history(self, group_id: str = None):
+        group_id = self._check_group_id_as_required(group_id)
+        return super()._get_consensus_history(group_id)
+
+    def get_consensus_current(self, group_id: str = None):
+        group_id = self._check_group_id_as_required(group_id)
+        return super()._get_consensus_current(group_id)
+
+    def update_consensus(
+        self,
+        start_from_epoch: int,
+        trx_epoch_tick: int = None,
+        agreement_tick_length: int = None,
+        agreement_tick_count=None,
+        producer_pubkey: list = None,
+        group_id: str = None,
+    ):
+        group_id = self._check_group_id_as_required(group_id)
+        req_id = self.get_consensus(group_id).get("proof_req_id")
+        req = self.get_consensus_req(req_id, group_id).get("resps")[0]["Req"]
+
+        if trx_epoch_tick and trx_epoch_tick < 500:
+            raise ValueError("trx_epoch_tick should be greater than 500(ms)")
+        if agreement_tick_length and agreement_tick_length < 1000:
+            raise ValueError(
+                "agreement_tick_length should be greater than 1000(ms)"
+            )
+        if agreement_tick_count and agreement_tick_count < 10:
+            raise ValueError("agreement_tick_count should be greater than 10")
+
+        _exist = {
+            "group_id": group_id,
+            "start_from_epoch": req.get("StartFromEpoch") or 1,
+            "trx_epoch_tick": req.get("TrxEpochTickLenInMs") or 500,
+            "agreement_tick_Length": req.get("AgreementTickLenInMs") or 1000,
+            "agreement_tick_count": req.get("AgreementTickCount") or 10,
+            "producer_pubkey": req.get("ProducerPubkeyList") or [],
+        }
+
+        payload = {
+            "group_id": group_id,
+            "start_from_epoch": start_from_epoch or _exist["start_from_epoch"],
+            "trx_epoch_tick": trx_epoch_tick or _exist["trx_epoch_tick"],
+            "agreement_tick_Length": agreement_tick_length
+            or _exist["agreement_tick_Length"],
+            "agreement_tick_count": agreement_tick_count
+            or _exist["agreement_tick_count"],
+            "producer_pubkey": producer_pubkey or _exist["producer_pubkey"],
+        }
+
+        if payload == _exist:
+            return {"message": "Nothing to update"}
+        return super()._update_consensus(payload)
+
+    def update_user(self, payload: dict = None):
+        return super()._update_user(payload)
+
     def get_announced_users(self, group_id: str = None):
         """get the announced users to approve(add or remove)"""
         group_id = self._check_group_id_as_required(group_id)
         return super()._get_announced_users(group_id)
 
     def get_announced_user(self, pubkey: str, group_id: str = None):
         """check the user is announced or not"""
```

### Comparing `quorum_fullnode_py-1.2.0/quorum_fullnode_py/client/_http.py` & `quorum_fullnode_py-1.3.0/quorum_fullnode_py/client/_http.py`

 * *Files identical despite different names*

### Comparing `quorum_fullnode_py-1.2.0/quorum_fullnode_py/client/fullnode.py` & `quorum_fullnode_py-1.3.0/quorum_fullnode_py/client/fullnode.py`

 * *Files identical despite different names*

### Comparing `quorum_fullnode_py-1.2.0/quorum_fullnode_py/exceptions.py` & `quorum_fullnode_py-1.3.0/quorum_fullnode_py/exceptions.py`

 * *Files identical despite different names*

### Comparing `quorum_fullnode_py-1.2.0/quorum_fullnode_py.egg-info/PKG-INFO` & `quorum_fullnode_py-1.3.0/quorum_fullnode_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum-fullnode-py
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python SDK for FullNode of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_fullnode_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_fullnode_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_fullnode_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_fullnode_py-1.2.0/quorum_fullnode_py.egg-info/SOURCES.txt` & `quorum_fullnode_py-1.3.0/quorum_fullnode_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quorum_fullnode_py-1.2.0/setup.py` & `quorum_fullnode_py-1.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quorum_fullnode_py",
-    version="1.2.0",
+    version="1.3.0",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="Python SDK for FullNode of QuoRum",
     keywords=["quorum_fullnode_py", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/quorum_fullnode_py",
```

### Comparing `quorum_fullnode_py-1.2.0/tests/test_fullnode.py` & `quorum_fullnode_py-1.3.0/tests/test_fullnode.py`

 * *Files identical despite different names*

