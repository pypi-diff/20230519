# Comparing `tmp/pyllamacpp-2.1.3.tar.gz` & `tmp/pyllamacpp-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllamacpp-2.1.3.tar", last modified: Sun May  7 00:23:35 2023, max compression
+gzip compressed data, was "pyllamacpp-2.2.0.tar", last modified: Fri May 19 00:24:58 2023, max compression
```

## Comparing `pyllamacpp-2.1.3.tar` & `pyllamacpp-2.2.0.tar`

### file list

```diff
@@ -1,109 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.980304 pyllamacpp-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-05-07 00:23:35.980304 pyllamacpp-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.968303 pyllamacpp-2.1.3/llama.cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-07 00:23:24.000000 pyllamacpp-2.1.3/llama.cpp/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.968303 pyllamacpp-2.1.3/llama.cpp/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-07 00:23:24.000000 pyllamacpp-2.1.3/llama.cpp/examples/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.968303 pyllamacpp-2.1.3/llama.cpp/examples/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-07 00:23:24.000000 pyllamacpp-2.1.3/llama.cpp/examples/embedding/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.968303 pyllamacpp-2.1.3/llama.cpp/examples/main/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-07 00:23:24.000000 pyllamacpp-2.1.3/llama.cpp/examples/main/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.968303 pyllamacpp-2.1.3/llama.cpp/examples/perplexity/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-07 00:23:24.000000 pyllamacpp-2.1.3/llama.cpp/examples/perplexity/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.968303 pyllamacpp-2.1.3/llama.cpp/examples/quantize/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-07 00:23:24.000000 pyllamacpp-2.1.3/llama.cpp/examples/quantize/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.968303 pyllamacpp-2.1.3/llama.cpp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-07 00:23:24.000000 pyllamacpp-2.1.3/llama.cpp/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.968303 pyllamacpp-2.1.3/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.964303 pyllamacpp-2.1.3/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.972303 pyllamacpp-2.1.3/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.972303 pyllamacpp-2.1.3/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.972303 pyllamacpp-2.1.3/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.972303 pyllamacpp-2.1.3/pybind11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.976304 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.976304 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.976304 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.976304 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.976304 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.976304 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.976304 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.976304 pyllamacpp-2.1.3/pybind11/tests/test_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tests/test_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.976304 pyllamacpp-2.1.3/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/setup_main.py.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.968303 pyllamacpp-2.1.3/pyllamacpp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pyllamacpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pyllamacpp/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pyllamacpp/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pyllamacpp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pyllamacpp/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pyllamacpp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pyllamacpp/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.976304 pyllamacpp-2.1.3/pyllamacpp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-05-07 00:23:35.000000 pyllamacpp-2.1.3/pyllamacpp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-07 00:23:35.000000 pyllamacpp-2.1.3/pyllamacpp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 00:23:35.000000 pyllamacpp-2.1.3/pyllamacpp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 00:23:35.000000 pyllamacpp-2.1.3/pyllamacpp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 00:23:35.000000 pyllamacpp-2.1.3/pyllamacpp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-07 00:23:35.000000 pyllamacpp-2.1.3/pyllamacpp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 00:23:35.980304 pyllamacpp-2.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.976304 pyllamacpp-2.1.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/src/llama.cpp_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28402 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/src/main.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.389226 pyllamacpp-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12730 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-05-19 00:24:58.389226 pyllamacpp-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)    13701 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/examples/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/examples/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/examples/benchmark/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/examples/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/examples/embedding/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/examples/main/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/examples/main/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/examples/perplexity/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/examples/perplexity/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/examples/quantize/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/examples/quantize/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/examples/quantize-stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/examples/quantize-stats/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/examples/save-load-state/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/examples/save-load-state/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/pocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/pocs/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/pocs/vdot/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/pocs/vdot/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/scripts/build-info.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/llama.cpp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-19 00:24:45.000000 pyllamacpp-2.2.0/llama.cpp/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.377225 pyllamacpp-2.2.0/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.385225 pyllamacpp-2.2.0/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.385225 pyllamacpp-2.2.0/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.385225 pyllamacpp-2.2.0/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.385225 pyllamacpp-2.2.0/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.385225 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.385225 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.385225 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.385225 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.385225 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.385225 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.385225 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.385225 pyllamacpp-2.2.0/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tests/test_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.389226 pyllamacpp-2.2.0/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/FindPythonLibsNew.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pybind11/tools/setup_main.py.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.381225 pyllamacpp-2.2.0/pyllamacpp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pyllamacpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pyllamacpp/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pyllamacpp/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pyllamacpp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pyllamacpp/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pyllamacpp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pyllamacpp/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.389226 pyllamacpp-2.2.0/pyllamacpp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-05-19 00:24:58.000000 pyllamacpp-2.2.0/pyllamacpp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-19 00:24:58.000000 pyllamacpp-2.2.0/pyllamacpp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 00:24:58.000000 pyllamacpp-2.2.0/pyllamacpp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-19 00:24:58.000000 pyllamacpp-2.2.0/pyllamacpp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 00:24:58.000000 pyllamacpp-2.2.0/pyllamacpp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 00:24:58.000000 pyllamacpp-2.2.0/pyllamacpp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 00:24:58.389226 pyllamacpp-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:24:58.389226 pyllamacpp-2.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/src/llama.cpp_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43662 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-19 00:24:44.000000 pyllamacpp-2.2.0/src/main.h
```

### Comparing `pyllamacpp-2.1.3/CMakeLists.txt` & `pyllamacpp-2.2.0/CMakeLists.txt`

 * *Files 22% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -pthread")
 
 add_subdirectory(pybind11)
 add_subdirectory(llama.cpp)
 # add_subdirectory(ggml)
 
 file (GLOB CPP_FILES "llama.cpp/*.cpp")
-file (GLOB C_FILES "llama.cpp/*.c")
-file (GLOB H_FILES "llama.cpp/*.h")
+file (GLOB C_FILES "llama.cpp/ggml.c")
+file (GLOB H_FILES "llama.cpp/ggml.h" "llama.cpp/llama.h")
 
 # ---------------------------------------------------------------------------------------------
 
 
 
 set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
 
@@ -72,27 +72,40 @@
 option(LLAMA_SANITIZE_ADDRESS       "llama: enable address sanitizer"                       OFF)
 option(LLAMA_SANITIZE_UNDEFINED     "llama: enable undefined sanitizer"                     OFF)
 
 # instruction set specific
 option(LLAMA_AVX                    "llama: enable AVX"                                     ON)
 option(LLAMA_AVX2                   "llama: enable AVX2"                                    ON)
 option(LLAMA_AVX512                 "llama: enable AVX512"                                  OFF)
+option(LLAMA_AVX512_VBMI            "llama: enable AVX512-VBMI"                             OFF)
+option(LLAMA_AVX512_VNNI            "llama: enable AVX512-VNNI"                             OFF)
 option(LLAMA_FMA                    "llama: enable FMA"                                     ON)
+# in MSVC F16C is implied with AVX2/AVX512
+if (NOT MSVC)
+    option(LLAMA_F16C               "llama: enable F16C"                                    ON)
+endif()
 
 # 3rd party libs
 option(LLAMA_ACCELERATE             "llama: enable Accelerate framework"                    ON)
 option(LLAMA_OPENBLAS               "llama: use OpenBLAS"                                   OFF)
+option(LLAMA_CUBLAS                 "llama: use cuBLAS"                                     OFF)
+option(LLAMA_CLBLAST                "llama: use CLBlast"                                    OFF)
 
 option(LLAMA_BUILD_TESTS            "llama: build tests"    ${LLAMA_STANDALONE})
 option(LLAMA_BUILD_EXAMPLES         "llama: build examples" ${LLAMA_STANDALONE})
 
 #
 # Compile flags
 #
 
+set(CMAKE_CXX_STANDARD 11)
+set(CMAKE_CXX_STANDARD_REQUIRED true)
+set(CMAKE_C_STANDARD 11)
+set(CMAKE_C_STANDARD_REQUIRED true)
+set(THREADS_PREFER_PTHREAD_FLAG ON)
 find_package(Threads REQUIRED)
 
 if (NOT MSVC)
     if (LLAMA_SANITIZE_THREAD)
         add_compile_options(-fsanitize=thread)
         link_libraries(-fsanitize=thread)
     endif()
@@ -115,62 +128,126 @@
 
         add_compile_definitions(GGML_USE_ACCELERATE)
         set(LLAMA_EXTRA_LIBS ${LLAMA_EXTRA_LIBS} ${ACCELERATE_FRAMEWORK})
     else()
         message(WARNING "Accelerate framework not found")
     endif()
 endif()
+
 if (LLAMA_OPENBLAS)
     if (LLAMA_STATIC)
         set(BLA_STATIC ON)
     endif()
 
     set(BLA_VENDOR OpenBLAS)
     find_package(BLAS)
     if (BLAS_FOUND)
         message(STATUS "OpenBLAS found")
 
         add_compile_definitions(GGML_USE_OPENBLAS)
         add_link_options(${BLAS_LIBRARIES})
+        set(LLAMA_EXTRA_LIBS ${LLAMA_EXTRA_LIBS} openblas)
+
+        # find header file
+        set(OPENBLAS_INCLUDE_SEARCH_PATHS
+            /usr/include
+            /usr/include/openblas
+            /usr/include/openblas-base
+            /usr/local/include
+            /usr/local/include/openblas
+            /usr/local/include/openblas-base
+            /opt/OpenBLAS/include
+            $ENV{OpenBLAS_HOME}
+            $ENV{OpenBLAS_HOME}/include
+            )
+        find_path(OPENBLAS_INC NAMES cblas.h PATHS ${OPENBLAS_INCLUDE_SEARCH_PATHS})
+        add_compile_options(-I${OPENBLAS_INC})
     else()
         message(WARNING "OpenBLAS not found")
     endif()
 endif()
 
+if (LLAMA_CUBLAS)
+    cmake_minimum_required(VERSION 3.17)
+
+    find_package(CUDAToolkit)
+    if (CUDAToolkit_FOUND)
+        message(STATUS "cuBLAS found")
+
+        enable_language(CUDA)
+
+        set(GGML_CUDA_SOURCES ggml-cuda.cu ggml-cuda.h)
+
+        add_compile_definitions(GGML_USE_CUBLAS)
+
+        if (LLAMA_STATIC)
+            set(LLAMA_EXTRA_LIBS ${LLAMA_EXTRA_LIBS} CUDA::cudart_static CUDA::cublas_static CUDA::cublasLt_static)
+        else()
+            set(LLAMA_EXTRA_LIBS ${LLAMA_EXTRA_LIBS} CUDA::cudart CUDA::cublas CUDA::cublasLt)
+        endif()
+
+    else()
+        message(WARNING "cuBLAS not found")
+    endif()
+endif()
+
+if (LLAMA_CLBLAST)
+    find_package(CLBlast)
+    if (CLBlast_FOUND)
+        message(STATUS "CLBlast found")
+
+        set(GGML_OPENCL_SOURCES ggml-opencl.c ggml-opencl.h)
+
+        add_compile_definitions(GGML_USE_CLBLAST)
+
+        set(LLAMA_EXTRA_LIBS ${LLAMA_EXTRA_LIBS} clblast)
+    else()
+        message(WARNING "CLBlast not found")
+    endif()
+endif()
+
 if (LLAMA_ALL_WARNINGS)
     if (NOT MSVC)
         set(c_flags
             -Wall
             -Wextra
             -Wpedantic
             -Wcast-qual
             -Wdouble-promotion
             -Wshadow
             -Wstrict-prototypes
             -Wpointer-arith
-            -Wno-unused-function
         )
         set(cxx_flags
             -Wall
             -Wextra
             -Wpedantic
             -Wcast-qual
             -Wno-unused-function
+            -Wno-multichar
         )
     else()
         # todo : msvc
     endif()
 
     add_compile_options(
             "$<$<COMPILE_LANGUAGE:C>:${c_flags}>"
             "$<$<COMPILE_LANGUAGE:CXX>:${cxx_flags}>"
     )
 
 endif()
 
+if (MSVC)
+    add_compile_definitions(_CRT_SECURE_NO_WARNINGS)
+
+    if (BUILD_SHARED_LIBS)
+        set(CMAKE_WINDOWS_EXPORT_ALL_SYMBOLS ON)
+    endif()
+endif()
+
 if (LLAMA_LTO)
     include(CheckIPOSupported)
     check_ipo_supported(RESULT result OUTPUT output)
     if (result)
         set(CMAKE_INTERPROCEDURAL_OPTIMIZATION TRUE)
     else()
         message(WARNING "IPO is not supported: ${output}")
@@ -198,48 +275,85 @@
 
 if (${CMAKE_SYSTEM_PROCESSOR} MATCHES "arm" OR ${CMAKE_SYSTEM_PROCESSOR} MATCHES "aarch64")
     message(STATUS "ARM detected")
     if (MSVC)
         # TODO: arm msvc?
     else()
         if (${CMAKE_SYSTEM_PROCESSOR} MATCHES "aarch64")
+            # Apple M1, M2, etc.
+            # Raspberry Pi 3, 4, Zero 2 (64-bit)
             add_compile_options(-mcpu=native)
         endif()
-        # TODO: armv6,7,8 version specific flags
+        if (${CMAKE_SYSTEM_PROCESSOR} MATCHES "armv6")
+            # Raspberry Pi 1, Zero
+            add_compile_options(-mfpu=neon-fp-armv8 -mfp16-format=ieee -mno-unaligned-access)
+        endif()
+        if (${CMAKE_SYSTEM_PROCESSOR} MATCHES "armv7")
+            # Raspberry Pi 2
+            add_compile_options(-mfpu=neon-fp-armv8 -mfp16-format=ieee -mno-unaligned-access -funsafe-math-optimizations)
+        endif()
+        if (${CMAKE_SYSTEM_PROCESSOR} MATCHES "armv8")
+            # Raspberry Pi 3, 4, Zero 2 (32-bit)
+            add_compile_options(-mfp16-format=ieee -mno-unaligned-access)
+        endif()
     endif()
 elseif (${CMAKE_SYSTEM_PROCESSOR} MATCHES "^(x86_64|i686|AMD64)$")
     message(STATUS "x86 detected")
     if (MSVC)
         if (LLAMA_AVX512)
-            add_compile_options(/arch:AVX512)
+            add_compile_options($<$<COMPILE_LANGUAGE:C>:/arch:AVX512>)
+            add_compile_options($<$<COMPILE_LANGUAGE:CXX>:/arch:AVX512>)
+            # MSVC has no compile-time flags enabling specific
+            # AVX512 extensions, neither it defines the
+            # macros corresponding to the extensions.
+            # Do it manually.
+            if (LLAMA_AVX512_VBMI)
+                add_compile_definitions($<$<COMPILE_LANGUAGE:C>:__AVX512VBMI__>)
+                add_compile_definitions($<$<COMPILE_LANGUAGE:CXX>:__AVX512VBMI__>)
+            endif()
+            if (LLAMA_AVX512_VNNI)
+                add_compile_definitions($<$<COMPILE_LANGUAGE:C>:__AVX512VNNI__>)
+                add_compile_definitions($<$<COMPILE_LANGUAGE:CXX>:__AVX512VNNI__>)
+            endif()
         elseif (LLAMA_AVX2)
-            add_compile_options(/arch:AVX2)
+            add_compile_options($<$<COMPILE_LANGUAGE:C>:/arch:AVX2>)
+            add_compile_options($<$<COMPILE_LANGUAGE:CXX>:/arch:AVX2>)
         elseif (LLAMA_AVX)
-            add_compile_options(/arch:AVX)
+            add_compile_options($<$<COMPILE_LANGUAGE:C>:/arch:AVX>)
+            add_compile_options($<$<COMPILE_LANGUAGE:CXX>:/arch:AVX>)
         endif()
     else()
-        add_compile_options(-mf16c)
+        if (LLAMA_F16C)
+            add_compile_options(-mf16c)
+        endif()
         if (LLAMA_FMA)
             add_compile_options(-mfma)
         endif()
         if (LLAMA_AVX)
             add_compile_options(-mavx)
         endif()
         if (LLAMA_AVX2)
             add_compile_options(-mavx2)
         endif()
         if (LLAMA_AVX512)
             add_compile_options(-mavx512f)
-            # add_compile_options(-mavx512cd)
-            # add_compile_options(-mavx512dq)
-            # add_compile_options(-mavx512bw)
+            add_compile_options(-mavx512bw)
+        endif()
+        if (LLAMA_AVX512_VBMI)
+            add_compile_options(-mavx512vbmi)
+        endif()
+        if (LLAMA_AVX512_VNNI)
+            add_compile_options(-mavx512vnni)
         endif()
     endif()
+elseif (${CMAKE_SYSTEM_PROCESSOR} MATCHES "ppc64")
+    message(STATUS "PowerPC detected")
+    add_compile_options(-mcpu=native -mtune=native)
+    #TODO: Add  targets for Power8/Power9 (Altivec/VSX) and Power10(MMA) and query for big endian systems (ppc64/le/be)
 else()
-    # TODO: support PowerPC
     message(STATUS "Unknown architecture")
 endif()
 
 #
 # Build libraries
 #
```

