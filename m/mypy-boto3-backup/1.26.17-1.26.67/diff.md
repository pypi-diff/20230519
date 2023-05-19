# Comparing `tmp/mypy-boto3-backup-1.26.17.tar.gz` & `tmp/mypy-boto3-backup-1.26.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-backup-1.26.17.tar", last modified: Mon Nov 28 04:09:25 2022, max compression
+gzip compressed data, was "mypy-boto3-backup-1.26.67.tar", last modified: Wed Feb  8 20:27:03 2023, max compression
```

## Comparing `mypy-boto3-backup-1.26.17.tar` & `mypy-boto3-backup-1.26.67.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:09:25.520745 mypy-boto3-backup-1.26.17/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-28 04:08:29.000000 mypy-boto3-backup-1.26.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    21988 2022-11-28 04:09:25.516745 mypy-boto3-backup-1.26.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    20555 2022-11-28 04:08:29.000000 mypy-boto3-backup-1.26.17/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:09:25.512745 mypy-boto3-backup-1.26.17/mypy_boto3_backup/
--rw-r--r--   0 runner    (1001) docker     (122)     3394 2022-11-28 04:08:29.000000 mypy-boto3-backup-1.26.17/mypy_boto3_backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3393 2022-11-28 04:08:29.000000 mypy-boto3-backup-1.26.17/mypy_boto3_backup/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      904 2022-11-28 04:08:29.000000 mypy-boto3-backup-1.26.17/mypy_boto3_backup/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    54628 2022-11-28 04:08:30.000000 mypy-boto3-backup-1.26.17/mypy_boto3_backup/client.py
--rw-r--r--   0 runner    (1001) docker     (122)    54536 2022-11-28 04:08:30.000000 mypy-boto3-backup-1.26.17/mypy_boto3_backup/client.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    10592 2022-11-28 04:08:30.000000 mypy-boto3-backup-1.26.17/mypy_boto3_backup/literals.py
--rw-r--r--   0 runner    (1001) docker     (122)    10590 2022-11-28 04:08:30.000000 mypy-boto3-backup-1.26.17/mypy_boto3_backup/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    16562 2022-11-28 04:08:30.000000 mypy-boto3-backup-1.26.17/mypy_boto3_backup/paginator.py
--rw-r--r--   0 runner    (1001) docker     (122)    16547 2022-11-28 04:08:30.000000 mypy-boto3-backup-1.26.17/mypy_boto3_backup/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-28 04:08:29.000000 mypy-boto3-backup-1.26.17/mypy_boto3_backup/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    67349 2022-11-28 04:08:32.000000 mypy-boto3-backup-1.26.17/mypy_boto3_backup/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (122)    67274 2022-11-28 04:08:31.000000 mypy-boto3-backup-1.26.17/mypy_boto3_backup/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-28 04:08:29.000000 mypy-boto3-backup-1.26.17/mypy_boto3_backup/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:09:25.516745 mypy-boto3-backup-1.26.17/mypy_boto3_backup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    21988 2022-11-28 04:09:25.000000 mypy-boto3-backup-1.26.17/mypy_boto3_backup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      661 2022-11-28 04:09:25.000000 mypy-boto3-backup-1.26.17/mypy_boto3_backup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 04:09:25.000000 mypy-boto3-backup-1.26.17/mypy_boto3_backup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 04:09:25.000000 mypy-boto3-backup-1.26.17/mypy_boto3_backup.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-28 04:09:25.000000 mypy-boto3-backup-1.26.17/mypy_boto3_backup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2022-11-28 04:09:25.000000 mypy-boto3-backup-1.26.17/mypy_boto3_backup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 04:09:25.520745 mypy-boto3-backup-1.26.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1957 2022-11-28 04:08:29.000000 mypy-boto3-backup-1.26.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:27:03.702110 mypy-boto3-backup-1.26.67/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-08 20:26:20.000000 mypy-boto3-backup-1.26.67/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22037 2023-02-08 20:27:03.702110 mypy-boto3-backup-1.26.67/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20554 2023-02-08 20:26:20.000000 mypy-boto3-backup-1.26.67/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:27:03.702110 mypy-boto3-backup-1.26.67/mypy_boto3_backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-02-08 20:26:20.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-02-08 20:26:20.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-02-08 20:26:20.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54858 2023-02-08 20:26:21.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54766 2023-02-08 20:26:20.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10967 2023-02-08 20:26:21.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10965 2023-02-08 20:26:21.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16562 2023-02-08 20:26:21.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16547 2023-02-08 20:26:21.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 20:26:20.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    67581 2023-02-08 20:26:24.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67506 2023-02-08 20:26:23.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-08 20:26:20.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:27:03.702110 mypy-boto3-backup-1.26.67/mypy_boto3_backup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22037 2023-02-08 20:27:03.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-02-08 20:27:03.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 20:27:03.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 20:27:03.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-08 20:27:03.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-08 20:27:03.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 20:27:03.702110 mypy-boto3-backup-1.26.67/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-02-08 20:26:20.000000 mypy-boto3-backup-1.26.67/setup.py
```

### Comparing `mypy-boto3-backup-1.26.17/LICENSE` & `mypy-boto3-backup-1.26.67/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.26.17/PKG-INFO` & `mypy-boto3-backup-1.26.67/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backup
-Version: 1.26.17
-Summary: Type annotations for boto3.Backup 1.26.17 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.67
+Summary: Type annotations for boto3.Backup 1.26.67 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backup.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-backup?color=blue)](https://pypistats.org/packages/mypy-boto3-backup)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Backup 1.26.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
+[boto3.Backup 1.26.67](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-backup docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-backup-1.26.17/README.md` & `mypy-boto3-backup-1.26.67/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backup.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-backup?color=blue)](https://pypistats.org/packages/mypy-boto3-backup)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Backup 1.26.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
+[boto3.Backup 1.26.67](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-backup docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-backup-1.26.17/mypy_boto3_backup/__init__.py` & `mypy-boto3-backup-1.26.67/mypy_boto3_backup/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.26.17/mypy_boto3_backup/__init__.pyi` & `mypy-boto3-backup-1.26.67/mypy_boto3_backup/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.26.17/mypy_boto3_backup/__main__.py` & `mypy-boto3-backup-1.26.67/mypy_boto3_backup/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Backup 1.26.17\nVersion:         1.26.17\nBuilder version:"
-        " 7.11.11\nDocs:           "
+        "Type annotations for boto3.Backup 1.26.67\nVersion:         1.26.67\nBuilder version:"
+        " 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.17")
+    print("1.26.67")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-backup-1.26.17/mypy_boto3_backup/client.py` & `mypy-boto3-backup-1.26.67/mypy_boto3_backup/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,16 @@
         self,
         *,
         BackupPlanId: str,
         BackupSelection: BackupSelectionTypeDef,
         CreatorRequestId: str = ...
     ) -> CreateBackupSelectionOutputTypeDef:
         """
-        .
+        Creates a JSON document that specifies a set of resources to assign to a backup
+        plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_selection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#create_backup_selection)
         """
 
     def create_backup_vault(
         self,
@@ -527,15 +528,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_backup_plan_from_template)
         """
 
     def get_backup_selection(
         self, *, BackupPlanId: str, SelectionId: str
     ) -> GetBackupSelectionOutputTypeDef:
         """
