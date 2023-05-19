# Comparing `tmp/gempyp-1.0.70b0.tar.gz` & `tmp/gempyp-1.0.70b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gempyp-1.0.70b0.tar", max compression
+gzip compressed data, was "gempyp-1.0.70b1.tar", max compression
```

## Comparing `gempyp-1.0.70b0.tar` & `gempyp-1.0.70b1.tar`

### file list

```diff
@@ -1,94 +1,93 @@
--rw-r--r--   0        0        0      258 2023-05-05 14:21:56.330590 gempyp-1.0.70b0/gempyp/__init__.py
--rw-r--r--   0        0        0      155 2023-05-05 14:21:56.330590 gempyp-1.0.70b0/gempyp/Annotations.py
--rw-r--r--   0        0        0      108 2023-05-05 14:21:30.308048 gempyp-1.0.70b0/gempyp/cli.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.308048 gempyp-1.0.70b0/gempyp/config/__init__.py
--rw-r--r--   0        0        0     7387 2023-05-05 14:21:30.308048 gempyp-1.0.70b0/gempyp/config/baseConfig.py
--rw-r--r--   0        0        0      198 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/config/customParser.py
--rw-r--r--   0        0        0     1778 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/config/DefaultSettings.py
--rw-r--r--   0        0        0       62 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/config/gempyp.conf
--rw-r--r--   0        0        0     2145 2023-05-05 14:21:30.308048 gempyp-1.0.70b0/gempyp/config/GitLinkXML.py
--rw-r--r--   0        0        0    21143 2023-05-05 14:21:30.308048 gempyp-1.0.70b0/gempyp/config/Result.html
--rw-r--r--   0        0        0       26 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/config/suite_conf.json
--rw-r--r--   0        0        0       28 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/config/testcase_conf.json
--rw-r--r--   0        0        0     4007 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/config/xmlConfig.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/common/__init__.py
--rw-r--r--   0        0        0     3627 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/common/common_functions.py
--rw-r--r--   0        0        0      956 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/compare.py
--rw-r--r--   0        0        0      149 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/config/dvm.json
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/configurator/__init__.py
--rw-r--r--   0        0        0     4635 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/configurator/configurator.py
--rw-r--r--   0        0        0      320 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/configurator/validator.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/core/__init__.py
--rw-r--r--   0        0        0      589 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/core/comparator.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/core/Compare.py
--rw-r--r--   0        0        0    10157 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/core/python_obj_comparator.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/data/__init__.py
--rw-r--r--   0        0        0     5498 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/data/data.py
--rw-r--r--   0        0        0      869 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/data/database.py
--rw-r--r--   0        0        0     1903 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/data/db_mysql.py
--rw-r--r--   0        0        0     2646 2023-05-05 14:21:30.323318 gempyp-1.0.70b0/gempyp/data_compare/data/db_oracle.py
--rw-r--r--   0        0        0     2436 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/data_compare/data/db_postgre.py
--rw-r--r--   0        0        0     1999 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/data_compare/data/db_sqlite.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/data_compare/data/file_processor.py
--rw-r--r--   0        0        0    11161 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/data_compare/data_comp.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/data_compare/report/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/data_compare/tools/__init__.py
--rw-r--r--   0        0        0     3034 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/data_uploader.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/dv/__init__.py
--rw-r--r--   0        0        0     2285 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/dv/dfOperations.py
--rw-r--r--   0        0        0    10230 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/dv/dvCompare.py
--rw-r--r--   0        0        0      682 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/dv/dvDatabases.py
--rw-r--r--   0        0        0     9470 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/dv/dvDataframe.py
--rw-r--r--   0        0        0     1441 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/dv/dvObj.py
--rw-r--r--   0        0        0     3789 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/dv/dvReporting.py
--rw-r--r--   0        0        0    23248 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/dv/dvRunner.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/engine/__init__.py
--rw-r--r--   0        0        0     5092 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/engine/baseTemplate.py
--rw-r--r--   0        0        0     8414 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/engine/dataUpload.py
--rw-r--r--   0        0        0    40521 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/engine/engine.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.356805 gempyp-1.0.70b0/gempyp/engine/executors/__init__.py
--rw-r--r--   0        0        0      443 2023-05-05 14:21:30.372942 gempyp-1.0.70b0/gempyp/engine/executors/baseExecutor.py
--rw-r--r--   0        0        0      656 2023-05-05 14:21:30.373956 gempyp-1.0.70b0/gempyp/engine/gempypHelper.py
--rw-r--r--   0        0        0     5418 2023-05-05 14:21:30.374954 gempyp-1.0.70b0/gempyp/engine/runner.py
--rw-r--r--   0        0        0     5537 2023-05-05 14:21:30.374954 gempyp-1.0.70b0/gempyp/engine/simpleTestcase.py
--rw-r--r--   0        0        0    12428 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/engine/testData.py
--rw-r--r--   0        0        0    64741 2023-05-05 14:21:30.376963 gempyp-1.0.70b0/gempyp/final_report.html
--rw-r--r--   0        0        0     4724 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/gemPyp.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.379963 gempyp-1.0.70b0/gempyp/jira/__init__.py
--rw-r--r--   0        0        0     2337 2023-05-05 14:21:30.380963 gempyp-1.0.70b0/gempyp/jira/jiraIntegration.py
--rw-r--r--   0        0        0     4474 2023-05-05 14:21:30.380963 gempyp-1.0.70b0/gempyp/jira/jiraIntegrationCopy.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.381963 gempyp-1.0.70b0/gempyp/libs/__init__.py
--rw-r--r--   0        0        0     9045 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/libs/common.py
--rw-r--r--   0        0        0      131 2023-05-05 14:21:30.383963 gempyp-1.0.70b0/gempyp/libs/enums/run_types.py
--rw-r--r--   0        0        0      318 2023-05-05 14:21:56.341993 gempyp-1.0.70b0/gempyp/libs/enums/status.py
--rw-r--r--   0        0        0       47 2023-05-05 14:21:30.384963 gempyp-1.0.70b0/gempyp/libs/exceptions/__init__.py
--rw-r--r--   0        0        0     4352 2023-05-05 14:21:30.385646 gempyp-1.0.70b0/gempyp/libs/gem_s3_common.py
--rw-r--r--   0        0        0     2642 2023-05-05 14:21:30.386656 gempyp-1.0.70b0/gempyp/libs/logConfig.py
--rw-r--r--   0        0        0     1465 2023-05-05 14:21:30.386656 gempyp-1.0.70b0/gempyp/libs/parsers.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.387656 gempyp-1.0.70b0/gempyp/pyprest/__init__.py
--rw-r--r--   0        0        0     9844 2023-05-05 14:21:30.388723 gempyp-1.0.70b0/gempyp/pyprest/apiCommon.py
--rw-r--r--   0        0        0      491 2023-05-05 14:21:30.389602 gempyp-1.0.70b0/gempyp/pyprest/beforeAfterSample.py
--rw-r--r--   0        0        0    13694 2023-05-05 14:21:30.390435 gempyp-1.0.70b0/gempyp/pyprest/compareFunctions.py
--rw-r--r--   0        0        0    13567 2023-05-05 14:21:30.391447 gempyp-1.0.70b0/gempyp/pyprest/keyCheck.py
--rw-r--r--   0        0        0    15661 2023-05-05 14:21:30.392445 gempyp-1.0.70b0/gempyp/pyprest/legacyComparison.py
--rw-r--r--   0        0        0     1933 2023-05-05 14:21:30.393446 gempyp-1.0.70b0/gempyp/pyprest/miscVariables.py
--rw-r--r--   0        0        0    10792 2023-05-05 14:21:30.393446 gempyp-1.0.70b0/gempyp/pyprest/postAssertion.py
--rw-r--r--   0        0        0     4195 2023-05-05 14:21:30.394437 gempyp-1.0.70b0/gempyp/pyprest/postVariables.py
--rw-r--r--   0        0        0     8271 2023-05-05 14:21:30.396448 gempyp-1.0.70b0/gempyp/pyprest/predefinedFunctions.py
--rw-r--r--   0        0        0     3873 2023-05-05 14:21:30.395446 gempyp-1.0.70b0/gempyp/pyprest/preVariables.py
--rw-r--r--   0        0        0    36175 2023-05-05 14:21:30.397446 gempyp-1.0.70b0/gempyp/pyprest/pypRest.py
--rw-r--r--   0        0        0     4333 2023-05-05 14:21:30.398445 gempyp-1.0.70b0/gempyp/pyprest/reporting.py
--rw-r--r--   0        0        0     2725 2023-05-05 14:21:30.398445 gempyp-1.0.70b0/gempyp/pyprest/restEngine.py
--rw-r--r--   0        0        0     1031 2023-05-05 14:21:30.399475 gempyp-1.0.70b0/gempyp/pyprest/restObj.py
--rw-r--r--   0        0        0     6308 2023-05-05 14:21:30.400514 gempyp-1.0.70b0/gempyp/pyprest/utils.py
--rw-r--r--   0        0        0     5463 2023-05-05 14:21:30.400514 gempyp-1.0.70b0/gempyp/pyprest/variableReplacement.py
--rw-r--r--   0        0        0        0 2023-05-05 14:21:30.401512 gempyp-1.0.70b0/gempyp/reporter/__init__.py
--rw-r--r--   0        0        0     6959 2023-05-05 14:21:56.358422 gempyp-1.0.70b0/gempyp/reporter/reportGenerator.py
--rw-r--r--   0        0        0    12721 2023-05-05 14:21:56.360429 gempyp-1.0.70b0/gempyp/sdk/executor.py
--rw-r--r--   0        0        0     2508 2023-05-05 14:21:56.361432 gempyp-1.0.70b0/gempyp/sdk/worker.py
--rw-r--r--   0        0        0    11547 2023-05-05 14:21:30.404588 gempyp-1.0.70b0/gempyp/testcase.html
--rw-r--r--   0        0        0        2 2023-05-05 14:21:30.308048 gempyp-1.0.70b0/LICENSE
--rw-r--r--   0        0        0     1371 2023-05-05 14:30:57.265844 gempyp-1.0.70b0/pyproject.toml
--rw-r--r--   0        0        0     3161 2023-05-05 14:21:30.308048 gempyp-1.0.70b0/README.md
--rw-r--r--   0        0        0     4842 1970-01-01 00:00:00.000000 gempyp-1.0.70b0/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-05-19 10:29:23.809487 gempyp-1.0.70b1/gempyp/__init__.py
+-rw-r--r--   0        0        0      108 2023-05-05 14:21:30.308048 gempyp-1.0.70b1/gempyp/cli.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.308048 gempyp-1.0.70b1/gempyp/config/__init__.py
+-rw-r--r--   0        0        0     7387 2023-05-05 14:21:30.308048 gempyp-1.0.70b1/gempyp/config/baseConfig.py
+-rw-r--r--   0        0        0      198 2023-05-05 14:21:56.341993 gempyp-1.0.70b1/gempyp/config/customParser.py
+-rw-r--r--   0        0        0     1802 2023-05-19 10:29:23.812431 gempyp-1.0.70b1/gempyp/config/DefaultSettings.py
+-rw-r--r--   0        0        0       62 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/config/gempyp.conf
+-rw-r--r--   0        0        0     2145 2023-05-05 14:21:30.308048 gempyp-1.0.70b1/gempyp/config/GitLinkXML.py
+-rw-r--r--   0        0        0    21143 2023-05-05 14:21:30.308048 gempyp-1.0.70b1/gempyp/config/Result.html
+-rw-r--r--   0        0        0       26 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/config/suite_conf.json
+-rw-r--r--   0        0        0       28 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/config/testcase_conf.json
+-rw-r--r--   0        0        0     4007 2023-05-05 14:21:56.341993 gempyp-1.0.70b1/gempyp/config/xmlConfig.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/common/__init__.py
+-rw-r--r--   0        0        0     3627 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/common/common_functions.py
+-rw-r--r--   0        0        0      956 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/compare.py
+-rw-r--r--   0        0        0      149 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/config/dvm.json
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/configurator/__init__.py
+-rw-r--r--   0        0        0     4635 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/configurator/configurator.py
+-rw-r--r--   0        0        0      320 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/configurator/validator.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/core/__init__.py
+-rw-r--r--   0        0        0      589 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/core/comparator.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/core/Compare.py
+-rw-r--r--   0        0        0    10157 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/core/python_obj_comparator.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/data/__init__.py
+-rw-r--r--   0        0        0     5498 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/data/data.py
+-rw-r--r--   0        0        0      869 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/data/database.py
+-rw-r--r--   0        0        0     1903 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/data/db_mysql.py
+-rw-r--r--   0        0        0     2646 2023-05-05 14:21:30.323318 gempyp-1.0.70b1/gempyp/data_compare/data/db_oracle.py
+-rw-r--r--   0        0        0     2436 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/data_compare/data/db_postgre.py
+-rw-r--r--   0        0        0     1999 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/data_compare/data/db_sqlite.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/data_compare/data/file_processor.py
+-rw-r--r--   0        0        0    11161 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/data_compare/data_comp.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/data_compare/report/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/data_compare/tools/__init__.py
+-rw-r--r--   0        0        0     6758 2023-05-19 10:29:23.813426 gempyp-1.0.70b1/gempyp/data_uploader.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/dv/__init__.py
+-rw-r--r--   0        0        0     2285 2023-05-05 14:21:56.341993 gempyp-1.0.70b1/gempyp/dv/dfOperations.py
+-rw-r--r--   0        0        0    10230 2023-05-05 14:21:56.341993 gempyp-1.0.70b1/gempyp/dv/dvCompare.py
+-rw-r--r--   0        0        0      682 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/dv/dvDatabases.py
+-rw-r--r--   0        0        0     9470 2023-05-05 14:21:56.341993 gempyp-1.0.70b1/gempyp/dv/dvDataframe.py
+-rw-r--r--   0        0        0     1441 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/dv/dvObj.py
+-rw-r--r--   0        0        0     3789 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/dv/dvReporting.py
+-rw-r--r--   0        0        0    23229 2023-05-19 10:29:23.814426 gempyp-1.0.70b1/gempyp/dv/dvRunner.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/engine/__init__.py
+-rw-r--r--   0        0        0     5092 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/engine/baseTemplate.py
+-rw-r--r--   0        0        0     8414 2023-05-05 14:21:56.341993 gempyp-1.0.70b1/gempyp/engine/dataUpload.py
+-rw-r--r--   0        0        0    41041 2023-05-19 10:29:23.816426 gempyp-1.0.70b1/gempyp/engine/engine.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.356805 gempyp-1.0.70b1/gempyp/engine/executors/__init__.py
+-rw-r--r--   0        0        0      443 2023-05-05 14:21:30.372942 gempyp-1.0.70b1/gempyp/engine/executors/baseExecutor.py
+-rw-r--r--   0        0        0      656 2023-05-05 14:21:30.373956 gempyp-1.0.70b1/gempyp/engine/gempypHelper.py
+-rw-r--r--   0        0        0     5483 2023-05-19 10:29:23.818430 gempyp-1.0.70b1/gempyp/engine/runner.py
+-rw-r--r--   0        0        0     5537 2023-05-05 14:21:30.374954 gempyp-1.0.70b1/gempyp/engine/simpleTestcase.py
+-rw-r--r--   0        0        0    12428 2023-05-05 14:21:56.341993 gempyp-1.0.70b1/gempyp/engine/testData.py
+-rw-r--r--   0        0        0    64741 2023-05-05 14:21:30.376963 gempyp-1.0.70b1/gempyp/final_report.html
+-rw-r--r--   0        0        0     4566 2023-05-19 10:29:23.819425 gempyp-1.0.70b1/gempyp/gemPyp.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.379963 gempyp-1.0.70b1/gempyp/jira/__init__.py
+-rw-r--r--   0        0        0     2337 2023-05-05 14:21:30.380963 gempyp-1.0.70b1/gempyp/jira/jiraIntegration.py
+-rw-r--r--   0        0        0     4474 2023-05-05 14:21:30.380963 gempyp-1.0.70b1/gempyp/jira/jiraIntegrationCopy.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.381963 gempyp-1.0.70b1/gempyp/libs/__init__.py
+-rw-r--r--   0        0        0     9045 2023-05-05 14:21:56.341993 gempyp-1.0.70b1/gempyp/libs/common.py
+-rw-r--r--   0        0        0      131 2023-05-05 14:21:30.383963 gempyp-1.0.70b1/gempyp/libs/enums/run_types.py
+-rw-r--r--   0        0        0      318 2023-05-05 14:21:56.341993 gempyp-1.0.70b1/gempyp/libs/enums/status.py
+-rw-r--r--   0        0        0       47 2023-05-05 14:21:30.384963 gempyp-1.0.70b1/gempyp/libs/exceptions/__init__.py
+-rw-r--r--   0        0        0     4352 2023-05-05 14:21:30.385646 gempyp-1.0.70b1/gempyp/libs/gem_s3_common.py
+-rw-r--r--   0        0        0     2642 2023-05-05 14:21:30.386656 gempyp-1.0.70b1/gempyp/libs/logConfig.py
+-rw-r--r--   0        0        0     1465 2023-05-05 14:21:30.386656 gempyp-1.0.70b1/gempyp/libs/parsers.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.387656 gempyp-1.0.70b1/gempyp/pyprest/__init__.py
+-rw-r--r--   0        0        0     9844 2023-05-05 14:21:30.388723 gempyp-1.0.70b1/gempyp/pyprest/apiCommon.py
+-rw-r--r--   0        0        0      491 2023-05-05 14:21:30.389602 gempyp-1.0.70b1/gempyp/pyprest/beforeAfterSample.py
+-rw-r--r--   0        0        0    13694 2023-05-05 14:21:30.390435 gempyp-1.0.70b1/gempyp/pyprest/compareFunctions.py
+-rw-r--r--   0        0        0    13567 2023-05-05 14:21:30.391447 gempyp-1.0.70b1/gempyp/pyprest/keyCheck.py
+-rw-r--r--   0        0        0    15661 2023-05-05 14:21:30.392445 gempyp-1.0.70b1/gempyp/pyprest/legacyComparison.py
+-rw-r--r--   0        0        0     1933 2023-05-05 14:21:30.393446 gempyp-1.0.70b1/gempyp/pyprest/miscVariables.py
+-rw-r--r--   0        0        0    10792 2023-05-05 14:21:30.393446 gempyp-1.0.70b1/gempyp/pyprest/postAssertion.py
+-rw-r--r--   0        0        0     4195 2023-05-05 14:21:30.394437 gempyp-1.0.70b1/gempyp/pyprest/postVariables.py
+-rw-r--r--   0        0        0     8271 2023-05-05 14:21:30.396448 gempyp-1.0.70b1/gempyp/pyprest/predefinedFunctions.py
+-rw-r--r--   0        0        0     3873 2023-05-05 14:21:30.395446 gempyp-1.0.70b1/gempyp/pyprest/preVariables.py
+-rw-r--r--   0        0        0    36175 2023-05-05 14:21:30.397446 gempyp-1.0.70b1/gempyp/pyprest/pypRest.py
+-rw-r--r--   0        0        0     4333 2023-05-05 14:21:30.398445 gempyp-1.0.70b1/gempyp/pyprest/reporting.py
+-rw-r--r--   0        0        0     2725 2023-05-05 14:21:30.398445 gempyp-1.0.70b1/gempyp/pyprest/restEngine.py
+-rw-r--r--   0        0        0     1031 2023-05-05 14:21:30.399475 gempyp-1.0.70b1/gempyp/pyprest/restObj.py
+-rw-r--r--   0        0        0     6308 2023-05-05 14:21:30.400514 gempyp-1.0.70b1/gempyp/pyprest/utils.py
+-rw-r--r--   0        0        0     5463 2023-05-05 14:21:30.400514 gempyp-1.0.70b1/gempyp/pyprest/variableReplacement.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:21:30.401512 gempyp-1.0.70b1/gempyp/reporter/__init__.py
+-rw-r--r--   0        0        0     6959 2023-05-05 14:21:56.358422 gempyp-1.0.70b1/gempyp/reporter/reportGenerator.py
+-rw-r--r--   0        0        0    13086 2023-05-19 10:29:23.821450 gempyp-1.0.70b1/gempyp/sdk/executor.py
+-rw-r--r--   0        0        0     2490 2023-05-19 10:29:23.823426 gempyp-1.0.70b1/gempyp/sdk/worker.py
+-rw-r--r--   0        0        0    11547 2023-05-05 14:21:30.404588 gempyp-1.0.70b1/gempyp/testcase.html
+-rw-r--r--   0        0        0        2 2023-05-05 14:21:30.308048 gempyp-1.0.70b1/LICENSE
+-rw-r--r--   0        0        0     1431 2023-05-19 10:53:48.974856 gempyp-1.0.70b1/pyproject.toml
+-rw-r--r--   0        0        0     3161 2023-05-05 14:21:30.308048 gempyp-1.0.70b1/README.md
+-rw-r--r--   0        0        0     4941 1970-01-01 00:00:00.000000 gempyp-1.0.70b1/PKG-INFO
```

### Comparing `gempyp-1.0.70b0/gempyp/config/baseConfig.py` & `gempyp-1.0.70b1/gempyp/config/baseConfig.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/config/DefaultSettings.py` & `gempyp-1.0.70b1/gempyp/config/DefaultSettings.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
             logging.warning("Error Occurs While Getting the BASE_URLs")
         else:
             logging.info("Some Error From the Client Side, Maybe username or bridgeToken, Therefore terminating execution")
             sys.exit()
     except Exception as e:
             traceback.print_exc()
             logging.warning("Error Occurs While Getting the BASE_URLs")
