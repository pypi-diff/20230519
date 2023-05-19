# Comparing `tmp/makeapp-1.9.0.tar.gz` & `tmp/makeapp-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makeapp-1.9.0.tar", last modified: Sat Jan 21 05:03:05 2023, max compression
+gzip compressed data, was "makeapp-1.9.1.tar", last modified: Fri May 19 12:25:12 2023, max compression
```

## Comparing `makeapp-1.9.0.tar` & `makeapp-1.9.1.tar`

### file list

```diff
@@ -1,181 +1,181 @@
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.422195 makeapp-1.9.0/
--rw-rw-r--   0 idle      (1000) idle      (1000)      125 2014-06-07 05:37:42.000000 makeapp-1.9.0/AUTHORS
--rw-rw-r--   0 idle      (1000) idle      (1000)     6833 2023-01-21 05:02:58.000000 makeapp-1.9.0/CHANGELOG
--rw-rw-r--   0 idle      (1000) idle      (1000)      443 2016-07-21 10:53:31.000000 makeapp-1.9.0/INSTALL
--rw-rw-r--   0 idle      (1000) idle      (1000)     1499 2023-01-21 04:58:04.000000 makeapp-1.9.0/LICENSE
--rw-rw-r--   0 idle      (1000) idle      (1000)      378 2017-05-13 17:28:02.000000 makeapp-1.9.0/MANIFEST.in
--rw-rw-r--   0 idle      (1000) idle      (1000)     3902 2023-01-21 05:03:05.422195 makeapp-1.9.0/PKG-INFO
--rw-rw-r--   0 idle      (1000) idle      (1000)     3150 2021-12-18 06:21:57.000000 makeapp-1.9.0/README.rst
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.402194 makeapp-1.9.0/docs/
--rw-rw-r--   0 idle      (1000) idle      (1000)     4598 2013-12-18 16:21:05.000000 makeapp-1.9.0/docs/Makefile
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.402194 makeapp-1.9.0/docs/source/
--rw-rw-r--   0 idle      (1000) idle      (1000)     7045 2023-01-21 04:58:07.000000 makeapp-1.9.0/docs/source/conf.py
--rw-rw-r--   0 idle      (1000) idle      (1000)     1447 2023-01-21 04:57:06.000000 makeapp-1.9.0/docs/source/index.rst
--rw-rw-r--   0 idle      (1000) idle      (1000)     2730 2020-09-20 03:33:45.000000 makeapp-1.9.0/docs/source/quickstart.rst
--rw-rw-r--   0 idle      (1000) idle      (1000)     1030 2013-12-18 16:21:05.000000 makeapp-1.9.0/docs/source/rst_guide.rst
--rw-rw-r--   0 idle      (1000) idle      (1000)     1832 2020-03-05 11:23:55.000000 makeapp-1.9.0/docs/source/skeletons.rst
--rw-rw-r--   0 idle      (1000) idle      (1000)     2222 2017-05-13 12:45:30.000000 makeapp-1.9.0/docs/source/userconf.rst
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.402194 makeapp-1.9.0/makeapp/
--rw-r--r--   0 idle      (1000) idle      (1000)      144 2023-01-21 05:02:58.000000 makeapp-1.9.0/makeapp/__init__.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.402194 makeapp-1.9.0/makeapp/app_templates/
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.414195 makeapp-1.9.0/makeapp/app_templates/__default__/
--rw-rw-r--   0 idle      (1000) idle      (1000)       34 2015-10-23 13:47:00.000000 makeapp-1.9.0/makeapp/app_templates/__default__/.coveragerc
--rw-rw-r--   0 idle      (1000) idle      (1000)      117 2019-07-14 03:23:16.000000 makeapp-1.9.0/makeapp/app_templates/__default__/.gitignore
--rw-rw-r--   0 idle      (1000) idle      (1000)      129 2019-07-14 03:23:16.000000 makeapp-1.9.0/makeapp/app_templates/__default__/.hgignore
--rw-rw-r--   0 idle      (1000) idle      (1000)      168 2017-05-28 03:11:06.000000 makeapp-1.9.0/makeapp/app_templates/__default__/AUTHORS
--rw-rw-r--   0 idle      (1000) idle      (1000)       84 2017-07-31 14:44:05.000000 makeapp-1.9.0/makeapp/app_templates/__default__/CHANGELOG
--rw-rw-r--   0 idle      (1000) idle      (1000)      632 2018-01-13 07:26:19.000000 makeapp-1.9.0/makeapp/app_templates/__default__/CONTRIBUTING
--rw-rw-r--   0 idle      (1000) idle      (1000)      475 2017-05-28 03:10:21.000000 makeapp-1.9.0/makeapp/app_templates/__default__/INSTALL
--rw-r--r--   0 idle      (1000) idle      (1000)      324 2017-05-26 15:11:58.000000 makeapp-1.9.0/makeapp/app_templates/__default__/MANIFEST.in
--rw-rw-r--   0 idle      (1000) idle      (1000)      503 2019-10-12 03:54:59.000000 makeapp-1.9.0/makeapp/app_templates/__default__/README.rst
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.414195 makeapp-1.9.0/makeapp/app_templates/__default__/__module_name__/
--rw-rw-r--   0 idle      (1000) idle      (1000)      212 2018-01-13 07:12:06.000000 makeapp-1.9.0/makeapp/app_templates/__default__/__module_name__/__init__.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.414195 makeapp-1.9.0/makeapp/app_templates/__default__/docs/
--rw-rw-r--   0 idle      (1000) idle      (1000)      616 2020-02-16 03:46:46.000000 makeapp-1.9.0/makeapp/app_templates/__default__/docs/Makefile
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.414195 makeapp-1.9.0/makeapp/app_templates/__default__/docs/build/
--rw-rw-r--   0 idle      (1000) idle      (1000)        0 2013-12-14 06:43:52.000000 makeapp-1.9.0/makeapp/app_templates/__default__/docs/build/empty
--rw-rw-r--   0 idle      (1000) idle      (1000)       78 2020-02-16 03:44:49.000000 makeapp-1.9.0/makeapp/app_templates/__default__/docs/requirements.txt
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.414195 makeapp-1.9.0/makeapp/app_templates/__default__/docs/source/
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.414195 makeapp-1.9.0/makeapp/app_templates/__default__/docs/source/_static/
--rw-rw-r--   0 idle      (1000) idle      (1000)        0 2013-12-14 06:43:52.000000 makeapp-1.9.0/makeapp/app_templates/__default__/docs/source/_static/empty
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.414195 makeapp-1.9.0/makeapp/app_templates/__default__/docs/source/_templates/
--rw-rw-r--   0 idle      (1000) idle      (1000)        0 2013-12-14 06:43:52.000000 makeapp-1.9.0/makeapp/app_templates/__default__/docs/source/_templates/empty
--rw-rw-r--   0 idle      (1000) idle      (1000)     4927 2020-04-24 14:13:10.000000 makeapp-1.9.0/makeapp/app_templates/__default__/docs/source/conf.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      291 2017-05-28 03:11:30.000000 makeapp-1.9.0/makeapp/app_templates/__default__/docs/source/index.rst
--rw-rw-r--   0 idle      (1000) idle      (1000)       69 2013-12-18 16:47:51.000000 makeapp-1.9.0/makeapp/app_templates/__default__/docs/source/quickstart.rst
--rw-rw-r--   0 idle      (1000) idle      (1000)     1388 2017-10-21 03:32:48.000000 makeapp-1.9.0/makeapp/app_templates/__default__/docs/source/rst_guide.rst
--rw-r--r--   0 idle      (1000) idle      (1000)       85 2023-01-21 04:53:31.000000 makeapp-1.9.0/makeapp/app_templates/__default__/setup.cfg
--rwxr-xr-x   0 idle      (1000) idle      (1000)     1805 2020-03-05 11:49:07.000000 makeapp-1.9.0/makeapp/app_templates/__default__/setup.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.414195 makeapp-1.9.0/makeapp/app_templates/__default__/tests/
--rw-rw-r--   0 idle      (1000) idle      (1000)      296 2015-10-23 13:45:56.000000 makeapp-1.9.0/makeapp/app_templates/__default__/tests/__init__.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      233 2014-01-20 13:50:22.000000 makeapp-1.9.0/makeapp/app_templates/__default__/tests/test_module.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      348 2023-01-21 04:53:06.000000 makeapp-1.9.0/makeapp/app_templates/__default__/tox.ini
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.414195 makeapp-1.9.0/makeapp/app_templates/click/
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.414195 makeapp-1.9.0/makeapp/app_templates/click/__module_name__/
--rw-rw-r--   0 idle      (1000) idle      (1000)      570 2019-07-13 02:53:52.000000 makeapp-1.9.0/makeapp/app_templates/click/__module_name__/cli.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      132 2020-03-05 11:53:59.000000 makeapp-1.9.0/makeapp/app_templates/click/makeappconf.py
--rwxrwxr-x   0 idle      (1000) idle      (1000)      106 2020-03-05 11:46:49.000000 makeapp-1.9.0/makeapp/app_templates/click/setup.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.418195 makeapp-1.9.0/makeapp/app_templates/console/
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.418195 makeapp-1.9.0/makeapp/app_templates/console/__module_name__/
--rw-rw-r--   0 idle      (1000) idle      (1000)      925 2018-01-13 07:12:06.000000 makeapp-1.9.0/makeapp/app_templates/console/__module_name__/cli.py
--rw-r--r--   0 idle      (1000) idle      (1000)      163 2020-03-05 11:50:39.000000 makeapp-1.9.0/makeapp/app_templates/console/setup.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.418195 makeapp-1.9.0/makeapp/app_templates/django/
--rw-rw-r--   0 idle      (1000) idle      (1000)      101 2020-02-16 12:07:35.000000 makeapp-1.9.0/makeapp/app_templates/django/.coveragerc
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.402194 makeapp-1.9.0/makeapp/app_templates/django/.github/
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.418195 makeapp-1.9.0/makeapp/app_templates/django/.github/workflows/
--rw-rw-r--   0 idle      (1000) idle      (1000)     1066 2023-01-21 04:52:07.000000 makeapp-1.9.0/makeapp/app_templates/django/.github/workflows/python-package.yml
--rw-r--r--   0 idle      (1000) idle      (1000)      390 2018-09-26 12:47:30.000000 makeapp-1.9.0/makeapp/app_templates/django/MANIFEST.in
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.418195 makeapp-1.9.0/makeapp/app_templates/django/__module_name__/
--rw-rw-r--   0 idle      (1000) idle      (1000)      155 2021-12-18 06:26:43.000000 makeapp-1.9.0/makeapp/app_templates/django/__module_name__/__init__.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      144 2020-02-16 12:16:54.000000 makeapp-1.9.0/makeapp/app_templates/django/__module_name__/admin.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      329 2020-05-07 10:34:05.000000 makeapp-1.9.0/makeapp/app_templates/django/__module_name__/apps.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.418195 makeapp-1.9.0/makeapp/app_templates/django/__module_name__/locale/
--rw-rw-r--   0 idle      (1000) idle      (1000)        0 2014-02-06 14:04:04.000000 makeapp-1.9.0/makeapp/app_templates/django/__module_name__/locale/empty
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.418195 makeapp-1.9.0/makeapp/app_templates/django/__module_name__/management/
--rw-rw-r--   0 idle      (1000) idle      (1000)        1 2011-11-09 13:09:44.000000 makeapp-1.9.0/makeapp/app_templates/django/__module_name__/management/__init__.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.418195 makeapp-1.9.0/makeapp/app_templates/django/__module_name__/management/commands/
--rw-r--r--   0 idle      (1000) idle      (1000)        0 2017-05-26 15:11:58.000000 makeapp-1.9.0/makeapp/app_templates/django/__module_name__/management/commands/__init__.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      361 2020-02-16 12:29:20.000000 makeapp-1.9.0/makeapp/app_templates/django/__module_name__/models.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.418195 makeapp-1.9.0/makeapp/app_templates/django/__module_name__/templates/
--rw-rw-r--   0 idle      (1000) idle      (1000)        0 2014-02-06 14:04:04.000000 makeapp-1.9.0/makeapp/app_templates/django/__module_name__/templates/empty
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.418195 makeapp-1.9.0/makeapp/app_templates/django/__module_name__/templatetags/
--rw-rw-r--   0 idle      (1000) idle      (1000)        0 2014-02-06 14:04:04.000000 makeapp-1.9.0/makeapp/app_templates/django/__module_name__/templatetags/empty
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.418195 makeapp-1.9.0/makeapp/app_templates/django/__module_name__/tests/
--rw-r--r--   0 idle      (1000) idle      (1000)       71 2017-05-26 15:11:58.000000 makeapp-1.9.0/makeapp/app_templates/django/__module_name__/tests/__init__.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      104 2020-02-16 12:12:50.000000 makeapp-1.9.0/makeapp/app_templates/django/__module_name__/tests/conftest.py
--rw-rw-r--   0 idle      (1000) idle      (1000)       91 2020-05-07 10:19:18.000000 makeapp-1.9.0/makeapp/app_templates/django/__module_name__/tests/test_basic.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      412 2014-02-18 14:41:14.000000 makeapp-1.9.0/makeapp/app_templates/django/__module_name__/views.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      204 2020-05-07 10:27:33.000000 makeapp-1.9.0/makeapp/app_templates/django/makeappconf.py
--rw-rw-r--   0 idle      (1000) idle      (1000)       28 2020-02-06 12:10:13.000000 makeapp-1.9.0/makeapp/app_templates/django/pytest.ini
--rw-rw-r--   0 idle      (1000) idle      (1000)      121 2023-01-21 04:51:18.000000 makeapp-1.9.0/makeapp/app_templates/django/setup.py
--rw-r--r--   0 idle      (1000) idle      (1000)      462 2023-01-21 04:51:05.000000 makeapp-1.9.0/makeapp/app_templates/django/tox.ini
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.418195 makeapp-1.9.0/makeapp/app_templates/pytest/
--rw-r--r--   0 idle      (1000) idle      (1000)       93 2018-09-26 12:47:30.000000 makeapp-1.9.0/makeapp/app_templates/pytest/setup.cfg
--rwxr-xr-x   0 idle      (1000) idle      (1000)      277 2020-03-05 11:47:48.000000 makeapp-1.9.0/makeapp/app_templates/pytest/setup.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.418195 makeapp-1.9.0/makeapp/app_templates/pytest/tests/
--rw-rw-r--   0 idle      (1000) idle      (1000)        0 2019-05-18 02:54:40.000000 makeapp-1.9.0/makeapp/app_templates/pytest/tests/__init__.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      161 2020-02-16 13:18:27.000000 makeapp-1.9.0/makeapp/app_templates/pytest/tests/test_module.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.418195 makeapp-1.9.0/makeapp/app_templates/pytestplugin/
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.418195 makeapp-1.9.0/makeapp/app_templates/pytestplugin/__module_name__/
--rw-rw-r--   0 idle      (1000) idle      (1000)      104 2020-03-05 11:15:08.000000 makeapp-1.9.0/makeapp/app_templates/pytestplugin/__module_name__/entry.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      145 2020-03-05 11:05:23.000000 makeapp-1.9.0/makeapp/app_templates/pytestplugin/makeappconf.py
--rwxr-xr-x   0 idle      (1000) idle      (1000)      412 2020-03-05 11:50:43.000000 makeapp-1.9.0/makeapp/app_templates/pytestplugin/setup.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.418195 makeapp-1.9.0/makeapp/app_templates/pytestplugin/tests/
--rw-rw-r--   0 idle      (1000) idle      (1000)       62 2020-03-05 11:15:27.000000 makeapp-1.9.0/makeapp/app_templates/pytestplugin/tests/test_module.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.418195 makeapp-1.9.0/makeapp/app_templates/webscaff/
--rw-rw-r--   0 idle      (1000) idle      (1000)      117 2020-02-16 02:17:28.000000 makeapp-1.9.0/makeapp/app_templates/webscaff/.gitignore
--rw-rw-r--   0 idle      (1000) idle      (1000)      117 2020-02-16 02:17:23.000000 makeapp-1.9.0/makeapp/app_templates/webscaff/.hgignore
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.418195 makeapp-1.9.0/makeapp/app_templates/webscaff/__module_name__/
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.418195 makeapp-1.9.0/makeapp/app_templates/webscaff/__module_name__/core/
--rw-rw-r--   0 idle      (1000) idle      (1000)      329 2020-02-12 11:23:30.000000 makeapp-1.9.0/makeapp/app_templates/webscaff/__module_name__/core/uwsgiinit.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.418195 makeapp-1.9.0/makeapp/app_templates/webscaff/__module_name__/settings/
--rw-rw-r--   0 idle      (1000) idle      (1000)        0 2019-07-13 11:00:02.000000 makeapp-1.9.0/makeapp/app_templates/webscaff/__module_name__/settings/__init__.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      689 2020-02-16 02:16:33.000000 makeapp-1.9.0/makeapp/app_templates/webscaff/__module_name__/settings/auto.py
--rw-rw-r--   0 idle      (1000) idle      (1000)       80 2019-07-13 12:16:19.000000 makeapp-1.9.0/makeapp/app_templates/webscaff/__module_name__/settings/base.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      298 2020-09-20 02:49:15.000000 makeapp-1.9.0/makeapp/app_templates/webscaff/__module_name__/settings/env_development.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      144 2020-09-20 02:49:27.000000 makeapp-1.9.0/makeapp/app_templates/webscaff/__module_name__/settings/env_testing.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      760 2020-09-20 05:28:30.000000 makeapp-1.9.0/makeapp/app_templates/webscaff/__module_name__/settings/sub_paths.py
--rw-rw-r--   0 idle      (1000) idle      (1000)     1499 2021-01-15 05:40:17.000000 makeapp-1.9.0/makeapp/app_templates/webscaff/__module_name__/uwsgicfg.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.418195 makeapp-1.9.0/makeapp/app_templates/webscaff/conf/
--rwxrwxr-x   0 idle      (1000) idle      (1000)      150 2020-01-26 04:10:45.000000 makeapp-1.9.0/makeapp/app_templates/webscaff/conf/__module_name__-certbot-hook.sh
--rw-rw-r--   0 idle      (1000) idle      (1000)     1178 2020-09-20 05:05:12.000000 makeapp-1.9.0/makeapp/app_templates/webscaff/conf/__module_name__.service
--rw-rw-r--   0 idle      (1000) idle      (1000)      843 2021-05-22 03:52:45.000000 makeapp-1.9.0/makeapp/app_templates/webscaff/conf/env_production.py
--rw-rw-r--   0 idle      (1000) idle      (1000)     4874 2021-05-23 10:48:39.000000 makeapp-1.9.0/makeapp/app_templates/webscaff/makeappconf.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      164 2023-01-21 04:55:35.000000 makeapp-1.9.0/makeapp/app_templates/webscaff/requirements.txt
--rw-rw-r--   0 idle      (1000) idle      (1000)      280 2023-01-21 04:54:50.000000 makeapp-1.9.0/makeapp/app_templates/webscaff/setup.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.402194 makeapp-1.9.0/makeapp/app_templates/webscaff/state/
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.418195 makeapp-1.9.0/makeapp/app_templates/webscaff/state/certbot/
--rw-rw-r--   0 idle      (1000) idle      (1000)        0 2019-10-01 13:41:42.000000 makeapp-1.9.0/makeapp/app_templates/webscaff/state/certbot/empty
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.418195 makeapp-1.9.0/makeapp/app_templates/webscaff/state/dumps/
--rw-rw-r--   0 idle      (1000) idle      (1000)        0 2019-07-13 11:42:55.000000 makeapp-1.9.0/makeapp/app_templates/webscaff/state/dumps/empty
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.422195 makeapp-1.9.0/makeapp/app_templates/webscaff/state/media/
--rw-rw-r--   0 idle      (1000) idle      (1000)        0 2019-10-01 13:41:42.000000 makeapp-1.9.0/makeapp/app_templates/webscaff/state/media/empty
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.422195 makeapp-1.9.0/makeapp/app_templates/webscaff/state/spool/
--rw-rw-r--   0 idle      (1000) idle      (1000)        0 2019-10-01 13:41:42.000000 makeapp-1.9.0/makeapp/app_templates/webscaff/state/spool/empty
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.422195 makeapp-1.9.0/makeapp/app_templates/webscaff/state/static/
--rw-rw-r--   0 idle      (1000) idle      (1000)        0 2019-10-01 13:41:42.000000 makeapp-1.9.0/makeapp/app_templates/webscaff/state/static/empty
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.422195 makeapp-1.9.0/makeapp/app_templates/webscaff/tests/
--rw-rw-r--   0 idle      (1000) idle      (1000)      277 2020-02-16 03:03:48.000000 makeapp-1.9.0/makeapp/app_templates/webscaff/tests/conftest.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      123 2021-05-22 03:35:21.000000 makeapp-1.9.0/makeapp/app_templates/webscaff/tests/requirements.txt
--rw-rw-r--   0 idle      (1000) idle      (1000)      147 2020-02-12 11:45:16.000000 makeapp-1.9.0/makeapp/app_templates/webscaff/tests/test_module.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      234 2019-10-01 11:42:01.000000 makeapp-1.9.0/makeapp/app_templates/webscaff/wscaff.yml
--rw-rw-r--   0 idle      (1000) idle      (1000)     3640 2021-01-15 14:09:31.000000 makeapp-1.9.0/makeapp/appconfig.py
--rw-r--r--   0 idle      (1000) idle      (1000)    18155 2020-12-10 12:58:38.000000 makeapp-1.9.0/makeapp/appmaker.py
--rw-rw-r--   0 idle      (1000) idle      (1000)     6508 2020-02-17 14:25:31.000000 makeapp-1.9.0/makeapp/apptemplate.py
--rw-r--r--   0 idle      (1000) idle      (1000)    13656 2023-01-21 04:02:29.000000 makeapp-1.9.0/makeapp/apptools.py
--rwxrwxr-x   0 idle      (1000) idle      (1000)     5815 2020-12-10 13:11:15.000000 makeapp-1.9.0/makeapp/cli.py
--rw-r--r--   0 idle      (1000) idle      (1000)      365 2017-05-13 16:43:44.000000 makeapp-1.9.0/makeapp/exceptions.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.422195 makeapp-1.9.0/makeapp/helpers/
--rw-r--r--   0 idle      (1000) idle      (1000)        0 2017-05-13 14:27:56.000000 makeapp-1.9.0/makeapp/helpers/__init__.py
--rw-rw-r--   0 idle      (1000) idle      (1000)     1167 2023-01-21 04:49:15.000000 makeapp-1.9.0/makeapp/helpers/dist.py
--rw-r--r--   0 idle      (1000) idle      (1000)     1744 2020-02-17 14:36:54.000000 makeapp-1.9.0/makeapp/helpers/files.py
--rw-r--r--   0 idle      (1000) idle      (1000)     5313 2020-02-17 14:39:34.000000 makeapp-1.9.0/makeapp/helpers/vcs.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.422195 makeapp-1.9.0/makeapp/license_templates/
--rw-rw-r--   0 idle      (1000) idle      (1000)    10173 2013-12-17 13:52:31.000000 makeapp-1.9.0/makeapp/license_templates/apache2
--rw-rw-r--   0 idle      (1000) idle      (1000)      589 2013-12-17 13:56:17.000000 makeapp-1.9.0/makeapp/license_templates/apache2_src
--rw-rw-r--   0 idle      (1000) idle      (1000)     1301 2013-12-17 14:12:00.000000 makeapp-1.9.0/makeapp/license_templates/bsd2cl
--rw-rw-r--   0 idle      (1000) idle      (1000)     1494 2016-07-21 10:49:28.000000 makeapp-1.9.0/makeapp/license_templates/bsd3cl
--rw-rw-r--   0 idle      (1000) idle      (1000)    15238 2013-12-17 13:58:22.000000 makeapp-1.9.0/makeapp/license_templates/gpl2
--rw-rw-r--   0 idle      (1000) idle      (1000)      809 2013-12-17 14:07:27.000000 makeapp-1.9.0/makeapp/license_templates/gpl2_src
--rw-rw-r--   0 idle      (1000) idle      (1000)    32472 2013-12-17 14:02:56.000000 makeapp-1.9.0/makeapp/license_templates/gpl3
--rw-rw-r--   0 idle      (1000) idle      (1000)      737 2013-12-17 14:03:53.000000 makeapp-1.9.0/makeapp/license_templates/gpl3_src
--rw-rw-r--   0 idle      (1000) idle      (1000)     1085 2013-12-17 13:47:33.000000 makeapp-1.9.0/makeapp/license_templates/mit
--rw-rw-r--   0 idle      (1000) idle      (1000)       34 2013-12-17 14:06:48.000000 makeapp-1.9.0/makeapp/license_templates/no
--rw-rw-r--   0 idle      (1000) idle      (1000)       34 2013-12-17 14:06:48.000000 makeapp-1.9.0/makeapp/license_templates/no_src
--rw-rw-r--   0 idle      (1000) idle      (1000)     4043 2020-12-10 13:00:01.000000 makeapp-1.9.0/makeapp/rendering.py
--rw-r--r--   0 idle      (1000) idle      (1000)     2881 2020-12-10 12:37:54.000000 makeapp-1.9.0/makeapp/utils.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.414195 makeapp-1.9.0/makeapp.egg-info/
--rw-rw-r--   0 idle      (1000) idle      (1000)     3902 2023-01-21 05:03:05.000000 makeapp-1.9.0/makeapp.egg-info/PKG-INFO
--rw-rw-r--   0 idle      (1000) idle      (1000)     5473 2023-01-21 05:03:05.000000 makeapp-1.9.0/makeapp.egg-info/SOURCES.txt
--rw-rw-r--   0 idle      (1000) idle      (1000)        1 2023-01-21 05:03:05.000000 makeapp-1.9.0/makeapp.egg-info/dependency_links.txt
--rw-rw-r--   0 idle      (1000) idle      (1000)       46 2023-01-21 05:03:05.000000 makeapp-1.9.0/makeapp.egg-info/entry_points.txt
--rw-rw-r--   0 idle      (1000) idle      (1000)        1 2019-06-06 12:17:33.000000 makeapp-1.9.0/makeapp.egg-info/not-zip-safe
--rw-rw-r--   0 idle      (1000) idle      (1000)       56 2023-01-21 05:03:05.000000 makeapp-1.9.0/makeapp.egg-info/requires.txt
--rw-rw-r--   0 idle      (1000) idle      (1000)        8 2023-01-21 05:03:05.000000 makeapp-1.9.0/makeapp.egg-info/top_level.txt
--rw-rw-r--   0 idle      (1000) idle      (1000)      136 2023-01-21 05:03:05.422195 makeapp-1.9.0/setup.cfg
--rw-rw-r--   0 idle      (1000) idle      (1000)     1923 2023-01-21 05:00:28.000000 makeapp-1.9.0/setup.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-01-21 05:03:05.422195 makeapp-1.9.0/tests/
--rw-rw-r--   0 idle      (1000) idle      (1000)     1289 2020-05-07 10:26:52.000000 makeapp-1.9.0/tests/conftest.py
--rw-rw-r--   0 idle      (1000) idle      (1000)     3592 2021-12-18 06:38:59.000000 makeapp-1.9.0/tests/test_appmaker.py
--rw-rw-r--   0 idle      (1000) idle      (1000)     1326 2023-01-21 04:48:58.000000 makeapp-1.9.0/tests/test_apptools.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      115 2023-01-21 04:49:01.000000 makeapp-1.9.0/tests/test_helpers.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.250158 makeapp-1.9.1/
+-rw-rw-r--   0 idle      (1000) idle      (1000)      125 2014-06-07 05:37:42.000000 makeapp-1.9.1/AUTHORS
+-rw-rw-r--   0 idle      (1000) idle      (1000)     7014 2023-05-19 12:25:06.000000 makeapp-1.9.1/CHANGELOG
+-rw-rw-r--   0 idle      (1000) idle      (1000)      443 2016-07-21 10:53:31.000000 makeapp-1.9.1/INSTALL
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1499 2023-01-21 04:58:04.000000 makeapp-1.9.1/LICENSE
+-rw-rw-r--   0 idle      (1000) idle      (1000)      378 2017-05-13 17:28:02.000000 makeapp-1.9.1/MANIFEST.in
+-rw-rw-r--   0 idle      (1000) idle      (1000)     3902 2023-05-19 12:25:12.250158 makeapp-1.9.1/PKG-INFO
+-rw-rw-r--   0 idle      (1000) idle      (1000)     3150 2021-12-18 06:21:57.000000 makeapp-1.9.1/README.rst
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.230157 makeapp-1.9.1/docs/
+-rw-rw-r--   0 idle      (1000) idle      (1000)     4598 2013-12-18 16:21:05.000000 makeapp-1.9.1/docs/Makefile
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.230157 makeapp-1.9.1/docs/source/
+-rw-rw-r--   0 idle      (1000) idle      (1000)     7045 2023-01-21 04:58:07.000000 makeapp-1.9.1/docs/source/conf.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1447 2023-01-21 04:57:06.000000 makeapp-1.9.1/docs/source/index.rst
+-rw-rw-r--   0 idle      (1000) idle      (1000)     2730 2020-09-20 03:33:45.000000 makeapp-1.9.1/docs/source/quickstart.rst
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1030 2013-12-18 16:21:05.000000 makeapp-1.9.1/docs/source/rst_guide.rst
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1832 2020-03-05 11:23:55.000000 makeapp-1.9.1/docs/source/skeletons.rst
+-rw-rw-r--   0 idle      (1000) idle      (1000)     2222 2017-05-13 12:45:30.000000 makeapp-1.9.1/docs/source/userconf.rst
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.234157 makeapp-1.9.1/makeapp/
+-rw-r--r--   0 idle      (1000) idle      (1000)      144 2023-05-19 12:25:06.000000 makeapp-1.9.1/makeapp/__init__.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.230157 makeapp-1.9.1/makeapp/app_templates/
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/__default__/
+-rw-rw-r--   0 idle      (1000) idle      (1000)       34 2015-10-23 13:47:00.000000 makeapp-1.9.1/makeapp/app_templates/__default__/.coveragerc
+-rw-rw-r--   0 idle      (1000) idle      (1000)      117 2019-07-14 03:23:16.000000 makeapp-1.9.1/makeapp/app_templates/__default__/.gitignore
+-rw-rw-r--   0 idle      (1000) idle      (1000)      129 2019-07-14 03:23:16.000000 makeapp-1.9.1/makeapp/app_templates/__default__/.hgignore
+-rw-rw-r--   0 idle      (1000) idle      (1000)      168 2017-05-28 03:11:06.000000 makeapp-1.9.1/makeapp/app_templates/__default__/AUTHORS
+-rw-rw-r--   0 idle      (1000) idle      (1000)       84 2017-07-31 14:44:05.000000 makeapp-1.9.1/makeapp/app_templates/__default__/CHANGELOG
+-rw-rw-r--   0 idle      (1000) idle      (1000)      632 2018-01-13 07:26:19.000000 makeapp-1.9.1/makeapp/app_templates/__default__/CONTRIBUTING
+-rw-rw-r--   0 idle      (1000) idle      (1000)      475 2017-05-28 03:10:21.000000 makeapp-1.9.1/makeapp/app_templates/__default__/INSTALL
+-rw-r--r--   0 idle      (1000) idle      (1000)      324 2017-05-26 15:11:58.000000 makeapp-1.9.1/makeapp/app_templates/__default__/MANIFEST.in
+-rw-rw-r--   0 idle      (1000) idle      (1000)      503 2019-10-12 03:54:59.000000 makeapp-1.9.1/makeapp/app_templates/__default__/README.rst
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/__default__/__module_name__/
+-rw-rw-r--   0 idle      (1000) idle      (1000)      212 2018-01-13 07:12:06.000000 makeapp-1.9.1/makeapp/app_templates/__default__/__module_name__/__init__.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/__default__/docs/
+-rw-rw-r--   0 idle      (1000) idle      (1000)      616 2020-02-16 03:46:46.000000 makeapp-1.9.1/makeapp/app_templates/__default__/docs/Makefile
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/__default__/docs/build/
+-rw-rw-r--   0 idle      (1000) idle      (1000)        0 2013-12-14 06:43:52.000000 makeapp-1.9.1/makeapp/app_templates/__default__/docs/build/empty
+-rw-rw-r--   0 idle      (1000) idle      (1000)       78 2020-02-16 03:44:49.000000 makeapp-1.9.1/makeapp/app_templates/__default__/docs/requirements.txt
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/__default__/docs/source/
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/__default__/docs/source/_static/
+-rw-rw-r--   0 idle      (1000) idle      (1000)        0 2013-12-14 06:43:52.000000 makeapp-1.9.1/makeapp/app_templates/__default__/docs/source/_static/empty
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/__default__/docs/source/_templates/
+-rw-rw-r--   0 idle      (1000) idle      (1000)        0 2013-12-14 06:43:52.000000 makeapp-1.9.1/makeapp/app_templates/__default__/docs/source/_templates/empty
+-rw-rw-r--   0 idle      (1000) idle      (1000)     4927 2020-04-24 14:13:10.000000 makeapp-1.9.1/makeapp/app_templates/__default__/docs/source/conf.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      291 2017-05-28 03:11:30.000000 makeapp-1.9.1/makeapp/app_templates/__default__/docs/source/index.rst
+-rw-rw-r--   0 idle      (1000) idle      (1000)       69 2013-12-18 16:47:51.000000 makeapp-1.9.1/makeapp/app_templates/__default__/docs/source/quickstart.rst
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1388 2017-10-21 03:32:48.000000 makeapp-1.9.1/makeapp/app_templates/__default__/docs/source/rst_guide.rst
+-rw-r--r--   0 idle      (1000) idle      (1000)       85 2023-01-21 04:53:31.000000 makeapp-1.9.1/makeapp/app_templates/__default__/setup.cfg
+-rwxr-xr-x   0 idle      (1000) idle      (1000)     1805 2020-03-05 11:49:07.000000 makeapp-1.9.1/makeapp/app_templates/__default__/setup.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/__default__/tests/
+-rw-rw-r--   0 idle      (1000) idle      (1000)      296 2015-10-23 13:45:56.000000 makeapp-1.9.1/makeapp/app_templates/__default__/tests/__init__.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      233 2014-01-20 13:50:22.000000 makeapp-1.9.1/makeapp/app_templates/__default__/tests/test_module.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      348 2023-01-21 04:53:06.000000 makeapp-1.9.1/makeapp/app_templates/__default__/tox.ini
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/click/
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/click/__module_name__/
+-rw-rw-r--   0 idle      (1000) idle      (1000)      570 2019-07-13 02:53:52.000000 makeapp-1.9.1/makeapp/app_templates/click/__module_name__/cli.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      132 2020-03-05 11:53:59.000000 makeapp-1.9.1/makeapp/app_templates/click/makeappconf.py
+-rwxrwxr-x   0 idle      (1000) idle      (1000)      106 2020-03-05 11:46:49.000000 makeapp-1.9.1/makeapp/app_templates/click/setup.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/console/
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/console/__module_name__/
+-rw-rw-r--   0 idle      (1000) idle      (1000)      925 2018-01-13 07:12:06.000000 makeapp-1.9.1/makeapp/app_templates/console/__module_name__/cli.py
+-rw-r--r--   0 idle      (1000) idle      (1000)      163 2020-03-05 11:50:39.000000 makeapp-1.9.1/makeapp/app_templates/console/setup.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/django/
+-rw-rw-r--   0 idle      (1000) idle      (1000)      101 2020-02-16 12:07:35.000000 makeapp-1.9.1/makeapp/app_templates/django/.coveragerc
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.230157 makeapp-1.9.1/makeapp/app_templates/django/.github/
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/django/.github/workflows/
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1066 2023-01-21 04:52:07.000000 makeapp-1.9.1/makeapp/app_templates/django/.github/workflows/python-package.yml
+-rw-r--r--   0 idle      (1000) idle      (1000)      390 2018-09-26 12:47:30.000000 makeapp-1.9.1/makeapp/app_templates/django/MANIFEST.in
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/django/__module_name__/
+-rw-rw-r--   0 idle      (1000) idle      (1000)      155 2021-12-18 06:26:43.000000 makeapp-1.9.1/makeapp/app_templates/django/__module_name__/__init__.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      144 2020-02-16 12:16:54.000000 makeapp-1.9.1/makeapp/app_templates/django/__module_name__/admin.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      329 2020-05-07 10:34:05.000000 makeapp-1.9.1/makeapp/app_templates/django/__module_name__/apps.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/django/__module_name__/locale/
+-rw-rw-r--   0 idle      (1000) idle      (1000)        0 2014-02-06 14:04:04.000000 makeapp-1.9.1/makeapp/app_templates/django/__module_name__/locale/empty
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/django/__module_name__/management/
+-rw-rw-r--   0 idle      (1000) idle      (1000)        1 2011-11-09 13:09:44.000000 makeapp-1.9.1/makeapp/app_templates/django/__module_name__/management/__init__.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/django/__module_name__/management/commands/
+-rw-r--r--   0 idle      (1000) idle      (1000)        0 2017-05-26 15:11:58.000000 makeapp-1.9.1/makeapp/app_templates/django/__module_name__/management/commands/__init__.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      361 2020-02-16 12:29:20.000000 makeapp-1.9.1/makeapp/app_templates/django/__module_name__/models.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/django/__module_name__/templates/
+-rw-rw-r--   0 idle      (1000) idle      (1000)        0 2014-02-06 14:04:04.000000 makeapp-1.9.1/makeapp/app_templates/django/__module_name__/templates/empty
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/django/__module_name__/templatetags/
+-rw-rw-r--   0 idle      (1000) idle      (1000)        0 2014-02-06 14:04:04.000000 makeapp-1.9.1/makeapp/app_templates/django/__module_name__/templatetags/empty
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/django/__module_name__/tests/
+-rw-r--r--   0 idle      (1000) idle      (1000)       71 2017-05-26 15:11:58.000000 makeapp-1.9.1/makeapp/app_templates/django/__module_name__/tests/__init__.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      104 2020-02-16 12:12:50.000000 makeapp-1.9.1/makeapp/app_templates/django/__module_name__/tests/conftest.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)       91 2020-05-07 10:19:18.000000 makeapp-1.9.1/makeapp/app_templates/django/__module_name__/tests/test_basic.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      412 2014-02-18 14:41:14.000000 makeapp-1.9.1/makeapp/app_templates/django/__module_name__/views.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      204 2020-05-07 10:27:33.000000 makeapp-1.9.1/makeapp/app_templates/django/makeappconf.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)       28 2020-02-06 12:10:13.000000 makeapp-1.9.1/makeapp/app_templates/django/pytest.ini
+-rw-rw-r--   0 idle      (1000) idle      (1000)      121 2023-01-21 04:51:18.000000 makeapp-1.9.1/makeapp/app_templates/django/setup.py
+-rw-r--r--   0 idle      (1000) idle      (1000)      462 2023-01-21 04:51:05.000000 makeapp-1.9.1/makeapp/app_templates/django/tox.ini
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/pytest/
+-rw-r--r--   0 idle      (1000) idle      (1000)       93 2018-09-26 12:47:30.000000 makeapp-1.9.1/makeapp/app_templates/pytest/setup.cfg
+-rwxr-xr-x   0 idle      (1000) idle      (1000)      277 2020-03-05 11:47:48.000000 makeapp-1.9.1/makeapp/app_templates/pytest/setup.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/pytest/tests/
+-rw-rw-r--   0 idle      (1000) idle      (1000)        0 2019-05-18 02:54:40.000000 makeapp-1.9.1/makeapp/app_templates/pytest/tests/__init__.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      161 2020-02-16 13:18:27.000000 makeapp-1.9.1/makeapp/app_templates/pytest/tests/test_module.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/pytestplugin/
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/pytestplugin/__module_name__/
+-rw-rw-r--   0 idle      (1000) idle      (1000)      104 2020-03-05 11:15:08.000000 makeapp-1.9.1/makeapp/app_templates/pytestplugin/__module_name__/entry.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      145 2020-03-05 11:05:23.000000 makeapp-1.9.1/makeapp/app_templates/pytestplugin/makeappconf.py
+-rwxr-xr-x   0 idle      (1000) idle      (1000)      412 2020-03-05 11:50:43.000000 makeapp-1.9.1/makeapp/app_templates/pytestplugin/setup.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.246158 makeapp-1.9.1/makeapp/app_templates/pytestplugin/tests/
+-rw-rw-r--   0 idle      (1000) idle      (1000)       62 2020-03-05 11:15:27.000000 makeapp-1.9.1/makeapp/app_templates/pytestplugin/tests/test_module.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.250158 makeapp-1.9.1/makeapp/app_templates/webscaff/
+-rw-rw-r--   0 idle      (1000) idle      (1000)      117 2020-02-16 02:17:28.000000 makeapp-1.9.1/makeapp/app_templates/webscaff/.gitignore
+-rw-rw-r--   0 idle      (1000) idle      (1000)      117 2020-02-16 02:17:23.000000 makeapp-1.9.1/makeapp/app_templates/webscaff/.hgignore
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.250158 makeapp-1.9.1/makeapp/app_templates/webscaff/__module_name__/
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.250158 makeapp-1.9.1/makeapp/app_templates/webscaff/__module_name__/core/
+-rw-rw-r--   0 idle      (1000) idle      (1000)      329 2020-02-12 11:23:30.000000 makeapp-1.9.1/makeapp/app_templates/webscaff/__module_name__/core/uwsgiinit.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.250158 makeapp-1.9.1/makeapp/app_templates/webscaff/__module_name__/settings/
+-rw-rw-r--   0 idle      (1000) idle      (1000)        0 2019-07-13 11:00:02.000000 makeapp-1.9.1/makeapp/app_templates/webscaff/__module_name__/settings/__init__.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      689 2020-02-16 02:16:33.000000 makeapp-1.9.1/makeapp/app_templates/webscaff/__module_name__/settings/auto.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)       80 2019-07-13 12:16:19.000000 makeapp-1.9.1/makeapp/app_templates/webscaff/__module_name__/settings/base.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      298 2020-09-20 02:49:15.000000 makeapp-1.9.1/makeapp/app_templates/webscaff/__module_name__/settings/env_development.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      144 2020-09-20 02:49:27.000000 makeapp-1.9.1/makeapp/app_templates/webscaff/__module_name__/settings/env_testing.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      760 2020-09-20 05:28:30.000000 makeapp-1.9.1/makeapp/app_templates/webscaff/__module_name__/settings/sub_paths.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1499 2021-01-15 05:40:17.000000 makeapp-1.9.1/makeapp/app_templates/webscaff/__module_name__/uwsgicfg.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.250158 makeapp-1.9.1/makeapp/app_templates/webscaff/conf/
+-rwxrwxr-x   0 idle      (1000) idle      (1000)      150 2020-01-26 04:10:45.000000 makeapp-1.9.1/makeapp/app_templates/webscaff/conf/__module_name__-certbot-hook.sh
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1178 2020-09-20 05:05:12.000000 makeapp-1.9.1/makeapp/app_templates/webscaff/conf/__module_name__.service
+-rw-rw-r--   0 idle      (1000) idle      (1000)      843 2021-05-22 03:52:45.000000 makeapp-1.9.1/makeapp/app_templates/webscaff/conf/env_production.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)     4874 2021-05-23 10:48:39.000000 makeapp-1.9.1/makeapp/app_templates/webscaff/makeappconf.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      164 2023-01-21 04:55:35.000000 makeapp-1.9.1/makeapp/app_templates/webscaff/requirements.txt
+-rw-rw-r--   0 idle      (1000) idle      (1000)      280 2023-01-21 04:54:50.000000 makeapp-1.9.1/makeapp/app_templates/webscaff/setup.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.230157 makeapp-1.9.1/makeapp/app_templates/webscaff/state/
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.250158 makeapp-1.9.1/makeapp/app_templates/webscaff/state/certbot/
+-rw-rw-r--   0 idle      (1000) idle      (1000)        0 2019-10-01 13:41:42.000000 makeapp-1.9.1/makeapp/app_templates/webscaff/state/certbot/empty
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.250158 makeapp-1.9.1/makeapp/app_templates/webscaff/state/dumps/
+-rw-rw-r--   0 idle      (1000) idle      (1000)        0 2019-07-13 11:42:55.000000 makeapp-1.9.1/makeapp/app_templates/webscaff/state/dumps/empty
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.250158 makeapp-1.9.1/makeapp/app_templates/webscaff/state/media/
+-rw-rw-r--   0 idle      (1000) idle      (1000)        0 2019-10-01 13:41:42.000000 makeapp-1.9.1/makeapp/app_templates/webscaff/state/media/empty
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.250158 makeapp-1.9.1/makeapp/app_templates/webscaff/state/spool/
+-rw-rw-r--   0 idle      (1000) idle      (1000)        0 2019-10-01 13:41:42.000000 makeapp-1.9.1/makeapp/app_templates/webscaff/state/spool/empty
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.250158 makeapp-1.9.1/makeapp/app_templates/webscaff/state/static/
+-rw-rw-r--   0 idle      (1000) idle      (1000)        0 2019-10-01 13:41:42.000000 makeapp-1.9.1/makeapp/app_templates/webscaff/state/static/empty
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.250158 makeapp-1.9.1/makeapp/app_templates/webscaff/tests/
+-rw-rw-r--   0 idle      (1000) idle      (1000)      277 2020-02-16 03:03:48.000000 makeapp-1.9.1/makeapp/app_templates/webscaff/tests/conftest.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      123 2021-05-22 03:35:21.000000 makeapp-1.9.1/makeapp/app_templates/webscaff/tests/requirements.txt
+-rw-rw-r--   0 idle      (1000) idle      (1000)      147 2020-02-12 11:45:16.000000 makeapp-1.9.1/makeapp/app_templates/webscaff/tests/test_module.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      234 2019-10-01 11:42:01.000000 makeapp-1.9.1/makeapp/app_templates/webscaff/wscaff.yml
+-rw-rw-r--   0 idle      (1000) idle      (1000)     3640 2021-01-15 14:09:31.000000 makeapp-1.9.1/makeapp/appconfig.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)    18257 2023-05-19 12:15:36.000000 makeapp-1.9.1/makeapp/appmaker.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)     6508 2020-02-17 14:25:31.000000 makeapp-1.9.1/makeapp/apptemplate.py
+-rw-r--r--   0 idle      (1000) idle      (1000)    13656 2023-01-21 04:02:29.000000 makeapp-1.9.1/makeapp/apptools.py
+-rwxrwxr-x   0 idle      (1000) idle      (1000)     5777 2023-05-19 12:16:36.000000 makeapp-1.9.1/makeapp/cli.py
+-rw-r--r--   0 idle      (1000) idle      (1000)      365 2017-05-13 16:43:44.000000 makeapp-1.9.1/makeapp/exceptions.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.250158 makeapp-1.9.1/makeapp/helpers/
+-rw-r--r--   0 idle      (1000) idle      (1000)        0 2017-05-13 14:27:56.000000 makeapp-1.9.1/makeapp/helpers/__init__.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1167 2023-01-21 04:49:15.000000 makeapp-1.9.1/makeapp/helpers/dist.py
+-rw-r--r--   0 idle      (1000) idle      (1000)     1744 2020-02-17 14:36:54.000000 makeapp-1.9.1/makeapp/helpers/files.py
+-rw-r--r--   0 idle      (1000) idle      (1000)     5313 2020-02-17 14:39:34.000000 makeapp-1.9.1/makeapp/helpers/vcs.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.250158 makeapp-1.9.1/makeapp/license_templates/
+-rw-rw-r--   0 idle      (1000) idle      (1000)    10173 2013-12-17 13:52:31.000000 makeapp-1.9.1/makeapp/license_templates/apache2
+-rw-rw-r--   0 idle      (1000) idle      (1000)      589 2013-12-17 13:56:17.000000 makeapp-1.9.1/makeapp/license_templates/apache2_src
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1301 2013-12-17 14:12:00.000000 makeapp-1.9.1/makeapp/license_templates/bsd2cl
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1494 2016-07-21 10:49:28.000000 makeapp-1.9.1/makeapp/license_templates/bsd3cl
+-rw-rw-r--   0 idle      (1000) idle      (1000)    15238 2013-12-17 13:58:22.000000 makeapp-1.9.1/makeapp/license_templates/gpl2
+-rw-rw-r--   0 idle      (1000) idle      (1000)      809 2013-12-17 14:07:27.000000 makeapp-1.9.1/makeapp/license_templates/gpl2_src
+-rw-rw-r--   0 idle      (1000) idle      (1000)    32472 2013-12-17 14:02:56.000000 makeapp-1.9.1/makeapp/license_templates/gpl3
+-rw-rw-r--   0 idle      (1000) idle      (1000)      737 2013-12-17 14:03:53.000000 makeapp-1.9.1/makeapp/license_templates/gpl3_src
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1085 2013-12-17 13:47:33.000000 makeapp-1.9.1/makeapp/license_templates/mit
+-rw-rw-r--   0 idle      (1000) idle      (1000)       34 2013-12-17 14:06:48.000000 makeapp-1.9.1/makeapp/license_templates/no
+-rw-rw-r--   0 idle      (1000) idle      (1000)       34 2013-12-17 14:06:48.000000 makeapp-1.9.1/makeapp/license_templates/no_src
+-rw-rw-r--   0 idle      (1000) idle      (1000)     4043 2020-12-10 13:00:01.000000 makeapp-1.9.1/makeapp/rendering.py
+-rw-r--r--   0 idle      (1000) idle      (1000)     2881 2020-12-10 12:37:54.000000 makeapp-1.9.1/makeapp/utils.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.242158 makeapp-1.9.1/makeapp.egg-info/
+-rw-rw-r--   0 idle      (1000) idle      (1000)     3902 2023-05-19 12:25:12.000000 makeapp-1.9.1/makeapp.egg-info/PKG-INFO
+-rw-rw-r--   0 idle      (1000) idle      (1000)     5473 2023-05-19 12:25:12.000000 makeapp-1.9.1/makeapp.egg-info/SOURCES.txt
+-rw-rw-r--   0 idle      (1000) idle      (1000)        1 2023-05-19 12:25:12.000000 makeapp-1.9.1/makeapp.egg-info/dependency_links.txt
+-rw-rw-r--   0 idle      (1000) idle      (1000)       46 2023-05-19 12:25:12.000000 makeapp-1.9.1/makeapp.egg-info/entry_points.txt
+-rw-rw-r--   0 idle      (1000) idle      (1000)        1 2019-06-06 12:17:33.000000 makeapp-1.9.1/makeapp.egg-info/not-zip-safe
+-rw-rw-r--   0 idle      (1000) idle      (1000)       56 2023-05-19 12:25:12.000000 makeapp-1.9.1/makeapp.egg-info/requires.txt
+-rw-rw-r--   0 idle      (1000) idle      (1000)        8 2023-05-19 12:25:12.000000 makeapp-1.9.1/makeapp.egg-info/top_level.txt
+-rw-rw-r--   0 idle      (1000) idle      (1000)      136 2023-05-19 12:25:12.250158 makeapp-1.9.1/setup.cfg
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1923 2023-01-21 05:00:28.000000 makeapp-1.9.1/setup.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-05-19 12:25:12.250158 makeapp-1.9.1/tests/
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1289 2020-05-07 10:26:52.000000 makeapp-1.9.1/tests/conftest.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)     3592 2021-12-18 06:38:59.000000 makeapp-1.9.1/tests/test_appmaker.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1326 2023-01-21 04:48:58.000000 makeapp-1.9.1/tests/test_apptools.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      115 2023-01-21 04:49:01.000000 makeapp-1.9.1/tests/test_helpers.py
```

### Comparing `makeapp-1.9.0/CHANGELOG` & `makeapp-1.9.1/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 makeapp changelog
 =================
 
 
