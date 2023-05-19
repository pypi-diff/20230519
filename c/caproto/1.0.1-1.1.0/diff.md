# Comparing `tmp/caproto-1.0.1.tar.gz` & `tmp/caproto-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caproto-1.0.1.tar", last modified: Wed Mar 29 16:31:24 2023, max compression
+gzip compressed data, was "caproto-1.1.0.tar", last modified: Fri May 19 21:30:02 2023, max compression
```

## Comparing `caproto-1.0.1.tar` & `caproto-1.1.0.tar`

### file list

```diff
@@ -1,272 +1,238 @@
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.816605 caproto-1.0.1/
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.588703 caproto-1.0.1/.ci/
--rw-r--r--   0 klauer   (1318172782) 1704612529      395 2022-09-02 15:59:08.000000 caproto-1.0.1/.ci/azure_env.sh
--rwxr-xr-x   0 klauer   (1318172782) 1704612529      235 2022-09-02 15:59:08.000000 caproto-1.0.1/.ci/install.sh
--rw-r--r--   0 klauer   (1318172782) 1704612529      177 2022-09-02 15:59:08.000000 caproto-1.0.1/.codecov.yml
--rw-r--r--   0 klauer   (1318172782) 1704612529      140 2022-09-02 15:59:08.000000 caproto-1.0.1/.coveragerc
--rw-r--r--   0 klauer   (1318172782) 1704612529       97 2022-09-02 15:59:08.000000 caproto-1.0.1/.editorconfig
--rw-r--r--   0 klauer   (1318172782) 1704612529      198 2022-09-02 15:59:08.000000 caproto-1.0.1/.flake8
--rw-r--r--   0 klauer   (1318172782) 1704612529       33 2022-09-02 15:59:08.000000 caproto-1.0.1/.gitattributes
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.558461 caproto-1.0.1/.github/
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.593859 caproto-1.0.1/.github/workflows/
--rw-r--r--   0 klauer   (1318172782) 1704612529     3256 2022-09-02 15:59:08.000000 caproto-1.0.1/.github/workflows/docs.yml
--rw-r--r--   0 klauer   (1318172782) 1704612529      632 2022-09-02 15:59:08.000000 caproto-1.0.1/.github/workflows/flake8.yml
--rw-r--r--   0 klauer   (1318172782) 1704612529      680 2022-09-02 15:59:08.000000 caproto-1.0.1/.github/workflows/pypi.yml
--rw-r--r--   0 klauer   (1318172782) 1704612529     1337 2022-09-02 15:59:12.000000 caproto-1.0.1/.github/workflows/testing.yml
--rw-r--r--   0 klauer   (1318172782) 1704612529      219 2022-09-02 15:59:08.000000 caproto-1.0.1/.gitignore
--rw-r--r--   0 klauer   (1318172782) 1704612529      130 2022-09-02 15:59:12.000000 caproto-1.0.1/.gitmodules
--rw-r--r--   0 klauer   (1318172782) 1704612529      710 2022-09-02 15:59:08.000000 caproto-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 klauer   (1318172782) 1704612529   185272 2022-09-02 15:59:08.000000 caproto-1.0.1/CAproto.html
--rw-r--r--   0 klauer   (1318172782) 1704612529      640 2022-09-02 15:59:08.000000 caproto-1.0.1/CONTRIBUTING.md
--rw-r--r--   0 klauer   (1318172782) 1704612529     1585 2022-09-02 15:59:08.000000 caproto-1.0.1/LICENSE
--rw-r--r--   0 klauer   (1318172782) 1704612529      508 2022-09-02 15:59:08.000000 caproto-1.0.1/MANIFEST.in
--rw-r--r--   0 klauer   (1318172782) 1704612529      802 2023-03-29 16:31:24.817592 caproto-1.0.1/PKG-INFO
--rw-r--r--   0 klauer   (1318172782) 1704612529      395 2022-09-02 15:59:08.000000 caproto-1.0.1/README.md
--rw-r--r--   0 klauer   (1318172782) 1704612529     3075 2022-09-02 15:59:12.000000 caproto-1.0.1/azure-pipelines.yml
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.824984 caproto-1.0.1/caproto/
--rw-r--r--   0 klauer   (1318172782) 1704612529      531 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     4220 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/_array_backend.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    12723 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/_backend.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     6707 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/_broadcaster.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    41986 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/_circuit.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    53877 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/_commands.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      892 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/_constants.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    68007 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/_data.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    35471 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/_dbr.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    25232 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/_headers.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    14945 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/_log.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2599 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/_numpy_backend.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    13280 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/_state.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    12567 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/_status.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    32847 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/_utils.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      471 2023-03-29 16:31:24.825584 caproto-1.0.1/caproto/_version.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      358 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/_windows_compat.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.610678 caproto-1.0.1/caproto/asyncio/
--rw-r--r--   0 klauer   (1318172782) 1704612529       37 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/asyncio/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    85609 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/asyncio/client.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    11204 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/asyncio/server.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     7852 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/asyncio/utils.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.613206 caproto-1.0.1/caproto/benchmarking/
--rw-r--r--   0 klauer   (1318172782) 1704612529       28 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/benchmarking/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    12580 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/benchmarking/util.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.617350 caproto-1.0.1/caproto/client/
--rw-r--r--   0 klauer   (1318172782) 1704612529       90 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/client/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     3306 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/client/common.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    12349 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/client/search_results.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.622035 caproto-1.0.1/caproto/commandline/
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/commandline/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     9733 2023-03-29 16:29:43.000000 caproto-1.0.1/caproto/commandline/cli_print_formats.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    12657 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/commandline/get.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     9873 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/commandline/monitor.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     7498 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/commandline/put.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2359 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/commandline/repeater.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2059 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/commandline/shark.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.626016 caproto-1.0.1/caproto/curio/
--rw-r--r--   0 klauer   (1318172782) 1704612529       29 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/curio/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    10101 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/curio/server.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      813 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/curio/utils.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.628317 caproto-1.0.1/caproto/docs/
--rw-r--r--   0 klauer   (1318172782) 1704612529      773 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/docs/__init__.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.629312 caproto-1.0.1/caproto/docs/templates/
--rw-r--r--   0 klauer   (1318172782) 1704612529       88 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/docs/templates/__init__.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.632722 caproto-1.0.1/caproto/docs/templates/autosummary/
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/docs/templates/autosummary/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      106 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/docs/templates/autosummary/base.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529     5375 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/docs/templates/autosummary/class.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529     1071 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/docs/templates/autosummary/module.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529     7563 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/docs/utils.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.636104 caproto-1.0.1/caproto/examples/
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/examples/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2360 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/examples/asyncio_client_simple.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2700 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/examples/benchmark_connections.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     1554 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/examples/thread_client_simple.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2579 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/examples/trio_server_simple.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.665711 caproto-1.0.1/caproto/ioc_examples/
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/__init__.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.668785 caproto-1.0.1/caproto/ioc_examples/advanced/
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/advanced/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1348 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/advanced/raw_timestamp.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     5435 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/advanced/thread_client_monitor.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     3410 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/advanced/type_varieties.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     1039 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/autosave.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     1084 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/ioc_examples/big_image_noisy_neighbor.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     2085 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/chirp.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     2444 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/client_monitor_async.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     1253 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/custom_write.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     2705 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/decay.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     1884 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/enums.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     5536 2023-03-29 16:29:43.000000 caproto-1.0.1/caproto/ioc_examples/fake_motor_record.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     4542 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/formula_ioc.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.670726 caproto-1.0.1/caproto/ioc_examples/hardware_specific/
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/hardware_specific/__init__.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     1837 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/hardware_specific/barcode_reader.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     3319 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/hardware_specific/gamepad.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     3284 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/io_interrupt.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    12346 2023-03-29 16:29:43.000000 caproto-1.0.1/caproto/ioc_examples/lakeshore.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529      886 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/macros.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     7369 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/mini_beamline.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     1885 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/mirror.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     1038 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/no_pvproperty.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.673223 caproto-1.0.1/caproto/ioc_examples/pathological/
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/pathological/__init__.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     1085 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/pathological/defaultdict_server.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     1030 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/pathological/reading_counter.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     4059 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/ioc_examples/pathological/spoof_beamline.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     1169 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/random_walk.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     3611 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/ioc_examples/records.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     2089 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/records_subclass.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     1318 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/rpc_function.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     2191 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/scalars_and_arrays.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     1810 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/scan_rate.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     1614 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/setpoint_rbv_pair.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529      777 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/simple.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     3313 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/ioc_examples/simple_with_type_hints.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     1155 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/skip_write.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     1292 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/ioc_examples/startup_and_shutdown_hooks.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     1599 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/states.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     1868 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/subgroups.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     2320 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/thermo_sim.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.678709 caproto-1.0.1/caproto/ioc_examples/too_clever/
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/too_clever/__init__.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529    14680 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/too_clever/areadetector_image.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     3508 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/too_clever/caproto_to_ophyd.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     1199 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/too_clever/caproto_to_typhos.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     3167 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/too_clever/dynamic_calc.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     1833 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/too_clever/dynamic_pvgroups.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     6384 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/too_clever/shared_memory.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     3194 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/too_clever/trigger_with_pc.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     2358 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/worker_thread.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     1748 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/ioc_examples/worker_thread_pc.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.689605 caproto-1.0.1/caproto/server/
--rw-r--r--   0 klauer   (1318172782) 1704612529     1766 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/server/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    11135 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/server/autosave.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    49908 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/server/common.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    25709 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/server/conversion.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    20732 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/server/menus.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.697459 caproto-1.0.1/caproto/server/records/
--rw-r--r--   0 klauer   (1318172782) 1704612529      534 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/server/records/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529   216379 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/server/records/base.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2267 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/server/records/menus.jinja2
--rw-r--r--   0 klauer   (1318172782) 1704612529     4478 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/server/records/mixins.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      881 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/server/records/record_body.jinja2
--rw-r--r--   0 klauer   (1318172782) 1704612529     1844 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/server/records/records.jinja2
--rw-r--r--   0 klauer   (1318172782) 1704612529    14554 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/server/records/records.py
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/server/records/registry.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     3970 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/server/records/utils.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    75851 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/server/server.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    16638 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/server/stats.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     3742 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/server/typing.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.700776 caproto-1.0.1/caproto/sync/
--rw-r--r--   0 klauer   (1318172782) 1704612529       64 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/sync/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    34503 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/sync/client.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     9377 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/sync/repeater.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     9830 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/sync/shark.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.749810 caproto-1.0.1/caproto/tests/
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    29092 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/tests/conftest.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.751800 caproto-1.0.1/caproto/tests/data/
--rw-r--r--   0 klauer   (1318172782) 1704612529     4426 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/data/example_tcp_data.pcap
--rw-r--r--   0 klauer   (1318172782) 1704612529      840 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/data/example_udp_data.pcap
--rw-r--r--   0 klauer   (1318172782) 1704612529     6488 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/dbd.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1560 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/debug.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     7521 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/epics_test_utils.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1749 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/example_runner.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     3040 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/ioc_all_in_one.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1799 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/ioc_any_record.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529      998 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/ioc_inline_style.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     1153 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/ioc_process.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     5612 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/tests/test_catvs.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     5431 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/tests/test_channel_filters.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    10626 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/test_cli_scripts.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    14951 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/test_core.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    16254 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/test_data_conversion.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     5971 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/tests/test_data_copy.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    13060 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/test_dbr_types.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2350 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/test_doc_utils.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     8646 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/tests/test_examples.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      372 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/test_fixtures.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     3538 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/test_logging.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1843 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/test_macros.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     8009 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/test_nonet.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    34635 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/test_pyepics_compat.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1690 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/test_pyepics_compat2.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     4074 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/test_record_compliance.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2671 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/tests/test_records.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      865 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/test_repeater.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    12660 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/test_serialization.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    14304 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/tests/test_server.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      639 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/test_shark.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     4374 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/test_status.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    24341 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/test_threading_client.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1257 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/test_timestamp.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     7988 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/tests/test_utils.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      504 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/verify_with_catvs.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2235 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/tests/view_leaks.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.755346 caproto-1.0.1/caproto/threading/
--rw-r--r--   0 klauer   (1318172782) 1704612529       41 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/threading/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529   101862 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/threading/client.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    39380 2023-03-29 16:29:43.000000 caproto-1.0.1/caproto/threading/pyepics_compat.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.759744 caproto-1.0.1/caproto/trio/
--rw-r--r--   0 klauer   (1318172782) 1704612529       29 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/trio/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    14021 2022-09-02 15:59:12.000000 caproto-1.0.1/caproto/trio/server.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      508 2022-09-02 15:59:08.000000 caproto-1.0.1/caproto/trio/util.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.607292 caproto-1.0.1/caproto.egg-info/
--rw-r--r--   0 klauer   (1318172782) 1704612529      802 2023-03-29 16:31:24.000000 caproto-1.0.1/caproto.egg-info/PKG-INFO
--rw-r--r--   0 klauer   (1318172782) 1704612529     7177 2023-03-29 16:31:24.000000 caproto-1.0.1/caproto.egg-info/SOURCES.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529        1 2023-03-29 16:31:24.000000 caproto-1.0.1/caproto.egg-info/dependency_links.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529      422 2023-03-29 16:31:24.000000 caproto-1.0.1/caproto.egg-info/entry_points.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529      314 2023-03-29 16:31:24.000000 caproto-1.0.1/caproto.egg-info/requires.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529        8 2023-03-29 16:31:24.000000 caproto-1.0.1/caproto.egg-info/top_level.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529      228 2022-09-02 15:59:08.000000 caproto-1.0.1/codecov.yml
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.769606 caproto-1.0.1/doc/
--rw-r--r--   0 klauer   (1318172782) 1704612529     7644 2022-09-02 15:59:12.000000 caproto-1.0.1/doc/Makefile
--rw-r--r--   0 klauer   (1318172782) 1704612529     1915 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/gen_graphs.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     4409 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/github_deploy_key.enc
--rw-r--r--   0 klauer   (1318172782) 1704612529     7743 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/make.bat
--rw-r--r--   0 klauer   (1318172782) 1704612529      973 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/rebuild.sh
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.811537 caproto-1.0.1/doc/source/
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.813629 caproto-1.0.1/doc/source/_static/
--rw-r--r--   0 klauer   (1318172782) 1704612529       65 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/source/_static/inheritance.css
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/source/_static/placeholder
--rw-r--r--   0 klauer   (1318172782) 1704612529    11905 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/source/api.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529    12564 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/source/async-clients.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529    16501 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/source/basics.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529     1210 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/source/clients.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529    24270 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/source/command-line-client.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529    10304 2022-09-02 15:59:12.000000 caproto-1.0.1/doc/source/conf.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2006 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/source/containers.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529     5138 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/source/cookiecutter.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529     2029 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/source/environment_variables.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529      184 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/source/example_autosummary.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529     2986 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/source/example_conf.py
--rw-r--r--   0 klauer   (1318172782) 1704612529       73 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/source/example_requirements-docs.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529     6780 2022-09-02 15:59:12.000000 caproto-1.0.1/doc/source/index.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529     3275 2022-09-02 15:59:12.000000 caproto-1.0.1/doc/source/install.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529    48617 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/source/iocs.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529    10159 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/source/loggers.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529     1286 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/source/own_docs.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529     2898 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/source/protocol-compliance.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529     3821 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/source/pyepics-compat-client.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529     2944 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/source/records.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529     1625 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/source/references.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529    36688 2023-03-29 16:29:43.000000 caproto-1.0.1/doc/source/release-notes.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529     7097 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/source/server_api.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529     3010 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/source/servers.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529     7765 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/source/shark.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529     8381 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/source/sync-client.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529    12872 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/source/threading-client.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529      514 2022-09-02 15:59:08.000000 caproto-1.0.1/doc/spec-issues.md
--rw-r--r--   0 klauer   (1318172782) 1704612529     5914 2022-09-02 15:59:08.000000 caproto-1.0.1/generate_headers.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     3324 2022-09-02 15:59:08.000000 caproto-1.0.1/headers.tpl
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-03-29 16:31:24.815430 caproto-1.0.1/other_licenses/
--rw-r--r--   0 klauer   (1318172782) 1704612529     4070 2022-09-02 15:59:08.000000 caproto-1.0.1/other_licenses/pyepics
--rw-r--r--   0 klauer   (1318172782) 1704612529    11358 2022-09-02 15:59:08.000000 caproto-1.0.1/other_licenses/tornado
--rw-r--r--   0 klauer   (1318172782) 1704612529       37 2022-09-02 15:59:08.000000 caproto-1.0.1/pytest.ini
--rw-r--r--   0 klauer   (1318172782) 1704612529      114 2022-09-02 15:59:12.000000 caproto-1.0.1/requirements-doc.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529      219 2022-09-02 15:59:08.000000 caproto-1.0.1/requirements-test.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529      115 2022-09-02 15:59:08.000000 caproto-1.0.1/run_tests.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      173 2023-03-29 16:31:24.822958 caproto-1.0.1/setup.cfg
--rw-r--r--   0 klauer   (1318172782) 1704612529     2967 2022-09-02 15:59:12.000000 caproto-1.0.1/setup.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     1260 2022-09-02 15:59:08.000000 caproto-1.0.1/setup_development_network.sh
--rw-r--r--   0 klauer   (1318172782) 1704612529      176 2022-09-02 15:59:08.000000 caproto-1.0.1/setup_local_dev_env.sh
--rw-r--r--   0 klauer   (1318172782) 1704612529    62436 2022-09-02 15:59:08.000000 caproto-1.0.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.573238 caproto-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-19 21:29:51.000000 caproto-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-19 21:29:51.000000 caproto-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-19 21:29:51.000000 caproto-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-19 21:30:02.573238 caproto-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-19 21:29:51.000000 caproto-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.573238 caproto-1.1.0/caproto/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/_array_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/_broadcaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41986 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53877 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68459 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35471 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/_dbr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25232 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14945 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13280 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34930 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-19 21:30:02.573238 caproto-1.1.0/caproto/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/_windows_compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.557238 caproto-1.1.0/caproto/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85609 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/asyncio/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/asyncio/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/asyncio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.561238 caproto-1.1.0/caproto/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12580 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/benchmarking/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.561238 caproto-1.1.0/caproto/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/client/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12349 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/client/search_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.561238 caproto-1.1.0/caproto/commandline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/commandline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/commandline/cli_print_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/commandline/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/commandline/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/commandline/put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/commandline/repeater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/commandline/shark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.561238 caproto-1.1.0/caproto/curio/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/curio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/curio/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/curio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.561238 caproto-1.1.0/caproto/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.561238 caproto-1.1.0/caproto/docs/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/docs/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.561238 caproto-1.1.0/caproto/docs/templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/docs/templates/autosummary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/docs/templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/docs/templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/docs/templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/docs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.561238 caproto-1.1.0/caproto/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/examples/asyncio_client_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/examples/benchmark_connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1554 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/examples/thread_client_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/examples/trio_server_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.565238 caproto-1.1.0/caproto/ioc_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.565238 caproto-1.1.0/caproto/ioc_examples/advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/advanced/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/advanced/raw_timestamp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5435 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/advanced/thread_client_monitor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3410 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/advanced/type_varieties.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1039 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/autosave.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1084 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/big_image_noisy_neighbor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2085 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/chirp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2444 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/client_monitor_async.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1253 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/custom_write.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2705 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/decay.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1884 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/enums.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5575 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/fake_motor_record.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4542 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/formula_ioc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.565238 caproto-1.1.0/caproto/ioc_examples/hardware_specific/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/hardware_specific/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1837 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/hardware_specific/barcode_reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3319 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/hardware_specific/gamepad.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3284 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/io_interrupt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/lakeshore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      886 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/macros.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7369 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/mini_beamline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1885 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/mirror.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1038 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/no_pvproperty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.565238 caproto-1.1.0/caproto/ioc_examples/pathological/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/pathological/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1085 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/pathological/defaultdict_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1030 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/pathological/reading_counter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4059 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/pathological/spoof_beamline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1169 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/random_walk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3611 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/records.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2089 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/records_subclass.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1318 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/rpc_function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2191 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/scalars_and_arrays.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1810 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/scan_rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1614 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/setpoint_rbv_pair.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      777 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/simple.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3313 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/simple_with_type_hints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1155 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/skip_write.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1292 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/startup_and_shutdown_hooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1599 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/states.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1868 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/subgroups.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2320 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/thermo_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.565238 caproto-1.1.0/caproto/ioc_examples/too_clever/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/too_clever/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14680 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/too_clever/areadetector_image.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3508 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/too_clever/caproto_to_ophyd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1199 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/too_clever/caproto_to_typhos.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3167 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/too_clever/dynamic_calc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1833 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/too_clever/dynamic_pvgroups.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6384 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/too_clever/shared_memory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3194 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/too_clever/trigger_with_pc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2358 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/worker_thread.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1748 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/ioc_examples/worker_thread_pc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.565238 caproto-1.1.0/caproto/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11135 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/server/autosave.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52337 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/server/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25709 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/server/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20732 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/server/menus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.565238 caproto-1.1.0/caproto/server/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/server/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   216379 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/server/records/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/server/records/menus.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/server/records/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/server/records/record_body.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/server/records/records.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/server/records/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/server/records/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/server/records/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77613 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16638 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/server/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/server/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.569238 caproto-1.1.0/caproto/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34503 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/sync/client.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9377 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/sync/repeater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9830 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/sync/shark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.569238 caproto-1.1.0/caproto/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29092 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/dbd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/epics_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/example_runner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3040 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/ioc_all_in_one.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/ioc_any_record.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      998 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/ioc_inline_style.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1153 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/ioc_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/issue_797_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_catvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_channel_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10626 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_cli_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14951 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16254 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_data_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_data_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13060 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_dbr_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_doc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_events_off.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_nonet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34635 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_pyepics_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_pyepics_compat2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_record_compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_repeater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14304 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_shark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24341 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_threading_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/verify_with_catvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/tests/view_leaks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.569238 caproto-1.1.0/caproto/threading/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/threading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101862 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/threading/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39380 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/threading/pyepics_compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.573238 caproto-1.1.0/caproto/trio/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/trio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14016 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/trio/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-19 21:29:51.000000 caproto-1.1.0/caproto/trio/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.557238 caproto-1.1.0/caproto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-19 21:30:02.000000 caproto-1.1.0/caproto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-05-19 21:30:02.000000 caproto-1.1.0/caproto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 21:30:02.000000 caproto-1.1.0/caproto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-19 21:30:02.000000 caproto-1.1.0/caproto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-19 21:30:02.000000 caproto-1.1.0/caproto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-19 21:30:02.000000 caproto-1.1.0/caproto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.573238 caproto-1.1.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/gen_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.573238 caproto-1.1.0/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:02.573238 caproto-1.1.0/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/_static/inheritance.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11905 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12564 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/async-clients.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16501 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/clients.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    24270 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/command-line-client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10302 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/containers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/cookiecutter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/environment_variables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/example_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    49995 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/iocs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/loggers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/own_docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/protocol-compliance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/pyepics-compat-client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/records.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/references.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    36905 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/server_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/servers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/shark.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/sync-client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12872 2023-05-19 21:29:51.000000 caproto-1.1.0/doc/source/threading-client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-05-19 21:29:51.000000 caproto-1.1.0/generate_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-19 21:29:51.000000 caproto-1.1.0/headers.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-19 21:29:51.000000 caproto-1.1.0/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-19 21:29:51.000000 caproto-1.1.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-19 21:30:02.573238 caproto-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-19 21:29:51.000000 caproto-1.1.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62436 2023-05-19 21:29:51.000000 caproto-1.1.0/versioneer.py
```

### Comparing `caproto-1.0.1/CONTRIBUTING.md` & `caproto-1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/LICENSE` & `caproto-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/__init__.py` & `caproto-1.1.0/caproto/__init__.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/_array_backend.py` & `caproto-1.1.0/caproto/_array_backend.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/_backend.py` & `caproto-1.1.0/caproto/_backend.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/_broadcaster.py` & `caproto-1.1.0/caproto/_broadcaster.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/_circuit.py` & `caproto-1.1.0/caproto/_circuit.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/_commands.py` & `caproto-1.1.0/caproto/_commands.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/_data.py` & `caproto-1.1.0/caproto/_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # These classes ChannelData classes hold the state associated with the data
 # source underlying a Channel, including data values, alarm state, and
 # metadata. They perform data type conversions in response to requests to read
 # data as a certain type, and they push updates into queues registered by a
 # higher-level server.
 import copy
