# Comparing `tmp/loko-cli-0.0.4.tar.gz` & `tmp/loko-cli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loko-cli-0.0.4.tar", last modified: Fri Apr  7 10:50:57 2023, max compression
+gzip compressed data, was "loko-cli-0.0.5.tar", last modified: Fri May 19 10:31:48 2023, max compression
```

## Comparing `loko-cli-0.0.4.tar` & `loko-cli-0.0.5.tar`

### file list

```diff
@@ -1,77 +1,79 @@
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-04-07 10:50:57.171879 loko-cli-0.0.4/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)       57 2023-01-18 12:14:39.000000 loko-cli-0.0.4/MANIFEST.in
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      318 2023-04-07 10:50:57.171879 loko-cli-0.0.4/PKG-INFO
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-04-07 10:50:57.163879 loko-cli-0.0.4/loko_cli/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/__init__.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-04-07 10:50:57.167879 loko-cli-0.0.4/loko_cli/apps/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/apps/__init__.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     2518 2023-04-07 10:07:23.000000 loko-cli-0.0.4/loko_cli/apps/cl.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     6005 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/apps/loko_project_deploy.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     3109 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/apps/loko_project_planning.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      124 2023-01-19 16:12:55.000000 loko-cli-0.0.4/loko_cli/apps/modify_a_container.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     3082 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/apps/prova_extensions.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      646 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/apps/prova_push.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     2799 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/apps/provaceci.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     2505 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/apps/provakubedepl.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     2358 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/apps/provaorch.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)    16002 2023-04-07 10:04:57.000000 loko-cli-0.0.4/loko_cli/apps/total.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      664 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/apps/volumes.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-04-07 10:50:57.167879 loko-cli-0.0.4/loko_cli/business/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/business/__init__.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-04-07 10:50:57.167879 loko-cli-0.0.4/loko_cli/business/deployment/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/business/deployment/__init__.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-04-07 10:50:57.167879 loko-cli-0.0.4/loko_cli/business/deployment/appliers/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/business/deployment/appliers/__init__.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      178 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/business/deployment/appliers/appliers.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      149 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/business/deployment/appliers/dcapplier2.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     5708 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/business/deployment/appliers/docker_compose_applier.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-04-07 10:50:57.167879 loko-cli-0.0.4/loko_cli/business/deployment/cloud/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/business/deployment/cloud/__init__.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     5758 2023-04-07 09:57:46.000000 loko-cli-0.0.4/loko_cli/business/deployment/cloud/ec2.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-04-07 10:50:57.167879 loko-cli-0.0.4/loko_cli/business/deployment/planners/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/business/deployment/planners/__init__.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     4695 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/business/deployment/planners/docker_compose_planner.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      537 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/business/deployment/planners/planners.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      717 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/business/deployment/planners/provagendc.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-04-07 10:50:57.167879 loko-cli-0.0.4/loko_cli/business/docker/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/business/docker/__init__.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)    14375 2023-03-31 07:55:08.000000 loko-cli-0.0.4/loko_cli/business/docker/dockermanager.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     1546 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/business/docker/log_collector.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     1047 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/business/docker/utils.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-04-07 10:50:57.167879 loko-cli-0.0.4/loko_cli/config/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/config/__init__.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/config/app_config.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     2081 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/config/app_init.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-04-07 10:50:57.167879 loko-cli-0.0.4/loko_cli/dao/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/dao/__init__.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      905 2023-01-19 13:08:33.000000 loko-cli-0.0.4/loko_cli/dao/loko.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-04-07 10:50:57.167879 loko-cli-0.0.4/loko_cli/examples/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/examples/__init__.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-04-07 10:50:57.171879 loko-cli-0.0.4/loko_cli/model/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/model/__init__.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     5736 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/model/loko.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     1137 2023-01-19 13:08:33.000000 loko-cli-0.0.4/loko_cli/model/microservices.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     2781 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/model/plan.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-04-07 10:50:57.171879 loko-cli-0.0.4/loko_cli/resources/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/resources/__init__.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-04-07 10:50:57.171879 loko-cli-0.0.4/loko_cli/services/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/services/__init__.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/services/services.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-04-07 10:50:57.171879 loko-cli-0.0.4/loko_cli/test/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/test/__init__.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-04-07 10:50:57.171879 loko-cli-0.0.4/loko_cli/utils/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/utils/__init__.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     2011 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/utils/jsonutils.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      586 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/utils/path_utils.py
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     2051 2023-01-18 12:14:39.000000 loko-cli-0.0.4/loko_cli/utils/project_utils.py
-drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-04-07 10:50:57.163879 loko-cli-0.0.4/loko_cli.egg-info/
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      318 2023-04-07 10:50:57.000000 loko-cli-0.0.4/loko_cli.egg-info/PKG-INFO
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     1862 2023-04-07 10:50:57.000000 loko-cli-0.0.4/loko_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        1 2023-04-07 10:50:57.000000 loko-cli-0.0.4/loko_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)       47 2023-04-07 10:50:57.000000 loko-cli-0.0.4/loko_cli.egg-info/entry_points.txt
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)       89 2023-04-07 10:50:57.000000 loko-cli-0.0.4/loko_cli.egg-info/requires.txt
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        9 2023-04-07 10:50:57.000000 loko-cli-0.0.4/loko_cli.egg-info/top_level.txt
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      285 2023-04-06 13:07:08.000000 loko-cli-0.0.4/ppom.json
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)       89 2023-04-04 14:10:53.000000 loko-cli-0.0.4/requirements.txt
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)       38 2023-04-07 10:50:57.171879 loko-cli-0.0.4/setup.cfg
--rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      826 2023-04-04 15:15:00.000000 loko-cli-0.0.4/setup.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-05-19 10:31:48.231505 loko-cli-0.0.5/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)       57 2023-01-18 12:14:39.000000 loko-cli-0.0.5/MANIFEST.in
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      318 2023-05-19 10:31:48.231505 loko-cli-0.0.5/PKG-INFO
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-05-19 10:31:48.227505 loko-cli-0.0.5/loko_cli/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/__init__.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-05-19 10:31:48.227505 loko-cli-0.0.5/loko_cli/apps/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/apps/__init__.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     4103 2023-05-19 10:29:25.000000 loko-cli-0.0.5/loko_cli/apps/cl.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     6005 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/apps/loko_project_deploy.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     3109 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/apps/loko_project_planning.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      124 2023-01-19 16:12:55.000000 loko-cli-0.0.5/loko_cli/apps/modify_a_container.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     5306 2023-05-16 08:41:06.000000 loko-cli-0.0.5/loko_cli/apps/other.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     3082 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/apps/prova_extensions.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      646 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/apps/prova_push.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     2799 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/apps/provaceci.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     2505 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/apps/provakubedepl.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     2358 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/apps/provaorch.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)    18392 2023-05-18 08:53:09.000000 loko-cli-0.0.5/loko_cli/apps/total.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      664 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/apps/volumes.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-05-19 10:31:48.227505 loko-cli-0.0.5/loko_cli/business/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/business/__init__.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-05-19 10:31:48.227505 loko-cli-0.0.5/loko_cli/business/deployment/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/business/deployment/__init__.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-05-19 10:31:48.227505 loko-cli-0.0.5/loko_cli/business/deployment/appliers/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/business/deployment/appliers/__init__.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      178 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/business/deployment/appliers/appliers.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      149 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/business/deployment/appliers/dcapplier2.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     5708 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/business/deployment/appliers/docker_compose_applier.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-05-19 10:31:48.231505 loko-cli-0.0.5/loko_cli/business/deployment/cloud/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/business/deployment/cloud/__init__.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)    11162 2023-05-16 12:36:40.000000 loko-cli-0.0.5/loko_cli/business/deployment/cloud/azure.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     5869 2023-05-12 10:29:19.000000 loko-cli-0.0.5/loko_cli/business/deployment/cloud/ec2.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-05-19 10:31:48.231505 loko-cli-0.0.5/loko_cli/business/deployment/planners/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/business/deployment/planners/__init__.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     4695 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/business/deployment/planners/docker_compose_planner.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      537 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/business/deployment/planners/planners.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      717 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/business/deployment/planners/provagendc.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-05-19 10:31:48.231505 loko-cli-0.0.5/loko_cli/business/docker/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/business/docker/__init__.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)    14375 2023-03-31 07:55:08.000000 loko-cli-0.0.5/loko_cli/business/docker/dockermanager.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     1546 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/business/docker/log_collector.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     1047 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/business/docker/utils.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-05-19 10:31:48.231505 loko-cli-0.0.5/loko_cli/config/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/config/__init__.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/config/app_config.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     2081 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/config/app_init.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-05-19 10:31:48.231505 loko-cli-0.0.5/loko_cli/dao/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/dao/__init__.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      905 2023-01-19 13:08:33.000000 loko-cli-0.0.5/loko_cli/dao/loko.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-05-19 10:31:48.231505 loko-cli-0.0.5/loko_cli/examples/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/examples/__init__.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-05-19 10:31:48.231505 loko-cli-0.0.5/loko_cli/model/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/model/__init__.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     5736 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/model/loko.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     1137 2023-01-19 13:08:33.000000 loko-cli-0.0.5/loko_cli/model/microservices.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     2781 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/model/plan.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-05-19 10:31:48.231505 loko-cli-0.0.5/loko_cli/resources/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/resources/__init__.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-05-19 10:31:48.231505 loko-cli-0.0.5/loko_cli/services/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/services/__init__.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/services/services.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-05-19 10:31:48.231505 loko-cli-0.0.5/loko_cli/test/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/test/__init__.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-05-19 10:31:48.231505 loko-cli-0.0.5/loko_cli/utils/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        0 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/utils/__init__.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     2011 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/utils/jsonutils.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      586 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/utils/path_utils.py
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     2051 2023-01-18 12:14:39.000000 loko-cli-0.0.5/loko_cli/utils/project_utils.py
+drwxrwxr-x   0 cecilia   (1001) cecilia   (1001)        0 2023-05-19 10:31:48.227505 loko-cli-0.0.5/loko_cli.egg-info/
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      318 2023-05-19 10:31:48.000000 loko-cli-0.0.5/loko_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)     1929 2023-05-19 10:31:48.000000 loko-cli-0.0.5/loko_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        1 2023-05-19 10:31:48.000000 loko-cli-0.0.5/loko_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)       47 2023-05-19 10:31:48.000000 loko-cli-0.0.5/loko_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      162 2023-05-19 10:31:48.000000 loko-cli-0.0.5/loko_cli.egg-info/requires.txt
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)        9 2023-05-19 10:31:48.000000 loko-cli-0.0.5/loko_cli.egg-info/top_level.txt
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      285 2023-05-18 08:54:25.000000 loko-cli-0.0.5/ppom.json
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      162 2023-05-16 08:42:22.000000 loko-cli-0.0.5/requirements.txt
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)       38 2023-05-19 10:31:48.231505 loko-cli-0.0.5/setup.cfg
+-rw-rw-r--   0 cecilia   (1001) cecilia   (1001)      826 2023-04-04 15:15:00.000000 loko-cli-0.0.5/setup.py
```

### Comparing `loko-cli-0.0.4/loko_cli/apps/cl.py` & `loko-cli-0.0.5/loko_cli/apps/cl.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import click
 
 import loko_cli.apps.total as tt
 from loguru import logger
 
 