+v1.9.1 [2023-05-19]
+-------------------
+* Added '-i' shortcut for '--increment' option of 'release' command.
+* Fix license and vcs options handling for 'new' command (closes #5).
+
+
 v1.9.0 [2023-01-21]
 -------------------
 + App templates updated.
 + Dropped QA for Py 3.6.
 + Switched to 'twine' for package publishing.
 * Switched to 'python3' binary.
```

### Comparing `makeapp-1.9.0/LICENSE` & `makeapp-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/PKG-INFO` & `makeapp-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makeapp
-Version: 1.9.0
+Version: 1.9.1
 Summary: Simplifies Python application rollout and publishing.
 Home-page: https://github.com/idlesign/makeapp
 Author: Igor `idle sign` Starikov
 Author-email: idlesign@yandex.ru
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `makeapp-1.9.0/README.rst` & `makeapp-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/docs/Makefile` & `makeapp-1.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/docs/source/conf.py` & `makeapp-1.9.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/docs/source/index.rst` & `makeapp-1.9.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/docs/source/quickstart.rst` & `makeapp-1.9.1/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/docs/source/rst_guide.rst` & `makeapp-1.9.1/docs/source/rst_guide.rst`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/docs/source/skeletons.rst` & `makeapp-1.9.1/docs/source/skeletons.rst`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/docs/source/userconf.rst` & `makeapp-1.9.1/docs/source/userconf.rst`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/app_templates/__default__/CONTRIBUTING` & `makeapp-1.9.1/makeapp/app_templates/__default__/CONTRIBUTING`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/app_templates/__default__/docs/Makefile` & `makeapp-1.9.1/makeapp/app_templates/__default__/docs/Makefile`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/app_templates/__default__/docs/source/conf.py` & `makeapp-1.9.1/makeapp/app_templates/__default__/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/app_templates/__default__/docs/source/rst_guide.rst` & `makeapp-1.9.1/makeapp/app_templates/__default__/docs/source/rst_guide.rst`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/app_templates/__default__/setup.py` & `makeapp-1.9.1/makeapp/app_templates/__default__/setup.py`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/app_templates/click/__module_name__/cli.py` & `makeapp-1.9.1/makeapp/app_templates/click/__module_name__/cli.py`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/app_templates/console/__module_name__/cli.py` & `makeapp-1.9.1/makeapp/app_templates/console/__module_name__/cli.py`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/app_templates/django/.github/workflows/python-package.yml` & `makeapp-1.9.1/makeapp/app_templates/django/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/app_templates/webscaff/__module_name__/settings/auto.py` & `makeapp-1.9.1/makeapp/app_templates/webscaff/__module_name__/settings/auto.py`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/app_templates/webscaff/__module_name__/settings/sub_paths.py` & `makeapp-1.9.1/makeapp/app_templates/webscaff/__module_name__/settings/sub_paths.py`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/app_templates/webscaff/__module_name__/uwsgicfg.py` & `makeapp-1.9.1/makeapp/app_templates/webscaff/__module_name__/uwsgicfg.py`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/app_templates/webscaff/conf/__module_name__.service` & `makeapp-1.9.1/makeapp/app_templates/webscaff/conf/__module_name__.service`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/app_templates/webscaff/conf/env_production.py` & `makeapp-1.9.1/makeapp/app_templates/webscaff/conf/env_production.py`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/app_templates/webscaff/makeappconf.py` & `makeapp-1.9.1/makeapp/app_templates/webscaff/makeappconf.py`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/appconfig.py` & `makeapp-1.9.1/makeapp/appconfig.py`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/appmaker.py` & `makeapp-1.9.1/makeapp/appmaker.py`

 * *Files 1% similar despite different names*

```diff
@@ -567,8 +567,11 @@
         settings_base = settings_base or self.settings
 
         settings_base.update(settings_new)
         for name, val in settings_base.items():
             settings_base[name] = self._replace_settings_markers(val, settings=settings_base)
 
         self._validate_setting('license', list(self.LICENSES), settings_base)
+        
+        settings_base['license_title'] = self.LICENSES[settings_base['license']][0]
+        
         self._validate_setting('vcs', list(self.VCS), settings_base)
```

### Comparing `makeapp-1.9.0/makeapp/apptemplate.py` & `makeapp-1.9.1/makeapp/apptemplate.py`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/apptools.py` & `makeapp-1.9.1/makeapp/apptools.py`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/cli.py` & `makeapp-1.9.1/makeapp/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,18 +36,18 @@
 @click.option(
     '--debug', is_flag=True,
     help='Show debug messages while processing')
 @click.option(
     '-d', '--description',
     help='Short application description')
 @click.option(
-    '-l', '--license', type=click.Choice(AppMaker.LICENSES.keys()), default=AppMaker.default_license,
+    '-l', '--license', type=click.Choice(AppMaker.LICENSES.keys()),
     help='License to use')
 @click.option(
-    '-vcs', '--vcs', type=click.Choice(AppMaker.VCS.keys()), default=AppMaker.default_vcs,
+    '-vcs', '--vcs', type=click.Choice(AppMaker.VCS.keys()),
     help='VCS type to initialize a repo')
 @click.option(
     '-f', '--configuration_file', type=click.Path(exists=True, dir_okay=False),
     help='Path to configuration file containing settings to read from')
 @click.option(
     '-s', '--templates_source_path', type=click.Path(exists=True, file_okay=False),
     help='Directory containing application structure templates')
@@ -136,16 +136,22 @@
         remote_address=remote_address,
         remote_push=remote_push,
     )
     click.secho('Done', fg='green')
 
 
 @entry_point.command()