+import logging
 import time
 import weakref
 from collections import defaultdict, namedtuple
 from collections.abc import Iterable
 from typing import Any
 
+from . import _constants as constants
 from ._backend import backend
 from ._commands import parse_metadata
 from ._constants import MAX_ENUM_STATES, MAX_ENUM_STRING_SIZE
 from ._dbr import (DBR_STSACK_STRING, DBR_TYPES, AccessRights, AlarmSeverity,
                    AlarmStatus, ChannelType, GraphicControlBase,
                    SubscriptionType, TimeStamp, _channel_type_by_name,
                    _LongStringChannelType, native_type, native_types,
@@ -32,14 +34,16 @@
            'ChannelInteger',
            'ChannelNumeric',
            'ChannelShort',
            'ChannelString',
            'SkipWrite',
            )
 
+logger = logging.getLogger(__name__)
+
 SubscriptionUpdate = namedtuple('SubscriptionUpdate',
                                 ('sub_specs', 'metadata', 'values',
                                  'flags', 'sub'))
 
 
 class Forbidden(CaprotoError):
     ...
@@ -266,18 +270,27 @@
         Though this is not a record, the channel access protocol supports
         querying the record type.  This can be set to mimic an actual
         record or be set to something arbitrary.  Defaults to 'caproto'.
     """
     data_type = ChannelType.LONG
     default_value: Any = 0
     _compatible_array_types = {}
+    max_subscription_backlog: int
 
-    def __init__(self, *, alarm=None, value=None, timestamp=None,
-                 max_length=None, string_encoding='latin-1',
-                 reported_record_type='caproto'):
+    def __init__(
+        self,
+        *,
+        alarm=None,
+        value=None,
+        timestamp=None,
+        max_length=None,
+        string_encoding="latin-1",
+        reported_record_type="caproto",
+        max_subscription_backlog: int = constants.MAX_SUBSCRIPTION_BACKLOG,
+    ):
         if timestamp is None:
             timestamp = time.time()
         if alarm is None:
             alarm = ChannelAlarm()
 
         self._alarm = None
         self._status = None
@@ -314,14 +327,15 @@
                 lambda: defaultdict(set)))
 
         # Cache results of data_type conversions. This maps data_type to
         # (metdata, value). This is cleared each time publish() is called.
         self._content = {}
         self._snapshots = defaultdict(dict)
         self._fill_at_next_write = list()
+        self.max_subscription_backlog = max_subscription_backlog
 
     def __getstate__(self):
         state = dict(self.__dict__)
         state.pop("_queues", None)
         state.pop("_snapshots", None)
         return state
 
@@ -1664,21 +1678,35 @@
     units : str, optional
         Engineering units indicator, which can be retrieved over channel
         access.
     """
     data_type = ChannelType.CHAR
     _compatible_array_types = {'|u1', '|i1', '|b1'}
 
