# Comparing `tmp/dan-build-0.2.1.tar.gz` & `tmp/dan-build-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dan-build-0.2.1.tar", last modified: Thu May 18 18:41:29 2023, max compression
+gzip compressed data, was "dan-build-0.2.2.tar", last modified: Fri May 19 06:38:37 2023, max compression
```

## Comparing `dan-build-0.2.1.tar` & `dan-build-0.2.2.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.241839 dan-build-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-18 18:41:19.000000 dan-build-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-05-18 18:41:29.241839 dan-build-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-05-18 18:41:19.000000 dan-build-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.233839 dan-build-0.2.1/completion/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.233839 dan-build-0.2.1/completion/bash/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-18 18:41:19.000000 dan-build-0.2.1/completion/bash/dan-io.sh
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-18 18:41:19.000000 dan-build-0.2.1/completion/bash/dan.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.233839 dan-build-0.2.1/completion/zsh/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-18 18:41:19.000000 dan-build-0.2.1/completion/zsh/dan-io.sh
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-18 18:41:19.000000 dan-build-0.2.1/completion/zsh/dan.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.233839 dan-build-0.2.1/dan/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.237839 dan-build-0.2.1/dan/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cli/click.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cli/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cli/vscode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.237839 dan-build-0.2.1/dan/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cmake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cmake/configure_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.237839 dan-build-0.2.1/dan/conan/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/conan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/conan/requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.237839 dan-build-0.2.1/dan/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/aiofiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/find.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/include.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/makefile.py
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/osinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/pm.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    15950 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/core/win.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.241839 dan-build-0.2.1/dan/cxx/
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cxx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cxx/compile_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.241839 dan-build-0.2.1/dan/cxx/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cxx/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cxx/data/detect.cmd
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cxx/data/empty.c
--rw-r--r--   0 runner    (1001) docker     (123)    21030 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cxx/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cxx/msvc_toolchain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.241839 dan-build-0.2.1/dan/cxx/support/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cxx/support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cxx/support/qt.py
--rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cxx/targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cxx/toolchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/cxx/unix_toolchain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.241839 dan-build-0.2.1/dan/io/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/io/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/io/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/make.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.241839 dan-build-0.2.1/dan/pkgconfig/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/pkgconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/pkgconfig/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.241839 dan-build-0.2.1/dan/pkgconfig/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/pkgconfig/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/pkgconfig/templates/pkg.pc.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.241839 dan-build-0.2.1/dan/src/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/src/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/src/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/src/tar.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-18 18:41:19.000000 dan-build-0.2.1/dan/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.241839 dan-build-0.2.1/dan_build.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-05-18 18:41:29.000000 dan-build-0.2.1/dan_build.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-18 18:41:29.000000 dan-build-0.2.1/dan_build.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:41:29.000000 dan-build-0.2.1/dan_build.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-18 18:41:29.000000 dan-build-0.2.1/dan_build.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-18 18:41:29.000000 dan-build-0.2.1/dan_build.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-18 18:41:29.000000 dan-build-0.2.1/dan_build.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-18 18:41:19.000000 dan-build-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 18:41:29.241839 dan-build-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:41:29.241839 dan-build-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-18 18:41:19.000000 dan-build-0.2.1/tests/test_cxx_libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-18 18:41:19.000000 dan-build-0.2.1/tests/test_cxx_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-18 18:41:19.000000 dan-build-0.2.1/tests/test_cxx_smc_catch2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.503644 dan-build-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-19 06:38:28.000000 dan-build-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-19 06:38:37.499644 dan-build-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-19 06:38:28.000000 dan-build-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.487644 dan-build-0.2.2/completion/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.491644 dan-build-0.2.2/completion/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-19 06:38:28.000000 dan-build-0.2.2/completion/bash/dan-io.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-19 06:38:28.000000 dan-build-0.2.2/completion/bash/dan.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.491644 dan-build-0.2.2/completion/zsh/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-19 06:38:28.000000 dan-build-0.2.2/completion/zsh/dan-io.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-19 06:38:28.000000 dan-build-0.2.2/completion/zsh/dan.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.491644 dan-build-0.2.2/dan/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.491644 dan-build-0.2.2/dan/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cli/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cli/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cli/vscode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.491644 dan-build-0.2.2/dan/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cmake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cmake/configure_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.491644 dan-build-0.2.2/dan/conan/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/conan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/conan/requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.495644 dan-build-0.2.2/dan/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/aiofiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/osinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/pm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15950 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/core/win.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.495644 dan-build-0.2.2/dan/cxx/
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cxx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cxx/compile_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.499644 dan-build-0.2.2/dan/cxx/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cxx/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cxx/data/detect.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cxx/data/empty.c
+-rw-r--r--   0 runner    (1001) docker     (123)    21030 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cxx/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cxx/msvc_toolchain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.499644 dan-build-0.2.2/dan/cxx/support/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cxx/support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cxx/support/qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cxx/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cxx/toolchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/cxx/unix_toolchain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.499644 dan-build-0.2.2/dan/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7396 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/io/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/io/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/make.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.499644 dan-build-0.2.2/dan/pkgconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/pkgconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/pkgconfig/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.499644 dan-build-0.2.2/dan/pkgconfig/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/pkgconfig/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/pkgconfig/templates/pkg.pc.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.499644 dan-build-0.2.2/dan/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/src/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/src/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/src/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-19 06:38:28.000000 dan-build-0.2.2/dan/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.499644 dan-build-0.2.2/dan_build.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-19 06:38:37.000000 dan-build-0.2.2/dan_build.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-19 06:38:37.000000 dan-build-0.2.2/dan_build.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 06:38:37.000000 dan-build-0.2.2/dan_build.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-19 06:38:37.000000 dan-build-0.2.2/dan_build.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-19 06:38:37.000000 dan-build-0.2.2/dan_build.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-19 06:38:37.000000 dan-build-0.2.2/dan_build.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-19 06:38:28.000000 dan-build-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 06:38:37.503644 dan-build-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:38:37.499644 dan-build-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-19 06:38:28.000000 dan-build-0.2.2/tests/test_cxx_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-19 06:38:28.000000 dan-build-0.2.2/tests/test_cxx_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-19 06:38:28.000000 dan-build-0.2.2/tests/test_cxx_smc_catch2.py
```

### Comparing `dan-build-0.2.1/LICENSE` & `dan-build-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/PKG-INFO` & `dan-build-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dan-build
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python-based build system.
 Author-email: Garcia Sylvain <garcia.6l20@gmail.com>, garcia.6l20@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Sylvain Garcia
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -80,38 +80,40 @@
             await dst.write(await src.read())
 ```
 
 ### C/CXX
 
 #### Libraries/Executables
 
-    ```python
-    from dan.cxx import Library, Executable
-    class MyLib(Library):
-        name = 'my-lib'
-        sources = ['src/my-lib.cpp']
-        public_includes = ['include']
-
-    class MyExe(Executable):
-        name = 'my-exe'
-        sources = ['src/main.cpp']
-        dependencies = [MyLib]
+```python
+from dan.cxx import Library, Executable
+class MyLib(Library):
+    name = 'my-lib'
+    sources = ['src/my-lib.cpp']
+    public_includes = ['include']
+
+class MyExe(Executable):
+    name = 'my-exe'
+    sources = ['src/main.cpp']
+    dependencies = [MyLib]
 
-    ```
+```
 
 #### Packages
-    [dan.io](https://github.com/Garcia6l20/dan.io) is the main (default) package source repository (custom repositories are supported by editting _~/.dan/repositories.json_) [documentation comming soon].
-    ```python
-    class MyExe(Executable):
-        name = 'my-exe'
-        sources = ['src/main.cpp']
-        dependencies = ['boost:headers@dan.io >= 1.82']
-    ```
 
-## dan cli usage
+[dan.io](https://github.com/Garcia6l20/dan.io) is the main (default) package source repository (custom repositories are supported by editting _~/.dan/repositories.json_), documentation comming soon.
+
+```python
+class MyExe(Executable):
+    name = 'my-exe'
+    sources = ['src/main.cpp']
+    dependencies = ['boost:headers@dan.io >= 1.82']
+```
+
+## `dan` cli usage
 
 `dan` is the main executable to build your project, it can build, test, list targets/test, ...
 
 ```bash
 dan --help
 Usage: dan [OPTIONS] COMMAND [ARGS]...
 
