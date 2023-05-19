# Comparing `tmp/zgrobot-2.0.4.tar.gz` & `tmp/zgrobot-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zgrobot-2.0.4.tar", last modified: Sun Mar  5 13:26:36 2023, max compression
+gzip compressed data, was "zgrobot-2.0.5.tar", last modified: Fri May 19 06:40:13 2023, max compression
```

## Comparing `zgrobot-2.0.4.tar` & `zgrobot-2.0.5.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 13:26:36.554393 zgrobot-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-03-05 13:26:26.000000 zgrobot-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-05 13:26:26.000000 zgrobot-2.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-03-05 13:26:36.554393 zgrobot-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-03-05 13:26:26.000000 zgrobot-2.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-05 13:26:26.000000 zgrobot-2.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-05 13:26:36.554393 zgrobot-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-03-05 13:26:26.000000 zgrobot-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 13:26:36.542393 zgrobot-2.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-05 13:26:26.000000 zgrobot-2.0.4/tests/client_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 13:26:36.542393 zgrobot-2.0.4/tests/django_test_env/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 13:26:36.542393 zgrobot-2.0.4/tests/django_test_env/django_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 13:26:26.000000 zgrobot-2.0.4/tests/django_test_env/django_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-03-05 13:26:26.000000 zgrobot-2.0.4/tests/django_test_env/django_test/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-03-05 13:26:26.000000 zgrobot-2.0.4/tests/django_test_env/django_test/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-05 13:26:26.000000 zgrobot-2.0.4/tests/django_test_env/django_test/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-05 13:26:26.000000 zgrobot-2.0.4/tests/django_test_env/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 13:26:36.546393 zgrobot-2.0.4/tests/media/
--rw-r--r--   0 runner    (1001) docker     (123)   592422 2023-03-05 13:26:26.000000 zgrobot-2.0.4/tests/media/123.png
--rw-r--r--   0 runner    (1001) docker     (123)   590398 2023-03-05 13:26:26.000000 zgrobot-2.0.4/tests/media/234.pngw
--rw-r--r--   0 runner    (1001) docker     (123)  1249842 2023-03-05 13:26:26.000000 zgrobot-2.0.4/tests/media/456.mp4
--rw-r--r--   0 runner    (1001) docker     (123)   245795 2023-03-05 13:26:26.000000 zgrobot-2.0.4/tests/media/track1.mp3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 13:26:36.546393 zgrobot-2.0.4/tests/messages/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-03-05 13:26:26.000000 zgrobot-2.0.4/tests/messages/test_entries.py
--rw-r--r--   0 runner    (1001) docker     (123)    69072 2023-03-05 13:26:26.000000 zgrobot-2.0.4/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-05 13:26:26.000000 zgrobot-2.0.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-03-05 13:26:26.000000 zgrobot-2.0.4/tests/test_contrib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-05 13:26:26.000000 zgrobot-2.0.4/tests/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)    32519 2023-03-05 13:26:26.000000 zgrobot-2.0.4/tests/test_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-05 13:26:26.000000 zgrobot-2.0.4/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    36151 2023-03-05 13:26:26.000000 zgrobot-2.0.4/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-03-05 13:26:26.000000 zgrobot-2.0.4/tests/test_replies.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-03-05 13:26:26.000000 zgrobot-2.0.4/tests/test_robot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-03-05 13:26:26.000000 zgrobot-2.0.4/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-03-05 13:26:26.000000 zgrobot-2.0.4/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 13:26:36.550393 zgrobot-2.0.4/zgrobot/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43523 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 13:26:36.550393 zgrobot-2.0.4/zgrobot/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/contrib/bottle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/contrib/django.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/contrib/error.html
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/contrib/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/contrib/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/contrib/tornado.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 13:26:36.550393 zgrobot-2.0.4/zgrobot/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/crypto/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/crypto/pkcs7.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 13:26:36.550393 zgrobot-2.0.4/zgrobot/messages/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/messages/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/messages/entries.py
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/messages/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/messages/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/pay.py
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/replies.py
--rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/robot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 13:26:36.554393 zgrobot-2.0.4/zgrobot/session/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/session/filestorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/session/mongodbstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/session/mysqlstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/session/postgresqlstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/session/redisstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/session/saekvstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/session/sqlitestorage.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-03-05 13:26:26.000000 zgrobot-2.0.4/zgrobot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 13:26:36.550393 zgrobot-2.0.4/zgrobot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-03-05 13:26:36.000000 zgrobot-2.0.4/zgrobot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-03-05 13:26:36.000000 zgrobot-2.0.4/zgrobot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 13:26:36.000000 zgrobot-2.0.4/zgrobot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-05 13:26:36.000000 zgrobot-2.0.4/zgrobot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-05 13:26:36.000000 zgrobot-2.0.4/zgrobot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:40:13.471846 zgrobot-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-19 06:39:57.000000 zgrobot-2.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-19 06:39:57.000000 zgrobot-2.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-19 06:40:13.471846 zgrobot-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-19 06:39:57.000000 zgrobot-2.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-19 06:39:57.000000 zgrobot-2.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-19 06:40:13.471846 zgrobot-2.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-19 06:39:57.000000 zgrobot-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:40:13.463846 zgrobot-2.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-19 06:39:57.000000 zgrobot-2.0.5/tests/client_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:40:13.463846 zgrobot-2.0.5/tests/django_test_env/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:40:13.463846 zgrobot-2.0.5/tests/django_test_env/django_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:39:57.000000 zgrobot-2.0.5/tests/django_test_env/django_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-19 06:39:57.000000 zgrobot-2.0.5/tests/django_test_env/django_test/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-19 06:39:57.000000 zgrobot-2.0.5/tests/django_test_env/django_test/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-19 06:39:57.000000 zgrobot-2.0.5/tests/django_test_env/django_test/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-19 06:39:57.000000 zgrobot-2.0.5/tests/django_test_env/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:40:13.467846 zgrobot-2.0.5/tests/media/
+-rw-r--r--   0 runner    (1001) docker     (123)   593346 2023-05-19 06:39:57.000000 zgrobot-2.0.5/tests/media/123.png
+-rw-r--r--   0 runner    (1001) docker     (123)   590398 2023-05-19 06:39:57.000000 zgrobot-2.0.5/tests/media/234.pngw
+-rw-r--r--   0 runner    (1001) docker     (123)  1249842 2023-05-19 06:39:57.000000 zgrobot-2.0.5/tests/media/456.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)   245795 2023-05-19 06:39:57.000000 zgrobot-2.0.5/tests/media/track1.mp3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:40:13.467846 zgrobot-2.0.5/tests/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-19 06:39:57.000000 zgrobot-2.0.5/tests/messages/test_entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69072 2023-05-19 06:39:57.000000 zgrobot-2.0.5/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-19 06:39:57.000000 zgrobot-2.0.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10456 2023-05-19 06:39:57.000000 zgrobot-2.0.5/tests/test_contrib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-19 06:39:57.000000 zgrobot-2.0.5/tests/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32519 2023-05-19 06:39:57.000000 zgrobot-2.0.5/tests/test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-19 06:39:57.000000 zgrobot-2.0.5/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36151 2023-05-19 06:39:57.000000 zgrobot-2.0.5/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-05-19 06:39:57.000000 zgrobot-2.0.5/tests/test_replies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-05-19 06:39:57.000000 zgrobot-2.0.5/tests/test_robot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-19 06:39:57.000000 zgrobot-2.0.5/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-19 06:39:57.000000 zgrobot-2.0.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:40:13.467846 zgrobot-2.0.5/zgrobot/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43523 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:40:13.471846 zgrobot-2.0.5/zgrobot/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/contrib/bottle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/contrib/django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/contrib/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/contrib/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/contrib/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/contrib/tornado.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:40:13.471846 zgrobot-2.0.5/zgrobot/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/crypto/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/crypto/pkcs7.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:40:13.471846 zgrobot-2.0.5/zgrobot/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/messages/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/messages/entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/messages/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/messages/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/pay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/replies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23093 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/robot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:40:13.471846 zgrobot-2.0.5/zgrobot/session/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/session/filestorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/session/mongodbstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/session/mysqlstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/session/postgresqlstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/session/redisstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/session/saekvstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/session/sqlitestorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-05-19 06:39:57.000000 zgrobot-2.0.5/zgrobot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:40:13.471846 zgrobot-2.0.5/zgrobot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-19 06:40:13.000000 zgrobot-2.0.5/zgrobot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-19 06:40:13.000000 zgrobot-2.0.5/zgrobot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 06:40:13.000000 zgrobot-2.0.5/zgrobot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-19 06:40:13.000000 zgrobot-2.0.5/zgrobot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-19 06:40:13.000000 zgrobot-2.0.5/zgrobot.egg-info/top_level.txt
```

### Comparing `zgrobot-2.0.4/LICENSE` & `zgrobot-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/PKG-INFO` & `zgrobot-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zgrobot
-Version: 2.0.4
+Version: 2.0.5
 Summary: ZgRoBot: writing WeChat Offical Account Robots with fun
 Home-page: https://github.com/pylover7/ZgRobot
 Author: pylover
 Author-email: shuoshuoyun@foxmail.com
 License: MIT License
 Project-URL: Documentation, https://zgrobot.readthedocs.io/zh/stable/
 Project-URL: Source, https://github.com/pylover7/ZgRobot
