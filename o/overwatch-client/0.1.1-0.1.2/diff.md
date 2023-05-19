# Comparing `tmp/overwatch_client-0.1.1.tar.gz` & `tmp/overwatch_client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overwatch_client-0.1.1.tar", max compression
+gzip compressed data, was "overwatch_client-0.1.2.tar", max compression
```

## Comparing `overwatch_client-0.1.1.tar` & `overwatch_client-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      289 2023-05-02 14:37:02.200028 overwatch_client-0.1.1/README.md
--rw-r--r--   0        0        0       32 2023-05-02 14:37:02.200028 overwatch_client-0.1.1/overwatch_client/__init__.py
--rw-r--r--   0        0        0     6908 2023-05-02 14:37:02.200028 overwatch_client-0.1.1/overwatch_client/client.py
--rw-r--r--   0        0        0      179 2023-05-02 14:37:02.200028 overwatch_client-0.1.1/overwatch_client/utils.py
--rw-r--r--   0        0        0     1016 2023-05-09 15:19:38.633779 overwatch_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 overwatch_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1209 2023-05-19 13:50:48.938301 overwatch_client-0.1.2/README.md
+-rw-r--r--   0        0        0       32 2023-05-19 13:50:48.938301 overwatch_client-0.1.2/overwatch_client/__init__.py
+-rw-r--r--   0        0        0    10311 2023-05-19 13:50:48.938301 overwatch_client-0.1.2/overwatch_client/client.py
+-rw-r--r--   0        0        0      378 2023-05-19 13:50:48.938301 overwatch_client-0.1.2/overwatch_client/utils.py
+-rw-r--r--   0        0        0     1044 2023-05-19 13:50:48.942301 overwatch_client-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1713 1970-01-01 00:00:00.000000 overwatch_client-0.1.2/PKG-INFO
```

### Comparing `overwatch_client-0.1.1/overwatch_client/client.py` & `overwatch_client-0.1.2/overwatch_client/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,101 +2,183 @@
 import requests
 import time
 from typing import Optional, Sequence, Dict
 from .utils import generate_uuid
 
 
 class HTTPClient:
+    """The base client for communicating with an overwatch server and it's model registry.
+
+    The client is used to register, patch, delete and infer on models with the overwatch server.
+
+    Attributes:
+        ow_server_url (str): The url of the overwatch server.
+        model_registry_url (str): The url of the model registry.
+        header_payload (Dict[str, str]): The headers for the request.
+        inference_timer (List[float]): A list of inference times.
+        inference_counter (List[int]): A list of inference counts (number of inputs per inference call).
+    """
+
+
     def __init__(
         self,
         overwatch_server_url: str = "https://overwatch.distributive.network",
         model_registry_url: str = "https://models.overwatch.distributive.network",
         header_key: str = "ovwatch-secret-key",
     ):
+        """
+        Initializes the client with the overwatch server url and model registry url.
+
+        Args:
+            overwatch_server_url (str): The url of the overwatch server.
+            model_registry_url (str): The url of the model registry.
+            header_key (str): The header key for the request.
+        """
         self.ow_server_url = overwatch_server_url
         self.model_registry_url = model_registry_url
         self.header_payload = {"key": header_key}
         self.inference_timer = []
         self.inference_counter = []
 
     def check_overwatch_server_connection(self) -> bool:
+        """
+        Checks if the Overwatch server is reachable.
+
+        Returns:
+            Bool: True if the Overwatch server is reachable.
+        """
         try:
             response = requests.get(f"{self.ow_server_url}/status", headers=self.header_payload)
             response.raise_for_status()
             return True
         except requests.exceptions.ConnectionError:
             return False
 
     def __get_file__(self, file_path: str) -> bytes:
         """
         Retrieves the contents of a file from disk and returns it as bytes. 
 
-        :param file_path: The path to the file. 
-        :return: The contents of the file as bytes.
+        Args:
+            file_path (str): The path to the file.
+
+        Returns:
+            bytes: The contents of the file as bytes.
         """
         with open(file_path, "rb") as f:
             ret_bytes: bytes = f.read()
         return ret_bytes
 
