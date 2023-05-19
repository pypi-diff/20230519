# Comparing `tmp/streamingcli-1.9.0.tar.gz` & `tmp/streamingcli-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamingcli-1.9.0.tar", last modified: Wed Mar  1 13:33:21 2023, max compression
+gzip compressed data, was "streamingcli-1.9.1.tar", last modified: Thu Mar  2 10:16:59 2023, max compression
```

## Comparing `streamingcli-1.9.0.tar` & `streamingcli-1.9.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:21.001145 streamingcli-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-01 13:33:14.000000 streamingcli-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-01 13:33:14.000000 streamingcli-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-03-01 13:33:21.001145 streamingcli-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-03-01 13:33:14.000000 streamingcli-1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-03-01 13:33:20.000000 streamingcli-1.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-03-01 13:33:21.001145 streamingcli-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-03-01 13:33:14.000000 streamingcli-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:20.993145 streamingcli-1.9.0/streamingcli/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:20.993145 streamingcli-1.9.0/streamingcli/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/docker/login_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/docker_response_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:20.993145 streamingcli-1.9.0/streamingcli/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/jupyter/jar_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/jupyter/notebook_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:20.993145 streamingcli-1.9.0/streamingcli/platform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/platform/apitoken_create_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/platform/apitoken_remove_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/platform/deployment_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/platform/deployment_target_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:20.997145 streamingcli-1.9.0/streamingcli/platform/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/platform/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/platform/k8s/config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/platform/k8s/deployment_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/platform/k8s/secret_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:20.997145 streamingcli-1.9.0/streamingcli/platform/ververica/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/platform/ververica/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/platform/ververica/apitoken_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/platform/ververica/deployment_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/platform/ververica/deployment_target_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:20.997145 streamingcli-1.9.0/streamingcli/profile/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/profile/profile_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/profile/profile_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:20.997145 streamingcli-1.9.0/streamingcli/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/project/build_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/project/cicd_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/project/deploy_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:20.997145 streamingcli-1.9.0/streamingcli/project/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/project/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/project/jupyter/jupyter_project_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/project/local_project_config.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/project/project_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/project/publish_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:20.997145 streamingcli-1.9.0/streamingcli/project/python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/project/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/project/python/python_project_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/project/template_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:20.997145 streamingcli-1.9.0/streamingcli/project/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/project/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/project/templates/deployment_target.yml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/project/templates/flink_app.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/project/templates/gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/project/templates/k8s_flink_deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/project/templates/vvp_flink_deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-01 13:33:14.000000 streamingcli-1.9.0/streamingcli/project/yaml_merger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:20.993145 streamingcli-1.9.0/streamingcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-03-01 13:33:20.000000 streamingcli-1.9.0/streamingcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-03-01 13:33:20.000000 streamingcli-1.9.0/streamingcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 13:33:20.000000 streamingcli-1.9.0/streamingcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-01 13:33:20.000000 streamingcli-1.9.0/streamingcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-03-01 13:33:20.000000 streamingcli-1.9.0/streamingcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-01 13:33:20.000000 streamingcli-1.9.0/streamingcli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:20.997145 streamingcli-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:14.000000 streamingcli-1.9.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:20.997145 streamingcli-1.9.0/tests/streamingcli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:14.000000 streamingcli-1.9.0/tests/streamingcli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:21.001145 streamingcli-1.9.0/tests/streamingcli/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:14.000000 streamingcli-1.9.0/tests/streamingcli/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-03-01 13:33:14.000000 streamingcli-1.9.0/tests/streamingcli/jupyter/test_notebook_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:21.001145 streamingcli-1.9.0/tests/streamingcli/profile/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:14.000000 streamingcli-1.9.0/tests/streamingcli/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-03-01 13:33:14.000000 streamingcli-1.9.0/tests/streamingcli/profile/test_profile_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:21.001145 streamingcli-1.9.0/tests/streamingcli/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:33:14.000000 streamingcli-1.9.0/tests/streamingcli/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-01 13:33:14.000000 streamingcli-1.9.0/tests/streamingcli/project/test_yaml_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-03-01 13:33:14.000000 streamingcli-1.9.0/tests/streamingcli/test_k82_deployment_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-01 13:33:14.000000 streamingcli-1.9.0/tests/streamingcli/test_k8s_secret_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.856937 streamingcli-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-02 10:16:53.000000 streamingcli-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-02 10:16:53.000000 streamingcli-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-03-02 10:16:59.856937 streamingcli-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-03-02 10:16:53.000000 streamingcli-1.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-03-02 10:16:59.000000 streamingcli-1.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-03-02 10:16:59.856937 streamingcli-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-03-02 10:16:53.000000 streamingcli-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.848937 streamingcli-1.9.1/streamingcli/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.848937 streamingcli-1.9.1/streamingcli/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/docker/login_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/docker_response_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.852937 streamingcli-1.9.1/streamingcli/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/jupyter/jar_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/jupyter/notebook_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.852937 streamingcli-1.9.1/streamingcli/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/apitoken_create_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/apitoken_remove_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/deployment_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/deployment_target_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.852937 streamingcli-1.9.1/streamingcli/platform/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/k8s/config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/k8s/deployment_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/k8s/secret_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.852937 streamingcli-1.9.1/streamingcli/platform/ververica/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/ververica/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/ververica/apitoken_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/ververica/deployment_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/platform/ververica/deployment_target_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.852937 streamingcli-1.9.1/streamingcli/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/profile/profile_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/profile/profile_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.852937 streamingcli-1.9.1/streamingcli/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/build_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/cicd_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/deploy_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.852937 streamingcli-1.9.1/streamingcli/project/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/jupyter/jupyter_project_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/local_project_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/project_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/publish_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.852937 streamingcli-1.9.1/streamingcli/project/python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/python/python_project_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/template_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.856937 streamingcli-1.9.1/streamingcli/project/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/templates/deployment_target.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/templates/flink_app.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/templates/gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/templates/k8s_flink_deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/templates/vvp_flink_deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-02 10:16:53.000000 streamingcli-1.9.1/streamingcli/project/yaml_merger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.848937 streamingcli-1.9.1/streamingcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-03-02 10:16:59.000000 streamingcli-1.9.1/streamingcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-03-02 10:16:59.000000 streamingcli-1.9.1/streamingcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 10:16:59.000000 streamingcli-1.9.1/streamingcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-02 10:16:59.000000 streamingcli-1.9.1/streamingcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-03-02 10:16:59.000000 streamingcli-1.9.1/streamingcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-02 10:16:59.000000 streamingcli-1.9.1/streamingcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.856937 streamingcli-1.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.856937 streamingcli-1.9.1/tests/streamingcli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/tests/streamingcli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.856937 streamingcli-1.9.1/tests/streamingcli/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/tests/streamingcli/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-03-02 10:16:53.000000 streamingcli-1.9.1/tests/streamingcli/jupyter/test_notebook_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.856937 streamingcli-1.9.1/tests/streamingcli/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/tests/streamingcli/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-03-02 10:16:53.000000 streamingcli-1.9.1/tests/streamingcli/profile/test_profile_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:59.856937 streamingcli-1.9.1/tests/streamingcli/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:16:53.000000 streamingcli-1.9.1/tests/streamingcli/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-02 10:16:53.000000 streamingcli-1.9.1/tests/streamingcli/project/test_yaml_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-03-02 10:16:53.000000 streamingcli-1.9.1/tests/streamingcli/test_k82_deployment_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-02 10:16:53.000000 streamingcli-1.9.1/tests/streamingcli/test_k8s_secret_validation.py
```

### Comparing `streamingcli-1.9.0/LICENSE` & `streamingcli-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/PKG-INFO` & `streamingcli-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamingcli
-Version: 1.9.0
+Version: 1.9.1
 Summary: Streaming platform CLI
 Home-page: https://github.com/getindata/streaming-cli
 Author: GetInData
 Author-email: office@getindata.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `streamingcli-1.9.0/README.md` & `streamingcli-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/requirements.txt` & `streamingcli-1.9.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/setup.cfg` & `streamingcli-1.9.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.9.0
+current_version = 1.9.1
 
 [flake8]
 exclude = .git,__pycache__,build,dist,*.yml
 max-line-length = 120
 extend-ignore = E203
 
 [mypy]
```