### Comparing `pyllamacpp-2.1.3/LICENSE` & `pyllamacpp-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/PKG-INFO` & `pyllamacpp-2.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyllamacpp
-Version: 2.1.3
+Version: 2.2.0
 Summary: Python bindings for llama.cpp
 Author: Abdeladim Sadiki
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/pyllamacpp
 Project-URL: Source, https://github.com/abdeladim-s/pyllamacpp
 Project-URL: Tracker, https://github.com/abdeladim-s/pyllamacpp/issues
 Requires-Python: >=3.8
@@ -177,18 +177,15 @@
       print(f"{token}", end='', flush=True)
       print()
   except KeyboardInterrupt:
     break
 ```
 
 # Supported models
-
-Fully tested with [GPT4All](https://github.com/nomic-ai/gpt4all) model, see [PyGPT4All](https://github.com/nomic-ai/pygpt4all).
-
-But all models supported by `llama.cpp` should be supported as well:
+All models supported by `llama.cpp` should be supported basically:
 
 <blockquote>
 
 **Supported models:**
 
 - [X] LLaMA 🦙
 - [X] [Alpaca](https://github.com/ggerganov/llama.cpp#instruction-mode-with-alpaca)
```

### Comparing `pyllamacpp-2.1.3/README.md` & `pyllamacpp-2.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -164,18 +164,15 @@
       print(f"{token}", end='', flush=True)
       print()
   except KeyboardInterrupt:
     break
 ```
 
 # Supported models
-
-Fully tested with [GPT4All](https://github.com/nomic-ai/gpt4all) model, see [PyGPT4All](https://github.com/nomic-ai/pygpt4all).
-
-But all models supported by `llama.cpp` should be supported as well:
+All models supported by `llama.cpp` should be supported basically:
 
 <blockquote>
 
 **Supported models:**
 
 - [X] LLaMA 🦙
 - [X] [Alpaca](https://github.com/ggerganov/llama.cpp#instruction-mode-with-alpaca)
```

### Comparing `pyllamacpp-2.1.3/llama.cpp/examples/CMakeLists.txt` & `pyllamacpp-2.2.0/llama.cpp/examples/CMakeLists.txt`

 * *Files 20% similar despite different names*

```diff
@@ -27,10 +27,13 @@
 
 include_directories(${CMAKE_CURRENT_SOURCE_DIR})
 
 if (EMSCRIPTEN)
 else()
     add_subdirectory(main)
     add_subdirectory(quantize)
+    add_subdirectory(quantize-stats)
     add_subdirectory(perplexity)
     add_subdirectory(embedding)
+    add_subdirectory(save-load-state)
+    add_subdirectory(benchmark)
 endif()
```

