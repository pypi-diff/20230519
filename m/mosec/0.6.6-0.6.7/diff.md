# Comparing `tmp/mosec-0.6.6.tar.gz` & `tmp/mosec-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosec-0.6.6.tar", last modified: Thu May  4 09:35:21 2023, max compression
+gzip compressed data, was "mosec-0.6.7.tar", last modified: Fri May 19 11:21:43 2023, max compression
```

## Comparing `mosec-0.6.6.tar` & `mosec-0.6.7.tar`

### file list

```diff
@@ -1,85 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:21.926152 mosec-0.6.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:21.918152 mosec-0.6.6/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-04 09:32:45.000000 mosec-0.6.6/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-04 09:32:45.000000 mosec-0.6.6/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-04 09:32:45.000000 mosec-0.6.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-04 09:32:45.000000 mosec-0.6.6/.lycheeignore
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-04 09:32:45.000000 mosec-0.6.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-04 09:32:45.000000 mosec-0.6.6/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-04 09:32:45.000000 mosec-0.6.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    26636 2023-05-04 09:32:45.000000 mosec-0.6.6/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-04 09:32:45.000000 mosec-0.6.6/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-05-04 09:32:45.000000 mosec-0.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-04 09:32:45.000000 mosec-0.6.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-04 09:32:45.000000 mosec-0.6.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    13357 2023-05-04 09:35:21.926152 mosec-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-05-04 09:32:45.000000 mosec-0.6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-04 09:32:45.000000 mosec-0.6.6/build.envd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:21.918152 mosec-0.6.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-04 09:32:45.000000 mosec-0.6.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-04 09:32:45.000000 mosec-0.6.6/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:21.918152 mosec-0.6.6/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-04 09:32:45.000000 mosec-0.6.6/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:21.918152 mosec-0.6.6/docs/source/development/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-04 09:32:45.000000 mosec-0.6.6/docs/source/development/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-04 09:32:45.000000 mosec-0.6.6/docs/source/development/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:21.918152 mosec-0.6.6/docs/source/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-04 09:32:45.000000 mosec-0.6.6/docs/source/examples/echo.md
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-04 09:32:45.000000 mosec-0.6.6/docs/source/examples/env.md
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-04 09:32:45.000000 mosec-0.6.6/docs/source/examples/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-04 09:32:45.000000 mosec-0.6.6/docs/source/examples/ipc.md
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-04 09:32:45.000000 mosec-0.6.6/docs/source/examples/jax.md
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-04 09:32:45.000000 mosec-0.6.6/docs/source/examples/metric.md
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-04 09:32:45.000000 mosec-0.6.6/docs/source/examples/pytorch.md
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-04 09:32:45.000000 mosec-0.6.6/docs/source/examples/stable_diffusion.md
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-04 09:32:45.000000 mosec-0.6.6/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-04 09:32:45.000000 mosec-0.6.6/docs/source/license.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:21.918152 mosec-0.6.6/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-04 09:32:45.000000 mosec-0.6.6/docs/source/reference/arguments.md
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-04 09:32:45.000000 mosec-0.6.6/docs/source/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-04 09:32:45.000000 mosec-0.6.6/docs/source/reference/interface.md
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-04 09:32:45.000000 mosec-0.6.6/license.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:21.922152 mosec-0.6.6/mosec/
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-04 09:32:45.000000 mosec-0.6.6/mosec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 09:35:21.000000 mosec-0.6.6/mosec/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-04 09:32:45.000000 mosec-0.6.6/mosec/args.py
--rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-05-04 09:32:45.000000 mosec-0.6.6/mosec/coordinator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-05-04 09:32:45.000000 mosec-0.6.6/mosec/dry_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-04 09:32:45.000000 mosec-0.6.6/mosec/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-04 09:32:45.000000 mosec-0.6.6/mosec/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-04 09:32:45.000000 mosec-0.6.6/mosec/ipc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-05-04 09:32:45.000000 mosec-0.6.6/mosec/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:21.922152 mosec-0.6.6/mosec/mixin/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-04 09:32:45.000000 mosec-0.6.6/mosec/mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-04 09:32:45.000000 mosec-0.6.6/mosec/mixin/msgpack_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-04 09:32:45.000000 mosec-0.6.6/mosec/mixin/numbin_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:21.922152 mosec-0.6.6/mosec/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-04 09:32:45.000000 mosec-0.6.6/mosec/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-04 09:32:45.000000 mosec-0.6.6/mosec/plugins/plasma_shm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-05-04 09:32:45.000000 mosec-0.6.6/mosec/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 09:32:45.000000 mosec-0.6.6/mosec/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-05-04 09:32:45.000000 mosec-0.6.6/mosec/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-05-04 09:32:45.000000 mosec-0.6.6/mosec/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:21.922152 mosec-0.6.6/mosec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13357 2023-05-04 09:35:21.000000 mosec-0.6.6/mosec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-04 09:35:21.000000 mosec-0.6.6/mosec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:35:21.000000 mosec-0.6.6/mosec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:35:21.000000 mosec-0.6.6/mosec.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-04 09:35:21.000000 mosec-0.6.6/mosec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 09:35:21.000000 mosec-0.6.6/mosec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-04 09:32:45.000000 mosec-0.6.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:21.922152 mosec-0.6.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-04 09:32:45.000000 mosec-0.6.6/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-04 09:32:45.000000 mosec-0.6.6/requirements/doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-04 09:32:45.000000 mosec-0.6.6/requirements/plugin.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-04 09:32:45.000000 mosec-0.6.6/rustfmt.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:35:21.926152 mosec-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-04 09:32:45.000000 mosec-0.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:21.926152 mosec-0.6.6/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-04 09:32:45.000000 mosec-0.6.6/src/args.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-04 09:32:45.000000 mosec-0.6.6/src/coordinator.rs
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-04 09:32:45.000000 mosec-0.6.6/src/errors.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-05-04 09:32:45.000000 mosec-0.6.6/src/main.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-05-04 09:32:45.000000 mosec-0.6.6/src/metrics.rs
--rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-05-04 09:32:45.000000 mosec-0.6.6/src/protocol.rs
--rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-05-04 09:32:45.000000 mosec-0.6.6/src/tasks.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.702897 mosec-0.6.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.690897 mosec-0.6.7/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-19 11:19:15.000000 mosec-0.6.7/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-19 11:19:15.000000 mosec-0.6.7/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-19 11:19:15.000000 mosec-0.6.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-19 11:19:15.000000 mosec-0.6.7/.lycheeignore
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-19 11:19:15.000000 mosec-0.6.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-19 11:19:15.000000 mosec-0.6.7/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-19 11:19:15.000000 mosec-0.6.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    26636 2023-05-19 11:19:15.000000 mosec-0.6.7/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-19 11:19:15.000000 mosec-0.6.7/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-05-19 11:19:15.000000 mosec-0.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-19 11:19:15.000000 mosec-0.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-19 11:19:15.000000 mosec-0.6.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-05-19 11:21:43.702897 mosec-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-05-19 11:19:15.000000 mosec-0.6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-19 11:19:15.000000 mosec-0.6.7/build.envd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.694897 mosec-0.6.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.694897 mosec-0.6.7/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.694897 mosec-0.6.7/docs/source/development/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/development/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/development/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.694897 mosec-0.6.7/docs/source/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/examples/echo.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/examples/env.md
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/examples/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/examples/ipc.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/examples/jax.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/examples/metric.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/examples/pytorch.md
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/examples/stable_diffusion.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/examples/validate.md
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/license.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.694897 mosec-0.6.7/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/reference/arguments.md
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-19 11:19:15.000000 mosec-0.6.7/docs/source/reference/interface.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-19 11:19:15.000000 mosec-0.6.7/license.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.698897 mosec-0.6.7/mosec/
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-19 11:21:43.000000 mosec-0.6.7/mosec/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/coordinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/dry_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/ipc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.702897 mosec-0.6.7/mosec/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/mixin/msgpack_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/mixin/numbin_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/mixin/plasma_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/mixin/typed_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.702897 mosec-0.6.7/mosec/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/plugins/plasma_shm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-05-19 11:19:15.000000 mosec-0.6.7/mosec/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.698897 mosec-0.6.7/mosec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-05-19 11:21:43.000000 mosec-0.6.7/mosec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-19 11:21:43.000000 mosec-0.6.7/mosec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:21:43.000000 mosec-0.6.7/mosec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:21:43.000000 mosec-0.6.7/mosec.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-19 11:21:43.000000 mosec-0.6.7/mosec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 11:21:43.000000 mosec-0.6.7/mosec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-19 11:19:15.000000 mosec-0.6.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.702897 mosec-0.6.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-19 11:19:15.000000 mosec-0.6.7/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-19 11:19:15.000000 mosec-0.6.7/requirements/doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-19 11:19:15.000000 mosec-0.6.7/requirements/mixin.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-19 11:19:15.000000 mosec-0.6.7/rustfmt.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 11:21:43.702897 mosec-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-19 11:19:15.000000 mosec-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:43.702897 mosec-0.6.7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-19 11:19:15.000000 mosec-0.6.7/src/args.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-19 11:19:15.000000 mosec-0.6.7/src/coordinator.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-19 11:19:15.000000 mosec-0.6.7/src/errors.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-05-19 11:19:15.000000 mosec-0.6.7/src/main.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-05-19 11:19:15.000000 mosec-0.6.7/src/metrics.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-05-19 11:19:15.000000 mosec-0.6.7/src/protocol.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-05-19 11:19:15.000000 mosec-0.6.7/src/tasks.rs
```

### Comparing `mosec-0.6.6/.gitignore` & `mosec-0.6.7/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -140,7 +140,10 @@
 
 # IDE
 .vscode/*
 .idea/*
 
 # version file generated by setuptools_scm
 mosec/_version.py
+
+# ruff
+.ruff_cache/
```

### Comparing `mosec-0.6.6/CONTRIBUTING.md` & `mosec-0.6.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/Cargo.lock` & `mosec-0.6.7/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -56,17 +56,17 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "axum"
-version = "0.6.17"
+version = "0.6.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b70caf9f1b0c045f7da350636435b775a9733adf2df56e8aa2a29210fbc335d4"
+checksum = "f8175979259124331c1d7bf6586ee7e0da434155e4b2d48ec2c8386281d8df39"
 dependencies = [
  "async-trait",
  "axum-core",
  "bitflags",
  "bytes",
  "futures-util",
  "http",
@@ -353,15 +353,15 @@
  "log",
  "wasi",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "mosec"
-version = "0.6.6"
+version = "0.6.7"
 dependencies = [
  "argh",
  "async-channel",
  "axum",
  "bytes",
  "derive_more",
  "hyper",
@@ -694,17 +694,17 @@
 checksum = "fd80a657e71da814b8e5d60d3374fc6d35045062245d80224748ae522dd76f36"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
 name = "tokio"
-version = "1.28.0"
+version = "1.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3c786bf8134e5a3a166db9b29ab8f48134739014a3eca7bc6bfa95d673b136f"
+checksum = "0aa32867d44e6f2ce3385e89dceb990188b8bb0fb25b0cf576647a6f98ac5105"
 dependencies = [
  "autocfg",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "pin-project-lite",
```

### Comparing `mosec-0.6.6/Cargo.toml` & `mosec-0.6.7/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "mosec"
-version = "0.6.6"
+version = "0.6.7"
 authors = ["Keming <kemingy94@gmail.com>", "Zichen <lkevinzc@gmail.com>"]
 edition = "2021"
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/mosecorg/mosec"
 description = "Model Serving made Efficient in the Cloud."
 documentation = "https://docs.rs/mosec"
@@ -19,8 +19,8 @@
 tokio = { version = "1", features = ["rt", "rt-multi-thread", "time", "macros", "sync", "signal", "io-util"] }
 derive_more = { version = "0.99", features = ["display", "error"] }
 # MPMS that only one consumer sees each message & async
 async-channel = { version = "1" }
 once_cell = "1.17"
 prometheus-client = "0.20.0"
 argh = "0.1"
-axum = "0.6.17"
+axum = "0.6.18"
```

### Comparing `mosec-0.6.6/LICENSE` & `mosec-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/Makefile` & `mosec-0.6.7/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .DEFAULT_GOAL:=dev
 
 PY_SOURCE_FILES=mosec tests examples setup.py
 RUST_SOURCE_FILES=src/*
 
 install:
-	pip install -e .[dev,doc,plugin]
+	pip install -e .[dev,doc,mixin]
 	pre-commit install
 	rustup toolchain install nightly
 	rustup component add rustfmt --toolchain nightly
 
 dev:
 	cargo build
 	@mkdir -p mosec/bin
@@ -17,21 +17,21 @@
 
 test: dev
 	echo "Running tests for the main logic"
 	pytest tests -vv -s -m "not arrow"
 	RUST_BACKTRACE=1 cargo test -vv
 
 test_arrow: dev
-	@pip install -q -r requirements/plugin.txt
-	echo "Running tests for the plugin"
+	@pip install -q -r requirements/mixin.txt
+	echo "Running tests for the mixin"
 	pytest tests -vv -s -m "arrow"
-	pip uninstall -y -r requirements/plugin.txt
+	pip uninstall -y -r requirements/mixin.txt
 
 test_all: dev
-	@pip install -q -r requirements/plugin.txt
+	@pip install -q -r requirements/mixin.txt
 	echo "Running tests for the all features"
 	pytest tests -vv -s
 	RUST_BACKTRACE=1 cargo test -vv
 
 doc:
 	@cd docs && make html && cd ../
 	@python -m http.server -d docs/build/html
```

### Comparing `mosec-0.6.6/PKG-INFO` & `mosec-0.6.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: mosec
-Version: 0.6.6
+Version: 0.6.7
 Summary: Model Serving made Efficient in the Cloud.
 Home-page: https://github.com/mosecorg/mosec
 Author: Keming Yang
 Author-email: kemingy94@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: plugin
+Provides-Extra: mixin
 Provides-Extra: doc
 License-File: LICENSE
 
 <p align="center">
   <img src="https://user-images.githubusercontent.com/38581401/134487662-49733d45-2ba0-4c19-aa07-1f43fd35c453.png" height="230" alt="MOSEC" />
 </p>
 
@@ -175,14 +175,15 @@
 That's it! You have just hosted your **_stable-diffusion model_** as a service! 😉
 
 ## Examples
 
 More ready-to-use examples can be found in the [Example](https://mosecorg.github.io/mosec/examples/index.html) section. It includes:
 
 - [Multi-stage workflow demo](https://mosecorg.github.io/mosec/examples/echo.html): a simple echo demo even without any ML model.
+- [Request validation](https://mosecorg.github.io/mosec/examples/validate.html): validate the request with type annotation.
 - [Shared memory IPC](https://mosecorg.github.io/mosec/examples/ipc.html): inter-process communication with shared memory.
 - [Customized GPU allocation](https://mosecorg.github.io/mosec/examples/env.html): deploy multiple replicas, each using different GPUs.
 - [Customized metrics](https://mosecorg.github.io/mosec/examples/metric.html): record your own metrics for monitoring.
 - [Jax jitted inference](https://mosecorg.github.io/mosec/examples/jax.html): just-in-time compilation speeds up the inference.
 - PyTorch deep learning models:
   - [sentiment analysis](https://mosecorg.github.io/mosec/examples/pytorch.html#natural-language-processing): infer the sentiment of a sentence.
   - [image recognition](https://mosecorg.github.io/mosec/examples/pytorch.html#computer-vision): categorize a given image.
@@ -209,15 +210,16 @@
 - Stop the service with `SIGINT` or `SIGTERM` since it has the graceful shutdown logic.
 
 ## Adopters
 
 Here are some of the companies and individual users that are using Mosec:
 
 - [Modelz](https://modelz.ai): Serverless platform for ML inference.
-- [MOSS](https://github.com/OpenLMLab/MOSS/): An open sourced conversational language model like ChatGPT.
+- [MOSS](https://github.com/OpenLMLab/MOSS/blob/main/README_en.md): An open sourced conversational language model like ChatGPT.
+- [TencentCloud](https://www.tencentcloud.com/document/product/1141/45261): Tencent Cloud Machine Learning Platform, using Mosec as the [core inference server framework](https://cloud.tencent.com/document/product/851/74148).
 - [TensorChord](https://github.com/tensorchord): Cloud native AI infrastructure company.
 
 ## Citation
 
 If you find this software useful for your research, please consider citing
 
 ```
```

### Comparing `mosec-0.6.6/README.md` & `mosec-0.6.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,15 @@
 That's it! You have just hosted your **_stable-diffusion model_** as a service! 😉
 
 ## Examples
 
 More ready-to-use examples can be found in the [Example](https://mosecorg.github.io/mosec/examples/index.html) section. It includes:
 
 - [Multi-stage workflow demo](https://mosecorg.github.io/mosec/examples/echo.html): a simple echo demo even without any ML model.
+- [Request validation](https://mosecorg.github.io/mosec/examples/validate.html): validate the request with type annotation.
 - [Shared memory IPC](https://mosecorg.github.io/mosec/examples/ipc.html): inter-process communication with shared memory.
 - [Customized GPU allocation](https://mosecorg.github.io/mosec/examples/env.html): deploy multiple replicas, each using different GPUs.
 - [Customized metrics](https://mosecorg.github.io/mosec/examples/metric.html): record your own metrics for monitoring.
 - [Jax jitted inference](https://mosecorg.github.io/mosec/examples/jax.html): just-in-time compilation speeds up the inference.
 - PyTorch deep learning models:
   - [sentiment analysis](https://mosecorg.github.io/mosec/examples/pytorch.html#natural-language-processing): infer the sentiment of a sentence.
   - [image recognition](https://mosecorg.github.io/mosec/examples/pytorch.html#computer-vision): categorize a given image.
@@ -193,15 +194,16 @@
 - Stop the service with `SIGINT` or `SIGTERM` since it has the graceful shutdown logic.
 
 ## Adopters
 
 Here are some of the companies and individual users that are using Mosec:
 
 - [Modelz](https://modelz.ai): Serverless platform for ML inference.
-- [MOSS](https://github.com/OpenLMLab/MOSS/): An open sourced conversational language model like ChatGPT.
+- [MOSS](https://github.com/OpenLMLab/MOSS/blob/main/README_en.md): An open sourced conversational language model like ChatGPT.
+- [TencentCloud](https://www.tencentcloud.com/document/product/1141/45261): Tencent Cloud Machine Learning Platform, using Mosec as the [core inference server framework](https://cloud.tencent.com/document/product/851/74148).
 - [TensorChord](https://github.com/tensorchord): Cloud native AI infrastructure company.
 
 ## Citation
 
 If you find this software useful for your research, please consider citing
 
 ```
```

### Comparing `mosec-0.6.6/build.envd` & `mosec-0.6.7/build.envd`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/docs/Makefile` & `mosec-0.6.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/docs/make.bat` & `mosec-0.6.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/docs/source/conf.py` & `mosec-0.6.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/docs/source/examples/echo.md` & `mosec-0.6.7/docs/source/examples/echo.md`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/docs/source/examples/env.md` & `mosec-0.6.7/docs/source/examples/env.md`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/docs/source/examples/index.md` & `mosec-0.6.7/docs/source/examples/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 echo
 env
 ipc
 jax
 metric
 pytorch
 stable_diffusion
+validate
 ```
 
 We provide examples across different ML frameworks and for various tasks in this section.
 
 ## Requirements
 
 All the examples in this section are self-contained and tested. Feel free to grab one and run:
```

### Comparing `mosec-0.6.6/docs/source/examples/ipc.md` & `mosec-0.6.7/docs/source/examples/ipc.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Shared Memory IPC
 
 This is an example demonstrating how you can enable the plasma shared memory store or customize your own IPC wrapper.
 
 Mosec's multi-stage pipeline requires the output data from the previous stage to be transferred to the next stage across python processes. This is coordinated via Unix domain socket between every Python worker process from all stages and the Rust controller process.
 
-By default, we serialize the data and directly transfer the bytes over the socket. However, users may find wrapping this IPC useful or more efficient for specific use cases. Therefore, we provide the `mosec.plugins.IPCWrapper` interface and an example implementation `PlasmaShmWrapper` based on [`pyarrow.plasma`](https://arrow.apache.org/docs/python/plasma.html).
+By default, we serialize the data and directly transfer the bytes over the socket. However, users may find wrapping this IPC useful or more efficient for specific use cases. Therefore, we provide an example implementation `PlasmaShmIPCMixin` based on [`pyarrow.plasma`](https://arrow.apache.org/docs/11.0/python/plasma.html).
+
+```{warning}
+`plasma` is deprecated. Please use Redis instead.
+```
 
 The additional subprocess can be registered as a daemon thus it will be checked by mosec regularly and trigger graceful shutdown when the daemon exits.
 
 ## **`plasma_shm_ipc.py`**
 
 ```{include} ../../../examples/plasma_shm_ipc.py
 :code: python
```

### Comparing `mosec-0.6.6/docs/source/examples/jax.md` & `mosec-0.6.7/docs/source/examples/jax.md`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/docs/source/examples/metric.md` & `mosec-0.6.7/docs/source/examples/metric.md`

 * *Files 19% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 This example has a simple WSGI app as the monitoring metrics service. In each worker process, the `Counter` will collect the inference results and export them to the metrics service. For the inference part, it parses the batch data and compares them with the average value.
 
 For more information about the multiprocess mode for the metrics, check the [Prometheus doc](https://github.com/prometheus/client_python#multiprocess-mode-eg-gunicorn).
 
 ## **`python_side_metrics.py`**
 
-```{include} ../../../examples/python_side_metrics.py
+```{include} ../../../examples/monitor/python_side_metrics.py
 :code: python
 ```
 
 ## Start
 
 ```shell
 python python_side_metrics.py
@@ -40,7 +40,10 @@
 ```
 
 ## Check the Rust side metrics
 
 ```shell
 http :8000/metrics
 ```
+
+```{include} ../../../examples/monitor/README.md
+```
```

### Comparing `mosec-0.6.6/docs/source/examples/pytorch.md` & `mosec-0.6.7/docs/source/examples/pytorch.md`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 ### Image Recognition
 
 This server receives an image and classify it according to the [ImageNet](https://www.image-net.org/) categorization. We specifically use [ResNet](https://arxiv.org/abs/1512.03385) as an image classifier and build a model service based on it. Nevertheless, this file serves as the starter code for any kind of image recognition model server.
 
 We enable multiprocessing for `Preprocess` stage, so that it can produce enough tasks for `Inference` stage to do **batch inference**, which better exploits the GPU computing power. More interestingly, we also started multiple model by setting the number of worker for `Inference` stage to 2. This is because a single model hardly fully occupy the GPU memory or utilization. Multiple models running on the same device in parallel can further increase our service throughput.
 
-When instantiating the `Server`, we enable `plasma_shm`, which utilizes the [`pyarrow.plasma`](https://arrow.apache.org/docs/python/plasma.html) as a shared memory data store for IPC. This could benefit the data transfer, especially when the data is large (preprocessed image data in this case), since its implementation uses [`nogil`](https://cython.readthedocs.io/en/latest/src/userguide/external_C_code.html#releasing-the-gil) to escape the limitation of GIL. Note that you need to use `pip install -U "mosec[shm]"` to install necessary dependencies.
+When instantiating the `Server`, we enable `plasma_shm`, which utilizes the [`pyarrow.plasma`](https://arrow.apache.org/docs/11.0/python/plasma.html) as a shared memory data store for IPC. This could benefit the data transfer, especially when the data is large (preprocessed image data in this case). Note that you need to use `pip install -U pyarrow==11` to install necessary dependencies.
 
 We also demonstrate how to customized **validation** on the data content through this example. In the `forward` method of the `Preprocess` worker, we firstly check the key of the input, then try to decode the str and load it into array. If any of these steps fails, we raise the `ValidationError`. The status will be finally returned to our clients as [HTTP 422](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/422).
 
 #### Server
 
 ```shell
 python resnet50_server_msgpack.py
```

### Comparing `mosec-0.6.6/docs/source/examples/stable_diffusion.md` & `mosec-0.6.7/docs/source/examples/stable_diffusion.md`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/docs/source/index.md` & `mosec-0.6.7/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/license.json` & `mosec-0.6.7/license.json`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/mosec/__init__.py` & `mosec-0.6.7/mosec/__init__.py`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/mosec/args.py` & `mosec-0.6.7/mosec/args.py`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/mosec/coordinator.py` & `mosec-0.6.7/mosec/coordinator.py`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/mosec/dry_run.py` & `mosec-0.6.7/mosec/dry_run.py`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/mosec/env.py` & `mosec-0.6.7/mosec/env.py`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/mosec/errors.py` & `mosec-0.6.7/mosec/errors.py`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/mosec/ipc.py` & `mosec-0.6.7/mosec/ipc.py`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/mosec/log.py` & `mosec-0.6.7/mosec/log.py`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/mosec/mixin/msgpack_worker.py` & `mosec-0.6.7/mosec/mixin/msgpack_worker.py`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/mosec/mixin/numbin_worker.py` & `mosec-0.6.7/mosec/mixin/numbin_worker.py`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/mosec/plugins/__init__.py` & `mosec-0.6.7/mosec/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/mosec/plugins/plasma_shm.py` & `mosec-0.6.7/mosec/plugins/plasma_shm.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,19 @@
 """Provide another data transfer way between workers.
 
 The data will be stored in plasma shared memory, while the object ID will be
 sent via the original way.
 
     use case: large image tensors
     benefits: more stable P99 latency
+
+```{warning}
+This implementation is deprecated. Please use
+:py:mod:`PlasmaShmIPCMixin <mosec.mixin.PlasmaShmIPCMixin>`
+```
 """
 
 import warnings
 from typing import TYPE_CHECKING, List
 
 from mosec.ipc import IPCWrapper
```

### Comparing `mosec-0.6.6/mosec/protocol.py` & `mosec-0.6.7/mosec/protocol.py`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/mosec/server.py` & `mosec-0.6.7/mosec/server.py`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/mosec/worker.py` & `mosec-0.6.7/mosec/worker.py`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/mosec.egg-info/PKG-INFO` & `mosec-0.6.7/mosec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: mosec
-Version: 0.6.6
+Version: 0.6.7
 Summary: Model Serving made Efficient in the Cloud.
 Home-page: https://github.com/mosecorg/mosec
 Author: Keming Yang
 Author-email: kemingy94@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: plugin
+Provides-Extra: mixin
 Provides-Extra: doc
 License-File: LICENSE
 
 <p align="center">
   <img src="https://user-images.githubusercontent.com/38581401/134487662-49733d45-2ba0-4c19-aa07-1f43fd35c453.png" height="230" alt="MOSEC" />
 </p>
 
@@ -175,14 +175,15 @@
 That's it! You have just hosted your **_stable-diffusion model_** as a service! 😉
 
 ## Examples
 
 More ready-to-use examples can be found in the [Example](https://mosecorg.github.io/mosec/examples/index.html) section. It includes:
 
 - [Multi-stage workflow demo](https://mosecorg.github.io/mosec/examples/echo.html): a simple echo demo even without any ML model.
+- [Request validation](https://mosecorg.github.io/mosec/examples/validate.html): validate the request with type annotation.
 - [Shared memory IPC](https://mosecorg.github.io/mosec/examples/ipc.html): inter-process communication with shared memory.
 - [Customized GPU allocation](https://mosecorg.github.io/mosec/examples/env.html): deploy multiple replicas, each using different GPUs.
 - [Customized metrics](https://mosecorg.github.io/mosec/examples/metric.html): record your own metrics for monitoring.
 - [Jax jitted inference](https://mosecorg.github.io/mosec/examples/jax.html): just-in-time compilation speeds up the inference.
 - PyTorch deep learning models:
   - [sentiment analysis](https://mosecorg.github.io/mosec/examples/pytorch.html#natural-language-processing): infer the sentiment of a sentence.
   - [image recognition](https://mosecorg.github.io/mosec/examples/pytorch.html#computer-vision): categorize a given image.
@@ -209,15 +210,16 @@
 - Stop the service with `SIGINT` or `SIGTERM` since it has the graceful shutdown logic.
 
 ## Adopters
 
 Here are some of the companies and individual users that are using Mosec:
 
 - [Modelz](https://modelz.ai): Serverless platform for ML inference.
-- [MOSS](https://github.com/OpenLMLab/MOSS/): An open sourced conversational language model like ChatGPT.
+- [MOSS](https://github.com/OpenLMLab/MOSS/blob/main/README_en.md): An open sourced conversational language model like ChatGPT.
+- [TencentCloud](https://www.tencentcloud.com/document/product/1141/45261): Tencent Cloud Machine Learning Platform, using Mosec as the [core inference server framework](https://cloud.tencent.com/document/product/851/74148).
 - [TensorChord](https://github.com/tensorchord): Cloud native AI infrastructure company.
 
 ## Citation
 
 If you find this software useful for your research, please consider citing
 
 ```
```

### Comparing `mosec-0.6.6/mosec.egg-info/SOURCES.txt` & `mosec-0.6.7/mosec.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 docs/source/examples/env.md
 docs/source/examples/index.md
 docs/source/examples/ipc.md
 docs/source/examples/jax.md
 docs/source/examples/metric.md
 docs/source/examples/pytorch.md
 docs/source/examples/stable_diffusion.md
+docs/source/examples/validate.md
 docs/source/reference/arguments.md
 docs/source/reference/index.md
 docs/source/reference/interface.md
 mosec/__init__.py
 mosec/_version.py
 mosec/args.py
 mosec/coordinator.py
@@ -52,19 +53,21 @@
 mosec.egg-info/dependency_links.txt
 mosec.egg-info/not-zip-safe
 mosec.egg-info/requires.txt
 mosec.egg-info/top_level.txt
 mosec/mixin/__init__.py
 mosec/mixin/msgpack_worker.py
 mosec/mixin/numbin_worker.py
+mosec/mixin/plasma_worker.py
+mosec/mixin/typed_worker.py
 mosec/plugins/__init__.py
 mosec/plugins/plasma_shm.py
 requirements/dev.txt
 requirements/doc.txt
-requirements/plugin.txt
+requirements/mixin.txt
 src/args.rs
 src/coordinator.rs
 src/errors.rs
 src/main.rs
 src/metrics.rs
 src/protocol.rs
 src/tasks.rs
```

### Comparing `mosec-0.6.6/pyproject.toml` & `mosec-0.6.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 requires-python = ">=3.6"
 classifiers = [
     "Environment :: GPU",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Rust",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
@@ -56,15 +55,15 @@
 [tool.mypy]
 warn_redundant_casts = true
 warn_unreachable = true
 pretty = true
 
 [tool.pyright]
 pythonPlatform = "All"
-pythonVersion = "3.7"
+pythonVersion = "3.8"
 include = ["mosec", "tests", "examples"]
 
 [tool.isort]
 profile = "black"
 
 [tool.pylint.master]
 load-plugins = "pylint.extensions.docparams,pylint.extensions.docstyle,pylint.extensions.no_self_use"
```

### Comparing `mosec-0.6.6/setup.py` & `mosec-0.6.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 with open(os.path.join(here, "requirements/dev.txt"), encoding="utf-8") as f:
     dev_requirements = f.read().splitlines()
 
 with open(os.path.join(here, "requirements/doc.txt"), encoding="utf-8") as f:
     doc_requirements = f.read().splitlines()
 
-with open(os.path.join(here, "requirements/plugin.txt"), encoding="utf-8") as f:
-    plugin_requirements = f.read().splitlines()
+with open(os.path.join(here, "requirements/mixin.txt"), encoding="utf-8") as f:
+    mixin_requirements = f.read().splitlines()
 
 
 class RustExtension(Extension):
     """Custom Extension class for rust"""
 
 
 ext_modules = []
@@ -76,18 +76,18 @@
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/mosecorg/mosec",
     license="Apache License 2.0",
     use_scm_version=True,
     packages=find_packages(exclude=["examples*", "tests*"]),
     include_package_data=True,
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     setup_requires=["setuptools_scm>=7.0"],
     extras_require={
         "dev": dev_requirements,
-        "plugin": plugin_requirements,
+        "mixin": mixin_requirements,
         "doc": doc_requirements,
     },
     zip_safe=False,
     ext_modules=ext_modules,  # type: ignore
     cmdclass=dict(build_ext=RustBuildExt),  # type: ignore
 )
```

### Comparing `mosec-0.6.6/src/args.rs` & `mosec-0.6.7/src/args.rs`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/src/coordinator.rs` & `mosec-0.6.7/src/coordinator.rs`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/src/errors.rs` & `mosec-0.6.7/src/errors.rs`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/src/main.rs` & `mosec-0.6.7/src/main.rs`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/src/metrics.rs` & `mosec-0.6.7/src/metrics.rs`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/src/protocol.rs` & `mosec-0.6.7/src/protocol.rs`

 * *Files identical despite different names*

### Comparing `mosec-0.6.6/src/tasks.rs` & `mosec-0.6.7/src/tasks.rs`

 * *Files identical despite different names*