-    def __init__(self, *, alarm=None, value=None, timestamp=None,
-                 max_length=None, string_encoding='latin-1',
-                 reported_record_type='caproto', report_as_string=False):
-        super().__init__(alarm=alarm, value=value, timestamp=timestamp,
-                         max_length=max_length,
-                         string_encoding=string_encoding,
-                         reported_record_type=reported_record_type)
+    def __init__(
+        self,
+        *,
+        alarm=None,
+        value=None,
+        timestamp=None,
+        max_length=None,
+        string_encoding="latin-1",
+        reported_record_type="caproto",
+        report_as_string=False,
+        **kwargs
+    ):
+        super().__init__(
+            alarm=alarm,
+            value=value,
+            timestamp=timestamp,
+            max_length=max_length,
+            string_encoding=string_encoding,
+            reported_record_type=reported_record_type,
+            **kwargs,
+        )
 
         if report_as_string:
             self.data_type = ChannelType.STRING
 
     @property
     def long_string_max_length(self):
         'The maximum number of elements (length) of the current value'
@@ -1758,19 +1786,25 @@
         querying the record type.  This can be set to mimic an actual
         record or be set to something arbitrary.  Defaults to 'caproto'.
     """
     data_type = ChannelType.STRING
 
     def __init__(self, *, alarm=None, value=None, timestamp=None,
                  max_length=None, string_encoding='latin-1',
-                 reported_record_type='caproto', long_string_max_length=81):
-        super().__init__(alarm=alarm, value=value, timestamp=timestamp,
-                         max_length=max_length,
-                         string_encoding=string_encoding,
-                         reported_record_type=reported_record_type)
+                 reported_record_type='caproto', long_string_max_length=81,
+                 **kwargs):
+        super().__init__(
+            alarm=alarm,
+            value=value,
+            timestamp=timestamp,
+            max_length=max_length,
+            string_encoding=string_encoding,
+            reported_record_type=reported_record_type,
+            **kwargs,
+        )
 
         self._long_string_max_length = long_string_max_length
 
     @property
     def long_string_max_length(self):
         'The maximum number of elements (length) of the current value'
         return self._long_string_max_length
```

### Comparing `caproto-1.0.1/caproto/_dbr.py` & `caproto-1.1.0/caproto/_dbr.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/_headers.py` & `caproto-1.1.0/caproto/_headers.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/_log.py` & `caproto-1.1.0/caproto/_log.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/_numpy_backend.py` & `caproto-1.1.0/caproto/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/_state.py` & `caproto-1.1.0/caproto/_state.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/_status.py` & `caproto-1.1.0/caproto/_status.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/_utils.py` & `caproto-1.1.0/caproto/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # This module includes all exceptions raised by caproto, sentinel objects used
 # throughout the package (see detailed comment below), various network-related
 # helper functions, and other miscellaneous utilities.
+from __future__ import annotations
+
 import argparse
 import array
 import collections
+import copy
 import enum
 import functools
 import inspect
 import ipaddress
 import json
 import logging
 import os
@@ -16,18 +19,24 @@
 import struct
 import sys
 import threading
 import typing
 import weakref
 from collections import namedtuple
 from contextlib import contextmanager
+from typing import Iterable
 from warnings import warn
 
+from ._dbr import SubscriptionType
 from ._version import get_versions
 
+if typing.TYPE_CHECKING:
+    from .server.common import Subscription
+
+
 __version__ = get_versions()['version']
 
 try:
     import fcntl
     import termios
 except ImportError:
     fcntl = None
@@ -849,14 +858,71 @@
         if stop == -1:
             stop = None
         else:
             stop += 1
     return values[start:stop:step]
 
 
+def apply_deadband_filter(
+    previous_value,
+    new_value,
+    sub: Subscription,
+    flags: int,
+    host_endian: str,
+):
+    """
+    Apply the Subscription-specified deadband filter.
+
+    Requires caller to track state between subscription updates.
+    If outside of the deadband range, this will return the value to be
+    tracked.
+    """
+    if hasattr(new_value, "endian"):
+        if new_value.endian != host_endian:
+            new_value = copy.copy(new_value)
+            new_value.byteswap()
+
+    if previous_value is None:
+        # First entry:
+        return new_value
+
+    old_iterable = isinstance(previous_value, Iterable)
+    new_iterable = isinstance(new_value, Iterable)
+    if (not old_iterable or (old_iterable and len(previous_value) == 1)) and (
+        not new_iterable or (new_iterable and len(new_value) == 1)
+    ):
+        if old_iterable:
+            (previous_value,) = previous_value
+        if new_iterable:
+            (new_value,) = new_value
+
+        # Cool that was fun. (git blame may say klauer but you must dig deeper
+        # to find the truth)
+        if sub.channel_filter.dbnd.m == "rel":
+            out_of_band = sub.channel_filter.dbnd.d < abs(
+                (previous_value - new_value) / previous_value
+            )
+        else:  # must be 'abs' -- was already validated
+            out_of_band = sub.channel_filter.dbnd.d < abs(previous_value - new_value)
+        # We have verified that that EPICS considers DBE_LOG
+        # etc. to be an absolute (not relative) threshold.
+        abs_diff = abs(previous_value - new_value)
+        if abs_diff > sub.db_entry.log_atol:
+            flags |= SubscriptionType.DBE_LOG
+            if abs_diff > sub.db_entry.value_atol:
+                flags |= SubscriptionType.DBE_VALUE
+
+        if not (out_of_band and (sub.mask & flags)):
+            return None
+
+        return new_value
+
+    return None
+
+
 def batch_requests(request_iter, max_length):
     '''Batch a set of items with length, thresholded on sum of item length
 
     Yields
     ------
     batch : collections.deque
         Batch of items from request_iter, where:
```

### Comparing `caproto-1.0.1/caproto/asyncio/client.py` & `caproto-1.1.0/caproto/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/asyncio/server.py` & `caproto-1.1.0/caproto/asyncio/server.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/asyncio/utils.py` & `caproto-1.1.0/caproto/asyncio/utils.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/benchmarking/util.py` & `caproto-1.1.0/caproto/benchmarking/util.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/client/common.py` & `caproto-1.1.0/caproto/client/common.py`

 * *Files 23% similar despite different names*

```diff
@@ -24,22 +24,36 @@
 # sentinels used as default values for arguments
 GLOBAL_DEFAULT_TIMEOUT = float(os.environ.get("CAPROTO_DEFAULT_TIMEOUT", 2.))
 
 CONTEXT_DEFAULT_TIMEOUT = _sentinel('CONTEXT_DEFAULT_TIMEOUT')
 PV_DEFAULT_TIMEOUT = _sentinel('PV_DEFAULT_TIMEOUT')
 VALID_CHANNEL_MARKER = _sentinel('VALID_CHANNEL_MARKER')
 
-AUTOMONITOR_MAXLENGTH = 65536
-BEACON_MARGIN = 1
-EVENT_ADD_BATCH_MAX_BYTES = 2**16
-MAX_RETRY_SEARCHES_INTERVAL = 5
-MIN_RETRY_SEARCHES_INTERVAL = 0.03
-RESTART_SUBS_PERIOD = 0.1
-RETRY_RETIRED_SEARCHES_INTERVAL = 60
-SEARCH_RETIREMENT_AGE = 8 * 60
+AUTOMONITOR_MAXLENGTH = int(
+    os.environ.get("CAPROTO_CLIENT_AUTOMONITOR_MAXLENGTH", 65536)
+)
+BEACON_MARGIN = float(os.environ.get("CAPROTO_CLIENT_BEACON_MARGIN_SEC", 1))
+EVENT_ADD_BATCH_MAX_BYTES = int(
+    os.environ.get("CAPROTO_CLIENT_EVENT_ADD_BATCH_MAX_BYTES", 2 ** 16)
+)
+MAX_RETRY_SEARCHES_INTERVAL = float(
+    os.environ.get("CAPROTO_CLIENT_MAX_RETRY_SEARCHES_INTERVAL_SEC", 5)
+)
+MIN_RETRY_SEARCHES_INTERVAL = float(
+    os.environ.get("CAPROTO_CLIENT_MIN_RETRY_SEARCHES_INTERVAL_SEC", 0.03)
+)
+RESTART_SUBS_PERIOD = float(
+    os.environ.get("CAPROTO_CLIENT_RESTART_SUBS_PERIOD_SEC", 0.1)
+)
+RETRY_RETIRED_SEARCHES_INTERVAL = float(
+    os.environ.get("CAPROTO_CLIENT_RETRY_RETIRED_SEARCHES_INTERVAL_SEC", 60.)
+)
+SEARCH_RETIREMENT_AGE = int(
+    os.environ.get("CAPROTO_CLIENT_SEARCH_RETIREMENT_AGE_SEC", 8 * 60)
+)
 STR_ENC = os.environ.get('CAPROTO_STRING_ENCODING', 'latin-1')
 
 
 # class VirtualCircuit:
 #     "Wraps a caproto.VirtualCircuit and adds transport."
 #     def __init__(self, circuit):
 #         self.circuit = circuit  # a caproto.VirtualCircuit
```

### Comparing `caproto-1.0.1/caproto/client/search_results.py` & `caproto-1.1.0/caproto/client/search_results.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/commandline/cli_print_formats.py` & `caproto-1.1.0/caproto/commandline/cli_print_formats.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/commandline/get.py` & `caproto-1.1.0/caproto/commandline/get.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/commandline/monitor.py` & `caproto-1.1.0/caproto/commandline/monitor.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/commandline/put.py` & `caproto-1.1.0/caproto/commandline/put.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/commandline/repeater.py` & `caproto-1.1.0/caproto/commandline/repeater.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/commandline/shark.py` & `caproto-1.1.0/caproto/commandline/shark.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/curio/server.py` & `caproto-1.1.0/caproto/curio/server.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/curio/utils.py` & `caproto-1.1.0/caproto/curio/utils.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/docs/__init__.py` & `caproto-1.1.0/caproto/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/docs/templates/autosummary/class.rst` & `caproto-1.1.0/caproto/docs/templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/docs/templates/autosummary/module.rst` & `caproto-1.1.0/caproto/docs/templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/docs/utils.py` & `caproto-1.1.0/caproto/docs/utils.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/examples/asyncio_client_simple.py` & `caproto-1.1.0/caproto/examples/asyncio_client_simple.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/examples/benchmark_connections.py` & `caproto-1.1.0/caproto/examples/benchmark_connections.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/examples/thread_client_simple.py` & `caproto-1.1.0/caproto/examples/thread_client_simple.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/examples/trio_server_simple.py` & `caproto-1.1.0/caproto/examples/trio_server_simple.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/advanced/raw_timestamp.py` & `caproto-1.1.0/caproto/ioc_examples/advanced/raw_timestamp.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/advanced/thread_client_monitor.py` & `caproto-1.1.0/caproto/ioc_examples/advanced/thread_client_monitor.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/advanced/type_varieties.py` & `caproto-1.1.0/caproto/ioc_examples/advanced/type_varieties.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/autosave.py` & `caproto-1.1.0/caproto/ioc_examples/autosave.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/big_image_noisy_neighbor.py` & `caproto-1.1.0/caproto/ioc_examples/big_image_noisy_neighbor.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/chirp.py` & `caproto-1.1.0/caproto/ioc_examples/chirp.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/client_monitor_async.py` & `caproto-1.1.0/caproto/ioc_examples/client_monitor_async.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/custom_write.py` & `caproto-1.1.0/caproto/ioc_examples/custom_write.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/decay.py` & `caproto-1.1.0/caproto/ioc_examples/decay.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/enums.py` & `caproto-1.1.0/caproto/ioc_examples/enums.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/fake_motor_record.py` & `caproto-1.1.0/caproto/ioc_examples/fake_motor_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 from textwrap import dedent
 
 from caproto.server import PVGroup, SubGroup, ioc_arg_parser, pvproperty, run
+from caproto.server.records import MotorFields
 
 
 async def broadcast_precision_to_fields(record):
     """Update precision of all fields to that of the given record."""
 
     precision = record.precision
     for field, prop in record.field_inst.pvdb.items():
@@ -37,15 +38,15 @@
             precision=3,
             acceleration=1.0,
             resolution=1e-6,
             tick_rate_hz=10.,
             user_limits=(0.0, 100.0),
         )
 
-    fields = instance.field_inst  # type: MotorFields
+    fields: MotorFields = instance.field_inst
     have_new_position = False
 
     async def value_write_hook(fields, value):
         nonlocal have_new_position
         # This happens when a user puts to `motor.VAL`
         # print("New position requested!", value)
         have_new_position = True
```

### Comparing `caproto-1.0.1/caproto/ioc_examples/formula_ioc.py` & `caproto-1.1.0/caproto/ioc_examples/formula_ioc.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/hardware_specific/barcode_reader.py` & `caproto-1.1.0/caproto/ioc_examples/hardware_specific/barcode_reader.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/hardware_specific/gamepad.py` & `caproto-1.1.0/caproto/ioc_examples/hardware_specific/gamepad.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/io_interrupt.py` & `caproto-1.1.0/caproto/ioc_examples/io_interrupt.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/lakeshore.py` & `caproto-1.1.0/caproto/ioc_examples/lakeshore.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/macros.py` & `caproto-1.1.0/caproto/ioc_examples/macros.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/mini_beamline.py` & `caproto-1.1.0/caproto/ioc_examples/mini_beamline.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/mirror.py` & `caproto-1.1.0/caproto/ioc_examples/mirror.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/no_pvproperty.py` & `caproto-1.1.0/caproto/ioc_examples/no_pvproperty.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/pathological/defaultdict_server.py` & `caproto-1.1.0/caproto/ioc_examples/pathological/defaultdict_server.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/pathological/reading_counter.py` & `caproto-1.1.0/caproto/ioc_examples/pathological/reading_counter.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/pathological/spoof_beamline.py` & `caproto-1.1.0/caproto/ioc_examples/pathological/spoof_beamline.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/random_walk.py` & `caproto-1.1.0/caproto/ioc_examples/random_walk.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/records.py` & `caproto-1.1.0/caproto/ioc_examples/records.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/records_subclass.py` & `caproto-1.1.0/caproto/ioc_examples/records_subclass.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/rpc_function.py` & `caproto-1.1.0/caproto/ioc_examples/rpc_function.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/scalars_and_arrays.py` & `caproto-1.1.0/caproto/ioc_examples/scalars_and_arrays.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/scan_rate.py` & `caproto-1.1.0/caproto/ioc_examples/scan_rate.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/setpoint_rbv_pair.py` & `caproto-1.1.0/caproto/ioc_examples/setpoint_rbv_pair.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/simple.py` & `caproto-1.1.0/caproto/ioc_examples/simple.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/simple_with_type_hints.py` & `caproto-1.1.0/caproto/ioc_examples/simple_with_type_hints.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/skip_write.py` & `caproto-1.1.0/caproto/ioc_examples/skip_write.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/startup_and_shutdown_hooks.py` & `caproto-1.1.0/caproto/ioc_examples/startup_and_shutdown_hooks.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/states.py` & `caproto-1.1.0/caproto/ioc_examples/states.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/subgroups.py` & `caproto-1.1.0/caproto/ioc_examples/subgroups.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/thermo_sim.py` & `caproto-1.1.0/caproto/ioc_examples/thermo_sim.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/too_clever/areadetector_image.py` & `caproto-1.1.0/caproto/ioc_examples/too_clever/areadetector_image.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/too_clever/caproto_to_ophyd.py` & `caproto-1.1.0/caproto/ioc_examples/too_clever/caproto_to_ophyd.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/too_clever/caproto_to_typhos.py` & `caproto-1.1.0/caproto/ioc_examples/too_clever/caproto_to_typhos.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/too_clever/dynamic_calc.py` & `caproto-1.1.0/caproto/ioc_examples/too_clever/dynamic_calc.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/too_clever/dynamic_pvgroups.py` & `caproto-1.1.0/caproto/ioc_examples/too_clever/dynamic_pvgroups.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/too_clever/shared_memory.py` & `caproto-1.1.0/caproto/ioc_examples/too_clever/shared_memory.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/too_clever/trigger_with_pc.py` & `caproto-1.1.0/caproto/ioc_examples/too_clever/trigger_with_pc.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/worker_thread.py` & `caproto-1.1.0/caproto/ioc_examples/worker_thread.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/ioc_examples/worker_thread_pc.py` & `caproto-1.1.0/caproto/ioc_examples/worker_thread_pc.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/server/__init__.py` & `caproto-1.1.0/caproto/server/__init__.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/server/autosave.py` & `caproto-1.1.0/caproto/server/autosave.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/server/common.py` & `caproto-1.1.0/caproto/server/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,61 @@
-import copy
+from __future__ import annotations
+
 import logging
+import os
 import sys
 import time
+import typing
 import weakref
 from collections import ChainMap, defaultdict, deque, namedtuple
-from collections.abc import Iterable
+from typing import DefaultDict, Deque, Tuple
 
 import caproto as ca
 from caproto import (CaprotoKeyError, CaprotoNetworkError, CaprotoRuntimeError,
                      ChannelType, RemoteProtocolError, apply_arr_filter,
                      get_environment_variables)
 
 from .._constants import MAX_UDP_RECV
-from .._dbr import SubscriptionType, _LongStringChannelType
+from .._dbr import DbrTypeBase, _LongStringChannelType
+from .._utils import apply_deadband_filter
+
+if typing.TYPE_CHECKING:
+    from .._circuit import ServerChannel, SubscriptionType
+    from .._data import ChannelData
+    from .._utils import ChannelFilter
+
 
 # ** Tuning this parameters will affect the servers' performance **
 # ** under high load. **
 # If the queue of subscriptions to has a new update ready within this timeout,
 # we consider ourselves under high load and trade accept some latency for some
 # efficiency.
-HIGH_LOAD_TIMEOUT = 0.01
+HIGH_LOAD_TIMEOUT = float(
+    os.environ.get("CAPROTO_SERVER_HIGH_LOAD_TIMEOUT_SEC", 0.01)
+)
+HIGH_LOAD_EVENT_TIME_THRESHOLD = float(
+    os.environ.get("CAPROTO_SERVER_HIGH_LOAD_EVENT_TIME_THRESHOLD_SEC", 0.1)
+)
+# Warn the user if packets are delayed by more than this amount: 30ms
+# Set to 0 to disable the warning entirely.
+HIGH_LOAD_WARN_LATENCY_SEC = float(
+    os.environ.get("CAPROTO_SERVER_HIGH_LOAD_WARN_LATENCY_SEC", 0.03)
+)
 # When a batch of subscription updates has this many bytes or more, send it.
-SUB_BATCH_THRESH = 2**16
+SUB_BATCH_THRESH = int(os.environ.get("CAPROTO_SERVER_SUB_BATCH_THRESH", 2 ** 16))
 # Tune this to change the max time between packets. If it's too high, the
 # client will experience long gaps when the server is under load. If it's too
 # low, the *overall* latency will be higher because the server will have to
 # waste time bundling many small packets.
-MAX_LATENCY = 1
+MAX_LATENCY = float(os.environ.get("CAPROTO_SERVER_MAX_LATENCY_SEC", 1.0))
 # If a Read[Notify]Request or EventAddRequest is received, wait for up to this
 # long for the currently-processing Write[Notify]Request to finish.
-WRITE_LOCK_TIMEOUT = 0.001
+WRITE_LOCK_TIMEOUT = float(
+    os.environ.get("CAPROTO_SERVER_WRITE_LOCK_TIMEOUT_SEC", 0.001)
+)
 
 
 class DisconnectedCircuit(Exception):
     ...
 
 
 class LoopExit(Exception):
@@ -64,14 +86,22 @@
     data_count : int
         The number of requested elements
     subscriptionid : int
         The ID of the subscription
     db_entry : ChannelData
         The database entry
     '''
+    mask: SubscriptionType
+    channel_filter: ChannelFilter
+    circuit: VirtualCircuit
+    channel: ServerChannel
+    data_type: ChannelType
+    data_count: int
+    subscriptionid: int
+    db_entry: ChannelData
 
 
 class SubscriptionSpec(namedtuple('SubscriptionSpec',
                                   ('db_entry', 'data_type_name', 'mask',
                                    'channel_filter'))
                        ):
     '''
@@ -88,14 +118,18 @@
         and :class:`_LongStringChannelType`.
     mask : SubscriptionType
         The subscription mask indicating different properties
     channel_filter : ChannelFilter
         The channel filter specified, including timestamp, deadband,
         array and sync options.
     '''
+    db_entry: ChannelData
+    data_type_name: str
+    mask: SubscriptionType
+    channel_filter: ChannelFilter
 
 
 host_endian = ('>' if sys.byteorder == 'big' else '<')
 
 
 class VirtualCircuit:
     circuit: ca.VirtualCircuit
@@ -108,17 +142,17 @@
         self.client = client
         self.context = context
         self.client_hostname = None
         self.client_username = None
         # The structure of self.subscriptions is:
         # {SubscriptionSpec: deque([Subscription, Subscription, ...]), ...}
         self.subscriptions = defaultdict(deque)
-        self.unexpired_updates = defaultdict(
-            lambda: deque(maxlen=ca.MAX_SUBSCRIPTION_BACKLOG))
-        self.most_recent_updates = {}
+        self.unexpired_updates = {}
+        self.subscriptions_to_resend = {}
+        self.time_events_toggled = time.monotonic()
         # This dict is passed to the loggers.
         self._tags = {'their_address': self.circuit.address,
                       'our_address': self.circuit.our_address,
                       'direction': '<<<---',
                       'role': repr(self.circuit.our_role)}
         # Subclasses are expected to define:
         # self.QueueFull = ...
@@ -307,14 +341,15 @@
     async def subscription_queue_loop(self):
         maybe_awaitable = self.events_on.set()
         # The curio backend makes this an awaitable thing.
         if maybe_awaitable is not None:
             await maybe_awaitable
         commands = deque()
         latency_limit = HIGH_LOAD_TIMEOUT
+        deadline = 0.0
         while True:
             send_now = False
             commands.clear()
             commands_bytes = 0
             num_expired = 0
             try:
                 # We are covering two regimes of operation here. In the "slow
@@ -381,21 +416,30 @@
                     # were expired.)
                     if commands and send_now:
                         break
             except self.TaskCancelled:
                 break
             try:
                 len_commands = len(commands)
-                if num_expired:
+
+                # If events are toggled by the client, subscriptions values get
+                # garbage- collected.  It's not a high load situation.  Let's
+                # warn only if we're relatively sure that it wasn't due to
+                # recent event toggling.
+                time_since_events_toggled = time.monotonic() - self.time_events_toggled
+                if num_expired and time_since_events_toggled > HIGH_LOAD_EVENT_TIME_THRESHOLD:
                     self.log.warning("High load. Dropped %d responses.", num_expired)
-                if len_commands > 1:
-                    self.log.info(
-                        "High load. Batched %d commands (%dB) with %.4fs latency.",
-                        len_commands, commands_bytes,
-                        now - deadline + latency_limit)
+
+                if len_commands > 1 and HIGH_LOAD_WARN_LATENCY_SEC > 0:
+                    latency = now - deadline + latency_limit
+                    if latency >= HIGH_LOAD_WARN_LATENCY_SEC:
+                        self.log.warning(
+                            "High load. Batched %d commands (%dB) with %.4fs latency.",
+                            len_commands, commands_bytes, latency
+                        )
 
                 # Ensure at the last possible moment that we don't send
                 # responses for Subscriptions that have been canceled at some
                 # time after the response was queued. The important thing is
                 # that no EventAddResponse be sent after the corresponding
                 # EventCancelResponse.
                 all_subscription_ids = set(sub.subscriptionid
@@ -426,15 +470,17 @@
         to_remove = []
         for sub_spec, subs in self.subscriptions.items():
             for sub in subs:
                 if func(sub):
                     to_remove.append((sub_spec, sub))
         for sub_spec, sub in to_remove:
             self.subscriptions[sub_spec].remove(sub)
-            self.most_recent_updates.pop(sub.subscriptionid, None)
+            resends = self.subscriptions_to_resend.get(sub_spec, [])
+            if sub in resends:
+                resends.remove(sub)
             self.context.subscriptions[sub_spec].remove(sub)
             self.context.last_dead_band.pop(sub, None)
             self.context.last_sync_edge_update.pop(sub, None)
             # Does anything else on the Context still care about sub_spec?
             # If not unsubscribe the Context's queue from the db_entry.
             if not self.context.subscriptions[sub_spec]:
                 queue = self.context.subscription_queue
@@ -649,35 +695,46 @@
                 data_count = removed_sub.data_count
             else:
                 data_count = db_entry.length
             to_send = [chan.unsubscribe(command.subscriptionid,
                                         data_type=command.data_type,
                                         data_count=data_count)]
         elif isinstance(command, ca.EventsOnRequest):
-            # Immediately send most recent updates for all subscriptions.
-            most_recent_updates = list(self.most_recent_updates.values())
-            self.most_recent_updates.clear()
-            if most_recent_updates:
-                await self.send(*most_recent_updates)
+            self.circuit.log.info("Client at %s:%d has turned events on.",
+                                  *self.circuit.address)
+
+            self.time_events_toggled = time.monotonic()
             maybe_awaitable = self.events_on.set()
             # The curio backend makes this an awaitable thing.
             if maybe_awaitable is not None:
                 await maybe_awaitable
-            self.circuit.log.info("Client at %s:%d has turned events on.",
-                                  *self.circuit.address)
+
+            # Send all subscriptions that were marked as "to be sent" during
+            # the period that events were off.
+            resend = list(self.subscriptions_to_resend.items())
+            self.subscriptions_to_resend.clear()
+            for sub_spec, subs in resend:
+                for sub in subs:
+                    await sub.db_entry.subscribe(
+                        self.context.subscription_queue,
+                        sub_spec=sub_spec,
+                        sub=sub,
+                    )
+
             to_send = []
         elif isinstance(command, ca.EventsOffRequest):
-            # The client has signaled that it does not think it will be able to
-            # catch up to the backlog. Clear all updates queued to be sent...
-            self.unexpired_updates.clear()
+            self.circuit.log.info("Client at %s:%d has turned events off.",
+                                  *self.circuit.address)
+            self.time_events_toggled = time.monotonic()
             # ...and tell the Context that any future updates from ChannelData
             # should not be added to this circuit's queue until further notice.
             self.events_on.clear()
-            self.circuit.log.info("Client at %s:%d has turned events off.",
-                                  *self.circuit.address)
+            # The client has signaled that it does not think it will be able to
+            # catch up to the backlog. Clear all updates queued to be sent...
+            self.unexpired_updates.clear()
             to_send = []
         elif isinstance(command, ca.ClearChannelRequest):
             chan, db_entry = self._get_db_entry_from_command(command)
             await self._cull_subscriptions(
                 db_entry,
                 lambda sub: sub.channel == command.sid)
             to_send = [chan.clear()]
@@ -686,14 +743,16 @@
         if isinstance(command, ca.Message):
             tags['bytesize'] = len(command)
             self.log.debug("%r", command, extra=tags)
         return to_send
 
 
 class Context:
+    subscriptions: DefaultDict[SubscriptionSpec, Deque[Subscription]]
+
     def __init__(self, pvdb, interfaces=None):
         if interfaces is None:
             interfaces = ca.get_server_address_list()
         self.interfaces = interfaces
         self.udp_socks = {}  # map each interface to a UDP socket for searches
         self.beacon_socks = {}  # map each interface to a UDP socket for beacons
         self.pvdb = pvdb
@@ -883,143 +942,181 @@
         Async library implementations can (and should) reimplement this.
         Coroutine which evaluates one item from the circuit command queue.
         """
         while True:
             # This queue receives updates that match the db_entry, data_type
             # and mask ("subscription spec") of one or more subscriptions.
             sub_specs, metadata, values, flags, sub = await self.subscription_queue.get()