+            sys.exit()
 
 # for sending urls to dataupload file
 def getUrls(apiName):
     return urls["data"].get(apiName, None)
 
 def checkUrl(url):
     try:
```

### Comparing `gempyp-1.0.70b0/gempyp/config/GitLinkXML.py` & `gempyp-1.0.70b1/gempyp/config/GitLinkXML.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/config/Result.html` & `gempyp-1.0.70b1/gempyp/config/Result.html`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/config/xmlConfig.py` & `gempyp-1.0.70b1/gempyp/config/xmlConfig.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/data_compare/common/common_functions.py` & `gempyp-1.0.70b1/gempyp/data_compare/common/common_functions.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/data_compare/compare.py` & `gempyp-1.0.70b1/gempyp/data_compare/compare.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/data_compare/configurator/configurator.py` & `gempyp-1.0.70b1/gempyp/data_compare/configurator/configurator.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/data_compare/core/comparator.py` & `gempyp-1.0.70b1/gempyp/data_compare/core/comparator.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/data_compare/core/python_obj_comparator.py` & `gempyp-1.0.70b1/gempyp/data_compare/core/python_obj_comparator.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/data_compare/data/data.py` & `gempyp-1.0.70b1/gempyp/data_compare/data/data.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/data_compare/data/database.py` & `gempyp-1.0.70b1/gempyp/data_compare/data/database.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/data_compare/data/db_mysql.py` & `gempyp-1.0.70b1/gempyp/data_compare/data/db_mysql.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/data_compare/data/db_oracle.py` & `gempyp-1.0.70b1/gempyp/data_compare/data/db_oracle.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/data_compare/data/db_postgre.py` & `gempyp-1.0.70b1/gempyp/data_compare/data/db_postgre.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/data_compare/data/db_sqlite.py` & `gempyp-1.0.70b1/gempyp/data_compare/data/db_sqlite.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/data_compare/data_comp.py` & `gempyp-1.0.70b1/gempyp/data_compare/data_comp.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/dv/dfOperations.py` & `gempyp-1.0.70b1/gempyp/dv/dfOperations.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/dv/dvCompare.py` & `gempyp-1.0.70b1/gempyp/dv/dvCompare.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/dv/dvDatabases.py` & `gempyp-1.0.70b1/gempyp/dv/dvDatabases.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/dv/dvDataframe.py` & `gempyp-1.0.70b1/gempyp/dv/dvDataframe.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/dv/dvObj.py` & `gempyp-1.0.70b1/gempyp/dv/dvObj.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/dv/dvReporting.py` & `gempyp-1.0.70b1/gempyp/dv/dvReporting.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/dv/dvRunner.py` & `gempyp-1.0.70b1/gempyp/dv/dvRunner.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,15 +288,15 @@
                 s3_url = None
                 try:
                     s3_url = create_s3_link(url=upload_to_s3(DefaultSettings.urls["data"]["bucket-file-upload-api"], bridge_token=self.data["SUITE_VARS"]
                                             ["bridge_token"], tag="public", username=self.data["SUITE_VARS"]["username"], file=excelPath)[0]["Url"])
                 except Exception as e:
                     logging.warn(e)
                 if not s3_url:
-                    self.reporter.addRow("Data Validation Report", f"Matched Keys: {keys_length['common_keys']}, Keys only in Source: {keys_length['keys_only_in_src']}, Keys only in Target: {keys_length['keys_only_in_tgt']}, Mismatched Cells: {value_check}, Duplicate Keys: {dup_keys_len}, DV Result File:", status=status.FAIL,Attachment=[excel])
+                    self.reporter.addRow("Data Validation Report", f"Matched Keys: {keys_length['common_keys']}, Keys only in Source: {keys_length['keys_only_in_src']}, Keys only in Target: {keys_length['keys_only_in_tgt']}, Mismatched Cells: {value_check}, Duplicate Keys: {dup_keys_len}, DV Result File:", status=status.FAIL,Attachment=[excelPath])
                 else:
                     self.reporter.addRow("Data Validation Report", f"Matched Keys: {keys_length['common_keys']}, Keys only in Source: {keys_length['keys_only_in_src']}, Keys only in Target: {keys_length['keys_only_in_tgt']}, Mismatched Cells: {value_check}, Duplicate Keys: {dup_keys_len}, DV Result File:", status=status.FAIL,Attachment=[s3_url])
 
                 self.reporter.addMisc("REASON OF FAILURE", str(
                     f"Mismatched Keys: {key_check},Mismatched Cells: {value_check}"))
             self.reporter.addMisc("common Keys", str(keys_length['common_keys']))
             self.reporter.addMisc("Keys Only in Source",
@@ -473,15 +473,14 @@
             value=config.get(key)
             if(type(value)!=logging.Logger):
                 if re.search("mysql.connector.connect",value) or re.search("^{",value):
                     config[key] = re.sub(pattern, lambda match: f"'{os.environ.get(match.group(1), '')}'", value)
                 else:
                     if("ENV." in value):
                         config[key]=os.environ.get(value.replace("ENV.",""))
-        print(config)
         return config
     
     def parseConfigDict(self,conf):
         for key in conf.keys():
             if("ENV." in conf.get(key) and os.environ.get(conf.get(key).replace("ENV.",""))):
                 conf[key]=os.environ.get(conf.get(key).replace("ENV.",""))
         return conf
```

