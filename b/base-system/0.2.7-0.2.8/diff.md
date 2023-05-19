# Comparing `tmp/base_system-0.2.7.tar.gz` & `tmp/base_system-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "base_system-0.2.7.tar", last modified: Fri May 12 09:44:02 2023, max compression
+gzip compressed data, was "base_system-0.2.8.tar", last modified: Fri May 19 03:10:51 2023, max compression
```

## Comparing `base_system-0.2.7.tar` & `base_system-0.2.8.tar`

### file list

```diff
@@ -1,68 +1,70 @@
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 09:44:02.699733 base_system-0.2.7/
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)     1562 2023-01-04 07:42:57.000000 base_system-0.2.7/.gitignore
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      113 2023-02-07 05:55:05.000000 base_system-0.2.7/.pypirc
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 09:44:02.687724 base_system-0.2.7/BaseFunctionModule/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 05:21:26.000000 base_system-0.2.7/BaseFunctionModule/__init__.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.7/BaseFunctionModule/asgi.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    11801 2023-05-06 02:43:22.000000 base_system-0.2.7/BaseFunctionModule/settings.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      917 2023-04-17 08:52:27.000000 base_system-0.2.7/BaseFunctionModule/urls.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.7/BaseFunctionModule/wsgi.py
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      280 2023-01-04 05:21:25.000000 base_system-0.2.7/Dockerfile
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1554 2023-01-04 05:21:26.000000 base_system-0.2.7/LICENCE
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      106 2023-01-04 05:21:25.000000 base_system-0.2.7/MANIFEST.in
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-12 09:44:02.695730 base_system-0.2.7/PKG-INFO
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      756 2023-04-25 05:48:42.000000 base_system-0.2.7/README.rst
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 09:44:02.691727 base_system-0.2.7/base_system/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 03:02:16.000000 base_system-0.2.7/base_system/__init__.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 09:44:02.695730 base_system-0.2.7/base_system/__pycache__/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      148 2023-04-17 09:28:42.000000 base_system-0.2.7/base_system/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-17 09:28:43.000000 base_system-0.2.7/base_system/__pycache__/admin.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      434 2023-04-17 09:28:42.000000 base_system-0.2.7/base_system/__pycache__/apps.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    10658 2023-05-06 02:06:31.000000 base_system-0.2.7/base_system/__pycache__/export_viewset.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    19926 2023-05-12 09:42:05.000000 base_system-0.2.7/base_system/__pycache__/models.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    27610 2023-05-06 02:44:00.000000 base_system-0.2.7/base_system/__pycache__/serializers.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-18 01:10:23.000000 base_system-0.2.7/base_system/__pycache__/tests.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3179 2023-05-06 02:06:30.000000 base_system-0.2.7/base_system/__pycache__/urls.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    23682 2023-05-09 03:12:52.000000 base_system-0.2.7/base_system/__pycache__/views.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    11929 2023-05-12 09:42:07.000000 base_system-0.2.7/base_system/__pycache__/viewsets.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       63 2022-09-27 03:45:06.000000 base_system-0.2.7/base_system/admin.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      153 2022-09-27 03:45:06.000000 base_system-0.2.7/base_system/apps.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3320 2022-09-27 03:45:06.000000 base_system-0.2.7/base_system/auth.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    15572 2023-04-26 08:23:42.000000 base_system-0.2.7/base_system/export_viewset.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 09:44:02.695730 base_system-0.2.7/base_system/migrations/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    39429 2023-04-27 08:58:52.000000 base_system-0.2.7/base_system/migrations/0001_initial.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      441 2023-05-04 02:32:29.000000 base_system-0.2.7/base_system/migrations/0002_drugdirectory_code_medu_cur.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      557 2023-05-04 07:38:30.000000 base_system-0.2.7/base_system/migrations/0003_alter_extragroup_hospital.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      443 2023-05-04 08:07:17.000000 base_system-0.2.7/base_system/migrations/0004_alter_extragroup_role_name.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1144 2023-05-09 03:12:53.000000 base_system-0.2.7/base_system/migrations/0005_expensetype.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      433 2023-05-09 07:38:03.000000 base_system-0.2.7/base_system/migrations/0006_alter_doctor_photo.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      563 2023-05-12 09:42:07.000000 base_system-0.2.7/base_system/migrations/0007_auto_20230512_1742.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2022-09-27 03:45:06.000000 base_system-0.2.7/base_system/migrations/__init__.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 09:44:02.695730 base_system-0.2.7/base_system/migrations/__pycache__/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    15056 2023-05-04 02:32:29.000000 base_system-0.2.7/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      666 2023-05-04 07:38:30.000000 base_system-0.2.7/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      794 2023-05-04 07:38:38.000000 base_system-0.2.7/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      667 2023-05-06 01:27:34.000000 base_system-0.2.7/base_system/migrations/__pycache__/0004_alter_extragroup_role_name.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1093 2023-05-09 07:38:03.000000 base_system-0.2.7/base_system/migrations/__pycache__/0005_expensetype.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      652 2023-05-12 09:42:07.000000 base_system-0.2.7/base_system/migrations/__pycache__/0006_alter_doctor_photo.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      726 2023-05-12 09:42:23.000000 base_system-0.2.7/base_system/migrations/__pycache__/0007_auto_20230512_1742.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      159 2023-04-17 09:28:44.000000 base_system-0.2.7/base_system/migrations/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    25981 2023-05-12 09:41:48.000000 base_system-0.2.7/base_system/models.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    23752 2023-05-06 02:43:58.000000 base_system-0.2.7/base_system/serializers.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       60 2023-02-13 08:28:28.000000 base_system-0.2.7/base_system/tests.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     4071 2023-05-06 02:06:28.000000 base_system-0.2.7/base_system/urls.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    58056 2023-05-09 03:12:22.000000 base_system-0.2.7/base_system/views.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    15097 2023-05-12 09:18:57.000000 base_system-0.2.7/base_system/viewsets.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 09:44:02.691727 base_system-0.2.7/base_system.egg-info/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-12 09:44:02.000000 base_system-0.2.7/base_system.egg-info/PKG-INFO
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     2168 2023-05-12 09:44:02.000000 base_system-0.2.7/base_system.egg-info/SOURCES.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-12 09:44:02.000000 base_system-0.2.7/base_system.egg-info/dependency_links.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-04 03:18:55.000000 base_system-0.2.7/base_system.egg-info/not-zip-safe
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      108 2023-05-12 09:44:02.000000 base_system-0.2.7/base_system.egg-info/requires.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       12 2023-05-12 09:44:02.000000 base_system-0.2.7/base_system.egg-info/top_level.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)   262434 2023-01-04 05:21:26.000000 base_system-0.2.7/init_data.json
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      674 2023-04-17 08:52:27.000000 base_system-0.2.7/manage.py
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      888 2023-01-04 05:21:25.000000 base_system-0.2.7/requirements.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      574 2023-04-17 08:52:27.000000 base_system-0.2.7/runtests.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       38 2023-05-12 09:44:02.699733 base_system-0.2.7/setup.cfg
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     2650 2023-05-12 09:43:42.000000 base_system-0.2.7/setup.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-19 03:10:51.502165 base_system-0.2.8/
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)     1562 2023-01-04 07:42:57.000000 base_system-0.2.8/.gitignore
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      113 2023-02-07 05:55:05.000000 base_system-0.2.8/.pypirc
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-19 03:10:51.434126 base_system-0.2.8/BaseFunctionModule/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 05:21:26.000000 base_system-0.2.8/BaseFunctionModule/__init__.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.8/BaseFunctionModule/asgi.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    11801 2023-05-18 07:09:09.000000 base_system-0.2.8/BaseFunctionModule/settings.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      917 2023-04-17 08:52:27.000000 base_system-0.2.8/BaseFunctionModule/urls.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.8/BaseFunctionModule/wsgi.py
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      280 2023-01-04 05:21:25.000000 base_system-0.2.8/Dockerfile
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1554 2023-01-04 05:21:26.000000 base_system-0.2.8/LICENCE
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      106 2023-01-04 05:21:25.000000 base_system-0.2.8/MANIFEST.in
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-19 03:10:51.502165 base_system-0.2.8/PKG-INFO
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      756 2023-04-25 05:48:42.000000 base_system-0.2.8/README.rst
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-19 03:10:51.462142 base_system-0.2.8/base_system/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 03:02:16.000000 base_system-0.2.8/base_system/__init__.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-19 03:10:51.482154 base_system-0.2.8/base_system/__pycache__/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      148 2023-04-17 09:28:42.000000 base_system-0.2.8/base_system/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-17 09:28:43.000000 base_system-0.2.8/base_system/__pycache__/admin.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      434 2023-04-17 09:28:42.000000 base_system-0.2.8/base_system/__pycache__/apps.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    10658 2023-05-06 02:06:31.000000 base_system-0.2.8/base_system/__pycache__/export_viewset.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    21108 2023-05-18 07:23:45.000000 base_system-0.2.8/base_system/__pycache__/models.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    27610 2023-05-06 02:44:00.000000 base_system-0.2.8/base_system/__pycache__/serializers.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-18 01:10:23.000000 base_system-0.2.8/base_system/__pycache__/tests.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     3283 2023-05-18 07:17:34.000000 base_system-0.2.8/base_system/__pycache__/urls.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    24024 2023-05-18 07:17:35.000000 base_system-0.2.8/base_system/__pycache__/views.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    11929 2023-05-12 09:42:07.000000 base_system-0.2.8/base_system/__pycache__/viewsets.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       63 2022-09-27 03:45:06.000000 base_system-0.2.8/base_system/admin.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      153 2022-09-27 03:45:06.000000 base_system-0.2.8/base_system/apps.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     3320 2022-09-27 03:45:06.000000 base_system-0.2.8/base_system/auth.py
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)   154032 2023-02-13 10:31:46.000000 base_system-0.2.8/base_system/examination_dic.json
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    15572 2023-04-26 08:23:42.000000 base_system-0.2.8/base_system/export_viewset.py
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)   428136 2023-02-13 10:31:46.000000 base_system-0.2.8/base_system/inspdic.json
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-19 03:10:51.490158 base_system-0.2.8/base_system/migrations/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    39429 2023-04-27 08:58:52.000000 base_system-0.2.8/base_system/migrations/0001_initial.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      441 2023-05-04 02:32:29.000000 base_system-0.2.8/base_system/migrations/0002_drugdirectory_code_medu_cur.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      557 2023-05-04 07:38:30.000000 base_system-0.2.8/base_system/migrations/0003_alter_extragroup_hospital.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      443 2023-05-04 08:07:17.000000 base_system-0.2.8/base_system/migrations/0004_alter_extragroup_role_name.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1144 2023-05-09 03:12:53.000000 base_system-0.2.8/base_system/migrations/0005_expensetype.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      433 2023-05-09 07:38:03.000000 base_system-0.2.8/base_system/migrations/0006_alter_doctor_photo.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      563 2023-05-12 09:42:07.000000 base_system-0.2.8/base_system/migrations/0007_auto_20230512_1742.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2022-09-27 03:45:06.000000 base_system-0.2.8/base_system/migrations/__init__.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-19 03:10:51.498163 base_system-0.2.8/base_system/migrations/__pycache__/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    15056 2023-05-04 02:32:29.000000 base_system-0.2.8/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      666 2023-05-04 07:38:30.000000 base_system-0.2.8/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      794 2023-05-04 07:38:38.000000 base_system-0.2.8/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      667 2023-05-06 01:27:34.000000 base_system-0.2.8/base_system/migrations/__pycache__/0004_alter_extragroup_role_name.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1093 2023-05-09 07:38:03.000000 base_system-0.2.8/base_system/migrations/__pycache__/0005_expensetype.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      652 2023-05-12 09:42:07.000000 base_system-0.2.8/base_system/migrations/__pycache__/0006_alter_doctor_photo.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      726 2023-05-12 09:42:23.000000 base_system-0.2.8/base_system/migrations/__pycache__/0007_auto_20230512_1742.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      159 2023-04-17 09:28:44.000000 base_system-0.2.8/base_system/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    27939 2023-05-18 07:23:43.000000 base_system-0.2.8/base_system/models.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    23752 2023-05-06 02:43:58.000000 base_system-0.2.8/base_system/serializers.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       60 2023-02-13 08:28:28.000000 base_system-0.2.8/base_system/tests.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     4244 2023-05-19 03:09:13.000000 base_system-0.2.8/base_system/urls.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    56505 2023-05-19 03:06:33.000000 base_system-0.2.8/base_system/views.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    15097 2023-05-12 09:18:57.000000 base_system-0.2.8/base_system/viewsets.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-19 03:10:51.466144 base_system-0.2.8/base_system.egg-info/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-19 03:10:51.000000 base_system-0.2.8/base_system.egg-info/PKG-INFO
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     2226 2023-05-19 03:10:51.000000 base_system-0.2.8/base_system.egg-info/SOURCES.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-19 03:10:51.000000 base_system-0.2.8/base_system.egg-info/dependency_links.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-04 03:18:55.000000 base_system-0.2.8/base_system.egg-info/not-zip-safe
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      108 2023-05-19 03:10:51.000000 base_system-0.2.8/base_system.egg-info/requires.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       12 2023-05-19 03:10:51.000000 base_system-0.2.8/base_system.egg-info/top_level.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)   262434 2023-01-04 05:21:26.000000 base_system-0.2.8/init_data.json
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      674 2023-04-17 08:52:27.000000 base_system-0.2.8/manage.py
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      888 2023-01-04 05:21:25.000000 base_system-0.2.8/requirements.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      574 2023-04-17 08:52:27.000000 base_system-0.2.8/runtests.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       38 2023-05-19 03:10:51.502165 base_system-0.2.8/setup.cfg
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     2650 2023-05-19 03:10:33.000000 base_system-0.2.8/setup.py
```

### Comparing `base_system-0.2.7/.gitignore` & `base_system-0.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/BaseFunctionModule/settings.py` & `base_system-0.2.8/BaseFunctionModule/settings.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/BaseFunctionModule/urls.py` & `base_system-0.2.8/BaseFunctionModule/urls.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/LICENCE` & `base_system-0.2.8/LICENCE`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/PKG-INFO` & `base_system-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: base_system
-Version: 0.2.7
+Version: 0.2.8
 Summary: Basic feature component
 Home-page: https://github.com/zcjwin
 Author: zcjwin
 Author-email: win_zcj@163.com
 License: UNKNOWN
 Keywords: base_system
 Platform: UNKNOWN
```

### Comparing `base_system-0.2.7/README.rst` & `base_system-0.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/base_system/__pycache__/export_viewset.cpython-39.pyc` & `base_system-0.2.8/base_system/__pycache__/export_viewset.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/base_system/__pycache__/models.cpython-39.pyc` & `base_system-0.2.8/base_system/__pycache__/models.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May 12 09:41:48 2023 UTC, .py size: 25981 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,1246 +1,1320 @@
-00000000: 610d 0d0a 0000 0000 dc09 5e64 7d65 0000  a.........^d}e..
+00000000: 610d 0d0a 0000 0000 7fd2 6564 236d 0000  a.........ed#m..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 de01 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 ea01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
-00000050: 6d05 5a05 0100 6400 6403 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
+00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
+00000050: 5a04 6400 6403 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6404 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
-00000070: 6405 6c0a 6d0b 5a0b 0100 6406 5a0c 4700  d.l.m.Z...d.Z.G.
-00000080: 6407 6408 8400 6408 6509 6a0d 8303 5a0e  d.d...d.e.j...Z.
-00000090: 4700 6409 640a 8400 640a 650e 8303 5a0f  G.d.d...d.e...Z.
-000000a0: 4700 640b 640c 8400 640c 650e 8303 5a10  G.d.d...d.e...Z.
-000000b0: 4700 640d 640e 8400 640e 650e 8303 5a11  G.d.d...d.e...Z.
-000000c0: 4700 640f 6410 8400 6410 650e 8303 5a12  G.d.d...d.e...Z.
-000000d0: 4700 6411 6412 8400 6412 6504 8303 5a13  G.d.d...d.e...Z.
-000000e0: 4700 6413 6414 8400 6414 6509 6a0d 8303  G.d.d...d.e.j...
-000000f0: 5a14 4700 6415 6416 8400 6416 6509 6a0d  Z.G.d.d...d.e.j.
-00000100: 8303 5a15 4700 6417 6418 8400 6418 6509  ..Z.G.d.d...d.e.
-00000110: 6a0d 8303 5a16 4700 6419 641a 8400 641a  j...Z.G.d.d...d.
-00000120: 650e 8303 5a17 4700 641b 641c 8400 641c  e...Z.G.d.d...d.
-00000130: 650e 8303 5a18 4700 641d 641e 8400 641e  e...Z.G.d.d...d.
-00000140: 650e 8303 5a19 4700 641f 6420 8400 6420  e...Z.G.d.d ..d 
-00000150: 650e 8303 5a1a 4700 6421 6422 8400 6422  e...Z.G.d!d"..d"
-00000160: 650e 8303 5a1b 4700 6423 6424 8400 6424  e...Z.G.d#d$..d$
-00000170: 650e 8303 5a1c 4700 6425 6426 8400 6426  e...Z.G.d%d&..d&
-00000180: 650e 8303 5a1d 4700 6427 6428 8400 6428  e...Z.G.d'd(..d(
-00000190: 650e 8303 5a1e 4700 6429 642a 8400 642a  e...Z.G.d)d*..d*
-000001a0: 650e 8303 5a1f 4700 642b 642c 8400 642c  e...Z.G.d+d,..d,
-000001b0: 650e 8303 5a20 4700 642d 642e 8400 642e  e...Z G.d-d...d.
-000001c0: 650e 8303 5a21 4700 642f 6430 8400 6430  e...Z!G.d/d0..d0
-000001d0: 650e 8303 5a22 4700 6431 6432 8400 6432  e...Z"G.d1d2..d2
-000001e0: 650e 8303 5a23 4700 6433 6434 8400 6434  e...Z#G.d3d4..d4
-000001f0: 650e 8303 5a24 4700 6435 6436 8400 6436  e...Z$G.d5d6..d6
-00000200: 6509 6a0d 8303 5a25 6401 5300 2937 e900  e.j...Z%d.S.)7..
-00000210: 0000 004e 2902 da0c 4162 7374 7261 6374  ...N)...Abstract
-00000220: 5573 6572 da05 4772 6f75 7029 01da 0b43  User..Group)...C
-00000230: 6f6e 7465 6e74 5479 7065 2901 da06 6d6f  ontentType)...mo
-00000240: 6465 6c73 2901 da08 7365 7474 696e 6773  dels)...settings
-00000250: 2902 2902 da01 3175 0300 0000 e794 b729  ).)...1u.......)
-00000260: 02da 0130 7503 0000 00e5 a5b3 6300 0000  ...0u.......c...
-00000270: 0000 0000 0000 0000 0000 0000 0005 0000  ................
-00000280: 0040 0000 0073 4800 0000 6500 5a01 6400  .@...sH...e.Z.d.
-00000290: 5a02 6503 6a04 6401 6402 6402 6403 8d03  Z.e.j.d.d.d.d...
-000002a0: 5a05 6503 6a04 6404 6402 6402 6405 8d03  Z.e.j.d.d.d.d...
-000002b0: 5a06 6503 6a07 6406 6402 6407 8d02 5a08  Z.e.j.d.d.d...Z.
-000002c0: 4700 6408 6409 8400 6409 8302 5a09 640a  G.d.d...d...Z.d.
-000002d0: 5300 290b da10 4d65 6469 6361 6c42 6173  S.)...MedicalBas
-000002e0: 654d 6f64 656c f50c 0000 00e5 889b e5bb  eModel..........
-000002f0: bae6 97b6 e997 b454 a903 da0c 7665 7262  .......T....verb
-00000300: 6f73 655f 6e61 6d65 da0c 6175 746f 5f6e  ose_name..auto_n
-00000310: 6f77 5f61 6464 da04 6e75 6c6c f50c 0000  ow_add..null....
-00000320: 00e6 9bb4 e696 b0e6 97b6 e997 b4a9 0372  ...............r
-00000330: 0c00 0000 da08 6175 746f 5f6e 6f77 720e  ......auto_nowr.
-00000340: 0000 00f5 0c00 0000 e698 afe5 90a6 e590  ................
-00000350: afe7 94a8 a902 720c 0000 00da 0764 6566  ......r......def
-00000360: 6175 6c74 6300 0000 0000 0000 0000 0000  aultc...........
-00000370: 0000 0000 0001 0000 0040 0000 0073 1000  .........@...s..
-00000380: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-00000390: 5300 2903 7a15 4d65 6469 6361 6c42 6173  S.).z.MedicalBas
-000003a0: 654d 6f64 656c 2e4d 6574 6154 4e29 04da  eModel.MetaTN)..
-000003b0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-000003c0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-000003d0: 655f 5fda 0861 6273 7472 6163 74a9 0072  e__..abstract..r
-000003e0: 1900 0000 7219 0000 00fa 372f 686f 6d65  ....r.....7/home
-000003f0: 2f6c 7968 2f77 6f72 6b2f 4261 7365 4675  /lyh/work/BaseFu
-00000400: 6e63 7469 6f6e 4d6f 6475 6c65 2f62 6173  nctionModule/bas
-00000410: 655f 7379 7374 656d 2f6d 6f64 656c 732e  e_system/models.
-00000420: 7079 da04 4d65 7461 1500 0000 7302 0000  py..Meta....s...
-00000430: 0008 0172 1b00 0000 4e29 0a72 1500 0000  ...r....N).r....
-00000440: 7216 0000 0072 1700 0000 7205 0000 00da  r....r....r.....
-00000450: 0d44 6174 6554 696d 6546 6965 6c64 da0c  .DateTimeField..
-00000460: 6372 6561 7465 645f 7469 6d65 da0c 7570  created_time..up
-00000470: 6461 7465 645f 7469 6d65 da0c 426f 6f6c  dated_time..Bool
-00000480: 6561 6e46 6965 6c64 da09 6973 5f61 6374  eanField..is_act
-00000490: 6976 6572 1b00 0000 7219 0000 0072 1900  iver....r....r..
-000004a0: 0000 7219 0000 0072 1a00 0000 7209 0000  ..r....r....r...
-000004b0: 0010 0000 0073 0800 0000 0801 1001 1001  .....s..........
-000004c0: 0e02 7209 0000 0063 0000 0000 0000 0000  ..r....c........
-000004d0: 0000 0000 0000 0000 0600 0000 4000 0000  ............@...
-000004e0: 73d8 0000 0065 005a 0164 005a 0265 036a  s....e.Z.d.Z.e.j
-000004f0: 0464 0164 0264 038d 025a 0565 036a 0464  .d.d.d...Z.e.j.d
-00000500: 0464 0564 0664 0664 078d 045a 0665 036a  .d.d.d.d...Z.e.j
-00000510: 0764 0864 0664 0664 098d 035a 0865 036a  .d.d.d.d...Z.e.j
-00000520: 0464 0264 0a64 0664 0b8d 035a 0965 036a  .d.d.d.d...Z.e.j
-00000530: 0764 0c64 0d8d 015a 0a65 036a 0b64 0e64  .d.d...Z.e.j.d.d
-00000540: 0d8d 015a 0c65 036a 0b64 0f64 0d8d 015a  ...Z.e.j.d.d...Z
-00000550: 0d65 036a 0e64 1064 1165 036a 0f64 0664  .e.j.d.d.e.j.d.d
-00000560: 128d 045a 1065 036a 0464 1364 0564 1464  ...Z.e.j.d.d.d.d
-00000570: 0664 158d 045a 1165 036a 0464 1664 0564  .d...Z.e.j.d.d.d
-00000580: 1764 188d 035a 1265 036a 0464 1964 0564  .d...Z.e.j.d.d.d
-00000590: 0664 0664 078d 045a 1365 036a 0464 1a64  .d.d...Z.e.j.d.d
-000005a0: 0564 0664 0664 078d 045a 1447 0064 1b64  .d.d.d...Z.G.d.d
-000005b0: 1c84 0064 1c83 025a 1564 1d53 0029 1eda  ...d...Z.d.S.)..
-000005c0: 0848 6f73 7069 7461 6cf5 0600 0000 e590  .Hospital.......
-000005d0: 8de7 a7b0 e9ff 0000 00a9 0272 0c00 0000  ...........r....
-000005e0: da0a 6d61 785f 6c65 6e67 7468 f50c 0000  ..max_length....
-000005f0: 00e8 8194 e7b3 bbe6 96b9 e5bc 8fe9 6400  ..............d.
-00000600: 0000 54a9 0472 0c00 0000 7225 0000 0072  ..T..r....r%...r
-00000610: 0e00 0000 da05 626c 616e 6b75 0c00 0000  ......blanku....
-00000620: e58c bbe9 99a2 e7ae 80e4 bb8b a903 720c  ..............r.
-00000630: 0000 0072 0e00 0000 7229 0000 00f5 0600  ...r....r)......
-00000640: 0000 e7bc 96e7 a081 a903 7225 0000 0072  ..........r%...r
-00000650: 0c00 0000 da06 756e 6971 7565 750c 0000  ......uniqueu...
-00000660: 00e5 8cbb e999 a2e5 9cb0 e59d 8029 0172  .............).r
-00000670: 0c00 0000 7506 0000 00e7 bb8f e5ba a675  ....u..........u
-00000680: 0600 0000 e7bb b4e5 baa6 da04 7365 6c66  ............self
-00000690: f50c 0000 00e6 8980 e5b1 9ee5 8cbb e999  ................
-000006a0: a2a9 0372 0c00 0000 da09 6f6e 5f64 656c  ...r......on_del
-000006b0: 6574 6572 0e00 0000 750c 0000 00e5 8cbb  eter....u.......
-000006c0: e999 a2e5 9bbe e789 875a 0f68 6f73 7069  .........Z.hospi
-000006d0: 7461 6c5f 696d 6167 6573 2904 720c 0000  tal_images).r...
-000006e0: 0072 2500 0000 7214 0000 0072 2900 0000  .r%...r....r)...
-000006f0: da04 6c6f 676f 5a0d 686f 7370 6974 616c  ..logoZ.hospital
-00000700: 5f6c 6f67 6fa9 0372 0c00 0000 7225 0000  _logo..r....r%..
-00000710: 0072 1400 0000 f509 0000 00e5 889b e5bb  .r..............
-00000720: bae4 baba f509 0000 00e6 9bb4 e696 b0e4  ................
-00000730: baba 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000740: 0000 0001 0000 0040 0000 0073 1800 0000  .......@...s....
-00000750: 6500 5a01 6400 5a02 6401 5a03 6402 5a04  e.Z.d.Z.d.Z.d.Z.
-00000760: 6504 5a05 6403 5300 2904 7a0d 486f 7370  e.Z.d.S.).z.Hosp
-00000770: 6974 616c 2e4d 6574 615a 0b62 735f 686f  ital.MetaZ.bs_ho
-00000780: 7370 6974 616c 7506 0000 00e5 8cbb e999  spitalu.........
-00000790: a24e a906 7215 0000 0072 1600 0000 7217  .N..r....r....r.
-000007a0: 0000 00da 0864 625f 7461 626c 6572 0c00  .....db_tabler..
-000007b0: 0000 da13 7665 7262 6f73 655f 6e61 6d65  ....verbose_name
-000007c0: 5f70 6c75 7261 6c72 1900 0000 7219 0000  _pluralr....r...
-000007d0: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
-000007e0: 2e00 0000 7306 0000 0008 0104 0104 0172  ....s..........r
-000007f0: 1b00 0000 4e29 1672 1500 0000 7216 0000  ....N).r....r...
-00000800: 0072 1700 0000 7205 0000 00da 0943 6861  .r....r......Cha
-00000810: 7246 6965 6c64 da04 6e61 6d65 da05 7068  rField..name..ph
-00000820: 6f6e 65da 0954 6578 7446 6965 6c64 da09  one..TextField..
-00000830: 696e 7472 6f64 7563 65da 0763 6f64 656e  introduce..coden
-00000840: 756d da07 6164 6472 6573 73da 0a46 6c6f  um..address..Flo
-00000850: 6174 4669 656c 645a 096c 6f6e 6769 7475  atFieldZ.longitu
-00000860: 6465 5a08 6c61 7469 7475 6465 da0a 466f  deZ.latitude..Fo
-00000870: 7265 6967 6e4b 6579 da07 4341 5343 4144  reignKey..CASCAD
-00000880: 45da 0670 6172 656e 745a 0a68 6f73 5f69  E..parentZ.hos_i
-00000890: 6d61 6765 7372 3200 0000 da0a 6372 6561  magesr2.....crea
-000008a0: 7465 645f 6279 da0a 7570 6461 7465 645f  ted_by..updated_
-000008b0: 6279 721b 0000 0072 1900 0000 7219 0000  byr....r....r...
-000008c0: 0072 1900 0000 721a 0000 0072 2100 0000  .r....r....r!...
-000008d0: 1900 0000 7324 0000 0008 010e 0112 0110  ....s$..........
-000008e0: 0110 010c 010c 010c 0104 0102 0102 0104  ................
-000008f0: 0102 fc06 0712 0210 0112 0112 0272 2100  .............r!.
-00000900: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000910: 0000 0006 0000 0040 0000 0073 a200 0000  .......@...s....
-00000920: 6500 5a01 6400 5a02 6503 6a04 6401 6402  e.Z.d.Z.e.j.d.d.
-00000930: 6403 8d02 5a05 6503 6a04 6404 6402 6405  d...Z.e.j.d.d.d.
-00000940: 6405 6406 8d04 5a06 6503 6a04 6407 6402  d.d...Z.e.j.d.d.
-00000950: 6405 6405 6406 8d04 5a07 6503 6a04 6408  d.d.d...Z.e.j.d.
-00000960: 6402 6403 8d02 5a08 6503 6a04 6409 640a  d.d...Z.e.j.d.d.
-00000970: 6405 6405 6406 8d04 5a09 6503 6a0a 640b  d.d.d...Z.e.j.d.
-00000980: 6405 6405 640c 8d03 5a0b 6503 6a0c 650d  d.d.d...Z.e.j.e.
-00000990: 640d 6503 6a0e 640e 8d03 5a0f 6503 6a0c  d.e.j.d...Z.e.j.
-000009a0: 640f 6410 6503 6a0e 6405 6411 8d04 5a10  d.d.e.j.d.d...Z.
-000009b0: 4700 6412 6413 8400 6413 8302 5a11 6414  G.d.d...d...Z.d.
-000009c0: 5300 2915 da06 4f66 6669 6365 7222 0000  S.)...Officer"..
-000009d0: 0072 2300 0000 7224 0000 0075 0c00 0000  .r#...r$...u....
-000009e0: e7a7 91e5 aea4 e4bd 8de7 bdae 5472 2800  ............Tr(.
-000009f0: 0000 7226 0000 00f5 0c00 0000 e7a7 91e5  ..r&............
-00000a00: aea4 e7bc 96e7 a081 7506 0000 00e7 b1bb  ........u.......
-00000a10: e59e 8b72 2700 0000 750c 0000 00e7 a791  ...r'...u.......
-00000a20: e5ae a4e7 ae80 e4bb 8b72 2a00 0000 722f  .........r*...r/
-00000a30: 0000 00a9 0272 0c00 0000 7231 0000 0072  .....r....r1...r
-00000a40: 2e00 0000 750c 0000 00e4 b88a e7ba a7e7  ....u...........
-00000a50: a791 e5ae a472 3000 0000 6300 0000 0000  .....r0...c.....
-00000a60: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
-00000a70: 0000 0073 1c00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00000a80: 6401 5a03 6402 5a04 6504 5a05 6403 5a06  d.Z.d.Z.e.Z.d.Z.
-00000a90: 6404 5300 2905 7a0b 4f66 6669 6365 2e4d  d.S.).z.Office.M
-00000aa0: 6574 615a 0962 735f 6f66 6669 6365 7506  etaZ.bs_officeu.
-00000ab0: 0000 00e7 a791 e5ae a4a9 0129 0272 3e00  ...........).r>.
-00000ac0: 0000 da08 686f 7370 6974 616c 4ea9 0772  ....hospitalN..r
-00000ad0: 1500 0000 7216 0000 0072 1700 0000 7237  ....r....r....r7
-00000ae0: 0000 0072 0c00 0000 7238 0000 00da 0f75  ...r....r8.....u
-00000af0: 6e69 7175 655f 746f 6765 7468 6572 7219  nique_togetherr.
-00000b00: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-00000b10: 0000 721b 0000 004a 0000 0073 0800 0000  ..r....J...s....
-00000b20: 0801 0401 0401 0401 721b 0000 004e 2912  ........r....N).
-00000b30: 7215 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-00000b40: 0500 0000 7239 0000 0072 3a00 0000 723f  ....r9...r:...r?
-00000b50: 0000 0072 3b00 0000 723e 0000 005a 0b6f  ...r;...r>...Z.o
-00000b60: 6666 6963 655f 7479 7065 723c 0000 0072  ffice_typer<...r
-00000b70: 3d00 0000 7241 0000 0072 2100 0000 7242  =...rA...r!...rB
-00000b80: 0000 0072 4a00 0000 7243 0000 0072 1b00  ...rJ...rC...r..
-00000b90: 0000 7219 0000 0072 1900 0000 7219 0000  ..r....r....r...
-00000ba0: 0072 1a00 0000 7246 0000 0037 0000 0073  .r....rF...7...s
-00000bb0: 2400 0000 0801 0e01 1201 1201 0e01 1201  $...............
-00000bc0: 1001 0401 0201 0201 04fd 0605 0401 0201  ................
-00000bd0: 0201 0401 02fc 0607 7246 0000 0063 0000  ........rF...c..
-00000be0: 0000 0000 0000 0000 0000 0000 0000 0600  ................
-00000bf0: 0000 4000 0000 736c 0000 0065 005a 0164  ..@...sl...e.Z.d
-00000c00: 005a 0265 036a 0464 0164 0264 038d 025a  .Z.e.j.d.d.d...Z
-00000c10: 0565 036a 0464 0464 0264 038d 025a 0665  .e.j.d.d.d...Z.e
-00000c20: 036a 0765 0864 0565 036a 0964 068d 035a  .j.e.d.e.j.d...Z
-00000c30: 0a65 036a 0464 0764 0864 0964 0964 0a8d  .e.j.d.d.d.d.d..
-00000c40: 045a 0b65 036a 0464 0b64 0864 0964 0964  .Z.e.j.d.d.d.d.d
-00000c50: 0a8d 045a 0c47 0064 0c64 0d84 0064 0d83  ...Z.G.d.d...d..
-00000c60: 025a 0d64 0e53 0029 0fda 0d50 6f73 6974  .Z.d.S.)...Posit
-00000c70: 696f 6e54 6974 6c65 7222 0000 0072 2300  ionTitler"...r#.
-00000c80: 0000 7224 0000 0075 0c00 0000 e881 8ce7  ..r$...u........
-00000c90: a7b0 e7bc 96e7 a081 722f 0000 0072 4800  ........r/...rH.
-00000ca0: 0000 7234 0000 0072 2700 0000 5472 2800  ..r4...r'...Tr(.
-00000cb0: 0000 7235 0000 0063 0000 0000 0000 0000  ..r5...c........
-00000cc0: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
-00000cd0: 731c 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
-00000ce0: 0364 025a 0465 045a 0564 035a 0664 0453  .d.Z.e.Z.d.Z.d.S
-00000cf0: 0029 057a 1250 6f73 6974 696f 6e54 6974  .).z.PositionTit
-00000d00: 6c65 2e4d 6574 615a 1162 735f 706f 7369  le.MetaZ.bs_posi
-00000d10: 7469 6f6e 5f74 6974 6c65 f506 0000 00e8  tion_title......
-00000d20: 818c e7a7 b072 4900 0000 4e72 4b00 0000  .....rI...NrK...
-00000d30: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-00000d40: 1a00 0000 721b 0000 005e 0000 0073 0800  ....r....^...s..
-00000d50: 0000 0801 0401 0401 0401 721b 0000 004e  ..........r....N
-00000d60: 290e 7215 0000 0072 1600 0000 7217 0000  ).r....r....r...
-00000d70: 0072 0500 0000 7239 0000 0072 3a00 0000  .r....r9...r:...
-00000d80: 723e 0000 0072 4100 0000 7221 0000 0072  r>...rA...r!...r
-00000d90: 4200 0000 724a 0000 0072 4400 0000 7245  B...rJ...rD...rE
-00000da0: 0000 0072 1b00 0000 7219 0000 0072 1900  ...r....r....r..
-00000db0: 0000 7219 0000 0072 1a00 0000 724d 0000  ..r....r....rM..
-00000dc0: 0053 0000 0073 1400 0000 0801 0e01 0e01  .S...s..........
-00000dd0: 0401 0201 0201 04fd 0605 1201 1202 724d  ..............rM
-00000de0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000df0: 0000 0000 0700 0000 4000 0000 734e 0100  ........@...sN..
-00000e00: 0065 005a 0164 005a 0265 036a 0464 0164  .e.Z.d.Z.e.j.d.d
-00000e10: 0264 038d 025a 0565 036a 0464 0464 0264  .d...Z.e.j.d.d.d
-00000e20: 0564 0564 068d 045a 0665 036a 0464 0764  .d.d...Z.e.j.d.d
-00000e30: 0864 0564 0564 068d 045a 0765 036a 0464  .d.d.d...Z.e.j.d
-00000e40: 0964 0a64 0564 0564 068d 045a 0865 036a  .d.d.d.d...Z.e.j
-00000e50: 0464 0b64 0c64 038d 025a 0965 036a 0464  .d.d.d...Z.e.j.d
-00000e60: 0d64 0264 0564 0564 068d 045a 0a65 036a  .d.d.d.d...Z.e.j
-00000e70: 0b65 0c64 0e65 036a 0d64 0f8d 035a 0e65  .e.d.e.j.d...Z.e
-00000e80: 036a 0464 1064 1165 0f64 0564 0564 128d  .j.d.d.e.d.d.d..
-00000e90: 055a 1065 036a 0464 1364 1464 0564 0564  .Z.e.j.d.d.d.d.d
-00000ea0: 068d 045a 1165 036a 0464 1564 0864 0564  ...Z.e.j.d.d.d.d
-00000eb0: 0564 068d 045a 1265 036a 0b65 1364 1665  .d...Z.e.j.e.d.e
-00000ec0: 036a 0d64 0f8d 035a 1465 036a 0b65 1564  .j.d...Z.e.j.e.d
-00000ed0: 1765 036a 0d64 0f8d 035a 1665 036a 1764  .e.j.d...Z.e.j.d
-00000ee0: 1864 0564 0564 198d 035a 1865 036a 0464  .d.d.d...Z.e.j.d
-00000ef0: 1a64 1b64 1c64 1d8d 035a 1965 036a 1a64  .d.d.d...Z.e.j.d
-00000f00: 1e64 0564 0564 198d 035a 1b65 036a 0464  .d.d.d...Z.e.j.d
-00000f10: 1f64 0264 0564 0564 068d 045a 1c65 036a  .d.d.d.d...Z.e.j
-00000f20: 0464 2064 0264 0564 0564 068d 045a 1d65  .d d.d.d.d...Z.e
-00000f30: 036a 1e64 2164 0564 228d 025a 1f47 0064  .j.d!d.d"..Z.G.d
-00000f40: 2364 2484 0064 2483 025a 2064 2553 0029  #d$..d$..Z d%S.)
-00000f50: 26da 0644 6f63 746f 7272 2200 0000 e914  &..Doctorr".....
-00000f60: 0000 0072 2400 0000 7226 0000 0054 7228  ...r$...r&...Tr(
-00000f70: 0000 0075 0600 0000 e982 aee7 aeb1 7227  ...u..........r'
-00000f80: 0000 0075 0600 0000 e59c b0e5 9d80 7223  ...u..........r#
-00000f90: 0000 0075 0600 0000 e5b7 a5e5 8fb7 e940  ...u...........@
-00000fa0: 0000 0075 0600 0000 e881 8ce4 bd8d 724e  ...u..........rN
-00000fb0: 0000 0072 4800 0000 f506 0000 00e6 80a7  ...rH...........
-00000fc0: e588 abe9 0200 0000 a905 720c 0000 0072  ..........r....r
-00000fd0: 2500 0000 da07 6368 6f69 6365 7372 0e00  %.....choicesr..
-00000fe0: 0000 7229 0000 0075 0600 0000 e6b0 91e6  ..r)...u........
-00000ff0: 978f e90a 0000 00f5 0c00 0000 e8ba abe4  ................
-00001000: bbbd e8af 81e5 8fb7 f50c 0000 00e6 8980  ................
-00001010: e5b1 9ee7 a791 e5ae a472 2f00 0000 f50c  .........r/.....
-00001020: 0000 00e5 87ba e794 9fe6 97a5 e69c 9f72  ...............r
-00001030: 2a00 0000 750c 0000 00e5 8cbb e794 9fe7  *...u...........
-00001040: 85a7 e789 87e9 3200 0000 5a0c 646f 6374  ......2...Z.doct
-00001050: 6f72 5f70 686f 746f 7233 0000 0075 0c00  or_photor3...u..
-00001060: 0000 e58c bbe7 949f e68f 8fe8 bfb0 7234  ..............r4
-00001070: 0000 0072 3500 0000 7515 0000 00e6 98af  ...r5...u.......
-00001080: e590 a6e4 ba92 e881 94e7 bd91 e68e a5e8  ................
-00001090: af8a 7213 0000 0063 0000 0000 0000 0000  ..r....c........
-000010a0: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
-000010b0: 7318 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
-000010c0: 0364 025a 0465 045a 0564 0353 0029 047a  .d.Z.e.Z.d.S.).z
-000010d0: 0b44 6f63 746f 722e 4d65 7461 5a09 6273  .Doctor.MetaZ.bs
-000010e0: 5f64 6f63 746f 7275 0900 0000 e58c bbe7  _doctoru........
-000010f0: 949f e8a1 a84e 7236 0000 0072 1900 0000  .....Nr6...r....
-00001100: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
-00001110: 1b00 0000 8900 0000 7306 0000 0008 0104  ........s.......
-00001120: 0104 0172 1b00 0000 4e29 2172 1500 0000  ...r....N)!r....
-00001130: 7216 0000 0072 1700 0000 7205 0000 0072  r....r....r....r
-00001140: 3900 0000 723a 0000 0072 3b00 0000 da05  9...r:...r;.....
-00001150: 656d 6169 6c72 3f00 0000 723e 0000 00da  emailr?...r>....
-00001160: 0870 6f73 6974 696f 6e72 4100 0000 724d  .positionrA...rM
-00001170: 0000 0072 4200 0000 5a0e 706f 7369 7469  ...rB...Z.positi
-00001180: 6f6e 5f74 6974 6c65 da0d 4745 4e44 4552  on_title..GENDER
-00001190: 5f43 484f 4943 45da 0667 656e 6465 725a  _CHOICE..genderZ
-000011a0: 066e 6174 696f 6e5a 0569 646e 756d 7246  .nationZ.idnumrF
-000011b0: 0000 00da 066f 6666 6963 6572 2100 0000  .....officer!...
-000011c0: 724a 0000 00da 0944 6174 6546 6965 6c64  rJ.....DateField
-000011d0: da08 6269 7274 6864 6179 5a05 7068 6f74  ..birthdayZ.phot
-000011e0: 6f72 3c00 0000 da08 6465 7363 7269 6265  or<.....describe
-000011f0: 7244 0000 0072 4500 0000 721f 0000 005a  rD...rE...r....Z
-00001200: 1169 735f 6f6e 6c69 6e65 5f63 6f6e 7375  .is_online_consu
-00001210: 6c74 721b 0000 0072 1900 0000 7219 0000  ltr....r....r...
-00001220: 0072 1900 0000 721a 0000 0072 4f00 0000  .r....r....rO...
-00001230: 6700 0000 733e 0000 0008 010e 0112 0112  g...s>..........
-00001240: 0112 010e 0112 0104 0102 0102 0104 fd06  ................
-00001250: 0514 0112 0112 0104 0102 0102 0104 fd06  ................
-00001260: 0504 0102 0102 0104 fd06 0510 0210 0110  ................
-00001270: 0112 0112 020e 0272 4f00 0000 6300 0000  .......rO...c...
-00001280: 0000 0000 0000 0000 0000 0000 0007 0000  ................
-00001290: 0040 0000 0073 6e01 0000 6500 5a01 6400  .@...sn...e.Z.d.
-000012a0: 5a02 6503 6a04 6401 6402 6403 6403 6404  Z.e.j.d.d.d.d.d.
-000012b0: 8d04 5a05 6503 6a04 6405 6406 6403 6403  ..Z.e.j.d.d.d.d.
-000012c0: 6404 8d04 5a06 6503 6a07 6407 6403 6403  d...Z.e.j.d.d.d.
-000012d0: 6408 8d03 5a08 6503 6a04 6409 640a 6509  d...Z.e.j.d.d.e.
-000012e0: 6403 6403 640b 8d05 5a0a 6503 6a04 640c  d.d.d...Z.e.j.d.
-000012f0: 6406 6403 6403 6404 8d04 5a0b 6503 6a0c  d.d.d.d...Z.e.j.
-00001300: 640d 640e 6403 6403 640f 8d04 5a0d 6503  d.d.d.d.d...Z.e.
-00001310: 6a0e 650f 6410 6503 6a10 6403 6411 8d04  j.e.d.e.j.d.d...
-00001320: 5a11 6503 6a0e 6512 6412 6503 6a10 6403  Z.e.j.e.d.e.j.d.
-00001330: 6411 8d04 5a13 6503 6a0e 6514 6413 6503  d...Z.e.j.e.d.e.
-00001340: 6a10 6403 6411 8d04 5a15 6503 6a04 6414  j.d.d...Z.e.j.d.
-00001350: 6406 6415 6416 8d03 5a16 6503 6a04 6417  d.d.d...Z.e.j.d.
-00001360: 6402 6403 6403 6404 8d04 5a17 6503 6a04  d.d.d.d...Z.e.j.
-00001370: 6418 6402 6403 6403 6404 8d04 5a18 6503  d.d.d.d.d...Z.e.
-00001380: 6a19 6419 6403 6403 6408 8d03 5a1a 6503  j.d.d.d.d...Z.e.
-00001390: 6a04 641a 6406 6403 6403 6404 8d04 5a1b  j.d.d.d.d.d...Z.
-000013a0: 6503 6a04 641b 6406 6403 6403 6404 8d04  e.j.d.d.d.d.d...
-000013b0: 5a1c 6503 6a1d 641c 6403 6403 641d 8d03  Z.e.j.d.d.d.d...
-000013c0: 5a1e 6503 6a1d 641e 6403 6403 641f 8d03  Z.e.j.d.d.d.d...
-000013d0: 5a1f 4700 6420 6421 8400 6421 8302 5a20  Z.G.d d!..d!..Z 
-000013e0: 6521 6422 6423 8400 8301 5a22 6521 6424  e!d"d#....Z"e!d$
-000013f0: 6425 8400 8301 5a23 6521 6426 6427 8400  d%....Z#e!d&d'..
-00001400: 8301 5a24 6428 5300 2929 da04 5573 6572  ..Z$d(S.))..User
-00001410: 7222 0000 0072 2300 0000 5472 2800 0000  r"...r#...Tr(...
-00001420: 7226 0000 0072 2700 0000 7259 0000 0072  r&...r'...rY...r
-00001430: 2a00 0000 7252 0000 0072 5300 0000 7254  *...rR...rS...rT
-00001440: 0000 0072 5700 0000 f506 0000 00e6 8e92  ...rW...........
-00001450: e5ba 8fe9 0100 0000 a904 720c 0000 0072  ..........r....r
-00001460: 1400 0000 720e 0000 0072 2900 0000 7258  ....r....r)...rX
-00001470: 0000 0072 3000 0000 722f 0000 0075 0c00  ...r0...r/...u..
-00001480: 0000 e7bb 91e5 ae9a e58c bbe7 949f 750c  ..............u.
-00001490: 0000 00e7 94a8 e688 b7e5 a4b4 e583 8f5a  ...............Z
-000014a0: 0b75 7365 725f 6176 6174 6172 7233 0000  .user_avatarr3..
-000014b0: 0075 0c00 0000 e9bb 98e8 aea4 e8a7 92e8  .u..............
-000014c0: 89b2 750f 0000 00e5 8faf e693 8de4 bd9c  ..u.............
-000014d0: e7a7 91e5 aea4 750c 0000 00e6 b3a8 e987  ......u.........
-000014e0: 8ae8 afb4 e698 8e72 3400 0000 7235 0000  .......r4...r5..
-000014f0: 0072 0a00 0000 720b 0000 0072 0f00 0000  .r....r....r....
-00001500: 7210 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00001510: 0000 0000 0000 0100 0000 4000 0000 7310  ..........@...s.
-00001520: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
-00001530: 0253 0029 037a 0955 7365 722e 4d65 7461  .S.).z.User.Meta
-00001540: 750c 0000 00e7 94a8 e688 b7e4 bfa1 e681  u...............
-00001550: af4e 2904 7215 0000 0072 1600 0000 7217  .N).r....r....r.
-00001560: 0000 0072 0c00 0000 7219 0000 0072 1900  ...r....r....r..
-00001570: 0000 7219 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-00001580: 00b2 0000 0073 0200 0000 0802 721b 0000  .....s......r...
-00001590: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-000015a0: 0000 0200 0000 4300 0000 7318 0000 007c  ......C...s....|
-000015b0: 006a 007d 017c 0173 147c 006a 01a0 02a1  .j.}.|.s.|.j....
-000015c0: 007d 017c 0153 0029 0175 8e00 0000 0a20  .}.|.S.).u..... 
-000015d0: 2020 2020 2020 20e8 8eb7 e58f 96e5 bd93         .........
-000015e0: e589 8de7 94a8 e688 b7e9 bb98 e8ae a4e7  ................
-000015f0: 94a8 e688 b7e7 bb84 2c0a 2020 2020 2020  ........,.      
-00001600: 2020 e5a6 82e6 9e9c e69c aae8 aebe e7bd    ..............
-00001610: aeef bc8c e8bf 94e5 9b9e e7ac ace4 b880  ................
-00001620: e4b8 aae7 94a8 e688 b7e7 bb84 0a20 2020  .............   
-00001630: 2020 2020 20e5 90a6 e588 99e8 bf94 e59b       ...........
-00001640: 9ee8 aebe e7bd aee7 9a84 e794 a8e6 88b7  ................
-00001650: e7bb 840a 2020 2020 2020 2020 2903 5a0d  ....        ).Z.
-00001660: 6465 6661 756c 745f 6772 6f75 70da 0667  default_group..g
-00001670: 726f 7570 73da 0566 6972 7374 a902 722e  roups..first..r.
-00001680: 0000 005a 0972 6574 5f67 726f 7570 7219  ...Z.ret_groupr.
-00001690: 0000 0072 1900 0000 721a 0000 00da 1167  ...r....r......g
-000016a0: 6574 5f64 6566 6175 6c74 5f67 726f 7570  et_default_group
-000016b0: ba00 0000 7308 0000 0000 0706 0104 010a  ....s...........
-000016c0: 017a 1655 7365 722e 6765 745f 6465 6661  .z.User.get_defa
-000016d0: 756c 745f 6772 6f75 7063 0100 0000 0000  ult_groupc......
-000016e0: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
-000016f0: 0000 731c 0000 007c 006a 00a0 01a1 007d  ..s....|.j.....}
-00001700: 017c 0173 187c 006a 00a0 02a1 007d 017c  .|.s.|.j.....}.|
-00001710: 0153 00a9 014e 2903 7267 0000 00da 0361  .S...N).rg.....a
-00001720: 6c6c da04 6e6f 6e65 7269 0000 0072 1900  ll..noneri...r..
-00001730: 0000 7219 0000 0072 1a00 0000 da0d 6765  ..r....r......ge
-00001740: 745f 616c 6c67 726f 7570 73c6 0000 0073  t_allgroups....s
-00001750: 0800 0000 0002 0a01 0401 0a01 7a12 5573  ............z.Us
-00001760: 6572 2e67 6574 5f61 6c6c 6772 6f75 7073  er.get_allgroups
-00001770: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00001780: 0001 0000 0043 0000 0073 1800 0000 6401  .....C...s....d.
-00001790: 7d01 7c00 6a00 7d01 7c01 7314 7c00 6a01  }.|.j.}.|.s.|.j.
-000017a0: 7d01 7c01 5300 2902 7533 0000 000a 2020  }.|.S.).u3....  
-000017b0: 2020 2020 2020 e88e b7e5 8f96 e794 a8e6        ..........
-000017c0: 88b7 e9bb 98e8 aea4 e79a 84e7 bb84 e7bb  ................
-000017d0: 87e6 9cba e69e 840a 2020 2020 2020 2020  ........        
-000017e0: 4e29 0272 5f00 0000 724a 0000 0029 0272  N).r_...rJ...).r
-000017f0: 2e00 0000 5a07 7265 745f 6f72 6772 1900  ....Z.ret_orgr..
-00001800: 0000 7219 0000 0072 1a00 0000 da18 6765  ..r....r......ge
-00001810: 745f 6465 6661 756c 745f 6f72 6761 6e69  t_default_organi
-00001820: 7a61 7469 6f6e cd00 0000 730a 0000 0000  zation....s.....
-00001830: 0504 0106 0104 0106 017a 1d55 7365 722e  .........z.User.
-00001840: 6765 745f 6465 6661 756c 745f 6f72 6761  get_default_orga
-00001850: 6e69 7a61 7469 6f6e 4e29 2572 1500 0000  nizationN)%r....
-00001860: 7216 0000 0072 1700 0000 7205 0000 0072  r....r....r....r
-00001870: 3900 0000 723a 0000 0072 3b00 0000 7260  9...r:...r;...r`
-00001880: 0000 0072 6100 0000 725d 0000 0072 5e00  ...ra...r]...r^.
-00001890: 0000 5a09 6964 6361 7264 6e75 6dda 0c49  ..Z.idcardnum..I
-000018a0: 6e74 6567 6572 4669 656c 64da 086f 7264  ntegerField..ord
-000018b0: 6572 5f62 7972 4100 0000 7246 0000 0072  er_byrA...rF...r
-000018c0: 4200 0000 725f 0000 0072 2100 0000 724a  B...r_...r!...rJ
-000018d0: 0000 0072 4f00 0000 5a06 646f 6374 6f72  ...rO...Z.doctor
-000018e0: 5a0a 6176 6174 6172 5f75 726c 5a10 6465  Z.avatar_urlZ.de
-000018f0: 6661 756c 745f 6772 6f75 705f 6964 5a0c  fault_group_idZ.
-00001900: 616c 6c6f 775f 6f66 6669 6365 723c 0000  allow_officer<..
-00001910: 00da 046e 6f74 6572 4400 0000 7245 0000  ...noterD...rE..
-00001920: 0072 1c00 0000 721d 0000 0072 1e00 0000  .r....r....r....
-00001930: 721b 0000 00da 0870 726f 7065 7274 7972  r......propertyr
-00001940: 6a00 0000 726e 0000 0072 6f00 0000 7219  j...rn...ro...r.
-00001950: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-00001960: 0000 7263 0000 008f 0000 0073 4e00 0000  ..rc.......sN...
-00001970: 0801 1201 1201 1001 1401 1201 1201 0401  ................
-00001980: 0201 0201 0401 02fc 0606 0401 0201 0201  ................
-00001990: 0401 02fc 0606 0401 0201 0201 0401 02fc  ................
-000019a0: 0607 1001 1201 1201 1001 1201 1201 1001  ................
-000019b0: 1002 0e08 0201 0a0b 0201 0a06 0201 7263  ..............rc
-000019c0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000019d0: 0000 0000 0700 0000 4000 0000 73cc 0000  ........@...s...
-000019e0: 0065 005a 0164 005a 0264 015a 0365 046a  .e.Z.d.Z.d.Z.e.j
-000019f0: 0565 0665 046a 0764 0264 0364 0364 048d  .e.e.j.d.d.d.d..
-00001a00: 055a 0865 046a 0964 0564 0664 078d 025a  .Z.e.j.d.d.d...Z
-00001a10: 0a65 046a 0964 0564 0864 0364 098d 035a  .e.j.d.d.d.d...Z
-00001a20: 0b65 046a 0c64 0364 0a64 0364 0b8d 035a  .e.j.d.d.d.d...Z
-00001a30: 0d65 046a 0964 0c64 0564 0364 0364 0d8d  .e.j.d.d.d.d.d..
-00001a40: 045a 0e65 046a 0f65 1064 0e65 046a 0764  .Z.e.j.e.d.e.j.d
-00001a50: 0f64 0364 108d 055a 1165 046a 1264 1164  .d.d...Z.e.j.d.d
-00001a60: 1264 0364 138d 035a 1365 046a 0964 0564  .d.d...Z.e.j.d.d
-00001a70: 1464 0364 0364 158d 045a 1465 046a 1564  .d.d.d...Z.e.j.d
-00001a80: 1664 0364 0364 178d 035a 1665 046a 1564  .d.d.d...Z.e.j.d
-00001a90: 1864 0364 0364 198d 035a 1747 0064 1a64  .d.d.d...Z.G.d.d
-00001aa0: 1b84 0064 1b83 025a 1864 1c53 0029 1dda  ...d...Z.d.S.)..
-00001ab0: 0a45 7874 7261 4772 6f75 7075 1900 0000  .ExtraGroupu....
-00001ac0: 0a20 2020 20e8 a792 e889 b2e6 89a9 e585  .    ...........
-00001ad0: 85e8 a1a8 0a20 2020 20da 0b65 7874 7261  .....    ..extra
-00001ae0: 5f67 726f 7570 5429 0472 3100 0000 da0c  _groupT).r1.....
-00001af0: 7265 6c61 7465 645f 6e61 6d65 720e 0000  related_namer...
-00001b00: 0072 2900 0000 725a 0000 0075 0c00 0000  .r)...rZ...u....
-00001b10: e8a7 92e8 89b2 e4bb a3e7 a081 a902 7225  ..............r%
-00001b20: 0000 0072 0c00 0000 750c 0000 00e8 a792  ...r....u.......
-00001b30: e889 b2e5 908d e7a7 b029 0372 2500 0000  .........).r%...
-00001b40: 720c 0000 0072 2900 0000 7212 0000 0029  r....r)...r....)
-00001b50: 0372 1400 0000 720c 0000 0072 0e00 0000  .r....r....r....
-00001b60: 7506 0000 00e6 8f8f e8bf b029 0372 2500  u..........).r%.
-00001b70: 0000 720e 0000 0072 2900 0000 722f 0000  ..r....r)...r/..
-00001b80: 0072 6700 0000 a904 720c 0000 0072 3100  .rg.....r....r1.
-00001b90: 0000 7276 0000 0072 0e00 0000 7264 0000  ..rv...r....rd..
-00001ba0: 0072 6500 0000 a903 720c 0000 0072 1400  .re.....r....r..
-00001bb0: 0000 720e 0000 0072 3400 0000 a904 7225  ..r....r4.....r%
-00001bc0: 0000 0072 0c00 0000 720e 0000 0072 2900  ...r....r....r).
-00001bd0: 0000 720a 0000 0072 0b00 0000 7512 0000  ..r....r....u...
-00001be0: 00e6 9c80 e590 8ee6 9bb4 e696 b0e6 97b6  ................
-00001bf0: e997 b472 1000 0000 6300 0000 0000 0000  ...r....c.......
-00001c00: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
-00001c10: 0073 1c00 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
-00001c20: 5a03 6402 5a04 6504 5a05 6403 5a06 6404  Z.d.Z.e.Z.d.Z.d.
-00001c30: 5300 2905 7a0f 4578 7472 6147 726f 7570  S.).z.ExtraGroup
-00001c40: 2e4d 6574 615a 0e62 735f 6578 7472 615f  .MetaZ.bs_extra_
-00001c50: 6772 6f75 7075 0600 0000 e8a7 92e8 89b2  groupu..........
-00001c60: 2901 2902 da09 726f 6c65 5f63 6f64 6572  ).)...role_coder
-00001c70: 4a00 0000 4e72 4b00 0000 7219 0000 0072  J...NrK...r....r
-00001c80: 1900 0000 7219 0000 0072 1a00 0000 721b  ....r....r....r.
-00001c90: 0000 00ee 0000 0073 0800 0000 0801 0401  .......s........
-00001ca0: 0401 0401 721b 0000 004e 2919 7215 0000  ....r....N).r...
-00001cb0: 0072 1600 0000 7217 0000 00da 075f 5f64  .r....r......__d
-00001cc0: 6f63 5f5f 7205 0000 00da 0d4f 6e65 546f  oc__r......OneTo
-00001cd0: 4f6e 6546 6965 6c64 7203 0000 0072 4200  OneFieldr....rB.
-00001ce0: 0000 da05 6772 6f75 7072 3900 0000 727b  ....groupr9...r{
-00001cf0: 0000 005a 0972 6f6c 655f 6e61 6d65 721f  ...Z.role_namer.
-00001d00: 0000 0072 2000 0000 7272 0000 0072 4100  ...r ...rr...rA.
-00001d10: 0000 7221 0000 0072 4a00 0000 7270 0000  ..r!...rJ...rp..
-00001d20: 0072 7100 0000 5a0c 6372 6561 7465 645f  .rq...Z.created_
-00001d30: 7573 6572 721c 0000 005a 0a63 7265 6174  userr....Z.creat
-00001d40: 6564 5f61 745a 0a75 7064 6174 6564 5f61  ed_atZ.updated_a
-00001d50: 7472 1b00 0000 7219 0000 0072 1900 0000  tr....r....r....
-00001d60: 7219 0000 0072 1a00 0000 7274 0000 00d9  r....r....rt....
-00001d70: 0000 0073 2400 0000 0801 0403 1601 0e01  ...s$...........
-00001d80: 1001 1001 1201 0401 0201 0201 0401 0201  ................
-00001d90: 02fb 0607 1001 1201 1001 1002 7274 0000  ............rt..
-00001da0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00001db0: 0000 0700 0000 4000 0000 738c 0000 0065  ......@...s....e
-00001dc0: 005a 0164 005a 0264 015a 0365 046a 0564  .Z.d.Z.d.Z.e.j.d
-00001dd0: 0264 0364 048d 025a 0665 046a 0764 0564  .d.d...Z.e.j.d.d
-00001de0: 0664 078d 025a 0865 046a 0964 0864 0964  .d...Z.e.j.d.d.d
-00001df0: 0664 0a8d 035a 0a65 046a 0964 0b64 0964  .d...Z.e.j.d.d.d
-00001e00: 0664 0664 0c8d 045a 0b65 046a 0564 0d64  .d.d...Z.e.j.d.d
-00001e10: 0e64 0664 0664 0f8d 045a 0c65 046a 0d64  .d.d.d...Z.e.j.d
-00001e20: 1064 1165 046a 0e64 1264 0664 138d 055a  .d.e.j.d.d.d...Z
-00001e30: 0f47 0064 1464 1584 0064 1583 025a 1064  .G.d.d...d...Z.d
-00001e40: 1664 1784 005a 1164 1853 0029 19da 1043  .d...Z.d.S.)...C
-00001e50: 6f6e 7465 6e74 5479 7065 4361 7465 7375  ontentTypeCatesu
-00001e60: 1600 0000 0a20 2020 20e8 8f9c e58d 95e5  .....    .......
-00001e70: 908d e7a7 b00a 2020 2020 7222 0000 0072  ......    r"...r
-00001e80: 5000 0000 2901 7225 0000 0072 1200 0000  P...).r%...r....
-00001e90: 5429 0172 1400 0000 7264 0000 0072 6500  T).r....rd...re.
-00001ea0: 0000 7279 0000 0075 0600 0000 e7ba a7e5  ..ry...u........
-00001eb0: 88ab 7266 0000 00f5 0600 0000 e59b bee6  ..rf............
-00001ec0: a087 e9f4 0100 0072 2800 0000 722e 0000  .......r(...r...
-00001ed0: 0075 0c00 0000 e788 b6e7 baa7 e88f 9ce5  .u..............
-00001ee0: 8d95 da08 6368 696c 6472 656e 7278 0000  ....childrenrx..
-00001ef0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00001f00: 0000 0100 0000 4000 0000 731c 0000 0065  ......@...s....e
-00001f10: 005a 0164 005a 0264 015a 0364 025a 0465  .Z.d.Z.d.Z.d.Z.e
-00001f20: 045a 0564 035a 0664 0453 0029 057a 1543  .Z.d.Z.d.S.).z.C
-00001f30: 6f6e 7465 6e74 5479 7065 4361 7465 732e  ontentTypeCates.
-00001f40: 4d65 7461 5a14 6273 5f63 6f6e 7465 6e74  MetaZ.bs_content
-00001f50: 5f74 7970 655f 6361 7473 750c 0000 00e8  _type_catsu.....
-00001f60: 8f9c e58d 95e5 908d e7a7 b0a9 0172 7100  .............rq.
-00001f70: 0000 4ea9 0772 1500 0000 7216 0000 0072  ..N..r....r....r
-00001f80: 1700 0000 7237 0000 0072 0c00 0000 7238  ....r7...r....r8
-00001f90: 0000 00da 086f 7264 6572 696e 6772 1900  .....orderingr..
-00001fa0: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00001fb0: 0072 1b00 0000 0801 0000 7308 0000 0008  .r........s.....
-00001fc0: 0104 0104 0104 0172 1b00 0000 6301 0000  .......r....c...
-00001fd0: 0000 0000 0000 0000 0001 0000 0001 0000  ................
-00001fe0: 0043 0000 0073 0600 0000 7c00 6a00 5300  .C...s....|.j.S.
-00001ff0: 726b 0000 00a9 0172 3a00 0000 a901 722e  rk.....r:.....r.
-00002000: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-00002010: 0000 da07 5f5f 7374 725f 5f0e 0100 0073  ....__str__....s
-00002020: 0200 0000 0001 7a18 436f 6e74 656e 7454  ......z.ContentT
-00002030: 7970 6543 6174 6573 2e5f 5f73 7472 5f5f  ypeCates.__str__
-00002040: 4e29 1272 1500 0000 7216 0000 0072 1700  N).r....r....r..
-00002050: 0000 727c 0000 0072 0500 0000 7239 0000  ..r|...r....r9..
-00002060: 0072 3a00 0000 721f 0000 0072 2000 0000  .r:...r....r ...
-00002070: 7270 0000 0072 7100 0000 da05 6c65 7665  rp...rq.....leve
-00002080: 6cda 0a69 636f 6e5f 636c 6173 7372 4100  l..icon_classrA.
-00002090: 0000 7242 0000 0072 4300 0000 721b 0000  ..rB...rC...r...
-000020a0: 0072 8800 0000 7219 0000 0072 1900 0000  .r....r....r....
-000020b0: 7219 0000 0072 1a00 0000 727f 0000 00f7  r....r....r.....
-000020c0: 0000 0073 1e00 0000 0801 0403 0e01 0e01  ...s............
-000020d0: 1001 1201 1201 0401 0201 0201 0401 0201  ................
-000020e0: 02fb 0608 0e06 727f 0000 0063 0000 0000  ......r....c....
-000020f0: 0000 0000 0000 0000 0000 0000 0600 0000  ................
-00002100: 4000 0000 73ce 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-00002110: 0264 015a 0365 046a 0564 0264 0364 0464  .d.Z.e.j.d.d.d.d
-00002120: 058d 035a 0665 046a 0765 0864 0665 046a  ...Z.e.j.e.d.e.j
-00002130: 0964 0764 088d 045a 0a65 046a 0764 0964  .d.d...Z.e.j.d.d
-00002140: 0a65 046a 0964 0b64 088d 045a 0b65 046a  .e.j.d.d...Z.e.j
-00002150: 0564 0c64 0d64 0464 0464 0e8d 045a 0c65  .d.d.d.d.d...Z.e
-00002160: 046a 0d64 0f64 0464 0464 108d 035a 0e65  .j.d.d.d.d...Z.e
-00002170: 046a 0d64 1164 0464 0464 108d 035a 0f65  .j.d.d.d.d...Z.e
-00002180: 046a 0564 1264 1364 0464 148d 035a 1065  .j.d.d.d.d...Z.e
-00002190: 046a 1164 1564 0464 168d 025a 1265 046a  .j.d.d.d...Z.e.j
-000021a0: 1364 1764 0464 0464 188d 035a 1465 046a  .d.d.d.d...Z.e.j
-000021b0: 1564 1964 1a64 0464 1b8d 035a 1647 0064  .d.d.d.d...Z.G.d
-000021c0: 1c64 1d84 0064 1d83 025a 1764 1e64 1f84  .d...d...Z.d.d..
-000021d0: 005a 1864 2053 0029 21da 0d43 6f6e 7465  .Z.d S.)!..Conte
-000021e0: 6e74 5479 7065 4578 7516 0000 000a 2020  ntTypeExu.....  
-000021f0: 2020 e58a 9fe8 83bd e7b1 bbe5 88ab 0a20    ............. 
-00002200: 2020 2072 2200 0000 7250 0000 0054 2902     r"...rP...T).
-00002210: 7225 0000 0072 0e00 0000 750c 0000 00e7  r%...r....u.....
-00002220: b3bb e7bb 9fe5 ba94 e794 a8da 0965 7874  .............ext
-00002230: 656e 7369 6f6e 2903 720c 0000 0072 3100  ension).r....r1.
-00002240: 0000 7276 0000 0072 7f00 0000 7506 0000  ..rv...r....u...
-00002250: 00e8 8f9c e58d 955a 0d63 6f6e 7465 6e74  .......Z.content
-00002260: 5f63 6174 6573 7280 0000 0072 8100 0000  _catesr....r....
-00002270: 7228 0000 00da 0375 726c 722a 0000 0075  r(.....urlr*...u
-00002280: 0600 0000 e7bb 84e6 8890 7506 0000 00e5  ..........u.....
-00002290: 8f82 e695 b072 5a00 0000 a903 720c 0000  .....rZ.....r...
-000022a0: 0072 2500 0000 720e 0000 0075 0900 0000  .r%...r....u....
-000022b0: e987 8de5 ae9a e590 91a9 0272 0c00 0000  ...........r....
-000022c0: 720e 0000 0072 1200 0000 2902 7214 0000  r....r....).r...
-000022d0: 0072 0e00 0000 7264 0000 0072 6500 0000  .r....rd...re...
-000022e0: 7279 0000 0063 0000 0000 0000 0000 0000  ry...c..........
-000022f0: 0000 0000 0000 0100 0000 4000 0000 731c  ..........@...s.
-00002300: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
-00002310: 025a 0465 045a 0564 035a 0664 0453 0029  .Z.e.Z.d.Z.d.S.)
-00002320: 057a 1243 6f6e 7465 6e74 5479 7065 4578  .z.ContentTypeEx
-00002330: 2e4d 6574 615a 1262 735f 636f 6e74 656e  .MetaZ.bs_conten
-00002340: 745f 7479 7065 5f65 7875 1200 0000 e58a  t_type_exu......
-00002350: 9fe8 83bd e7b1 bbe5 88ab e8a1 a5e5 8585  ................
-00002360: 7283 0000 004e 7284 0000 0072 1900 0000  r....Nr....r....
-00002370: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
-00002380: 1b00 0000 2b01 0000 7308 0000 0008 0104  ....+...s.......
-00002390: 0104 0104 0172 1b00 0000 6301 0000 0000  .....r....c.....
-000023a0: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-000023b0: 0000 0073 0600 0000 7c00 6a00 5300 726b  ...s....|.j.S.rk
-000023c0: 0000 0072 8600 0000 7287 0000 0072 1900  ...r....r....r..
-000023d0: 0000 7219 0000 0072 1a00 0000 7288 0000  ..r....r....r...
-000023e0: 0031 0100 0073 0200 0000 0001 7a15 436f  .1...s......z.Co
-000023f0: 6e74 656e 7454 7970 6545 782e 5f5f 7374  ntentTypeEx.__st
-00002400: 725f 5f4e 2919 7215 0000 0072 1600 0000  r__N).r....r....
-00002410: 7217 0000 0072 7c00 0000 7205 0000 0072  r....r|...r....r
-00002420: 3900 0000 723a 0000 0072 4100 0000 7204  9...r:...rA...r.
-00002430: 0000 0072 4200 0000 da0c 636f 6e74 656e  ...rB.....conten
-00002440: 745f 7479 7065 5a10 636f 6e74 656e 745f  t_typeZ.content_
-00002450: 7479 7065 5f63 6174 728a 0000 0072 3c00  type_catr....r<.
-00002460: 0000 da09 6672 6f6e 745f 7572 6c5a 0f66  ....front_urlZ.f
-00002470: 726f 6e74 5f63 6f6d 706f 6e65 6e74 5a0c  ront_componentZ.
-00002480: 6672 6f6e 745f 7061 7261 6d73 da08 5552  front_params..UR
-00002490: 4c46 6965 6c64 5a12 6672 6f6e 745f 7265  LFieldZ.front_re
-000024a0: 6469 7265 6374 5f75 726c 721f 0000 0072  direct_urlr....r
-000024b0: 2000 0000 7270 0000 0072 7100 0000 721b   ...rp...rq...r.
-000024c0: 0000 0072 8800 0000 7219 0000 0072 1900  ...r....r....r..
-000024d0: 0000 7219 0000 0072 1a00 0000 728b 0000  ..r....r....r...
-000024e0: 0012 0100 0073 2e00 0000 0801 0403 1001  .....s..........
-000024f0: 0401 0201 0201 0401 02fc 0606 0401 0201  ................
-00002500: 0201 0401 02fc 0606 1201 1001 1001 1001  ................
-00002510: 0e01 1001 1002 0e06 728b 0000 0063 0000  ........r....c..
-00002520: 0000 0000 0000 0000 0000 0000 0000 0400  ................
-00002530: 0000 4000 0000 733a 0000 0065 005a 0164  ..@...s:...e.Z.d
-00002540: 005a 0264 015a 0365 046a 0564 0264 0364  .Z.d.Z.e.j.d.d.d
-00002550: 048d 025a 0665 046a 0564 0564 0364 048d  ...Z.e.j.d.d.d..
-00002560: 025a 0747 0064 0664 0784 0064 0783 025a  .Z.G.d.d...d...Z
-00002570: 0864 0853 0029 09da 0b45 7870 656e 7365  .d.S.)...Expense
-00002580: 5479 7065 7516 0000 000a 2020 2020 e8b4  Typeu.....    ..
-00002590: b9e7 94a8 e7b1 bbe5 9e8b 0a20 2020 2072  ...........    r
-000025a0: 2200 0000 7251 0000 0072 2400 0000 722b  "...rQ...r$...r+
-000025b0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000025c0: 0000 0000 0100 0000 4000 0000 7318 0000  ........@...s...
-000025d0: 0065 005a 0164 005a 0264 015a 0364 025a  .e.Z.d.Z.d.Z.d.Z
-000025e0: 0465 045a 0564 0353 0029 047a 1045 7870  .e.Z.d.S.).z.Exp
-000025f0: 656e 7365 5479 7065 2e4d 6574 615a 0f62  enseType.MetaZ.b
-00002600: 735f 6578 7065 6e73 655f 7479 7065 f50c  s_expense_type..
-00002610: 0000 00e8 b4b9 e794 a8e7 b1bb e59e 8b4e  ...............N
-00002620: 7236 0000 0072 1900 0000 7219 0000 0072  r6...r....r....r
-00002630: 1900 0000 721a 0000 0072 1b00 0000 3c01  ....r....r....<.
-00002640: 0000 7306 0000 0008 0104 0104 0172 1b00  ..s..........r..
-00002650: 0000 4e29 0972 1500 0000 7216 0000 0072  ..N).r....r....r
-00002660: 1700 0000 727c 0000 0072 0500 0000 7239  ....r|...r....r9
-00002670: 0000 0072 3a00 0000 da04 636f 6465 721b  ...r:.....coder.
-00002680: 0000 0072 1900 0000 7219 0000 0072 1900  ...r....r....r..
-00002690: 0000 721a 0000 0072 9300 0000 3501 0000  ..r....r....5...
-000026a0: 7308 0000 0008 0104 030e 010e 0272 9300  s............r..
-000026b0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-000026c0: 0000 0006 0000 0040 0000 0073 9c00 0000  .......@...s....
-000026d0: 6500 5a01 6400 5a02 6503 6a04 6401 6402  e.Z.d.Z.e.j.d.d.
-000026e0: 6403 6404 8d03 5a05 6503 6a04 6405 6402  d.d...Z.e.j.d.d.
-000026f0: 6406 8d02 5a06 6503 6a04 6407 6408 6406  d...Z.e.j.d.d.d.
-00002700: 8d02 5a07 6503 6a08 6409 6403 640a 8d02  ..Z.e.j.d.d.d...
-00002710: 5a09 6503 6a0a 650b 640b 6503 6a0c 6403  Z.e.j.e.d.e.j.d.
-00002720: 640c 8d04 5a0d 6503 6a04 640d 6402 6403  d...Z.e.j.d.d.d.
-00002730: 6403 640e 8d04 5a0e 6503 6a04 640f 6402  d.d...Z.e.j.d.d.
-00002740: 6403 6403 640e 8d04 5a0f 6503 6a10 6511  d.d.d...Z.e.j.e.
-00002750: 6410 6403 6411 8d03 5a12 4700 6412 6413  d.d.d...Z.G.d.d.
-00002760: 8400 6413 8302 5a13 6414 5300 2915 da0f  ..d...Z.d.S.)...
-00002770: 4578 7065 6e73 6553 7461 6e64 6172 6472  ExpenseStandardr
-00002780: 9400 0000 7227 0000 0054 728e 0000 0075  ....r'...Tr....u
-00002790: 0c00 0000 e6a0 87e5 8786 e590 8de7 a7b0  ................
-000027a0: 7224 0000 0075 0c00 0000 e6a0 87e5 8786  r$...u..........
-000027b0: e7bc 96e7 a081 7223 0000 0075 0600 0000  ......r#...u....
-000027c0: e8b4 b9e7 94a8 728f 0000 0072 2f00 0000  ......r....r/...
-000027d0: 7230 0000 0072 3400 0000 7228 0000 0072  r0...r4...r(...r
-000027e0: 3500 0000 7512 0000 00e5 8cbb e794 9fe8  5...u...........
-000027f0: b4b9 e794 a8e6 a087 e587 8629 0272 0c00  ...........).r..
-00002800: 0000 7229 0000 0063 0000 0000 0000 0000  ..r)...c........
-00002810: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
-00002820: 731c 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
-00002830: 0364 025a 0465 045a 0564 035a 0664 0453  .d.Z.e.Z.d.Z.d.S
-00002840: 0029 057a 1445 7870 656e 7365 5374 616e  .).z.ExpenseStan
-00002850: 6461 7264 2e4d 6574 615a 1362 735f 6578  dard.MetaZ.bs_ex
-00002860: 7065 6e73 655f 7374 616e 6461 7264 750f  pense_standardu.
-00002870: 0000 00e8 b4b9 e794 a8e6 a087 e587 86e8  ................
-00002880: a1a8 2901 2902 da0d 7374 616e 6461 7264  ..).)...standard
-00002890: 5f63 6f64 6572 4a00 0000 4e72 4b00 0000  _coderJ...NrK...
-000028a0: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-000028b0: 1a00 0000 721b 0000 0052 0100 0073 0800  ....r....R...s..
-000028c0: 0000 0801 0401 0401 0401 721b 0000 004e  ..........r....N
-000028d0: 2914 7215 0000 0072 1600 0000 7217 0000  ).r....r....r...
-000028e0: 0072 0500 0000 7239 0000 005a 0c65 7870  .r....r9...Z.exp
-000028f0: 656e 7365 5f74 7970 655a 0d73 7461 6e64  ense_typeZ.stand
-00002900: 6172 645f 6e61 6d65 7297 0000 0072 4000  ard_namer....r@.
-00002910: 0000 5a04 6665 6573 7241 0000 0072 2100  ..Z.feesrA...r!.
-00002920: 0000 7242 0000 0072 4a00 0000 7244 0000  ..rB...rJ...rD..
-00002930: 0072 4500 0000 da0f 4d61 6e79 546f 4d61  .rE.....ManyToMa
-00002940: 6e79 4669 656c 6472 4f00 0000 5a07 646f  nyFieldrO...Z.do
-00002950: 6374 6f72 7372 1b00 0000 7219 0000 0072  ctorsr....r....r
-00002960: 1900 0000 7219 0000 0072 1a00 0000 7296  ....r....r....r.
-00002970: 0000 0042 0100 0073 1c00 0000 0802 1001  ...B...s........
-00002980: 0e01 0e01 0e01 0401 0201 0201 0401 02fc  ................
-00002990: 0606 1201 1201 1002 7296 0000 0063 0000  ........r....c..
-000029a0: 0000 0000 0000 0000 0000 0000 0000 0700  ................
-000029b0: 0000 4000 0000 734c 0000 0065 005a 0164  ..@...sL...e.Z.d
-000029c0: 005a 0265 036a 0464 0164 0264 038d 025a  .Z.e.j.d.d.d...Z
-000029d0: 0565 036a 0464 0464 0264 038d 025a 0665  .e.j.d.d.d...Z.e
-000029e0: 036a 0764 0564 0665 036a 0864 0764 0864  .j.d.d.e.j.d.d.d
-000029f0: 098d 055a 0947 0064 0a64 0b84 0064 0b83  ...Z.G.d.d...d..
-00002a00: 025a 0a64 0c53 0029 0dda 0e49 6e73 7065  .Z.d.S.)...Inspe
-00002a10: 6374 696f 6e54 7970 65f5 1200 0000 e6a3  ctionType.......
-00002a20: 80e6 9fa5 e7b1 bbe5 9e8b e7bc 96e7 a081  ................
-00002a30: 725a 0000 0072 2400 0000 f512 0000 00e6  rZ...r$.........
-00002a40: a380 e69f a5e7 b1bb e59e 8be5 908d e7a7  ................
-00002a50: b072 2e00 0000 f506 0000 00e7 88b6 e7ba  .r..............
-00002a60: a772 8200 0000 5472 7800 0000 6300 0000  .r....Trx...c...
-00002a70: 0000 0000 0000 0000 0000 0000 0001 0000  ................
-00002a80: 0040 0000 0073 1800 0000 6500 5a01 6400  .@...s....e.Z.d.
-00002a90: 5a02 6401 5a03 6402 5a04 6504 5a05 6403  Z.d.Z.d.Z.e.Z.d.
-00002aa0: 5300 2904 7a13 496e 7370 6563 7469 6f6e  S.).z.Inspection
-00002ab0: 5479 7065 2e4d 6574 615a 1262 735f 696e  Type.MetaZ.bs_in
-00002ac0: 7370 6563 7469 6f6e 5f74 7970 6575 1200  spection_typeu..
-00002ad0: 0000 e6a3 80e6 9fa5 e5ad 97e5 85b8 e7b1  ................
-00002ae0: bbe5 9e8b 4e72 3600 0000 7219 0000 0072  ....Nr6...r....r
-00002af0: 1900 0000 7219 0000 0072 1a00 0000 721b  ....r....r....r.
-00002b00: 0000 0066 0100 0073 0600 0000 0801 0401  ...f...s........
-00002b10: 0401 721b 0000 004e a90b 7215 0000 0072  ..r....N..r....r
-00002b20: 1600 0000 7217 0000 0072 0500 0000 7239  ....r....r....r9
-00002b30: 0000 00da 0a63 6f64 655f 7372 7674 70da  .....code_srvtp.
-00002b40: 0a6e 616d 655f 7372 7674 7072 4100 0000  .name_srvtprA...
-00002b50: 7242 0000 0072 4300 0000 721b 0000 0072  rB...rC...r....r
-00002b60: 1900 0000 7219 0000 0072 1900 0000 721a  ....r....r....r.
-00002b70: 0000 0072 9900 0000 5b01 0000 7314 0000  ...r....[...s...
-00002b80: 0008 010e 010e 0104 0102 0102 0104 0102  ................
-00002b90: 0102 fb06 0872 9900 0000 6300 0000 0000  .....r....c.....
-00002ba0: 0000 0000 0000 0000 0000 0006 0000 0040  ...............@
-00002bb0: 0000 0073 a600 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00002bc0: 6503 6a04 6401 6402 6403 6404 8d03 5a05  e.j.d.d.d.d...Z.
-00002bd0: 6503 6a04 6405 6406 6407 8d02 5a06 6503  e.j.d.d.d...Z.e.
-00002be0: 6a04 6408 6409 6407 8d02 5a07 6503 6a04  j.d.d.d...Z.e.j.
-00002bf0: 6408 640a 6407 8d02 5a08 6503 6a09 640b  d.d.d...Z.e.j.d.
-00002c00: 6403 640c 8d02 5a0a 6503 6a04 6408 640d  d.d...Z.e.j.d.d.
-00002c10: 6403 6403 640e 8d04 5a0b 6503 6a04 6408  d.d.d...Z.e.j.d.
-00002c20: 640f 6403 6403 640e 8d04 5a0c 6503 6a04  d.d.d.d...Z.e.j.
-00002c30: 6410 6411 6403 6412 8d03 5a0d 6503 6a04  d.d.d.d...Z.e.j.
-00002c40: 6413 6411 6403 6412 8d03 5a0e 4700 6414  d.d.d.d...Z.G.d.
-00002c50: 6415 8400 6415 8302 5a0f 6416 5300 2917  d...d...Z.d.S.).
-00002c60: da16 496e 7370 6563 7469 6f6e 4469 6374  ..InspectionDict
-00002c70: 696f 6e61 7269 6573 7223 0000 00f5 0c00  ionariesr#......
-00002c80: 0000 e9a1 b9e7 9bae e7bc 96e7 a081 5472  ..............Tr
-00002c90: 2c00 0000 7251 0000 00f5 0c00 0000 e9a1  ,...rQ..........
-00002ca0: b9e7 9bae e590 8de7 a7b0 7277 0000 00e9  ..........rw....
-00002cb0: 8000 0000 f50c 0000 00e5 8cbb e999 a2e7  ................
-00002cc0: bc96 e7a0 8172 4700 0000 f50c 0000 00e9  .....rG.........
-00002cd0: a1b9 e79b aee8 b4b9 e794 a872 8f00 0000  ...........r....
-00002ce0: f506 0000 00e5 a487 e6b3 a872 7a00 0000  ...........rz...
-00002cf0: f50c 0000 00e5 8cba e588 86e5 ad97 e6ae  ................
-00002d00: b572 9a00 0000 725a 0000 0072 8e00 0000  .r....rZ...r....
-00002d10: 729b 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00002d20: 0000 0000 0000 0100 0000 4000 0000 7318  ..........@...s.
-00002d30: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
-00002d40: 025a 0465 045a 0564 0353 0029 047a 1b49  .Z.e.Z.d.S.).z.I
-00002d50: 6e73 7065 6374 696f 6e44 6963 7469 6f6e  nspectionDiction
-00002d60: 6172 6965 732e 4d65 7461 5a1a 6273 5f69  aries.MetaZ.bs_i
-00002d70: 6e73 7065 6374 696f 6e5f 6469 6374 696f  nspection_dictio
-00002d80: 6e61 7269 6573 750c 0000 00e6 a380 e69f  nariesu.........
-00002d90: a5e5 ad97 e585 b84e 7236 0000 0072 1900  .......Nr6...r..
-00002da0: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00002db0: 0072 1b00 0000 7701 0000 7306 0000 0008  .r....w...s.....
-00002dc0: 0104 0104 0172 1b00 0000 4ea9 1072 1500  .....r....N..r..
-00002dd0: 0000 7216 0000 0072 1700 0000 7205 0000  ..r....r....r...
-00002de0: 0072 3900 0000 5a0c 7072 6f6a 6563 745f  .r9...Z.project_
-00002df0: 636f 6465 5a0c 7072 6f6a 6563 745f 6e61  codeZ.project_na
-00002e00: 6d65 da0d 686f 7370 6974 616c 5f63 6f64  me..hospital_cod
-00002e10: 655a 0b6f 6666 6963 655f 636f 6465 7240  eZ.office_coder@
-00002e20: 0000 005a 0c70 726f 6a65 6374 5f66 6565  ...Z.project_fee
-00002e30: 735a 0772 656d 6172 6b73 5a0b 6469 7374  sZ.remarksZ.dist
-00002e40: 696e 6775 6973 6872 9e00 0000 729f 0000  inguishr....r...
-00002e50: 0072 1b00 0000 7219 0000 0072 1900 0000  .r....r....r....
-00002e60: 7219 0000 0072 1a00 0000 72a0 0000 006c  r....r....r....l
-00002e70: 0100 0073 1400 0000 0801 1001 0e01 0e01  ...s............
-00002e80: 0e01 0e01 1201 1201 1001 1002 72a0 0000  ............r...
-00002e90: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00002ea0: 0000 0700 0000 4000 0000 734c 0000 0065  ......@...sL...e
-00002eb0: 005a 0164 005a 0265 036a 0464 0164 0264  .Z.d.Z.e.j.d.d.d
-00002ec0: 038d 025a 0565 036a 0464 0464 0264 038d  ...Z.e.j.d.d.d..
-00002ed0: 025a 0665 036a 0764 0564 0665 036a 0864  .Z.e.j.d.d.e.j.d
-00002ee0: 0764 0864 098d 055a 0947 0064 0a64 0b84  .d.d...Z.G.d.d..
-00002ef0: 0064 0b83 025a 0a64 0c53 0029 0dda 0f45  .d...Z.d.S.)...E
-00002f00: 7861 6d69 6e61 7469 6f6e 5479 7065 729a  xaminationTyper.
-00002f10: 0000 0072 5a00 0000 7224 0000 0072 9b00  ...rZ...r$...r..
-00002f20: 0000 722e 0000 0072 9c00 0000 7282 0000  ..r....r....r...
-00002f30: 0054 7278 0000 0063 0000 0000 0000 0000  .Trx...c........
-00002f40: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
-00002f50: 7318 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
-00002f60: 0364 025a 0465 045a 0564 0353 0029 047a  .d.Z.e.Z.d.S.).z
-00002f70: 1445 7861 6d69 6e61 7469 6f6e 5479 7065  .ExaminationType
-00002f80: 2e4d 6574 615a 1362 735f 6578 616d 696e  .MetaZ.bs_examin
-00002f90: 6174 696f 6e5f 7479 7065 7512 0000 00e6  ation_typeu.....
-00002fa0: a380 e9aa 8ce5 ad97 e585 b8e7 b1bb e59e  ................
-00002fb0: 8b4e 7236 0000 0072 1900 0000 7219 0000  .Nr6...r....r...
-00002fc0: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00002fd0: 8801 0000 7306 0000 0008 0104 0104 0172  ....s..........r
-00002fe0: 1b00 0000 4e72 9d00 0000 7219 0000 0072  ....Nr....r....r
-00002ff0: 1900 0000 7219 0000 0072 1a00 0000 72aa  ....r....r....r.
-00003000: 0000 007d 0100 0073 1400 0000 0801 0e01  ...}...s........
-00003010: 0e01 0401 0201 0201 0401 0201 02fb 0608  ................
-00003020: 72aa 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00003030: 0000 0000 0000 0600 0000 4000 0000 73a6  ..........@...s.
-00003040: 0000 0065 005a 0164 005a 0265 036a 0464  ...e.Z.d.Z.e.j.d
-00003050: 0164 0264 0364 048d 035a 0565 036a 0464  .d.d.d...Z.e.j.d
-00003060: 0564 0664 078d 025a 0665 036a 0464 0864  .d.d...Z.e.j.d.d
-00003070: 0964 078d 025a 0765 036a 0464 0864 0a64  .d...Z.e.j.d.d.d
-00003080: 078d 025a 0865 036a 0964 0b64 0364 0c8d  ...Z.e.j.d.d.d..
-00003090: 025a 0a65 036a 0464 0864 0d64 0364 0364  .Z.e.j.d.d.d.d.d
-000030a0: 0e8d 045a 0b65 036a 0464 0864 0f64 0364  ...Z.e.j.d.d.d.d
-000030b0: 0364 0e8d 045a 0c65 036a 0464 1064 1164  .d...Z.e.j.d.d.d
-000030c0: 0364 128d 035a 0d65 036a 0464 1364 1164  .d...Z.e.j.d.d.d
-000030d0: 0364 128d 035a 0e47 0064 1464 1584 0064  .d...Z.G.d.d...d
-000030e0: 1583 025a 0f64 1653 0029 17da 1745 7861  ...Z.d.S.)...Exa
-000030f0: 6d69 6e61 7469 6f6e 4469 6374 696f 6e61  minationDictiona
-00003100: 7269 6573 7223 0000 0072 a100 0000 5472  riesr#...r....Tr
-00003110: 2c00 0000 7251 0000 0072 a200 0000 7277  ,...rQ...r....rw
-00003120: 0000 0072 a300 0000 72a4 0000 0072 4700  ...r....r....rG.
-00003130: 0000 72a5 0000 0072 8f00 0000 72a6 0000  ..r....r....r...
-00003140: 0072 7a00 0000 72a7 0000 0075 1200 0000  .rz...r....u....
-00003150: e6a3 80e9 aa8c e7b1 bbe5 9e8b e7bc 96e7  ................
-00003160: a081 725a 0000 0072 8e00 0000 7512 0000  ..rZ...r....u...
-00003170: 00e6 a380 e9aa 8ce7 b1bb e59e 8be5 908d  ................
-00003180: e7a7 b063 0000 0000 0000 0000 0000 0000  ...c............
-00003190: 0000 0000 0100 0000 4000 0000 7318 0000  ........@...s...
-000031a0: 0065 005a 0164 005a 0264 015a 0364 025a  .e.Z.d.Z.d.Z.d.Z
-000031b0: 0465 045a 0564 0353 0029 047a 1c45 7861  .e.Z.d.S.).z.Exa
-000031c0: 6d69 6e61 7469 6f6e 4469 6374 696f 6e61  minationDictiona
-000031d0: 7269 6573 2e4d 6574 615a 1b62 735f 6578  ries.MetaZ.bs_ex
-000031e0: 616d 696e 6174 696f 6e5f 6469 6374 696f  amination_dictio
-000031f0: 6e61 7269 6573 750c 0000 00e6 a380 e9aa  nariesu.........
-00003200: 8ce5 ad97 e585 b84e 7236 0000 0072 1900  .......Nr6...r..
-00003210: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00003220: 0072 1b00 0000 9901 0000 7306 0000 0008  .r........s.....
-00003230: 0104 0104 0172 1b00 0000 4e72 a800 0000  .....r....Nr....
-00003240: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-00003250: 1a00 0000 72ab 0000 008e 0100 0073 1400  ....r........s..
-00003260: 0000 0801 1001 0e01 0e01 0e01 0e01 1201  ................
-00003270: 1201 1001 1002 72ab 0000 0063 0000 0000  ......r....c....
-00003280: 0000 0000 0000 0000 0000 0000 0600 0000  ................
-00003290: 4000 0000 733c 0000 0065 005a 0164 005a  @...s<...e.Z.d.Z
-000032a0: 0265 036a 0464 0164 0264 0364 048d 035a  .e.j.d.d.d.d...Z
-000032b0: 0565 036a 0464 0564 0664 0364 0364 078d  .e.j.d.d.d.d.d..
-000032c0: 045a 0647 0064 0864 0984 0064 0983 025a  .Z.G.d.d...d...Z
-000032d0: 0764 0a53 0029 0bda 1344 7275 6750 7265  .d.S.)...DrugPre
-000032e0: 7061 7261 7469 6f6e 5479 7065 7223 0000  parationTyper#..
-000032f0: 0072 2b00 0000 5472 2c00 0000 7251 0000  .r+...Tr,...rQ..
-00003300: 0075 0c00 0000 e7b1 bbe5 9e8b e590 8de7  .u..............
-00003310: a7b0 727a 0000 0063 0000 0000 0000 0000  ..rz...c........
-00003320: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
-00003330: 7318 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
-00003340: 0364 025a 0465 045a 0564 0353 0029 047a  .d.Z.e.Z.d.S.).z
-00003350: 1844 7275 6750 7265 7061 7261 7469 6f6e  .DrugPreparation
-00003360: 5479 7065 2e4d 6574 615a 1862 735f 6472  Type.MetaZ.bs_dr
-00003370: 7567 5f70 7265 7061 7261 7469 6f6e 5f74  ug_preparation_t
-00003380: 7970 6575 1200 0000 e88d afe5 9381 e588  ypeu............
-00003390: b6e5 8982 e7b1 bbe5 9e8b 4e72 3600 0000  ..........Nr6...
-000033a0: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-000033b0: 1a00 0000 721b 0000 00a3 0100 0073 0600  ....r........s..
-000033c0: 0000 0801 0401 0401 721b 0000 004e 2908  ........r....N).
-000033d0: 7215 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-000033e0: 0500 0000 7239 0000 0072 3e00 0000 da09  ....r9...r>.....
-000033f0: 7479 7065 5f6e 616d 6572 1b00 0000 7219  type_namer....r.
-00003400: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-00003410: 0000 72ac 0000 009f 0100 0073 0600 0000  ..r........s....
-00003420: 0801 1001 1202 72ac 0000 0063 0000 0000  ......r....c....
-00003430: 0000 0000 0000 0000 0000 0000 0600 0000  ................
-00003440: 4000 0000 733c 0000 0065 005a 0164 005a  @...s<...e.Z.d.Z
-00003450: 0265 036a 0464 0164 0264 0364 048d 035a  .e.j.d.d.d.d...Z
-00003460: 0565 036a 0464 0564 0664 0364 0364 078d  .e.j.d.d.d.d.d..
-00003470: 045a 0647 0064 0864 0984 0064 0983 025a  .Z.G.d.d...d...Z
-00003480: 0764 0a53 0029 0bda 0844 7275 6754 7970  .d.S.)...DrugTyp
-00003490: 6572 2b00 0000 7223 0000 0054 a903 720c  er+...r#...T..r.
-000034a0: 0000 0072 2500 0000 722d 0000 0072 2200  ...r%...r-...r".
-000034b0: 0000 7251 0000 0072 2800 0000 6300 0000  ..rQ...r(...c...
-000034c0: 0000 0000 0000 0000 0000 0000 0001 0000  ................
-000034d0: 0040 0000 0073 1800 0000 6500 5a01 6400  .@...s....e.Z.d.
-000034e0: 5a02 6401 5a03 6402 5a04 6504 5a05 6403  Z.d.Z.d.Z.e.Z.d.
-000034f0: 5300 2904 7a0d 4472 7567 5479 7065 2e4d  S.).z.DrugType.M
-00003500: 6574 615a 0c62 735f 6472 7567 5f74 7970  etaZ.bs_drug_typ
-00003510: 65f5 0c00 0000 e88d afe5 9381 e7b1 bbe5  e...............
-00003520: 9e8b 4e72 3600 0000 7219 0000 0072 1900  ..Nr6...r....r..
-00003530: 0000 7219 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-00003540: 00ad 0100 0073 0600 0000 0801 0401 0401  .....s..........
-00003550: 721b 0000 004e a908 7215 0000 0072 1600  r....N..r....r..
-00003560: 0000 7217 0000 0072 0500 0000 7239 0000  ..r....r....r9..
-00003570: 0072 9500 0000 723a 0000 0072 1b00 0000  .r....r:...r....
-00003580: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-00003590: 1a00 0000 72ae 0000 00a9 0100 0073 0600  ....r........s..
-000035a0: 0000 0801 1001 1202 72ae 0000 0063 0000  ........r....c..
-000035b0: 0000 0000 0000 0000 0000 0000 0000 0600  ................
-000035c0: 0000 4000 0000 733c 0000 0065 005a 0164  ..@...s<...e.Z.d
-000035d0: 005a 0265 036a 0464 0164 0264 0364 048d  .Z.e.j.d.d.d.d..
-000035e0: 035a 0565 036a 0464 0564 0664 0364 0364  .Z.e.j.d.d.d.d.d
-000035f0: 078d 045a 0647 0064 0864 0984 0064 0983  ...Z.G.d.d...d..
-00003600: 025a 0764 0a53 0029 0bda 0c44 7275 6743  .Z.d.S.)...DrugC
-00003610: 6174 6567 6f72 7972 2300 0000 722b 0000  ategoryr#...r+..
-00003620: 0054 722c 0000 0072 5100 0000 750c 0000  .Tr,...rQ...u...
-00003630: 00e7 b1bb e588 abe5 908d e7a7 b072 7a00  .............rz.
-00003640: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00003650: 0000 0001 0000 0040 0000 0073 1800 0000  .......@...s....
-00003660: 6500 5a01 6400 5a02 6401 5a03 6402 5a04  e.Z.d.Z.d.Z.d.Z.
-00003670: 6504 5a05 6403 5300 2904 7a11 4472 7567  e.Z.d.S.).z.Drug
-00003680: 4361 7465 676f 7279 2e4d 6574 615a 1062  Category.MetaZ.b
-00003690: 735f 6472 7567 5f63 6174 6567 6f72 7975  s_drug_categoryu
-000036a0: 0c00 0000 e88d afe5 9381 e7b1 bbe5 88ab  ................
-000036b0: 4e72 3600 0000 7219 0000 0072 1900 0000  Nr6...r....r....
-000036c0: 7219 0000 0072 1a00 0000 721b 0000 00b7  r....r....r.....
-000036d0: 0100 0073 0600 0000 0801 0401 0401 721b  ...s..........r.
-000036e0: 0000 004e 2908 7215 0000 0072 1600 0000  ...N).r....r....
-000036f0: 7217 0000 0072 0500 0000 7239 0000 0072  r....r....r9...r
-00003700: 3e00 0000 5a0d 6361 7465 676f 7279 5f6e  >...Z.category_n
-00003710: 616d 6572 1b00 0000 7219 0000 0072 1900  amer....r....r..
-00003720: 0000 7219 0000 0072 1a00 0000 72b2 0000  ..r....r....r...
-00003730: 00b3 0100 0073 0600 0000 0801 1001 1202  .....s..........
-00003740: 72b2 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00003750: 0000 0000 0000 0600 0000 4000 0000 739e  ..........@...s.
-00003760: 0100 0065 005a 0164 005a 0265 036a 0464  ...e.Z.d.Z.e.j.d
-00003770: 0164 0264 0364 048d 035a 0565 036a 0464  .d.d.d...Z.e.j.d
-00003780: 0564 0664 0364 0364 078d 045a 0665 036a  .d.d.d.d...Z.e.j
-00003790: 0464 0564 0864 0364 0364 078d 045a 0765  .d.d.d.d.d...Z.e
-000037a0: 036a 0464 0564 0964 0364 0364 078d 045a  .j.d.d.d.d.d...Z
-000037b0: 0865 036a 0464 0a64 0b64 0364 0364 0c8d  .e.j.d.d.d.d.d..
-000037c0: 045a 0965 036a 0a65 0b64 0d65 036a 0c64  .Z.e.j.e.d.e.j.d
-000037d0: 0e8d 035a 0d65 036a 0a65 0e64 0f65 036a  ...Z.e.j.e.d.e.j
-000037e0: 0c64 0e8d 035a 0f65 036a 0a65 1064 1065  .d...Z.e.j.e.d.e
-000037f0: 036a 0c64 0e8d 035a 1165 036a 0464 1164  .j.d...Z.e.j.d.d
-00003800: 0b64 0364 0364 0c8d 045a 1265 036a 0464  .d.d.d...Z.e.j.d
-00003810: 1264 0b64 0364 0364 0c8d 045a 1365 036a  .d.d.d.d...Z.e.j
-00003820: 0464 1364 0b64 0364 0364 0c8d 045a 1465  .d.d.d.d.d...Z.e
-00003830: 036a 0464 1464 0b64 0364 0364 0c8d 045a  .j.d.d.d.d.d...Z
-00003840: 1565 036a 0464 1564 0b64 0364 0364 0c8d  .e.j.d.d.d.d.d..
-00003850: 045a 1665 036a 0464 1664 0b64 0364 0364  .Z.e.j.d.d.d.d.d
-00003860: 0c8d 045a 1765 036a 0464 1764 0b64 0364  ...Z.e.j.d.d.d.d
-00003870: 0364 0c8d 045a 1865 036a 1964 1864 0364  .d...Z.e.j.d.d.d
-00003880: 198d 025a 1a65 036a 0464 1a64 0564 0364  ...Z.e.j.d.d.d.d
-00003890: 0364 0c8d 045a 1b65 036a 0464 1b64 0564  .d...Z.e.j.d.d.d
-000038a0: 0364 0364 0c8d 045a 1c65 036a 0464 1c64  .d.d...Z.e.j.d.d
-000038b0: 0564 0364 0364 0c8d 045a 1d65 036a 0464  .d.d.d...Z.e.j.d
-000038c0: 0564 1d64 0364 0364 078d 045a 1e65 036a  .d.d.d.d...Z.e.j
-000038d0: 0464 0564 1e64 0364 0364 078d 045a 1f65  .d.d.d.d.d...Z.e
-000038e0: 036a 0464 1f64 0564 0364 208d 035a 2047  .j.d.d.d.d ..Z G
-000038f0: 0064 2164 2284 0064 2283 025a 2164 2353  .d!d"..d"..Z!d#S
-00003900: 0029 24da 0d44 7275 6744 6972 6563 746f  .)$..DrugDirecto
-00003910: 7279 f50c 0000 00e8 8daf e593 81e7 bc96  ry..............
-00003920: e7a0 8172 2300 0000 5472 af00 0000 7251  ...r#...Tr....rQ
-00003930: 0000 00f5 0c00 0000 e88d afe5 9381 e590  ................
-00003940: 8de7 a7b0 727a 0000 00f5 0600 0000 e8a7  ....rz..........
-00003950: 84e6 a0bc 750c 0000 00e5 9fba e69c ace5  ....u...........
-00003960: 8d95 e4bd 8d75 1200 0000 e680 bbe9 878f  .....u..........
-00003970: e58d 95e4 bd8d e7bc 96e7 a081 7250 0000  ............rP..
-00003980: 0072 2800 0000 f50c 0000 00e5 88b6 e589  .r(.............
-00003990: 82e7 b1bb e59e 8b72 4800 0000 f506 0000  .......rH.......
-000039a0: 00e7 b1bb e588 ab72 b000 0000 750c 0000  .......r....u...
-000039b0: 00e5 8d95 e4bd 8de5 8982 e987 8f75 1300  .............u..
-000039c0: 0000 e8ae a1e9 878f 2fe9 9bb6 e594 aee5  ......../.......
-000039d0: 8d95 e4bd 8d75 1200 0000 e8ae a1e9 878f  .....u..........
-000039e0: e58d 95e4 bd8d e7bc 96e7 a081 f50c 0000  ................
-000039f0: 00e5 ba93 e5ad 98e6 95b0 e987 8f75 0c00  .............u..
-00003a00: 0000 e5ba 93e5 ad98 e58d 95e4 bd8d 750c  ..............u.
-00003a10: 0000 00e5 8cbb e4bf 9de7 b1bb e588 ab75  ...............u
-00003a20: 0c00 0000 e586 9ce5 9088 e7b1 bbe5 88ab  ................
-00003a30: 750f 0000 00e6 98af e590 a6e6 98af e59f  u...............
-00003a40: bae8 8daf 7213 0000 0075 0c00 0000 e9ab  ....r....u......
-00003a50: 98e5 8db1 e7ad 89e7 baa7 7512 0000 00e5  ..........u.....
-00003a60: 9bbd e5ae b6e8 b4af e6a0 87e7 bc96 e7a0  ................
-00003a70: 8175 1200 0000 e59b bde5 aeb6 e8b4 afe6  .u..............
-00003a80: a087 e590 8de7 a7b0 f506 0000 00e4 baa7  ................
-00003a90: e59c b0f5 0c00 0000 e794 9fe4 baa7 e58e  ................
-00003aa0: 82e5 aeb6 7518 0000 00e5 8d95 e6ac a1e7  ....u...........
-00003ab0: 94a8 e987 8fe5 8d95 e4bd 8de7 bc96 e7a0  ................
-00003ac0: 8172 8e00 0000 6300 0000 0000 0000 0000  .r....c.........
-00003ad0: 0000 0000 0000 0001 0000 0040 0000 0073  ...........@...s
-00003ae0: 1800 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
-00003af0: 6402 5a04 6504 5a05 6403 5300 2904 7a12  d.Z.e.Z.d.S.).z.
-00003b00: 4472 7567 4469 7265 6374 6f72 792e 4d65  DrugDirectory.Me
-00003b10: 7461 5a11 6273 5f64 7275 675f 6469 7265  taZ.bs_drug_dire
-00003b20: 6374 6f72 7975 0c00 0000 e88d afe5 9381  ctoryu..........
-00003b30: e79b aee5 bd95 4e72 3600 0000 7219 0000  ......Nr6...r...
-00003b40: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
-00003b50: 721b 0000 00e1 0100 0073 0600 0000 0801  r........s......
-00003b60: 0401 0401 721b 0000 004e 2922 7215 0000  ....r....N)"r...
-00003b70: 0072 1600 0000 7217 0000 0072 0500 0000  .r....r....r....
-00003b80: 7239 0000 00da 0964 7275 675f 636f 6465  r9.....drug_code
-00003b90: da09 6472 7567 5f6e 616d 65da 0973 7461  ..drug_name..sta
-00003ba0: 6e64 6172 6473 5a0a 746f 7461 6c5f 756e  ndardsZ.total_un
-00003bb0: 6974 5a0f 746f 7461 6c5f 756e 6974 5f63  itZ.total_unit_c
-00003bc0: 6f64 6572 4100 0000 72ac 0000 00da 0a44  oderA...r......D
-00003bd0: 4f5f 4e4f 5448 494e 47da 1070 7265 7061  O_NOTHING..prepa
-00003be0: 7261 7469 6f6e 5f74 7970 6572 b200 0000  ration_typer....
-00003bf0: da08 6361 7465 676f 7279 72ae 0000 00da  ..categoryr.....
-00003c00: 0964 7275 675f 7479 7065 5a09 756e 6974  .drug_typeZ.unit
-00003c10: 5f64 6f73 655a 0c6d 6561 7375 7265 5f75  _doseZ.measure_u
-00003c20: 6e69 745a 116d 6561 7375 7265 5f75 6e69  nitZ.measure_uni
-00003c30: 745f 636f 6465 5a0a 7374 6f63 6b5f 6c65  t_codeZ.stock_le
-00003c40: 6674 5a0a 7374 6f63 6b5f 756e 6974 5a03  ftZ.stock_unitZ.
-00003c50: 6d69 635a 0c72 6363 5f63 6174 6567 6f72  micZ.rcc_categor
-00003c60: 7972 1f00 0000 5a0c 6973 5f65 7373 656e  yr....Z.is_essen
-00003c70: 7469 616c 5a08 6872 5f6c 6576 656c 5a07  tialZ.hr_levelZ.
-00003c80: 6762 5f63 6f64 655a 0767 625f 6e61 6d65  gb_codeZ.gb_name
-00003c90: da0c 6f72 6967 696e 5f70 6c61 6365 da0c  ..origin_place..
-00003ca0: 6d61 6e75 6661 6374 7572 6572 5a0d 636f  manufacturerZ.co
-00003cb0: 6465 5f6d 6564 755f 6375 7272 1b00 0000  de_medu_curr....
-00003cc0: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-00003cd0: 1a00 0000 72b3 0000 00bd 0100 0073 4600  ....r........sF.
-00003ce0: 0000 0801 1001 1201 1201 1201 1201 0401  ................
-00003cf0: 0201 0201 04fd 0605 0401 0201 0201 04fd  ................
-00003d00: 0605 0401 0201 0201 04fd 0605 1201 1201  ................
-00003d10: 1201 1201 1201 1201 1201 0e01 1201 1201  ................
-00003d20: 1201 1201 1201 1002 72b3 0000 0063 0000  ........r....c..
-00003d30: 0000 0000 0000 0000 0000 0000 0000 0600  ................
-00003d40: 0000 4000 0000 733c 0000 0065 005a 0164  ..@...s<...e.Z.d
-00003d50: 005a 0265 036a 0464 0164 0264 0364 048d  .Z.e.j.d.d.d.d..
-00003d60: 035a 0565 036a 0464 0564 0664 0364 0364  .Z.e.j.d.d.d.d.d
-00003d70: 078d 045a 0647 0064 0864 0984 0064 0983  ...Z.G.d.d...d..
-00003d80: 025a 0764 0a53 0029 0bda 0c50 6861 726d  .Z.d.S.)...Pharm
-00003d90: 6163 7954 7970 6572 2b00 0000 7223 0000  acyTyper+...r#..
-00003da0: 0054 72af 0000 0072 2200 0000 7251 0000  .Tr....r"...rQ..
-00003db0: 0072 2800 0000 6300 0000 0000 0000 0000  .r(...c.........
-00003dc0: 0000 0000 0000 0001 0000 0040 0000 0073  ...........@...s
-00003dd0: 1800 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
-00003de0: 6402 5a04 6504 5a05 6403 5300 2904 7a11  d.Z.e.Z.d.S.).z.
-00003df0: 5068 6172 6d61 6379 5479 7065 2e4d 6574  PharmacyType.Met
-00003e00: 615a 1062 735f 7068 6172 6d61 6379 5f74  aZ.bs_pharmacy_t
-00003e10: 7970 65f5 0c00 0000 e88d afe6 88bf e7b1  ype.............
-00003e20: bbe5 9e8b 4e72 3600 0000 7219 0000 0072  ....Nr6...r....r
-00003e30: 1900 0000 7219 0000 0072 1a00 0000 721b  ....r....r....r.
-00003e40: 0000 00eb 0100 0073 0600 0000 0801 0401  .......s........
-00003e50: 0401 721b 0000 004e 72b1 0000 0072 1900  ..r....Nr....r..
-00003e60: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00003e70: 0072 c500 0000 e701 0000 7306 0000 0008  .r........s.....
-00003e80: 0110 0112 0272 c500 0000 6300 0000 0000  .....r....c.....
-00003e90: 0000 0000 0000 0000 0000 0006 0000 0040  ...............@
-00003ea0: 0000 0073 3c00 0000 6500 5a01 6400 5a02  ...s<...e.Z.d.Z.
-00003eb0: 6503 6a04 6401 6402 6403 6404 8d03 5a05  e.j.d.d.d.d...Z.
-00003ec0: 6503 6a04 6405 6406 6403 6403 6407 8d04  e.j.d.d.d.d.d...
-00003ed0: 5a06 4700 6408 6409 8400 6409 8302 5a07  Z.G.d.d...d...Z.
-00003ee0: 640a 5300 290b da12 5068 6172 6d61 6379  d.S.)...Pharmacy
-00003ef0: 456e 7465 7270 7269 7365 722b 0000 0072  Enterpriser+...r
-00003f00: 2300 0000 5472 af00 0000 7222 0000 0072  #...Tr....r"...r
-00003f10: 5100 0000 7228 0000 0063 0000 0000 0000  Q...r(...c......
-00003f20: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
-00003f30: 0000 7318 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-00003f40: 015a 0364 025a 0465 045a 0564 0353 0029  .Z.d.Z.e.Z.d.S.)
-00003f50: 047a 1750 6861 726d 6163 7945 6e74 6572  .z.PharmacyEnter
-00003f60: 7072 6973 652e 4d65 7461 5a16 6273 5f70  prise.MetaZ.bs_p
-00003f70: 6861 726d 6163 795f 656e 7465 7270 7269  harmacy_enterpri
-00003f80: 7365 750c 0000 00e8 8daf e4bc 81e7 aea1  seu.............
-00003f90: e790 864e 7236 0000 0072 1900 0000 7219  ...Nr6...r....r.
-00003fa0: 0000 0072 1900 0000 721a 0000 0072 1b00  ...r....r....r..
-00003fb0: 0000 f501 0000 7306 0000 0008 0104 0104  ......s.........
-00003fc0: 0172 1b00 0000 4e72 b100 0000 7219 0000  .r....Nr....r...
-00003fd0: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
-00003fe0: 72c7 0000 00f1 0100 0073 0600 0000 0801  r........s......
-00003ff0: 1001 1202 72c7 0000 0063 0000 0000 0000  ....r....c......
-00004000: 0000 0000 0000 0000 0000 0600 0000 4000  ..............@.
-00004010: 0000 7386 0000 0065 005a 0164 005a 0265  ..s....e.Z.d.Z.e
-00004020: 036a 0464 0164 0264 0364 048d 035a 0565  .j.d.d.d.d...Z.e
-00004030: 036a 0464 0564 0664 0364 0364 078d 045a  .j.d.d.d.d.d...Z
-00004040: 0665 036a 0765 0864 0865 036a 0964 098d  .e.j.e.d.e.j.d..
-00004050: 035a 0a65 036a 0b64 0a64 0364 0364 0b8d  .Z.e.j.d.d.d.d..
-00004060: 035a 0c65 036a 0765 0d64 0c65 036a 0e64  .Z.e.j.e.d.e.j.d
-00004070: 0364 0d8d 045a 0f65 036a 0765 1064 0e65  .d...Z.e.j.e.d.e
-00004080: 036a 0e64 0364 0d8d 045a 1147 0064 0f64  .j.d.d...Z.G.d.d
-00004090: 1084 0064 1083 025a 1264 1153 0029 12da  ...d...Z.d.S.)..
-000040a0: 1250 6861 726d 6163 794d 616e 6167 656d  .PharmacyManagem
-000040b0: 656e 7475 0c00 0000 e88d afe6 88bf e7bc  entu............
-000040c0: 96e7 a081 7223 0000 0054 72af 0000 0075  ....r#...Tr....u
-000040d0: 0c00 0000 e88d afe6 88bf e590 8de7 a7b0  ................
-000040e0: 7251 0000 0072 2800 0000 72c6 0000 0072  rQ...r(...r....r
-000040f0: 4800 0000 750c 0000 00e8 8daf e688 bfe5  H...u...........
-00004100: 9cb0 e59d 8072 2a00 0000 722f 0000 0072  .....r*...r/...r
-00004110: 3000 0000 750c 0000 00e6 8980 e5b1 9ee8  0...u...........
-00004120: 8daf e4bc 8163 0000 0000 0000 0000 0000  .....c..........
-00004130: 0000 0000 0000 0100 0000 4000 0000 7318  ..........@...s.
-00004140: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
-00004150: 025a 0465 045a 0564 0353 0029 047a 1750  .Z.e.Z.d.S.).z.P
-00004160: 6861 726d 6163 794d 616e 6167 656d 656e  harmacyManagemen
-00004170: 742e 4d65 7461 5a16 6273 5f70 6861 726d  t.MetaZ.bs_pharm
-00004180: 6163 795f 6d61 6e61 6765 6d65 6e74 750c  acy_managementu.
-00004190: 0000 00e8 8daf e688 bfe7 aea1 e790 864e  ...............N
-000041a0: 7236 0000 0072 1900 0000 7219 0000 0072  r6...r....r....r
-000041b0: 1900 0000 721a 0000 0072 1b00 0000 0702  ....r....r......
-000041c0: 0000 7306 0000 0008 0104 0104 0172 1b00  ..s..........r..
-000041d0: 0000 4e29 1372 1500 0000 7216 0000 0072  ..N).r....r....r
-000041e0: 1700 0000 7205 0000 0072 3900 0000 5a0d  ....r....r9...Z.
-000041f0: 7068 6172 6d61 6379 5f63 6f64 655a 0d70  pharmacy_codeZ.p
-00004200: 6861 726d 6163 795f 6e61 6d65 7241 0000  harmacy_namerA..
-00004210: 0072 c500 0000 72bf 0000 005a 0d70 6861  .r....r....Z.pha
-00004220: 726d 6163 795f 7479 7065 723c 0000 0072  rmacy_typer<...r
-00004230: 3f00 0000 7221 0000 0072 4200 0000 724a  ?...r!...rB...rJ
-00004240: 0000 0072 c700 0000 5a0a 656e 7465 7270  ...r....Z.enterp
-00004250: 7269 7365 721b 0000 0072 1900 0000 7219  riser....r....r.
-00004260: 0000 0072 1900 0000 721a 0000 0072 c800  ...r....r....r..
-00004270: 0000 fb01 0000 7316 0000 0008 0110 0112  ......s.........
-00004280: 0104 0102 0102 0104 fd06 0510 0114 0114  ................
-00004290: 0272 c800 0000 6300 0000 0000 0000 0000  .r....c.........
-000042a0: 0000 0000 0000 0006 0000 0040 0000 0073  ...........@...s
-000042b0: 4e01 0000 6500 5a01 6400 5a02 6503 6a04  N...e.Z.d.Z.e.j.
-000042c0: 6505 6401 6503 6a06 6402 6403 8d04 5a07  e.d.e.j.d.d...Z.
-000042d0: 6503 6a08 6404 6405 6402 6402 6406 8d04  e.j.d.d.d.d.d...
-000042e0: 5a09 6503 6a08 6407 6408 6402 6402 6409  Z.e.j.d.d.d.d.d.
-000042f0: 8d04 5a0a 6503 6a08 6407 640a 6402 6402  ..Z.e.j.d.d.d.d.
-00004300: 6409 8d04 5a0b 6503 6a08 6407 640b 6402  d...Z.e.j.d.d.d.
-00004310: 6402 6409 8d04 5a0c 6503 6a04 650d 640c  d.d...Z.e.j.e.d.
-00004320: 6503 6a0e 640d 8d03 5a0f 6503 6a04 6510  e.j.d...Z.e.j.e.
-00004330: 640e 6503 6a0e 640d 8d03 5a11 6503 6a04  d.e.j.d...Z.e.j.
-00004340: 6512 640f 6503 6a0e 640d 8d03 5a13 6503  e.d.e.j.d...Z.e.
-00004350: 6a08 6410 6411 6402 6402 6409 8d04 5a14  j.d.d.d.d.d...Z.
-00004360: 6503 6a08 6412 6413 6402 6402 6409 8d04  e.j.d.d.d.d.d...
-00004370: 5a15 6503 6a04 6516 6414 6503 6a06 6402  Z.e.j.e.d.e.j.d.
-00004380: 6403 8d04 5a17 6503 6a18 6415 6402 6402  d...Z.e.j.d.d.d.
-00004390: 6416 8d03 5a19 6503 6a1a 6417 6418 6402  d...Z.e.j.d.d.d.
-000043a0: 6419 8d03 5a1b 6503 6a08 6407 641a 6402  d...Z.e.j.d.d.d.
-000043b0: 6402 6409 8d04 5a1c 6503 6a1d 641b 6402  d.d...Z.e.j.d.d.
-000043c0: 641c 8d02 5a1e 6503 6a1d 641d 6402 641c  d...Z.e.j.d.d.d.
-000043d0: 8d02 5a1f 6503 6a1d 641e 6402 641c 8d02  ..Z.e.j.d.d.d...
-000043e0: 5a20 6503 6a1d 641f 6402 641c 8d02 5a21  Z e.j.d.d.d...Z!
-000043f0: 4700 6420 6421 8400 6421 8302 5a22 6422  G.d d!..d!..Z"d"
-00004400: 5300 2923 da0c 5068 6172 6d61 6379 4472  S.)#..PharmacyDr
-00004410: 7567 750c 0000 00e6 8980 e5b1 9ee8 8daf  ugu.............
-00004420: e688 bf54 7230 0000 0072 b400 0000 7223  ...Tr0...r....r#
-00004430: 0000 0072 2800 0000 7251 0000 0072 b500  ...r(...rQ...r..
-00004440: 0000 727a 0000 0072 b600 0000 7506 0000  ..rz...r....u...
-00004450: 00e5 8d95 e4bd 8d72 b700 0000 7248 0000  .......r....rH..
-00004460: 0072 b000 0000 72b8 0000 0072 8100 0000  .r....r....r....
-00004470: 72ba 0000 00e9 c800 0000 72bb 0000 0072  r.........r....r
-00004480: 2f00 0000 750c 0000 00e6 9c89 e695 88e6  /...u...........
-00004490: 97a5 e69c 9f72 1000 0000 72b9 0000 0072  .....r....r....r
-000044a0: 0100 0000 7279 0000 0075 0c00 0000 e8ae  ....ry...u......
-000044b0: a1e9 878f e58d 95e4 bd8d 750c 0000 00e6  ..........u.....
-000044c0: 8890 e69c ace5 8d95 e4bb b772 8f00 0000  ...........r....
-000044d0: 750c 0000 00e6 8890 e69c ace9 8791 e9a2  u...............
-000044e0: 9d75 0c00 0000 e99b b6e5 94ae e58d 95e4  .u..............
-000044f0: bbb7 750c 0000 00e9 9bb6 e594 aee9 8791  ..u.............
-00004500: e9a2 9d63 0000 0000 0000 0000 0000 0000  ...c............
-00004510: 0000 0000 0100 0000 4000 0000 7318 0000  ........@...s...
-00004520: 0065 005a 0164 005a 0264 015a 0364 025a  .e.Z.d.Z.d.Z.d.Z
-00004530: 0465 045a 0564 0353 0029 047a 1150 6861  .e.Z.d.S.).z.Pha
-00004540: 726d 6163 7944 7275 672e 4d65 7461 5a10  rmacyDrug.MetaZ.
-00004550: 6273 5f70 6861 726d 6163 795f 6472 7567  bs_pharmacy_drug
-00004560: 750d 0000 00e8 8daf e688 bf2d e88d afe5  u..........-....
-00004570: 9381 4e72 3600 0000 7219 0000 0072 1900  ..Nr6...r....r..
-00004580: 0000 7219 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-00004590: 002d 0200 0073 0600 0000 0801 0401 0401  .-...s..........
-000045a0: 721b 0000 004e 2923 7215 0000 0072 1600  r....N)#r....r..
-000045b0: 0000 7217 0000 0072 0500 0000 7241 0000  ..r....r....rA..
-000045c0: 0072 c800 0000 7242 0000 005a 0870 6861  .r....rB...Z.pha
-000045d0: 726d 6163 7972 3900 0000 72bc 0000 0072  rmacyr9...r....r
-000045e0: bd00 0000 72be 0000 00da 0575 6e69 7473  ....r......units
-000045f0: 72ac 0000 0072 bf00 0000 72c0 0000 0072  r....r....r....r
-00004600: ae00 0000 72c2 0000 0072 b200 0000 72c1  ....r....r....r.
-00004610: 0000 0072 c300 0000 72c4 0000 0072 2100  ...r....r....r!.
-00004620: 0000 724a 0000 0072 6000 0000 5a0a 7661  ..rJ...r`...Z.va
-00004630: 6c69 645f 6461 7465 7270 0000 005a 1269  lid_daterp...Z.i
-00004640: 6e76 656e 746f 7279 5f71 7561 6e74 6974  nventory_quantit
-00004650: 795a 106d 6561 7375 7265 6d65 6e74 5f75  yZ.measurement_u
-00004660: 6e69 7472 4000 0000 5a0f 636f 7374 5f75  nitr@...Z.cost_u
-00004670: 6e69 745f 7072 6963 655a 0b63 6f73 745f  nit_priceZ.cost_
-00004680: 616d 6f75 6e74 5a11 7265 7461 696c 5f75  amountZ.retail_u
-00004690: 6e69 745f 7072 6963 655a 0d72 6574 6169  nit_priceZ.retai
-000046a0: 6c5f 616d 6f75 6e74 721b 0000 0072 1900  l_amountr....r..
-000046b0: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-000046c0: 0072 c900 0000 0d02 0000 733e 0000 0008  .r........s>....
-000046d0: 0114 0112 0112 0112 0112 0104 0102 0102  ................
-000046e0: 0104 fd06 0504 0102 0102 0104 fd06 0504  ................
-000046f0: 0102 0102 0104 fd06 0512 0112 0114 0110  ................
-00004700: 0110 0112 010e 010e 010e 010e 0272 c900  .............r..
-00004710: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00004720: 0000 0006 0000 0040 0000 0073 b600 0000  .......@...s....
-00004730: 6500 5a01 6400 5a02 6503 6a04 6401 6402  e.Z.d.Z.e.j.d.d.
-00004740: 6403 8d02 5a05 6503 6a04 6401 6404 6403  d...Z.e.j.d.d.d.
-00004750: 8d02 5a06 6503 6a04 6401 6405 6406 6406  ..Z.e.j.d.d.d.d.
-00004760: 6407 8d04 5a07 6503 6a04 6401 6408 6403  d...Z.e.j.d.d.d.
-00004770: 8d02 5a08 6503 6a04 6401 6409 6403 8d02  ..Z.e.j.d.d.d...
-00004780: 5a09 6503 6a04 640a 640b 6403 8d02 5a0a  Z.e.j.d.d.d...Z.
-00004790: 6503 6a04 640a 640c 6403 8d02 5a0b 6503  e.j.d.d.d...Z.e.
-000047a0: 6a0c 640d 6406 6406 640e 8d03 5a0d 6503  j.d.d.d.d...Z.e.
-000047b0: 6a0c 640f 6406 6406 6410 8d03 5a0e 6503  j.d.d.d.d...Z.e.
-000047c0: 6a0f 6411 6406 6412 8d02 5a10 4700 6413  j.d.d.d...Z.G.d.
-000047d0: 6414 8400 6414 8302 5a11 6415 6416 8400  d...d...Z.d.d...
-000047e0: 5a12 6417 5300 2918 da07 4170 6949 6e66  Z.d.S.)...ApiInf
-000047f0: 6f72 5a00 0000 72a4 0000 0072 7700 0000  orZ...r....rw...
-00004800: 750c 0000 00e8 afb7 e6b1 82e7 bc96 e7a0  u...............
-00004810: 8175 0c00 0000 e8af b7e6 b182 e590 8de7  .u..............
-00004820: a7b0 5472 7a00 0000 750c 0000 00e8 afb7  ..Trz...u.......
-00004830: e6b1 82e6 96b9 e5bc 8f75 1200 0000 e8af  .........u......
-00004840: b7e6 b182 e695 b0e6 8dae e7b1 bbe5 9e8b  ................
-00004850: 72ca 0000 0075 1100 0000 6970 e59c b0e5  r....u....ip....
-00004860: 9d80 e688 96e5 9f9f e590 8d75 0c00 0000  ...........u....
-00004870: e8af b7e6 b182 e8b7 afe7 94b1 720a 0000  ............r...
-00004880: 0072 0b00 0000 720f 0000 0072 1000 0000  .r....r....r....
-00004890: 7212 0000 0072 1300 0000 6300 0000 0000  r....r....c.....
-000048a0: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
-000048b0: 0000 0073 1c00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-000048c0: 6401 5a03 6402 5a04 6504 5a05 6403 5a06  d.Z.d.Z.e.Z.d.Z.
-000048d0: 6404 5300 2905 7a0c 4170 6949 6e66 6f2e  d.S.).z.ApiInfo.
-000048e0: 4d65 7461 5a0b 6273 5f61 7069 5f69 6e66  MetaZ.bs_api_inf
-000048f0: 6f75 0c00 0000 e68e a5e5 8fa3 e4bf a1e6  ou..............
-00004900: 81af 2901 a902 da08 6f72 675f 636f 6465  ..).....org_code
-00004910: da08 7265 715f 636f 6465 4e72 4b00 0000  ..req_codeNrK...
-00004920: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-00004930: 1a00 0000 721b 0000 003f 0200 0073 0800  ....r....?...s..
-00004940: 0000 0801 0401 0401 0401 721b 0000 0063  ..........r....c
-00004950: 0300 0000 0000 0000 0000 0000 0700 0000  ................
-00004960: 0500 0000 4300 0000 73ba 0000 0074 006a  ....C...s....t.j
-00004970: 016a 027c 0164 0119 007c 0264 028d 02a0  .j.|.d...|.d....
-00004980: 03a1 007d 037c 0372 a87c 036a 047c 036a  ...}.|.r.|.j.|.j
-00004990: 0517 007d 047c 036a 0664 036b 0272 4274  ...}.|.j.d.k.rBt
-000049a0: 076a 087c 047c 0164 048d 027d 056e 587c  .j.|.|.d...}.nX|
-000049b0: 036a 0664 056b 0272 5c74 076a 097c 047c  .j.d.k.r\t.j.|.|
-000049c0: 0164 068d 027d 056e 3e7c 036a 0664 076b  .d...}.n>|.j.d.k
-000049d0: 0272 7674 076a 0a7c 047c 0164 088d 027d  .rvt.j.|.|.d...}
-000049e0: 056e 247c 036a 0664 096b 0272 8e74 076a  .n$|.j.d.k.r.t.j
-000049f0: 0b7c 0464 0a8d 017d 056e 0c74 076a 0c7c  .|.d...}.n.t.j.|
-00004a00: 0464 0a8d 017d 0574 0da0 0e7c 056a 0fa1  .d...}.t...|.j..
-00004a10: 017d 066e 0e64 0b64 0c64 0d69 0064 0e9c  .}.n.d.d.d.i.d..
-00004a20: 047d 067c 0653 0029 0f4e 72a9 0000 0072  .}.|.S.).Nr....r
-00004a30: cd00 0000 da04 504f 5354 2902 728d 0000  ......POST).r...
-00004a40: 00da 046a 736f 6eda 0347 4554 2902 728d  ...json..GET).r.
-00004a50: 0000 00da 0670 6172 616d 73da 0350 5554  .....params..PUT
-00004a60: 2902 728d 0000 00da 0464 6174 61da 0644  ).r......data..D
-00004a70: 454c 4554 4529 0172 8d00 0000 4669 d107  ELETE).r....Fi..
-00004a80: 0000 751e 0000 00e4 b88d e5ad 98e5 9ca8  ..u.............
-00004a90: e5af b9e6 8ea5 e58c bbe9 99a2 e4bf a1e6  ................
-00004aa0: 81af efbc 8129 04da 0773 7563 6365 7373  .....)...success
-00004ab0: 7295 0000 00da 076d 6573 7361 6765 72d5  r......messager.
-00004ac0: 0000 0029 1072 cc00 0000 da07 6f62 6a65  ...).r......obje
-00004ad0: 6374 73da 0666 696c 7465 7272 6800 0000  cts..filterrh...
-00004ae0: da09 6970 5f64 6f6d 6169 6e72 9100 0000  ..ip_domainr....
-00004af0: da0a 7265 715f 6d65 7468 6f64 da08 7265  ..req_method..re
-00004b00: 7175 6573 7473 da04 706f 7374 da03 6765  quests..post..ge
-00004b10: 74da 0370 7574 da06 6465 6c65 7465 da05  t..put..delete..
-00004b20: 7061 7463 6872 d100 0000 da05 6c6f 6164  patchr......load
-00004b30: 73da 0474 6578 7429 0772 2e00 0000 5a07  s..text).r....Z.
-00004b40: 696e 5f64 6174 6172 cf00 0000 5a0c 6170  in_datar....Z.ap
-00004b50: 695f 696e 666f 5f6f 626a 5a07 636d 735f  i_info_objZ.cms_
-00004b60: 7572 6cda 0372 6573 5a08 7265 735f 6a73  url..resZ.res_js
-00004b70: 6f6e 7219 0000 0072 1900 0000 721a 0000  onr....r....r...
-00004b80: 00da 0977 7269 7465 6261 636b 4702 0000  ...writebackG...
-00004b90: 731e 0000 0000 0118 0104 010c 010a 0110  s...............
-00004ba0: 010a 0110 010a 0110 010a 010e 020c 010e  ................
-00004bb0: 020e 017a 1141 7069 496e 666f 2e77 7269  ...z.ApiInfo.wri
-00004bc0: 7465 6261 636b 4e29 1372 1500 0000 7216  tebackN).r....r.
-00004bd0: 0000 0072 1700 0000 7205 0000 0072 3900  ...r....r....r9.
-00004be0: 0000 72ce 0000 0072 cf00 0000 5a08 7265  ..r....r....Z.re
-00004bf0: 715f 6e61 6d65 72dc 0000 0072 9000 0000  q_namer....r....
-00004c00: 72db 0000 0072 9100 0000 721c 0000 0072  r....r....r....r
-00004c10: 1d00 0000 721e 0000 0072 1f00 0000 7220  ....r....r....r 
-00004c20: 0000 0072 1b00 0000 72e6 0000 0072 1900  ...r....r....r..
-00004c30: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00004c40: 0072 cc00 0000 3302 0000 7318 0000 0008  .r....3...s.....
-00004c50: 010e 010e 0112 010e 010e 010e 010e 0110  ................
-00004c60: 0110 010e 020e 0872 cc00 0000 2926 72d1  .......r....)&r.
-00004c70: 0000 00da 026f 7372 dd00 0000 da1a 646a  .....osr......dj
-00004c80: 616e 676f 2e63 6f6e 7472 6962 2e61 7574  ango.contrib.aut
-00004c90: 682e 6d6f 6465 6c73 7202 0000 0072 0300  h.modelsr....r..
-00004ca0: 0000 da22 646a 616e 676f 2e63 6f6e 7472  ..."django.contr
-00004cb0: 6962 2e63 6f6e 7465 6e74 7479 7065 732e  ib.contenttypes.
-00004cc0: 6d6f 6465 6c73 7204 0000 00da 0964 6a61  modelsr......dja
-00004cd0: 6e67 6f2e 6462 7205 0000 00da 0b64 6a61  ngo.dbr......dja
-00004ce0: 6e67 6f2e 636f 6e66 7206 0000 0072 5d00  ngo.confr....r].
-00004cf0: 0000 da05 4d6f 6465 6c72 0900 0000 7221  ....Modelr....r!
-00004d00: 0000 0072 4600 0000 724d 0000 0072 4f00  ...rF...rM...rO.
-00004d10: 0000 7263 0000 0072 7400 0000 727f 0000  ..rc...rt...r...
-00004d20: 0072 8b00 0000 7293 0000 0072 9600 0000  .r....r....r....
-00004d30: 7299 0000 0072 a000 0000 72aa 0000 0072  r....r....r....r
-00004d40: ab00 0000 72ac 0000 0072 ae00 0000 72b2  ....r....r....r.
-00004d50: 0000 0072 b300 0000 72c5 0000 0072 c700  ...r....r....r..
-00004d60: 0000 72c8 0000 0072 c900 0000 72cc 0000  ..r....r....r...
-00004d70: 0072 1900 0000 7219 0000 0072 1900 0000  .r....r....r....
-00004d80: 721a 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00004d90: 0000 0073 3e00 0000 0801 0802 0801 1001  ...s>...........
-00004da0: 0c01 0c01 0c02 0406 1209 101e 101c 1014  ................
-00004db0: 1028 104a 121e 121b 1223 100d 1019 1011  .(.J.....#......
-00004dc0: 1011 1011 1011 100a 100a 100a 102a 100a  .............*..
-00004dd0: 100a 1012 1026                           .....&
+00000070: 6405 6c02 6d0a 5a0a 0100 6400 6406 6c0b  d.l.m.Z...d.d.l.
+00000080: 6d0c 5a0c 0100 6407 5a0d 4700 6408 6409  m.Z...d.Z.G.d.d.
+00000090: 8400 6409 650a 6a0e 8303 5a0f 4700 640a  ..d.e.j...Z.G.d.
+000000a0: 640b 8400 640b 650f 8303 5a10 4700 640c  d...d.e...Z.G.d.
+000000b0: 640d 8400 640d 650f 8303 5a11 4700 640e  d...d.e...Z.G.d.
+000000c0: 640f 8400 640f 650f 8303 5a12 4700 6410  d...d.e...Z.G.d.
+000000d0: 6411 8400 6411 650f 8303 5a13 4700 6412  d...d.e...Z.G.d.
+000000e0: 6413 8400 6413 6506 8303 5a14 4700 6414  d...d.e...Z.G.d.
+000000f0: 6415 8400 6415 650a 6a0e 8303 5a15 4700  d...d.e.j...Z.G.
+00000100: 6416 6417 8400 6417 650a 6a0e 8303 5a16  d.d...d.e.j...Z.
+00000110: 4700 6418 6419 8400 6419 650a 6a0e 8303  G.d.d...d.e.j...
+00000120: 5a17 4700 641a 641b 8400 641b 650f 8303  Z.G.d.d...d.e...
+00000130: 5a18 4700 641c 641d 8400 641d 650f 8303  Z.G.d.d...d.e...
+00000140: 5a19 4700 641e 641f 8400 641f 650f 8303  Z.G.d.d...d.e...
+00000150: 5a1a 4700 6420 6421 8400 6421 650f 8303  Z.G.d d!..d!e...
+00000160: 5a1b 4700 6422 6423 8400 6423 650f 8303  Z.G.d"d#..d#e...
+00000170: 5a1c 4700 6424 6425 8400 6425 650f 8303  Z.G.d$d%..d%e...
+00000180: 5a1d 4700 6426 6427 8400 6427 650f 8303  Z.G.d&d'..d'e...
+00000190: 5a1e 4700 6428 6429 8400 6429 650f 8303  Z.G.d(d)..d)e...
+000001a0: 5a1f 4700 642a 642b 8400 642b 650f 8303  Z.G.d*d+..d+e...
+000001b0: 5a20 4700 642c 642d 8400 642d 650f 8303  Z G.d,d-..d-e...
+000001c0: 5a21 4700 642e 642f 8400 642f 650f 8303  Z!G.d.d/..d/e...
+000001d0: 5a22 4700 6430 6431 8400 6431 650f 8303  Z"G.d0d1..d1e...
+000001e0: 5a23 4700 6432 6433 8400 6433 650f 8303  Z#G.d2d3..d3e...
+000001f0: 5a24 4700 6434 6435 8400 6435 650f 8303  Z$G.d4d5..d5e...
+00000200: 5a25 4700 6436 6437 8400 6437 650a 6a0e  Z%G.d6d7..d7e.j.
+00000210: 8303 5a26 6401 5300 2938 e900 0000 004e  ..Z&d.S.)8.....N
+00000220: 2901 da0b 7472 616e 7361 6374 696f 6e29  )...transaction)
+00000230: 02da 0c41 6273 7472 6163 7455 7365 72da  ...AbstractUser.
+00000240: 0547 726f 7570 2901 da0b 436f 6e74 656e  .Group)...Conten
+00000250: 7454 7970 6529 01da 066d 6f64 656c 7329  tType)...models)
+00000260: 01da 0873 6574 7469 6e67 7329 0229 02da  ...settings).)..
+00000270: 0131 7503 0000 00e7 94b7 2902 da01 3075  .1u.......)...0u
+00000280: 0300 0000 e5a5 b363 0000 0000 0000 0000  .......c........
+00000290: 0000 0000 0000 0000 0500 0000 4000 0000  ............@...
+000002a0: 7348 0000 0065 005a 0164 005a 0265 036a  sH...e.Z.d.Z.e.j
+000002b0: 0464 0164 0264 0264 038d 035a 0565 036a  .d.d.d.d...Z.e.j
+000002c0: 0464 0464 0264 0264 058d 035a 0665 036a  .d.d.d.d...Z.e.j
+000002d0: 0764 0664 0264 078d 025a 0847 0064 0864  .d.d.d...Z.G.d.d
+000002e0: 0984 0064 0983 025a 0964 0a53 0029 0bda  ...d...Z.d.S.)..
+000002f0: 104d 6564 6963 616c 4261 7365 4d6f 6465  .MedicalBaseMode
+00000300: 6cf5 0c00 0000 e588 9be5 bbba e697 b6e9  l...............
+00000310: 97b4 54a9 03da 0c76 6572 626f 7365 5f6e  ..T....verbose_n
+00000320: 616d 65da 0c61 7574 6f5f 6e6f 775f 6164  ame..auto_now_ad
+00000330: 64da 046e 756c 6cf5 0c00 0000 e69b b4e6  d..null.........
+00000340: 96b0 e697 b6e9 97b4 a903 720d 0000 00da  ..........r.....
+00000350: 0861 7574 6f5f 6e6f 7772 0f00 0000 f50c  .auto_nowr......
+00000360: 0000 00e6 98af e590 a6e5 90af e794 a8a9  ................
+00000370: 0272 0d00 0000 da07 6465 6661 756c 7463  .r......defaultc
+00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000390: 0100 0000 4000 0000 7310 0000 0065 005a  ....@...s....e.Z
+000003a0: 0164 005a 0264 015a 0364 0253 0029 037a  .d.Z.d.Z.d.S.).z
+000003b0: 154d 6564 6963 616c 4261 7365 4d6f 6465  .MedicalBaseMode
+000003c0: 6c2e 4d65 7461 544e 2904 da08 5f5f 6e61  l.MetaTN)...__na
+000003d0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+000003e0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da08  ..__qualname__..
+000003f0: 6162 7374 7261 6374 a900 721a 0000 0072  abstract..r....r
+00000400: 1a00 0000 fa37 2f68 6f6d 652f 6c79 682f  .....7/home/lyh/
+00000410: 776f 726b 2f42 6173 6546 756e 6374 696f  work/BaseFunctio
+00000420: 6e4d 6f64 756c 652f 6261 7365 5f73 7973  nModule/base_sys
+00000430: 7465 6d2f 6d6f 6465 6c73 2e70 79da 044d  tem/models.py..M
+00000440: 6574 6116 0000 0073 0200 0000 0801 721c  eta....s......r.
+00000450: 0000 004e 290a 7216 0000 0072 1700 0000  ...N).r....r....
+00000460: 7218 0000 0072 0600 0000 da0d 4461 7465  r....r......Date
+00000470: 5469 6d65 4669 656c 64da 0c63 7265 6174  TimeField..creat
+00000480: 6564 5f74 696d 65da 0c75 7064 6174 6564  ed_time..updated
+00000490: 5f74 696d 65da 0c42 6f6f 6c65 616e 4669  _time..BooleanFi
+000004a0: 656c 64da 0969 735f 6163 7469 7665 721c  eld..is_activer.
+000004b0: 0000 0072 1a00 0000 721a 0000 0072 1a00  ...r....r....r..
+000004c0: 0000 721b 0000 0072 0a00 0000 1100 0000  ..r....r........
+000004d0: 7308 0000 0008 0110 0110 010e 0272 0a00  s............r..
+000004e0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000004f0: 0000 0006 0000 0040 0000 0073 d800 0000  .......@...s....
+00000500: 6500 5a01 6400 5a02 6503 6a04 6401 6402  e.Z.d.Z.e.j.d.d.
+00000510: 6403 8d02 5a05 6503 6a04 6404 6405 6406  d...Z.e.j.d.d.d.
+00000520: 6406 6407 8d04 5a06 6503 6a07 6408 6406  d.d...Z.e.j.d.d.
+00000530: 6406 6409 8d03 5a08 6503 6a04 6402 640a  d.d...Z.e.j.d.d.
+00000540: 6406 640b 8d03 5a09 6503 6a07 640c 640d  d.d...Z.e.j.d.d.
+00000550: 8d01 5a0a 6503 6a0b 640e 640d 8d01 5a0c  ..Z.e.j.d.d...Z.
+00000560: 6503 6a0b 640f 640d 8d01 5a0d 6503 6a0e  e.j.d.d...Z.e.j.
+00000570: 6410 6411 6503 6a0f 6406 6412 8d04 5a10  d.d.e.j.d.d...Z.
+00000580: 6503 6a04 6413 6405 6414 6406 6415 8d04  e.j.d.d.d.d.d...
+00000590: 5a11 6503 6a04 6416 6405 6417 6418 8d03  Z.e.j.d.d.d.d...
+000005a0: 5a12 6503 6a04 6419 6405 6406 6406 6407  Z.e.j.d.d.d.d.d.
+000005b0: 8d04 5a13 6503 6a04 641a 6405 6406 6406  ..Z.e.j.d.d.d.d.
+000005c0: 6407 8d04 5a14 4700 641b 641c 8400 641c  d...Z.G.d.d...d.
+000005d0: 8302 5a15 641d 5300 291e da08 486f 7370  ..Z.d.S.)...Hosp
+000005e0: 6974 616c f506 0000 00e5 908d e7a7 b0e9  ital............
+000005f0: ff00 0000 a902 720d 0000 00da 0a6d 6178  ......r......max
+00000600: 5f6c 656e 6774 68f5 0c00 0000 e881 94e7  _length.........
+00000610: b3bb e696 b9e5 bc8f e964 0000 0054 a904  .........d...T..
+00000620: 720d 0000 0072 2600 0000 720f 0000 00da  r....r&...r.....
+00000630: 0562 6c61 6e6b 750c 0000 00e5 8cbb e999  .blanku.........
+00000640: a2e7 ae80 e4bb 8ba9 0372 0d00 0000 720f  .........r....r.
+00000650: 0000 0072 2a00 0000 f506 0000 00e7 bc96  ...r*...........
+00000660: e7a0 81a9 0372 2600 0000 720d 0000 00da  .....r&...r.....
+00000670: 0675 6e69 7175 6575 0c00 0000 e58c bbe9  .uniqueu........
+00000680: 99a2 e59c b0e5 9d80 2901 720d 0000 0075  ........).r....u
+00000690: 0600 0000 e7bb 8fe5 baa6 7506 0000 00e7  ..........u.....
+000006a0: bbb4 e5ba a6da 0473 656c 66f5 0c00 0000  .......self.....
+000006b0: e689 80e5 b19e e58c bbe9 99a2 a903 720d  ..............r.
+000006c0: 0000 00da 096f 6e5f 6465 6c65 7465 720f  .....on_deleter.
+000006d0: 0000 0075 0c00 0000 e58c bbe9 99a2 e59b  ...u............
+000006e0: bee7 8987 5a0f 686f 7370 6974 616c 5f69  ....Z.hospital_i
+000006f0: 6d61 6765 7329 0472 0d00 0000 7226 0000  mages).r....r&..
+00000700: 0072 1500 0000 722a 0000 00da 046c 6f67  .r....r*.....log
+00000710: 6f5a 0d68 6f73 7069 7461 6c5f 6c6f 676f  oZ.hospital_logo
+00000720: a903 720d 0000 0072 2600 0000 7215 0000  ..r....r&...r...
+00000730: 00f5 0900 0000 e588 9be5 bbba e4ba baf5  ................
+00000740: 0900 0000 e69b b4e6 96b0 e4ba ba63 0000  .............c..
+00000750: 0000 0000 0000 0000 0000 0000 0000 0100  ................
+00000760: 0000 4000 0000 7318 0000 0065 005a 0164  ..@...s....e.Z.d
+00000770: 005a 0264 015a 0364 025a 0465 045a 0564  .Z.d.Z.d.Z.e.Z.d
+00000780: 0353 0029 047a 0d48 6f73 7069 7461 6c2e  .S.).z.Hospital.
+00000790: 4d65 7461 5a0b 6273 5f68 6f73 7069 7461  MetaZ.bs_hospita
+000007a0: 6c75 0600 0000 e58c bbe9 99a2 4ea9 0672  lu..........N..r
+000007b0: 1600 0000 7217 0000 0072 1800 0000 da08  ....r....r......
+000007c0: 6462 5f74 6162 6c65 720d 0000 00da 1376  db_tabler......v
+000007d0: 6572 626f 7365 5f6e 616d 655f 706c 7572  erbose_name_plur
+000007e0: 616c 721a 0000 0072 1a00 0000 721a 0000  alr....r....r...
+000007f0: 0072 1b00 0000 721c 0000 002f 0000 0073  .r....r..../...s
+00000800: 0600 0000 0801 0401 0401 721c 0000 004e  ..........r....N
+00000810: 2916 7216 0000 0072 1700 0000 7218 0000  ).r....r....r...
+00000820: 0072 0600 0000 da09 4368 6172 4669 656c  .r......CharFiel
+00000830: 64da 046e 616d 65da 0570 686f 6e65 da09  d..name..phone..
+00000840: 5465 7874 4669 656c 64da 0969 6e74 726f  TextField..intro
+00000850: 6475 6365 da07 636f 6465 6e75 6dda 0761  duce..codenum..a
+00000860: 6464 7265 7373 da0a 466c 6f61 7446 6965  ddress..FloatFie
+00000870: 6c64 5a09 6c6f 6e67 6974 7564 655a 086c  ldZ.longitudeZ.l
+00000880: 6174 6974 7564 65da 0a46 6f72 6569 676e  atitude..Foreign
+00000890: 4b65 79da 0743 4153 4341 4445 da06 7061  Key..CASCADE..pa
+000008a0: 7265 6e74 5a0a 686f 735f 696d 6167 6573  rentZ.hos_images
+000008b0: 7233 0000 00da 0a63 7265 6174 6564 5f62  r3.....created_b
+000008c0: 79da 0a75 7064 6174 6564 5f62 7972 1c00  y..updated_byr..
+000008d0: 0000 721a 0000 0072 1a00 0000 721a 0000  ..r....r....r...
+000008e0: 0072 1b00 0000 7222 0000 001a 0000 0073  .r....r".......s
+000008f0: 2400 0000 0801 0e01 1201 1001 1001 0c01  $...............
+00000900: 0c01 0c01 0401 0201 0201 0401 02fc 0607  ................
+00000910: 1202 1001 1201 1202 7222 0000 0063 0000  ........r"...c..
+00000920: 0000 0000 0000 0000 0000 0000 0000 0600  ................
+00000930: 0000 4000 0000 73a2 0000 0065 005a 0164  ..@...s....e.Z.d
+00000940: 005a 0265 036a 0464 0164 0264 038d 025a  .Z.e.j.d.d.d...Z
+00000950: 0565 036a 0464 0464 0264 0564 0564 068d  .e.j.d.d.d.d.d..
+00000960: 045a 0665 036a 0464 0764 0264 0564 0564  .Z.e.j.d.d.d.d.d
+00000970: 068d 045a 0765 036a 0464 0864 0264 038d  ...Z.e.j.d.d.d..
+00000980: 025a 0865 036a 0464 0964 0a64 0564 0564  .Z.e.j.d.d.d.d.d
+00000990: 068d 045a 0965 036a 0a64 0b64 0564 0564  ...Z.e.j.d.d.d.d
+000009a0: 0c8d 035a 0b65 036a 0c65 0d64 0d65 036a  ...Z.e.j.e.d.e.j
+000009b0: 0e64 0e8d 035a 0f65 036a 0c64 0f64 1065  .d...Z.e.j.d.d.e
+000009c0: 036a 0e64 0564 118d 045a 1047 0064 1264  .j.d.d...Z.G.d.d
+000009d0: 1384 0064 1383 025a 1164 1453 0029 15da  ...d...Z.d.S.)..
+000009e0: 064f 6666 6963 6572 2300 0000 7224 0000  .Officer#...r$..
+000009f0: 0072 2500 0000 750c 0000 00e7 a791 e5ae  .r%...u.........
+00000a00: a4e4 bd8d e7bd ae54 7229 0000 0072 2700  .......Tr)...r'.
+00000a10: 0000 f50c 0000 00e7 a791 e5ae a4e7 bc96  ................
+00000a20: e7a0 8175 0600 0000 e7b1 bbe5 9e8b 7228  ...u..........r(
+00000a30: 0000 0075 0c00 0000 e7a7 91e5 aea4 e7ae  ...u............
+00000a40: 80e4 bb8b 722b 0000 0072 3000 0000 a902  ....r+...r0.....
+00000a50: 720d 0000 0072 3200 0000 722f 0000 0075  r....r2...r/...u
+00000a60: 0c00 0000 e4b8 8ae7 baa7 e7a7 91e5 aea4  ................
+00000a70: 7231 0000 0063 0000 0000 0000 0000 0000  r1...c..........
+00000a80: 0000 0000 0000 0100 0000 4000 0000 731c  ..........@...s.
+00000a90: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
+00000aa0: 025a 0465 045a 0564 035a 0664 0453 0029  .Z.e.Z.d.Z.d.S.)
+00000ab0: 057a 0b4f 6666 6963 652e 4d65 7461 5a09  .z.Office.MetaZ.
+00000ac0: 6273 5f6f 6666 6963 6575 0600 0000 e7a7  bs_officeu......
+00000ad0: 91e5 aea4 a901 2902 723f 0000 00da 0868  ......).r?.....h
+00000ae0: 6f73 7069 7461 6c4e a907 7216 0000 0072  ospitalN..r....r
+00000af0: 1700 0000 7218 0000 0072 3800 0000 720d  ....r....r8...r.
+00000b00: 0000 0072 3900 0000 da0f 756e 6971 7565  ...r9.....unique
+00000b10: 5f74 6f67 6574 6865 7272 1a00 0000 721a  _togetherr....r.
+00000b20: 0000 0072 1a00 0000 721b 0000 0072 1c00  ...r....r....r..
+00000b30: 0000 4b00 0000 7308 0000 0008 0104 0104  ..K...s.........
+00000b40: 0104 0172 1c00 0000 4e29 1272 1600 0000  ...r....N).r....
+00000b50: 7217 0000 0072 1800 0000 7206 0000 0072  r....r....r....r
+00000b60: 3a00 0000 723b 0000 0072 4000 0000 723c  :...r;...r@...r<
+00000b70: 0000 0072 3f00 0000 5a0b 6f66 6669 6365  ...r?...Z.office
+00000b80: 5f74 7970 6572 3d00 0000 723e 0000 0072  _typer=...r>...r
+00000b90: 4200 0000 7222 0000 0072 4300 0000 724b  B...r"...rC...rK
+00000ba0: 0000 0072 4400 0000 721c 0000 0072 1a00  ...rD...r....r..
+00000bb0: 0000 721a 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00000bc0: 0072 4700 0000 3800 0000 7324 0000 0008  .rG...8...s$....
+00000bd0: 010e 0112 0112 010e 0112 0110 0104 0102  ................
+00000be0: 0102 0104 fd06 0504 0102 0102 0104 0102  ................
+00000bf0: fc06 0772 4700 0000 6300 0000 0000 0000  ...rG...c.......
+00000c00: 0000 0000 0000 0000 0006 0000 0040 0000  .............@..
+00000c10: 0073 6c00 0000 6500 5a01 6400 5a02 6503  .sl...e.Z.d.Z.e.
+00000c20: 6a04 6401 6402 6403 8d02 5a05 6503 6a04  j.d.d.d...Z.e.j.
+00000c30: 6404 6402 6403 8d02 5a06 6503 6a07 6508  d.d.d...Z.e.j.e.
+00000c40: 6405 6503 6a09 6406 8d03 5a0a 6503 6a04  d.e.j.d...Z.e.j.
+00000c50: 6407 6408 6409 6409 640a 8d04 5a0b 6503  d.d.d.d.d...Z.e.
+00000c60: 6a04 640b 6408 6409 6409 640a 8d04 5a0c  j.d.d.d.d.d...Z.
+00000c70: 4700 640c 640d 8400 640d 8302 5a0d 640e  G.d.d...d...Z.d.
+00000c80: 5300 290f da0d 506f 7369 7469 6f6e 5469  S.)...PositionTi
+00000c90: 746c 6572 2300 0000 7224 0000 0072 2500  tler#...r$...r%.
+00000ca0: 0000 750c 0000 00e8 818c e7a7 b0e7 bc96  ..u.............
+00000cb0: e7a0 8172 3000 0000 7249 0000 0072 3500  ...r0...rI...r5.
+00000cc0: 0000 7228 0000 0054 7229 0000 0072 3600  ..r(...Tr)...r6.
+00000cd0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000ce0: 0000 0001 0000 0040 0000 0073 1c00 0000  .......@...s....
+00000cf0: 6500 5a01 6400 5a02 6401 5a03 6402 5a04  e.Z.d.Z.d.Z.d.Z.
+00000d00: 6504 5a05 6403 5a06 6404 5300 2905 7a12  e.Z.d.Z.d.S.).z.
+00000d10: 506f 7369 7469 6f6e 5469 746c 652e 4d65  PositionTitle.Me
+00000d20: 7461 5a11 6273 5f70 6f73 6974 696f 6e5f  taZ.bs_position_
+00000d30: 7469 746c 65f5 0600 0000 e881 8ce7 a7b0  title...........
+00000d40: 724a 0000 004e 724c 0000 0072 1a00 0000  rJ...NrL...r....
+00000d50: 721a 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
+00000d60: 1c00 0000 5f00 0000 7308 0000 0008 0104  ...._...s.......
+00000d70: 0104 0104 0172 1c00 0000 4e29 0e72 1600  .....r....N).r..
+00000d80: 0000 7217 0000 0072 1800 0000 7206 0000  ..r....r....r...
+00000d90: 0072 3a00 0000 723b 0000 0072 3f00 0000  .r:...r;...r?...
+00000da0: 7242 0000 0072 2200 0000 7243 0000 0072  rB...r"...rC...r
+00000db0: 4b00 0000 7245 0000 0072 4600 0000 721c  K...rE...rF...r.
+00000dc0: 0000 0072 1a00 0000 721a 0000 0072 1a00  ...r....r....r..
+00000dd0: 0000 721b 0000 0072 4e00 0000 5400 0000  ..r....rN...T...
+00000de0: 7314 0000 0008 010e 010e 0104 0102 0102  s...............
+00000df0: 0104 fd06 0512 0112 0272 4e00 0000 6300  .........rN...c.
+00000e00: 0000 0000 0000 0000 0000 0000 0000 0007  ................
+00000e10: 0000 0040 0000 0073 4e01 0000 6500 5a01  ...@...sN...e.Z.
+00000e20: 6400 5a02 6503 6a04 6401 6402 6403 8d02  d.Z.e.j.d.d.d...
+00000e30: 5a05 6503 6a04 6404 6402 6405 6405 6406  Z.e.j.d.d.d.d.d.
+00000e40: 8d04 5a06 6503 6a04 6407 6408 6405 6405  ..Z.e.j.d.d.d.d.
+00000e50: 6406 8d04 5a07 6503 6a04 6409 640a 6405  d...Z.e.j.d.d.d.
+00000e60: 6405 6406 8d04 5a08 6503 6a04 640b 640c  d.d...Z.e.j.d.d.
+00000e70: 6403 8d02 5a09 6503 6a04 640d 6402 6405  d...Z.e.j.d.d.d.
+00000e80: 6405 6406 8d04 5a0a 6503 6a0b 650c 640e  d.d...Z.e.j.e.d.
+00000e90: 6503 6a0d 640f 8d03 5a0e 6503 6a04 6410  e.j.d...Z.e.j.d.
+00000ea0: 6411 650f 6405 6405 6412 8d05 5a10 6503  d.e.d.d.d...Z.e.
+00000eb0: 6a04 6413 6414 6405 6405 6406 8d04 5a11  j.d.d.d.d.d...Z.
+00000ec0: 6503 6a04 6415 6408 6405 6405 6406 8d04  e.j.d.d.d.d.d...
+00000ed0: 5a12 6503 6a0b 6513 6416 6503 6a0d 640f  Z.e.j.e.d.e.j.d.
+00000ee0: 8d03 5a14 6503 6a0b 6515 6417 6503 6a0d  ..Z.e.j.e.d.e.j.
+00000ef0: 640f 8d03 5a16 6503 6a17 6418 6405 6405  d...Z.e.j.d.d.d.
+00000f00: 6419 8d03 5a18 6503 6a04 641a 641b 641c  d...Z.e.j.d.d.d.
+00000f10: 641d 8d03 5a19 6503 6a1a 641e 6405 6405  d...Z.e.j.d.d.d.
+00000f20: 6419 8d03 5a1b 6503 6a04 641f 6402 6405  d...Z.e.j.d.d.d.
+00000f30: 6405 6406 8d04 5a1c 6503 6a04 6420 6402  d.d...Z.e.j.d d.
+00000f40: 6405 6405 6406 8d04 5a1d 6503 6a1e 6421  d.d.d...Z.e.j.d!
+00000f50: 6405 6422 8d02 5a1f 4700 6423 6424 8400  d.d"..Z.G.d#d$..
+00000f60: 6424 8302 5a20 6425 5300 2926 da06 446f  d$..Z d%S.)&..Do
+00000f70: 6374 6f72 7223 0000 00e9 1400 0000 7225  ctorr#........r%
+00000f80: 0000 0072 2700 0000 5472 2900 0000 7506  ...r'...Tr)...u.
+00000f90: 0000 00e9 82ae e7ae b172 2800 0000 7506  .........r(...u.
+00000fa0: 0000 00e5 9cb0 e59d 8072 2400 0000 7506  .........r$...u.
+00000fb0: 0000 00e5 b7a5 e58f b7e9 4000 0000 7506  ..........@...u.
+00000fc0: 0000 00e8 818c e4bd 8d72 4f00 0000 7249  .........rO...rI
+00000fd0: 0000 00f5 0600 0000 e680 a7e5 88ab e902  ................
+00000fe0: 0000 00a9 0572 0d00 0000 7226 0000 00da  .....r....r&....
+00000ff0: 0763 686f 6963 6573 720f 0000 0072 2a00  .choicesr....r*.
+00001000: 0000 7506 0000 00e6 b091 e697 8fe9 0a00  ..u.............
+00001010: 0000 f50c 0000 00e8 baab e4bb bde8 af81  ................
+00001020: e58f b7f5 0c00 0000 e689 80e5 b19e e7a7  ................
+00001030: 91e5 aea4 7230 0000 00f5 0c00 0000 e587  ....r0..........
+00001040: bae7 949f e697 a5e6 9c9f 722b 0000 0075  ..........r+...u
+00001050: 0c00 0000 e58c bbe7 949f e785 a7e7 8987  ................
+00001060: e932 0000 005a 0c64 6f63 746f 725f 7068  .2...Z.doctor_ph
+00001070: 6f74 6f72 3400 0000 750c 0000 00e5 8cbb  otor4...u.......
+00001080: e794 9fe6 8f8f e8bf b072 3500 0000 7236  .........r5...r6
+00001090: 0000 0075 1500 0000 e698 afe5 90a6 e4ba  ...u............
+000010a0: 92e8 8194 e7bd 91e6 8ea5 e8af 8a72 1400  .............r..
+000010b0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000010c0: 0000 0001 0000 0040 0000 0073 1800 0000  .......@...s....
+000010d0: 6500 5a01 6400 5a02 6401 5a03 6402 5a04  e.Z.d.Z.d.Z.d.Z.
+000010e0: 6504 5a05 6403 5300 2904 7a0b 446f 6374  e.Z.d.S.).z.Doct
+000010f0: 6f72 2e4d 6574 615a 0962 735f 646f 6374  or.MetaZ.bs_doct
+00001100: 6f72 7509 0000 00e5 8cbb e794 9fe8 a1a8  oru.............
+00001110: 4e72 3700 0000 721a 0000 0072 1a00 0000  Nr7...r....r....
+00001120: 721a 0000 0072 1b00 0000 721c 0000 008a  r....r....r.....
+00001130: 0000 0073 0600 0000 0801 0401 0401 721c  ...s..........r.
+00001140: 0000 004e 2921 7216 0000 0072 1700 0000  ...N)!r....r....
+00001150: 7218 0000 0072 0600 0000 723a 0000 0072  r....r....r:...r
+00001160: 3b00 0000 723c 0000 00da 0565 6d61 696c  ;...r<.....email
+00001170: 7240 0000 0072 3f00 0000 da08 706f 7369  r@...r?.....posi
+00001180: 7469 6f6e 7242 0000 0072 4e00 0000 7243  tionrB...rN...rC
+00001190: 0000 005a 0e70 6f73 6974 696f 6e5f 7469  ...Z.position_ti
+000011a0: 746c 65da 0d47 454e 4445 525f 4348 4f49  tle..GENDER_CHOI
+000011b0: 4345 da06 6765 6e64 6572 5a06 6e61 7469  CE..genderZ.nati
+000011c0: 6f6e 5a05 6964 6e75 6d72 4700 0000 da06  onZ.idnumrG.....
+000011d0: 6f66 6669 6365 7222 0000 0072 4b00 0000  officer"...rK...
+000011e0: da09 4461 7465 4669 656c 64da 0862 6972  ..DateField..bir
+000011f0: 7468 6461 795a 0570 686f 746f 723d 0000  thdayZ.photor=..
+00001200: 00da 0864 6573 6372 6962 6572 4500 0000  ...describerE...
+00001210: 7246 0000 0072 2000 0000 5a11 6973 5f6f  rF...r ...Z.is_o
+00001220: 6e6c 696e 655f 636f 6e73 756c 7472 1c00  nline_consultr..
+00001230: 0000 721a 0000 0072 1a00 0000 721a 0000  ..r....r....r...
+00001240: 0072 1b00 0000 7250 0000 0068 0000 0073  .r....rP...h...s
+00001250: 3e00 0000 0801 0e01 1201 1201 1201 0e01  >...............
+00001260: 1201 0401 0201 0201 04fd 0605 1401 1201  ................
+00001270: 1201 0401 0201 0201 04fd 0605 0401 0201  ................
+00001280: 0201 04fd 0605 1002 1001 1001 1201 1202  ................
+00001290: 0e02 7250 0000 0063 0000 0000 0000 0000  ..rP...c........
+000012a0: 0000 0000 0000 0000 0700 0000 4000 0000  ............@...
+000012b0: 736e 0100 0065 005a 0164 005a 0265 036a  sn...e.Z.d.Z.e.j
+000012c0: 0464 0164 0264 0364 0364 048d 045a 0565  .d.d.d.d.d...Z.e
+000012d0: 036a 0464 0564 0664 0364 0364 048d 045a  .j.d.d.d.d.d...Z
+000012e0: 0665 036a 0764 0764 0364 0364 088d 035a  .e.j.d.d.d.d...Z
+000012f0: 0865 036a 0464 0964 0a65 0964 0364 0364  .e.j.d.d.e.d.d.d
+00001300: 0b8d 055a 0a65 036a 0464 0c64 0664 0364  ...Z.e.j.d.d.d.d
+00001310: 0364 048d 045a 0b65 036a 0c64 0d64 0e64  .d...Z.e.j.d.d.d
+00001320: 0364 0364 0f8d 045a 0d65 036a 0e65 0f64  .d.d...Z.e.j.e.d
+00001330: 1065 036a 1064 0364 118d 045a 1165 036a  .e.j.d.d...Z.e.j
+00001340: 0e65 1264 1265 036a 1064 0364 118d 045a  .e.d.e.j.d.d...Z
+00001350: 1365 036a 0e65 1464 1365 036a 1064 0364  .e.j.e.d.e.j.d.d
+00001360: 118d 045a 1565 036a 0464 1464 0664 1564  ...Z.e.j.d.d.d.d
+00001370: 168d 035a 1665 036a 0464 1764 0264 0364  ...Z.e.j.d.d.d.d
+00001380: 0364 048d 045a 1765 036a 0464 1864 0264  .d...Z.e.j.d.d.d
+00001390: 0364 0364 048d 045a 1865 036a 1964 1964  .d.d...Z.e.j.d.d
+000013a0: 0364 0364 088d 035a 1a65 036a 0464 1a64  .d.d...Z.e.j.d.d
+000013b0: 0664 0364 0364 048d 045a 1b65 036a 0464  .d.d.d...Z.e.j.d
+000013c0: 1b64 0664 0364 0364 048d 045a 1c65 036a  .d.d.d.d...Z.e.j
+000013d0: 1d64 1c64 0364 0364 1d8d 035a 1e65 036a  .d.d.d.d...Z.e.j
+000013e0: 1d64 1e64 0364 0364 1f8d 035a 1f47 0064  .d.d.d.d...Z.G.d
+000013f0: 2064 2184 0064 2183 025a 2065 2164 2264   d!..d!..Z e!d"d
+00001400: 2384 0083 015a 2265 2164 2464 2584 0083  #....Z"e!d$d%...
+00001410: 015a 2365 2164 2664 2784 0083 015a 2464  .Z#e!d&d'....Z$d
+00001420: 2853 0029 29da 0455 7365 7272 2300 0000  (S.))..Userr#...
+00001430: 7224 0000 0054 7229 0000 0072 2700 0000  r$...Tr)...r'...
+00001440: 7228 0000 0072 5a00 0000 722b 0000 0072  r(...rZ...r+...r
+00001450: 5300 0000 7254 0000 0072 5500 0000 7258  S...rT...rU...rX
+00001460: 0000 00f5 0600 0000 e68e 92e5 ba8f e901  ................
+00001470: 0000 00a9 0472 0d00 0000 7215 0000 0072  .....r....r....r
+00001480: 0f00 0000 722a 0000 0072 5900 0000 7231  ....r*...rY...r1
+00001490: 0000 0072 3000 0000 750c 0000 00e7 bb91  ...r0...u.......
+000014a0: e5ae 9ae5 8cbb e794 9f75 0c00 0000 e794  .........u......
+000014b0: a8e6 88b7 e5a4 b4e5 838f 5a0b 7573 6572  ..........Z.user
+000014c0: 5f61 7661 7461 7272 3400 0000 750c 0000  _avatarr4...u...
+000014d0: 00e9 bb98 e8ae a4e8 a792 e889 b275 0f00  .............u..
+000014e0: 0000 e58f afe6 938d e4bd 9ce7 a791 e5ae  ................
+000014f0: a475 0c00 0000 e6b3 a8e9 878a e8af b4e6  .u..............
+00001500: 988e 7235 0000 0072 3600 0000 720b 0000  ..r5...r6...r...
+00001510: 0072 0c00 0000 7210 0000 0072 1100 0000  .r....r....r....
+00001520: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00001530: 0001 0000 0040 0000 0073 1000 0000 6500  .....@...s....e.
+00001540: 5a01 6400 5a02 6401 5a03 6402 5300 2903  Z.d.Z.d.Z.d.S.).
+00001550: 7a09 5573 6572 2e4d 6574 6175 0c00 0000  z.User.Metau....
+00001560: e794 a8e6 88b7 e4bf a1e6 81af 4e29 0472  ............N).r
+00001570: 1600 0000 7217 0000 0072 1800 0000 720d  ....r....r....r.
+00001580: 0000 0072 1a00 0000 721a 0000 0072 1a00  ...r....r....r..
+00001590: 0000 721b 0000 0072 1c00 0000 b300 0000  ..r....r........
+000015a0: 7302 0000 0008 0272 1c00 0000 6301 0000  s......r....c...
+000015b0: 0000 0000 0000 0000 0002 0000 0002 0000  ................
+000015c0: 0043 0000 0073 1800 0000 7c00 6a00 7d01  .C...s....|.j.}.
+000015d0: 7c01 7314 7c00 6a01 a002 a100 7d01 7c01  |.s.|.j.....}.|.
+000015e0: 5300 2901 758e 0000 000a 2020 2020 2020  S.).u.....      
+000015f0: 2020 e88e b7e5 8f96 e5bd 93e5 898d e794    ..............
+00001600: a8e6 88b7 e9bb 98e8 aea4 e794 a8e6 88b7  ................
+00001610: e7bb 842c 0a20 2020 2020 2020 20e5 a682  ...,.        ...
+00001620: e69e 9ce6 9caa e8ae bee7 bdae efbc 8ce8  ................
+00001630: bf94 e59b 9ee7 acac e4b8 80e4 b8aa e794  ................
+00001640: a8e6 88b7 e7bb 840a 2020 2020 2020 2020  ........        
+00001650: e590 a6e5 8899 e8bf 94e5 9b9e e8ae bee7  ................
+00001660: bdae e79a 84e7 94a8 e688 b7e7 bb84 0a20  ............... 
+00001670: 2020 2020 2020 2029 035a 0d64 6566 6175         ).Z.defau
+00001680: 6c74 5f67 726f 7570 da06 6772 6f75 7073  lt_group..groups
+00001690: da05 6669 7273 74a9 0272 2f00 0000 5a09  ..first..r/...Z.
+000016a0: 7265 745f 6772 6f75 7072 1a00 0000 721a  ret_groupr....r.
+000016b0: 0000 0072 1b00 0000 da11 6765 745f 6465  ...r......get_de
+000016c0: 6661 756c 745f 6772 6f75 70bb 0000 0073  fault_group....s
+000016d0: 0800 0000 0007 0601 0401 0a01 7a16 5573  ............z.Us
+000016e0: 6572 2e67 6574 5f64 6566 6175 6c74 5f67  er.get_default_g
+000016f0: 726f 7570 6301 0000 0000 0000 0000 0000  roupc...........
+00001700: 0002 0000 0002 0000 0043 0000 0073 1c00  .........C...s..
+00001710: 0000 7c00 6a00 a001 a100 7d01 7c01 7318  ..|.j.....}.|.s.
+00001720: 7c00 6a00 a002 a100 7d01 7c01 5300 a901  |.j.....}.|.S...
+00001730: 4e29 0372 6800 0000 da03 616c 6cda 046e  N).rh.....all..n
+00001740: 6f6e 6572 6a00 0000 721a 0000 0072 1a00  onerj...r....r..
+00001750: 0000 721b 0000 00da 0d67 6574 5f61 6c6c  ..r......get_all
+00001760: 6772 6f75 7073 c700 0000 7308 0000 0000  groups....s.....
+00001770: 020a 0104 010a 017a 1255 7365 722e 6765  .......z.User.ge
+00001780: 745f 616c 6c67 726f 7570 7363 0100 0000  t_allgroupsc....
+00001790: 0000 0000 0000 0000 0200 0000 0100 0000  ................
+000017a0: 4300 0000 7318 0000 0064 017d 017c 006a  C...s....d.}.|.j
+000017b0: 007d 017c 0173 147c 006a 017d 017c 0153  .}.|.s.|.j.}.|.S
+000017c0: 0029 0275 3300 0000 0a20 2020 2020 2020  .).u3....       
+000017d0: 20e8 8eb7 e58f 96e7 94a8 e688 b7e9 bb98   ...............
+000017e0: e8ae a4e7 9a84 e7bb 84e7 bb87 e69c bae6  ................
+000017f0: 9e84 0a20 2020 2020 2020 204e 2902 7260  ...        N).r`
+00001800: 0000 0072 4b00 0000 2902 722f 0000 005a  ...rK...).r/...Z
+00001810: 0772 6574 5f6f 7267 721a 0000 0072 1a00  .ret_orgr....r..
+00001820: 0000 721b 0000 00da 1867 6574 5f64 6566  ..r......get_def
+00001830: 6175 6c74 5f6f 7267 616e 697a 6174 696f  ault_organizatio
+00001840: 6ece 0000 0073 0a00 0000 0005 0401 0601  n....s..........
+00001850: 0401 0601 7a1d 5573 6572 2e67 6574 5f64  ....z.User.get_d
+00001860: 6566 6175 6c74 5f6f 7267 616e 697a 6174  efault_organizat
+00001870: 696f 6e4e 2925 7216 0000 0072 1700 0000  ionN)%r....r....
+00001880: 7218 0000 0072 0600 0000 723a 0000 0072  r....r....r:...r
+00001890: 3b00 0000 723c 0000 0072 6100 0000 7262  ;...r<...ra...rb
+000018a0: 0000 0072 5e00 0000 725f 0000 005a 0969  ...r^...r_...Z.i
+000018b0: 6463 6172 646e 756d da0c 496e 7465 6765  dcardnum..Intege
+000018c0: 7246 6965 6c64 da08 6f72 6465 725f 6279  rField..order_by
+000018d0: 7242 0000 0072 4700 0000 7243 0000 0072  rB...rG...rC...r
+000018e0: 6000 0000 7222 0000 0072 4b00 0000 7250  `...r"...rK...rP
+000018f0: 0000 005a 0664 6f63 746f 725a 0a61 7661  ...Z.doctorZ.ava
+00001900: 7461 725f 7572 6c5a 1064 6566 6175 6c74  tar_urlZ.default
+00001910: 5f67 726f 7570 5f69 645a 0c61 6c6c 6f77  _group_idZ.allow
+00001920: 5f6f 6666 6963 6572 3d00 0000 da04 6e6f  _officer=.....no
+00001930: 7465 7245 0000 0072 4600 0000 721d 0000  terE...rF...r...
+00001940: 0072 1e00 0000 721f 0000 0072 1c00 0000  .r....r....r....
+00001950: da08 7072 6f70 6572 7479 726b 0000 0072  ..propertyrk...r
+00001960: 6f00 0000 7270 0000 0072 1a00 0000 721a  o...rp...r....r.
+00001970: 0000 0072 1a00 0000 721b 0000 0072 6400  ...r....r....rd.
+00001980: 0000 9000 0000 734e 0000 0008 0112 0112  ......sN........
+00001990: 0110 0114 0112 0112 0104 0102 0102 0104  ................
+000019a0: 0102 fc06 0604 0102 0102 0104 0102 fc06  ................
+000019b0: 0604 0102 0102 0104 0102 fc06 0710 0112  ................
+000019c0: 0112 0110 0112 0112 0110 0110 020e 0802  ................
+000019d0: 010a 0b02 010a 0602 0172 6400 0000 6300  .........rd...c.
+000019e0: 0000 0000 0000 0000 0000 0000 0000 0007  ................
+000019f0: 0000 0040 0000 0073 cc00 0000 6500 5a01  ...@...s....e.Z.
+00001a00: 6400 5a02 6401 5a03 6504 6a05 6506 6504  d.Z.d.Z.e.j.e.e.
+00001a10: 6a07 6402 6403 6403 6404 8d05 5a08 6504  j.d.d.d.d...Z.e.
+00001a20: 6a09 6405 6406 6407 8d02 5a0a 6504 6a09  j.d.d.d...Z.e.j.
+00001a30: 6405 6408 6403 6409 8d03 5a0b 6504 6a0c  d.d.d.d...Z.e.j.
+00001a40: 6403 640a 6403 640b 8d03 5a0d 6504 6a09  d.d.d.d...Z.e.j.
+00001a50: 640c 6405 6403 6403 640d 8d04 5a0e 6504  d.d.d.d.d...Z.e.
+00001a60: 6a0f 6510 640e 6504 6a07 640f 6403 6410  j.e.d.e.j.d.d.d.
+00001a70: 8d05 5a11 6504 6a12 6411 6412 6403 6413  ..Z.e.j.d.d.d.d.
+00001a80: 8d03 5a13 6504 6a09 6405 6414 6403 6403  ..Z.e.j.d.d.d.d.
+00001a90: 6415 8d04 5a14 6504 6a15 6416 6403 6403  d...Z.e.j.d.d.d.
+00001aa0: 6417 8d03 5a16 6504 6a15 6418 6403 6403  d...Z.e.j.d.d.d.
+00001ab0: 6419 8d03 5a17 4700 641a 641b 8400 641b  d...Z.G.d.d...d.
+00001ac0: 8302 5a18 641c 5300 291d da0a 4578 7472  ..Z.d.S.)...Extr
+00001ad0: 6147 726f 7570 7519 0000 000a 2020 2020  aGroupu.....    
+00001ae0: e8a7 92e8 89b2 e689 a9e5 8585 e8a1 a80a  ................
+00001af0: 2020 2020 da0b 6578 7472 615f 6772 6f75      ..extra_grou
+00001b00: 7054 2904 7232 0000 00da 0c72 656c 6174  pT).r2.....relat
+00001b10: 6564 5f6e 616d 6572 0f00 0000 722a 0000  ed_namer....r*..
+00001b20: 0072 5b00 0000 750c 0000 00e8 a792 e889  .r[...u.........
+00001b30: b2e4 bba3 e7a0 81a9 0272 2600 0000 720d  .........r&...r.
+00001b40: 0000 0075 0c00 0000 e8a7 92e8 89b2 e590  ...u............
+00001b50: 8de7 a7b0 2903 7226 0000 0072 0d00 0000  ....).r&...r....
+00001b60: 722a 0000 0072 1300 0000 2903 7215 0000  r*...r....).r...
+00001b70: 0072 0d00 0000 720f 0000 0075 0600 0000  .r....r....u....
+00001b80: e68f 8fe8 bfb0 2903 7226 0000 0072 0f00  ......).r&...r..
+00001b90: 0000 722a 0000 0072 3000 0000 7268 0000  ..r*...r0...rh..
+00001ba0: 00a9 0472 0d00 0000 7232 0000 0072 7700  ...r....r2...rw.
+00001bb0: 0000 720f 0000 0072 6500 0000 7266 0000  ..r....re...rf..
+00001bc0: 00a9 0372 0d00 0000 7215 0000 0072 0f00  ...r....r....r..
+00001bd0: 0000 7235 0000 00a9 0472 2600 0000 720d  ..r5.....r&...r.
+00001be0: 0000 0072 0f00 0000 722a 0000 0072 0b00  ...r....r*...r..
+00001bf0: 0000 720c 0000 0075 1200 0000 e69c 80e5  ..r....u........
+00001c00: 908e e69b b4e6 96b0 e697 b6e9 97b4 7211  ..............r.
+00001c10: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00001c20: 0000 0000 0100 0000 4000 0000 731c 0000  ........@...s...
+00001c30: 0065 005a 0164 005a 0264 015a 0364 025a  .e.Z.d.Z.d.Z.d.Z
+00001c40: 0465 045a 0564 035a 0664 0453 0029 057a  .e.Z.d.Z.d.S.).z
+00001c50: 0f45 7874 7261 4772 6f75 702e 4d65 7461  .ExtraGroup.Meta
+00001c60: 5a0e 6273 5f65 7874 7261 5f67 726f 7570  Z.bs_extra_group
+00001c70: 7506 0000 00e8 a792 e889 b229 0129 02da  u..........).)..
+00001c80: 0972 6f6c 655f 636f 6465 724b 0000 004e  .role_coderK...N
+00001c90: 724c 0000 0072 1a00 0000 721a 0000 0072  rL...r....r....r
+00001ca0: 1a00 0000 721b 0000 0072 1c00 0000 ef00  ....r....r......
+00001cb0: 0000 7308 0000 0008 0104 0104 0104 0172  ..s............r
+00001cc0: 1c00 0000 4e29 1972 1600 0000 7217 0000  ....N).r....r...
+00001cd0: 0072 1800 0000 da07 5f5f 646f 635f 5f72  .r......__doc__r
+00001ce0: 0600 0000 da0d 4f6e 6554 6f4f 6e65 4669  ......OneToOneFi
+00001cf0: 656c 6472 0400 0000 7243 0000 00da 0567  eldr....rC.....g
+00001d00: 726f 7570 723a 0000 0072 7c00 0000 5a09  roupr:...r|...Z.
+00001d10: 726f 6c65 5f6e 616d 6572 2000 0000 7221  role_namer ...r!
+00001d20: 0000 0072 7300 0000 7242 0000 0072 2200  ...rs...rB...r".
+00001d30: 0000 724b 0000 0072 7100 0000 7272 0000  ..rK...rq...rr..
+00001d40: 005a 0c63 7265 6174 6564 5f75 7365 7272  .Z.created_userr
+00001d50: 1d00 0000 5a0a 6372 6561 7465 645f 6174  ....Z.created_at
+00001d60: 5a0a 7570 6461 7465 645f 6174 721c 0000  Z.updated_atr...
+00001d70: 0072 1a00 0000 721a 0000 0072 1a00 0000  .r....r....r....
+00001d80: 721b 0000 0072 7500 0000 da00 0000 7324  r....ru.......s$
+00001d90: 0000 0008 0104 0316 010e 0110 0110 0112  ................
+00001da0: 0104 0102 0102 0104 0102 0102 fb06 0710  ................
+00001db0: 0112 0110 0110 0272 7500 0000 6300 0000  .......ru...c...
+00001dc0: 0000 0000 0000 0000 0000 0000 0007 0000  ................
+00001dd0: 0040 0000 0073 8c00 0000 6500 5a01 6400  .@...s....e.Z.d.
+00001de0: 5a02 6401 5a03 6504 6a05 6402 6403 6404  Z.d.Z.e.j.d.d.d.
+00001df0: 8d02 5a06 6504 6a07 6405 6406 6407 8d02  ..Z.e.j.d.d.d...
+00001e00: 5a08 6504 6a09 6408 6409 6406 640a 8d03  Z.e.j.d.d.d.d...
+00001e10: 5a0a 6504 6a09 640b 6409 6406 6406 640c  Z.e.j.d.d.d.d.d.
+00001e20: 8d04 5a0b 6504 6a05 640d 640e 6406 6406  ..Z.e.j.d.d.d.d.
+00001e30: 640f 8d04 5a0c 6504 6a0d 6410 6411 6504  d...Z.e.j.d.d.e.
+00001e40: 6a0e 6412 6406 6413 8d05 5a0f 4700 6414  j.d.d.d...Z.G.d.
+00001e50: 6415 8400 6415 8302 5a10 6416 6417 8400  d...d...Z.d.d...
+00001e60: 5a11 6418 5300 2919 da10 436f 6e74 656e  Z.d.S.)...Conten
+00001e70: 7454 7970 6543 6174 6573 7516 0000 000a  tTypeCatesu.....
+00001e80: 2020 2020 e88f 9ce5 8d95 e590 8de7 a7b0      ............
+00001e90: 0a20 2020 2072 2300 0000 7251 0000 0029  .    r#...rQ...)
+00001ea0: 0172 2600 0000 7213 0000 0054 2901 7215  .r&...r....T).r.
+00001eb0: 0000 0072 6500 0000 7266 0000 0072 7a00  ...re...rf...rz.
+00001ec0: 0000 7506 0000 00e7 baa7 e588 ab72 6700  ..u..........rg.
+00001ed0: 0000 f506 0000 00e5 9bbe e6a0 87e9 f401  ................
+00001ee0: 0000 7229 0000 0072 2f00 0000 750c 0000  ..r)...r/...u...
+00001ef0: 00e7 88b6 e7ba a7e8 8f9c e58d 95da 0863  ...............c
+00001f00: 6869 6c64 7265 6e72 7900 0000 6300 0000  hildrenry...c...
+00001f10: 0000 0000 0000 0000 0000 0000 0001 0000  ................
+00001f20: 0040 0000 0073 1c00 0000 6500 5a01 6400  .@...s....e.Z.d.
+00001f30: 5a02 6401 5a03 6402 5a04 6504 5a05 6403  Z.d.Z.d.Z.e.Z.d.
+00001f40: 5a06 6404 5300 2905 7a15 436f 6e74 656e  Z.d.S.).z.Conten
+00001f50: 7454 7970 6543 6174 6573 2e4d 6574 615a  tTypeCates.MetaZ
+00001f60: 1462 735f 636f 6e74 656e 745f 7479 7065  .bs_content_type
+00001f70: 5f63 6174 7375 0c00 0000 e88f 9ce5 8d95  _catsu..........
+00001f80: e590 8de7 a7b0 a901 7272 0000 004e a907  ........rr...N..
+00001f90: 7216 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
+00001fa0: 3800 0000 720d 0000 0072 3900 0000 da08  8...r....r9.....
+00001fb0: 6f72 6465 7269 6e67 721a 0000 0072 1a00  orderingr....r..
+00001fc0: 0000 721a 0000 0072 1b00 0000 721c 0000  ..r....r....r...
+00001fd0: 0009 0100 0073 0800 0000 0801 0401 0401  .....s..........
+00001fe0: 0401 721c 0000 0063 0100 0000 0000 0000  ..r....c........
+00001ff0: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
+00002000: 7306 0000 007c 006a 0053 0072 6c00 0000  s....|.j.S.rl...
+00002010: a901 723b 0000 00a9 0172 2f00 0000 721a  ..r;.....r/...r.
+00002020: 0000 0072 1a00 0000 721b 0000 00da 075f  ...r....r......_
+00002030: 5f73 7472 5f5f 0f01 0000 7302 0000 0000  _str__....s.....
+00002040: 017a 1843 6f6e 7465 6e74 5479 7065 4361  .z.ContentTypeCa
+00002050: 7465 732e 5f5f 7374 725f 5f4e 2912 7216  tes.__str__N).r.
+00002060: 0000 0072 1700 0000 7218 0000 0072 7d00  ...r....r....r}.
+00002070: 0000 7206 0000 0072 3a00 0000 723b 0000  ..r....r:...r;..
+00002080: 0072 2000 0000 7221 0000 0072 7100 0000  .r ...r!...rq...
+00002090: 7272 0000 00da 056c 6576 656c da0a 6963  rr.....level..ic
+000020a0: 6f6e 5f63 6c61 7373 7242 0000 0072 4300  on_classrB...rC.
+000020b0: 0000 7244 0000 0072 1c00 0000 7289 0000  ..rD...r....r...
+000020c0: 0072 1a00 0000 721a 0000 0072 1a00 0000  .r....r....r....
+000020d0: 721b 0000 0072 8000 0000 f800 0000 731e  r....r........s.
+000020e0: 0000 0008 0104 030e 010e 0110 0112 0112  ................
+000020f0: 0104 0102 0102 0104 0102 0102 fb06 080e  ................
+00002100: 0672 8000 0000 6300 0000 0000 0000 0000  .r....c.........
+00002110: 0000 0000 0000 0006 0000 0040 0000 0073  ...........@...s
+00002120: ce00 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
+00002130: 6504 6a05 6402 6403 6404 6405 8d03 5a06  e.j.d.d.d.d...Z.
+00002140: 6504 6a07 6508 6406 6504 6a09 6407 6408  e.j.e.d.e.j.d.d.
+00002150: 8d04 5a0a 6504 6a07 6409 640a 6504 6a09  ..Z.e.j.d.d.e.j.
+00002160: 640b 6408 8d04 5a0b 6504 6a05 640c 640d  d.d...Z.e.j.d.d.
+00002170: 6404 6404 640e 8d04 5a0c 6504 6a0d 640f  d.d.d...Z.e.j.d.
+00002180: 6404 6404 6410 8d03 5a0e 6504 6a0d 6411  d.d.d...Z.e.j.d.
+00002190: 6404 6404 6410 8d03 5a0f 6504 6a05 6412  d.d.d...Z.e.j.d.
+000021a0: 6413 6404 6414 8d03 5a10 6504 6a11 6415  d.d.d...Z.e.j.d.
+000021b0: 6404 6416 8d02 5a12 6504 6a13 6417 6404  d.d...Z.e.j.d.d.
+000021c0: 6404 6418 8d03 5a14 6504 6a15 6419 641a  d.d...Z.e.j.d.d.
+000021d0: 6404 641b 8d03 5a16 4700 641c 641d 8400  d.d...Z.G.d.d...
+000021e0: 641d 8302 5a17 641e 641f 8400 5a18 6420  d...Z.d.d...Z.d 
+000021f0: 5300 2921 da0d 436f 6e74 656e 7454 7970  S.)!..ContentTyp
+00002200: 6545 7875 1600 0000 0a20 2020 20e5 8a9f  eExu.....    ...
+00002210: e883 bde7 b1bb e588 ab0a 2020 2020 7223  ..........    r#
+00002220: 0000 0072 5100 0000 5429 0272 2600 0000  ...rQ...T).r&...
+00002230: 720f 0000 0075 0c00 0000 e7b3 bbe7 bb9f  r....u..........
+00002240: e5ba 94e7 94a8 da09 6578 7465 6e73 696f  ........extensio
+00002250: 6e29 0372 0d00 0000 7232 0000 0072 7700  n).r....r2...rw.
+00002260: 0000 7280 0000 0075 0600 0000 e88f 9ce5  ..r....u........
+00002270: 8d95 5a0d 636f 6e74 656e 745f 6361 7465  ..Z.content_cate
+00002280: 7372 8100 0000 7282 0000 0072 2900 0000  sr....r....r)...
+00002290: da03 7572 6c72 2b00 0000 7506 0000 00e7  ..urlr+...u.....
+000022a0: bb84 e688 9075 0600 0000 e58f 82e6 95b0  .....u..........
+000022b0: 725b 0000 00a9 0372 0d00 0000 7226 0000  r[.....r....r&..
+000022c0: 0072 0f00 0000 7509 0000 00e9 878d e5ae  .r....u.........
+000022d0: 9ae5 9091 a902 720d 0000 0072 0f00 0000  ......r....r....
+000022e0: 7213 0000 0029 0272 1500 0000 720f 0000  r....).r....r...
+000022f0: 0072 6500 0000 7266 0000 0072 7a00 0000  .re...rf...rz...
+00002300: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00002310: 0001 0000 0040 0000 0073 1c00 0000 6500  .....@...s....e.
+00002320: 5a01 6400 5a02 6401 5a03 6402 5a04 6504  Z.d.Z.d.Z.d.Z.e.
+00002330: 5a05 6403 5a06 6404 5300 2905 7a12 436f  Z.d.Z.d.S.).z.Co
+00002340: 6e74 656e 7454 7970 6545 782e 4d65 7461  ntentTypeEx.Meta
+00002350: 5a12 6273 5f63 6f6e 7465 6e74 5f74 7970  Z.bs_content_typ
+00002360: 655f 6578 7512 0000 00e5 8a9f e883 bde7  e_exu...........
+00002370: b1bb e588 abe8 a1a5 e585 8572 8400 0000  ...........r....
+00002380: 4e72 8500 0000 721a 0000 0072 1a00 0000  Nr....r....r....
+00002390: 721a 0000 0072 1b00 0000 721c 0000 002c  r....r....r....,
+000023a0: 0100 0073 0800 0000 0801 0401 0401 0401  ...s............
+000023b0: 721c 0000 0063 0100 0000 0000 0000 0000  r....c..........
+000023c0: 0000 0100 0000 0100 0000 4300 0000 7306  ..........C...s.
+000023d0: 0000 007c 006a 0053 0072 6c00 0000 7287  ...|.j.S.rl...r.
+000023e0: 0000 0072 8800 0000 721a 0000 0072 1a00  ...r....r....r..
+000023f0: 0000 721b 0000 0072 8900 0000 3201 0000  ..r....r....2...
+00002400: 7302 0000 0000 017a 1543 6f6e 7465 6e74  s......z.Content
+00002410: 5479 7065 4578 2e5f 5f73 7472 5f5f 4e29  TypeEx.__str__N)
+00002420: 1972 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
+00002430: 727d 0000 0072 0600 0000 723a 0000 0072  r}...r....r:...r
+00002440: 3b00 0000 7242 0000 0072 0500 0000 7243  ;...rB...r....rC
+00002450: 0000 00da 0c63 6f6e 7465 6e74 5f74 7970  .....content_typ
+00002460: 655a 1063 6f6e 7465 6e74 5f74 7970 655f  eZ.content_type_
+00002470: 6361 7472 8b00 0000 723d 0000 00da 0966  catr....r=.....f
+00002480: 726f 6e74 5f75 726c 5a0f 6672 6f6e 745f  ront_urlZ.front_
+00002490: 636f 6d70 6f6e 656e 745a 0c66 726f 6e74  componentZ.front
+000024a0: 5f70 6172 616d 73da 0855 524c 4669 656c  _params..URLFiel
+000024b0: 645a 1266 726f 6e74 5f72 6564 6972 6563  dZ.front_redirec
+000024c0: 745f 7572 6c72 2000 0000 7221 0000 0072  t_urlr ...r!...r
+000024d0: 7100 0000 7272 0000 0072 1c00 0000 7289  q...rr...r....r.
+000024e0: 0000 0072 1a00 0000 721a 0000 0072 1a00  ...r....r....r..
+000024f0: 0000 721b 0000 0072 8c00 0000 1301 0000  ..r....r........
+00002500: 732e 0000 0008 0104 0310 0104 0102 0102  s...............
+00002510: 0104 0102 fc06 0604 0102 0102 0104 0102  ................
+00002520: fc06 0612 0110 0110 0110 010e 0110 0110  ................
+00002530: 020e 0672 8c00 0000 6300 0000 0000 0000  ...r....c.......
+00002540: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
+00002550: 0073 3a00 0000 6500 5a01 6400 5a02 6401  .s:...e.Z.d.Z.d.
+00002560: 5a03 6504 6a05 6402 6403 6404 8d02 5a06  Z.e.j.d.d.d...Z.
+00002570: 6504 6a05 6405 6403 6404 8d02 5a07 4700  e.j.d.d.d...Z.G.
+00002580: 6406 6407 8400 6407 8302 5a08 6408 5300  d.d...d...Z.d.S.
+00002590: 2909 da0b 4578 7065 6e73 6554 7970 6575  )...ExpenseTypeu
+000025a0: 1600 0000 0a20 2020 20e8 b4b9 e794 a8e7  .....    .......
+000025b0: b1bb e59e 8b0a 2020 2020 7223 0000 0072  ......    r#...r
+000025c0: 5200 0000 7225 0000 0072 2c00 0000 6300  R...r%...r,...c.
+000025d0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
+000025e0: 0000 0040 0000 0073 1800 0000 6500 5a01  ...@...s....e.Z.
+000025f0: 6400 5a02 6401 5a03 6402 5a04 6504 5a05  d.Z.d.Z.d.Z.e.Z.
+00002600: 6403 5300 2904 7a10 4578 7065 6e73 6554  d.S.).z.ExpenseT
+00002610: 7970 652e 4d65 7461 5a0f 6273 5f65 7870  ype.MetaZ.bs_exp
+00002620: 656e 7365 5f74 7970 65f5 0c00 0000 e8b4  ense_type.......
+00002630: b9e7 94a8 e7b1 bbe5 9e8b 4e72 3700 0000  ..........Nr7...
+00002640: 721a 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
+00002650: 1b00 0000 721c 0000 003d 0100 0073 0600  ....r....=...s..
+00002660: 0000 0801 0401 0401 721c 0000 004e 2909  ........r....N).
+00002670: 7216 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
+00002680: 7d00 0000 7206 0000 0072 3a00 0000 723b  }...r....r:...r;
+00002690: 0000 00da 0463 6f64 6572 1c00 0000 721a  .....coder....r.
+000026a0: 0000 0072 1a00 0000 721a 0000 0072 1b00  ...r....r....r..
+000026b0: 0000 7294 0000 0036 0100 0073 0800 0000  ..r....6...s....
+000026c0: 0801 0403 0e01 0e02 7294 0000 0063 0000  ........r....c..
+000026d0: 0000 0000 0000 0000 0000 0000 0000 0600  ................
+000026e0: 0000 4000 0000 739c 0000 0065 005a 0164  ..@...s....e.Z.d
+000026f0: 005a 0265 036a 0464 0164 0264 0364 048d  .Z.e.j.d.d.d.d..
+00002700: 035a 0565 036a 0464 0564 0264 068d 025a  .Z.e.j.d.d.d...Z
+00002710: 0665 036a 0464 0764 0864 068d 025a 0765  .e.j.d.d.d...Z.e
+00002720: 036a 0864 0964 0364 0a8d 025a 0965 036a  .j.d.d.d...Z.e.j
+00002730: 0a65 0b64 0b65 036a 0c64 0364 0c8d 045a  .e.d.e.j.d.d...Z
+00002740: 0d65 036a 0464 0d64 0264 0364 0364 0e8d  .e.j.d.d.d.d.d..
+00002750: 045a 0e65 036a 0464 0f64 0264 0364 0364  .Z.e.j.d.d.d.d.d
+00002760: 0e8d 045a 0f65 036a 1065 1164 1064 0364  ...Z.e.j.e.d.d.d
+00002770: 118d 035a 1247 0064 1264 1384 0064 1383  ...Z.G.d.d...d..
+00002780: 025a 1364 1453 0029 15da 0f45 7870 656e  .Z.d.S.)...Expen
+00002790: 7365 5374 616e 6461 7264 7295 0000 0072  seStandardr....r
+000027a0: 2800 0000 5472 8f00 0000 750c 0000 00e6  (...Tr....u.....
+000027b0: a087 e587 86e5 908d e7a7 b072 2500 0000  ...........r%...
+000027c0: 750c 0000 00e6 a087 e587 86e7 bc96 e7a0  u...............
+000027d0: 8172 2400 0000 7506 0000 00e8 b4b9 e794  .r$...u.........
+000027e0: a872 9000 0000 7230 0000 0072 3100 0000  .r....r0...r1...
+000027f0: 7235 0000 0072 2900 0000 7236 0000 0075  r5...r)...r6...u
+00002800: 1200 0000 e58c bbe7 949f e8b4 b9e7 94a8  ................
+00002810: e6a0 87e5 8786 2902 720d 0000 0072 2a00  ......).r....r*.
+00002820: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00002830: 0000 0001 0000 0040 0000 0073 1c00 0000  .......@...s....
+00002840: 6500 5a01 6400 5a02 6401 5a03 6402 5a04  e.Z.d.Z.d.Z.d.Z.
+00002850: 6504 5a05 6403 5a06 6404 5300 2905 7a14  e.Z.d.Z.d.S.).z.
+00002860: 4578 7065 6e73 6553 7461 6e64 6172 642e  ExpenseStandard.
+00002870: 4d65 7461 5a13 6273 5f65 7870 656e 7365  MetaZ.bs_expense
+00002880: 5f73 7461 6e64 6172 6475 0f00 0000 e8b4  _standardu......
+00002890: b9e7 94a8 e6a0 87e5 8786 e8a1 a829 0129  .............).)
+000028a0: 02da 0d73 7461 6e64 6172 645f 636f 6465  ...standard_code
+000028b0: 724b 0000 004e 724c 0000 0072 1a00 0000  rK...NrL...r....
+000028c0: 721a 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
+000028d0: 1c00 0000 5301 0000 7308 0000 0008 0104  ....S...s.......
+000028e0: 0104 0104 0172 1c00 0000 4e29 1472 1600  .....r....N).r..
+000028f0: 0000 7217 0000 0072 1800 0000 7206 0000  ..r....r....r...
+00002900: 0072 3a00 0000 5a0c 6578 7065 6e73 655f  .r:...Z.expense_
+00002910: 7479 7065 5a0d 7374 616e 6461 7264 5f6e  typeZ.standard_n
+00002920: 616d 6572 9800 0000 7241 0000 005a 0466  amer....rA...Z.f
+00002930: 6565 7372 4200 0000 7222 0000 0072 4300  eesrB...r"...rC.
+00002940: 0000 724b 0000 0072 4500 0000 7246 0000  ..rK...rE...rF..
+00002950: 00da 0f4d 616e 7954 6f4d 616e 7946 6965  ...ManyToManyFie
+00002960: 6c64 7250 0000 005a 0764 6f63 746f 7273  ldrP...Z.doctors
+00002970: 721c 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
+00002980: 1a00 0000 721b 0000 0072 9700 0000 4301  ....r....r....C.
+00002990: 0000 731c 0000 0008 0210 010e 010e 010e  ..s.............
+000029a0: 0104 0102 0102 0104 0102 fc06 0612 0112  ................
+000029b0: 0110 0272 9700 0000 6300 0000 0000 0000  ...r....c.......
+000029c0: 0000 0000 0000 0000 0007 0000 0040 0000  .............@..
+000029d0: 0073 4c00 0000 6500 5a01 6400 5a02 6503  .sL...e.Z.d.Z.e.
+000029e0: 6a04 6401 6402 6403 8d02 5a05 6503 6a04  j.d.d.d...Z.e.j.
+000029f0: 6404 6402 6403 8d02 5a06 6503 6a07 6405  d.d.d...Z.e.j.d.
+00002a00: 6406 6503 6a08 6407 6408 6409 8d05 5a09  d.e.j.d.d.d...Z.
+00002a10: 4700 640a 640b 8400 640b 8302 5a0a 640c  G.d.d...d...Z.d.
+00002a20: 5300 290d da0e 496e 7370 6563 7469 6f6e  S.)...Inspection
+00002a30: 5479 7065 f512 0000 00e6 a380 e69f a5e7  Type............
+00002a40: b1bb e59e 8be7 bc96 e7a0 8172 5b00 0000  ...........r[...
+00002a50: 7225 0000 00f5 1200 0000 e6a3 80e6 9fa5  r%..............
+00002a60: e7b1 bbe5 9e8b e590 8de7 a7b0 722f 0000  ............r/..
+00002a70: 00f5 0600 0000 e788 b6e7 baa7 7283 0000  ............r...
+00002a80: 0054 7279 0000 0063 0000 0000 0000 0000  .Try...c........
+00002a90: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
+00002aa0: 7318 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
+00002ab0: 0364 025a 0465 045a 0564 0353 0029 047a  .d.Z.e.Z.d.S.).z
+00002ac0: 1349 6e73 7065 6374 696f 6e54 7970 652e  .InspectionType.
+00002ad0: 4d65 7461 5a12 6273 5f69 6e73 7065 6374  MetaZ.bs_inspect
+00002ae0: 696f 6e5f 7479 7065 7512 0000 00e6 a380  ion_typeu.......
+00002af0: e69f a5e5 ad97 e585 b8e7 b1bb e59e 8b4e  ...............N
+00002b00: 7237 0000 0072 1a00 0000 721a 0000 0072  r7...r....r....r
+00002b10: 1a00 0000 721b 0000 0072 1c00 0000 6701  ....r....r....g.
+00002b20: 0000 7306 0000 0008 0104 0104 0172 1c00  ..s..........r..
+00002b30: 0000 4ea9 0b72 1600 0000 7217 0000 0072  ..N..r....r....r
+00002b40: 1800 0000 7206 0000 0072 3a00 0000 da0a  ....r....r:.....
+00002b50: 636f 6465 5f73 7276 7470 da0a 6e61 6d65  code_srvtp..name
+00002b60: 5f73 7276 7470 7242 0000 0072 4300 0000  _srvtprB...rC...
+00002b70: 7244 0000 0072 1c00 0000 721a 0000 0072  rD...r....r....r
+00002b80: 1a00 0000 721a 0000 0072 1b00 0000 729a  ....r....r....r.
+00002b90: 0000 005c 0100 0073 1400 0000 0801 0e01  ...\...s........
+00002ba0: 0e01 0401 0201 0201 0401 0201 02fb 0608  ................
+00002bb0: 729a 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00002bc0: 0000 0000 0000 0600 0000 4000 0000 73ae  ..........@...s.
+00002bd0: 0000 0065 005a 0164 005a 0265 036a 0464  ...e.Z.d.Z.e.j.d
+00002be0: 0164 0264 0364 048d 035a 0565 036a 0464  .d.d.d...Z.e.j.d
+00002bf0: 0564 0664 078d 025a 0665 036a 0464 0864  .d.d...Z.e.j.d.d
+00002c00: 0964 078d 025a 0765 036a 0464 0864 0a64  .d...Z.e.j.d.d.d
+00002c10: 078d 025a 0865 036a 0964 0b64 0364 0c8d  ...Z.e.j.d.d.d..
+00002c20: 025a 0a65 036a 0464 0864 0d64 0364 0364  .Z.e.j.d.d.d.d.d
+00002c30: 0e8d 045a 0b65 036a 0464 0864 0f64 0364  ...Z.e.j.d.d.d.d
+00002c40: 0364 0e8d 045a 0c65 036a 0464 1064 1164  .d...Z.e.j.d.d.d
+00002c50: 0364 128d 035a 0d65 036a 0464 1364 1164  .d...Z.e.j.d.d.d
+00002c60: 0364 128d 035a 0e47 0064 1464 1584 0064  .d...Z.G.d.d...d
+00002c70: 1583 025a 0f64 1664 1784 005a 1064 1853  ...Z.d.d...Z.d.S
+00002c80: 0029 19da 1649 6e73 7065 6374 696f 6e44  .)...InspectionD
+00002c90: 6963 7469 6f6e 6172 6965 7372 2400 0000  ictionariesr$...
+00002ca0: f50c 0000 00e9 a1b9 e79b aee7 bc96 e7a0  ................
+00002cb0: 8154 722d 0000 0072 5200 0000 f50c 0000  .Tr-...rR.......
+00002cc0: 00e9 a1b9 e79b aee5 908d e7a7 b072 7800  .............rx.
+00002cd0: 0000 e980 0000 00f5 0c00 0000 e58c bbe9  ................
+00002ce0: 99a2 e7bc 96e7 a081 7248 0000 00f5 0c00  ........rH......
+00002cf0: 0000 e9a1 b9e7 9bae e8b4 b9e7 94a8 7290  ..............r.
+00002d00: 0000 00f5 0600 0000 e5a4 87e6 b3a8 727b  ..............r{
+00002d10: 0000 00f5 0c00 0000 e58c bae5 8886 e5ad  ................
+00002d20: 97e6 aeb5 729b 0000 0072 5b00 0000 728f  ....r....r[...r.
+00002d30: 0000 0072 9c00 0000 6300 0000 0000 0000  ...r....c.......
+00002d40: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
+00002d50: 0073 1800 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+00002d60: 5a03 6402 5a04 6504 5a05 6403 5300 2904  Z.d.Z.e.Z.d.S.).
+00002d70: 7a1b 496e 7370 6563 7469 6f6e 4469 6374  z.InspectionDict
+00002d80: 696f 6e61 7269 6573 2e4d 6574 615a 1a62  ionaries.MetaZ.b
+00002d90: 735f 696e 7370 6563 7469 6f6e 5f64 6963  s_inspection_dic
+00002da0: 7469 6f6e 6172 6965 7375 0c00 0000 e6a3  tionariesu......
+00002db0: 80e6 9fa5 e5ad 97e5 85b8 4e72 3700 0000  ..........Nr7...
+00002dc0: 721a 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
+00002dd0: 1b00 0000 721c 0000 0078 0100 0073 0600  ....r....x...s..
+00002de0: 0000 0801 0401 0401 721c 0000 0063 0100  ........r....c..
+00002df0: 0000 0000 0000 0000 0000 0600 0000 0b00  ................
+00002e00: 0000 4300 0000 73d4 0000 0074 0064 0164  ..C...s....t.d.d
+00002e10: 0264 038d 028f b47d 0174 01a0 027c 01a1  .d.....}.t...|..
+00002e20: 017d 027c 0264 0419 0064 0519 0064 0619  .}.|.d...d...d..
+00002e30: 0064 0719 007d 0374 03a0 04a1 008f 6a01  .d...}.t......j.
+00002e40: 007c 0344 005d 547d 0474 057c 0483 0101  .|.D.]T}.t.|....
+00002e50: 0074 066a 076a 087c 0464 0819 0064 098d  .t.j.j.|.d...d..
+00002e60: 017d 057c 0573 3a74 066a 076a 097c 0464  .}.|.s:t.j.j.|.d
+00002e70: 0819 007c 0464 0a19 007c 0464 0b19 007c  ...|.d...|.d...|
+00002e80: 04a0 0a64 0ca1 017c 0464 0d19 007c 0464  ...d...|.d...|.d
+00002e90: 0e19 0064 0f8d 0601 0071 3a57 0064 0004  ...d.....q:W.d..
+00002ea0: 0004 0083 0301 006e 1031 0073 a430 0001  .......n.1.s.0..
+00002eb0: 0001 0001 0059 0001 007c 0357 0002 0064  .....Y...|.W...d
+00002ec0: 0004 0004 0083 0301 0053 0031 0073 c630  .........S.1.s.0
+00002ed0: 0001 0001 0001 0059 0001 0064 0053 0029  .......Y...d.S.)
+00002ee0: 104e 7a1a 2e2f 6261 7365 5f73 7973 7465  .Nz../base_syste
+00002ef0: 6d2f 696e 7370 6469 632e 6a73 6f6e fa05  m/inspdic.json..
+00002f00: 7574 662d 38a9 01da 0865 6e63 6f64 696e  utf-8....encodin
+00002f10: 67da 0763 6f6e 7465 6e74 da04 6461 7461  g..content..data
+00002f20: da0c 6974 656d 7372 7669 6e66 6f73 da0b  ..itemsrvinfos..
+00002f30: 6974 656d 7372 7669 6e66 6fda 0863 6f64  itemsrvinfo..cod
+00002f40: 655f 7372 76a9 01da 0c70 726f 6a65 6374  e_srv....project
+00002f50: 5f63 6f64 65da 086e 616d 655f 7372 76da  _code..name_srv.
+00002f60: 0863 6f64 655f 6f72 67da 0570 7269 6365  .code_org..price
+00002f70: 729f 0000 0072 a000 0000 a906 72b2 0000  r....r......r...
+00002f80: 00da 0c70 726f 6a65 6374 5f6e 616d 65da  ...project_name.
+00002f90: 0d68 6f73 7069 7461 6c5f 636f 6465 da0c  .hospital_code..
+00002fa0: 7072 6f6a 6563 745f 6665 6573 729f 0000  project_feesr...
+00002fb0: 0072 a000 0000 290b da04 6f70 656e da04  .r....)...open..
+00002fc0: 6a73 6f6e da04 6c6f 6164 7202 0000 00da  json..loadr.....
+00002fd0: 0661 746f 6d69 63da 0570 7269 6e74 72a1  .atomic..printr.
+00002fe0: 0000 00da 076f 626a 6563 7473 da06 6669  .....objects..fi
+00002ff0: 6c74 6572 da06 6372 6561 7465 da03 6765  lter..create..ge
+00003000: 74a9 0672 2f00 0000 da01 61da 0672 6573  t..r/.....a..res
+00003010: 756c 7472 ad00 0000 da03 7265 735a 0673  ultr......resZ.s
+00003020: 705f 6469 6372 1a00 0000 721a 0000 0072  p_dicr....r....r
+00003030: 1b00 0000 da06 7570 6c6f 6164 7e01 0000  ......upload~...
+00003040: 7322 0000 0000 010e 020a 0114 010a 0108  s"..............
+00003050: 0108 0112 0104 0106 0106 0106 0106 0108  ................
+00003060: 0106 0106 fa26 087a 1d49 6e73 7065 6374  .....&.z.Inspect
+00003070: 696f 6e44 6963 7469 6f6e 6172 6965 732e  ionDictionaries.
+00003080: 7570 6c6f 6164 4ea9 1172 1600 0000 7217  uploadN..r....r.
+00003090: 0000 0072 1800 0000 7206 0000 0072 3a00  ...r....r....r:.
+000030a0: 0000 72b2 0000 0072 b700 0000 72b8 0000  ..r....r....r...
+000030b0: 005a 0b6f 6666 6963 655f 636f 6465 7241  .Z.office_coderA
+000030c0: 0000 0072 b900 0000 5a07 7265 6d61 726b  ...r....Z.remark
+000030d0: 735a 0b64 6973 7469 6e67 7569 7368 729f  sZ.distinguishr.
+000030e0: 0000 0072 a000 0000 721c 0000 0072 c700  ...r....r....r..
+000030f0: 0000 721a 0000 0072 1a00 0000 721a 0000  ..r....r....r...
+00003100: 0072 1b00 0000 72a1 0000 006d 0100 0073  .r....r....m...s
+00003110: 1600 0000 0801 1001 0e01 0e01 0e01 0e01  ................
+00003120: 1201 1201 1001 1002 0e06 72a1 0000 0063  ..........r....c
+00003130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003140: 0700 0000 4000 0000 734c 0000 0065 005a  ....@...sL...e.Z
+00003150: 0164 005a 0265 036a 0464 0164 0264 038d  .d.Z.e.j.d.d.d..
+00003160: 025a 0565 036a 0464 0464 0264 038d 025a  .Z.e.j.d.d.d...Z
+00003170: 0665 036a 0764 0564 0665 036a 0864 0764  .e.j.d.d.e.j.d.d
+00003180: 0864 098d 055a 0947 0064 0a64 0b84 0064  .d...Z.G.d.d...d
+00003190: 0b83 025a 0a64 0c53 0029 0dda 0f45 7861  ...Z.d.S.)...Exa
+000031a0: 6d69 6e61 7469 6f6e 5479 7065 729b 0000  minationTyper...
+000031b0: 0072 5b00 0000 7225 0000 0072 9c00 0000  .r[...r%...r....
+000031c0: 722f 0000 0072 9d00 0000 7283 0000 0054  r/...r....r....T
+000031d0: 7279 0000 0063 0000 0000 0000 0000 0000  ry...c..........
+000031e0: 0000 0000 0000 0100 0000 4000 0000 7318  ..........@...s.
+000031f0: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
+00003200: 025a 0465 045a 0564 0353 0029 047a 1445  .Z.e.Z.d.S.).z.E
+00003210: 7861 6d69 6e61 7469 6f6e 5479 7065 2e4d  xaminationType.M
+00003220: 6574 615a 1362 735f 6578 616d 696e 6174  etaZ.bs_examinat
+00003230: 696f 6e5f 7479 7065 7512 0000 00e6 a380  ion_typeu.......
+00003240: e9aa 8ce5 ad97 e585 b8e7 b1bb e59e 8b4e  ...............N
+00003250: 7237 0000 0072 1a00 0000 721a 0000 0072  r7...r....r....r
+00003260: 1a00 0000 721b 0000 0072 1c00 0000 9e01  ....r....r......
+00003270: 0000 7306 0000 0008 0104 0104 0172 1c00  ..s..........r..
+00003280: 0000 4e72 9e00 0000 721a 0000 0072 1a00  ..Nr....r....r..
+00003290: 0000 721a 0000 0072 1b00 0000 72c9 0000  ..r....r....r...
+000032a0: 0093 0100 0073 1400 0000 0801 0e01 0e01  .....s..........
+000032b0: 0401 0201 0201 0401 0201 02fb 0608 72c9  ..............r.
+000032c0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000032d0: 0000 0000 0600 0000 4000 0000 73ae 0000  ........@...s...
+000032e0: 0065 005a 0164 005a 0265 036a 0464 0164  .e.Z.d.Z.e.j.d.d
+000032f0: 0264 0364 048d 035a 0565 036a 0464 0564  .d.d...Z.e.j.d.d
+00003300: 0664 078d 025a 0665 036a 0464 0864 0964  .d...Z.e.j.d.d.d
+00003310: 078d 025a 0765 036a 0464 0864 0a64 078d  ...Z.e.j.d.d.d..
+00003320: 025a 0865 036a 0964 0b64 0364 0c8d 025a  .Z.e.j.d.d.d...Z
+00003330: 0a65 036a 0464 0864 0d64 0364 0364 0e8d  .e.j.d.d.d.d.d..
+00003340: 045a 0b65 036a 0464 0864 0f64 0364 0364  .Z.e.j.d.d.d.d.d
+00003350: 0e8d 045a 0c65 036a 0464 1064 1164 0364  ...Z.e.j.d.d.d.d
+00003360: 128d 035a 0d65 036a 0464 1364 1164 0364  ...Z.e.j.d.d.d.d
+00003370: 128d 035a 0e47 0064 1464 1584 0064 1583  ...Z.G.d.d...d..
+00003380: 025a 0f64 1664 1784 005a 1064 1853 0029  .Z.d.d...Z.d.S.)
+00003390: 19da 1745 7861 6d69 6e61 7469 6f6e 4469  ...ExaminationDi
+000033a0: 6374 696f 6e61 7269 6573 7224 0000 0072  ctionariesr$...r
+000033b0: a200 0000 5472 2d00 0000 7252 0000 0072  ....Tr-...rR...r
+000033c0: a300 0000 7278 0000 0072 a400 0000 72a5  ....rx...r....r.
+000033d0: 0000 0072 4800 0000 72a6 0000 0072 9000  ...rH...r....r..
+000033e0: 0000 72a7 0000 0072 7b00 0000 72a8 0000  ..r....r{...r...
+000033f0: 0075 1200 0000 e6a3 80e9 aa8c e7b1 bbe5  .u..............
+00003400: 9e8b e7bc 96e7 a081 725b 0000 0072 8f00  ........r[...r..
+00003410: 0000 7512 0000 00e6 a380 e9aa 8ce7 b1bb  ..u.............
+00003420: e59e 8be5 908d e7a7 b063 0000 0000 0000  .........c......
+00003430: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
+00003440: 0000 7318 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
+00003450: 015a 0364 025a 0465 045a 0564 0353 0029  .Z.d.Z.e.Z.d.S.)
+00003460: 047a 1c45 7861 6d69 6e61 7469 6f6e 4469  .z.ExaminationDi
+00003470: 6374 696f 6e61 7269 6573 2e4d 6574 615a  ctionaries.MetaZ
+00003480: 1b62 735f 6578 616d 696e 6174 696f 6e5f  .bs_examination_
+00003490: 6469 6374 696f 6e61 7269 6573 750c 0000  dictionariesu...
+000034a0: 00e6 a380 e9aa 8ce5 ad97 e585 b84e 7237  .............Nr7
+000034b0: 0000 0072 1a00 0000 721a 0000 0072 1a00  ...r....r....r..
+000034c0: 0000 721b 0000 0072 1c00 0000 af01 0000  ..r....r........
+000034d0: 7306 0000 0008 0104 0104 0172 1c00 0000  s..........r....
+000034e0: 6301 0000 0000 0000 0000 0000 0006 0000  c...............
+000034f0: 000b 0000 0043 0000 0073 d000 0000 7400  .....C...s....t.
+00003500: 6401 6402 6403 8d02 8fb0 7d01 7401 a002  d.d.d.....}.t...
+00003510: 7c01 a101 7d02 7c02 6404 1900 6405 1900  |...}.|.d...d...
+00003520: 6406 1900 6407 1900 7d03 7403 a004 a100  d...d...}.t.....
+00003530: 8f6a 0100 7c03 4400 5d54 7d04 7405 7c04  .j..|.D.]T}.t.|.
+00003540: 8301 0100 7406 6a07 6a08 7c04 6408 1900  ....t.j.j.|.d...
+00003550: 6409 8d01 7d05 7c05 733a 7406 6a07 6a09  d...}.|.s:t.j.j.
+00003560: 7c04 6408 1900 7c04 640a 1900 7c04 640b  |.d...|.d...|.d.
+00003570: 1900 7c04 a00a 640c a101 7c04 640d 1900  ..|...d...|.d...
+00003580: 7c04 640e 1900 640f 8d06 0100 713a 5700  |.d...d.....q:W.
+00003590: 6400 0400 0400 8303 0100 6e10 3100 73a4  d.........n.1.s.
+000035a0: 3000 0100 0100 0100 5900 0100 5700 6400  0.......Y...W.d.
+000035b0: 0400 0400 8303 0100 6e10 3100 73c2 3000  ........n.1.s.0.
+000035c0: 0100 0100 0100 5900 0100 7c03 5300 2910  ......Y...|.S.).
+000035d0: 4e7a 222e 2f62 6173 655f 7379 7374 656d  Nz"./base_system
+000035e0: 2f65 7861 6d69 6e61 7469 6f6e 5f64 6963  /examination_dic
+000035f0: 2e6a 736f 6e72 a900 0000 72aa 0000 0072  .jsonr....r....r
+00003600: ac00 0000 72ad 0000 0072 ae00 0000 72af  ....r....r....r.
+00003610: 0000 0072 b000 0000 72b1 0000 0072 b300  ...r....r....r..
+00003620: 0000 72b4 0000 0072 b500 0000 729f 0000  ..r....r....r...
+00003630: 0072 a000 0000 72b6 0000 0029 0b72 ba00  .r....r....).r..
+00003640: 0000 72bb 0000 0072 bc00 0000 7202 0000  ..r....r....r...
+00003650: 0072 bd00 0000 72be 0000 0072 ca00 0000  .r....r....r....
+00003660: 72bf 0000 0072 c000 0000 72c1 0000 0072  r....r....r....r
+00003670: c200 0000 72c3 0000 0072 1a00 0000 721a  ....r....r....r.
+00003680: 0000 0072 1b00 0000 72c7 0000 00b5 0100  ...r....r.......
+00003690: 0073 2200 0000 0001 0e02 0a01 1401 0a01  .s".............
+000036a0: 0801 0801 1201 0401 0601 0601 0601 0601  ................
+000036b0: 0801 0601 06fa 4408 7a1e 4578 616d 696e  ......D.z.Examin
+000036c0: 6174 696f 6e44 6963 7469 6f6e 6172 6965  ationDictionarie
+000036d0: 732e 7570 6c6f 6164 4e72 c800 0000 721a  s.uploadNr....r.
+000036e0: 0000 0072 1a00 0000 721a 0000 0072 1b00  ...r....r....r..
+000036f0: 0000 72ca 0000 00a4 0100 0073 1600 0000  ..r........s....
+00003700: 0801 1001 0e01 0e01 0e01 0e01 1201 1201  ................
+00003710: 1001 1002 0e06 72ca 0000 0063 0000 0000  ......r....c....
+00003720: 0000 0000 0000 0000 0000 0000 0600 0000  ................
+00003730: 4000 0000 733c 0000 0065 005a 0164 005a  @...s<...e.Z.d.Z
+00003740: 0265 036a 0464 0164 0264 0364 048d 035a  .e.j.d.d.d.d...Z
+00003750: 0565 036a 0464 0564 0664 0364 0364 078d  .e.j.d.d.d.d.d..
+00003760: 045a 0647 0064 0864 0984 0064 0983 025a  .Z.G.d.d...d...Z
+00003770: 0764 0a53 0029 0bda 1344 7275 6750 7265  .d.S.)...DrugPre
+00003780: 7061 7261 7469 6f6e 5479 7065 7224 0000  parationTyper$..
+00003790: 0072 2c00 0000 5472 2d00 0000 7252 0000  .r,...Tr-...rR..
+000037a0: 0075 0c00 0000 e7b1 bbe5 9e8b e590 8de7  .u..............
+000037b0: a7b0 727b 0000 0063 0000 0000 0000 0000  ..r{...c........
+000037c0: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
+000037d0: 7318 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
+000037e0: 0364 025a 0465 045a 0564 0353 0029 047a  .d.Z.e.Z.d.S.).z
+000037f0: 1844 7275 6750 7265 7061 7261 7469 6f6e  .DrugPreparation
+00003800: 5479 7065 2e4d 6574 615a 1862 735f 6472  Type.MetaZ.bs_dr
+00003810: 7567 5f70 7265 7061 7261 7469 6f6e 5f74  ug_preparation_t
+00003820: 7970 6575 1200 0000 e88d afe5 9381 e588  ypeu............
+00003830: b6e5 8982 e7b1 bbe5 9e8b 4e72 3700 0000  ..........Nr7...
+00003840: 721a 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
+00003850: 1b00 0000 721c 0000 00ce 0100 0073 0600  ....r........s..
+00003860: 0000 0801 0401 0401 721c 0000 004e 2908  ........r....N).
+00003870: 7216 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
+00003880: 0600 0000 723a 0000 0072 3f00 0000 da09  ....r:...r?.....
+00003890: 7479 7065 5f6e 616d 6572 1c00 0000 721a  type_namer....r.
+000038a0: 0000 0072 1a00 0000 721a 0000 0072 1b00  ...r....r....r..
+000038b0: 0000 72cb 0000 00ca 0100 0073 0600 0000  ..r........s....
+000038c0: 0801 1001 1202 72cb 0000 0063 0000 0000  ......r....c....
+000038d0: 0000 0000 0000 0000 0000 0000 0600 0000  ................
+000038e0: 4000 0000 733c 0000 0065 005a 0164 005a  @...s<...e.Z.d.Z
+000038f0: 0265 036a 0464 0164 0264 0364 048d 035a  .e.j.d.d.d.d...Z
+00003900: 0565 036a 0464 0564 0664 0364 0364 078d  .e.j.d.d.d.d.d..
+00003910: 045a 0647 0064 0864 0984 0064 0983 025a  .Z.G.d.d...d...Z
+00003920: 0764 0a53 0029 0bda 0844 7275 6754 7970  .d.S.)...DrugTyp
+00003930: 6572 2c00 0000 7224 0000 0054 a903 720d  er,...r$...T..r.
+00003940: 0000 0072 2600 0000 722e 0000 0072 2300  ...r&...r....r#.
+00003950: 0000 7252 0000 0072 2900 0000 6300 0000  ..rR...r)...c...
+00003960: 0000 0000 0000 0000 0000 0000 0001 0000  ................
+00003970: 0040 0000 0073 1800 0000 6500 5a01 6400  .@...s....e.Z.d.
+00003980: 5a02 6401 5a03 6402 5a04 6504 5a05 6403  Z.d.Z.d.Z.e.Z.d.
+00003990: 5300 2904 7a0d 4472 7567 5479 7065 2e4d  S.).z.DrugType.M
+000039a0: 6574 615a 0c62 735f 6472 7567 5f74 7970  etaZ.bs_drug_typ
+000039b0: 65f5 0c00 0000 e88d afe5 9381 e7b1 bbe5  e...............
+000039c0: 9e8b 4e72 3700 0000 721a 0000 0072 1a00  ..Nr7...r....r..
+000039d0: 0000 721a 0000 0072 1b00 0000 721c 0000  ..r....r....r...
+000039e0: 00d8 0100 0073 0600 0000 0801 0401 0401  .....s..........
+000039f0: 721c 0000 004e a908 7216 0000 0072 1700  r....N..r....r..
+00003a00: 0000 7218 0000 0072 0600 0000 723a 0000  ..r....r....r:..
+00003a10: 0072 9600 0000 723b 0000 0072 1c00 0000  .r....r;...r....
+00003a20: 721a 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
+00003a30: 1b00 0000 72cd 0000 00d4 0100 0073 0600  ....r........s..
+00003a40: 0000 0801 1001 1202 72cd 0000 0063 0000  ........r....c..
+00003a50: 0000 0000 0000 0000 0000 0000 0000 0600  ................
+00003a60: 0000 4000 0000 733c 0000 0065 005a 0164  ..@...s<...e.Z.d
+00003a70: 005a 0265 036a 0464 0164 0264 0364 048d  .Z.e.j.d.d.d.d..
+00003a80: 035a 0565 036a 0464 0564 0664 0364 0364  .Z.e.j.d.d.d.d.d
+00003a90: 078d 045a 0647 0064 0864 0984 0064 0983  ...Z.G.d.d...d..
+00003aa0: 025a 0764 0a53 0029 0bda 0c44 7275 6743  .Z.d.S.)...DrugC
+00003ab0: 6174 6567 6f72 7972 2400 0000 722c 0000  ategoryr$...r,..
+00003ac0: 0054 722d 0000 0072 5200 0000 750c 0000  .Tr-...rR...u...
+00003ad0: 00e7 b1bb e588 abe5 908d e7a7 b072 7b00  .............r{.
+00003ae0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00003af0: 0000 0001 0000 0040 0000 0073 1800 0000  .......@...s....
+00003b00: 6500 5a01 6400 5a02 6401 5a03 6402 5a04  e.Z.d.Z.d.Z.d.Z.
+00003b10: 6504 5a05 6403 5300 2904 7a11 4472 7567  e.Z.d.S.).z.Drug
+00003b20: 4361 7465 676f 7279 2e4d 6574 615a 1062  Category.MetaZ.b
+00003b30: 735f 6472 7567 5f63 6174 6567 6f72 7975  s_drug_categoryu
+00003b40: 0c00 0000 e88d afe5 9381 e7b1 bbe5 88ab  ................
+00003b50: 4e72 3700 0000 721a 0000 0072 1a00 0000  Nr7...r....r....
+00003b60: 721a 0000 0072 1b00 0000 721c 0000 00e2  r....r....r.....
+00003b70: 0100 0073 0600 0000 0801 0401 0401 721c  ...s..........r.
+00003b80: 0000 004e 2908 7216 0000 0072 1700 0000  ...N).r....r....
+00003b90: 7218 0000 0072 0600 0000 723a 0000 0072  r....r....r:...r
+00003ba0: 3f00 0000 5a0d 6361 7465 676f 7279 5f6e  ?...Z.category_n
+00003bb0: 616d 6572 1c00 0000 721a 0000 0072 1a00  amer....r....r..
+00003bc0: 0000 721a 0000 0072 1b00 0000 72d1 0000  ..r....r....r...
+00003bd0: 00de 0100 0073 0600 0000 0801 1001 1202  .....s..........
+00003be0: 72d1 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00003bf0: 0000 0000 0000 0600 0000 4000 0000 739e  ..........@...s.
+00003c00: 0100 0065 005a 0164 005a 0265 036a 0464  ...e.Z.d.Z.e.j.d
+00003c10: 0164 0264 0364 048d 035a 0565 036a 0464  .d.d.d...Z.e.j.d
+00003c20: 0564 0664 0364 0364 078d 045a 0665 036a  .d.d.d.d...Z.e.j
+00003c30: 0464 0564 0864 0364 0364 078d 045a 0765  .d.d.d.d.d...Z.e
+00003c40: 036a 0464 0564 0964 0364 0364 078d 045a  .j.d.d.d.d.d...Z
+00003c50: 0865 036a 0464 0a64 0b64 0364 0364 0c8d  .e.j.d.d.d.d.d..
+00003c60: 045a 0965 036a 0a65 0b64 0d65 036a 0c64  .Z.e.j.e.d.e.j.d
+00003c70: 0e8d 035a 0d65 036a 0a65 0e64 0f65 036a  ...Z.e.j.e.d.e.j
+00003c80: 0c64 0e8d 035a 0f65 036a 0a65 1064 1065  .d...Z.e.j.e.d.e
+00003c90: 036a 0c64 0e8d 035a 1165 036a 0464 1164  .j.d...Z.e.j.d.d
+00003ca0: 0b64 0364 0364 0c8d 045a 1265 036a 0464  .d.d.d...Z.e.j.d
+00003cb0: 1264 0b64 0364 0364 0c8d 045a 1365 036a  .d.d.d.d...Z.e.j
+00003cc0: 0464 1364 0b64 0364 0364 0c8d 045a 1465  .d.d.d.d.d...Z.e
+00003cd0: 036a 0464 1464 0b64 0364 0364 0c8d 045a  .j.d.d.d.d.d...Z
+00003ce0: 1565 036a 0464 1564 0b64 0364 0364 0c8d  .e.j.d.d.d.d.d..
+00003cf0: 045a 1665 036a 0464 1664 0b64 0364 0364  .Z.e.j.d.d.d.d.d
+00003d00: 0c8d 045a 1765 036a 0464 1764 0b64 0364  ...Z.e.j.d.d.d.d
+00003d10: 0364 0c8d 045a 1865 036a 1964 1864 0364  .d...Z.e.j.d.d.d
+00003d20: 198d 025a 1a65 036a 0464 1a64 0564 0364  ...Z.e.j.d.d.d.d
+00003d30: 0364 0c8d 045a 1b65 036a 0464 1b64 0564  .d...Z.e.j.d.d.d
+00003d40: 0364 0364 0c8d 045a 1c65 036a 0464 1c64  .d.d...Z.e.j.d.d
+00003d50: 0564 0364 0364 0c8d 045a 1d65 036a 0464  .d.d.d...Z.e.j.d
+00003d60: 0564 1d64 0364 0364 078d 045a 1e65 036a  .d.d.d.d...Z.e.j
+00003d70: 0464 0564 1e64 0364 0364 078d 045a 1f65  .d.d.d.d.d...Z.e
+00003d80: 036a 0464 1f64 0564 0364 208d 035a 2047  .j.d.d.d.d ..Z G
+00003d90: 0064 2164 2284 0064 2283 025a 2164 2353  .d!d"..d"..Z!d#S
+00003da0: 0029 24da 0d44 7275 6744 6972 6563 746f  .)$..DrugDirecto
+00003db0: 7279 f50c 0000 00e8 8daf e593 81e7 bc96  ry..............
+00003dc0: e7a0 8172 2400 0000 5472 ce00 0000 7252  ...r$...Tr....rR
+00003dd0: 0000 00f5 0c00 0000 e88d afe5 9381 e590  ................
+00003de0: 8de7 a7b0 727b 0000 00f5 0600 0000 e8a7  ....r{..........
+00003df0: 84e6 a0bc 750c 0000 00e5 9fba e69c ace5  ....u...........
+00003e00: 8d95 e4bd 8d75 1200 0000 e680 bbe9 878f  .....u..........
+00003e10: e58d 95e4 bd8d e7bc 96e7 a081 7251 0000  ............rQ..
+00003e20: 0072 2900 0000 f50c 0000 00e5 88b6 e589  .r).............
+00003e30: 82e7 b1bb e59e 8b72 4900 0000 f506 0000  .......rI.......
+00003e40: 00e7 b1bb e588 ab72 cf00 0000 750c 0000  .......r....u...
+00003e50: 00e5 8d95 e4bd 8de5 8982 e987 8f75 1300  .............u..
+00003e60: 0000 e8ae a1e9 878f 2fe9 9bb6 e594 aee5  ......../.......
+00003e70: 8d95 e4bd 8d75 1200 0000 e8ae a1e9 878f  .....u..........
+00003e80: e58d 95e4 bd8d e7bc 96e7 a081 f50c 0000  ................
+00003e90: 00e5 ba93 e5ad 98e6 95b0 e987 8f75 0c00  .............u..
+00003ea0: 0000 e5ba 93e5 ad98 e58d 95e4 bd8d 750c  ..............u.
+00003eb0: 0000 00e5 8cbb e4bf 9de7 b1bb e588 ab75  ...............u
+00003ec0: 0c00 0000 e586 9ce5 9088 e7b1 bbe5 88ab  ................
+00003ed0: 750f 0000 00e6 98af e590 a6e6 98af e59f  u...............
+00003ee0: bae8 8daf 7214 0000 0075 0c00 0000 e9ab  ....r....u......
+00003ef0: 98e5 8db1 e7ad 89e7 baa7 7512 0000 00e5  ..........u.....
+00003f00: 9bbd e5ae b6e8 b4af e6a0 87e7 bc96 e7a0  ................
+00003f10: 8175 1200 0000 e59b bde5 aeb6 e8b4 afe6  .u..............
+00003f20: a087 e590 8de7 a7b0 f506 0000 00e4 baa7  ................
+00003f30: e59c b0f5 0c00 0000 e794 9fe4 baa7 e58e  ................
+00003f40: 82e5 aeb6 7518 0000 00e5 8d95 e6ac a1e7  ....u...........
+00003f50: 94a8 e987 8fe5 8d95 e4bd 8de7 bc96 e7a0  ................
+00003f60: 8172 8f00 0000 6300 0000 0000 0000 0000  .r....c.........
+00003f70: 0000 0000 0000 0001 0000 0040 0000 0073  ...........@...s
+00003f80: 1800 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
+00003f90: 6402 5a04 6504 5a05 6403 5300 2904 7a12  d.Z.e.Z.d.S.).z.
+00003fa0: 4472 7567 4469 7265 6374 6f72 792e 4d65  DrugDirectory.Me
+00003fb0: 7461 5a11 6273 5f64 7275 675f 6469 7265  taZ.bs_drug_dire
+00003fc0: 6374 6f72 7975 0c00 0000 e88d afe5 9381  ctoryu..........
+00003fd0: e79b aee5 bd95 4e72 3700 0000 721a 0000  ......Nr7...r...
+00003fe0: 0072 1a00 0000 721a 0000 0072 1b00 0000  .r....r....r....
+00003ff0: 721c 0000 000c 0200 0073 0600 0000 0801  r........s......
+00004000: 0401 0401 721c 0000 004e 2922 7216 0000  ....r....N)"r...
+00004010: 0072 1700 0000 7218 0000 0072 0600 0000  .r....r....r....
+00004020: 723a 0000 00da 0964 7275 675f 636f 6465  r:.....drug_code
+00004030: da09 6472 7567 5f6e 616d 65da 0973 7461  ..drug_name..sta
+00004040: 6e64 6172 6473 5a0a 746f 7461 6c5f 756e  ndardsZ.total_un
+00004050: 6974 5a0f 746f 7461 6c5f 756e 6974 5f63  itZ.total_unit_c
+00004060: 6f64 6572 4200 0000 72cb 0000 00da 0a44  oderB...r......D
+00004070: 4f5f 4e4f 5448 494e 47da 1070 7265 7061  O_NOTHING..prepa
+00004080: 7261 7469 6f6e 5f74 7970 6572 d100 0000  ration_typer....
+00004090: da08 6361 7465 676f 7279 72cd 0000 00da  ..categoryr.....
+000040a0: 0964 7275 675f 7479 7065 5a09 756e 6974  .drug_typeZ.unit
+000040b0: 5f64 6f73 655a 0c6d 6561 7375 7265 5f75  _doseZ.measure_u
+000040c0: 6e69 745a 116d 6561 7375 7265 5f75 6e69  nitZ.measure_uni
+000040d0: 745f 636f 6465 5a0a 7374 6f63 6b5f 6c65  t_codeZ.stock_le
+000040e0: 6674 5a0a 7374 6f63 6b5f 756e 6974 5a03  ftZ.stock_unitZ.
+000040f0: 6d69 635a 0c72 6363 5f63 6174 6567 6f72  micZ.rcc_categor
+00004100: 7972 2000 0000 5a0c 6973 5f65 7373 656e  yr ...Z.is_essen
+00004110: 7469 616c 5a08 6872 5f6c 6576 656c 5a07  tialZ.hr_levelZ.
+00004120: 6762 5f63 6f64 655a 0767 625f 6e61 6d65  gb_codeZ.gb_name
+00004130: da0c 6f72 6967 696e 5f70 6c61 6365 da0c  ..origin_place..
+00004140: 6d61 6e75 6661 6374 7572 6572 5a0d 636f  manufacturerZ.co
+00004150: 6465 5f6d 6564 755f 6375 7272 1c00 0000  de_medu_curr....
+00004160: 721a 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
+00004170: 1b00 0000 72d2 0000 00e8 0100 0073 4600  ....r........sF.
+00004180: 0000 0801 1001 1201 1201 1201 1201 0401  ................
+00004190: 0201 0201 04fd 0605 0401 0201 0201 04fd  ................
+000041a0: 0605 0401 0201 0201 04fd 0605 1201 1201  ................
+000041b0: 1201 1201 1201 1201 1201 0e01 1201 1201  ................
+000041c0: 1201 1201 1201 1002 72d2 0000 0063 0000  ........r....c..
+000041d0: 0000 0000 0000 0000 0000 0000 0000 0600  ................
+000041e0: 0000 4000 0000 733c 0000 0065 005a 0164  ..@...s<...e.Z.d
+000041f0: 005a 0265 036a 0464 0164 0264 0364 048d  .Z.e.j.d.d.d.d..
+00004200: 035a 0565 036a 0464 0564 0664 0364 0364  .Z.e.j.d.d.d.d.d
+00004210: 078d 045a 0647 0064 0864 0984 0064 0983  ...Z.G.d.d...d..
+00004220: 025a 0764 0a53 0029 0bda 0c50 6861 726d  .Z.d.S.)...Pharm
+00004230: 6163 7954 7970 6572 2c00 0000 7224 0000  acyTyper,...r$..
+00004240: 0054 72ce 0000 0072 2300 0000 7252 0000  .Tr....r#...rR..
+00004250: 0072 2900 0000 6300 0000 0000 0000 0000  .r)...c.........
+00004260: 0000 0000 0000 0001 0000 0040 0000 0073  ...........@...s
+00004270: 1800 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
+00004280: 6402 5a04 6504 5a05 6403 5300 2904 7a11  d.Z.e.Z.d.S.).z.
+00004290: 5068 6172 6d61 6379 5479 7065 2e4d 6574  PharmacyType.Met
+000042a0: 615a 1062 735f 7068 6172 6d61 6379 5f74  aZ.bs_pharmacy_t
+000042b0: 7970 65f5 0c00 0000 e88d afe6 88bf e7b1  ype.............
+000042c0: bbe5 9e8b 4e72 3700 0000 721a 0000 0072  ....Nr7...r....r
+000042d0: 1a00 0000 721a 0000 0072 1b00 0000 721c  ....r....r....r.
+000042e0: 0000 0016 0200 0073 0600 0000 0801 0401  .......s........
+000042f0: 0401 721c 0000 004e 72d0 0000 0072 1a00  ..r....Nr....r..
+00004300: 0000 721a 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00004310: 0072 e400 0000 1202 0000 7306 0000 0008  .r........s.....
+00004320: 0110 0112 0272 e400 0000 6300 0000 0000  .....r....c.....
+00004330: 0000 0000 0000 0000 0000 0006 0000 0040  ...............@
+00004340: 0000 0073 3c00 0000 6500 5a01 6400 5a02  ...s<...e.Z.d.Z.
+00004350: 6503 6a04 6401 6402 6403 6404 8d03 5a05  e.j.d.d.d.d...Z.
+00004360: 6503 6a04 6405 6406 6403 6403 6407 8d04  e.j.d.d.d.d.d...
+00004370: 5a06 4700 6408 6409 8400 6409 8302 5a07  Z.G.d.d...d...Z.
+00004380: 640a 5300 290b da12 5068 6172 6d61 6379  d.S.)...Pharmacy
+00004390: 456e 7465 7270 7269 7365 722c 0000 0072  Enterpriser,...r
+000043a0: 2400 0000 5472 ce00 0000 7223 0000 0072  $...Tr....r#...r
+000043b0: 5200 0000 7229 0000 0063 0000 0000 0000  R...r)...c......
+000043c0: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
+000043d0: 0000 7318 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
+000043e0: 015a 0364 025a 0465 045a 0564 0353 0029  .Z.d.Z.e.Z.d.S.)
+000043f0: 047a 1750 6861 726d 6163 7945 6e74 6572  .z.PharmacyEnter
+00004400: 7072 6973 652e 4d65 7461 5a16 6273 5f70  prise.MetaZ.bs_p
+00004410: 6861 726d 6163 795f 656e 7465 7270 7269  harmacy_enterpri
+00004420: 7365 750c 0000 00e8 8daf e4bc 81e7 aea1  seu.............
+00004430: e790 864e 7237 0000 0072 1a00 0000 721a  ...Nr7...r....r.
+00004440: 0000 0072 1a00 0000 721b 0000 0072 1c00  ...r....r....r..
+00004450: 0000 2002 0000 7306 0000 0008 0104 0104  .. ...s.........
+00004460: 0172 1c00 0000 4e72 d000 0000 721a 0000  .r....Nr....r...
+00004470: 0072 1a00 0000 721a 0000 0072 1b00 0000  .r....r....r....
+00004480: 72e6 0000 001c 0200 0073 0600 0000 0801  r........s......
+00004490: 1001 1202 72e6 0000 0063 0000 0000 0000  ....r....c......
+000044a0: 0000 0000 0000 0000 0000 0600 0000 4000  ..............@.
+000044b0: 0000 7386 0000 0065 005a 0164 005a 0265  ..s....e.Z.d.Z.e
+000044c0: 036a 0464 0164 0264 0364 048d 035a 0565  .j.d.d.d.d...Z.e
+000044d0: 036a 0464 0564 0664 0364 0364 078d 045a  .j.d.d.d.d.d...Z
+000044e0: 0665 036a 0765 0864 0865 036a 0964 098d  .e.j.e.d.e.j.d..
+000044f0: 035a 0a65 036a 0b64 0a64 0364 0364 0b8d  .Z.e.j.d.d.d.d..
+00004500: 035a 0c65 036a 0765 0d64 0c65 036a 0e64  .Z.e.j.e.d.e.j.d
+00004510: 0364 0d8d 045a 0f65 036a 0765 1064 0e65  .d...Z.e.j.e.d.e
+00004520: 036a 0e64 0364 0d8d 045a 1147 0064 0f64  .j.d.d...Z.G.d.d
+00004530: 1084 0064 1083 025a 1264 1153 0029 12da  ...d...Z.d.S.)..
+00004540: 1250 6861 726d 6163 794d 616e 6167 656d  .PharmacyManagem
+00004550: 656e 7475 0c00 0000 e88d afe6 88bf e7bc  entu............
+00004560: 96e7 a081 7224 0000 0054 72ce 0000 0075  ....r$...Tr....u
+00004570: 0c00 0000 e88d afe6 88bf e590 8de7 a7b0  ................
+00004580: 7252 0000 0072 2900 0000 72e5 0000 0072  rR...r)...r....r
+00004590: 4900 0000 750c 0000 00e8 8daf e688 bfe5  I...u...........
+000045a0: 9cb0 e59d 8072 2b00 0000 7230 0000 0072  .....r+...r0...r
+000045b0: 3100 0000 750c 0000 00e6 8980 e5b1 9ee8  1...u...........
+000045c0: 8daf e4bc 8163 0000 0000 0000 0000 0000  .....c..........
+000045d0: 0000 0000 0000 0100 0000 4000 0000 7318  ..........@...s.
+000045e0: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
+000045f0: 025a 0465 045a 0564 0353 0029 047a 1750  .Z.e.Z.d.S.).z.P
+00004600: 6861 726d 6163 794d 616e 6167 656d 656e  harmacyManagemen
+00004610: 742e 4d65 7461 5a16 6273 5f70 6861 726d  t.MetaZ.bs_pharm
+00004620: 6163 795f 6d61 6e61 6765 6d65 6e74 750c  acy_managementu.
+00004630: 0000 00e8 8daf e688 bfe7 aea1 e790 864e  ...............N
+00004640: 7237 0000 0072 1a00 0000 721a 0000 0072  r7...r....r....r
+00004650: 1a00 0000 721b 0000 0072 1c00 0000 3202  ....r....r....2.
+00004660: 0000 7306 0000 0008 0104 0104 0172 1c00  ..s..........r..
+00004670: 0000 4e29 1372 1600 0000 7217 0000 0072  ..N).r....r....r
+00004680: 1800 0000 7206 0000 0072 3a00 0000 5a0d  ....r....r:...Z.
+00004690: 7068 6172 6d61 6379 5f63 6f64 655a 0d70  pharmacy_codeZ.p
+000046a0: 6861 726d 6163 795f 6e61 6d65 7242 0000  harmacy_namerB..
+000046b0: 0072 e400 0000 72de 0000 005a 0d70 6861  .r....r....Z.pha
+000046c0: 726d 6163 795f 7479 7065 723d 0000 0072  rmacy_typer=...r
+000046d0: 4000 0000 7222 0000 0072 4300 0000 724b  @...r"...rC...rK
+000046e0: 0000 0072 e600 0000 5a0a 656e 7465 7270  ...r....Z.enterp
+000046f0: 7269 7365 721c 0000 0072 1a00 0000 721a  riser....r....r.
+00004700: 0000 0072 1a00 0000 721b 0000 0072 e700  ...r....r....r..
+00004710: 0000 2602 0000 7316 0000 0008 0110 0112  ..&...s.........
+00004720: 0104 0102 0102 0104 fd06 0510 0114 0114  ................
+00004730: 0272 e700 0000 6300 0000 0000 0000 0000  .r....c.........
+00004740: 0000 0000 0000 0006 0000 0040 0000 0073  ...........@...s
+00004750: 4e01 0000 6500 5a01 6400 5a02 6503 6a04  N...e.Z.d.Z.e.j.
+00004760: 6505 6401 6503 6a06 6402 6403 8d04 5a07  e.d.e.j.d.d...Z.
+00004770: 6503 6a08 6404 6405 6402 6402 6406 8d04  e.j.d.d.d.d.d...
+00004780: 5a09 6503 6a08 6407 6408 6402 6402 6409  Z.e.j.d.d.d.d.d.
+00004790: 8d04 5a0a 6503 6a08 6407 640a 6402 6402  ..Z.e.j.d.d.d.d.
+000047a0: 6409 8d04 5a0b 6503 6a08 6407 640b 6402  d...Z.e.j.d.d.d.
+000047b0: 6402 6409 8d04 5a0c 6503 6a04 650d 640c  d.d...Z.e.j.e.d.
+000047c0: 6503 6a0e 640d 8d03 5a0f 6503 6a04 6510  e.j.d...Z.e.j.e.
+000047d0: 640e 6503 6a0e 640d 8d03 5a11 6503 6a04  d.e.j.d...Z.e.j.
+000047e0: 6512 640f 6503 6a0e 640d 8d03 5a13 6503  e.d.e.j.d...Z.e.
+000047f0: 6a08 6410 6411 6402 6402 6409 8d04 5a14  j.d.d.d.d.d...Z.
+00004800: 6503 6a08 6412 6413 6402 6402 6409 8d04  e.j.d.d.d.d.d...
+00004810: 5a15 6503 6a04 6516 6414 6503 6a06 6402  Z.e.j.e.d.e.j.d.
+00004820: 6403 8d04 5a17 6503 6a18 6415 6402 6402  d...Z.e.j.d.d.d.
+00004830: 6416 8d03 5a19 6503 6a1a 6417 6418 6402  d...Z.e.j.d.d.d.
+00004840: 6419 8d03 5a1b 6503 6a08 6407 641a 6402  d...Z.e.j.d.d.d.
+00004850: 6402 6409 8d04 5a1c 6503 6a1d 641b 6402  d.d...Z.e.j.d.d.
+00004860: 641c 8d02 5a1e 6503 6a1d 641d 6402 641c  d...Z.e.j.d.d.d.
+00004870: 8d02 5a1f 6503 6a1d 641e 6402 641c 8d02  ..Z.e.j.d.d.d...
+00004880: 5a20 6503 6a1d 641f 6402 641c 8d02 5a21  Z e.j.d.d.d...Z!
+00004890: 4700 6420 6421 8400 6421 8302 5a22 6422  G.d d!..d!..Z"d"
+000048a0: 5300 2923 da0c 5068 6172 6d61 6379 4472  S.)#..PharmacyDr
+000048b0: 7567 750c 0000 00e6 8980 e5b1 9ee8 8daf  ugu.............
+000048c0: e688 bf54 7231 0000 0072 d300 0000 7224  ...Tr1...r....r$
+000048d0: 0000 0072 2900 0000 7252 0000 0072 d400  ...r)...rR...r..
+000048e0: 0000 727b 0000 0072 d500 0000 7506 0000  ..r{...r....u...
+000048f0: 00e5 8d95 e4bd 8d72 d600 0000 7249 0000  .......r....rI..
+00004900: 0072 cf00 0000 72d7 0000 0072 8200 0000  .r....r....r....
+00004910: 72d9 0000 00e9 c800 0000 72da 0000 0072  r.........r....r
+00004920: 3000 0000 750c 0000 00e6 9c89 e695 88e6  0...u...........
+00004930: 97a5 e69c 9f72 1100 0000 72d8 0000 0072  .....r....r....r
+00004940: 0100 0000 727a 0000 0075 0c00 0000 e8ae  ....rz...u......
+00004950: a1e9 878f e58d 95e4 bd8d 750c 0000 00e6  ..........u.....
+00004960: 8890 e69c ace5 8d95 e4bb b772 9000 0000  ...........r....
+00004970: 750c 0000 00e6 8890 e69c ace9 8791 e9a2  u...............
+00004980: 9d75 0c00 0000 e99b b6e5 94ae e58d 95e4  .u..............
+00004990: bbb7 750c 0000 00e9 9bb6 e594 aee9 8791  ..u.............
+000049a0: e9a2 9d63 0000 0000 0000 0000 0000 0000  ...c............
+000049b0: 0000 0000 0100 0000 4000 0000 7318 0000  ........@...s...
+000049c0: 0065 005a 0164 005a 0264 015a 0364 025a  .e.Z.d.Z.d.Z.d.Z
+000049d0: 0465 045a 0564 0353 0029 047a 1150 6861  .e.Z.d.S.).z.Pha
+000049e0: 726d 6163 7944 7275 672e 4d65 7461 5a10  rmacyDrug.MetaZ.
+000049f0: 6273 5f70 6861 726d 6163 795f 6472 7567  bs_pharmacy_drug
+00004a00: 750d 0000 00e8 8daf e688 bf2d e88d afe5  u..........-....
+00004a10: 9381 4e72 3700 0000 721a 0000 0072 1a00  ..Nr7...r....r..
+00004a20: 0000 721a 0000 0072 1b00 0000 721c 0000  ..r....r....r...
+00004a30: 0058 0200 0073 0600 0000 0801 0401 0401  .X...s..........
+00004a40: 721c 0000 004e 2923 7216 0000 0072 1700  r....N)#r....r..
+00004a50: 0000 7218 0000 0072 0600 0000 7242 0000  ..r....r....rB..
+00004a60: 0072 e700 0000 7243 0000 005a 0870 6861  .r....rC...Z.pha
+00004a70: 726d 6163 7972 3a00 0000 72db 0000 0072  rmacyr:...r....r
+00004a80: dc00 0000 72dd 0000 00da 0575 6e69 7473  ....r......units
+00004a90: 72cb 0000 0072 de00 0000 72df 0000 0072  r....r....r....r
+00004aa0: cd00 0000 72e1 0000 0072 d100 0000 72e0  ....r....r....r.
+00004ab0: 0000 0072 e200 0000 72e3 0000 0072 2200  ...r....r....r".
+00004ac0: 0000 724b 0000 0072 6100 0000 5a0a 7661  ..rK...ra...Z.va
+00004ad0: 6c69 645f 6461 7465 7271 0000 005a 1269  lid_daterq...Z.i
+00004ae0: 6e76 656e 746f 7279 5f71 7561 6e74 6974  nventory_quantit
+00004af0: 795a 106d 6561 7375 7265 6d65 6e74 5f75  yZ.measurement_u
+00004b00: 6e69 7472 4100 0000 5a0f 636f 7374 5f75  nitrA...Z.cost_u
+00004b10: 6e69 745f 7072 6963 655a 0b63 6f73 745f  nit_priceZ.cost_
+00004b20: 616d 6f75 6e74 5a11 7265 7461 696c 5f75  amountZ.retail_u
+00004b30: 6e69 745f 7072 6963 655a 0d72 6574 6169  nit_priceZ.retai
+00004b40: 6c5f 616d 6f75 6e74 721c 0000 0072 1a00  l_amountr....r..
+00004b50: 0000 721a 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00004b60: 0072 e800 0000 3802 0000 733e 0000 0008  .r....8...s>....
+00004b70: 0114 0112 0112 0112 0112 0104 0102 0102  ................
+00004b80: 0104 fd06 0504 0102 0102 0104 fd06 0504  ................
+00004b90: 0102 0102 0104 fd06 0512 0112 0114 0110  ................
+00004ba0: 0110 0112 010e 010e 010e 010e 0272 e800  .............r..
+00004bb0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00004bc0: 0000 0006 0000 0040 0000 0073 b600 0000  .......@...s....
+00004bd0: 6500 5a01 6400 5a02 6503 6a04 6401 6402  e.Z.d.Z.e.j.d.d.
+00004be0: 6403 8d02 5a05 6503 6a04 6401 6404 6403  d...Z.e.j.d.d.d.
+00004bf0: 8d02 5a06 6503 6a04 6401 6405 6406 6406  ..Z.e.j.d.d.d.d.
+00004c00: 6407 8d04 5a07 6503 6a04 6401 6408 6403  d...Z.e.j.d.d.d.
+00004c10: 8d02 5a08 6503 6a04 6401 6409 6403 8d02  ..Z.e.j.d.d.d...
+00004c20: 5a09 6503 6a04 640a 640b 6403 8d02 5a0a  Z.e.j.d.d.d...Z.
+00004c30: 6503 6a04 640a 640c 6403 8d02 5a0b 6503  e.j.d.d.d...Z.e.
+00004c40: 6a0c 640d 6406 6406 640e 8d03 5a0d 6503  j.d.d.d.d...Z.e.
+00004c50: 6a0c 640f 6406 6406 6410 8d03 5a0e 6503  j.d.d.d.d...Z.e.
+00004c60: 6a0f 6411 6406 6412 8d02 5a10 4700 6413  j.d.d.d...Z.G.d.
+00004c70: 6414 8400 6414 8302 5a11 6415 6416 8400  d...d...Z.d.d...
+00004c80: 5a12 6417 5300 2918 da07 4170 6949 6e66  Z.d.S.)...ApiInf
+00004c90: 6f72 5b00 0000 72a5 0000 0072 7800 0000  or[...r....rx...
+00004ca0: 750c 0000 00e8 afb7 e6b1 82e7 bc96 e7a0  u...............
+00004cb0: 8175 0c00 0000 e8af b7e6 b182 e590 8de7  .u..............
+00004cc0: a7b0 5472 7b00 0000 750c 0000 00e8 afb7  ..Tr{...u.......
+00004cd0: e6b1 82e6 96b9 e5bc 8f75 1200 0000 e8af  .........u......
+00004ce0: b7e6 b182 e695 b0e6 8dae e7b1 bbe5 9e8b  ................
+00004cf0: 72e9 0000 0075 1100 0000 6970 e59c b0e5  r....u....ip....
+00004d00: 9d80 e688 96e5 9f9f e590 8d75 0c00 0000  ...........u....
+00004d10: e8af b7e6 b182 e8b7 afe7 94b1 720b 0000  ............r...
+00004d20: 0072 0c00 0000 7210 0000 0072 1100 0000  .r....r....r....
+00004d30: 7213 0000 0072 1400 0000 6300 0000 0000  r....r....c.....
+00004d40: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
+00004d50: 0000 0073 1c00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00004d60: 6401 5a03 6402 5a04 6504 5a05 6403 5a06  d.Z.d.Z.e.Z.d.Z.
+00004d70: 6404 5300 2905 7a0c 4170 6949 6e66 6f2e  d.S.).z.ApiInfo.
+00004d80: 4d65 7461 5a0b 6273 5f61 7069 5f69 6e66  MetaZ.bs_api_inf
+00004d90: 6f75 0c00 0000 e68e a5e5 8fa3 e4bf a1e6  ou..............
+00004da0: 81af 2901 a902 da08 6f72 675f 636f 6465  ..).....org_code
+00004db0: da08 7265 715f 636f 6465 4e72 4c00 0000  ..req_codeNrL...
+00004dc0: 721a 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
+00004dd0: 1b00 0000 721c 0000 006a 0200 0073 0800  ....r....j...s..
+00004de0: 0000 0801 0401 0401 0401 721c 0000 0063  ..........r....c
+00004df0: 0300 0000 0000 0000 0000 0000 0700 0000  ................
+00004e00: 0500 0000 4300 0000 73ba 0000 0074 006a  ....C...s....t.j
+00004e10: 016a 027c 0164 0119 007c 0264 028d 02a0  .j.|.d...|.d....
+00004e20: 03a1 007d 037c 0372 a87c 036a 047c 036a  ...}.|.r.|.j.|.j
+00004e30: 0517 007d 047c 036a 0664 036b 0272 4274  ...}.|.j.d.k.rBt
+00004e40: 076a 087c 047c 0164 048d 027d 056e 587c  .j.|.|.d...}.nX|
+00004e50: 036a 0664 056b 0272 5c74 076a 097c 047c  .j.d.k.r\t.j.|.|
+00004e60: 0164 068d 027d 056e 3e7c 036a 0664 076b  .d...}.n>|.j.d.k
+00004e70: 0272 7674 076a 0a7c 047c 0164 088d 027d  .rvt.j.|.|.d...}
+00004e80: 056e 247c 036a 0664 096b 0272 8e74 076a  .n$|.j.d.k.r.t.j
+00004e90: 0b7c 0464 0a8d 017d 056e 0c74 076a 0c7c  .|.d...}.n.t.j.|
+00004ea0: 0464 0a8d 017d 0574 0da0 0e7c 056a 0fa1  .d...}.t...|.j..
+00004eb0: 017d 066e 0e64 0b64 0c64 0d69 0064 0e9c  .}.n.d.d.d.i.d..
+00004ec0: 047d 067c 0653 0029 0f4e 72b8 0000 0072  .}.|.S.).Nr....r
+00004ed0: ec00 0000 da04 504f 5354 2902 728e 0000  ......POST).r...
+00004ee0: 0072 bb00 0000 da03 4745 5429 0272 8e00  .r......GET).r..
+00004ef0: 0000 da06 7061 7261 6d73 da03 5055 5429  ....params..PUT)
+00004f00: 0272 8e00 0000 72ad 0000 00da 0644 454c  .r....r......DEL
+00004f10: 4554 4529 0172 8e00 0000 4669 d107 0000  ETE).r....Fi....
+00004f20: 751e 0000 00e4 b88d e5ad 98e5 9ca8 e5af  u...............
+00004f30: b9e6 8ea5 e58c bbe9 99a2 e4bf a1e6 81af  ................
+00004f40: efbc 8129 04da 0773 7563 6365 7373 7296  ...)...successr.
+00004f50: 0000 00da 076d 6573 7361 6765 72ad 0000  .....messager...
+00004f60: 0029 1072 eb00 0000 72bf 0000 0072 c000  .).r....r....r..
+00004f70: 0000 7269 0000 00da 0969 705f 646f 6d61  ..ri.....ip_doma
+00004f80: 696e 7292 0000 00da 0a72 6571 5f6d 6574  inr......req_met
+00004f90: 686f 64da 0872 6571 7565 7374 73da 0470  hod..requests..p
+00004fa0: 6f73 7472 c200 0000 da03 7075 74da 0664  ostr......put..d
+00004fb0: 656c 6574 65da 0570 6174 6368 72bb 0000  elete..patchr...
+00004fc0: 00da 056c 6f61 6473 da04 7465 7874 2907  ...loads..text).
+00004fd0: 722f 0000 005a 0769 6e5f 6461 7461 72ee  r/...Z.in_datar.
+00004fe0: 0000 005a 0c61 7069 5f69 6e66 6f5f 6f62  ...Z.api_info_ob
+00004ff0: 6a5a 0763 6d73 5f75 726c 72c6 0000 005a  jZ.cms_urlr....Z
+00005000: 0872 6573 5f6a 736f 6e72 1a00 0000 721a  .res_jsonr....r.
+00005010: 0000 0072 1b00 0000 da09 7772 6974 6562  ...r......writeb
+00005020: 6163 6b72 0200 0073 1e00 0000 0001 1801  ackr...s........
+00005030: 0401 0c01 0a01 1001 0a01 1001 0a01 1001  ................
+00005040: 0a01 0e02 0c01 0e02 0e01 7a11 4170 6949  ..........z.ApiI
+00005050: 6e66 6f2e 7772 6974 6562 6163 6b4e 2913  nfo.writebackN).
+00005060: 7216 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
+00005070: 0600 0000 723a 0000 0072 ed00 0000 72ee  ....r:...r....r.
+00005080: 0000 005a 0872 6571 5f6e 616d 6572 f700  ...Z.req_namer..
+00005090: 0000 7291 0000 0072 f600 0000 7292 0000  ..r....r....r...
+000050a0: 0072 1d00 0000 721e 0000 0072 1f00 0000  .r....r....r....
+000050b0: 7220 0000 0072 2100 0000 721c 0000 0072  r ...r!...r....r
+000050c0: ff00 0000 721a 0000 0072 1a00 0000 721a  ....r....r....r.
+000050d0: 0000 0072 1b00 0000 72eb 0000 005e 0200  ...r....r....^..
+000050e0: 0073 1800 0000 0801 0e01 0e01 1201 0e01  .s..............
+000050f0: 0e01 0e01 0e01 1001 1001 0e02 0e08 72eb  ..............r.
+00005100: 0000 0029 2772 bb00 0000 da02 6f73 da09  ...)'r......os..
+00005110: 646a 616e 676f 2e64 6272 0200 0000 72f8  django.dbr....r.
+00005120: 0000 00da 1a64 6a61 6e67 6f2e 636f 6e74  .....django.cont
+00005130: 7269 622e 6175 7468 2e6d 6f64 656c 7372  rib.auth.modelsr
+00005140: 0300 0000 7204 0000 00da 2264 6a61 6e67  ....r....."djang
+00005150: 6f2e 636f 6e74 7269 622e 636f 6e74 656e  o.contrib.conten
+00005160: 7474 7970 6573 2e6d 6f64 656c 7372 0500  ttypes.modelsr..
+00005170: 0000 7206 0000 00da 0b64 6a61 6e67 6f2e  ..r......django.
+00005180: 636f 6e66 7207 0000 0072 5e00 0000 da05  confr....r^.....
+00005190: 4d6f 6465 6c72 0a00 0000 7222 0000 0072  Modelr....r"...r
+000051a0: 4700 0000 724e 0000 0072 5000 0000 7264  G...rN...rP...rd
+000051b0: 0000 0072 7500 0000 7280 0000 0072 8c00  ...ru...r....r..
+000051c0: 0000 7294 0000 0072 9700 0000 729a 0000  ..r....r....r...
+000051d0: 0072 a100 0000 72c9 0000 0072 ca00 0000  .r....r....r....
+000051e0: 72cb 0000 0072 cd00 0000 72d1 0000 0072  r....r....r....r
+000051f0: d200 0000 72e4 0000 0072 e600 0000 72e7  ....r....r....r.
+00005200: 0000 0072 e800 0000 72eb 0000 0072 1a00  ...r....r....r..
+00005210: 0000 721a 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00005220: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00005230: 4000 0000 0801 0801 0c02 0801 1001 0c01  @...............
+00005240: 0c01 0c02 0406 1209 101e 101c 1014 1028  ...............(
+00005250: 104a 121e 121b 1223 100d 1019 1011 1026  .J.....#.......&
+00005260: 1011 1026 100a 100a 100a 102a 100a 100a  ...&.......*....
+00005270: 1012 1026                                ...&
```

### Comparing `base_system-0.2.7/base_system/__pycache__/serializers.cpython-39.pyc` & `base_system-0.2.8/base_system/__pycache__/serializers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/base_system/__pycache__/urls.cpython-39.pyc` & `base_system-0.2.8/base_system/__pycache__/urls.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat May  6 02:06:28 2023 UTC, .py size: 4071 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 610d 0d0a 0000 0000 24b6 5564 e70f 0000  a.......$.Ud....
+00000000: 610d 0d0a 0000 0000 fed0 6564 5b10 0000  a.........ed[...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0012 0000 0040 0000 0073 5802 0000 6400  .....@...sX...d.
+00000020: 0014 0000 0040 0000 0073 6c02 0000 6400  .....@...sl...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6401  d.l.m.Z.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6405 6406 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6401 6407 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6408 6c0c 6d0d 5a0d 6d0e 5a0e  ..d.d.l.m.Z.m.Z.
 00000080: 0100 6401 6409 6c0f 6d10 5a10 0100 6401  ..d.d.l.m.Z...d.
 00000090: 640a 6c0f 6d11 5a11 0100 6401 640b 6c0f  d.l.m.Z...d.d.l.
@@ -14,186 +14,193 @@
 000000d0: a100 6411 6412 8d03 6504 6413 6509 6a15  ..d.d...e.d.e.j.
 000000e0: 8302 6504 6414 650d 6a16 8302 6504 6415  ..e.d.e.j...e.d.
 000000f0: 650d 6a17 8302 6504 6416 6509 6a18 8302  e.j...e.d.e.j...
 00000100: 6504 6417 6509 6a19 8302 6504 6418 6509  e.d.e.j...e.d.e.
 00000110: 6a1a 8302 6504 6419 6509 6a1b 8302 6504  j...e.d.e.j...e.
 00000120: 641a 6509 6a1c 8302 6504 641b 6509 6a1d  d.e.j...e.d.e.j.
 00000130: 8302 6504 641c 6509 6a1e 8302 6504 641d  ..e.d.e.j...e.d.
-00000140: 650d 6a1f 8302 6710 5a20 6507 a021 a100  e.j...g.Z e..!..
-00000150: 5a22 6522 a013 641e 650d 6a23 a102 0100  Z"e"..d.e.j#....
-00000160: 6522 a013 641f 650d 6a24 a102 0100 6522  e"..d.e.j$....e"
-00000170: a013 6420 650d 6a25 a102 0100 6522 a013  ..d e.j%....e"..
-00000180: 6421 650d 6a26 a102 0100 6522 a013 6422  d!e.j&....e"..d"
-00000190: 6509 6a27 a102 0100 6522 a013 6423 6509  e.j'....e"..d#e.
-000001a0: 6a28 a102 0100 6522 a013 6424 6509 6a29  j(....e"..d$e.j)
-000001b0: a102 0100 6522 a013 6425 6509 6a2a a102  ....e"..d%e.j*..
-000001c0: 0100 6522 a013 6426 6509 6a2b a102 0100  ..e"..d&e.j+....
-000001d0: 6522 a013 6427 6509 6a2c a102 0100 6522  e"..d'e.j,....e"
-000001e0: a013 6428 6509 6a2d a102 0100 6522 a013  ..d(e.j-....e"..
-000001f0: 6429 6509 6a2e a102 0100 6522 a013 642a  d)e.j.....e"..d*
-00000200: 650e 6a2f a102 0100 6522 a013 642b 650e  e.j/....e"..d+e.
-00000210: 6a30 a102 0100 6522 a013 642c 650e 6a31  j0....e"..d,e.j1
-00000220: a102 0100 6522 a013 642d 650e 6a32 a102  ....e"..d-e.j2..
-00000230: 0100 6522 a013 642e 650e 6a33 a102 0100  ..e"..d.e.j3....
-00000240: 6522 a013 642f 650e 6a34 a102 0100 6522  e"..d/e.j4....e"
-00000250: a013 6430 650e 6a35 a102 0100 6522 a013  ..d0e.j5....e"..
-00000260: 6431 650e 6a36 a102 0100 6522 a013 6432  d1e.j6....e"..d2
-00000270: 650e 6a37 a102 0100 6520 6522 6a38 3700  e.j7....e e"j87.
-00000280: 5a20 6433 5300 2934 6176 0200 004d 6564  Z d3S.)4av...Med
-00000290: 6963 616c 5379 7374 656d 2055 524c 2043  icalSystem URL C
-000002a0: 6f6e 6669 6775 7261 7469 6f6e 0a0a 5468  onfiguration..Th
-000002b0: 6520 6075 726c 7061 7474 6572 6e73 6020  e `urlpatterns` 
-000002c0: 6c69 7374 2072 6f75 7465 7320 5552 4c73  list routes URLs
-000002d0: 2074 6f20 7669 6577 732e 2046 6f72 206d   to views. For m
-000002e0: 6f72 6520 696e 666f 726d 6174 696f 6e20  ore information 
-000002f0: 706c 6561 7365 2073 6565 3a0a 2020 2020  please see:.    
-00000300: 6874 7470 733a 2f2f 646f 6373 2e64 6a61  https://docs.dja
-00000310: 6e67 6f70 726f 6a65 6374 2e63 6f6d 2f65  ngoproject.com/e
-00000320: 6e2f 342e 312f 746f 7069 6373 2f68 7474  n/4.1/topics/htt
-00000330: 702f 7572 6c73 2f0a 4578 616d 706c 6573  p/urls/.Examples
-00000340: 3a0a 4675 6e63 7469 6f6e 2076 6965 7773  :.Function views
-00000350: 0a20 2020 2031 2e20 4164 6420 616e 2069  .    1. Add an i
-00000360: 6d70 6f72 743a 2020 6672 6f6d 206d 795f  mport:  from my_
-00000370: 6170 7020 696d 706f 7274 2076 6965 7773  app import views
-00000380: 0a20 2020 2032 2e20 4164 6420 6120 5552  .    2. Add a UR
-00000390: 4c20 746f 2075 726c 7061 7474 6572 6e73  L to urlpatterns
-000003a0: 3a20 2070 6174 6828 2727 2c20 7669 6577  :  path('', view
-000003b0: 732e 686f 6d65 2c20 6e61 6d65 3d27 686f  s.home, name='ho
-000003c0: 6d65 2729 0a43 6c61 7373 2d62 6173 6564  me').Class-based
-000003d0: 2076 6965 7773 0a20 2020 2031 2e20 4164   views.    1. Ad
-000003e0: 6420 616e 2069 6d70 6f72 743a 2020 6672  d an import:  fr
-000003f0: 6f6d 206f 7468 6572 5f61 7070 2e76 6965  om other_app.vie
-00000400: 7773 2069 6d70 6f72 7420 486f 6d65 0a20  ws import Home. 
-00000410: 2020 2032 2e20 4164 6420 6120 5552 4c20     2. Add a URL 
-00000420: 746f 2075 726c 7061 7474 6572 6e73 3a20  to urlpatterns: 
-00000430: 2070 6174 6828 2727 2c20 486f 6d65 2e61   path('', Home.a
-00000440: 735f 7669 6577 2829 2c20 6e61 6d65 3d27  s_view(), name='
-00000450: 686f 6d65 2729 0a49 6e63 6c75 6469 6e67  home').Including
-00000460: 2061 6e6f 7468 6572 2055 524c 636f 6e66   another URLconf
-00000470: 0a20 2020 2031 2e20 496d 706f 7274 2074  .    1. Import t
-00000480: 6865 2069 6e63 6c75 6465 2829 2066 756e  he include() fun
-00000490: 6374 696f 6e3a 2066 726f 6d20 646a 616e  ction: from djan
-000004a0: 676f 2e75 726c 7320 696d 706f 7274 2069  go.urls import i
-000004b0: 6e63 6c75 6465 2c20 7061 7468 0a20 2020  nclude, path.   
-000004c0: 2032 2e20 4164 6420 6120 5552 4c20 746f   2. Add a URL to
-000004d0: 2075 726c 7061 7474 6572 6e73 3a20 2070   urlpatterns:  p
-000004e0: 6174 6828 2762 6c6f 672f 272c 2069 6e63  ath('blog/', inc
-000004f0: 6c75 6465 2827 626c 6f67 2e75 726c 7327  lude('blog.urls'
-00000500: 2929 0ae9 0000 0000 2901 da05 6164 6d69  ))......)...admi
-00000510: 6e29 02da 0470 6174 68da 0769 6e63 6c75  n)...path..inclu
-00000520: 6465 2901 da07 726f 7574 6572 73e9 0100  de)...routers...
-00000530: 0000 2901 da05 7669 6577 7329 01da 0f50  ..)...views)...P
-00000540: 6572 6d69 7373 696f 6e73 5669 6577 2902  ermissionsView).
-00000550: da08 7669 6577 7365 7473 da0e 6578 706f  ..viewsets..expo
-00000560: 7274 5f76 6965 7773 6574 2901 da10 6f62  rt_viewset)...ob
-00000570: 7461 696e 5f6a 7774 5f74 6f6b 656e 2901  tain_jwt_token).
-00000580: da11 7265 6672 6573 685f 6a77 745f 746f  ..refresh_jwt_to
-00000590: 6b65 6e29 01da 1076 6572 6966 795f 6a77  ken)...verify_jw
-000005a0: 745f 746f 6b65 6e7a 0972 6567 6973 7465  t_tokenz.registe
-000005b0: 722f 7a06 6c6f 6769 6e2f 7a0e 746f 6b65  r/z.login/z.toke
-000005c0: 6e2f 7265 6672 6573 682f 7a07 7665 7269  n/refresh/z.veri
-000005d0: 6679 2f7a 0c70 6572 6d69 7373 696f 6e73  fy/z.permissions
-000005e0: 2fda 0b70 6572 6d69 7373 696f 6e73 2901  /..permissions).
-000005f0: da04 6e61 6d65 7a10 6368 616e 6765 2d70  ..namez.change-p
-00000600: 6173 7377 6f72 642f 7a10 616c 6c2d 7065  assword/z.all-pe
-00000610: 726d 6973 7369 6f6e 732f 7a09 6f77 6e2d  rmissions/z.own-
-00000620: 6d65 6e75 2f7a 1669 6d70 6f72 745f 706f  menu/z.import_po
-00000630: 7369 7469 6f6e 5f74 6974 6c65 2f7a 0e69  sition_title/z.i
-00000640: 6d70 6f72 745f 6f66 6669 6365 2f7a 0e69  mport_office/z.i
-00000650: 6d70 6f72 745f 646f 6374 6f72 2f7a 0f69  mport_doctor/z.i
-00000660: 6d70 6f72 745f 696e 735f 6469 632f 7a0f  mport_ins_dic/z.
-00000670: 696d 706f 7274 5f65 7861 5f64 6963 2f7a  import_exa_dic/z
-00000680: 1069 6d70 6f72 745f 6472 7567 5f64 6972  .import_drug_dir
-00000690: 2f7a 1569 6d70 6f72 745f 7068 6172 6d61  /z.import_pharma
-000006a0: 6379 5f64 7275 672f 7a11 6d65 6e75 5f70  cy_drug/z.menu_p
-000006b0: 6572 6d69 7373 696f 6e73 2f5a 0968 6f73  ermissions/Z.hos
-000006c0: 7069 7461 6c73 5a07 6f66 6669 6365 73da  pitalsZ.offices.
-000006d0: 0764 6f63 746f 7273 da06 6772 6f75 7073  .doctors..groups
-000006e0: da05 7573 6572 735a 0761 7069 6e66 6f73  ..usersZ.apinfos
-000006f0: 5a0f 696e 7370 6563 7469 6f6e 7479 7065  Z.inspectiontype
-00000700: 735a 0769 6e73 5f64 6963 5a10 6578 616d  sZ.ins_dicZ.exam
-00000710: 696e 6174 696f 6e74 7970 6573 5a07 6578  inationtypesZ.ex
-00000720: 615f 6469 635a 1370 6861 726d 6163 795f  a_dicZ.pharmacy_
-00000730: 6d61 6e61 6765 6d65 6e74 5a10 6472 7567  managementZ.drug
-00000740: 5f64 6972 6563 746f 7269 6573 5a0f 6578  _directoriesZ.ex
-00000750: 706f 7274 5f68 6f73 7069 7461 6c5a 0d65  port_hospitalZ.e
-00000760: 7870 6f72 745f 6f66 6669 6365 5a0c 6578  xport_officeZ.ex
-00000770: 706f 7274 5f67 726f 7570 5a0d 6578 706f  port_groupZ.expo
-00000780: 7274 5f64 6f63 746f 725a 0b65 7870 6f72  rt_doctorZ.expor
-00000790: 745f 7573 6572 5a0e 6578 706f 7274 5f69  t_userZ.export_i
-000007a0: 6e73 5f64 6963 5a0e 6578 706f 7274 5f65  ns_dicZ.export_e
-000007b0: 7861 5f64 6963 5a15 6578 706f 7274 5f64  xa_dicZ.export_d
-000007c0: 7275 675f 6469 7265 6374 6f72 795a 1465  rug_directoryZ.e
-000007d0: 7870 6f72 745f 7068 6172 6d61 6379 5f64  xport_pharmacy_d
-000007e0: 7275 674e 2939 da07 5f5f 646f 635f 5fda  rugN)9..__doc__.
-000007f0: 0e64 6a61 6e67 6f2e 636f 6e74 7269 6272  .django.contribr
-00000800: 0200 0000 da0b 646a 616e 676f 2e75 726c  ......django.url
-00000810: 7372 0300 0000 7204 0000 00da 0e72 6573  sr....r......res
-00000820: 745f 6672 616d 6577 6f72 6b72 0500 0000  t_frameworkr....
-00000830: da00 7207 0000 00da 1162 6173 655f 7379  ..r......base_sy
-00000840: 7374 656d 2e76 6965 7773 7208 0000 00da  stem.viewsr.....
-00000850: 0b62 6173 655f 7379 7374 656d 7209 0000  .base_systemr...
-00000860: 0072 0a00 0000 5a18 7265 7374 5f66 7261  .r....Z.rest_fra
-00000870: 6d65 776f 726b 5f6a 7774 2e76 6965 7773  mework_jwt.views
-00000880: 720b 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
-00000890: 0872 6567 6973 7465 72da 0761 735f 7669  .register..as_vi
-000008a0: 6577 5a0f 6368 616e 6765 5f70 6173 7377  ewZ.change_passw
-000008b0: 6f72 645a 0f61 6c6c 5f70 6572 6d69 7373  ordZ.all_permiss
-000008c0: 696f 6e73 5a13 6765 745f 6f77 6e5f 7065  ionsZ.get_own_pe
-000008d0: 726d 6973 7369 6f6e 735a 1569 6d70 6f72  rmissionsZ.impor
-000008e0: 745f 706f 7369 7469 6f6e 5f74 6974 6c65  t_position_title
-000008f0: 5a0d 696d 706f 7274 5f6f 6666 6963 655a  Z.import_officeZ
-00000900: 0d69 6d70 6f72 745f 646f 6374 6f72 5a1e  .import_doctorZ.
-00000910: 696d 706f 7274 5f69 6e73 7065 6374 696f  import_inspectio
-00000920: 6e5f 6469 6374 696f 6e61 7269 6573 5a1f  n_dictionariesZ.
-00000930: 696d 706f 7274 5f65 7861 6d69 6e61 7469  import_examinati
-00000940: 6f6e 5f64 6963 7469 6f6e 6172 6965 735a  on_dictionariesZ
-00000950: 1569 6d70 6f72 745f 6472 7567 5f64 6972  .import_drug_dir
-00000960: 6563 746f 7279 5a14 696d 706f 7274 5f70  ectoryZ.import_p
-00000970: 6861 726d 6163 795f 6472 7567 5a10 6d65  harmacy_drugZ.me
-00000980: 6e75 5f70 6572 6d69 7373 696f 6e73 da0b  nu_permissions..
-00000990: 7572 6c70 6174 7465 726e 735a 0d44 6566  urlpatternsZ.Def
-000009a0: 6175 6c74 526f 7574 6572 da06 726f 7574  aultRouter..rout
-000009b0: 6572 5a0f 486f 7370 6974 616c 5669 6577  erZ.HospitalView
-000009c0: 5365 745a 0d4f 6666 6963 6556 6965 7753  SetZ.OfficeViewS
-000009d0: 6574 5a0d 446f 6374 6f72 5669 6577 5365  etZ.DoctorViewSe
-000009e0: 745a 0c47 726f 7570 5669 6577 5365 745a  tZ.GroupViewSetZ
-000009f0: 0b55 7365 7256 6965 7753 6574 5a0e 4170  .UserViewSetZ.Ap
-00000a00: 6949 6e66 6f56 6965 7753 6574 5a15 496e  iInfoViewSetZ.In
-00000a10: 7370 6563 7469 6f6e 5479 7065 5669 6577  spectionTypeView
-00000a20: 5365 745a 1d49 6e73 7065 6374 696f 6e44  SetZ.InspectionD
-00000a30: 6963 7469 6f6e 6172 6965 7356 6965 7753  ictionariesViewS
-00000a40: 6574 5a16 4578 616d 696e 6174 696f 6e54  etZ.ExaminationT
-00000a50: 7970 6556 6965 7753 6574 5a1e 4578 616d  ypeViewSetZ.Exam
-00000a60: 696e 6174 696f 6e44 6963 7469 6f6e 6172  inationDictionar
-00000a70: 6965 7356 6965 7753 6574 5a19 5068 6172  iesViewSetZ.Phar
-00000a80: 6d61 6379 4d61 6e61 6765 6d65 6e74 5669  macyManagementVi
-00000a90: 6577 5365 745a 1444 7275 6744 6972 6563  ewSetZ.DrugDirec
-00000aa0: 746f 7279 5669 6577 5365 745a 1948 6f73  toryViewSetZ.Hos
-00000ab0: 7069 7461 6c49 6e66 6f45 7870 6f72 7456  pitalInfoExportV
-00000ac0: 6965 7753 6574 5a17 4f66 6669 6365 496e  iewSetZ.OfficeIn
-00000ad0: 666f 4578 706f 7274 5669 6577 5365 745a  foExportViewSetZ
-00000ae0: 1247 726f 7570 4578 706f 7274 5669 6577  .GroupExportView
-00000af0: 5365 745a 1744 6f63 746f 7249 6e66 6f45  SetZ.DoctorInfoE
-00000b00: 7870 6f72 7456 6965 7753 6574 5a15 5573  xportViewSetZ.Us
-00000b10: 6572 496e 666f 4578 706f 7274 5669 6577  erInfoExportView
-00000b20: 5365 745a 2749 6e73 7065 6374 696f 6e44  SetZ'InspectionD
-00000b30: 6963 7469 6f6e 6172 6965 7349 6e66 6f45  ictionariesInfoE
-00000b40: 7870 6f72 7456 6965 7753 6574 5a28 4578  xportViewSetZ(Ex
-00000b50: 616d 696e 6174 696f 6e44 6963 7469 6f6e  aminationDiction
-00000b60: 6172 6965 7349 6e66 6f45 7870 6f72 7456  ariesInfoExportV
-00000b70: 6965 7753 6574 5a1a 4472 7567 4469 7265  iewSetZ.DrugDire
-00000b80: 6374 6f72 7945 7870 6f72 7456 6965 7753  ctoryExportViewS
-00000b90: 6574 5a19 5068 6172 6d61 6379 4472 7567  etZ.PharmacyDrug
-00000ba0: 4578 706f 7274 5669 6577 5365 74da 0475  ExportViewSet..u
-00000bb0: 726c 73a9 0072 1f00 0000 721f 0000 00fa  rls..r....r.....
-00000bc0: 352f 686f 6d65 2f6c 7968 2f77 6f72 6b2f  5/home/lyh/work/
-00000bd0: 4261 7365 4675 6e63 7469 6f6e 4d6f 6475  BaseFunctionModu
-00000be0: 6c65 2f62 6173 655f 7379 7374 656d 2f75  le/base_system/u
-00000bf0: 726c 732e 7079 da08 3c6d 6f64 756c 653e  rls.py..<module>
-00000c00: 0100 0000 7362 0000 0004 0f0c 0110 010c  ....sb..........
-00000c10: 020c 010c 0110 010c 010c 010c 040a 0108  ................
-00000c20: 0108 0108 0110 010a 010a 010a 010a 010a  ................
-00000c30: 010a 010a 010a 010a 010a 010a ef04 1408  ................
-00000c40: 020e 010e 010e 010e 010e 010e 020e 010e  ................
-00000c50: 010e 010e 010e 010e 020e 010e 010e 010e  ................
-00000c60: 010e 010e 010e 010e 010e 02              ...........
+00000140: 650d 6a1f 8302 6504 641e 6509 6a20 8302  e.j...e.d.e.j ..
+00000150: 6504 641f 6509 6a21 8302 6712 5a22 6507  e.d.e.j!..g.Z"e.
+00000160: a023 a100 5a24 6524 a013 6420 650d 6a25  .#..Z$e$..d e.j%
+00000170: a102 0100 6524 a013 6421 650d 6a26 a102  ....e$..d!e.j&..
+00000180: 0100 6524 a013 6422 650d 6a27 a102 0100  ..e$..d"e.j'....
+00000190: 6524 a013 6423 650d 6a28 a102 0100 6524  e$..d#e.j(....e$
+000001a0: a013 6424 6509 6a29 a102 0100 6524 a013  ..d$e.j)....e$..
+000001b0: 6425 6509 6a2a a102 0100 6524 a013 6426  d%e.j*....e$..d&
+000001c0: 6509 6a2b a102 0100 6524 a013 6427 6509  e.j+....e$..d'e.
+000001d0: 6a2c a102 0100 6524 a013 6428 6509 6a2d  j,....e$..d(e.j-
+000001e0: a102 0100 6524 a013 6429 6509 6a2e a102  ....e$..d)e.j...
+000001f0: 0100 6524 a013 642a 6509 6a2f a102 0100  ..e$..d*e.j/....
+00000200: 6524 a013 642b 6509 6a30 a102 0100 6524  e$..d+e.j0....e$
+00000210: a013 642c 650e 6a31 a102 0100 6524 a013  ..d,e.j1....e$..
+00000220: 642d 650e 6a32 a102 0100 6524 a013 642e  d-e.j2....e$..d.
+00000230: 650e 6a33 a102 0100 6524 a013 642f 650e  e.j3....e$..d/e.
+00000240: 6a34 a102 0100 6524 a013 6430 650e 6a35  j4....e$..d0e.j5
+00000250: a102 0100 6524 a013 6431 650e 6a36 a102  ....e$..d1e.j6..
+00000260: 0100 6524 a013 6432 650e 6a37 a102 0100  ..e$..d2e.j7....
+00000270: 6524 a013 6433 650e 6a38 a102 0100 6524  e$..d3e.j8....e$
+00000280: a013 6434 650e 6a39 a102 0100 6522 6524  ..d4e.j9....e"e$
+00000290: 6a3a 3700 5a22 6435 5300 2936 6176 0200  j:7.Z"d5S.)6av..
+000002a0: 004d 6564 6963 616c 5379 7374 656d 2055  .MedicalSystem U
+000002b0: 524c 2043 6f6e 6669 6775 7261 7469 6f6e  RL Configuration
+000002c0: 0a0a 5468 6520 6075 726c 7061 7474 6572  ..The `urlpatter
+000002d0: 6e73 6020 6c69 7374 2072 6f75 7465 7320  ns` list routes 
+000002e0: 5552 4c73 2074 6f20 7669 6577 732e 2046  URLs to views. F
+000002f0: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
+00000300: 696f 6e20 706c 6561 7365 2073 6565 3a0a  ion please see:.
+00000310: 2020 2020 6874 7470 733a 2f2f 646f 6373      https://docs
+00000320: 2e64 6a61 6e67 6f70 726f 6a65 6374 2e63  .djangoproject.c
+00000330: 6f6d 2f65 6e2f 342e 312f 746f 7069 6373  om/en/4.1/topics
+00000340: 2f68 7474 702f 7572 6c73 2f0a 4578 616d  /http/urls/.Exam
+00000350: 706c 6573 3a0a 4675 6e63 7469 6f6e 2076  ples:.Function v
+00000360: 6965 7773 0a20 2020 2031 2e20 4164 6420  iews.    1. Add 
+00000370: 616e 2069 6d70 6f72 743a 2020 6672 6f6d  an import:  from
+00000380: 206d 795f 6170 7020 696d 706f 7274 2076   my_app import v
+00000390: 6965 7773 0a20 2020 2032 2e20 4164 6420  iews.    2. Add 
+000003a0: 6120 5552 4c20 746f 2075 726c 7061 7474  a URL to urlpatt
+000003b0: 6572 6e73 3a20 2070 6174 6828 2727 2c20  erns:  path('', 
+000003c0: 7669 6577 732e 686f 6d65 2c20 6e61 6d65  views.home, name
+000003d0: 3d27 686f 6d65 2729 0a43 6c61 7373 2d62  ='home').Class-b
+000003e0: 6173 6564 2076 6965 7773 0a20 2020 2031  ased views.    1
+000003f0: 2e20 4164 6420 616e 2069 6d70 6f72 743a  . Add an import:
+00000400: 2020 6672 6f6d 206f 7468 6572 5f61 7070    from other_app
+00000410: 2e76 6965 7773 2069 6d70 6f72 7420 486f  .views import Ho
+00000420: 6d65 0a20 2020 2032 2e20 4164 6420 6120  me.    2. Add a 
+00000430: 5552 4c20 746f 2075 726c 7061 7474 6572  URL to urlpatter
+00000440: 6e73 3a20 2070 6174 6828 2727 2c20 486f  ns:  path('', Ho
+00000450: 6d65 2e61 735f 7669 6577 2829 2c20 6e61  me.as_view(), na
+00000460: 6d65 3d27 686f 6d65 2729 0a49 6e63 6c75  me='home').Inclu
+00000470: 6469 6e67 2061 6e6f 7468 6572 2055 524c  ding another URL
+00000480: 636f 6e66 0a20 2020 2031 2e20 496d 706f  conf.    1. Impo
+00000490: 7274 2074 6865 2069 6e63 6c75 6465 2829  rt the include()
+000004a0: 2066 756e 6374 696f 6e3a 2066 726f 6d20   function: from 
+000004b0: 646a 616e 676f 2e75 726c 7320 696d 706f  django.urls impo
+000004c0: 7274 2069 6e63 6c75 6465 2c20 7061 7468  rt include, path
+000004d0: 0a20 2020 2032 2e20 4164 6420 6120 5552  .    2. Add a UR
+000004e0: 4c20 746f 2075 726c 7061 7474 6572 6e73  L to urlpatterns
+000004f0: 3a20 2070 6174 6828 2762 6c6f 672f 272c  :  path('blog/',
+00000500: 2069 6e63 6c75 6465 2827 626c 6f67 2e75   include('blog.u
+00000510: 726c 7327 2929 0ae9 0000 0000 2901 da05  rls'))......)...
+00000520: 6164 6d69 6e29 02da 0470 6174 68da 0769  admin)...path..i
+00000530: 6e63 6c75 6465 2901 da07 726f 7574 6572  nclude)...router
+00000540: 73e9 0100 0000 2901 da05 7669 6577 7329  s.....)...views)
+00000550: 01da 0f50 6572 6d69 7373 696f 6e73 5669  ...PermissionsVi
+00000560: 6577 2902 da08 7669 6577 7365 7473 da0e  ew)...viewsets..
+00000570: 6578 706f 7274 5f76 6965 7773 6574 2901  export_viewset).
+00000580: da10 6f62 7461 696e 5f6a 7774 5f74 6f6b  ..obtain_jwt_tok
+00000590: 656e 2901 da11 7265 6672 6573 685f 6a77  en)...refresh_jw
+000005a0: 745f 746f 6b65 6e29 01da 1076 6572 6966  t_token)...verif
+000005b0: 795f 6a77 745f 746f 6b65 6e7a 0972 6567  y_jwt_tokenz.reg
+000005c0: 6973 7465 722f 7a06 6c6f 6769 6e2f 7a0e  ister/z.login/z.
+000005d0: 746f 6b65 6e2f 7265 6672 6573 682f 7a07  token/refresh/z.
+000005e0: 7665 7269 6679 2f7a 0c70 6572 6d69 7373  verify/z.permiss
+000005f0: 696f 6e73 2fda 0b70 6572 6d69 7373 696f  ions/..permissio
+00000600: 6e73 2901 da04 6e61 6d65 7a10 6368 616e  ns)...namez.chan
+00000610: 6765 2d70 6173 7377 6f72 642f 7a10 616c  ge-password/z.al
+00000620: 6c2d 7065 726d 6973 7369 6f6e 732f 7a09  l-permissions/z.
+00000630: 6f77 6e2d 6d65 6e75 2f7a 1669 6d70 6f72  own-menu/z.impor
+00000640: 745f 706f 7369 7469 6f6e 5f74 6974 6c65  t_position_title
+00000650: 2f7a 0e69 6d70 6f72 745f 6f66 6669 6365  /z.import_office
+00000660: 2f7a 0e69 6d70 6f72 745f 646f 6374 6f72  /z.import_doctor
+00000670: 2f7a 0f69 6d70 6f72 745f 696e 735f 6469  /z.import_ins_di
+00000680: 632f 7a0f 696d 706f 7274 5f65 7861 5f64  c/z.import_exa_d
+00000690: 6963 2f7a 1069 6d70 6f72 745f 6472 7567  ic/z.import_drug
+000006a0: 5f64 6972 2f7a 1569 6d70 6f72 745f 7068  _dir/z.import_ph
+000006b0: 6172 6d61 6379 5f64 7275 672f 7a11 6d65  armacy_drug/z.me
+000006c0: 6e75 5f70 6572 6d69 7373 696f 6e73 2f7a  nu_permissions/z
+000006d0: 1269 6e73 7065 6374 696f 6e2f 696d 706f  .inspection/impo
+000006e0: 7274 2f7a 1365 7861 6d69 6e61 7469 6f6e  rt/z.examination
+000006f0: 2f69 6d70 6f72 742f 5a09 686f 7370 6974  /import/Z.hospit
+00000700: 616c 735a 076f 6666 6963 6573 da07 646f  alsZ.offices..do
+00000710: 6374 6f72 73da 0667 726f 7570 73da 0575  ctors..groups..u
+00000720: 7365 7273 5a07 6170 696e 666f 735a 0f69  sersZ.apinfosZ.i
+00000730: 6e73 7065 6374 696f 6e74 7970 6573 5a07  nspectiontypesZ.
+00000740: 696e 735f 6469 635a 1065 7861 6d69 6e61  ins_dicZ.examina
+00000750: 7469 6f6e 7479 7065 735a 0765 7861 5f64  tiontypesZ.exa_d
+00000760: 6963 5a13 7068 6172 6d61 6379 5f6d 616e  icZ.pharmacy_man
+00000770: 6167 656d 656e 745a 1064 7275 675f 6469  agementZ.drug_di
+00000780: 7265 6374 6f72 6965 735a 0f65 7870 6f72  rectoriesZ.expor
+00000790: 745f 686f 7370 6974 616c 5a0d 6578 706f  t_hospitalZ.expo
+000007a0: 7274 5f6f 6666 6963 655a 0c65 7870 6f72  rt_officeZ.expor
+000007b0: 745f 6772 6f75 705a 0d65 7870 6f72 745f  t_groupZ.export_
+000007c0: 646f 6374 6f72 5a0b 6578 706f 7274 5f75  doctorZ.export_u
+000007d0: 7365 725a 0e65 7870 6f72 745f 696e 735f  serZ.export_ins_
+000007e0: 6469 635a 0e65 7870 6f72 745f 6578 615f  dicZ.export_exa_
+000007f0: 6469 635a 1565 7870 6f72 745f 6472 7567  dicZ.export_drug
+00000800: 5f64 6972 6563 746f 7279 5a14 6578 706f  _directoryZ.expo
+00000810: 7274 5f70 6861 726d 6163 795f 6472 7567  rt_pharmacy_drug
+00000820: 4e29 3bda 075f 5f64 6f63 5f5f da0e 646a  N);..__doc__..dj
+00000830: 616e 676f 2e63 6f6e 7472 6962 7202 0000  ango.contribr...
+00000840: 00da 0b64 6a61 6e67 6f2e 7572 6c73 7203  ...django.urlsr.
+00000850: 0000 0072 0400 0000 da0e 7265 7374 5f66  ...r......rest_f
+00000860: 7261 6d65 776f 726b 7205 0000 00da 0072  rameworkr......r
+00000870: 0700 0000 da11 6261 7365 5f73 7973 7465  ......base_syste
+00000880: 6d2e 7669 6577 7372 0800 0000 da0b 6261  m.viewsr......ba
+00000890: 7365 5f73 7973 7465 6d72 0900 0000 720a  se_systemr....r.
+000008a0: 0000 005a 1872 6573 745f 6672 616d 6577  ...Z.rest_framew
+000008b0: 6f72 6b5f 6a77 742e 7669 6577 7372 0b00  ork_jwt.viewsr..
+000008c0: 0000 720c 0000 0072 0d00 0000 da08 7265  ..r....r......re
+000008d0: 6769 7374 6572 da07 6173 5f76 6965 775a  gister..as_viewZ
+000008e0: 0f63 6861 6e67 655f 7061 7373 776f 7264  .change_password
+000008f0: 5a0f 616c 6c5f 7065 726d 6973 7369 6f6e  Z.all_permission
+00000900: 735a 1367 6574 5f6f 776e 5f70 6572 6d69  sZ.get_own_permi
+00000910: 7373 696f 6e73 5a15 696d 706f 7274 5f70  ssionsZ.import_p
+00000920: 6f73 6974 696f 6e5f 7469 746c 655a 0d69  osition_titleZ.i
+00000930: 6d70 6f72 745f 6f66 6669 6365 5a0d 696d  mport_officeZ.im
+00000940: 706f 7274 5f64 6f63 746f 725a 1e69 6d70  port_doctorZ.imp
+00000950: 6f72 745f 696e 7370 6563 7469 6f6e 5f64  ort_inspection_d
+00000960: 6963 7469 6f6e 6172 6965 735a 1f69 6d70  ictionariesZ.imp
+00000970: 6f72 745f 6578 616d 696e 6174 696f 6e5f  ort_examination_
+00000980: 6469 6374 696f 6e61 7269 6573 5a15 696d  dictionariesZ.im
+00000990: 706f 7274 5f64 7275 675f 6469 7265 6374  port_drug_direct
+000009a0: 6f72 795a 1469 6d70 6f72 745f 7068 6172  oryZ.import_phar
+000009b0: 6d61 6379 5f64 7275 675a 106d 656e 755f  macy_drugZ.menu_
+000009c0: 7065 726d 6973 7369 6f6e 735a 1169 6e73  permissionsZ.ins
+000009d0: 7065 6374 696f 6e5f 696d 706f 7274 5a12  pection_importZ.
+000009e0: 6578 616d 696e 6174 696f 6e5f 696d 706f  examination_impo
+000009f0: 7274 da0b 7572 6c70 6174 7465 726e 735a  rt..urlpatternsZ
+00000a00: 0d44 6566 6175 6c74 526f 7574 6572 da06  .DefaultRouter..
+00000a10: 726f 7574 6572 5a0f 486f 7370 6974 616c  routerZ.Hospital
+00000a20: 5669 6577 5365 745a 0d4f 6666 6963 6556  ViewSetZ.OfficeV
+00000a30: 6965 7753 6574 5a0d 446f 6374 6f72 5669  iewSetZ.DoctorVi
+00000a40: 6577 5365 745a 0c47 726f 7570 5669 6577  ewSetZ.GroupView
+00000a50: 5365 745a 0b55 7365 7256 6965 7753 6574  SetZ.UserViewSet
+00000a60: 5a0e 4170 6949 6e66 6f56 6965 7753 6574  Z.ApiInfoViewSet
+00000a70: 5a15 496e 7370 6563 7469 6f6e 5479 7065  Z.InspectionType
+00000a80: 5669 6577 5365 745a 1d49 6e73 7065 6374  ViewSetZ.Inspect
+00000a90: 696f 6e44 6963 7469 6f6e 6172 6965 7356  ionDictionariesV
+00000aa0: 6965 7753 6574 5a16 4578 616d 696e 6174  iewSetZ.Examinat
+00000ab0: 696f 6e54 7970 6556 6965 7753 6574 5a1e  ionTypeViewSetZ.
+00000ac0: 4578 616d 696e 6174 696f 6e44 6963 7469  ExaminationDicti
+00000ad0: 6f6e 6172 6965 7356 6965 7753 6574 5a19  onariesViewSetZ.
+00000ae0: 5068 6172 6d61 6379 4d61 6e61 6765 6d65  PharmacyManageme
+00000af0: 6e74 5669 6577 5365 745a 1444 7275 6744  ntViewSetZ.DrugD
+00000b00: 6972 6563 746f 7279 5669 6577 5365 745a  irectoryViewSetZ
+00000b10: 1948 6f73 7069 7461 6c49 6e66 6f45 7870  .HospitalInfoExp
+00000b20: 6f72 7456 6965 7753 6574 5a17 4f66 6669  ortViewSetZ.Offi
+00000b30: 6365 496e 666f 4578 706f 7274 5669 6577  ceInfoExportView
+00000b40: 5365 745a 1247 726f 7570 4578 706f 7274  SetZ.GroupExport
+00000b50: 5669 6577 5365 745a 1744 6f63 746f 7249  ViewSetZ.DoctorI
+00000b60: 6e66 6f45 7870 6f72 7456 6965 7753 6574  nfoExportViewSet
+00000b70: 5a15 5573 6572 496e 666f 4578 706f 7274  Z.UserInfoExport
+00000b80: 5669 6577 5365 745a 2749 6e73 7065 6374  ViewSetZ'Inspect
+00000b90: 696f 6e44 6963 7469 6f6e 6172 6965 7349  ionDictionariesI
+00000ba0: 6e66 6f45 7870 6f72 7456 6965 7753 6574  nfoExportViewSet
+00000bb0: 5a28 4578 616d 696e 6174 696f 6e44 6963  Z(ExaminationDic
+00000bc0: 7469 6f6e 6172 6965 7349 6e66 6f45 7870  tionariesInfoExp
+00000bd0: 6f72 7456 6965 7753 6574 5a1a 4472 7567  ortViewSetZ.Drug
+00000be0: 4469 7265 6374 6f72 7945 7870 6f72 7456  DirectoryExportV
+00000bf0: 6965 7753 6574 5a19 5068 6172 6d61 6379  iewSetZ.Pharmacy
+00000c00: 4472 7567 4578 706f 7274 5669 6577 5365  DrugExportViewSe
+00000c10: 74da 0475 726c 73a9 0072 1f00 0000 721f  t..urls..r....r.
+00000c20: 0000 00fa 352f 686f 6d65 2f6c 7968 2f77  ....5/home/lyh/w
+00000c30: 6f72 6b2f 4261 7365 4675 6e63 7469 6f6e  ork/BaseFunction
+00000c40: 4d6f 6475 6c65 2f62 6173 655f 7379 7374  Module/base_syst
+00000c50: 656d 2f75 726c 732e 7079 da08 3c6d 6f64  em/urls.py..<mod
+00000c60: 756c 653e 0100 0000 7366 0000 0004 0f0c  ule>....sf......
+00000c70: 0110 010c 020c 010c 0110 010c 010c 010c  ................
+00000c80: 040a 0108 0108 0108 0110 010a 010a 010a  ................
+00000c90: 010a 010a 010a 010a 010a 010a 010a 010a  ................
+00000ca0: 020a 010a ec04 1708 020e 010e 010e 010e  ................
+00000cb0: 010e 010e 020e 010e 010e 010e 010e 010e  ................
+00000cc0: 020e 010e 010e 010e 010e 010e 010e 010e  ................
+00000cd0: 010e 02                                  ...
```

### Comparing `base_system-0.2.7/base_system/__pycache__/views.cpython-39.pyc` & `base_system-0.2.8/base_system/__pycache__/views.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue May  9 03:12:22 2023 UTC, .py size: 58056 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 610d 0d0a 0000 0000 16ba 5964 c8e2 0000  a.........Yd....
+00000000: 610d 0d0a 0000 0000 fed0 6564 31dd 0000  a.........ed1...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 1003 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 2003 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6402 6c06 6d07 5a07 0100 6400 6403 6c08  d.l.m.Z...d.d.l.
 00000070: 6d09 5a09 0100 6400 6404 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000080: 0100 6400 6405 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
 00000090: 6406 6c0e 6d0f 5a0f 6d10 5a10 0100 6400  d.l.m.Z.m.Z...d.
@@ -32,1450 +32,1471 @@
 000001f0: 5a4c 4700 641c 641d 8400 641d 8302 5a4d  ZLG.d.d...d...ZM
 00000200: 650d 6a4e 641e 641f 8400 8301 5a4f 4700  e.jNd.d.....ZOG.
 00000210: 6420 6421 8400 6421 6512 6a50 8303 5a51  d d!..d!e.jP..ZQ
 00000220: 4700 6422 6423 8400 6423 6523 8303 5a52  G.d"d#..d#e#..ZR
 00000230: 4700 6424 6425 8400 6425 6523 8303 5a53  G.d$d%..d%e#..ZS
 00000240: 4700 6426 6427 8400 6427 6512 6a50 8303  G.d&d'..d'e.jP..
 00000250: 5a54 4700 6428 6429 8400 6429 6523 8303  ZTG.d(d)..d)e#..
-00000260: 5a55 4700 642a 642b 8400 642b 6523 8303  ZUG.d*d+..d+e#..
-00000270: 5a56 4700 642c 642d 8400 642d 6512 6a50  ZVG.d,d-..d-e.jP
-00000280: 8303 5a57 4700 642e 642f 8400 642f 6523  ..ZWG.d.d/..d/e#
-00000290: 8303 5a58 4700 6430 6431 8400 6431 6523  ..ZXG.d0d1..d1e#
-000002a0: 8303 5a59 650d 6a4e 6432 6433 8400 8301  ..ZYe.jNd2d3....
-000002b0: 5a5a 650d 6a4e 6434 6435 8400 8301 5a5b  ZZe.jNd4d5....Z[
-000002c0: 6436 6437 8400 5a5c 4700 6438 6439 8400  d6d7..Z\G.d8d9..
-000002d0: 6439 6512 6a50 8303 5a5d 643a 643b 8400  d9e.jP..Z]d:d;..
-000002e0: 5a5e 4700 643c 643d 8400 643d 6523 8303  Z^G.d<d=..d=e#..
-000002f0: 5a5f 4700 643e 643f 8400 643f 6523 8303  Z_G.d>d?..d?e#..
-00000300: 5a60 650d 6a4e 6440 6441 8400 8301 5a61  Z`e.jNd@dA....Za
-00000310: 650d 6a4e 6442 6443 8400 8301 5a62 650d  e.jNdBdC....Zbe.
-00000320: 6a4e 6444 6445 8400 8301 5a63 650d 6a4e  jNdDdE....Zce.jN
-00000330: 6446 6447 8400 8301 5a64 6401 5300 2948  dFdG....Zdd.S.)H
-00000340: e900 0000 004e 2901 da0c 4d6f 6465 6c42  .....N)...ModelB
-00000350: 6163 6b65 6e64 2901 da0d 6d61 6b65 5f70  ackend)...make_p
-00000360: 6173 7377 6f72 6429 01da 0a50 6572 6d69  assword)...Permi
-00000370: 7373 696f 6e29 01da 0b74 7261 6e73 6163  ssion)...transac
-00000380: 7469 6f6e 2902 da0c 4a73 6f6e 5265 7370  tion)...JsonResp
-00000390: 6f6e 7365 da0c 4874 7470 5265 7370 6f6e  onse..HttpRespon
-000003a0: 7365 2901 da0d 584c 5358 4669 6c65 4d69  se)...XLSXFileMi
-000003b0: 7869 6e29 01da 0c58 4c53 5852 656e 6465  xin)...XLSXRende
-000003c0: 7265 7229 01da 0673 7461 7475 7329 01da  rer)...status)..
-000003d0: 0661 6374 696f 6e29 01da 0b4c 6973 7441  .action)...ListA
-000003e0: 5049 5669 6577 2901 da0f 4973 4175 7468  PIView)...IsAuth
-000003f0: 656e 7469 6361 7465 6429 01da 0852 6573  enticated)...Res
-00000400: 706f 6e73 6529 02da 1452 6561 644f 6e6c  ponse)...ReadOnl
-00000410: 794d 6f64 656c 5669 6577 5365 74da 0c4d  yModelViewSet..M
-00000420: 6f64 656c 5669 6577 5365 7429 12da 0848  odelViewSet)...H
-00000430: 6f73 7069 7461 6cda 064f 6666 6963 65da  ospital..Office.
-00000440: 0644 6f63 746f 72da 0d50 6f73 6974 696f  .Doctor..Positio
-00000450: 6e54 6974 6c65 da04 5573 6572 da0a 4578  nTitle..User..Ex
-00000460: 7472 6147 726f 7570 da16 496e 7370 6563  traGroup..Inspec
-00000470: 7469 6f6e 4469 6374 696f 6e61 7269 6573  tionDictionaries
-00000480: da17 4578 616d 696e 6174 696f 6e44 6963  ..ExaminationDic
-00000490: 7469 6f6e 6172 6965 73da 0d44 7275 6744  tionaries..DrugD
-000004a0: 6972 6563 746f 7279 da12 5068 6172 6d61  irectory..Pharma
-000004b0: 6379 4d61 6e61 6765 6d65 6e74 da0f 4578  cyManagement..Ex
-000004c0: 7065 6e73 6553 7461 6e64 6172 64da 0741  penseStandard..A
-000004d0: 7069 496e 666f da13 4472 7567 5072 6570  piInfo..DrugPrep
-000004e0: 6172 6174 696f 6e54 7970 65da 0844 7275  arationType..Dru
-000004f0: 6754 7970 65da 0c44 7275 6743 6174 6567  gType..DrugCateg
-00000500: 6f72 79da 0c50 6861 726d 6163 7944 7275  ory..PharmacyDru
-00000510: 67da 0e49 6e73 7065 6374 696f 6e54 7970  g..InspectionTyp
-00000520: 65da 0f45 7861 6d69 6e61 7469 6f6e 5479  e..ExaminationTy
-00000530: 7065 2909 da0e 5573 6572 5365 7269 616c  pe)...UserSerial
-00000540: 697a 6572 da12 5061 7373 776f 7264 5365  izer..PasswordSe
-00000550: 7269 616c 697a 6572 da20 496e 7370 6563  rializer. Inspec
-00000560: 7469 6f6e 4469 6374 696f 6e61 7269 6573  tionDictionaries
-00000570: 5365 7269 616c 697a 6572 da21 4578 616d  Serializer.!Exam
-00000580: 696e 6174 696f 6e44 6963 7469 6f6e 6172  inationDictionar
-00000590: 6965 7353 6572 6961 6c69 7a65 72da 1c50  iesSerializer..P
-000005a0: 6861 726d 6163 794d 616e 6167 656d 656e  harmacyManagemen
-000005b0: 7453 6572 6961 6c69 7a65 72da 1744 7275  tSerializer..Dru
-000005c0: 6744 6972 6563 746f 7279 5365 7269 616c  gDirectorySerial
-000005d0: 697a 6572 da11 4170 6949 6e66 6f53 6572  izer..ApiInfoSer
-000005e0: 6961 6c69 7a65 72da 1849 6e73 7065 6374  ializer..Inspect
-000005f0: 696f 6e54 7970 6553 6572 6961 6c69 7a65  ionTypeSerialize
-00000600: 72da 1945 7861 6d69 6e61 7469 6f6e 5479  r..ExaminationTy
-00000610: 7065 5365 7269 616c 697a 6572 2901 da14  peSerializer)...
-00000620: 5065 726d 6973 7369 6f6e 5365 7269 616c  PermissionSerial
-00000630: 697a 6572 2901 da08 7365 7474 696e 6773  izer)...settings
-00000640: 2901 da0f 786c 6461 7465 5f61 735f 7475  )...xldate_as_tu
-00000650: 706c 6563 0100 0000 0000 0000 0000 0000  plec............
-00000660: 0500 0000 0500 0000 4300 0000 7386 0000  ........C...s...
-00000670: 007c 006a 0064 016b 0272 8274 01a0 027c  .|.j.d.k.r.t...|
-00000680: 006a 03a0 0464 02a1 01a1 017d 017c 0164  .j...d.....}.|.d
-00000690: 0319 007d 027c 0164 0419 007d 0374 056a  ...}.|.d...}.t.j
-000006a0: 066a 077c 0364 058d 01a0 08a1 007d 047c  .j.|.d.......}.|
-000006b0: 0472 767c 046a 0964 0675 0072 7664 077c  .rv|.j.d.u.rvd.|
-000006c0: 045f 097c 04a0 0a64 08a1 0101 007c 027c  ._.|...d.....|.|
-000006d0: 045f 0b7c 04a0 0ca1 0001 0074 0d64 0964  ._.|.......t.d.d
-000006e0: 0769 0183 0153 0074 0d64 0964 0a69 0183  .i...S.t.d.d.i..
-000006f0: 0153 0064 0b53 0029 0c75 0f00 0000 e6b3  .S.d.S.).u......
-00000700: a8e5 868c e8af a6e6 8385 e9a1 b5da 0450  ...............P
-00000710: 4f53 54fa 0575 7466 2d38 da05 7068 6f6e  OST..utf-8..phon
-00000720: 65da 0875 7365 726e 616d 65a9 0172 3200  e..username..r2.
-00000730: 0000 4654 da06 3132 3334 3536 da04 6461  ..FT..123456..da
-00000740: 7461 7533 0000 00e8 afa5 e5b7 a5e5 8fb7  tau3............
-00000750: e994 99e8 afaf e688 96e8 8085 e5b7 b2e8  ................
-00000760: a2ab e6b3 a8e5 868c efbc 8ce8 afb7 e7a1  ................
-00000770: aee8 aea4 e5b7 a5e5 8fb7 4e29 0eda 066d  ..........N)...m
-00000780: 6574 686f 64da 046a 736f 6eda 056c 6f61  ethod..json..loa
-00000790: 6473 da04 626f 6479 da06 6465 636f 6465  ds..body..decode
-000007a0: 7215 0000 00da 076f 626a 6563 7473 da06  r......objects..
-000007b0: 6669 6c74 6572 da05 6669 7273 74da 0969  filter..first..i
-000007c0: 735f 6163 7469 7665 da0c 7365 745f 7061  s_active..set_pa
-000007d0: 7373 776f 7264 7231 0000 00da 0473 6176  sswordr1.....sav
-000007e0: 6572 0600 0000 2905 da07 7265 7175 6573  er....)...reques
-000007f0: 7472 3500 0000 7231 0000 0072 3200 0000  tr5...r1...r2...
-00000800: da04 7573 6572 a900 7243 0000 00fa 362f  ..user..rC....6/
-00000810: 686f 6d65 2f6c 7968 2f77 6f72 6b2f 4261  home/lyh/work/Ba
-00000820: 7365 4675 6e63 7469 6f6e 4d6f 6475 6c65  seFunctionModule
-00000830: 2f62 6173 655f 7379 7374 656d 2f76 6965  /base_system/vie
-00000840: 7773 2e70 79da 0872 6567 6973 7465 7229  ws.py..register)
-00000850: 0000 0073 1800 0000 0002 0a01 1201 0801  ...s............
-00000860: 0801 1202 0e02 0601 0a01 0601 0801 0c02  ................
-00000870: 7245 0000 0063 0100 0000 0000 0000 0000  rE...c..........
-00000880: 0000 0600 0000 0500 0000 4300 0000 737a  ..........C...sz
-00000890: 0000 0074 00a0 017c 006a 02a0 0364 01a1  ...t...|.j...d..
-000008a0: 01a1 017d 0174 047c 0183 0101 007c 0164  ...}.t.|.....|.d
-000008b0: 0219 007d 027c 0164 0319 007d 0374 056a  ...}.|.d...}.t.j
-000008c0: 066a 077c 0264 048d 017d 047c 0372 767c  .j.|.d...}.|.rv|
-000008d0: 04a0 087c 03a1 0101 0064 057c 045f 0974  ...|.....d.|._.t
-000008e0: 0a6a 0aa0 0ba1 007c 045f 0c64 067c 045f  .j.....|._.d.|._
-000008f0: 0d7c 04a0 0ea1 0001 0064 0764 0669 017d  .|.......d.d.i.}
-00000900: 0574 0f7c 0583 0153 0064 0853 0029 0975  .t.|...S.d.S.).u
-00000910: 1200 0000 e4bf aee6 94b9 e794 a8e6 88b7  ................
-00000920: e4bf a1e6 81af 7230 0000 00da 0775 7365  ......r0.....use
-00000930: 725f 6964 da08 7061 7373 776f 7264 2901  r_id..password).
-00000940: da02 6964 7201 0000 0054 7235 0000 004e  ..idr....Tr5...N
-00000950: 2910 7237 0000 0072 3800 0000 7239 0000  ).r7...r8...r9..
-00000960: 0072 3a00 0000 da05 7072 696e 7472 1500  .r:.....printr..
-00000970: 0000 723b 0000 00da 0367 6574 723f 0000  ..r;.....getr?..
-00000980: 00da 0b65 7272 6f72 5f74 696d 6573 da08  ...error_times..
-00000990: 6461 7465 7469 6d65 da03 6e6f 77da 106c  datetime..now..l
-000009a0: 6173 745f 6368 616e 6765 5f74 696d 65da  ast_change_time.
-000009b0: 0d69 735f 6368 616e 6765 5f70 7764 7240  .is_change_pwdr@
-000009c0: 0000 0072 0600 0000 2906 7241 0000 0072  ...r....).rA...r
-000009d0: 3500 0000 7246 0000 0072 4700 0000 7242  5...rF...rG...rB
-000009e0: 0000 00da 0372 6573 7243 0000 0072 4300  .....resrC...rC.
-000009f0: 0000 7244 0000 00da 0f63 6861 6e67 655f  ..rD.....change_
-00000a00: 7061 7373 776f 7264 3c00 0000 731a 0000  password<...s...
-00000a10: 0000 0212 0108 0108 0108 010e 0204 010a  ................
-00000a20: 0106 010c 0106 0108 0108 0172 5100 0000  ...........rQ...
-00000a30: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000a40: 0002 0000 0040 0000 0073 2e00 0000 6500  .....@...s....e.
-00000a50: 5a01 6400 5a02 6401 5a03 6504 5a05 6506  Z.d.Z.d.Z.e.Z.e.
-00000a60: 6601 5a07 6402 5a08 6403 6404 8400 5a09  f.Z.d.Z.d.d...Z.
-00000a70: 6405 6406 8400 5a0a 6402 5300 2907 da0f  d.d...Z.d.S.)...
-00000a80: 5065 726d 6973 7369 6f6e 7356 6965 7775  PermissionsViewu
-00000a90: 2800 0000 0a20 2020 20e8 8eb7 e58f 96e5  (....    .......
-00000aa0: bd93 e589 8de7 94a8 e688 b7e5 898d e7ab  ................
-00000ab0: afe6 9d83 e999 900a 2020 2020 4e63 0100  ........    Nc..
-00000ac0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
-00000ad0: 0000 4300 0000 7308 0000 007c 006a 006a  ..C...s....|.j.j
-00000ae0: 0153 0029 014e 2902 7241 0000 0072 4200  .S.).N).rA...rB.
-00000af0: 0000 2901 da04 7365 6c66 7243 0000 0072  ..)...selfrC...r
-00000b00: 4300 0000 7244 0000 00da 0a67 6574 5f6f  C...rD.....get_o
-00000b10: 626a 6563 7456 0000 0073 0200 0000 0001  bjectV...s......
-00000b20: 7a1a 5065 726d 6973 7369 6f6e 7356 6965  z.PermissionsVie
-00000b30: 772e 6765 745f 6f62 6a65 6374 6301 0000  w.get_objectc...
-00000b40: 0000 0000 0000 0000 0003 0000 0003 0000  ................
-00000b50: 0043 0000 0073 3400 0000 7c00 6a00 6a01  .C...s4...|.j.j.
-00000b60: 6a02 a003 a100 7d01 7c01 7226 7404 6a05  j.....}.|.r&t.j.
-00000b70: 6a06 7c01 6401 8d01 a007 a100 7d02 6e0a  j.|.d.......}.n.
-00000b80: 7404 6a05 a008 a100 7d02 7c02 5300 2902  t.j.....}.|.S.).
-00000b90: 7524 0000 000a 2020 2020 2020 2020 e5be  u$....        ..
-00000ba0: 97e5 88b0 e8a7 92e8 89b2 e69d 83e9 9990  ................
-00000bb0: 0a20 2020 2020 2020 2029 015a 0967 726f  .        ).Z.gro
-00000bc0: 7570 5f5f 696e 2909 7241 0000 0072 4200  up__in).rA...rB.
-00000bd0: 0000 da06 6772 6f75 7073 da03 616c 6c72  ....groups..allr
-00000be0: 0400 0000 723b 0000 0072 3c00 0000 da08  ....r;...r<.....
-00000bf0: 6469 7374 696e 6374 da04 6e6f 6e65 2903  distinct..none).
-00000c00: 7253 0000 0072 5500 0000 da0b 7065 726d  rS...rU.....perm
-00000c10: 6973 7369 6f6e 7372 4300 0000 7243 0000  issionsrC...rC..
-00000c20: 0072 4400 0000 da0c 6765 745f 7175 6572  .rD.....get_quer
-00000c30: 7973 6574 5900 0000 730a 0000 0000 050e  ysetY...s.......
-00000c40: 0104 0114 020a 017a 1c50 6572 6d69 7373  .......z.Permiss
-00000c50: 696f 6e73 5669 6577 2e67 6574 5f71 7565  ionsView.get_que
-00000c60: 7279 7365 7429 0bda 085f 5f6e 616d 655f  ryset)...__name_
-00000c70: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000c80: 5f71 7561 6c6e 616d 655f 5fda 075f 5f64  _qualname__..__d
-00000c90: 6f63 5f5f 722c 0000 00da 1073 6572 6961  oc__r,.....seria
-00000ca0: 6c69 7a65 725f 636c 6173 7372 0d00 0000  lizer_classr....
-00000cb0: da12 7065 726d 6973 7369 6f6e 5f63 6c61  ..permission_cla
-00000cc0: 7373 6573 da10 7061 6769 6e61 7469 6f6e  sses..pagination
-00000cd0: 5f63 6c61 7373 7254 0000 0072 5a00 0000  _classrT...rZ...
-00000ce0: 7243 0000 0072 4300 0000 7243 0000 0072  rC...rC...rC...r
-00000cf0: 4400 0000 7252 0000 004e 0000 0073 0c00  D...rR...N...s..
-00000d00: 0000 0801 0403 0401 0601 0402 0803 7252  ..............rR
-00000d10: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000d20: 0000 0000 0300 0000 4000 0000 731a 0000  ........@...s...
-00000d30: 0065 005a 0164 005a 0264 015a 0364 0564  .e.Z.d.Z.d.Z.d.d
-00000d40: 0364 0484 015a 0464 0253 0029 06da 1a4f  .d...Z.d.S.)...O
-00000d50: 7665 7272 6964 6555 7365 7241 7574 6865  verrideUserAuthe
-00000d60: 6e74 6963 6174 696f 6e75 5000 0000 0a20  nticationuP.... 
-00000d70: 2020 20e9 878d e586 99e7 94a8 e688 b7e9     .............
-00000d80: aa8c e8af 810a 2020 2020 4175 7468 656e  ......    Authen
-00000d90: 7469 6361 7465 7320 6167 6169 6e73 7420  ticates against 
-00000da0: 7365 7474 696e 6773 2e41 5554 485f 5553  settings.AUTH_US
-00000db0: 4552 5f4d 4f44 454c 2e0a 2020 2020 4e63  ER_MODEL..    Nc
-00000dc0: 0500 0000 0000 0000 0000 0000 0c00 0000  ................
-00000dd0: 0a00 0000 4b00 0000 736c 0000 007a 3264  ....K...sl...z2d
-00000de0: 017d 0674 007c 0683 017d 077c 07a0 017c  .}.t.|...}.|...|
-00000df0: 02a1 017d 087c 07a0 017c 03a1 017d 0974  ...}.|...|...}.t
-00000e00: 026a 036a 047c 0864 028d 017d 0a57 006e  .j.j.|.d...}.W.n
-00000e10: 2604 0074 0579 5801 007d 0b01 007a 0e57  &..t.yX..}...z.W
-00000e20: 0059 0064 007d 0b7e 0b64 0053 0064 007d  .Y.d.}.~.d.S.d.}
-00000e30: 0b7e 0b30 0030 007c 0aa0 067c 09a1 0172  .~.0.0.|...|...r
-00000e40: 687c 0a53 0064 0053 0029 034e da10 4b33  h|.S.d.S.).N..K3
-00000e50: 6244 4436 5a79 7475 7235 524c 434a 7233  bDD6Zytur5RLCJr3
-00000e60: 0000 0029 07da 0650 7944 4553 33da 0764  ...)...PyDES3..d
-00000e70: 6563 7279 7074 7215 0000 0072 3b00 0000  ecryptr....r;...
-00000e80: 724a 0000 00da 0945 7863 6570 7469 6f6e  rJ.....Exception
-00000e90: da0e 6368 6563 6b5f 7061 7373 776f 7264  ..check_password
-00000ea0: 290c 7253 0000 0072 4100 0000 7232 0000  ).rS...rA...r2..
-00000eb0: 0072 4700 0000 5a05 6170 7073 73da 066b  .rG...Z.appss..k
-00000ec0: 7761 7267 73da 036b 6579 da05 7064 6573  wargs..key..pdes
-00000ed0: 32da 1064 6563 7279 7074 5f75 7365 726e  2..decrypt_usern
-00000ee0: 616d 655a 1064 6563 7279 7074 5f70 6173  ameZ.decrypt_pas
-00000ef0: 7377 6f72 6472 4200 0000 da01 6572 4300  swordrB.....erC.
-00000f00: 0000 7243 0000 0072 4400 0000 da0c 6175  ..rC...rD.....au
-00000f10: 7468 656e 7469 6361 7465 6c00 0000 7314  thenticatel...s.
-00000f20: 0000 0000 0102 0104 0108 010a 010a 0112  ................
-00000f30: 010e 0318 020a 017a 274f 7665 7272 6964  .......z'Overrid
-00000f40: 6555 7365 7241 7574 6865 6e74 6963 6174  eUserAuthenticat
-00000f50: 696f 6e2e 6175 7468 656e 7469 6361 7465  ion.authenticate
-00000f60: 2903 4e4e 4e29 0572 5b00 0000 725c 0000  ).NNN).r[...r\..
-00000f70: 0072 5d00 0000 725e 0000 0072 6d00 0000  .r]...r^...rm...
-00000f80: 7243 0000 0072 4300 0000 7243 0000 0072  rC...rC...rC...r
-00000f90: 4400 0000 7262 0000 0066 0000 0073 0400  D...rb...f...s..
-00000fa0: 0000 0801 0405 7262 0000 0063 0000 0000  ......rb...c....
-00000fb0: 0000 0000 0000 0000 0000 0000 0200 0000  ................
-00000fc0: 4000 0000 7324 0000 0065 005a 0164 005a  @...s$...e.Z.d.Z
-00000fd0: 0264 0164 0284 005a 0364 0364 0484 005a  .d.d...Z.d.d...Z
-00000fe0: 0464 0564 0684 005a 0564 0753 0029 0872  .d.d...Z.d.S.).r
-00000ff0: 6400 0000 6302 0000 0000 0000 0000 0000  d...c...........
-00001000: 0002 0000 0004 0000 0043 0000 0073 1600  .........C...s..
-00001010: 0000 7400 6a01 7c01 7400 6a02 6401 8d02  ..t.j.|.t.j.d...
-00001020: 7c00 5f03 6402 5300 2903 755d 0000 000a  |._.d.S.).u]....
-00001030: 2020 2020 2020 2020 e4b8 89e9 878d 4445          ......DE
-00001040: 53e5 8aa0 e5af 86e3 8081 e5af b9e7 a7b0  S...............
-00001050: e58a a0e5 af86 e380 8270 7932 e4b8 8be4  .........py2....
-00001060: b88d e58f afe7 94a8 0a20 2020 2020 2020  .........       
-00001070: 203a 7061 7261 6d20 6b65 793a 20e5 af86   :param key: ...
-00001080: e992 a50a 2020 2020 2020 2020 2901 5a07  ....        ).Z.
-00001090: 7061 646d 6f64 654e 2904 da05 7079 4465  padmodeN)...pyDe
-000010a0: 735a 0a74 7269 706c 655f 6465 735a 0950  sZ.triple_desZ.P
-000010b0: 4144 5f50 4b43 5335 da07 6372 7970 746f  AD_PKCS5..crypto
-000010c0: 7229 0272 5300 0000 7269 0000 0072 4300  r).rS...ri...rC.
-000010d0: 0000 7243 0000 0072 4400 0000 da08 5f5f  ..rC...rD.....__
-000010e0: 696e 6974 5f5f 8700 0000 7302 0000 0000  init__....s.....
-000010f0: 057a 0f50 7944 4553 332e 5f5f 696e 6974  .z.PyDES3.__init
-00001100: 5f5f 6302 0000 0000 0000 0000 0000 0003  __c.............
-00001110: 0000 0004 0000 0043 0000 0073 1e00 0000  .......C...s....
-00001120: 7c00 6a00 a001 7c01 a002 a100 a101 7d02  |.j...|.......}.
-00001130: 7403 a004 7c02 a101 a005 a100 5300 2901  t...|.......S.).
-00001140: 753e 0000 000a 2020 2020 2020 2020 e58a  u>....        ..
-00001150: a0e5 af86 0a20 2020 2020 2020 203a 7061  .....        :pa
-00001160: 7261 6d20 7465 7874 3a0a 2020 2020 2020  ram text:.      
-00001170: 2020 3a72 6574 7572 6e3a 0a20 2020 2020    :return:.     
-00001180: 2020 2029 0672 6f00 0000 da07 656e 6372     ).ro.....encr
-00001190: 7970 74da 0665 6e63 6f64 65da 0662 6173  ypt..encode..bas
-000011a0: 6536 34da 1273 7461 6e64 6172 645f 6236  e64..standard_b6
-000011b0: 3465 6e63 6f64 6572 3a00 0000 a903 7253  4encoder:.....rS
-000011c0: 0000 00da 0474 6578 74da 0178 7243 0000  .....text..xrC..
-000011d0: 0072 4300 0000 7244 0000 0072 7100 0000  .rC...rD...rq...
-000011e0: 8e00 0000 7304 0000 0000 0610 017a 0e50  ....s........z.P
-000011f0: 7944 4553 332e 656e 6372 7970 7463 0200  yDES3.encryptc..
-00001200: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00001210: 0000 4300 0000 7322 0000 0074 00a0 017c  ..C...s"...t...|
-00001220: 01a0 02a1 00a1 017d 027c 006a 03a0 047c  .......}.|.j...|
-00001230: 02a1 017d 027c 02a0 05a1 0053 0029 0175  ...}.|.....S.).u
-00001240: 3e00 0000 0a20 2020 2020 2020 20e8 a7a3  >....        ...
-00001250: e5af 860a 2020 2020 2020 2020 3a70 6172  ....        :par
-00001260: 616d 2074 6578 743a 0a20 2020 2020 2020  am text:.       
-00001270: 203a 7265 7475 726e 3a0a 2020 2020 2020   :return:.      
-00001280: 2020 2906 7273 0000 00da 1273 7461 6e64    ).rs.....stand
-00001290: 6172 645f 6236 3464 6563 6f64 6572 7200  ard_b64decoderr.
-000012a0: 0000 726f 0000 0072 6500 0000 723a 0000  ..ro...re...r:..
-000012b0: 0072 7500 0000 7243 0000 0072 4300 0000  .ru...rC...rC...
-000012c0: 7244 0000 0072 6500 0000 9700 0000 7306  rD...re.......s.
-000012d0: 0000 0000 060e 010c 017a 0e50 7944 4553  .........z.PyDES
-000012e0: 332e 6465 6372 7970 744e 2906 725b 0000  3.decryptN).r[..
-000012f0: 0072 5c00 0000 725d 0000 0072 7000 0000  .r\...r]...rp...
-00001300: 7271 0000 0072 6500 0000 7243 0000 0072  rq...re...rC...r
-00001310: 4300 0000 7243 0000 0072 4400 0000 7264  C...rC...rD...rd
-00001320: 0000 0086 0000 0073 0600 0000 0801 0807  .......s........
-00001330: 0809 7264 0000 0063 0100 0000 0000 0000  ..rd...c........
-00001340: 0000 0000 1600 0000 0b00 0000 4300 0000  ............C...
-00001350: 73ac 0100 007c 006a 00a0 0164 01a1 017d  s....|.j...d...}
-00001360: 017c 006a 02a0 0164 0264 03a1 027d 027c  .|.j...d.d...}.|
-00001370: 026a 03a0 0464 04a1 0164 0519 00a0 0464  .j...d...d.....d
-00001380: 06a1 0164 0719 007d 0367 007d 047c 0364  ...d...}.g.}.|.d
-00001390: 0876 0090 0172 8c90 017a 1c74 056a 0664  .v...r...z.t.j.d
-000013a0: 097c 02a0 07a1 0064 0a64 0b8d 037d 057c  .|.....d.d...}.|
-000013b0: 05a0 08a1 007d 067c 0644 005d f67d 077c  .....}.|.D.].}.|
-000013c0: 076a 097d 0874 0a64 0c7c 0883 0244 005d  .j.}.t.d.|...D.]
-000013d0: e07d 097c 07a0 0b7c 09a1 017d 0a7c 0a72  .}.|...|...}.|.r
-000013e0: 7a7c 07a0 0c7c 0964 07a1 026a 0d7d 0b7c  z|...|.d...j.}.|
-000013f0: 07a0 0e7c 0964 07a1 027d 0c7c 0b64 0c6b  ...|.d...}.|.d.k
-00001400: 0272 c27c 0c64 0516 0064 076b 0272 c274  .r.|.d...d.k.r.t
-00001410: 0f7c 0c83 017d 0c7c 0a64 0519 007d 0d7c  .|...}.|.d...}.|
-00001420: 0a64 0c19 007d 0e74 106a 116a 017c 0e64  .d...}.t.j.j.|.d
-00001430: 0d8d 016a 127d 0f7c 0a64 0e19 007d 107c  ...j.}.|.d...}.|
-00001440: 0a64 0f19 007d 1174 136a 116a 147c 0c64  .d...}.t.j.j.|.d
-00001450: 108d 017d 127c 1290 0172 247c 126a 1566  ...}.|...r$|.j.f
-00001460: 0069 007c 0c7c 0d7c 0f7c 107c 1164 119c  .i.|.|.|.|.|.d..
-00001470: 05a4 018e 0101 006e 1c7c 126a 1666 0069  .......n.|.j.f.i
-00001480: 007c 0c7c 0d7c 0f7c 107c 1164 119c 05a4  .|.|.|.|.|.d....
-00001490: 018e 0101 007c 0c7c 0d7c 0f7c 107c 1164  .....|.|.|.|.|.d
-000014a0: 119c 057d 137c 04a0 177c 13a1 0101 0071  ...}.|...|.....q
-000014b0: 7a71 6657 006e 2a04 0074 1890 0179 8a01  zqfW.n*..t...y..
-000014c0: 007d 1401 007a 107c 1482 0157 0059 0064  .}...z.|...W.Y.d
-000014d0: 097d 147e 146e 0a64 097d 147e 1430 0030  .}.~.n.d.}.~.0.0
-000014e0: 007c 0490 0172 9c64 127c 0469 017d 156e  .|...r.d.|.i.}.n
-000014f0: 0864 1264 1369 017d 1574 197c 1583 0153  .d.d.i.}.t.|...S
-00001500: 0029 1475 1400 0000 e5af bce5 85a5 6578  .).u..........ex
-00001510: 6365 6ce8 a1a8 e695 b0e6 8dae da0c 6372  cel...........cr
-00001520: 6561 7465 645f 7573 6572 da0a 6578 6365  eated_user..exce
-00001530: 6c5f 6669 6c65 da00 da01 2ee9 0100 0000  l_file..........
-00001540: fa01 2272 0100 0000 a902 da04 786c 7378  .."r........xlsx
-00001550: 5a03 786c 734e 54a9 03da 0866 696c 656e  Z.xlsNT....filen
-00001560: 616d 65da 0d66 696c 655f 636f 6e74 656e  ame..file_conten
-00001570: 7473 5a0b 7261 6767 6564 5f72 6f77 73e9  tsZ.ragged_rows.
-00001580: 0200 0000 a901 da04 6e61 6d65 e903 0000  ........name....
-00001590: 00e9 0400 0000 a901 da07 636f 6465 6e75  ..........codenu
-000015a0: 6d29 0572 8a00 0000 7286 0000 00da 0868  m).r....r......h
-000015b0: 6f73 7069 7461 6cda 0c63 7265 6174 6564  ospital..created
-000015c0: 5f74 696d 65da 0a63 7265 6174 6564 5f62  _time..created_b
-000015d0: 7972 3500 0000 f53f 0000 00e6 9687 e4bb  yr5....?........
-000015e0: b6e5 8685 e5ae b9e6 a0bc e5bc 8fe6 9c89  ................
-000015f0: e8af afef bc8c e8af b7e6 a380 e69f a5e5  ................
-00001600: 8685 e5ae b9e6 a0bc e5bc 8fe6 98af e590  ................
-00001610: a6e6 ada3 e7a1 aeef bc81 291a 722f 0000  ..........).r/..
-00001620: 0072 4a00 0000 da05 4649 4c45 5372 8600  .rJ.....FILESr..
-00001630: 0000 da05 7370 6c69 74da 0478 6c72 64da  ....split..xlrd.
-00001640: 0d6f 7065 6e5f 776f 726b 626f 6f6b da04  .open_workbook..
-00001650: 7265 6164 da06 7368 6565 7473 da05 6e72  read..sheets..nr
-00001660: 6f77 73da 0572 616e 6765 da0a 726f 775f  ows..range..row_
-00001670: 7661 6c75 6573 da04 6365 6c6c da05 6374  values..cell..ct
-00001680: 7970 65da 0a63 656c 6c5f 7661 6c75 65da  ype..cell_value.
-00001690: 0369 6e74 7211 0000 0072 3b00 0000 7248  .intr....r;...rH
-000016a0: 0000 0072 1400 0000 723c 0000 00da 0675  ...r....r<.....u
-000016b0: 7064 6174 65da 0663 7265 6174 65da 0661  pdate..create..a
-000016c0: 7070 656e 6472 6600 0000 7206 0000 0029  ppendrf...r....)
-000016d0: 1672 4100 0000 7279 0000 0072 7a00 0000  .rA...ry...rz...
-000016e0: da09 6669 6c65 5f74 7970 65da 0964 6174  ..file_type..dat
-000016f0: 615f 6c69 7374 7235 0000 0072 9400 0000  a_listr5...r....
-00001700: da05 7368 6565 74da 0472 6f77 73da 0372  ..sheet..rows..r
-00001710: 6f77 7297 0000 0072 9900 0000 728a 0000  owr....r....r...
-00001720: 0072 8600 0000 da0d 686f 7370 6974 616c  .r......hospital
-00001730: 5f6e 616d 6572 8b00 0000 728c 0000 0072  _namer....r....r
-00001740: 8d00 0000 5a0d 706f 7369 7469 6f6e 7469  ....Z.positionti
-00001750: 746c 65da 0a65 7863 656c 5f64 6174 6172  tle..excel_datar
-00001760: 6c00 0000 7250 0000 0072 4300 0000 7243  l...rP...rC...rC
-00001770: 0000 0072 4400 0000 da15 696d 706f 7274  ...rD.....import
-00001780: 5f70 6f73 6974 696f 6e5f 7469 746c 65a2  _position_title.
-00001790: 0000 0073 6200 0000 0003 0c01 0e01 1a02  ...sb...........
-000017a0: 0402 0a02 0401 1401 0801 0801 0601 0e01  ................
-000017b0: 0a01 0402 0e01 0c01 1401 0801 0801 0801  ................
-000017c0: 1001 0801 0801 0e01 0601 0a01 0201 0201  ................
-000017d0: 0201 02fc 0c07 0a01 0201 0201 0201 02fc  ................
-000017e0: 0a07 0201 0201 0201 0201 02fb 0607 1201  ................
-000017f0: 1001 1a02 0601 0a02 0801 72a6 0000 0063  ..........r....c
-00001800: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001810: 0400 0000 4000 0000 7340 0000 0065 005a  ....@...s@...e.Z
-00001820: 0164 005a 0265 036a 0464 0164 028d 015a  .d.Z.e.j.d.d...Z
-00001830: 0565 036a 0664 0364 0464 058d 025a 0765  .e.j.d.d.d...Z.e
-00001840: 036a 0664 0664 028d 015a 0847 0064 0764  .j.d.d...Z.G.d.d
-00001850: 0884 0064 0883 025a 0964 0953 0029 0ada  ...d...Z.d.S.)..
-00001860: 0a55 7365 7246 696c 7465 72da 0667 656e  .UserFilter..gen
-00001870: 6465 72a9 01da 0a66 6965 6c64 5f6e 616d  der....field_nam
-00001880: 6572 8600 0000 da09 6963 6f6e 7461 696e  er......icontain
-00001890: 73a9 0272 aa00 0000 da0b 6c6f 6f6b 7570  s..r......lookup
-000018a0: 5f65 7870 72da 0a61 7661 7461 725f 7572  _expr..avatar_ur
-000018b0: 6c63 0000 0000 0000 0000 0000 0000 0000  lc..............
-000018c0: 0000 0100 0000 4000 0000 7314 0000 0065  ......@...s....e
-000018d0: 005a 0164 005a 0265 035a 0464 015a 0564  .Z.d.Z.e.Z.d.Z.d
-000018e0: 0253 0029 037a 0f55 7365 7246 696c 7465  .S.).z.UserFilte
-000018f0: 722e 4d65 7461 da07 5f5f 616c 6c5f 5f4e  r.Meta..__all__N
-00001900: 2906 725b 0000 0072 5c00 0000 725d 0000  ).r[...r\...r]..
-00001910: 0072 1500 0000 da05 6d6f 6465 6cda 0666  .r......model..f
-00001920: 6965 6c64 7372 4300 0000 7243 0000 0072  ieldsrC...rC...r
-00001930: 4300 0000 7244 0000 00da 044d 6574 61e8  C...rD.....Meta.
-00001940: 0000 0073 0400 0000 0801 0401 72b2 0000  ...s........r...
-00001950: 004e 290a 725b 0000 0072 5c00 0000 725d  .N).r[...r\...r]
-00001960: 0000 00da 0766 696c 7465 7273 da0c 4e75  .....filters..Nu
-00001970: 6d62 6572 4669 6c74 6572 72a8 0000 00da  mberFilterr.....
-00001980: 0a43 6861 7246 696c 7465 7272 8600 0000  .CharFilterr....
-00001990: 72ae 0000 0072 b200 0000 7243 0000 0072  r....r....rC...r
-000019a0: 4300 0000 7243 0000 0072 4400 0000 72a7  C...rC...rD...r.
-000019b0: 0000 00e0 0000 0073 0800 0000 0804 0c01  .......s........
-000019c0: 0e01 0c02 72a7 0000 0063 0000 0000 0000  ....r....c......
-000019d0: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
-000019e0: 0000 733e 0000 0065 005a 0164 005a 0265  ..s>...e.Z.d.Z.e
-000019f0: 036a 04a0 05a1 00a0 0664 01a1 015a 0765  .j.......d...Z.e
-00001a00: 085a 0965 0a5a 0b64 025a 0c65 0d64 0367  .Z.e.Z.d.Z.e.d.g
-00001a10: 0164 0464 058d 0264 0664 0784 0083 015a  .d.d...d.d.....Z
-00001a20: 0e64 0853 0029 09da 0b55 7365 7256 6965  .d.S.)...UserVie
-00001a30: 7753 6574 fa03 2d69 6472 af00 0000 da03  wSet..-idr......
-00001a40: 5055 5454 2902 da07 6d65 7468 6f64 73da  PUTT)...methods.
-00001a50: 0664 6574 6169 6c63 0300 0000 0000 0000  .detailc........
-00001a60: 0000 0000 0600 0000 0400 0000 4300 0000  ............C...
-00001a70: 736e 0000 0074 007c 016a 0164 017c 0169  sn...t.|.j.d.|.i
-00001a80: 0164 028d 027d 037c 036a 0264 0364 048d  .d...}.|.j.d.d..
-00001a90: 0101 007c 036a 01a0 0364 05a1 017d 047c  ...|.j...d...}.|
-00001aa0: 00a0 04a1 007d 057c 05a0 057c 04a1 0101  .....}.|...|....
-00001ab0: 0074 066a 06a0 07a1 007c 055f 0864 067c  .t.j.....|._.d.|
-00001ac0: 055f 0964 077c 055f 0a7c 05a0 0ba1 0001  ._.d.|._.|......
-00001ad0: 0074 0c64 0864 0969 0174 0d6a 0e64 0a8d  .t.d.d.i.t.j.d..
-00001ae0: 0253 0029 0b4e 7241 0000 0029 0272 3500  .S.).NrA...).r5.
-00001af0: 0000 da07 636f 6e74 6578 7454 2901 da0f  ....contextT)...
-00001b00: 7261 6973 655f 6578 6365 7074 696f 6e72  raise_exceptionr
-00001b10: 4700 0000 7201 0000 0046 da07 6d65 7373  G...r....F..mess
-00001b20: 6167 6575 0c00 0000 e4bf aee6 94b9 e688  ageu............
-00001b30: 90e5 8a9f a902 7235 0000 0072 0a00 0000  ......r5...r....
-00001b40: 290f 7224 0000 0072 3500 0000 da08 6973  ).r$...r5.....is
-00001b50: 5f76 616c 6964 724a 0000 0072 5400 0000  _validrJ...rT...
-00001b60: 723f 0000 0072 4c00 0000 724d 0000 0072  r?...rL...rM...r
-00001b70: 4e00 0000 724b 0000 0072 4f00 0000 7240  N...rK...rO...r@
-00001b80: 0000 0072 0e00 0000 720a 0000 00da 1648  ...r....r......H
-00001b90: 5454 505f 3230 355f 5245 5345 545f 434f  TTP_205_RESET_CO
-00001ba0: 4e54 454e 5429 0672 5300 0000 7241 0000  NTENT).rS...rA..
-00001bb0: 00da 0270 6bda 0a73 6572 6961 6c69 7a65  ...pk..serialize
-00001bc0: 7272 4700 0000 7242 0000 0072 4300 0000  rrG...rB...rC...
-00001bd0: 7243 0000 0072 4400 0000 7251 0000 00f3  rC...rD...rQ....
-00001be0: 0000 0073 1400 0000 0003 1201 0c01 0c01  ...s............
-00001bf0: 0801 0a01 0c01 0601 0601 0802 7a1b 5573  ............z.Us
-00001c00: 6572 5669 6577 5365 742e 6368 616e 6765  erViewSet.change
-00001c10: 5f70 6173 7377 6f72 644e 290f 725b 0000  _passwordN).r[..
-00001c20: 0072 5c00 0000 725d 0000 0072 1500 0000  .r\...r]...r....
-00001c30: 723b 0000 0072 5600 0000 da08 6f72 6465  r;...rV.....orde
-00001c40: 725f 6279 da08 7175 6572 7973 6574 7223  r_by..querysetr#
-00001c50: 0000 0072 5f00 0000 72a7 0000 00da 0f66  ...r_...r......f
-00001c60: 696c 7465 7273 6574 5f63 6c61 7373 da0d  ilterset_class..
-00001c70: 6669 6c74 6572 5f66 6965 6c64 7372 0b00  filter_fieldsr..
-00001c80: 0000 7251 0000 0072 4300 0000 7243 0000  ..rQ...rC...rC..
-00001c90: 0072 4300 0000 7244 0000 0072 b600 0000  .rC...rD...r....
-00001ca0: ed00 0000 730c 0000 0008 0110 0104 0104  ....s...........
-00001cb0: 0104 020c 0172 b600 0000 6300 0000 0000  .....r....c.....
-00001cc0: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
-00001cd0: 0000 0073 2600 0000 6500 5a01 6400 5a02  ...s&...e.Z.d.Z.
-00001ce0: 6401 5a03 6504 6a05 6a06 6402 6403 8d01  d.Z.e.j.j.d.d...
-00001cf0: 5a07 6508 5a09 6402 5a0a 6402 5300 2904  Z.e.Z.d.Z.d.S.).
-00001d00: da15 496e 7370 6563 7469 6f6e 5479 7065  ..InspectionType
-00001d10: 5669 6577 5365 74f5 0c00 0000 e6a3 80e6  ViewSet.........
-00001d20: 9fa5 e5ad 97e5 85b8 4ea9 01da 0670 6172  ........N....par
-00001d30: 656e 7429 0b72 5b00 0000 725c 0000 0072  ent).r[...r\...r
-00001d40: 5d00 0000 725e 0000 0072 2100 0000 723b  ]...r^...r!...r;
-00001d50: 0000 0072 3c00 0000 72c4 0000 0072 2a00  ...r<...r....r*.
-00001d60: 0000 725f 0000 0072 6100 0000 7243 0000  ..r_...ra...rC..
-00001d70: 0072 4300 0000 7243 0000 0072 4400 0000  .rC...rC...rD...
-00001d80: 72c7 0000 0003 0100 0073 0800 0000 0801  r........s......
-00001d90: 0401 0e01 0401 72c7 0000 0063 0000 0000  ......r....c....
-00001da0: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-00001db0: 4000 0000 7360 0000 0065 005a 0164 005a  @...s`...e.Z.d.Z
-00001dc0: 0265 036a 0464 0164 0264 038d 025a 0565  .e.j.d.d.d...Z.e
-00001dd0: 036a 0464 0464 0264 038d 025a 0665 036a  .j.d.d.d...Z.e.j
-00001de0: 0464 0564 0264 038d 025a 0765 036a 0464  .d.d.d...Z.e.j.d
-00001df0: 0664 0264 038d 025a 0865 036a 0464 0764  .d.d...Z.e.j.d.d
-00001e00: 0264 038d 025a 0947 0064 0864 0984 0064  .d...Z.G.d.d...d
-00001e10: 0983 025a 0a64 0a53 0029 0bda 1449 6e73  ...Z.d.S.)...Ins
-00001e20: 7065 6374 696f 6e44 6963 7446 696c 7465  pectionDictFilte
-00001e30: 72da 0c70 726f 6a65 6374 5f63 6f64 6572  r..project_coder
-00001e40: ab00 0000 72ac 0000 00da 0c70 726f 6a65  ....r......proje
-00001e50: 6374 5f6e 616d 65da 0d68 6f73 7069 7461  ct_name..hospita
-00001e60: 6c5f 636f 6465 da0b 6f66 6669 6365 5f63  l_code..office_c
-00001e70: 6f64 65da 0b64 6973 7469 6e67 7569 7368  ode..distinguish
-00001e80: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00001e90: 0001 0000 0040 0000 0073 1400 0000 6500  .....@...s....e.
-00001ea0: 5a01 6400 5a02 6503 5a04 6401 5a05 6402  Z.d.Z.e.Z.d.Z.d.
-00001eb0: 5300 2903 7a19 496e 7370 6563 7469 6f6e  S.).z.Inspection
-00001ec0: 4469 6374 4669 6c74 6572 2e4d 6574 6172  DictFilter.Metar
-00001ed0: af00 0000 4e29 0672 5b00 0000 725c 0000  ....N).r[...r\..
-00001ee0: 0072 5d00 0000 7217 0000 0072 b000 0000  .r]...r....r....
-00001ef0: 72b1 0000 0072 4300 0000 7243 0000 0072  r....rC...rC...r
-00001f00: 4300 0000 7244 0000 0072 b200 0000 1101  C...rD...r......
-00001f10: 0000 7304 0000 0008 0104 0172 b200 0000  ..s........r....
-00001f20: 4ea9 0b72 5b00 0000 725c 0000 0072 5d00  N..r[...r\...r].
-00001f30: 0000 72b3 0000 0072 b500 0000 72cc 0000  ..r....r....r...
-00001f40: 0072 cd00 0000 72ce 0000 0072 cf00 0000  .r....r....r....
-00001f50: 72d0 0000 0072 b200 0000 7243 0000 0072  r....r....rC...r
-00001f60: 4300 0000 7243 0000 0072 4400 0000 72cb  C...rC...rD...r.
-00001f70: 0000 000a 0100 0073 0c00 0000 0801 0e01  .......s........
-00001f80: 0e01 0e01 0e01 0e02 72cb 0000 0063 0000  ........r....c..
-00001f90: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-00001fa0: 0000 4000 0000 7328 0000 0065 005a 0164  ..@...s(...e.Z.d
-00001fb0: 005a 0264 015a 0365 046a 05a0 06a1 00a0  .Z.d.Z.e.j......
-00001fc0: 0764 02a1 015a 0865 095a 0a65 0b5a 0c64  .d...Z.e.Z.e.Z.d
-00001fd0: 0353 0029 04da 1d49 6e73 7065 6374 696f  .S.)...Inspectio
-00001fe0: 6e44 6963 7469 6f6e 6172 6965 7356 6965  nDictionariesVie
-00001ff0: 7753 6574 72c8 0000 0072 b700 0000 4e29  wSetr....r....N)
-00002000: 0d72 5b00 0000 725c 0000 0072 5d00 0000  .r[...r\...r]...
-00002010: 725e 0000 0072 1700 0000 723b 0000 0072  r^...r....r;...r
-00002020: 5600 0000 72c3 0000 0072 c400 0000 7225  V...r....r....r%
-00002030: 0000 0072 5f00 0000 72cb 0000 0072 c500  ...r_...r....r..
-00002040: 0000 7243 0000 0072 4300 0000 7243 0000  ..rC...rC...rC..
-00002050: 0072 4400 0000 72d2 0000 0016 0100 0073  .rD...r........s
-00002060: 0800 0000 0801 0401 1001 0402 72d2 0000  ............r...
-00002070: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00002080: 0000 0300 0000 4000 0000 7326 0000 0065  ......@...s&...e
-00002090: 005a 0164 005a 0264 015a 0365 046a 056a  .Z.d.Z.d.Z.e.j.j
-000020a0: 0664 0264 038d 015a 0765 085a 0964 025a  .d.d...Z.e.Z.d.Z
-000020b0: 0a64 0253 0029 04da 1645 7861 6d69 6e61  .d.S.)...Examina
-000020c0: 7469 6f6e 5479 7065 5669 6577 5365 7472  tionTypeViewSetr
-000020d0: c800 0000 4e72 c900 0000 290b 725b 0000  ....Nr....).r[..
-000020e0: 0072 5c00 0000 725d 0000 0072 5e00 0000  .r\...r]...r^...
-000020f0: 7222 0000 0072 3b00 0000 723c 0000 0072  r"...r;...r<...r
-00002100: c400 0000 722b 0000 0072 5f00 0000 7261  ....r+...r_...ra
-00002110: 0000 0072 4300 0000 7243 0000 0072 4300  ...rC...rC...rC.
-00002120: 0000 7244 0000 0072 d300 0000 3001 0000  ..rD...r....0...
-00002130: 7308 0000 0008 0104 010e 0104 0172 d300  s............r..
-00002140: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00002150: 0000 0004 0000 0040 0000 0073 6000 0000  .......@...s`...
-00002160: 6500 5a01 6400 5a02 6503 6a04 6401 6402  e.Z.d.Z.e.j.d.d.
-00002170: 6403 8d02 5a05 6503 6a04 6404 6402 6403  d...Z.e.j.d.d.d.
-00002180: 8d02 5a06 6503 6a04 6405 6402 6403 8d02  ..Z.e.j.d.d.d...
-00002190: 5a07 6503 6a04 6406 6402 6403 8d02 5a08  Z.e.j.d.d.d...Z.
-000021a0: 6503 6a04 6407 6402 6403 8d02 5a09 4700  e.j.d.d.d...Z.G.
-000021b0: 6408 6409 8400 6409 8302 5a0a 640a 5300  d.d...d...Z.d.S.
-000021c0: 290b da15 4578 616d 696e 6174 696f 6e44  )...ExaminationD
-000021d0: 6963 7446 696c 7465 7272 cc00 0000 72ab  ictFilterr....r.
-000021e0: 0000 0072 ac00 0000 72cd 0000 0072 ce00  ...r....r....r..
-000021f0: 0000 72cf 0000 0072 d000 0000 6300 0000  ..r....r....c...
-00002200: 0000 0000 0000 0000 0000 0000 0001 0000  ................
-00002210: 0040 0000 0073 1400 0000 6500 5a01 6400  .@...s....e.Z.d.
-00002220: 5a02 6503 5a04 6401 5a05 6402 5300 2903  Z.e.Z.d.Z.d.S.).
-00002230: 7a1a 4578 616d 696e 6174 696f 6e44 6963  z.ExaminationDic
-00002240: 7446 696c 7465 722e 4d65 7461 72af 0000  tFilter.Metar...
-00002250: 004e 2906 725b 0000 0072 5c00 0000 725d  .N).r[...r\...r]
-00002260: 0000 0072 1800 0000 72b0 0000 0072 b100  ...r....r....r..
-00002270: 0000 7243 0000 0072 4300 0000 7243 0000  ..rC...rC...rC..
-00002280: 0072 4400 0000 72b2 0000 003e 0100 0073  .rD...r....>...s
-00002290: 0400 0000 0801 0401 72b2 0000 004e 72d1  ........r....Nr.
-000022a0: 0000 0072 4300 0000 7243 0000 0072 4300  ...rC...rC...rC.
-000022b0: 0000 7244 0000 0072 d400 0000 3701 0000  ..rD...r....7...
-000022c0: 730c 0000 0008 010e 010e 010e 010e 010e  s...............
-000022d0: 0272 d400 0000 6300 0000 0000 0000 0000  .r....c.........
-000022e0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
-000022f0: 2800 0000 6500 5a01 6400 5a02 6401 5a03  (...e.Z.d.Z.d.Z.
-00002300: 6504 6a05 a006 a100 a007 6402 a101 5a08  e.j.......d...Z.
-00002310: 6509 5a0a 650b 5a0c 6403 5300 2904 da1e  e.Z.e.Z.d.S.)...
-00002320: 4578 616d 696e 6174 696f 6e44 6963 7469  ExaminationDicti
-00002330: 6f6e 6172 6965 7356 6965 7753 6574 750c  onariesViewSetu.
-00002340: 0000 00e6 a380 e9aa 8ce5 ad97 e585 b872  ...............r
-00002350: b700 0000 4e29 0d72 5b00 0000 725c 0000  ....N).r[...r\..
-00002360: 0072 5d00 0000 725e 0000 0072 1800 0000  .r]...r^...r....
-00002370: 723b 0000 0072 5600 0000 72c3 0000 0072  r;...rV...r....r
-00002380: c400 0000 7226 0000 0072 5f00 0000 72d4  ....r&...r_...r.
-00002390: 0000 0072 c500 0000 7243 0000 0072 4300  ...r....rC...rC.
-000023a0: 0000 7243 0000 0072 4400 0000 72d5 0000  ..rC...rD...r...
-000023b0: 0043 0100 0073 0800 0000 0801 0401 1001  .C...s..........
-000023c0: 0402 72d5 0000 0063 0000 0000 0000 0000  ..r....c........
-000023d0: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-000023e0: 7328 0000 0065 005a 0164 005a 0264 015a  s(...e.Z.d.Z.d.Z
-000023f0: 0365 046a 05a0 06a1 00a0 0764 02a1 015a  .e.j.......d...Z
-00002400: 0865 095a 0a64 035a 0b64 0453 0029 05da  .e.Z.d.Z.d.S.)..
-00002410: 1950 6861 726d 6163 794d 616e 6167 656d  .PharmacyManagem
-00002420: 656e 7456 6965 7753 6574 750c 0000 00e8  entViewSetu.....
-00002430: 8daf e688 bfe7 aea1 e790 8672 b700 0000  ...........r....
-00002440: 72af 0000 004e 290c 725b 0000 0072 5c00  r....N).r[...r\.
-00002450: 0000 725d 0000 0072 5e00 0000 721a 0000  ..r]...r^...r...
-00002460: 0072 3b00 0000 7256 0000 0072 c300 0000  .r;...rV...r....
-00002470: 72c4 0000 0072 2700 0000 725f 0000 0072  r....r'...r_...r
-00002480: c600 0000 7243 0000 0072 4300 0000 7243  ....rC...rC...rC
-00002490: 0000 0072 4400 0000 72d6 0000 005f 0100  ...rD...r...._..
-000024a0: 0073 0800 0000 0801 0401 1001 0401 72d6  .s............r.
-000024b0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-000024c0: 1900 0000 0f00 0000 4300 0000 7306 0200  ........C...s...
-000024d0: 007c 006a 00a0 0164 01a1 017d 017c 006a  .|.j...d...}.|.j
-000024e0: 02a0 0164 0264 03a1 027d 027c 026a 03a0  ...d.d...}.|.j..
-000024f0: 0464 04a1 0164 0519 00a0 0464 06a1 0164  .d...d.....d...d
-00002500: 0719 007d 0367 007d 047c 0364 0876 0090  ...}.g.}.|.d.v..
-00002510: 0172 e690 017a 7674 056a 0664 097c 02a0  .r...zvt.j.d.|..
-00002520: 07a1 0064 0a64 0b8d 037d 057c 05a0 08a1  ...d.d...}.|....
-00002530: 007d 067c 0644 0090 015d 4e7d 077c 076a  .}.|.D...]N}.|.j
-00002540: 097d 0874 0a64 0c7c 0883 0244 0090 015d  .}.t.d.|...D...]
-00002550: 367d 097c 07a0 0b7c 09a1 017d 0a7c 0a72  6}.|...|...}.|.r
-00002560: 7c7c 07a0 0c7c 0964 07a1 026a 0d7d 0b7c  ||...|.d...j.}.|
-00002570: 07a0 0e7c 0964 07a1 027d 0c7c 0b64 0c6b  ...|.d...}.|.d.k
-00002580: 0272 c67c 0c64 0516 0064 076b 0272 c674  .r.|.d...d.k.r.t
-00002590: 0f7c 0c83 017d 0c7c 0a64 0519 007d 0d7c  .|...}.|.d...}.|
-000025a0: 0a64 0c19 007d 0e74 106a 116a 017c 0e64  .d...}.t.j.j.|.d
-000025b0: 0d8d 016a 127d 0f7c 0a64 0e19 007d 107c  ...j.}.|.d...}.|
-000025c0: 1090 0172 0674 136a 116a 017c 1064 0d8d  ...r.t.j.j.|.d..
-000025d0: 016a 127d 116e 0464 097d 117c 0a64 0f19  .j.}.n.d.}.|.d..
-000025e0: 007d 127c 0a64 1019 007d 137c 0a64 1119  .}.|.d...}.|.d..
-000025f0: 007d 1474 136a 116a 147c 0c64 128d 017d  .}.t.j.j.|.d...}
-00002600: 157c 1590 0172 627c 156a 1566 0069 007c  .|...rb|.j.f.i.|
-00002610: 0c7c 0d7c 0f7c 117c 127c 137c 1474 166a  .|.|.|.|.|.|.t.j
-00002620: 16a0 17a1 007c 0164 139c 09a4 018e 0101  .....|.d........
-00002630: 006e 2a7c 156a 1866 0069 007c 0c7c 0d7c  .n*|.j.f.i.|.|.|
-00002640: 0f7c 117c 127c 137c 1474 166a 16a0 17a1  .|.|.|.|.t.j....
-00002650: 007c 0164 139c 09a4 018e 0101 007c 0c7c  .|.d.........|.|
-00002660: 0d7c 0f7c 117c 127c 137c 1474 166a 16a0  .|.|.|.|.|.t.j..
-00002670: 17a1 007c 0164 149c 097d 167c 04a0 197c  ...|.d...}.|...|
-00002680: 16a1 0101 0071 7c71 6657 006e 2a04 0074  .....q|qfW.n*..t
-00002690: 1a90 0179 e401 007d 1701 007a 107c 1782  ...y...}...z.|..
-000026a0: 0157 0059 0064 097d 177e 176e 0a64 097d  .W.Y.d.}.~.n.d.}
-000026b0: 177e 1730 0030 007c 0490 0172 f664 157c  .~.0.0.|...r.d.|
-000026c0: 0469 017d 186e 0864 1564 1669 017d 1874  .i.}.n.d.d.i.}.t
-000026d0: 1b7c 1883 0153 0029 1775 1a00 0000 e5af  .|...S.).u......
-000026e0: bce5 85a5 6578 6365 6ce8 a1a8 e7a7 91e5  ....excel.......
-000026f0: aea4 e695 b0e6 8dae 7279 0000 0072 7a00  ........ry...rz.
-00002700: 0000 727b 0000 0072 7c00 0000 727d 0000  ..r{...r|...r}..
-00002710: 0072 7e00 0000 7201 0000 0072 7f00 0000  .r~...r....r....
-00002720: 4e54 7281 0000 0072 8400 0000 7285 0000  NTr....r....r...
-00002730: 0072 8700 0000 7288 0000 00e9 0500 0000  .r....r.........
-00002740: e906 0000 0072 8900 0000 2909 728a 0000  .....r....).r...
-00002750: 0072 8600 0000 da0b 686f 7370 6974 616c  .r......hospital
-00002760: 5f69 64da 0970 6172 656e 745f 6964 da07  _id..parent_id..
-00002770: 6164 6472 6573 7372 3100 0000 da09 696e  addressr1.....in
-00002780: 7472 6f64 7563 6572 8c00 0000 728d 0000  troducer....r...
-00002790: 0029 0972 8a00 0000 7286 0000 0072 8b00  .).r....r....r..
-000027a0: 0000 72ca 0000 0072 db00 0000 7231 0000  ..r....r....r1..
-000027b0: 0072 dc00 0000 728c 0000 0072 8d00 0000  .r....r....r....
-000027c0: 7235 0000 0072 8e00 0000 291c 722f 0000  r5...r....).r/..
-000027d0: 0072 4a00 0000 728f 0000 0072 8600 0000  .rJ...r....r....
-000027e0: 7290 0000 00da 0578 6c72 6432 7292 0000  r......xlrd2r...
-000027f0: 0072 9300 0000 7294 0000 0072 9500 0000  .r....r....r....
-00002800: 7296 0000 0072 9700 0000 7298 0000 0072  r....r....r....r
-00002810: 9900 0000 729a 0000 0072 9b00 0000 7211  ....r....r....r.
-00002820: 0000 0072 3b00 0000 7248 0000 0072 1200  ...r;...rH...r..
-00002830: 0000 723c 0000 0072 9c00 0000 724c 0000  ..r<...r....rL..
-00002840: 0072 4d00 0000 729d 0000 0072 9e00 0000  .rM...r....r....
-00002850: 7266 0000 0072 0600 0000 2919 7241 0000  rf...r....).rA..
-00002860: 0072 7900 0000 727a 0000 0072 9f00 0000  .ry...rz...r....
-00002870: 72a0 0000 0072 3500 0000 7294 0000 0072  r....r5...r....r
-00002880: a100 0000 72a2 0000 0072 a300 0000 7297  ....r....r....r.
-00002890: 0000 0072 9900 0000 728a 0000 0072 8600  ...r....r....r..
-000028a0: 0000 72a4 0000 0072 8b00 0000 da0b 7061  ..r....r......pa
-000028b0: 7265 6e74 5f6e 616d 6572 ca00 0000 72db  rent_namer....r.
-000028c0: 0000 0072 3100 0000 72dc 0000 00da 066f  ...r1...r......o
-000028d0: 6666 6963 6572 a500 0000 726c 0000 0072  fficer....rl...r
-000028e0: 5000 0000 7243 0000 0072 4300 0000 7244  P...rC...rC...rD
-000028f0: 0000 00da 0d69 6d70 6f72 745f 6f66 6669  .....import_offi
-00002900: 6365 6601 0000 7384 0000 0000 030c 010e  cef...s.........
-00002910: 011a 0204 020a 0204 0114 0108 010a 0106  ................
-00002920: 0110 010a 0104 020e 010c 0114 0108 0108  ................
-00002930: 0108 0110 0108 0106 0112 0204 0108 0108  ................
-00002940: 0108 030e 0106 010a 0102 0102 0102 0102  ................
-00002950: 0102 0102 0108 0102 f80c 0b0a 0102 0102  ................
-00002960: 0102 0102 0102 0102 0108 0102 f80a 0b02  ................
-00002970: 0102 0102 0102 0102 0102 0102 0108 0102  ................
-00002980: f706 0b12 0110 011a 0206 010a 0208 0172  ...............r
-00002990: e000 0000 6301 0000 0000 0000 0000 0000  ....c...........
-000029a0: 0031 0000 0013 0000 0043 0000 0073 9e04  .1.......C...s..
-000029b0: 0000 7c00 6a00 a001 6401 a101 7d01 7c00  ..|.j...d...}.|.
-000029c0: 6a02 a001 6402 6403 a102 7d02 7c02 6a03  j...d.d...}.|.j.
-000029d0: a004 6404 a101 6405 1900 a004 6406 a101  ..d...d.....d...
-000029e0: 6407 1900 7d03 6700 7d04 7c03 6408 7600  d...}.g.}.|.d.v.
-000029f0: 9004 727e 9004 7a0e 7405 6a06 6409 7c02  ..r~..z.t.j.d.|.
-00002a00: a007 a100 640a 640b 8d03 7d05 7c05 a008  ....d.d...}.|...
-00002a10: a100 7d06 7c06 4400 9003 5de6 7d07 7c07  ..}.|.D...].}.|.
-00002a20: 6a09 7d08 740a 640c 7c08 8302 4400 9003  j.}.t.d.|...D...
-00002a30: 5dce 7d09 7c07 a00b 7c09 a101 7d0a 7c0a  ].}.|...|...}.|.
-00002a40: 727c 7c07 a00c 7c09 640c a102 6a0d 7d0b  r||...|.d...j.}.
-00002a50: 7c07 a00e 7c09 640c a102 7d0c 7c0b 640c  |...|.d...}.|.d.
-00002a60: 6b02 72c6 7c0c 6405 1600 6407 6b02 72c6  k.r.|.d...d.k.r.
-00002a70: 740f 7c0c 8301 7d0c 7c0a 640d 1900 7d0d  t.|...}.|.d...}.
-00002a80: 7c0a 6407 1900 7d0e 7410 6a11 6a12 7c0e  |.d...}.t.j.j.|.
-00002a90: 640e 8d01 a013 a100 7d0f 7c0f 72f4 7c0f  d.......}.|.r.|.
-00002aa0: 6a14 7d10 6e26 7c0c 7c0d 7c0e 6409 6409  j.}.n&|.|.|.d.d.
-00002ab0: 6409 6409 6409 7c01 640f 6410 9c0a 7d11  d.d.d.|.d.d...}.
-00002ac0: 7c04 a015 7c11 a101 0100 717c 7c0a 6405  |...|.....q||.d.
-00002ad0: 1900 7d12 7c12 9001 726e 7416 6a11 6a12  ..}.|...rnt.j.j.
-00002ae0: 7c12 7c10 6411 8d02 a013 a100 7d13 7c13  |.|.d.......}.|.
-00002af0: 9001 724a 7c13 6a14 7d14 6e24 7c0c 7c0d  ..rJ|.j.}.n$|.|.
-00002b00: 7c0e 7c12 6409 6409 6409 7c01 6412 6413  |.|.d.d.d.|.d.d.
-00002b10: 9c09 7d11 7c04 a015 7c11 a101 0100 717c  ..}.|...|.....q|
-00002b20: 7c0a 6414 1900 7d15 7c15 9001 72a0 7c15  |.d...}.|...r.|.
-00002b30: 6415 6b02 9001 728c 6416 7d16 6e14 7c15  d.k...r.d.}.n.|.
-00002b40: 6417 6b02 9001 729c 6418 7d16 6e04 6409  d.k...r.d.}.n.d.
-00002b50: 7d16 7c0a 6419 1900 7d17 7c17 9001 72b6  }.|.d...}.|...r.
-00002b60: 740f 7c17 8301 7d18 7c0a 641a 1900 7d19  t.|...}.|.d...}.
-00002b70: 7c19 9001 72cc 740f 7c19 8301 7d1a 7c0a  |...r.t.|...}.|.
-00002b80: 641b 1900 7d1b 7c1b 9002 7220 7417 6a11  d...}.|...r t.j.
-00002b90: 6a12 7c1b 7c10 6411 8d02 a013 a100 7d1c  j.|.|.d.......}.
-00002ba0: 7c1c 9001 72fc 7c1c 6a14 7d1d 6e24 7c0c  |...r.|.j.}.n$|.
-00002bb0: 7c0d 7c0e 7c12 7c1b 6409 6409 7c01 641c  |.|.|.|.d.d.|.d.
-00002bc0: 6413 9c09 7d11 7c04 a015 7c11 a101 0100  d...}.|...|.....
-00002bd0: 717c 7c0a 641d 1900 7d1e 7c0a 641e 1900  q||.d...}.|.d...
-00002be0: 7d1f 7c1f 641f 6b02 9002 7240 640a 7d20  }.|.d.k...r@d.} 
-00002bf0: 6e04 6420 7d20 7418 6a11 6a12 7c0c 6421  n.d } t.j.j.|.d!
-00002c00: 8d01 7d21 7c21 9002 7290 7c21 6a19 6600  ..}!|!..r.|!j.f.
-00002c10: 6900 7c0c 7c0d 7c10 7c14 7c1d 7c1c 6a03  i.|.|.|.|.|.|.j.
-00002c20: 7c1e 7c16 7c18 7c1a 7c20 741a 6a1a a01b  |.|.|.|.| t.j...
-00002c30: a100 7c01 6422 9c0d a401 8e01 0100 9001  ..|.d"..........
-00002c40: 6e94 7c21 6a1c 6600 6900 7c0c 7c0d 7c10  n.|!j.f.i.|.|.|.
-00002c50: 7c14 7c1d 7c1c 6a03 7c1e 7c16 7c18 7c1a  |.|.|.j.|.|.|.|.
-00002c60: 7c20 741a 6a1a a01b a100 7c01 6423 9c0d  | t.j.....|.d#..
-00002c70: a401 8e01 7d22 741d 6a11 6a1c 6600 6900  ....}"t.j.j.f.i.
-00002c80: 7c0d 7c0c 6424 741e 6425 8301 7c22 6a14  |.|.d$t.d%..|"j.
-00002c90: 7c10 7c14 7c1d 7c16 7c18 7c1a 7c01 6426  |.|.|.|.|.|.|.d&
-00002ca0: 9c0c a401 8e01 0100 7c20 9004 7224 741f  ........| ..r$t.
-00002cb0: 7c0e 8301 7d23 741f 7c1b 8301 7d24 6427  |...}#t.|...}$d'
-00002cc0: 7c23 9b00 6428 7c24 9b00 9d04 7d25 7420  |#..d(|$....}%t 
-00002cd0: 6a11 6a12 7c25 7c10 6429 8d02 a013 a100  j.j.|%|.d)......
-00002ce0: 7d26 642a 7c23 9b00 6428 7c24 9b00 9d04  }&d*|#..d(|$....
-00002cf0: 7d27 7420 6a11 6a12 7c27 7c10 6429 8d02  }'t j.j.|'|.d)..
-00002d00: a013 a100 7d28 642b 7c23 9b00 6428 7c24  ....}(d+|#..d(|$
-00002d10: 9b00 9d04 7d29 7420 6a11 6a12 7c29 7c10  ....})t j.j.|)|.
-00002d20: 6429 8d02 a013 a100 7d2a 642c 7c23 9b00  d)......}*d,|#..
-00002d30: 6428 7c24 9b00 9d04 7d2b 7420 6a11 6a12  d(|$....}+t j.j.
-00002d40: 7c2b 7c10 6429 8d02 a013 a100 7d2c 7c26  |+|.d)......},|&
-00002d50: 9003 73b4 7c28 9003 73b4 7c2a 9003 73b4  ..s.|(..s.|*..s.
-00002d60: 7c2c 9003 72fa 6700 7d2d 7c2d a015 7c26  |,..r.g.}-|-..|&
-00002d70: a101 0100 7c2d a015 7c28 a101 0100 7c2d  ....|-..|(....|-
-00002d80: a015 7c2a a101 0100 7c2d a015 7c2c a101  ..|*....|-..|,..
-00002d90: 0100 7c2d 4400 5d12 7d2e 7c2e 6a21 a022  ..|-D.].}.|.j!."
-00002da0: 7c22 a101 0100 9003 71e4 6e2a 7c0c 7c0d  |"......q.n*|.|.
-00002db0: 7c0e 7c12 7c1b 7c1f 741a 6a1a a01b a100  |.|.|.|.t.j.....
-00002dc0: 7c01 642d 6413 9c09 7d11 7c04 a015 7c11  |.d-d...}.|...|.
-00002dd0: a101 0100 717c 7c0c 7c0d 7c0e 7c12 7c1b  ....q||.|.|.|.|.
-00002de0: 7c1f 741a 6a1a a01b a100 7c01 642e 6413  |.t.j.....|.d.d.
-00002df0: 9c09 7d11 7c04 a015 7c11 a101 0100 717c  ..}.|...|.....q|
-00002e00: 7166 5700 6e2a 0400 7423 9004 797c 0100  qfW.n*..t#..y|..
-00002e10: 7d2f 0100 7a10 7c2f 8201 5700 5900 6409  }/..z.|/..W.Y.d.
-00002e20: 7d2f 7e2f 6e0a 6409 7d2f 7e2f 3000 3000  }/~/n.d.}/~/0.0.
-00002e30: 7c04 9004 728e 642f 7c04 6901 7d30 6e08  |...r.d/|.i.}0n.
-00002e40: 642f 6430 6901 7d30 7424 7c30 8301 5300  d/d0i.}0t$|0..S.
-00002e50: 2931 751a 0000 00e5 afbc e585 a565 7863  )1u..........exc
-00002e60: 656c e8a1 a8e5 8cbb e794 9fe6 95b0 e68d  el..............
-00002e70: ae72 7900 0000 727a 0000 0072 7b00 0000  .ry...rz...r{...
-00002e80: 727c 0000 0072 7d00 0000 727e 0000 0072  r|...r}...r~...r
-00002e90: 0100 0000 727f 0000 004e 5472 8100 0000  ....r....NTr....
-00002ea0: 7284 0000 0072 8700 0000 7285 0000 0075  r....r....r....u
-00002eb0: 2700 0000 e58c bbe9 99a2 e69f a5e8 afa2  '...............
-00002ec0: e69c 89e8 afaf efbc 8ce8 afb7 e6a3 80e6  ................
-00002ed0: 9fa5 efbc 81ef bc81 efbc 8129 0ada 0a6a  ...........)...j
-00002ee0: 6f62 5f6e 756d 6265 7272 8600 0000 728b  ob_numberr....r.
-00002ef0: 0000 00da 0b6f 6666 6963 655f 6e61 6d65  .....office_name
-00002f00: da0d 646f 635f 7261 6e6b 5f6e 616d 65da  ..doc_rank_name.
-00002f10: 0864 6573 6372 6962 65da 1169 735f 6f6e  .describe..is_on
-00002f20: 6c69 6e65 5f63 6f6e 7375 6c74 728c 0000  line_consultr...
-00002f30: 0072 8d00 0000 da03 6d73 6729 0272 8600  .r......msg).r..
-00002f40: 0000 72d9 0000 0075 6300 0000 e8af a5e6  ..r....uc.......
-00002f50: 9da1 e8ae b0e5 bd95 e58c bbe9 99a2 e4b8  ................
-00002f60: 8be7 9a84 e7a7 91e5 aea4 e69f a5e8 afa2  ................
-00002f70: e69c 89e8 afaf efbc 8ce8 afb7 e6a3 80e6  ................
-00002f80: 9fa5 efbc 81ef bc81 efbc 81e5 b7b2 e887  ................
-00002f90: aae5 8aa8 e8b7 b3e8 bf87 e8af a5e6 9da1  ................
-00002fa0: e8ae b0e5 bd95 e79a 84e5 afbc e585 a529  ...............)
-00002fb0: 0972 e100 0000 7286 0000 0072 8b00 0000  .r....r....r....
-00002fc0: 72e2 0000 0072 e300 0000 72e5 0000 0072  r....r....r....r
-00002fd0: 8c00 0000 728d 0000 0072 e600 0000 7288  ....r....r....r.
-00002fe0: 0000 0075 0300 0000 e794 b7da 0131 7503  ...u.........1u.
-00002ff0: 0000 00e5 a5b3 da01 3072 d700 0000 72d8  ........0r....r.
-00003000: 0000 00e9 0700 0000 7563 0000 00e8 afa5  ........uc......
-00003010: e69d a1e8 aeb0 e5bd 95e5 8cbb e999 a2e4  ................
-00003020: b88b e79a 84e8 818c e7a7 b0e6 9fa5 e8af  ................
-00003030: a2e6 9c89 e8af afef bc8c e8af b7e6 a380  ................
-00003040: e69f a5ef bc81 efbc 81ef bc81 e5b7 b2e8  ................
-00003050: 87aa e58a a8e8 b7b3 e8bf 87e8 afa5 e69d  ................
-00003060: a1e8 aeb0 e5bd 95e7 9a84 e5af bce5 85a5  ................
-00003070: e908 0000 00e9 0900 0000 f503 0000 00e6  ................
-00003080: 98af 4629 0172 e100 0000 290d 72e1 0000  ..F).r....).r...
-00003090: 0072 8600 0000 72d9 0000 00da 096f 6666  .r....r......off
-000030a0: 6963 655f 6964 da0b 646f 635f 7261 6e6b  ice_id..doc_rank
-000030b0: 5f69 64da 0870 6f73 6974 696f 6e72 e400  _id..positionr..
-000030c0: 0000 72a8 0000 0072 3100 0000 da05 6964  ..r....r1.....id
-000030d0: 6e75 6d72 e500 0000 da0c 7570 6461 7465  numr......update
-000030e0: 645f 7469 6d65 728d 0000 0029 0d72 e100  d_timer....).r..
-000030f0: 0000 7286 0000 0072 d900 0000 72ed 0000  ..r....r....r...
-00003100: 0072 ee00 0000 72ef 0000 0072 e400 0000  .r....r....r....
-00003110: 72a8 0000 0072 3100 0000 72f0 0000 0072  r....r1...r....r
-00003120: e500 0000 728c 0000 0072 8d00 0000 7a0a  ....r....r....z.
-00003130: 3131 3140 7171 2e63 6f6d 7234 0000 0029  111@qq.comr4...)
-00003140: 0c72 8600 0000 7232 0000 00da 0565 6d61  .r....r2.....ema
-00003150: 696c 7247 0000 00da 0964 6f63 746f 725f  ilrG.....doctor_
-00003160: 6964 72d9 0000 0072 ed00 0000 5a0c 7573  idr....r....Z.us
-00003170: 6572 5f72 616e 6b5f 6964 72a8 0000 0072  er_rank_idr....r
-00003180: 3100 0000 da09 6964 6361 7264 6e75 6d72  1.....idcardnumr
-00003190: 8d00 0000 5a02 315f da01 5f29 02da 0d73  ....Z.1_.._)...s
-000031a0: 7461 6e64 6172 645f 636f 6465 72d9 0000  tandard_coder...
-000031b0: 005a 0232 5f5a 0233 5f5a 0234 5f75 6000  .Z.2_Z.3_Z.4_u`.
-000031c0: 0000 e688 90e5 8a9f efbc 81e4 bd86 e698  ................
-000031d0: afe8 b4b9 e794 a8e6 a087 e587 86e6 9fa5  ................
-000031e0: e8af a2e5 87ba e994 99ef bc81 efbc 81ef  ................
-000031f0: bc81 e8af b7e6 898b e58a a8e4 b8ba e8af  ................
-00003200: a5e5 8cbb e794 9fe6 b7bb e58a a0e8 b4b9  ................
-00003210: e794 a8e6 a087 e587 86ef bc81 efbc 81ef  ................
-00003220: bc81 750f 0000 00e6 8890 e58a 9fef bc81  ..u.............
-00003230: efbc 81ef bc81 7235 0000 0072 8e00 0000  ......r5...r....
-00003240: 2925 722f 0000 0072 4a00 0000 728f 0000  )%r/...rJ...r...
-00003250: 0072 8600 0000 7290 0000 0072 dd00 0000  .r....r....r....
-00003260: 7292 0000 0072 9300 0000 7294 0000 0072  r....r....r....r
-00003270: 9500 0000 7296 0000 0072 9700 0000 7298  ....r....r....r.
-00003280: 0000 0072 9900 0000 729a 0000 0072 9b00  ...r....r....r..
-00003290: 0000 7211 0000 0072 3b00 0000 723c 0000  ..r....r;...r<..
-000032a0: 0072 3d00 0000 7248 0000 0072 9e00 0000  .r=...rH...r....
-000032b0: 7212 0000 0072 1400 0000 7213 0000 0072  r....r....r....r
-000032c0: 9c00 0000 724c 0000 0072 4d00 0000 729d  ....rL...rM...r.
-000032d0: 0000 0072 1500 0000 7203 0000 00da 1367  ...r....r......g
-000032e0: 6574 5f70 696e 7969 6e5f 696e 6974 6961  et_pinyin_initia
-000032f0: 6c73 721b 0000 00da 0764 6f63 746f 7273  lsr......doctors
-00003300: da03 6164 6472 6600 0000 7206 0000 0029  ..addrf...r....)
-00003310: 3172 4100 0000 7279 0000 0072 7a00 0000  1rA...ry...rz...
-00003320: 729f 0000 0072 a000 0000 7235 0000 0072  r....r....r5...r
-00003330: 9400 0000 72a1 0000 0072 a200 0000 72a3  ....r....r....r.
-00003340: 0000 0072 9700 0000 7299 0000 0072 e100  ...r....r....r..
-00003350: 0000 7286 0000 0072 a400 0000 728b 0000  ..r....r....r...
-00003360: 0072 d900 0000 72a5 0000 0072 e200 0000  .r....r....r....
-00003370: 72df 0000 0072 ed00 0000 72a8 0000 005a  r....r....r....Z
-00003380: 0b67 656e 6465 725f 766c 7565 7231 0000  .gender_vluer1..
-00003390: 005a 0970 686f 6e65 5f69 6e74 72f0 0000  .Z.phone_intr...
-000033a0: 005a 0969 646e 756d 5f69 6e74 72e3 0000  .Z.idnum_intr...
-000033b0: 005a 0864 6f63 5f72 616e 6b72 ee00 0000  .Z.doc_rankr....
-000033c0: 72e4 0000 0072 e500 0000 5a07 6973 5f74  r....r....Z.is_t
-000033d0: 7275 65da 0664 6f63 746f 725a 0764 6f63  rue..doctorZ.doc
-000033e0: 746f 7231 5a10 496e 6974 6961 6c5f 686f  tor1Z.Initial_ho
-000033f0: 7370 6974 616c 5a10 496e 6974 6961 6c5f  spitalZ.Initial_
-00003400: 646f 635f 7261 6e6b 5a0f 636f 6d62 696e  doc_rankZ.combin
-00003410: 6174 696f 6e5f 6864 315a 0465 735f 315a  ation_hd1Z.es_1Z
-00003420: 0f63 6f6d 6269 6e61 7469 6f6e 5f68 6432  .combination_hd2
-00003430: 5a04 6573 5f32 5a0f 636f 6d62 696e 6174  Z.es_2Z.combinat
-00003440: 696f 6e5f 6864 335a 0465 735f 335a 0f63  ion_hd3Z.es_3Z.c
-00003450: 6f6d 6269 6e61 7469 6f6e 5f68 6434 5a04  ombination_hd4Z.
-00003460: 6573 5f34 5a07 6573 5f6c 6973 74da 0265  es_4Z.es_list..e
-00003470: 7372 6c00 0000 7250 0000 0072 4300 0000  srl...rP...rC...
-00003480: 7243 0000 0072 4400 0000 da0d 696d 706f  rC...rD.....impo
-00003490: 7274 5f64 6f63 746f 72b8 0100 0073 7601  rt_doctor....sv.
-000034a0: 0000 0003 0c01 0e01 1a02 0402 0a02 0401  ................
-000034b0: 1401 0801 0a01 0601 1001 0a01 0402 0e01  ................
-000034c0: 0c01 1401 0801 0801 0801 1201 0401 0803  ................
-000034d0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000034e0: 0201 02f6 060c 0a01 0202 0801 0601 1401  ................
-000034f0: 0601 0803 0201 0201 0201 0201 0201 0201  ................
-00003500: 0201 0201 02f7 060b 0a01 0201 0801 0601  ................
-00003510: 0a01 0601 0a01 0602 0401 0801 0601 0801  ................
-00003520: 0801 0601 0801 0801 0601 1401 0601 0803  ................
-00003530: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00003540: 02f7 060b 0a01 0201 0801 0801 0a01 0602  ................
-00003550: 0401 0e01 0601 0a01 0201 0201 0201 0201  ................
-00003560: 0401 0201 0201 0201 0201 0201 0801 02f4  ................
-00003570: 0e0f 0a01 0201 0201 0201 0201 0401 0201  ................
-00003580: 0201 0201 0201 0201 0801 02f4 0a0f 0a01  ................
-00003590: 0201 0201 0201 0601 0401 0201 0201 0201  ................
-000035a0: 0201 0201 0203 02f2 0a10 0601 0801 0801  ................
-000035b0: 1001 0801 02ff 0a02 1001 0801 02ff 0a02  ................
-000035c0: 1001 0801 02ff 0a02 1001 0801 02ff 0a02  ................
-000035d0: 1801 0401 0a01 0a01 0a01 0a01 0801 1203  ................
-000035e0: 0201 0201 0201 0201 0201 0201 0801 0201  ................
-000035f0: 02f7 060b 0a01 0202 0201 0201 0201 0201  ................
-00003600: 0201 0201 0801 0201 02f7 060b 1201 1001  ................
-00003610: 1a02 0601 0a02 0801 72fc 0000 0063 0100  ........r....c..
-00003620: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00003630: 0000 4300 0000 7316 0000 0074 006a 017c  ..C...s....t.j.|
-00003640: 0064 0164 028d 02a0 02a1 007d 017c 0153  .d.d.......}.|.S
-00003650: 0029 034e 727b 0000 0029 01da 0964 656c  .).Nr{...)...del
-00003660: 696d 6974 6572 2903 da06 7069 6e79 696e  imiter)...pinyin
-00003670: da0b 6765 745f 696e 6974 6961 6cda 0575  ..get_initial..u
-00003680: 7070 6572 2902 7286 0000 005a 0a73 616d  pper).r....Z.sam
-00003690: 706c 656e 616d 6572 4300 0000 7243 0000  plenamerC...rC..
-000036a0: 0072 4400 0000 72f7 0000 008b 0200 0073  .rD...r........s
-000036b0: 0400 0000 0001 1201 72f7 0000 0063 0000  ........r....c..
-000036c0: 0000 0000 0000 0000 0000 0000 0000 0400  ................
-000036d0: 0000 4000 0000 7320 0100 0065 005a 0164  ..@...s ...e.Z.d
-000036e0: 005a 0265 036a 0464 0164 0264 038d 025a  .Z.e.j.d.d.d...Z
-000036f0: 0565 036a 0464 0464 0264 038d 025a 0665  .e.j.d.d.d...Z.e
-00003700: 036a 0464 0564 0264 038d 025a 0765 036a  .j.d.d.d...Z.e.j
-00003710: 0464 0664 0264 038d 025a 0865 036a 0464  .d.d.d...Z.e.j.d
-00003720: 0764 0264 038d 025a 0965 036a 0464 0864  .d.d...Z.e.j.d.d
-00003730: 0264 038d 025a 0a65 036a 0464 0964 0264  .d...Z.e.j.d.d.d
-00003740: 038d 025a 0b65 036a 0464 0a64 0264 038d  ...Z.e.j.d.d.d..
-00003750: 025a 0c65 036a 0464 0b64 0264 038d 025a  .Z.e.j.d.d.d...Z
-00003760: 0d65 036a 0464 0c64 0264 038d 025a 0e65  .e.j.d.d.d...Z.e
-00003770: 036a 0464 0d64 0264 038d 025a 0f65 036a  .j.d.d.d...Z.e.j
-00003780: 0464 0e64 0264 038d 025a 1065 036a 1164  .d.d.d...Z.e.j.d
-00003790: 0f64 108d 015a 1265 036a 0464 1164 0264  .d...Z.e.j.d.d.d
-000037a0: 038d 025a 1365 036a 0464 1264 0264 038d  ...Z.e.j.d.d.d..
-000037b0: 025a 1465 036a 0464 1364 0264 038d 025a  .Z.e.j.d.d.d...Z
-000037c0: 1565 036a 0464 1464 0264 038d 025a 1665  .e.j.d.d.d...Z.e
-000037d0: 036a 0464 1564 0264 038d 025a 1765 036a  .j.d.d.d...Z.e.j
-000037e0: 1164 1664 108d 015a 1847 0064 1764 1884  .d.d...Z.G.d.d..
-000037f0: 0064 1883 025a 1964 1953 0029 1ada 1344  .d...Z.d.S.)...D
-00003800: 7275 6744 6972 6563 746f 7279 4669 6c74  rugDirectoryFilt
-00003810: 6572 da09 6472 7567 5f63 6f64 6572 ab00  er..drug_coder..
-00003820: 0000 72ac 0000 00da 0964 7275 675f 6e61  ..r......drug_na
-00003830: 6d65 da09 7374 616e 6461 7264 73da 0c6d  me..standards..m
-00003840: 6561 7375 7265 5f75 6e69 745a 1670 7265  easure_unitZ.pre
-00003850: 7061 7261 7469 6f6e 5f74 7970 655f 5f6e  paration_type__n
-00003860: 616d 655a 0e63 6174 6567 6f72 795f 5f6e  ameZ.category__n
-00003870: 616d 655a 0f64 7275 675f 7479 7065 5f5f  ameZ.drug_type__
-00003880: 6e61 6d65 da09 756e 6974 5f64 6f73 65da  name..unit_dose.
-00003890: 0a73 746f 636b 5f6c 6566 74da 0a73 746f  .stock_left..sto
-000038a0: 636b 5f75 6e69 74da 036d 6963 da0c 7263  ck_unit..mic..rc
-000038b0: 635f 6361 7465 676f 7279 da0c 6973 5f65  c_category..is_e
-000038c0: 7373 656e 7469 616c 72a9 0000 00da 0868  ssentialr......h
-000038d0: 725f 6c65 7665 6cda 0767 625f 636f 6465  r_level..gb_code
-000038e0: da07 6762 5f6e 616d 65da 0c6f 7269 6769  ..gb_name..origi
-000038f0: 6e5f 706c 6163 65da 0c6d 616e 7566 6163  n_place..manufac
-00003900: 7475 7265 7272 3e00 0000 6300 0000 0000  turerr>...c.....
-00003910: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
-00003920: 0000 0073 1400 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00003930: 6503 5a04 6401 5a05 6402 5300 2903 7a18  e.Z.d.Z.d.S.).z.
-00003940: 4472 7567 4469 7265 6374 6f72 7946 696c  DrugDirectoryFil
-00003950: 7465 722e 4d65 7461 72af 0000 004e 2906  ter.Metar....N).
-00003960: 725b 0000 0072 5c00 0000 725d 0000 0072  r[...r\...r]...r
-00003970: 1900 0000 72b0 0000 0072 b100 0000 7243  ....r....r....rC
-00003980: 0000 0072 4300 0000 7243 0000 0072 4400  ...rC...rC...rD.
-00003990: 0000 72b2 0000 00ac 0200 0073 0400 0000  ..r........s....
-000039a0: 0801 0401 72b2 0000 004e 291a 725b 0000  ....r....N).r[..
-000039b0: 0072 5c00 0000 725d 0000 0072 b300 0000  .r\...r]...r....
-000039c0: 72b5 0000 0072 0201 0000 7203 0100 005a  r....r....r....Z
-000039d0: 0d73 7065 6369 6669 6361 7469 6f6e 7205  .specificationr.
-000039e0: 0100 00da 1070 7265 7061 7261 7469 6f6e  .....preparation
-000039f0: 5f74 7970 65da 0863 6174 6567 6f72 79da  _type..category.
-00003a00: 0964 7275 675f 7479 7065 7206 0100 0072  .drug_typer....r
-00003a10: 0701 0000 7208 0100 0072 0901 0000 720a  ....r....r....r.
-00003a20: 0100 00da 0d42 6f6f 6c65 616e 4669 6c74  .....BooleanFilt
-00003a30: 6572 720b 0100 0072 0c01 0000 720d 0100  err....r....r...
-00003a40: 0072 0e01 0000 720f 0100 0072 1001 0000  .r....r....r....
-00003a50: 723e 0000 0072 b200 0000 7243 0000 0072  r>...r....rC...r
-00003a60: 4300 0000 7243 0000 0072 4400 0000 7201  C...rC...rD...r.
-00003a70: 0100 0097 0200 0073 2800 0000 0801 0e01  .......s(.......
-00003a80: 0e01 0e01 0e01 0e01 0e01 0e01 0e01 0e01  ................
-00003a90: 0e01 0e01 0e01 0c01 0e01 0e01 0e01 0e01  ................
-00003aa0: 0e01 0c02 7201 0100 0063 0100 0000 0000  ....r....c......
-00003ab0: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
-00003ac0: 0000 7320 0000 0064 017d 017c 0144 005d  ..s ...d.}.|.D.]
-00003ad0: 127d 027c 027c 0076 0072 0801 0064 0253  .}.|.|.v.r...d.S
-00003ae0: 0071 0864 0353 0029 044e 751d 0000 007e  .q.d.S.).Nu....~
-00003af0: 2140 2324 255e 262a 2829 2b2d 2a2f 3c3e  !@#$%^&*()+-*/<>
-00003b00: 2c2e 5b5d 5c2f 7c27 60e3 8081 5446 7243  ,.[]\/|'`...TFrC
-00003b10: 0000 0029 03da 076b 6579 776f 7264 da07  ...)...keyword..
-00003b20: 7379 6d62 6f6c 73da 0673 796d 626f 6c72  symbols..symbolr
-00003b30: 4300 0000 7243 0000 0072 4400 0000 da11  C...rC...rD.....
-00003b40: 6966 5f63 6f6e 7461 696e 5f73 796d 626f  if_contain_symbo
-00003b50: 6cb1 0200 0073 0a00 0000 0001 0401 0801  l....s..........
-00003b60: 0801 0802 7218 0100 0063 0000 0000 0000  ....r....c......
-00003b70: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-00003b80: 0000 732c 0000 0065 005a 0164 005a 0265  ..s,...e.Z.d.Z.e
-00003b90: 036a 04a0 05a1 00a0 0664 01a1 015a 0765  .j.......d...Z.e
-00003ba0: 085a 0965 0a5a 0b64 0264 0384 005a 0c64  .Z.e.Z.d.d...Z.d
-00003bb0: 0453 0029 05da 1444 7275 6744 6972 6563  .S.)...DrugDirec
-00003bc0: 746f 7279 5669 6577 5365 7472 b700 0000  toryViewSetr....
-00003bd0: 6302 0000 0000 0000 0000 0000 0012 0000  c...............
-00003be0: 0007 0000 004f 0000 0073 2801 0000 7c00  .....O...s(...|.
-00003bf0: 6a00 6a01 a002 6401 a101 7d04 7c00 6a00  j.j...d...}.|.j.
-00003c00: 6a01 a002 6402 a101 7d05 7c00 6a00 6a01  j...d...}.|.j.j.
-00003c10: a002 6403 a101 7d06 7c00 6a00 6a01 a002  ..d...}.|.j.j...
-00003c20: 6404 a101 7d07 7403 7c05 8301 7d08 7c08  d...}.t.|...}.|.
-00003c30: 7250 7404 6405 6406 6407 8d02 5300 6408  rPt.d.d.d...S.d.
-00003c40: 7d09 7c09 72d0 7c04 6409 640a 7c05 7c06  }.|.r.|.d.d.|.|.
-00003c50: 7c07 640b 9c06 7d0a 7405 8300 7d0b 7c0b  |.d...}.t...}.|.
-00003c60: a006 7c0a 640c a102 7d0c 7c0c 640d 1900  ..|.d...}.|.d...
-00003c70: 640e 6b02 72be 7407 640f 8301 0100 7c0c  d.k.r.t.d.....|.
-00003c80: 6410 1900 6411 1900 7d0d 7c0c 6410 1900  d...d...}.|.d...
-00003c90: 6412 1900 7d0e 7c0e 6413 1900 7c0d 6414  d...}.|.d...|.d.
-00003ca0: 9c02 7d0f 7404 7c0f 8301 5300 7407 6415  ..}.t.|...S.t.d.
-00003cb0: 8301 0100 7404 7c0c 8301 5300 6e54 7c00  ....t.|...S.nT|.
-00003cc0: a008 7c00 a009 a100 a101 7d10 7c00 a00a  ..|.......}.|...
-00003cd0: 7c10 a101 7d06 7c06 6400 7501 9001 720c  |...}.|.d.u...r.
-00003ce0: 7c00 6a0b 7c06 6416 6417 8d02 7d11 7c00  |.j.|.d.d...}.|.
-00003cf0: a00c 7c11 6a0d a101 5300 7c00 6a0b 7c10  ..|.j...S.|.j.|.
-00003d00: 6416 6417 8d02 7d11 7404 7c11 6a0d 8301  d.d...}.t.|.j...
-00003d10: 5300 6400 5300 2918 4e72 ce00 0000 7203  S.d.S.).Nr....r.
-00003d20: 0100 00da 0470 6167 65da 0970 6167 655f  .....page..page_
-00003d30: 7369 7a65 750f 0000 00e5 8f82 e695 b0e9  sizeu...........
-00003d40: 9499 e8af afef bc81 6990 0100 0072 be00  ........i....r..
-00003d50: 0000 727d 0000 00da 044e 616d 65da 0230  ..r}.....Name..0
-00003d60: 3329 0672 ce00 0000 5a0a 436f 6465 5f66  3).r....Z.Code_f
-00003d70: 6965 6c64 5a09 436f 6465 5f6f 7065 725a  ieldZ.Code_operZ
-00003d80: 0b56 616c 7565 5f66 6965 6c64 5a09 5061  .Value_fieldZ.Pa
-00003d90: 6765 696e 6465 785a 0850 6167 6573 697a  geindexZ.Pagesiz
-00003da0: 655a 0659 5044 4143 58da 0463 6f64 65e9  eZ.YPDACX..code.
-00003db0: c800 0000 7512 0000 00e8 8daf e593 81e6  ....u...........
-00003dc0: 9fa5 e8af a2e6 8890 e58a 9fda 0763 6f6e  .............con
-00003dd0: 7465 6e74 7235 0000 005a 0870 6167 6569  tentr5...Z.pagei
-00003de0: 6e66 6f5a 0c72 6563 6f72 6473 636f 756e  nfoZ.recordscoun
-00003df0: 7429 02da 0563 6f75 6e74 da07 7265 7375  t)...count..resu
-00003e00: 6c74 7375 1200 0000 e88d afe5 9381 e69f  ltsu............
-00003e10: a5e8 afa2 e5a4 b1e8 b4a5 5429 01da 046d  ..........T)...m
-00003e20: 616e 7929 0e72 4100 0000 da0c 7175 6572  any).rA.....quer
-00003e30: 795f 7061 7261 6d73 724a 0000 0072 1801  y_paramsrJ...r..
-00003e40: 0000 720e 0000 0072 1c00 0000 da09 7772  ..r....r......wr
-00003e50: 6974 6562 6163 6b72 4900 0000 da0f 6669  itebackrI.....fi
-00003e60: 6c74 6572 5f71 7565 7279 7365 7472 5a00  lter_querysetrZ.
-00003e70: 0000 da11 7061 6769 6e61 7465 5f71 7565  ....paginate_que
-00003e80: 7279 7365 74da 0e67 6574 5f73 6572 6961  ryset..get_seria
-00003e90: 6c69 7a65 72da 1667 6574 5f70 6167 696e  lizer..get_pagin
-00003ea0: 6174 6564 5f72 6573 706f 6e73 6572 3500  ated_responser5.
-00003eb0: 0000 2912 7253 0000 0072 4100 0000 da04  ..).rS...rA.....
-00003ec0: 6172 6773 7268 0000 0072 ce00 0000 7203  argsrh...r....r.
-00003ed0: 0100 0072 1a01 0000 721b 0100 0072 1701  ...r....r....r..
-00003ee0: 0000 da04 666c 6167 da07 696e 5f64 6174  ....flag..in_dat
-00003ef0: 615a 0861 7069 5f69 6e66 6fda 0472 6573  aZ.api_info..res
-00003f00: 745a 0972 6573 745f 6461 7461 5a09 7061  tZ.rest_dataZ.pa
-00003f10: 6765 5f69 6e66 6f5a 0972 6573 745f 6469  ge_infoZ.rest_di
-00003f20: 6374 72c4 0000 0072 c200 0000 7243 0000  ctr....r....rC..
-00003f30: 0072 4300 0000 7244 0000 00da 046c 6973  .rC...rD.....lis
-00003f40: 74bf 0200 0073 4200 0000 0001 0e01 0e01  t....sB.........
-00003f50: 0e01 0e01 0801 0401 0c01 0401 0402 0201  ................
-00003f60: 0201 0201 0201 0201 02fa 0608 0601 0c01  ................
-00003f70: 0c01 0801 0c01 0c01 0e01 0802 0801 0a02  ................
-00003f80: 0e02 0a01 0a01 0e01 0c02 0e01 7a19 4472  ............z.Dr
-00003f90: 7567 4469 7265 6374 6f72 7956 6965 7753  ugDirectoryViewS
-00003fa0: 6574 2e6c 6973 744e 290d 725b 0000 0072  et.listN).r[...r
-00003fb0: 5c00 0000 725d 0000 0072 1900 0000 723b  \...r]...r....r;
-00003fc0: 0000 0072 5600 0000 72c3 0000 0072 c400  ...rV...r....r..
-00003fd0: 0000 7228 0000 0072 5f00 0000 7201 0100  ..r(...r_...r...
-00003fe0: 0072 c500 0000 722e 0100 0072 4300 0000  .r....r....rC...
-00003ff0: 7243 0000 0072 4300 0000 7244 0000 0072  rC...rC...rD...r
-00004000: 1901 0000 ba02 0000 7308 0000 0008 0110  ........s.......
-00004010: 0104 0104 0272 1901 0000 6300 0000 0000  .....r....c.....
-00004020: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
-00004030: 0000 0073 2000 0000 6500 5a01 6400 5a02  ...s ...e.Z.d.Z.
-00004040: 6503 6a04 a005 a100 a006 6401 a101 5a07  e.j.......d...Z.
-00004050: 6508 5a09 6402 5300 2903 da0e 4170 6949  e.Z.d.S.)...ApiI
-00004060: 6e66 6f56 6965 7753 6574 72b7 0000 004e  nfoViewSetr....N
-00004070: 290a 725b 0000 0072 5c00 0000 725d 0000  ).r[...r\...r]..
-00004080: 0072 1c00 0000 723b 0000 0072 5600 0000  .r....r;...rV...
-00004090: 72c3 0000 0072 c400 0000 7229 0000 0072  r....r....r)...r
-000040a0: 5f00 0000 7243 0000 0072 4300 0000 7243  _...rC...rC...rC
-000040b0: 0000 0072 4400 0000 722f 0100 00e8 0200  ...rD...r/......
-000040c0: 0073 0400 0000 0801 1001 722f 0100 0063  .s........r/...c
-000040d0: 0100 0000 0000 0000 0000 0000 1c00 0000  ................
-000040e0: 0e00 0000 4300 0000 73f0 0100 007c 006a  ....C...s....|.j
-000040f0: 00a0 0164 01a1 017d 017c 006a 02a0 0164  ...d...}.|.j...d
-00004100: 0264 03a1 027d 027c 026a 03a0 0464 04a1  .d...}.|.j...d..
-00004110: 0164 0519 00a0 0464 06a1 0164 0719 007d  .d.....d...d...}
-00004120: 0367 007d 047c 0364 0876 0090 0172 d090  .g.}.|.d.v...r..
-00004130: 017a 6074 056a 0664 097c 02a0 07a1 0064  .z`t.j.d.|.....d
-00004140: 0a64 0b8d 037d 057c 05a0 08a1 007d 067c  .d...}.|.....}.|
-00004150: 0644 0090 015d 387d 077c 076a 097d 0874  .D...]8}.|.j.}.t
-00004160: 0a64 0c7c 0883 0244 0090 015d 207d 097c  .d.|...D...] }.|
-00004170: 07a0 0b7c 09a1 017d 0a7c 0a72 7c7c 07a0  ...|...}.|.r||..
-00004180: 0c7c 0964 07a1 026a 0d7d 0b74 0e7c 07a0  .|.d...j.}.t.|..
-00004190: 0f7c 0964 07a1 0283 017d 0c7c 0a64 0519  .|.d.....}.|.d..
-000041a0: 007d 0d7c 0a64 0c19 007d 0e74 106a 116a  .}.|.d...}.t.j.j
-000041b0: 127c 0e64 0d8d 01a0 13a1 007d 0f7c 0f6a  .|.d.......}.|.j
-000041c0: 147d 107c 0a64 0e19 007d 1174 156a 116a  .}.|.d...}.t.j.j
-000041d0: 127c 0f6a 167c 1164 0f8d 02a0 13a1 007d  .|.j.|.d.......}
-000041e0: 127c 126a 147d 137c 0a64 1019 007d 1474  .|.j.}.|.d...}.t
-000041f0: 0e7c 0a64 1119 0083 017d 157c 0a64 1219  .|.d.....}.|.d..
-00004200: 007d 167c 0a64 1319 007d 1774 176a 116a  .}.|.d...}.t.j.j
-00004210: 127c 0c64 148d 01a0 13a1 007d 187c 1890  .|.d.......}.|..
-00004220: 0172 5a7c 186a 1866 0069 007c 0c7c 0d7c  .rZ|.j.f.i.|.|.|
-00004230: 107c 137c 147c 157c 167c 1764 159c 08a4  .|.|.|.|.|.d....
-00004240: 018e 0101 006e 2474 176a 116a 1966 0069  .....n$t.j.j.f.i
-00004250: 007c 0c7c 0d7c 107c 137c 147c 157c 167c  .|.|.|.|.|.|.|.|
-00004260: 1764 159c 08a4 018e 0101 007c 0c7c 0d7c  .d.........|.|.|
-00004270: 0e7c 117c 147c 157c 167c 1764 169c 087d  .|.|.|.|.|.d...}
-00004280: 197c 04a0 1a7c 19a1 0101 0071 7c71 6657  .|...|.....q|qfW
-00004290: 006e 2a04 0074 1b90 0179 ce01 007d 1a01  .n*..t...y...}..
-000042a0: 007a 107c 1a82 0157 0059 0064 097d 1a7e  .z.|...W.Y.d.}.~
-000042b0: 1a6e 0a64 097d 1a7e 1a30 0030 007c 0490  .n.d.}.~.0.0.|..
-000042c0: 0172 e064 177c 0469 017d 1b6e 0864 1764  .r.d.|.i.}.n.d.d
-000042d0: 1869 017d 1b74 1c7c 1b83 0153 0029 1975  .i.}.t.|...S.).u
-000042e0: 2000 0000 e5af bce5 85a5 e6a3 80e6 9fa5   ...............
-000042f0: e5ad 97e5 85b8 6578 6365 6ce8 a1a8 e695  ......excel.....
-00004300: b0e6 8dae 7279 0000 0072 7a00 0000 727b  ....ry...rz...r{
-00004310: 0000 0072 7c00 0000 727d 0000 0072 7e00  ...r|...r}...r~.
-00004320: 0000 7201 0000 0072 7f00 0000 4e54 7281  ..r....r....NTr.
-00004330: 0000 0072 8400 0000 7285 0000 0072 8700  ...r....r....r..
-00004340: 0000 a902 72d9 0000 0072 8600 0000 7288  ....r....r....r.
-00004350: 0000 0072 d700 0000 72d8 0000 0072 e900  ...r....r....r..
-00004360: 0000 a901 72cc 0000 00a9 0872 cc00 0000  ....r......r....
-00004370: 72cd 0000 0072 ce00 0000 72cf 0000 00da  r....r....r.....
-00004380: 0c70 726f 6a65 6374 5f66 6565 73da 0a63  .project_fees..c
-00004390: 6f64 655f 7372 7674 70da 0a6e 616d 655f  ode_srvtp..name_
-000043a0: 7372 7674 70da 0772 656d 6172 6b73 a908  srvtp..remarks..
-000043b0: 72cc 0000 0072 cd00 0000 72a4 0000 0072  r....r....r....r
-000043c0: e200 0000 7233 0100 0072 3401 0000 7235  ....r3...r4...r5
-000043d0: 0100 0072 3601 0000 7235 0000 0072 8e00  ...r6...r5...r..
-000043e0: 0000 291d 722f 0000 0072 4a00 0000 728f  ..).r/...rJ...r.
-000043f0: 0000 0072 8600 0000 7290 0000 0072 dd00  ...r....r....r..
-00004400: 0000 7292 0000 0072 9300 0000 7294 0000  ..r....r....r...
-00004410: 0072 9500 0000 7296 0000 0072 9700 0000  .r....r....r....
-00004420: 7298 0000 0072 9900 0000 729b 0000 0072  r....r....r....r
-00004430: 9a00 0000 7211 0000 0072 3b00 0000 723c  ....r....r;...r<
-00004440: 0000 0072 3d00 0000 728a 0000 0072 1200  ...r=...r....r..
-00004450: 0000 7248 0000 0072 1700 0000 729c 0000  ..rH...r....r...
-00004460: 0072 9d00 0000 729e 0000 0072 6600 0000  .r....r....rf...
-00004470: 7206 0000 0029 1c72 4100 0000 7279 0000  r....).rA...ry..
-00004480: 0072 7a00 0000 729f 0000 0072 a000 0000  .rz...r....r....
-00004490: 7235 0000 0072 9400 0000 72a1 0000 0072  r5...r....r....r
-000044a0: a200 0000 72a3 0000 0072 9700 0000 7299  ....r....r....r.
-000044b0: 0000 0072 cc00 0000 72cd 0000 0072 a400  ...r....r....r..
-000044c0: 0000 728b 0000 0072 ce00 0000 72e2 0000  ..r....r....r...
-000044d0: 0072 df00 0000 72cf 0000 0072 3301 0000  .r....r....r3...
-000044e0: 7234 0100 0072 3501 0000 7236 0100 005a  r4...r5...r6...Z
-000044f0: 1069 6e73 5f64 6963 7469 6f6e 6172 6965  .ins_dictionarie
-00004500: 7372 a500 0000 726c 0000 0072 5000 0000  sr....rl...rP...
-00004510: 7243 0000 0072 4300 0000 7244 0000 00da  rC...rC...rD....
-00004520: 1e69 6d70 6f72 745f 696e 7370 6563 7469  .import_inspecti
-00004530: 6f6e 5f64 6963 7469 6f6e 6172 6965 73ed  on_dictionaries.
-00004540: 0200 0073 7c00 0000 0003 0c01 0e01 1a02  ...s|...........
-00004550: 0402 0a02 0401 1401 0801 0a01 0601 1001  ................
-00004560: 0a01 0402 0e01 1001 0801 0801 1201 0602  ................
-00004570: 0801 1601 0601 0801 0c01 0801 0801 1201  ................
-00004580: 0601 0a01 0201 0201 0201 0201 0201 0201  ................
-00004590: 02f9 0c0a 0c01 0201 0201 0201 0201 0201  ................
-000045a0: 0201 02f9 0a0a 0201 0201 0201 0201 0201  ................
-000045b0: 0201 0201 02f8 060a 1201 1001 1a02 0601  ................
-000045c0: 0a02 0801 7238 0100 0063 0100 0000 0000  ....r8...c......
-000045d0: 0000 0000 0000 1c00 0000 0e00 0000 4300  ..............C.
-000045e0: 0000 73f0 0100 007c 006a 00a0 0164 01a1  ..s....|.j...d..
-000045f0: 017d 017c 006a 02a0 0164 0264 03a1 027d  .}.|.j...d.d...}
-00004600: 027c 026a 03a0 0464 04a1 0164 0519 00a0  .|.j...d...d....
-00004610: 0464 06a1 0164 0719 007d 0367 007d 047c  .d...d...}.g.}.|
-00004620: 0364 0876 0090 0172 d090 017a 6074 056a  .d.v...r...z`t.j
-00004630: 0664 097c 02a0 07a1 0064 0a64 0b8d 037d  .d.|.....d.d...}
-00004640: 057c 05a0 08a1 007d 067c 0644 0090 015d  .|.....}.|.D...]
-00004650: 387d 077c 076a 097d 0874 0a64 0c7c 0883  8}.|.j.}.t.d.|..
-00004660: 0244 0090 015d 207d 097c 07a0 0b7c 09a1  .D...] }.|...|..
-00004670: 017d 0a7c 0a72 7c7c 07a0 0c7c 0964 07a1  .}.|.r||...|.d..
-00004680: 026a 0d7d 0b74 0e7c 07a0 0f7c 0964 07a1  .j.}.t.|...|.d..
-00004690: 0283 017d 0c7c 0a64 0519 007d 0d7c 0a64  ...}.|.d...}.|.d
-000046a0: 0c19 007d 0e74 106a 116a 127c 0e64 0d8d  ...}.t.j.j.|.d..
-000046b0: 01a0 13a1 007d 0f7c 0f6a 147d 107c 0a64  .....}.|.j.}.|.d
-000046c0: 0e19 007d 1174 156a 116a 127c 0f6a 167c  ...}.t.j.j.|.j.|
-000046d0: 1164 0f8d 02a0 13a1 007d 127c 126a 147d  .d.......}.|.j.}
-000046e0: 137c 0a64 1019 007d 1474 0e7c 0a64 1119  .|.d...}.t.|.d..
-000046f0: 0083 017d 157c 0a64 1219 007d 167c 0a64  ...}.|.d...}.|.d
-00004700: 1319 007d 1774 176a 116a 127c 0c64 148d  ...}.t.j.j.|.d..
-00004710: 01a0 13a1 007d 187c 1890 0172 5a7c 186a  .....}.|...rZ|.j
-00004720: 1866 0069 007c 0c7c 0d7c 107c 137c 147c  .f.i.|.|.|.|.|.|
-00004730: 157c 167c 1764 159c 08a4 018e 0101 006e  .|.|.d.........n
-00004740: 2474 176a 116a 1966 0069 007c 0c7c 0d7c  $t.j.j.f.i.|.|.|
-00004750: 107c 137c 147c 157c 167c 1764 159c 08a4  .|.|.|.|.|.d....
-00004760: 018e 0101 007c 0c7c 0d7c 0e7c 117c 147c  .....|.|.|.|.|.|
-00004770: 157c 167c 1764 169c 087d 197c 04a0 1a7c  .|.|.d...}.|...|
-00004780: 19a1 0101 0071 7c71 6657 006e 2a04 0074  .....q|qfW.n*..t
-00004790: 1b90 0179 ce01 007d 1a01 007a 107c 1a82  ...y...}...z.|..
-000047a0: 0157 0059 0064 097d 1a7e 1a6e 0a64 097d  .W.Y.d.}.~.n.d.}
-000047b0: 1a7e 1a30 0030 007c 0490 0172 e064 177c  .~.0.0.|...r.d.|
-000047c0: 0469 017d 1b6e 0864 1764 1869 017d 1b74  .i.}.n.d.d.i.}.t
-000047d0: 1c7c 1b83 0153 0029 1975 2000 0000 e5af  .|...S.).u .....
-000047e0: bce5 85a5 e6a3 80e9 aa8c e5ad 97e5 85b8  ................
-000047f0: 6578 6365 6ce8 a1a8 e695 b0e6 8dae 7279  excel.........ry
-00004800: 0000 0072 7a00 0000 727b 0000 0072 7c00  ...rz...r{...r|.
-00004810: 0000 727d 0000 0072 7e00 0000 7201 0000  ..r}...r~...r...
-00004820: 0072 7f00 0000 4e54 7281 0000 0072 8400  .r....NTr....r..
-00004830: 0000 7285 0000 0072 8700 0000 7230 0100  ..r....r....r0..
-00004840: 0072 8800 0000 72d7 0000 0072 d800 0000  .r....r....r....
-00004850: 72e9 0000 0072 3101 0000 7232 0100 0072  r....r1...r2...r
-00004860: 3701 0000 7235 0000 0072 8e00 0000 291d  7...r5...r....).
-00004870: 722f 0000 0072 4a00 0000 728f 0000 0072  r/...rJ...r....r
-00004880: 8600 0000 7290 0000 0072 dd00 0000 7292  ....r....r....r.
-00004890: 0000 0072 9300 0000 7294 0000 0072 9500  ...r....r....r..
-000048a0: 0000 7296 0000 0072 9700 0000 7298 0000  ..r....r....r...
-000048b0: 0072 9900 0000 729b 0000 0072 9a00 0000  .r....r....r....
-000048c0: 7211 0000 0072 3b00 0000 723c 0000 0072  r....r;...r<...r
-000048d0: 3d00 0000 728a 0000 0072 1200 0000 7248  =...r....r....rH
-000048e0: 0000 0072 1800 0000 729c 0000 0072 9d00  ...r....r....r..
-000048f0: 0000 729e 0000 0072 6600 0000 7206 0000  ..r....rf...r...
-00004900: 0029 1c72 4100 0000 7279 0000 0072 7a00  .).rA...ry...rz.
-00004910: 0000 729f 0000 0072 a000 0000 7235 0000  ..r....r....r5..
-00004920: 0072 9400 0000 72a1 0000 0072 a200 0000  .r....r....r....
-00004930: 72a3 0000 0072 9700 0000 7299 0000 0072  r....r....r....r
-00004940: cc00 0000 72cd 0000 0072 a400 0000 728b  ....r....r....r.
-00004950: 0000 0072 ce00 0000 72e2 0000 0072 df00  ...r....r....r..
-00004960: 0000 72cf 0000 0072 3301 0000 7234 0100  ..r....r3...r4..
-00004970: 0072 3501 0000 7236 0100 005a 1065 7861  .r5...r6...Z.exa
-00004980: 5f64 6963 7469 6f6e 6172 6965 7372 a500  _dictionariesr..
-00004990: 0000 726c 0000 0072 5000 0000 7243 0000  ..rl...rP...rC..
-000049a0: 0072 4300 0000 7244 0000 00da 1f69 6d70  .rC...rD.....imp
-000049b0: 6f72 745f 6578 616d 696e 6174 696f 6e5f  ort_examination_
-000049c0: 6469 6374 696f 6e61 7269 6573 3903 0000  dictionaries9...
-000049d0: 737c 0000 0000 030c 010e 011a 0204 020a  s|..............
-000049e0: 0204 0114 0108 010a 0106 0110 010a 0104  ................
-000049f0: 020e 0110 0108 0108 0112 0106 0208 0116  ................
-00004a00: 0106 0108 010c 0108 0108 0112 0106 010a  ................
-00004a10: 0102 0102 0102 0102 0102 0102 0102 f90c  ................
-00004a20: 0a0c 0102 0102 0102 0102 0102 0102 0102  ................
-00004a30: f90a 0a02 0102 0102 0102 0102 0102 0102  ................
-00004a40: 0102 f806 0a12 0110 011a 0206 010a 0208  ................
-00004a50: 0172 3901 0000 6301 0000 0000 0000 0000  .r9...c.........
-00004a60: 0000 0027 0000 0019 0000 0043 0000 0073  ...'.......C...s
-00004a70: 9e02 0000 7c00 6a00 a001 6401 a101 7d01  ....|.j...d...}.
-00004a80: 7c00 6a02 a001 6402 6403 a102 7d02 7c02  |.j...d.d...}.|.
-00004a90: 6a03 a004 6404 a101 6405 1900 a004 6406  j...d...d.....d.
-00004aa0: a101 6407 1900 7d03 6700 7d04 7c03 6408  ..d...}.g.}.|.d.
-00004ab0: 7600 9002 727e 9002 7a0e 7405 6a06 6409  v...r~..z.t.j.d.
-00004ac0: 7c02 a007 a100 640a 640b 8d03 7d05 7c05  |.....d.d...}.|.
-00004ad0: a008 a100 7d06 7c06 4400 9001 5de6 7d07  ....}.|.D...].}.
-00004ae0: 7c07 6a09 7d08 740a 640c 7c08 8302 4400  |.j.}.t.d.|...D.
-00004af0: 9001 5dce 7d09 7c07 a00b 7c09 a101 7d0a  ..].}.|...|...}.
-00004b00: 7c0a 727c 7c07 a00c 7c09 6407 a102 6a0d  |.r||...|.d...j.
-00004b10: 7d0b 740e 7c07 a00f 7c09 6407 a102 8301  }.t.|...|.d.....
-00004b20: 7d0c 7c0a 6405 1900 7d0d 7c0a 640c 1900  }.|.d...}.|.d...
-00004b30: 7d0e 7c0a 640d 1900 7d0f 7c0a 640e 1900  }.|.d...}.|.d...
-00004b40: 7d10 7410 6a11 6a12 7c10 640f 8d01 a013  }.t.j.j.|.d.....
-00004b50: a100 7d11 7c0a 6410 1900 7d12 7414 6a11  ..}.|.d...}.t.j.
-00004b60: 6a12 7c12 6411 8d01 a013 a100 7d13 7c0a  j.|.d.......}.|.
-00004b70: 6412 1900 7d14 7415 6a11 6a12 7c14 6413  d...}.t.j.j.|.d.
-00004b80: 8d01 a013 a100 7d15 7c0a 6414 1900 7d16  ......}.|.d...}.
-00004b90: 7c0a 6415 1900 7d17 7c0a 6416 1900 7d18  |.d...}.|.d...}.
-00004ba0: 7c0a 6417 1900 7d19 7c0a 6418 1900 7d1a  |.d...}.|.d...}.
-00004bb0: 7c0a 6419 1900 7d1b 7c0a 641a 1900 7d1c  |.d...}.|.d...}.
-00004bc0: 7c0a 641b 1900 7d1d 7c0a 641c 1900 7d1e  |.d...}.|.d...}.
-00004bd0: 7c1e 641d 6b02 9001 726c 640a 7d1f 6e04  |.d.k...rld.}.n.
-00004be0: 641e 7d1f 7c0a 641f 1900 7d20 7c0a 6420  d.}.|.d...} |.d 
-00004bf0: 1900 7d21 7c0a 6421 1900 7d22 7416 6a11  ..}!|.d!..}"t.j.
-00004c00: 6a12 7c0c 6422 8d01 7d23 7c23 9001 72dc  j.|.d"..}#|#..r.
-00004c10: 7c23 6a17 6600 6900 7c0c 7c0d 7c0e 7c0f  |#j.f.i.|.|.|.|.
-00004c20: 7c11 6a18 7c13 6a18 7c15 6a18 7c16 7c17  |.j.|.j.|.j.|.|.
-00004c30: 7c18 7c19 7c1a 7c1b 7c1c 7c1d 7c1f 7c20  |.|.|.|.|.|.|.| 
-00004c40: 7c21 7c22 6423 9c13 a401 8e01 0100 6e3a  |!|"d#........n:
-00004c50: 7416 6a11 6a19 6600 6900 7c0c 7c0d 7c0e  t.j.j.f.i.|.|.|.
-00004c60: 7c0f 7c11 7c13 7c15 7c16 7c17 7c18 7c19  |.|.|.|.|.|.|.|.
-00004c70: 7c1a 7c1b 7c1c 7c1d 7c1f 7c20 7c21 7c22  |.|.|.|.|.| |!|"
-00004c80: 6423 9c13 a401 8e01 0100 7c0c 7c0d 7c0e  d#........|.|.|.
-00004c90: 7c0f 7c10 7c12 7c14 7c16 7c17 7c18 7c19  |.|.|.|.|.|.|.|.
-00004ca0: 7c1a 7c1b 7c1c 7c1d 7c1e 7c20 7c21 7c22  |.|.|.|.|.| |!|"
-00004cb0: 6424 9c13 7d24 7c04 a01a 7c24 a101 0100  d$..}$|...|$....
-00004cc0: 717c 7166 5700 6e2a 0400 741b 9002 797c  q|qfW.n*..t...y|
-00004cd0: 0100 7d25 0100 7a10 7c25 8201 5700 5900  ..}%..z.|%..W.Y.
-00004ce0: 6409 7d25 7e25 6e0a 6409 7d25 7e25 3000  d.}%~%n.d.}%~%0.
-00004cf0: 3000 7c04 9002 728e 6425 7c04 6901 7d26  0.|...r.d%|.i.}&
-00004d00: 6e08 6425 6426 6901 7d26 741c 7c26 8301  n.d%d&i.}&t.|&..
-00004d10: 5300 2927 7520 0000 00e5 afbc e585 a5e8  S.)'u ..........
-00004d20: 8daf e593 81e7 9bae e5bd 9565 7863 656c  ...........excel
-00004d30: e8a1 a8e6 95b0 e68d ae72 7900 0000 727a  .........ry...rz
-00004d40: 0000 0072 7b00 0000 727c 0000 0072 7d00  ...r{...r|...r}.
-00004d50: 0000 727e 0000 0072 0100 0000 727f 0000  ..r~...r....r...
-00004d60: 004e 5472 8100 0000 7284 0000 0072 8700  .NTr....r....r..
-00004d70: 0000 7288 0000 00a9 01da 0974 7970 655f  ..r........type_
-00004d80: 6e61 6d65 72d7 0000 0072 8500 0000 72d8  namer....r....r.
-00004d90: 0000 00a9 01da 0d63 6174 6567 6f72 795f  .......category_
-00004da0: 6e61 6d65 72e9 0000 0072 ea00 0000 72eb  namer....r....r.
-00004db0: 0000 00e9 0a00 0000 e90b 0000 00e9 0c00  ................
-00004dc0: 0000 e90d 0000 00e9 0e00 0000 e90f 0000  ................
-00004dd0: 0072 ec00 0000 46e9 1000 0000 e911 0000  .r....F.........
-00004de0: 00e9 1200 0000 a901 7202 0100 0029 1372  ........r....).r
-00004df0: 0201 0000 7203 0100 0072 0401 0000 da05  ....r....r......
-00004e00: 756e 6974 7372 1101 0000 7213 0100 0072  unitsr....r....r
-00004e10: 1201 0000 720f 0100 0072 1001 0000 7206  ....r....r....r.
-00004e20: 0100 0072 0501 0000 7207 0100 0072 0801  ...r....r....r..
-00004e30: 0000 7209 0100 0072 0a01 0000 720b 0100  ..r....r....r...
-00004e40: 0072 0c01 0000 720d 0100 0072 0e01 0000  .r....r....r....
-00004e50: 2913 7202 0100 0072 0301 0000 7204 0100  ).r....r....r...
-00004e60: 0072 4801 0000 da15 7072 6570 6172 6174  .rH.....preparat
-00004e70: 696f 6e5f 7479 7065 5f6e 616d 65da 0e64  ion_type_name..d
-00004e80: 7275 675f 7479 7065 5f6e 616d 6572 3d01  rug_type_namer=.
-00004e90: 0000 720f 0100 0072 1001 0000 7206 0100  ..r....r....r...
-00004ea0: 0072 0501 0000 7207 0100 0072 0801 0000  .r....r....r....
-00004eb0: 7209 0100 0072 0a01 0000 720b 0100 0072  r....r....r....r
-00004ec0: 0c01 0000 720d 0100 0072 0e01 0000 7235  ....r....r....r5
-00004ed0: 0000 0072 8e00 0000 291d 722f 0000 0072  ...r....).r/...r
-00004ee0: 4a00 0000 728f 0000 0072 8600 0000 7290  J...r....r....r.
-00004ef0: 0000 0072 dd00 0000 7292 0000 0072 9300  ...r....r....r..
-00004f00: 0000 7294 0000 0072 9500 0000 7296 0000  ..r....r....r...
-00004f10: 0072 9700 0000 7298 0000 0072 9900 0000  .r....r....r....
-00004f20: 729b 0000 0072 9a00 0000 721d 0000 0072  r....r....r....r
-00004f30: 3b00 0000 723c 0000 0072 3d00 0000 721e  ;...r<...r=...r.
-00004f40: 0000 0072 1f00 0000 7219 0000 0072 9c00  ...r....r....r..
-00004f50: 0000 7248 0000 0072 9d00 0000 729e 0000  ..rH...r....r...
-00004f60: 0072 6600 0000 7206 0000 0029 2772 4100  .rf...r....)'rA.
-00004f70: 0000 7279 0000 0072 7a00 0000 729f 0000  ..ry...rz...r...
-00004f80: 0072 a000 0000 7235 0000 0072 9400 0000  .r....r5...r....
-00004f90: 72a1 0000 0072 a200 0000 72a3 0000 0072  r....r....r....r
-00004fa0: 9700 0000 7299 0000 0072 0201 0000 7203  ....r....r....r.
-00004fb0: 0100 0072 0401 0000 7248 0100 0072 4901  ...r....rH...rI.
-00004fc0: 0000 7211 0100 0072 4a01 0000 7213 0100  ..r....rJ...r...
-00004fd0: 0072 3d01 0000 7212 0100 0072 0f01 0000  .r=...r....r....
-00004fe0: 7210 0100 0072 0601 0000 7205 0100 0072  r....r....r....r
-00004ff0: 0701 0000 7208 0100 0072 0901 0000 720a  ....r....r....r.
-00005000: 0100 005a 1069 735f 6573 7365 6e74 6961  ...Z.is_essentia
-00005010: 6c5f 7374 7272 0b01 0000 720c 0100 0072  l_strr....r....r
-00005020: 0d01 0000 720e 0100 005a 0e64 7275 675f  ....r....Z.drug_
-00005030: 6469 7265 6374 6f72 7972 a500 0000 726c  directoryr....rl
-00005040: 0000 0072 5000 0000 7243 0000 0072 4300  ...rP...rC...rC.
-00005050: 0000 7244 0000 00da 1569 6d70 6f72 745f  ..rD.....import_
-00005060: 6472 7567 5f64 6972 6563 746f 7279 8503  drug_directory..
-00005070: 0000 73d8 0000 0000 030c 010e 011a 0204  ..s.............
-00005080: 020a 0204 0114 0108 010a 0106 0110 010a  ................
-00005090: 0104 020e 0110 0108 0108 0108 0108 0112  ................
-000050a0: 0108 0112 0108 0112 0108 0108 0108 0108  ................
-000050b0: 0108 0108 0108 0108 0108 010a 0106 0204  ................
-000050c0: 0108 0108 0108 010e 0106 010a 0102 0102  ................
-000050d0: 0102 0104 0104 0104 0102 0102 0102 0102  ................
-000050e0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-000050f0: ee0c 150c 0102 0102 0102 0102 0102 0102  ................
-00005100: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00005110: 0102 0102 0102 0102 ee0a 1502 0102 0102  ................
-00005120: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00005130: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00005140: ed06 1512 0110 011a 0206 010a 0208 0172  ...............r
-00005150: 4b01 0000 6301 0000 0000 0000 0000 0000  K...c...........
-00005160: 0027 0000 0017 0000 0043 0000 0073 c002  .'.......C...s..
-00005170: 0000 7c00 6a00 a001 6401 a101 7d01 7c00  ..|.j...d...}.|.
-00005180: 6a02 a001 6402 6403 a102 7d02 7c02 6a03  j...d.d...}.|.j.
-00005190: a004 6404 a101 6405 1900 a004 6406 a101  ..d...d.....d...
-000051a0: 6407 1900 7d03 6700 7d04 7c03 6408 7600  d...}.g.}.|.d.v.
-000051b0: 9002 72a0 9002 7a30 7405 6a06 6409 7c02  ..r...z0t.j.d.|.
-000051c0: a007 a100 640a 640b 8d03 7d05 7c05 a008  ....d.d...}.|...
-000051d0: a100 7d06 7c06 4400 9002 5d08 7d07 7c07  ..}.|.D...].}.|.
-000051e0: 6a09 7d08 740a 640c 7c08 8302 4400 9001  j.}.t.d.|...D...
-000051f0: 5df0 7d09 7c07 a00b 7c09 a101 7d0a 7c0a  ].}.|...|...}.|.
-00005200: 727c 7c07 a00c 7c09 6407 a102 6a0d 7d0b  r||...|.d...j.}.
-00005210: 7c07 a00e 7c09 6407 a102 7d0c 740f 6a10  |...|.d...}.t.j.
-00005220: 6a11 7c0c 640d 8d01 a012 a100 7d0d 7c0a  j.|.d.......}.|.
-00005230: 6405 1900 7d0e 7c0a 640c 1900 7d0f 7c0a  d...}.|.d...}.|.
-00005240: 640e 1900 7d10 7c0a 640f 1900 7d11 7413  d...}.|.d...}.t.
-00005250: 6a10 6a11 7c11 6410 8d01 a012 a100 7d12  j.j.|.d.......}.
-00005260: 7c0a 6411 1900 7d13 7414 6a10 6a11 7c13  |.d...}.t.j.j.|.
-00005270: 6412 8d01 a012 a100 7d14 7c0a 6413 1900  d.......}.|.d...
-00005280: 7d15 7415 6a10 6a11 7c15 6414 8d01 a012  }.t.j.j.|.d.....
-00005290: a100 7d16 7c0a 6415 1900 7d17 7c0a 6416  ..}.|.d...}.|.d.
-000052a0: 1900 7d18 7c0a 6417 1900 7d19 7416 6a16  ..}.|.d...}.t.j.
-000052b0: a017 7c19 6418 a102 7d1a 7c0a 6419 1900  ..|.d...}.|.d...
-000052c0: 7d1b 7c0a 641a 1900 7d1c 7c0a 641b 1900  }.|.d...}.|.d...
-000052d0: 7d1d 7c0a 641c 1900 7d1e 7c0a 641d 1900  }.|.d...}.|.d...
-000052e0: 7d1f 7c0a 641e 1900 7d20 7c20 641f 6b02  }.|.d...} | d.k.
-000052f0: 9001 7288 640a 7d21 6e04 6420 7d21 7c0a  ..r.d.}!n.d }!|.
-00005300: 6421 1900 7d22 7418 6a10 6a11 7c0e 6422  d!..}"t.j.j.|.d"
-00005310: 8d01 7d23 7c23 9001 72f6 7c23 6a19 6600  ..}#|#..r.|#j.f.
-00005320: 6900 7c0e 7c0d 6a1a 7c0f 7c10 7c12 6a1a  i.|.|.j.|.|.|.j.
-00005330: 7c14 6a1a 7c16 6a1a 7c17 7c18 7c1a 7c1b  |.j.|.j.|.|.|.|.
-00005340: 7c1c 741b 7c1d 8301 741b 7c1e 8301 741b  |.t.|...t.|...t.
-00005350: 7c1f 8301 7c21 741b 7c22 8301 6423 9c11  |...|!t.|"..d#..
-00005360: a401 8e01 0100 6e46 7418 6a10 6a1c 6600  ......nFt.j.j.f.
-00005370: 6900 7c0e 7c0d 7c0f 7c10 7c12 7c14 7c16  i.|.|.|.|.|.|.|.
-00005380: 7c17 7c18 7c1a 7c1b 7c1c 741b 7c1d 8301  |.|.|.|.|.t.|...
-00005390: 741b 7c1e 8301 741b 7c1f 8301 7c21 741b  t.|...t.|...|!t.
-000053a0: 7c22 8301 6423 9c11 a401 8e01 0100 7c0c  |"..d#........|.
-000053b0: 7c0e 7c0f 7c10 7c11 7c13 7c15 7c17 7c18  |.|.|.|.|.|.|.|.
-000053c0: 7c1a 7c1b 7c1c 7c1d 7c1e 7c1f 7c21 7c22  |.|.|.|.|.|.|!|"
-000053d0: 6424 9c11 7d24 7c04 a01d 7c24 a101 0100  d$..}$|...|$....
-000053e0: 717c 7166 5700 6e2a 0400 741e 9002 799e  q|qfW.n*..t...y.
-000053f0: 0100 7d25 0100 7a10 7c25 8201 5700 5900  ..}%..z.|%..W.Y.
-00005400: 6409 7d25 7e25 6e0a 6409 7d25 7e25 3000  d.}%~%n.d.}%~%0.
-00005410: 3000 7c04 9002 72b0 6425 7c04 6901 7d26  0.|...r.d%|.i.}&
-00005420: 6e08 6425 6426 6901 7d26 741f 7c26 8301  n.d%d&i.}&t.|&..
-00005430: 5300 2927 7520 0000 00e5 afbc e585 a5e8  S.)'u ..........
-00005440: 8daf e688 bfe8 8daf e593 8165 7863 656c  ...........excel
-00005450: e8a1 a8e6 95b0 e68d ae72 7900 0000 727a  .........ry...rz
-00005460: 0000 0072 7b00 0000 727c 0000 0072 7d00  ...r{...r|...r}.
-00005470: 0000 727e 0000 0072 0100 0000 727f 0000  ..r~...r....r...
-00005480: 004e 5472 8100 0000 7284 0000 0029 01da  .NTr....r....)..
-00005490: 0d70 6861 726d 6163 795f 6e61 6d65 7287  .pharmacy_namer.
-000054a0: 0000 0072 8800 0000 723a 0100 0072 d700  ...r....r:...r..
-000054b0: 0000 7285 0000 0072 d800 0000 723c 0100  ..r....r....r<..
-000054c0: 0072 e900 0000 72ea 0000 0072 eb00 0000  .r....r....r....
-000054d0: 7a08 2559 2d25 6d2d 2564 723e 0100 0072  z.%Y-%m-%dr>...r
-000054e0: 3f01 0000 7240 0100 0072 4101 0000 7242  ?...r@...rA...rB
-000054f0: 0100 0072 4401 0000 72ec 0000 0046 7243  ...rD...r....FrC
-00005500: 0100 0072 4701 0000 2911 7202 0100 00da  ...rG...).r.....
-00005510: 0870 6861 726d 6163 7972 0301 0000 7204  .pharmacyr....r.
-00005520: 0100 0072 1101 0000 7213 0100 0072 1201  ...r....r....r..
-00005530: 0000 720f 0100 0072 1001 0000 da0a 7661  ..r....r......va
-00005540: 6c69 645f 6461 7465 da12 696e 7665 6e74  lid_date..invent
-00005550: 6f72 795f 7175 616e 7469 7479 da10 6d65  ory_quantity..me
-00005560: 6173 7572 656d 656e 745f 756e 6974 da0f  asurement_unit..
-00005570: 636f 7374 5f75 6e69 745f 7072 6963 65da  cost_unit_price.
-00005580: 0b63 6f73 745f 616d 6f75 6e74 da11 7265  .cost_amount..re
-00005590: 7461 696c 5f75 6e69 745f 7072 6963 6572  tail_unit_pricer
-000055a0: 3e00 0000 da0d 7265 7461 696c 5f61 6d6f  >.....retail_amo
-000055b0: 756e 7429 1172 4c01 0000 7202 0100 0072  unt).rL...r....r
-000055c0: 0301 0000 7204 0100 0072 4901 0000 724a  ....r....rI...rJ
-000055d0: 0100 0072 3d01 0000 720f 0100 0072 1001  ...r=...r....r..
-000055e0: 0000 724e 0100 0072 4f01 0000 7250 0100  ..rN...rO...rP..
-000055f0: 0072 5101 0000 7252 0100 0072 5301 0000  .rQ...rR...rS...
-00005600: 723e 0000 0072 5401 0000 7235 0000 0072  r>...rT...r5...r
-00005610: 8e00 0000 2920 722f 0000 0072 4a00 0000  ....) r/...rJ...
-00005620: 728f 0000 0072 8600 0000 7290 0000 0072  r....r....r....r
-00005630: dd00 0000 7292 0000 0072 9300 0000 7294  ....r....r....r.
-00005640: 0000 0072 9500 0000 7296 0000 0072 9700  ...r....r....r..
-00005650: 0000 7298 0000 0072 9900 0000 729a 0000  ..r....r....r...
-00005660: 0072 1a00 0000 723b 0000 0072 3c00 0000  .r....r;...r<...
-00005670: 723d 0000 0072 1d00 0000 721e 0000 0072  r=...r....r....r
-00005680: 1f00 0000 724c 0000 00da 0873 7472 7074  ....rL.....strpt
-00005690: 696d 6572 2000 0000 729c 0000 0072 4800  imer ...r....rH.
-000056a0: 0000 da05 666c 6f61 7472 9d00 0000 729e  ....floatr....r.
-000056b0: 0000 0072 6600 0000 7206 0000 0029 2772  ...rf...r....)'r
-000056c0: 4100 0000 7279 0000 0072 7a00 0000 729f  A...ry...rz...r.
-000056d0: 0000 0072 a000 0000 7235 0000 0072 9400  ...r....r5...r..
-000056e0: 0000 72a1 0000 0072 a200 0000 72a3 0000  ..r....r....r...
-000056f0: 0072 9700 0000 7299 0000 0072 4c01 0000  .r....r....rL...
-00005700: da13 7068 6172 6d61 6379 5f6d 616e 6167  ..pharmacy_manag
-00005710: 656d 656e 7472 0201 0000 7203 0100 0072  ementr....r....r
-00005720: 0401 0000 7249 0100 0072 1101 0000 724a  ....rI...r....rJ
-00005730: 0100 0072 1301 0000 723d 0100 0072 1201  ...r....r=...r..
-00005740: 0000 720f 0100 0072 1001 0000 5a0e 7661  ..r....r....Z.va
-00005750: 6c69 645f 6461 7465 5f73 7472 724e 0100  lid_date_strrN..
-00005760: 0072 4f01 0000 7250 0100 0072 5101 0000  .rO...rP...rQ...
-00005770: 7252 0100 0072 5301 0000 5a0d 6973 5f61  rR...rS...Z.is_a
-00005780: 6374 6976 655f 7374 7272 3e00 0000 7254  ctive_strr>...rT
-00005790: 0100 005a 0d70 6861 726d 6163 795f 6472  ...Z.pharmacy_dr
-000057a0: 7567 72a5 0000 0072 6c00 0000 7250 0000  ugr....rl...rP..
-000057b0: 0072 4300 0000 7243 0000 0072 4400 0000  .rC...rC...rD...
-000057c0: da14 696d 706f 7274 5f70 6861 726d 6163  ..import_pharmac
-000057d0: 795f 6472 7567 ff03 0000 73cc 0000 0000  y_drug....s.....
-000057e0: 030c 010e 011a 0204 020a 0204 0114 0108  ................
-000057f0: 010a 0106 0110 010a 0104 020e 010c 0112  ................
-00005800: 0108 0108 0108 0108 0112 0108 0112 0108  ................
-00005810: 0112 0108 0108 0108 010e 0108 0108 0108  ................
-00005820: 0108 0108 0108 010a 0106 0204 0108 010e  ................
-00005830: 0106 010a 0104 0102 0102 0104 0104 0104  ................
-00005840: 0102 0102 0102 0102 0102 0106 0106 0106  ................
-00005850: 0102 0106 f00c 130c 0102 0102 0102 0102  ................
-00005860: 0102 0102 0102 0102 0102 0102 0102 0106  ................
-00005870: 0106 0106 0102 0106 f00a 1302 0102 0102  ................
-00005880: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00005890: 0102 0102 0102 0102 0102 0102 ef06 1312  ................
-000058a0: 0110 011a 0206 010a 0208 0172 5801 0000  ...........rX...
-000058b0: 2965 7273 0000 0072 4c00 0000 7237 0000  )ers...rL...r7..
-000058c0: 00da 0872 6571 7565 7374 7372 dd00 0000  ...requestsr....
-000058d0: 726e 0000 005a 1c64 6a61 6e67 6f2e 636f  rn...Z.django.co
-000058e0: 6e74 7269 622e 6175 7468 2e62 6163 6b65  ntrib.auth.backe
-000058f0: 6e64 7372 0200 0000 da1b 646a 616e 676f  ndsr......django
-00005900: 2e63 6f6e 7472 6962 2e61 7574 682e 6861  .contrib.auth.ha
-00005910: 7368 6572 7372 0300 0000 da1a 646a 616e  shersr......djan
-00005920: 676f 2e63 6f6e 7472 6962 2e61 7574 682e  go.contrib.auth.
-00005930: 6d6f 6465 6c73 7204 0000 00da 0964 6a61  modelsr......dja
-00005940: 6e67 6f2e 6462 7205 0000 00da 0b64 6a61  ngo.dbr......dja
-00005950: 6e67 6f2e 6874 7470 7206 0000 0072 0700  ngo.httpr....r..
-00005960: 0000 da0e 646a 616e 676f 5f66 696c 7465  ....django_filte
-00005970: 7273 72b3 0000 005a 1064 7266 5f65 7863  rsr....Z.drf_exc
-00005980: 656c 2e6d 6978 696e 7372 0800 0000 5a13  el.mixinsr....Z.
-00005990: 6472 665f 6578 6365 6c2e 7265 6e64 6572  drf_excel.render
-000059a0: 6572 7372 0900 0000 da0e 7265 7374 5f66  ersr......rest_f
-000059b0: 7261 6d65 776f 726b 720a 0000 005a 1972  rameworkr....Z.r
-000059c0: 6573 745f 6672 616d 6577 6f72 6b2e 6465  est_framework.de
-000059d0: 636f 7261 746f 7273 720b 0000 005a 1772  coratorsr....Z.r
-000059e0: 6573 745f 6672 616d 6577 6f72 6b2e 6765  est_framework.ge
-000059f0: 6e65 7269 6373 720c 0000 005a 1a72 6573  nericsr....Z.res
-00005a00: 745f 6672 616d 6577 6f72 6b2e 7065 726d  t_framework.perm
-00005a10: 6973 7369 6f6e 7372 0d00 0000 da17 7265  issionsr......re
-00005a20: 7374 5f66 7261 6d65 776f 726b 2e72 6573  st_framework.res
-00005a30: 706f 6e73 6572 0e00 0000 5a17 7265 7374  ponser....Z.rest
-00005a40: 5f66 7261 6d65 776f 726b 2e76 6965 7773  _framework.views
-00005a50: 6574 7372 0f00 0000 7210 0000 00da 1262  etsr....r......b
-00005a60: 6173 655f 7379 7374 656d 2e6d 6f64 656c  ase_system.model
-00005a70: 7372 1100 0000 7212 0000 0072 1300 0000  sr....r....r....
-00005a80: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00005a90: 1700 0000 7218 0000 0072 1900 0000 721a  ....r....r....r.
-00005aa0: 0000 0072 1b00 0000 721c 0000 0072 1d00  ...r....r....r..
-00005ab0: 0000 721e 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
-00005ac0: 0072 2100 0000 7222 0000 005a 1762 6173  .r!...r"...Z.bas
-00005ad0: 655f 7379 7374 656d 2e73 6572 6961 6c69  e_system.seriali
-00005ae0: 7a65 7273 7223 0000 0072 2400 0000 7225  zersr#...r$...r%
-00005af0: 0000 0072 2600 0000 7227 0000 0072 2800  ...r&...r'...r(.
-00005b00: 0000 7229 0000 0072 2a00 0000 722b 0000  ..r)...r*...r+..
-00005b10: 0072 2c00 0000 da0b 646a 616e 676f 2e63  .r,.....django.c
-00005b20: 6f6e 6672 2d00 0000 da0f 646a 616e 676f  onfr-.....django
-00005b30: 5f73 6574 7469 6e67 7372 9100 0000 722e  _settingsr....r.
-00005b40: 0000 00da 0272 6572 fe00 0000 7245 0000  .....rer....rE..
-00005b50: 0072 5100 0000 7252 0000 0072 6200 0000  .rQ...rR...rb...
-00005b60: 7264 0000 00da 0661 746f 6d69 6372 a600  rd.....atomicr..
-00005b70: 0000 da09 4669 6c74 6572 5365 7472 a700  ....FilterSetr..
-00005b80: 0000 72b6 0000 0072 c700 0000 72cb 0000  ..r....r....r...
-00005b90: 0072 d200 0000 72d3 0000 0072 d400 0000  .r....r....r....
-00005ba0: 72d5 0000 0072 d600 0000 72e0 0000 0072  r....r....r....r
-00005bb0: fc00 0000 72f7 0000 0072 0101 0000 7218  ....r....r....r.
-00005bc0: 0100 0072 1901 0000 722f 0100 0072 3801  ...r....r/...r8.
-00005bd0: 0000 7239 0100 0072 4b01 0000 7258 0100  ..r9...rK...rX..
-00005be0: 0072 4300 0000 7243 0000 0072 4300 0000  .rC...rC...rC...
-00005bf0: 7244 0000 00da 083c 6d6f 6475 6c65 3e01  rD.....<module>.
-00005c00: 0000 0073 7a00 0000 0801 0801 0802 0801  ...sz...........
-00005c10: 0802 0801 0c01 0c01 0c01 0c01 1001 0801  ................
-00005c20: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 1002  ................
-00005c30: 5003 2c04 0c01 0c03 0801 0c01 0801 0803  P.,.............
-00005c40: 0813 0812 1018 1020 0e1c 0401 0a3d 120d  ....... .....=..
-00005c50: 1016 1007 120c 101a 1007 120c 101c 1007  ................
-00005c60: 0401 0a51 0401 0a7f 0053 080c 121a 0809  ...Q.....S......
-00005c70: 102e 1005 0401 0a4b 0401 0a4b 0401 0a79  .......K...K...y
-00005c80: 0401                                     ..
+00000260: 5a55 642a 642b 8400 5a56 4700 642c 642d  ZUd*d+..ZVG.d,d-
+00000270: 8400 642d 6523 8303 5a57 4700 642e 642f  ..d-e#..ZWG.d.d/
+00000280: 8400 642f 6512 6a50 8303 5a58 4700 6430  ..d/e.jP..ZXG.d0
+00000290: 6431 8400 6431 6523 8303 5a59 6432 6433  d1..d1e#..ZYd2d3
+000002a0: 8400 5a5a 4700 6434 6435 8400 6435 6523  ..ZZG.d4d5..d5e#
+000002b0: 8303 5a5b 650d 6a4e 6436 6437 8400 8301  ..Z[e.jNd6d7....
+000002c0: 5a5c 650d 6a4e 6438 6439 8400 8301 5a5d  Z\e.jNd8d9....Z]
+000002d0: 643a 643b 8400 5a5e 4700 643c 643d 8400  d:d;..Z^G.d<d=..
+000002e0: 643d 6512 6a50 8303 5a5f 643e 643f 8400  d=e.jP..Z_d>d?..
+000002f0: 5a60 4700 6440 6441 8400 6441 6523 8303  Z`G.d@dA..dAe#..
+00000300: 5a61 4700 6442 6443 8400 6443 6523 8303  ZaG.dBdC..dCe#..
+00000310: 5a62 650d 6a4e 6444 6445 8400 8301 5a63  Zbe.jNdDdE....Zc
+00000320: 650d 6a4e 6446 6447 8400 8301 5a64 650d  e.jNdFdG....Zde.
+00000330: 6a4e 6448 6449 8400 8301 5a65 650d 6a4e  jNdHdI....Zee.jN
+00000340: 644a 644b 8400 8301 5a66 6401 5300 294c  dJdK....Zfd.S.)L
+00000350: e900 0000 004e 2901 da0c 4d6f 6465 6c42  .....N)...ModelB
+00000360: 6163 6b65 6e64 2901 da0d 6d61 6b65 5f70  ackend)...make_p
+00000370: 6173 7377 6f72 6429 01da 0a50 6572 6d69  assword)...Permi
+00000380: 7373 696f 6e29 01da 0b74 7261 6e73 6163  ssion)...transac
+00000390: 7469 6f6e 2902 da0c 4a73 6f6e 5265 7370  tion)...JsonResp
+000003a0: 6f6e 7365 da0c 4874 7470 5265 7370 6f6e  onse..HttpRespon
+000003b0: 7365 2901 da0d 584c 5358 4669 6c65 4d69  se)...XLSXFileMi
+000003c0: 7869 6e29 01da 0c58 4c53 5852 656e 6465  xin)...XLSXRende
+000003d0: 7265 7229 01da 0673 7461 7475 7329 01da  rer)...status)..
+000003e0: 0661 6374 696f 6e29 01da 0b4c 6973 7441  .action)...ListA
+000003f0: 5049 5669 6577 2901 da0f 4973 4175 7468  PIView)...IsAuth
+00000400: 656e 7469 6361 7465 6429 01da 0852 6573  enticated)...Res
+00000410: 706f 6e73 6529 02da 1452 6561 644f 6e6c  ponse)...ReadOnl
+00000420: 794d 6f64 656c 5669 6577 5365 74da 0c4d  yModelViewSet..M
+00000430: 6f64 656c 5669 6577 5365 7429 12da 0848  odelViewSet)...H
+00000440: 6f73 7069 7461 6cda 064f 6666 6963 65da  ospital..Office.
+00000450: 0644 6f63 746f 72da 0d50 6f73 6974 696f  .Doctor..Positio
+00000460: 6e54 6974 6c65 da04 5573 6572 da0a 4578  nTitle..User..Ex
+00000470: 7472 6147 726f 7570 da16 496e 7370 6563  traGroup..Inspec
+00000480: 7469 6f6e 4469 6374 696f 6e61 7269 6573  tionDictionaries
+00000490: da17 4578 616d 696e 6174 696f 6e44 6963  ..ExaminationDic
+000004a0: 7469 6f6e 6172 6965 73da 0d44 7275 6744  tionaries..DrugD
+000004b0: 6972 6563 746f 7279 da12 5068 6172 6d61  irectory..Pharma
+000004c0: 6379 4d61 6e61 6765 6d65 6e74 da0f 4578  cyManagement..Ex
+000004d0: 7065 6e73 6553 7461 6e64 6172 64da 0741  penseStandard..A
+000004e0: 7069 496e 666f da13 4472 7567 5072 6570  piInfo..DrugPrep
+000004f0: 6172 6174 696f 6e54 7970 65da 0844 7275  arationType..Dru
+00000500: 6754 7970 65da 0c44 7275 6743 6174 6567  gType..DrugCateg
+00000510: 6f72 79da 0c50 6861 726d 6163 7944 7275  ory..PharmacyDru
+00000520: 67da 0e49 6e73 7065 6374 696f 6e54 7970  g..InspectionTyp
+00000530: 65da 0f45 7861 6d69 6e61 7469 6f6e 5479  e..ExaminationTy
+00000540: 7065 2909 da0e 5573 6572 5365 7269 616c  pe)...UserSerial
+00000550: 697a 6572 da12 5061 7373 776f 7264 5365  izer..PasswordSe
+00000560: 7269 616c 697a 6572 da20 496e 7370 6563  rializer. Inspec
+00000570: 7469 6f6e 4469 6374 696f 6e61 7269 6573  tionDictionaries
+00000580: 5365 7269 616c 697a 6572 da21 4578 616d  Serializer.!Exam
+00000590: 696e 6174 696f 6e44 6963 7469 6f6e 6172  inationDictionar
+000005a0: 6965 7353 6572 6961 6c69 7a65 72da 1c50  iesSerializer..P
+000005b0: 6861 726d 6163 794d 616e 6167 656d 656e  harmacyManagemen
+000005c0: 7453 6572 6961 6c69 7a65 72da 1744 7275  tSerializer..Dru
+000005d0: 6744 6972 6563 746f 7279 5365 7269 616c  gDirectorySerial
+000005e0: 697a 6572 da11 4170 6949 6e66 6f53 6572  izer..ApiInfoSer
+000005f0: 6961 6c69 7a65 72da 1849 6e73 7065 6374  ializer..Inspect
+00000600: 696f 6e54 7970 6553 6572 6961 6c69 7a65  ionTypeSerialize
+00000610: 72da 1945 7861 6d69 6e61 7469 6f6e 5479  r..ExaminationTy
+00000620: 7065 5365 7269 616c 697a 6572 2901 da14  peSerializer)...
+00000630: 5065 726d 6973 7369 6f6e 5365 7269 616c  PermissionSerial
+00000640: 697a 6572 2901 da08 7365 7474 696e 6773  izer)...settings
+00000650: 2901 da0f 786c 6461 7465 5f61 735f 7475  )...xldate_as_tu
+00000660: 706c 6563 0100 0000 0000 0000 0000 0000  plec............
+00000670: 0500 0000 0500 0000 4300 0000 7386 0000  ........C...s...
+00000680: 007c 006a 0064 016b 0272 8274 01a0 027c  .|.j.d.k.r.t...|
+00000690: 006a 03a0 0464 02a1 01a1 017d 017c 0164  .j...d.....}.|.d
+000006a0: 0319 007d 027c 0164 0419 007d 0374 056a  ...}.|.d...}.t.j
+000006b0: 066a 077c 0364 058d 01a0 08a1 007d 047c  .j.|.d.......}.|
+000006c0: 0472 767c 046a 0964 0675 0072 7664 077c  .rv|.j.d.u.rvd.|
+000006d0: 045f 097c 04a0 0a64 08a1 0101 007c 027c  ._.|...d.....|.|
+000006e0: 045f 0b7c 04a0 0ca1 0001 0074 0d64 0964  ._.|.......t.d.d
+000006f0: 0769 0183 0153 0074 0d64 0964 0a69 0183  .i...S.t.d.d.i..
+00000700: 0153 0064 0b53 0029 0c75 0f00 0000 e6b3  .S.d.S.).u......
+00000710: a8e5 868c e8af a6e6 8385 e9a1 b5da 0450  ...............P
+00000720: 4f53 54fa 0575 7466 2d38 da05 7068 6f6e  OST..utf-8..phon
+00000730: 65da 0875 7365 726e 616d 65a9 0172 3200  e..username..r2.
+00000740: 0000 4654 da06 3132 3334 3536 da04 6461  ..FT..123456..da
+00000750: 7461 7533 0000 00e8 afa5 e5b7 a5e5 8fb7  tau3............
+00000760: e994 99e8 afaf e688 96e8 8085 e5b7 b2e8  ................
+00000770: a2ab e6b3 a8e5 868c efbc 8ce8 afb7 e7a1  ................
+00000780: aee8 aea4 e5b7 a5e5 8fb7 4e29 0eda 066d  ..........N)...m
+00000790: 6574 686f 64da 046a 736f 6eda 056c 6f61  ethod..json..loa
+000007a0: 6473 da04 626f 6479 da06 6465 636f 6465  ds..body..decode
+000007b0: 7215 0000 00da 076f 626a 6563 7473 da06  r......objects..
+000007c0: 6669 6c74 6572 da05 6669 7273 74da 0969  filter..first..i
+000007d0: 735f 6163 7469 7665 da0c 7365 745f 7061  s_active..set_pa
+000007e0: 7373 776f 7264 7231 0000 00da 0473 6176  sswordr1.....sav
+000007f0: 6572 0600 0000 2905 da07 7265 7175 6573  er....)...reques
+00000800: 7472 3500 0000 7231 0000 0072 3200 0000  tr5...r1...r2...
+00000810: da04 7573 6572 a900 7243 0000 00fa 362f  ..user..rC....6/
+00000820: 686f 6d65 2f6c 7968 2f77 6f72 6b2f 4261  home/lyh/work/Ba
+00000830: 7365 4675 6e63 7469 6f6e 4d6f 6475 6c65  seFunctionModule
+00000840: 2f62 6173 655f 7379 7374 656d 2f76 6965  /base_system/vie
+00000850: 7773 2e70 79da 0872 6567 6973 7465 7229  ws.py..register)
+00000860: 0000 0073 1800 0000 0002 0a01 1201 0801  ...s............
+00000870: 0801 1202 0e02 0601 0a01 0601 0801 0c02  ................
+00000880: 7245 0000 0063 0100 0000 0000 0000 0000  rE...c..........
+00000890: 0000 0600 0000 0500 0000 4300 0000 737a  ..........C...sz
+000008a0: 0000 0074 00a0 017c 006a 02a0 0364 01a1  ...t...|.j...d..
+000008b0: 01a1 017d 0174 047c 0183 0101 007c 0164  ...}.t.|.....|.d
+000008c0: 0219 007d 027c 0164 0319 007d 0374 056a  ...}.|.d...}.t.j
+000008d0: 066a 077c 0264 048d 017d 047c 0372 767c  .j.|.d...}.|.rv|
+000008e0: 04a0 087c 03a1 0101 0064 057c 045f 0974  ...|.....d.|._.t
+000008f0: 0a6a 0aa0 0ba1 007c 045f 0c64 067c 045f  .j.....|._.d.|._
+00000900: 0d7c 04a0 0ea1 0001 0064 0764 0669 017d  .|.......d.d.i.}
+00000910: 0574 0f7c 0583 0153 0064 0853 0029 0975  .t.|...S.d.S.).u
+00000920: 1200 0000 e4bf aee6 94b9 e794 a8e6 88b7  ................
+00000930: e4bf a1e6 81af 7230 0000 00da 0775 7365  ......r0.....use
+00000940: 725f 6964 da08 7061 7373 776f 7264 2901  r_id..password).
+00000950: da02 6964 7201 0000 0054 7235 0000 004e  ..idr....Tr5...N
+00000960: 2910 7237 0000 0072 3800 0000 7239 0000  ).r7...r8...r9..
+00000970: 0072 3a00 0000 da05 7072 696e 7472 1500  .r:.....printr..
+00000980: 0000 723b 0000 00da 0367 6574 723f 0000  ..r;.....getr?..
+00000990: 00da 0b65 7272 6f72 5f74 696d 6573 da08  ...error_times..
+000009a0: 6461 7465 7469 6d65 da03 6e6f 77da 106c  datetime..now..l
+000009b0: 6173 745f 6368 616e 6765 5f74 696d 65da  ast_change_time.
+000009c0: 0d69 735f 6368 616e 6765 5f70 7764 7240  .is_change_pwdr@
+000009d0: 0000 0072 0600 0000 2906 7241 0000 0072  ...r....).rA...r
+000009e0: 3500 0000 7246 0000 0072 4700 0000 7242  5...rF...rG...rB
+000009f0: 0000 00da 0372 6573 7243 0000 0072 4300  .....resrC...rC.
+00000a00: 0000 7244 0000 00da 0f63 6861 6e67 655f  ..rD.....change_
+00000a10: 7061 7373 776f 7264 3c00 0000 731a 0000  password<...s...
+00000a20: 0000 0212 0108 0108 0108 010e 0204 010a  ................
+00000a30: 0106 010c 0106 0108 0108 0172 5100 0000  ...........rQ...
+00000a40: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000a50: 0002 0000 0040 0000 0073 2e00 0000 6500  .....@...s....e.
+00000a60: 5a01 6400 5a02 6401 5a03 6504 5a05 6506  Z.d.Z.d.Z.e.Z.e.
+00000a70: 6601 5a07 6402 5a08 6403 6404 8400 5a09  f.Z.d.Z.d.d...Z.
+00000a80: 6405 6406 8400 5a0a 6402 5300 2907 da0f  d.d...Z.d.S.)...
+00000a90: 5065 726d 6973 7369 6f6e 7356 6965 7775  PermissionsViewu
+00000aa0: 2800 0000 0a20 2020 20e8 8eb7 e58f 96e5  (....    .......
+00000ab0: bd93 e589 8de7 94a8 e688 b7e5 898d e7ab  ................
+00000ac0: afe6 9d83 e999 900a 2020 2020 4e63 0100  ........    Nc..
+00000ad0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+00000ae0: 0000 4300 0000 7308 0000 007c 006a 006a  ..C...s....|.j.j
+00000af0: 0153 0029 014e 2902 7241 0000 0072 4200  .S.).N).rA...rB.
+00000b00: 0000 2901 da04 7365 6c66 7243 0000 0072  ..)...selfrC...r
+00000b10: 4300 0000 7244 0000 00da 0a67 6574 5f6f  C...rD.....get_o
+00000b20: 626a 6563 7456 0000 0073 0200 0000 0001  bjectV...s......
+00000b30: 7a1a 5065 726d 6973 7369 6f6e 7356 6965  z.PermissionsVie
+00000b40: 772e 6765 745f 6f62 6a65 6374 6301 0000  w.get_objectc...
+00000b50: 0000 0000 0000 0000 0003 0000 0003 0000  ................
+00000b60: 0043 0000 0073 3400 0000 7c00 6a00 6a01  .C...s4...|.j.j.
+00000b70: 6a02 a003 a100 7d01 7c01 7226 7404 6a05  j.....}.|.r&t.j.
+00000b80: 6a06 7c01 6401 8d01 a007 a100 7d02 6e0a  j.|.d.......}.n.
+00000b90: 7404 6a05 a008 a100 7d02 7c02 5300 2902  t.j.....}.|.S.).
+00000ba0: 7524 0000 000a 2020 2020 2020 2020 e5be  u$....        ..
+00000bb0: 97e5 88b0 e8a7 92e8 89b2 e69d 83e9 9990  ................
+00000bc0: 0a20 2020 2020 2020 2029 015a 0967 726f  .        ).Z.gro
+00000bd0: 7570 5f5f 696e 2909 7241 0000 0072 4200  up__in).rA...rB.
+00000be0: 0000 da06 6772 6f75 7073 da03 616c 6c72  ....groups..allr
+00000bf0: 0400 0000 723b 0000 0072 3c00 0000 da08  ....r;...r<.....
+00000c00: 6469 7374 696e 6374 da04 6e6f 6e65 2903  distinct..none).
+00000c10: 7253 0000 0072 5500 0000 da0b 7065 726d  rS...rU.....perm
+00000c20: 6973 7369 6f6e 7372 4300 0000 7243 0000  issionsrC...rC..
+00000c30: 0072 4400 0000 da0c 6765 745f 7175 6572  .rD.....get_quer
+00000c40: 7973 6574 5900 0000 730a 0000 0000 050e  ysetY...s.......
+00000c50: 0104 0114 020a 017a 1c50 6572 6d69 7373  .......z.Permiss
+00000c60: 696f 6e73 5669 6577 2e67 6574 5f71 7565  ionsView.get_que
+00000c70: 7279 7365 7429 0bda 085f 5f6e 616d 655f  ryset)...__name_
+00000c80: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000c90: 5f71 7561 6c6e 616d 655f 5fda 075f 5f64  _qualname__..__d
+00000ca0: 6f63 5f5f 722c 0000 00da 1073 6572 6961  oc__r,.....seria
+00000cb0: 6c69 7a65 725f 636c 6173 7372 0d00 0000  lizer_classr....
+00000cc0: da12 7065 726d 6973 7369 6f6e 5f63 6c61  ..permission_cla
+00000cd0: 7373 6573 da10 7061 6769 6e61 7469 6f6e  sses..pagination
+00000ce0: 5f63 6c61 7373 7254 0000 0072 5a00 0000  _classrT...rZ...
+00000cf0: 7243 0000 0072 4300 0000 7243 0000 0072  rC...rC...rC...r
+00000d00: 4400 0000 7252 0000 004e 0000 0073 0c00  D...rR...N...s..
+00000d10: 0000 0801 0403 0401 0601 0402 0803 7252  ..............rR
+00000d20: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000d30: 0000 0000 0300 0000 4000 0000 731a 0000  ........@...s...
+00000d40: 0065 005a 0164 005a 0264 015a 0364 0564  .e.Z.d.Z.d.Z.d.d
+00000d50: 0364 0484 015a 0464 0253 0029 06da 1a4f  .d...Z.d.S.)...O
+00000d60: 7665 7272 6964 6555 7365 7241 7574 6865  verrideUserAuthe
+00000d70: 6e74 6963 6174 696f 6e75 5000 0000 0a20  nticationuP.... 
+00000d80: 2020 20e9 878d e586 99e7 94a8 e688 b7e9     .............
+00000d90: aa8c e8af 810a 2020 2020 4175 7468 656e  ......    Authen
+00000da0: 7469 6361 7465 7320 6167 6169 6e73 7420  ticates against 
+00000db0: 7365 7474 696e 6773 2e41 5554 485f 5553  settings.AUTH_US
+00000dc0: 4552 5f4d 4f44 454c 2e0a 2020 2020 4e63  ER_MODEL..    Nc
+00000dd0: 0500 0000 0000 0000 0000 0000 0c00 0000  ................
+00000de0: 0a00 0000 4b00 0000 736c 0000 007a 3264  ....K...sl...z2d
+00000df0: 017d 0674 007c 0683 017d 077c 07a0 017c  .}.t.|...}.|...|
+00000e00: 02a1 017d 087c 07a0 017c 03a1 017d 0974  ...}.|...|...}.t
+00000e10: 026a 036a 047c 0864 028d 017d 0a57 006e  .j.j.|.d...}.W.n
+00000e20: 2604 0074 0579 5801 007d 0b01 007a 0e57  &..t.yX..}...z.W
+00000e30: 0059 0064 007d 0b7e 0b64 0053 0064 007d  .Y.d.}.~.d.S.d.}
+00000e40: 0b7e 0b30 0030 007c 0aa0 067c 09a1 0172  .~.0.0.|...|...r
+00000e50: 687c 0a53 0064 0053 0029 034e da10 4b33  h|.S.d.S.).N..K3
+00000e60: 6244 4436 5a79 7475 7235 524c 434a 7233  bDD6Zytur5RLCJr3
+00000e70: 0000 0029 07da 0650 7944 4553 33da 0764  ...)...PyDES3..d
+00000e80: 6563 7279 7074 7215 0000 0072 3b00 0000  ecryptr....r;...
+00000e90: 724a 0000 00da 0945 7863 6570 7469 6f6e  rJ.....Exception
+00000ea0: da0e 6368 6563 6b5f 7061 7373 776f 7264  ..check_password
+00000eb0: 290c 7253 0000 0072 4100 0000 7232 0000  ).rS...rA...r2..
+00000ec0: 0072 4700 0000 5a05 6170 7073 73da 066b  .rG...Z.appss..k
+00000ed0: 7761 7267 73da 036b 6579 da05 7064 6573  wargs..key..pdes
+00000ee0: 32da 1064 6563 7279 7074 5f75 7365 726e  2..decrypt_usern
+00000ef0: 616d 655a 1064 6563 7279 7074 5f70 6173  ameZ.decrypt_pas
+00000f00: 7377 6f72 6472 4200 0000 da01 6572 4300  swordrB.....erC.
+00000f10: 0000 7243 0000 0072 4400 0000 da0c 6175  ..rC...rD.....au
+00000f20: 7468 656e 7469 6361 7465 6c00 0000 7314  thenticatel...s.
+00000f30: 0000 0000 0102 0104 0108 010a 010a 0112  ................
+00000f40: 010e 0318 020a 017a 274f 7665 7272 6964  .......z'Overrid
+00000f50: 6555 7365 7241 7574 6865 6e74 6963 6174  eUserAuthenticat
+00000f60: 696f 6e2e 6175 7468 656e 7469 6361 7465  ion.authenticate
+00000f70: 2903 4e4e 4e29 0572 5b00 0000 725c 0000  ).NNN).r[...r\..
+00000f80: 0072 5d00 0000 725e 0000 0072 6d00 0000  .r]...r^...rm...
+00000f90: 7243 0000 0072 4300 0000 7243 0000 0072  rC...rC...rC...r
+00000fa0: 4400 0000 7262 0000 0066 0000 0073 0400  D...rb...f...s..
+00000fb0: 0000 0801 0405 7262 0000 0063 0000 0000  ......rb...c....
+00000fc0: 0000 0000 0000 0000 0000 0000 0200 0000  ................
+00000fd0: 4000 0000 7324 0000 0065 005a 0164 005a  @...s$...e.Z.d.Z
+00000fe0: 0264 0164 0284 005a 0364 0364 0484 005a  .d.d...Z.d.d...Z
+00000ff0: 0464 0564 0684 005a 0564 0753 0029 0872  .d.d...Z.d.S.).r
+00001000: 6400 0000 6302 0000 0000 0000 0000 0000  d...c...........
+00001010: 0002 0000 0004 0000 0043 0000 0073 1600  .........C...s..
+00001020: 0000 7400 6a01 7c01 7400 6a02 6401 8d02  ..t.j.|.t.j.d...
+00001030: 7c00 5f03 6402 5300 2903 755d 0000 000a  |._.d.S.).u]....
+00001040: 2020 2020 2020 2020 e4b8 89e9 878d 4445          ......DE
+00001050: 53e5 8aa0 e5af 86e3 8081 e5af b9e7 a7b0  S...............
+00001060: e58a a0e5 af86 e380 8270 7932 e4b8 8be4  .........py2....
+00001070: b88d e58f afe7 94a8 0a20 2020 2020 2020  .........       
+00001080: 203a 7061 7261 6d20 6b65 793a 20e5 af86   :param key: ...
+00001090: e992 a50a 2020 2020 2020 2020 2901 5a07  ....        ).Z.
+000010a0: 7061 646d 6f64 654e 2904 da05 7079 4465  padmodeN)...pyDe
+000010b0: 735a 0a74 7269 706c 655f 6465 735a 0950  sZ.triple_desZ.P
+000010c0: 4144 5f50 4b43 5335 da07 6372 7970 746f  AD_PKCS5..crypto
+000010d0: 7229 0272 5300 0000 7269 0000 0072 4300  r).rS...ri...rC.
+000010e0: 0000 7243 0000 0072 4400 0000 da08 5f5f  ..rC...rD.....__
+000010f0: 696e 6974 5f5f 8700 0000 7302 0000 0000  init__....s.....
+00001100: 057a 0f50 7944 4553 332e 5f5f 696e 6974  .z.PyDES3.__init
+00001110: 5f5f 6302 0000 0000 0000 0000 0000 0003  __c.............
+00001120: 0000 0004 0000 0043 0000 0073 1e00 0000  .......C...s....
+00001130: 7c00 6a00 a001 7c01 a002 a100 a101 7d02  |.j...|.......}.
+00001140: 7403 a004 7c02 a101 a005 a100 5300 2901  t...|.......S.).
+00001150: 753e 0000 000a 2020 2020 2020 2020 e58a  u>....        ..
+00001160: a0e5 af86 0a20 2020 2020 2020 203a 7061  .....        :pa
+00001170: 7261 6d20 7465 7874 3a0a 2020 2020 2020  ram text:.      
+00001180: 2020 3a72 6574 7572 6e3a 0a20 2020 2020    :return:.     
+00001190: 2020 2029 0672 6f00 0000 da07 656e 6372     ).ro.....encr
+000011a0: 7970 74da 0665 6e63 6f64 65da 0662 6173  ypt..encode..bas
+000011b0: 6536 34da 1273 7461 6e64 6172 645f 6236  e64..standard_b6
+000011c0: 3465 6e63 6f64 6572 3a00 0000 a903 7253  4encoder:.....rS
+000011d0: 0000 00da 0474 6578 74da 0178 7243 0000  .....text..xrC..
+000011e0: 0072 4300 0000 7244 0000 0072 7100 0000  .rC...rD...rq...
+000011f0: 8e00 0000 7304 0000 0000 0610 017a 0e50  ....s........z.P
+00001200: 7944 4553 332e 656e 6372 7970 7463 0200  yDES3.encryptc..
+00001210: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+00001220: 0000 4300 0000 7322 0000 0074 00a0 017c  ..C...s"...t...|
+00001230: 01a0 02a1 00a1 017d 027c 006a 03a0 047c  .......}.|.j...|
+00001240: 02a1 017d 027c 02a0 05a1 0053 0029 0175  ...}.|.....S.).u
+00001250: 3e00 0000 0a20 2020 2020 2020 20e8 a7a3  >....        ...
+00001260: e5af 860a 2020 2020 2020 2020 3a70 6172  ....        :par
+00001270: 616d 2074 6578 743a 0a20 2020 2020 2020  am text:.       
+00001280: 203a 7265 7475 726e 3a0a 2020 2020 2020   :return:.      
+00001290: 2020 2906 7273 0000 00da 1273 7461 6e64    ).rs.....stand
+000012a0: 6172 645f 6236 3464 6563 6f64 6572 7200  ard_b64decoderr.
+000012b0: 0000 726f 0000 0072 6500 0000 723a 0000  ..ro...re...r:..
+000012c0: 0072 7500 0000 7243 0000 0072 4300 0000  .ru...rC...rC...
+000012d0: 7244 0000 0072 6500 0000 9700 0000 7306  rD...re.......s.
+000012e0: 0000 0000 060e 010c 017a 0e50 7944 4553  .........z.PyDES
+000012f0: 332e 6465 6372 7970 744e 2906 725b 0000  3.decryptN).r[..
+00001300: 0072 5c00 0000 725d 0000 0072 7000 0000  .r\...r]...rp...
+00001310: 7271 0000 0072 6500 0000 7243 0000 0072  rq...re...rC...r
+00001320: 4300 0000 7243 0000 0072 4400 0000 7264  C...rC...rD...rd
+00001330: 0000 0086 0000 0073 0600 0000 0801 0807  .......s........
+00001340: 0809 7264 0000 0063 0100 0000 0000 0000  ..rd...c........
+00001350: 0000 0000 1600 0000 0b00 0000 4300 0000  ............C...
+00001360: 73ac 0100 007c 006a 00a0 0164 01a1 017d  s....|.j...d...}
+00001370: 017c 006a 02a0 0164 0264 03a1 027d 027c  .|.j...d.d...}.|
+00001380: 026a 03a0 0464 04a1 0164 0519 00a0 0464  .j...d...d.....d
+00001390: 06a1 0164 0719 007d 0367 007d 047c 0364  ...d...}.g.}.|.d
+000013a0: 0876 0090 0172 8c90 017a 1c74 056a 0664  .v...r...z.t.j.d
+000013b0: 097c 02a0 07a1 0064 0a64 0b8d 037d 057c  .|.....d.d...}.|
+000013c0: 05a0 08a1 007d 067c 0644 005d f67d 077c  .....}.|.D.].}.|
+000013d0: 076a 097d 0874 0a64 0c7c 0883 0244 005d  .j.}.t.d.|...D.]
+000013e0: e07d 097c 07a0 0b7c 09a1 017d 0a7c 0a72  .}.|...|...}.|.r
+000013f0: 7a7c 07a0 0c7c 0964 07a1 026a 0d7d 0b7c  z|...|.d...j.}.|
+00001400: 07a0 0e7c 0964 07a1 027d 0c7c 0b64 0c6b  ...|.d...}.|.d.k
+00001410: 0272 c27c 0c64 0516 0064 076b 0272 c274  .r.|.d...d.k.r.t
+00001420: 0f7c 0c83 017d 0c7c 0a64 0519 007d 0d7c  .|...}.|.d...}.|
+00001430: 0a64 0c19 007d 0e74 106a 116a 017c 0e64  .d...}.t.j.j.|.d
+00001440: 0d8d 016a 127d 0f7c 0a64 0e19 007d 107c  ...j.}.|.d...}.|
+00001450: 0a64 0f19 007d 1174 136a 116a 147c 0c64  .d...}.t.j.j.|.d
+00001460: 108d 017d 127c 1290 0172 247c 126a 1566  ...}.|...r$|.j.f
+00001470: 0069 007c 0c7c 0d7c 0f7c 107c 1164 119c  .i.|.|.|.|.|.d..
+00001480: 05a4 018e 0101 006e 1c7c 126a 1666 0069  .......n.|.j.f.i
+00001490: 007c 0c7c 0d7c 0f7c 107c 1164 119c 05a4  .|.|.|.|.|.d....
+000014a0: 018e 0101 007c 0c7c 0d7c 0f7c 107c 1164  .....|.|.|.|.|.d
+000014b0: 119c 057d 137c 04a0 177c 13a1 0101 0071  ...}.|...|.....q
+000014c0: 7a71 6657 006e 2a04 0074 1890 0179 8a01  zqfW.n*..t...y..
+000014d0: 007d 1401 007a 107c 1482 0157 0059 0064  .}...z.|...W.Y.d
+000014e0: 097d 147e 146e 0a64 097d 147e 1430 0030  .}.~.n.d.}.~.0.0
+000014f0: 007c 0490 0172 9c64 127c 0469 017d 156e  .|...r.d.|.i.}.n
+00001500: 0864 1264 1369 017d 1574 197c 1583 0153  .d.d.i.}.t.|...S
+00001510: 0029 1475 1400 0000 e5af bce5 85a5 6578  .).u..........ex
+00001520: 6365 6ce8 a1a8 e695 b0e6 8dae da0c 6372  cel...........cr
+00001530: 6561 7465 645f 7573 6572 da0a 6578 6365  eated_user..exce
+00001540: 6c5f 6669 6c65 da00 da01 2ee9 0100 0000  l_file..........
+00001550: fa01 2272 0100 0000 a902 da04 786c 7378  .."r........xlsx
+00001560: 5a03 786c 734e 54a9 03da 0866 696c 656e  Z.xlsNT....filen
+00001570: 616d 65da 0d66 696c 655f 636f 6e74 656e  ame..file_conten
+00001580: 7473 5a0b 7261 6767 6564 5f72 6f77 73e9  tsZ.ragged_rows.
+00001590: 0200 0000 a901 da04 6e61 6d65 e903 0000  ........name....
+000015a0: 00e9 0400 0000 a901 da07 636f 6465 6e75  ..........codenu
+000015b0: 6d29 0572 8a00 0000 7286 0000 00da 0868  m).r....r......h
+000015c0: 6f73 7069 7461 6cda 0c63 7265 6174 6564  ospital..created
+000015d0: 5f74 696d 65da 0a63 7265 6174 6564 5f62  _time..created_b
+000015e0: 7972 3500 0000 f53f 0000 00e6 9687 e4bb  yr5....?........
+000015f0: b6e5 8685 e5ae b9e6 a0bc e5bc 8fe6 9c89  ................
+00001600: e8af afef bc8c e8af b7e6 a380 e69f a5e5  ................
+00001610: 8685 e5ae b9e6 a0bc e5bc 8fe6 98af e590  ................
+00001620: a6e6 ada3 e7a1 aeef bc81 291a 722f 0000  ..........).r/..
+00001630: 0072 4a00 0000 da05 4649 4c45 5372 8600  .rJ.....FILESr..
+00001640: 0000 da05 7370 6c69 74da 0478 6c72 64da  ....split..xlrd.
+00001650: 0d6f 7065 6e5f 776f 726b 626f 6f6b da04  .open_workbook..
+00001660: 7265 6164 da06 7368 6565 7473 da05 6e72  read..sheets..nr
+00001670: 6f77 73da 0572 616e 6765 da0a 726f 775f  ows..range..row_
+00001680: 7661 6c75 6573 da04 6365 6c6c da05 6374  values..cell..ct
+00001690: 7970 65da 0a63 656c 6c5f 7661 6c75 65da  ype..cell_value.
+000016a0: 0369 6e74 7211 0000 0072 3b00 0000 7248  .intr....r;...rH
+000016b0: 0000 0072 1400 0000 723c 0000 00da 0675  ...r....r<.....u
+000016c0: 7064 6174 65da 0663 7265 6174 65da 0661  pdate..create..a
+000016d0: 7070 656e 6472 6600 0000 7206 0000 0029  ppendrf...r....)
+000016e0: 1672 4100 0000 7279 0000 0072 7a00 0000  .rA...ry...rz...
+000016f0: da09 6669 6c65 5f74 7970 65da 0964 6174  ..file_type..dat
+00001700: 615f 6c69 7374 7235 0000 0072 9400 0000  a_listr5...r....
+00001710: da05 7368 6565 74da 0472 6f77 73da 0372  ..sheet..rows..r
+00001720: 6f77 7297 0000 0072 9900 0000 728a 0000  owr....r....r...
+00001730: 0072 8600 0000 da0d 686f 7370 6974 616c  .r......hospital
+00001740: 5f6e 616d 6572 8b00 0000 728c 0000 0072  _namer....r....r
+00001750: 8d00 0000 5a0d 706f 7369 7469 6f6e 7469  ....Z.positionti
+00001760: 746c 65da 0a65 7863 656c 5f64 6174 6172  tle..excel_datar
+00001770: 6c00 0000 7250 0000 0072 4300 0000 7243  l...rP...rC...rC
+00001780: 0000 0072 4400 0000 da15 696d 706f 7274  ...rD.....import
+00001790: 5f70 6f73 6974 696f 6e5f 7469 746c 65a2  _position_title.
+000017a0: 0000 0073 6200 0000 0003 0c01 0e01 1a02  ...sb...........
+000017b0: 0402 0a02 0401 1401 0801 0801 0601 0e01  ................
+000017c0: 0a01 0402 0e01 0c01 1401 0801 0801 0801  ................
+000017d0: 1001 0801 0801 0e01 0601 0a01 0201 0201  ................
+000017e0: 0201 02fc 0c07 0a01 0201 0201 0201 02fc  ................
+000017f0: 0a07 0201 0201 0201 0201 02fb 0607 1201  ................
+00001800: 1001 1a02 0601 0a02 0801 72a6 0000 0063  ..........r....c
+00001810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001820: 0400 0000 4000 0000 7340 0000 0065 005a  ....@...s@...e.Z
+00001830: 0164 005a 0265 036a 0464 0164 028d 015a  .d.Z.e.j.d.d...Z
+00001840: 0565 036a 0664 0364 0464 058d 025a 0765  .e.j.d.d.d...Z.e
+00001850: 036a 0664 0664 028d 015a 0847 0064 0764  .j.d.d...Z.G.d.d
+00001860: 0884 0064 0883 025a 0964 0953 0029 0ada  ...d...Z.d.S.)..
+00001870: 0a55 7365 7246 696c 7465 72da 0667 656e  .UserFilter..gen
+00001880: 6465 72a9 01da 0a66 6965 6c64 5f6e 616d  der....field_nam
+00001890: 6572 8600 0000 da09 6963 6f6e 7461 696e  er......icontain
+000018a0: 73a9 0272 aa00 0000 da0b 6c6f 6f6b 7570  s..r......lookup
+000018b0: 5f65 7870 72da 0a61 7661 7461 725f 7572  _expr..avatar_ur
+000018c0: 6c63 0000 0000 0000 0000 0000 0000 0000  lc..............
+000018d0: 0000 0100 0000 4000 0000 7314 0000 0065  ......@...s....e
+000018e0: 005a 0164 005a 0265 035a 0464 015a 0564  .Z.d.Z.e.Z.d.Z.d
+000018f0: 0253 0029 037a 0f55 7365 7246 696c 7465  .S.).z.UserFilte
+00001900: 722e 4d65 7461 da07 5f5f 616c 6c5f 5f4e  r.Meta..__all__N
+00001910: 2906 725b 0000 0072 5c00 0000 725d 0000  ).r[...r\...r]..
+00001920: 0072 1500 0000 da05 6d6f 6465 6cda 0666  .r......model..f
+00001930: 6965 6c64 7372 4300 0000 7243 0000 0072  ieldsrC...rC...r
+00001940: 4300 0000 7244 0000 00da 044d 6574 61e8  C...rD.....Meta.
+00001950: 0000 0073 0400 0000 0801 0401 72b2 0000  ...s........r...
+00001960: 004e 290a 725b 0000 0072 5c00 0000 725d  .N).r[...r\...r]
+00001970: 0000 00da 0766 696c 7465 7273 da0c 4e75  .....filters..Nu
+00001980: 6d62 6572 4669 6c74 6572 72a8 0000 00da  mberFilterr.....
+00001990: 0a43 6861 7246 696c 7465 7272 8600 0000  .CharFilterr....
+000019a0: 72ae 0000 0072 b200 0000 7243 0000 0072  r....r....rC...r
+000019b0: 4300 0000 7243 0000 0072 4400 0000 72a7  C...rC...rD...r.
+000019c0: 0000 00e0 0000 0073 0800 0000 0804 0c01  .......s........
+000019d0: 0e01 0c02 72a7 0000 0063 0000 0000 0000  ....r....c......
+000019e0: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
+000019f0: 0000 733e 0000 0065 005a 0164 005a 0265  ..s>...e.Z.d.Z.e
+00001a00: 036a 04a0 05a1 00a0 0664 01a1 015a 0765  .j.......d...Z.e
+00001a10: 085a 0965 0a5a 0b64 025a 0c65 0d64 0367  .Z.e.Z.d.Z.e.d.g
+00001a20: 0164 0464 058d 0264 0664 0784 0083 015a  .d.d...d.d.....Z
+00001a30: 0e64 0853 0029 09da 0b55 7365 7256 6965  .d.S.)...UserVie
+00001a40: 7753 6574 fa03 2d69 6472 af00 0000 da03  wSet..-idr......
+00001a50: 5055 5454 2902 da07 6d65 7468 6f64 73da  PUTT)...methods.
+00001a60: 0664 6574 6169 6c63 0300 0000 0000 0000  .detailc........
+00001a70: 0000 0000 0600 0000 0400 0000 4300 0000  ............C...
+00001a80: 736e 0000 0074 007c 016a 0164 017c 0169  sn...t.|.j.d.|.i
+00001a90: 0164 028d 027d 037c 036a 0264 0364 048d  .d...}.|.j.d.d..
+00001aa0: 0101 007c 036a 01a0 0364 05a1 017d 047c  ...|.j...d...}.|
+00001ab0: 00a0 04a1 007d 057c 05a0 057c 04a1 0101  .....}.|...|....
+00001ac0: 0074 066a 06a0 07a1 007c 055f 0864 067c  .t.j.....|._.d.|
+00001ad0: 055f 0964 077c 055f 0a7c 05a0 0ba1 0001  ._.d.|._.|......
+00001ae0: 0074 0c64 0864 0969 0174 0d6a 0e64 0a8d  .t.d.d.i.t.j.d..
+00001af0: 0253 0029 0b4e 7241 0000 0029 0272 3500  .S.).NrA...).r5.
+00001b00: 0000 da07 636f 6e74 6578 7454 2901 da0f  ....contextT)...
+00001b10: 7261 6973 655f 6578 6365 7074 696f 6e72  raise_exceptionr
+00001b20: 4700 0000 7201 0000 0046 da07 6d65 7373  G...r....F..mess
+00001b30: 6167 6575 0c00 0000 e4bf aee6 94b9 e688  ageu............
+00001b40: 90e5 8a9f a902 7235 0000 0072 0a00 0000  ......r5...r....
+00001b50: 290f 7224 0000 0072 3500 0000 da08 6973  ).r$...r5.....is
+00001b60: 5f76 616c 6964 724a 0000 0072 5400 0000  _validrJ...rT...
+00001b70: 723f 0000 0072 4c00 0000 724d 0000 0072  r?...rL...rM...r
+00001b80: 4e00 0000 724b 0000 0072 4f00 0000 7240  N...rK...rO...r@
+00001b90: 0000 0072 0e00 0000 720a 0000 00da 1648  ...r....r......H
+00001ba0: 5454 505f 3230 355f 5245 5345 545f 434f  TTP_205_RESET_CO
+00001bb0: 4e54 454e 5429 0672 5300 0000 7241 0000  NTENT).rS...rA..
+00001bc0: 00da 0270 6bda 0a73 6572 6961 6c69 7a65  ...pk..serialize
+00001bd0: 7272 4700 0000 7242 0000 0072 4300 0000  rrG...rB...rC...
+00001be0: 7243 0000 0072 4400 0000 7251 0000 00f3  rC...rD...rQ....
+00001bf0: 0000 0073 1400 0000 0003 1201 0c01 0c01  ...s............
+00001c00: 0801 0a01 0c01 0601 0601 0802 7a1b 5573  ............z.Us
+00001c10: 6572 5669 6577 5365 742e 6368 616e 6765  erViewSet.change
+00001c20: 5f70 6173 7377 6f72 644e 290f 725b 0000  _passwordN).r[..
+00001c30: 0072 5c00 0000 725d 0000 0072 1500 0000  .r\...r]...r....
+00001c40: 723b 0000 0072 5600 0000 da08 6f72 6465  r;...rV.....orde
+00001c50: 725f 6279 da08 7175 6572 7973 6574 7223  r_by..querysetr#
+00001c60: 0000 0072 5f00 0000 72a7 0000 00da 0f66  ...r_...r......f
+00001c70: 696c 7465 7273 6574 5f63 6c61 7373 da0d  ilterset_class..
+00001c80: 6669 6c74 6572 5f66 6965 6c64 7372 0b00  filter_fieldsr..
+00001c90: 0000 7251 0000 0072 4300 0000 7243 0000  ..rQ...rC...rC..
+00001ca0: 0072 4300 0000 7244 0000 0072 b600 0000  .rC...rD...r....
+00001cb0: ed00 0000 730c 0000 0008 0110 0104 0104  ....s...........
+00001cc0: 0104 020c 0172 b600 0000 6300 0000 0000  .....r....c.....
+00001cd0: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
+00001ce0: 0000 0073 2600 0000 6500 5a01 6400 5a02  ...s&...e.Z.d.Z.
+00001cf0: 6401 5a03 6504 6a05 6a06 6402 6403 8d01  d.Z.e.j.j.d.d...
+00001d00: 5a07 6508 5a09 6402 5a0a 6402 5300 2904  Z.e.Z.d.Z.d.S.).
+00001d10: da15 496e 7370 6563 7469 6f6e 5479 7065  ..InspectionType
+00001d20: 5669 6577 5365 74f5 0c00 0000 e6a3 80e6  ViewSet.........
+00001d30: 9fa5 e5ad 97e5 85b8 4ea9 01da 0670 6172  ........N....par
+00001d40: 656e 7429 0b72 5b00 0000 725c 0000 0072  ent).r[...r\...r
+00001d50: 5d00 0000 725e 0000 0072 2100 0000 723b  ]...r^...r!...r;
+00001d60: 0000 0072 3c00 0000 72c4 0000 0072 2a00  ...r<...r....r*.
+00001d70: 0000 725f 0000 0072 6100 0000 7243 0000  ..r_...ra...rC..
+00001d80: 0072 4300 0000 7243 0000 0072 4400 0000  .rC...rC...rD...
+00001d90: 72c7 0000 0003 0100 0073 0800 0000 0801  r........s......
+00001da0: 0401 0e01 0401 72c7 0000 0063 0000 0000  ......r....c....
+00001db0: 0000 0000 0000 0000 0000 0000 0400 0000  ................
+00001dc0: 4000 0000 7360 0000 0065 005a 0164 005a  @...s`...e.Z.d.Z
+00001dd0: 0265 036a 0464 0164 0264 038d 025a 0565  .e.j.d.d.d...Z.e
+00001de0: 036a 0464 0464 0264 038d 025a 0665 036a  .j.d.d.d...Z.e.j
+00001df0: 0464 0564 0264 038d 025a 0765 036a 0464  .d.d.d...Z.e.j.d
+00001e00: 0664 0264 038d 025a 0865 036a 0464 0764  .d.d...Z.e.j.d.d
+00001e10: 0264 038d 025a 0947 0064 0864 0984 0064  .d...Z.G.d.d...d
+00001e20: 0983 025a 0a64 0a53 0029 0bda 1449 6e73  ...Z.d.S.)...Ins
+00001e30: 7065 6374 696f 6e44 6963 7446 696c 7465  pectionDictFilte
+00001e40: 72da 0c70 726f 6a65 6374 5f63 6f64 6572  r..project_coder
+00001e50: ab00 0000 72ac 0000 00da 0c70 726f 6a65  ....r......proje
+00001e60: 6374 5f6e 616d 65da 0d68 6f73 7069 7461  ct_name..hospita
+00001e70: 6c5f 636f 6465 da0b 6f66 6669 6365 5f63  l_code..office_c
+00001e80: 6f64 65da 0b64 6973 7469 6e67 7569 7368  ode..distinguish
+00001e90: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00001ea0: 0001 0000 0040 0000 0073 1400 0000 6500  .....@...s....e.
+00001eb0: 5a01 6400 5a02 6503 5a04 6401 5a05 6402  Z.d.Z.e.Z.d.Z.d.
+00001ec0: 5300 2903 7a19 496e 7370 6563 7469 6f6e  S.).z.Inspection
+00001ed0: 4469 6374 4669 6c74 6572 2e4d 6574 6172  DictFilter.Metar
+00001ee0: af00 0000 4e29 0672 5b00 0000 725c 0000  ....N).r[...r\..
+00001ef0: 0072 5d00 0000 7217 0000 0072 b000 0000  .r]...r....r....
+00001f00: 72b1 0000 0072 4300 0000 7243 0000 0072  r....rC...rC...r
+00001f10: 4300 0000 7244 0000 0072 b200 0000 1101  C...rD...r......
+00001f20: 0000 7304 0000 0008 0104 0172 b200 0000  ..s........r....
+00001f30: 4ea9 0b72 5b00 0000 725c 0000 0072 5d00  N..r[...r\...r].
+00001f40: 0000 72b3 0000 0072 b500 0000 72cc 0000  ..r....r....r...
+00001f50: 0072 cd00 0000 72ce 0000 0072 cf00 0000  .r....r....r....
+00001f60: 72d0 0000 0072 b200 0000 7243 0000 0072  r....r....rC...r
+00001f70: 4300 0000 7243 0000 0072 4400 0000 72cb  C...rC...rD...r.
+00001f80: 0000 000a 0100 0073 0c00 0000 0801 0e01  .......s........
+00001f90: 0e01 0e01 0e01 0e02 72cb 0000 0063 0000  ........r....c..
+00001fa0: 0000 0000 0000 0000 0000 0000 0000 0300  ................
+00001fb0: 0000 4000 0000 7328 0000 0065 005a 0164  ..@...s(...e.Z.d
+00001fc0: 005a 0264 015a 0365 046a 05a0 06a1 00a0  .Z.d.Z.e.j......
+00001fd0: 0764 02a1 015a 0865 095a 0a65 0b5a 0c64  .d...Z.e.Z.e.Z.d
+00001fe0: 0353 0029 04da 1d49 6e73 7065 6374 696f  .S.)...Inspectio
+00001ff0: 6e44 6963 7469 6f6e 6172 6965 7356 6965  nDictionariesVie
+00002000: 7753 6574 72c8 0000 0072 b700 0000 4e29  wSetr....r....N)
+00002010: 0d72 5b00 0000 725c 0000 0072 5d00 0000  .r[...r\...r]...
+00002020: 725e 0000 0072 1700 0000 723b 0000 0072  r^...r....r;...r
+00002030: 5600 0000 72c3 0000 0072 c400 0000 7225  V...r....r....r%
+00002040: 0000 0072 5f00 0000 72cb 0000 0072 c500  ...r_...r....r..
+00002050: 0000 7243 0000 0072 4300 0000 7243 0000  ..rC...rC...rC..
+00002060: 0072 4400 0000 72d2 0000 0016 0100 0073  .rD...r........s
+00002070: 0800 0000 0801 0401 1001 0402 72d2 0000  ............r...
+00002080: 0063 0100 0000 0000 0000 0000 0000 0300  .c..............
+00002090: 0000 0300 0000 4300 0000 731a 0000 0074  ......C...s....t
+000020a0: 0083 007d 017c 01a0 01a1 007d 0274 0264  ...}.|.....}.t.d
+000020b0: 017c 0269 0183 0153 00a9 024e 7235 0000  .|.i...S...Nr5..
+000020c0: 0029 0372 1700 0000 da06 7570 6c6f 6164  .).r......upload
+000020d0: 7206 0000 0029 0372 4100 0000 5a07 696e  r....).rA...Z.in
+000020e0: 7370 6469 6372 5000 0000 7243 0000 0072  spdicrP...rC...r
+000020f0: 4300 0000 7244 0000 00da 1169 6e73 7065  C...rD.....inspe
+00002100: 6374 696f 6e5f 696d 706f 7274 1e01 0000  ction_import....
+00002110: 7306 0000 0000 0106 0108 0172 d500 0000  s..........r....
+00002120: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00002130: 0003 0000 0040 0000 0073 2600 0000 6500  .....@...s&...e.
+00002140: 5a01 6400 5a02 6401 5a03 6504 6a05 6a06  Z.d.Z.d.Z.e.j.j.
+00002150: 6402 6403 8d01 5a07 6508 5a09 6402 5a0a  d.d...Z.e.Z.d.Z.
+00002160: 6402 5300 2904 da16 4578 616d 696e 6174  d.S.)...Examinat
+00002170: 696f 6e54 7970 6556 6965 7753 6574 72c8  ionTypeViewSetr.
+00002180: 0000 004e 72c9 0000 0029 0b72 5b00 0000  ...Nr....).r[...
+00002190: 725c 0000 0072 5d00 0000 725e 0000 0072  r\...r]...r^...r
+000021a0: 2200 0000 723b 0000 0072 3c00 0000 72c4  "...r;...r<...r.
+000021b0: 0000 0072 2b00 0000 725f 0000 0072 6100  ...r+...r_...ra.
+000021c0: 0000 7243 0000 0072 4300 0000 7243 0000  ..rC...rC...rC..
+000021d0: 0072 4400 0000 72d6 0000 0024 0100 0073  .rD...r....$...s
+000021e0: 0800 0000 0801 0401 0e01 0401 72d6 0000  ............r...
+000021f0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00002200: 0000 0400 0000 4000 0000 7360 0000 0065  ......@...s`...e
+00002210: 005a 0164 005a 0265 036a 0464 0164 0264  .Z.d.Z.e.j.d.d.d
+00002220: 038d 025a 0565 036a 0464 0464 0264 038d  ...Z.e.j.d.d.d..
+00002230: 025a 0665 036a 0464 0564 0264 038d 025a  .Z.e.j.d.d.d...Z
+00002240: 0765 036a 0464 0664 0264 038d 025a 0865  .e.j.d.d.d...Z.e
+00002250: 036a 0464 0764 0264 038d 025a 0947 0064  .j.d.d.d...Z.G.d
+00002260: 0864 0984 0064 0983 025a 0a64 0a53 0029  .d...d...Z.d.S.)
+00002270: 0bda 1545 7861 6d69 6e61 7469 6f6e 4469  ...ExaminationDi
+00002280: 6374 4669 6c74 6572 72cc 0000 0072 ab00  ctFilterr....r..
+00002290: 0000 72ac 0000 0072 cd00 0000 72ce 0000  ..r....r....r...
+000022a0: 0072 cf00 0000 72d0 0000 0063 0000 0000  .r....r....c....
+000022b0: 0000 0000 0000 0000 0000 0000 0100 0000  ................
+000022c0: 4000 0000 7314 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
+000022d0: 0265 035a 0464 015a 0564 0253 0029 037a  .e.Z.d.Z.d.S.).z
+000022e0: 1a45 7861 6d69 6e61 7469 6f6e 4469 6374  .ExaminationDict
+000022f0: 4669 6c74 6572 2e4d 6574 6172 af00 0000  Filter.Metar....
+00002300: 4e29 0672 5b00 0000 725c 0000 0072 5d00  N).r[...r\...r].
+00002310: 0000 7218 0000 0072 b000 0000 72b1 0000  ..r....r....r...
+00002320: 0072 4300 0000 7243 0000 0072 4300 0000  .rC...rC...rC...
+00002330: 7244 0000 0072 b200 0000 3201 0000 7304  rD...r....2...s.
+00002340: 0000 0008 0104 0172 b200 0000 4e72 d100  .......r....Nr..
+00002350: 0000 7243 0000 0072 4300 0000 7243 0000  ..rC...rC...rC..
+00002360: 0072 4400 0000 72d7 0000 002b 0100 0073  .rD...r....+...s
+00002370: 0c00 0000 0801 0e01 0e01 0e01 0e01 0e02  ................
+00002380: 72d7 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00002390: 0000 0000 0000 0300 0000 4000 0000 7328  ..........@...s(
+000023a0: 0000 0065 005a 0164 005a 0264 015a 0365  ...e.Z.d.Z.d.Z.e
+000023b0: 046a 05a0 06a1 00a0 0764 02a1 015a 0865  .j.......d...Z.e
+000023c0: 095a 0a65 0b5a 0c64 0353 0029 04da 1e45  .Z.e.Z.d.S.)...E
+000023d0: 7861 6d69 6e61 7469 6f6e 4469 6374 696f  xaminationDictio
+000023e0: 6e61 7269 6573 5669 6577 5365 7475 0c00  nariesViewSetu..
+000023f0: 0000 e6a3 80e9 aa8c e5ad 97e5 85b8 72b7  ..............r.
+00002400: 0000 004e 290d 725b 0000 0072 5c00 0000  ...N).r[...r\...
+00002410: 725d 0000 0072 5e00 0000 7218 0000 0072  r]...r^...r....r
+00002420: 3b00 0000 7256 0000 0072 c300 0000 72c4  ;...rV...r....r.
+00002430: 0000 0072 2600 0000 725f 0000 0072 d700  ...r&...r_...r..
+00002440: 0000 72c5 0000 0072 4300 0000 7243 0000  ..r....rC...rC..
+00002450: 0072 4300 0000 7244 0000 0072 d800 0000  .rC...rD...r....
+00002460: 3701 0000 7308 0000 0008 0104 0110 0104  7...s...........
+00002470: 0272 d800 0000 6301 0000 0000 0000 0000  .r....c.........
+00002480: 0000 0003 0000 0003 0000 0043 0000 0073  ...........C...s
+00002490: 1a00 0000 7400 8300 7d01 7c01 a001 a100  ....t...}.|.....
+000024a0: 7d02 7402 6401 7c02 6901 8301 5300 72d3  }.t.d.|.i...S.r.
+000024b0: 0000 0029 0372 1800 0000 72d4 0000 0072  ...).r....r....r
+000024c0: 0600 0000 2903 7241 0000 005a 0665 7861  ....).rA...Z.exa
+000024d0: 6469 6372 5000 0000 7243 0000 0072 4300  dicrP...rC...rC.
+000024e0: 0000 7244 0000 00da 1265 7861 6d69 6e61  ..rD.....examina
+000024f0: 7469 6f6e 5f69 6d70 6f72 743e 0100 0073  tion_import>...s
+00002500: 0600 0000 0001 0601 0801 72d9 0000 0063  ..........r....c
+00002510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002520: 0300 0000 4000 0000 7328 0000 0065 005a  ....@...s(...e.Z
+00002530: 0164 005a 0264 015a 0365 046a 05a0 06a1  .d.Z.d.Z.e.j....
+00002540: 00a0 0764 02a1 015a 0865 095a 0a64 035a  ...d...Z.e.Z.d.Z
+00002550: 0b64 0453 0029 05da 1950 6861 726d 6163  .d.S.)...Pharmac
+00002560: 794d 616e 6167 656d 656e 7456 6965 7753  yManagementViewS
+00002570: 6574 750c 0000 00e8 8daf e688 bfe7 aea1  etu.............
+00002580: e790 8672 b700 0000 72af 0000 004e 290c  ...r....r....N).
+00002590: 725b 0000 0072 5c00 0000 725d 0000 0072  r[...r\...r]...r
+000025a0: 5e00 0000 721a 0000 0072 3b00 0000 7256  ^...r....r;...rV
+000025b0: 0000 0072 c300 0000 72c4 0000 0072 2700  ...r....r....r'.
+000025c0: 0000 725f 0000 0072 c600 0000 7243 0000  ..r_...r....rC..
+000025d0: 0072 4300 0000 7243 0000 0072 4400 0000  .rC...rC...rD...
+000025e0: 72da 0000 0044 0100 0073 0800 0000 0801  r....D...s......
+000025f0: 0401 1001 0401 72da 0000 0063 0100 0000  ......r....c....
+00002600: 0000 0000 0000 0000 1900 0000 0f00 0000  ................
+00002610: 4300 0000 7306 0200 007c 006a 00a0 0164  C...s....|.j...d
+00002620: 01a1 017d 017c 006a 02a0 0164 0264 03a1  ...}.|.j...d.d..
+00002630: 027d 027c 026a 03a0 0464 04a1 0164 0519  .}.|.j...d...d..
+00002640: 00a0 0464 06a1 0164 0719 007d 0367 007d  ...d...d...}.g.}
+00002650: 047c 0364 0876 0090 0172 e690 017a 7674  .|.d.v...r...zvt
+00002660: 056a 0664 097c 02a0 07a1 0064 0a64 0b8d  .j.d.|.....d.d..
+00002670: 037d 057c 05a0 08a1 007d 067c 0644 0090  .}.|.....}.|.D..
+00002680: 015d 4e7d 077c 076a 097d 0874 0a64 0c7c  .]N}.|.j.}.t.d.|
+00002690: 0883 0244 0090 015d 367d 097c 07a0 0b7c  ...D...]6}.|...|
+000026a0: 09a1 017d 0a7c 0a72 7c7c 07a0 0c7c 0964  ...}.|.r||...|.d
+000026b0: 07a1 026a 0d7d 0b7c 07a0 0e7c 0964 07a1  ...j.}.|...|.d..
+000026c0: 027d 0c7c 0b64 0c6b 0272 c67c 0c64 0516  .}.|.d.k.r.|.d..
+000026d0: 0064 076b 0272 c674 0f7c 0c83 017d 0c7c  .d.k.r.t.|...}.|
+000026e0: 0a64 0519 007d 0d7c 0a64 0c19 007d 0e74  .d...}.|.d...}.t
+000026f0: 106a 116a 017c 0e64 0d8d 016a 127d 0f7c  .j.j.|.d...j.}.|
+00002700: 0a64 0e19 007d 107c 1090 0172 0674 136a  .d...}.|...r.t.j
+00002710: 116a 017c 1064 0d8d 016a 127d 116e 0464  .j.|.d...j.}.n.d
+00002720: 097d 117c 0a64 0f19 007d 127c 0a64 1019  .}.|.d...}.|.d..
+00002730: 007d 137c 0a64 1119 007d 1474 136a 116a  .}.|.d...}.t.j.j
+00002740: 147c 0c64 128d 017d 157c 1590 0172 627c  .|.d...}.|...rb|
+00002750: 156a 1566 0069 007c 0c7c 0d7c 0f7c 117c  .j.f.i.|.|.|.|.|
+00002760: 127c 137c 1474 166a 16a0 17a1 007c 0164  .|.|.t.j.....|.d
+00002770: 139c 09a4 018e 0101 006e 2a7c 156a 1866  .........n*|.j.f
+00002780: 0069 007c 0c7c 0d7c 0f7c 117c 127c 137c  .i.|.|.|.|.|.|.|
+00002790: 1474 166a 16a0 17a1 007c 0164 139c 09a4  .t.j.....|.d....
+000027a0: 018e 0101 007c 0c7c 0d7c 0f7c 117c 127c  .....|.|.|.|.|.|
+000027b0: 137c 1474 166a 16a0 17a1 007c 0164 149c  .|.t.j.....|.d..
+000027c0: 097d 167c 04a0 197c 16a1 0101 0071 7c71  .}.|...|.....q|q
+000027d0: 6657 006e 2a04 0074 1a90 0179 e401 007d  fW.n*..t...y...}
+000027e0: 1701 007a 107c 1782 0157 0059 0064 097d  ...z.|...W.Y.d.}
+000027f0: 177e 176e 0a64 097d 177e 1730 0030 007c  .~.n.d.}.~.0.0.|
+00002800: 0490 0172 f664 157c 0469 017d 186e 0864  ...r.d.|.i.}.n.d
+00002810: 1564 1669 017d 1874 1b7c 1883 0153 0029  .d.i.}.t.|...S.)
+00002820: 1775 1a00 0000 e5af bce5 85a5 6578 6365  .u..........exce
+00002830: 6ce8 a1a8 e7a7 91e5 aea4 e695 b0e6 8dae  l...............
+00002840: 7279 0000 0072 7a00 0000 727b 0000 0072  ry...rz...r{...r
+00002850: 7c00 0000 727d 0000 0072 7e00 0000 7201  |...r}...r~...r.
+00002860: 0000 0072 7f00 0000 4e54 7281 0000 0072  ...r....NTr....r
+00002870: 8400 0000 7285 0000 0072 8700 0000 7288  ....r....r....r.
+00002880: 0000 00e9 0500 0000 e906 0000 0072 8900  .............r..
+00002890: 0000 2909 728a 0000 0072 8600 0000 da0b  ..).r....r......
+000028a0: 686f 7370 6974 616c 5f69 64da 0970 6172  hospital_id..par
+000028b0: 656e 745f 6964 da07 6164 6472 6573 7372  ent_id..addressr
+000028c0: 3100 0000 da09 696e 7472 6f64 7563 6572  1.....introducer
+000028d0: 8c00 0000 728d 0000 0029 0972 8a00 0000  ....r....).r....
+000028e0: 7286 0000 0072 8b00 0000 72ca 0000 0072  r....r....r....r
+000028f0: df00 0000 7231 0000 0072 e000 0000 728c  ....r1...r....r.
+00002900: 0000 0072 8d00 0000 7235 0000 0072 8e00  ...r....r5...r..
+00002910: 0000 291c 722f 0000 0072 4a00 0000 728f  ..).r/...rJ...r.
+00002920: 0000 0072 8600 0000 7290 0000 00da 0578  ...r....r......x
+00002930: 6c72 6432 7292 0000 0072 9300 0000 7294  lrd2r....r....r.
+00002940: 0000 0072 9500 0000 7296 0000 0072 9700  ...r....r....r..
+00002950: 0000 7298 0000 0072 9900 0000 729a 0000  ..r....r....r...
+00002960: 0072 9b00 0000 7211 0000 0072 3b00 0000  .r....r....r;...
+00002970: 7248 0000 0072 1200 0000 723c 0000 0072  rH...r....r<...r
+00002980: 9c00 0000 724c 0000 0072 4d00 0000 729d  ....rL...rM...r.
+00002990: 0000 0072 9e00 0000 7266 0000 0072 0600  ...r....rf...r..
+000029a0: 0000 2919 7241 0000 0072 7900 0000 727a  ..).rA...ry...rz
+000029b0: 0000 0072 9f00 0000 72a0 0000 0072 3500  ...r....r....r5.
+000029c0: 0000 7294 0000 0072 a100 0000 72a2 0000  ..r....r....r...
+000029d0: 0072 a300 0000 7297 0000 0072 9900 0000  .r....r....r....
+000029e0: 728a 0000 0072 8600 0000 72a4 0000 0072  r....r....r....r
+000029f0: 8b00 0000 da0b 7061 7265 6e74 5f6e 616d  ......parent_nam
+00002a00: 6572 ca00 0000 72df 0000 0072 3100 0000  er....r....r1...
+00002a10: 72e0 0000 00da 066f 6666 6963 6572 a500  r......officer..
+00002a20: 0000 726c 0000 0072 5000 0000 7243 0000  ..rl...rP...rC..
+00002a30: 0072 4300 0000 7244 0000 00da 0d69 6d70  .rC...rD.....imp
+00002a40: 6f72 745f 6f66 6669 6365 4b01 0000 7384  ort_officeK...s.
+00002a50: 0000 0000 030c 010e 011a 0204 020a 0204  ................
+00002a60: 0114 0108 010a 0106 0110 010a 0104 020e  ................
+00002a70: 010c 0114 0108 0108 0108 0110 0108 0106  ................
+00002a80: 0112 0204 0108 0108 0108 030e 0106 010a  ................
+00002a90: 0102 0102 0102 0102 0102 0102 0108 0102  ................
+00002aa0: f80c 0b0a 0102 0102 0102 0102 0102 0102  ................
+00002ab0: 0108 0102 f80a 0b02 0102 0102 0102 0102  ................
+00002ac0: 0102 0102 0108 0102 f706 0b12 0110 011a  ................
+00002ad0: 0206 010a 0208 0172 e400 0000 6301 0000  .......r....c...
+00002ae0: 0000 0000 0000 0000 0031 0000 0013 0000  .........1......
+00002af0: 0043 0000 0073 9e04 0000 7c00 6a00 a001  .C...s....|.j...
+00002b00: 6401 a101 7d01 7c00 6a02 a001 6402 6403  d...}.|.j...d.d.
+00002b10: a102 7d02 7c02 6a03 a004 6404 a101 6405  ..}.|.j...d...d.
+00002b20: 1900 a004 6406 a101 6407 1900 7d03 6700  ....d...d...}.g.
+00002b30: 7d04 7c03 6408 7600 9004 727e 9004 7a0e  }.|.d.v...r~..z.
+00002b40: 7405 6a06 6409 7c02 a007 a100 640a 640b  t.j.d.|.....d.d.
+00002b50: 8d03 7d05 7c05 a008 a100 7d06 7c06 4400  ..}.|.....}.|.D.
+00002b60: 9003 5de6 7d07 7c07 6a09 7d08 740a 640c  ..].}.|.j.}.t.d.
+00002b70: 7c08 8302 4400 9003 5dce 7d09 7c07 a00b  |...D...].}.|...
+00002b80: 7c09 a101 7d0a 7c0a 727c 7c07 a00c 7c09  |...}.|.r||...|.
+00002b90: 640c a102 6a0d 7d0b 7c07 a00e 7c09 640c  d...j.}.|...|.d.
+00002ba0: a102 7d0c 7c0b 640c 6b02 72c6 7c0c 6405  ..}.|.d.k.r.|.d.
+00002bb0: 1600 6407 6b02 72c6 740f 7c0c 8301 7d0c  ..d.k.r.t.|...}.
+00002bc0: 7c0a 640d 1900 7d0d 7c0a 6407 1900 7d0e  |.d...}.|.d...}.
+00002bd0: 7410 6a11 6a12 7c0e 640e 8d01 a013 a100  t.j.j.|.d.......
+00002be0: 7d0f 7c0f 72f4 7c0f 6a14 7d10 6e26 7c0c  }.|.r.|.j.}.n&|.
+00002bf0: 7c0d 7c0e 6409 6409 6409 6409 6409 7c01  |.|.d.d.d.d.d.|.
+00002c00: 640f 6410 9c0a 7d11 7c04 a015 7c11 a101  d.d...}.|...|...
+00002c10: 0100 717c 7c0a 6405 1900 7d12 7c12 9001  ..q||.d...}.|...
+00002c20: 726e 7416 6a11 6a12 7c12 7c10 6411 8d02  rnt.j.j.|.|.d...
+00002c30: a013 a100 7d13 7c13 9001 724a 7c13 6a14  ....}.|...rJ|.j.
+00002c40: 7d14 6e24 7c0c 7c0d 7c0e 7c12 6409 6409  }.n$|.|.|.|.d.d.
+00002c50: 6409 7c01 6412 6413 9c09 7d11 7c04 a015  d.|.d.d...}.|...
+00002c60: 7c11 a101 0100 717c 7c0a 6414 1900 7d15  |.....q||.d...}.
+00002c70: 7c15 9001 72a0 7c15 6415 6b02 9001 728c  |...r.|.d.k...r.
+00002c80: 6416 7d16 6e14 7c15 6417 6b02 9001 729c  d.}.n.|.d.k...r.
+00002c90: 6418 7d16 6e04 6409 7d16 7c0a 6419 1900  d.}.n.d.}.|.d...
+00002ca0: 7d17 7c17 9001 72b6 740f 7c17 8301 7d18  }.|...r.t.|...}.
+00002cb0: 7c0a 641a 1900 7d19 7c19 9001 72cc 740f  |.d...}.|...r.t.
+00002cc0: 7c19 8301 7d1a 7c0a 641b 1900 7d1b 7c1b  |...}.|.d...}.|.
+00002cd0: 9002 7220 7417 6a11 6a12 7c1b 7c10 6411  ..r t.j.j.|.|.d.
+00002ce0: 8d02 a013 a100 7d1c 7c1c 9001 72fc 7c1c  ......}.|...r.|.
+00002cf0: 6a14 7d1d 6e24 7c0c 7c0d 7c0e 7c12 7c1b  j.}.n$|.|.|.|.|.
+00002d00: 6409 6409 7c01 641c 6413 9c09 7d11 7c04  d.d.|.d.d...}.|.
+00002d10: a015 7c11 a101 0100 717c 7c0a 641d 1900  ..|.....q||.d...
+00002d20: 7d1e 7c0a 641e 1900 7d1f 7c1f 641f 6b02  }.|.d...}.|.d.k.
+00002d30: 9002 7240 640a 7d20 6e04 6420 7d20 7418  ..r@d.} n.d } t.
+00002d40: 6a11 6a12 7c0c 6421 8d01 7d21 7c21 9002  j.j.|.d!..}!|!..
+00002d50: 7290 7c21 6a19 6600 6900 7c0c 7c0d 7c10  r.|!j.f.i.|.|.|.
+00002d60: 7c14 7c1d 7c1c 6a03 7c1e 7c16 7c18 7c1a  |.|.|.j.|.|.|.|.
+00002d70: 7c20 741a 6a1a a01b a100 7c01 6422 9c0d  | t.j.....|.d"..
+00002d80: a401 8e01 0100 9001 6e94 7c21 6a1c 6600  ........n.|!j.f.
+00002d90: 6900 7c0c 7c0d 7c10 7c14 7c1d 7c1c 6a03  i.|.|.|.|.|.|.j.
+00002da0: 7c1e 7c16 7c18 7c1a 7c20 741a 6a1a a01b  |.|.|.|.| t.j...
+00002db0: a100 7c01 6423 9c0d a401 8e01 7d22 741d  ..|.d#......}"t.
+00002dc0: 6a11 6a1c 6600 6900 7c0d 7c0c 6424 741e  j.j.f.i.|.|.d$t.
+00002dd0: 6425 8301 7c22 6a14 7c10 7c14 7c1d 7c16  d%..|"j.|.|.|.|.
+00002de0: 7c18 7c1a 7c01 6426 9c0c a401 8e01 0100  |.|.|.d&........
+00002df0: 7c20 9004 7224 741f 7c0e 8301 7d23 741f  | ..r$t.|...}#t.
+00002e00: 7c1b 8301 7d24 6427 7c23 9b00 6428 7c24  |...}$d'|#..d(|$
+00002e10: 9b00 9d04 7d25 7420 6a11 6a12 7c25 7c10  ....}%t j.j.|%|.
+00002e20: 6429 8d02 a013 a100 7d26 642a 7c23 9b00  d)......}&d*|#..
+00002e30: 6428 7c24 9b00 9d04 7d27 7420 6a11 6a12  d(|$....}'t j.j.
+00002e40: 7c27 7c10 6429 8d02 a013 a100 7d28 642b  |'|.d)......}(d+
+00002e50: 7c23 9b00 6428 7c24 9b00 9d04 7d29 7420  |#..d(|$....})t 
+00002e60: 6a11 6a12 7c29 7c10 6429 8d02 a013 a100  j.j.|)|.d)......
+00002e70: 7d2a 642c 7c23 9b00 6428 7c24 9b00 9d04  }*d,|#..d(|$....
+00002e80: 7d2b 7420 6a11 6a12 7c2b 7c10 6429 8d02  }+t j.j.|+|.d)..
+00002e90: a013 a100 7d2c 7c26 9003 73b4 7c28 9003  ....},|&..s.|(..
+00002ea0: 73b4 7c2a 9003 73b4 7c2c 9003 72fa 6700  s.|*..s.|,..r.g.
+00002eb0: 7d2d 7c2d a015 7c26 a101 0100 7c2d a015  }-|-..|&....|-..
+00002ec0: 7c28 a101 0100 7c2d a015 7c2a a101 0100  |(....|-..|*....
+00002ed0: 7c2d a015 7c2c a101 0100 7c2d 4400 5d12  |-..|,....|-D.].
+00002ee0: 7d2e 7c2e 6a21 a022 7c22 a101 0100 9003  }.|.j!."|"......
+00002ef0: 71e4 6e2a 7c0c 7c0d 7c0e 7c12 7c1b 7c1f  q.n*|.|.|.|.|.|.
+00002f00: 741a 6a1a a01b a100 7c01 642d 6413 9c09  t.j.....|.d-d...
+00002f10: 7d11 7c04 a015 7c11 a101 0100 717c 7c0c  }.|...|.....q||.
+00002f20: 7c0d 7c0e 7c12 7c1b 7c1f 741a 6a1a a01b  |.|.|.|.|.t.j...
+00002f30: a100 7c01 642e 6413 9c09 7d11 7c04 a015  ..|.d.d...}.|...
+00002f40: 7c11 a101 0100 717c 7166 5700 6e2a 0400  |.....q|qfW.n*..
+00002f50: 7423 9004 797c 0100 7d2f 0100 7a10 7c2f  t#..y|..}/..z.|/
+00002f60: 8201 5700 5900 6409 7d2f 7e2f 6e0a 6409  ..W.Y.d.}/~/n.d.
+00002f70: 7d2f 7e2f 3000 3000 7c04 9004 728e 642f  }/~/0.0.|...r.d/
+00002f80: 7c04 6901 7d30 6e08 642f 6430 6901 7d30  |.i.}0n.d/d0i.}0
+00002f90: 7424 7c30 8301 5300 2931 751a 0000 00e5  t$|0..S.)1u.....
+00002fa0: afbc e585 a565 7863 656c e8a1 a8e5 8cbb  .....excel......
+00002fb0: e794 9fe6 95b0 e68d ae72 7900 0000 727a  .........ry...rz
+00002fc0: 0000 0072 7b00 0000 727c 0000 0072 7d00  ...r{...r|...r}.
+00002fd0: 0000 727e 0000 0072 0100 0000 727f 0000  ..r~...r....r...
+00002fe0: 004e 5472 8100 0000 7284 0000 0072 8700  .NTr....r....r..
+00002ff0: 0000 7285 0000 0075 2700 0000 e58c bbe9  ..r....u'.......
+00003000: 99a2 e69f a5e8 afa2 e69c 89e8 afaf efbc  ................
+00003010: 8ce8 afb7 e6a3 80e6 9fa5 efbc 81ef bc81  ................
+00003020: efbc 8129 0ada 0a6a 6f62 5f6e 756d 6265  ...)...job_numbe
+00003030: 7272 8600 0000 728b 0000 00da 0b6f 6666  rr....r......off
+00003040: 6963 655f 6e61 6d65 da0d 646f 635f 7261  ice_name..doc_ra
+00003050: 6e6b 5f6e 616d 65da 0864 6573 6372 6962  nk_name..describ
+00003060: 65da 1169 735f 6f6e 6c69 6e65 5f63 6f6e  e..is_online_con
+00003070: 7375 6c74 728c 0000 0072 8d00 0000 da03  sultr....r......
+00003080: 6d73 6729 0272 8600 0000 72dd 0000 0075  msg).r....r....u
+00003090: 6300 0000 e8af a5e6 9da1 e8ae b0e5 bd95  c...............
+000030a0: e58c bbe9 99a2 e4b8 8be7 9a84 e7a7 91e5  ................
+000030b0: aea4 e69f a5e8 afa2 e69c 89e8 afaf efbc  ................
+000030c0: 8ce8 afb7 e6a3 80e6 9fa5 efbc 81ef bc81  ................
+000030d0: efbc 81e5 b7b2 e887 aae5 8aa8 e8b7 b3e8  ................
+000030e0: bf87 e8af a5e6 9da1 e8ae b0e5 bd95 e79a  ................
+000030f0: 84e5 afbc e585 a529 0972 e500 0000 7286  .......).r....r.
+00003100: 0000 0072 8b00 0000 72e6 0000 0072 e700  ...r....r....r..
+00003110: 0000 72e9 0000 0072 8c00 0000 728d 0000  ..r....r....r...
+00003120: 0072 ea00 0000 7288 0000 0075 0300 0000  .r....r....u....
+00003130: e794 b7da 0131 7503 0000 00e5 a5b3 da01  .....1u.........
+00003140: 3072 db00 0000 72dc 0000 00e9 0700 0000  0r....r.........
+00003150: 7563 0000 00e8 afa5 e69d a1e8 aeb0 e5bd  uc..............
+00003160: 95e5 8cbb e999 a2e4 b88b e79a 84e8 818c  ................
+00003170: e7a7 b0e6 9fa5 e8af a2e6 9c89 e8af afef  ................
+00003180: bc8c e8af b7e6 a380 e69f a5ef bc81 efbc  ................
+00003190: 81ef bc81 e5b7 b2e8 87aa e58a a8e8 b7b3  ................
+000031a0: e8bf 87e8 afa5 e69d a1e8 aeb0 e5bd 95e7  ................
+000031b0: 9a84 e5af bce5 85a5 e908 0000 00e9 0900  ................
+000031c0: 0000 f503 0000 00e6 98af 4629 0172 e500  ..........F).r..
+000031d0: 0000 290d 72e5 0000 0072 8600 0000 72dd  ..).r....r....r.
+000031e0: 0000 00da 096f 6666 6963 655f 6964 da0b  .....office_id..
+000031f0: 646f 635f 7261 6e6b 5f69 64da 0870 6f73  doc_rank_id..pos
+00003200: 6974 696f 6e72 e800 0000 72a8 0000 0072  itionr....r....r
+00003210: 3100 0000 da05 6964 6e75 6d72 e900 0000  1.....idnumr....
+00003220: da0c 7570 6461 7465 645f 7469 6d65 728d  ..updated_timer.
+00003230: 0000 0029 0d72 e500 0000 7286 0000 0072  ...).r....r....r
+00003240: dd00 0000 72f1 0000 0072 f200 0000 72f3  ....r....r....r.
+00003250: 0000 0072 e800 0000 72a8 0000 0072 3100  ...r....r....r1.
+00003260: 0000 72f4 0000 0072 e900 0000 728c 0000  ..r....r....r...
+00003270: 0072 8d00 0000 7a0a 3131 3140 7171 2e63  .r....z.111@qq.c
+00003280: 6f6d 7234 0000 0029 0c72 8600 0000 7232  omr4...).r....r2
+00003290: 0000 00da 0565 6d61 696c 7247 0000 00da  .....emailrG....
+000032a0: 0964 6f63 746f 725f 6964 72dd 0000 0072  .doctor_idr....r
+000032b0: f100 0000 5a0c 7573 6572 5f72 616e 6b5f  ....Z.user_rank_
+000032c0: 6964 72a8 0000 0072 3100 0000 da09 6964  idr....r1.....id
+000032d0: 6361 7264 6e75 6d72 8d00 0000 5a02 315f  cardnumr....Z.1_
+000032e0: da01 5f29 02da 0d73 7461 6e64 6172 645f  .._)...standard_
+000032f0: 636f 6465 72dd 0000 005a 0232 5f5a 0233  coder....Z.2_Z.3
+00003300: 5f5a 0234 5f75 6000 0000 e688 90e5 8a9f  _Z.4_u`.........
+00003310: efbc 81e4 bd86 e698 afe8 b4b9 e794 a8e6  ................
+00003320: a087 e587 86e6 9fa5 e8af a2e5 87ba e994  ................
+00003330: 99ef bc81 efbc 81ef bc81 e8af b7e6 898b  ................
+00003340: e58a a8e4 b8ba e8af a5e5 8cbb e794 9fe6  ................
+00003350: b7bb e58a a0e8 b4b9 e794 a8e6 a087 e587  ................
+00003360: 86ef bc81 efbc 81ef bc81 750f 0000 00e6  ..........u.....
+00003370: 8890 e58a 9fef bc81 efbc 81ef bc81 7235  ..............r5
+00003380: 0000 0072 8e00 0000 2925 722f 0000 0072  ...r....)%r/...r
+00003390: 4a00 0000 728f 0000 0072 8600 0000 7290  J...r....r....r.
+000033a0: 0000 0072 e100 0000 7292 0000 0072 9300  ...r....r....r..
+000033b0: 0000 7294 0000 0072 9500 0000 7296 0000  ..r....r....r...
+000033c0: 0072 9700 0000 7298 0000 0072 9900 0000  .r....r....r....
+000033d0: 729a 0000 0072 9b00 0000 7211 0000 0072  r....r....r....r
+000033e0: 3b00 0000 723c 0000 0072 3d00 0000 7248  ;...r<...r=...rH
+000033f0: 0000 0072 9e00 0000 7212 0000 0072 1400  ...r....r....r..
+00003400: 0000 7213 0000 0072 9c00 0000 724c 0000  ..r....r....rL..
+00003410: 0072 4d00 0000 729d 0000 0072 1500 0000  .rM...r....r....
+00003420: 7203 0000 00da 1367 6574 5f70 696e 7969  r......get_pinyi
+00003430: 6e5f 696e 6974 6961 6c73 721b 0000 00da  n_initialsr.....
+00003440: 0764 6f63 746f 7273 da03 6164 6472 6600  .doctors..addrf.
+00003450: 0000 7206 0000 0029 3172 4100 0000 7279  ..r....)1rA...ry
+00003460: 0000 0072 7a00 0000 729f 0000 0072 a000  ...rz...r....r..
+00003470: 0000 7235 0000 0072 9400 0000 72a1 0000  ..r5...r....r...
+00003480: 0072 a200 0000 72a3 0000 0072 9700 0000  .r....r....r....
+00003490: 7299 0000 0072 e500 0000 7286 0000 0072  r....r....r....r
+000034a0: a400 0000 728b 0000 0072 dd00 0000 72a5  ....r....r....r.
+000034b0: 0000 0072 e600 0000 72e3 0000 0072 f100  ...r....r....r..
+000034c0: 0000 72a8 0000 005a 0b67 656e 6465 725f  ..r....Z.gender_
+000034d0: 766c 7565 7231 0000 005a 0970 686f 6e65  vluer1...Z.phone
+000034e0: 5f69 6e74 72f4 0000 005a 0969 646e 756d  _intr....Z.idnum
+000034f0: 5f69 6e74 72e7 0000 005a 0864 6f63 5f72  _intr....Z.doc_r
+00003500: 616e 6b72 f200 0000 72e8 0000 0072 e900  ankr....r....r..
+00003510: 0000 5a07 6973 5f74 7275 65da 0664 6f63  ..Z.is_true..doc
+00003520: 746f 725a 0764 6f63 746f 7231 5a10 496e  torZ.doctor1Z.In
+00003530: 6974 6961 6c5f 686f 7370 6974 616c 5a10  itial_hospitalZ.
+00003540: 496e 6974 6961 6c5f 646f 635f 7261 6e6b  Initial_doc_rank
+00003550: 5a0f 636f 6d62 696e 6174 696f 6e5f 6864  Z.combination_hd
+00003560: 315a 0465 735f 315a 0f63 6f6d 6269 6e61  1Z.es_1Z.combina
+00003570: 7469 6f6e 5f68 6432 5a04 6573 5f32 5a0f  tion_hd2Z.es_2Z.
+00003580: 636f 6d62 696e 6174 696f 6e5f 6864 335a  combination_hd3Z
+00003590: 0465 735f 335a 0f63 6f6d 6269 6e61 7469  .es_3Z.combinati
+000035a0: 6f6e 5f68 6434 5a04 6573 5f34 5a07 6573  on_hd4Z.es_4Z.es
+000035b0: 5f6c 6973 74da 0265 7372 6c00 0000 7250  _list..esrl...rP
+000035c0: 0000 0072 4300 0000 7243 0000 0072 4400  ...rC...rC...rD.
+000035d0: 0000 da0d 696d 706f 7274 5f64 6f63 746f  ....import_docto
+000035e0: 729d 0100 0073 7601 0000 0003 0c01 0e01  r....sv.........
+000035f0: 1a02 0402 0a02 0401 1401 0801 0a01 0601  ................
+00003600: 1001 0a01 0402 0e01 0c01 1401 0801 0801  ................
+00003610: 0801 1201 0401 0803 0201 0201 0201 0201  ................
+00003620: 0201 0201 0201 0201 0201 02f6 060c 0a01  ................
+00003630: 0202 0801 0601 1401 0601 0803 0201 0201  ................
+00003640: 0201 0201 0201 0201 0201 0201 02f7 060b  ................
+00003650: 0a01 0201 0801 0601 0a01 0601 0a01 0602  ................
+00003660: 0401 0801 0601 0801 0801 0601 0801 0801  ................
+00003670: 0601 1401 0601 0803 0201 0201 0201 0201  ................
+00003680: 0201 0201 0201 0201 02f7 060b 0a01 0201  ................
+00003690: 0801 0801 0a01 0602 0401 0e01 0601 0a01  ................
+000036a0: 0201 0201 0201 0201 0401 0201 0201 0201  ................
+000036b0: 0201 0201 0801 02f4 0e0f 0a01 0201 0201  ................
+000036c0: 0201 0201 0401 0201 0201 0201 0201 0201  ................
+000036d0: 0801 02f4 0a0f 0a01 0201 0201 0201 0601  ................
+000036e0: 0401 0201 0201 0201 0201 0201 0203 02f2  ................
+000036f0: 0a10 0601 0801 0801 1001 0801 02ff 0a02  ................
+00003700: 1001 0801 02ff 0a02 1001 0801 02ff 0a02  ................
+00003710: 1001 0801 02ff 0a02 1801 0401 0a01 0a01  ................
+00003720: 0a01 0a01 0801 1203 0201 0201 0201 0201  ................
+00003730: 0201 0201 0801 0201 02f7 060b 0a01 0202  ................
+00003740: 0201 0201 0201 0201 0201 0201 0801 0201  ................
+00003750: 02f7 060b 1201 1001 1a02 0601 0a02 0801  ................
+00003760: 7200 0100 0063 0100 0000 0000 0000 0000  r....c..........
+00003770: 0000 0200 0000 0400 0000 4300 0000 7316  ..........C...s.
+00003780: 0000 0074 006a 017c 0064 0164 028d 02a0  ...t.j.|.d.d....
+00003790: 02a1 007d 017c 0153 0029 034e 727b 0000  ...}.|.S.).Nr{..
+000037a0: 0029 01da 0964 656c 696d 6974 6572 2903  .)...delimiter).
+000037b0: da06 7069 6e79 696e da0b 6765 745f 696e  ..pinyin..get_in
+000037c0: 6974 6961 6cda 0575 7070 6572 2902 7286  itial..upper).r.
+000037d0: 0000 005a 0a73 616d 706c 656e 616d 6572  ...Z.samplenamer
+000037e0: 4300 0000 7243 0000 0072 4400 0000 72fb  C...rC...rD...r.
+000037f0: 0000 0070 0200 0073 0400 0000 0001 1201  ...p...s........
+00003800: 72fb 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00003810: 0000 0000 0000 0400 0000 4000 0000 7320  ..........@...s 
+00003820: 0100 0065 005a 0164 005a 0265 036a 0464  ...e.Z.d.Z.e.j.d
+00003830: 0164 0264 038d 025a 0565 036a 0464 0464  .d.d...Z.e.j.d.d
+00003840: 0264 038d 025a 0665 036a 0464 0564 0264  .d...Z.e.j.d.d.d
+00003850: 038d 025a 0765 036a 0464 0664 0264 038d  ...Z.e.j.d.d.d..
+00003860: 025a 0865 036a 0464 0764 0264 038d 025a  .Z.e.j.d.d.d...Z
+00003870: 0965 036a 0464 0864 0264 038d 025a 0a65  .e.j.d.d.d...Z.e
+00003880: 036a 0464 0964 0264 038d 025a 0b65 036a  .j.d.d.d...Z.e.j
+00003890: 0464 0a64 0264 038d 025a 0c65 036a 0464  .d.d.d...Z.e.j.d
+000038a0: 0b64 0264 038d 025a 0d65 036a 0464 0c64  .d.d...Z.e.j.d.d
+000038b0: 0264 038d 025a 0e65 036a 0464 0d64 0264  .d...Z.e.j.d.d.d
+000038c0: 038d 025a 0f65 036a 0464 0e64 0264 038d  ...Z.e.j.d.d.d..
+000038d0: 025a 1065 036a 1164 0f64 108d 015a 1265  .Z.e.j.d.d...Z.e
+000038e0: 036a 0464 1164 0264 038d 025a 1365 036a  .j.d.d.d...Z.e.j
+000038f0: 0464 1264 0264 038d 025a 1465 036a 0464  .d.d.d...Z.e.j.d
+00003900: 1364 0264 038d 025a 1565 036a 0464 1464  .d.d...Z.e.j.d.d
+00003910: 0264 038d 025a 1665 036a 0464 1564 0264  .d...Z.e.j.d.d.d
+00003920: 038d 025a 1765 036a 1164 1664 108d 015a  ...Z.e.j.d.d...Z
+00003930: 1847 0064 1764 1884 0064 1883 025a 1964  .G.d.d...d...Z.d
+00003940: 1953 0029 1ada 1344 7275 6744 6972 6563  .S.)...DrugDirec
+00003950: 746f 7279 4669 6c74 6572 da09 6472 7567  toryFilter..drug
+00003960: 5f63 6f64 6572 ab00 0000 72ac 0000 00da  _coder....r.....
+00003970: 0964 7275 675f 6e61 6d65 da09 7374 616e  .drug_name..stan
+00003980: 6461 7264 73da 0c6d 6561 7375 7265 5f75  dards..measure_u
+00003990: 6e69 745a 1670 7265 7061 7261 7469 6f6e  nitZ.preparation
+000039a0: 5f74 7970 655f 5f6e 616d 655a 0e63 6174  _type__nameZ.cat
+000039b0: 6567 6f72 795f 5f6e 616d 655a 0f64 7275  egory__nameZ.dru
+000039c0: 675f 7479 7065 5f5f 6e61 6d65 da09 756e  g_type__name..un
+000039d0: 6974 5f64 6f73 65da 0a73 746f 636b 5f6c  it_dose..stock_l
+000039e0: 6566 74da 0a73 746f 636b 5f75 6e69 74da  eft..stock_unit.
+000039f0: 036d 6963 da0c 7263 635f 6361 7465 676f  .mic..rcc_catego
+00003a00: 7279 da0c 6973 5f65 7373 656e 7469 616c  ry..is_essential
+00003a10: 72a9 0000 00da 0868 725f 6c65 7665 6cda  r......hr_level.
+00003a20: 0767 625f 636f 6465 da07 6762 5f6e 616d  .gb_code..gb_nam
+00003a30: 65da 0c6f 7269 6769 6e5f 706c 6163 65da  e..origin_place.
+00003a40: 0c6d 616e 7566 6163 7475 7265 7272 3e00  .manufacturerr>.
+00003a50: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00003a60: 0000 0001 0000 0040 0000 0073 1400 0000  .......@...s....
+00003a70: 6500 5a01 6400 5a02 6503 5a04 6401 5a05  e.Z.d.Z.e.Z.d.Z.
+00003a80: 6402 5300 2903 7a18 4472 7567 4469 7265  d.S.).z.DrugDire
+00003a90: 6374 6f72 7946 696c 7465 722e 4d65 7461  ctoryFilter.Meta
+00003aa0: 72af 0000 004e 2906 725b 0000 0072 5c00  r....N).r[...r\.
+00003ab0: 0000 725d 0000 0072 1900 0000 72b0 0000  ..r]...r....r...
+00003ac0: 0072 b100 0000 7243 0000 0072 4300 0000  .r....rC...rC...
+00003ad0: 7243 0000 0072 4400 0000 72b2 0000 0091  rC...rD...r.....
+00003ae0: 0200 0073 0400 0000 0801 0401 72b2 0000  ...s........r...
+00003af0: 004e 291a 725b 0000 0072 5c00 0000 725d  .N).r[...r\...r]
+00003b00: 0000 0072 b300 0000 72b5 0000 0072 0601  ...r....r....r..
+00003b10: 0000 7207 0100 005a 0d73 7065 6369 6669  ..r....Z.specifi
+00003b20: 6361 7469 6f6e 7209 0100 00da 1070 7265  cationr......pre
+00003b30: 7061 7261 7469 6f6e 5f74 7970 65da 0863  paration_type..c
+00003b40: 6174 6567 6f72 79da 0964 7275 675f 7479  ategory..drug_ty
+00003b50: 7065 720a 0100 0072 0b01 0000 720c 0100  per....r....r...
+00003b60: 0072 0d01 0000 720e 0100 00da 0d42 6f6f  .r....r......Boo
+00003b70: 6c65 616e 4669 6c74 6572 720f 0100 0072  leanFilterr....r
+00003b80: 1001 0000 7211 0100 0072 1201 0000 7213  ....r....r....r.
+00003b90: 0100 0072 1401 0000 723e 0000 0072 b200  ...r....r>...r..
+00003ba0: 0000 7243 0000 0072 4300 0000 7243 0000  ..rC...rC...rC..
+00003bb0: 0072 4400 0000 7205 0100 007c 0200 0073  .rD...r....|...s
+00003bc0: 2800 0000 0801 0e01 0e01 0e01 0e01 0e01  (...............
+00003bd0: 0e01 0e01 0e01 0e01 0e01 0e01 0e01 0c01  ................
+00003be0: 0e01 0e01 0e01 0e01 0e01 0c02 7205 0100  ............r...
+00003bf0: 0063 0100 0000 0000 0000 0000 0000 0300  .c..............
+00003c00: 0000 0300 0000 4300 0000 7320 0000 0064  ......C...s ...d
+00003c10: 017d 017c 0144 005d 127d 027c 027c 0076  .}.|.D.].}.|.|.v
+00003c20: 0072 0801 0064 0253 0071 0864 0353 0029  .r...d.S.q.d.S.)
+00003c30: 044e 751d 0000 007e 2140 2324 255e 262a  .Nu....~!@#$%^&*
+00003c40: 2829 2b2d 2a2f 3c3e 2c2e 5b5d 5c2f 7c27  ()+-*/<>,.[]\/|'
+00003c50: 60e3 8081 5446 7243 0000 0029 03da 076b  `...TFrC...)...k
+00003c60: 6579 776f 7264 da07 7379 6d62 6f6c 73da  eyword..symbols.
+00003c70: 0673 796d 626f 6c72 4300 0000 7243 0000  .symbolrC...rC..
+00003c80: 0072 4400 0000 da11 6966 5f63 6f6e 7461  .rD.....if_conta
+00003c90: 696e 5f73 796d 626f 6c96 0200 0073 0a00  in_symbol....s..
+00003ca0: 0000 0001 0401 0801 0801 0802 721c 0100  ............r...
+00003cb0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00003cc0: 0000 0300 0000 4000 0000 732c 0000 0065  ......@...s,...e
+00003cd0: 005a 0164 005a 0265 036a 04a0 05a1 00a0  .Z.d.Z.e.j......
+00003ce0: 0664 01a1 015a 0765 085a 0965 0a5a 0b64  .d...Z.e.Z.e.Z.d
+00003cf0: 0264 0384 005a 0c64 0453 0029 05da 1444  .d...Z.d.S.)...D
+00003d00: 7275 6744 6972 6563 746f 7279 5669 6577  rugDirectoryView
+00003d10: 5365 7472 b700 0000 6302 0000 0000 0000  Setr....c.......
+00003d20: 0000 0000 0012 0000 0007 0000 004f 0000  .............O..
+00003d30: 0073 2801 0000 7c00 6a00 6a01 a002 6401  .s(...|.j.j...d.
+00003d40: a101 7d04 7c00 6a00 6a01 a002 6402 a101  ..}.|.j.j...d...
+00003d50: 7d05 7c00 6a00 6a01 a002 6403 a101 7d06  }.|.j.j...d...}.
+00003d60: 7c00 6a00 6a01 a002 6404 a101 7d07 7403  |.j.j...d...}.t.
+00003d70: 7c05 8301 7d08 7c08 7250 7404 6405 6406  |...}.|.rPt.d.d.
+00003d80: 6407 8d02 5300 6408 7d09 7c09 72d0 7c04  d...S.d.}.|.r.|.
+00003d90: 6409 640a 7c05 7c06 7c07 640b 9c06 7d0a  d.d.|.|.|.d...}.
+00003da0: 7405 8300 7d0b 7c0b a006 7c0a 640c a102  t...}.|...|.d...
+00003db0: 7d0c 7c0c 640d 1900 640e 6b02 72be 7407  }.|.d...d.k.r.t.
+00003dc0: 640f 8301 0100 7c0c 6410 1900 6411 1900  d.....|.d...d...
+00003dd0: 7d0d 7c0c 6410 1900 6412 1900 7d0e 7c0e  }.|.d...d...}.|.
+00003de0: 6413 1900 7c0d 6414 9c02 7d0f 7404 7c0f  d...|.d...}.t.|.
+00003df0: 8301 5300 7407 6415 8301 0100 7404 7c0c  ..S.t.d.....t.|.
+00003e00: 8301 5300 6e54 7c00 a008 7c00 a009 a100  ..S.nT|...|.....
+00003e10: a101 7d10 7c00 a00a 7c10 a101 7d06 7c06  ..}.|...|...}.|.
+00003e20: 6400 7501 9001 720c 7c00 6a0b 7c06 6416  d.u...r.|.j.|.d.
+00003e30: 6417 8d02 7d11 7c00 a00c 7c11 6a0d a101  d...}.|...|.j...
+00003e40: 5300 7c00 6a0b 7c10 6416 6417 8d02 7d11  S.|.j.|.d.d...}.
+00003e50: 7404 7c11 6a0d 8301 5300 6400 5300 2918  t.|.j...S.d.S.).
+00003e60: 4e72 ce00 0000 7207 0100 00da 0470 6167  Nr....r......pag
+00003e70: 65da 0970 6167 655f 7369 7a65 750f 0000  e..page_sizeu...
+00003e80: 00e5 8f82 e695 b0e9 9499 e8af afef bc81  ................
+00003e90: 6990 0100 0072 be00 0000 727d 0000 00da  i....r....r}....
+00003ea0: 044e 616d 65da 0230 3329 0672 ce00 0000  .Name..03).r....
+00003eb0: 5a0a 436f 6465 5f66 6965 6c64 5a09 436f  Z.Code_fieldZ.Co
+00003ec0: 6465 5f6f 7065 725a 0b56 616c 7565 5f66  de_operZ.Value_f
+00003ed0: 6965 6c64 5a09 5061 6765 696e 6465 785a  ieldZ.PageindexZ
+00003ee0: 0850 6167 6573 697a 655a 0659 5044 4143  .PagesizeZ.YPDAC
+00003ef0: 58da 0463 6f64 65e9 c800 0000 7512 0000  X..code.....u...
+00003f00: 00e8 8daf e593 81e6 9fa5 e8af a2e6 8890  ................
+00003f10: e58a 9fda 0763 6f6e 7465 6e74 7235 0000  .....contentr5..
+00003f20: 005a 0870 6167 6569 6e66 6f5a 0c72 6563  .Z.pageinfoZ.rec
+00003f30: 6f72 6473 636f 756e 7429 02da 0563 6f75  ordscount)...cou
+00003f40: 6e74 da07 7265 7375 6c74 7375 1200 0000  nt..resultsu....
+00003f50: e88d afe5 9381 e69f a5e8 afa2 e5a4 b1e8  ................
+00003f60: b4a5 5429 01da 046d 616e 7929 0e72 4100  ..T)...many).rA.
+00003f70: 0000 da0c 7175 6572 795f 7061 7261 6d73  ....query_params
+00003f80: 724a 0000 0072 1c01 0000 720e 0000 0072  rJ...r....r....r
+00003f90: 1c00 0000 da09 7772 6974 6562 6163 6b72  ......writebackr
+00003fa0: 4900 0000 da0f 6669 6c74 6572 5f71 7565  I.....filter_que
+00003fb0: 7279 7365 7472 5a00 0000 da11 7061 6769  rysetrZ.....pagi
+00003fc0: 6e61 7465 5f71 7565 7279 7365 74da 0e67  nate_queryset..g
+00003fd0: 6574 5f73 6572 6961 6c69 7a65 72da 1667  et_serializer..g
+00003fe0: 6574 5f70 6167 696e 6174 6564 5f72 6573  et_paginated_res
+00003ff0: 706f 6e73 6572 3500 0000 2912 7253 0000  ponser5...).rS..
+00004000: 0072 4100 0000 da04 6172 6773 7268 0000  .rA.....argsrh..
+00004010: 0072 ce00 0000 7207 0100 0072 1e01 0000  .r....r....r....
+00004020: 721f 0100 0072 1b01 0000 da04 666c 6167  r....r......flag
+00004030: da07 696e 5f64 6174 615a 0861 7069 5f69  ..in_dataZ.api_i
+00004040: 6e66 6fda 0472 6573 745a 0972 6573 745f  nfo..restZ.rest_
+00004050: 6461 7461 5a09 7061 6765 5f69 6e66 6f5a  dataZ.page_infoZ
+00004060: 0972 6573 745f 6469 6374 72c4 0000 0072  .rest_dictr....r
+00004070: c200 0000 7243 0000 0072 4300 0000 7244  ....rC...rC...rD
+00004080: 0000 00da 046c 6973 74a4 0200 0073 4200  .....list....sB.
+00004090: 0000 0001 0e01 0e01 0e01 0e01 0801 0401  ................
+000040a0: 0c01 0401 0402 0201 0201 0201 0201 0201  ................
+000040b0: 02fa 0608 0601 0c01 0c01 0801 0c01 0c01  ................
+000040c0: 0e01 0802 0801 0a02 0e02 0a01 0a01 0e01  ................
+000040d0: 0c02 0e01 7a19 4472 7567 4469 7265 6374  ....z.DrugDirect
+000040e0: 6f72 7956 6965 7753 6574 2e6c 6973 744e  oryViewSet.listN
+000040f0: 290d 725b 0000 0072 5c00 0000 725d 0000  ).r[...r\...r]..
+00004100: 0072 1900 0000 723b 0000 0072 5600 0000  .r....r;...rV...
+00004110: 72c3 0000 0072 c400 0000 7228 0000 0072  r....r....r(...r
+00004120: 5f00 0000 7205 0100 0072 c500 0000 7232  _...r....r....r2
+00004130: 0100 0072 4300 0000 7243 0000 0072 4300  ...rC...rC...rC.
+00004140: 0000 7244 0000 0072 1d01 0000 9f02 0000  ..rD...r........
+00004150: 7308 0000 0008 0110 0104 0104 0272 1d01  s............r..
+00004160: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00004170: 0000 0003 0000 0040 0000 0073 2000 0000  .......@...s ...
+00004180: 6500 5a01 6400 5a02 6503 6a04 a005 a100  e.Z.d.Z.e.j.....
+00004190: a006 6401 a101 5a07 6508 5a09 6402 5300  ..d...Z.e.Z.d.S.
+000041a0: 2903 da0e 4170 6949 6e66 6f56 6965 7753  )...ApiInfoViewS
+000041b0: 6574 72b7 0000 004e 290a 725b 0000 0072  etr....N).r[...r
+000041c0: 5c00 0000 725d 0000 0072 1c00 0000 723b  \...r]...r....r;
+000041d0: 0000 0072 5600 0000 72c3 0000 0072 c400  ...rV...r....r..
+000041e0: 0000 7229 0000 0072 5f00 0000 7243 0000  ..r)...r_...rC..
+000041f0: 0072 4300 0000 7243 0000 0072 4400 0000  .rC...rC...rD...
+00004200: 7233 0100 00cd 0200 0073 0400 0000 0801  r3.......s......
+00004210: 1001 7233 0100 0063 0100 0000 0000 0000  ..r3...c........
+00004220: 0000 0000 1c00 0000 0e00 0000 4300 0000  ............C...
+00004230: 73f0 0100 007c 006a 00a0 0164 01a1 017d  s....|.j...d...}
+00004240: 017c 006a 02a0 0164 0264 03a1 027d 027c  .|.j...d.d...}.|
+00004250: 026a 03a0 0464 04a1 0164 0519 00a0 0464  .j...d...d.....d
+00004260: 06a1 0164 0719 007d 0367 007d 047c 0364  ...d...}.g.}.|.d
+00004270: 0876 0090 0172 d090 017a 6074 056a 0664  .v...r...z`t.j.d
+00004280: 097c 02a0 07a1 0064 0a64 0b8d 037d 057c  .|.....d.d...}.|
+00004290: 05a0 08a1 007d 067c 0644 0090 015d 387d  .....}.|.D...]8}
+000042a0: 077c 076a 097d 0874 0a64 0c7c 0883 0244  .|.j.}.t.d.|...D
+000042b0: 0090 015d 207d 097c 07a0 0b7c 09a1 017d  ...] }.|...|...}
+000042c0: 0a7c 0a72 7c7c 07a0 0c7c 0964 07a1 026a  .|.r||...|.d...j
+000042d0: 0d7d 0b74 0e7c 07a0 0f7c 0964 07a1 0283  .}.t.|...|.d....
+000042e0: 017d 0c7c 0a64 0519 007d 0d7c 0a64 0c19  .}.|.d...}.|.d..
+000042f0: 007d 0e74 106a 116a 127c 0e64 0d8d 01a0  .}.t.j.j.|.d....
+00004300: 13a1 007d 0f7c 0f6a 147d 107c 0a64 0e19  ...}.|.j.}.|.d..
+00004310: 007d 1174 156a 116a 127c 0f6a 167c 1164  .}.t.j.j.|.j.|.d
+00004320: 0f8d 02a0 13a1 007d 127c 126a 147d 137c  .......}.|.j.}.|
+00004330: 0a64 1019 007d 1474 0e7c 0a64 1119 0083  .d...}.t.|.d....
+00004340: 017d 157c 0a64 1219 007d 167c 0a64 1319  .}.|.d...}.|.d..
+00004350: 007d 1774 176a 116a 127c 0c64 148d 01a0  .}.t.j.j.|.d....
+00004360: 13a1 007d 187c 1890 0172 5a7c 186a 1866  ...}.|...rZ|.j.f
+00004370: 0069 007c 0c7c 0d7c 107c 137c 147c 157c  .i.|.|.|.|.|.|.|
+00004380: 167c 1764 159c 08a4 018e 0101 006e 2474  .|.d.........n$t
+00004390: 176a 116a 1966 0069 007c 0c7c 0d7c 107c  .j.j.f.i.|.|.|.|
+000043a0: 137c 147c 157c 167c 1764 159c 08a4 018e  .|.|.|.|.d......
+000043b0: 0101 007c 0c7c 0d7c 0e7c 117c 147c 157c  ...|.|.|.|.|.|.|
+000043c0: 167c 1764 169c 087d 197c 04a0 1a7c 19a1  .|.d...}.|...|..
+000043d0: 0101 0071 7c71 6657 006e 2a04 0074 1b90  ...q|qfW.n*..t..
+000043e0: 0179 ce01 007d 1a01 007a 107c 1a82 0157  .y...}...z.|...W
+000043f0: 0059 0064 097d 1a7e 1a6e 0a64 097d 1a7e  .Y.d.}.~.n.d.}.~
+00004400: 1a30 0030 007c 0490 0172 e064 177c 0469  .0.0.|...r.d.|.i
+00004410: 017d 1b6e 0864 1764 1869 017d 1b74 1c7c  .}.n.d.d.i.}.t.|
+00004420: 1b83 0153 0029 1975 2000 0000 e5af bce5  ...S.).u .......
+00004430: 85a5 e6a3 80e6 9fa5 e5ad 97e5 85b8 6578  ..............ex
+00004440: 6365 6ce8 a1a8 e695 b0e6 8dae 7279 0000  cel.........ry..
+00004450: 0072 7a00 0000 727b 0000 0072 7c00 0000  .rz...r{...r|...
+00004460: 727d 0000 0072 7e00 0000 7201 0000 0072  r}...r~...r....r
+00004470: 7f00 0000 4e54 7281 0000 0072 8400 0000  ....NTr....r....
+00004480: 7285 0000 0072 8700 0000 a902 72dd 0000  r....r......r...
+00004490: 0072 8600 0000 7288 0000 0072 db00 0000  .r....r....r....
+000044a0: 72dc 0000 0072 ed00 0000 a901 72cc 0000  r....r......r...
+000044b0: 00a9 0872 cc00 0000 72cd 0000 0072 ce00  ...r....r....r..
+000044c0: 0000 72cf 0000 00da 0c70 726f 6a65 6374  ..r......project
+000044d0: 5f66 6565 73da 0a63 6f64 655f 7372 7674  _fees..code_srvt
+000044e0: 70da 0a6e 616d 655f 7372 7674 70da 0772  p..name_srvtp..r
+000044f0: 656d 6172 6b73 a908 72cc 0000 0072 cd00  emarks..r....r..
+00004500: 0000 72a4 0000 0072 e600 0000 7237 0100  ..r....r....r7..
+00004510: 0072 3801 0000 7239 0100 0072 3a01 0000  .r8...r9...r:...
+00004520: 7235 0000 0072 8e00 0000 291d 722f 0000  r5...r....).r/..
+00004530: 0072 4a00 0000 728f 0000 0072 8600 0000  .rJ...r....r....
+00004540: 7290 0000 0072 e100 0000 7292 0000 0072  r....r....r....r
+00004550: 9300 0000 7294 0000 0072 9500 0000 7296  ....r....r....r.
+00004560: 0000 0072 9700 0000 7298 0000 0072 9900  ...r....r....r..
+00004570: 0000 729b 0000 0072 9a00 0000 7211 0000  ..r....r....r...
+00004580: 0072 3b00 0000 723c 0000 0072 3d00 0000  .r;...r<...r=...
+00004590: 728a 0000 0072 1200 0000 7248 0000 0072  r....r....rH...r
+000045a0: 1700 0000 729c 0000 0072 9d00 0000 729e  ....r....r....r.
+000045b0: 0000 0072 6600 0000 7206 0000 0029 1c72  ...rf...r....).r
+000045c0: 4100 0000 7279 0000 0072 7a00 0000 729f  A...ry...rz...r.
+000045d0: 0000 0072 a000 0000 7235 0000 0072 9400  ...r....r5...r..
+000045e0: 0000 72a1 0000 0072 a200 0000 72a3 0000  ..r....r....r...
+000045f0: 0072 9700 0000 7299 0000 0072 cc00 0000  .r....r....r....
+00004600: 72cd 0000 0072 a400 0000 728b 0000 0072  r....r....r....r
+00004610: ce00 0000 72e6 0000 0072 e300 0000 72cf  ....r....r....r.
+00004620: 0000 0072 3701 0000 7238 0100 0072 3901  ...r7...r8...r9.
+00004630: 0000 723a 0100 005a 1069 6e73 5f64 6963  ..r:...Z.ins_dic
+00004640: 7469 6f6e 6172 6965 7372 a500 0000 726c  tionariesr....rl
+00004650: 0000 0072 5000 0000 7243 0000 0072 4300  ...rP...rC...rC.
+00004660: 0000 7244 0000 00da 1e69 6d70 6f72 745f  ..rD.....import_
+00004670: 696e 7370 6563 7469 6f6e 5f64 6963 7469  inspection_dicti
+00004680: 6f6e 6172 6965 73d2 0200 0073 7c00 0000  onaries....s|...
+00004690: 0003 0c01 0e01 1a02 0402 0a02 0401 1401  ................
+000046a0: 0801 0a01 0601 1001 0a01 0402 0e01 1001  ................
+000046b0: 0801 0801 1201 0602 0801 1601 0601 0801  ................
+000046c0: 0c01 0801 0801 1201 0601 0a01 0201 0201  ................
+000046d0: 0201 0201 0201 0201 02f9 0c0a 0c01 0201  ................
+000046e0: 0201 0201 0201 0201 0201 02f9 0a0a 0201  ................
+000046f0: 0201 0201 0201 0201 0201 0201 02f8 060a  ................
+00004700: 1201 1001 1a02 0601 0a02 0801 723c 0100  ............r<..
+00004710: 0063 0100 0000 0000 0000 0000 0000 1c00  .c..............
+00004720: 0000 0e00 0000 4300 0000 73f0 0100 007c  ......C...s....|
+00004730: 006a 00a0 0164 01a1 017d 017c 006a 02a0  .j...d...}.|.j..
+00004740: 0164 0264 03a1 027d 027c 026a 03a0 0464  .d.d...}.|.j...d
+00004750: 04a1 0164 0519 00a0 0464 06a1 0164 0719  ...d.....d...d..
+00004760: 007d 0367 007d 047c 0364 0876 0090 0172  .}.g.}.|.d.v...r
+00004770: d090 017a 6074 056a 0664 097c 02a0 07a1  ...z`t.j.d.|....
+00004780: 0064 0a64 0b8d 037d 057c 05a0 08a1 007d  .d.d...}.|.....}
+00004790: 067c 0644 0090 015d 387d 077c 076a 097d  .|.D...]8}.|.j.}
+000047a0: 0874 0a64 0c7c 0883 0244 0090 015d 207d  .t.d.|...D...] }
+000047b0: 097c 07a0 0b7c 09a1 017d 0a7c 0a72 7c7c  .|...|...}.|.r||
+000047c0: 07a0 0c7c 0964 07a1 026a 0d7d 0b74 0e7c  ...|.d...j.}.t.|
+000047d0: 07a0 0f7c 0964 07a1 0283 017d 0c7c 0a64  ...|.d.....}.|.d
+000047e0: 0519 007d 0d7c 0a64 0c19 007d 0e74 106a  ...}.|.d...}.t.j
+000047f0: 116a 127c 0e64 0d8d 01a0 13a1 007d 0f7c  .j.|.d.......}.|
+00004800: 0f6a 147d 107c 0a64 0e19 007d 1174 156a  .j.}.|.d...}.t.j
+00004810: 116a 127c 0f6a 167c 1164 0f8d 02a0 13a1  .j.|.j.|.d......
+00004820: 007d 127c 126a 147d 137c 0a64 1019 007d  .}.|.j.}.|.d...}
+00004830: 1474 0e7c 0a64 1119 0083 017d 157c 0a64  .t.|.d.....}.|.d
+00004840: 1219 007d 167c 0a64 1319 007d 1774 176a  ...}.|.d...}.t.j
+00004850: 116a 127c 0c64 148d 01a0 13a1 007d 187c  .j.|.d.......}.|
+00004860: 1890 0172 5a7c 186a 1866 0069 007c 0c7c  ...rZ|.j.f.i.|.|
+00004870: 0d7c 107c 137c 147c 157c 167c 1764 159c  .|.|.|.|.|.|.d..
+00004880: 08a4 018e 0101 006e 2474 176a 116a 1966  .......n$t.j.j.f
+00004890: 0069 007c 0c7c 0d7c 107c 137c 147c 157c  .i.|.|.|.|.|.|.|
+000048a0: 167c 1764 159c 08a4 018e 0101 007c 0c7c  .|.d.........|.|
+000048b0: 0d7c 0e7c 117c 147c 157c 167c 1764 169c  .|.|.|.|.|.|.d..
+000048c0: 087d 197c 04a0 1a7c 19a1 0101 0071 7c71  .}.|...|.....q|q
+000048d0: 6657 006e 2a04 0074 1b90 0179 ce01 007d  fW.n*..t...y...}
+000048e0: 1a01 007a 107c 1a82 0157 0059 0064 097d  ...z.|...W.Y.d.}
+000048f0: 1a7e 1a6e 0a64 097d 1a7e 1a30 0030 007c  .~.n.d.}.~.0.0.|
+00004900: 0490 0172 e064 177c 0469 017d 1b6e 0864  ...r.d.|.i.}.n.d
+00004910: 1764 1869 017d 1b74 1c7c 1b83 0153 0029  .d.i.}.t.|...S.)
+00004920: 1975 2000 0000 e5af bce5 85a5 e6a3 80e9  .u .............
+00004930: aa8c e5ad 97e5 85b8 6578 6365 6ce8 a1a8  ........excel...
+00004940: e695 b0e6 8dae 7279 0000 0072 7a00 0000  ......ry...rz...
+00004950: 727b 0000 0072 7c00 0000 727d 0000 0072  r{...r|...r}...r
+00004960: 7e00 0000 7201 0000 0072 7f00 0000 4e54  ~...r....r....NT
+00004970: 7281 0000 0072 8400 0000 7285 0000 0072  r....r....r....r
+00004980: 8700 0000 7234 0100 0072 8800 0000 72db  ....r4...r....r.
+00004990: 0000 0072 dc00 0000 72ed 0000 0072 3501  ...r....r....r5.
+000049a0: 0000 7236 0100 0072 3b01 0000 7235 0000  ..r6...r;...r5..
+000049b0: 0072 8e00 0000 291d 722f 0000 0072 4a00  .r....).r/...rJ.
+000049c0: 0000 728f 0000 0072 8600 0000 7290 0000  ..r....r....r...
+000049d0: 0072 e100 0000 7292 0000 0072 9300 0000  .r....r....r....
+000049e0: 7294 0000 0072 9500 0000 7296 0000 0072  r....r....r....r
+000049f0: 9700 0000 7298 0000 0072 9900 0000 729b  ....r....r....r.
+00004a00: 0000 0072 9a00 0000 7211 0000 0072 3b00  ...r....r....r;.
+00004a10: 0000 723c 0000 0072 3d00 0000 728a 0000  ..r<...r=...r...
+00004a20: 0072 1200 0000 7248 0000 0072 1800 0000  .r....rH...r....
+00004a30: 729c 0000 0072 9d00 0000 729e 0000 0072  r....r....r....r
+00004a40: 6600 0000 7206 0000 0029 1c72 4100 0000  f...r....).rA...
+00004a50: 7279 0000 0072 7a00 0000 729f 0000 0072  ry...rz...r....r
+00004a60: a000 0000 7235 0000 0072 9400 0000 72a1  ....r5...r....r.
+00004a70: 0000 0072 a200 0000 72a3 0000 0072 9700  ...r....r....r..
+00004a80: 0000 7299 0000 0072 cc00 0000 72cd 0000  ..r....r....r...
+00004a90: 0072 a400 0000 728b 0000 0072 ce00 0000  .r....r....r....
+00004aa0: 72e6 0000 0072 e300 0000 72cf 0000 0072  r....r....r....r
+00004ab0: 3701 0000 7238 0100 0072 3901 0000 723a  7...r8...r9...r:
+00004ac0: 0100 005a 1065 7861 5f64 6963 7469 6f6e  ...Z.exa_diction
+00004ad0: 6172 6965 7372 a500 0000 726c 0000 0072  ariesr....rl...r
+00004ae0: 5000 0000 7243 0000 0072 4300 0000 7244  P...rC...rC...rD
+00004af0: 0000 00da 1f69 6d70 6f72 745f 6578 616d  .....import_exam
+00004b00: 696e 6174 696f 6e5f 6469 6374 696f 6e61  ination_dictiona
+00004b10: 7269 6573 1e03 0000 737c 0000 0000 030c  ries....s|......
+00004b20: 010e 011a 0204 020a 0204 0114 0108 010a  ................
+00004b30: 0106 0110 010a 0104 020e 0110 0108 0108  ................
+00004b40: 0112 0106 0208 0116 0106 0108 010c 0108  ................
+00004b50: 0108 0112 0106 010a 0102 0102 0102 0102  ................
+00004b60: 0102 0102 0102 f90c 0a0c 0102 0102 0102  ................
+00004b70: 0102 0102 0102 0102 f90a 0a02 0102 0102  ................
+00004b80: 0102 0102 0102 0102 0102 f806 0a12 0110  ................
+00004b90: 011a 0206 010a 0208 0172 3d01 0000 6301  .........r=...c.
+00004ba0: 0000 0000 0000 0000 0000 0027 0000 0019  ...........'....
+00004bb0: 0000 0043 0000 0073 9e02 0000 7c00 6a00  ...C...s....|.j.
+00004bc0: a001 6401 a101 7d01 7c00 6a02 a001 6402  ..d...}.|.j...d.
+00004bd0: 6403 a102 7d02 7c02 6a03 a004 6404 a101  d...}.|.j...d...
+00004be0: 6405 1900 a004 6406 a101 6407 1900 7d03  d.....d...d...}.
+00004bf0: 6700 7d04 7c03 6408 7600 9002 727e 9002  g.}.|.d.v...r~..
+00004c00: 7a0e 7405 6a06 6409 7c02 a007 a100 640a  z.t.j.d.|.....d.
+00004c10: 640b 8d03 7d05 7c05 a008 a100 7d06 7c06  d...}.|.....}.|.
+00004c20: 4400 9001 5de6 7d07 7c07 6a09 7d08 740a  D...].}.|.j.}.t.
+00004c30: 640c 7c08 8302 4400 9001 5dce 7d09 7c07  d.|...D...].}.|.
+00004c40: a00b 7c09 a101 7d0a 7c0a 727c 7c07 a00c  ..|...}.|.r||...
+00004c50: 7c09 6407 a102 6a0d 7d0b 740e 7c07 a00f  |.d...j.}.t.|...
+00004c60: 7c09 6407 a102 8301 7d0c 7c0a 6405 1900  |.d.....}.|.d...
+00004c70: 7d0d 7c0a 640c 1900 7d0e 7c0a 640d 1900  }.|.d...}.|.d...
+00004c80: 7d0f 7c0a 640e 1900 7d10 7410 6a11 6a12  }.|.d...}.t.j.j.
+00004c90: 7c10 640f 8d01 a013 a100 7d11 7c0a 6410  |.d.......}.|.d.
+00004ca0: 1900 7d12 7414 6a11 6a12 7c12 6411 8d01  ..}.t.j.j.|.d...
+00004cb0: a013 a100 7d13 7c0a 6412 1900 7d14 7415  ....}.|.d...}.t.
+00004cc0: 6a11 6a12 7c14 6413 8d01 a013 a100 7d15  j.j.|.d.......}.
+00004cd0: 7c0a 6414 1900 7d16 7c0a 6415 1900 7d17  |.d...}.|.d...}.
+00004ce0: 7c0a 6416 1900 7d18 7c0a 6417 1900 7d19  |.d...}.|.d...}.
+00004cf0: 7c0a 6418 1900 7d1a 7c0a 6419 1900 7d1b  |.d...}.|.d...}.
+00004d00: 7c0a 641a 1900 7d1c 7c0a 641b 1900 7d1d  |.d...}.|.d...}.
+00004d10: 7c0a 641c 1900 7d1e 7c1e 641d 6b02 9001  |.d...}.|.d.k...
+00004d20: 726c 640a 7d1f 6e04 641e 7d1f 7c0a 641f  rld.}.n.d.}.|.d.
+00004d30: 1900 7d20 7c0a 6420 1900 7d21 7c0a 6421  ..} |.d ..}!|.d!
+00004d40: 1900 7d22 7416 6a11 6a12 7c0c 6422 8d01  ..}"t.j.j.|.d"..
+00004d50: 7d23 7c23 9001 72dc 7c23 6a17 6600 6900  }#|#..r.|#j.f.i.
+00004d60: 7c0c 7c0d 7c0e 7c0f 7c11 6a18 7c13 6a18  |.|.|.|.|.j.|.j.
+00004d70: 7c15 6a18 7c16 7c17 7c18 7c19 7c1a 7c1b  |.j.|.|.|.|.|.|.
+00004d80: 7c1c 7c1d 7c1f 7c20 7c21 7c22 6423 9c13  |.|.|.| |!|"d#..
+00004d90: a401 8e01 0100 6e3a 7416 6a11 6a19 6600  ......n:t.j.j.f.
+00004da0: 6900 7c0c 7c0d 7c0e 7c0f 7c11 7c13 7c15  i.|.|.|.|.|.|.|.
+00004db0: 7c16 7c17 7c18 7c19 7c1a 7c1b 7c1c 7c1d  |.|.|.|.|.|.|.|.
+00004dc0: 7c1f 7c20 7c21 7c22 6423 9c13 a401 8e01  |.| |!|"d#......
+00004dd0: 0100 7c0c 7c0d 7c0e 7c0f 7c10 7c12 7c14  ..|.|.|.|.|.|.|.
+00004de0: 7c16 7c17 7c18 7c19 7c1a 7c1b 7c1c 7c1d  |.|.|.|.|.|.|.|.
+00004df0: 7c1e 7c20 7c21 7c22 6424 9c13 7d24 7c04  |.| |!|"d$..}$|.
+00004e00: a01a 7c24 a101 0100 717c 7166 5700 6e2a  ..|$....q|qfW.n*
+00004e10: 0400 741b 9002 797c 0100 7d25 0100 7a10  ..t...y|..}%..z.
+00004e20: 7c25 8201 5700 5900 6409 7d25 7e25 6e0a  |%..W.Y.d.}%~%n.
+00004e30: 6409 7d25 7e25 3000 3000 7c04 9002 728e  d.}%~%0.0.|...r.
+00004e40: 6425 7c04 6901 7d26 6e08 6425 6426 6901  d%|.i.}&n.d%d&i.
+00004e50: 7d26 741c 7c26 8301 5300 2927 7520 0000  }&t.|&..S.)'u ..
+00004e60: 00e5 afbc e585 a5e8 8daf e593 81e7 9bae  ................
+00004e70: e5bd 9565 7863 656c e8a1 a8e6 95b0 e68d  ...excel........
+00004e80: ae72 7900 0000 727a 0000 0072 7b00 0000  .ry...rz...r{...
+00004e90: 727c 0000 0072 7d00 0000 727e 0000 0072  r|...r}...r~...r
+00004ea0: 0100 0000 727f 0000 004e 5472 8100 0000  ....r....NTr....
+00004eb0: 7284 0000 0072 8700 0000 7288 0000 00a9  r....r....r.....
+00004ec0: 01da 0974 7970 655f 6e61 6d65 72db 0000  ...type_namer...
+00004ed0: 0072 8500 0000 72dc 0000 00a9 01da 0d63  .r....r........c
+00004ee0: 6174 6567 6f72 795f 6e61 6d65 72ed 0000  ategory_namer...
+00004ef0: 0072 ee00 0000 72ef 0000 00e9 0a00 0000  .r....r.........
+00004f00: e90b 0000 00e9 0c00 0000 e90d 0000 00e9  ................
+00004f10: 0e00 0000 e90f 0000 0072 f000 0000 46e9  .........r....F.
+00004f20: 1000 0000 e911 0000 00e9 1200 0000 a901  ................
+00004f30: 7206 0100 0029 1372 0601 0000 7207 0100  r....).r....r...
+00004f40: 0072 0801 0000 da05 756e 6974 7372 1501  .r......unitsr..
+00004f50: 0000 7217 0100 0072 1601 0000 7213 0100  ..r....r....r...
+00004f60: 0072 1401 0000 720a 0100 0072 0901 0000  .r....r....r....
+00004f70: 720b 0100 0072 0c01 0000 720d 0100 0072  r....r....r....r
+00004f80: 0e01 0000 720f 0100 0072 1001 0000 7211  ....r....r....r.
+00004f90: 0100 0072 1201 0000 2913 7206 0100 0072  ...r....).r....r
+00004fa0: 0701 0000 7208 0100 0072 4c01 0000 da15  ....r....rL.....
+00004fb0: 7072 6570 6172 6174 696f 6e5f 7479 7065  preparation_type
+00004fc0: 5f6e 616d 65da 0e64 7275 675f 7479 7065  _name..drug_type
+00004fd0: 5f6e 616d 6572 4101 0000 7213 0100 0072  _namerA...r....r
+00004fe0: 1401 0000 720a 0100 0072 0901 0000 720b  ....r....r....r.
+00004ff0: 0100 0072 0c01 0000 720d 0100 0072 0e01  ...r....r....r..
+00005000: 0000 720f 0100 0072 1001 0000 7211 0100  ..r....r....r...
+00005010: 0072 1201 0000 7235 0000 0072 8e00 0000  .r....r5...r....
+00005020: 291d 722f 0000 0072 4a00 0000 728f 0000  ).r/...rJ...r...
+00005030: 0072 8600 0000 7290 0000 0072 e100 0000  .r....r....r....
+00005040: 7292 0000 0072 9300 0000 7294 0000 0072  r....r....r....r
+00005050: 9500 0000 7296 0000 0072 9700 0000 7298  ....r....r....r.
+00005060: 0000 0072 9900 0000 729b 0000 0072 9a00  ...r....r....r..
+00005070: 0000 721d 0000 0072 3b00 0000 723c 0000  ..r....r;...r<..
+00005080: 0072 3d00 0000 721e 0000 0072 1f00 0000  .r=...r....r....
+00005090: 7219 0000 0072 9c00 0000 7248 0000 0072  r....r....rH...r
+000050a0: 9d00 0000 729e 0000 0072 6600 0000 7206  ....r....rf...r.
+000050b0: 0000 0029 2772 4100 0000 7279 0000 0072  ...)'rA...ry...r
+000050c0: 7a00 0000 729f 0000 0072 a000 0000 7235  z...r....r....r5
+000050d0: 0000 0072 9400 0000 72a1 0000 0072 a200  ...r....r....r..
+000050e0: 0000 72a3 0000 0072 9700 0000 7299 0000  ..r....r....r...
+000050f0: 0072 0601 0000 7207 0100 0072 0801 0000  .r....r....r....
+00005100: 724c 0100 0072 4d01 0000 7215 0100 0072  rL...rM...r....r
+00005110: 4e01 0000 7217 0100 0072 4101 0000 7216  N...r....rA...r.
+00005120: 0100 0072 1301 0000 7214 0100 0072 0a01  ...r....r....r..
+00005130: 0000 7209 0100 0072 0b01 0000 720c 0100  ..r....r....r...
+00005140: 0072 0d01 0000 720e 0100 005a 1069 735f  .r....r....Z.is_
+00005150: 6573 7365 6e74 6961 6c5f 7374 7272 0f01  essential_strr..
+00005160: 0000 7210 0100 0072 1101 0000 7212 0100  ..r....r....r...
+00005170: 005a 0e64 7275 675f 6469 7265 6374 6f72  .Z.drug_director
+00005180: 7972 a500 0000 726c 0000 0072 5000 0000  yr....rl...rP...
+00005190: 7243 0000 0072 4300 0000 7244 0000 00da  rC...rC...rD....
+000051a0: 1569 6d70 6f72 745f 6472 7567 5f64 6972  .import_drug_dir
+000051b0: 6563 746f 7279 6a03 0000 73d8 0000 0000  ectoryj...s.....
+000051c0: 030c 010e 011a 0204 020a 0204 0114 0108  ................
+000051d0: 010a 0106 0110 010a 0104 020e 0110 0108  ................
+000051e0: 0108 0108 0108 0112 0108 0112 0108 0112  ................
+000051f0: 0108 0108 0108 0108 0108 0108 0108 0108  ................
+00005200: 0108 010a 0106 0204 0108 0108 0108 010e  ................
+00005210: 0106 010a 0102 0102 0102 0104 0104 0104  ................
+00005220: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00005230: 0102 0102 0102 0102 ee0c 150c 0102 0102  ................
+00005240: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00005250: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00005260: ee0a 1502 0102 0102 0102 0102 0102 0102  ................
+00005270: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00005280: 0102 0102 0102 0102 ed06 1512 0110 011a  ................
+00005290: 0206 010a 0208 0172 4f01 0000 6301 0000  .......rO...c...
+000052a0: 0000 0000 0000 0000 0027 0000 0017 0000  .........'......
+000052b0: 0043 0000 0073 c002 0000 7c00 6a00 a001  .C...s....|.j...
+000052c0: 6401 a101 7d01 7c00 6a02 a001 6402 6403  d...}.|.j...d.d.
+000052d0: a102 7d02 7c02 6a03 a004 6404 a101 6405  ..}.|.j...d...d.
+000052e0: 1900 a004 6406 a101 6407 1900 7d03 6700  ....d...d...}.g.
+000052f0: 7d04 7c03 6408 7600 9002 72a0 9002 7a30  }.|.d.v...r...z0
+00005300: 7405 6a06 6409 7c02 a007 a100 640a 640b  t.j.d.|.....d.d.
+00005310: 8d03 7d05 7c05 a008 a100 7d06 7c06 4400  ..}.|.....}.|.D.
+00005320: 9002 5d08 7d07 7c07 6a09 7d08 740a 640c  ..].}.|.j.}.t.d.
+00005330: 7c08 8302 4400 9001 5df0 7d09 7c07 a00b  |...D...].}.|...
+00005340: 7c09 a101 7d0a 7c0a 727c 7c07 a00c 7c09  |...}.|.r||...|.
+00005350: 6407 a102 6a0d 7d0b 7c07 a00e 7c09 6407  d...j.}.|...|.d.
+00005360: a102 7d0c 740f 6a10 6a11 7c0c 640d 8d01  ..}.t.j.j.|.d...
+00005370: a012 a100 7d0d 7c0a 6405 1900 7d0e 7c0a  ....}.|.d...}.|.
+00005380: 640c 1900 7d0f 7c0a 640e 1900 7d10 7c0a  d...}.|.d...}.|.
+00005390: 640f 1900 7d11 7413 6a10 6a11 7c11 6410  d...}.t.j.j.|.d.
+000053a0: 8d01 a012 a100 7d12 7c0a 6411 1900 7d13  ......}.|.d...}.
+000053b0: 7414 6a10 6a11 7c13 6412 8d01 a012 a100  t.j.j.|.d.......
+000053c0: 7d14 7c0a 6413 1900 7d15 7415 6a10 6a11  }.|.d...}.t.j.j.
+000053d0: 7c15 6414 8d01 a012 a100 7d16 7c0a 6415  |.d.......}.|.d.
+000053e0: 1900 7d17 7c0a 6416 1900 7d18 7c0a 6417  ..}.|.d...}.|.d.
+000053f0: 1900 7d19 7416 6a16 a017 7c19 6418 a102  ..}.t.j...|.d...
+00005400: 7d1a 7c0a 6419 1900 7d1b 7c0a 641a 1900  }.|.d...}.|.d...
+00005410: 7d1c 7c0a 641b 1900 7d1d 7c0a 641c 1900  }.|.d...}.|.d...
+00005420: 7d1e 7c0a 641d 1900 7d1f 7c0a 641e 1900  }.|.d...}.|.d...
+00005430: 7d20 7c20 641f 6b02 9001 7288 640a 7d21  } | d.k...r.d.}!
+00005440: 6e04 6420 7d21 7c0a 6421 1900 7d22 7418  n.d }!|.d!..}"t.
+00005450: 6a10 6a11 7c0e 6422 8d01 7d23 7c23 9001  j.j.|.d"..}#|#..
+00005460: 72f6 7c23 6a19 6600 6900 7c0e 7c0d 6a1a  r.|#j.f.i.|.|.j.
+00005470: 7c0f 7c10 7c12 6a1a 7c14 6a1a 7c16 6a1a  |.|.|.j.|.j.|.j.
+00005480: 7c17 7c18 7c1a 7c1b 7c1c 741b 7c1d 8301  |.|.|.|.|.t.|...
+00005490: 741b 7c1e 8301 741b 7c1f 8301 7c21 741b  t.|...t.|...|!t.
+000054a0: 7c22 8301 6423 9c11 a401 8e01 0100 6e46  |"..d#........nF
+000054b0: 7418 6a10 6a1c 6600 6900 7c0e 7c0d 7c0f  t.j.j.f.i.|.|.|.
+000054c0: 7c10 7c12 7c14 7c16 7c17 7c18 7c1a 7c1b  |.|.|.|.|.|.|.|.
+000054d0: 7c1c 741b 7c1d 8301 741b 7c1e 8301 741b  |.t.|...t.|...t.
+000054e0: 7c1f 8301 7c21 741b 7c22 8301 6423 9c11  |...|!t.|"..d#..
+000054f0: a401 8e01 0100 7c0c 7c0e 7c0f 7c10 7c11  ......|.|.|.|.|.
+00005500: 7c13 7c15 7c17 7c18 7c1a 7c1b 7c1c 7c1d  |.|.|.|.|.|.|.|.
+00005510: 7c1e 7c1f 7c21 7c22 6424 9c11 7d24 7c04  |.|.|!|"d$..}$|.
+00005520: a01d 7c24 a101 0100 717c 7166 5700 6e2a  ..|$....q|qfW.n*
+00005530: 0400 741e 9002 799e 0100 7d25 0100 7a10  ..t...y...}%..z.
+00005540: 7c25 8201 5700 5900 6409 7d25 7e25 6e0a  |%..W.Y.d.}%~%n.
+00005550: 6409 7d25 7e25 3000 3000 7c04 9002 72b0  d.}%~%0.0.|...r.
+00005560: 6425 7c04 6901 7d26 6e08 6425 6426 6901  d%|.i.}&n.d%d&i.
+00005570: 7d26 741f 7c26 8301 5300 2927 7520 0000  }&t.|&..S.)'u ..
+00005580: 00e5 afbc e585 a5e8 8daf e688 bfe8 8daf  ................
+00005590: e593 8165 7863 656c e8a1 a8e6 95b0 e68d  ...excel........
+000055a0: ae72 7900 0000 727a 0000 0072 7b00 0000  .ry...rz...r{...
+000055b0: 727c 0000 0072 7d00 0000 727e 0000 0072  r|...r}...r~...r
+000055c0: 0100 0000 727f 0000 004e 5472 8100 0000  ....r....NTr....
+000055d0: 7284 0000 0029 01da 0d70 6861 726d 6163  r....)...pharmac
+000055e0: 795f 6e61 6d65 7287 0000 0072 8800 0000  y_namer....r....
+000055f0: 723e 0100 0072 db00 0000 7285 0000 0072  r>...r....r....r
+00005600: dc00 0000 7240 0100 0072 ed00 0000 72ee  ....r@...r....r.
+00005610: 0000 0072 ef00 0000 7a08 2559 2d25 6d2d  ...r....z.%Y-%m-
+00005620: 2564 7242 0100 0072 4301 0000 7244 0100  %drB...rC...rD..
+00005630: 0072 4501 0000 7246 0100 0072 4801 0000  .rE...rF...rH...
+00005640: 72f0 0000 0046 7247 0100 0072 4b01 0000  r....FrG...rK...
+00005650: 2911 7206 0100 00da 0870 6861 726d 6163  ).r......pharmac
+00005660: 7972 0701 0000 7208 0100 0072 1501 0000  yr....r....r....
+00005670: 7217 0100 0072 1601 0000 7213 0100 0072  r....r....r....r
+00005680: 1401 0000 da0a 7661 6c69 645f 6461 7465  ......valid_date
+00005690: da12 696e 7665 6e74 6f72 795f 7175 616e  ..inventory_quan
+000056a0: 7469 7479 da10 6d65 6173 7572 656d 656e  tity..measuremen
+000056b0: 745f 756e 6974 da0f 636f 7374 5f75 6e69  t_unit..cost_uni
+000056c0: 745f 7072 6963 65da 0b63 6f73 745f 616d  t_price..cost_am
+000056d0: 6f75 6e74 da11 7265 7461 696c 5f75 6e69  ount..retail_uni
+000056e0: 745f 7072 6963 6572 3e00 0000 da0d 7265  t_pricer>.....re
+000056f0: 7461 696c 5f61 6d6f 756e 7429 1172 5001  tail_amount).rP.
+00005700: 0000 7206 0100 0072 0701 0000 7208 0100  ..r....r....r...
+00005710: 0072 4d01 0000 724e 0100 0072 4101 0000  .rM...rN...rA...
+00005720: 7213 0100 0072 1401 0000 7252 0100 0072  r....r....rR...r
+00005730: 5301 0000 7254 0100 0072 5501 0000 7256  S...rT...rU...rV
+00005740: 0100 0072 5701 0000 723e 0000 0072 5801  ...rW...r>...rX.
+00005750: 0000 7235 0000 0072 8e00 0000 2920 722f  ..r5...r....) r/
+00005760: 0000 0072 4a00 0000 728f 0000 0072 8600  ...rJ...r....r..
+00005770: 0000 7290 0000 0072 e100 0000 7292 0000  ..r....r....r...
+00005780: 0072 9300 0000 7294 0000 0072 9500 0000  .r....r....r....
+00005790: 7296 0000 0072 9700 0000 7298 0000 0072  r....r....r....r
+000057a0: 9900 0000 729a 0000 0072 1a00 0000 723b  ....r....r....r;
+000057b0: 0000 0072 3c00 0000 723d 0000 0072 1d00  ...r<...r=...r..
+000057c0: 0000 721e 0000 0072 1f00 0000 724c 0000  ..r....r....rL..
+000057d0: 00da 0873 7472 7074 696d 6572 2000 0000  ...strptimer ...
+000057e0: 729c 0000 0072 4800 0000 da05 666c 6f61  r....rH.....floa
+000057f0: 7472 9d00 0000 729e 0000 0072 6600 0000  tr....r....rf...
+00005800: 7206 0000 0029 2772 4100 0000 7279 0000  r....)'rA...ry..
+00005810: 0072 7a00 0000 729f 0000 0072 a000 0000  .rz...r....r....
+00005820: 7235 0000 0072 9400 0000 72a1 0000 0072  r5...r....r....r
+00005830: a200 0000 72a3 0000 0072 9700 0000 7299  ....r....r....r.
+00005840: 0000 0072 5001 0000 da13 7068 6172 6d61  ...rP.....pharma
+00005850: 6379 5f6d 616e 6167 656d 656e 7472 0601  cy_managementr..
+00005860: 0000 7207 0100 0072 0801 0000 724d 0100  ..r....r....rM..
+00005870: 0072 1501 0000 724e 0100 0072 1701 0000  .r....rN...r....
+00005880: 7241 0100 0072 1601 0000 7213 0100 0072  rA...r....r....r
+00005890: 1401 0000 5a0e 7661 6c69 645f 6461 7465  ....Z.valid_date
+000058a0: 5f73 7472 7252 0100 0072 5301 0000 7254  _strrR...rS...rT
+000058b0: 0100 0072 5501 0000 7256 0100 0072 5701  ...rU...rV...rW.
+000058c0: 0000 5a0d 6973 5f61 6374 6976 655f 7374  ..Z.is_active_st
+000058d0: 7272 3e00 0000 7258 0100 005a 0d70 6861  rr>...rX...Z.pha
+000058e0: 726d 6163 795f 6472 7567 72a5 0000 0072  rmacy_drugr....r
+000058f0: 6c00 0000 7250 0000 0072 4300 0000 7243  l...rP...rC...rC
+00005900: 0000 0072 4400 0000 da14 696d 706f 7274  ...rD.....import
+00005910: 5f70 6861 726d 6163 795f 6472 7567 e403  _pharmacy_drug..
+00005920: 0000 73cc 0000 0000 030c 010e 011a 0204  ..s.............
+00005930: 020a 0204 0114 0108 010a 0106 0110 010a  ................
+00005940: 0104 020e 010c 0112 0108 0108 0108 0108  ................
+00005950: 0112 0108 0112 0108 0112 0108 0108 0108  ................
+00005960: 010e 0108 0108 0108 0108 0108 0108 010a  ................
+00005970: 0106 0204 0108 010e 0106 010a 0104 0102  ................
+00005980: 0102 0104 0104 0104 0102 0102 0102 0102  ................
+00005990: 0102 0106 0106 0106 0102 0106 f00c 130c  ................
+000059a0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+000059b0: 0102 0102 0102 0106 0106 0106 0102 0106  ................
+000059c0: f00a 1302 0102 0102 0102 0102 0102 0102  ................
+000059d0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+000059e0: 0102 0102 ef06 1312 0110 011a 0206 010a  ................
+000059f0: 0208 0172 5c01 0000 2967 7273 0000 0072  ...r\...)grs...r
+00005a00: 4c00 0000 7237 0000 00da 0872 6571 7565  L...r7.....reque
+00005a10: 7374 7372 e100 0000 726e 0000 005a 1c64  stsr....rn...Z.d
+00005a20: 6a61 6e67 6f2e 636f 6e74 7269 622e 6175  jango.contrib.au
+00005a30: 7468 2e62 6163 6b65 6e64 7372 0200 0000  th.backendsr....
+00005a40: da1b 646a 616e 676f 2e63 6f6e 7472 6962  ..django.contrib
+00005a50: 2e61 7574 682e 6861 7368 6572 7372 0300  .auth.hashersr..
+00005a60: 0000 da1a 646a 616e 676f 2e63 6f6e 7472  ....django.contr
+00005a70: 6962 2e61 7574 682e 6d6f 6465 6c73 7204  ib.auth.modelsr.
+00005a80: 0000 00da 0964 6a61 6e67 6f2e 6462 7205  .....django.dbr.
+00005a90: 0000 00da 0b64 6a61 6e67 6f2e 6874 7470  .....django.http
+00005aa0: 7206 0000 0072 0700 0000 da0e 646a 616e  r....r......djan
+00005ab0: 676f 5f66 696c 7465 7273 72b3 0000 005a  go_filtersr....Z
+00005ac0: 1064 7266 5f65 7863 656c 2e6d 6978 696e  .drf_excel.mixin
+00005ad0: 7372 0800 0000 5a13 6472 665f 6578 6365  sr....Z.drf_exce
+00005ae0: 6c2e 7265 6e64 6572 6572 7372 0900 0000  l.renderersr....
+00005af0: da0e 7265 7374 5f66 7261 6d65 776f 726b  ..rest_framework
+00005b00: 720a 0000 005a 1972 6573 745f 6672 616d  r....Z.rest_fram
+00005b10: 6577 6f72 6b2e 6465 636f 7261 746f 7273  ework.decorators
+00005b20: 720b 0000 005a 1772 6573 745f 6672 616d  r....Z.rest_fram
+00005b30: 6577 6f72 6b2e 6765 6e65 7269 6373 720c  ework.genericsr.
+00005b40: 0000 005a 1a72 6573 745f 6672 616d 6577  ...Z.rest_framew
+00005b50: 6f72 6b2e 7065 726d 6973 7369 6f6e 7372  ork.permissionsr
+00005b60: 0d00 0000 da17 7265 7374 5f66 7261 6d65  ......rest_frame
+00005b70: 776f 726b 2e72 6573 706f 6e73 6572 0e00  work.responser..
+00005b80: 0000 5a17 7265 7374 5f66 7261 6d65 776f  ..Z.rest_framewo
+00005b90: 726b 2e76 6965 7773 6574 7372 0f00 0000  rk.viewsetsr....
+00005ba0: 7210 0000 00da 1262 6173 655f 7379 7374  r......base_syst
+00005bb0: 656d 2e6d 6f64 656c 7372 1100 0000 7212  em.modelsr....r.
+00005bc0: 0000 0072 1300 0000 7214 0000 0072 1500  ...r....r....r..
+00005bd0: 0000 7216 0000 0072 1700 0000 7218 0000  ..r....r....r...
+00005be0: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
+00005bf0: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
+00005c00: 1f00 0000 7220 0000 0072 2100 0000 7222  ....r ...r!...r"
+00005c10: 0000 005a 1762 6173 655f 7379 7374 656d  ...Z.base_system
+00005c20: 2e73 6572 6961 6c69 7a65 7273 7223 0000  .serializersr#..
+00005c30: 0072 2400 0000 7225 0000 0072 2600 0000  .r$...r%...r&...
+00005c40: 7227 0000 0072 2800 0000 7229 0000 0072  r'...r(...r)...r
+00005c50: 2a00 0000 722b 0000 0072 2c00 0000 da0b  *...r+...r,.....
+00005c60: 646a 616e 676f 2e63 6f6e 6672 2d00 0000  django.confr-...
+00005c70: da0f 646a 616e 676f 5f73 6574 7469 6e67  ..django_setting
+00005c80: 7372 9100 0000 722e 0000 00da 0272 6572  sr....r......rer
+00005c90: 0201 0000 7245 0000 0072 5100 0000 7252  ....rE...rQ...rR
+00005ca0: 0000 0072 6200 0000 7264 0000 00da 0661  ...rb...rd.....a
+00005cb0: 746f 6d69 6372 a600 0000 da09 4669 6c74  tomicr......Filt
+00005cc0: 6572 5365 7472 a700 0000 72b6 0000 0072  erSetr....r....r
+00005cd0: c700 0000 72cb 0000 0072 d200 0000 72d5  ....r....r....r.
+00005ce0: 0000 0072 d600 0000 72d7 0000 0072 d800  ...r....r....r..
+00005cf0: 0000 72d9 0000 0072 da00 0000 72e4 0000  ..r....r....r...
+00005d00: 0072 0001 0000 72fb 0000 0072 0501 0000  .r....r....r....
+00005d10: 721c 0100 0072 1d01 0000 7233 0100 0072  r....r....r3...r
+00005d20: 3c01 0000 723d 0100 0072 4f01 0000 725c  <...r=...rO...r\
+00005d30: 0100 0072 4300 0000 7243 0000 0072 4300  ...rC...rC...rC.
+00005d40: 0000 7244 0000 00da 083c 6d6f 6475 6c65  ..rD.....<module
+00005d50: 3e01 0000 0073 7e00 0000 0801 0801 0802  >....s~.........
+00005d60: 0801 0802 0801 0c01 0c01 0c01 0c01 1001  ................
+00005d70: 0801 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00005d80: 1002 5003 2c04 0c01 0c03 0801 0c01 0801  ..P.,...........
+00005d90: 0803 0813 0812 1018 1020 0e1c 0401 0a3d  ......... .....=
+00005da0: 120d 1016 1007 120c 1008 0806 1007 120c  ................
+00005db0: 1007 0806 1007 0401 0a51 0401 0a7f 0053  .........Q.....S
+00005dc0: 080c 121a 0809 102e 1005 0401 0a4b 0401  .............K..
+00005dd0: 0a4b 0401 0a79 0401                      .K...y..
```

### Comparing `base_system-0.2.7/base_system/__pycache__/viewsets.cpython-39.pyc` & `base_system-0.2.8/base_system/__pycache__/viewsets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/base_system/auth.py` & `base_system-0.2.8/base_system/auth.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/base_system/export_viewset.py` & `base_system-0.2.8/base_system/export_viewset.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/base_system/migrations/0001_initial.py` & `base_system-0.2.8/base_system/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/base_system/migrations/0003_alter_extragroup_hospital.py` & `base_system-0.2.8/base_system/migrations/0003_alter_extragroup_hospital.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/base_system/migrations/0005_expensetype.py` & `base_system-0.2.8/base_system/migrations/0005_expensetype.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/base_system/migrations/0007_auto_20230512_1742.py` & `base_system-0.2.8/base_system/migrations/0007_auto_20230512_1742.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc` & `base_system-0.2.8/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc` & `base_system-0.2.8/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc` & `base_system-0.2.8/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/base_system/migrations/__pycache__/0004_alter_extragroup_role_name.cpython-39.pyc` & `base_system-0.2.8/base_system/migrations/__pycache__/0004_alter_extragroup_role_name.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/base_system/migrations/__pycache__/0005_expensetype.cpython-39.pyc` & `base_system-0.2.8/base_system/migrations/__pycache__/0005_expensetype.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/base_system/migrations/__pycache__/0006_alter_doctor_photo.cpython-39.pyc` & `base_system-0.2.8/base_system/migrations/__pycache__/0006_alter_doctor_photo.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/base_system/migrations/__pycache__/0007_auto_20230512_1742.cpython-39.pyc` & `base_system-0.2.8/base_system/migrations/__pycache__/0007_auto_20230512_1742.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/base_system/models.py` & `base_system-0.2.8/base_system/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import os
+from django.db import transaction
 
 import requests
 from django.contrib.auth.models import AbstractUser, Group
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
 from django.conf import settings
 
@@ -373,14 +374,35 @@
     name_srvtp = models.CharField(verbose_name="检查类型名称", max_length=50, null=True)
 
     class Meta:
         db_table = 'bs_inspection_dictionaries'
         verbose_name = '检查字典'
         verbose_name_plural = verbose_name
 
+    # 导入json文件数据
+    def upload(self):
+        with open('./base_system/inspdic.json', encoding='utf-8') as a:
+            # 读取文件
+            result = json.load(a)
+            data = result['content']['data']['itemsrvinfos']['itemsrvinfo']
+            with transaction.atomic():
+                for res in data:
+                    print(res)
+                    sp_dic = InspectionDictionaries.objects.filter(project_code=res['code_srv'])
+                    if not sp_dic:
+                        InspectionDictionaries.objects.create(
+                            project_code=res['code_srv'],
+                            project_name=res['name_srv'],
+                            hospital_code=res['code_org'],
+                            project_fees=res.get('price'),
+                            code_srvtp=res['code_srvtp'],
+                            name_srvtp=res['name_srvtp'],
+                        )
+            return data
+
 
 class ExaminationType(MedicalBaseModel):
     code_srvtp = models.CharField(verbose_name="检查类型编码", max_length=50)
     name_srvtp = models.CharField(verbose_name="检查类型名称", max_length=50)
     parent = models.ForeignKey(
         'self',
         verbose_name='父级',
@@ -407,14 +429,35 @@
     name_srvtp = models.CharField(verbose_name="检验类型名称", max_length=50, null=True)
 
     class Meta:
         db_table = 'bs_examination_dictionaries'
         verbose_name = '检验字典'
         verbose_name_plural = verbose_name
 
+    # 导入json文件数据
+    def upload(self):
+        with open('./base_system/examination_dic.json', encoding='utf-8') as a:
+            # 读取文件
+            result = json.load(a)
+            data = result['content']['data']['itemsrvinfos']['itemsrvinfo']
+            with transaction.atomic():
+                for res in data:
+                    print(res)
+                    sp_dic = ExaminationDictionaries.objects.filter(project_code=res['code_srv'])
+                    if not sp_dic:
+                        ExaminationDictionaries.objects.create(
+                            project_code=res['code_srv'],
+                            project_name=res['name_srv'],
+                            hospital_code=res['code_org'],
+                            project_fees=res.get('price'),
+                            code_srvtp=res['code_srvtp'],
+                            name_srvtp=res['name_srvtp'],
+                        )
+        return data
+
 
 class DrugPreparationType(MedicalBaseModel):
     codenum = models.CharField(max_length=255, verbose_name="编码", unique=True)
     type_name = models.CharField(max_length=64, verbose_name="类型名称", null=True, blank=True)
 
     class Meta:
         db_table = 'bs_drug_preparation_type'
```

### Comparing `base_system-0.2.7/base_system/serializers.py` & `base_system-0.2.8/base_system/serializers.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/base_system/urls.py` & `base_system-0.2.8/base_system/urls.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,17 @@
     path('import_doctor/', views.import_doctor),  # 医生信息导入接口
     path('import_ins_dic/', views.import_inspection_dictionaries),  # 导入检查字典excel表数据
     path('import_exa_dic/', views.import_examination_dictionaries),  # 导入检验字典excel表数据
     path('import_drug_dir/', views.import_drug_directory),  # 导入药品目录excel表数据
     path('import_pharmacy_drug/', views.import_pharmacy_drug),  # 导入药房药品excel表数据
     path('menu_permissions/', viewsets.menu_permissions),
 
+    path('inspection/import/', views.inspection_import),  # 检查字典数据导入
+    path('examination/import/', views.examination_import),  # 检验字典数据接口
+
 ]
 router = routers.DefaultRouter()
 
 router.register(r'hospitals', viewsets.HospitalViewSet)
 router.register(r'offices', viewsets.OfficeViewSet)
 router.register(r'doctors', viewsets.DoctorViewSet)
 router.register(r'groups', viewsets.GroupViewSet)  # 角色
```

### Comparing `base_system-0.2.7/base_system/views.py` & `base_system-0.2.8/base_system/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,17 +244,14 @@
     def change_password(self, request, pk):
         # 更改密码
         serializer = PasswordSerializer(data=request.data, context={"request": request})
         serializer.is_valid(raise_exception=True)
         password = serializer.data.get("password")
         user = self.get_object()
         user.set_password(password)
-        user.last_change_time = datetime.datetime.now()
-        user.error_times = 0
-        user.is_change_pwd = False
         user.save()
 
         return Response(data={"message": "修改成功"}, status=status.HTTP_205_RESET_CONTENT)
 
 
 class InspectionTypeViewSet(ModelViewSet):
     """检查字典"""
@@ -278,31 +275,19 @@
 class InspectionDictionariesViewSet(ModelViewSet):
     """检查字典"""
     queryset = InspectionDictionaries.objects.all().order_by('-id')
     serializer_class = InspectionDictionariesSerializer
     # filter_fields = "__all__"
     filterset_class = InspectionDictFilter
 
-    # 导入json文件数据
-    # def create(self, request, *args, **kwargs):
-    #     with open('spdic.json', encoding='utf-8') as a:
-    #         # 读取文件
-    #         result = json.load(a)
-    #         data = result['content']['data']['itemsrvinfos']['itemsrvinfo']
-    #         for res in data:
-    #             print(res)
-    #             InspectionDictionaries.objects.create(
-    #                 project_code=res['code_srv'],
-    #                 project_name=res['name_srv'],
-    #                 hospital_code=res['code_org'],
-    #                 project_fees=res['price'],
-    #                 code_srvtp=res['code_srvtp'],
-    #                 name_srvtp=res['name_srvtp'],
-    #             )
-    #     return Response({"data": data})
+
+def inspection_import(request):
+    inspdic = InspectionDictionaries()
+    res = inspdic.upload()
+    return JsonResponse({"data": res})
 
 
 class ExaminationTypeViewSet(ModelViewSet):
     """检查字典"""
     queryset = ExaminationType.objects.filter(parent=None)
     serializer_class = ExaminationTypeSerializer
     pagination_class = None
@@ -323,33 +308,18 @@
 class ExaminationDictionariesViewSet(ModelViewSet):
     """检验字典"""
     queryset = ExaminationDictionaries.objects.all().order_by('-id')
     serializer_class = ExaminationDictionariesSerializer
     # filter_fields = "__all__"
     filterset_class = ExaminationDictFilter
 
-    # 导入json文件数据
-    # def create(self, request, *args, **kwargs):
-    #     with open('response.json', encoding='utf-8') as a:
-    #         # 读取文件
-    #         result = json.load(a)
-    #         data = result['content']['data']['itemsrvinfos']['itemsrvinfo']
-    #         for res in data:
-    #             print(res)
-    #             sp_dic = InspectionDictionaries.objects.filter(project_code=res['code_srv'])
-    #             if not sp_dic:
-    #                 ExaminationDictionaries.objects.create(
-    #                     project_code=res['code_srv'],
-    #                     project_name=res['name_srv'],
-    #                     hospital_code=res['code_org'],
-    #                     project_fees=res.get('price'),
-    #                     code_srvtp=res['code_srvtp'],
-    #                     name_srvtp=res['name_srvtp'],
-    #                 )
-    #     return Response({"data": data})
+def examination_import(request):
+    exadic = ExaminationDictionaries()
+    res = exadic.upload()
+    return JsonResponse({"data": res})
 
 
 class PharmacyManagementViewSet(ModelViewSet):
     """药房管理"""
     queryset = PharmacyManagement.objects.all().order_by('-id')
     serializer_class = PharmacyManagementSerializer
     filter_fields = "__all__"
```

### Comparing `base_system-0.2.7/base_system/viewsets.py` & `base_system-0.2.8/base_system/viewsets.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/base_system.egg-info/PKG-INFO` & `base_system-0.2.8/base_system.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: base-system
-Version: 0.2.7
+Version: 0.2.8
 Summary: Basic feature component
 Home-page: https://github.com/zcjwin
 Author: zcjwin
 Author-email: win_zcj@163.com
 License: UNKNOWN
 Keywords: base_system
 Platform: UNKNOWN
```

### Comparing `base_system-0.2.7/base_system.egg-info/SOURCES.txt` & `base_system-0.2.8/base_system.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 BaseFunctionModule/settings.py
 BaseFunctionModule/urls.py
 BaseFunctionModule/wsgi.py
 base_system/__init__.py
 base_system/admin.py
 base_system/apps.py
 base_system/auth.py
+base_system/examination_dic.json
 base_system/export_viewset.py
+base_system/inspdic.json
 base_system/models.py
 base_system/serializers.py
 base_system/tests.py
 base_system/urls.py
 base_system/views.py
 base_system/viewsets.py
 base_system.egg-info/PKG-INFO
```

### Comparing `base_system-0.2.7/init_data.json` & `base_system-0.2.8/init_data.json`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/manage.py` & `base_system-0.2.8/manage.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/requirements.txt` & `base_system-0.2.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/runtests.py` & `base_system-0.2.8/runtests.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.7/setup.py` & `base_system-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name="base_system",
-    version='0.2.7',
+    version='0.2.8',
     description="Basic feature component",
     keywords='base_system',
     # long_description=README,
     long_description_content_type="text/markdown",
     author='zcjwin',
     author_email='win_zcj@163.com',
     url="https://github.com/zcjwin",
```

