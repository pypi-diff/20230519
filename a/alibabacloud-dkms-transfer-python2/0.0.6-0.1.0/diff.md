# Comparing `tmp/alibabacloud-dkms-transfer-python2-0.0.6.tar.gz` & `tmp/alibabacloud-dkms-transfer-python2-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud-dkms-transfer-python2-0.0.6.tar", last modified: Wed Mar 15 05:40:00 2023, max compression
+gzip compressed data, was "dist/alibabacloud-dkms-transfer-python2-0.1.0.tar", last modified: Fri May 19 10:43:35 2023, max compression
```

## Comparing `alibabacloud-dkms-transfer-python2-0.0.6.tar` & `alibabacloud-dkms-transfer-python2-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 05:40:00.000000 alibabacloud-dkms-transfer-python2-0.0.6/
--rw-r--r--   0 root         (0) root         (0)     3877 2023-03-15 05:40:00.000000 alibabacloud-dkms-transfer-python2-0.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2525 2023-03-15 05:39:59.000000 alibabacloud-dkms-transfer-python2-0.0.6/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 05:40:00.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-15 05:39:59.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 05:40:00.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/handlers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-15 05:39:59.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2103 2023-03-15 05:39:59.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/handlers/asymmetic_decrypt_transfer_handler.py
--rw-r--r--   0 root         (0) root         (0)     2093 2023-03-15 05:39:59.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/handlers/asymmetic_encrypt_transfer_handler.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-03-15 05:39:59.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/handlers/asymmetic_sign_transfer_handler.py
--rw-r--r--   0 root         (0) root         (0)     2269 2023-03-15 05:39:59.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/handlers/asymmetic_verify_transfer_handler.py
--rw-r--r--   0 root         (0) root         (0)     2465 2023-03-15 05:39:59.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/handlers/decrypt_transfer_handler.py
--rw-r--r--   0 root         (0) root         (0)     2524 2023-03-15 05:39:59.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/handlers/encrypt_transfer_handler.py
--rw-r--r--   0 root         (0) root         (0)     3624 2023-03-15 05:39:59.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/handlers/generate_data_key_transfer_handler.py
--rw-r--r--   0 root         (0) root         (0)     3664 2023-03-15 05:39:59.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/handlers/generate_data_key_without_plaintext_transfer_handler.py
--rw-r--r--   0 root         (0) root         (0)     1793 2023-03-15 05:39:59.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/handlers/get_public_key_transfer_handler.py
--rw-r--r--   0 root         (0) root         (0)     2100 2023-03-15 05:39:59.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/handlers/get_secret_value_transfer_handler.py
--rw-r--r--   0 root         (0) root         (0)     5325 2023-03-15 05:39:59.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/handlers/kms_transfer_handler.py
--rw-r--r--   0 root         (0) root         (0)     5271 2023-03-15 05:39:59.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/kms_transfer_acs_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 05:40:00.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-15 05:39:59.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      809 2023-03-15 05:39:59.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/utils/consts.py
--rw-r--r--   0 root         (0) root         (0)     1556 2023-03-15 05:39:59.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/utils/kms_error_code_transfer_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 05:40:00.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer_python2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3877 2023-03-15 05:39:59.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer_python2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1393 2023-03-15 05:40:00.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer_python2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-15 05:39:59.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer_python2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       99 2023-03-15 05:39:59.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer_python2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-03-15 05:39:59.000000 alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer_python2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-15 05:40:00.000000 alibabacloud-dkms-transfer-python2-0.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1495 2023-03-15 05:39:59.000000 alibabacloud-dkms-transfer-python2-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/
+-rw-r--r--   0 root         (0) root         (0)     3877 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2525 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/handlers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2103 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/handlers/asymmetic_decrypt_transfer_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2093 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/handlers/asymmetic_encrypt_transfer_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/handlers/asymmetic_sign_transfer_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2269 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/handlers/asymmetic_verify_transfer_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2465 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/handlers/decrypt_transfer_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/handlers/encrypt_transfer_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3624 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/handlers/generate_data_key_transfer_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/handlers/generate_data_key_without_plaintext_transfer_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1793 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/handlers/get_public_key_transfer_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2100 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/handlers/get_secret_value_transfer_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5325 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/handlers/kms_transfer_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5474 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/kms_transfer_acs_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      809 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/utils/consts.py
+-rw-r--r--   0 root         (0) root         (0)     1556 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/utils/kms_error_code_transfer_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer_python2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3877 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer_python2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer_python2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer_python2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       99 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer_python2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer_python2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-05-19 10:43:35.000000 alibabacloud-dkms-transfer-python2-0.1.0/setup.py
```

### Comparing `alibabacloud-dkms-transfer-python2-0.0.6/PKG-INFO` & `alibabacloud-dkms-transfer-python2-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: alibabacloud-dkms-transfer-python2
-Version: 0.0.6
+Version: 0.1.0
 Summary: Alibaba Cloud Dedicated KMS Transfer SDK for Python2
 Home-page: https://github.com/aliyun/alibabacloud-dkms-transfer-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: Alibaba Cloud Dedicated KMS Transfer SDK for Python2
         ====================================================