### Comparing `gempyp-1.0.70b0/gempyp/engine/baseTemplate.py` & `gempyp-1.0.70b1/gempyp/engine/baseTemplate.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/engine/dataUpload.py` & `gempyp-1.0.70b1/gempyp/engine/dataUpload.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/engine/engine.py` & `gempyp-1.0.70b1/gempyp/engine/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,15 +214,16 @@
         make outputFolder for report named as gempyp_reports in user home directory if not given by the user and makes log fplder for log files
         if given by user than set user given path for reports file   
         """
 
         logging.info("---------- Making output folders -------------")
         report_folder_name = f"{self.project_name}_{self.project_env}"
         if self.report_name:
-            report_folder_name = report_folder_name + f"_{self.report_name}"
+            report_name = "_".join(self.report_name.split())
+            report_folder_name = report_folder_name + f"_{report_name}"
         date = datetime.now().strftime("%Y_%b_%d_%H%M%S_%f")
         report_folder_name = report_folder_name + f"_{date}"
         if "REPORT_LOCATION" in self.PARAMS and self.PARAMS["REPORT_LOCATION"]:
             self.ouput_folder = os.path.join(
                 self.PARAMS["REPORT_LOCATION"], report_folder_name
             )
         else:
@@ -233,14 +234,20 @@
 
         os.makedirs(self.ouput_folder)
         self.testcase_folder = os.path.join(self.ouput_folder, "testcases")
         os.makedirs(self.testcase_folder)
         self.testcase_log_folder = os.path.join(self.ouput_folder, "logs")
         os.environ['TESTCASE_LOG_FOLDER'] = self.testcase_log_folder
         os.makedirs(self.testcase_log_folder)
+    def verify(self,value):
+        if(re.search(r'[^a-zA-Z0-9_ ]',value)):
+                logging.info("Some Error From the Client Side. May be s_run_id, project_name or ENV is not in a correct format")
+                sys.exit()
+        else:
+                return value
 
     def setUP(self, config: Type[AbstarctBaseConfig]):
 
         """
 
         assigning values to some attributes which will be used in method makeSuiteDetails
 