-@click.group(name="loko", help="version 0.0.4")
+@click.group(name="loko", help="version 0.0.5")
 @click.option('--verbose', default=False, show_default=True, help='Verbose output')
 def loko(verbose):
     if not verbose:
         logger.remove()
         logger.add(sys.stderr, level='INFO')
     pass
 
@@ -27,28 +27,50 @@
     """Prepare the plan for the deployment of the Loko project"""
     logger.info("Planning")
     asyncio.run(tt.plan(Path(os.getcwd()), push=push, company=company, gateway_port=gateway_port, https=https))
 
 
 @loko.command()
 @click.option("--name", required=True, type=str, help="the name of the instance")
+@click.option("--region_name", default=None, type=str, help="the region name of the instance")
 @click.option("--security_group", default="default", help="the security group associated to the instance",
               show_default=True, type=str)
 @click.option("--instance_type", default="t2.micro", help="the instance type", show_default=True, type=str)
 @click.option("--ami", default="ami-0a691527202ea8b3d", help="the instance ami", show_default=True, type=str)
-@click.option("--device_volume_size", default=30, help="the instance volume size in GigaBytes", show_default=True, type=int)
-@click.option("--pem", default=Path.home() / "loko.pem", help="the aws key path", show_default=True, type=str)
-def ec2(name, security_group, instance_type, ami, device_volume_size, pem):
+@click.option("--device_volume_size", default=30, help="the instance volume size in GigaBytes", show_default=True,
+              type=int)
+@click.option("--pem", default=Path.home() / "loko.pem", help="the SSH Key path", show_default=True, type=str)
+def ec2(name, region_name, security_group, instance_type, ami, device_volume_size, pem):
     """Manage ec2 instances"""
     p = Path(os.getcwd())
