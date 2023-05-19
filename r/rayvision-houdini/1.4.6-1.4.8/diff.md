# Comparing `tmp/rayvision_houdini-1.4.6.tar.gz` & `tmp/rayvision_houdini-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rayvision_houdini-1.4.6.tar", last modified: Wed May 10 11:37:35 2023, max compression
+gzip compressed data, was "dist/rayvision_houdini-1.4.8.tar", last modified: Fri May 19 10:14:21 2023, max compression
```

## Comparing `rayvision_houdini-1.4.6.tar` & `rayvision_houdini-1.4.8.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:37:35.000000 rayvision_houdini-1.4.6/
--rw-rw-rw-   0 root         (0) root         (0)      252 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.6/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      187 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.6/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1121 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.6/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      259 2022-09-06 06:16:59.000000 rayvision_houdini-1.4.6/.pylintrc
--rw-r--r--   0 root         (0) root         (0)      472 2023-05-10 11:37:35.000000 rayvision_houdini-1.4.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      664 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)       44 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.6/dev_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:37:35.000000 rayvision_houdini-1.4.6/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.6/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     5357 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.6/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.6/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      760 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.6/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:37:35.000000 rayvision_houdini-1.4.6/docs/rayvision_houdini/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:37:35.000000 rayvision_houdini-1.4.6/docs/rayvision_houdini/core/
--rw-rw-rw-   0 root         (0) root         (0)      141 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.6/docs/rayvision_houdini/core/cg.rst
--rw-rw-rw-   0 root         (0) root         (0)      296 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.6/docs/rayvision_houdini/core/constants.rst
--rw-rw-rw-   0 root         (0) root         (0)     5108 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.6/docs/rayvision_houdini/first_look.rst
--rw-rw-rw-   0 root         (0) root         (0)      854 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.6/docs/rayvision_houdini/installation_guide.rst
--rw-rw-rw-   0 root         (0) root         (0)      128 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.6/docs/rayvision_houdini/modules.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:37:35.000000 rayvision_houdini-1.4.6/help/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.6/help/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:37:35.000000 rayvision_houdini-1.4.6/help/doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:37:35.000000 rayvision_houdini-1.4.6/help/doc/docs/
--rw-rw-rw-   0 root         (0) root         (0)     8755 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.6/help/doc/docs/Configuration Documentation--Maya.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:37:35.000000 rayvision_houdini-1.4.6/help/doc/docs_zh/
--rw-rw-rw-   0 root         (0) root         (0)     8250 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.6/help/doc/docs_zh/配置文件文档之Maya.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:37:35.000000 rayvision_houdini-1.4.6/help/examples/
--rw-rw-rw-   0 root         (0) root         (0)     3338 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.6/help/examples/houdini_demo.py
--rw-rw-rw-   0 root         (0) root         (0)      432 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.6/help/examples/only_analyze.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:37:35.000000 rayvision_houdini-1.4.6/help/scenes/
--rw-rw-rw-   0 root         (0) root         (0)   277555 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.6/help/scenes/sphere.hip
--rw-rw-rw-   0 root         (0) root         (0)      452 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.6/init_pycharm_setup.cmd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:37:35.000000 rayvision_houdini-1.4.6/rayvision_houdini/
--rw-rw-rw-   0 root         (0) root         (0)      449 2022-09-06 06:16:59.000000 rayvision_houdini-1.4.6/rayvision_houdini/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15977 2023-04-23 06:59:02.000000 rayvision_houdini-1.4.6/rayvision_houdini/analyze_houdini.py
--rw-rw-rw-   0 root         (0) root         (0)       82 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.6/rayvision_houdini/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:37:35.000000 rayvision_houdini-1.4.6/rayvision_houdini/hanalyse/
--rw-rw-rw-   0 root         (0) root         (0)      498 2022-09-06 06:09:27.000000 rayvision_houdini-1.4.6/rayvision_houdini/hanalyse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:37:35.000000 rayvision_houdini-1.4.6/rayvision_houdini/hanalyse/py27/
--rw-rw-rw-   0 root         (0) root         (0)       12 2022-09-06 03:41:48.000000 rayvision_houdini-1.4.6/rayvision_houdini/hanalyse/py27/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   601600 2023-05-10 11:23:49.000000 rayvision_houdini-1.4.6/rayvision_houdini/hanalyse/py27/hanalyse.pyd
--rw-rw-rw-   0 root         (0) root         (0)  4217104 2023-05-10 11:23:49.000000 rayvision_houdini-1.4.6/rayvision_houdini/hanalyse/py27/hanalyse.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:37:35.000000 rayvision_houdini-1.4.6/rayvision_houdini/hanalyse/py37/
--rw-rw-rw-   0 root         (0) root         (0)       12 2022-09-06 03:41:48.000000 rayvision_houdini-1.4.6/rayvision_houdini/hanalyse/py37/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   575488 2023-05-10 11:23:49.000000 rayvision_houdini-1.4.6/rayvision_houdini/hanalyse/py37/hanalyse.pyd
--rw-rw-rw-   0 root         (0) root         (0)  5355088 2023-05-10 11:23:49.000000 rayvision_houdini-1.4.6/rayvision_houdini/hanalyse/py37/hanalyse.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:37:35.000000 rayvision_houdini-1.4.6/rayvision_houdini/hanalyse/py39/
--rw-rw-rw-   0 root         (0) root         (0)       12 2022-09-06 03:41:48.000000 rayvision_houdini-1.4.6/rayvision_houdini/hanalyse/py39/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   579584 2023-05-10 11:23:49.000000 rayvision_houdini-1.4.6/rayvision_houdini/hanalyse/py39/hanalyse.pyd
--rw-rw-rw-   0 root         (0) root         (0)  5511584 2023-05-10 11:23:50.000000 rayvision_houdini-1.4.6/rayvision_houdini/hanalyse/py39/hanalyse.so
--rw-rw-rw-   0 root         (0) root         (0)      787 2022-09-06 04:23:37.000000 rayvision_houdini-1.4.6/rayvision_houdini/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:37:35.000000 rayvision_houdini-1.4.6/rayvision_houdini/tests/
--rw-rw-rw-   0 root         (0) root         (0)       39 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.6/rayvision_houdini/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      803 2022-09-06 03:45:31.000000 rayvision_houdini-1.4.6/rayvision_houdini/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      949 2022-09-06 06:16:59.000000 rayvision_houdini-1.4.6/rayvision_houdini/tests/test_analyze_houdini.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:37:35.000000 rayvision_houdini-1.4.6/rayvision_houdini.egg-info/
--rw-r--r--   0 root         (0) root         (0)      472 2023-05-10 11:37:35.000000 rayvision_houdini-1.4.6/rayvision_houdini.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1946 2023-05-10 11:37:35.000000 rayvision_houdini-1.4.6/rayvision_houdini.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 11:37:35.000000 rayvision_houdini-1.4.6/rayvision_houdini.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-10 11:37:35.000000 rayvision_houdini-1.4.6/rayvision_houdini.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-10 11:37:35.000000 rayvision_houdini-1.4.6/rayvision_houdini.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-04-28 04:38:46.000000 rayvision_houdini-1.4.6/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-10 11:37:35.000000 rayvision_houdini-1.4.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1057 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.6/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     3073 2023-05-05 06:19:19.000000 rayvision_houdini-1.4.6/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:14:21.000000 rayvision_houdini-1.4.8/
+-rw-rw-rw-   0 root         (0) root         (0)      252 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.8/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      187 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.8/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.8/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      259 2022-09-06 06:16:59.000000 rayvision_houdini-1.4.8/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)      472 2023-05-19 10:14:21.000000 rayvision_houdini-1.4.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      664 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       44 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.8/dev_requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:14:21.000000 rayvision_houdini-1.4.8/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.8/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     5357 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.8/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.8/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      760 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.8/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:14:21.000000 rayvision_houdini-1.4.8/docs/rayvision_houdini/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:14:21.000000 rayvision_houdini-1.4.8/docs/rayvision_houdini/core/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.8/docs/rayvision_houdini/core/cg.rst
+-rw-rw-rw-   0 root         (0) root         (0)      296 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.8/docs/rayvision_houdini/core/constants.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5108 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.8/docs/rayvision_houdini/first_look.rst
+-rw-rw-rw-   0 root         (0) root         (0)      854 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.8/docs/rayvision_houdini/installation_guide.rst
+-rw-rw-rw-   0 root         (0) root         (0)      128 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.8/docs/rayvision_houdini/modules.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:14:21.000000 rayvision_houdini-1.4.8/help/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.8/help/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:14:21.000000 rayvision_houdini-1.4.8/help/doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:14:21.000000 rayvision_houdini-1.4.8/help/doc/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     8755 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.8/help/doc/docs/Configuration Documentation--Maya.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:14:21.000000 rayvision_houdini-1.4.8/help/doc/docs_zh/
+-rw-rw-rw-   0 root         (0) root         (0)     8250 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.8/help/doc/docs_zh/配置文件文档之Maya.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:14:21.000000 rayvision_houdini-1.4.8/help/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     3338 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.8/help/examples/houdini_demo.py
+-rw-rw-rw-   0 root         (0) root         (0)      432 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.8/help/examples/only_analyze.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:14:21.000000 rayvision_houdini-1.4.8/help/scenes/
+-rw-rw-rw-   0 root         (0) root         (0)   277555 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.8/help/scenes/sphere.hip
+-rw-rw-rw-   0 root         (0) root         (0)      452 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.8/init_pycharm_setup.cmd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:14:21.000000 rayvision_houdini-1.4.8/rayvision_houdini/
+-rw-rw-rw-   0 root         (0) root         (0)      449 2022-09-06 06:16:59.000000 rayvision_houdini-1.4.8/rayvision_houdini/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15384 2023-05-19 09:43:05.000000 rayvision_houdini-1.4.8/rayvision_houdini/analyze_houdini.py
+-rw-rw-rw-   0 root         (0) root         (0)       82 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.8/rayvision_houdini/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:14:21.000000 rayvision_houdini-1.4.8/rayvision_houdini/hanalyse/
+-rw-rw-rw-   0 root         (0) root         (0)      498 2022-09-06 06:09:27.000000 rayvision_houdini-1.4.8/rayvision_houdini/hanalyse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:14:21.000000 rayvision_houdini-1.4.8/rayvision_houdini/hanalyse/py27/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2022-09-06 03:41:48.000000 rayvision_houdini-1.4.8/rayvision_houdini/hanalyse/py27/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   612864 2023-05-19 09:43:05.000000 rayvision_houdini-1.4.8/rayvision_houdini/hanalyse/py27/hanalyse.pyd
+-rw-rw-rw-   0 root         (0) root         (0)  4217104 2023-05-10 11:23:49.000000 rayvision_houdini-1.4.8/rayvision_houdini/hanalyse/py27/hanalyse.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:14:21.000000 rayvision_houdini-1.4.8/rayvision_houdini/hanalyse/py37/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2022-09-06 03:41:48.000000 rayvision_houdini-1.4.8/rayvision_houdini/hanalyse/py37/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   561664 2023-05-19 09:43:05.000000 rayvision_houdini-1.4.8/rayvision_houdini/hanalyse/py37/hanalyse.pyd
+-rw-rw-rw-   0 root         (0) root         (0)  5355088 2023-05-10 11:23:49.000000 rayvision_houdini-1.4.8/rayvision_houdini/hanalyse/py37/hanalyse.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:14:21.000000 rayvision_houdini-1.4.8/rayvision_houdini/hanalyse/py39/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2022-09-06 03:41:48.000000 rayvision_houdini-1.4.8/rayvision_houdini/hanalyse/py39/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   564224 2023-05-19 09:43:05.000000 rayvision_houdini-1.4.8/rayvision_houdini/hanalyse/py39/hanalyse.pyd
+-rw-rw-rw-   0 root         (0) root         (0)  5511584 2023-05-10 11:23:50.000000 rayvision_houdini-1.4.8/rayvision_houdini/hanalyse/py39/hanalyse.so
+-rw-rw-rw-   0 root         (0) root         (0)      787 2022-09-06 04:23:37.000000 rayvision_houdini-1.4.8/rayvision_houdini/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:14:21.000000 rayvision_houdini-1.4.8/rayvision_houdini/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.8/rayvision_houdini/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      803 2022-09-06 03:45:31.000000 rayvision_houdini-1.4.8/rayvision_houdini/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      849 2023-05-19 09:50:53.000000 rayvision_houdini-1.4.8/rayvision_houdini/tests/test_analyze_houdini.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:14:21.000000 rayvision_houdini-1.4.8/rayvision_houdini.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      472 2023-05-19 10:14:21.000000 rayvision_houdini-1.4.8/rayvision_houdini.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-05-19 10:14:21.000000 rayvision_houdini-1.4.8/rayvision_houdini.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 10:14:21.000000 rayvision_houdini-1.4.8/rayvision_houdini.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-19 10:14:21.000000 rayvision_houdini-1.4.8/rayvision_houdini.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-19 10:14:21.000000 rayvision_houdini-1.4.8/rayvision_houdini.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-04-28 04:38:46.000000 rayvision_houdini-1.4.8/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-19 10:14:21.000000 rayvision_houdini-1.4.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.8/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     3073 2023-05-05 06:19:19.000000 rayvision_houdini-1.4.8/tox.ini
```

### Comparing `rayvision_houdini-1.4.6/.pre-commit-config.yaml` & `rayvision_houdini-1.4.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.6/README.md` & `rayvision_houdini-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.6/docs/Makefile` & `rayvision_houdini-1.4.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.6/docs/conf.py` & `rayvision_houdini-1.4.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.6/docs/index.rst` & `rayvision_houdini-1.4.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.6/docs/make.bat` & `rayvision_houdini-1.4.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.6/docs/rayvision_houdini/first_look.rst` & `rayvision_houdini-1.4.8/docs/rayvision_houdini/first_look.rst`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.6/docs/rayvision_houdini/installation_guide.rst` & `rayvision_houdini-1.4.8/docs/rayvision_houdini/installation_guide.rst`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.6/help/doc/docs/Configuration Documentation--Maya.md` & `rayvision_houdini-1.4.8/help/doc/docs/Configuration Documentation--Maya.md`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.6/help/doc/docs_zh/配置文件文档之Maya.md` & `rayvision_houdini-1.4.8/help/doc/docs_zh/配置文件文档之Maya.md`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.6/help/examples/houdini_demo.py` & `rayvision_houdini-1.4.8/help/examples/houdini_demo.py`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.6/help/scenes/sphere.hip` & `rayvision_houdini-1.4.8/help/scenes/sphere.hip`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.6/rayvision_houdini/hanalyse/py27/hanalyse.so` & `rayvision_houdini-1.4.8/rayvision_houdini/hanalyse/py27/hanalyse.so`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.6/rayvision_houdini/hanalyse/py37/hanalyse.so` & `rayvision_houdini-1.4.8/rayvision_houdini/hanalyse/py37/hanalyse.so`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.6/rayvision_houdini/hanalyse/py39/hanalyse.so` & `rayvision_houdini-1.4.8/rayvision_houdini/hanalyse/py39/hanalyse.so`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.6/rayvision_houdini/run.py` & `rayvision_houdini-1.4.8/rayvision_houdini/run.py`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.6/rayvision_houdini/tests/conftest.py` & `rayvision_houdini-1.4.8/rayvision_houdini/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.6/rayvision_houdini/tests/test_analyze_houdini.py` & `rayvision_houdini-1.4.8/rayvision_houdini/tests/test_analyze_houdini.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,22 +8,21 @@
     https://docs.pytest.org/en/2.7.3/plugins.html
 
 """
 
 import pytest
 
 from rayvision_houdini.analyze_houdini import AnalyzeHoudini
-from rayvision_utils.exception.exception import CGFileNotExistsError
+from rayvision_utils.exception.exception import CGExeNotExistError
 
 
-def test_get_save_version(houdini, cg_file_h):
+def test_get_save_version(houdini):
     """Test get_save_version function."""
-    # result = houdini.get_save_version(cg_file_h["cg_file"])
-    with pytest.raises(CGFileNotExistsError):
-        houdini.get_save_version(cg_file_h["cg_file"])
+    with pytest.raises(CGExeNotExistError):
+        houdini.find_location()
 
 
 def test_find_location(houdini, mocker, tmpdir):
     """Test find_location action."""
     mocker_cg_file = mocker.patch.object(AnalyzeHoudini, 'find_location')
     mocker_cg_file.return_value = tmpdir.join('muti_layer_test.hip')
     assert houdini.find_location() == str(tmpdir.join('muti_layer_test.hip'))
```

### Comparing `rayvision_houdini-1.4.6/rayvision_houdini.egg-info/SOURCES.txt` & `rayvision_houdini-1.4.8/rayvision_houdini.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.6/setup.py` & `rayvision_houdini-1.4.8/setup.py`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.6/tox.ini` & `rayvision_houdini-1.4.8/tox.ini`

 * *Files identical despite different names*