```

### Comparing `zgrobot-2.0.4/README.md` & `zgrobot-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/setup.py` & `zgrobot-2.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/tests/django_test_env/django_test/settings.py` & `zgrobot-2.0.5/tests/django_test_env/django_test/settings.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/tests/django_test_env/django_test/urls.py` & `zgrobot-2.0.5/tests/django_test_env/django_test/urls.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/tests/media/123.png` & `zgrobot-2.0.5/tests/media/123.png`

 * *Format-specific differences are supported for PNG images but no file-specific differences were detected; falling back to a binary diff. file(1) reports: PNG image data, 742 x 519, 8-bit/color RGBA, non-interlaced*

 * *Files 4% similar despite different names*

```diff
@@ -37020,8 +37020,66 @@
 000909b0: 7420 6120 7465 7374 6a75 7374 2061 2074  t a testjust a t
 000909c0: 6573 746a 7573 7420 6120 7465 7374 6a75  estjust a testju
 000909d0: 7374 2061 2074 6573 746a 7573 7420 6120  st a testjust a 
 000909e0: 7465 7374 6a75 7374 2061 2074 6573 746a  testjust a testj
 000909f0: 7573 7420 6120 7465 7374 6a75 7374 2061  ust a testjust a
 00090a00: 2074 6573 746a 7573 7420 6120 7465 7374   testjust a test
 00090a10: 6a75 7374 2061 2074 6573 746a 7573 7420  just a testjust 
