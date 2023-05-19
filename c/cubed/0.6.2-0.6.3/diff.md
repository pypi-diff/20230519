# Comparing `tmp/cubed-0.6.2.tar.gz` & `tmp/cubed-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubed-0.6.2.tar", last modified: Fri May 12 11:19:21 2023, max compression
+gzip compressed data, was "cubed-0.6.3.tar", last modified: Fri May 19 11:17:54 2023, max compression
```

## Comparing `cubed-0.6.2.tar` & `cubed-0.6.3.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.078756 cubed-0.6.2/
--rw-r--r--   0 tom        (501) staff       (20)    11358 2023-05-12 10:58:36.000000 cubed-0.6.2/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)     1868 2023-05-12 11:19:21.078886 cubed-0.6.2/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      939 2023-02-21 09:42:15.000000 cubed-0.6.2/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.062905 cubed-0.6.2/cubed/
--rw-r--r--   0 tom        (501) staff       (20)      846 2023-05-05 10:22:49.000000 cubed-0.6.2/cubed/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.066460 cubed-0.6.2/cubed/array_api/
--rw-r--r--   0 tom        (501) staff       (20)     3578 2023-02-16 11:53:37.000000 cubed-0.6.2/cubed/array_api/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    12924 2023-02-16 11:53:37.000000 cubed-0.6.2/cubed/array_api/array_object.py
--rw-r--r--   0 tom        (501) staff       (20)       81 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/array_api/constants.py
--rw-r--r--   0 tom        (501) staff       (20)     8760 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/array_api/creation_functions.py
--rw-r--r--   0 tom        (501) staff       (20)      751 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/array_api/data_type_functions.py
--rw-r--r--   0 tom        (501) staff       (20)      471 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/array_api/dtypes.py
--rw-r--r--   0 tom        (501) staff       (20)    11395 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/array_api/elementwise_functions.py
--rw-r--r--   0 tom        (501) staff       (20)       83 2023-02-16 11:53:37.000000 cubed-0.6.2/cubed/array_api/indexing_functions.py
--rw-r--r--   0 tom        (501) staff       (20)     4016 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/array_api/linear_algebra_functions.py
--rw-r--r--   0 tom        (501) staff       (20)     9132 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/array_api/manipulation_functions.py
--rw-r--r--   0 tom        (501) staff       (20)     1010 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/array_api/searching_functions.py
--rw-r--r--   0 tom        (501) staff       (20)     3693 2023-03-17 17:46:35.000000 cubed-0.6.2/cubed/array_api/statistical_functions.py
--rw-r--r--   0 tom        (501) staff       (20)      479 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/array_api/utility_functions.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.067894 cubed-0.6.2/cubed/core/
--rw-r--r--   0 tom        (501) staff       (20)      431 2023-02-17 17:56:56.000000 cubed-0.6.2/cubed/core/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    11826 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/core/array.py
--rw-r--r--   0 tom        (501) staff       (20)     5531 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/core/gufunc.py
--rw-r--r--   0 tom        (501) staff       (20)    26650 2023-05-11 13:34:35.000000 cubed-0.6.2/cubed/core/ops.py
--rw-r--r--   0 tom        (501) staff       (20)    11573 2023-05-11 13:34:35.000000 cubed-0.6.2/cubed/core/plan.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.068648 cubed-0.6.2/cubed/extensions/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/extensions/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1164 2023-05-11 13:34:35.000000 cubed-0.6.2/cubed/extensions/history.py
--rw-r--r--   0 tom        (501) staff       (20)     2738 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/extensions/timeline.py
--rw-r--r--   0 tom        (501) staff       (20)     1439 2023-02-16 11:53:37.000000 cubed-0.6.2/cubed/extensions/tqdm.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.069469 cubed-0.6.2/cubed/primitive/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/primitive/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    10932 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/primitive/blockwise.py
--rw-r--r--   0 tom        (501) staff       (20)     1853 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/primitive/rechunk.py
--rw-r--r--   0 tom        (501) staff       (20)      355 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/primitive/types.py
--rw-r--r--   0 tom        (501) staff       (20)     1381 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/random.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.070768 cubed-0.6.2/cubed/runtime/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/runtime/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      953 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/runtime/backup.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.072337 cubed-0.6.2/cubed/runtime/executors/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/runtime/executors/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     8292 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/runtime/executors/beam.py
--rw-r--r--   0 tom        (501) staff       (20)     9228 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/runtime/executors/lithops.py
--rw-r--r--   0 tom        (501) staff       (20)     3460 2023-03-27 13:45:10.000000 cubed-0.6.2/cubed/runtime/executors/modal.py
--rw-r--r--   0 tom        (501) staff       (20)     6115 2023-05-10 09:39:13.000000 cubed-0.6.2/cubed/runtime/executors/modal_async.py
--rw-r--r--   0 tom        (501) staff       (20)     1279 2023-02-16 11:53:37.000000 cubed-0.6.2/cubed/runtime/executors/python.py
--rw-r--r--   0 tom        (501) staff       (20)     4187 2023-05-10 09:39:13.000000 cubed-0.6.2/cubed/runtime/executors/python_async.py
--rw-r--r--   0 tom        (501) staff       (20)     3620 2023-03-17 17:46:35.000000 cubed-0.6.2/cubed/runtime/pipeline.py
--rw-r--r--   0 tom        (501) staff       (20)      251 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/runtime/types.py
--rw-r--r--   0 tom        (501) staff       (20)      118 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/runtime/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.074620 cubed-0.6.2/cubed/tests/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/tests/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.075109 cubed-0.6.2/cubed/tests/primitive/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/tests/primitive/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     6308 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/tests/primitive/test_blockwise.py
--rw-r--r--   0 tom        (501) staff       (20)     2505 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/tests/primitive/test_rechunk.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.075847 cubed-0.6.2/cubed/tests/runtime/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/tests/runtime/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      860 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/tests/runtime/test_backup.py
--rw-r--r--   0 tom        (501) staff       (20)     4014 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/tests/runtime/test_lithops.py
--rw-r--r--   0 tom        (501) staff       (20)     4691 2023-03-27 13:45:10.000000 cubed-0.6.2/cubed/tests/runtime/test_modal_async.py
--rw-r--r--   0 tom        (501) staff       (20)    16651 2023-02-16 11:53:37.000000 cubed-0.6.2/cubed/tests/test_array_api.py
--rw-r--r--   0 tom        (501) staff       (20)    14366 2023-05-11 10:25:04.000000 cubed-0.6.2/cubed/tests/test_core.py
--rw-r--r--   0 tom        (501) staff       (20)     3024 2023-02-21 09:41:17.000000 cubed-0.6.2/cubed/tests/test_gufunc.py
--rw-r--r--   0 tom        (501) staff       (20)     1450 2023-02-16 11:53:37.000000 cubed-0.6.2/cubed/tests/test_indexing.py
--rw-r--r--   0 tom        (501) staff       (20)     6778 2023-05-11 13:34:35.000000 cubed-0.6.2/cubed/tests/test_mem_utilization.py
--rw-r--r--   0 tom        (501) staff       (20)     2393 2023-02-16 11:53:37.000000 cubed-0.6.2/cubed/tests/test_optimization.py
--rw-r--r--   0 tom        (501) staff       (20)     1221 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/tests/test_random.py
--rw-r--r--   0 tom        (501) staff       (20)     2231 2023-02-16 11:53:37.000000 cubed-0.6.2/cubed/tests/test_utils.py
--rw-r--r--   0 tom        (501) staff       (20)     2703 2023-05-11 08:51:38.000000 cubed-0.6.2/cubed/tests/utils.py
--rw-r--r--   0 tom        (501) staff       (20)     4302 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.076035 cubed-0.6.2/cubed/vendor/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/vendor/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.076763 cubed-0.6.2/cubed/vendor/dask/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/vendor/dask/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.077498 cubed-0.6.2/cubed/vendor/dask/array/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/vendor/dask/array/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    17366 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/vendor/dask/array/core.py
--rw-r--r--   0 tom        (501) staff       (20)     1685 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/vendor/dask/array/gufunc.py
--rw-r--r--   0 tom        (501) staff       (20)     4670 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/vendor/dask/array/reshape.py
--rw-r--r--   0 tom        (501) staff       (20)      543 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/vendor/dask/array/utils.py
--rw-r--r--   0 tom        (501) staff       (20)    14901 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/vendor/dask/blockwise.py
--rw-r--r--   0 tom        (501) staff       (20)      608 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/vendor/dask/core.py
--rw-r--r--   0 tom        (501) staff       (20)     2221 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/vendor/dask/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.078336 cubed-0.6.2/cubed/vendor/rechunker/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/vendor/rechunker/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    13197 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/vendor/rechunker/algorithm.py
--rw-r--r--   0 tom        (501) staff       (20)    12312 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/vendor/rechunker/api.py
--rw-r--r--   0 tom        (501) staff       (20)      309 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/vendor/rechunker/compat.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.078612 cubed-0.6.2/cubed/vendor/rechunker/executors/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/vendor/rechunker/executors/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      923 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/vendor/rechunker/executors/python.py
--rw-r--r--   0 tom        (501) staff       (20)     3421 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/vendor/rechunker/types.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.063696 cubed-0.6.2/cubed.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)     1868 2023-05-12 11:19:21.000000 cubed-0.6.2/cubed.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     2506 2023-05-12 11:19:21.000000 cubed-0.6.2/cubed.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-05-12 11:19:21.000000 cubed-0.6.2/cubed.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)      407 2023-05-12 11:19:21.000000 cubed-0.6.2/cubed.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)        6 2023-05-12 11:19:21.000000 cubed-0.6.2/cubed.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)     1652 2023-05-12 11:18:26.000000 cubed-0.6.2/pyproject.toml
--rw-r--r--   0 tom        (501) staff       (20)     1195 2023-05-12 11:19:21.079544 cubed-0.6.2/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)      289 2023-05-12 07:47:27.000000 cubed-0.6.2/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.267562 cubed-0.6.3/
+-rw-r--r--   0 tom        (501) staff       (20)    11358 2023-05-16 07:59:53.000000 cubed-0.6.3/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)     1868 2023-05-19 11:17:54.267632 cubed-0.6.3/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      939 2023-02-21 09:42:15.000000 cubed-0.6.3/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.256810 cubed-0.6.3/cubed/
+-rw-r--r--   0 tom        (501) staff       (20)      846 2023-05-05 10:22:49.000000 cubed-0.6.3/cubed/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.259121 cubed-0.6.3/cubed/array_api/
+-rw-r--r--   0 tom        (501) staff       (20)     3578 2023-02-16 11:53:37.000000 cubed-0.6.3/cubed/array_api/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    12924 2023-02-16 11:53:37.000000 cubed-0.6.3/cubed/array_api/array_object.py
+-rw-r--r--   0 tom        (501) staff       (20)       81 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/array_api/constants.py
+-rw-r--r--   0 tom        (501) staff       (20)     8760 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/array_api/creation_functions.py
+-rw-r--r--   0 tom        (501) staff       (20)      751 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/array_api/data_type_functions.py
+-rw-r--r--   0 tom        (501) staff       (20)      471 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/array_api/dtypes.py
+-rw-r--r--   0 tom        (501) staff       (20)    11395 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/array_api/elementwise_functions.py
+-rw-r--r--   0 tom        (501) staff       (20)       83 2023-02-16 11:53:37.000000 cubed-0.6.3/cubed/array_api/indexing_functions.py
+-rw-r--r--   0 tom        (501) staff       (20)     4016 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/array_api/linear_algebra_functions.py
+-rw-r--r--   0 tom        (501) staff       (20)     9132 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/array_api/manipulation_functions.py
+-rw-r--r--   0 tom        (501) staff       (20)     1010 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/array_api/searching_functions.py
+-rw-r--r--   0 tom        (501) staff       (20)     3693 2023-03-17 17:46:35.000000 cubed-0.6.3/cubed/array_api/statistical_functions.py
+-rw-r--r--   0 tom        (501) staff       (20)      479 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/array_api/utility_functions.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.259813 cubed-0.6.3/cubed/core/
+-rw-r--r--   0 tom        (501) staff       (20)      431 2023-02-17 17:56:56.000000 cubed-0.6.3/cubed/core/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    11826 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/core/array.py
+-rw-r--r--   0 tom        (501) staff       (20)     5531 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/core/gufunc.py
+-rw-r--r--   0 tom        (501) staff       (20)    26650 2023-05-19 08:43:28.000000 cubed-0.6.3/cubed/core/ops.py
+-rw-r--r--   0 tom        (501) staff       (20)    11573 2023-05-19 08:43:28.000000 cubed-0.6.3/cubed/core/plan.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.260500 cubed-0.6.3/cubed/extensions/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/extensions/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1164 2023-05-19 08:43:28.000000 cubed-0.6.3/cubed/extensions/history.py
+-rw-r--r--   0 tom        (501) staff       (20)     2738 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/extensions/timeline.py
+-rw-r--r--   0 tom        (501) staff       (20)     1439 2023-02-16 11:53:37.000000 cubed-0.6.3/cubed/extensions/tqdm.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.261086 cubed-0.6.3/cubed/primitive/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/primitive/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    10932 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/primitive/blockwise.py
+-rw-r--r--   0 tom        (501) staff       (20)     1853 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/primitive/rechunk.py
+-rw-r--r--   0 tom        (501) staff       (20)      355 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/primitive/types.py
+-rw-r--r--   0 tom        (501) staff       (20)     1381 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/random.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.261829 cubed-0.6.3/cubed/runtime/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/runtime/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      953 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/runtime/backup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.263041 cubed-0.6.3/cubed/runtime/executors/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/runtime/executors/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     8292 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/runtime/executors/beam.py
+-rw-r--r--   0 tom        (501) staff       (20)     9228 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/runtime/executors/lithops.py
+-rw-r--r--   0 tom        (501) staff       (20)     3460 2023-03-27 13:45:10.000000 cubed-0.6.3/cubed/runtime/executors/modal.py
+-rw-r--r--   0 tom        (501) staff       (20)     6115 2023-05-10 09:39:13.000000 cubed-0.6.3/cubed/runtime/executors/modal_async.py
+-rw-r--r--   0 tom        (501) staff       (20)     1279 2023-02-16 11:53:37.000000 cubed-0.6.3/cubed/runtime/executors/python.py
+-rw-r--r--   0 tom        (501) staff       (20)     4187 2023-05-10 09:39:13.000000 cubed-0.6.3/cubed/runtime/executors/python_async.py
+-rw-r--r--   0 tom        (501) staff       (20)     3620 2023-03-17 17:46:35.000000 cubed-0.6.3/cubed/runtime/pipeline.py
+-rw-r--r--   0 tom        (501) staff       (20)      251 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/runtime/types.py
+-rw-r--r--   0 tom        (501) staff       (20)      118 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/runtime/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.264359 cubed-0.6.3/cubed/tests/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/tests/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.264718 cubed-0.6.3/cubed/tests/primitive/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/tests/primitive/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     6323 2023-05-19 11:15:54.000000 cubed-0.6.3/cubed/tests/primitive/test_blockwise.py
+-rw-r--r--   0 tom        (501) staff       (20)     2505 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/tests/primitive/test_rechunk.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.265197 cubed-0.6.3/cubed/tests/runtime/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/tests/runtime/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      860 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/tests/runtime/test_backup.py
+-rw-r--r--   0 tom        (501) staff       (20)     4014 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/tests/runtime/test_lithops.py
+-rw-r--r--   0 tom        (501) staff       (20)     4691 2023-03-27 13:45:10.000000 cubed-0.6.3/cubed/tests/runtime/test_modal_async.py
+-rw-r--r--   0 tom        (501) staff       (20)    16651 2023-02-16 11:53:37.000000 cubed-0.6.3/cubed/tests/test_array_api.py
+-rw-r--r--   0 tom        (501) staff       (20)    14469 2023-05-19 11:15:54.000000 cubed-0.6.3/cubed/tests/test_core.py
+-rw-r--r--   0 tom        (501) staff       (20)     3024 2023-02-21 09:41:17.000000 cubed-0.6.3/cubed/tests/test_gufunc.py
+-rw-r--r--   0 tom        (501) staff       (20)     1450 2023-02-16 11:53:37.000000 cubed-0.6.3/cubed/tests/test_indexing.py
+-rw-r--r--   0 tom        (501) staff       (20)     6778 2023-05-19 08:43:28.000000 cubed-0.6.3/cubed/tests/test_mem_utilization.py
+-rw-r--r--   0 tom        (501) staff       (20)     2393 2023-02-16 11:53:37.000000 cubed-0.6.3/cubed/tests/test_optimization.py
+-rw-r--r--   0 tom        (501) staff       (20)     1221 2022-10-17 16:19:52.000000 cubed-0.6.3/cubed/tests/test_random.py
+-rw-r--r--   0 tom        (501) staff       (20)     2292 2023-05-19 11:15:54.000000 cubed-0.6.3/cubed/tests/test_utils.py
+-rw-r--r--   0 tom        (501) staff       (20)     2861 2023-05-19 11:15:54.000000 cubed-0.6.3/cubed/tests/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)     4494 2023-05-19 11:15:54.000000 cubed-0.6.3/cubed/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.265323 cubed-0.6.3/cubed/vendor/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/vendor/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.265777 cubed-0.6.3/cubed/vendor/dask/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/vendor/dask/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.266386 cubed-0.6.3/cubed/vendor/dask/array/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/vendor/dask/array/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    17366 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/vendor/dask/array/core.py
+-rw-r--r--   0 tom        (501) staff       (20)     1685 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/vendor/dask/array/gufunc.py
+-rw-r--r--   0 tom        (501) staff       (20)     4670 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/vendor/dask/array/reshape.py
+-rw-r--r--   0 tom        (501) staff       (20)      543 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/vendor/dask/array/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)    14901 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/vendor/dask/blockwise.py
+-rw-r--r--   0 tom        (501) staff       (20)      608 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/vendor/dask/core.py
+-rw-r--r--   0 tom        (501) staff       (20)     2221 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/vendor/dask/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.267219 cubed-0.6.3/cubed/vendor/rechunker/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/vendor/rechunker/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    13197 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/vendor/rechunker/algorithm.py
+-rw-r--r--   0 tom        (501) staff       (20)    12312 2023-03-21 10:44:51.000000 cubed-0.6.3/cubed/vendor/rechunker/api.py
+-rw-r--r--   0 tom        (501) staff       (20)      309 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/vendor/rechunker/compat.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.267455 cubed-0.6.3/cubed/vendor/rechunker/executors/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/vendor/rechunker/executors/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      923 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/vendor/rechunker/executors/python.py
+-rw-r--r--   0 tom        (501) staff       (20)     3421 2023-03-17 13:01:21.000000 cubed-0.6.3/cubed/vendor/rechunker/types.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-19 11:17:54.257462 cubed-0.6.3/cubed.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)     1868 2023-05-19 11:17:54.000000 cubed-0.6.3/cubed.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     2506 2023-05-19 11:17:54.000000 cubed-0.6.3/cubed.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-05-19 11:17:54.000000 cubed-0.6.3/cubed.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)      407 2023-05-19 11:17:54.000000 cubed-0.6.3/cubed.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)        6 2023-05-19 11:17:54.000000 cubed-0.6.3/cubed.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)     1652 2023-05-19 11:17:18.000000 cubed-0.6.3/pyproject.toml
+-rw-r--r--   0 tom        (501) staff       (20)     1195 2023-05-19 11:17:54.268182 cubed-0.6.3/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)      289 2023-05-16 07:59:53.000000 cubed-0.6.3/setup.py
```

### Comparing `cubed-0.6.2/LICENSE` & `cubed-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/PKG-INFO` & `cubed-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubed
-Version: 0.6.2
+Version: 0.6.3
 Summary: Bounded-memory serverless distributed N-dimensional array processing
 Author-email: Tom White <tom.e.white@gmail.com>
 License: Apache License 2.0
 Project-URL: homepage, https://github.com/tomwhite/cubed
 Project-URL: documentation, https://tomwhite.github.io/cubed
 Project-URL: repository, https://github.com/tomwhite/cubed
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cubed-0.6.2/README.md` & `cubed-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/__init__.py` & `cubed-0.6.3/cubed/__init__.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/array_api/__init__.py` & `cubed-0.6.3/cubed/array_api/__init__.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/array_api/array_object.py` & `cubed-0.6.3/cubed/array_api/array_object.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/array_api/creation_functions.py` & `cubed-0.6.3/cubed/array_api/creation_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/array_api/data_type_functions.py` & `cubed-0.6.3/cubed/array_api/data_type_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/array_api/elementwise_functions.py` & `cubed-0.6.3/cubed/array_api/elementwise_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/array_api/linear_algebra_functions.py` & `cubed-0.6.3/cubed/array_api/linear_algebra_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/array_api/manipulation_functions.py` & `cubed-0.6.3/cubed/array_api/manipulation_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/array_api/searching_functions.py` & `cubed-0.6.3/cubed/array_api/searching_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/array_api/statistical_functions.py` & `cubed-0.6.3/cubed/array_api/statistical_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/core/array.py` & `cubed-0.6.3/cubed/core/array.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/core/gufunc.py` & `cubed-0.6.3/cubed/core/gufunc.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/core/ops.py` & `cubed-0.6.3/cubed/core/ops.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/core/plan.py` & `cubed-0.6.3/cubed/core/plan.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/extensions/history.py` & `cubed-0.6.3/cubed/extensions/history.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/extensions/timeline.py` & `cubed-0.6.3/cubed/extensions/timeline.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/extensions/tqdm.py` & `cubed-0.6.3/cubed/extensions/tqdm.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/primitive/blockwise.py` & `cubed-0.6.3/cubed/primitive/blockwise.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/primitive/rechunk.py` & `cubed-0.6.3/cubed/primitive/rechunk.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/random.py` & `cubed-0.6.3/cubed/random.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/runtime/backup.py` & `cubed-0.6.3/cubed/runtime/backup.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/runtime/executors/beam.py` & `cubed-0.6.3/cubed/runtime/executors/beam.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/runtime/executors/lithops.py` & `cubed-0.6.3/cubed/runtime/executors/lithops.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/runtime/executors/modal.py` & `cubed-0.6.3/cubed/runtime/executors/modal.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/runtime/executors/modal_async.py` & `cubed-0.6.3/cubed/runtime/executors/modal_async.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/runtime/executors/python.py` & `cubed-0.6.3/cubed/runtime/executors/python.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/runtime/executors/python_async.py` & `cubed-0.6.3/cubed/runtime/executors/python_async.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/runtime/pipeline.py` & `cubed-0.6.3/cubed/runtime/pipeline.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/tests/primitive/test_blockwise.py` & `cubed-0.6.3/cubed/tests/primitive/test_blockwise.py`

 * *Files 8% similar despite different names*

```diff
@@ -116,18 +116,18 @@
     assert_array_equal(
         res[:], np.transpose(np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]]), axes=(1, 0))
     )
 
 
 def test_blockwise_max_mem_exceeded(tmp_path):
     source1 = create_zarr(
-        [0, 1, 2], dtype=int, chunks=2, store=tmp_path / "source1.zarr"
+        [0, 1, 2], dtype=np.int64, chunks=2, store=tmp_path / "source1.zarr"
     )
     source2 = create_zarr(
-        [10, 50, 100], dtype=int, chunks=2, store=tmp_path / "source2.zarr"
+        [10, 50, 100], dtype=np.int64, chunks=2, store=tmp_path / "source2.zarr"
     )
     max_mem = 100
     target_store = tmp_path / "target.zarr"
 
     with pytest.raises(
         ValueError, match=r"Blockwise memory \(\d+\) exceeds max_mem \(100\)"
     ):
