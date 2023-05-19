# Comparing `tmp/cdk-opinionated-constructs-2.0.1.tar.gz` & `tmp/cdk-opinionated-constructs-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-opinionated-constructs-2.0.1.tar", last modified: Thu Apr 20 10:39:09 2023, max compression
+gzip compressed data, was "cdk-opinionated-constructs-2.1.0.tar", last modified: Fri May 19 08:38:33 2023, max compression
```

## Comparing `cdk-opinionated-constructs-2.0.1.tar` & `cdk-opinionated-constructs-2.1.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-04-20 10:39:09.302361 cdk-opinionated-constructs-2.0.1/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1071 2022-11-05 20:03:58.000000 cdk-opinionated-constructs-2.0.1/LICENSE
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      339 2023-04-20 10:39:09.303619 cdk-opinionated-constructs-2.0.1/PKG-INFO
--rw-r--r--   0 tomaszszuster   (501) staff       (20)    27443 2023-04-18 12:21:33.000000 cdk-opinionated-constructs-2.0.1/README.md
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-04-20 10:39:09.127497 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)       50 2022-11-05 21:10:53.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     4879 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/alb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2235 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/ecr.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     8661 2023-04-20 10:19:32.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/lmb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     5811 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/nlb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     4643 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/rds_instance.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2798 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/s3.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1464 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/sns.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)    11940 2022-12-03 22:01:00.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/wafv2.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-04-20 10:39:09.298337 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs.egg-info/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      339 2023-04-20 10:39:09.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs.egg-info/PKG-INFO
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1221 2023-04-20 10:39:09.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        1 2023-04-20 10:39:09.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)       89 2023-04-20 10:39:09.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs.egg-info/requires.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)       32 2023-04-20 10:39:09.000000 cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs.egg-info/top_level.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3649 2023-04-20 10:39:09.309152 cdk-opinionated-constructs-2.0.1/setup.cfg
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      760 2023-04-20 10:38:52.000000 cdk-opinionated-constructs-2.0.1/setup.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-04-20 10:39:09.135496 cdk-opinionated-constructs-2.0.1/test/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.0.1/test/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1781 2023-04-20 10:28:48.000000 cdk-opinionated-constructs-2.0.1/test/app.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-04-20 10:39:09.243334 cdk-opinionated-constructs-2.0.1/test/stacks/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.0.1/test/stacks/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2322 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.1/test/stacks/alb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1012 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-2.0.1/test/stacks/ecr_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3241 2023-04-20 10:37:59.000000 cdk-opinionated-constructs-2.0.1/test/stacks/lmb_docker_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3590 2022-11-25 10:57:28.000000 cdk-opinionated-constructs-2.0.1/test/stacks/lmb_monitoring_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2810 2023-04-20 10:37:59.000000 cdk-opinionated-constructs-2.0.1/test/stacks/lmb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2225 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.1/test/stacks/nlb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3290 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.0.1/test/stacks/rds_mysql_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3304 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.0.1/test/stacks/rds_postgresql_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1630 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.1/test/stacks/s3_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1108 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-2.0.1/test/stacks/sns_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2593 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.0.1/test/stacks/wafv2_stack.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-04-20 10:39:09.273664 cdk-opinionated-constructs-2.0.1/test/unit/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.0.1/test/unit/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1102 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.0.1/test/unit/test_alb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      701 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.0.1/test/unit/test_ecr_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1100 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.0.1/test/unit/test_lmb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      850 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.0.1/test/unit/test_s3_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      685 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.0.1/test/unit/test_sns_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1921 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.0.1/test/unit/test_wafv2_stack.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-05-19 08:38:33.401882 cdk-opinionated-constructs-2.1.0/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1071 2022-11-05 20:03:58.000000 cdk-opinionated-constructs-2.1.0/LICENSE
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      339 2023-05-19 08:38:33.402033 cdk-opinionated-constructs-2.1.0/PKG-INFO
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)    27443 2023-04-18 12:21:33.000000 cdk-opinionated-constructs-2.1.0/README.md
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-05-19 08:38:33.334492 cdk-opinionated-constructs-2.1.0/cdk_opinionated_constructs/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)       50 2022-11-05 21:10:53.000000 cdk-opinionated-constructs-2.1.0/cdk_opinionated_constructs/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     4879 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.0/cdk_opinionated_constructs/alb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2235 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-2.1.0/cdk_opinionated_constructs/ecr.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     8661 2023-04-20 10:19:32.000000 cdk-opinionated-constructs-2.1.0/cdk_opinionated_constructs/lmb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     5811 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.0/cdk_opinionated_constructs/nlb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     4643 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.1.0/cdk_opinionated_constructs/rds_instance.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3160 2023-05-19 08:35:31.000000 cdk-opinionated-constructs-2.1.0/cdk_opinionated_constructs/s3.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1464 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-2.1.0/cdk_opinionated_constructs/sns.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)    11940 2022-12-03 22:01:00.000000 cdk-opinionated-constructs-2.1.0/cdk_opinionated_constructs/wafv2.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-05-19 08:38:33.400698 cdk-opinionated-constructs-2.1.0/cdk_opinionated_constructs.egg-info/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      339 2023-05-19 08:38:33.000000 cdk-opinionated-constructs-2.1.0/cdk_opinionated_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1221 2023-05-19 08:38:33.000000 cdk-opinionated-constructs-2.1.0/cdk_opinionated_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        1 2023-05-19 08:38:33.000000 cdk-opinionated-constructs-2.1.0/cdk_opinionated_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)       89 2023-05-19 08:38:33.000000 cdk-opinionated-constructs-2.1.0/cdk_opinionated_constructs.egg-info/requires.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)       32 2023-05-19 08:38:33.000000 cdk-opinionated-constructs-2.1.0/cdk_opinionated_constructs.egg-info/top_level.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3649 2023-05-19 08:38:33.402884 cdk-opinionated-constructs-2.1.0/setup.cfg
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      760 2023-05-19 07:37:49.000000 cdk-opinionated-constructs-2.1.0/setup.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-05-19 08:38:33.335297 cdk-opinionated-constructs-2.1.0/test/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.1.0/test/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1781 2023-04-20 10:28:48.000000 cdk-opinionated-constructs-2.1.0/test/app.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-05-19 08:38:33.371305 cdk-opinionated-constructs-2.1.0/test/stacks/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.1.0/test/stacks/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2322 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.0/test/stacks/alb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1012 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-2.1.0/test/stacks/ecr_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3241 2023-04-20 10:37:59.000000 cdk-opinionated-constructs-2.1.0/test/stacks/lmb_docker_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3590 2022-11-25 10:57:28.000000 cdk-opinionated-constructs-2.1.0/test/stacks/lmb_monitoring_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2810 2023-04-20 10:37:59.000000 cdk-opinionated-constructs-2.1.0/test/stacks/lmb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2225 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.0/test/stacks/nlb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3290 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.1.0/test/stacks/rds_mysql_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3304 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.1.0/test/stacks/rds_postgresql_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1630 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.0/test/stacks/s3_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1108 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-2.1.0/test/stacks/sns_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2593 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.0/test/stacks/wafv2_stack.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-05-19 08:38:33.375294 cdk-opinionated-constructs-2.1.0/test/unit/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.1.0/test/unit/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1102 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.0/test/unit/test_alb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      701 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.0/test/unit/test_ecr_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1100 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.0/test/unit/test_lmb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      850 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.0/test/unit/test_s3_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      685 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.0/test/unit/test_sns_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1921 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.0/test/unit/test_wafv2_stack.py
```

### Comparing `cdk-opinionated-constructs-2.0.1/LICENSE` & `cdk-opinionated-constructs-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/README.md` & `cdk-opinionated-constructs-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/alb.py` & `cdk-opinionated-constructs-2.1.0/cdk_opinionated_constructs/alb.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/ecr.py` & `cdk-opinionated-constructs-2.1.0/cdk_opinionated_constructs/ecr.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/lmb.py` & `cdk-opinionated-constructs-2.1.0/cdk_opinionated_constructs/lmb.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/nlb.py` & `cdk-opinionated-constructs-2.1.0/cdk_opinionated_constructs/nlb.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/rds_instance.py` & `cdk-opinionated-constructs-2.1.0/cdk_opinionated_constructs/rds_instance.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/s3.py` & `cdk-opinionated-constructs-2.1.0/cdk_opinionated_constructs/s3.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 """Opinionated CDK construct to create S3 bucket.
 
 Security parameters are set by default
 """
 from constructs import Construct
 import aws_cdk as cdk
 import aws_cdk.aws_s3 as s3
