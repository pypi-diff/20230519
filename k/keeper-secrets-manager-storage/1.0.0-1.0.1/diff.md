# Comparing `tmp/keeper-secrets-manager-storage-1.0.0.tar.gz` & `tmp/keeper-secrets-manager-storage-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keeper-secrets-manager-storage-1.0.0.tar", last modified: Tue Sep 27 23:38:57 2022, max compression
+gzip compressed data, was "keeper-secrets-manager-storage-1.0.1.tar", last modified: Fri May 19 06:15:19 2023, max compression
```

## Comparing `keeper-secrets-manager-storage-1.0.0.tar` & `keeper-secrets-manager-storage-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 23:38:57.203555 keeper-secrets-manager-storage-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-27 23:38:46.000000 keeper-secrets-manager-storage-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1571 2022-09-27 23:38:57.203555 keeper-secrets-manager-storage-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-27 23:38:46.000000 keeper-secrets-manager-storage-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 23:38:57.203555 keeper-secrets-manager-storage-1.0.0/keeper_secrets_manager_hsm/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-27 23:38:46.000000 keeper-secrets-manager-storage-1.0.0/keeper_secrets_manager_hsm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11593 2022-09-27 23:38:46.000000 keeper-secrets-manager-storage-1.0.0/keeper_secrets_manager_hsm/storage_aws_kms.py
--rw-r--r--   0 runner    (1001) docker     (121)    16365 2022-09-27 23:38:46.000000 keeper-secrets-manager-storage-1.0.0/keeper_secrets_manager_hsm/storage_hsm_nfast.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 23:38:57.203555 keeper-secrets-manager-storage-1.0.0/keeper_secrets_manager_storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1571 2022-09-27 23:38:57.000000 keeper-secrets-manager-storage-1.0.0/keeper_secrets_manager_storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      491 2022-09-27 23:38:57.000000 keeper-secrets-manager-storage-1.0.0/keeper_secrets_manager_storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 23:38:57.000000 keeper-secrets-manager-storage-1.0.0/keeper_secrets_manager_storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 23:38:56.000000 keeper-secrets-manager-storage-1.0.0/keeper_secrets_manager_storage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-09-27 23:38:57.000000 keeper-secrets-manager-storage-1.0.0/keeper_secrets_manager_storage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-09-27 23:38:57.000000 keeper-secrets-manager-storage-1.0.0/keeper_secrets_manager_storage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-09-27 23:38:57.203555 keeper-secrets-manager-storage-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1805 2022-09-27 23:38:46.000000 keeper-secrets-manager-storage-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:15:19.124084 keeper-secrets-manager-storage-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:15:07.000000 keeper-secrets-manager-storage-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-19 06:15:19.124084 keeper-secrets-manager-storage-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-19 06:15:07.000000 keeper-secrets-manager-storage-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:15:19.124084 keeper-secrets-manager-storage-1.0.1/keeper_secrets_manager_hsm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:15:07.000000 keeper-secrets-manager-storage-1.0.1/keeper_secrets_manager_hsm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11593 2023-05-19 06:15:07.000000 keeper-secrets-manager-storage-1.0.1/keeper_secrets_manager_hsm/storage_aws_kms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-05-19 06:15:07.000000 keeper-secrets-manager-storage-1.0.1/keeper_secrets_manager_hsm/storage_hsm_nfast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:15:19.124084 keeper-secrets-manager-storage-1.0.1/keeper_secrets_manager_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:15:07.000000 keeper-secrets-manager-storage-1.0.1/keeper_secrets_manager_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-19 06:15:07.000000 keeper-secrets-manager-storage-1.0.1/keeper_secrets_manager_storage/config_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21758 2023-05-19 06:15:07.000000 keeper-secrets-manager-storage-1.0.1/keeper_secrets_manager_storage/storage_aws_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-05-19 06:15:07.000000 keeper-secrets-manager-storage-1.0.1/keeper_secrets_manager_storage/storage_azure_keyvault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:15:19.124084 keeper-secrets-manager-storage-1.0.1/keeper_secrets_manager_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-19 06:15:19.000000 keeper-secrets-manager-storage-1.0.1/keeper_secrets_manager_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-19 06:15:19.000000 keeper-secrets-manager-storage-1.0.1/keeper_secrets_manager_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 06:15:19.000000 keeper-secrets-manager-storage-1.0.1/keeper_secrets_manager_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 06:15:18.000000 keeper-secrets-manager-storage-1.0.1/keeper_secrets_manager_storage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-19 06:15:19.000000 keeper-secrets-manager-storage-1.0.1/keeper_secrets_manager_storage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-19 06:15:19.000000 keeper-secrets-manager-storage-1.0.1/keeper_secrets_manager_storage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-19 06:15:19.124084 keeper-secrets-manager-storage-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-19 06:15:07.000000 keeper-secrets-manager-storage-1.0.1/setup.py
```

### Comparing `keeper-secrets-manager-storage-1.0.0/PKG-INFO` & `keeper-secrets-manager-storage-1.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keeper-secrets-manager-storage
-Version: 1.0.0
+Version: 1.0.1
 Summary: Keeper Secrets Manager SDK helper for managing configurations key-value storage.
 Home-page: https://github.com/Keeper-Security/secrets-manager
 Author: Keeper Security
 Author-email: sm@keepersecurity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Keeper-Security/secrets-manager/issues
 Project-URL: Documentation, https://docs.keeper.io/secrets-manager/secrets-manager/overview