-00090a20: 6120 7465 7374                           a test
+00090a20: 6120 7465 7374 6a75 7374 2061 2074 6573  a testjust a tes
+00090a30: 746a 7573 7420 6120 7465 7374 6a75 7374  tjust a testjust
+00090a40: 2061 2074 6573 746a 7573 7420 6120 7465   a testjust a te
+00090a50: 7374 6a75 7374 2061 2074 6573 746a 7573  stjust a testjus
+00090a60: 7420 6120 7465 7374 6a75 7374 2061 2074  t a testjust a t
+00090a70: 6573 746a 7573 7420 6120 7465 7374 6a75  estjust a testju
+00090a80: 7374 2061 2074 6573 746a 7573 7420 6120  st a testjust a 
+00090a90: 7465 7374 6a75 7374 2061 2074 6573 746a  testjust a testj
+00090aa0: 7573 7420 6120 7465 7374 6a75 7374 2061  ust a testjust a
+00090ab0: 2074 6573 746a 7573 7420 6120 7465 7374   testjust a test
+00090ac0: 6a75 7374 2061 2074 6573 746a 7573 7420  just a testjust 
+00090ad0: 6120 7465 7374 6a75 7374 2061 2074 6573  a testjust a tes
+00090ae0: 746a 7573 7420 6120 7465 7374 6a75 7374  tjust a testjust
+00090af0: 2061 2074 6573 746a 7573 7420 6120 7465   a testjust a te
+00090b00: 7374 6a75 7374 2061 2074 6573 746a 7573  stjust a testjus
+00090b10: 7420 6120 7465 7374 6a75 7374 2061 2074  t a testjust a t
+00090b20: 6573 746a 7573 7420 6120 7465 7374 6a75  estjust a testju
+00090b30: 7374 2061 2074 6573 746a 7573 7420 6120  st a testjust a 
+00090b40: 7465 7374 6a75 7374 2061 2074 6573 746a  testjust a testj
+00090b50: 7573 7420 6120 7465 7374 6a75 7374 2061  ust a testjust a
+00090b60: 2074 6573 746a 7573 7420 6120 7465 7374   testjust a test
+00090b70: 6a75 7374 2061 2074 6573 746a 7573 7420  just a testjust 
+00090b80: 6120 7465 7374 6a75 7374 2061 2074 6573  a testjust a tes
+00090b90: 746a 7573 7420 6120 7465 7374 6a75 7374  tjust a testjust
+00090ba0: 2061 2074 6573 746a 7573 7420 6120 7465   a testjust a te
+00090bb0: 7374 6a75 7374 2061 2074 6573 746a 7573  stjust a testjus
+00090bc0: 7420 6120 7465 7374 6a75 7374 2061 2074  t a testjust a t
+00090bd0: 6573 746a 7573 7420 6120 7465 7374 6a75  estjust a testju
+00090be0: 7374 2061 2074 6573 746a 7573 7420 6120  st a testjust a 
+00090bf0: 7465 7374 6a75 7374 2061 2074 6573 746a  testjust a testj
+00090c00: 7573 7420 6120 7465 7374 6a75 7374 2061  ust a testjust a
+00090c10: 2074 6573 746a 7573 7420 6120 7465 7374   testjust a test
+00090c20: 6a75 7374 2061 2074 6573 746a 7573 7420  just a testjust 
+00090c30: 6120 7465 7374 6a75 7374 2061 2074 6573  a testjust a tes
+00090c40: 746a 7573 7420 6120 7465 7374 6a75 7374  tjust a testjust
+00090c50: 2061 2074 6573 746a 7573 7420 6120 7465   a testjust a te
+00090c60: 7374 6a75 7374 2061 2074 6573 746a 7573  stjust a testjus
+00090c70: 7420 6120 7465 7374 6a75 7374 2061 2074  t a testjust a t
+00090c80: 6573 746a 7573 7420 6120 7465 7374 6a75  estjust a testju
+00090c90: 7374 2061 2074 6573 746a 7573 7420 6120  st a testjust a 
+00090ca0: 7465 7374 6a75 7374 2061 2074 6573 746a  testjust a testj
+00090cb0: 7573 7420 6120 7465 7374 6a75 7374 2061  ust a testjust a
+00090cc0: 2074 6573 746a 7573 7420 6120 7465 7374   testjust a test
+00090cd0: 6a75 7374 2061 2074 6573 746a 7573 7420  just a testjust 
+00090ce0: 6120 7465 7374 6a75 7374 2061 2074 6573  a testjust a tes
+00090cf0: 746a 7573 7420 6120 7465 7374 6a75 7374  tjust a testjust
+00090d00: 2061 2074 6573 746a 7573 7420 6120 7465   a testjust a te
+00090d10: 7374 6a75 7374 2061 2074 6573 746a 7573  stjust a testjus
+00090d20: 7420 6120 7465 7374 6a75 7374 2061 2074  t a testjust a t
+00090d30: 6573 746a 7573 7420 6120 7465 7374 6a75  estjust a testju
+00090d40: 7374 2061 2074 6573 746a 7573 7420 6120  st a testjust a 
+00090d50: 7465 7374 6a75 7374 2061 2074 6573 746a  testjust a testj
+00090d60: 7573 7420 6120 7465 7374 6a75 7374 2061  ust a testjust a
+00090d70: 2074 6573 746a 7573 7420 6120 7465 7374   testjust a test
+00090d80: 6a75 7374 2061 2074 6573 746a 7573 7420  just a testjust 
+00090d90: 6120 7465 7374 6a75 7374 2061 2074 6573  a testjust a tes
+00090da0: 746a 7573 7420 6120 7465 7374 6a75 7374  tjust a testjust
+00090db0: 2061 2074 6573 746a 7573 7420 6120 7465   a testjust a te
+00090dc0: 7374                                     st
```

### Comparing `zgrobot-2.0.4/tests/media/234.pngw` & `zgrobot-2.0.5/tests/media/234.pngw`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/tests/media/456.mp4` & `zgrobot-2.0.5/tests/media/456.mp4`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/tests/media/track1.mp3` & `zgrobot-2.0.5/tests/media/track1.mp3`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/tests/messages/test_entries.py` & `zgrobot-2.0.5/tests/messages/test_entries.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/tests/test_client.py` & `zgrobot-2.0.5/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/tests/test_config.py` & `zgrobot-2.0.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/tests/test_contrib.py` & `zgrobot-2.0.5/tests/test_contrib.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,15 @@
         "/", make_view(robot=hello_robot), methods=["GET", "POST"]
     )
 
     token = generate_token()
     hello_robot.token = token
     timestamp = str(time.time())
     nonce = str(random.randint(0, 10000))
+    echostr = str(random.randint(0, 10000))
     signature = get_signature(token, timestamp, nonce)
 
     response = client.post(
         url="/",
         params=f"timestamp={timestamp}&nonce={nonce}&signature={signature}",
         data="""<xml>
                                         <ToUserName><![CDATA[123]]></ToUserName>
@@ -121,14 +122,21 @@
     assert response.content.decode('utf-8') == u'喵'
 
     response = client.options("/")
     assert response.status_code == 405
     assert eval(response.content.decode('utf-8')
                 )["detail"] == "Method Not Allowed"
 
+    response = client.get(
+        url="/",
+        params=
+        f"timestamp={timestamp}&nonce={nonce}&signature={signature}&echostr={echostr}"
+    )
+    assert response.content.decode('utf-8') == echostr
+
 
 def test_django():
     os.environ.setdefault("DJANGO_SETTINGS_MODULE", "django_test.settings")
     sys.path.append(
         os.path.join(
             os.path.abspath(os.path.dirname(__file__)), 'django_test_env'
         )
```

