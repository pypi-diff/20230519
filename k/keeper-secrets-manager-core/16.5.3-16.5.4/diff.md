# Comparing `tmp/keeper-secrets-manager-core-16.5.3.tar.gz` & `tmp/keeper-secrets-manager-core-16.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keeper-secrets-manager-core-16.5.3.tar", last modified: Mon Apr 17 20:28:16 2023, max compression
+gzip compressed data, was "keeper-secrets-manager-core-16.5.4.tar", last modified: Fri May 19 06:03:08 2023, max compression
```

## Comparing `keeper-secrets-manager-core-16.5.3.tar` & `keeper-secrets-manager-core-16.5.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:28:16.970933 keeper-secrets-manager-core-16.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-17 20:28:16.970933 keeper-secrets-manager-core-16.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:28:16.966933 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/configkeys.py
--rw-r--r--   0 runner    (1001) docker     (123)    67982 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:28:16.966933 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/dto/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17963 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/dto/dtos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/dto/payload.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/keeper_globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    20916 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:28:16.966933 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-17 20:28:16.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-17 20:28:16.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 20:28:16.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 20:28:16.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-17 20:28:16.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 20:28:16.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-17 20:28:16.970933 keeper-secrets-manager-core-16.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:03:08.428097 keeper-secrets-manager-core-16.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-19 06:03:08.428097 keeper-secrets-manager-core-16.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:03:08.424097 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/configkeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67982 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:03:08.428097 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/dto/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17984 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/dto/dtos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/dto/payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/keeper_globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21238 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:03:08.424097 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-19 06:03:08.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-19 06:03:08.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 06:03:08.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 06:03:08.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-19 06:03:08.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-19 06:03:08.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-19 06:03:08.428097 keeper-secrets-manager-core-16.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/setup.py
```

### Comparing `keeper-secrets-manager-core-16.5.3/PKG-INFO` & `keeper-secrets-manager-core-16.5.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keeper-secrets-manager-core
-Version: 16.5.3
+Version: 16.5.4
 Summary: Keeper Secrets Manager for Python 3
 Home-page: https://github.com/Keeper-Security/secrets-manager
 Author: Keeper Security
 Author-email: sm@keepersecurity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Keeper-Security/secrets-manager/issues
 Project-URL: Documentation, https://github.com/Keeper-Security/secrets-manager
@@ -27,14 +27,21 @@
 
 # Keeper Secrets Manager Python SDK
 
 For more information see our official documentation page https://docs.keeper.io/secrets-manager/secrets-manager/developer-sdk-library/python-sdk
 
 # Change Log
 
+## 16.5.4
+* KSM-405 - Added new script field type and oneTimeCode to PAM record types
+* KSM-410 - New field type: Passkey
+* KSM-394 - Ability to load configuration from AWS Secrets Manager using AWS AIM role in EC2 instance or AWS IAM user
+* KSM-416 - Fix OS detection bug
+* KSM-400 - Unpinned few dependencies
+
 ## 16.5.3
 * KSM-393 - Fix file permissions on localized Windows OS
 
 ## 16.5.2
 * KSM-375 - Make HTTPError to be more informative
 * KSM-376 - Support for PAM record types
 * KSM-381 - Transactions
```

### Comparing `keeper-secrets-manager-core-16.5.3/README.md` & `keeper-secrets-manager-core-16.5.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 # Keeper Secrets Manager Python SDK
 
 For more information see our official documentation page https://docs.keeper.io/secrets-manager/secrets-manager/developer-sdk-library/python-sdk
 
 # Change Log
 
+## 16.5.4
+* KSM-405 - Added new script field type and oneTimeCode to PAM record types
+* KSM-410 - New field type: Passkey
+* KSM-394 - Ability to load configuration from AWS Secrets Manager using AWS AIM role in EC2 instance or AWS IAM user
+* KSM-416 - Fix OS detection bug
+* KSM-400 - Unpinned few dependencies
+
 ## 16.5.3
 * KSM-393 - Fix file permissions on localized Windows OS
 
 ## 16.5.2
 * KSM-375 - Make HTTPError to be more informative
 * KSM-376 - Support for PAM record types
 * KSM-381 - Transactions