-    asyncio.run(tt.init_ec2(p, name, instance_type, ami, security_group, device_volume_size, pem))
+    asyncio.run(tt.init_ec2(p, name, instance_type, ami, security_group, device_volume_size, pem, region_name))
+
+@loko.command()
+@click.option("--name", required=True, type=str, help="the name of the VM")
+@click.option("--region_name", default='westeurope', type=str, help="the region name of the instance",
+              show_default=True)
+@click.option("--resource_group", default="loko", type=str, help="the name of the resource group", show_default=True)
+@click.option("--security_group", default="loko", help="the security group associated to the instance",
+              show_default=True, type=str)
+@click.option("--virtual_network", default="loko", help="the virtual network associated to the instance",
+              show_default=True, type=str)
+@click.option("--instance_type", default="Standard_B1s", help="the instance type", show_default=True, type=str)
+@click.option("--img", default="loko", help="the vm image", show_default=True, type=str)
+@click.option("--device_volume_size", default=30, help="the instance volume size in GigaBytes", show_default=True,
+              type=int)
+@click.option("--pem", default=Path.home() / "loko_azure.pem", help="the SSH Key path", show_default=True, type=str)
+def azure(name, region_name, resource_group, security_group, virtual_network, instance_type, img, device_volume_size, pem):
+    """Manage Azure VMs"""
+    p = Path(os.getcwd())
+    asyncio.run(tt.init_azure(p, name, instance_type, img, resource_group, security_group, virtual_network,
+                              device_volume_size, pem, region_name))
 
 
 @loko.command()
