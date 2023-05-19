# Comparing `tmp/prancer-basic-3.0.5.tar.gz` & `tmp/prancer-basic-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prancer-basic-3.0.5.tar", last modified: Fri May  5 11:39:43 2023, max compression
+gzip compressed data, was "prancer-basic-3.0.6.tar", last modified: Fri May 19 13:44:29 2023, max compression
```

## Comparing `prancer-basic-3.0.5.tar` & `prancer-basic-3.0.6.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.901557 prancer-basic-3.0.5/
--rwxrwxrwx   0 runner    (1001) docker     (123)    16725 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/LICENSE
--rwxrwxrwx   0 runner    (1001) docker     (123)       57 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/PKG-INFO
--rwxrwxrwx   0 runner    (1001) docker     (123)     6966 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 11:39:43.901557 prancer-basic-3.0.5/setup.cfg
--rwxrwxrwx   0 runner    (1001) docker     (123)     1890 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.881557 prancer-basic-3.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.885557 prancer-basic-3.0.5/src/prancer_basic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-05 11:39:43.000000 prancer-basic-3.0.5/src/prancer_basic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-05 11:39:43.000000 prancer-basic-3.0.5/src/prancer_basic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:39:43.000000 prancer-basic-3.0.5/src/prancer_basic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-05 11:39:43.000000 prancer-basic-3.0.5/src/prancer_basic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-05 11:39:43.000000 prancer-basic-3.0.5/src/prancer_basic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 11:39:43.000000 prancer-basic-3.0.5/src/prancer_basic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.885557 prancer-basic-3.0.5/src/processor/
--rwxrwxrwx   0 runner    (1001) docker     (123)       39 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.885557 prancer-basic-3.0.5/src/processor/collection_config/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/collection_config/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     6485 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/collection_config/config_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.885557 prancer-basic-3.0.5/src/processor/comparison/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2524 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/comparison_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.885557 prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    13229 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/comparatorLexer.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      655 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/comparatorListener.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    28827 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/comparatorParser.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2224 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/compare_types.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    19688 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/rule_interpreter.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1641 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/test_comparator.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    39624 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.885557 prancer-basic-3.0.5/src/processor/comparison/rules/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.885557 prancer-basic-3.0.5/src/processor/comparison/rules/arm/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/rules/arm/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     7732 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/rules/arm/secret_azure_iac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.885557 prancer-basic-3.0.5/src/processor/comparison/rules/cloudformation/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/rules/cloudformation/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    21971 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/rules/cloudformation/secret_aws_iac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.889557 prancer-basic-3.0.5/src/processor/comparison/rules/common/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/rules/common/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      863 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/rules/common/sensitive_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.889557 prancer-basic-3.0.5/src/processor/comparison/rules/deploymentmanager/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/rules/deploymentmanager/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    21900 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/rules/deploymentmanager/secret_gcp_iac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.889557 prancer-basic-3.0.5/src/processor/comparison/rules/terraform/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/rules/terraform/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    38629 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/comparison/rules/terraform/secret_tf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.889557 prancer-basic-3.0.5/src/processor/connector/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1557 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/arn_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.889557 prancer-basic-3.0.5/src/processor/connector/git_connector/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/git_connector/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     7243 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/git_connector/git_functions.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    10890 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/git_connector/git_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    10831 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/populate_json.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    19921 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    58392 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot_aws.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    23681 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot_azure.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    11475 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot_azure_refactor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     5593 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot_base.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    23145 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot_custom.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    16164 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot_custom_refactor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     6353 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot_db.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      265 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot_exception.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     6721 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot_fs.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    33285 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot_google.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    26211 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot_kubernetes.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2367 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/snapshot_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.889557 prancer-basic-3.0.5/src/processor/connector/special_compliance/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/special_compliance/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1717 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/special_compliance/compliances.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.889557 prancer-basic-3.0.5/src/processor/connector/special_crawler/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/special_crawler/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     4256 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/special_crawler/azure_crawler.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      416 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/special_crawler/base_crawler.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    34555 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/validation.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     7256 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/connector/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.889557 prancer-basic-3.0.5/src/processor/crawler/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/crawler/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    24954 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/crawler/master_snapshot.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    13961 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/crawler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/database/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/database/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     9830 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/database/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/helper/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/helper/config/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/config/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     5203 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/config/config_utils.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     5311 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/config/remote_utils.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     5181 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/config/rundata_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/helper/file/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/file/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1090 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/file/file_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/helper/hcl/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/hcl/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      927 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/hcl/hcl_utils.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      893 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/hcl/parser.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      301 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/hcl/transformer.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    21915 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/hcl/yacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/helper/httpapi/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/httpapi/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     5822 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/httpapi/http_utils.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     3094 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/httpapi/restapi.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    14551 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/httpapi/restapi_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/helper/jinja/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/jinja/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     3383 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/jinja/jinja_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/helper/json/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/json/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     7147 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/json/commentjson.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     8248 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/json/json_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/helper/utils/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/utils/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      715 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/utils/cli_generate_azure_vault_key.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    14311 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/utils/cli_populate_json.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1620 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/utils/cli_terraform_to_json.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    29976 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/utils/cli_validator.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    10769 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/utils/compliance_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/helper/utils/jinjatemplates/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/utils/jinjatemplates/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      147 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/utils/jinjatemplates/fs_connector.json
--rwxrwxrwx   0 runner    (1001) docker     (123)      212 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/utils/jinjatemplates/git_connector.json
--rwxrwxrwx   0 runner    (1001) docker     (123)      461 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/utils/jinjatemplates/mastersnapshot.json
--rwxrwxrwx   0 runner    (1001) docker     (123)      236 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/utils/jinjatemplates/mastertest.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/helper/yaml/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/yaml/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2516 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/helper/yaml/yaml_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/logging/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/logging/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     5625 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/logging/dburl_kv.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    16365 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/logging/log_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.893557 prancer-basic-3.0.5/src/processor/reporting/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/reporting/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     4672 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/reporting/json_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/template_processor/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1777 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/ack_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1777 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/aso_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     4053 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/aws_template_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     6180 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/azure_template_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/template_processor/base/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/base/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1675 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/base/base_template_constatns.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    33402 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/base/base_template_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2181 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/google_template_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2245 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/helm_chart_template_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1989 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/json_template_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1777 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/kcc_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2295 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/kubernetes_template_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     5778 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/terraform_template_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2026 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/template_processor/yaml_template_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/templates/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/templates/aws/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/aws/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    14373 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/aws/aws_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/templates/azure/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/azure/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    17363 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/azure/azure_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/templates/base/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/base/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     3483 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/base/template_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/templates/google/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/google/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     8857 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/google/google_parser.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2549 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/google/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/templates/helm/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/helm/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      935 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/helm/helm_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/templates/kubernetes/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/kubernetes/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1275 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/kubernetes/kubernetes_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/templates/terraform/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/templates/terraform/helper/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/helper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/templates/terraform/helper/expression/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/helper/expression/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      912 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/helper/expression/base_expressions.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      195 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/helper/expression/terraform_expressions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:43.897557 prancer-basic-3.0.5/src/processor/templates/terraform/helper/function/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/helper/function/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     3995 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/helper/function/collection_functions.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      755 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/helper/function/encoding_function.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1119 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/helper/function/numeric_functions.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2257 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/helper/function/string_functions.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     3829 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/helper/function/terraform_functions.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     3490 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/helper/module_parser.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    52928 2023-05-05 11:37:23.000000 prancer-basic-3.0.5/src/processor/templates/terraform/terraform_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.491254 prancer-basic-3.0.6/
+-rwxrwxrwx   0 runner    (1001) docker     (123)    16725 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/LICENSE
+-rwxrwxrwx   0 runner    (1001) docker     (123)       57 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-19 13:44:29.491254 prancer-basic-3.0.6/PKG-INFO
+-rwxrwxrwx   0 runner    (1001) docker     (123)     6966 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 13:44:29.491254 prancer-basic-3.0.6/setup.cfg
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1890 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.475254 prancer-basic-3.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.475254 prancer-basic-3.0.6/src/prancer_basic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-19 13:44:29.000000 prancer-basic-3.0.6/src/prancer_basic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-19 13:44:29.000000 prancer-basic-3.0.6/src/prancer_basic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 13:44:29.000000 prancer-basic-3.0.6/src/prancer_basic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-19 13:44:29.000000 prancer-basic-3.0.6/src/prancer_basic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-19 13:44:29.000000 prancer-basic-3.0.6/src/prancer_basic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 13:44:29.000000 prancer-basic-3.0.6/src/prancer_basic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.479254 prancer-basic-3.0.6/src/processor/
+-rwxrwxrwx   0 runner    (1001) docker     (123)       39 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.479254 prancer-basic-3.0.6/src/processor/collection_config/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/collection_config/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     6485 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/collection_config/config_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.479254 prancer-basic-3.0.6/src/processor/comparison/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/comparison/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2524 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/comparison/comparison_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.479254 prancer-basic-3.0.6/src/processor/comparison/comparisonantlr/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/comparison/comparisonantlr/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    13229 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/comparison/comparisonantlr/comparatorLexer.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      655 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/comparison/comparisonantlr/comparatorListener.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    28827 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/comparison/comparisonantlr/comparatorParser.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2224 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/comparison/comparisonantlr/compare_types.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    19688 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/comparison/comparisonantlr/rule_interpreter.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1641 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/comparison/comparisonantlr/test_comparator.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    39624 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/comparison/interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.479254 prancer-basic-3.0.6/src/processor/comparison/rules/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/comparison/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.479254 prancer-basic-3.0.6/src/processor/comparison/rules/arm/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/comparison/rules/arm/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     7732 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/comparison/rules/arm/secret_azure_iac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.479254 prancer-basic-3.0.6/src/processor/comparison/rules/cloudformation/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/comparison/rules/cloudformation/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    21971 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/comparison/rules/cloudformation/secret_aws_iac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.479254 prancer-basic-3.0.6/src/processor/comparison/rules/common/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/comparison/rules/common/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      863 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/comparison/rules/common/sensitive_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.479254 prancer-basic-3.0.6/src/processor/comparison/rules/deploymentmanager/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/comparison/rules/deploymentmanager/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    21900 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/comparison/rules/deploymentmanager/secret_gcp_iac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.479254 prancer-basic-3.0.6/src/processor/comparison/rules/terraform/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/comparison/rules/terraform/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    38629 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/comparison/rules/terraform/secret_tf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.483254 prancer-basic-3.0.6/src/processor/connector/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1557 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/arn_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.483254 prancer-basic-3.0.6/src/processor/connector/git_connector/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/git_connector/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     7243 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/git_connector/git_functions.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    10890 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/git_connector/git_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    10831 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/populate_json.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    19921 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/snapshot.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    58392 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/snapshot_aws.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    23681 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/snapshot_azure.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    11475 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/snapshot_azure_refactor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     5593 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/snapshot_base.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    23145 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/snapshot_custom.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    16164 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/snapshot_custom_refactor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     6353 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/snapshot_db.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      265 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/snapshot_exception.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     6721 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/snapshot_fs.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    33187 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/snapshot_google.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    26211 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/snapshot_kubernetes.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2367 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/snapshot_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.483254 prancer-basic-3.0.6/src/processor/connector/special_compliance/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/special_compliance/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1717 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/special_compliance/compliances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.483254 prancer-basic-3.0.6/src/processor/connector/special_crawler/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/special_crawler/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     4256 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/special_crawler/azure_crawler.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      416 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/special_crawler/base_crawler.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    34555 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/validation.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     7256 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/connector/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.483254 prancer-basic-3.0.6/src/processor/crawler/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/crawler/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    24954 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/crawler/master_snapshot.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    13969 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/crawler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.483254 prancer-basic-3.0.6/src/processor/database/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/database/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     9830 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/database/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.483254 prancer-basic-3.0.6/src/processor/helper/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.483254 prancer-basic-3.0.6/src/processor/helper/config/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/config/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     5203 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/config/config_utils.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     5311 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/config/remote_utils.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     5181 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/config/rundata_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.483254 prancer-basic-3.0.6/src/processor/helper/file/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/file/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1090 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/file/file_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.483254 prancer-basic-3.0.6/src/processor/helper/hcl/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/hcl/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      927 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/hcl/hcl_utils.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      893 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/hcl/parser.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      301 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/hcl/transformer.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    21915 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/hcl/yacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.483254 prancer-basic-3.0.6/src/processor/helper/httpapi/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/httpapi/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     5822 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/httpapi/http_utils.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     3094 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/httpapi/restapi.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    14551 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/httpapi/restapi_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.483254 prancer-basic-3.0.6/src/processor/helper/jinja/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/jinja/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     3383 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/jinja/jinja_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.483254 prancer-basic-3.0.6/src/processor/helper/json/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/json/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     7147 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/json/commentjson.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     8248 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/json/json_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.487254 prancer-basic-3.0.6/src/processor/helper/utils/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/utils/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      715 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/utils/cli_generate_azure_vault_key.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    14311 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/utils/cli_populate_json.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1620 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/utils/cli_terraform_to_json.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    29976 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/utils/cli_validator.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    10769 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/utils/compliance_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.487254 prancer-basic-3.0.6/src/processor/helper/utils/jinjatemplates/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/utils/jinjatemplates/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      147 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/utils/jinjatemplates/fs_connector.json
+-rwxrwxrwx   0 runner    (1001) docker     (123)      212 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/utils/jinjatemplates/git_connector.json
+-rwxrwxrwx   0 runner    (1001) docker     (123)      461 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/utils/jinjatemplates/mastersnapshot.json
+-rwxrwxrwx   0 runner    (1001) docker     (123)      236 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/utils/jinjatemplates/mastertest.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.487254 prancer-basic-3.0.6/src/processor/helper/yaml/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/yaml/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2516 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/helper/yaml/yaml_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.487254 prancer-basic-3.0.6/src/processor/logging/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/logging/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     5625 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/logging/dburl_kv.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    16365 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/logging/log_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.487254 prancer-basic-3.0.6/src/processor/reporting/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/reporting/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     4672 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/reporting/json_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.487254 prancer-basic-3.0.6/src/processor/template_processor/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/template_processor/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1777 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/template_processor/ack_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1777 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/template_processor/aso_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     4053 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/template_processor/aws_template_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     6180 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/template_processor/azure_template_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.487254 prancer-basic-3.0.6/src/processor/template_processor/base/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/template_processor/base/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1675 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/template_processor/base/base_template_constatns.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    33402 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/template_processor/base/base_template_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2181 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/template_processor/google_template_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2245 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/template_processor/helm_chart_template_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1989 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/template_processor/json_template_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1777 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/template_processor/kcc_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2295 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/template_processor/kubernetes_template_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     5778 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/template_processor/terraform_template_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2026 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/template_processor/yaml_template_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.487254 prancer-basic-3.0.6/src/processor/templates/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.487254 prancer-basic-3.0.6/src/processor/templates/aws/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/aws/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    14373 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/aws/aws_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.487254 prancer-basic-3.0.6/src/processor/templates/azure/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/azure/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    17363 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/azure/azure_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.487254 prancer-basic-3.0.6/src/processor/templates/base/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/base/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     3483 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/base/template_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.487254 prancer-basic-3.0.6/src/processor/templates/google/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/google/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     8857 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/google/google_parser.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2549 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/google/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.487254 prancer-basic-3.0.6/src/processor/templates/helm/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/helm/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      935 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/helm/helm_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.487254 prancer-basic-3.0.6/src/processor/templates/kubernetes/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/kubernetes/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1275 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/kubernetes/kubernetes_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.491254 prancer-basic-3.0.6/src/processor/templates/terraform/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/terraform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.491254 prancer-basic-3.0.6/src/processor/templates/terraform/helper/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/terraform/helper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.491254 prancer-basic-3.0.6/src/processor/templates/terraform/helper/expression/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/terraform/helper/expression/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      912 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/terraform/helper/expression/base_expressions.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      195 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/terraform/helper/expression/terraform_expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:44:29.491254 prancer-basic-3.0.6/src/processor/templates/terraform/helper/function/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/terraform/helper/function/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     3995 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/terraform/helper/function/collection_functions.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      755 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/terraform/helper/function/encoding_function.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1119 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/terraform/helper/function/numeric_functions.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2257 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/terraform/helper/function/string_functions.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     3829 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/terraform/helper/function/terraform_functions.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     3490 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/terraform/helper/module_parser.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    52928 2023-05-19 13:42:00.000000 prancer-basic-3.0.6/src/processor/templates/terraform/terraform_parser.py
```

### Comparing `prancer-basic-3.0.5/LICENSE` & `prancer-basic-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/PKG-INFO` & `prancer-basic-3.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: prancer-basic
-Version: 3.0.5
+Version: 3.0.6
 Summary: Prancer Basic, http://prancer.io/
 Home-page: https://github.com/prancer-io/cloud-validation-framework
 Author: Farshid M/Ajey Khanapuri
 Author-email: ajey.khanapuri@liquware.com
 License: BSD
 Description: 
          Prancer Basic allows to users to run cloud validation.
