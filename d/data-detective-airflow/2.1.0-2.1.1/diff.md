# Comparing `tmp/data_detective_airflow-2.1.0.tar.gz` & `tmp/data_detective_airflow-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_detective_airflow-2.1.0.tar", max compression
+gzip compressed data, was "data_detective_airflow-2.1.1.tar", max compression
```

## Comparing `data_detective_airflow-2.1.0.tar` & `data_detective_airflow-2.1.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1016 2022-10-12 09:00:19.823203 data_detective_airflow-2.1.0/README.md
--rw-r--r--   0        0        0        0 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/__init__.py
--rw-r--r--   0        0        0     1833 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/constants.py
--rw-r--r--   0        0        0      380 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/__init__.py
--rw-r--r--   0        0        0      269 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/dags/__init__.py
--rw-r--r--   0        0        0     1205 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/dags/python_dag.py
--rw-r--r--   0        0        0     5798 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/dags/tdag.py
--rw-r--r--   0        0        0     2205 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/dags/yaml_dag.py
--rw-r--r--   0        0        0     2304 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/generator.py
--rw-r--r--   0        0        0      309 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/results/__init__.py
--rw-r--r--   0        0        0     2246 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/results/base_result.py
--rw-r--r--   0        0        0     2475 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/results/pg_result.py
--rw-r--r--   0        0        0     1794 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/results/pickle_result.py
--rw-r--r--   0        0        0      554 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/works/__init__.py
--rw-r--r--   0        0        0     2441 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/works/base_db_work.py
--rw-r--r--   0        0        0     2445 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/works/base_file_work.py
--rw-r--r--   0        0        0     6609 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/works/base_work.py
--rw-r--r--   0        0        0     2739 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/works/file_work.py
--rw-r--r--   0        0        0    10786 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/works/pg_work.py
--rw-r--r--   0        0        0     4127 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/works/s3_work.py
--rw-r--r--   0        0        0     7520 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/works/sftp_work.py
--rw-r--r--   0        0        0     1986 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/operators/__init__.py
--rw-r--r--   0        0        0      591 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/operators/extractors/__init__.py
--rw-r--r--   0        0        0      946 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/operators/extractors/db_dump.py
--rw-r--r--   0        0        0      854 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/operators/extractors/python_dump.py
--rw-r--r--   0        0        0     3189 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/operators/extractors/request_dump.py
--rw-r--r--   0        0        0     2537 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/operators/extractors/s3_dump.py
--rw-r--r--   0        0        0     3187 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/operators/extractors/s3_list_bucket.py
--rw-r--r--   0        0        0      992 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/operators/extractors/tsftpoperator.py
--rw-r--r--   0        0        0      261 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/operators/sinks/__init__.py
--rw-r--r--   0        0        0     1720 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/operators/sinks/pg_loader.py
--rw-r--r--   0        0        0    14341 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/operators/sinks/pg_scd1.py
--rw-r--r--   0        0        0     6448 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/operators/sinks/pg_scd1_df_update_insert.py
--rw-r--r--   0        0        0     4604 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/operators/sinks/pg_single_target_loader.py
--rw-r--r--   0        0        0     6218 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/operators/sinks/pg_single_target_utils.py
--rw-r--r--   0        0        0     2782 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/operators/sinks/s3_delete.py
--rw-r--r--   0        0        0     2782 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/operators/sinks/s3_load.py
--rw-r--r--   0        0        0     4626 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/operators/tbaseoperator.py
--rw-r--r--   0        0        0      287 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/operators/transformers/__init__.py
--rw-r--r--   0        0        0     1180 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/operators/transformers/append.py
--rw-r--r--   0        0        0     1994 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/operators/transformers/pg_sql.py
--rw-r--r--   0        0        0     2002 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/operators/transformers/py_transform.py
--rw-r--r--   0        0        0      781 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/test_utilities/__init__.py
--rw-r--r--   0        0        0     1044 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/test_utilities/airflow.py
--rw-r--r--   0        0        0     1570 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/test_utilities/assertions.py
--rw-r--r--   0        0        0     1852 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/test_utilities/datasets.py
--rw-r--r--   0        0        0     2163 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/test_utilities/generate.py
--rw-r--r--   0        0        0     3218 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/test_utilities/generate_df.py
--rw-r--r--   0        0        0     3488 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/test_utilities/test_helper.py
--rw-r--r--   0        0        0     1595 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/test_utilities/test_utils_petl.py
--rw-r--r--   0        0        0      933 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/utils/logging_thread.py
--rw-r--r--   0        0        0      422 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/utils/notnull.py
--rw-r--r--   0        0        0     1223 2022-10-12 09:00:19.827203 data_detective_airflow-2.1.0/data_detective_airflow/utils/petl_utils.py
--rw-r--r--   0        0        0     2056 2022-10-12 09:00:19.831203 data_detective_airflow-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     2350 2022-10-12 09:03:03.162400 data_detective_airflow-2.1.0/setup.py
--rw-r--r--   0        0        0     2363 2022-10-12 09:03:03.162907 data_detective_airflow-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1016 2023-05-19 06:47:27.214679 data_detective_airflow-2.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/__init__.py
+-rw-r--r--   0        0        0     1833 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/constants.py
+-rw-r--r--   0        0        0      380 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/__init__.py
+-rw-r--r--   0        0        0      269 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/dags/__init__.py
+-rw-r--r--   0        0        0     1205 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/dags/python_dag.py
+-rw-r--r--   0        0        0     5798 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/dags/tdag.py
+-rw-r--r--   0        0        0     2205 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/dags/yaml_dag.py
+-rw-r--r--   0        0        0     2304 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/generator.py
+-rw-r--r--   0        0        0      309 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/results/__init__.py
+-rw-r--r--   0        0        0     2246 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/results/base_result.py
+-rw-r--r--   0        0        0     2475 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/results/pg_result.py
+-rw-r--r--   0        0        0     1794 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/results/pickle_result.py
+-rw-r--r--   0        0        0      554 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/__init__.py
+-rw-r--r--   0        0        0     2441 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/base_db_work.py
+-rw-r--r--   0        0        0     2445 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/base_file_work.py
+-rw-r--r--   0        0        0     6609 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/base_work.py
+-rw-r--r--   0        0        0     2739 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/file_work.py
+-rw-r--r--   0        0        0    10786 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/pg_work.py
+-rw-r--r--   0        0        0     4127 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/s3_work.py
+-rw-r--r--   0        0        0     7520 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/sftp_work.py
+-rw-r--r--   0        0        0     1986 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/__init__.py
+-rw-r--r--   0        0        0      591 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/__init__.py
+-rw-r--r--   0        0        0      946 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/db_dump.py
+-rw-r--r--   0        0        0      854 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/python_dump.py
+-rw-r--r--   0        0        0     3189 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/request_dump.py
+-rw-r--r--   0        0        0     2537 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/s3_dump.py
+-rw-r--r--   0        0        0     3187 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/s3_list_bucket.py
+-rw-r--r--   0        0        0      992 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/tsftpoperator.py
+-rw-r--r--   0        0        0      261 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/__init__.py
+-rw-r--r--   0        0        0     1720 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/pg_loader.py
+-rw-r--r--   0        0        0    14341 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/pg_scd1.py
+-rw-r--r--   0        0        0     6448 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/pg_scd1_df_update_insert.py
+-rw-r--r--   0        0        0     4604 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/pg_single_target_loader.py
+-rw-r--r--   0        0        0     6218 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/pg_single_target_utils.py
+-rw-r--r--   0        0        0     2782 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/s3_delete.py
+-rw-r--r--   0        0        0     2782 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/s3_load.py
+-rw-r--r--   0        0        0     4626 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/tbaseoperator.py
+-rw-r--r--   0        0        0      287 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/transformers/__init__.py
+-rw-r--r--   0        0        0     1180 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/transformers/append.py
+-rw-r--r--   0        0        0     1994 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/transformers/pg_sql.py
+-rw-r--r--   0        0        0     2002 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/operators/transformers/py_transform.py
+-rw-r--r--   0        0        0      781 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/__init__.py
+-rw-r--r--   0        0        0     1044 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/airflow.py
+-rw-r--r--   0        0        0     1570 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/assertions.py
+-rw-r--r--   0        0        0     1852 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/datasets.py
+-rw-r--r--   0        0        0     2552 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/generate.py
+-rw-r--r--   0        0        0     3218 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/generate_df.py
+-rw-r--r--   0        0        0     3488 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/test_helper.py
+-rw-r--r--   0        0        0     1595 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/test_utils_petl.py
+-rw-r--r--   0        0        0      933 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/utils/logging_thread.py
+-rw-r--r--   0        0        0      422 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/utils/notnull.py
+-rw-r--r--   0        0        0     1223 2023-05-19 06:47:27.218679 data_detective_airflow-2.1.1/data_detective_airflow/utils/petl_utils.py
+-rw-r--r--   0        0        0     2056 2023-05-19 06:47:27.222679 data_detective_airflow-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2358 1970-01-01 00:00:00.000000 data_detective_airflow-2.1.1/setup.py
+-rw-r--r--   0        0        0     2464 1970-01-01 00:00:00.000000 data_detective_airflow-2.1.1/PKG-INFO
```

### Comparing `data_detective_airflow-2.1.0/README.md` & `data_detective_airflow-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/constants.py` & `data_detective_airflow-2.1.1/data_detective_airflow/constants.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/dags/python_dag.py` & `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/dags/python_dag.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/dags/tdag.py` & `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/dags/tdag.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/dags/yaml_dag.py` & `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/dags/yaml_dag.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/generator.py` & `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/generator.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/results/base_result.py` & `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/results/base_result.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/results/pg_result.py` & `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/results/pg_result.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/results/pickle_result.py` & `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/results/pickle_result.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/works/__init__.py` & `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/__init__.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/works/base_db_work.py` & `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/base_db_work.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/works/base_file_work.py` & `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/base_file_work.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/works/base_work.py` & `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/base_work.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/works/file_work.py` & `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/file_work.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/works/pg_work.py` & `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/pg_work.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/works/s3_work.py` & `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/s3_work.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/dag_generator/works/sftp_work.py` & `data_detective_airflow-2.1.1/data_detective_airflow/dag_generator/works/sftp_work.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/operators/__init__.py` & `data_detective_airflow-2.1.1/data_detective_airflow/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/operators/extractors/__init__.py` & `data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/operators/extractors/db_dump.py` & `data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/db_dump.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/operators/extractors/python_dump.py` & `data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/python_dump.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/operators/extractors/request_dump.py` & `data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/request_dump.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/operators/extractors/s3_dump.py` & `data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/s3_dump.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/operators/extractors/s3_list_bucket.py` & `data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/s3_list_bucket.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/operators/extractors/tsftpoperator.py` & `data_detective_airflow-2.1.1/data_detective_airflow/operators/extractors/tsftpoperator.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/operators/sinks/pg_loader.py` & `data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/pg_loader.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/operators/sinks/pg_scd1.py` & `data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/pg_scd1.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/operators/sinks/pg_scd1_df_update_insert.py` & `data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/pg_scd1_df_update_insert.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/operators/sinks/pg_single_target_loader.py` & `data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/pg_single_target_loader.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/operators/sinks/pg_single_target_utils.py` & `data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/pg_single_target_utils.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/operators/sinks/s3_delete.py` & `data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/s3_delete.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/operators/sinks/s3_load.py` & `data_detective_airflow-2.1.1/data_detective_airflow/operators/sinks/s3_load.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/operators/tbaseoperator.py` & `data_detective_airflow-2.1.1/data_detective_airflow/operators/tbaseoperator.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/operators/transformers/append.py` & `data_detective_airflow-2.1.1/data_detective_airflow/operators/transformers/append.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/operators/transformers/pg_sql.py` & `data_detective_airflow-2.1.1/data_detective_airflow/operators/transformers/pg_sql.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/operators/transformers/py_transform.py` & `data_detective_airflow-2.1.1/data_detective_airflow/operators/transformers/py_transform.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/test_utilities/__init__.py` & `data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/test_utilities/airflow.py` & `data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/airflow.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/test_utilities/assertions.py` & `data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/assertions.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/test_utilities/datasets.py` & `data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/datasets.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/test_utilities/generate.py` & `data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/generate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,37 @@
 import logging
 import os
 from typing import Union
 
 import pandas
 import petl as etl