-    def register_model(
+    def register_model_with_bytes(
         self,
         model_name: str,
-        model_path: str,
-        preprocess_path: str,
-        postprocess_path: str,
+        model_bytes: bytes,
+        preprocess_bytes: bytes,
+        postprocess_bytes: bytes,
         password: str = "DefaultPassword",
         language: Optional[str] = None,
         packages: Optional[Sequence[str]] = None,
     ) -> requests.Response:
+        """
+        Registers a new model with the model registry. Will throw if the model already exists.
+
+        Args:
+            model_name (str): The name of the model to register.
+            model_bytes (bytes): The bytes of the model.
+            preprocess_bytes (bytes): The bytes of the preprocess file for this model.
+            postprocess_bytes (bytes): The bytes of the postprocess file for this model.
+            password (str): The password for this model.
+            language (str): The language for this model. Can be either javascript or python.
+            packages (Sequence[str]): A list of packages required for this model.
+
+        Returns:
+            requests.Resposne: The response from the model registry.
+        """
+
         url = f"{self.model_registry_url}/models"
         data_payload = {
             "modelID": model_name,
             "password": password,
             "reqPackages": packages if packages is not None else [],
             "language": "javascript" if language is None else language,
         }
 
         files_payload = {
-            "model": self.__get_file__(model_path),
-            "preprocess": self.__get_file__(preprocess_path),
-            "postprocess": self.__get_file__(postprocess_path),
+            "model": model_bytes,
+            "preprocess": preprocess_bytes,
+            "postprocess": postprocess_bytes,
         }
 
         response = requests.post(
             url,
             headers=self.header_payload,
             data=data_payload,
             files=files_payload,
         )
+        return response 
 
-        response.raise_for_status()
+    def register_model(
+        self,
+        model_name: str,
+        model_path: str,
+        preprocess_path: str,
+        postprocess_path: str,
+        password: str = "DefaultPassword",
+        language: Optional[str] = None,
+        packages: Optional[Sequence[str]] = None,
+    ) -> requests.Response:
+        """
+        Registers a new model with the model registry. Will throw if the model already exists.
 
-        return response
+        Args:
+            model_name (str): The name of the model to register.
+            model_path (str): The path to the model.
+            preprocess_path (str): The path to the preprocess file for this model.
+            postprocess_path (str): The path to the postprocess file for this model.
+            password (str): The password for this model.
+            language (str): The language for this model. Can be either javascript or python.
+            packages (Sequence[str]): A list of packages required for this model.
+
+        Returns:
+            requests.Resposne: The response from the model registry.
+        """
+
+        return self.register_model_with_bytes(
+            model_name, 
+            self.__get_file__(model_path),
+            self.__get_file__(preprocess_path),
+            self.__get_file__(postprocess_path),
+            password,
+            language,
+            packages
+        )
 
     def patch_model(
         self,
         model_name: str,
         model_path: str,
         preprocess_path: str,
         postprocess_path: str,
         password: str = "DefaultPassword",
         language: Optional[str] = None,
         packages: Optional[Sequence[str]] = None,
     ) -> requests.Response:
         """
         Patches a specified model from the model registry with provided information.
 
-        :param model_name: The name of the model to patch.
-        :param model_path: The path to the model.
-        :param preprocess_path: The path to the preprocess file for this model.
-        :param postprocess_path: The path to the postprocess file for this model.
-        :param password: The password for this model.
-        :param language: The language for this model. Can be either javascript or python.
-        :param packages: A list of packages required for this model. 
-        :return: [TODO:description]
+        Args:
+            model_name(str): The name of the model to patch.
+            model_path(str): The path to the model.
+            preprocess_path(str): The path to the preprocess file for this model.
+            postprocess_path(str): The path to the postprocess file for this model.
+            password(str): The password for this model.
+            language(str): The language for this model. Can be either javascript or python.
+            packages(Sequence[str]): A list of packages required for this model.
+
+        Returns:
+            requests.Response: The response from the model registry.
         """
         url = f"{self.model_registry_url}/models/{model_name}"
         data_payload = {
             "modelID": model_name,
             "password": password,
             "reqPackages": packages if packages is not None else [],
             "language": "javascript" if language is None else language,
@@ -121,17 +203,20 @@
 
     def delete_model(
         self, model_name: str, password: str = "DefaultPassword"
     ) -> requests.Response:
         """
         Deletes the specified model from the model registry.
 
-        :param model_name: The name of the model to delete.
-        :param password: The associated password for the modelself.
-        :return: The response object from the model registry after deleting the model.
+        Args:
+            model_name (str): The name of the model to delete.
+            password (str): The associated password for the modelself.
+
+        Returns:
+            requests.Response: The response object from the model registry after deleting the model.
         """
         url = f"{self.model_registry_url}/models/{model_name}"
 
         header_payload = {
             "key": self.header_payload["key"],
             "password": password,
         }
@@ -144,17 +229,20 @@
         response.raise_for_status()
 
         return response
 
     def get_model(self, model_name: str) -> requests.Response:
         """
         Retrieves a model from the model registry.
+        
+        Args:
+            model_name (str): The name of the model to retrieve.
 
-        :param model_name: The model to retrieve.
-        :return: A response object containing the response from the model registry.
+        Returns:
+            requests.Response: The response object from the model registry.
         """
         url = f"{self.model_registry_url}/models/{model_name}"
 
         response = requests.get(url, headers=self.header_payload)
 
         response.raise_for_status()
 
@@ -168,20 +256,23 @@
         inference_id: Optional[str] = None,
         compute_group_info: Optional[str] = None,
     ) -> Dict:
         """
         Performs an inference on the provided inputs using the model specified. Returns 
         the inference results as a dictionary.
 
-        :param inputs: A list of inputs in byte format.
-        :param model_name: The model name we will be inferencing on.
-        :param slice_batch: The number of inputs per slice.
-        :param inference_id: A special ID for this inference instance.
-        :param compute_group_info: Compute group information in the form of "<joinKey>/<joinSecret>".
-        :return: The inference results as a dictionary.
+        Args:
+            inputs(Sequence[bytes]): A list of inputs in byte format.
+            model_name(str): The model name we will be inferencing on.
+            slice_batch(int): The number of inputs to run per slice.
+            inference_id(Optional[str]): A special ID for this inference instance (Optional).
+            compute_group_info(Optional[str]): Compute group information in the form of "<joinKey>/<joinSecret>".
+
+        Returns:
+            Dict: The inference results as a dictionary.
         """
         inference_id = (
             inference_id
             if inference_id is not None
             else f"{model_name}_{generate_uuid()}"
         )
         url = f"{self.ow_server_url}/Prediction/{inference_id}/detect/iterations/{model_name}/{slice_batch}"
```

### Comparing `overwatch_client-0.1.1/pyproject.toml` & `overwatch_client-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "overwatch-client"
-version = "0.1.1"
+version = "0.1.2"
 description = "A python based Overwatch Client for interacting with the overwatch server with higher level apis."
 authors = ["Hamada Gasmallah <hamada@distributive.network>"]
 readme = "README.md"
 packages = [{include = "overwatch_client"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -18,14 +18,15 @@
 
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^6.1.3"
 sphinxcontrib-napoleon = "^0.7"
 myst-parser = "^1.0.0"
 sphinx-markdown-builder = "^0.5.5"
+sphinx-rtd-theme = "^1.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.black]
```

