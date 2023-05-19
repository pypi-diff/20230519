# Comparing `tmp/types-setuptools-67.7.0.2.tar.gz` & `tmp/types-setuptools-67.7.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-setuptools-67.7.0.2.tar", last modified: Wed May 10 15:20:33 2023, max compression
+gzip compressed data, was "types-setuptools-67.7.0.3.tar", last modified: Fri May 19 06:18:47 2023, max compression
```

## Comparing `types-setuptools-67.7.0.2.tar` & `types-setuptools-67.7.0.3.tar`

### file list

```diff
@@ -1,79 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:33.030217 types-setuptools-67.7.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-05-10 15:20:32.000000 types-setuptools-67.7.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:20:32.000000 types-setuptools-67.7.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-10 15:20:33.030217 types-setuptools-67.7.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:33.022217 types-setuptools-67.7.0.2/pkg_resources-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-10 15:20:32.000000 types-setuptools-67.7.0.2/pkg_resources-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/pkg_resources-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:20:33.030217 types-setuptools-67.7.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-10 15:20:32.000000 types-setuptools-67.7.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:33.026217 types-setuptools-67.7.0.2/setuptools-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-10 15:20:32.000000 types-setuptools-67.7.0.2/setuptools-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:33.026217 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/cmd.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:33.026217 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/build_clib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/build_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/build_py.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/install.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/install_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/install_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/register.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/sdist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/upload.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/dist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/extension.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/filelist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/archive_util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/build_meta.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:33.030217 types-setuptools-67.7.0.2/setuptools-stubs/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/alias.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/build_clib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/build_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/build_py.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/develop.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/dist_info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/easy_install.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/egg_info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/install.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/install_egg_info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/install_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/install_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/register.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/rotate.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/saveopts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/sdist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/setopt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/test.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/upload.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/upload_docs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/dep_util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/depends.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/dist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/extension.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:33.030217 types-setuptools-67.7.0.2/setuptools-stubs/extern/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/extern/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/glob.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/installer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/launch.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/monkey.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/msvc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/namespaces.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/package_index.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/sandbox.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/unicode_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/warnings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/wheel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/windows_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:33.030217 types-setuptools-67.7.0.2/types_setuptools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-10 15:20:32.000000 types-setuptools-67.7.0.2/types_setuptools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-10 15:20:32.000000 types-setuptools-67.7.0.2/types_setuptools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:20:32.000000 types-setuptools-67.7.0.2/types_setuptools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-10 15:20:32.000000 types-setuptools-67.7.0.2/types_setuptools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:18:47.278708 types-setuptools-67.7.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-05-19 06:18:44.000000 types-setuptools-67.7.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 06:18:44.000000 types-setuptools-67.7.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-19 06:18:47.278708 types-setuptools-67.7.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:18:47.270707 types-setuptools-67.7.0.3/pkg_resources-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-19 06:18:44.000000 types-setuptools-67.7.0.3/pkg_resources-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    15339 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/pkg_resources-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 06:18:47.278708 types-setuptools-67.7.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-19 06:18:44.000000 types-setuptools-67.7.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:18:47.274708 types-setuptools-67.7.0.3/setuptools-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-19 06:18:44.000000 types-setuptools-67.7.0.3/setuptools-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:18:47.274708 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/cmd.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:18:47.274708 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/bdist_rpm.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/build_clib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/build_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/build_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/install.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/install_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/install_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/register.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/sdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/upload.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/dist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/_distutils/filelist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/archive_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/build_meta.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:18:47.278708 types-setuptools-67.7.0.3/setuptools-stubs/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/alias.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/bdist_egg.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/bdist_rpm.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/build_clib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/build_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/build_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/develop.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/dist_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/easy_install.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/editable_wheel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/egg_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/install.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/install_egg_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/install_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/install_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/register.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/rotate.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/saveopts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/sdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/setopt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/test.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/upload.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/command/upload_docs.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:18:47.278708 types-setuptools-67.7.0.3/setuptools-stubs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/config/expand.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/config/pyprojecttoml.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/config/setupcfg.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/dep_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/depends.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/discovery.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/dist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/extension.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:18:47.278708 types-setuptools-67.7.0.3/setuptools-stubs/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/extern/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/glob.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/installer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/launch.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/logging.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/monkey.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/msvc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/namespaces.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/package_index.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/py312compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/sandbox.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/unicode_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/warnings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/wheel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-19 06:18:29.000000 types-setuptools-67.7.0.3/setuptools-stubs/windows_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:18:47.278708 types-setuptools-67.7.0.3/types_setuptools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-19 06:18:47.000000 types-setuptools-67.7.0.3/types_setuptools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-19 06:18:47.000000 types-setuptools-67.7.0.3/types_setuptools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 06:18:47.000000 types-setuptools-67.7.0.3/types_setuptools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-19 06:18:47.000000 types-setuptools-67.7.0.3/types_setuptools.egg-info/top_level.txt
```

### Comparing `types-setuptools-67.7.0.2/CHANGELOG.md` & `types-setuptools-67.7.0.3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 67.7.0.3 (2023-05-19)
+
+Don't ignore missing stubs in setuptools (#10058)
+
 ## 67.7.0.2 (2023-05-10)
 
 Add `partial_stub` metadata field (#10157)
 
 ## 67.7.0.1 (2023-05-01)
 
 Avoid unnecessary forward refs in class definitions (#10124)
```

### Comparing `types-setuptools-67.7.0.2/PKG-INFO` & `types-setuptools-67.7.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-setuptools
-Version: 67.7.0.2
+Version: 67.7.0.3
 Summary: Typing stubs for setuptools
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `setuptools`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `b5c9d8d6770e09dff00648b79281702e111d4e01`.
```

### Comparing `types-setuptools-67.7.0.2/pkg_resources-stubs/__init__.pyi` & `types-setuptools-67.7.0.3/pkg_resources-stubs/__init__.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -2,55 +2,61 @@
 import types
 import zipimport
 from _typeshed import Incomplete
 from abc import ABCMeta
 from collections.abc import Callable, Generator, Iterable, Sequence
 from io import BytesIO
 from re import Pattern
-from typing import IO, Any, ClassVar, TypeVar, overload
+from typing import IO, Any, ClassVar, Protocol, TypeVar, overload, type_check_only
 from typing_extensions import Literal, Self, TypeAlias
 
 _Version: TypeAlias = Incomplete  # from packaging.version
 
 _T = TypeVar("_T")
 _D = TypeVar("_D", bound=Distribution)
 _NestedStr: TypeAlias = str | Iterable[str | Iterable[Any]]
 _InstallerType: TypeAlias = Callable[[Requirement], Distribution | None]
 _EPDistType: TypeAlias = Distribution | Requirement | str
 _MetadataType: TypeAlias = IResourceProvider | None
 _PkgReqType: TypeAlias = str | Requirement
 _DistFinderType: TypeAlias = Callable[[_Importer, str, bool], Generator[Distribution, None, None]]
 _NSHandlerType: TypeAlias = Callable[[_Importer, str, str, types.ModuleType], str]
 
-def declare_namespace(name: str) -> None: ...
-def fixup_namespace_packages(path_item: str) -> None: ...
+def declare_namespace(packageName: str) -> None: ...
+def fixup_namespace_packages(path_item: str, parent=None) -> None: ...
 
 class WorkingSet:
     entries: list[str]
     def __init__(self, entries: Iterable[str] | None = None) -> None: ...
     def require(self, *requirements: _NestedStr) -> Sequence[Distribution]: ...
     def run_script(self, requires: str, script_name: str) -> None: ...
     def iter_entry_points(self, group: str, name: str | None = None) -> Generator[EntryPoint, None, None]: ...
     def add_entry(self, entry: str) -> None: ...
     def __contains__(self, dist: Distribution) -> bool: ...
     def __iter__(self) -> Generator[Distribution, None, None]: ...
     def find(self, req: Requirement) -> Distribution | None: ...
     def resolve(
-        self, requirements: Iterable[Requirement], env: Environment | None = None, installer: _InstallerType | None = None
+        self,
+        requirements: Iterable[Requirement],
+        env: Environment | None = None,
+        installer: _InstallerType | None = None,
+        replace_conflicting: bool = False,
+        extras=None,
     ) -> list[Distribution]: ...
     def add(self, dist: Distribution, entry: str | None = None, insert: bool = True, replace: bool = False) -> None: ...
-    def subscribe(self, callback: Callable[[Distribution], object]) -> None: ...
+    def subscribe(self, callback: Callable[[Distribution], object], existing: bool = True) -> None: ...
     def find_plugins(
-        self, plugin_env: Environment, full_env: Environment | None = None, fallback: bool = True
+        self, plugin_env: Environment, full_env: Environment | None = None, installer=None, fallback: bool = True
     ) -> tuple[list[Distribution], dict[Distribution, Exception]]: ...
 
 working_set: WorkingSet
 
 require = working_set.require
 run_script = working_set.run_script
+run_main = run_script
 iter_entry_points = working_set.iter_entry_points
 add_activation_listener = working_set.subscribe
 
 class Environment:
     def __init__(
         self, search_path: Sequence[str] | None = None, platform: str | None = ..., python: str | None = ...
     ) -> None: ...
@@ -58,21 +64,23 @@
     def __iter__(self) -> Generator[str, None, None]: ...
     def add(self, dist: Distribution) -> None: ...
     def remove(self, dist: Distribution) -> None: ...
     def can_add(self, dist: Distribution) -> bool: ...
     def __add__(self, other: Distribution | Environment) -> Environment: ...
     def __iadd__(self, other: Distribution | Environment) -> Self: ...
     @overload
-    def best_match(self, req: Requirement, working_set: WorkingSet, *, replace_conflicting: bool = False) -> Distribution: ...
+    def best_match(
+        self, req: Requirement, working_set: WorkingSet, installer: None = None, replace_conflicting: bool = False
+    ) -> Distribution: ...
     @overload
     def best_match(
         self, req: Requirement, working_set: WorkingSet, installer: Callable[[Requirement], _T], replace_conflicting: bool = False
     ) -> _T: ...
     @overload
-    def obtain(self, requirement: Requirement) -> None: ...
+    def obtain(self, requirement: Requirement, installer: None = None) -> None: ...
     @overload
     def obtain(self, requirement: Requirement, installer: Callable[[Requirement], _T]) -> _T: ...
     def scan(self, search_path: Sequence[str] | None = None) -> None: ...
 
 def parse_requirements(strs: str | Iterable[str]) -> Generator[Requirement, None, None]: ...
 
 class Requirement:
@@ -81,27 +89,29 @@
     key: str
     extras: tuple[str, ...]
     specs: list[tuple[str, str]]
     url: str | None
     # TODO: change this to packaging.markers.Marker | None once we can import
     #       packaging.markers
     marker: Incomplete | None
+    def __init__(self, requirement_string: str) -> None: ...
     @staticmethod
     def parse(s: str | Iterable[str]) -> Requirement: ...
     def __contains__(self, item: Distribution | str | tuple[str, ...]) -> bool: ...
     def __eq__(self, other_requirement: object) -> bool: ...
 
 def load_entry_point(dist: _EPDistType, group: str, name: str) -> Any: ...
 def get_entry_info(dist: _EPDistType, group: str, name: str) -> EntryPoint | None: ...
 @overload
-def get_entry_map(dist: _EPDistType) -> dict[str, dict[str, EntryPoint]]: ...
+def get_entry_map(dist: _EPDistType, group: None = None) -> dict[str, dict[str, EntryPoint]]: ...
 @overload
 def get_entry_map(dist: _EPDistType, group: str) -> dict[str, EntryPoint]: ...
 
 class EntryPoint:
+    pattern: ClassVar[Pattern[str]]
     name: str
     module_name: str
     attrs: tuple[str, ...]
     extras: tuple[str, ...]
     dist: Distribution | None
     def __init__(
         self,
@@ -139,34 +149,34 @@
 def resource_stream(package_or_requirement: _PkgReqType, resource_name: str) -> IO[bytes]: ...
 def resource_string(package_or_requirement: _PkgReqType, resource_name: str) -> bytes: ...
 def resource_isdir(package_or_requirement: _PkgReqType, resource_name: str) -> bool: ...
 def resource_listdir(package_or_requirement: _PkgReqType, resource_name: str) -> list[str]: ...
 def resource_filename(package_or_requirement: _PkgReqType, resource_name: str) -> str: ...
 def set_extraction_path(path: str) -> None: ...
 def cleanup_resources(force: bool = False) -> list[str]: ...
-
-class IResourceManager:
+@type_check_only
+class _IResourceManager(Protocol):
     def resource_exists(self, package_or_requirement: _PkgReqType, resource_name: str) -> bool: ...
     def resource_stream(self, package_or_requirement: _PkgReqType, resource_name: str) -> IO[bytes]: ...
     def resource_string(self, package_or_requirement: _PkgReqType, resource_name: str) -> bytes: ...
     def resource_isdir(self, package_or_requirement: _PkgReqType, resource_name: str) -> bool: ...
     def resource_listdir(self, package_or_requirement: _PkgReqType, resource_name: str) -> list[str]: ...
     def resource_filename(self, package_or_requirement: _PkgReqType, resource_name: str) -> str: ...
     def set_extraction_path(self, path: str) -> None: ...
     def cleanup_resources(self, force: bool = ...) -> list[str]: ...
     def get_cache_path(self, archive_name: str, names: Iterable[str] = ...) -> str: ...
     def extraction_error(self) -> None: ...
     def postprocess(self, tempname: str, filename: str) -> None: ...
 
 @overload
-def get_provider(package_or_requirement: str) -> IResourceProvider: ...
+def get_provider(moduleOrReq: str) -> IResourceProvider: ...
 @overload
-def get_provider(package_or_requirement: Requirement) -> Distribution: ...
+def get_provider(moduleOrReq: Requirement) -> Distribution: ...
 
-class IMetadataProvider:
+class IMetadataProvider(Protocol):
     def has_metadata(self, name: str) -> bool | None: ...
     def metadata_isdir(self, name: str) -> bool: ...
     def metadata_listdir(self, name: str) -> list[str]: ...
     def get_metadata(self, name: str) -> str: ...
     def get_metadata_lines(self, name: str) -> Generator[str, None, None]: ...
     def run_script(self, script_name: str, namespace: dict[str, Any]) -> None: ...
 
@@ -192,51 +202,70 @@
 class ContextualVersionConflict(VersionConflict):
     @property
     def required_by(self) -> set[Distribution | str]: ...
 
 class UnknownExtra(ResolutionError): ...
 
 class ExtractionError(Exception):
-    manager: IResourceManager
+    manager: _IResourceManager
     cache_path: str
     original_error: Exception
 
 class _Importer(importlib.abc.MetaPathFinder, importlib.abc.InspectLoader, metaclass=ABCMeta): ...
 
 def register_finder(importer_type: type, distribution_finder: _DistFinderType) -> None: ...
 def register_loader_type(loader_type: type, provider_factory: Callable[[types.ModuleType], IResourceProvider]) -> None: ...
 def register_namespace_handler(importer_type: type, namespace_handler: _NSHandlerType) -> None: ...
 
-class IResourceProvider(IMetadataProvider): ...
+class IResourceProvider(IMetadataProvider, Protocol):
+    def get_resource_filename(self, manager: _IResourceManager, resource_name): ...
+    def get_resource_stream(self, manager: _IResourceManager, resource_name): ...
+    def get_resource_string(self, manager: _IResourceManager, resource_name): ...
+    def has_resource(self, resource_name): ...
+    def resource_isdir(self, resource_name): ...
+    def resource_listdir(self, resource_name): ...
+
+def invalid_marker(text) -> SyntaxError | Literal[False]: ...
+def evaluate_marker(text, extra: Incomplete | None = None): ...
 
 class NullProvider:
     egg_name: str | None
     egg_info: str | None
     loader: types._LoaderProtocol | None
     module_path: str | None
 
     def __init__(self, module) -> None: ...
-    def get_resource_filename(self, manager, resource_name) -> str: ...
-    def get_resource_stream(self, manager, resource_name) -> BytesIO: ...
-    def get_resource_string(self, manager, resource_name): ...
+    def get_resource_filename(self, manager: _IResourceManager, resource_name) -> str: ...
+    def get_resource_stream(self, manager: _IResourceManager, resource_name) -> BytesIO: ...
+    def get_resource_string(self, manager: _IResourceManager, resource_name): ...
     def has_resource(self, resource_name) -> bool: ...
     def has_metadata(self, name: str) -> bool | None: ...
     def get_metadata(self, name: str) -> str: ...
     def get_metadata_lines(self, name: str) -> Generator[str, None, None]: ...
     def resource_isdir(self, resource_name) -> bool: ...
     def metadata_isdir(self, name: str) -> bool: ...
     def resource_listdir(self, resource_name) -> list[str]: ...
     def metadata_listdir(self, name: str) -> list[str]: ...
     def run_script(self, script_name: str, namespace: dict[str, Any]) -> None: ...
 
-class Distribution(NullProvider, IResourceProvider, IMetadataProvider):
+# Doesn't actually extend NullProvider
+class Distribution(NullProvider):
     PKG_INFO: ClassVar[str]
     location: str
     project_name: str
     @property
+    def hashcmp(self) -> tuple[Incomplete, int, str, Incomplete | None, str, str]: ...
+    def __hash__(self) -> int: ...
+    def __lt__(self, other: Distribution) -> bool: ...
+    def __le__(self, other: Distribution) -> bool: ...
+    def __gt__(self, other: Distribution) -> bool: ...
+    def __ge__(self, other: Distribution) -> bool: ...
+    def __eq__(self, other: object) -> bool: ...
+    def __ne__(self, other: object) -> bool: ...
+    @property
     def key(self) -> str: ...
     @property
     def extras(self) -> list[str]: ...
     @property
     def version(self) -> str: ...
     @property
     def parsed_version(self) -> tuple[str, ...]: ...
@@ -255,68 +284,76 @@
     ) -> None: ...
     @classmethod
     def from_location(
         cls, location: str, basename: str, metadata: _MetadataType = None, **kw: str | None | int
     ) -> Distribution: ...
     @classmethod
     def from_filename(cls, filename: str, metadata: _MetadataType = None, **kw: str | None | int) -> Distribution: ...
-    def activate(self, path: list[str] | None = None) -> None: ...
+    def activate(self, path: list[str] | None = None, replace: bool = False) -> None: ...
     def as_requirement(self) -> Requirement: ...
     def requires(self, extras: tuple[str, ...] = ()) -> list[Requirement]: ...
+    def check_version_conflict(self) -> None: ...
+    def has_version(self) -> bool: ...
     def clone(self, **kw: str | int | None) -> Requirement: ...
     def egg_name(self) -> str: ...  # type: ignore[override]  # supertype's egg_name is a variable, not a method
-    def __cmp__(self, other: Any) -> bool: ...
     def get_entry_info(self, group: str, name: str) -> EntryPoint | None: ...
+    def insert_on(self, path, loc: Incomplete | None = None, replace: bool = False) -> None: ...
     @overload
-    def get_entry_map(self) -> dict[str, dict[str, EntryPoint]]: ...
+    def get_entry_map(self, group: None = None) -> dict[str, dict[str, EntryPoint]]: ...
     @overload
     def get_entry_map(self, group: str) -> dict[str, EntryPoint]: ...
     def load_entry_point(self, group: str, name: str) -> Any: ...
 
 class DistInfoDistribution(Distribution):
     PKG_INFO: ClassVar[Literal["METADATA"]]
     EQEQ: ClassVar[Pattern[str]]
 
 class EggProvider(NullProvider):
     egg_root: str
 
 class DefaultProvider(EggProvider): ...
 
-class PathMetadata(DefaultProvider, IResourceProvider):
+class PathMetadata(DefaultProvider):
     egg_info: str
     module_path: str
     def __init__(self, path: str, egg_info: str) -> None: ...
 
 class ZipProvider(EggProvider):
     eagers: list[str] | None
     zip_pre: str
+    @property
+    def zipinfo(self): ...
 
-class EggMetadata(ZipProvider, IResourceProvider):
+class EggMetadata(ZipProvider):
     loader: zipimport.zipimporter
     module_path: str
-    def __init__(self, zipimporter: zipimport.zipimporter) -> None: ...
+    def __init__(self, importer: zipimport.zipimporter) -> None: ...
 
 class EmptyProvider(NullProvider):
     module_path: None
     def __init__(self) -> None: ...
 
 empty_provider: EmptyProvider
 
-class FileMetadata(EmptyProvider, IResourceProvider):
-    def __init__(self, path_to_pkg_info: str) -> None: ...
+class FileMetadata(EmptyProvider):
+    def __init__(self, path: str) -> None: ...
+
+class PEP440Warning(RuntimeWarning): ...
 
 parse_version = _Version
 
 def yield_lines(iterable: _NestedStr) -> Generator[str, None, None]: ...
-def split_sections(strs: _NestedStr) -> Generator[tuple[str | None, list[str]], None, None]: ...
+def split_sections(s: _NestedStr) -> Generator[tuple[str | None, list[str]], None, None]: ...
 def safe_name(name: str) -> str: ...
 def safe_version(version: str) -> str: ...
 def safe_extra(extra: str) -> str: ...
-def to_filename(name_or_version: str) -> str: ...
+def to_filename(name: str) -> str: ...
 def get_build_platform() -> str: ...
 def get_platform() -> str: ...
 def get_supported_platform() -> str: ...
 def compatible_platforms(provided: str | None, required: str | None) -> bool: ...
 def get_default_cache() -> str: ...
 def get_importer(path_item: str) -> _Importer: ...
 def ensure_directory(path: str) -> None: ...
 def normalize_path(filename: str) -> str: ...
+
+class PkgResourcesDeprecationWarning(Warning): ...
```

### Comparing `types-setuptools-67.7.0.2/setup.py` & `types-setuptools-67.7.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,32 +12,32 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `setuptools`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `b5c9d8d6770e09dff00648b79281702e111d4e01`.
 '''.lstrip()
 
 setup(name=name,
-      version="67.7.0.2",
+      version="67.7.0.3",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['pkg_resources-stubs', 'setuptools-stubs'],
-      package_data={'pkg_resources-stubs': ['__init__.pyi', 'METADATA.toml'], 'setuptools-stubs': ['__init__.pyi', '_distutils/cmd.pyi', '_distutils/command/build_clib.pyi', '_distutils/command/build_ext.pyi', '_distutils/command/build_py.pyi', '_distutils/command/install.pyi', '_distutils/command/install_lib.pyi', '_distutils/command/install_scripts.pyi', '_distutils/command/register.pyi', '_distutils/command/sdist.pyi', '_distutils/command/upload.pyi', '_distutils/config.pyi', '_distutils/dist.pyi', '_distutils/errors.pyi', '_distutils/extension.pyi', '_distutils/filelist.pyi', 'archive_util.pyi', 'build_meta.pyi', 'command/__init__.pyi', 'command/alias.pyi', 'command/build_clib.pyi', 'command/build_ext.pyi', 'command/build_py.pyi', 'command/develop.pyi', 'command/dist_info.pyi', 'command/easy_install.pyi', 'command/egg_info.pyi', 'command/install.pyi', 'command/install_egg_info.pyi', 'command/install_lib.pyi', 'command/install_scripts.pyi', 'command/register.pyi', 'command/rotate.pyi', 'command/saveopts.pyi', 'command/sdist.pyi', 'command/setopt.pyi', 'command/test.pyi', 'command/upload.pyi', 'command/upload_docs.pyi', 'config.pyi', 'dep_util.pyi', 'depends.pyi', 'dist.pyi', 'errors.pyi', 'extension.pyi', 'extern/__init__.pyi', 'glob.pyi', 'installer.pyi', 'launch.pyi', 'monkey.pyi', 'msvc.pyi', 'namespaces.pyi', 'package_index.pyi', 'sandbox.pyi', 'unicode_utils.pyi', 'version.pyi', 'warnings.pyi', 'wheel.pyi', 'windows_support.pyi', 'METADATA.toml']},
+      package_data={'pkg_resources-stubs': ['__init__.pyi', 'METADATA.toml'], 'setuptools-stubs': ['__init__.pyi', '_distutils/cmd.pyi', '_distutils/command/bdist_rpm.pyi', '_distutils/command/build.pyi', '_distutils/command/build_clib.pyi', '_distutils/command/build_ext.pyi', '_distutils/command/build_py.pyi', '_distutils/command/install.pyi', '_distutils/command/install_lib.pyi', '_distutils/command/install_scripts.pyi', '_distutils/command/register.pyi', '_distutils/command/sdist.pyi', '_distutils/command/upload.pyi', '_distutils/config.pyi', '_distutils/dist.pyi', '_distutils/errors.pyi', '_distutils/extension.pyi', '_distutils/filelist.pyi', 'archive_util.pyi', 'build_meta.pyi', 'command/__init__.pyi', 'command/alias.pyi', 'command/bdist_egg.pyi', 'command/bdist_rpm.pyi', 'command/build.pyi', 'command/build_clib.pyi', 'command/build_ext.pyi', 'command/build_py.pyi', 'command/develop.pyi', 'command/dist_info.pyi', 'command/easy_install.pyi', 'command/editable_wheel.pyi', 'command/egg_info.pyi', 'command/install.pyi', 'command/install_egg_info.pyi', 'command/install_lib.pyi', 'command/install_scripts.pyi', 'command/register.pyi', 'command/rotate.pyi', 'command/saveopts.pyi', 'command/sdist.pyi', 'command/setopt.pyi', 'command/test.pyi', 'command/upload.pyi', 'command/upload_docs.pyi', 'config/__init__.pyi', 'config/expand.pyi', 'config/pyprojecttoml.pyi', 'config/setupcfg.pyi', 'dep_util.pyi', 'depends.pyi', 'discovery.pyi', 'dist.pyi', 'errors.pyi', 'extension.pyi', 'extern/__init__.pyi', 'glob.pyi', 'installer.pyi', 'launch.pyi', 'logging.pyi', 'monkey.pyi', 'msvc.pyi', 'namespaces.pyi', 'package_index.pyi', 'py312compat.pyi', 'sandbox.pyi', 'unicode_utils.pyi', 'version.pyi', 'warnings.pyi', 'wheel.pyi', 'windows_support.pyi', 'METADATA.toml']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/__init__.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/__init__.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 from abc import abstractmethod
 from collections.abc import Iterable, Mapping, Sequence
 from typing import Any
 
-from setuptools.depends import Require as Require
-from setuptools.dist import Distribution as Distribution
-from setuptools.extension import Extension as Extension
-from setuptools.warnings import SetuptoolsDeprecationWarning as SetuptoolsDeprecationWarning
-
 from ._distutils.cmd import Command as _Command
+from .depends import Require as Require
+from .discovery import _Path
+from .dist import Distribution as Distribution
+from .extension import Extension as Extension
+from .warnings import SetuptoolsDeprecationWarning as SetuptoolsDeprecationWarning
+
+__all__ = [
+    "setup",
+    "Distribution",
+    "Command",
+    "Extension",
+    "Require",
+    "SetuptoolsDeprecationWarning",
+    "find_packages",
+    "find_namespace_packages",
+]
 
 __version__: str
 
-class PackageFinder:
-    @classmethod
-    def find(cls, where: str = ".", exclude: Iterable[str] = (), include: Iterable[str] = ("*",)) -> list[str]: ...
-
-class PEP420PackageFinder(PackageFinder): ...
-
-find_packages = PackageFinder.find
-find_namespace_packages = PEP420PackageFinder.find
-
+# Pytype fails with the following:
+# find_packages = PackageFinder.find
+# find_namespace_packages = PEP420PackageFinder.find
+def find_packages(where: _Path = ".", exclude: Iterable[str] = (), include: Iterable[str] = ("*",)) -> list[str]: ...
+def find_namespace_packages(where: _Path = ".", exclude: Iterable[str] = (), include: Iterable[str] = ("*",)) -> list[str]: ...
 def setup(
     *,
     name: str = ...,
     version: str = ...,
     description: str = ...,
     long_description: str = ...,
     author: str = ...,
```

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/_distutils/cmd.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/cmd.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/build_clib.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/build_clib.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/build_ext.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/build_ext.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/build_py.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/build_py.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/install.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/install.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/install_lib.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/install_lib.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/register.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/register.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/sdist.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/command/sdist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/_distutils/dist.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/dist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/_distutils/errors.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/_distutils/extension.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/extension.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/_distutils/filelist.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/_distutils/filelist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/archive_util.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/archive_util.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 from _typeshed import Incomplete
 from typing import Any
 
 from ._distutils.errors import DistutilsError
 
+__all__ = [
+    "unpack_archive",
+    "unpack_zipfile",
+    "unpack_tarfile",
+    "default_filter",
+    "UnrecognizedFormat",
+    "extraction_drivers",
+    "unpack_directory",
+]
+
 class UnrecognizedFormat(DistutilsError): ...
 
 def default_filter(src, dst): ...
 def unpack_archive(filename, extract_dir, progress_filter=..., drivers: Incomplete | None = None) -> None: ...
 def unpack_directory(filename, extract_dir, progress_filter=...) -> None: ...
 def unpack_zipfile(filename, extract_dir, progress_filter=...) -> None: ...
 def unpack_tarfile(filename, extract_dir, progress_filter=...): ...
```

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/build_meta.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/build_meta.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 from collections.abc import Mapping
 from typing import Any
 
-from setuptools import dist
+from . import dist
+
+__all__ = [
+    "get_requires_for_build_sdist",
+    "get_requires_for_build_wheel",
+    "prepare_metadata_for_build_wheel",
+    "build_wheel",
+    "build_sdist",
+    "get_requires_for_build_editable",
+    "prepare_metadata_for_build_editable",
+    "build_editable",
+    "__legacy__",
+    "SetupRequirementsError",
+]
 
 class SetupRequirementsError(BaseException):
     specifiers: Any
     def __init__(self, specifiers) -> None: ...
 
 class Distribution(dist.Distribution):
     def fetch_build_eggs(self, specifiers) -> None: ...
@@ -37,8 +50,12 @@
 _BACKEND: _BuildMetaBackend
 get_requires_for_build_wheel = _BACKEND.get_requires_for_build_wheel
 get_requires_for_build_sdist = _BACKEND.get_requires_for_build_sdist
 prepare_metadata_for_build_wheel = _BACKEND.prepare_metadata_for_build_wheel
 build_wheel = _BACKEND.build_wheel
 build_sdist = _BACKEND.build_sdist
 
+get_requires_for_build_editable = _BACKEND.get_requires_for_build_editable
+prepare_metadata_for_build_editable = _BACKEND.prepare_metadata_for_build_editable
+build_editable = _BACKEND.build_editable
+
 __legacy__: _BuildMetaLegacyBackend
```

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/command/build_ext.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/command/build_ext.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from _typeshed import Incomplete
-from typing import Any
+from typing import Any, ClassVar
 
 from .._distutils.command.build_ext import build_ext as _build_ext
 
 have_rtld: bool
 use_stubs: bool
 libtype: str
 
 def if_dl(s): ...
 def get_abi3_suffix(): ...
 
 class build_ext(_build_ext):
+    editable_mode: ClassVar[bool]
     inplace: Any
     def run(self) -> None: ...
     def copy_extensions_to_source(self) -> None: ...
     def get_ext_filename(self, fullname): ...
     shlib_compiler: Any
     shlibs: Any
     ext_map: Any
@@ -23,14 +24,15 @@
     def finalize_options(self) -> None: ...
     def setup_shlib_compiler(self) -> None: ...
     def get_export_symbols(self, ext): ...
     compiler: Any
     def build_extension(self, ext) -> None: ...
     def links_to_dynamic(self, ext): ...
     def get_outputs(self): ...
+    def get_output_mapping(self) -> dict[str, str]: ...
     def write_stub(self, output_dir, ext, compile: bool = False) -> None: ...
 
 def link_shared_object(
     self,
     objects,
     output_libname,
     output_dir: Incomplete | None = None,
```

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/command/build_py.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/command/build_py.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,28 @@
-from typing import Any
+from _typeshed import Incomplete
+from typing import Any, ClassVar
 
 from .._distutils.command import build_py as orig
 
 def make_writable(target) -> None: ...
 
 class build_py(orig.build_py):
+    editable_mode: ClassVar[bool]
     package_data: Any
     exclude_package_data: Any
     def finalize_options(self) -> None: ...
     def run(self) -> None: ...
     data_files: Any
     def __getattr__(self, attr: str): ...
     def build_module(self, module, module_file, package): ...
+    def get_data_files_without_manifest(self) -> list[tuple[Incomplete, Incomplete, Incomplete, list[Incomplete]]]: ...
     def find_data_files(self, package, src_dir): ...
     def build_package_data(self) -> None: ...
     manifest_files: Any
+    def get_output_mapping(self) -> dict[str, str]: ...
     def analyze_manifest(self) -> None: ...
     def get_data_files(self) -> None: ...
     def check_package(self, package, package_dir): ...
     packages_checked: Any
     def initialize_options(self) -> None: ...
     def get_package_dir(self, package): ...
     def exclude_data_files(self, package, src_dir, files): ...
```

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/command/develop.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/command/develop.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any
 
-from setuptools import namespaces
-from setuptools.command.easy_install import easy_install
+from .. import namespaces
+from .easy_install import easy_install
 
 class develop(namespaces.DevelopInstaller, easy_install):
     description: str
     user_options: Any
     boolean_options: Any
     command_consumes_arguments: bool
     multi_version: bool
```

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/command/easy_install.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/command/easy_install.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from _typeshed import Incomplete
 from collections.abc import Iterator
 from typing import Any
 
 from pkg_resources import Environment
-from setuptools import Command, SetuptoolsDeprecationWarning
+
+from .. import Command, SetuptoolsDeprecationWarning
+
+__all__ = ["easy_install", "PthDistributions", "extract_wininst_cfg", "get_exe_prefixes"]
 
 class easy_install(Command):
     description: str
     command_consumes_arguments: bool
     user_options: Any
     boolean_options: Any
     negative_opt: Any
```

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/command/egg_info.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/command/egg_info.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import Any
+from typing_extensions import Final
 
-from setuptools import Command, SetuptoolsDeprecationWarning
-from setuptools.command.sdist import sdist
-
+from .. import Command, SetuptoolsDeprecationWarning
 from .._distutils.filelist import FileList as _FileList
+from .sdist import sdist
+
+PY_MAJOR: Final[str]
 
 def translate_pattern(glob): ...
 
 class InfoCommon:
     tag_build: Any
     tag_date: Any
     @property
```

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/command/sdist.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/command/sdist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/command/setopt.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/command/setopt.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from abc import abstractmethod
 from typing import Any
 
-from setuptools import Command
+from .. import Command
+
+__all__ = ["config_file", "edit_config", "option_base", "setopt"]
 
 def config_file(kind: str = "local"): ...
 def edit_config(filename, settings, dry_run: bool = False) -> None: ...
 
 class option_base(Command):
     user_options: Any
     boolean_options: Any
```

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/command/test.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/command/test.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from _typeshed import Incomplete, Unused
 from collections.abc import Callable
 from types import ModuleType
 from typing import Any, Generic, TypeVar, overload
 from typing_extensions import Self
 from unittest import TestLoader, TestSuite
 
-from setuptools import Command
+from .. import Command
 
 _T = TypeVar("_T")
 
 class ScanningLoader(TestLoader):
     def __init__(self) -> None: ...
     def loadTestsFromModule(self, module: ModuleType, pattern: Incomplete | None = None) -> list[TestSuite]: ...  # type: ignore[override]
```

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/command/upload_docs.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/command/upload_docs.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/depends.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/depends.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,16 @@
 from _typeshed import Incomplete
+from typing import IO, Any
+from typing_extensions import Literal
+
+__all__ = ["Require", "find_module", "get_module_constant", "extract_constant"]
+
+def find_module(
+    module, paths=None
+) -> tuple[IO[Any], str | None, tuple[str, Literal["", "r", "rb"], Literal[7, 6, 1, 2, 3, -1]]]: ...
 
 class Require:
     def __init__(
         self,
         name,
         requested_version,
         module,
```

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/dist.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/dist.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from collections.abc import Iterable, Iterator, Mapping, MutableMapping
 from typing import Any
 
-from setuptools import Command, SetuptoolsDeprecationWarning
-
+from . import Command, SetuptoolsDeprecationWarning
 from ._distutils.dist import Distribution as _Distribution
 
+__all__ = ["Distribution"]
+
 class Distribution(_Distribution):
     def patch_missing_pkg_info(self, attrs: Mapping[str, Any]) -> None: ...
     src_root: str | None
     dependency_links: list[str]
     setup_requires: list[str]
     def __init__(self, attrs: MutableMapping[str, Any] | None = None) -> None: ...
     def warn_dash_deprecation(self, opt: str, section: str) -> str: ...
```

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/errors.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/extension.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/extension.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/extern/__init__.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/extern/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/msvc.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/msvc.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.2/setuptools-stubs/package_index.pyi` & `types-setuptools-67.7.0.3/setuptools-stubs/package_index.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import configparser
 from _typeshed import Incomplete
 from typing import Any
 
 from pkg_resources import Environment
 
+__all__ = ["PackageIndex", "distros_for_url", "parse_bdist_wininst", "interpret_distro_name"]
+
 def parse_bdist_wininst(name): ...
 def distros_for_url(url, metadata: Incomplete | None = None) -> None: ...
 def interpret_distro_name(
     location, basename, metadata, py_version: Incomplete | None = None, precedence=1, platform: Incomplete | None = None
 ) -> None: ...
 
 class ContentChecker:
```

### Comparing `types-setuptools-67.7.0.2/types_setuptools.egg-info/PKG-INFO` & `types-setuptools-67.7.0.3/types_setuptools.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-setuptools
-Version: 67.7.0.2
+Version: 67.7.0.3
 Summary: Typing stubs for setuptools
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `setuptools`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `b5c9d8d6770e09dff00648b79281702e111d4e01`.
```

### Comparing `types-setuptools-67.7.0.2/types_setuptools.egg-info/SOURCES.txt` & `types-setuptools-67.7.0.3/types_setuptools.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,67 +3,79 @@
 setup.py
 pkg_resources-stubs/METADATA.toml
 pkg_resources-stubs/__init__.pyi
 setuptools-stubs/METADATA.toml
 setuptools-stubs/__init__.pyi
 setuptools-stubs/archive_util.pyi
 setuptools-stubs/build_meta.pyi
-setuptools-stubs/config.pyi
 setuptools-stubs/dep_util.pyi
 setuptools-stubs/depends.pyi
+setuptools-stubs/discovery.pyi
 setuptools-stubs/dist.pyi
 setuptools-stubs/errors.pyi
 setuptools-stubs/extension.pyi
 setuptools-stubs/glob.pyi
 setuptools-stubs/installer.pyi
 setuptools-stubs/launch.pyi
+setuptools-stubs/logging.pyi
 setuptools-stubs/monkey.pyi
 setuptools-stubs/msvc.pyi
 setuptools-stubs/namespaces.pyi
 setuptools-stubs/package_index.pyi
+setuptools-stubs/py312compat.pyi
 setuptools-stubs/sandbox.pyi
 setuptools-stubs/unicode_utils.pyi
 setuptools-stubs/version.pyi
 setuptools-stubs/warnings.pyi
 setuptools-stubs/wheel.pyi
 setuptools-stubs/windows_support.pyi
 setuptools-stubs/_distutils/cmd.pyi
 setuptools-stubs/_distutils/config.pyi
 setuptools-stubs/_distutils/dist.pyi
 setuptools-stubs/_distutils/errors.pyi
 setuptools-stubs/_distutils/extension.pyi
 setuptools-stubs/_distutils/filelist.pyi
+setuptools-stubs/_distutils/command/bdist_rpm.pyi
+setuptools-stubs/_distutils/command/build.pyi
 setuptools-stubs/_distutils/command/build_clib.pyi
 setuptools-stubs/_distutils/command/build_ext.pyi
 setuptools-stubs/_distutils/command/build_py.pyi
 setuptools-stubs/_distutils/command/install.pyi
 setuptools-stubs/_distutils/command/install_lib.pyi
 setuptools-stubs/_distutils/command/install_scripts.pyi
 setuptools-stubs/_distutils/command/register.pyi
 setuptools-stubs/_distutils/command/sdist.pyi
 setuptools-stubs/_distutils/command/upload.pyi
 setuptools-stubs/command/__init__.pyi
 setuptools-stubs/command/alias.pyi
+setuptools-stubs/command/bdist_egg.pyi
+setuptools-stubs/command/bdist_rpm.pyi
+setuptools-stubs/command/build.pyi
 setuptools-stubs/command/build_clib.pyi
 setuptools-stubs/command/build_ext.pyi
 setuptools-stubs/command/build_py.pyi
 setuptools-stubs/command/develop.pyi
 setuptools-stubs/command/dist_info.pyi
 setuptools-stubs/command/easy_install.pyi
+setuptools-stubs/command/editable_wheel.pyi
 setuptools-stubs/command/egg_info.pyi
 setuptools-stubs/command/install.pyi
 setuptools-stubs/command/install_egg_info.pyi
 setuptools-stubs/command/install_lib.pyi
 setuptools-stubs/command/install_scripts.pyi
 setuptools-stubs/command/register.pyi
 setuptools-stubs/command/rotate.pyi
 setuptools-stubs/command/saveopts.pyi
 setuptools-stubs/command/sdist.pyi
 setuptools-stubs/command/setopt.pyi
 setuptools-stubs/command/test.pyi
 setuptools-stubs/command/upload.pyi
 setuptools-stubs/command/upload_docs.pyi
+setuptools-stubs/config/__init__.pyi
+setuptools-stubs/config/expand.pyi
+setuptools-stubs/config/pyprojecttoml.pyi
+setuptools-stubs/config/setupcfg.pyi
 setuptools-stubs/extern/__init__.pyi
 types_setuptools.egg-info/PKG-INFO
 types_setuptools.egg-info/SOURCES.txt
 types_setuptools.egg-info/dependency_links.txt
 types_setuptools.egg-info/top_level.txt
```

