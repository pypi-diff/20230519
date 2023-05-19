# Comparing `tmp/johnsnowlabs_tmp-4.2.9.tar.gz` & `tmp/johnsnowlabs_tmp-4.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "johnsnowlabs_tmp-4.2.9.tar", last modified: Wed Feb  1 18:17:16 2023, max compression
+gzip compressed data, was "johnsnowlabs_tmp-4.4.5.tar", last modified: Fri May 19 04:11:39 2023, max compression
```

## Comparing `johnsnowlabs_tmp-4.2.9.tar` & `johnsnowlabs_tmp-4.4.5.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-02-01 18:17:16.716349 johnsnowlabs_tmp-4.2.9/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1343 2023-02-01 18:17:16.716349 johnsnowlabs_tmp-4.2.9/PKG-INFO
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      389 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.2.9/README.md
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-02-01 18:17:16.708349 johnsnowlabs_tmp-4.2.9/johnsnowlabs/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1001 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-02-01 18:17:16.708349 johnsnowlabs_tmp-4.2.9/johnsnowlabs/abstract_base/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/abstract_base/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      395 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/abstract_base/base_enum.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9775 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/abstract_base/lib_resolver.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      733 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/abstract_base/pydantic_model.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9287 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/abstract_base/software_product.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-02-01 18:17:16.708349 johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-02-01 18:17:16.712349 johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/databricks/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/databricks/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2173 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/databricks/dbfs.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9531 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/databricks/install_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6612 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/databricks/work_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-02-01 18:17:16.712349 johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/health_checks/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/health_checks/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      973 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/health_checks/hc_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      884 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/health_checks/nlp_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2076 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/health_checks/ocr_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3496 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/health_checks/report.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6935 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/install_flow.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11362 2023-02-01 13:41:22.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/install_software.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12079 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/jsl_home.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-02-01 18:17:16.712349 johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/lib_resolvers/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      124 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/lib_resolvers/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2061 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3188 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2105 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8828 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/offline_install.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9133 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/softwares.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3875 2023-02-01 13:42:32.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/finance.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      212 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/lab.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3844 2023-02-01 13:42:27.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/legal.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3976 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/medical.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1367 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/nlp.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-02-01 18:17:16.712349 johnsnowlabs_tmp-4.2.9/johnsnowlabs/py_models/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/py_models/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4826 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/py_models/install_info.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    30708 2023-01-31 09:04:19.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/py_models/jsl_secrets.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4168 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/py_models/lib_version.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        2 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/py_models/license_info.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      128 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/py_models/primitive.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2079 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/py_models/url_dependency.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2204 2023-02-01 18:16:46.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/settings.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-02-01 18:17:16.716349 johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6657 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/enums.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1687 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/env_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      759 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/file_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1005 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/functional.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3326 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/modelhub_markdown.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10004 2023-01-31 09:04:19.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/my_jsl_api.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10654 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/notebooks.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5856 2023-01-31 09:04:19.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/pip_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      982 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/print_messages.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4371 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/py_process.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8019 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/sparksession_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-02-01 18:17:16.716349 johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/testing/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:29:40.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/testing/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4050 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/testing/jsl_pre_processor.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1778 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/testing/nb_code_match.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1132 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/testing/nb_nodes.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3460 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/testing/test_settings.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4353 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/venv_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1253 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/visual.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      408 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs/viz.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-02-01 18:17:16.716349 johnsnowlabs_tmp-4.2.9/johnsnowlabs_tmp.egg-info/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1343 2023-02-01 18:17:16.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs_tmp.egg-info/PKG-INFO
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2478 2023-02-01 18:17:16.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs_tmp.egg-info/SOURCES.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2023-02-01 18:17:16.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs_tmp.egg-info/dependency_links.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      114 2023-02-01 18:17:16.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs_tmp.egg-info/requires.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       13 2023-02-01 18:17:16.000000 johnsnowlabs_tmp-4.2.9/johnsnowlabs_tmp.egg-info/top_level.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2023-02-01 18:17:16.716349 johnsnowlabs_tmp-4.2.9/setup.cfg
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2060 2023-02-01 18:16:46.000000 johnsnowlabs_tmp-4.2.9/setup.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:11:39.793934 johnsnowlabs_tmp-4.4.5/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11356 2023-03-31 15:38:35.000000 johnsnowlabs_tmp-4.4.5/LICENSE
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9282 2023-05-19 04:11:39.793934 johnsnowlabs_tmp-4.4.5/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8307 2023-03-31 15:38:35.000000 johnsnowlabs_tmp-4.4.5/README.md
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:11:39.789934 johnsnowlabs_tmp-4.4.5/johnsnowlabs/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      932 2023-04-26 14:30:28.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:11:39.789934 johnsnowlabs_tmp-4.4.5/johnsnowlabs/abstract_base/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/abstract_base/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      395 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/abstract_base/base_enum.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9775 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/abstract_base/lib_resolver.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      733 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/abstract_base/pydantic_model.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9287 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/abstract_base/software_product.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:11:39.789934 johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:11:39.789934 johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/databricks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/databricks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2623 2023-03-26 01:30:02.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/databricks/dbfs.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12144 2023-03-26 01:30:02.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/databricks/install_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6612 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/databricks/work_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:11:39.789934 johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/health_checks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/health_checks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      973 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/health_checks/hc_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      884 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/health_checks/nlp_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2076 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/health_checks/ocr_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3496 2023-03-30 22:32:50.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/health_checks/report.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6935 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/install_flow.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11362 2023-02-01 13:41:22.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/install_software.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12079 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/jsl_home.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:11:39.789934 johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/lib_resolvers/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      124 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/lib_resolvers/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2061 2023-04-13 00:38:10.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3187 2023-05-16 18:50:33.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2105 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9118 2023-05-16 20:30:52.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/offline_install.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9133 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/softwares.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4710 2023-04-26 14:30:28.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/finance.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      212 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/lab.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4639 2023-04-26 14:30:28.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/legal.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4526 2023-04-26 14:30:28.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/medical.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1367 2023-04-13 01:03:52.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/nlp.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:11:39.789934 johnsnowlabs_tmp-4.4.5/johnsnowlabs/py_models/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/py_models/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4826 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/py_models/install_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    31165 2023-03-26 01:30:02.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/py_models/jsl_secrets.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4168 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/py_models/lib_version.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        2 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/py_models/license_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      128 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/py_models/primitive.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2077 2023-05-16 20:23:18.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/py_models/url_dependency.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2201 2023-05-19 04:10:41.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/settings.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:11:39.793934 johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6657 2023-03-31 10:39:36.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/enums.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4253 2023-04-26 21:13:04.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/env_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      759 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/file_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1005 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/functional.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3326 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/modelhub_markdown.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10004 2023-03-19 17:22:02.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/my_jsl_api.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10654 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/notebooks.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5856 2023-01-31 09:04:19.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/pip_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      982 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/print_messages.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4371 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/py_process.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8019 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/sparksession_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:11:39.793934 johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/testing/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:29:40.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/testing/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4050 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/testing/jsl_pre_processor.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1778 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/testing/nb_code_match.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1132 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/testing/nb_nodes.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3460 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/testing/test_settings.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4353 2023-04-26 21:13:04.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/venv_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1332 2023-04-26 14:30:28.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/visual.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      408 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs/viz.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:11:39.793934 johnsnowlabs_tmp-4.4.5/johnsnowlabs_tmp.egg-info/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9282 2023-05-19 04:11:39.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs_tmp.egg-info/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2486 2023-05-19 04:11:39.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs_tmp.egg-info/SOURCES.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2023-05-19 04:11:39.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs_tmp.egg-info/dependency_links.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      126 2023-05-19 04:11:39.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs_tmp.egg-info/requires.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       13 2023-05-19 04:11:39.000000 johnsnowlabs_tmp-4.4.5/johnsnowlabs_tmp.egg-info/top_level.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2023-05-19 04:11:39.793934 johnsnowlabs_tmp-4.4.5/setup.cfg
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2043 2023-05-19 04:10:58.000000 johnsnowlabs_tmp-4.4.5/setup.py
```

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/__init__.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,20 +10,14 @@
 
     lab = AnnotationLab()
 
 if try_import_lib("sparkocr") and try_import_lib("sparknlp"):
     from johnsnowlabs import visual
 
 
-def refresh_imports():
-    import inspect
-
-    inspect.__globals__
-
-
 def new_version_online():
     from .utils.pip_utils import get_latest_lib_version_on_pypi
 
     # we are outdated, if current version does not match the latest on PypPi
     from .auto_install.softwares import Software
 
     return settings.raw_version_jsl_lib != get_latest_lib_version_on_pypi(
```

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/abstract_base/lib_resolver.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/abstract_base/lib_resolver.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/abstract_base/pydantic_model.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/abstract_base/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/abstract_base/software_product.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/abstract_base/software_product.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/databricks/dbfs.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/databricks/dbfs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # https://pypi.org/project/databricks-api/
+import base64
+import json
+from os.path import dirname
 from typing import Union
 
 from databricks_api import DatabricksAPI
 
 from johnsnowlabs import settings
