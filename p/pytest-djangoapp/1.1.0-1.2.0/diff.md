# Comparing `tmp/pytest-djangoapp-1.1.0.tar.gz` & `tmp/pytest-djangoapp-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-djangoapp-1.1.0.tar", last modified: Sat Mar 18 10:20:30 2023, max compression
+gzip compressed data, was "pytest-djangoapp-1.2.0.tar", last modified: Fri May 19 12:17:21 2023, max compression
```

## Comparing `pytest-djangoapp-1.1.0.tar` & `pytest-djangoapp-1.2.0.tar`

### file list

```diff
@@ -1,87 +1,90 @@
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-03-18 10:20:30.747204 pytest-djangoapp-1.1.0/
--rw-rw-r--   0 idle      (1000) idle      (1000)      248 2022-11-09 11:39:55.000000 pytest-djangoapp-1.1.0/AUTHORS
--rw-rw-r--   0 idle      (1000) idle      (1000)     3037 2023-03-18 10:20:24.000000 pytest-djangoapp-1.1.0/CHANGELOG
--rw-r--r--   0 idle      (1000) idle      (1000)      506 2018-06-14 13:30:02.000000 pytest-djangoapp-1.1.0/INSTALL
--rw-rw-r--   0 idle      (1000) idle      (1000)     1509 2023-03-18 09:27:40.000000 pytest-djangoapp-1.1.0/LICENSE
--rw-r--r--   0 idle      (1000) idle      (1000)      280 2018-06-14 13:30:02.000000 pytest-djangoapp-1.1.0/MANIFEST.in
--rw-rw-r--   0 idle      (1000) idle      (1000)     4315 2023-03-18 10:20:30.747204 pytest-djangoapp-1.1.0/PKG-INFO
--rw-rw-r--   0 idle      (1000) idle      (1000)     3266 2022-11-09 13:04:17.000000 pytest-djangoapp-1.1.0/README.rst
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-03-18 10:20:30.739204 pytest-djangoapp-1.1.0/docs/
--rw-r--r--   0 idle      (1000) idle      (1000)     4635 2018-06-14 13:30:02.000000 pytest-djangoapp-1.1.0/docs/Makefile
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-03-18 10:20:30.743204 pytest-djangoapp-1.1.0/docs/source/
--rw-rw-r--   0 idle      (1000) idle      (1000)     8286 2023-03-18 09:27:47.000000 pytest-djangoapp-1.1.0/docs/source/conf.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      347 2023-03-18 09:24:59.000000 pytest-djangoapp-1.1.0/docs/source/fixtures.rst
--rw-rw-r--   0 idle      (1000) idle      (1000)      143 2018-06-18 12:42:49.000000 pytest-djangoapp-1.1.0/docs/source/fixtures_commands.rst
--rw-rw-r--   0 idle      (1000) idle      (1000)      161 2019-10-19 06:34:29.000000 pytest-djangoapp-1.1.0/docs/source/fixtures_db.rst
--rw-rw-r--   0 idle      (1000) idle      (1000)      126 2018-07-24 13:46:52.000000 pytest-djangoapp-1.1.0/docs/source/fixtures_mail.rst
--rw-rw-r--   0 idle      (1000) idle      (1000)      132 2018-09-14 14:44:08.000000 pytest-djangoapp-1.1.0/docs/source/fixtures_messages.rst
--rw-rw-r--   0 idle      (1000) idle      (1000)      147 2022-11-09 11:43:41.000000 pytest-djangoapp-1.1.0/docs/source/fixtures_migrations.rst
--rw-rw-r--   0 idle      (1000) idle      (1000)      136 2018-06-16 10:05:14.000000 pytest-djangoapp-1.1.0/docs/source/fixtures_request.rst
--rw-rw-r--   0 idle      (1000) idle      (1000)      145 2018-06-16 10:04:33.000000 pytest-djangoapp-1.1.0/docs/source/fixtures_settings.rst
--rw-rw-r--   0 idle      (1000) idle      (1000)      143 2018-06-16 10:04:52.000000 pytest-djangoapp-1.1.0/docs/source/fixtures_templates.rst
--rw-rw-r--   0 idle      (1000) idle      (1000)      120 2018-06-16 10:05:32.000000 pytest-djangoapp-1.1.0/docs/source/fixtures_users.rst
--rw-rw-r--   0 idle      (1000) idle      (1000)      109 2023-03-18 09:25:51.000000 pytest-djangoapp-1.1.0/docs/source/fixtures_utils.rst
--rw-rw-r--   0 idle      (1000) idle      (1000)      682 2022-11-09 13:04:17.000000 pytest-djangoapp-1.1.0/docs/source/index.rst
--rw-rw-r--   0 idle      (1000) idle      (1000)     4318 2020-01-25 08:36:44.000000 pytest-djangoapp-1.1.0/docs/source/quickstart.rst
--rw-r--r--   0 idle      (1000) idle      (1000)     1389 2018-06-14 13:30:02.000000 pytest-djangoapp-1.1.0/docs/source/rst_guide.rst
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-03-18 10:20:30.743204 pytest-djangoapp-1.1.0/pytest_djangoapp/
--rw-rw-r--   0 idle      (1000) idle      (1000)      193 2023-03-18 10:20:24.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/__init__.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      438 2022-11-09 12:39:21.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/compat.py
--rw-rw-r--   0 idle      (1000) idle      (1000)     9259 2023-03-18 09:22:44.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/configuration.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-03-18 10:20:30.743204 pytest-djangoapp-1.1.0/pytest_djangoapp/fixtures/
--rw-rw-r--   0 idle      (1000) idle      (1000)      496 2023-03-18 10:05:40.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/fixtures/__init__.py
--rw-rw-r--   0 idle      (1000) idle      (1000)     1828 2023-03-18 10:05:08.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/fixtures/commands.py
--rw-rw-r--   0 idle      (1000) idle      (1000)     3264 2022-11-09 12:14:06.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/fixtures/db.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      368 2022-11-09 12:15:09.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/fixtures/mail.py
--rw-rw-r--   0 idle      (1000) idle      (1000)     1462 2022-11-09 12:17:44.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/fixtures/messages.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      706 2023-03-18 10:06:24.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/fixtures/migrations.py
--rw-rw-r--   0 idle      (1000) idle      (1000)     5452 2022-11-09 12:35:32.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/fixtures/request.py
--rw-rw-r--   0 idle      (1000) idle      (1000)     2555 2022-11-09 12:27:48.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/fixtures/settings.py
--rw-rw-r--   0 idle      (1000) idle      (1000)     4273 2023-03-18 09:35:01.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/fixtures/templates.py
--rw-rw-r--   0 idle      (1000) idle      (1000)     2117 2022-11-09 12:53:20.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/fixtures/users.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      363 2023-03-18 09:26:39.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/fixtures/utils.py
--rw-rw-r--   0 idle      (1000) idle      (1000)     1059 2022-11-09 12:46:23.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/plugin.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-03-18 10:20:30.747204 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/
--rw-rw-r--   0 idle      (1000) idle      (1000)        0 2020-01-25 08:47:25.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/__init__.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      643 2022-11-09 11:39:55.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/conftest.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      163 2021-08-02 11:46:50.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/settings_project.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      805 2023-03-18 09:22:44.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/test_configuration.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      678 2021-08-02 11:48:59.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/test_etc.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      521 2023-03-18 10:05:57.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/test_fixtures_commands.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      309 2020-01-25 08:47:25.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/test_fixtures_mail.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      447 2022-11-09 12:02:45.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/test_fixtures_messages.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      892 2022-11-09 11:49:40.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/test_fixtures_migrations.py
--rw-rw-r--   0 idle      (1000) idle      (1000)     1399 2020-09-20 13:13:40.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/test_fixtures_request.py
--rw-rw-r--   0 idle      (1000) idle      (1000)     2442 2020-07-30 10:07:08.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/test_fixtures_settings.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      678 2023-03-18 09:38:19.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/test_fixtures_templates.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      326 2020-01-25 08:47:25.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/test_fixtures_users.py
--rw-rw-r--   0 idle      (1000) idle      (1000)       88 2023-03-18 09:19:49.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/test_fixtures_utils.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      599 2020-01-25 08:47:25.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/test_models.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-03-18 10:20:30.747204 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/testapp/
--rw-rw-r--   0 idle      (1000) idle      (1000)        0 2020-01-25 08:47:25.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/testapp/__init__.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-03-18 10:20:30.747204 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/testapp/management/
--rw-rw-r--   0 idle      (1000) idle      (1000)        0 2020-01-25 08:47:25.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/testapp/management/__init__.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-03-18 10:20:30.747204 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/testapp/management/commands/
--rw-rw-r--   0 idle      (1000) idle      (1000)        0 2020-01-25 08:47:25.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/testapp/management/commands/__init__.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      735 2022-11-09 13:02:05.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/testapp/management/commands/compat.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      616 2022-11-09 12:53:58.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/testapp/management/commands/my_command.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-03-18 10:20:30.747204 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/testapp/migrations/
--rw-rw-r--   0 idle      (1000) idle      (1000)      489 2022-11-09 11:39:55.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/testapp/migrations/0001_initial.py
--rw-rw-r--   0 idle      (1000) idle      (1000)        0 2022-11-09 11:39:55.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/testapp/migrations/__init__.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      106 2020-01-25 08:47:25.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/testapp/models.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      829 2022-11-09 12:53:46.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/testapp/urls.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-03-18 10:20:30.747204 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/testapp_missing_migrations/
--rw-rw-r--   0 idle      (1000) idle      (1000)        0 2022-11-09 11:39:55.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/testapp_missing_migrations/__init__.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-03-18 10:20:30.747204 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/testapp_missing_migrations/migrations/
--rw-rw-r--   0 idle      (1000) idle      (1000)        0 2022-11-09 11:39:55.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/testapp_missing_migrations/migrations/__init__.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      106 2022-11-09 11:39:55.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/tests/testapp_missing_migrations/models.py
--rw-rw-r--   0 idle      (1000) idle      (1000)     3075 2022-11-09 12:50:12.000000 pytest-djangoapp-1.1.0/pytest_djangoapp/toolbox.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-03-18 10:20:30.743204 pytest-djangoapp-1.1.0/pytest_djangoapp.egg-info/
--rw-rw-r--   0 idle      (1000) idle      (1000)     4315 2023-03-18 10:20:30.000000 pytest-djangoapp-1.1.0/pytest_djangoapp.egg-info/PKG-INFO
--rw-rw-r--   0 idle      (1000) idle      (1000)     2659 2023-03-18 10:20:30.000000 pytest-djangoapp-1.1.0/pytest_djangoapp.egg-info/SOURCES.txt
--rw-rw-r--   0 idle      (1000) idle      (1000)        1 2023-03-18 10:20:30.000000 pytest-djangoapp-1.1.0/pytest_djangoapp.egg-info/dependency_links.txt
--rw-rw-r--   0 idle      (1000) idle      (1000)        1 2021-08-02 11:34:48.000000 pytest-djangoapp-1.1.0/pytest_djangoapp.egg-info/not-zip-safe
--rw-rw-r--   0 idle      (1000) idle      (1000)        7 2023-03-18 10:20:30.000000 pytest-djangoapp-1.1.0/pytest_djangoapp.egg-info/requires.txt
--rw-rw-r--   0 idle      (1000) idle      (1000)       17 2023-03-18 10:20:30.000000 pytest-djangoapp-1.1.0/pytest_djangoapp.egg-info/top_level.txt
--rw-r--r--   0 idle      (1000) idle      (1000)      110 2023-03-18 10:20:30.747204 pytest-djangoapp-1.1.0/setup.cfg
--rw-rw-r--   0 idle      (1000) idle      (1000)     2239 2023-03-18 10:10:57.000000 pytest-djangoapp-1.1.0/setup.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:17:21.668973 pytest-djangoapp-1.2.0/
+-rw-rw-r--   0 idle      (1000) idle      (1000)      248 2022-11-09 11:39:55.000000 pytest-djangoapp-1.2.0/AUTHORS
+-rw-rw-r--   0 idle      (1000) idle      (1000)     3138 2023-05-19 12:17:15.000000 pytest-djangoapp-1.2.0/CHANGELOG
+-rw-r--r--   0 idle      (1000) idle      (1000)      506 2018-06-14 13:30:02.000000 pytest-djangoapp-1.2.0/INSTALL
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1509 2023-03-18 09:27:40.000000 pytest-djangoapp-1.2.0/LICENSE
+-rw-r--r--   0 idle      (1000) idle      (1000)      280 2018-06-14 13:30:02.000000 pytest-djangoapp-1.2.0/MANIFEST.in
+-rw-rw-r--   0 idle      (1000) idle      (1000)     4349 2023-05-19 12:17:21.668973 pytest-djangoapp-1.2.0/PKG-INFO
+-rw-rw-r--   0 idle      (1000) idle      (1000)     3300 2023-05-19 05:00:23.000000 pytest-djangoapp-1.2.0/README.rst
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:17:21.660973 pytest-djangoapp-1.2.0/docs/
+-rw-rw-r--   0 idle      (1000) idle      (1000)     4635 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/docs/Makefile
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:17:21.664973 pytest-djangoapp-1.2.0/docs/source/
+-rw-rw-r--   0 idle      (1000) idle      (1000)     7737 2023-05-19 12:12:39.000000 pytest-djangoapp-1.2.0/docs/source/conf.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      365 2023-05-19 03:30:31.000000 pytest-djangoapp-1.2.0/docs/source/fixtures.rst
+-rw-rw-r--   0 idle      (1000) idle      (1000)      143 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/docs/source/fixtures_commands.rst
+-rw-rw-r--   0 idle      (1000) idle      (1000)      161 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/docs/source/fixtures_db.rst
+-rw-rw-r--   0 idle      (1000) idle      (1000)      205 2023-05-19 12:14:40.000000 pytest-djangoapp-1.2.0/docs/source/fixtures_live.rst
+-rw-rw-r--   0 idle      (1000) idle      (1000)      126 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/docs/source/fixtures_mail.rst
+-rw-rw-r--   0 idle      (1000) idle      (1000)      132 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/docs/source/fixtures_messages.rst
+-rw-rw-r--   0 idle      (1000) idle      (1000)      147 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/docs/source/fixtures_migrations.rst
+-rw-rw-r--   0 idle      (1000) idle      (1000)      136 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/docs/source/fixtures_request.rst
+-rw-rw-r--   0 idle      (1000) idle      (1000)      145 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/docs/source/fixtures_settings.rst
+-rw-rw-r--   0 idle      (1000) idle      (1000)      143 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/docs/source/fixtures_templates.rst
+-rw-rw-r--   0 idle      (1000) idle      (1000)      120 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/docs/source/fixtures_users.rst
+-rw-rw-r--   0 idle      (1000) idle      (1000)      109 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/docs/source/fixtures_utils.rst
+-rw-rw-r--   0 idle      (1000) idle      (1000)      716 2023-05-19 05:00:23.000000 pytest-djangoapp-1.2.0/docs/source/index.rst
+-rw-rw-r--   0 idle      (1000) idle      (1000)     4318 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/docs/source/quickstart.rst
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1389 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/docs/source/rst_guide.rst
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:17:21.664973 pytest-djangoapp-1.2.0/pytest_djangoapp/
+-rw-rw-r--   0 idle      (1000) idle      (1000)      193 2023-05-19 12:17:15.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/__init__.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      438 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/compat.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)     9259 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/configuration.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:17:21.664973 pytest-djangoapp-1.2.0/pytest_djangoapp/fixtures/
+-rw-rw-r--   0 idle      (1000) idle      (1000)      537 2023-05-19 04:25:26.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/fixtures/__init__.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1828 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/fixtures/commands.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)     3264 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/fixtures/db.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)     3347 2023-05-19 11:29:56.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/fixtures/live.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      368 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/fixtures/mail.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1462 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/fixtures/messages.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      706 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/fixtures/migrations.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)     5452 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/fixtures/request.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)     2555 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/fixtures/settings.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)     4273 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/fixtures/templates.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)     2117 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/fixtures/users.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      363 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/fixtures/utils.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1059 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/plugin.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:17:21.664973 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/
+-rw-rw-r--   0 idle      (1000) idle      (1000)        0 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/__init__.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      643 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/conftest.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      163 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/settings_project.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      805 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/test_configuration.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      678 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/test_etc.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      521 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/test_fixtures_commands.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      770 2023-05-19 11:31:10.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/test_fixtures_live.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      309 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/test_fixtures_mail.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      447 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/test_fixtures_messages.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      892 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/test_fixtures_migrations.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1399 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/test_fixtures_request.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)     2442 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/test_fixtures_settings.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      678 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/test_fixtures_templates.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      326 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/test_fixtures_users.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)       88 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/test_fixtures_utils.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      599 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/test_models.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:17:21.664973 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/testapp/
+-rw-rw-r--   0 idle      (1000) idle      (1000)        0 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/testapp/__init__.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:17:21.664973 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/testapp/management/
+-rw-rw-r--   0 idle      (1000) idle      (1000)        0 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/testapp/management/__init__.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:17:21.668973 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/testapp/management/commands/
+-rw-rw-r--   0 idle      (1000) idle      (1000)        0 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/testapp/management/commands/__init__.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      735 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/testapp/management/commands/compat.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      616 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/testapp/management/commands/my_command.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:17:21.668973 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/testapp/migrations/
+-rw-rw-r--   0 idle      (1000) idle      (1000)      489 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/testapp/migrations/0001_initial.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)        0 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/testapp/migrations/__init__.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      106 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/testapp/models.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      829 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/testapp/urls.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:17:21.668973 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/testapp_missing_migrations/
+-rw-rw-r--   0 idle      (1000) idle      (1000)        0 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/testapp_missing_migrations/__init__.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:17:21.668973 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/testapp_missing_migrations/migrations/
+-rw-rw-r--   0 idle      (1000) idle      (1000)        0 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/testapp_missing_migrations/migrations/__init__.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      106 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/tests/testapp_missing_migrations/models.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)     3075 2023-03-18 10:20:24.000000 pytest-djangoapp-1.2.0/pytest_djangoapp/toolbox.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:17:21.664973 pytest-djangoapp-1.2.0/pytest_djangoapp.egg-info/
+-rw-rw-r--   0 idle      (1000) idle      (1000)     4349 2023-05-19 12:17:21.000000 pytest-djangoapp-1.2.0/pytest_djangoapp.egg-info/PKG-INFO
+-rw-rw-r--   0 idle      (1000) idle      (1000)     2768 2023-05-19 12:17:21.000000 pytest-djangoapp-1.2.0/pytest_djangoapp.egg-info/SOURCES.txt
+-rw-rw-r--   0 idle      (1000) idle      (1000)        1 2023-05-19 12:17:21.000000 pytest-djangoapp-1.2.0/pytest_djangoapp.egg-info/dependency_links.txt
+-rw-rw-r--   0 idle      (1000) idle      (1000)        1 2021-08-02 11:34:48.000000 pytest-djangoapp-1.2.0/pytest_djangoapp.egg-info/not-zip-safe
+-rw-rw-r--   0 idle      (1000) idle      (1000)        7 2023-05-19 12:17:21.000000 pytest-djangoapp-1.2.0/pytest_djangoapp.egg-info/requires.txt
+-rw-rw-r--   0 idle      (1000) idle      (1000)       17 2023-05-19 12:17:21.000000 pytest-djangoapp-1.2.0/pytest_djangoapp.egg-info/top_level.txt
+-rw-r--r--   0 idle      (1000) idle      (1000)      110 2023-05-19 12:17:21.668973 pytest-djangoapp-1.2.0/setup.cfg
+-rw-rw-r--   0 idle      (1000) idle      (1000)     2239 2023-03-18 10:10:57.000000 pytest-djangoapp-1.2.0/setup.py
```

### Comparing `pytest-djangoapp-1.1.0/CHANGELOG` & `pytest-djangoapp-1.2.0/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 pytest-djangoapp changelog
 ==========================
 
 
