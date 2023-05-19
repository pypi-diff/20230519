# Comparing `tmp/scargo-1.4.0.tar.gz` & `tmp/scargo-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scargo-1.4.0.tar", last modified: Tue May  9 10:25:23 2023, max compression
+gzip compressed data, was "scargo-1.5.0.tar", last modified: Fri May 19 06:46:32 2023, max compression
```

## Comparing `scargo-1.4.0.tar` & `scargo-1.5.0.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0        0        0     4508 2023-05-09 10:25:17.600083 scargo-1.4.0/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0     1066 2023-05-09 10:25:17.600083 scargo-1.4.0/LICENSE
--rw-r--r--   0        0        0     2488 2023-05-09 10:25:17.600083 scargo-1.4.0/README.md
--rw-r--r--   0        0        0     2748 2023-05-09 10:25:17.720082 scargo-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      108 2023-05-09 10:25:17.720082 scargo-1.4.0/scargo/__init__.py
--rwxr-xr-x   0        0        0    19839 2023-05-09 10:25:17.720082 scargo-1.4.0/scargo/certs/certGen.sh
--rwxr-xr-x   0        0        0     4914 2023-05-09 10:25:17.720082 scargo-1.4.0/scargo/certs/generateAllCertificates.sh
--rw-r--r--   0        0        0     3967 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/certs/openssl_device_intermediate_ca.cnf
--rw-r--r--   0        0        0     3957 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/certs/openssl_root_ca.cnf
--rw-r--r--   0        0        0      698 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/clang_utils.py
--rw-r--r--   0        0        0    12706 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/cli.py
--rw-r--r--   0        0        0       86 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/__init__.py
--rw-r--r--   0        0        0     1738 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/build.py
--rw-r--r--   0        0        0    12212 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/check.py
--rw-r--r--   0        0        0     1142 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/clean.py
--rw-r--r--   0        0        0     4343 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/debug.py
--rw-r--r--   0        0        0     3402 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/doc.py
--rw-r--r--   0        0        0     3369 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/docker.py
--rw-r--r--   0        0        0     1124 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/fix.py
--rw-r--r--   0        0        0     3927 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/flash.py
--rw-r--r--   0        0        0     6677 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/gen.py
--rw-r--r--   0        0        0     2857 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/new.py
--rw-r--r--   0        0        0     3405 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/publish.py
--rw-r--r--   0        0        0     1688 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/run.py
--rw-r--r--   0        0        0     3347 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/test.py
--rw-r--r--   0        0        0     4419 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/update.py
--rw-r--r--   0        0        0      228 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/version.py
--rw-r--r--   0        0        0     6707 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/config.py
--rw-r--r--   0        0        0     2255 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/config_utils.py
--rw-r--r--   0        0        0     2174 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/docker_utils.py
--rw-r--r--   0        0        0       86 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/__init__.py
--rw-r--r--   0        0        0     1658 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/base_gen.py
--rw-r--r--   0        0        0      441 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/cicd_gen.py
--rw-r--r--   0        0        0       86 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/clang_parser/__init__.py
--rw-r--r--   0        0        0     2251 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/clang_parser/data_classes.py
--rw-r--r--   0        0        0     1197 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/clang_parser/header_parser.py
--rw-r--r--   0        0        0     2348 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/clang_parser/params_extractor.py
--rw-r--r--   0        0        0      395 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/cmake_gen.py
--rw-r--r--   0        0        0      569 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/conan_gen.py
--rw-r--r--   0        0        0     2468 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/cpp_gen.py
--rw-r--r--   0        0        0     3186 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/docker_gen.py
--rw-r--r--   0        0        0     1115 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/env_gen.py
--rwxr-xr-x   0        0        0     1607 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/mock_gen.py
--rw-r--r--   0        0        0      454 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/readme_gen.py
--rw-r--r--   0        0        0     4834 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/.gitlab-ci.yml.j2
--rw-r--r--   0        0        0     1580 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/CMakeLists.txt.j2
--rw-r--r--   0        0        0     4275 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/README.md.j2
--rw-r--r--   0        0        0     1693 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/conan/conanfile.py.j2
--rw-r--r--   0        0        0     1464 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/conan/conanfiletest.j2
--rw-r--r--   0        0        0      150 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/cpp/cmake-src-esp32.j2
--rw-r--r--   0        0        0     2423 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/cpp/cmake-src-stm32.j2
--rw-r--r--   0        0        0      886 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/cpp/cmake-src-x86.j2
--rw-r--r--   0        0        0      181 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/cpp/lib.cpp.j2
--rw-r--r--   0        0        0      213 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/cpp/lib.h.j2
--rw-r--r--   0        0        0      715 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/cpp/main.cpp.j2
--rw-r--r--   0        0        0      159 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/docker/Dockerfile-custom.j2
--rw-r--r--   0        0        0     2067 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/docker/Dockerfile-esp32.j2
--rw-r--r--   0        0        0      754 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/docker/Dockerfile-stm32.j2
--rw-r--r--   0        0        0       49 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/docker/Dockerfile-x86.j2
--rw-r--r--   0        0        0     2359 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/docker/Dockerfile.j2
--rw-r--r--   0        0        0      158 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/docker/devcontainer.json.j2
--rw-r--r--   0        0        0     1000 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/docker/docker-compose.yaml.j2
--rw-r--r--   0        0        0      287 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/docker/env.txt.j2
--rw-r--r--   0        0        0       22 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/docker/stm32.cfg.j2
--rw-r--r--   0        0        0      294 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/esp32.cmake.j2
--rw-r--r--   0        0        0       39 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/mock/.clang-format
--rw-r--r--   0        0        0      475 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/mock/CMakeLists.txt
--rw-r--r--   0        0        0      594 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/mock/class_interface.h.j2
--rw-r--r--   0        0        0      835 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/mock/class_mock.cpp.j2
--rw-r--r--   0        0        0      697 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/mock/class_mock.h.j2
--rw-r--r--   0        0        0      510 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/project.cmake.j2
--rw-r--r--   0        0        0     2228 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/scargo.toml.j2
--rw-r--r--   0        0        0      802 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/stm32.cmake.j2
--rw-r--r--   0        0        0       91 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/tests/CMakeLists-it.txt.j2
--rw-r--r--   0        0        0      100 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/tests/CMakeLists-mocks.txt.j2
--rw-r--r--   0        0        0     1079 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2
--rw-r--r--   0        0        0       84 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/tests/CMakeLists-ut.txt.j2
--rw-r--r--   0        0        0      326 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/tests/static_mock/CMakeLists.txt
--rw-r--r--   0        0        0     1046 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/tests/static_mock/static_mock.h
--rw-r--r--   0        0        0       39 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/ut/.clang-format
--rw-r--r--   0        0        0      575 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/ut/CMakeLists.txt.j2
--rw-r--r--   0        0        0      719 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/ut/ut.cpp.j2
--rw-r--r--   0        0        0      213 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/x86.cmake.j2
--rw-r--r--   0        0        0     1597 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/tests_gen.py
--rw-r--r--   0        0        0      550 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/toml_gen.py
--rw-r--r--   0        0        0     5357 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/ut_gen.py
--rw-r--r--   0        0        0      629 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/global_values.py
--rw-r--r--   0        0        0     2044 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/logger.py
--rw-r--r--   0        0        0     1137 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/path_utils.py
--rw-r--r--   0        0        0     2953 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/templates/.clang-format
--rw-r--r--   0        0        0     8780 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/templates/.clang-tidy
--rw-r--r--   0        0        0     2361 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/templates/.gitignore
--rw-r--r--   0        0        0     1066 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/templates/LICENSE
--rw-r--r--   0        0        0      519 2023-05-09 10:25:17.724082 scargo-1.4.0/setup.cfg
--rw-r--r--   0        0        0     5229 1970-01-01 00:00:00.000000 scargo-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     4508 2023-05-19 06:46:27.278807 scargo-1.5.0/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0     1066 2023-05-19 06:46:27.278807 scargo-1.5.0/LICENSE
+-rw-r--r--   0        0        0     2488 2023-05-19 06:46:27.278807 scargo-1.5.0/README.md
+-rw-r--r--   0        0        0     2748 2023-05-19 06:46:27.406804 scargo-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/__init__.py
+-rwxr-xr-x   0        0        0    19734 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/certs/certGen.sh
+-rwxr-xr-x   0        0        0     5226 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/certs/generateAllCertificates.sh
+-rw-r--r--   0        0        0     3967 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/certs/openssl_device_intermediate_ca.cnf
+-rw-r--r--   0        0        0     3957 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/certs/openssl_root_ca.cnf
+-rw-r--r--   0        0        0      698 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/clang_utils.py
+-rw-r--r--   0        0        0    12706 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/cli.py
+-rw-r--r--   0        0        0       86 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/__init__.py
+-rw-r--r--   0        0        0     1738 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/build.py
+-rw-r--r--   0        0        0    12212 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/check.py
+-rw-r--r--   0        0        0     1142 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/clean.py
+-rw-r--r--   0        0        0     4343 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/debug.py
+-rw-r--r--   0        0        0     3402 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/doc.py
+-rw-r--r--   0        0        0     3369 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/docker.py
+-rw-r--r--   0        0        0     1124 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/fix.py
+-rw-r--r--   0        0        0     3927 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/flash.py
+-rw-r--r--   0        0        0     6677 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/gen.py
+-rw-r--r--   0        0        0     2857 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/new.py
+-rw-r--r--   0        0        0     3405 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/publish.py
+-rw-r--r--   0        0        0     1688 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/run.py
+-rw-r--r--   0        0        0     3347 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/test.py
+-rw-r--r--   0        0        0     4419 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/update.py
+-rw-r--r--   0        0        0      228 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/version.py
+-rw-r--r--   0        0        0     6707 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/config.py
+-rw-r--r--   0        0        0     2255 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/config_utils.py
+-rw-r--r--   0        0        0     2174 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/docker_utils.py
+-rw-r--r--   0        0        0       86 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/__init__.py
+-rw-r--r--   0        0        0     1658 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/base_gen.py
+-rw-r--r--   0        0        0      441 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/cicd_gen.py
+-rw-r--r--   0        0        0       86 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/clang_parser/__init__.py
+-rw-r--r--   0        0        0     2251 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/clang_parser/data_classes.py
+-rw-r--r--   0        0        0     1197 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/clang_parser/header_parser.py
+-rw-r--r--   0        0        0     2348 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/clang_parser/params_extractor.py
+-rw-r--r--   0        0        0      395 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/cmake_gen.py
+-rw-r--r--   0        0        0      569 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/conan_gen.py
+-rw-r--r--   0        0        0     2468 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/cpp_gen.py
+-rw-r--r--   0        0        0     3186 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/docker_gen.py
+-rw-r--r--   0        0        0     1115 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/env_gen.py
+-rwxr-xr-x   0        0        0     1607 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/mock_gen.py
+-rw-r--r--   0        0        0      454 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/readme_gen.py
+-rw-r--r--   0        0        0     4834 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/.gitlab-ci.yml.j2
+-rw-r--r--   0        0        0     1580 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/CMakeLists.txt.j2
+-rw-r--r--   0        0        0     4275 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/README.md.j2
+-rw-r--r--   0        0        0     1693 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/conan/conanfile.py.j2
+-rw-r--r--   0        0        0     1464 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/conan/conanfiletest.j2
+-rw-r--r--   0        0        0      150 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/cpp/cmake-src-esp32.j2
+-rw-r--r--   0        0        0     2423 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/cpp/cmake-src-stm32.j2
+-rw-r--r--   0        0        0      886 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/cpp/cmake-src-x86.j2
+-rw-r--r--   0        0        0      181 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/cpp/lib.cpp.j2
+-rw-r--r--   0        0        0      213 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/cpp/lib.h.j2
+-rw-r--r--   0        0        0      715 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/cpp/main.cpp.j2
+-rw-r--r--   0        0        0      159 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/docker/Dockerfile-custom.j2
+-rw-r--r--   0        0        0     2067 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/docker/Dockerfile-esp32.j2
+-rw-r--r--   0        0        0      754 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/docker/Dockerfile-stm32.j2
+-rw-r--r--   0        0        0       49 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/docker/Dockerfile-x86.j2
+-rw-r--r--   0        0        0     2359 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/docker/Dockerfile.j2
+-rw-r--r--   0        0        0      158 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/docker/devcontainer.json.j2
+-rw-r--r--   0        0        0     1000 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/docker/docker-compose.yaml.j2
+-rw-r--r--   0        0        0      287 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/docker/env.txt.j2
+-rw-r--r--   0        0        0       22 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/docker/stm32.cfg.j2
+-rw-r--r--   0        0        0      294 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/esp32.cmake.j2
+-rw-r--r--   0        0        0       39 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/mock/.clang-format
+-rw-r--r--   0        0        0      475 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/mock/CMakeLists.txt
+-rw-r--r--   0        0        0      594 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/mock/class_interface.h.j2
+-rw-r--r--   0        0        0      835 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/mock/class_mock.cpp.j2
+-rw-r--r--   0        0        0      697 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/mock/class_mock.h.j2
+-rw-r--r--   0        0        0      510 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/project.cmake.j2
+-rw-r--r--   0        0        0     2228 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/scargo.toml.j2
+-rw-r--r--   0        0        0      802 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/stm32.cmake.j2
+-rw-r--r--   0        0        0       91 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/tests/CMakeLists-it.txt.j2
+-rw-r--r--   0        0        0      100 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/tests/CMakeLists-mocks.txt.j2
+-rw-r--r--   0        0        0     1079 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2
+-rw-r--r--   0        0        0       84 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/tests/CMakeLists-ut.txt.j2
+-rw-r--r--   0        0        0      326 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/tests/static_mock/CMakeLists.txt
+-rw-r--r--   0        0        0     1046 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/tests/static_mock/static_mock.h
+-rw-r--r--   0        0        0       39 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/ut/.clang-format
+-rw-r--r--   0        0        0      575 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/ut/CMakeLists.txt.j2
+-rw-r--r--   0        0        0      719 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/ut/ut.cpp.j2
+-rw-r--r--   0        0        0      213 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/x86.cmake.j2
+-rw-r--r--   0        0        0     1597 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/tests_gen.py
+-rw-r--r--   0        0        0      550 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/toml_gen.py
+-rw-r--r--   0        0        0     5357 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/ut_gen.py
+-rw-r--r--   0        0        0      629 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/global_values.py
+-rw-r--r--   0        0        0     2044 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/logger.py
+-rw-r--r--   0        0        0     1137 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/path_utils.py
+-rw-r--r--   0        0        0     2953 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/templates/.clang-format
+-rw-r--r--   0        0        0     8780 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/templates/.clang-tidy
+-rw-r--r--   0        0        0     2361 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/templates/.gitignore
+-rw-r--r--   0        0        0     1066 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/templates/LICENSE
+-rw-r--r--   0        0        0      519 2023-05-19 06:46:27.410804 scargo-1.5.0/setup.cfg
+-rw-r--r--   0        0        0     5229 1970-01-01 00:00:00.000000 scargo-1.5.0/PKG-INFO
```

### Comparing `scargo-1.4.0/CODE-OF-CONDUCT.md` & `scargo-1.5.0/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/LICENSE` & `scargo-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/README.md` & `scargo-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/pyproject.toml` & `scargo-1.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/certs/certGen.sh` & `scargo-1.5.0/scargo/certs/certGen.sh`

 * *Files 1% similar despite different names*

```diff
@@ -109,21 +109,18 @@
     case $OSTYPE in win32) result="/${result}"
     esac
     echo "$result"
 }
 
 function warn_certs_not_for_production()
 {
-    [ ! -z "$TERM" ] && tput smso
-    [ ! -z "$TERM" ] && tput setaf 3
     echo "Certs generated by this script are not for production (e.g. they have hard-coded passwords of '1234'."
     echo "This script is only to help you understand Azure IoT Hub CA Certificates."
     echo "Use your official, secure mechanisms for this cert generation."
     echo "Also note that these certs will expire in ${days_till_expire} days."
-    [ ! -z "$TERM" ] && tput sgr0
 }
 
 function generate_root_ca()
 {
     local common_name="Azure IoT Hub CA Cert Test Only"
     local password_cmd=" -aes256 -passout pass:${root_ca_password} "
```

### Comparing `scargo-1.4.0/scargo/certs/generateAllCertificates.sh` & `scargo-1.5.0/scargo/certs/generateAllCertificates.sh`

 * *Files 4% similar despite different names*

```diff
@@ -93,20 +93,30 @@
 
 rm -f ${OUTPUT_DIR}/ca.pem
 
 if [ -f "$BALTIMORE_CERT" ]; then
     echo "$BALTIMORE_CERT already exists."
 else
     wget https://cacerts.digicert.com/BaltimoreCyberTrustRoot.crt.pem -O ${OUTPUT_DIR}/baltimore.pem
+    if [ $? -ne 0 ]; then
+        echo -e "${RED} Failed to download Baltimore certificate" >&2
+        rm ${OUTPUT_DIR}/baltimore.pem
+        exit 1
+    fi
 fi
 
 if [ -f "$DIGIROOT_CERT" ]; then
     echo "$DIGIROOT_CERT already exists."
 else
     wget https://cacerts.digicert.com/DigiCertGlobalRootG2.crt.pem -O ${OUTPUT_DIR}/digiroot.pem
+    if [ $? -ne 0 ]; then
+        echo -e "${RED} Failed to download Digiroot certificate" >&2
+        rm ${OUTPUT_DIR}/digiroot.pem
+        exit 1
+    fi
 fi
 
 cat ${OUTPUT_DIR}/baltimore.pem >> ${OUTPUT_DIR}/ca_temp.pem
 cat ${OUTPUT_DIR}/digiroot.pem >> ${OUTPUT_DIR}/ca_temp.pem
 grep . ${OUTPUT_DIR}/ca_temp.pem > ${OUTPUT_DIR}/ca.pem
 rm -f ${OUTPUT_DIR}/ca_temp.pem
```

### Comparing `scargo-1.4.0/scargo/certs/openssl_device_intermediate_ca.cnf` & `scargo-1.5.0/scargo/certs/openssl_device_intermediate_ca.cnf`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/certs/openssl_root_ca.cnf` & `scargo-1.5.0/scargo/certs/openssl_root_ca.cnf`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/clang_utils.py` & `scargo-1.5.0/scargo/clang_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/cli.py` & `scargo-1.5.0/scargo/cli.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/commands/build.py` & `scargo-1.5.0/scargo/commands/build.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/commands/check.py` & `scargo-1.5.0/scargo/commands/check.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/commands/clean.py` & `scargo-1.5.0/scargo/commands/clean.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/commands/debug.py` & `scargo-1.5.0/scargo/commands/debug.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/commands/doc.py` & `scargo-1.5.0/scargo/commands/doc.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/commands/docker.py` & `scargo-1.5.0/scargo/commands/docker.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/commands/fix.py` & `scargo-1.5.0/scargo/commands/fix.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/commands/flash.py` & `scargo-1.5.0/scargo/commands/flash.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/commands/gen.py` & `scargo-1.5.0/scargo/commands/gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/commands/new.py` & `scargo-1.5.0/scargo/commands/new.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/commands/publish.py` & `scargo-1.5.0/scargo/commands/publish.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/commands/run.py` & `scargo-1.5.0/scargo/commands/run.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/commands/test.py` & `scargo-1.5.0/scargo/commands/test.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/commands/update.py` & `scargo-1.5.0/scargo/commands/update.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/config.py` & `scargo-1.5.0/scargo/config.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/config_utils.py` & `scargo-1.5.0/scargo/config_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/docker_utils.py` & `scargo-1.5.0/scargo/docker_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/base_gen.py` & `scargo-1.5.0/scargo/file_generators/base_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/clang_parser/data_classes.py` & `scargo-1.5.0/scargo/file_generators/clang_parser/data_classes.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/clang_parser/header_parser.py` & `scargo-1.5.0/scargo/file_generators/clang_parser/header_parser.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/clang_parser/params_extractor.py` & `scargo-1.5.0/scargo/file_generators/clang_parser/params_extractor.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/conan_gen.py` & `scargo-1.5.0/scargo/file_generators/conan_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/cpp_gen.py` & `scargo-1.5.0/scargo/file_generators/cpp_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/docker_gen.py` & `scargo-1.5.0/scargo/file_generators/docker_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/env_gen.py` & `scargo-1.5.0/scargo/file_generators/env_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/mock_gen.py` & `scargo-1.5.0/scargo/file_generators/mock_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/templates/.gitlab-ci.yml.j2` & `scargo-1.5.0/scargo/file_generators/templates/.gitlab-ci.yml.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/templates/CMakeLists.txt.j2` & `scargo-1.5.0/scargo/file_generators/templates/CMakeLists.txt.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/templates/README.md.j2` & `scargo-1.5.0/scargo/file_generators/templates/README.md.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/templates/conan/conanfile.py.j2` & `scargo-1.5.0/scargo/file_generators/templates/conan/conanfile.py.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/templates/conan/conanfiletest.j2` & `scargo-1.5.0/scargo/file_generators/templates/conan/conanfiletest.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/templates/cpp/cmake-src-stm32.j2` & `scargo-1.5.0/scargo/file_generators/templates/cpp/cmake-src-stm32.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/templates/cpp/cmake-src-x86.j2` & `scargo-1.5.0/scargo/file_generators/templates/cpp/cmake-src-x86.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/templates/cpp/main.cpp.j2` & `scargo-1.5.0/scargo/file_generators/templates/cpp/main.cpp.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/templates/docker/Dockerfile-esp32.j2` & `scargo-1.5.0/scargo/file_generators/templates/docker/Dockerfile-esp32.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/templates/docker/Dockerfile-stm32.j2` & `scargo-1.5.0/scargo/file_generators/templates/docker/Dockerfile-stm32.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/templates/docker/Dockerfile.j2` & `scargo-1.5.0/scargo/file_generators/templates/docker/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/templates/docker/docker-compose.yaml.j2` & `scargo-1.5.0/scargo/file_generators/templates/docker/docker-compose.yaml.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/templates/mock/class_interface.h.j2` & `scargo-1.5.0/scargo/file_generators/templates/mock/class_interface.h.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/templates/mock/class_mock.cpp.j2` & `scargo-1.5.0/scargo/file_generators/templates/mock/class_mock.cpp.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/templates/mock/class_mock.h.j2` & `scargo-1.5.0/scargo/file_generators/templates/mock/class_mock.h.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/templates/scargo.toml.j2` & `scargo-1.5.0/scargo/file_generators/templates/scargo.toml.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/templates/stm32.cmake.j2` & `scargo-1.5.0/scargo/file_generators/templates/stm32.cmake.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2` & `scargo-1.5.0/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/templates/tests/static_mock/static_mock.h` & `scargo-1.5.0/scargo/file_generators/templates/tests/static_mock/static_mock.h`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/templates/ut/CMakeLists.txt.j2` & `scargo-1.5.0/scargo/file_generators/templates/ut/CMakeLists.txt.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/templates/ut/ut.cpp.j2` & `scargo-1.5.0/scargo/file_generators/templates/ut/ut.cpp.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/tests_gen.py` & `scargo-1.5.0/scargo/file_generators/tests_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/toml_gen.py` & `scargo-1.5.0/scargo/file_generators/toml_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/file_generators/ut_gen.py` & `scargo-1.5.0/scargo/file_generators/ut_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/global_values.py` & `scargo-1.5.0/scargo/global_values.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/logger.py` & `scargo-1.5.0/scargo/logger.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/path_utils.py` & `scargo-1.5.0/scargo/path_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/templates/.clang-format` & `scargo-1.5.0/scargo/templates/.clang-format`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/templates/.clang-tidy` & `scargo-1.5.0/scargo/templates/.clang-tidy`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/templates/.gitignore` & `scargo-1.5.0/scargo/templates/.gitignore`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/scargo/templates/LICENSE` & `scargo-1.5.0/scargo/templates/LICENSE`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/setup.cfg` & `scargo-1.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `scargo-1.4.0/PKG-INFO` & `scargo-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scargo
-Version: 1.4.0
+Version: 1.5.0
 Summary: C/C++ package and software development life cycle manager inspired by RUST cargo idea.
 Keywords: scargo,Package manager,C++
 Author-email: "Spyrosoft Solutions S.A." <aak@spyro-soft.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