-            await self._subscription_queue_iteration(sub_specs, metadata,
-                                                     values, flags, sub)
-
-    async def _subscription_queue_iteration(self, sub_specs, metadata, values,
-                                            flags, sub):
-        '''Called on every item from the Context subscription queue
+            await self._subscription_queue_iteration(
+                sub_specs,
+                metadata,
+                values,
+                flags,
+                sub,
+            )
 
-        This queue receives updates that match the db_entry, data_type and mask
-        ("subscription spec") of one or more subscriptions.
-        '''
-        subs = []
+    async def _subscription_queue_iteration(
+        self,
+        sub_specs: Tuple[SubscriptionSpec, ...],
+        metadata: DbrTypeBase,
+        values,
+        flags: int,
+        sub: Subscription,
+    ):
+        """This handles a single queue item from ``subscription_queue``."""
         if sub is None:
             # Broadcast to all Subscriptions for the relevant
             # SubscriptionSpec(s).
             for sub_spec in sub_specs:
-                subs.extend(self.subscriptions[sub_spec])
+                for sub in self.subscriptions[sub_spec]:
+                    await self._subscription_queue_send(
+                        sub_spec,
+                        sub,
+                        metadata=metadata,
+                        values=values,
+                        flags=flags,
+                    )
         else:
             # A specific Subscription has been specified, which means this
             # specific update was prompted by Subscription being new, not
             # prompted by a new value. The update should only be sent to that
             # specific Subscription.