-        .
+        Returns selection metadata and a document in JSON format that specifies a list
+        of resources that are associated with a backup plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_backup_selection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_backup_selection)
         """
 
     def get_backup_vault_access_policy(
         self, *, BackupVaultName: str
```

### Comparing `mypy-boto3-backup-1.26.17/mypy_boto3_backup/client.pyi` & `mypy-boto3-backup-1.26.67/mypy_boto3_backup/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,16 @@
         self,
         *,
         BackupPlanId: str,
         BackupSelection: BackupSelectionTypeDef,
         CreatorRequestId: str = ...
     ) -> CreateBackupSelectionOutputTypeDef:
         """
-        .
+        Creates a JSON document that specifies a set of resources to assign to a backup
+        plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_selection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#create_backup_selection)
         """
     def create_backup_vault(
         self,
         *,
@@ -486,15 +487,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_backup_plan_from_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_backup_plan_from_template)
         """
     def get_backup_selection(
         self, *, BackupPlanId: str, SelectionId: str
     ) -> GetBackupSelectionOutputTypeDef:
         """
-        .
+        Returns selection metadata and a document in JSON format that specifies a list
+        of resources that are associated with a backup plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_backup_selection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_backup_selection)
         """
     def get_backup_vault_access_policy(
         self, *, BackupVaultName: str
     ) -> GetBackupVaultAccessPolicyOutputTypeDef:
```

### Comparing `mypy-boto3-backup-1.26.17/mypy_boto3_backup/literals.py` & `mypy-boto3-backup-1.26.67/mypy_boto3_backup/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -137,27 +138,30 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -186,14 +190,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -260,30 +265,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -316,28 +324,31 @@
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
     "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -365,30 +376,34 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