@@ -151,30 +153,29 @@
 
 ```bash
 dan build [-B <build_path>] [-v] [--for-install] [TARGETS]...
 ```
 
 ### Install
 
-Install targets marked with `self.install(...)` to the *install.destination* setting.
+Install targets marked with `install = True` property to the *install.destination* setting.
 
 ```bash
 dan install [-B <build_path>] [TARGETS]... [user|dev]
 ```
 
 Settings:
 - *install.destination*: The install destination (default: /usr/local).
 - *install.runtime_prefix*: Executables installation prefix (default: bin).
 - *install.libraries_prefix*: Libraries installation prefix (default: lib).
 - *install.includes_prefix*: Includes installation prefix (default: include).
 - *install.data_prefix*: Data files installation prefix (default: share).
 - *install.project_prefix*: !!! NOT USED YET !!! Project prefix (default: None).
 
-
-## dan-io cli usage
+## `dan-io` cli usage
 
 `dan-io` is a secondary utility to interract with package management system.
 
 ```bash
 $ dan-io --help 
 Usage: dan-io [OPTIONS] COMMAND [ARGS]...
 
@@ -200,22 +201,22 @@
   repositories  List available repositories
   versions      Get LIBRARY's available versions
 ```
 
 
 ## Auto completion
 
-`bash` and `zsh` completions are currently supported:
+_bash_ and _zsh_ completions are currently supported:
 