@@ -137,15 +137,15 @@
             source1,
             "i",
             source2,
             "j",
             max_mem=max_mem,
             target_store=target_store,
             shape=(3, 3),
-            dtype=int,
+            dtype=np.int64,
             chunks=(2, 2),
         )
 
 
 def test_make_blockwise_function_map():
     func = lambda x: 0
```

### Comparing `cubed-0.6.2/cubed/tests/primitive/test_rechunk.py` & `cubed-0.6.3/cubed/tests/primitive/test_rechunk.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/tests/runtime/test_backup.py` & `cubed-0.6.3/cubed/tests/runtime/test_backup.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/tests/runtime/test_lithops.py` & `cubed-0.6.3/cubed/tests/runtime/test_lithops.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/tests/runtime/test_modal_async.py` & `cubed-0.6.3/cubed/tests/runtime/test_modal_async.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/tests/test_array_api.py` & `cubed-0.6.3/cubed/tests/test_array_api.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/tests/test_core.py` & `cubed-0.6.3/cubed/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import platform
+
 import dill
 import fsspec
 import numpy as np
 import pytest
 import zarr
 from numpy.testing import assert_array_equal
 
@@ -436,14 +438,15 @@
 
     # since c has already been computed, when computing d only 4 tasks are run, instead of 8
     task_counter = TaskCounter()
     d.compute(callbacks=[task_counter], optimize_graph=False)
     assert task_counter.value == 4
 
 
