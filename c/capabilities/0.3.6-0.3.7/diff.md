# Comparing `tmp/capabilities-0.3.6.tar.gz` & `tmp/capabilities-0.3.7.tar.gz`

## Comparing `capabilities-0.3.6.tar` & `capabilities-0.3.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 capabilities-0.3.6/setup.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 capabilities-0.3.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/__about__.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/__main__.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/cli.py
--rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/config.py
--rw-r--r--   0        0        0    12246 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/core.py
--rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/dec.py
--rw-r--r--   0        0        0    15164 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/example.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/search/__init__.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/search/hf.py
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/search/loader.py
--rw-r--r--   0        0        0     6160 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/search/nomic_index.py
--rw-r--r--   0        0        0     6507 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/search/oai.py
--rw-r--r--   0        0        0    12504 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/search/search_index.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/search/simple_vector_index.py
--rw-r--r--   0        0        0     7150 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/search/types.py
--rw-r--r--   0        0        0     5375 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/search/util.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/util/__init__.py
--rw-r--r--   0        0        0     9199 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/util/config.py
--rw-r--r--   0        0        0     6705 2020-02-02 00:00:00.000000 capabilities-0.3.6/capabilities/util/misc.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 capabilities-0.3.6/examples/cheese.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 capabilities-0.3.6/examples/leansearch.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 capabilities-0.3.6/examples/readme.txt
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 capabilities-0.3.6/examples/tesla10k.py
--rw-r--r--   0        0        0   840980 2020-02-02 00:00:00.000000 capabilities-0.3.6/examples/data/apple10k.pdf
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 capabilities-0.3.6/examples/data/sample.md
--rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 capabilities-0.3.6/examples/data/sample.pdf
--rw-r--r--   0        0        0   157134 2020-02-02 00:00:00.000000 capabilities-0.3.6/examples/data/tesla10k.txt
--rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 capabilities-0.3.6/tests/test_docs.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 capabilities-0.3.6/tests/test_document_loader.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 capabilities-0.3.6/tests/test_search.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 capabilities-0.3.6/tests/test_search_util.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 capabilities-0.3.6/tests/test_tutorial1.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 capabilities-0.3.6/tests/test_vector_idx.py
--rw-r--r--   0        0        0   353564 2020-02-02 00:00:00.000000 capabilities-0.3.6/tests/snapshots/test_search/test_search_e2e/NomicIndex-openai/r0.txt
--rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.6/tests/snapshots/test_search/test_search_e2e/NomicIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
--rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.6/tests/snapshots/test_search/test_search_e2e/SearchIndex-openai/r0.txt
--rw-r--r--   0        0        0   353565 2020-02-02 00:00:00.000000 capabilities-0.3.6/tests/snapshots/test_search/test_search_e2e/SearchIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 capabilities-0.3.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 capabilities-0.3.6/LICENSE
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 capabilities-0.3.6/README.md
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 capabilities-0.3.6/pyproject.toml
--rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 capabilities-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 capabilities-0.3.7/setup.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 capabilities-0.3.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 capabilities-0.3.7/capabilities/__about__.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 capabilities-0.3.7/capabilities/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 capabilities-0.3.7/capabilities/__main__.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 capabilities-0.3.7/capabilities/cli.py
+-rw-r--r--   0        0        0     6200 2020-02-02 00:00:00.000000 capabilities-0.3.7/capabilities/config.py
+-rw-r--r--   0        0        0    12712 2020-02-02 00:00:00.000000 capabilities-0.3.7/capabilities/core.py
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 capabilities-0.3.7/capabilities/dec.py
+-rw-r--r--   0        0        0    15164 2020-02-02 00:00:00.000000 capabilities-0.3.7/capabilities/example.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 capabilities-0.3.7/capabilities/search/__init__.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 capabilities-0.3.7/capabilities/search/hf.py
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 capabilities-0.3.7/capabilities/search/loader.py
+-rw-r--r--   0        0        0     6160 2020-02-02 00:00:00.000000 capabilities-0.3.7/capabilities/search/nomic_index.py
+-rw-r--r--   0        0        0     7340 2020-02-02 00:00:00.000000 capabilities-0.3.7/capabilities/search/oai.py
+-rw-r--r--   0        0        0    12504 2020-02-02 00:00:00.000000 capabilities-0.3.7/capabilities/search/search_index.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 capabilities-0.3.7/capabilities/search/simple_vector_index.py
+-rw-r--r--   0        0        0     7150 2020-02-02 00:00:00.000000 capabilities-0.3.7/capabilities/search/types.py
+-rw-r--r--   0        0        0     5375 2020-02-02 00:00:00.000000 capabilities-0.3.7/capabilities/search/util.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 capabilities-0.3.7/capabilities/util/__init__.py
+-rw-r--r--   0        0        0     9199 2020-02-02 00:00:00.000000 capabilities-0.3.7/capabilities/util/config.py
+-rw-r--r--   0        0        0     6705 2020-02-02 00:00:00.000000 capabilities-0.3.7/capabilities/util/misc.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 capabilities-0.3.7/examples/cheese.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 capabilities-0.3.7/examples/leansearch.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 capabilities-0.3.7/examples/readme.txt
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 capabilities-0.3.7/examples/tesla10k.py
+-rw-r--r--   0        0        0   840980 2020-02-02 00:00:00.000000 capabilities-0.3.7/examples/data/apple10k.pdf
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 capabilities-0.3.7/examples/data/sample.md
+-rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 capabilities-0.3.7/examples/data/sample.pdf
+-rw-r--r--   0        0        0   157134 2020-02-02 00:00:00.000000 capabilities-0.3.7/examples/data/tesla10k.txt
+-rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 capabilities-0.3.7/tests/test_docs.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 capabilities-0.3.7/tests/test_document_loader.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 capabilities-0.3.7/tests/test_search.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 capabilities-0.3.7/tests/test_search_util.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 capabilities-0.3.7/tests/test_tutorial1.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 capabilities-0.3.7/tests/test_vector_idx.py
+-rw-r--r--   0        0        0   353564 2020-02-02 00:00:00.000000 capabilities-0.3.7/tests/snapshots/test_search/test_search_e2e/NomicIndex-openai/r0.txt
+-rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.7/tests/snapshots/test_search/test_search_e2e/NomicIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
+-rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.7/tests/snapshots/test_search/test_search_e2e/SearchIndex-openai/r0.txt
+-rw-r--r--   0        0        0   353565 2020-02-02 00:00:00.000000 capabilities-0.3.7/tests/snapshots/test_search/test_search_e2e/SearchIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 capabilities-0.3.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 capabilities-0.3.7/LICENSE
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 capabilities-0.3.7/README.md
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 capabilities-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 capabilities-0.3.7/PKG-INFO
```

### Comparing `capabilities-0.3.6/.github/workflows/python-publish.yml` & `capabilities-0.3.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/capabilities/cli.py` & `capabilities-0.3.7/capabilities/cli.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/capabilities/config.py` & `capabilities-0.3.7/capabilities/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,29 +9,39 @@
 from pathlib import Path
 import requests
 from rich import print
 import sys
 import logging
 from capabilities.util.config import SecretPersist, get_app_config_dir
 from capabilities.search.oai import CONFIG as OAI