-@click.option('--increment', help='Version number chunk to increment', type=click.Choice(VERSION_NUMBER_CHUNKS))
-@click.option('--debug', help='Show debug messages while processing', is_flag=True)
+@click.option(
+    '-i', '--increment',
+    help='Version number chunk to increment', type=click.Choice(VERSION_NUMBER_CHUNKS)
+)
+@click.option(
+    '--debug',
+    help='Show debug messages while processing', is_flag=True
+)
 def release(increment, debug):
     """Performs new application version release."""
 
     if debug:
         configure_logging(logging.DEBUG)
 
     project = Project()
```

### Comparing `makeapp-1.9.0/makeapp/helpers/dist.py` & `makeapp-1.9.1/makeapp/helpers/dist.py`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/helpers/files.py` & `makeapp-1.9.1/makeapp/helpers/files.py`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/helpers/vcs.py` & `makeapp-1.9.1/makeapp/helpers/vcs.py`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/license_templates/apache2` & `makeapp-1.9.1/makeapp/license_templates/apache2`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/license_templates/apache2_src` & `makeapp-1.9.1/makeapp/license_templates/apache2_src`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/license_templates/bsd2cl` & `makeapp-1.9.1/makeapp/license_templates/bsd2cl`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/license_templates/bsd3cl` & `makeapp-1.9.1/makeapp/license_templates/bsd3cl`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/license_templates/gpl2` & `makeapp-1.9.1/makeapp/license_templates/gpl2`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/license_templates/gpl2_src` & `makeapp-1.9.1/makeapp/license_templates/gpl2_src`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/license_templates/gpl3` & `makeapp-1.9.1/makeapp/license_templates/gpl3`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/license_templates/gpl3_src` & `makeapp-1.9.1/makeapp/license_templates/gpl3_src`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/license_templates/mit` & `makeapp-1.9.1/makeapp/license_templates/mit`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/rendering.py` & `makeapp-1.9.1/makeapp/rendering.py`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp/utils.py` & `makeapp-1.9.1/makeapp/utils.py`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/makeapp.egg-info/PKG-INFO` & `makeapp-1.9.1/makeapp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makeapp
-Version: 1.9.0
+Version: 1.9.1
 Summary: Simplifies Python application rollout and publishing.
 Home-page: https://github.com/idlesign/makeapp
 Author: Igor `idle sign` Starikov
 Author-email: idlesign@yandex.ru
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `makeapp-1.9.0/makeapp.egg-info/SOURCES.txt` & `makeapp-1.9.1/makeapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/setup.py` & `makeapp-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/tests/conftest.py` & `makeapp-1.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/tests/test_appmaker.py` & `makeapp-1.9.1/tests/test_appmaker.py`

 * *Files identical despite different names*

### Comparing `makeapp-1.9.0/tests/test_apptools.py` & `makeapp-1.9.1/tests/test_apptools.py`

 * *Files identical despite different names*