@@ -281,17 +288,17 @@
                 self.skip_jira = 1
         except Exception as e:
             pass
 
         mail_items={"to":"EMAIL_TO","cc":"EMAIL_CC","bcc":"EMAIL_BCC"}
         self.mail={key:common.parseMails(self.PARAMS.get(value,None)) for key,value in mail_items.items()}
 
-        self.project_name = self.PARAMS["PROJECT_NAME"]
+        self.project_name=self.verify(self.PARAMS["PROJECT_NAME"])
+        self.project_env=self.verify(self.PARAMS["ENVIRONMENT"])
         self.report_name = self.PARAMS.get("REPORT_NAME")
-        self.project_env = self.PARAMS["ENVIRONMENT"]
         self.unique_id = self.PARAMS["UNIQUE_ID"]
         self.user_suite_variables = self.PARAMS.get("SUITE_VARS", {})
         self.jewel_run = False
         self.jewel_user = False
         self.s3_url = ""
         if self.bridgetoken and self.username:
             self.user_suite_variables["bridge_token"]=self.bridgetoken
@@ -305,16 +312,19 @@
             #     logging.info("Trying to call Api for getting urls")
             #     DefaultSettings.getEnterPoint(self.PARAMS["BASE_URL"] ,self.PARAMS["BRIDGE_TOKEN"], self.PARAMS["USERNAME"])
 
             if self.PARAMS.get("S_ID", None):
                 self.jewel_run = True
             else:
                 try:
-                    self.s3_url = upload_to_s3(DefaultSettings.urls["data"]["bucket-file-upload-api"], bridge_token=self.bridgetoken, username=self.username, file=self.PARAMS["config"])[0]["Url"]
-                    logging.info("--------- url" + str(self.s3_url))
+                    if DefaultSettings.apiSuccess:
+                        self.s3_url = upload_to_s3(DefaultSettings.urls["data"]["bucket-file-upload-api"], bridge_token=self.bridgetoken, username=self.username, file=self.PARAMS["config"])[0]["Url"]
+                        logging.info("--------- url" + str(self.s3_url))
+                    else:
+                        self.s3_url = self.PARAMS["config"]
                 except Exception as e:
                     logging.info(e)
         #add suite_vars here 
 
     # def parseMails(self):
     #     """
     #     to get the mail from the configData
@@ -323,21 +333,21 @@
     #         self.mail = common.parseMails(self.PARAMS["MAIL"])
 
     def makeSuiteDetails(self):
         """
         making suiteDetails dictionary and assign it to DATA.suiteDetail 
         """
         if "S_RUN_ID" in self.PARAMS:
-            self.s_run_id = self.PARAMS["S_RUN_ID"]
+            self.s_run_id = self.verify(self.PARAMS["S_RUN_ID"])
         else:
             if not self.unique_id:
                 self.unique_id = uuid.uuid4()
             self.s_run_id = f"{self.project_name}_{self.project_env}_{self.unique_id}"
             self.s_run_id = self.s_run_id.upper()