```

### Comparing `prancer-basic-3.0.5/README.md` & `prancer-basic-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/setup.py` & `prancer-basic-3.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  Prancer Basic allows to users to run cloud validation.
  The supported cloud frameworks are azure, aws and git.
 """
 
 setup(
     name='prancer-basic',
     # also update the version in processor.__init__.py file
-    version='3.0.5',
+    version='3.0.6',
     description='Prancer Basic, http://prancer.io/',
     long_description=LONG_DESCRIPTION,
     license = "BSD",
     # The project's main homepage.
     url='https://github.com/prancer-io/cloud-validation-framework',
     # Author(s) details
     author='Farshid M/Ajey Khanapuri',
```

### Comparing `prancer-basic-3.0.5/src/prancer_basic.egg-info/PKG-INFO` & `prancer-basic-3.0.6/src/prancer_basic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: prancer-basic
-Version: 3.0.5
+Version: 3.0.6
 Summary: Prancer Basic, http://prancer.io/
 Home-page: https://github.com/prancer-io/cloud-validation-framework
 Author: Farshid M/Ajey Khanapuri
 Author-email: ajey.khanapuri@liquware.com
 License: BSD
 Description: 
          Prancer Basic allows to users to run cloud validation.
```

### Comparing `prancer-basic-3.0.5/src/prancer_basic.egg-info/SOURCES.txt` & `prancer-basic-3.0.6/src/prancer_basic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/prancer_basic.egg-info/requires.txt` & `prancer-basic-3.0.6/src/prancer_basic.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/collection_config/config_handler.py` & `prancer-basic-3.0.6/src/processor/collection_config/config_handler.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/comparison/comparison_functions.py` & `prancer-basic-3.0.6/src/processor/comparison/comparison_functions.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/comparatorLexer.py` & `prancer-basic-3.0.6/src/processor/comparison/comparisonantlr/comparatorLexer.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/comparatorListener.py` & `prancer-basic-3.0.6/src/processor/comparison/comparisonantlr/comparatorListener.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/comparatorParser.py` & `prancer-basic-3.0.6/src/processor/comparison/comparisonantlr/comparatorParser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/compare_types.py` & `prancer-basic-3.0.6/src/processor/comparison/comparisonantlr/compare_types.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/rule_interpreter.py` & `prancer-basic-3.0.6/src/processor/comparison/comparisonantlr/rule_interpreter.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/comparison/comparisonantlr/test_comparator.py` & `prancer-basic-3.0.6/src/processor/comparison/comparisonantlr/test_comparator.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/comparison/interpreter.py` & `prancer-basic-3.0.6/src/processor/comparison/interpreter.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/comparison/rules/arm/secret_azure_iac.py` & `prancer-basic-3.0.6/src/processor/comparison/rules/arm/secret_azure_iac.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/comparison/rules/cloudformation/secret_aws_iac.py` & `prancer-basic-3.0.6/src/processor/comparison/rules/cloudformation/secret_aws_iac.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/comparison/rules/common/sensitive_extension.py` & `prancer-basic-3.0.6/src/processor/comparison/rules/common/sensitive_extension.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/comparison/rules/deploymentmanager/secret_gcp_iac.py` & `prancer-basic-3.0.6/src/processor/comparison/rules/deploymentmanager/secret_gcp_iac.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/comparison/rules/terraform/secret_tf.py` & `prancer-basic-3.0.6/src/processor/comparison/rules/terraform/secret_tf.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/connector/arn_parser.py` & `prancer-basic-3.0.6/src/processor/connector/arn_parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/connector/git_connector/git_functions.py` & `prancer-basic-3.0.6/src/processor/connector/git_connector/git_functions.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/connector/git_connector/git_processor.py` & `prancer-basic-3.0.6/src/processor/connector/git_connector/git_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/connector/populate_json.py` & `prancer-basic-3.0.6/src/processor/connector/populate_json.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/connector/snapshot.py` & `prancer-basic-3.0.6/src/processor/connector/snapshot.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/connector/snapshot_aws.py` & `prancer-basic-3.0.6/src/processor/connector/snapshot_aws.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/connector/snapshot_azure.py` & `prancer-basic-3.0.6/src/processor/connector/snapshot_azure.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/connector/snapshot_azure_refactor.py` & `prancer-basic-3.0.6/src/processor/connector/snapshot_azure_refactor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/connector/snapshot_base.py` & `prancer-basic-3.0.6/src/processor/connector/snapshot_base.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/connector/snapshot_custom.py` & `prancer-basic-3.0.6/src/processor/connector/snapshot_custom.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/connector/snapshot_custom_refactor.py` & `prancer-basic-3.0.6/src/processor/connector/snapshot_custom_refactor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/connector/snapshot_db.py` & `prancer-basic-3.0.6/src/processor/connector/snapshot_db.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/connector/snapshot_fs.py` & `prancer-basic-3.0.6/src/processor/connector/snapshot_fs.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/connector/snapshot_google.py` & `prancer-basic-3.0.6/src/processor/connector/snapshot_google.py`

 * *Files 0% similar despite different names*

```diff
@@ -621,22 +621,21 @@
     project_id = get_field_value(snapshot, 'project-id')
     sub_data = get_google_data(snapshot_source, container)
     snapshot_nodes = get_field_value(snapshot, 'nodes')
     snapshot_data, valid_snapshotids = validate_snapshot_nodes(snapshot_nodes)
     if valid_snapshotids and sub_data and snapshot_nodes:
         logger.debug(sub_data)
         try:
+            credentials = get_google_client_data(sub_data, snapshot_user, "", project_id)
+            if not credentials:
+                logger.info("No  GCE connection in the snapshot to access Google resource!...")
+                return snapshot_data
             for node in snapshot['nodes']:
                 validate = node['validate'] if 'validate' in node else True
                 logger.info(node)
-                node_type = get_field_value_with_default(node, 'type',"")
-                credentials = get_google_client_data(sub_data, snapshot_user, node_type, project_id)
-                if not credentials:
-                    logger.info("No  GCE connection in the snapshot to access Google resource!...")
-                    return snapshot_data
                 if 'snapshotId' in node:
                     if validate:
                         data = get_node(credentials, node, snapshot_source, snapshot)
                         if data:
                             error_str = data.pop('error', None)
                             if get_dbtests():
                                 if get_collection_size(data['collection']) == 0:
```

### Comparing `prancer-basic-3.0.5/src/processor/connector/snapshot_kubernetes.py` & `prancer-basic-3.0.6/src/processor/connector/snapshot_kubernetes.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/connector/snapshot_utils.py` & `prancer-basic-3.0.6/src/processor/connector/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/connector/special_compliance/compliances.py` & `prancer-basic-3.0.6/src/processor/connector/special_compliance/compliances.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/connector/special_crawler/azure_crawler.py` & `prancer-basic-3.0.6/src/processor/connector/special_crawler/azure_crawler.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/connector/validation.py` & `prancer-basic-3.0.6/src/processor/connector/validation.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/connector/vault.py` & `prancer-basic-3.0.6/src/processor/connector/vault.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/crawler/master_snapshot.py` & `prancer-basic-3.0.6/src/processor/crawler/master_snapshot.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/crawler/utils.py` & `prancer-basic-3.0.6/src/processor/crawler/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         if project.get("users") and str(project.get("all-accounts")).lower() == "true":
             all_account = True
             user = project["users"][0]
             client_email = user["client_email"]
             client_id = user["client_id"]
             private_key_id = user["private_key_id"]
             name = user["name"]
-            private_key = user["private_key"]
+            private_key = user.get("private_key")
             name = re.sub(r"-\d+$", "", name)
             account_list += get_projects_list(private_key_id, private_key, client_email, client_id, name)
     updated_data = copy.deepcopy(structure_data)
     updated_data["projects"] = account_list
     update_collection_data(container, source, updated_data, dbname, collection)
     return account_list, all_account
 
@@ -197,15 +197,15 @@
     project_list = []
     if not private_key:
         new_private_key = get_vault_data(private_key_id)
     else:
         new_private_key = private_key
 
     if new_private_key:
-        access_token = access_token_from_service_account(private_key_id, private_key, client_email, client_id)
+        access_token = access_token_from_service_account(private_key_id, new_private_key, client_email, client_id)
         if access_token:
             hdrs = {"Accept": "application/json", "Authorization": "Bearer %s" % access_token }
             url = "https://cloudresourcemanager.googleapis.com/v1/projects"
             resp = requests.get(url, headers=hdrs)
             if resp.status_code == 200:
                 projectData = resp.json()
                 if projectData and  'projects' in projectData:
```

### Comparing `prancer-basic-3.0.5/src/processor/database/database.py` & `prancer-basic-3.0.6/src/processor/database/database.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/helper/config/config_utils.py` & `prancer-basic-3.0.6/src/processor/helper/config/config_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/helper/config/remote_utils.py` & `prancer-basic-3.0.6/src/processor/helper/config/remote_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/helper/config/rundata_utils.py` & `prancer-basic-3.0.6/src/processor/helper/config/rundata_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/helper/file/file_utils.py` & `prancer-basic-3.0.6/src/processor/helper/file/file_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/helper/hcl/hcl_utils.py` & `prancer-basic-3.0.6/src/processor/helper/hcl/hcl_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/helper/hcl/parser.py` & `prancer-basic-3.0.6/src/processor/helper/hcl/parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/helper/hcl/yacc.py` & `prancer-basic-3.0.6/src/processor/helper/hcl/yacc.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/helper/httpapi/http_utils.py` & `prancer-basic-3.0.6/src/processor/helper/httpapi/http_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/helper/httpapi/restapi.py` & `prancer-basic-3.0.6/src/processor/helper/httpapi/restapi.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/helper/httpapi/restapi_azure.py` & `prancer-basic-3.0.6/src/processor/helper/httpapi/restapi_azure.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/helper/jinja/jinja_utils.py` & `prancer-basic-3.0.6/src/processor/helper/jinja/jinja_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/helper/json/commentjson.py` & `prancer-basic-3.0.6/src/processor/helper/json/commentjson.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/helper/json/json_utils.py` & `prancer-basic-3.0.6/src/processor/helper/json/json_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/helper/utils/cli_generate_azure_vault_key.py` & `prancer-basic-3.0.6/src/processor/helper/utils/cli_generate_azure_vault_key.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/helper/utils/cli_populate_json.py` & `prancer-basic-3.0.6/src/processor/helper/utils/cli_populate_json.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/helper/utils/cli_terraform_to_json.py` & `prancer-basic-3.0.6/src/processor/helper/utils/cli_terraform_to_json.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/helper/utils/cli_validator.py` & `prancer-basic-3.0.6/src/processor/helper/utils/cli_validator.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/helper/utils/compliance_utils.py` & `prancer-basic-3.0.6/src/processor/helper/utils/compliance_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/helper/yaml/yaml_utils.py` & `prancer-basic-3.0.6/src/processor/helper/yaml/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/logging/dburl_kv.py` & `prancer-basic-3.0.6/src/processor/logging/dburl_kv.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/logging/log_handler.py` & `prancer-basic-3.0.6/src/processor/logging/log_handler.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/reporting/json_output.py` & `prancer-basic-3.0.6/src/processor/reporting/json_output.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/template_processor/ack_processor.py` & `prancer-basic-3.0.6/src/processor/template_processor/ack_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/template_processor/aso_processor.py` & `prancer-basic-3.0.6/src/processor/template_processor/aso_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/template_processor/aws_template_processor.py` & `prancer-basic-3.0.6/src/processor/template_processor/aws_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/template_processor/azure_template_processor.py` & `prancer-basic-3.0.6/src/processor/template_processor/azure_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/template_processor/base/base_template_constatns.py` & `prancer-basic-3.0.6/src/processor/template_processor/base/base_template_constatns.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/template_processor/base/base_template_processor.py` & `prancer-basic-3.0.6/src/processor/template_processor/base/base_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/template_processor/google_template_processor.py` & `prancer-basic-3.0.6/src/processor/template_processor/google_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/template_processor/helm_chart_template_processor.py` & `prancer-basic-3.0.6/src/processor/template_processor/helm_chart_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/template_processor/json_template_processor.py` & `prancer-basic-3.0.6/src/processor/template_processor/json_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/template_processor/kcc_processor.py` & `prancer-basic-3.0.6/src/processor/template_processor/kcc_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/template_processor/kubernetes_template_processor.py` & `prancer-basic-3.0.6/src/processor/template_processor/kubernetes_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/template_processor/terraform_template_processor.py` & `prancer-basic-3.0.6/src/processor/template_processor/terraform_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/template_processor/yaml_template_processor.py` & `prancer-basic-3.0.6/src/processor/template_processor/yaml_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/templates/aws/aws_parser.py` & `prancer-basic-3.0.6/src/processor/templates/aws/aws_parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/templates/azure/azure_parser.py` & `prancer-basic-3.0.6/src/processor/templates/azure/azure_parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/templates/base/template_parser.py` & `prancer-basic-3.0.6/src/processor/templates/base/template_parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/templates/google/google_parser.py` & `prancer-basic-3.0.6/src/processor/templates/google/google_parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/templates/google/util.py` & `prancer-basic-3.0.6/src/processor/templates/google/util.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/templates/helm/helm_parser.py` & `prancer-basic-3.0.6/src/processor/templates/helm/helm_parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/templates/kubernetes/kubernetes_parser.py` & `prancer-basic-3.0.6/src/processor/templates/kubernetes/kubernetes_parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/templates/terraform/helper/expression/base_expressions.py` & `prancer-basic-3.0.6/src/processor/templates/terraform/helper/expression/base_expressions.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/templates/terraform/helper/function/collection_functions.py` & `prancer-basic-3.0.6/src/processor/templates/terraform/helper/function/collection_functions.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/templates/terraform/helper/function/encoding_function.py` & `prancer-basic-3.0.6/src/processor/templates/terraform/helper/function/encoding_function.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/templates/terraform/helper/function/numeric_functions.py` & `prancer-basic-3.0.6/src/processor/templates/terraform/helper/function/numeric_functions.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/templates/terraform/helper/function/string_functions.py` & `prancer-basic-3.0.6/src/processor/templates/terraform/helper/function/string_functions.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/templates/terraform/helper/function/terraform_functions.py` & `prancer-basic-3.0.6/src/processor/templates/terraform/helper/function/terraform_functions.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/templates/terraform/helper/module_parser.py` & `prancer-basic-3.0.6/src/processor/templates/terraform/helper/module_parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.5/src/processor/templates/terraform/terraform_parser.py` & `prancer-basic-3.0.6/src/processor/templates/terraform/terraform_parser.py`

 * *Files identical despite different names*