-from johnsnowlabs.py_models.install_info import PyInstallInfo, JvmInstallInfo
+from johnsnowlabs.py_models.install_info import JvmInstallInfo, PyInstallInfo
 from johnsnowlabs.utils.file_utils import path_tail
 
 
 def dbfs_file_exists(db: DatabricksAPI, path: str):
     try:
         dbfs_ls(db, path)
         return True
@@ -36,14 +39,28 @@
         path=dbfs_path,
         overwrite=overwrite,
         # contents=None,
         src_path=local_path,
     )
 
 
+def put_file_on_dbfs(
+    db: DatabricksAPI, path: str, content: any, overwrite: bool = True
+):
+    try:
+        directory = dirname(path)
+        db.dbfs.mkdirs(directory)
+    except:
+        pass
+    if type(content) != "string":
+        content = json.dumps(content)
+    content = base64.b64encode(content.encode()).decode()
+    db.dbfs.put(path=path, overwrite=overwrite, contents=content)
+
+
 def get_db_path(local_info: Union[JvmInstallInfo, PyInstallInfo, str]):
     """Get a deterministic path for a JvmInstallInfo or PyInstallInfo or local files on dbfs.
     Always use this method to generate output file path for dbfs.
     """
     if isinstance(local_info, JvmInstallInfo):
         return f"{settings.dbfs_java_dir}/{local_info.file_name}"
     elif isinstance(local_info, PyInstallInfo):