-            subs = [sub]
+            if len(sub_specs) != 1:
+                raise RuntimeError("Unexpected sub_specs length")
+
             sub_spec, = sub_specs
+            await self._subscription_queue_send(
+                sub_spec,
+                sub,
+                metadata=metadata,
+                values=values,
+                flags=flags,
+            )
+
+    async def _subscription_queue_send(
+        self,
+        sub_spec: SubscriptionSpec,
+        sub: Subscription,
+        metadata: DbrTypeBase,
+        values,
+        flags: int,
+    ):
+        '''Called on every item from the Context subscription queue
+
+        This queue receives updates that match the db_entry, data_type and mask
+        ("subscription spec") of one or more subscriptions.
+        '''
+        circuit = sub.circuit
+
+        # If this circuit has been sent EventsOff by the client, do not queue
+        # any updates until the client sends EventsOn to signal that it has
+        # caught up. Instead, mark this subscription as something that needs to
+        # be redone when events come back on.
+        if not circuit.events_on.is_set():
+            to_resend = circuit.subscriptions_to_resend.setdefault(sub_spec, [])
+            if sub not in to_resend:
+                to_resend.append(sub)
+            return
+
         # Pack the data and metadata into an EventAddResponse and send it.  We
         # have to make a new response for each channel because each may have a
         # different requested data_count.