+@pytest.mark.skipif(platform.system() == "Windows", reason="does not run on windows")
 def test_measure_reserved_memory(executor):
     pytest.importorskip("lithops")
 
     from cubed.runtime.executors.lithops import LithopsDagExecutor
 
     if not isinstance(executor, LithopsDagExecutor):
         pytest.skip(f"{type(executor)} does not support measure_reserved_memory")
```

### Comparing `cubed-0.6.2/cubed/tests/test_gufunc.py` & `cubed-0.6.3/cubed/tests/test_gufunc.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/tests/test_indexing.py` & `cubed-0.6.3/cubed/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/tests/test_mem_utilization.py` & `cubed-0.6.3/cubed/tests/test_mem_utilization.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/tests/test_optimization.py` & `cubed-0.6.3/cubed/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/tests/test_random.py` & `cubed-0.6.3/cubed/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/tests/test_utils.py` & `cubed-0.6.3/cubed/tests/test_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import inspect
+import platform
 
 import numpy as np
 import pytest
 
 from cubed.utils import (
     chunk_memory,
     extract_stack_summaries,
@@ -10,15 +11,14 @@
     memory_repr,
     peak_memory,
     to_chunksize,
 )
 
 
 def test_chunk_memory():
-    assert chunk_memory(int, (3,)) == 24
     assert chunk_memory(np.int64, (3,)) == 24
     assert chunk_memory(np.int32, (3,)) == 12
     assert chunk_memory(np.int32, (3, 5)) == 60
     assert chunk_memory(np.int32, (0,)) == 0
 
 
 def test_to_chunksize():