### Comparing `pyllamacpp-2.1.3/pybind11/CMakeLists.txt` & `pyllamacpp-2.2.0/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/LICENSE` & `pyllamacpp-2.2.0/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/attr.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/buffer_info.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/cast.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/chrono.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/complex.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/detail/class.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/detail/common.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/detail/descr.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/detail/init.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/detail/internals.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/detail/type_caster_base.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/detail/typeid.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/eigen.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/embed.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/eval.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/functional.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/gil.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/iostream.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/numpy.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/operators.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/options.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/pybind11.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/pytypes.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/stl/filesystem.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/stl.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/include/pybind11/stl_bind.h` & `pyllamacpp-2.2.0/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/tests/CMakeLists.txt` & `pyllamacpp-2.2.0/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/CMakeLists.txt` & `pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `pyllamacpp-2.2.0/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/tests/test_embed/CMakeLists.txt` & `pyllamacpp-2.2.0/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/tools/FindCatch.cmake` & `pyllamacpp-2.2.0/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/tools/FindEigen3.cmake` & `pyllamacpp-2.2.0/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/tools/FindPythonLibsNew.cmake` & `pyllamacpp-2.2.0/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/tools/check-style.sh` & `pyllamacpp-2.2.0/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/tools/cmake_uninstall.cmake.in` & `pyllamacpp-2.2.0/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/tools/libsize.py` & `pyllamacpp-2.2.0/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/tools/make_changelog.py` & `pyllamacpp-2.2.0/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/tools/pybind11Common.cmake` & `pyllamacpp-2.2.0/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/tools/pybind11Config.cmake.in` & `pyllamacpp-2.2.0/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/tools/pybind11NewTools.cmake` & `pyllamacpp-2.2.0/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/tools/pybind11Tools.cmake` & `pyllamacpp-2.2.0/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/tools/setup_global.py.in` & `pyllamacpp-2.2.0/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pybind11/tools/setup_main.py.in` & `pyllamacpp-2.2.0/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pyllamacpp/_logger.py` & `pyllamacpp-2.2.0/pyllamacpp/_logger.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pyllamacpp/cli.py` & `pyllamacpp-2.2.0/pyllamacpp/cli.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pyllamacpp/utils.py` & `pyllamacpp-2.2.0/pyllamacpp/utils.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pyllamacpp/webui.py` & `pyllamacpp-2.2.0/pyllamacpp/webui.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/pyllamacpp.egg-info/PKG-INFO` & `pyllamacpp-2.2.0/pyllamacpp.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyllamacpp
-Version: 2.1.3
+Version: 2.2.0
 Summary: Python bindings for llama.cpp
 Author: Abdeladim Sadiki
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/pyllamacpp
 Project-URL: Source, https://github.com/abdeladim-s/pyllamacpp
 Project-URL: Tracker, https://github.com/abdeladim-s/pyllamacpp/issues
 Requires-Python: >=3.8
@@ -177,18 +177,15 @@
       print(f"{token}", end='', flush=True)
       print()
   except KeyboardInterrupt:
     break
 ```
 
 # Supported models
-
-Fully tested with [GPT4All](https://github.com/nomic-ai/gpt4all) model, see [PyGPT4All](https://github.com/nomic-ai/pygpt4all).
-
-But all models supported by `llama.cpp` should be supported as well:
+All models supported by `llama.cpp` should be supported basically:
 
 <blockquote>
 
 **Supported models:**
 
 - [X] LLaMA 🦙
 - [X] [Alpaca](https://github.com/ggerganov/llama.cpp#instruction-mode-with-alpaca)
```

### Comparing `pyllamacpp-2.1.3/pyllamacpp.egg-info/SOURCES.txt` & `pyllamacpp-2.2.0/pyllamacpp.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -9,18 +9,24 @@
 ./pyllamacpp/cli.py
 ./pyllamacpp/constants.py
 ./pyllamacpp/model.py
 ./pyllamacpp/utils.py
 ./pyllamacpp/webui.py
 llama.cpp/CMakeLists.txt
 llama.cpp/examples/CMakeLists.txt
+llama.cpp/examples/benchmark/CMakeLists.txt
 llama.cpp/examples/embedding/CMakeLists.txt
 llama.cpp/examples/main/CMakeLists.txt
 llama.cpp/examples/perplexity/CMakeLists.txt
 llama.cpp/examples/quantize/CMakeLists.txt
+llama.cpp/examples/quantize-stats/CMakeLists.txt
+llama.cpp/examples/save-load-state/CMakeLists.txt
+llama.cpp/pocs/CMakeLists.txt
+llama.cpp/pocs/vdot/CMakeLists.txt
+llama.cpp/scripts/build-info.cmake
 llama.cpp/tests/CMakeLists.txt
 pybind11/CMakeLists.txt
 pybind11/LICENSE
 pybind11/include/pybind11/attr.h
 pybind11/include/pybind11/buffer_info.h
 pybind11/include/pybind11/cast.h
 pybind11/include/pybind11/chrono.h
```

### Comparing `pyllamacpp-2.1.3/pyproject.toml` & `pyllamacpp-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/setup.py` & `pyllamacpp-2.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="pyllamacpp",
-    version="2.1.3",
+    version="2.2.0",
     author="Abdeladim Sadiki",
     description="Python bindings for llama.cpp",
     long_description=long_description,
     ext_modules=[CMakeExtension("_pyllamacpp")],
     cmdclass={"build_ext": CMakeBuild},
     zip_safe=False,
     # extras_require={"test": ["pytest>=6.0"]},