-        for sub in subs:
-            circuit = sub.circuit
-            s_flags = flags
-            chan = sub.channel
+        chan = sub.channel
 
-            # This is a pass-through if arr is None.
-            values = apply_arr_filter(sub_spec.channel_filter.arr, values)
+        # This is a pass-through if arr is None.
+        values = apply_arr_filter(sub_spec.channel_filter.arr, values)
 
-            # If the subscription has a non-zero value respect it, else default
-            # to the full length of the data.
-            data_count = sub.data_count or len(values)
-            if data_count != len(values):
-                values = values[:data_count]
-
-            command = chan.subscribe(
-                data=values, metadata=metadata, data_type=sub.data_type,
-                data_count=data_count, subscriptionid=sub.subscriptionid,
-                status=1)
-
-            dbnd = sub.channel_filter.dbnd
-            if dbnd is not None:
-                new = values
-                if hasattr(new, 'endian'):
-                    if new.endian != host_endian:
-                        new = copy.copy(new)
-                        new.byteswap()
-                old = self.last_dead_band.get(sub)
-                if old is not None:
-                    old_iterable = isinstance(old, Iterable)
-                    new_iterable = isinstance(new, Iterable)
-                    if ((not old_iterable or (old_iterable and len(old) == 1)) and
-                            (not new_iterable or (new_iterable and len(new) == 1))):
-                        if old_iterable:
-                            old, = old
-                        if new_iterable:
-                            new, = new
-                        # Cool that was fun.
-                        if dbnd.m == 'rel':
-                            out_of_band = dbnd.d < abs((old - new) / old)
-                        else:  # must be 'abs' -- was already validated
-                            out_of_band = dbnd.d < abs(old - new)
-                        # We have verified that that EPICS considers DBE_LOG
-                        # etc. to be an absolute (not relative) threshold.
-                        abs_diff = abs(old - new)
-                        if abs_diff > sub.db_entry.log_atol:
-                            s_flags |= SubscriptionType.DBE_LOG
-                            if abs_diff > sub.db_entry.value_atol:
-                                s_flags |= SubscriptionType.DBE_VALUE
-
-                        if not (out_of_band and (sub.mask & s_flags)):
-                            continue
-                        else:
-                            self.last_dead_band[sub] = new
-                else:
-                    self.last_dead_band[sub] = new
+        # If the subscription has a non-zero value respect it, else default
+        # to the full length of the data.
+        data_count = sub.data_count or len(values)
+        if data_count != len(values):
+            values = values[:data_count]
+
+        command = chan.subscribe(
+            data=values,
+            metadata=metadata,
+            data_type=sub.data_type,
+            data_count=data_count,
+            subscriptionid=sub.subscriptionid,
+            status=1,
+        )
+
+        dbnd = sub.channel_filter.dbnd
+        if dbnd is not None:
+            deadband_tracking_value = apply_deadband_filter(
+                previous_value=self.last_dead_band.get(sub),
+                new_value=values,
+                sub=sub,
+                flags=flags,
+                host_endian=host_endian
+            )
+            if deadband_tracking_value is None:
+                return
 
-            # Special-case for edge-triggered modes of the sync Channel
-            # Filter (before, after, first, last). Only send the first
-            # update to each channel.
-            sync = sub.channel_filter.sync
-            if sync is not None:
-                last_update = self.last_sync_edge_update[sub][sync.s].get(sync.m)
-                if last_update and last_update == command:
-                    # This is a redundant update. Do not send.
-                    continue
-                else:
-                    # Stash this and then send it.
-                    self.last_sync_edge_update[sub][sync.s][sync.m] = command
+            self.last_dead_band[sub] = deadband_tracking_value
+
+        # Special-case for edge-triggered modes of the sync Channel
+        # Filter (before, after, first, last). Only send the first
+        # update to each channel.
+        sync = sub.channel_filter.sync
+        if sync is not None:
+            last_update = self.last_sync_edge_update[sub][sync.s].get(sync.m)
+            if last_update and last_update == command:
+                # This is a redundant update. Do not send.
+                return
 
-            # This update will be put at the back of the line of updates to be
-            # sent.
-            #
-            # If len(unexpired_updates[id]) == SUBSCRIPTION_BACKLOG_QUOTA, then
-            # the command at the front of the line will be kicked out.  It is
-            # not literally removed from the queue but whenever it reaches the
-            # front of the line it will dropped on the floor instead of sent.
-            # This effectively prioritizes sending the client "new news"
-            # instead of "old news".
-
-            # If this circuit has been sent EventsOff by the client, do not
-            # queue any updates until the client sends EventsOn to signal that
-            # it has caught up. But stash the most recent update for each
-            # subscription, which will immediately send when we turn events
-            # back on.
-            if not circuit.events_on.is_set():
-                circuit.most_recent_updates[sub.subscriptionid] = command
-                continue
-
-            # This is an OrderedBoundedSet, a set with a maxlen, containing
-            # only commands for this particular subscription.
-            circuit.unexpired_updates[sub.subscriptionid].append(command)
+            # Stash this and then send it.
+            self.last_sync_edge_update[sub][sync.s][sync.m] = command
 
-            # This is a queue with the commands from _all_ subscriptions on
-            # this circuit.
-            try:
-                await circuit.subscription_queue.put(weakref.ref(command))
-            except circuit.QueueFull:
-                # We have hit the overall max for subscription backlog.
-                circuit.log.warning(
-                    "Critically high EventAddResponse load. Dropping all "
-                    "queued responses on this circuit.")
-                circuit.subscription_queue.clear()
-                circuit.unexpired_updates.clear()
+        # This update will be put at the back of the line of updates to be
+        # sent.
+        #
+        # If len(unexpired_updates[id]) == SUBSCRIPTION_BACKLOG_QUOTA, then the
+        # command at the front of the line will be kicked out.  It is not
+        # literally removed from the queue but whenever it reaches the front of
+        # the line it will dropped on the floor instead of sent. This
+        # effectively prioritizes sending the client "new news" instead of "old
+        # news".
+
+        # This is an OrderedBoundedSet, a set with a maxlen, containing only
+        # commands for this particular subscription.
+
+        if sub.subscriptionid not in circuit.unexpired_updates:
+            circuit.unexpired_updates[sub.subscriptionid] = deque(
+                maxlen=sub.db_entry.max_subscription_backlog,
+            )
+
+        circuit.unexpired_updates[sub.subscriptionid].append(command)
+
+        def destroyed(_):
+            # If events are on, we hit a high load scenario and should drop
+            # this subscription entirely.
+            if circuit.events_on.is_set():
+                return
+
+            # However, if events are off, the data likely just got garbage
+            # collected because the client requested as much.
+            # Track this as a subscription to resend when events come back
+            # online, but don't store the data.
+            to_resend = circuit.subscriptions_to_resend.setdefault(sub_spec, [])
+            if sub not in to_resend:
+                to_resend.append(sub)
+
+        # This is a queue with the commands from _all_ subscriptions on this
+        # circuit.
+        try:
+            await circuit.subscription_queue.put(weakref.ref(command, destroyed))
+        except circuit.QueueFull:
+            # We have hit the overall max for subscription backlog.
+            circuit.log.warning(
+                "Critically high EventAddResponse load. Dropping all "
+                "queued responses on this circuit."
+            )
+            circuit.subscription_queue.clear()
+            circuit.unexpired_updates.clear()
 
     async def broadcast_beacon_loop(self):
         self.log.debug('Will send beacons to %r',
                        [f'{h}:{p}' for h, p in self.beacon_socks.keys()])
         MIN_BEACON_PERIOD = 0.02  # "RECOMMENDED" by the CA spec
         BEACON_BACKOFF = 2  # "RECOMMENDED" by the CA spec
         max_beacon_period = self.environ['EPICS_CAS_BEACON_PERIOD']