+from capabilities.search.oai import AzureOpenAISettings
+
+AOAI = AzureOpenAISettings()
 
 logger = logging.getLogger(__name__)
 
-_FORWARD_WARNED = False
+_OPENAI_FORWARD_WARNED = False
+_AZURE_FORWARD_WARNED = False
 
 
 class Config(pydantic.BaseSettings, SecretPersist):
     api_key: Optional[pydantic.SecretStr] = pydantic.Field(default=None, is_secret=True)
     api_url: str = "https://api.blazon.ai"
     forward_openai: bool = False
     """ If this value is true, capabilities will forward your OPENAI_API_KEY to the capabilities API if it is present.
 
     This is useful if you want to use credits on your own OpenAI account or want to avoid rate limits.
     The capabilities server only knows this key for the duration of the API call. It is not stored.
     """
+    forward_azure: bool = False
+    """ If this value is true, capabilities will forward your AZURE_OPENAI_API_KEY to the capabilities API if it is present.
+
+    This is useful if you want to use credits on your own OpenAI account or want to avoid rate limits.
+    The capabilities server only knows this key for the duration of the API call. It is not stored.
+    """
 
     config_dir: Path = pydantic.Field(default_factory=lambda: get_app_config_dir("capabilities"))
 
     @property
     def secrets_file(self) -> Optional[Path]:
         if self.config_dir.exists():
             return self.config_dir / "secrets.json"
@@ -47,43 +57,52 @@
     def get_api_key(self) -> Optional[str]:
         api_key = self.get_secret("api_key")
         if api_key is None and not getattr(self, "_api_key_warned", False):
             print(
                 (
                     r" \[[red bold]warning[/]\] "
                     "CAPABILITIES_API_KEY not set, get one here: https://blazon.ai/signin"
+                    "then try `capabilities login ${paste_api_key_here}`"
                     "\n"
                 ),
                 file=sys.stderr,
             )
             self._api_key_warned = True
         assert isinstance(api_key, Optional[str])
         return api_key
 
     def get_headers(self) -> dict:
         k = self.get_api_key()
         if k is None:
-            raise ValueError("CAPABILITIES_API_KEY not set")
+            raise ValueError("CAPABILITIES_API_KEY not set, get one here: https://blazon.ai/signin")
         return {
             "Content-Type": "application/json",
             "api-key": self.get_api_key(),
         }
 
     def post_sync(self, endpoint, payload):
         patience = 8
         count = 0
         headers = self.get_headers()
         url = f"{self.api_url}{endpoint}"
         payload = dict(**payload)
+        if "clients" not in payload:
+            payload["clients"] = []
         if self.forward_openai and OAI.api_key is not None:
-            global _FORWARD_WARNED
-            if not _FORWARD_WARNED:
+            global _OPENAI_FORWARD_WARNED
+            if not _OPENAI_FORWARD_WARNED:
                 logger.warn("WARNING: forwarding OPENAI_API_KEY to capabilities API")
-                _FORWARD_WARNED = True
-            payload["clients"] = [{"api_key": OAI.api_key.get_secret_value()}]
+                _OPENAI_FORWARD_WARNED = True
+            payload["clients"] += [{"api_key": OAI.api_key.get_secret_value(), "api_url": OAI.api_url}]
+        if self.forward_azure and AOAI.api_key is not None:
+            global _AZURE_FORWARD_WARNED
+            if not _AZURE_FORWARD_WARNED:
+                logger.warn("WARNING: forwarding AZURE_OPENAI_API_KEY to capabilities API")
+                _AZURE_FORWARD_WARNED = True
+            payload["clients"] += [{"api_key": AOAI.api_key.get_secret_value(), "api_url": AOAI.api_url}]
         while True:
             try:
                 resp = requests.post(url, json=payload, headers=headers)
                 resp.raise_for_status()
                 return resp.json()
             except Exception as e:
                 if count >= patience:
@@ -96,16 +115,28 @@
 
     async def post_async(self, endpoint, payload):
         patience = 8
         count = 0
         headers = self.get_headers()
         url = f"{self.api_url}{endpoint}"
         payload = dict(**payload)
+        if "clients" not in payload:
+            payload["clients"] = []
         if self.forward_openai and OAI.api_key is not None:
-            payload["clients"] = [{"api_key": OAI.api_key.get_secret_value()}]
+            global _OPENAI_FORWARD_WARNED
+            if not _OPENAI_FORWARD_WARNED:
+                logger.warn("forwarding OPENAI_API_KEY to capabilities API")
+                _OPENAI_FORWARD_WARNED = True
+            payload["clients"] += [{"api_key": OAI.api_key.get_secret_value(), "api_url": OAI.api_url}]
+        if self.forward_azure and AOAI.api_key is not None:
+            global _AZURE_FORWARD_WARNED
+            if not _AZURE_FORWARD_WARNED:
+                logger.warn("forwarding AZURE_OPENAI_API_KEY to capabilities API")
+                _AZURE_FORWARD_WARNED = True
+            payload["clients"] += [{"api_key": AOAI.api_key.get_secret_value(), "api_url": AOAI.api_url}]
         while True:
             try:
                 async with aiohttp.ClientSession(
                     connector=aiohttp.TCPConnector(ssl=False)
                 ) as session:
                     async with session.post(url, json=payload, headers=headers) as resp:
                         resp.raise_for_status()
```

### Comparing `capabilities-0.3.6/capabilities/core.py` & `capabilities-0.3.7/capabilities/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,22 +45,36 @@
     _capability: Optional[CapabilityBase] = None
 
     def __call__(self, *args, **kwargs):
         print(
             colored("[  ✓  ]", "green"),
             f"Capability({self.uri}) running with {len(args) + len(kwargs)} arguments",
         )
-        return self._capability(*args, **kwargs)
+        try:
+            return self._capability(*args, **kwargs)
+        except Exception as e:
+            print(
+                colored("[  ✗  ]", "red"),
+                f"Encountered exception={e}\nRead the docs at https://docs.blazon.ai",
+            )
+            raise e
 
     async def run_async(self, *args, **kwargs):
         print(
             colored("[  ✓  ]", "green"),
             f"Capability({self.uri}) running async with {len(args) + len(kwargs)} arguments",
         )