@@ -52,14 +52,15 @@
     assert memory_repr(999) == "999 bytes"
     assert memory_repr(1_000) == "1.0 KB"
     assert memory_repr(9_999) == "10.0 KB"
     assert memory_repr(1_000_000) == "1.0 MB"
     assert memory_repr(1_000_000_000_000_000) == "1.0 PB"
 
 
+@pytest.mark.skipif(platform.system() == "Windows", reason="does not run on windows")
 def test_peak_memory():
     assert peak_memory() > 0
 
 
 def test_extract_stack_summaries():
     frame = inspect.currentframe()
     stack_summaries = extract_stack_summaries(frame)
```

### Comparing `cubed-0.6.2/cubed/tests/utils.py` & `cubed-0.6.3/cubed/tests/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import platform
 from typing import Iterable
 
 import numpy as np
 import zarr
 
 from cubed.core.array import Callback
 from cubed.runtime.executors.python import PythonDagExecutor
@@ -9,20 +10,25 @@
 from cubed.vendor.rechunker.executors.python import PythonPipelineExecutor
 
 LITHOPS_LOCAL_CONFIG = {"lithops": {"backend": "localhost", "storage": "localhost"}}
 
 ALL_EXECUTORS = [
     PythonPipelineExecutor(),
     PythonDagExecutor(),
-    AsyncPythonDagExecutor(),
 ]
 
 # don't run all tests on every executor as it's too slow, so just have a subset
 MAIN_EXECUTORS = [PythonPipelineExecutor(), PythonDagExecutor()]
 