-- bash:
+- _bash_:
     ```bash
     for script in ~/.local/etc/bash_completion.d/*.sh; do
         source ${script}
     done
     ```
 
-- ksh:
+- _ksh_:
     ```ksh
     for script in ~/.local/etc/ksh_completion.d/*.sh; do
         source ${script}
     done
     ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dan-build-0.2.1/README.md` & `dan-build-0.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -44,38 +44,40 @@
             await dst.write(await src.read())
 ```
 
 ### C/CXX
 
 #### Libraries/Executables
 
-    ```python
-    from dan.cxx import Library, Executable
-    class MyLib(Library):
-        name = 'my-lib'
-        sources = ['src/my-lib.cpp']
-        public_includes = ['include']
-
-    class MyExe(Executable):
-        name = 'my-exe'
-        sources = ['src/main.cpp']
-        dependencies = [MyLib]
+```python
+from dan.cxx import Library, Executable
+class MyLib(Library):
+    name = 'my-lib'
+    sources = ['src/my-lib.cpp']
+    public_includes = ['include']
+
+class MyExe(Executable):
+    name = 'my-exe'
+    sources = ['src/main.cpp']
+    dependencies = [MyLib]
 
-    ```
+```
 
 #### Packages
-    [dan.io](https://github.com/Garcia6l20/dan.io) is the main (default) package source repository (custom repositories are supported by editting _~/.dan/repositories.json_) [documentation comming soon].
-    ```python
-    class MyExe(Executable):
-        name = 'my-exe'
-        sources = ['src/main.cpp']
-        dependencies = ['boost:headers@dan.io >= 1.82']
-    ```
 
-## dan cli usage
+[dan.io](https://github.com/Garcia6l20/dan.io) is the main (default) package source repository (custom repositories are supported by editting _~/.dan/repositories.json_), documentation comming soon.
+
+```python
+class MyExe(Executable):
+    name = 'my-exe'
+    sources = ['src/main.cpp']
+    dependencies = ['boost:headers@dan.io >= 1.82']
+```
+
+## `dan` cli usage
 
 `dan` is the main executable to build your project, it can build, test, list targets/test, ...
 
 ```bash
 dan --help
 Usage: dan [OPTIONS] COMMAND [ARGS]...
 
@@ -115,30 +117,29 @@
 
 ```bash
 dan build [-B <build_path>] [-v] [--for-install] [TARGETS]...
 ```
 
 ### Install
 
-Install targets marked with `self.install(...)` to the *install.destination* setting.
+Install targets marked with `install = True` property to the *install.destination* setting.
 
 ```bash
 dan install [-B <build_path>] [TARGETS]... [user|dev]
 ```
 
 Settings:
 - *install.destination*: The install destination (default: /usr/local).
 - *install.runtime_prefix*: Executables installation prefix (default: bin).
 - *install.libraries_prefix*: Libraries installation prefix (default: lib).
 - *install.includes_prefix*: Includes installation prefix (default: include).
 - *install.data_prefix*: Data files installation prefix (default: share).
 - *install.project_prefix*: !!! NOT USED YET !!! Project prefix (default: None).
 
-
-## dan-io cli usage
+## `dan-io` cli usage
 
 `dan-io` is a secondary utility to interract with package management system.
 
 ```bash
 $ dan-io --help 
 Usage: dan-io [OPTIONS] COMMAND [ARGS]...
 
@@ -164,22 +165,22 @@
   repositories  List available repositories
   versions      Get LIBRARY's available versions
 ```
 
 
 ## Auto completion
 
-`bash` and `zsh` completions are currently supported:
+_bash_ and _zsh_ completions are currently supported:
 
-- bash:
+- _bash_:
     ```bash
     for script in ~/.local/etc/bash_completion.d/*.sh; do
         source ${script}
     done
     ```
 
-- ksh:
+- _ksh_:
     ```ksh
     for script in ~/.local/etc/ksh_completion.d/*.sh; do
         source ${script}
     done
     ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dan-build-0.2.1/completion/bash/dan-io.sh` & `dan-build-0.2.2/completion/bash/dan-io.sh`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/completion/bash/dan.sh` & `dan-build-0.2.2/completion/bash/dan.sh`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/completion/zsh/dan-io.sh` & `dan-build-0.2.2/completion/zsh/dan-io.sh`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/completion/zsh/dan.sh` & `dan-build-0.2.2/completion/zsh/dan.sh`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/cli/click.py` & `dan-build-0.2.2/dan/cli/click.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/cli/io.py` & `dan-build-0.2.2/dan/cli/io.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/cli/main.py` & `dan-build-0.2.2/dan/cli/main.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/cli/vscode.py` & `dan-build-0.2.2/dan/cli/vscode.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/cmake/configure_file.py` & `dan-build-0.2.2/dan/cmake/configure_file.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/conan/requirements.py` & `dan-build-0.2.2/dan/conan/requirements.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/core/aiofiles.py` & `dan-build-0.2.2/dan/core/aiofiles.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/core/asyncio.py` & `dan-build-0.2.2/dan/core/asyncio.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/core/cache.py` & `dan-build-0.2.2/dan/core/cache.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/core/find.py` & `dan-build-0.2.2/dan/core/find.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/core/functools.py` & `dan-build-0.2.2/dan/core/functools.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/core/generator.py` & `dan-build-0.2.2/dan/core/generator.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/core/include.py` & `dan-build-0.2.2/dan/core/include.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/core/makefile.py` & `dan-build-0.2.2/dan/core/makefile.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/core/osinfo.py` & `dan-build-0.2.2/dan/core/osinfo.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/core/pathlib.py` & `dan-build-0.2.2/dan/core/pathlib.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/core/pm.py` & `dan-build-0.2.2/dan/core/pm.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/core/register.py` & `dan-build-0.2.2/dan/core/register.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/core/requirements.py` & `dan-build-0.2.2/dan/core/requirements.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/core/runners.py` & `dan-build-0.2.2/dan/core/runners.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/core/settings.py` & `dan-build-0.2.2/dan/core/settings.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/core/target.py` & `dan-build-0.2.2/dan/core/target.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/core/test.py` & `dan-build-0.2.2/dan/core/test.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/core/utils.py` & `dan-build-0.2.2/dan/core/utils.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/core/version.py` & `dan-build-0.2.2/dan/core/version.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/core/win.py` & `dan-build-0.2.2/dan/core/win.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/cxx/__init__.py` & `dan-build-0.2.2/dan/cxx/__init__.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/cxx/compile_commands.py` & `dan-build-0.2.2/dan/cxx/compile_commands.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/cxx/detect.py` & `dan-build-0.2.2/dan/cxx/detect.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/cxx/msvc_toolchain.py` & `dan-build-0.2.2/dan/cxx/msvc_toolchain.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/cxx/support/qt.py` & `dan-build-0.2.2/dan/cxx/support/qt.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/cxx/targets.py` & `dan-build-0.2.2/dan/cxx/targets.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/cxx/toolchain.py` & `dan-build-0.2.2/dan/cxx/toolchain.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/cxx/unix_toolchain.py` & `dan-build-0.2.2/dan/cxx/unix_toolchain.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/io/package.py` & `dan-build-0.2.2/dan/io/package.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,17 @@
         self.preload_dependencies.add(self.repo)
         self._package_makefile = None
         self._build_path = None
 
     @property
     def package_makefile(self):
         if self._package_makefile is None:
+            target = self.repo.find(self.name, self.package)
+            if target is None:
+                raise RuntimeError(f'cannot find {self.name} in {self.repo.name}')
             self._package_makefile = self.repo.find(self.name, self.package).makefile
         return self._package_makefile
 
     def get_sources(self):
         makefile = self.package_makefile
         sources = None
         for target in makefile.all_targets:
@@ -52,15 +55,20 @@
                         self.version = version
                         break
 
         packages_path = get_packages_path()
         from dan.cxx import target_toolchain as toolchain
         self._build_path = packages_path / toolchain.system / toolchain.arch / toolchain.build_type.name / self.package / str(self.version)
         self.install_settings = InstallSettings(self.build_path)
-        self.output = self.install_settings.libraries_prefix
+
+        makefile = self.package_makefile
+        for target in makefile.all_installed:
+            target.package_name = f'{self.package}:{target.name}'
+
+        self.output = Path(self.install_settings.libraries_prefix) / 'pkgconfig' / f'{target.package_name}.pc'
         sources.output = 'src' # TODO source_prefix in install settings
 
         return await super().__initialize__()
     
     @property
     def build_path(self) -> Path:
         return self._build_path
```

### Comparing `dan-build-0.2.1/dan/io/repositories.py` & `dan-build-0.2.2/dan/io/repositories.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         return self._package_makefile
 
     @property
     def installed(self) -> dict[str, Target]:
         pkgs = self.pkgs_makefile
         return {f'{lib.makefile.name}:{lib.name}@{self.name}' : lib for lib in pkgs.all_installed}
     
-    def find(self, name, package) -> Target:
+    def find(self, name: str, package: str) -> Target:
         if package is None:
             package = name
 
         for lib in self.pkgs_makefile.all_installed:
             if lib.name == name and lib.makefile.name == package:
                 return lib
```

### Comparing `dan-build-0.2.1/dan/jinja.py` & `dan-build-0.2.2/dan/jinja.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/logging.py` & `dan-build-0.2.2/dan/logging.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/make.py` & `dan-build-0.2.2/dan/make.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/pkgconfig/package.py` & `dan-build-0.2.2/dan/pkgconfig/package.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/src/git.py` & `dan-build-0.2.2/dan/src/git.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/src/github.py` & `dan-build-0.2.2/dan/src/github.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan/src/tar.py` & `dan-build-0.2.2/dan/src/tar.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/dan_build.egg-info/PKG-INFO` & `dan-build-0.2.2/dan_build.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dan-build
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python-based build system.
 Author-email: Garcia Sylvain <garcia.6l20@gmail.com>, garcia.6l20@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Sylvain Garcia
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -80,38 +80,40 @@
             await dst.write(await src.read())
 ```
 
 ### C/CXX
 
 #### Libraries/Executables
 
-    ```python
-    from dan.cxx import Library, Executable
-    class MyLib(Library):
-        name = 'my-lib'
-        sources = ['src/my-lib.cpp']
-        public_includes = ['include']
-
-    class MyExe(Executable):
-        name = 'my-exe'
-        sources = ['src/main.cpp']
-        dependencies = [MyLib]
+```python
+from dan.cxx import Library, Executable
+class MyLib(Library):
+    name = 'my-lib'
+    sources = ['src/my-lib.cpp']
+    public_includes = ['include']
+
+class MyExe(Executable):
+    name = 'my-exe'
+    sources = ['src/main.cpp']
+    dependencies = [MyLib]
 
-    ```
+```
 
 #### Packages
-    [dan.io](https://github.com/Garcia6l20/dan.io) is the main (default) package source repository (custom repositories are supported by editting _~/.dan/repositories.json_) [documentation comming soon].
-    ```python
-    class MyExe(Executable):
-        name = 'my-exe'
-        sources = ['src/main.cpp']
-        dependencies = ['boost:headers@dan.io >= 1.82']
-    ```
 
-## dan cli usage
+[dan.io](https://github.com/Garcia6l20/dan.io) is the main (default) package source repository (custom repositories are supported by editting _~/.dan/repositories.json_), documentation comming soon.
+
+```python
+class MyExe(Executable):
+    name = 'my-exe'
+    sources = ['src/main.cpp']
+    dependencies = ['boost:headers@dan.io >= 1.82']
+```
+
+## `dan` cli usage
 
 `dan` is the main executable to build your project, it can build, test, list targets/test, ...
 
 ```bash
 dan --help
 Usage: dan [OPTIONS] COMMAND [ARGS]...
 
@@ -151,30 +153,29 @@
 
 ```bash
 dan build [-B <build_path>] [-v] [--for-install] [TARGETS]...
 ```
 
 ### Install
 
-Install targets marked with `self.install(...)` to the *install.destination* setting.
+Install targets marked with `install = True` property to the *install.destination* setting.
 
 ```bash
 dan install [-B <build_path>] [TARGETS]... [user|dev]
 ```
 
 Settings:
 - *install.destination*: The install destination (default: /usr/local).
 - *install.runtime_prefix*: Executables installation prefix (default: bin).
 - *install.libraries_prefix*: Libraries installation prefix (default: lib).
 - *install.includes_prefix*: Includes installation prefix (default: include).
 - *install.data_prefix*: Data files installation prefix (default: share).
 - *install.project_prefix*: !!! NOT USED YET !!! Project prefix (default: None).
 
-
-## dan-io cli usage
+## `dan-io` cli usage
 
 `dan-io` is a secondary utility to interract with package management system.
 
 ```bash
 $ dan-io --help 
 Usage: dan-io [OPTIONS] COMMAND [ARGS]...
 
@@ -200,22 +201,22 @@
   repositories  List available repositories
   versions      Get LIBRARY's available versions
 ```
 
 
 ## Auto completion
 
-`bash` and `zsh` completions are currently supported:
+_bash_ and _zsh_ completions are currently supported:
 
-- bash:
+- _bash_:
     ```bash
     for script in ~/.local/etc/bash_completion.d/*.sh; do
         source ${script}
     done
     ```
 
-- ksh:
+- _ksh_:
     ```ksh
     for script in ~/.local/etc/ksh_completion.d/*.sh; do
         source ${script}
     done
     ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dan-build-0.2.1/dan_build.egg-info/SOURCES.txt` & `dan-build-0.2.2/dan_build.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/pyproject.toml` & `dan-build-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/tests/test_cxx_libraries.py` & `dan-build-0.2.2/tests/test_cxx_libraries.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/tests/test_cxx_simple.py` & `dan-build-0.2.2/tests/test_cxx_simple.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.1/tests/test_cxx_smc_catch2.py` & `dan-build-0.2.2/tests/test_cxx_smc_catch2.py`

 * *Files identical despite different names*