+v1.2.0 [2023-05-19]
+-------------------
++ Add 'liveserver' and 'liveclient' fixtures (closes #24).
+
+
 v1.1.0 [2023-03-18]
 -------------------
 + Added 'command_makemigrations' fixture.
 + Added 'conf_app_name' fixture (see #17).
 + Fixture 'template_context' now accepts a username.
```

### Comparing `pytest-djangoapp-1.1.0/LICENSE` & `pytest-djangoapp-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/PKG-INFO` & `pytest-djangoapp-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-djangoapp
-Version: 1.1.0
+Version: 1.2.0
 Summary: Nice pytest plugin to help you with Django pluggable application testing.
 Home-page: https://github.com/idlesign/pytest-djangoapp
 Author: Igor `idle sign` Starikov
 Author-email: idlesign@yandex.ru
 License: BSD 3-Clause License
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -53,14 +53,15 @@
 * User creation
 * Request object creation
 * Management command calls
 * Mailing
 * Migrations
 * Messages
 * DB queries audit
+* Live server & client UI testing
 * etc.
 
 Suitable for testing apps for Django 1.8+.
 
 
 How to use
 ----------
```

### Comparing `pytest-djangoapp-1.1.0/README.rst` & `pytest-djangoapp-1.2.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 * User creation
 * Request object creation
 * Management command calls
 * Mailing
 * Migrations
 * Messages
 * DB queries audit
+* Live server & client UI testing
 * etc.
 
 Suitable for testing apps for Django 1.8+.
 
 
 How to use
 ----------
```

### Comparing `pytest-djangoapp-1.1.0/docs/Makefile` & `pytest-djangoapp-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/docs/source/conf.py` & `pytest-djangoapp-1.2.0/docs/source/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,45 +19,27 @@
 from pytest_djangoapp import VERSION
 
 # -- Mocking ------------------------------------------------------------------
 
 # This is used to mock certain modules.
 # It helps to build docs in environments where those modules are not available.
 # E.g. it could be useful for http://readthedocs.org/
-MODULES_TO_MOCK = []
+MODULES_TO_MOCK = [
+    'django.conf',
+    'django.conf.settings',
+    'django.conf.locale',
+]
 
 
 if MODULES_TO_MOCK:
 
-    class ModuleMock(object):
-
-        __all__ = []
-
-        def __init__(self, *args, **kwargs):
-            pass
-
-        def __call__(self, *args, **kwargs):
-            return ModuleMock()
-
-        def __iter__(self):
-            return iter([])
-
-        @classmethod
-        def __getattr__(cls, name):
-            if name in ('__file__', '__path__'):
-                return '/dev/null'
-            elif name.upper() != name and name[0] == name[0].upper():
-                # Mock classes.
-                MockType = type(name, (ModuleMock,), {})
-                MockType.__module__ = __name__
-                return MockType
-            return ModuleMock()
+    from unittest.mock import MagicMock
 
     for mod_name in MODULES_TO_MOCK:
-        sys.modules[mod_name] = ModuleMock()
+        sys.modules[mod_name] = MagicMock()
 
 
 # -- General configuration -----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #needs_sphinx = '1.0'
```

### Comparing `pytest-djangoapp-1.1.0/docs/source/index.rst` & `pytest-djangoapp-1.2.0/docs/source/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 * User creation
 * Request object creation
 * Management command calls
 * Mailing
 * Migrations
 * Messages
 * DB queries audit
+* Live server & client UI testing
 * etc.
 
 Suitable for testing apps for Django 1.8+.
 
 
 Requirements
 ------------
```

### Comparing `pytest-djangoapp-1.1.0/docs/source/quickstart.rst` & `pytest-djangoapp-1.2.0/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/docs/source/rst_guide.rst` & `pytest-djangoapp-1.2.0/docs/source/rst_guide.rst`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/pytest_djangoapp/configuration.py` & `pytest-djangoapp-1.2.0/pytest_djangoapp/configuration.py`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/pytest_djangoapp/fixtures/commands.py` & `pytest-djangoapp-1.2.0/pytest_djangoapp/fixtures/commands.py`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/pytest_djangoapp/fixtures/db.py` & `pytest-djangoapp-1.2.0/pytest_djangoapp/fixtures/db.py`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/pytest_djangoapp/fixtures/messages.py` & `pytest-djangoapp-1.2.0/pytest_djangoapp/fixtures/messages.py`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/pytest_djangoapp/fixtures/migrations.py` & `pytest-djangoapp-1.2.0/pytest_djangoapp/fixtures/migrations.py`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/pytest_djangoapp/fixtures/request.py` & `pytest-djangoapp-1.2.0/pytest_djangoapp/fixtures/request.py`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/pytest_djangoapp/fixtures/settings.py` & `pytest-djangoapp-1.2.0/pytest_djangoapp/fixtures/settings.py`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/pytest_djangoapp/fixtures/templates.py` & `pytest-djangoapp-1.2.0/pytest_djangoapp/fixtures/templates.py`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/pytest_djangoapp/fixtures/users.py` & `pytest-djangoapp-1.2.0/pytest_djangoapp/fixtures/users.py`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/pytest_djangoapp/plugin.py` & `pytest-djangoapp-1.2.0/pytest_djangoapp/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/pytest_djangoapp/tests/conftest.py` & `pytest-djangoapp-1.2.0/pytest_djangoapp/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/pytest_djangoapp/tests/test_configuration.py` & `pytest-djangoapp-1.2.0/pytest_djangoapp/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/pytest_djangoapp/tests/test_etc.py` & `pytest-djangoapp-1.2.0/pytest_djangoapp/tests/test_etc.py`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/pytest_djangoapp/tests/test_fixtures_commands.py` & `pytest-djangoapp-1.2.0/pytest_djangoapp/tests/test_fixtures_commands.py`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/pytest_djangoapp/tests/test_fixtures_migrations.py` & `pytest-djangoapp-1.2.0/pytest_djangoapp/tests/test_fixtures_migrations.py`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/pytest_djangoapp/tests/test_fixtures_request.py` & `pytest-djangoapp-1.2.0/pytest_djangoapp/tests/test_fixtures_request.py`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/pytest_djangoapp/tests/test_fixtures_settings.py` & `pytest-djangoapp-1.2.0/pytest_djangoapp/tests/test_fixtures_settings.py`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/pytest_djangoapp/tests/test_fixtures_templates.py` & `pytest-djangoapp-1.2.0/pytest_djangoapp/tests/test_fixtures_templates.py`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/pytest_djangoapp/tests/test_models.py` & `pytest-djangoapp-1.2.0/pytest_djangoapp/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/pytest_djangoapp/tests/testapp/management/commands/compat.py` & `pytest-djangoapp-1.2.0/pytest_djangoapp/tests/testapp/management/commands/compat.py`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/pytest_djangoapp/tests/testapp/management/commands/my_command.py` & `pytest-djangoapp-1.2.0/pytest_djangoapp/tests/testapp/management/commands/my_command.py`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/pytest_djangoapp/tests/testapp/urls.py` & `pytest-djangoapp-1.2.0/pytest_djangoapp/tests/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/pytest_djangoapp/toolbox.py` & `pytest-djangoapp-1.2.0/pytest_djangoapp/toolbox.py`

 * *Files identical despite different names*

### Comparing `pytest-djangoapp-1.1.0/pytest_djangoapp.egg-info/PKG-INFO` & `pytest-djangoapp-1.2.0/pytest_djangoapp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-djangoapp
-Version: 1.1.0
+Version: 1.2.0
 Summary: Nice pytest plugin to help you with Django pluggable application testing.
 Home-page: https://github.com/idlesign/pytest-djangoapp
 Author: Igor `idle sign` Starikov
 Author-email: idlesign@yandex.ru
 License: BSD 3-Clause License
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -53,14 +53,15 @@
 * User creation
 * Request object creation
 * Management command calls
 * Mailing
 * Migrations
 * Messages
 * DB queries audit
+* Live server & client UI testing
 * etc.
 
 Suitable for testing apps for Django 1.8+.
 
 
 How to use
 ----------
```

### Comparing `pytest-djangoapp-1.1.0/pytest_djangoapp.egg-info/SOURCES.txt` & `pytest-djangoapp-1.2.0/pytest_djangoapp.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 setup.cfg
 setup.py
 docs/Makefile
 docs/source/conf.py
 docs/source/fixtures.rst
 docs/source/fixtures_commands.rst
 docs/source/fixtures_db.rst
+docs/source/fixtures_live.rst
 docs/source/fixtures_mail.rst
 docs/source/fixtures_messages.rst
 docs/source/fixtures_migrations.rst
 docs/source/fixtures_request.rst
 docs/source/fixtures_settings.rst
 docs/source/fixtures_templates.rst
 docs/source/fixtures_users.rst
@@ -32,28 +33,30 @@
 pytest_djangoapp.egg-info/dependency_links.txt
 pytest_djangoapp.egg-info/not-zip-safe
 pytest_djangoapp.egg-info/requires.txt
 pytest_djangoapp.egg-info/top_level.txt
 pytest_djangoapp/fixtures/__init__.py
 pytest_djangoapp/fixtures/commands.py
 pytest_djangoapp/fixtures/db.py
+pytest_djangoapp/fixtures/live.py
 pytest_djangoapp/fixtures/mail.py
 pytest_djangoapp/fixtures/messages.py
 pytest_djangoapp/fixtures/migrations.py
 pytest_djangoapp/fixtures/request.py
 pytest_djangoapp/fixtures/settings.py
 pytest_djangoapp/fixtures/templates.py
 pytest_djangoapp/fixtures/users.py
 pytest_djangoapp/fixtures/utils.py
 pytest_djangoapp/tests/__init__.py
 pytest_djangoapp/tests/conftest.py
 pytest_djangoapp/tests/settings_project.py
 pytest_djangoapp/tests/test_configuration.py
 pytest_djangoapp/tests/test_etc.py
 pytest_djangoapp/tests/test_fixtures_commands.py
+pytest_djangoapp/tests/test_fixtures_live.py
 pytest_djangoapp/tests/test_fixtures_mail.py
 pytest_djangoapp/tests/test_fixtures_messages.py
 pytest_djangoapp/tests/test_fixtures_migrations.py
 pytest_djangoapp/tests/test_fixtures_request.py
 pytest_djangoapp/tests/test_fixtures_settings.py
 pytest_djangoapp/tests/test_fixtures_templates.py
 pytest_djangoapp/tests/test_fixtures_users.py
```

### Comparing `pytest-djangoapp-1.1.0/setup.py` & `pytest-djangoapp-1.2.0/setup.py`

 * *Files identical despite different names*