-from airflow.models import BaseOperator, TaskInstance
-from airflow.utils import timezone
+from airflow.models import BaseOperator, DagRun, TaskInstance
 
 from data_detective_airflow.operators.tbaseoperator import TBaseOperator
 from data_detective_airflow.test_utilities.datasets import JSONPandasDataset, JSONPetlDataset
 from data_detective_airflow.test_utilities.test_helper import run_and_read
 
 
 # pylint: disable=too-many-statements
-def run_and_gen_ds(task: Union[TBaseOperator, BaseOperator], folder, dag_run, drop_cols: list[str] = None):
+def run_and_gen_ds(
+    task: Union[TBaseOperator, BaseOperator],
+    folder: str,
+    dag_run: DagRun,
+    drop_cols: list[str] = None,
+    save_md: bool = False,
+):
+    """Run the task and generate dataset and JSON/Markdown for check
+
+    :param task: Id of the running task
+    :param folder: Path to DAG's folder
+    :param dag_run: Airflow DagRun
+    :param drop_cols: Columns for drop
+    :param save_md: Flag for generating Markdown
+    """
+
     drop_cols = drop_cols or []
     if 'processed_dttm' not in drop_cols:
         drop_cols.append('processed_dttm')
 
     task_instance = TaskInstance(task=task, run_id=dag_run.run_id, execution_date=dag_run.execution_date)
     context = task_instance.get_template_context()
 