### Comparing `zgrobot-2.0.4/tests/test_crypto.py` & `zgrobot-2.0.5/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/tests/test_handler.py` & `zgrobot-2.0.5/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/tests/test_logger.py` & `zgrobot-2.0.5/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/tests/test_parser.py` & `zgrobot-2.0.5/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/tests/test_replies.py` & `zgrobot-2.0.5/tests/test_replies.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/tests/test_robot.py` & `zgrobot-2.0.5/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/tests/test_session.py` & `zgrobot-2.0.5/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/tests/test_utils.py` & `zgrobot-2.0.5/tests/test_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import os
 import re
-import time
 
-from zgrobot.utils import check_file_type_and_size, str2button, exit_after
+from zgrobot.utils import check_file_type_and_size, str2button
 from zgrobot.utils import generate_token, check_token, to_text, to_binary
 from zgrobot.utils import pay_sign_dict, make_error_page, is_regex
 
 
 def test_token_generator():
     assert not check_token('AA C')
     assert check_token(generate_token())
@@ -89,23 +88,7 @@
             ), "rb"
         )
     )
 
 
 def test_str2button():
     assert type(str2button(button_txt="123", reply_txt="456")) is str
-
-
-def test_exit_after():
-    def timeout_func(s: int):
-        @exit_after()
-        def handle():
-            time.sleep(s)
-            return "false"
-
-        try:
-            return handle()
-        except KeyboardInterrupt:
-            return "true"
-
-    assert timeout_func(1) == "false"
-    assert timeout_func(6) == "true"
```

### Comparing `zgrobot-2.0.4/zgrobot/client.py` & `zgrobot-2.0.5/zgrobot/client.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/zgrobot/config.py` & `zgrobot-2.0.5/zgrobot/config.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/zgrobot/contrib/bottle.py` & `zgrobot-2.0.5/zgrobot/contrib/bottle.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/zgrobot/contrib/django.py` & `zgrobot-2.0.5/zgrobot/contrib/django.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/zgrobot/contrib/error.html` & `zgrobot-2.0.5/zgrobot/contrib/error.html`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     <body>
         <img
             src="https://cdn.rawgit.com/whtsky/ZgRoBot/master/artwork/logo.svg"
             alt=""
         />
         <h1>
             这是一个
-            <a href="https://github.com/whtsky/ZgRoBot/">ZgRoBot</a> 应用
+            <a href="https://github.com/pylover7/ZgRoBot/">ZgRoBot</a> 应用
         </h1>
         <p>想要使用本机器人，请在微信后台中将 URL 设置为</p>
         <pre>{url}</pre>
         <p>并将 Token 值设置正确。</p>
         <p>更多信息请与网站所有者联系</p>
     </body>
 </html>
```