```

### Comparing `pyllamacpp-2.1.3/src/llama.cpp_LICENSE` & `pyllamacpp-2.2.0/src/llama.cpp_LICENSE`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.3/src/main.cpp` & `pyllamacpp-2.2.0/src/main.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -45,14 +45,57 @@
 }
 
 
 void llama_free_wrapper(struct llama_context_wrapper * ctx_w){
     llama_free(ctx_w->ptr);
 }
 
+void llama_apply_lora_from_file_wrapper(struct llama_context_wrapper * ctx_w,
+                                        const char * path_lora,
+                                        const char * path_base_model,
+                                        int   n_threads){
+    struct llama_context * ctx = ctx_w->ptr;
+    llama_apply_lora_from_file(ctx, path_lora, path_base_model, n_threads);
+}
+
+int llama_get_kv_cache_token_count_wrapper(struct llama_context_wrapper * ctx_w){
+    return llama_get_kv_cache_token_count(ctx_w->ptr);
+}
+
+void llama_set_rng_seed_wrapper(struct llama_context_wrapper * ctx_w, int seed){
+    llama_set_rng_seed(ctx_w->ptr, seed);
+}
+
+size_t llama_get_state_size_wrapper(struct llama_context_wrapper * ctx_w){
+    return llama_get_state_size(ctx_w->ptr);
+}
+
+bool llama_load_session_file_wrapper(struct llama_context_wrapper * ctx_w,
+                                     const char * path_session,
+                                     py::array_t<llama_token> tokens,
+                                     size_t n_token_capacity,
+                                     size_t * n_token_count_out){
+    struct llama_context * ctx = ctx_w->ptr;
+    py::buffer_info buf = tokens.request();
+    llama_token *tokens_ptr = static_cast<llama_token *>(buf.ptr);
+    return llama_load_session_file(ctx, path_session, tokens_ptr, n_token_capacity, n_token_count_out);
+
+}
+
+bool llama_save_session_file_wrapper(struct llama_context_wrapper * ctx_w,
+                                    const char * path_session,
+                                   py::array_t<llama_token> tokens,
+                                    size_t n_token_count){
+    struct llama_context * ctx = ctx_w->ptr;
+    py::buffer_info buf = tokens.request();
+    llama_token *tokens_ptr = static_cast<llama_token *>(buf.ptr);
+    return llama_save_session_file(ctx, path_session, tokens_ptr, n_token_count);
+
+}
+
 int llama_eval_wrapper(struct llama_context_wrapper * ctx_w,
                py::array_t<llama_token> tokens,
                int   n_tokens,
                int   n_past,
                int   n_threads){
    struct llama_context * ctx = ctx_w->ptr;
    py::buffer_info buf = tokens.request();
@@ -69,27 +112,14 @@
         std::vector<llama_token> tokens((text.size() + (int)add_bos));
         int new_size = llama_tokenize(ctx, text.c_str(), tokens.data(), tokens.size(), add_bos);
         assert(new_size >= 0);
         tokens.resize(new_size);
         return tokens;
 }
 
-//py::array_t<llama_token> llama_tokenize_wrapper(
-//        struct llama_context_wrapper * ctx_w,
-//        const char * text,
-//        int   n_max_tokens,
-//        bool   add_bos){
-//    struct llama_context * ctx = ctx_w->ptr;
-//
-//    py::array_t<llama_token> tokens;
-//    py::buffer_info buf = tokens.request();
-//    llama_token *tokens_ptr = static_cast<llama_token *>(buf.ptr);
-//    llama_tokenize(ctx, text, tokens_ptr, n_max_tokens, add_bos);
-//    return tokens;
-//}
 
 std::string llama_tokens_to_str_wrapper(struct llama_context_wrapper* ctx_w, py::array_t<llama_token> tokens_array) {
     std::string result;
     struct llama_context * ctx = ctx_w->ptr;
     bool all_tokens_valid = true;
 
     for (int i = 0; i < tokens_array.size(); i++) {
@@ -159,48 +189,209 @@
 }
 
 const char * llama_token_to_str_wrapper(struct llama_context_wrapper * ctx_w, llama_token token){
     struct llama_context * ctx = ctx_w->ptr;
     return llama_token_to_str(ctx, token);
 }
 
-llama_token llama_sample_top_p_top_k_wrapper(
-        struct llama_context_wrapper * ctx_w,
-        py::array_t<llama_token> last_n_tokens_data,
-        int   last_n_tokens_size,
-        int   top_k,
-        float   top_p,
-        float   temp,
-        float   repeat_penalty){
-    struct llama_context * ctx = ctx_w->ptr;
-    py::buffer_info buf1 = last_n_tokens_data.request();
-    auto *last_n_tokens_data_ptr = static_cast<llama_token *>(buf1.ptr);
-    return llama_sample_top_p_top_k(ctx, last_n_tokens_data_ptr, last_n_tokens_size, top_k, top_p, temp, repeat_penalty);
+// sampling fcts
+
+void llama_sample_repetition_penalty_wrapper(struct llama_context_wrapper * ctx_w,
+                                     llama_token_data_array * candidates,
+                                     py::array_t<llama_token> last_tokens,
+                                     size_t last_tokens_size,
+                                     float penalty){
+    struct llama_context * ctx = ctx_w->ptr;
+    py::buffer_info buf = last_tokens.request();
+    llama_token *last_tokens_ptr = static_cast<llama_token *>(buf.ptr);
+    llama_sample_repetition_penalty(ctx, candidates, last_tokens_ptr, last_tokens_size, penalty);
+}
+
+void llama_sample_frequency_and_presence_penalties_wrapper(struct llama_context_wrapper * ctx_w,
+                                             llama_token_data_array * candidates,
+                                             py::array_t<llama_token> last_tokens,
+                                             size_t last_tokens_size,
+                                             float alpha_frequency,
+                                             float alpha_presence){
+    struct llama_context * ctx = ctx_w->ptr;
+    py::buffer_info buf = last_tokens.request();
+    llama_token *last_tokens_ptr = static_cast<llama_token *>(buf.ptr);
+    llama_sample_frequency_and_presence_penalties(ctx, candidates, last_tokens_ptr, last_tokens_size, alpha_frequency, alpha_presence);
+}
+
+void llama_sample_softmax_wrapper(struct llama_context_wrapper * ctx_w,
+                                             llama_token_data_array * candidates){
+    struct llama_context * ctx = ctx_w->ptr;
+    llama_sample_softmax(ctx, candidates);
+}
+
+void llama_sample_top_k_wrapper(struct llama_context_wrapper * ctx_w,
+                                llama_token_data_array * candidates,
+                                int k,
+                                size_t min_keep){
+    struct llama_context * ctx = ctx_w->ptr;
+    llama_sample_top_k(ctx, candidates, k, min_keep);
+}
+
+void llama_sample_top_p_wrapper(struct llama_context_wrapper * ctx_w,
+                                llama_token_data_array * candidates,
+                                float p,
+                                size_t min_keep){
+    struct llama_context * ctx = ctx_w->ptr;
+    llama_sample_top_p(ctx, candidates, p, min_keep);
+}
+
+void llama_sample_tail_free_wrapper(struct llama_context_wrapper * ctx_w,
+                                llama_token_data_array * candidates,
+                                float z,
+                                size_t min_keep){
+    struct llama_context * ctx = ctx_w->ptr;
+    llama_sample_tail_free(ctx, candidates, z, min_keep);
+}
+
+void llama_sample_typical_wrapper(struct llama_context_wrapper * ctx_w,
+                                llama_token_data_array * candidates,
+                                float p,
+                                size_t min_keep){
+    struct llama_context * ctx = ctx_w->ptr;
+    llama_sample_typical(ctx, candidates, p, min_keep);
+}
+
+void llama_sample_temperature_wrapper(struct llama_context_wrapper * ctx_w,
+                                llama_token_data_array * candidates,
+                                float temp){
+    struct llama_context * ctx = ctx_w->ptr;
+    llama_sample_temperature(ctx, candidates, temp);
+}
+
+llama_token llama_sample_token_mirostat_wrapper(struct llama_context_wrapper * ctx_w,
+                                llama_token_data_array * candidates,
+                                float tau,
+                                float eta,
+                                int m,
+                                float * mu){
+    struct llama_context * ctx = ctx_w->ptr;
+    return llama_sample_token_mirostat(ctx, candidates, tau, eta, m, mu);
+}
+
+llama_token llama_sample_token_mirostat_v2_wrapper(struct llama_context_wrapper * ctx_w,
+                                llama_token_data_array * candidates,
+                                float tau,
+                                float eta,
+                                float * mu){
+    struct llama_context * ctx = ctx_w->ptr;
+    return llama_sample_token_mirostat_v2(ctx, candidates, tau, eta, mu);
+}
+
+llama_token llama_sample_token_greedy_wrapper(struct llama_context_wrapper * ctx_w,
+                                llama_token_data_array * candidates){
+    struct llama_context * ctx = ctx_w->ptr;
+    return llama_sample_token_greedy(ctx, candidates);
 }
 
+llama_token llama_sample_token_wrapper(struct llama_context_wrapper * ctx_w,
+                                llama_token_data_array * candidates){
+    struct llama_context * ctx = ctx_w->ptr;
+    return llama_sample_token(ctx, candidates);
+}
+
+
 void llama_print_timings_wrapper(struct llama_context_wrapper * ctx_w){
     struct llama_context * ctx = ctx_w->ptr;
     return llama_print_timings(ctx);
 }
 
 void llama_reset_timings_wrapper(struct llama_context_wrapper * ctx_w){
     struct llama_context * ctx = ctx_w->ptr;
     return llama_reset_timings(ctx);
 }
 
-//void _llama_progress_callback(float progress, void *ctx){
-//    struct llama_context_wrapper ctx_w;
-//    ctx_w.ptr = ctx;
-//    // call the python callback
-////    py::gil_scoped_acquire gil;  // Acquire the GIL while in this scope.
-//    py_new_segment_callback(ctx_w, n_new, user_data);
-//};
+llama_token sample_next_token(struct llama_context_wrapper * ctx_w, gpt_params params, std::vector<llama_token> last_n_tokens){
+    // helper function to sample next token (based on the main example)
+    struct llama_context * ctx = ctx_w->ptr;
+    const int n_ctx = llama_n_ctx(ctx);
+    llama_token id = 0;
+
+    const float   temp            = params.temp;
+    const int32_t top_k           = params.top_k <= 0 ? llama_n_vocab(ctx) : params.top_k;
+    const float   top_p           = params.top_p;
+    const float   tfs_z           = params.tfs_z;
+    const float   typical_p       = params.typical_p;
+    const int32_t repeat_last_n   = params.repeat_last_n < 0 ? n_ctx : params.repeat_last_n;
+    const float   repeat_penalty  = params.repeat_penalty;
+    const float   alpha_presence  = params.presence_penalty;
+    const float   alpha_frequency = params.frequency_penalty;
+    const int     mirostat        = params.mirostat;
+    const float   mirostat_tau    = params.mirostat_tau;
+    const float   mirostat_eta    = params.mirostat_eta;
+    const bool    penalize_nl     = params.penalize_nl;
+
+    {
+        auto logits  = llama_get_logits(ctx);
+        auto n_vocab = llama_n_vocab(ctx);
+
+        // Apply params.logit_bias map
+        for (auto it = params.logit_bias.begin(); it != params.logit_bias.end(); it++) {
+            logits[it->first] += it->second;
+        }
+
+        std::vector<llama_token_data> candidates;
+        candidates.reserve(n_vocab);
+        for (llama_token token_id = 0; token_id < n_vocab; token_id++) {
+            candidates.emplace_back(llama_token_data{token_id, logits[token_id], 0.0f});
+        }
+
+        llama_token_data_array candidates_p = { candidates.data(), candidates.size(), false };
+
+        // Apply penalties
+        float nl_logit = logits[llama_token_nl()];
+        auto last_n_repeat = std::min(std::min((int)last_n_tokens.size(), repeat_last_n), n_ctx);
+        llama_sample_repetition_penalty(ctx, &candidates_p,
+                                        last_n_tokens.data() + last_n_tokens.size() - last_n_repeat,
+                                        last_n_repeat, repeat_penalty);
+        llama_sample_frequency_and_presence_penalties(ctx, &candidates_p,
+                                                      last_n_tokens.data() + last_n_tokens.size() - last_n_repeat,
+                                                      last_n_repeat, alpha_frequency, alpha_presence);
+        if (!penalize_nl) {
+            logits[llama_token_nl()] = nl_logit;
+        }
+
+        if (temp <= 0) {
+            // Greedy sampling
+            id = llama_sample_token_greedy(ctx, &candidates_p);
+        } else {
+            if (mirostat == 1) {
+                static float mirostat_mu = 2.0f * mirostat_tau;
+                const int mirostat_m = 100;
+                llama_sample_temperature(ctx, &candidates_p, temp);
+                id = llama_sample_token_mirostat(ctx, &candidates_p, mirostat_tau, mirostat_eta, mirostat_m, &mirostat_mu);
+            } else if (mirostat == 2) {
+                static float mirostat_mu = 2.0f * mirostat_tau;
+                llama_sample_temperature(ctx, &candidates_p, temp);
+                id = llama_sample_token_mirostat_v2(ctx, &candidates_p, mirostat_tau, mirostat_eta, &mirostat_mu);
+            } else {
+                // Temperature sampling
+                llama_sample_top_k(ctx, &candidates_p, top_k, 1);
+                llama_sample_tail_free(ctx, &candidates_p, tfs_z, 1);
+                llama_sample_typical(ctx, &candidates_p, typical_p, 1);
+                llama_sample_top_p(ctx, &candidates_p, top_p, 1);
+                llama_sample_temperature(ctx, &candidates_p, temp);
+                id = llama_sample_token(ctx, &candidates_p);
+            }
+        }
+        // printf("`%d`", candidates_p.size);
+
+//        last_n_tokens.erase(last_n_tokens.begin());
+//        last_n_tokens.push_back(id);
+    }
+
+    return id;
+}
 
 
-////////////////////////
 std::string gpt_random_prompt(std::mt19937 & rng) {
     const int r = rng() % 10;
     switch (r) {
         case 0: return "So";
         case 1: return "Once upon a time";
         case 2: return "When";
         case 3: return "The";
@@ -211,75 +402,36 @@
         case 8: return "She";
         case 9: return "They";
         default: return "To";
     }
 
     return "The";
 }
+static llama_context ** g_ctx;
 
-// quick and dirty implementation! just copied from main.cpp with some minor changes
-// Needs lots of improvements
 int llama_generate(struct llama_context_wrapper * ctx_w, gpt_params params, py::function new_text_callback){
-
-    if (params.perplexity) {
-        printf("\n************\n");
-        printf("%s: please use the 'perplexity' tool for perplexity calculations\n", __func__);
-        printf("************\n\n");
-
-
-        return 0;
-    }
-
-    if (params.embedding) {
-        printf("\n************\n");
-        printf("%s: please use the 'embedding' tool for embedding calculations\n", __func__);
-        printf("************\n\n");
-
-        return 0;
-    }
+    // main example from llama.cpp
+    struct llama_context * ctx = ctx_w->ptr;
+    g_ctx = &ctx;
 
     if (params.n_ctx > 2048) {
         fprintf(stderr, "%s: warning: model does not support context sizes greater than 2048 tokens (%d specified);"
                         "expect poor results\n", __func__, params.n_ctx);
     }
-
-    if (params.seed <= 0) {
+    if (params.seed < 0) {
         params.seed = time(NULL);
     }
 
-    fprintf(stderr, "%s: seed = %d\n", __func__, params.seed);
+    fprintf(stderr, "%s: seed  = %d\n", __func__, params.seed);
 
     std::mt19937 rng(params.seed);
     if (params.random_prompt) {
         params.prompt = gpt_random_prompt(rng);
     }
 
-//    params.prompt = R"(// this function checks if the number n is prime
-//bool is_prime(int n) {)";
-
-    struct llama_context * ctx = ctx_w->ptr;
-
-    // load the model
-//    {
-//        auto lparams = llama_context_default_params();
-//
-//        lparams.n_ctx      = params.n_ctx;
-//        lparams.n_parts    = params.n_parts;
-//        lparams.seed       = params.seed;
-//        lparams.f16_kv     = params.memory_f16;
-//        lparams.use_mlock  = params.use_mlock;
-//
-//        ctx = llama_init_from_file(params.model.c_str(), lparams);
-//
-//        if (ctx == NULL) {
-//            fprintf(stderr, "%s: error: failed to load model '%s'\n", __func__, params.model.c_str());
-//            return 1;
-//        }
-//    }
-
     // print system information
     {
         fprintf(stderr, "\n");
         fprintf(stderr, "system_info: n_threads = %d / %d | %s\n",
                 params.n_threads, std::thread::hardware_concurrency(), llama_print_system_info());
     }
 
@@ -301,46 +453,91 @@
 
         return 0;
     }
 
     // Add a space in front of the first character to match OG llama tokenizer behavior
     params.prompt.insert(0, 1, ' ');
 
+    std::string path_session = params.path_session;
+    std::vector<llama_token> session_tokens;
+
+    if (!path_session.empty()) {
+        fprintf(stderr, "%s: attempting to load saved session from '%s'\n", __func__, path_session.c_str());
+
+        // fopen to check for existing session
+        FILE * fp = std::fopen(path_session.c_str(), "rb");
+        if (fp != NULL) {
+            std::fclose(fp);
+
+            session_tokens.resize(params.n_ctx);
+            size_t n_token_count_out = 0;
+            if (!llama_load_session_file(ctx, path_session.c_str(), session_tokens.data(), session_tokens.capacity(), &n_token_count_out)) {
+                fprintf(stderr, "%s: error: failed to load session file '%s'\n", __func__, path_session.c_str());
+                return 1;
+            }
+            session_tokens.resize(n_token_count_out);
+
+            fprintf(stderr, "%s: loaded a session with prompt size of %d tokens\n", __func__, (int) session_tokens.size());
+        } else {
+            fprintf(stderr, "%s: session file does not exist, will create\n", __func__);
+        }
+    }
+
     // tokenize the prompt
-    auto embd_inp = ::llama_tokenize_wrapper(ctx_w, params.prompt, true);
+    auto embd_inp = llama_tokenize_wrapper(ctx_w, params.prompt, true);
 
     const int n_ctx = llama_n_ctx(ctx);
 
     if ((int) embd_inp.size() > n_ctx - 4) {
         fprintf(stderr, "%s: error: prompt is too long (%d tokens, max %d)\n", __func__, (int) embd_inp.size(), n_ctx - 4);
         return 1;
     }
 
+    // debug message about similarity of saved session, if applicable
+    size_t n_matching_session_tokens = 0;
+    if (session_tokens.size()) {
+        for (llama_token id : session_tokens) {
+            if (n_matching_session_tokens >= embd_inp.size() || id != embd_inp[n_matching_session_tokens]) {
+                break;
+            }
+            n_matching_session_tokens++;
+        }
+        if (n_matching_session_tokens >= embd_inp.size()) {
+            fprintf(stderr, "%s: session file has exact match for prompt!\n", __func__);
+        } else if (n_matching_session_tokens < (embd_inp.size() / 2)) {
+            fprintf(stderr, "%s: warning: session file has low similarity to prompt (%zu / %zu tokens); will mostly be reevaluated\n",
+                    __func__, n_matching_session_tokens, embd_inp.size());
+        } else {
+            fprintf(stderr, "%s: session file matches %zu / %zu tokens of prompt\n",
+                    __func__, n_matching_session_tokens, embd_inp.size());
+        }
+    }
+
     // number of tokens to keep when resetting context
-    if (params.n_keep < 0 || params.n_keep > (int)embd_inp.size() || params.instruct) {
+    if (params.n_keep < 0 || params.n_keep > (int) embd_inp.size() || params.instruct) {
         params.n_keep = (int)embd_inp.size();
     }
 
     // prefix & suffix for instruct mode
-    const auto inp_pfx = ::llama_tokenize_wrapper(ctx_w, "\n\n### Instruction:\n\n", true);
-    const auto inp_sfx = ::llama_tokenize_wrapper(ctx_w, "\n\n### Response:\n\n", false);
+    const auto inp_pfx = llama_tokenize_wrapper(ctx_w, "\n\n### Instruction:\n\n", true);
+    const auto inp_sfx = llama_tokenize_wrapper(ctx_w, "\n\n### Response:\n\n", false);
 
     // in instruct mode, we inject a prefix and a suffix to each input by the user
     if (params.instruct) {
-        params.interactive_start = true;
+        params.interactive_first = true;
         params.antiprompt.push_back("### Instruction:\n\n");
     }
 
     // enable interactive mode if reverse prompt or interactive start is specified
-    if (params.antiprompt.size() != 0 || params.interactive_start) {
+    if (params.antiprompt.size() != 0 || params.interactive_first) {
         params.interactive = true;
     }
 
     // determine newline token
-    auto llama_token_newline = ::llama_tokenize_wrapper(ctx_w, "\n", false);
+    auto llama_token_newline = llama_tokenize_wrapper(ctx_w, "\n", false);
 
     if (params.verbose_prompt) {
         fprintf(stderr, "\n");
         fprintf(stderr, "%s: prompt: '%s'\n", __func__, params.prompt.c_str());
         fprintf(stderr, "%s: number of tokens in prompt = %zu\n", __func__, embd_inp.size());
         for (int i = 0; i < (int) embd_inp.size(); i++) {
             fprintf(stderr, "%6d -> '%s'\n", embd_inp[i], llama_token_to_str(ctx, embd_inp[i]));
@@ -351,260 +548,265 @@
                 fprintf(stderr, "%s", llama_token_to_str(ctx, embd_inp[i]));
             }
             fprintf(stderr, "'\n");
         }
         fprintf(stderr, "\n");
     }
 
-//    if (params.interactive) {
-//#if defined (__unix__) || (defined (__APPLE__) && defined (__MACH__))
-//        struct sigaction sigint_action;
-//        sigint_action.sa_handler = sigint_handler;
-//        sigemptyset (&sigint_action.sa_mask);
-//        sigint_action.sa_flags = 0;
-//        sigaction(SIGINT, &sigint_action, NULL);
-//#elif defined (_WIN32)
-//        signal(SIGINT, sigint_handler);
-//#endif
-//
-//        fprintf(stderr, "%s: interactive mode on.\n", __func__);
-//
-//        if (params.antiprompt.size()) {
-//            for (auto antiprompt : params.antiprompt) {
-//                fprintf(stderr, "Reverse prompt: '%s'\n", antiprompt.c_str());
-//            }
-//        }
-//
-//        if (!params.input_prefix.empty()) {
-//            fprintf(stderr, "Input prefix: '%s'\n", params.input_prefix.c_str());
-//        }
-//    }
-    fprintf(stderr, "sampling: temp = %f, top_k = %d, top_p = %f, repeat_last_n = %i, repeat_penalty = %f\n",
-            params.temp, params.top_k, params.top_p, params.repeat_last_n, params.repeat_penalty);
+    if (params.interactive) {
+
+        fprintf(stderr, "%s: interactive mode on.\n", __func__);
+
+        if (params.antiprompt.size()) {
+            for (auto antiprompt : params.antiprompt) {
+                fprintf(stderr, "Reverse prompt: '%s'\n", antiprompt.c_str());
+            }
+        }
+
+        if (!params.input_prefix.empty()) {
+            fprintf(stderr, "Input prefix: '%s'\n", params.input_prefix.c_str());
+        }
+
+        if (!params.input_suffix.empty()) {
+            fprintf(stderr, "Input suffix: '%s'\n", params.input_suffix.c_str());
+        }
+    }
+
+    fprintf(stderr, "sampling: repeat_last_n = %d, repeat_penalty = %f, presence_penalty = %f, frequency_penalty = %f, top_k = %d, tfs_z = %f, top_p = %f, typical_p = %f, temp = %f, mirostat = %d, mirostat_lr = %f, mirostat_ent = %f\n",
+            params.repeat_last_n, params.repeat_penalty, params.presence_penalty, params.frequency_penalty, params.top_k, params.tfs_z, params.top_p, params.typical_p, params.temp, params.mirostat, params.mirostat_eta, params.mirostat_tau);
     fprintf(stderr, "generate: n_ctx = %d, n_batch = %d, n_predict = %d, n_keep = %d\n", n_ctx, params.n_batch, params.n_predict, params.n_keep);
     fprintf(stderr, "\n\n");
 
     // TODO: replace with ring-buffer
     std::vector<llama_token> last_n_tokens(n_ctx);
     std::fill(last_n_tokens.begin(), last_n_tokens.end(), 0);
 
     if (params.interactive) {
-        fprintf(stderr, "== Running in interactive mode. ==\n"
-                        #if defined (__unix__) || (defined (__APPLE__) && defined (__MACH__)) || defined (_WIN32)
-                        " - Press Ctrl+C to interject at any time.\n"
-                        #endif
-                        " - Press Return to return control to LLaMa.\n"
-                        " - If you want to submit another line, end your input in '\\'.\n\n");
-        is_interacting = params.interactive_start;
+        is_interacting = params.interactive_first;
     }
 
     bool is_antiprompt = false;
-    bool input_noecho  = false;
-
-    int n_past     = 0;
-    int n_remain   = params.n_predict;
-    int n_consumed = 0;
+    bool input_echo    = true;
 
+    // HACK - because session saving incurs a non-negligible delay, for now skip re-saving session
+    // if we loaded a session with at least 75% similarity. It's currently just used to speed up the
+    // initial prompt so it doesn't need to be an exact match.
+    bool need_to_save_session = !path_session.empty() && n_matching_session_tokens < (embd_inp.size() * 3 / 4);
+
+    int n_past             = 0;
+    int n_remain           = params.n_predict;
+    int n_consumed         = 0;
+    int n_session_consumed = 0;
 
     std::vector<llama_token> embd;
 
     while (n_remain != 0 || params.interactive) {
         // predict
         if (embd.size() > 0) {
             // infinite text generation via context swapping
             // if we run out of context:
             // - take the n_keep first tokens from the original prompt (via n_past)
-            // - take half of the last (n_ctx - n_keep) tokens and recompute the logits in a batch
+            // - take half of the last (n_ctx - n_keep) tokens and recompute the logits in batches
             if (n_past + (int) embd.size() > n_ctx) {
                 const int n_left = n_past - params.n_keep;
 
-                n_past = params.n_keep;
+                // always keep the first token - BOS
+                n_past = std::max(1, params.n_keep);
 
                 // insert n_left/2 tokens at the start of embd from last_n_tokens
                 embd.insert(embd.begin(), last_n_tokens.begin() + n_ctx - n_left/2 - embd.size(), last_n_tokens.end() - embd.size());
 
+                // stop saving session if we run out of context
+                path_session = "";
+
                 //printf("\n---\n");
                 //printf("resetting: '");
                 //for (int i = 0; i < (int) embd.size(); i++) {
                 //    printf("%s", llama_token_to_str(ctx, embd[i]));
                 //}
                 //printf("'\n");
                 //printf("\n---\n");
             }
 
-            if (llama_eval(ctx, embd.data(), embd.size(), n_past, params.n_threads)) {
-                fprintf(stderr, "%s : failed to eval\n", __func__);
-                return 1;
+            // try to reuse a matching prefix from the loaded session instead of re-eval (via n_past)
+            if (n_session_consumed < (int) session_tokens.size()) {
+                size_t i = 0;
+                for ( ; i < embd.size(); i++) {
+                    if (embd[i] != session_tokens[n_session_consumed]) {
+                        session_tokens.resize(n_session_consumed);
+                        break;
+                    }
+
+                    n_past++;
+                    n_session_consumed++;
+
+                    if (n_session_consumed >= (int) session_tokens.size()) {
+                        ++i;
+                        break;
+                    }
+                }
+                if (i > 0) {
+                    embd.erase(embd.begin(), embd.begin() + i);
+                }
+            }
+
+            // evaluate tokens in batches
+            // embd is typically prepared beforehand to fit within a batch, but not always
+            for (int i = 0; i < (int) embd.size(); i += params.n_batch) {
+                int n_eval = (int) embd.size() - i;
+                if (n_eval > params.n_batch) {
+                    n_eval = params.n_batch;
+                }
+                if (llama_eval(ctx, &embd[i], n_eval, n_past, params.n_threads)) {
+                    fprintf(stderr, "%s : failed to eval\n", __func__);
+                    return 1;
+                }
+                n_past += n_eval;
+            }
+
+            if (embd.size() > 0 && !path_session.empty()) {
+                session_tokens.insert(session_tokens.end(), embd.begin(), embd.end());
+                n_session_consumed = session_tokens.size();
             }
         }
 
-        n_past += embd.size();
         embd.clear();
 
         if ((int) embd_inp.size() <= n_consumed && !is_interacting) {
             // out of user input, sample next token
-            const int32_t top_k          = params.top_k;
-            const float   top_p          = params.top_p;
-            const float   temp           = params.temp;
-            const float   repeat_penalty = params.repeat_penalty;
+            const float   temp            = params.temp;
+            const int32_t top_k           = params.top_k <= 0 ? llama_n_vocab(ctx) : params.top_k;
+            const float   top_p           = params.top_p;
+            const float   tfs_z           = params.tfs_z;
+            const float   typical_p       = params.typical_p;
+            const int32_t repeat_last_n   = params.repeat_last_n < 0 ? n_ctx : params.repeat_last_n;
+            const float   repeat_penalty  = params.repeat_penalty;
+            const float   alpha_presence  = params.presence_penalty;
+            const float   alpha_frequency = params.frequency_penalty;
+            const int     mirostat        = params.mirostat;
+            const float   mirostat_tau    = params.mirostat_tau;
+            const float   mirostat_eta    = params.mirostat_eta;
+            const bool    penalize_nl     = params.penalize_nl;
+
+            // optionally save the session on first sample (for faster prompt loading next time)
+            if (!path_session.empty() && need_to_save_session) {
+                need_to_save_session = false;
+                llama_save_session_file(ctx, path_session.c_str(), session_tokens.data(), session_tokens.size());
+            }
 
             llama_token id = 0;
 
             {
-                auto logits = llama_get_logits(ctx);
+                auto logits  = llama_get_logits(ctx);
+                auto n_vocab = llama_n_vocab(ctx);
 
-                if (params.ignore_eos) {
-                    logits[llama_token_eos()] = 0;
+                // Apply params.logit_bias map
+                for (auto it = params.logit_bias.begin(); it != params.logit_bias.end(); it++) {
+                    logits[it->first] += it->second;
                 }
 
-                id = llama_sample_top_p_top_k(ctx,
-                                              last_n_tokens.data() + n_ctx - params.repeat_last_n,
-                                              params.repeat_last_n, top_k, top_p, temp, repeat_penalty);
+                std::vector<llama_token_data> candidates;
+                candidates.reserve(n_vocab);
+                for (llama_token token_id = 0; token_id < n_vocab; token_id++) {
+                    candidates.emplace_back(llama_token_data{token_id, logits[token_id], 0.0f});
+                }
+
+                llama_token_data_array candidates_p = { candidates.data(), candidates.size(), false };
+
+                // Apply penalties
+                float nl_logit = logits[llama_token_nl()];
+                auto last_n_repeat = std::min(std::min((int)last_n_tokens.size(), repeat_last_n), n_ctx);
+                llama_sample_repetition_penalty(ctx, &candidates_p,
+                                                last_n_tokens.data() + last_n_tokens.size() - last_n_repeat,
+                                                last_n_repeat, repeat_penalty);
+                llama_sample_frequency_and_presence_penalties(ctx, &candidates_p,
+                                                              last_n_tokens.data() + last_n_tokens.size() - last_n_repeat,
+                                                              last_n_repeat, alpha_frequency, alpha_presence);
+                if (!penalize_nl) {
+                    logits[llama_token_nl()] = nl_logit;
+                }
+
+                if (temp <= 0) {
+                    // Greedy sampling
+                    id = llama_sample_token_greedy(ctx, &candidates_p);
+                } else {
+                    if (mirostat == 1) {
+                        static float mirostat_mu = 2.0f * mirostat_tau;
+                        const int mirostat_m = 100;
+                        llama_sample_temperature(ctx, &candidates_p, temp);
+                        id = llama_sample_token_mirostat(ctx, &candidates_p, mirostat_tau, mirostat_eta, mirostat_m, &mirostat_mu);
+                    } else if (mirostat == 2) {
+                        static float mirostat_mu = 2.0f * mirostat_tau;
+                        llama_sample_temperature(ctx, &candidates_p, temp);
+                        id = llama_sample_token_mirostat_v2(ctx, &candidates_p, mirostat_tau, mirostat_eta, &mirostat_mu);
+                    } else {
+                        // Temperature sampling
+                        llama_sample_top_k(ctx, &candidates_p, top_k, 1);
+                        llama_sample_tail_free(ctx, &candidates_p, tfs_z, 1);
+                        llama_sample_typical(ctx, &candidates_p, typical_p, 1);
+                        llama_sample_top_p(ctx, &candidates_p, top_p, 1);
+                        llama_sample_temperature(ctx, &candidates_p, temp);
+                        id = llama_sample_token(ctx, &candidates_p);
+                    }
+                }
+                // printf("`%d`", candidates_p.size);
 
                 last_n_tokens.erase(last_n_tokens.begin());
                 last_n_tokens.push_back(id);
             }
 
             // replace end of text token with newline token when in interactive mode
             if (id == llama_token_eos() && params.interactive && !params.instruct) {
                 id = llama_token_newline.front();
                 if (params.antiprompt.size() != 0) {
                     // tokenize and inject first reverse prompt
-                    const auto first_antiprompt = ::llama_tokenize_wrapper(ctx_w, params.antiprompt.front(), false);
+                    const auto first_antiprompt = llama_tokenize_wrapper(ctx_w, params.antiprompt.front(), false);
                     embd_inp.insert(embd_inp.end(), first_antiprompt.begin(), first_antiprompt.end());
                 }
             }
 
             // add it to the context
             embd.push_back(id);
 
             // echo this to console
-            input_noecho = false;
+            input_echo = true;
 
             // decrement remaining sampling budget
             --n_remain;
-        }
-        else {
+        } else {
             // some user input remains from prompt or interaction, forward it to processing
             while ((int) embd_inp.size() > n_consumed) {
                 embd.push_back(embd_inp[n_consumed]);
                 last_n_tokens.erase(last_n_tokens.begin());
                 last_n_tokens.push_back(embd_inp[n_consumed]);
                 ++n_consumed;
                 if ((int) embd.size() >= params.n_batch) {
                     break;
                 }
             }
         }
 
         // display text
-        if (!input_noecho) {
+        if (input_echo) {
             for (auto id : embd) {
-//                printf("%s", llama_token_to_str(ctx, id));
-                //@NOTE: model.cpp_generate invokes llama_generate() with a python callback function.
-                //@NOTE: we need to make sure that when the python callback function is called, it gets callback with raw bytes
-                //@NOTE: of generated token, else pybind with implicityl try to decode it to Unicode, and cause UnicodeDecodeError
+                // @NOTE: model.cpp_generate invokes llama_generate() with a python callback function.
+                // @NOTE: we need to make sure that when the python callback function is called, it gets callback with raw bytes
+                // @NOTE: of generated token, else pybind with implicityl try to decode it to Unicode, and cause UnicodeDecodeError
                 std::string tok_str = llama_token_to_str(ctx, id);
                 new_text_callback(py::bytes(tok_str));
-
             }
             fflush(stdout);
         }
         // reset color to default if we there is no pending user input
-//        if (!input_noecho && (int)embd_inp.size() == n_consumed) {
-//            set_console_color(con_st, CONSOLE_COLOR_DEFAULT);
+//        if (input_echo && (int)embd_inp.size() == n_consumed) {
+//            console_set_color(con_st, CONSOLE_COLOR_DEFAULT);
 //        }
 
-        // in interactive mode, and not currently processing queued inputs;
-        // check if we should prompt the user for more
-        if (params.interactive && (int) embd_inp.size() <= n_consumed) {
-
-            // check for reverse prompt
-            if (params.antiprompt.size()) {
-                std::string last_output;
-                for (auto id : last_n_tokens) {
-                    last_output += llama_token_to_str(ctx, id);
-                }
-
-                is_antiprompt = false;
-                // Check if each of the reverse prompts appears at the end of the output.
-                for (std::string & antiprompt : params.antiprompt) {
-                    if (last_output.find(antiprompt.c_str(), last_output.length() - antiprompt.length(), antiprompt.length()) != std::string::npos) {
-                        is_interacting = true;
-                        is_antiprompt = true;
-//                        set_console_color(con_st, CONSOLE_COLOR_USER_INPUT);
-                        fflush(stdout);
-                        break;
-                    }
-                }
-            }
-
-            if (n_past > 0 && is_interacting) {
-                // potentially set color to indicate we are taking user input
-//                set_console_color(con_st, CONSOLE_COLOR_USER_INPUT);
-
-                if (params.instruct) {
-                    printf("\n> ");
-                }
-
-                std::string buffer;
-                if (!params.input_prefix.empty()) {
-                    buffer += params.input_prefix;
-                    printf("%s", buffer.c_str());
-                }
-
-                std::string line;
-                bool another_line = true;
-                do {
-                    if (!std::getline(std::cin, line)) {
-                        // input stream is bad or EOF received
-                        return 0;
-                    }
-                    if (line.empty() || line.back() != '\\') {
-                        another_line = false;
-                    } else {
-                        line.pop_back(); // Remove the continue character
-                    }
-                    buffer += line + '\n'; // Append the line to the result
-                } while (another_line);
-
-                // done taking input, reset color
-//                 set_console_color(con_st, CONSOLE_COLOR_DEFAULT);
-
-                // Add tokens to embd only if the input buffer is non-empty
-                // Entering a empty line lets the user pass control back
-                if (buffer.length() > 1) {
-
-                    // instruct mode: insert instruction prefix
-                    if (params.instruct && !is_antiprompt) {
-                        n_consumed = embd_inp.size();
-                        embd_inp.insert(embd_inp.end(), inp_pfx.begin(), inp_pfx.end());
-                    }
-
-                    auto line_inp = ::llama_tokenize_wrapper(ctx_w, buffer, false);
-                    embd_inp.insert(embd_inp.end(), line_inp.begin(), line_inp.end());
-
-                    // instruct mode: insert response suffix
-                    if (params.instruct) {
-                        embd_inp.insert(embd_inp.end(), inp_sfx.begin(), inp_sfx.end());
-                    }
-
-                    n_remain -= line_inp.size();
-                }
-
-                input_noecho = true; // do not echo this again
-            }
-
-            if (n_past > 0) {
-                is_interacting = false;
-            }
-        }
-
         // end of text token
-        if (embd.back() == llama_token_eos()) {
+        if (!embd.empty() && embd.back() == llama_token_eos()) {
             if (params.instruct) {
                 is_interacting = true;
             } else {
                 fprintf(stderr, " [end of text]\n");
                 break;
             }
         }
@@ -613,101 +815,157 @@
         if (params.interactive && n_remain <= 0 && params.n_predict != -1) {
             n_remain = params.n_predict;
             is_interacting = true;
         }
     }
 
     llama_print_timings(ctx);
-
     return 0;
 }
 
-// gptj
-//class PyLLModel : public LLModel {
-//public:
-//    /* Inherit the constructors */
-//    using LLModel::LLModel;
-//
-//    /* Trampoline (need one for each virtual function) */
-//    bool isModelLoaded() override {
-//        PYBIND11_OVERRIDE_PURE(
-//            bool, /* Return type */
-//            LLModel,      /* Parent class */
-//            isModelLoaded,          /* Name of function in C++ (must match Python name) */
-////            modelPath, fin,     /* Argument(s) */
-//        );
-//    }
-//};
 
 PYBIND11_MODULE(_pyllamacpp, m) {
     m.doc() = R"pbdoc(
-        PyLlamaCpp: Python binding to llama.cpp
+        PyLLaMACpp: Python binding for llama.cpp
         -----------------------
 
         .. currentmodule:: _pyllamacpp
 
         .. autosummary::
            :toctree: _generate
 
     )pbdoc";
 
     py::class_<gpt_params>(m,"gpt_params" /*,py::dynamic_attr()*/)
         .def(py::init<>())
         .def_readwrite("seed", &gpt_params::seed)
         .def_readwrite("n_threads", &gpt_params::n_threads)
         .def_readwrite("n_predict", &gpt_params::n_predict)
-        .def_readwrite("repeat_last_n", &gpt_params::repeat_last_n)
+        .def_readwrite("n_parts", &gpt_params::n_parts)
+        .def_readwrite("n_ctx", &gpt_params::n_ctx)
+        .def_readwrite("n_batch", &gpt_params::n_batch)
+        .def_readwrite("n_keep", &gpt_params::n_keep)
+
+        .def_readwrite("logit_bias", &gpt_params::logit_bias)
         .def_readwrite("top_k", &gpt_params::top_k)
         .def_readwrite("top_p", &gpt_params::top_p)
+        .def_readwrite("tfs_z", &gpt_params::tfs_z)
+        .def_readwrite("typical_p", &gpt_params::typical_p)
         .def_readwrite("temp", &gpt_params::temp)
         .def_readwrite("repeat_penalty", &gpt_params::repeat_penalty)
-        .def_readwrite("n_batch", &gpt_params::n_batch)
-        .def_readwrite("n_keep", &gpt_params::n_keep)
+        .def_readwrite("repeat_last_n", &gpt_params::repeat_last_n)
+        .def_readwrite("frequency_penalty", &gpt_params::frequency_penalty)
+        .def_readwrite("presence_penalty", &gpt_params::presence_penalty)
+        .def_readwrite("mirostat", &gpt_params::mirostat)
+        .def_readwrite("mirostat_tau", &gpt_params::mirostat_tau)
+        .def_readwrite("mirostat_eta", &gpt_params::mirostat_eta)
+
         .def_readwrite("model", &gpt_params::model)
         .def_readwrite("prompt", &gpt_params::prompt)
+        .def_readwrite("path_session", &gpt_params::path_session)
+        .def_readwrite("input_prefix", &gpt_params::input_prefix)
+        .def_readwrite("input_suffix", &gpt_params::input_suffix)
+        .def_readwrite("antiprompt", &gpt_params::antiprompt)
+
+        .def_readwrite("lora_adapter", &gpt_params::lora_adapter)
+        .def_readwrite("lora_base", &gpt_params::lora_base)
+
+        .def_readwrite("memory_f16", &gpt_params::memory_f16)
+        .def_readwrite("random_prompt", &gpt_params::random_prompt)
         .def_readwrite("use_color", &gpt_params::use_color)
         .def_readwrite("interactive", &gpt_params::interactive)
-        .def_readwrite("interactive_start", &gpt_params::interactive_start)
+
+        .def_readwrite("embedding", &gpt_params::embedding)
+        .def_readwrite("interactive_first", &gpt_params::interactive_first)
+        .def_readwrite("multiline_input", &gpt_params::multiline_input)
+
+        .def_readwrite("instruct", &gpt_params::instruct)
+        .def_readwrite("penalize_nl", &gpt_params::penalize_nl)
+        .def_readwrite("perplexity", &gpt_params::perplexity)
+        .def_readwrite("use_mmap", &gpt_params::use_mmap)
+        .def_readwrite("use_mlock", &gpt_params::use_mlock)
+        .def_readwrite("mem_test", &gpt_params::mem_test)
         .def_readwrite("verbose_prompt", &gpt_params::verbose_prompt)
-        .def_readwrite("antiprompt", &gpt_params::antiprompt)
-        .def_readwrite("ignore_eos", &gpt_params::ignore_eos)
-        .def_readwrite("instruct", &gpt_params::instruct);
+        ;
 
     py::class_<llama_context_wrapper>(m,"llama_context");
 
     py::class_<llama_token_data>(m,"llama_token_data")
         .def(py::init<>())
         .def_readwrite("id", &llama_token_data::id)
         .def_readwrite("p", &llama_token_data::p)
-        .def_readwrite("plog", &llama_token_data::plog);
-    
+        .def_readwrite("logit", &llama_token_data::logit);
+
+    PYBIND11_NUMPY_DTYPE(llama_token_data, id, p, logit); // to use llama_tokens in numpy
+    py::class_<llama_token_data_array>(m,"llama_token_data_array")
+        .def(py::init<>())
+        .def_readwrite("size", &llama_token_data_array::size)
+        .def_readwrite("sorted", &llama_token_data_array::sorted)
+        .def_property("data", [](llama_token_data_array &self) {
+            std::vector<llama_token_data> data(self.data, self.data + self.size);
+            for(int i=0; i<self.size; i++){
+                data[i] = self.data[i];
+            }
+            return data;
+        },
+        [](llama_token_data_array &self, py::array_t<llama_token_data> tokens) {
+//            py::buffer_info buf = tokens.request();
+//            llama_token_data *tokens_ptr = static_cast<llama_token_data *>(buf.ptr);
+//            self.data = tokens_ptr;
+        });
+
     py::class_<llama_context_params>(m,"llama_context_params")
         .def(py::init<>())
         .def_readwrite("n_ctx", &llama_context_params::n_ctx)
         .def_readwrite("n_parts", &llama_context_params::n_parts)
         .def_readwrite("seed", &llama_context_params::seed)
         .def_readwrite("f16_kv", &llama_context_params::f16_kv)
         .def_readwrite("logits_all", &llama_context_params::logits_all)
         .def_readwrite("vocab_only", &llama_context_params::vocab_only)
         .def_readwrite("use_mlock", &llama_context_params::use_mlock)
         .def_readwrite("embedding", &llama_context_params::embedding)
         .def_property("progress_callback", [](llama_context_params &self) {},
             [](llama_context_params &self, py::function callback) {
             py_llama_progress_callback = callback;
             self.progress_callback = [](float progress, void *ctx) {
-//                struct llama_context_wrapper ctx_w;
-//                ctx_w->ptr = ctx;
                 py_llama_progress_callback(progress, ctx);
                 };
         })
+
         .def_readwrite("progress_callback_user_data", &llama_context_params::progress_callback_user_data);
+
+    py::enum_<llama_ftype>(m, "llama_ftype")
+    .value("LLAMA_FTYPE_ALL_F32", llama_ftype::LLAMA_FTYPE_ALL_F32)
+    .value("LLAMA_FTYPE_MOSTLY_F16", llama_ftype::LLAMA_FTYPE_MOSTLY_F16)
+    .value("LLAMA_FTYPE_MOSTLY_Q4_0", llama_ftype::LLAMA_FTYPE_MOSTLY_Q4_0)
+    .value("LLAMA_FTYPE_MOSTLY_Q4_1", llama_ftype::LLAMA_FTYPE_MOSTLY_Q4_1)
+    .value("LLAMA_FTYPE_MOSTLY_Q4_1_SOME_F16", llama_ftype::LLAMA_FTYPE_MOSTLY_Q4_1_SOME_F16)
+    .value("LLAMA_FTYPE_MOSTLY_Q8_0", llama_ftype::LLAMA_FTYPE_MOSTLY_Q8_0)
+    .value("LLAMA_FTYPE_MOSTLY_Q5_0", llama_ftype::LLAMA_FTYPE_MOSTLY_Q5_0)
+    .value("LLAMA_FTYPE_MOSTLY_Q5_1", llama_ftype::LLAMA_FTYPE_MOSTLY_Q5_1)
+    .export_values();
+
     m.def("llama_context_default_params", &llama_context_default_params);
+
+    m.def("llama_mmap_supported", &llama_mmap_supported);
+    m.def("llama_mlock_supported", &llama_mlock_supported);
+
+
     m.def("llama_init_from_file", &llama_init_from_file_wrapper);
+
     m.def("llama_free", &llama_free_wrapper);
     m.def("llama_model_quantize", &llama_model_quantize);
+    m.def("llama_apply_lora_from_file", &llama_apply_lora_from_file_wrapper);
+    m.def("llama_get_kv_cache_token_count", &llama_get_kv_cache_token_count_wrapper);
+    m.def("llama_set_rng_seed", &llama_set_rng_seed_wrapper);
+    m.def("llama_get_state_size", &llama_get_state_size_wrapper);
+    m.def("llama_load_session_file", &llama_load_session_file_wrapper);
+    m.def("llama_save_session_file", &llama_save_session_file_wrapper);
+
+    m.def("llama_model_quantize", &llama_model_quantize);
     m.def("llama_eval", &llama_eval_wrapper);
     m.def("llama_tokenize", &llama_tokenize_wrapper);
     m.def("llama_n_vocab", &llama_n_vocab_wrapper);
     m.def("llama_n_ctx", &llama_n_ctx_wrapper);
     m.def("llama_n_embd", &llama_n_embd_wrapper);
     m.def("llama_get_logits", &llama_get_logits_wrapper);
     m.def("llama_get_embeddings", &llama_get_embeddings_wrapper);
@@ -718,37 +976,39 @@
         return py::bytes(llama_token_to_str_wrapper(ctx_w, token));
     });
     m.def("llama_tokens_to_str", &llama_tokens_to_str_wrapper);
 
 
     m.def("llama_token_bos", &llama_token_bos);
     m.def("llama_token_eos", &llama_token_eos);
+    m.def("llama_token_nl", &llama_token_nl);
 
-    m.def("llama_sample_top_p_top_k", &llama_sample_top_p_top_k_wrapper);
+    // sampling fcts
+    m.def("llama_sample_repetition_penalty", &llama_sample_repetition_penalty_wrapper);
+    m.def("llama_sample_frequency_and_presence_penalties", &llama_sample_frequency_and_presence_penalties_wrapper);
+    m.def("llama_sample_softmax", &llama_sample_softmax_wrapper);
+    m.def("llama_sample_top_k", &llama_sample_top_k_wrapper);
+    m.def("llama_sample_top_p", &llama_sample_top_p_wrapper);
+    m.def("llama_sample_tail_free", &llama_sample_tail_free_wrapper);
+    m.def("llama_sample_typical", &llama_sample_typical_wrapper);
+    m.def("llama_sample_temperature", &llama_sample_temperature_wrapper);
+    m.def("llama_sample_token_mirostat", &llama_sample_token_mirostat_wrapper);
+    m.def("llama_sample_token_mirostat_v2", &llama_sample_token_mirostat_v2_wrapper);
+    m.def("llama_sample_token_greedy", &llama_sample_token_greedy_wrapper);
+    m.def("llama_sample_token", &llama_sample_token_wrapper);
+
+    m.def("sample_next_token", &sample_next_token); // helper function / not part of the llama.h API
 
     m.def("llama_print_timings", &llama_print_timings_wrapper);
     m.def("llama_reset_timings", &llama_reset_timings_wrapper);
 
     m.def("llama_print_system_info", &llama_print_system_info);
 
     m.def("llama_generate", &llama_generate);
 
-    //////////////////////////////////////////////
-    // gptj
-//    py::class_<LLModel>(m, "LLModel")
-////      .def(py::init([]() { return new LLModel(); } /* no alias needed */,
-////        .def("loadModel", &LLModel::loadModel)
-////        .def("isModelLoaded", &LLModel::isModelLoaded)
-//        .def_readwrite("PromptContext", &LLModel::PromptContext)
-//        ;
-//     py::class_<LLModel, PyLLModel /* <--- trampoline*/>(m, "LLModel")
-//        .def(py::init<>())
-//        .def("loadModel", &LLModel::loadModel);
-
-
 
 #ifdef VERSION_INFO
     m.attr("__version__") = MACRO_STRINGIFY(VERSION_INFO);
 #else
     m.attr("__version__") = "dev";
 #endif
 }
```

