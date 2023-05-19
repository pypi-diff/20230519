# Comparing `tmp/hspylib-vault-0.9.82.tar.gz` & `tmp/hspylib-vault-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-vault-0.9.82.tar", last modified: Fri May 19 18:17:21 2023, max compression
+gzip compressed data, was "hspylib-vault-0.9.9.tar", last modified: Tue Feb 22 20:01:27 2022, max compression
```

## Comparing `hspylib-vault-0.9.82.tar` & `hspylib-vault-0.9.9.tar`

### file list

```diff
@@ -1,32 +1,37 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-19 18:17:21.313855 hspylib-vault-0.9.82/
--rw-r--r--   0 hjunior    (504) staff       (20)       96 2022-06-17 15:16:57.000000 hspylib-vault-0.9.82/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)     1543 2023-05-19 18:17:21.312826 hspylib-vault-0.9.82/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      675 2023-05-19 18:17:20.000000 hspylib-vault-0.9.82/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-19 18:17:21.278673 hspylib-vault-0.9.82/hspylib_vault.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)     1543 2023-05-19 18:17:21.000000 hspylib-vault-0.9.82/hspylib_vault.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      585 2023-05-19 18:17:21.000000 hspylib-vault-0.9.82/hspylib_vault.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-05-19 18:17:21.000000 hspylib-vault-0.9.82/hspylib_vault.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       73 2023-05-19 18:17:21.000000 hspylib-vault-0.9.82/hspylib_vault.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-05-19 18:17:21.000000 hspylib-vault-0.9.82/hspylib_vault.egg-info/top_level.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-05-19 18:17:21.314014 hspylib-vault-0.9.82/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     1854 2023-04-19 22:13:51.000000 hspylib-vault-0.9.82/setup.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-19 18:17:21.285377 hspylib-vault-0.9.82/vault/
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-05-19 18:17:20.000000 hspylib-vault-0.9.82/vault/.version
--rw-r--r--   0 hjunior    (504) staff       (20)      716 2023-04-19 22:01:58.000000 hspylib-vault-0.9.82/vault/__classpath__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      180 2023-05-19 18:17:20.000000 hspylib-vault-0.9.82/vault/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     5147 2023-04-19 22:13:51.000000 hspylib-vault-0.9.82/vault/__main__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-19 18:17:21.295898 hspylib-vault-0.9.82/vault/core/
--rw-r--r--   0 hjunior    (504) staff       (20)      219 2023-05-19 18:17:20.000000 hspylib-vault-0.9.82/vault/core/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)    13018 2023-04-19 22:18:03.000000 hspylib-vault-0.9.82/vault/core/vault.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1395 2023-04-19 22:18:03.000000 hspylib-vault-0.9.82/vault/core/vault_config.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1852 2023-04-19 22:18:03.000000 hspylib-vault-0.9.82/vault/core/vault_repository.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2358 2023-04-19 22:18:03.000000 hspylib-vault-0.9.82/vault/core/vault_service.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-19 18:17:21.302318 hspylib-vault-0.9.82/vault/domain/
--rw-r--r--   0 hjunior    (504) staff       (20)      165 2023-05-19 18:17:20.000000 hspylib-vault-0.9.82/vault/domain/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3466 2023-04-19 22:18:03.000000 hspylib-vault-0.9.82/vault/domain/vault_entry.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-19 18:17:21.309152 hspylib-vault-0.9.82/vault/exception/
--rw-r--r--   0 hjunior    (504) staff       (20)      167 2023-05-19 18:17:20.000000 hspylib-vault-0.9.82/vault/exception/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      839 2023-04-19 22:01:58.000000 hspylib-vault-0.9.82/vault/exception/exceptions.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-19 18:17:21.311020 hspylib-vault-0.9.82/vault/resources/
--rw-r--r--   0 hjunior    (504) staff       (20)       69 2022-11-12 19:14:13.000000 hspylib-vault-0.9.82/vault/resources/application.properties
--rw-r--r--   0 hjunior    (504) staff       (20)      168 2023-04-19 21:58:35.000000 hspylib-vault-0.9.82/vault/welcome.txt
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.651843 hspylib-vault-0.9.9/
+-rw-r--r--   0 hjunior    (504) staff       (20)      125 2022-02-18 20:26:39.000000 hspylib-vault-0.9.9/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)      662 2022-02-22 20:01:27.650723 hspylib-vault-0.9.9/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)       41 2022-02-13 18:46:58.000000 hspylib-vault-0.9.9/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.604944 hspylib-vault-0.9.9/hspylib_vault.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)      662 2022-02-22 20:01:27.000000 hspylib-vault-0.9.9/hspylib_vault.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      704 2022-02-22 20:01:27.000000 hspylib-vault-0.9.9/hspylib_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2022-02-22 20:01:27.000000 hspylib-vault-0.9.9/hspylib_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       57 2022-02-22 20:01:27.000000 hspylib-vault-0.9.9/hspylib_vault.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2022-02-22 20:01:27.000000 hspylib-vault-0.9.9/hspylib_vault.egg-info/top_level.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2022-02-22 20:01:27.651948 hspylib-vault-0.9.9/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     1557 2022-02-15 20:32:21.000000 hspylib-vault-0.9.9/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.615812 hspylib-vault-0.9.9/vault/
+-rw-r--r--   0 hjunior    (504) staff       (20)        5 2022-02-22 20:01:25.000000 hspylib-vault-0.9.9/vault/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      193 2022-02-22 19:09:15.000000 hspylib-vault-0.9.9/vault/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     4384 2022-02-18 21:07:53.000000 hspylib-vault-0.9.9/vault/__main__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.624864 hspylib-vault-0.9.9/vault/core/
+-rw-r--r--   0 hjunior    (504) staff       (20)      217 2022-02-22 19:09:15.000000 hspylib-vault-0.9.9/vault/core/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     8712 2022-02-22 08:50:25.000000 hspylib-vault-0.9.9/vault/core/vault.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1315 2022-02-15 20:32:21.000000 hspylib-vault-0.9.9/vault/core/vault_config.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2160 2022-02-22 08:50:25.000000 hspylib-vault-0.9.9/vault/core/vault_repository.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1089 2022-02-22 08:50:25.000000 hspylib-vault-0.9.9/vault/core/vault_service.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.628367 hspylib-vault-0.9.9/vault/entity/
+-rw-r--r--   0 hjunior    (504) staff       (20)      179 2022-02-22 19:09:15.000000 hspylib-vault-0.9.9/vault/entity/__init__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.631698 hspylib-vault-0.9.9/vault/entity/validator/
+-rw-r--r--   0 hjunior    (504) staff       (20)      177 2022-02-22 19:09:15.000000 hspylib-vault-0.9.9/vault/entity/validator/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2231 2022-02-22 08:50:25.000000 hspylib-vault-0.9.9/vault/entity/validator/entry_validator.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2128 2022-02-15 20:32:21.000000 hspylib-vault-0.9.9/vault/entity/vault_entry.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.634841 hspylib-vault-0.9.9/vault/exception/
+-rw-r--r--   0 hjunior    (504) staff       (20)      165 2022-02-22 19:09:15.000000 hspylib-vault-0.9.9/vault/exception/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      627 2022-02-11 19:26:38.000000 hspylib-vault-0.9.9/vault/exception/exceptions.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.642361 hspylib-vault-0.9.9/vault/resources/
+-rw-r--r--   0 hjunior    (504) staff       (20)       69 2022-02-15 20:32:21.000000 hspylib-vault-0.9.9/vault/resources/application.properties
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.649219 hspylib-vault-0.9.9/vault/resources/log/
+-rw-r--r--   0 hjunior    (504) staff       (20)        0 2022-02-02 16:37:07.000000 hspylib-vault-0.9.9/vault/resources/log/.gitkeep
+-rw-r--r--   0 hjunior    (504) staff       (20)     2572 2022-02-21 23:29:30.000000 hspylib-vault-0.9.9/vault/resources/log/application.log
+-rw-r--r--   0 hjunior    (504) staff       (20)      168 2022-02-18 20:29:20.000000 hspylib-vault-0.9.9/vault/welcome.txt
```

### Comparing `hspylib-vault-0.9.82/hspylib_vault.egg-info/SOURCES.txt` & `hspylib-vault-0.9.9/hspylib_vault.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 setup.py
 hspylib_vault.egg-info/PKG-INFO
 hspylib_vault.egg-info/SOURCES.txt
 hspylib_vault.egg-info/dependency_links.txt
 hspylib_vault.egg-info/requires.txt
 hspylib_vault.egg-info/top_level.txt
 vault/.version