+
+if platform.system() != "Windows":
+    # AsyncPythonDagExecutor calls `peak_memory` which is not supported on Windows
+    ALL_EXECUTORS.append(AsyncPythonDagExecutor())
+
+
 try:
     from cubed.runtime.executors.beam import BeamDagExecutor, BeamPipelineExecutor
 
     ALL_EXECUTORS.append(BeamDagExecutor())
     ALL_EXECUTORS.append(BeamPipelineExecutor())
 
     MAIN_EXECUTORS.append(BeamDagExecutor())
```

### Comparing `cubed-0.6.2/cubed/utils.py` & `cubed-0.6.3/cubed/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import sysconfig
 import traceback
 from dataclasses import dataclass
 from math import prod
 from operator import add
 from pathlib import Path
 from posixpath import join
-from resource import RUSAGE_SELF, getrusage
 from typing import Union
 from urllib.parse import quote, unquote, urlsplit, urlunsplit
 
 import numpy as np
 import tlz as toolz
 
 from cubed.vendor.dask.array.core import _check_regular_chunks
@@ -68,15 +67,24 @@
     for x in ["KB", "MB", "GB", "TB", "PB"]:
         if num < 1000.0:
             return f"{num:3.1f} {x}"
         num /= 1000.0
 
 
 def peak_memory():