### Comparing `pyllamacpp-2.1.3/src/main.h` & `pyllamacpp-2.2.0/src/main.h`

 * *Files 26% similar despite different names*

```diff
@@ -15,45 +15,58 @@
 #include <vector>
 #include <random>
 #include <thread>
 
 struct gpt_params {
     int32_t seed          = -1;   // RNG seed
     int32_t n_threads     = std::min(4, (int32_t) std::thread::hardware_concurrency());
-    int32_t n_predict     = 128;  // new tokens to predict
-    int32_t repeat_last_n = 64;   // last n tokens to penalize
+    int32_t n_predict     = -1;  // new tokens to predict
     int32_t n_parts       = -1;   // amount of model parts (-1 = determine from model dimensions)
     int32_t n_ctx         = 512;  // context size
-    int32_t n_batch       = 8;    // batch size for prompt processing
+    int32_t n_batch       = 512;  // batch size for prompt processing (must be >=32 to use BLAS)
     int32_t n_keep        = 0;    // number of tokens to keep from initial prompt
 
     // sampling parameters
-    int32_t top_k = 40;
-    float   top_p = 0.95f;
-    float   temp  = 0.80f;
-    float   repeat_penalty  = 1.10f;
+    std::unordered_map<llama_token, float> logit_bias; // logit bias for specific tokens
+    int32_t top_k             = 40;    // <= 0 to use vocab size
+    float   top_p             = 0.95f; // 1.0 = disabled
+    float   tfs_z             = 1.00f; // 1.0 = disabled
+    float   typical_p         = 1.00f; // 1.0 = disabled
+    float   temp              = 0.80f; // 1.0 = disabled
+    float   repeat_penalty    = 1.10f; // 1.0 = disabled
+    int32_t repeat_last_n     = 64;    // last n tokens to penalize (0 = disable penalty, -1 = context size)
+    float   frequency_penalty = 0.00f; // 0.0 = disabled
+    float   presence_penalty  = 0.00f; // 0.0 = disabled
+    int     mirostat          = 0;     // 0 = disabled, 1 = mirostat, 2 = mirostat 2.0
+    float   mirostat_tau      = 5.00f; // target entropy
+    float   mirostat_eta      = 0.10f; // learning rate
 
     std::string model  = "models/lamma-7B/ggml-model.bin"; // model path
     std::string prompt = "";
-    std::string input_prefix = ""; // string to prefix user inputs with
-
-
+    std::string path_session = "";       // path to file for saving/loading model eval state
+    std::string input_prefix = "";       // string to prefix user inputs with
+    std::string input_suffix = "";       // string to suffix user inputs with
     std::vector<std::string> antiprompt; // string upon seeing which more user input is prompted
 
+    std::string lora_adapter = "";  // lora adapter path
+    std::string lora_base = "";     // base model path for the lora adapter
+
     bool memory_f16        = true;  // use f16 instead of f32 for memory kv
     bool random_prompt     = false; // do not randomize prompt if none provided
     bool use_color         = false; // use color to distinguish generations and inputs
     bool interactive       = false; // interactive mode
 
     bool embedding         = false; // get only sentence embedding
-    bool interactive_start = false; // wait for user input immediately
+    bool interactive_first = false; // wait for user input immediately
+    bool multiline_input   = false; // reverse the usage of `\`
 
     bool instruct          = false; // instruction mode (used for Alpaca models)
-    bool ignore_eos        = false; // do not stop generating after eos
+    bool penalize_nl       = true;  // consider newlines as a repeatable token
     bool perplexity        = false; // compute perplexity over the prompt
+    bool use_mmap          = true;  // use mmap for faster loads
     bool use_mlock         = false; // use mlock to keep model in memory
     bool mem_test          = false; // compute maximum memory usage
     bool verbose_prompt    = false; // print prompt tokens before generation
 };
 
 
 #define ANSI_COLOR_RED     "\x1b[31m"
```

