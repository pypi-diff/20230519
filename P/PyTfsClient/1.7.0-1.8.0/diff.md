# Comparing `tmp/PyTfsClient-1.7.0.tar.gz` & `tmp/PyTfsClient-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyTfsClient-1.7.0.tar", last modified: Mon May 15 17:40:53 2023, max compression
+gzip compressed data, was "dist\PyTfsClient-1.8.0.tar", last modified: Fri May 19 19:56:44 2023, max compression
```

## Comparing `PyTfsClient-1.7.0.tar` & `PyTfsClient-1.8.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 17:40:53.743333 PyTfsClient-1.7.0/
--rw-rw-rw-   0        0        0      642 2023-05-15 17:40:53.730588 PyTfsClient-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     1859 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-15 17:40:53.751376 PyTfsClient-1.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1437 2023-05-15 17:40:37.000000 PyTfsClient-1.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 17:40:52.924842 PyTfsClient-1.7.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-15 17:40:53.189548 PyTfsClient-1.7.0/src/PyTfsClient.egg-info/
--rw-rw-rw-   0        0        0      642 2023-05-15 17:40:51.000000 PyTfsClient-1.7.0/src/PyTfsClient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2049 2023-05-15 17:40:51.000000 PyTfsClient-1.7.0/src/PyTfsClient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 17:40:51.000000 PyTfsClient-1.7.0/src/PyTfsClient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-02 15:09:42.000000 PyTfsClient-1.7.0/src/PyTfsClient.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       31 2023-05-15 17:40:51.000000 PyTfsClient-1.7.0/src/PyTfsClient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-15 17:40:51.000000 PyTfsClient-1.7.0/src/PyTfsClient.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-15 17:40:53.306710 PyTfsClient-1.7.0/src/pytfsclient/
--rw-rw-rw-   0        0        0        0 2022-03-04 20:05:30.000000 PyTfsClient-1.7.0/src/pytfsclient/__init__.py
--rw-rw-rw-   0        0        0     3536 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/client_connection.py
--rw-rw-rw-   0        0        0     6046 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/client_factory.py
-drwxrwxrwx   0        0        0        0 2023-05-15 17:40:53.338696 PyTfsClient-1.7.0/src/pytfsclient/models/
--rw-rw-rw-   0        0        0        0 2023-03-22 16:13:58.000000 PyTfsClient-1.7.0/src/pytfsclient/models/__init__.py
--rw-rw-rw-   0        0        0      118 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/models/client_error.py
--rw-rw-rw-   0        0        0      720 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/models/deprecated.py
--rw-rw-rw-   0        0        0      700 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/models/obsolete.py
-drwxrwxrwx   0        0        0        0 2023-05-15 17:40:53.384072 PyTfsClient-1.7.0/src/pytfsclient/models/project/
--rw-rw-rw-   0        0        0        0 2023-03-22 16:43:11.000000 PyTfsClient-1.7.0/src/pytfsclient/models/project/__init__.py
--rw-rw-rw-   0        0        0     2628 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/models/project/tfs_project.py
--rw-rw-rw-   0        0        0     1925 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/models/project/tfs_team.py
--rw-rw-rw-   0        0        0     3251 2023-05-15 17:25:05.000000 PyTfsClient-1.7.0/src/pytfsclient/models/project/tfs_team_member.py
-drwxrwxrwx   0        0        0        0 2023-05-15 17:40:53.465938 PyTfsClient-1.7.0/src/pytfsclient/models/workitems/
--rw-rw-rw-   0        0        0        0 2023-03-22 19:36:56.000000 PyTfsClient-1.7.0/src/pytfsclient/models/workitems/__init__.py
--rw-rw-rw-   0        0        0      364 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/models/workitems/tfs_update_relations_result.py
--rw-rw-rw-   0        0        0     1816 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/models/workitems/tfs_wiql_result.py
--rw-rw-rw-   0        0        0     8989 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/models/workitems/tfs_workitem.py
--rw-rw-rw-   0        0        0     6850 2023-04-15 15:18:40.000000 PyTfsClient-1.7.0/src/pytfsclient/models/workitems/tfs_workitem_changes.py
--rw-rw-rw-   0        0        0     3829 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/models/workitems/tfs_workitem_relation.py
-drwxrwxrwx   0        0        0        0 2023-05-15 17:40:53.498924 PyTfsClient-1.7.0/src/pytfsclient/services/
--rw-rw-rw-   0        0        0        0 2023-03-21 17:34:23.000000 PyTfsClient-1.7.0/src/pytfsclient/services/__init__.py
--rw-rw-rw-   0        0        0     1100 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/services/base_client.py
-drwxrwxrwx   0        0        0        0 2023-05-15 17:40:53.526602 PyTfsClient-1.7.0/src/pytfsclient/services/helpers/
--rw-rw-rw-   0        0        0        0 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/services/helpers/__init__.py
--rw-rw-rw-   0        0        0      303 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/services/helpers/batch_iterable.py
-drwxrwxrwx   0        0        0        0 2023-05-15 17:40:53.556578 PyTfsClient-1.7.0/src/pytfsclient/services/http/
--rw-rw-rw-   0        0        0        0 2023-03-21 17:05:15.000000 PyTfsClient-1.7.0/src/pytfsclient/services/http/__init__.py
--rw-rw-rw-   0        0        0     5035 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/services/http/http_client.py
-drwxrwxrwx   0        0        0        0 2023-05-15 17:40:53.590067 PyTfsClient-1.7.0/src/pytfsclient/services/mention_client/
--rw-rw-rw-   0        0        0        0 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/services/mention_client/__init__.py
--rw-rw-rw-   0        0        0     2305 2023-04-21 18:14:10.000000 PyTfsClient-1.7.0/src/pytfsclient/services/mention_client/mention_client.py
-drwxrwxrwx   0        0        0        0 2023-05-15 17:40:53.623621 PyTfsClient-1.7.0/src/pytfsclient/services/project_client/
--rw-rw-rw-   0        0        0        0 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/services/project_client/__init__.py
--rw-rw-rw-   0        0        0     8846 2023-04-14 17:19:50.000000 PyTfsClient-1.7.0/src/pytfsclient/services/project_client/project_client.py
-drwxrwxrwx   0        0        0        0 2023-05-15 17:40:53.653354 PyTfsClient-1.7.0/src/pytfsclient/services/workitem_client/
--rw-rw-rw-   0        0        0        0 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/services/workitem_client/__init__.py
--rw-rw-rw-   0        0        0    26102 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/services/workitem_client/workitem_client.py
--rw-rw-rw-   0        0        0     2674 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/tfs_client.py
--rw-rw-rw-   0        0        0     2904 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/tfs_client_factory.py
--rw-rw-rw-   0        0        0     4181 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/tfs_project_client.py
--rw-rw-rw-   0        0        0     4527 2023-04-01 16:47:59.000000 PyTfsClient-1.7.0/src/pytfsclient/tfs_project_model.py
--rw-rw-rw-   0        0        0     1042 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/tfs_wiql_model.py
--rw-rw-rw-   0        0        0    13483 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/tfs_workitem_client.py
--rw-rw-rw-   0        0        0     6809 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/tfs_workitem_model.py
--rw-rw-rw-   0        0        0     3074 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/src/pytfsclient/tfs_workitem_relation_model.py
-drwxrwxrwx   0        0        0        0 2023-05-15 17:40:53.721467 PyTfsClient-1.7.0/test/
--rw-rw-rw-   0        0        0     5924 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/test/test_backward_compatibility.py
--rw-rw-rw-   0        0        0     1052 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/test/test_client_connection.py
--rw-rw-rw-   0        0        0     1361 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/test/test_http_client_auth.py
--rw-rw-rw-   0        0        0     4568 2023-04-13 20:16:25.000000 PyTfsClient-1.7.0/test/test_http_client_basic.py
--rw-rw-rw-   0        0        0     9903 2023-04-14 18:48:58.000000 PyTfsClient-1.7.0/test/test_integration.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:56:44.723309 PyTfsClient-1.8.0/
+-rw-rw-rw-   0        0        0      642 2023-05-19 19:56:44.719403 PyTfsClient-1.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1859 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-19 19:56:44.727063 PyTfsClient-1.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1437 2023-05-19 19:56:11.000000 PyTfsClient-1.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:56:44.463745 PyTfsClient-1.8.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-19 19:56:44.561619 PyTfsClient-1.8.0/src/PyTfsClient.egg-info/
+-rw-rw-rw-   0        0        0      642 2023-05-19 19:56:44.000000 PyTfsClient-1.8.0/src/PyTfsClient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2049 2023-05-19 19:56:44.000000 PyTfsClient-1.8.0/src/PyTfsClient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 19:56:44.000000 PyTfsClient-1.8.0/src/PyTfsClient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-02 15:09:42.000000 PyTfsClient-1.8.0/src/PyTfsClient.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       31 2023-05-19 19:56:44.000000 PyTfsClient-1.8.0/src/PyTfsClient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-19 19:56:44.000000 PyTfsClient-1.8.0/src/PyTfsClient.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 19:56:44.598972 PyTfsClient-1.8.0/src/pytfsclient/
+-rw-rw-rw-   0        0        0        0 2022-03-04 20:05:30.000000 PyTfsClient-1.8.0/src/pytfsclient/__init__.py
+-rw-rw-rw-   0        0        0     3536 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/src/pytfsclient/client_connection.py
+-rw-rw-rw-   0        0        0     6046 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/src/pytfsclient/client_factory.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:56:44.610875 PyTfsClient-1.8.0/src/pytfsclient/models/
+-rw-rw-rw-   0        0        0        0 2023-03-22 16:13:58.000000 PyTfsClient-1.8.0/src/pytfsclient/models/__init__.py
+-rw-rw-rw-   0        0        0      118 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/src/pytfsclient/models/client_error.py
+-rw-rw-rw-   0        0        0      720 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/src/pytfsclient/models/deprecated.py
+-rw-rw-rw-   0        0        0      700 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/src/pytfsclient/models/obsolete.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:56:44.624232 PyTfsClient-1.8.0/src/pytfsclient/models/project/
+-rw-rw-rw-   0        0        0        0 2023-03-22 16:43:11.000000 PyTfsClient-1.8.0/src/pytfsclient/models/project/__init__.py
+-rw-rw-rw-   0        0        0     2628 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/src/pytfsclient/models/project/tfs_project.py
+-rw-rw-rw-   0        0        0     1925 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/src/pytfsclient/models/project/tfs_team.py
+-rw-rw-rw-   0        0        0     3251 2023-05-15 17:25:05.000000 PyTfsClient-1.8.0/src/pytfsclient/models/project/tfs_team_member.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:56:44.641270 PyTfsClient-1.8.0/src/pytfsclient/models/workitems/
+-rw-rw-rw-   0        0        0        0 2023-03-22 19:36:56.000000 PyTfsClient-1.8.0/src/pytfsclient/models/workitems/__init__.py
+-rw-rw-rw-   0        0        0      364 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/src/pytfsclient/models/workitems/tfs_update_relations_result.py
+-rw-rw-rw-   0        0        0     1845 2023-05-19 19:45:37.000000 PyTfsClient-1.8.0/src/pytfsclient/models/workitems/tfs_wiql_result.py
+-rw-rw-rw-   0        0        0     8989 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/src/pytfsclient/models/workitems/tfs_workitem.py
+-rw-rw-rw-   0        0        0     6850 2023-04-15 15:18:40.000000 PyTfsClient-1.8.0/src/pytfsclient/models/workitems/tfs_workitem_changes.py
+-rw-rw-rw-   0        0        0     3829 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/src/pytfsclient/models/workitems/tfs_workitem_relation.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:56:44.649770 PyTfsClient-1.8.0/src/pytfsclient/services/
+-rw-rw-rw-   0        0        0        0 2023-03-21 17:34:23.000000 PyTfsClient-1.8.0/src/pytfsclient/services/__init__.py
+-rw-rw-rw-   0        0        0     1100 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/src/pytfsclient/services/base_client.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:56:44.657789 PyTfsClient-1.8.0/src/pytfsclient/services/helpers/
+-rw-rw-rw-   0        0        0        0 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/src/pytfsclient/services/helpers/__init__.py
+-rw-rw-rw-   0        0        0      303 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/src/pytfsclient/services/helpers/batch_iterable.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:56:44.667006 PyTfsClient-1.8.0/src/pytfsclient/services/http/
+-rw-rw-rw-   0        0        0        0 2023-03-21 17:05:15.000000 PyTfsClient-1.8.0/src/pytfsclient/services/http/__init__.py
+-rw-rw-rw-   0        0        0     5035 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/src/pytfsclient/services/http/http_client.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:56:44.673151 PyTfsClient-1.8.0/src/pytfsclient/services/mention_client/
+-rw-rw-rw-   0        0        0        0 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/src/pytfsclient/services/mention_client/__init__.py
+-rw-rw-rw-   0        0        0     2305 2023-04-21 18:14:10.000000 PyTfsClient-1.8.0/src/pytfsclient/services/mention_client/mention_client.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:56:44.680827 PyTfsClient-1.8.0/src/pytfsclient/services/project_client/
+-rw-rw-rw-   0        0        0        0 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/src/pytfsclient/services/project_client/__init__.py
+-rw-rw-rw-   0        0        0     8846 2023-04-14 17:19:50.000000 PyTfsClient-1.8.0/src/pytfsclient/services/project_client/project_client.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:56:44.693915 PyTfsClient-1.8.0/src/pytfsclient/services/workitem_client/
+-rw-rw-rw-   0        0        0        0 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/src/pytfsclient/services/workitem_client/__init__.py
+-rw-rw-rw-   0        0        0    26102 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/src/pytfsclient/services/workitem_client/workitem_client.py
+-rw-rw-rw-   0        0        0     2674 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/src/pytfsclient/tfs_client.py
+-rw-rw-rw-   0        0        0     2904 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/src/pytfsclient/tfs_client_factory.py
+-rw-rw-rw-   0        0        0     4181 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/src/pytfsclient/tfs_project_client.py
+-rw-rw-rw-   0        0        0     4527 2023-04-01 16:47:59.000000 PyTfsClient-1.8.0/src/pytfsclient/tfs_project_model.py
+-rw-rw-rw-   0        0        0     1042 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/src/pytfsclient/tfs_wiql_model.py
+-rw-rw-rw-   0        0        0    13483 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/src/pytfsclient/tfs_workitem_client.py
+-rw-rw-rw-   0        0        0     6809 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/src/pytfsclient/tfs_workitem_model.py
+-rw-rw-rw-   0        0        0     3074 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/src/pytfsclient/tfs_workitem_relation_model.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:56:44.714764 PyTfsClient-1.8.0/test/
+-rw-rw-rw-   0        0        0     5924 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/test/test_backward_compatibility.py
+-rw-rw-rw-   0        0        0     1052 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/test/test_client_connection.py
+-rw-rw-rw-   0        0        0     1361 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/test/test_http_client_auth.py
+-rw-rw-rw-   0        0        0     4568 2023-04-13 20:16:25.000000 PyTfsClient-1.8.0/test/test_http_client_basic.py
+-rw-rw-rw-   0        0        0     9903 2023-04-14 18:48:58.000000 PyTfsClient-1.8.0/test/test_integration.py
```

### Comparing `PyTfsClient-1.7.0/PKG-INFO` & `PyTfsClient-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: PyTfsClient
-Version: 1.7.0
+Version: 1.8.0
 Summary: Python Microsoft Team Foundation Server Library is a  client that can work with Microsoft TFS workitems
 Home-page: https://github.com/TopTuK/PyTfsClient
 Author: TopTuK
 Author-email: cydoor88@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: TFS,AZURE,TFS API,Team Foundation Server