```

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/databricks/install_utils.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/databricks/install_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import re
 import time
 from pprint import pprint
+from typing import List, Optional
 
 from johnsnowlabs.auto_install import jsl_home
 from johnsnowlabs.auto_install.softwares import Software
 from johnsnowlabs.py_models.install_info import InstallSuite, LocalPy4JLib, LocalPyLib
 from johnsnowlabs.py_models.lib_version import LibVersion
-from .dbfs import *
+from johnsnowlabs.utils.env_utils import is_running_in_databricks
 
 # https://pypi.org/project/databricks-api/
 from ...utils.enums import DatabricksClusterStates
+from .dbfs import *
 
 
 def get_db_client_for_token(host, token) -> DatabricksAPI:
     # Get client via host or token
     return DatabricksAPI(host=host, token=token)
 
 
@@ -47,17 +49,27 @@
     if not install_suite:
         install_suite = jsl_home.get_install_suite_from_jsl_home()
 
     default_spark_conf = {
         "spark.kryoserializer.buffer.max": "2000M",
         "spark.serializer": "org.apache.spark.serializer.KryoSerializer",
     }
+    lic = {
+        "SECRET": install_suite.secrets.HC_SECRET,
+        "SPARK_OCR_SECRET": install_suite.secrets.OCR_SECRET,
+        "SPARK_NLP_LICENSE": install_suite.secrets.HC_LICENSE,
+        "SPARK_OCR_LICENSE": install_suite.secrets.OCR_LICENSE,
+    }
+    lic = {k: v for k, v in lic.items() if v is not None}
+
+    license_path = "/johnsnowlabs/license.json"
+    put_file_on_dbfs(db, license_path, lic, overwrite=True)
+
     default_spark_env_vars = dict(
-        SPARK_NLP_LICENSE=install_suite.secrets.HC_LICENSE,
-        SPARK_OCR_LICENSE=install_suite.secrets.OCR_LICENSE,
+        SPARK_NLP_LICENSE_FILE=f"/dbfs{license_path}",
         AWS_ACCESS_KEY_ID=install_suite.secrets.AWS_ACCESS_KEY_ID,
         AWS_SECRET_ACCESS_KEY=install_suite.secrets.AWS_SECRET_ACCESS_KEY,
     )
     # Env vars may not be None, so we drop any that are None
     default_spark_env_vars = {
         k: v for k, v in default_spark_env_vars.items() if v is not None
     }
@@ -139,65 +151,127 @@
     pprint(node_types)
 
 
 def install_jsl_suite_to_cluster(
     db: DatabricksAPI,
     cluster_id: str,
     install_suite: InstallSuite,
-    install_optional: bool = True,
 ):
+    py_deps = [
+        {"package": Software.nlu.pypi_name, "version": settings.raw_version_nlu},
+        {
+            "package": Software.sparknlp_display.pypi_name,
+            "version": settings.raw_version_nlp_display,
+        },
+        {
+            "package": Software.jsl_lib.pypi_name_databricks,
+            "version": settings.raw_version_jsl_lib,
+        },
+    ]
+    uninstall_old_libraries(db, cluster_id, py_deps)
     if install_suite.hc.get_py_path() and install_suite.hc.get_java_path():
         install_py4j_lib_via_hdfs(db, cluster_id, install_suite.hc)
         print(
             f"Installed {Software.spark_hc.logo + Software.spark_hc.name} Spark NLP for Healthcare ✅"
         )
     if install_suite.ocr.get_py_path() and install_suite.ocr.get_java_path():
         install_py4j_lib_via_hdfs(db, cluster_id, install_suite.ocr)
         print(
             f"Installed {Software.spark_ocr.logo + Software.spark_ocr.name} Spark OCR ✅"
         )
-    py_deps = [
-        Software.nlu.pypi_name,
-        Software.sparknlp_display.pypi_name,
-        Software.jsl_lib.pypi_name_databricks,
-    ]
+
     for dep in py_deps:
-        install_py_lib_via_pip(db, cluster_id, dep)
+        install_py_lib_via_pip(db, cluster_id, dep["package"], dep["version"])
 
     # Install Sparkr-NLP as last library, so we have the correct version
     if install_suite.nlp.get_py_path() and install_suite.nlp.get_java_path():
         install_py4j_lib_via_hdfs(db, cluster_id, install_suite.nlp)
         print(
             f"{Software.spark_nlp.logo + Software.spark_nlp.name} Installed Spark NLP! ✅"
         )
 
+    # On databricks environment should restart current cluster to apply uninstalls and installations
+    if is_running_in_databricks():
+        try:
+            restart_cluster(db, cluster_id)
+        except:
+            pass
+
 
 def block_till_cluster_ready_state(db: DatabricksAPI, cluster_id: str):
     status = None
     while status != DatabricksClusterStates.RUNNING:
         # https://docs.databricks.com/dev-tools/api/latest/clusters.html#clusterclusterstate
         status = DatabricksClusterStates(db.cluster.get_cluster(cluster_id)["state"])
         print(f"Cluster-Id={cluster_id} not ready, status={status.value}")
         time.sleep(10)
 
     print(f"👌 Cluster-Id {cluster_id} is ready!")
 
 
-def install_py_lib_via_pip(db: DatabricksAPI, cluster_id: str, pypi_lib: str):
+def uninstall_old_libraries(
+    db: DatabricksAPI,
+    cluster_id: str,
+    pypi_deps: List[dict],
+):
+    """
+    Tell Cluster to uninstall old libraries
+    # https://docs.databricks.com/dev-tools/api/latest/libraries.html
+    https://docs.databricks.com/dev-tools/api/latest/libraries.html#install
+    :param db:
+    :param cluster_id:
+    :param pypi_deps:
+    :return:
+    """
+    uninstalls = []
+    statuses = db.managed_library.cluster_status(cluster_id=cluster_id)
+    file_names = [
+        "spark_nlp",
+        "spark_nlp_jsl",
+        "spark_ocr",
+    ]
+    pypi_packages = [d["package"] for d in pypi_deps]
+    for status in statuses.get("library_statuses", []):
+        installation_types = ["jar", "whl", "pypi"]
+        for typ in installation_types:
+            path = status["library"].get(typ)
+            if path:
+                if typ == "pypi":
+                    pkg = path.get("package")
+                    if pkg in pypi_packages:
+                        uninstalls.append({typ: {"package": pkg}})
+                else:
+                    for fil in file_names:
+                        path = path.replace("/dbfs/", "dbfs:/")
+                        if fil in path.replace("-", "_"):
+                            uninstalls.append({typ: path})
+    if uninstalls:
+        db.managed_library.uninstall_libraries(
+            cluster_id=cluster_id, libraries=uninstalls
+        )
+
+
+def install_py_lib_via_pip(
+    db: DatabricksAPI, cluster_id: str, pypi_lib: str, version: Optional[str] = None
+):
     """
     Tell Cluster to install via public pypi
     # https://docs.databricks.com/dev-tools/api/latest/libraries.html
     https://docs.databricks.com/dev-tools/api/latest/libraries.html#install
     :param db:
     :param cluster_id:
-    :param lib:
+    :param pypi_lib:
+    :param version:
     :return:
     """
     # By not defining repo, we will use default pip index
-    payload = [dict(pypi=dict(package=pypi_lib))]
+    pypi = dict(package=pypi_lib)
+    if version:
+        pypi["version"] = version
+    payload = [dict(pypi=pypi)]
     db.managed_library.install_libraries(cluster_id=cluster_id, libraries=payload)
     print(f"Installed {pypi_lib} ✅")
 
 
 def install_py4j_lib_via_hdfs(db: DatabricksAPI, cluster_id: str, lib: LocalPy4JLib):
     """
     1. Copy lib files to HDFS if not present
@@ -268,7 +342,11 @@
         elif status in [
             DatabricksClusterStates.TERMINATED,
             DatabricksClusterStates.TERMINATING,
             DatabricksClusterStates.ERROR,
             DatabricksClusterStates.UNKNOWN,
         ]:
             return False
+
+
+def restart_cluster(db: DatabricksAPI, cluster_id: str):
+    db.cluster.restart_cluster(cluster_id=cluster_id)
```

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/databricks/work_utils.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/databricks/work_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/health_checks/hc_test.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/health_checks/hc_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/health_checks/nlp_test.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/health_checks/nlp_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/health_checks/ocr_test.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/health_checks/ocr_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/health_checks/report.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/health_checks/report.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/install_flow.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/install_flow.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/install_software.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/install_software.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/jsl_home.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/jsl_home.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py`

 * *Files 15% similar despite different names*

```diff
@@ -46,28 +46,27 @@
                 spark_version=SparkVersion.spark3xx,
                 product_name=product_name,
                 file_name=product_name.name,
                 dependency_version=lib_version,
             ),
         }
     }