-@click.option("--pem", default=Path.home() / "loko.pem", help="the aws key path", show_default=True, type=str)
+@click.option("--pem", default=Path.home() / "loko.pem", help="the SSH Key path", show_default=True, type=str)
 def deploy(pem):
     """Deploy the project"""
     p = Path(os.getcwd())
     asyncio.run(tt.deploy(p, pem))
 
 
 @loko.command()
@@ -64,9 +86,9 @@
 
 
 if __name__ == '__main__':
 
     try:
         loko()
     except Exception as inst:
-        logger.exception(inst)
+        logger.error(inst)
         sys.exit(1)
```

### Comparing `loko-cli-0.0.4/loko_cli/apps/loko_project_deploy.py` & `loko-cli-0.0.5/loko_cli/apps/loko_project_deploy.py`

 * *Files identical despite different names*

### Comparing `loko-cli-0.0.4/loko_cli/apps/loko_project_planning.py` & `loko-cli-0.0.5/loko_cli/apps/loko_project_planning.py`

 * *Files identical despite different names*

### Comparing `loko-cli-0.0.4/loko_cli/apps/prova_extensions.py` & `loko-cli-0.0.5/loko_cli/apps/prova_extensions.py`

 * *Files identical despite different names*

### Comparing `loko-cli-0.0.4/loko_cli/apps/prova_push.py` & `loko-cli-0.0.5/loko_cli/apps/prova_push.py`

 * *Files identical despite different names*

### Comparing `loko-cli-0.0.4/loko_cli/apps/provaceci.py` & `loko-cli-0.0.5/loko_cli/apps/provaceci.py`

 * *Files identical despite different names*

### Comparing `loko-cli-0.0.4/loko_cli/apps/provakubedepl.py` & `loko-cli-0.0.5/loko_cli/apps/provakubedepl.py`

 * *Files identical despite different names*

### Comparing `loko-cli-0.0.4/loko_cli/apps/provaorch.py` & `loko-cli-0.0.5/loko_cli/apps/provaorch.py`

 * *Files identical despite different names*

### Comparing `loko-cli-0.0.4/loko_cli/apps/volumes.py` & `loko-cli-0.0.5/loko_cli/apps/volumes.py`

 * *Files identical despite different names*

### Comparing `loko-cli-0.0.4/loko_cli/business/deployment/appliers/docker_compose_applier.py` & `loko-cli-0.0.5/loko_cli/business/deployment/appliers/docker_compose_applier.py`

 * *Files identical despite different names*

### Comparing `loko-cli-0.0.4/loko_cli/business/deployment/cloud/ec2.py` & `loko-cli-0.0.5/loko_cli/business/deployment/cloud/ec2.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,18 @@
                 'VolumeType': 'gp2'
             }
         },
     ]
 
 
 class EC2Manager:
-    def __init__(self, region_name='eu-central-1', pem=None):
-        self.ec2 = boto3.resource('ec2', region_name=region_name)
+    def __init__(self, region_name=None, pem=Path.home() / "loko.pem"):
+        my_session = boto3.session.Session()
+        my_region = my_session.region_name
+        self.ec2 = boto3.resource('ec2', region_name=region_name or my_region)
         if isinstance(pem, str):
             pem = Path(pem)
         self.pem = pem
 
     def get(self, id):
         for inst in self.all():
             if inst.id == id:
```

### Comparing `loko-cli-0.0.4/loko_cli/business/deployment/planners/docker_compose_planner.py` & `loko-cli-0.0.5/loko_cli/business/deployment/planners/docker_compose_planner.py`

 * *Files identical despite different names*

### Comparing `loko-cli-0.0.4/loko_cli/business/deployment/planners/planners.py` & `loko-cli-0.0.5/loko_cli/business/deployment/planners/planners.py`

 * *Files identical despite different names*

### Comparing `loko-cli-0.0.4/loko_cli/business/deployment/planners/provagendc.py` & `loko-cli-0.0.5/loko_cli/business/deployment/planners/provagendc.py`

 * *Files identical despite different names*

### Comparing `loko-cli-0.0.4/loko_cli/business/docker/dockermanager.py` & `loko-cli-0.0.5/loko_cli/business/docker/dockermanager.py`

 * *Files identical despite different names*

### Comparing `loko-cli-0.0.4/loko_cli/business/docker/log_collector.py` & `loko-cli-0.0.5/loko_cli/business/docker/log_collector.py`

 * *Files identical despite different names*

### Comparing `loko-cli-0.0.4/loko_cli/business/docker/utils.py` & `loko-cli-0.0.5/loko_cli/business/docker/utils.py`

 * *Files identical despite different names*

### Comparing `loko-cli-0.0.4/loko_cli/config/app_init.py` & `loko-cli-0.0.5/loko_cli/config/app_init.py`

 * *Files identical despite different names*

### Comparing `loko-cli-0.0.4/loko_cli/dao/loko.py` & `loko-cli-0.0.5/loko_cli/dao/loko.py`

 * *Files identical despite different names*

### Comparing `loko-cli-0.0.4/loko_cli/model/loko.py` & `loko-cli-0.0.5/loko_cli/model/loko.py`

 * *Files identical despite different names*

### Comparing `loko-cli-0.0.4/loko_cli/model/microservices.py` & `loko-cli-0.0.5/loko_cli/model/microservices.py`

 * *Files identical despite different names*

### Comparing `loko-cli-0.0.4/loko_cli/model/plan.py` & `loko-cli-0.0.5/loko_cli/model/plan.py`

 * *Files identical despite different names*

### Comparing `loko-cli-0.0.4/loko_cli/utils/jsonutils.py` & `loko-cli-0.0.5/loko_cli/utils/jsonutils.py`

 * *Files identical despite different names*

### Comparing `loko-cli-0.0.4/loko_cli/utils/path_utils.py` & `loko-cli-0.0.5/loko_cli/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `loko-cli-0.0.4/loko_cli/utils/project_utils.py` & `loko-cli-0.0.5/loko_cli/utils/project_utils.py`

 * *Files identical despite different names*

### Comparing `loko-cli-0.0.4/loko_cli.egg-info/SOURCES.txt` & `loko-cli-0.0.5/loko_cli.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,28 +10,30 @@
 loko_cli.egg-info/requires.txt
 loko_cli.egg-info/top_level.txt
 loko_cli/apps/__init__.py
 loko_cli/apps/cl.py
 loko_cli/apps/loko_project_deploy.py
 loko_cli/apps/loko_project_planning.py
 loko_cli/apps/modify_a_container.py
+loko_cli/apps/other.py
 loko_cli/apps/prova_extensions.py
 loko_cli/apps/prova_push.py
 loko_cli/apps/provaceci.py
 loko_cli/apps/provakubedepl.py
 loko_cli/apps/provaorch.py
 loko_cli/apps/total.py
 loko_cli/apps/volumes.py
 loko_cli/business/__init__.py
 loko_cli/business/deployment/__init__.py
 loko_cli/business/deployment/appliers/__init__.py
 loko_cli/business/deployment/appliers/appliers.py
 loko_cli/business/deployment/appliers/dcapplier2.py
 loko_cli/business/deployment/appliers/docker_compose_applier.py
 loko_cli/business/deployment/cloud/__init__.py
+loko_cli/business/deployment/cloud/azure.py
 loko_cli/business/deployment/cloud/ec2.py
 loko_cli/business/deployment/planners/__init__.py
 loko_cli/business/deployment/planners/docker_compose_planner.py
 loko_cli/business/deployment/planners/planners.py
 loko_cli/business/deployment/planners/provagendc.py
 loko_cli/business/docker/__init__.py
 loko_cli/business/docker/dockermanager.py
```

### Comparing `loko-cli-0.0.4/setup.py` & `loko-cli-0.0.5/setup.py`

 * *Files identical despite different names*