-vault/__classpath__.py
 vault/__init__.py
 vault/__main__.py
 vault/welcome.txt
 vault/core/__init__.py
 vault/core/vault.py
 vault/core/vault_config.py
 vault/core/vault_repository.py
 vault/core/vault_service.py
-vault/domain/__init__.py
-vault/domain/vault_entry.py
+vault/entity/__init__.py
+vault/entity/vault_entry.py
+vault/entity/validator/__init__.py
+vault/entity/validator/entry_validator.py
 vault/exception/__init__.py
 vault/exception/exceptions.py
-vault/resources/application.properties
+vault/resources/application.properties
+vault/resources/log/.gitkeep
+vault/resources/log/application.log
```

### Comparing `hspylib-vault-0.9.82/vault/core/vault.py` & `hspylib-vault-0.9.9/vault/core/vault.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,293 +1,216 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HsPyLib-Vault
-   @package: vault.core
+   TODO Purpose of the file
+   @project: HSPyLib
+   hspylib.app.vault.core
       @file: vault.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2023, HsPyLib team
+   Copyright 2021, HSPyLib team
 """
 
-from cryptography.fernet import InvalidToken
-from datasource.identity import Identity
-from hspylib.core.preconditions import check_not_none
-from hspylib.core.tools.commons import file_is_not_empty, safe_delete_file, syserr, sysout, touch_file
-from hspylib.modules.cache.ttl_keyring_be import TTLKeyringBE
-from hspylib.modules.security.security import b64_decode, decode_file, decrypt_file, encode_file, encrypt_file
-from typing import List
-from vault.core.vault_config import VaultConfig
-from vault.core.vault_service import VaultService
-from vault.domain.vault_entry import VaultEntry
-from vault.exception.exceptions import VaultCloseError, VaultExecutionException, VaultSecurityException
-
+import base64
 import binascii
-import contextlib
-import cryptocode
 import getpass
-import keyring
 import logging as log
 import os
-import shutil
 import uuid
 
+from cryptography.fernet import InvalidToken
+from hspylib.core.tools.commons import file_is_not_empty, safe_del_file, syserr, sysout, touch_file
+from hspylib.modules.cli.tui.menu.menu_utils import MenuUtils
+from hspylib.modules.security.security import decrypt, encrypt
 
-class Vault:
-    """Represents the vault and it's functionalities."""
+from vault.core.vault_config import VaultConfig
+from vault.core.vault_service import VaultService
+from vault.entity.vault_entry import VaultEntry
+from vault.exception.exceptions import VaultCloseError, VaultOpenError
 