```

### Comparing `caproto-1.0.1/caproto/server/conversion.py` & `caproto-1.1.0/caproto/server/conversion.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/server/menus.py` & `caproto-1.1.0/caproto/server/menus.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/server/records/__init__.py` & `caproto-1.1.0/caproto/server/records/__init__.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/server/records/base.py` & `caproto-1.1.0/caproto/server/records/base.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/server/records/menus.jinja2` & `caproto-1.1.0/caproto/server/records/menus.jinja2`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/server/records/mixins.py` & `caproto-1.1.0/caproto/server/records/mixins.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/server/records/record_body.jinja2` & `caproto-1.1.0/caproto/server/records/record_body.jinja2`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/server/records/records.jinja2` & `caproto-1.1.0/caproto/server/records/records.jinja2`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/server/records/records.py` & `caproto-1.1.0/caproto/server/records/records.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/server/records/utils.py` & `caproto-1.1.0/caproto/server/records/utils.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/server/server.py` & `caproto-1.1.0/caproto/server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from caproto._log import _set_handler_with_logger, set_handler
 
 from .. import (AccessRights, AlarmSeverity, AlarmStatus,
                 CaprotoAttributeError, CaprotoRuntimeError, CaprotoTypeError,
                 CaprotoValueError, ChannelAlarm, ChannelByte, ChannelChar,
                 ChannelData, ChannelDouble, ChannelEnum, ChannelFloat,
                 ChannelInteger, ChannelShort, ChannelString, ChannelType,
-                __version__, get_server_address_list)
+                __version__, _constants, get_server_address_list)
 from .._backend import backend
 from .typing import (AinitHook, AsyncLibraryLayer, BoundGetter, BoundPutter,
                      BoundScan, BoundShutdown, BoundStartup, Getter, Putter,
                      Scan, Shutdown, Startup)
 
 if typing.TYPE_CHECKING:
     from .records import RecordFieldGroup
@@ -245,27 +245,72 @@
                 name=f'{self.name}.fields')
 
             self.fields = self.field_inst.pvdb
         else:
             self.field_inst = None
             self.fields = {}
 
+        self._check_subscription_backlog_settings()
+
     def __getstate__(self):
         state = super().__getstate__()
         state["group"] = None
         return state
 
     def __getnewargs_ex__(self):
         args, kwargs = super().__getnewargs_ex__()
         kwargs["pvname"] = self.pvname
         kwargs["group"] = None
         kwargs["pvspec"] = self.pvspec
         kwargs["record"] = self.record_type
         return (args, kwargs)
 
+    def _check_subscription_backlog_settings(self) -> None:
+        warn_thresh = _constants.SUBSCRIPTION_BACKLOG_WARN_THRESHOLD_ELEMENTS
+        if warn_thresh <= 1:
+            # Warning disabled.
+            return
+        if not self.max_length or self.max_length <= 1:
+            # Never warn for scalars.
+            return
+        if (self.max_length * self.max_subscription_backlog) < warn_thresh:
+            # Not over the threshold, so don't warn.
+            return
+
+        logger = self.group.log if self.group is not None else module_logger
+        reduce = _constants.SUBSCRIPTION_BACKLOG_REDUCE_AT_WARN_LEVEL
+        if reduce:
+            self.max_subscription_backlog = max(
+                (
+                    # Use the warning threshold to squeeze in under the
+                    # warning,
+                    warn_thresh // self.max_length,
+                    # But at minimum, provide this many subscriptions in
+                    # the backlog.
+                    _constants.MIN_SUBSCRIPTION_BACKLOG,
+                )
+            )
+            details = (
+                f"Automatically reduced the subscription backlog based on "
+                f"settings: {self.max_subscription_backlog}"
+            )
+        else:
+            details = (
+                "Not reducing the subscription backlog as it has been disabled."
+            )
+
+        logger.warning(
+            "PV %r with up to %d elements has the potential to take up considerable "
+            "memory when subscribed to with the default backlog of %d.  %s",
+            self.pvname,
+            self.max_length,
+            _constants.MAX_SUBSCRIPTION_BACKLOG,
+            details,
+        )
+
     async def read(self, data_type):
         """
         The top-level read method, with a specific requested data type.
 
         This calls the getter (if defined, falling back to
         `PVGroup.group_read`).  If the getter returns a value, it will be
         written back to update the internal state and update any subscriptions.
@@ -729,14 +774,15 @@
         try:
             inst = cls(**kwargs)
         except Exception as ex:
             raise CaprotoRuntimeError(
                 f"Failed to instantiate {cls.__name__!r} from PVSpec: {ex} "
                 f"(kwargs={kwargs})"
             ) from ex
+
         inst.__doc__ = self.doc
         return inst
 
 
 def scan_wrapper(
     scan_function: Scan,
     period: float,
```

### Comparing `caproto-1.0.1/caproto/server/stats.py` & `caproto-1.1.0/caproto/server/stats.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/server/typing.py` & `caproto-1.1.0/caproto/server/typing.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/sync/client.py` & `caproto-1.1.0/caproto/sync/client.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/sync/repeater.py` & `caproto-1.1.0/caproto/sync/repeater.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/sync/shark.py` & `caproto-1.1.0/caproto/sync/shark.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/conftest.py` & `caproto-1.1.0/caproto/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/dbd.py` & `caproto-1.1.0/caproto/tests/dbd.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/debug.py` & `caproto-1.1.0/caproto/tests/debug.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/epics_test_utils.py` & `caproto-1.1.0/caproto/tests/epics_test_utils.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/example_runner.py` & `caproto-1.1.0/caproto/tests/example_runner.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/ioc_all_in_one.py` & `caproto-1.1.0/caproto/tests/ioc_all_in_one.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/ioc_any_record.py` & `caproto-1.1.0/caproto/tests/ioc_any_record.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/ioc_inline_style.py` & `caproto-1.1.0/caproto/tests/ioc_inline_style.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/ioc_process.py` & `caproto-1.1.0/caproto/tests/ioc_process.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/test_catvs.py` & `caproto-1.1.0/caproto/tests/test_catvs.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/test_channel_filters.py` & `caproto-1.1.0/caproto/tests/test_channel_filters.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/test_cli_scripts.py` & `caproto-1.1.0/caproto/tests/test_cli_scripts.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/test_core.py` & `caproto-1.1.0/caproto/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/test_data_conversion.py` & `caproto-1.1.0/caproto/tests/test_data_conversion.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/test_data_copy.py` & `caproto-1.1.0/caproto/tests/test_data_copy.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/test_dbr_types.py` & `caproto-1.1.0/caproto/tests/test_dbr_types.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/test_doc_utils.py` & `caproto-1.1.0/caproto/tests/test_doc_utils.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/test_examples.py` & `caproto-1.1.0/caproto/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/test_logging.py` & `caproto-1.1.0/caproto/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/test_macros.py` & `caproto-1.1.0/caproto/tests/test_macros.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/test_nonet.py` & `caproto-1.1.0/caproto/tests/test_nonet.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/test_pyepics_compat.py` & `caproto-1.1.0/caproto/tests/test_pyepics_compat.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/test_pyepics_compat2.py` & `caproto-1.1.0/caproto/tests/test_pyepics_compat2.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/test_record_compliance.py` & `caproto-1.1.0/caproto/tests/test_record_compliance.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/test_records.py` & `caproto-1.1.0/caproto/tests/test_records.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/test_repeater.py` & `caproto-1.1.0/caproto/tests/test_repeater.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/test_serialization.py` & `caproto-1.1.0/caproto/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/test_server.py` & `caproto-1.1.0/caproto/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/test_shark.py` & `caproto-1.1.0/caproto/tests/test_shark.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/test_status.py` & `caproto-1.1.0/caproto/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/test_threading_client.py` & `caproto-1.1.0/caproto/tests/test_threading_client.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/test_timestamp.py` & `caproto-1.1.0/caproto/tests/test_timestamp.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/test_utils.py` & `caproto-1.1.0/caproto/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/tests/view_leaks.py` & `caproto-1.1.0/caproto/tests/view_leaks.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/threading/client.py` & `caproto-1.1.0/caproto/threading/client.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/threading/pyepics_compat.py` & `caproto-1.1.0/caproto/threading/pyepics_compat.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/caproto/trio/server.py` & `caproto-1.1.0/caproto/trio/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         self.new_command_condition = trio.Condition()
         self.subscription_chan = open_memory_channel(ca.MAX_TOTAL_SUBSCRIPTION_BACKLOG)
 
         # For compatibility with server common:
         self.subscription_queue = self.subscription_chan.send
 
         self.write_event = Event()
-        self.events_on = trio.Event()
+        self.events_on = Event()
 
     async def run(self):
         await self.nursery.start(self.command_queue_loop)
         await self.nursery.start(self.subscription_queue_loop)
 
     async def _send_buffers(self, *buffers):
         """Send ``buffers`` over the wire."""
```

### Comparing `caproto-1.0.1/caproto.egg-info/SOURCES.txt` & `caproto-1.1.0/caproto.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,18 @@
-.codecov.yml
-.coveragerc
-.editorconfig
-.flake8
-.gitattributes
-.gitignore
-.gitmodules
-.pre-commit-config.yaml
-CAproto.html
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
-azure-pipelines.yml
-codecov.yml
 generate_headers.py
 headers.tpl
-pytest.ini
 requirements-doc.txt
 requirements-test.txt
-run_tests.py
 setup.cfg
 setup.py
-setup_development_network.sh
-setup_local_dev_env.sh
 versioneer.py