-
     compatible_spark_to_py_map = {
         SparkVersion.spark3xx: {
             # TODO HARDCODE HASH!!! OR grap from enum or somwhere comfy. Maybe configs/settings file?
             PyInstallTypes.wheel: UrlDependency(
-                url="https://files.pythonhosted.org/packages/53/ed/b90d8ce6dcacb824d72682100bb717e07a6c2c04748a80d14fc6f2ec3360/spark_nlp-{lib_version}-py2.py3-none-any.whl",
+                url="https://files.pythonhosted.org/packages/ad/02/b86152a985aaa66d628b9d07263a5df640daaae32388cbbf38851677baf6/spark_nlp-{lib_version}-py2.py3-none-any.whl",
                 dependency_type=PyInstallTypes.wheel,
                 spark_version=SparkVersion.spark3xx,
                 product_name=product_name,
                 file_name=product_name.name,
                 dependency_version=lib_version,
             ),
             PyInstallTypes.tar: UrlDependency(
-                url="https://files.pythonhosted.org/packages/5a/af/9c73a6a6a74f2848209001194bef19b74cfe04fdd070aec529d290ce239d/spark-nlp-{lib_version}.tar.gz",
+                url="https://files.pythonhosted.org/packages/35/89/87dc31013c9a4f1d0ce71b38e93172bad49652ec3f587a4d4e40c91b439e/spark-nlp-{lib_version}.tar.gz",
                 dependency_type=PyInstallTypes.tar,
                 spark_version=SparkVersion.spark3xx,
                 product_name=product_name,
                 file_name=product_name.name,
                 dependency_version=lib_version,
             ),
         }
```

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/offline_install.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/offline_install.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+
+import requests
 from typing import List, Tuple
 
+from johnsnowlabs import settings
+
 from johnsnowlabs.auto_install.lib_resolvers import (
     OcrLibResolver,
     HcLibResolver,
     NlpLibResolver,
 )
 from johnsnowlabs.py_models.jsl_secrets import JslSecrets
 from johnsnowlabs.py_models.url_dependency import UrlDependency
 from johnsnowlabs.utils.enums import PyInstallTypes, ProductLogo, JvmHardwareTarget
 
 
 def get_printable_dependency_urls(
-    secrets: JslSecrets,
-    jvm_install_type: JvmHardwareTarget = JvmHardwareTarget.cpu,
-    py_install_type: PyInstallTypes = PyInstallTypes.wheel,
-    spark_version=None,
+        secrets: JslSecrets,
+        jvm_install_type: JvmHardwareTarget = JvmHardwareTarget.cpu,
+        py_install_type: PyInstallTypes = PyInstallTypes.wheel,
+        spark_version=None,
 ) -> Tuple[List[str], List[str]]:
     """
     Get URL for every dependency to which the found_secrets have access to with respect to CURRENT pyspark install.
     If no pyspark is installed, this fails because we need to know pyspark version to generate correct URL
     :param jvm_install_type:
     :param spark_version:
     :param secrets:
@@ -91,22 +95,22 @@
     print(
         f"Make sure all these dependencies are installed on your Spark Driver and Worker nodes"
     )
     return java_dependencies, py_dependencies
 
 
 def get_py4j_dependency_urls(
-    secrets: JslSecrets,
-    jvm_install_type: JvmHardwareTarget = JvmHardwareTarget.cpu,
-    py_install_type: PyInstallTypes = PyInstallTypes.wheel,
-    spark_version=None,
-    get_all_jvm_hardware_targets: bool = False,
-    visual=False,
-    nlp=True,
-    spark_nlp=True,
+        secrets: JslSecrets,
+        jvm_install_type: JvmHardwareTarget = JvmHardwareTarget.cpu,
+        py_install_type: PyInstallTypes = PyInstallTypes.wheel,
+        spark_version=None,
+        get_all_jvm_hardware_targets: bool = False,
+        visual=False,
+        nlp=True,
+        spark_nlp=True,
 ) -> Tuple[List[UrlDependency], List[UrlDependency]]:
     """
     Get URL for every dependency to which the found_secrets have access to with respect to CURRENT pyspark install.
     If no pyspark is installed, this fails because we need to know pyspark version to generate correct URL
     :param jvm_install_type:
     :param spark_version:
     :param get_all_jvm_hardware_targets:
@@ -138,25 +142,17 @@
                 NlpLibResolver.get_jar_urls(
                     hardware_target=jvm_install_type,
                     spark_version_to_match=spark_version,
                 )
             )
 
         if py_install_type == PyInstallTypes.wheel:
-            py_dependencies.append(
-                NlpLibResolver.get_py_urls(
-                    install_type=py_install_type, spark_version_to_match=spark_version
-                )
-            )
-        else:
-            py_dependencies.append(
-                NlpLibResolver.get_py_urls(
-                    install_type=py_install_type, spark_version_to_match=spark_version
-                )
-            )
+            url = NlpLibResolver.get_py_urls(install_type=py_install_type, spark_version_to_match=spark_version)
+            url.url = get_wheel_and_pypi('spark-nlp', settings.raw_version_nlp)[0]
+            py_dependencies.append(url)
 
     if secrets and secrets.HC_SECRET and nlp:
         java_dependencies.append(
             HcLibResolver.get_jar_urls(
                 secret=secrets.HC_SECRET, spark_version_to_match=spark_version
             )
         )
@@ -164,22 +160,14 @@
             py_dependencies.append(
                 HcLibResolver.get_py_urls(
                     secret=secrets.HC_SECRET,
                     install_type=py_install_type,
                     spark_version_to_match=spark_version,
                 )
             )
-        else:
-            py_dependencies.append(
-                HcLibResolver.get_py_urls(
-                    secret=secrets.HC_SECRET,
-                    install_type=py_install_type,
-                    spark_version_to_match=spark_version,
-                )
-            )
 
     if secrets and secrets.OCR_SECRET and visual:
         java_dependencies.append(
             OcrLibResolver.get_jar_urls(
                 secret=secrets.OCR_SECRET, spark_version_to_match=spark_version
             )
         )
@@ -187,17 +175,37 @@
             py_dependencies.append(
                 OcrLibResolver.get_py_urls(
                     secret=secrets.OCR_SECRET,
                     install_type=py_install_type,
                     spark_version_to_match=spark_version,
                 )
             )
-        else:
-            py_dependencies.append(
-                OcrLibResolver.get_py_urls(
-                    secret=secrets.OCR_SECRET,
-                    install_type=py_install_type,
-                    spark_version_to_match=spark_version,
-                )
-            )
 
     return java_dependencies, py_dependencies
+
+def get_wheel_and_pypi(pypi_name, version):
+    # Construct the API URL
+    api_url = f"https://pypi.org/pypi/{pypi_name}/{version}/json"
+
+    try:
+        # Send a GET request to the PyPI API
+        response = requests.get(api_url)
+        response.raise_for_status()  # Raise an exception for any HTTP errors
+
+        # Parse the JSON response
+        data = response.json()
+
+        wheel_url = None
+        tarball_url = None
+
+        # Extract the download URLs for wheels and tarballs
+        for release in data["urls"]:
+            if release["packagetype"] == "bdist_wheel":
+                wheel_url = release["url"]
+            elif release["packagetype"] == "sdist":
+                tarball_url = release["url"]
+
+        return wheel_url, tarball_url
+
+    except requests.exceptions.RequestException as e:
+        print(f"Could not find Pypi Wheel/Tar for {pypi_name}=={version}: {e}")
+        return None, None
```

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/auto_install/softwares.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/auto_install/softwares.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/finance.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/finance.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 import traceback
 
 from johnsnowlabs.abstract_base.lib_resolver import try_import_lib
+from johnsnowlabs.utils.env_utils import reverse_compatibility_import
 from johnsnowlabs.utils.print_messages import log_broken_lib
 
 try:
 
     if try_import_lib("sparknlp_jsl") and try_import_lib("sparknlp"):
+        from sparknlp_jsl.functions import *
+        from sparknlp_jsl.training import *
         from sparknlp_jsl.structured_deidentification import StructuredDeidentification
         from sparknlp_jsl.base import FeaturesAssembler
+        from sparknlp_jsl.annotator.windowed.windowed_sentence import (
+            WindowedSentenceModel,
+        )
+        from sparknlp_jsl.training_log_parser import ner_log_parser
 
         from sparknlp_jsl.finance import (
+            GenericClassifierModel,
             FinanceNerQuestionGenerator as NerQuestionGenerator,
             FinanceDocumentHashCoder as DocumentHashCoder,
             FinanceBertForTokenClassification as BertForTokenClassification,
             FinanceDocumentMLClassifierModel as DocumentMLClassifierModel,
             FinanceDocumentMLClassifierApproach as DocumentMLClassifierApproach,
             DocMapperApproach,
             DocMapperModel,
@@ -30,18 +38,25 @@
             AssertionDLModel,
             RelationExtractionDLModel,
             ZeroShotRelationExtractionModel,
             ChunkMapperApproach,
             SentenceEntityResolverApproach,
             AssertionDLApproach,
             ZeroShotNerModel,
+            FinanceQuestionAnswering as QuestionAnswering,
+            FinanceTextGenerator as TextGenerator,
+            FinanceSummarizer as Summarizer,
         )
 
         # These are licensed annos shared across all libs
         from sparknlp_jsl.annotator import (
+            GenericSVMClassifierApproach,
+            GenericSVMClassifierModel,
+            GenericLogRegClassifierApproach,
+            GenericClassifierModel,
             SentenceDetector as TextSplitter,
             MedicalDistilBertForSequenceClassification as DistilBertForSequenceClassification,
             AssertionChunkConverter,
             AssertionLogRegModel,
             DeIdentificationModel,
             DocumentLogRegClassifierModel,
             RelationExtractionModel,
@@ -79,15 +94,15 @@
             NameChunkObfuscatorApproach,
             NameChunkObfuscator,
             Resolution2Chunk,
             ResolverMerger,
         )
 
         from sparknlp_jsl.modelTracer import ModelTracer
-        from sparknlp_jsl import training_log_parser
+        from sparknlp_jsl import training_log_parser, Deid
         from sparknlp_jsl.compatibility import Compatibility
         from sparknlp_jsl.pretrained import InternalResourceDownloader
         from sparknlp_jsl.eval import (
             NerDLMetrics,
             NerDLEvaluation,
             SymSpellEvaluation,
             POSEvaluation,
@@ -96,7 +111,9 @@
         )
 
 except Exception as err:
     if try_import_lib("sparknlp_jsl") and try_import_lib("sparknlp"):
         log_broken_lib("Enterprise Finance")
         print(f"Error Message : {err}")
         print(f"Error Trace: {traceback.format_exc()}")
+        print("Performing reverse compatibility import for legal module")
+        reverse_compatibility_import(__file__, globals())
```

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/legal.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/legal.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 import traceback
 
 from johnsnowlabs.abstract_base.lib_resolver import try_import_lib
+from johnsnowlabs.utils.env_utils import reverse_compatibility_import
 from johnsnowlabs.utils.print_messages import log_broken_lib
 
 try:
     if try_import_lib("sparknlp_jsl") and try_import_lib("sparknlp"):
+        from sparknlp_jsl.functions import *
+        from sparknlp_jsl.training import *
+        from sparknlp_jsl.annotator.windowed.windowed_sentence import (
+            WindowedSentenceModel,
+        )
+        from sparknlp_jsl.training_log_parser import ner_log_parser
+
         from sparknlp_jsl.base import FeaturesAssembler
 
         from sparknlp_jsl.legal import (
             LegalDocumentHashCoder as DocumentHashCoder,
             LegalNerQuestionGenerator as NerQuestionGenerator,
             LegalBertForSequenceClassification as BertForSequenceClassification,
             LegalDocumentMLClassifierModel as DocumentMLClassifierModel,
@@ -26,18 +34,25 @@
             AssertionDLModel,
             RelationExtractionDLModel,
             ZeroShotRelationExtractionModel,
             ChunkMapperApproach,
             SentenceEntityResolverApproach,
             AssertionDLApproach,
             ZeroShotNerModel,
+            LegalQuestionAnswering as QuestionAnswering,
+            LegalTextGenerator as TextGenerator,
+            LegalSummarizer as Summarizer,
         )
 
         # These are licensed annos shared across all libs
         from sparknlp_jsl.annotator import (
+            GenericSVMClassifierApproach,
+            GenericSVMClassifierModel,
+            GenericLogRegClassifierApproach,
+            GenericClassifierModel,
             SentenceDetector as TextSplitter,
             MedicalDistilBertForSequenceClassification as DistilBertForSequenceClassification,
             AssertionChunkConverter,
             AssertionLogRegModel,
             DeIdentificationModel,
             DocumentLogRegClassifierModel,
             RelationExtractionModel,
@@ -78,15 +93,16 @@
             # Resolution2Chunk,
             ResolverMerger,
         )
         from sparknlp_jsl.modelTracer import ModelTracer
 
         from sparknlp_jsl.structured_deidentification import StructuredDeidentification
 
-        from sparknlp_jsl import training_log_parser
+        from sparknlp_jsl import training_log_parser, Deid
+
         from sparknlp_jsl.compatibility import Compatibility
         from sparknlp_jsl.pretrained import InternalResourceDownloader
         from sparknlp_jsl.eval import (
             NerDLMetrics,
             NerDLEvaluation,
             SymSpellEvaluation,
             POSEvaluation,
@@ -96,7 +112,9 @@
 
 
 except Exception as err:
     if try_import_lib("sparknlp_jsl") and try_import_lib("sparknlp"):
         log_broken_lib("Enterprise Finance")
         print(f"Error Message : {err}")
         print(f"Error Trace: {traceback.format_exc()}")
+        print("Performing reverse compatibility import for legal module")
+        reverse_compatibility_import(__file__, globals())
```

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/medical.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/medical.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 import traceback
-
 from johnsnowlabs.abstract_base.lib_resolver import try_import_lib
 from johnsnowlabs.auto_install.softwares import Software
+from johnsnowlabs.utils.env_utils import reverse_compatibility_import
 from johnsnowlabs.utils.print_messages import log_outdated_lib, log_broken_lib
 
 warning_logged = False
 
 try:
     if try_import_lib("sparknlp_jsl") and try_import_lib("sparknlp"):
-        # Pretrained
+        from sparknlp_jsl.functions import *
+        from sparknlp_jsl.training import *
+        from sparknlp_jsl.annotator.windowed.windowed_sentence import (
+            WindowedSentenceModel,
+        )
         from sparknlp_jsl.annotator import (
+            GenericSVMClassifierApproach,
+            GenericSVMClassifierModel,
+            GenericLogRegClassifierApproach,
+            GenericClassifierModel,
             AssertionLogRegModel,
             AssertionDLModel,
             DeIdentificationModel,
             DocumentLogRegClassifierModel,
             RelationExtractionModel,
             RelationExtractionDLModel,
             ChunkMergeModel,
@@ -59,51 +67,52 @@
             DocMapperModel,
             DocMapperApproach,
             NameChunkObfuscatorApproach,
             NameChunkObfuscator,
             DocumentMLClassifierApproach,
             DocumentMLClassifierModel,
             Resolution2Chunk,
+            MedicalQuestionAnswering,
         )
         from sparknlp_jsl.structured_deidentification import StructuredDeidentification
         from sparknlp_jsl.modelTracer import ModelTracer
-        from sparknlp_jsl import training_log_parser
+        from sparknlp_jsl import training_log_parser, Deid
+        from sparknlp_jsl.training_log_parser import ner_log_parser
 
         from sparknlp_jsl.base import FeaturesAssembler
 
         from sparknlp_jsl.annotator.resolution.resolver_merger import ResolverMerger
 
-        from sparknlp_jsl.annotator import MedicalNerModel as NerModel
-        from sparknlp_jsl.annotator import MedicalNerApproach as NerApproach
-        from sparknlp_jsl.annotator import (
-            MedicalBertForTokenClassifier as BertForTokenClassification,
-        )
         from sparknlp_jsl.annotator import (
             MedicalDistilBertForSequenceClassification as DistilBertForSequenceClassification,
-        )
-        from sparknlp_jsl.annotator import (
             MedicalBertForSequenceClassification as BertForSequenceClassification,
+            MedicalBertForTokenClassifier as BertForTokenClassification,
+            MedicalNerModel as NerModel,
+            MedicalNerApproach as NerApproach,
+            MedicalQuestionAnswering as QuestionAnswering,
+            MedicalTextGenerator as TextGenerator,
+            MedicalSummarizer as Summarizer,
         )
         from sparknlp_jsl.compatibility import Compatibility
         from sparknlp_jsl.pretrained import InternalResourceDownloader
         from sparknlp_jsl.eval import (
             NerDLMetrics,
             NerDLEvaluation,
             SymSpellEvaluation,
             POSEvaluation,
             NerCrfEvaluation,
             NorvigSpellEvaluation,
         )
 
-        from sparknlp_jsl.functions import *
-        from sparknlp_jsl.training import *
 except Exception as err:
     log_broken_lib(Software.spark_hc)
     print(f"Error Message : {err}")
     print(f"Error Trace: {traceback.format_exc()}")
+    print("Performing reverse compatibility import for medical module")
+    reverse_compatibility_import(__file__, globals())
 
 if try_import_lib("sparknlp_jsl") and try_import_lib("sparknlp"):
     if not Software.spark_hc.check_installed_correct_version() and not warning_logged:
         warning_logged = True
         import sparknlp_jsl
 
         log_outdated_lib(Software.spark_hc, sparknlp_jsl.version())
```

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/nlp.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/nlp.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/py_models/install_info.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/py_models/install_info.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/py_models/jsl_secrets.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/py_models/jsl_secrets.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,24 @@
     "HC_VERSION",
     "OCR_SECRET",
     "OCR_LICENSE",
     "JSL_LEGAL_LICENSE",
     "JSL_FINANCE_LICENSE",
 ]
 
+license_file_keys = [
+    "JSL_NLP_LICENSE_FILE",
+    "SPARK_NLP_LICENSE_FILE",
+    "SPARK_OCR_LICENSE_FILE",
+    "JSL_OCR_LICENSE_FILE",
+    "JSL_LICENSE_FILE",
+    "JSL_LEGAL_LICENSE_FILE",
+    "JSL_FINANCE_LICENSE_FILE",
+]
+
 already_logged = False
 ocr_validation_logged = False
 hc_validation_logged = False
 
 
 class JslSecrets(WritableBaseModel):
     """Representation of a JSL credentials and helper
@@ -241,15 +251,17 @@
 
             # elif email and passw:
             #     found_secrets = JslSecrets.from_email_and_pass(email, passw,local_license_number)
 
             elif secrets_file:
                 # Load from JSON file from provided secret file
                 secrets = JslSecrets.from_json_file_path(secrets_file)
-
+            elif any([key for key in license_file_keys if key in os.environ]):
+                key = next(k for k in license_file_keys if os.environ.get(k))
+                secrets = JslSecrets.from_json_file_path(os.environ[key])
             if not secrets and not force_browser:
                 # Try auto Resolve credentials if none are supplied
                 secrets = JslSecrets.search_default_locations(
                     license_number=local_license_number
                 )
             if not secrets and not force_browser:
                 # Search Env Vars
```

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/py_models/lib_version.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/py_models/lib_version.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/py_models/url_dependency.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/py_models/url_dependency.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,17 @@
             return False
 
     def download_url(
         self, save_path, name_print_prefix: str = "", keep_default_file_name=True
     ):
         if not UrlDependency.internet_on():
             print(
-                f"Warning! It looks like there is no active internet connection on this machine"
+                f"Warning! It looks like there is no active internet connection on this machine "
+                f"Trying to continue but might run into problems..."
             )
-            print(f"Trying to continue but might run into problems...")
 
         if not self.validate():
             raise ValueError(f"Trying to download Invalid URL! {self.url}")
         if keep_default_file_name:
             self.file_name = self.url.split("/")[-1]
         save_path = save_path + "/" + self.file_name
```

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/settings.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 from johnsnowlabs.utils.env_utils import (
     is_running_in_databricks,
     set_py4j_logger_to_error_on_databricks,
     env_required_license,
 )
 
 # These versions are used for auto-installs and version  checks
-raw_version_jsl_lib = "4.2.9"
-raw_version_nlp = "4.2.8"
-raw_version_nlu = "4.0.1rc4"
+raw_version_jsl_lib = "4.4.5"
+raw_version_nlp = "4.4.1"
+raw_version_nlu = "4.2.0"
 raw_version_pyspark = "3.1.2"
 raw_version_nlp_display = "4.1"
 
-raw_version_medical = "4.2.8"
-raw_version_secret_medical = "4.2.8"
+raw_version_medical = "4.4.2"
+raw_version_secret_medical = "4.4.2"
 
-raw_version_secret_ocr = "4.3.0"
-raw_version_ocr = "4.3.0"
+raw_version_secret_ocr = "4.4.0"
+raw_version_ocr = "4.4.0"
 
 pypi_page = "https://pypi.org/project/johnsnowlabs"
 
 json_indent = 4
 enforce_secret_on_version = False
 enforce_versions = True
```

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/enums.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/enums.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/file_utils.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/functional.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/functional.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/modelhub_markdown.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/modelhub_markdown.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/my_jsl_api.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/my_jsl_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,15 +259,15 @@
     else:
         print("Please confirm authorization on :", url)
         webbrowser.open_new_tab(url)
 
 
 def get_access_key_from_browser():
     in_colab = is_in_colab_notebook()
-    client_id = "sI4MKSmLHOX2Pg7XhM3McJS2oyKG5PHcp0BlANEW"
+    client_id = "2hfGX0iZ5lvyxvLaK3IEzS9Bc9LGfTYCwVvKFfjY"
 
     class OauthRequestHandler(BaseHTTPRequestHandler):
         code = None
 
         def response(self, msg, code):
             self.send_response(code)
             self.end_headers()
```

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/notebooks.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/pip_utils.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/pip_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/print_messages.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/print_messages.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/py_process.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/py_process.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/sparksession_utils.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/sparksession_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/testing/jsl_pre_processor.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/testing/jsl_pre_processor.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/testing/nb_code_match.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/testing/nb_code_match.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/testing/nb_nodes.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/testing/nb_nodes.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/testing/test_settings.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/testing/test_settings.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/utils/venv_utils.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/utils/venv_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     print("______________STDERR:")
     print(result.stderr.decode())
 
 
 #
 # @dataclass
 # class VenvState:
-#     installed_libs: list[str]
+#     installed_libs: List[str]
 #     py_version: str
 
 
 class VenvWrapper:
     """
     Utils to install into a Python Executable, which is not the same as current the currently running one
     I.e. whenever you want to install to a local python executable which is != sys.executable use this
```

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs/visual.py` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs/visual.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from johnsnowlabs.utils.print_messages import log_outdated_lib, log_broken_lib
 from johnsnowlabs.abstract_base.lib_resolver import try_import_lib
 from johnsnowlabs.auto_install.softwares import Software
 
 warning_logged = False
 if try_import_lib("sparkocr") and try_import_lib("sparknlp"):
     try:
+        from sparkocr.base import *
+
         from sparkocr.transformers import *
         from sparkocr.enums import *
         import pkg_resources
         import sparkocr
         from sparkocr.utils import *
         from sparkocr.schemas import *
         from sparkocr.metrics import *
+        from sparkocr.pretrained import *
         from sparkocr.databricks import isRunningInDatabricks
 
         if isRunningInDatabricks():
             # Overwrites functions imported from sparkocr.utils
             # but this is fine, since these are not compatible on databricks
             from sparkocr.databricks import *
```

### Comparing `johnsnowlabs_tmp-4.2.9/johnsnowlabs_tmp.egg-info/SOURCES.txt` & `johnsnowlabs_tmp-4.4.5/johnsnowlabs_tmp.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 johnsnowlabs/__init__.py
 johnsnowlabs/finance.py
 johnsnowlabs/lab.py
 johnsnowlabs/legal.py
 johnsnowlabs/medical.py
```

### Comparing `johnsnowlabs_tmp-4.2.9/setup.py` & `johnsnowlabs_tmp-4.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 REQUIRED_PKGS = [
-    # f"pyspark=={johnsnowlabs.settings.raw_version_pyspark}",
+    f"pyspark=={johnsnowlabs.settings.raw_version_pyspark}",
     f"spark-nlp=={johnsnowlabs.settings.raw_version_nlp}",
     f"nlu=={johnsnowlabs.settings.raw_version_nlu}",
     f"spark-nlp-display=={johnsnowlabs.settings.raw_version_nlp_display}",
     "numpy",
     "dataclasses",
     "requests",
     "databricks-api",
     "pydantic",
     "colorama",
 ]
 
 setup(
     version=johnsnowlabs.settings.raw_version_jsl_lib,
-    # name='johnsnowlabs_for_databricks',
     name="johnsnowlabs_tmp",
+    # name="johnsnowlabs",
     description="The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for "
     "Finance, Legal and Medical domains. Easily scalable to Spark Cluster ",
     long_description=long_description,
     install_requires=REQUIRED_PKGS,
     long_description_content_type="text/markdown",
     url="https://www.johnsnowlabs.com/",
     author="John Snow Labs",
```