### Comparing `zgrobot-2.0.4/zgrobot/contrib/fastapi.py` & `zgrobot-2.0.5/zgrobot/contrib/fastapi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 import asyncio
 import html
 
 from fastapi import Request, Body
-from fastapi.responses import HTMLResponse, Response
+from fastapi.responses import HTMLResponse, Response, PlainTextResponse
 
 from zgrobot.robot import BaseRoBot
 
 
 def make_view(robot: BaseRoBot):
     """
     为一个 BaseRobot 生成 FastApi View。
@@ -42,15 +42,15 @@
             return HTMLResponse(
                 content=robot.make_error_page(
                     html.escape(request.url.__str__()),
                 ),
                 status_code=403
             )
         if request.method != "POST":
-            return request.path_params.get("echostr")
+            return PlainTextResponse(request.query_params.get("echostr"))
 
         message = robot.parse_message(
             body=asyncio.run(request.body()),
             timestamp=timestamp,
             nonce=nonce,
             msg_signature=request.path_params.get("msg_signature")
         )
```

### Comparing `zgrobot-2.0.4/zgrobot/contrib/flask.py` & `zgrobot-2.0.5/zgrobot/contrib/flask.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/zgrobot/contrib/tornado.py` & `zgrobot-2.0.5/zgrobot/contrib/tornado.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/zgrobot/crypto/__init__.py` & `zgrobot-2.0.5/zgrobot/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/zgrobot/logger.py` & `zgrobot-2.0.5/zgrobot/logger.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/zgrobot/messages/entries.py` & `zgrobot-2.0.5/zgrobot/messages/entries.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/zgrobot/messages/events.py` & `zgrobot-2.0.5/zgrobot/messages/events.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/zgrobot/messages/messages.py` & `zgrobot-2.0.5/zgrobot/messages/messages.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/zgrobot/parser.py` & `zgrobot-2.0.5/zgrobot/parser.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/zgrobot/pay.py` & `zgrobot-2.0.5/zgrobot/pay.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding:utf-8 -*-
 
 import time
 from functools import partial
 from hashlib import sha1, md5
-from urllib import urlencode
+from urllib.parse import urlencode
 
 from zgrobot.client import Client
 from zgrobot.utils import pay_sign_dict, generate_token
 
 NATIVE_BASE_URL = 'weixin://wxpay/bizpayurl?'
```

### Comparing `zgrobot-2.0.4/zgrobot/replies.py` & `zgrobot-2.0.5/zgrobot/replies.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/zgrobot/robot.py` & `zgrobot-2.0.5/zgrobot/robot.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from zgrobot.client import Client
 from zgrobot.config import Config, ConfigAttribute
 from zgrobot.exceptions import ConfigError
 from zgrobot.parser import parse_xml, process_message
 from zgrobot.replies import process_function_reply
 from zgrobot.utils import (
     to_binary, to_text, check_signature, make_error_page, cached_property,
-    is_regex, exit_after
+    is_regex
 )
 
 __all__ = ['BaseRoBot', 'ZgRoBot']
 
 _DEFAULT_CONFIG = dict(
     TOKEN=None,
     SERVER="auto",
@@ -567,15 +567,14 @@
                 nonce=nonce,
                 msg_signature=msg_signature,
                 encrypt_msg=message_dict["Encrypt"]
             )
             message_dict = parse_xml(xml)
         return process_message(message_dict)
 
-    @exit_after(4.5)
     def get_reply(self, message):
         """
         根据 message 的内容获取 Reply 对象。
 
         :param message: 要处理的 message
         :return: 获取的 Reply 对象
         """
@@ -592,18 +591,17 @@
             for handler, args_count in handlers:
                 args = [message, session][:args_count]
                 reply = handler(*args)
                 if session_storage and id:
                     session_storage[id] = session
                 if reply:
                     return process_function_reply(reply, message=message)
-        except KeyboardInterrupt:
-            return "success"
         except Exception as e:
             self.logger.exception(f"Catch an exception: {e}")
+            return "success"
 
     def get_encrypted_reply(self, message):
         """
         对一个指定的 ZgRoBot Message ，获取 handlers 处理后得到的 Reply。
         如果可能，对该 Reply 进行加密。
         返回 Reply Render 后的文本。