@@ -28,30 +42,35 @@
 
     if isinstance(task_result, pandas.DataFrame):
         pd_result = task_result.drop(labels=drop_cols, axis=1, errors='ignore')
 
         dataset = JSONPandasDataset(folder)
 
         dataset[task.task_id] = pd_result
-        try:
-            dataset.save_md(task.task_id, pd_result)
-        except UnicodeDecodeError:
-            logging.warning(f'Cant save md for {task.task_id}: containing non-ascii bytes')
+
+        if save_md:
+            try:
+                dataset.save_md(task.task_id, pd_result)
+            except UnicodeDecodeError:
+                logging.warning(f'Cant save md for {task.task_id}: containing non-ascii bytes')
+
     elif isinstance(task_result, etl.Table):
         header = etl.header(task_result)
         cut_header = [col for col in header if col not in drop_cols]
         cut_table = task_result.cut(cut_header)
 
         dataset = JSONPetlDataset(folder)
 
         dataset[task.task_id] = cut_table
-        try:
-            dataset.save_md(task.task_id, cut_table)
-        except UnicodeDecodeError:
-            logging.warning(f'Cant save md for {task.task_id}: containing non-ascii bytes')
+
+        if save_md:
+            try:
+                dataset.save_md(task.task_id, cut_table)
+            except UnicodeDecodeError:
+                logging.warning(f'Cant save md for {task.task_id}: containing non-ascii bytes')
     else:
         return
 
 
 def is_gen_dataset_mode() -> bool:
     """Switching the mode of checking and creating test data
```

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/test_utilities/generate_df.py` & `data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/generate_df.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/test_utilities/test_helper.py` & `data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/test_helper.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/test_utilities/test_utils_petl.py` & `data_detective_airflow-2.1.1/data_detective_airflow/test_utilities/test_utils_petl.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/utils/logging_thread.py` & `data_detective_airflow-2.1.1/data_detective_airflow/utils/logging_thread.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/data_detective_airflow/utils/petl_utils.py` & `data_detective_airflow-2.1.1/data_detective_airflow/utils/petl_utils.py`

 * *Files identical despite different names*

### Comparing `data_detective_airflow-2.1.0/pyproject.toml` & `data_detective_airflow-2.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "data_detective_airflow"
 license = "Apache-2.0"
-version = "2.1.0"
+version = "2.1.1"
 description = "Framework with task testing over Apache Airflow"
 authors = ["Tinkoff Data Detective Team"]
 readme = 'README.md'  # Markdown files are supported
 keywords = ["airflow testing result metadata governance catalog data detective"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

### Comparing `data_detective_airflow-2.1.0/setup.py` & `data_detective_airflow-2.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,22 +25,22 @@
  'apache-airflow-providers-ssh',
  'apache-airflow>=2.4,<2.5',
  'pandas>=1.1,<1.6',
  'petl>=1.7,<2.0']
 
 setup_kwargs = {
     'name': 'data-detective-airflow',
-    'version': '2.1.0',
+    'version': '2.1.1',
     'description': 'Framework with task testing over Apache Airflow',
     'long_description': '## Data Detective Airflow\n\n[Data Detective Airflow](https://github.com/tinkoff/data-detective/tree/master/data-detective-airflow) is a framework\nwhose main idea is to add the concepts of work and result to [Apache Airflow](https://airflow.apache.org/).\nIt supports tasks testing over [Apache Airflow](https://airflow.apache.org/).\nData Detective Airflow allows developers to create workflows in the form of directed acyclic graphs (DAGs) of tasks.\nThe easy-to-use Data Detective Airflow scheduler makes it possible to run tasks and save results into works. \nWork storage support for s3, ftp, local disk and database is also included.\n\n[More information about Data Detective Airflow](https://data-detective.dev/docs/data-detective-airflow/intro)\n\n## Installation\n\n#### Install from [PyPi](https://pypi.org/project/data-detective-airflow/)\n\n```bash\npip install data-detective-airflow\n```\n\nSee example DAG-s in [dags/dags](https://github.com/tinkoff/data-detective/tree/master/data-detective-airflow/dags/dags) folder.\n',
     'author': 'Tinkoff Data Detective Team',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'author_email': 'None',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.9,<4.0',
 }
```

### Comparing `data_detective_airflow-2.1.0/PKG-INFO` & `data_detective_airflow-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: data-detective-airflow
-Version: 2.1.0
+Version: 2.1.1
 Summary: Framework with task testing over Apache Airflow
 License: Apache-2.0
 Keywords: airflow testing result metadata governance catalog data detective
 Author: Tinkoff Data Detective Team
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: apache-airflow (>=2.4,<2.5)
 Requires-Dist: apache-airflow-providers-amazon
 Requires-Dist: apache-airflow-providers-celery
 Requires-Dist: apache-airflow-providers-postgres
 Requires-Dist: apache-airflow-providers-redis
```