-.ci/azure_env.sh
-.ci/install.sh
-.github/workflows/docs.yml
-.github/workflows/flake8.yml
-.github/workflows/pypi.yml
-.github/workflows/testing.yml
 caproto/__init__.py
 caproto/_array_backend.py
 caproto/_backend.py
 caproto/_broadcaster.py
 caproto/_circuit.py
 caproto/_commands.py
 caproto/_constants.py
@@ -162,22 +141,24 @@
 caproto/tests/debug.py
 caproto/tests/epics_test_utils.py
 caproto/tests/example_runner.py
 caproto/tests/ioc_all_in_one.py
 caproto/tests/ioc_any_record.py
 caproto/tests/ioc_inline_style.py
 caproto/tests/ioc_process.py
+caproto/tests/issue_797_server.py
 caproto/tests/test_catvs.py
 caproto/tests/test_channel_filters.py
 caproto/tests/test_cli_scripts.py
 caproto/tests/test_core.py
 caproto/tests/test_data_conversion.py
 caproto/tests/test_data_copy.py
 caproto/tests/test_dbr_types.py
 caproto/tests/test_doc_utils.py
+caproto/tests/test_events_off.py
 caproto/tests/test_examples.py
 caproto/tests/test_fixtures.py
 caproto/tests/test_logging.py
 caproto/tests/test_macros.py
 caproto/tests/test_nonet.py
 caproto/tests/test_pyepics_compat.py
 caproto/tests/test_pyepics_compat2.py
@@ -189,40 +170,33 @@
 caproto/tests/test_shark.py
 caproto/tests/test_status.py
 caproto/tests/test_threading_client.py
 caproto/tests/test_timestamp.py
 caproto/tests/test_utils.py
 caproto/tests/verify_with_catvs.py
 caproto/tests/view_leaks.py
-caproto/tests/data/example_tcp_data.pcap
-caproto/tests/data/example_udp_data.pcap
 caproto/threading/__init__.py
 caproto/threading/client.py
 caproto/threading/pyepics_compat.py
 caproto/trio/__init__.py
 caproto/trio/server.py
 caproto/trio/util.py
 doc/Makefile
 doc/gen_graphs.py
-doc/github_deploy_key.enc
 doc/make.bat
-doc/rebuild.sh
-doc/spec-issues.md
 doc/source/api.rst
 doc/source/async-clients.rst
 doc/source/basics.rst
 doc/source/clients.rst
 doc/source/command-line-client.rst
 doc/source/conf.py
 doc/source/containers.rst
 doc/source/cookiecutter.rst
 doc/source/environment_variables.rst
-doc/source/example_autosummary.txt
 doc/source/example_conf.py
-doc/source/example_requirements-docs.txt
 doc/source/index.rst
 doc/source/install.rst
 doc/source/iocs.rst
 doc/source/loggers.rst
 doc/source/own_docs.rst
 doc/source/protocol-compliance.rst
 doc/source/pyepics-compat-client.rst
@@ -230,11 +204,8 @@
 doc/source/references.rst
 doc/source/release-notes.rst
 doc/source/server_api.rst
 doc/source/servers.rst
 doc/source/shark.rst
 doc/source/sync-client.rst
 doc/source/threading-client.rst
-doc/source/_static/inheritance.css
-doc/source/_static/placeholder
-other_licenses/pyepics
-other_licenses/tornado
+doc/source/_static/inheritance.css
```

### Comparing `caproto-1.0.1/doc/Makefile` & `caproto-1.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/doc/gen_graphs.py` & `caproto-1.1.0/doc/gen_graphs.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/doc/make.bat` & `caproto-1.1.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/doc/source/api.rst` & `caproto-1.1.0/doc/source/api.rst`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/doc/source/async-clients.rst` & `caproto-1.1.0/doc/source/async-clients.rst`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/doc/source/basics.rst` & `caproto-1.1.0/doc/source/basics.rst`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/doc/source/clients.rst` & `caproto-1.1.0/doc/source/clients.rst`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/doc/source/command-line-client.rst` & `caproto-1.1.0/doc/source/command-line-client.rst`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/doc/source/conf.py` & `caproto-1.1.0/doc/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,18 @@
     'sphinx.ext.mathjax',
     'sphinx.ext.ifconfig',
     'sphinx.ext.viewcode',
     'sphinx.ext.githubpages',
     'IPython.sphinxext.ipython_directive',
     'IPython.sphinxext.ipython_console_highlighting',
     'numpydoc',
-    'doctr_versions_menu',
+    'docs_versions_menu',
 ]
 
-doctr_versions_menu_conf = {
+docs_versions_menu_conf = {
     'json_file': '/caproto/versions.json'
 }
 
 sys._caproto_hack_docs_source_path = os.path.dirname(__file__)
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = [os.path.relpath(caproto.docs.templates.PATH, start='.')]
```

### Comparing `caproto-1.0.1/doc/source/containers.rst` & `caproto-1.1.0/doc/source/containers.rst`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/doc/source/cookiecutter.rst` & `caproto-1.1.0/doc/source/cookiecutter.rst`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/doc/source/example_conf.py` & `caproto-1.1.0/doc/source/example_conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     'sphinx.ext.todo',
     'sphinx.ext.coverage',
     'sphinx.ext.mathjax',
     'sphinx.ext.viewcode',
     'sphinx.ext.githubpages',
     'sphinx.ext.intersphinx',
     'numpydoc',
-    # 'doctr_versions_menu',
+    # 'docs_versions_menu',
     'sphinx_rtd_theme',
 ]
 
 templates_path = [caproto.docs.templates.PATH]
 
 source_suffix = '.rst'
 master_doc = 'index'
```

### Comparing `caproto-1.0.1/doc/source/index.rst` & `caproto-1.1.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/doc/source/install.rst` & `caproto-1.1.0/doc/source/install.rst`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/doc/source/iocs.rst` & `caproto-1.1.0/doc/source/iocs.rst`

 * *Files 2% similar despite different names*

```diff
@@ -723,14 +723,43 @@
 
 Periodic updates should happen in ``scan`` loops.
 
 If PVGroup data is sourced from a database, real device, website, etc,
 then a different approach may be more appropriate.  See below in the "how do I"
 section.
 
+Help!
+=====
+
+
+My server is saying "High load"!
+--------------------------------
+
+You may have a real issue in your code, or you may have clients which are
+saturating your server with requests.
+
+Take a look at your code and see that you don't have any synchronous (i.e.,
+threaded) code being run in your async functions.  This is really important.
+Defer it to an executor and you can avoid further headaches: see
+`here <https://docs.python.org/3/library/asyncio-eventloop.html#asyncio.loop.run_in_executor>`_.
+
+If you just have a lot of clients hitting your server without any apparent
+negative effect, you can customize caproto's server settings to not display
+this message.
+
+This warning says my PV will take up a considerable amount of memory...
+-----------------------------------------------------------------------
+
+It's probably true and it's there to save you from the default settings.
+
+You may either set ``max_subscription_backlog`` for each of your big PVs
+manually, or let caproto tweak it for you in an automated fashion.
+
+See the environment variable section for details on what each variable means.
+
 How do I...
 ===========
 
 ... access ``async_lib`` directly in my class?
 ----------------------------------------------
 
 If you have any startup hooks defined, you can stash ``async_lib`` there.
@@ -979,14 +1008,21 @@
                 if key is not None:
                     await alarm.write(
                         status=AlarmStatus.COMM,
                         severity=AlarmSeverity.MAJOR_ALARM,
                     )
 
 
+... interact with threaded/non-async code, functions, and libraries?
+--------------------------------------------------------------------
+
+Defer it to an executor:
+`here <https://docs.python.org/3/library/asyncio-eventloop.html#asyncio.loop.run_in_executor>`_.
+
+
 ... get rid of PVGroup and pvproperty? I hate them!
 ---------------------------------------------------
 
 Those are some strong words!
 
 caproto developers think the ease of customization and terseness of the class
 definition are positives - making it the easiest possible way to spin up an IOC
```

### Comparing `caproto-1.0.1/doc/source/loggers.rst` & `caproto-1.1.0/doc/source/loggers.rst`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/doc/source/own_docs.rst` & `caproto-1.1.0/doc/source/own_docs.rst`

 * *Files 10% similar despite different names*

```diff
@@ -26,17 +26,18 @@
 necessary to run your package, most likely.  The caproto developers recommend
 creating a separate requirements file that can be installed by way of ``pip``
 or ``conda`` (i.e., ``pip install --requirement requirements-docs.txt`` or
 ``conda install --file requirements-docs.txt``).
 
 .. literalinclude:: example_requirements-docs.txt
 
-``doctr`` and ``doctr-versions-menu`` are useful if building documentation
-using continuous integration, but are unnecessary if you will only be building
-documentation locally.
+``docs-versions-menu`` is useful for building versioned documentation targeting
+GitHub pages using continuous integration.  It is unnecessary if you will only
+be building documentation locally or only care about the latest release
+documentation.
 
 
 Using autosummary
 =================
 
 .. literalinclude:: example_autosummary.txt
     :linenos:
```

### Comparing `caproto-1.0.1/doc/source/protocol-compliance.rst` & `caproto-1.1.0/doc/source/protocol-compliance.rst`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/doc/source/pyepics-compat-client.rst` & `caproto-1.1.0/doc/source/pyepics-compat-client.rst`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/doc/source/records.rst` & `caproto-1.1.0/doc/source/records.rst`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/doc/source/references.rst` & `caproto-1.1.0/doc/source/references.rst`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/doc/source/release-notes.rst` & `caproto-1.1.0/doc/source/release-notes.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 ***************
 Release History
 ***************
 
+v1.0.1 (2023-03-29)
+===================
+
+Added / Fixed
+-------------
+
+* Timeout no longer ignored in pyepics_compat's caget_many (@mcnanneyd, #806)
+* New example: Lakeshore temperature controller (@gwbischof, #809)
+
+
 v1.0.0 (2022-09-01)
 ===================
 
 Breaking Changes
 ----------------
 
 - Python 3.6 and Python 3.7 support has been dropped. Python 3.8 through Python
```

### Comparing `caproto-1.0.1/doc/source/server_api.rst` & `caproto-1.1.0/doc/source/server_api.rst`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/doc/source/servers.rst` & `caproto-1.1.0/doc/source/servers.rst`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/doc/source/shark.rst` & `caproto-1.1.0/doc/source/shark.rst`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/doc/source/sync-client.rst` & `caproto-1.1.0/doc/source/sync-client.rst`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/doc/source/threading-client.rst` & `caproto-1.1.0/doc/source/threading-client.rst`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/generate_headers.py` & `caproto-1.1.0/generate_headers.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/headers.tpl` & `caproto-1.1.0/headers.tpl`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/setup.py` & `caproto-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `caproto-1.0.1/versioneer.py` & `caproto-1.1.0/versioneer.py`

 * *Files identical despite different names*