@@ -29,9 +29,13 @@
 
 The Keeper Secrets Manager Storage module for working with custom key-value storages, creating and managing configuration files. To be used with keeper-secrets-manager-core.
 
 For more information see our official documentation page https://docs.keeper.io/secrets-manager/secrets-manager
 
 # Change Log
 
+## 1.0.1
+
+- Added new storage type storage type for AWS Secrets Manager
+
 ## 1.0.0
 - Initial release
```

### Comparing `keeper-secrets-manager-storage-1.0.0/keeper_secrets_manager_hsm/storage_aws_kms.py` & `keeper-secrets-manager-storage-1.0.1/keeper_secrets_manager_hsm/storage_aws_kms.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # | |/ /___ ___ _ __  ___ _ _ (R)
 # | ' </ -_) -_) '_ \/ -_) '_|
 # |_|\_\___\___| .__/\___|_|
 #              |_|
 #
 # Keeper Secrets Manager
 # Copyright 2022 Keeper Security Inc.
-# Contact: ops@keepersecurity.com
+# Contact: sm@keepersecurity.com
 import errno
 import hashlib
 import json
 import logging
 import os
 
 from json import JSONDecodeError
@@ -19,14 +19,15 @@
 
 from keeper_secrets_manager_core.storage import KeyValueStorage
 from keeper_secrets_manager_core.configkeys import ConfigKeys
 from keeper_secrets_manager_core.keeper_globals import logger_name
 from keeper_secrets_manager_core.utils import ENCODING
 
 logger = logging.getLogger(logger_name)
+
 try:
     import boto3
     from botocore.exceptions import ClientError
 except ImportError as ie:
     logger.error("Missing AWS SDK import dependencies."
         " To install missing packages run: \r\n"
         "pip3 install boto3\r\n")
```

### Comparing `keeper-secrets-manager-storage-1.0.0/keeper_secrets_manager_hsm/storage_hsm_nfast.py` & `keeper-secrets-manager-storage-1.0.1/keeper_secrets_manager_hsm/storage_hsm_nfast.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # | |/ /___ ___ _ __  ___ _ _ (R)
 # | ' </ -_) -_) '_ \/ -_) '_|
 # |_|\_\___\___| .__/\___|_|
 #              |_|
 #
 # Keeper Secrets Manager
 # Copyright 2022 Keeper Security Inc.
-# Contact: ops@keepersecurity.com
+# Contact: sm@keepersecurity.com
 
 # Requires: Entrust nShield SDK (nCore API)
 # Prerequisites: x86_64 Windows or Linux, nShield Security World 12.80 or later, user permissions to access kmdata files
 # Supported Python version: Python 3.8.5 (part of Entrust nShield SDK)
 # To use nShield Python 3 support with another version of Python 3, contact Entrust Support.
 # Usage:
 # /opt/nfast/python3/bin/python3 -m venv --copies venv
```

### Comparing `keeper-secrets-manager-storage-1.0.0/keeper_secrets_manager_storage.egg-info/PKG-INFO` & `keeper-secrets-manager-storage-1.0.1/keeper_secrets_manager_storage.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keeper-secrets-manager-storage
-Version: 1.0.0
+Version: 1.0.1
 Summary: Keeper Secrets Manager SDK helper for managing configurations key-value storage.
 Home-page: https://github.com/Keeper-Security/secrets-manager
 Author: Keeper Security
 Author-email: sm@keepersecurity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Keeper-Security/secrets-manager/issues
 Project-URL: Documentation, https://docs.keeper.io/secrets-manager/secrets-manager/overview
@@ -29,9 +29,13 @@
 
 The Keeper Secrets Manager Storage module for working with custom key-value storages, creating and managing configuration files. To be used with keeper-secrets-manager-core.
 
 For more information see our official documentation page https://docs.keeper.io/secrets-manager/secrets-manager
 
 # Change Log
 
+## 1.0.1
+
+- Added new storage type storage type for AWS Secrets Manager
+
 ## 1.0.0
 - Initial release
```

### Comparing `keeper-secrets-manager-storage-1.0.0/setup.py` & `keeper-secrets-manager-storage-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 install_requires = [
     'keeper-secrets-manager-core>=16.3.5'
 ]
 
 setup(
     name="keeper-secrets-manager-storage",
-    version="1.0.0",
+    version="1.0.1",
     description="Keeper Secrets Manager SDK helper for managing configurations key-value storage.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Keeper Security",
     author_email="sm@keepersecurity.com",
     url="https://github.com/Keeper-Security/secrets-manager",
     license="MIT",
```