-        self.s_run_id = re.sub(r'[^\w\s]', '',self.s_run_id)
+        # self.s_run_id = re.sub(r'[^\w\s]', '',self.s_run_id)
         self.s_run_id=re.sub(r'\s+', '_',self.s_run_id)
         logging.info("S_RUN_ID: {}".format(self.s_run_id))
         suite_details = {
             "s_run_id": self.s_run_id,
             "s_start_time": self.start_time,
             "s_end_time": None,
             "s_id": self.PARAMS.get("S_ID", "test_id"),
@@ -840,8 +850,8 @@
                 sorted_dict[key] = unsorted_dict[key]
                 unsorted_dict.pop(key)
             elif key == "PASS" or key == 'FAIL':
                 sorted_dict[key] = 0
         sorted_dict.update(unsorted_dict)
         return sorted_dict
     
-     
+
```

### Comparing `gempyp-1.0.70b0/gempyp/engine/gempypHelper.py` & `gempyp-1.0.70b1/gempyp/engine/gempypHelper.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/engine/runner.py` & `gempyp-1.0.70b1/gempyp/engine/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import uuid
 from typing import Dict, List, Tuple
 from gempyp.engine.simpleTestcase import AbstractSimpleTestcase
 import getpass
 from gempyp.libs.common import download_common_file, moduleImports
 from gempyp.libs.gem_s3_common import upload_to_s3, create_s3_link
 from gempyp.config import DefaultSettings
+import re
 
 def testcaseRunner(testcase_meta: Dict) -> Tuple[List, Dict]:
     result_data = None
     """
     actually imports the testcase files and call the run method 
     set the json data that is required to update in db
     """
@@ -71,14 +72,15 @@
     unique_id = uuid.uuid4()
     try:
         if os.environ.get('unique_id'):
             unique_id = os.environ.get('unique_id')
     except Exception:
         traceback.print_exc()
     tc_run_id = f"{data['NAME']}_{unique_id}"
+    tc_run_id=re.sub(r'[^a-zA-Z0-9]', '_',tc_run_id)
     tempdict["tc_run_id"] = tc_run_id
     tempdict["name"] = data["NAME"]
     tempdict["category"] = data["config_data"].get("CATEGORY", None)
     tempdict["status"] = data["STATUS"]
     tempdict["base_user"] = getpass.getuser()
     tempdict["invoke_user"] = data["TESTCASEMETADATA"]["INVOKE_USER"]
     tempdict["machine"] = data["TESTCASEMETADATA"]["MACHINE"]
```

### Comparing `gempyp-1.0.70b0/gempyp/engine/simpleTestcase.py` & `gempyp-1.0.70b1/gempyp/engine/simpleTestcase.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/engine/testData.py` & `gempyp-1.0.70b1/gempyp/engine/testData.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/final_report.html` & `gempyp-1.0.70b1/gempyp/final_report.html`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/gemPyp.py` & `gempyp-1.0.70b1/gempyp/gemPyp.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         """
         self.config = None
         self.MAIL = None
         self.PROJECT_NAME = None
         self.REPORT_NAME = None
         self.MODE = None
         self.ENVIRONMENT = None
-        self.args = None
+        self.args = {}
         self.THREADS = None
         self.JEWEL_BRIDGE_TOKEN = None 
         self.REPORT_LOCATION = None
         self.CATEGORY=None
         self.JEWEL_USER=None
         self.S_RUN_ID = None
         self.TESTCASE_LIST = None
@@ -59,42 +59,38 @@
         return args
 
     def runner(self):
         """
         This function takes the config and updates the config data in case or cli run and direct(python) run
         """
         s_run_id = vars(self)["S_RUN_ID"]
-        # if self.args != None:
-        if self.args.RE_RUN != None:
+        if self.args.get('RE_RUN',None) != None:
                 print("Trying to Reupload Data")
-                dataUploader(self.args.RE_RUN,self.args.JEWEL_BRIDGE_TOKEN)
+                dataUploader(self.args.get('RE_RUN'),self.args.get('JEWEL_BRIDGE_TOKEN',None))
         elif self.RE_RUN != None:
                 print("Trying to Reupload Data")
-                if self.args.JEWEL_BRIDGE_TOKEN:
-                    dataUploader(self.RE_RUN, self.args.JEWEL_BRIDGE_TOKEN)
-                else:
-                    dataUploader(self.RE_RUN, self.JEWEL_BRIDGE_TOKEN)
+                dataUploader(self.RE_RUN, self.JEWEL_BRIDGE_TOKEN)
         # if self.args.RE_RUN
         else:
             file_path=download_common_file(self.config)
             config=XmlConfig(file_path,s_run_id)
             if not self.args:
                 del self.__dict__["args"]
                 config.cli_config = vars(self)
             else:
-                config.cli_config = vars(self.args)
+                config.cli_config = self.args
             config.update()
             Engine(config)
 
     def parser(self):
         """Calls the parser and handles the case of no cli args"""
         args = self.argParser()
         if args.config != None:
             self.config = args.config
-        self.args = args
+        self.args = vars(args)
         self.runner()
 
 def main():
     obj = Gempyp()
     #obj.config = "C:\\Users\\an.pandey\\gempyp\\tests\\configTest\\Gempyp_Test_Suite.xml"
     #obj.ENV = ""
     #obj.MAIL = ""
```

### Comparing `gempyp-1.0.70b0/gempyp/jira/jiraIntegration.py` & `gempyp-1.0.70b1/gempyp/jira/jiraIntegration.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/jira/jiraIntegrationCopy.py` & `gempyp-1.0.70b1/gempyp/jira/jiraIntegrationCopy.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/libs/common.py` & `gempyp-1.0.70b1/gempyp/libs/common.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/libs/gem_s3_common.py` & `gempyp-1.0.70b1/gempyp/libs/gem_s3_common.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/libs/logConfig.py` & `gempyp-1.0.70b1/gempyp/libs/logConfig.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/libs/parsers.py` & `gempyp-1.0.70b1/gempyp/libs/parsers.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/pyprest/apiCommon.py` & `gempyp-1.0.70b1/gempyp/pyprest/apiCommon.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/pyprest/compareFunctions.py` & `gempyp-1.0.70b1/gempyp/pyprest/compareFunctions.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/pyprest/keyCheck.py` & `gempyp-1.0.70b1/gempyp/pyprest/keyCheck.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/pyprest/legacyComparison.py` & `gempyp-1.0.70b1/gempyp/pyprest/legacyComparison.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/pyprest/miscVariables.py` & `gempyp-1.0.70b1/gempyp/pyprest/miscVariables.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/pyprest/postAssertion.py` & `gempyp-1.0.70b1/gempyp/pyprest/postAssertion.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/pyprest/postVariables.py` & `gempyp-1.0.70b1/gempyp/pyprest/postVariables.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/pyprest/predefinedFunctions.py` & `gempyp-1.0.70b1/gempyp/pyprest/predefinedFunctions.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/pyprest/preVariables.py` & `gempyp-1.0.70b1/gempyp/pyprest/preVariables.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/pyprest/pypRest.py` & `gempyp-1.0.70b1/gempyp/pyprest/pypRest.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/pyprest/reporting.py` & `gempyp-1.0.70b1/gempyp/pyprest/reporting.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/pyprest/restEngine.py` & `gempyp-1.0.70b1/gempyp/pyprest/restEngine.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/pyprest/restObj.py` & `gempyp-1.0.70b1/gempyp/pyprest/restObj.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/pyprest/utils.py` & `gempyp-1.0.70b1/gempyp/pyprest/utils.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/pyprest/variableReplacement.py` & `gempyp-1.0.70b1/gempyp/pyprest/variableReplacement.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/reporter/reportGenerator.py` & `gempyp-1.0.70b1/gempyp/reporter/reportGenerator.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/gempyp/sdk/executor.py` & `gempyp-1.0.70b1/gempyp/sdk/executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 import tempfile
 import subprocess
 import sys
 import os
 import pandas as pd
 from gempyp.libs.enums.status import status
 from gempyp.libs.common import *
+from gempyp.engine.engine import Engine
 
 
 class Executor(TestcaseReporter):
     def __init__(self, **kwargs):
         self.method = kwargs.get("tc_name", self.getMethodName())
         self.log_file = tempfile.gettempdir() + "\logs.log"
         # os.makedirs("testcase_log_folder")
-        print(self.log_file)
         sys.stdout = sys.stderr =  open(self.log_file, 'w')
         logging.basicConfig(filename="logs.log", filemode='w', format='%(name)s - %(levelname)s - %(message)s',level=logging.DEBUG)
         # custom_logger = my_custom_logger("logs.log")
         logging.info("inside constructor here--------------------")
         logging.info(f"-------Executing testcase - {self.getMethodName()}---------")
         self.data = self.getTestcaseData()
         self.reporter = TestcaseReporter(self.data["PROJECT_NAME"], self.data["NAME"])
@@ -71,14 +71,15 @@
         # serializing data, adding suite data
         report_dict = self.reporter.serialize()
 
         report_dict["TESTCASEMETADATA"] = self.getMetaData()
         report_dict["config_data"] = self.getConfigData()
         # creating output json
         output.append(getOutput(report_dict))
+        output[0]['testcase_dict']['run_type'], output[0]['testcase_dict']['run_mode'],output[0]['testcase_dict']['job_name'],output[0]['testcase_dict']['job_runid'] = Engine.set_run_type_mode(self)
         for i in output:
             i["testcase_dict"]["steps"] = i["json_data"]["steps"]
             dict_ = {}
             dict_["testcases"] = {}
             dict_["REPORT_LOCATION"] = os.getenv("REPORT_LOCATION")
             dict_["misc_data"] = {}
             tmp_dir = os.path.join(tempfile.gettempdir(), self.s_run_id + ".txt")
@@ -105,15 +106,17 @@
                     data = json.loads(data)
                     data[self.s_run_id] = self.updateSuiteData(suite_data, data[self.s_run_id])
                     data["testcases"][i["testcase_dict"].get("tc_run_id")] = i["json_data"]
                     f.seek(0)
                     f.write(json.dumps(data))
             logging.info("---------------TC_RUN_ID-----------------"+i["testcase_dict"]["tc_run_id"].upper())
             dataUpload.sendTestcaseData((self.DATA.totestcaseJson(i["testcase_dict"]["tc_run_id"].upper(), self.data["S_RUN_ID"])), self.data["JEWEL_BRIDGE_TOKEN"], self.data["JEWEL_USER"])  # instead of output, I need to pass s_run id and  tc_run_id
-            
+            path = __file__
+            path = path.rsplit(os.sep, 1)[0]
+            subprocess.Popen([sys.executable, os.path.join(path, "worker.py")], shell=True)
             # sys.stdout.close()
         
             # os.rename(self.log_file, tmp_dir.rsplit(".", 1)[0] + ".log")
 
             
 
     def getTestcaseData(self):
@@ -200,15 +203,15 @@
             "env": self.data["ENVIRONMENT"],
             "machine": self.data["MACHINE"],
             "initiated_by": self.data["JEWEL_USER"],
             "run_mode": run_mode,
             "os": platform.system().upper(),
             "meta_data": [],
             "testcase_info": None,
-            "expected_testcases":2,
+            "expected_testcases":1,
             "framework_name": "GEMPYP",
         }
         self.DATA.suite_detail = self.DATA.suite_detail.append(
             Suite_details, ignore_index=True
         )