@@ -465,14 +480,15 @@
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-backup-1.26.17/mypy_boto3_backup/literals.pyi` & `mypy-boto3-backup-1.26.67/mypy_boto3_backup/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -135,27 +136,30 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -184,14 +188,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -258,30 +263,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -314,28 +322,31 @@
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
     "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -363,30 +374,34 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
@@ -463,14 +478,15 @@
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-backup-1.26.17/mypy_boto3_backup/paginator.py` & `mypy-boto3-backup-1.26.67/mypy_boto3_backup/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.26.17/mypy_boto3_backup/paginator.pyi` & `mypy-boto3-backup-1.26.67/mypy_boto3_backup/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.26.17/mypy_boto3_backup/type_defs.py` & `mypy-boto3-backup-1.26.67/mypy_boto3_backup/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -837,14 +837,15 @@
 
 ProtectedResourceTypeDef = TypedDict(
     "ProtectedResourceTypeDef",
     {
         "ResourceArn": str,
         "ResourceType": str,
         "LastBackupTime": datetime,
+        "ResourceName": str,
     },
     total=False,
 )
 
 _RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
     "_RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef",
     {
@@ -936,14 +937,15 @@
         "Status": RecoveryPointStatusType,
         "StatusMessage": str,
         "EncryptionKeyArn": str,
         "BackupSizeBytes": int,
         "BackupVaultName": str,
         "IsParent": bool,
         "ParentRecoveryPointArn": str,
+        "ResourceName": str,
     },
     total=False,
 )
 
 ListReportJobsInputRequestTypeDef = TypedDict(
     "ListReportJobsInputRequestTypeDef",
     {
@@ -1209,14 +1211,15 @@
         "StartBy": datetime,
         "ResourceType": str,
         "BytesTransferred": int,
         "BackupOptions": Dict[str, str],
         "BackupType": str,
         "ParentJobId": str,
         "IsParent": bool,
+        "ResourceName": str,
     },
     total=False,
 )
 
 CopyJobTypeDef = TypedDict(
     "CopyJobTypeDef",
     {
@@ -1236,14 +1239,15 @@
         "CreatedBy": RecoveryPointCreatorTypeDef,
         "ResourceType": str,
         "ParentJobId": str,
         "IsParent": bool,
         "CompositeMemberIdentifier": str,
         "NumberOfChildJobs": int,
         "ChildJobsInState": Dict[CopyJobStateType, int],
+        "ResourceName": str,
     },
     total=False,
 )
 
 _RequiredCopyActionTypeDef = TypedDict(
     "_RequiredCopyActionTypeDef",
     {
@@ -1359,14 +1363,15 @@
         "Lifecycle": LifecycleTypeDef,
         "EncryptionKeyArn": str,
         "IsEncrypted": bool,
         "LastRestoreTime": datetime,
         "ParentRecoveryPointArn": str,
         "CompositeMemberIdentifier": str,
         "IsParent": bool,
+        "ResourceName": str,
     },
     total=False,
 )
 
 ConditionsTypeDef = TypedDict(
     "ConditionsTypeDef",
     {
@@ -1483,14 +1488,15 @@
         "StartBy": datetime,
         "BackupOptions": Dict[str, str],
         "BackupType": str,
         "ParentJobId": str,
         "IsParent": bool,
         "NumberOfChildJobs": int,
         "ChildJobsInState": Dict[BackupJobStateType, int],
+        "ResourceName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBackupVaultOutputTypeDef = TypedDict(
     "DescribeBackupVaultOutputTypeDef",
     {
@@ -1519,14 +1525,15 @@
 
 DescribeProtectedResourceOutputTypeDef = TypedDict(
     "DescribeProtectedResourceOutputTypeDef",
     {
         "ResourceArn": str,
         "ResourceType": str,
         "LastBackupTime": datetime,
+        "ResourceName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRecoveryPointOutputTypeDef = TypedDict(
     "DescribeRecoveryPointOutputTypeDef",
     {
@@ -1548,14 +1555,15 @@
         "EncryptionKeyArn": str,
         "IsEncrypted": bool,
         "StorageClass": StorageClassType,
         "LastRestoreTime": datetime,
         "ParentRecoveryPointArn": str,
         "CompositeMemberIdentifier": str,
         "IsParent": bool,
+        "ResourceName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRegionSettingsOutputTypeDef = TypedDict(
     "DescribeRegionSettingsOutputTypeDef",
     {
```

### Comparing `mypy-boto3-backup-1.26.17/mypy_boto3_backup/type_defs.pyi` & `mypy-boto3-backup-1.26.67/mypy_boto3_backup/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -822,14 +822,15 @@
 
 ProtectedResourceTypeDef = TypedDict(
     "ProtectedResourceTypeDef",
     {
         "ResourceArn": str,
         "ResourceType": str,
         "LastBackupTime": datetime,
+        "ResourceName": str,
     },
     total=False,
 )
 
 _RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
     "_RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef",
     {
@@ -915,14 +916,15 @@
         "Status": RecoveryPointStatusType,
         "StatusMessage": str,
         "EncryptionKeyArn": str,
         "BackupSizeBytes": int,
         "BackupVaultName": str,
         "IsParent": bool,
         "ParentRecoveryPointArn": str,
+        "ResourceName": str,
     },
     total=False,
 )
 
 ListReportJobsInputRequestTypeDef = TypedDict(
     "ListReportJobsInputRequestTypeDef",
     {
@@ -1178,14 +1180,15 @@
         "StartBy": datetime,
         "ResourceType": str,
         "BytesTransferred": int,
         "BackupOptions": Dict[str, str],
         "BackupType": str,
         "ParentJobId": str,
         "IsParent": bool,
+        "ResourceName": str,
     },
     total=False,
 )
 
 CopyJobTypeDef = TypedDict(
     "CopyJobTypeDef",
     {
@@ -1205,14 +1208,15 @@
         "CreatedBy": RecoveryPointCreatorTypeDef,
         "ResourceType": str,
         "ParentJobId": str,
         "IsParent": bool,
         "CompositeMemberIdentifier": str,
         "NumberOfChildJobs": int,
         "ChildJobsInState": Dict[CopyJobStateType, int],
+        "ResourceName": str,
     },
     total=False,
 )
 
 _RequiredCopyActionTypeDef = TypedDict(
     "_RequiredCopyActionTypeDef",
     {
@@ -1320,14 +1324,15 @@
         "Lifecycle": LifecycleTypeDef,
         "EncryptionKeyArn": str,
         "IsEncrypted": bool,
         "LastRestoreTime": datetime,
         "ParentRecoveryPointArn": str,
         "CompositeMemberIdentifier": str,
         "IsParent": bool,
+        "ResourceName": str,
     },
     total=False,
 )
 
 ConditionsTypeDef = TypedDict(
     "ConditionsTypeDef",
     {
@@ -1442,14 +1447,15 @@
         "StartBy": datetime,
         "BackupOptions": Dict[str, str],
         "BackupType": str,
         "ParentJobId": str,
         "IsParent": bool,
         "NumberOfChildJobs": int,
         "ChildJobsInState": Dict[BackupJobStateType, int],
+        "ResourceName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBackupVaultOutputTypeDef = TypedDict(
     "DescribeBackupVaultOutputTypeDef",
     {
@@ -1478,14 +1484,15 @@
 
 DescribeProtectedResourceOutputTypeDef = TypedDict(
     "DescribeProtectedResourceOutputTypeDef",
     {
         "ResourceArn": str,
         "ResourceType": str,
         "LastBackupTime": datetime,
+        "ResourceName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRecoveryPointOutputTypeDef = TypedDict(
     "DescribeRecoveryPointOutputTypeDef",
     {
@@ -1507,14 +1514,15 @@
         "EncryptionKeyArn": str,
         "IsEncrypted": bool,
         "StorageClass": StorageClassType,
         "LastRestoreTime": datetime,
         "ParentRecoveryPointArn": str,
         "CompositeMemberIdentifier": str,
         "IsParent": bool,
+        "ResourceName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRegionSettingsOutputTypeDef = TypedDict(
     "DescribeRegionSettingsOutputTypeDef",
     {
```

### Comparing `mypy-boto3-backup-1.26.17/mypy_boto3_backup.egg-info/PKG-INFO` & `mypy-boto3-backup-1.26.67/mypy_boto3_backup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backup
-Version: 1.26.17
-Summary: Type annotations for boto3.Backup 1.26.17 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.67
+Summary: Type annotations for boto3.Backup 1.26.67 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backup.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-backup?color=blue)](https://pypistats.org/packages/mypy-boto3-backup)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Backup 1.26.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
+[boto3.Backup 1.26.67](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-backup docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-backup-1.26.17/mypy_boto3_backup.egg-info/SOURCES.txt` & `mypy-boto3-backup-1.26.67/mypy_boto3_backup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.26.17/setup.py` & `mypy-boto3-backup-1.26.67/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,45 +6,45 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-backup",
-    version="1.26.17",
+    version="1.26.67",
     packages=["mypy_boto3_backup"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Backup 1.26.17 service generated with mypy-boto3-builder"
-        " 7.11.11"
+        "Type annotations for boto3.Backup 1.26.67 service generated with mypy-boto3-builder 7.12.3"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 backup type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_backup": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_backup": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