```

### Comparing `PyTfsClient-1.7.0/README.md` & `PyTfsClient-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/setup.py` & `PyTfsClient-1.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ### Execute
 # python setup.py sdist
 # twine upload dist/*
 
 # https://docs.python.org/3/distutils/setupscript.html
 setup(
     name='PyTfsClient',
-    version='1.7.0',
+    version='1.8.0',
     license='MIT',
     description='Python Microsoft Team Foundation Server Library is a  client that can work with Microsoft TFS workitems',
     url='https://github.com/TopTuK/PyTfsClient',
     author='TopTuK',
     author_email='cydoor88@gmail.com',
     package_dir={'': 'src'},
     packages=find_packages(where='src', include=['pytfsclient*'], exclude=['.test', '*.test', 'test', 'test*', 'test.*']),
```

### Comparing `PyTfsClient-1.7.0/src/PyTfsClient.egg-info/PKG-INFO` & `PyTfsClient-1.8.0/src/PyTfsClient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: PyTfsClient
-Version: 1.7.0
+Version: 1.8.0
 Summary: Python Microsoft Team Foundation Server Library is a  client that can work with Microsoft TFS workitems
 Home-page: https://github.com/TopTuK/PyTfsClient
 Author: TopTuK
 Author-email: cydoor88@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: TFS,AZURE,TFS API,Team Foundation Server
```

### Comparing `PyTfsClient-1.7.0/src/PyTfsClient.egg-info/SOURCES.txt` & `PyTfsClient-1.8.0/src/PyTfsClient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/src/pytfsclient/client_connection.py` & `PyTfsClient-1.8.0/src/pytfsclient/client_connection.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/src/pytfsclient/client_factory.py` & `PyTfsClient-1.8.0/src/pytfsclient/client_factory.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/src/pytfsclient/models/deprecated.py` & `PyTfsClient-1.8.0/src/pytfsclient/models/deprecated.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/src/pytfsclient/models/obsolete.py` & `PyTfsClient-1.8.0/src/pytfsclient/models/obsolete.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/src/pytfsclient/models/project/tfs_project.py` & `PyTfsClient-1.8.0/src/pytfsclient/models/project/tfs_project.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/src/pytfsclient/models/project/tfs_team.py` & `PyTfsClient-1.8.0/src/pytfsclient/models/project/tfs_team.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/src/pytfsclient/models/project/tfs_team_member.py` & `PyTfsClient-1.8.0/src/pytfsclient/models/project/tfs_team_member.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/src/pytfsclient/models/workitems/tfs_wiql_result.py` & `PyTfsClient-1.8.0/src/pytfsclient/models/workitems/tfs_wiql_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     @property
     def workitems(self) -> List[Workitem]:
         '''
         Returns:
             List of workitems.
         '''
 
-        return self.__client.get_workitems(self.item_ids)
+        return self.__client.get_workitems(self.item_ids) if not self.is_empty else []
     
     @classmethod
     def from_json(cls, tfs_client, json_response):
         '''
         Classmethod creates WiqlResult class instance from given json object.
 
         Args:
```

### Comparing `PyTfsClient-1.7.0/src/pytfsclient/models/workitems/tfs_workitem.py` & `PyTfsClient-1.8.0/src/pytfsclient/models/workitems/tfs_workitem.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/src/pytfsclient/models/workitems/tfs_workitem_changes.py` & `PyTfsClient-1.8.0/src/pytfsclient/models/workitems/tfs_workitem_changes.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/src/pytfsclient/models/workitems/tfs_workitem_relation.py` & `PyTfsClient-1.8.0/src/pytfsclient/models/workitems/tfs_workitem_relation.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/src/pytfsclient/services/base_client.py` & `PyTfsClient-1.8.0/src/pytfsclient/services/base_client.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/src/pytfsclient/services/http/http_client.py` & `PyTfsClient-1.8.0/src/pytfsclient/services/http/http_client.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/src/pytfsclient/services/mention_client/mention_client.py` & `PyTfsClient-1.8.0/src/pytfsclient/services/mention_client/mention_client.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/src/pytfsclient/services/project_client/project_client.py` & `PyTfsClient-1.8.0/src/pytfsclient/services/project_client/project_client.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/src/pytfsclient/services/workitem_client/workitem_client.py` & `PyTfsClient-1.8.0/src/pytfsclient/services/workitem_client/workitem_client.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/src/pytfsclient/tfs_client.py` & `PyTfsClient-1.8.0/src/pytfsclient/tfs_client.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/src/pytfsclient/tfs_client_factory.py` & `PyTfsClient-1.8.0/src/pytfsclient/tfs_client_factory.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/src/pytfsclient/tfs_project_client.py` & `PyTfsClient-1.8.0/src/pytfsclient/tfs_project_client.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/src/pytfsclient/tfs_project_model.py` & `PyTfsClient-1.8.0/src/pytfsclient/tfs_project_model.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/src/pytfsclient/tfs_wiql_model.py` & `PyTfsClient-1.8.0/src/pytfsclient/tfs_wiql_model.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/src/pytfsclient/tfs_workitem_client.py` & `PyTfsClient-1.8.0/src/pytfsclient/tfs_workitem_client.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/src/pytfsclient/tfs_workitem_model.py` & `PyTfsClient-1.8.0/src/pytfsclient/tfs_workitem_model.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/src/pytfsclient/tfs_workitem_relation_model.py` & `PyTfsClient-1.8.0/src/pytfsclient/tfs_workitem_relation_model.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/test/test_backward_compatibility.py` & `PyTfsClient-1.8.0/test/test_backward_compatibility.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/test/test_client_connection.py` & `PyTfsClient-1.8.0/test/test_client_connection.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/test/test_http_client_auth.py` & `PyTfsClient-1.8.0/test/test_http_client_auth.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/test/test_http_client_basic.py` & `PyTfsClient-1.8.0/test/test_http_client_basic.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.7.0/test/test_integration.py` & `PyTfsClient-1.8.0/test/test_integration.py`

 * *Files identical despite different names*