### Comparing `streamingcli-1.9.0/setup.py` & `streamingcli-1.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 from typing import List
 
 from setuptools import find_packages, setup
 from setuptools.command.install import install
 
-__version__ = "1.9.0"
+__version__ = "1.9.1"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 def get_requirements(filename: str) -> List[str]:
     with open(filename, "r", encoding="utf-8") as fp:
```

### Comparing `streamingcli-1.9.0/streamingcli/config.py` & `streamingcli-1.9.1/streamingcli/config.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/docker/login_command.py` & `streamingcli-1.9.1/streamingcli/docker/login_command.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/docker_response_reader.py` & `streamingcli-1.9.1/streamingcli/docker_response_reader.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/jupyter/jar_handler.py` & `streamingcli-1.9.1/streamingcli/jupyter/jar_handler.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/jupyter/notebook_converter.py` & `streamingcli-1.9.1/streamingcli/jupyter/notebook_converter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/main.py` & `streamingcli-1.9.1/streamingcli/main.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/platform/apitoken_create_command.py` & `streamingcli-1.9.1/streamingcli/platform/apitoken_create_command.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/platform/deployment_adapter.py` & `streamingcli-1.9.1/streamingcli/platform/deployment_adapter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/platform/deployment_target_command.py` & `streamingcli-1.9.1/streamingcli/platform/deployment_target_command.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/platform/k8s/config_loader.py` & `streamingcli-1.9.1/streamingcli/platform/k8s/config_loader.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/platform/k8s/deployment_adapter.py` & `streamingcli-1.9.1/streamingcli/platform/k8s/deployment_adapter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/platform/k8s/secret_adapter.py` & `streamingcli-1.9.1/streamingcli/platform/k8s/secret_adapter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/platform/ververica/apitoken_adapter.py` & `streamingcli-1.9.1/streamingcli/platform/ververica/apitoken_adapter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/platform/ververica/deployment_adapter.py` & `streamingcli-1.9.1/streamingcli/platform/ververica/deployment_adapter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/platform/ververica/deployment_target_adapter.py` & `streamingcli-1.9.1/streamingcli/platform/ververica/deployment_target_adapter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/profile/profile_adapter.py` & `streamingcli-1.9.1/streamingcli/profile/profile_adapter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/profile/profile_command.py` & `streamingcli-1.9.1/streamingcli/profile/profile_command.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/project/build_command.py` & `streamingcli-1.9.1/streamingcli/project/build_command.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/project/cicd_command.py` & `streamingcli-1.9.1/streamingcli/project/cicd_command.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/project/deploy_command.py` & `streamingcli-1.9.1/streamingcli/project/deploy_command.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/project/jupyter/jupyter_project_factory.py` & `streamingcli-1.9.1/streamingcli/project/jupyter/jupyter_project_factory.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/project/local_project_config.py` & `streamingcli-1.9.1/streamingcli/project/local_project_config.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/project/publish_command.py` & `streamingcli-1.9.1/streamingcli/project/publish_command.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/project/python/python_project_factory.py` & `streamingcli-1.9.1/streamingcli/project/python/python_project_factory.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/project/template_loader.py` & `streamingcli-1.9.1/streamingcli/project/template_loader.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/project/templates/flink_app.py.template` & `streamingcli-1.9.1/streamingcli/project/templates/flink_app.py.template`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/project/templates/gitlab-ci.yml` & `streamingcli-1.9.1/streamingcli/project/templates/gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/project/templates/k8s_flink_deployment.yml` & `streamingcli-1.9.1/streamingcli/project/templates/k8s_flink_deployment.yml`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli/project/templates/vvp_flink_deployment.yml` & `streamingcli-1.9.1/streamingcli/project/templates/vvp_flink_deployment.yml`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli.egg-info/PKG-INFO` & `streamingcli-1.9.1/streamingcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamingcli
-Version: 1.9.0
+Version: 1.9.1
 Summary: Streaming platform CLI
 Home-page: https://github.com/getindata/streaming-cli
 Author: GetInData
 Author-email: office@getindata.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `streamingcli-1.9.0/streamingcli.egg-info/SOURCES.txt` & `streamingcli-1.9.1/streamingcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/streamingcli.egg-info/requires.txt` & `streamingcli-1.9.1/streamingcli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/tests/streamingcli/jupyter/test_notebook_converter.py` & `streamingcli-1.9.1/tests/streamingcli/jupyter/test_notebook_converter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/tests/streamingcli/profile/test_profile_adapter.py` & `streamingcli-1.9.1/tests/streamingcli/profile/test_profile_adapter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/tests/streamingcli/test_k82_deployment_adapter.py` & `streamingcli-1.9.1/tests/streamingcli/test_k82_deployment_adapter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-1.9.0/tests/streamingcli/test_k8s_secret_validation.py` & `streamingcli-1.9.1/tests/streamingcli/test_k8s_secret_validation.py`

 * *Files identical despite different names*