```

### Comparing `alibabacloud-dkms-transfer-python2-0.0.6/README.rst` & `alibabacloud-dkms-transfer-python2-0.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/handlers/asymmetic_decrypt_transfer_handler.py` & `alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/handlers/asymmetic_decrypt_transfer_handler.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/handlers/asymmetic_encrypt_transfer_handler.py` & `alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/handlers/asymmetic_encrypt_transfer_handler.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/handlers/asymmetic_sign_transfer_handler.py` & `alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/handlers/asymmetic_sign_transfer_handler.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/handlers/asymmetic_verify_transfer_handler.py` & `alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/handlers/asymmetic_verify_transfer_handler.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/handlers/decrypt_transfer_handler.py` & `alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/handlers/decrypt_transfer_handler.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/handlers/encrypt_transfer_handler.py` & `alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/handlers/encrypt_transfer_handler.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/handlers/generate_data_key_transfer_handler.py` & `alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/handlers/generate_data_key_transfer_handler.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/handlers/generate_data_key_without_plaintext_transfer_handler.py` & `alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/handlers/generate_data_key_without_plaintext_transfer_handler.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/handlers/get_public_key_transfer_handler.py` & `alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/handlers/get_public_key_transfer_handler.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/handlers/get_secret_value_transfer_handler.py` & `alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/handlers/get_secret_value_transfer_handler.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/handlers/kms_transfer_handler.py` & `alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/handlers/kms_transfer_handler.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/kms_transfer_acs_client.py` & `alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/kms_transfer_acs_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 from alibabacloud_dkms_transfer.handlers.generate_data_key_without_plaintext_transfer_handler import \
     GenerateDataKeyWithoutPlaintextTransferHandler
 from alibabacloud_dkms_transfer.handlers.get_public_key_transfer_handler import GetPublicKeyTransferHandler
 from alibabacloud_dkms_transfer.handlers.get_secret_value_transfer_handler import GetSecretValueTransferHandler
 from alibabacloud_dkms_transfer.utils.consts import *
 
 
-class KmsTransferAcsClient(AcsClient):
+class KmsTransferAcsClient(AcsClient, object):
 
-    def __init__(self, config,
+    def __init__(self, config=None,
                  ak=None,
                  secret=None,
                  region_id="cn-hangzhou",
                  auto_retry=True,
                  max_retry_time=None,
                  user_agent=None,
                  port=80,
@@ -50,17 +50,21 @@
                            private_key=private_key,
                            session_period=session_period,
                            credential=credential,
                            debug=debug,
                            verify=verify,
                            pool_size=pool_size,
                            proxy=proxy)
-        self.handlers = dict()
-        self.client = Client(config)
-        self.init_kms_transfer_handlers()
+        if config is None:
+            self.is_use_kms_share_gateway = True
+        else:
+            self.is_use_kms_share_gateway = False
+            self.handlers = dict()
+            self.client = Client(config)
+            self.init_kms_transfer_handlers()
 
     def init_kms_transfer_handlers(self):
         self.handlers[ENCRYPT_API_NAME] = EncryptTransferHandler(self.client, ENCRYPT_API_NAME)
         self.handlers[DECRYPT_API_NAME] = DecryptTransferHandler(self.client, DECRYPT_API_NAME)
         self.handlers[ASYMMETRIC_ENCRYPT_API_NAME] = AsymmetricEncryptTransferHandler(self.client,
                                                                                       ASYMMETRIC_ENCRYPT_API_NAME)
         self.handlers[ASYMMETRIC_DECRYPT_API_NAME] = AsymmetricDecryptTransferHandler(self.client,
@@ -74,15 +78,15 @@
         self.handlers[GENERATE_DATA_KEY_WITHOUT_PLAINTEXT_API_NAME] = GenerateDataKeyWithoutPlaintextTransferHandler(
             self.client,
             GENERATE_DATA_KEY_WITHOUT_PLAINTEXT_API_NAME)
         self.handlers[GET_PUBLIC_KEY_API_NAME] = GetPublicKeyTransferHandler(self.client, GET_PUBLIC_KEY_API_NAME)
         self.handlers[GET_SECRET_VALUE_API_NAME] = GetSecretValueTransferHandler(self.client, GET_SECRET_VALUE_API_NAME)
 
     def _implementation_of_do_action(self, request, signer=None):
-        if self.handlers.__contains__(request.get_action_name()):
+        if not self.is_use_kms_share_gateway and self.handlers.__contains__(request.get_action_name()):
             return self.dispatch_dkms_action(request)
         return super(KmsTransferAcsClient, self)._implementation_of_do_action(request, signer)
 
     def dispatch_dkms_action(self, request):
         runtime_options = RuntimeOptions()
         if not self.get_verify():
             runtime_options.ignore_ssl = not self.get_verify()
```

### Comparing `alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/utils/consts.py` & `alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/utils/consts.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer/utils/kms_error_code_transfer_utils.py` & `alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer/utils/kms_error_code_transfer_utils.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer_python2.egg-info/PKG-INFO` & `alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer_python2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: alibabacloud-dkms-transfer-python2
-Version: 0.0.6
+Version: 0.1.0
 Summary: Alibaba Cloud Dedicated KMS Transfer SDK for Python2
 Home-page: https://github.com/aliyun/alibabacloud-dkms-transfer-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: Alibaba Cloud Dedicated KMS Transfer SDK for Python2
         ====================================================
```

### Comparing `alibabacloud-dkms-transfer-python2-0.0.6/alibabacloud_dkms_transfer_python2.egg-info/SOURCES.txt` & `alibabacloud-dkms-transfer-python2-0.1.0/alibabacloud_dkms_transfer_python2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud-dkms-transfer-python2-0.0.6/setup.py` & `alibabacloud-dkms-transfer-python2-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 packages = find_packages()
 NAME = "alibabacloud-dkms-transfer-python2"
 DESCRIPTION = "Alibaba Cloud Dedicated KMS Transfer SDK for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-dkms-transfer-python2-sdk"
-VERSION = "0.0.6"
+VERSION = "0.1.0"
 REQUIRES = [
     "alibabacloud_dkms_gcs_python2>=0.0.5",
     'aliyun_python_sdk_core>=2.13.30',
     'aliyun_python_sdk_kms>=2.14.0',
 ]
 
 LONG_DESCRIPTION = ''
```