-        return await self._capability.run_async(*args, **kwargs)
+        try:
+            return await self._capability.run_async(*args, **kwargs)
+        except Exception as e:
+            print(
+                colored("[  ✗  ]", "red"),
+                f"Encountered exception={e}\nRead the docs at https://docs.blazon.ai",
+            )
+            raise e
 
     def __post_init__(self):
         try:
             self._capability = _CAPABILITIES[self.uri]
         except KeyError as e:
             print(
                 colored("[  ✗  ]", "red"),
```

### Comparing `capabilities-0.3.6/capabilities/dec.py` & `capabilities-0.3.7/capabilities/dec.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/capabilities/example.py` & `capabilities-0.3.7/capabilities/example.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/capabilities/search/hf.py` & `capabilities-0.3.7/capabilities/search/hf.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/capabilities/search/loader.py` & `capabilities-0.3.7/capabilities/search/loader.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/capabilities/search/nomic_index.py` & `capabilities-0.3.7/capabilities/search/nomic_index.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/capabilities/search/oai.py` & `capabilities-0.3.7/capabilities/search/oai.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,39 @@
 from .types import EmbeddingModel
 from .util import argbatch, cache
 from rich.progress import track
 import requests
 
 """ A client for the OpenAI API. """
 
+class AzureOpenAISettings(BaseSettings):
+    api_key: Optional[SecretStr] = None
+    api_url: Optional[str] = None
+
+    class Config:
+        env_file = ".env"
+        env_file_encoding = "utf-8"
+        env_prefix = "AZURE_OPENAI_"
+
+    def create_headers(self):
+        if self.api_key is None:
+            raise ValueError(
+                "Azure OpenAI API key is not set. Either add it to the .env file or to your enviroment."
+            )
+        headers = {
+            "Content-Type": "application/json",
+            "Authorization": f"Bearer {self.api_key.get_secret_value()}",
+            "api-key": self.api_key.get_secret_value(),
+        }
+        return headers
+
+    def post(self, path: str, **kwargs):
+        url = f"{self.api_url}{path}"
+        return requests.post(url, headers=self.create_headers(), **kwargs)
+
 
 class OpenAISettings(BaseSettings):
     api_key: Optional[SecretStr] = None
     api_url: str = "https://api.openai.com"
 
     class Config:
         env_file = ".env"
```

### Comparing `capabilities-0.3.6/capabilities/search/search_index.py` & `capabilities-0.3.7/capabilities/search/search_index.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/capabilities/search/simple_vector_index.py` & `capabilities-0.3.7/capabilities/search/simple_vector_index.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/capabilities/search/types.py` & `capabilities-0.3.7/capabilities/search/types.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/capabilities/search/util.py` & `capabilities-0.3.7/capabilities/search/util.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/capabilities/util/config.py` & `capabilities-0.3.7/capabilities/util/config.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/capabilities/util/misc.py` & `capabilities-0.3.7/capabilities/util/misc.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/examples/cheese.py` & `capabilities-0.3.7/examples/cheese.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/examples/leansearch.py` & `capabilities-0.3.7/examples/leansearch.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/examples/tesla10k.py` & `capabilities-0.3.7/examples/tesla10k.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/examples/data/apple10k.pdf` & `capabilities-0.3.7/examples/data/apple10k.pdf`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/examples/data/sample.md` & `capabilities-0.3.7/examples/data/sample.md`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/examples/data/sample.pdf` & `capabilities-0.3.7/examples/data/sample.pdf`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/examples/data/tesla10k.txt` & `capabilities-0.3.7/examples/data/tesla10k.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/tests/test_docs.py` & `capabilities-0.3.7/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/tests/test_document_loader.py` & `capabilities-0.3.7/tests/test_document_loader.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/tests/test_search.py` & `capabilities-0.3.7/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/tests/test_search_util.py` & `capabilities-0.3.7/tests/test_search_util.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/tests/test_tutorial1.py` & `capabilities-0.3.7/tests/test_tutorial1.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/tests/test_vector_idx.py` & `capabilities-0.3.7/tests/test_vector_idx.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/tests/snapshots/test_search/test_search_e2e/NomicIndex-openai/r0.txt` & `capabilities-0.3.7/tests/snapshots/test_search/test_search_e2e/NomicIndex-openai/r0.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/tests/snapshots/test_search/test_search_e2e/NomicIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt` & `capabilities-0.3.7/tests/snapshots/test_search/test_search_e2e/NomicIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/tests/snapshots/test_search/test_search_e2e/SearchIndex-openai/r0.txt` & `capabilities-0.3.7/tests/snapshots/test_search/test_search_e2e/SearchIndex-openai/r0.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/tests/snapshots/test_search/test_search_e2e/SearchIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt` & `capabilities-0.3.7/tests/snapshots/test_search/test_search_e2e/SearchIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/.gitignore` & `capabilities-0.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/LICENSE` & `capabilities-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.6/pyproject.toml` & `capabilities-0.3.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "capabilities"
-# dynamic = ["version"]
-version="0.3.6"
+dynamic = ["version"]
+# version="0.3.6"
 authors = [
   { name="Blazon AI", email="support@blazon.ai" },
 ]
 description = "Build trusted, faster, and more powerful applications with the Blazon Capabilities API."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `capabilities-0.3.6/PKG-INFO` & `capabilities-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capabilities
-Version: 0.3.6
+Version: 0.3.7
 Summary: Build trusted, faster, and more powerful applications with the Blazon Capabilities API.
 Author-email: Blazon AI <support@blazon.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