-    # Vault hash code
-    _VAULT_HASHCODE = os.getenv("VAULT_HASHCODE", "e4f362fd1e02df6bc9c684c9310e3550")
 
-    # Vault keyring cache entry
-    _VAULT_CACHE_NAME = "VAULT_KEY_SERVICE"
+class Vault:
+    """Represents the vault and it's functionalities"""
 
-    def __init__(self, resource_dir: str) -> None:
-        self._is_unlocked = False
-        self._passphrase = None
-        self._configs = VaultConfig(resource_dir)
-        self.service = VaultService(self._configs)
-        keyring.set_keyring(TTLKeyringBE())
+    def __init__(self):
+        self.is_open = False
+        self.passphrase = None
+        self.configs = VaultConfig()
+        self.service = VaultService()
 
     def __str__(self):
         data = set(self.service.list())
         vault_str = ""
         for entry in data:
             vault_str += entry.key
         return vault_str
 
-    @property
-    def configs(self) -> VaultConfig:
-        return self._configs
-
-    @contextlib.contextmanager
     def open(self) -> bool:
-        """Open and read the Vault file."""
+        """Open and read the Vault file"""
         try:
-            self._sanity_check()
-            self._passphrase = self._read_passphrase()
-            if not self._is_unlocked:
+            self.passphrase = self._read_passphrase()
+            if not self.is_open:
                 self._unlock_vault()
                 log.debug("Vault open and unlocked")