```

### Comparing `zgrobot-2.0.4/zgrobot/session/filestorage.py` & `zgrobot-2.0.5/zgrobot/session/filestorage.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/zgrobot/session/mongodbstorage.py` & `zgrobot-2.0.5/zgrobot/session/mongodbstorage.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/zgrobot/session/mysqlstorage.py` & `zgrobot-2.0.5/zgrobot/session/mysqlstorage.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/zgrobot/session/postgresqlstorage.py` & `zgrobot-2.0.5/zgrobot/session/postgresqlstorage.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/zgrobot/session/redisstorage.py` & `zgrobot-2.0.5/zgrobot/session/redisstorage.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/zgrobot/session/saekvstorage.py` & `zgrobot-2.0.5/zgrobot/session/saekvstorage.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/zgrobot/session/sqlitestorage.py` & `zgrobot-2.0.5/zgrobot/session/sqlitestorage.py`

 * *Files identical despite different names*

### Comparing `zgrobot-2.0.4/zgrobot/utils.py` & `zgrobot-2.0.5/zgrobot/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # -*- coding: utf-8 -*-
-import _thread
 import io
 import json
 import os
 import random
 import re
 import string
-import sys
-import threading
 import time
 from functools import wraps
 from hashlib import sha1
 from typing import BinaryIO
 
 try:
     from secrets import choice