```

### Comparing `gempyp-1.0.70b0/gempyp/sdk/worker.py` & `gempyp-1.0.70b1/gempyp/sdk/worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,22 +31,22 @@
     except Exception as e:
         bridgetoken = None
     data = json.loads(data)
     runBaseUrls(jewel,config_file['ReportSetting'].get("enter_point", None),username,bridgetoken)
     json_data = data[s_run_id]
     testcaseData = data["testcases"]
     output_folder = data["REPORT_LOCATION"]
-    repJson, ouput_file_path = TemplateData().makeSuiteReport(json.dumps(json_data), testcaseData, output_folder,jewel)
+    repJson = TemplateData().makeSuiteReport(json.dumps(json_data), testcaseData,output_folder,jewel)
     suite_data = json_data["suits_details"]
     suite_data["misc_data"] = data["misc_data"]
     username = suite_data["initiated_by"]
     del suite_data["testcase_details"]
     del suite_data["testcase_info"]
     dataUpload.sendSuiteData(json.dumps(suite_data), bridgetoken, username, mode="PUT")
-    return ouput_file_path
+    return output_folder
 
 
 if __name__ == "__main__":
     while(True):
         if not pid_running(os.environ["PID"]):
             s_run_id = os.getenv("S_RUN_ID")
             if s_run_id:
@@ -56,10 +56,10 @@
                     with open(file_path, "r+") as f:
                         data = str(f.read())
                         output_file_path = create_report(data, s_run_id)
                         # where to get this json data from
                         current_pid = os.getpid()
                         logging.info(f"Find Gempyp logs at - {s_run_id + '.log'}")
                         logging.info(f"Find Gempyp Report at - {output_file_path}")
-                        os.rename("logs.log",f"{s_run_id}.log")
+                        # os.rename("logs.log",f"{s_run_id}.log")
                         os.kill(current_pid, 19)
                         sys.exit()