-from aws_cdk import aws_kms as kms
+import aws_cdk.aws_kms as kms
+import aws_cdk.aws_iam as iam
+
 
 from typing import Optional
 
 
 class S3Bucket(Construct):
     """Create opinionated S3 bucket including restricted public access,
     enforced encryption in transit as well as in rest, versioning and lifecycle
@@ -28,44 +30,41 @@
 
     def create_bucket(
         self,
         bucket_name: str,
         encryption: s3.BucketEncryption,
         kms_key: Optional[kms.IKey] = None,
         server_access_logs_bucket: Optional[s3.IBucket] = None,
-        enforce_ssl: bool = True,
         **kwargs,
     ) -> s3.Bucket:
         """Create S3 bucket.
 
         :param encryption: The type of encryption.
         :param kms_key: The kms to be used.
         :param bucket_name: The name of S3 bucket.
-        :param enforce_ssl: Bool value if SSL should be enforced.
         :param server_access_logs_bucket: The CDK object for S3 bucket.
         :param kwargs:
          event_bridge_enabled: bool - set to True if s3 events should be sent to event bridge
          server_access_logs_prefix: str - in which prefix logs should be stored
         :return: The S3 bucket CDK object
         """
 
-        return s3.Bucket(
+        bucket = s3.Bucket(
             self,
             id=bucket_name,
             auto_delete_objects=True,
             block_public_access=s3.BlockPublicAccess(
                 block_public_acls=True,
                 block_public_policy=True,
                 ignore_public_acls=True,
                 restrict_public_buckets=True,
             ),
             bucket_name=bucket_name,
             encryption=encryption,
             encryption_key=kms_key,
-            enforce_ssl=enforce_ssl,
             event_bridge_enabled=bool(kwargs.get("event_bridge_enabled")),
             lifecycle_rules=[
                 s3.LifecycleRule(
                     enabled=True,
                     noncurrent_version_expiration=cdk.Duration.days(amount=1),
                 ),
                 s3.LifecycleRule(
@@ -76,7 +75,20 @@
             ],
             public_read_access=False,
             removal_policy=cdk.RemovalPolicy.DESTROY,
             server_access_logs_prefix=kwargs.get("server_access_logs_prefix"),
             server_access_logs_bucket=server_access_logs_bucket,
             versioned=True,
         )
+
+        bucket.add_to_resource_policy(
+            iam.PolicyStatement(
+                sid="EnforceTLSv12orHigher",
+                principals=[iam.AnyPrincipal()],
+                actions=["*"],
+                effect=iam.Effect.DENY,
+                resources=[bucket.bucket_arn, f"{bucket.bucket_arn}/*"],
+                conditions={"Bool": {"aws:SecureTransport": "true"}, "NumericLessThan": {"s3:TlsVersion": 1.2}},
+            )
+        )
+
+        return bucket
```

### Comparing `cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/sns.py` & `cdk-opinionated-constructs-2.1.0/cdk_opinionated_constructs/sns.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs/wafv2.py` & `cdk-opinionated-constructs-2.1.0/cdk_opinionated_constructs/wafv2.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/cdk_opinionated_constructs.egg-info/SOURCES.txt` & `cdk-opinionated-constructs-2.1.0/cdk_opinionated_constructs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/setup.cfg` & `cdk-opinionated-constructs-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/setup.py` & `cdk-opinionated-constructs-2.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 https://packaging.python.org/en/latest/distributing.html
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name="cdk-opinionated-constructs",
-    version="2.0.1",
+    version="2.1.0",
     description="AWS CDK constructs come without added security configurations.",
     long_description="The idea behind this project is to create secured constructs from the start. \n"
     "Supported constructs: ALB, ECR, LMB, NLB, S3, SNS, WAF, RDS",
     license="MIT",
     package_dir={"": "."},
     packages=find_packages(where="."),
     install_requires=[
```

### Comparing `cdk-opinionated-constructs-2.0.1/test/app.py` & `cdk-opinionated-constructs-2.1.0/test/app.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/test/stacks/alb_stack.py` & `cdk-opinionated-constructs-2.1.0/test/stacks/alb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/test/stacks/ecr_stack.py` & `cdk-opinionated-constructs-2.1.0/test/stacks/ecr_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/test/stacks/lmb_docker_stack.py` & `cdk-opinionated-constructs-2.1.0/test/stacks/lmb_docker_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/test/stacks/lmb_monitoring_stack.py` & `cdk-opinionated-constructs-2.1.0/test/stacks/lmb_monitoring_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/test/stacks/lmb_stack.py` & `cdk-opinionated-constructs-2.1.0/test/stacks/lmb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/test/stacks/nlb_stack.py` & `cdk-opinionated-constructs-2.1.0/test/stacks/nlb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/test/stacks/rds_mysql_stack.py` & `cdk-opinionated-constructs-2.1.0/test/stacks/rds_mysql_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/test/stacks/rds_postgresql_stack.py` & `cdk-opinionated-constructs-2.1.0/test/stacks/rds_postgresql_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/test/stacks/s3_stack.py` & `cdk-opinionated-constructs-2.1.0/test/stacks/s3_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/test/stacks/sns_stack.py` & `cdk-opinionated-constructs-2.1.0/test/stacks/sns_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/test/stacks/wafv2_stack.py` & `cdk-opinionated-constructs-2.1.0/test/stacks/wafv2_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/test/unit/test_alb_stack.py` & `cdk-opinionated-constructs-2.1.0/test/unit/test_alb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/test/unit/test_ecr_stack.py` & `cdk-opinionated-constructs-2.1.0/test/unit/test_ecr_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/test/unit/test_lmb_stack.py` & `cdk-opinionated-constructs-2.1.0/test/unit/test_lmb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/test/unit/test_s3_stack.py` & `cdk-opinionated-constructs-2.1.0/test/unit/test_s3_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/test/unit/test_sns_stack.py` & `cdk-opinionated-constructs-2.1.0/test/unit/test_sns_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.0.1/test/unit/test_wafv2_stack.py` & `cdk-opinionated-constructs-2.1.0/test/unit/test_wafv2_stack.py`

 * *Files identical despite different names*