-    """Return the peak memory usage in bytes."""
+    """Return the peak memory usage in bytes.
+
+    Note: this function currently doesn't work on Windows.
+    """
+
+    if platform.system() == "Windows":
+        raise NotImplementedError("`peak_memory` is not implemented on Windows")
+
+    from resource import RUSAGE_SELF, getrusage
+
     ru_maxrss = getrusage(RUSAGE_SELF).ru_maxrss
     # note that on Linux ru_maxrss is in KiB, while on Mac it is in bytes
     # see https://pythonspeed.com/articles/estimating-memory-usage/#measuring-peak-memory-usage
     return ru_maxrss * 1024 if platform.system() == "Linux" else ru_maxrss
 
 
 def to_chunksize(chunkset):
```

### Comparing `cubed-0.6.2/cubed/vendor/dask/array/core.py` & `cubed-0.6.3/cubed/vendor/dask/array/core.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/vendor/dask/array/gufunc.py` & `cubed-0.6.3/cubed/vendor/dask/array/gufunc.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/vendor/dask/array/reshape.py` & `cubed-0.6.3/cubed/vendor/dask/array/reshape.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/vendor/dask/array/utils.py` & `cubed-0.6.3/cubed/vendor/dask/array/utils.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/vendor/dask/blockwise.py` & `cubed-0.6.3/cubed/vendor/dask/blockwise.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/vendor/dask/core.py` & `cubed-0.6.3/cubed/vendor/dask/core.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/vendor/dask/utils.py` & `cubed-0.6.3/cubed/vendor/dask/utils.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/vendor/rechunker/algorithm.py` & `cubed-0.6.3/cubed/vendor/rechunker/algorithm.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/vendor/rechunker/api.py` & `cubed-0.6.3/cubed/vendor/rechunker/api.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/vendor/rechunker/executors/python.py` & `cubed-0.6.3/cubed/vendor/rechunker/executors/python.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed/vendor/rechunker/types.py` & `cubed-0.6.3/cubed/vendor/rechunker/types.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/cubed.egg-info/PKG-INFO` & `cubed-0.6.3/cubed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubed
-Version: 0.6.2
+Version: 0.6.3
 Summary: Bounded-memory serverless distributed N-dimensional array processing
 Author-email: Tom White <tom.e.white@gmail.com>
 License: Apache License 2.0
 Project-URL: homepage, https://github.com/tomwhite/cubed
 Project-URL: documentation, https://tomwhite.github.io/cubed
 Project-URL: repository, https://github.com/tomwhite/cubed
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cubed-0.6.2/cubed.egg-info/SOURCES.txt` & `cubed-0.6.3/cubed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubed-0.6.2/pyproject.toml` & `cubed-0.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cubed"
-version = "0.6.2"
+version = "0.6.3"
 authors = [
     {name = "Tom White", email = "tom.e.white@gmail.com"},
 ]
 license = {text = "Apache License 2.0"}
 description = "Bounded-memory serverless distributed N-dimensional array processing"
 readme = {file = "README.md", content-type = "text/markdown"}
 classifiers = [
```

### Comparing `cubed-0.6.2/setup.cfg` & `cubed-0.6.3/setup.cfg`

 * *Files identical despite different names*

