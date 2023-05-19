# Comparing `tmp/satori_playbook_validator-1.0.0.tar.gz` & `tmp/satori_playbook_validator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_playbook_validator-1.0.0.tar", last modified: Fri May 19 04:20:52 2023, max compression
+gzip compressed data, was "satori_playbook_validator-1.0.1.tar", last modified: Fri May 19 04:33:56 2023, max compression
```

## Comparing `satori_playbook_validator-1.0.0.tar` & `satori_playbook_validator-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       30 2023-05-19 04:01:53.443821 satori_playbook_validator-1.0.0/README.md
--rw-r--r--   0        0        0      387 2023-05-19 04:20:52.172819 satori_playbook_validator-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 04:11:27.023785 satori_playbook_validator-1.0.0/src/satorici/__init__.py
--rw-r--r--   0        0        0       42 2023-05-19 03:52:56.967680 satori_playbook_validator-1.0.0/src/satorici/validator/__init__.py
--rw-r--r--   0        0        0     2772 2023-05-19 04:11:45.908997 satori_playbook_validator-1.0.0/src/satorici/validator/_validator.py
--rw-r--r--   0        0        0      267 2023-05-19 01:00:58.588993 satori_playbook_validator-1.0.0/src/satorici/validator/schemas/command.json
--rw-r--r--   0        0        0      251 2023-05-19 01:00:58.588993 satori_playbook_validator-1.0.0/src/satorici/validator/schemas/import.json
--rw-r--r--   0        0        0     2197 2023-05-19 01:00:58.588993 satori_playbook_validator-1.0.0/src/satorici/validator/schemas/input.json
--rw-r--r--   0        0        0     1025 2023-05-19 01:00:58.588993 satori_playbook_validator-1.0.0/src/satorici/validator/schemas/settings.json
--rw-r--r--   0        0        0     1743 2023-05-19 01:00:58.588993 satori_playbook_validator-1.0.0/src/satorici/validator/schemas/test.json
--rw-r--r--   0        0        0      286 1970-01-01 00:00:00.000000 satori_playbook_validator-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-05-19 04:01:53.443821 satori_playbook_validator-1.0.1/README.md
+-rw-r--r--   0        0        0      387 2023-05-19 04:33:56.517022 satori_playbook_validator-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-19 04:11:27.023785 satori_playbook_validator-1.0.1/src/satorici/__init__.py
+-rw-r--r--   0        0        0      163 2023-05-19 04:31:06.265674 satori_playbook_validator-1.0.1/src/satorici/validator/__init__.py
+-rw-r--r--   0        0        0     2772 2023-05-19 04:29:51.667588 satori_playbook_validator-1.0.1/src/satorici/validator/_validator.py
+-rw-r--r--   0        0        0      267 2023-05-19 01:00:58.588993 satori_playbook_validator-1.0.1/src/satorici/validator/schemas/command.json
+-rw-r--r--   0        0        0      251 2023-05-19 01:00:58.588993 satori_playbook_validator-1.0.1/src/satorici/validator/schemas/import.json
+-rw-r--r--   0        0        0     2197 2023-05-19 01:00:58.588993 satori_playbook_validator-1.0.1/src/satorici/validator/schemas/input.json
+-rw-r--r--   0        0        0     1025 2023-05-19 01:00:58.588993 satori_playbook_validator-1.0.1/src/satorici/validator/schemas/settings.json
+-rw-r--r--   0        0        0     1743 2023-05-19 01:00:58.588993 satori_playbook_validator-1.0.1/src/satorici/validator/schemas/test.json
+-rw-r--r--   0        0        0      286 1970-01-01 00:00:00.000000 satori_playbook_validator-1.0.1/PKG-INFO
```

### Comparing `satori_playbook_validator-1.0.0/src/satorici/validator/_validator.py` & `satori_playbook_validator-1.0.1/src/satorici/validator/_validator.py`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-1.0.0/src/satorici/validator/schemas/input.json` & `satori_playbook_validator-1.0.1/src/satorici/validator/schemas/input.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-1.0.0/src/satorici/validator/schemas/settings.json` & `satori_playbook_validator-1.0.1/src/satorici/validator/schemas/settings.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-1.0.0/src/satorici/validator/schemas/test.json` & `satori_playbook_validator-1.0.1/src/satorici/validator/schemas/test.json`

 * *Files identical despite different names*