-            yield self._is_unlocked or None
         except (UnicodeDecodeError, InvalidToken, binascii.Error) as err:
             log.error("Authentication failure => %s", err)
-            syserr("Authentication failure")
-            keyring.delete_password(self._VAULT_CACHE_NAME, self._configs.vault_user)
-            yield None
-        finally:
-            self.close()
+            MenuUtils.print_error('Authentication failure')
+            return False
+        except Exception as err:
+            raise VaultOpenError(f"Unable to open Vault file => {self.configs.vault_file()}", err) from err
 
-        return self._is_unlocked
+        return True
 
     def close(self) -> bool:
-        """Close the Vault file and cleanup temporary files."""
+        """Close the Vault file and cleanup temporary file_paths"""
         try:
-            if self._is_unlocked:
+            if self.is_open:
                 self._lock_vault()
                 log.debug("Vault closed and locked")
-        except (UnicodeDecodeError, InvalidToken, binascii.Error) as err:
+        except (UnicodeDecodeError, InvalidToken) as err:
             log.error("Authentication failure => %s", err)
-            syserr("Authentication failure")
+            MenuUtils.print_error('Authentication failure')
             return False
         except Exception as err:
-            raise VaultCloseError(f"Unable to close Vault file => {self._configs.vault_file}", err) from err
+            raise VaultCloseError(f"Unable to close Vault file => {self.configs.vault_file()}", err) from err
 
         return True
 
-    def list(self, filter_expr: List[str] = None) -> None:
+    def list(self, filter_expr: str = None) -> None:
         """List all vault entries filtered by filter_expr
-        :param filter_expr: The entry filter expression.
+        :param filter_expr: The filter expression
         """
-        data = self.service.list_by_key(filter_expr)
+        data = self.service.list(filter_expr)
         if len(data) > 0:
-            sysout(
-                "%YELLOW%{} {}%NC%".format(
-                    f"\n-=- Listing all ({len(data)}) vault entries ",
-                    f"matching '{filter_expr}' -=-" if filter_expr else "-=-",
-                )
-            )
+            sysout("%YELLOW%{} {}%NC%".format(
+                "\n=== Listing all vault entries",
+                f"matching \'{filter_expr}\' ===\n" if filter_expr else "===\n"))
             for entry in data:
                 sysout(entry.to_string())
         else:
             if filter_expr:
-                sysout(f"%YELLOW%%EOL%-=- No results to display containing '{filter_expr}' -=-%EOL%%NC%")
+                sysout(f"%YELLOW%\nxXx No results to display containing '{filter_expr}' xXx\n%NC%")
             else:
-                sysout("%YELLOW%%EOL%-=- Vault is empty -=-%EOL%%NC%")
+                sysout("%YELLOW%\nxXx Vault is empty xXx\n%NC%")
         log.debug("Vault list issued. User=%s", getpass.getuser())
 
-    def add(self, key: str, hint: str | None, password: str | None) -> None:
+    def add(self, key: str, hint: str, password: str) -> None:
         """Add a vault entry
-        :param key: the vault entry key to be added.
-        :param hint: the vault entry hint to be added.
-        :param password: the vault entry password to be added.
+        :param key: The vault entry name to be added
+        :param hint: The vault entry hint to be added
+        :param password: The vault entry password to be added
         """
-        check_not_none(key)
-        if not self.service.exists(key):
-            entry = VaultEntry(Identity(VaultEntry.VaultId(uuid.uuid4().hex)), key, key, password, hint)
-            if not hint or not password:
-                entry = VaultEntry.prompt(entry)
-            if entry:
-                self.service.save(entry)
-                sysout(f"%GREEN%%EOL%=== Entry saved ===%EOL%%EOL%%NC%{entry.to_string()}")
+        entry = self.service.get_by_key(key)
+        if not entry:
+            while not password:
+                password = getpass.getpass(f"Type the password for '{key}': ").strip()
+            entry = VaultEntry(uuid.uuid4(), key, key, password, hint)
+            self.service.save(entry)
+            sysout(f"%GREEN%\n=== Entry added ===\n\n%NC%{entry.to_string()}")
         else:
-            log.error("Attempt to add to Vault failed for key=%s", key)
+            log.error("Attempt to add to Vault failed for name=%s", key)
             syserr(f"### Entry specified by '{key}' already exists in vault")
         log.debug("Vault add issued. User=%s", getpass.getuser())
 
-    def update(self, key: str, hint: str | None, password: str | None) -> None:
-        """Update a vault entry
-        :param key: the vault entry key to be updated.
-        :param hint: the vault entry hint to be updated.
-        :param password: the vault entry password to be updated.
-        """
-        check_not_none(key)
-        if entry := self.service.get_by_key(key):
-            entry.hint = hint if hint else entry.hint
-            entry.password = password if password else self._decrypt_passphrase(entry.password)
-            if not hint or not password:
-                entry = VaultEntry.prompt(entry)
-            if entry:
-                entry.password = self._encrypt_passphrase(entry.password)
-                self.service.save(entry)
-                sysout(f"%GREEN%%EOL%=== Entry updated ===%EOL%%EOL%%NC%{entry.to_string()}")
-        else:
-            log.error("Attempt to update Vault failed for key=%s", key)
-            syserr(f"### No entry specified by '{key}' was found in vault")
-        log.debug("Vault update issued. User=%s", getpass.getuser())
-
     def get(self, key) -> None:
         """Display the vault entry specified by name
-        :param key: the vault entry key to get
+        :param key: The vault entry name to get
         """
         entry = self.service.get_by_key(key)
         if entry:
-            entry.password = cryptocode.decrypt(entry.password, self._VAULT_HASHCODE)
             sysout(f"\n{entry.to_string(True, True)}")
         else:
-            log.error("Attempt to get from Vault failed for key=%s", key)
-            syserr(f"### No entry specified by '{key}' was found in vault ###")
+            log.error("Attempt to get from Vault failed for name=%s", key)
+            syserr(f"### No entry specified by '{key}' was found in vault")
         log.debug("Vault get issued. User=%s", getpass.getuser())
 
+    def update(self, key, hint, password) -> None:
+        """Update a vault entry
+        :param key: The vault entry name to be updated
+        :param hint: The vault entry hint to be updated
+        :param password: The vault entry password to be updated
+        """
+        entry = self.service.get_by_key(key)
+        if entry:
+            if not password:
+                passphrase = getpass.getpass(f"Type a password for '{key}': ").strip()
+            else:
+                passphrase = password
+            upd_entry = VaultEntry(entry.uuid, key, key, passphrase, hint)
+            self.service.save(upd_entry)
+            sysout(f"%GREEN%\n=== Entry updated ===\n\n%NC%{entry.to_string()}")
+        else:
+            log.error("Attempt to update Vault failed for name=%s", key)
+            syserr(f"### No entry specified by '{key}' was found in vault")
+        log.debug("Vault update issued. User=%s", getpass.getuser())
+
     def remove(self, key: str) -> None:
         """Remove a vault entry
-        :param key: The vault entry key to be removed
+        :param key: The vault entry name to be removed
         """
         entry = self.service.get_by_key(key)
         if entry:
             self.service.remove(entry)
-            sysout(f"%GREEN%%EOL%=== Entry removed ===%EOL%%EOL%%NC%{entry.to_string()}")
+            sysout(f"%GREEN%\n=== Entry removed ===\n\n%NC%{entry.to_string()}")
         else:
-            log.error("Attempt to remove to Vault failed for key=%s", key)
+            log.error("Attempt to remove to Vault failed for name=%s", key)
             syserr(f"### No entry specified by '{key}' was found in vault")
         log.debug("Vault remove issued. User=%s", getpass.getuser())
 