```

### Comparing `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/configkeys.py` & `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/configkeys.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/core.py` & `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/core.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/crypto.py` & `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/crypto.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/dto/dtos.py` & `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/dto/dtos.py`

 * *Files 1% similar despite different names*

```diff
@@ -420,15 +420,15 @@
         self.type = None
 
 
 VALID_RECORD_FIELDS = ['login', 'password', 'url', 'fileRef', 'oneTimeCode', 'otp', 'name', 'birthDate', 'date',
                        'expirationDate', 'text', 'securityQuestion', 'multiline', 'email', 'cardRef', 'addressRef',
                        'pinCode', 'phone', 'secret', 'note', 'accountNumber', 'paymentCard', 'bankAccount', 'keyPair',
                        'host', 'address', 'licenseNumber', 'recordRef', 'schedule', 'directoryType', 'databaseType',
-                       'pamHostname', 'pamResources', 'checkbox']
+                       'pamHostname', 'pamResources', 'checkbox', 'passkey', 'script']
 
 
 class RecordField:
 
     def __init__(self, field_type=None, value=None, label=None, required=None, enforceGeneration=None,
                  privacyScreen=None, complexity=None):
```

### Comparing `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/dto/payload.py` & `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/dto/payload.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/exceptions.py` & `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/helpers.py` & `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/helpers.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/keeper_globals.py` & `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/keeper_globals.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/mock.py` & `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/mock.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/storage.py` & `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/storage.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/utils.py` & `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,21 @@
     return base64.urlsafe_b64decode(s)
 
 
 def base64_to_string(b64s):
     return base64.b64decode(b64s).decode('UTF-8')
 
 
+def is_base64(s):
+    try:
+        return base64.b64encode(base64.b64decode(s)) == str.encode(s)
+    except (Exception,):
+        return False
+
+
 def string_to_bytes(s):
     return s.encode(ENCODING)
 
 
 def url_safe_str_to_bytes(s):
     b = base64.urlsafe_b64decode(s + '==')
     return b
@@ -201,17 +208,20 @@
             sample += sample_string[pos]
 
     return sample
 
 
 def get_windows_user_sid_and_name(logger=None):
     try:
-        user_sid = subprocess.check_output(['whoami', '/user']).splitlines()[-1]
+        # WSL2 systems may run linux whoami command instead and fail
+        # whoami: extra operand '/user'
+        # Use the full name of the executable - whoami.exe
+        user_sid = subprocess.check_output(['whoami.exe', '/user']).splitlines()[-1]
     except subprocess.CalledProcessError as e:
-        logger.info(f'Cannot get current Windows user via "whoami": {e}')
+        logger.debug(f'Cannot get current Windows user via "whoami.exe": {e}')
         return None, None
     else:
         return reversed(user_sid.split(b'\\')[-1].rsplit(b' ', 1))
 
 
 def set_config_mode(file, logger=None):
```

### Comparing `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core.egg-info/PKG-INFO` & `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keeper-secrets-manager-core
-Version: 16.5.3
+Version: 16.5.4
 Summary: Keeper Secrets Manager for Python 3
 Home-page: https://github.com/Keeper-Security/secrets-manager
 Author: Keeper Security
 Author-email: sm@keepersecurity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Keeper-Security/secrets-manager/issues
 Project-URL: Documentation, https://github.com/Keeper-Security/secrets-manager
@@ -27,14 +27,21 @@
 
 # Keeper Secrets Manager Python SDK
 
 For more information see our official documentation page https://docs.keeper.io/secrets-manager/secrets-manager/developer-sdk-library/python-sdk
 
 # Change Log
 
+## 16.5.4
+* KSM-405 - Added new script field type and oneTimeCode to PAM record types
+* KSM-410 - New field type: Passkey
+* KSM-394 - Ability to load configuration from AWS Secrets Manager using AWS AIM role in EC2 instance or AWS IAM user
+* KSM-416 - Fix OS detection bug
+* KSM-400 - Unpinned few dependencies
+
 ## 16.5.3
 * KSM-393 - Fix file permissions on localized Windows OS
 
 ## 16.5.2
 * KSM-375 - Make HTTPError to be more informative
 * KSM-376 - Support for PAM record types
 * KSM-381 - Transactions
```

### Comparing `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core.egg-info/SOURCES.txt` & `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.3/setup.py` & `keeper-secrets-manager-core-16.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 # Get the long description from the README.md file
 with open(os.path.join(here, 'README.md'), "r", encoding='utf-8') as fp:
     long_description = fp.read()
 
 install_requires = [
     'keeper-secrets-manager-helper>=1.0.4',
     'ecdsa',
-    'requests==2.28.2',
+    'requests',
     'cryptography>=39.0.1',
-    'importlib_metadata==6.0.0'
+    'importlib_metadata'
 ]
 
 setup(
     name="keeper-secrets-manager-core",
-    version="16.5.3",
+    version="16.5.4",
     description="Keeper Secrets Manager for Python 3",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Keeper Security",
     author_email="sm@keepersecurity.com",
     url="https://github.com/Keeper-Security/secrets-manager",
     license="MIT",
```