@@ -186,36 +183,7 @@
     将普通文本包装为智能按钮
 
     :param button_txt: 想要转换为智能按钮的文本
     :param reply_txt: 按下智能按钮后回复的文本
     :return: 返回智能按钮的字符串
     """
     return f"<a href='weixin://bizmsgmenu?msgmenuid=1&msgmenucontent={button_txt}'>{reply_txt}</a>"
-
-
-def exit_after(second=5):
-    """
-    如果函数超过 second（5）秒，则出现 KeyboardInterrupt 异常
-    use as decorator to exit process if function takes longer than s seconds
-
-    :param: second 设置超时时间，默认为五秒
-    :return: None
-    """
-    def quit_function(fn_name):
-        # print to stderr, unbuffered in Python 2.
-        print('{0} took too long'.format(fn_name), file=sys.stderr)
-        sys.stderr.flush()  # Python 3 stderr is likely buffered.
-        _thread.interrupt_main()  # raises KeyboardInterrupt
-
-    def outer(fn):
-        def inner(*args, **kwargs):
-            timer = threading.Timer(second, quit_function, args=[fn.__name__])
-            timer.start()
-            try:
-                result = fn(*args, **kwargs)
-            finally:
-                timer.cancel()
-            return result
-
-        return inner
-
-    return outer
```

### Comparing `zgrobot-2.0.4/zgrobot.egg-info/PKG-INFO` & `zgrobot-2.0.5/zgrobot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zgrobot
-Version: 2.0.4
+Version: 2.0.5
 Summary: ZgRoBot: writing WeChat Offical Account Robots with fun
 Home-page: https://github.com/pylover7/ZgRobot
 Author: pylover
 Author-email: shuoshuoyun@foxmail.com
 License: MIT License
 Project-URL: Documentation, https://zgrobot.readthedocs.io/zh/stable/
 Project-URL: Source, https://github.com/pylover7/ZgRobot
```

### Comparing `zgrobot-2.0.4/zgrobot.egg-info/SOURCES.txt` & `zgrobot-2.0.5/zgrobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