```

### Comparing `gempyp-1.0.70b0/gempyp/testcase.html` & `gempyp-1.0.70b1/gempyp/testcase.html`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/pyproject.toml` & `gempyp-1.0.70b1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gempyp"
-version = "1.0.70b"
+version = "1.0.70b1"
 description = "An ecosystem of libraries useful for software development"
 authors = ["Gemini Solutions-QA"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://gempyp.readthedocs.io/en/latest/"
 homepage = "https://github.com/Gemini-Solutions/gempyp"
 repository = "https://github.com/Gemini-Solutions/gempyp"
@@ -33,14 +33,16 @@
 python-dateutil = "^2.8.2"
 pytz = "^2022.2.1"
 requests = "^2.27.1"
 requests-ntlm = "^1.1.0"
 six = "^1.16.0"
 urllib3 = "^1.26.12"
 XlsxWriter = "^3.0.3"
+pymongo = "^4.3.3"
+snowflake-connector-python = "^3.0.1"
 
 [tool.poetry.dev-dependencies]
 Sphinx = "^4.0.2"
 nbsphinx = "^0.8.5"
 ipykernel = "^5.5.5"
 sphinx-autoapi = "^1.8.1"
 sphinx-rtd-theme = "^0.5.2"
```

### Comparing `gempyp-1.0.70b0/README.md` & `gempyp-1.0.70b1/README.md`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.70b0/PKG-INFO` & `gempyp-1.0.70b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gempyp
-Version: 1.0.70b0
+Version: 1.0.70b1
 Summary: An ecosystem of libraries useful for software development
 Home-page: https://github.com/Gemini-Solutions/gempyp
 License: MIT
 Author: Gemini Solutions-QA
 Requires-Python: >=3.6.8,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -24,22 +24,24 @@
 Requires-Dist: lxml (>=4.9.0,<5.0.0)
 Requires-Dist: mysql-connector-python (>=8.0.30,<9.0.0)
 Requires-Dist: ntlm-auth (>=1.5.0,<2.0.0)
 Requires-Dist: numpy (>=1.19.5,<2.0.0)
 Requires-Dist: pandas (>=1.1.5,<2.0.0)
 Requires-Dist: pg8000 (>=1.26.0,<2.0.0)
 Requires-Dist: pycparser (>=2.21,<3.0)
+Requires-Dist: pymongo (>=4.3.3,<5.0.0)
 Requires-Dist: pyreadline (>=2.1,<3.0)
 Requires-Dist: pyreadline3 (>=3.4.1,<4.0.0)
 Requires-Dist: pytest (>=6.2.4,<7.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: pytz (>=2022.2.1,<2023.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: requests-ntlm (>=1.1.0,<2.0.0)
 Requires-Dist: six (>=1.16.0,<2.0.0)
+Requires-Dist: snowflake-connector-python (>=3.0.1,<4.0.0)
 Requires-Dist: urllib3 (>=1.26.12,<2.0.0)
 Project-URL: Documentation, https://gempyp.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/Gemini-Solutions/gempyp
 Description-Content-Type: text/markdown
 
 <h1 align="center">
 	<img
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gempyp Version: 1.0.70b0 Summary: An ecosystem of
+Metadata-Version: 2.1 Name: gempyp Version: 1.0.70b1 Summary: An ecosystem of
 libraries useful for software development Home-page: https://github.com/Gemini-
 Solutions/gempyp License: MIT Author: Gemini Solutions-QA Requires-Python:
 >=3.6.8,<4.0.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
@@ -11,22 +11,23 @@
 charset-normalizer (>=2.0.12,<3.0.0) Requires-Dist: coloredlogs
 (>=15.0.1,<16.0.0) Requires-Dist: cryptography (>=38.0.1,<39.0.0) Requires-
 Dist: humanfriendly (>=10.0,<11.0) Requires-Dist: idna (>=3.4,<4.0) Requires-
 Dist: lxml (>=4.9.0,<5.0.0) Requires-Dist: mysql-connector-python
 (>=8.0.30,<9.0.0) Requires-Dist: ntlm-auth (>=1.5.0,<2.0.0) Requires-Dist:
 numpy (>=1.19.5,<2.0.0) Requires-Dist: pandas (>=1.1.5,<2.0.0) Requires-Dist:
 pg8000 (>=1.26.0,<2.0.0) Requires-Dist: pycparser (>=2.21,<3.0) Requires-Dist:
-pyreadline (>=2.1,<3.0) Requires-Dist: pyreadline3 (>=3.4.1,<4.0.0) Requires-
-Dist: pytest (>=6.2.4,<7.0.0) Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: pytz (>=2022.2.1,<2023.0.0) Requires-Dist: requests
-(>=2.27.1,<3.0.0) Requires-Dist: requests-ntlm (>=1.1.0,<2.0.0) Requires-Dist:
-six (>=1.16.0,<2.0.0) Requires-Dist: urllib3 (>=1.26.12,<2.0.0) Project-URL:
-Documentation, https://gempyp.readthedocs.io/en/latest/ Project-URL:
-Repository, https://github.com/Gemini-Solutions/gempyp Description-Content-
-Type: text/markdown
+pymongo (>=4.3.3,<5.0.0) Requires-Dist: pyreadline (>=2.1,<3.0) Requires-Dist:
+pyreadline3 (>=3.4.1,<4.0.0) Requires-Dist: pytest (>=6.2.4,<7.0.0) Requires-
+Dist: python-dateutil (>=2.8.2,<3.0.0) Requires-Dist: pytz
+(>=2022.2.1,<2023.0.0) Requires-Dist: requests (>=2.27.1,<3.0.0) Requires-Dist:
+requests-ntlm (>=1.1.0,<2.0.0) Requires-Dist: six (>=1.16.0,<2.0.0) Requires-
+Dist: snowflake-connector-python (>=3.0.1,<4.0.0) Requires-Dist: urllib3
+(>=1.26.12,<2.0.0) Project-URL: Documentation, https://gempyp.readthedocs.io/
+en/latest/ Project-URL: Repository, https://github.com/Gemini-Solutions/gempyp
+Description-Content-Type: text/markdown
                             ****** [GemPyp] ******
                               ***** GemPyP *****
                  An out of the box Python Automation Framework
                            Website â¢ Docs â¢ Repo
 [https://img.shields.io/badge/python-3.6-blue] [https://img.shields.io/pypi/dw/
                     gempyp] [https://img.shields.io/pypi/v/
    gempyp?color=red&label=version&logo=gempyp] [https://img.shields.io/pypi/
```