-    def _encrypt_passphrase(self, passphrase: str) -> str:
-        """Encrypt current assigned passphrase.
-        :param passphrase: the passphrase to encrypt.
-        """
-        return cryptocode.encrypt(passphrase, self._VAULT_HASHCODE)
-
-    def _decrypt_passphrase(self, passphrase: str) -> str:
-        """Decrypt current assigned passphrase.
-        :param passphrase: the passphrase to decrypt.
-        """
-        return cryptocode.decrypt(passphrase, self._VAULT_HASHCODE)
-
     def _read_passphrase(self) -> str:
-        """Read and return the vault currently assigned passphrase."""
-        passphrase, confirm_passphrase = None, False
-        if file_is_not_empty(self._configs.vault_file):
-            if self._configs.passphrase:
-                return f"{self._configs.vault_user}:{b64_decode(self._configs.passphrase)}"
-        else:
-            sysout(f"%ORANGE%### Your Vault '{self._configs.vault_file}' file does not exist ###")
-            sysout("%ORANGE%>>> Enter the new passphrase to create a new Vault file <<<")
-            if not (confirm_passphrase := self._create_new_vault()):
-                raise VaultExecutionException(f"Unable to create vault file: {self._configs.vault_file}")
-        while not passphrase:
-            passphrase = self._getpass(confirm_passphrase)
-            if passphrase and confirm_passphrase:
-                passphrase_confirm = None
-                while not passphrase_confirm or passphrase_confirm != passphrase:
-                    passphrase_confirm = getpass.getpass("Repeat passphrase:").strip()
-                    if passphrase_confirm != passphrase:
-                        syserr("### Passphrase and confirmation mismatch")
-                        safe_delete_file(self._configs.vault_file)
-                sysout(f"%GREEN%Passphrase successfully stored at: '{self._configs.vault_file}'")
-                log.debug(
-                    "Vault passphrase created for user=%s and vault=%s",
-                    self._configs.vault_user,
-                    self._configs.vault_file,
-                )
-                self._is_unlocked = True
+        """Retrieve and read the vault passphrase"""
+        if file_is_not_empty(self.configs.vault_file()):
+            confirm_flag = False
+        else:
+            sysout(f"%ORANGE%### Your Vault '{self.configs.vault_file()}' file is empty.")
+            sysout("%ORANGE%>>> Enter the new passphrase for this Vault")
+            confirm_flag = True
+            touch_file(self.configs.vault_file())
+        passphrase = self.configs.passphrase()
+        if passphrase:
+            return f"{self.configs.vault_user()}:{base64.b64decode(passphrase).decode('utf-8')}"
 
-        return f"{self._configs.vault_user}:{passphrase}"
+        while not passphrase:
+            passphrase = getpass.getpass("Enter passphrase:").strip()
+            confirm = None
+            if passphrase and confirm_flag:
+                while not confirm:
+                    confirm = getpass.getpass("Repeat passphrase:").strip()
+                if confirm != passphrase:
+                    syserr("### Passphrase and confirmation mismatch")
+                    safe_del_file(self.configs.vault_file())
+                else:
+                    sysout("%GREEN%Passphrase successfully stored")
+                    log.debug("Vault passphrase created for user=%s", self.configs.vault_user())
+                    touch_file(self.configs.vault_file())
+                    self.is_open = True
+        return f"{self.configs.vault_user()}:{passphrase}"
 
     def _lock_vault(self) -> None:
-        """Lock the vault file (encode & encrypt)."""
-        if file_is_not_empty(self._configs.unlocked_vault_file):
-            encoded = f"{self._configs.unlocked_vault_file}-encoded"
-            encode_file(self._configs.unlocked_vault_file, encoded, binary=True)
-            encrypt_file(encoded, self._configs.vault_file, self._passphrase)
-            safe_delete_file(encoded)
+        """Encrypt the vault file"""
+        if file_is_not_empty(self.configs.unlocked_vault_file()):
+            encrypt(
+                self.configs.unlocked_vault_file(),
+                self.configs.vault_file(),
+                self.passphrase)
             log.debug("Vault file is encrypted")
         else:
-            os.rename(self._configs.unlocked_vault_file, self._configs.vault_file)
-        self._is_unlocked = False
-        safe_delete_file(self._configs.unlocked_vault_file)
+            os.rename(self.configs.unlocked_vault_file(), self.configs.vault_file())
+        self.is_open = False
+        safe_del_file(self.configs.unlocked_vault_file())
 
     def _unlock_vault(self) -> None:
-        """Unlock the vault file (decode & decrypt)."""
-        if file_is_not_empty(self._configs.vault_file):
-            encoded = f"{self._configs.unlocked_vault_file}-encoded"
-            decrypt_file(self._configs.vault_file, encoded, self._passphrase)
-            decode_file(encoded, self._configs.unlocked_vault_file, binary=True)
-            safe_delete_file(encoded)
+        """Decrypt the vault file"""
+        if file_is_not_empty(self.configs.vault_file()):
+            decrypt(
+                self.configs.vault_file(),
+                self.configs.unlocked_vault_file(),
+                self.passphrase, )
             log.debug("Vault file is decrypted")
         else:
-            os.rename(self._configs.vault_file, self._configs.unlocked_vault_file)
-        self._is_unlocked = True
-        safe_delete_file(self._configs.vault_file)
-
-    def _sanity_check(self) -> None:
-        """Check existing vault backups and apply a rollback if required."""
-        vault_file = self._configs.vault_file
-        unlocked_vault_file = self._configs.unlocked_vault_file
-        backup_file = f"{os.getenv('HOME', os.getenv('TEMP', '/tmp'))}/.{os.path.basename(vault_file)}.bak"
-        locked_empty = not file_is_not_empty(vault_file)
-        unlocked_empty = not file_is_not_empty(unlocked_vault_file)
-        if not locked_empty or not unlocked_empty:
-            if not locked_empty and unlocked_empty:
-                log.debug("Creating a vault backup before opening it => %s", backup_file)
-                shutil.copyfile(vault_file, backup_file)
-            else:
-                log.warning("Vault file was found open and will be removed => %s", vault_file)
-                if os.path.exists(backup_file):
-                    log.warning("Restoring last backup => %s", backup_file)
-                    shutil.copyfile(backup_file, vault_file)
-                    safe_delete_file(unlocked_vault_file)
-                else:
-                    log.warning("No backups found !")
-                    raise VaultSecurityException(
-                        "Unable to either restore or re-lock the vault file. Please manually "
-                        + f' backup your secrets and remove the unlocked file "{unlocked_vault_file}"'
-                    )
-
-    def _getpass(self, skip_cache: bool) -> str:
-        """Prompt for the user password or retrieved the cached one if skip cache is not set.
-        :param skip_cache: whether to skip the cached password value or not.
-        """
-        if skip_cache or (passwd := keyring.get_password(self._VAULT_CACHE_NAME, self._configs.vault_user)) is None:
-            passwd = getpass.getpass("Enter passphrase:").rstrip()
-            keyring.set_password(self._VAULT_CACHE_NAME, self._configs.vault_user, passwd)
-        return passwd
-
-    def _create_new_vault(self) -> bool:
-        """Create the vault SQLite DB file."""
-        touch_file(self._configs.vault_file)
-        self.service.create_vault_db()
-        return os.path.exists(self._configs.vault_file)
+            os.rename(self.configs.vault_file(), self.configs.unlocked_vault_file())
+        self.is_open = True
+        safe_del_file(self.configs.vault_file())
```

### Comparing `hspylib-vault-0.9.82/vault/exception/exceptions.py` & `hspylib-vault-0.9.9/vault/exception/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HsPyLib-Vault
-   @package: vault.exception
+   TODO Purpose of the file
+   @project: HSPyLib
+   hspylib.app.vault.exception
       @file: exceptions.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2023, HsPyLib team
+   Copyright 2021, HSPyLib team
 """
 from hspylib.core.exception.exceptions import HSBaseException
 
 
 class VaultCloseError(HSBaseException):
     """Raised when closing the vault"""
 
 
 class VaultOpenError(HSBaseException):
     """Raised when opening the vault"""
-
-
-class VaultSecurityException(HSBaseException):
-    """Raised when something unexpected happened to vault file"""
-
-
-class VaultExecutionException(HSBaseException):
-    """Raised when something unexpected happened to vault execution"""
```

