# Comparing `tmp/djaodjin-signup-0.8.1.tar.gz` & `tmp/djaodjin-signup-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djaodjin-signup-0.8.1.tar", last modified: Fri Apr 21 22:42:42 2023, max compression
+gzip compressed data, was "djaodjin-signup-0.8.2.tar", last modified: Thu May 18 23:23:16 2023, max compression
```

## Comparing `djaodjin-signup-0.8.1.tar` & `djaodjin-signup-0.8.2.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 22:42:42.324192 djaodjin-signup-0.8.1/
--rw-r--r--   0 smirolo    (501) staff       (20)     1318 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/LICENSE.txt
--rw-r--r--   0 smirolo    (501) staff       (20)       35 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/MANIFEST.in
--rw-r--r--   0 smirolo    (501) staff       (20)     3538 2023-04-21 22:42:42.324250 djaodjin-signup-0.8.1/PKG-INFO
--rw-r--r--   0 smirolo    (501) staff       (20)     2742 2023-04-21 22:41:35.000000 djaodjin-signup-0.8.1/README.md
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 22:42:42.305063 djaodjin-signup-0.8.1/djaodjin_signup.egg-info/
--rw-r--r--   0 smirolo    (501) staff       (20)     3538 2023-04-21 22:42:42.000000 djaodjin-signup-0.8.1/djaodjin_signup.egg-info/PKG-INFO
--rw-r--r--   0 smirolo    (501) staff       (20)     2517 2023-04-21 22:42:42.000000 djaodjin-signup-0.8.1/djaodjin_signup.egg-info/SOURCES.txt
--rw-r--r--   0 smirolo    (501) staff       (20)        1 2023-04-21 22:42:42.000000 djaodjin-signup-0.8.1/djaodjin_signup.egg-info/dependency_links.txt
--rw-r--r--   0 smirolo    (501) staff       (20)      300 2023-04-21 22:42:42.000000 djaodjin-signup-0.8.1/djaodjin_signup.egg-info/requires.txt
--rw-r--r--   0 smirolo    (501) staff       (20)        7 2023-04-21 22:42:42.000000 djaodjin-signup-0.8.1/djaodjin_signup.egg-info/top_level.txt
--rw-r--r--   0 smirolo    (501) staff       (20)     1951 2023-04-18 20:03:09.000000 djaodjin-signup-0.8.1/pyproject.toml
--rw-r--r--   0 smirolo    (501) staff       (20)       79 2023-04-21 22:42:42.324438 djaodjin-signup-0.8.1/setup.cfg
--rw-r--r--   0 smirolo    (501) staff       (20)     1381 2023-04-18 18:47:59.000000 djaodjin-signup-0.8.1/setup.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 22:42:42.310682 djaodjin-signup-0.8.1/signup/
--rw-r--r--   0 smirolo    (501) staff       (20)     1435 2023-04-21 22:04:30.000000 djaodjin-signup-0.8.1/signup/__init__.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 22:42:42.312523 djaodjin-signup-0.8.1/signup/api/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/api/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4728 2023-03-11 21:02:26.000000 djaodjin-signup-0.8.1/signup/api/activities.py
--rw-r--r--   0 smirolo    (501) staff       (20)    12165 2023-04-18 21:49:58.000000 djaodjin-signup-0.8.1/signup/api/auth.py
--rw-r--r--   0 smirolo    (501) staff       (20)     5142 2022-08-24 19:36:05.000000 djaodjin-signup-0.8.1/signup/api/contacts.py
--rw-r--r--   0 smirolo    (501) staff       (20)     5964 2023-04-14 19:38:34.000000 djaodjin-signup-0.8.1/signup/api/keys.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4702 2022-08-10 04:23:07.000000 djaodjin-signup-0.8.1/signup/api/tokens.py
--rw-r--r--   0 smirolo    (501) staff       (20)    32773 2023-04-18 22:37:09.000000 djaodjin-signup-0.8.1/signup/api/users.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2265 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/auth.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2798 2023-01-21 18:23:23.000000 djaodjin-signup-0.8.1/signup/authentication.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 22:42:42.314226 djaodjin-signup-0.8.1/signup/backends/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/backends/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     5598 2023-02-15 03:47:01.000000 djaodjin-signup-0.8.1/signup/backends/auth.py
--rw-r--r--   0 smirolo    (501) staff       (20)     5325 2023-02-15 03:47:20.000000 djaodjin-signup-0.8.1/signup/backends/auth_ldap.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2346 2023-04-14 20:11:36.000000 djaodjin-signup-0.8.1/signup/backends/mfa.py
--rw-r--r--   0 smirolo    (501) staff       (20)    10329 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/backends/sts_credentials.py
--rw-r--r--   0 smirolo    (501) staff       (20)     3680 2022-09-12 04:09:41.000000 djaodjin-signup-0.8.1/signup/compat.py
--rw-r--r--   0 smirolo    (501) staff       (20)    10578 2023-03-17 20:13:09.000000 djaodjin-signup-0.8.1/signup/decorators.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2317 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/docs.py
--rw-r--r--   0 smirolo    (501) staff       (20)    12836 2023-04-08 20:24:46.000000 djaodjin-signup-0.8.1/signup/filters.py
--rw-r--r--   0 smirolo    (501) staff       (20)    17661 2023-04-08 20:23:45.000000 djaodjin-signup-0.8.1/signup/forms.py
--rw-r--r--   0 smirolo    (501) staff       (20)     3472 2023-02-14 01:47:15.000000 djaodjin-signup-0.8.1/signup/helpers.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4463 2022-10-18 18:39:14.000000 djaodjin-signup-0.8.1/signup/middleware.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 22:42:42.316227 djaodjin-signup-0.8.1/signup/migrations/
--rw-r--r--   0 smirolo    (501) staff       (20)     2953 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/migrations/0001_v0_1_9.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1093 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/migrations/0002_0_2_0.py
--rw-r--r--   0 smirolo    (501) staff       (20)      941 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/migrations/0003_0_2_1.py
--rw-r--r--   0 smirolo    (501) staff       (20)      595 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/migrations/0004_0_2_6.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1086 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/migrations/0005_0_2_8.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4912 2023-04-14 19:44:41.000000 djaodjin-signup-0.8.1/signup/migrations/0006_v0_4_7.py
--rw-r--r--   0 smirolo    (501) staff       (20)      552 2022-09-07 17:51:52.000000 djaodjin-signup-0.8.1/signup/migrations/0007_v0_4_8.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1171 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/migrations/0008_v0_6_0.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1830 2023-04-14 20:13:48.000000 djaodjin-signup-0.8.1/signup/migrations/0009_v0_8_0.py
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/migrations/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)    24697 2023-04-21 22:03:29.000000 djaodjin-signup-0.8.1/signup/mixins.py
--rw-r--r--   0 smirolo    (501) staff       (20)    35468 2023-04-21 21:37:07.000000 djaodjin-signup-0.8.1/signup/models.py
--rw-r--r--   0 smirolo    (501) staff       (20)     9177 2023-04-12 16:28:00.000000 djaodjin-signup-0.8.1/signup/serializers.py
--rw-r--r--   0 smirolo    (501) staff       (20)     7863 2022-09-12 17:12:06.000000 djaodjin-signup-0.8.1/signup/serializers_overrides.py
--rw-r--r--   0 smirolo    (501) staff       (20)     6675 2023-04-16 21:58:55.000000 djaodjin-signup-0.8.1/signup/settings.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1887 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/signals.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 22:42:42.302806 djaodjin-signup-0.8.1/signup/static/
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 22:42:42.317312 djaodjin-signup-0.8.1/signup/static/js/
--rw-r--r--   0 smirolo    (501) staff       (20)    14494 2023-04-12 16:40:38.000000 djaodjin-signup-0.8.1/signup/static/js/djaodjin-password-strength.js
--rw-r--r--   0 smirolo    (501) staff       (20)    51604 2023-04-14 17:35:46.000000 djaodjin-signup-0.8.1/signup/static/js/djaodjin-resources-vue.js
--rw-r--r--   0 smirolo    (501) staff       (20)     5924 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/static/js/djaodjin-resources.js
--rw-r--r--   0 smirolo    (501) staff       (20)    10225 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/static/js/djaodjin-signup-angular.js
--rw-r--r--   0 smirolo    (501) staff       (20)    13054 2023-04-14 19:06:38.000000 djaodjin-signup-0.8.1/signup/static/js/djaodjin-signup-vue.js
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 22:42:42.303043 djaodjin-signup-0.8.1/signup/templates/
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 22:42:42.318179 djaodjin-signup-0.8.1/signup/templates/accounts/
--rw-r--r--   0 smirolo    (501) staff       (20)      291 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/templates/accounts/disabled.html
--rw-r--r--   0 smirolo    (501) staff       (20)      775 2023-03-16 16:54:13.000000 djaodjin-signup-0.8.1/signup/templates/accounts/login.html
--rw-r--r--   0 smirolo    (501) staff       (20)      102 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/templates/accounts/logout.html
--rw-r--r--   0 smirolo    (501) staff       (20)      796 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/templates/accounts/recover.html
--rw-r--r--   0 smirolo    (501) staff       (20)      755 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/templates/accounts/register.html
--rw-r--r--   0 smirolo    (501) staff       (20)      362 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/templates/accounts/reset.html
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 22:42:42.318911 djaodjin-signup-0.8.1/signup/templates/notification/
--rw-r--r--   0 smirolo    (501) staff       (20)      247 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/templates/notification/password_reset.eml
--rw-r--r--   0 smirolo    (501) staff       (20)      221 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/templates/notification/user_activated.eml
--rw-r--r--   0 smirolo    (501) staff       (20)      207 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/templates/notification/user_registered.eml
--rw-r--r--   0 smirolo    (501) staff       (20)      241 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/templates/notification/verification.eml
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 22:42:42.319651 djaodjin-signup-0.8.1/signup/templates/users/
--rw-r--r--   0 smirolo    (501) staff       (20)     1465 2023-03-02 23:05:43.000000 djaodjin-signup-0.8.1/signup/templates/users/index.html
--rw-r--r--   0 smirolo    (501) staff       (20)      259 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/templates/users/notifications.html
--rw-r--r--   0 smirolo    (501) staff       (20)     2856 2023-04-14 19:13:40.000000 djaodjin-signup-0.8.1/signup/templates/users/password.html
--rw-r--r--   0 smirolo    (501) staff       (20)     1839 2023-02-15 21:47:15.000000 djaodjin-signup-0.8.1/signup/templates/users/pubkey.html
--rw-r--r--   0 smirolo    (501) staff       (20)     5702 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/tests.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 22:42:42.319862 djaodjin-signup-0.8.1/signup/urls/
--rw-r--r--   0 smirolo    (501) staff       (20)     1551 2023-02-14 15:00:54.000000 djaodjin-signup-0.8.1/signup/urls/__init__.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 22:42:42.321712 djaodjin-signup-0.8.1/signup/urls/api/
--rw-r--r--   0 smirolo    (501) staff       (20)     1751 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/urls/api/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1541 2022-08-10 04:42:34.000000 djaodjin-signup-0.8.1/signup/urls/api/activate.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1926 2023-03-08 02:03:00.000000 djaodjin-signup-0.8.1/signup/urls/api/activities.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1857 2023-03-02 05:24:17.000000 djaodjin-signup-0.8.1/signup/urls/api/auth.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1906 2022-08-10 04:14:49.000000 djaodjin-signup-0.8.1/signup/urls/api/contacts.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1651 2022-08-10 04:15:39.000000 djaodjin-signup-0.8.1/signup/urls/api/keys.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1637 2022-08-10 04:16:27.000000 djaodjin-signup-0.8.1/signup/urls/api/tokens.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2165 2023-04-05 22:33:04.000000 djaodjin-signup-0.8.1/signup/urls/api/users.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 22:42:42.323004 djaodjin-signup-0.8.1/signup/urls/views/
--rw-r--r--   0 smirolo    (501) staff       (20)     1924 2022-10-19 16:04:48.000000 djaodjin-signup-0.8.1/signup/urls/views/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2545 2023-03-02 05:23:57.000000 djaodjin-signup-0.8.1/signup/urls/views/accounts.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1649 2023-03-04 00:46:08.000000 djaodjin-signup-0.8.1/signup/urls/views/contacts.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1469 2022-10-11 17:31:10.000000 djaodjin-signup-0.8.1/signup/urls/views/saml.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2031 2023-04-05 22:31:53.000000 djaodjin-signup-0.8.1/signup/urls/views/users.py
--rw-r--r--   0 smirolo    (501) staff       (20)     9044 2023-04-11 21:48:35.000000 djaodjin-signup-0.8.1/signup/utils.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4272 2023-02-15 03:45:50.000000 djaodjin-signup-0.8.1/signup/validators.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-21 22:42:42.323950 djaodjin-signup-0.8.1/signup/views/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.1/signup/views/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)    16266 2023-04-21 22:32:22.000000 djaodjin-signup-0.8.1/signup/views/auth.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2739 2023-02-15 03:48:21.000000 djaodjin-signup-0.8.1/signup/views/contacts.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1903 2023-02-15 03:50:06.000000 djaodjin-signup-0.8.1/signup/views/saml.py
--rw-r--r--   0 smirolo    (501) staff       (20)    12714 2023-04-06 00:58:50.000000 djaodjin-signup-0.8.1/signup/views/users.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.042556 djaodjin-signup-0.8.2/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1318 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/LICENSE.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)       35 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/MANIFEST.in
+-rw-r--r--   0 smirolo    (501) staff       (20)     3538 2023-05-18 23:23:16.042625 djaodjin-signup-0.8.2/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     2742 2023-04-21 22:41:35.000000 djaodjin-signup-0.8.2/README.md
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.023269 djaodjin-signup-0.8.2/djaodjin_signup.egg-info/
+-rw-r--r--   0 smirolo    (501) staff       (20)     3538 2023-05-18 23:23:16.000000 djaodjin-signup-0.8.2/djaodjin_signup.egg-info/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     2517 2023-05-18 23:23:16.000000 djaodjin-signup-0.8.2/djaodjin_signup.egg-info/SOURCES.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)        1 2023-05-18 23:23:16.000000 djaodjin-signup-0.8.2/djaodjin_signup.egg-info/dependency_links.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)      300 2023-05-18 23:23:16.000000 djaodjin-signup-0.8.2/djaodjin_signup.egg-info/requires.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)        7 2023-05-18 23:23:16.000000 djaodjin-signup-0.8.2/djaodjin_signup.egg-info/top_level.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)     1951 2023-04-18 20:03:09.000000 djaodjin-signup-0.8.2/pyproject.toml
+-rw-r--r--   0 smirolo    (501) staff       (20)       79 2023-05-18 23:23:16.042836 djaodjin-signup-0.8.2/setup.cfg
+-rw-r--r--   0 smirolo    (501) staff       (20)     1381 2023-04-18 18:47:59.000000 djaodjin-signup-0.8.2/setup.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.028587 djaodjin-signup-0.8.2/signup/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1435 2023-05-18 23:22:28.000000 djaodjin-signup-0.8.2/signup/__init__.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.030221 djaodjin-signup-0.8.2/signup/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4728 2023-03-11 21:02:26.000000 djaodjin-signup-0.8.2/signup/api/activities.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    12165 2023-04-18 21:49:58.000000 djaodjin-signup-0.8.2/signup/api/auth.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     5142 2022-08-24 19:36:05.000000 djaodjin-signup-0.8.2/signup/api/contacts.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     6122 2023-05-12 22:07:01.000000 djaodjin-signup-0.8.2/signup/api/keys.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4702 2022-08-10 04:23:07.000000 djaodjin-signup-0.8.2/signup/api/tokens.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    33478 2023-05-18 20:21:41.000000 djaodjin-signup-0.8.2/signup/api/users.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2265 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/auth.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2798 2023-01-21 18:23:23.000000 djaodjin-signup-0.8.2/signup/authentication.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.031460 djaodjin-signup-0.8.2/signup/backends/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/backends/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     5598 2023-05-12 18:10:12.000000 djaodjin-signup-0.8.2/signup/backends/auth.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     6083 2023-05-12 22:39:02.000000 djaodjin-signup-0.8.2/signup/backends/auth_ldap.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2346 2023-05-12 22:07:01.000000 djaodjin-signup-0.8.2/signup/backends/mfa.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    10329 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/backends/sts_credentials.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     3680 2022-09-12 04:09:41.000000 djaodjin-signup-0.8.2/signup/compat.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    10560 2023-05-12 20:52:33.000000 djaodjin-signup-0.8.2/signup/decorators.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2317 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/docs.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    12836 2023-04-08 20:24:46.000000 djaodjin-signup-0.8.2/signup/filters.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    17812 2023-05-12 21:32:45.000000 djaodjin-signup-0.8.2/signup/forms.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     3762 2023-05-12 22:07:01.000000 djaodjin-signup-0.8.2/signup/helpers.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4463 2022-10-18 18:39:14.000000 djaodjin-signup-0.8.2/signup/middleware.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.033371 djaodjin-signup-0.8.2/signup/migrations/
+-rw-r--r--   0 smirolo    (501) staff       (20)     2953 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/migrations/0001_v0_1_9.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1093 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/migrations/0002_0_2_0.py
+-rw-r--r--   0 smirolo    (501) staff       (20)      941 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/migrations/0003_0_2_1.py
+-rw-r--r--   0 smirolo    (501) staff       (20)      595 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/migrations/0004_0_2_6.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1086 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/migrations/0005_0_2_8.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4912 2023-04-14 19:44:41.000000 djaodjin-signup-0.8.2/signup/migrations/0006_v0_4_7.py
+-rw-r--r--   0 smirolo    (501) staff       (20)      552 2022-09-07 17:51:52.000000 djaodjin-signup-0.8.2/signup/migrations/0007_v0_4_8.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1171 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/migrations/0008_v0_6_0.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1830 2023-04-14 20:13:48.000000 djaodjin-signup-0.8.2/signup/migrations/0009_v0_8_0.py
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/migrations/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    25217 2023-05-18 21:06:48.000000 djaodjin-signup-0.8.2/signup/mixins.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    36070 2023-05-18 20:39:54.000000 djaodjin-signup-0.8.2/signup/models.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     9177 2023-04-12 16:28:00.000000 djaodjin-signup-0.8.2/signup/serializers.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     7863 2022-09-12 17:12:06.000000 djaodjin-signup-0.8.2/signup/serializers_overrides.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     6677 2023-05-08 17:19:44.000000 djaodjin-signup-0.8.2/signup/settings.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1887 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/signals.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.021050 djaodjin-signup-0.8.2/signup/static/
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.034644 djaodjin-signup-0.8.2/signup/static/js/
+-rw-r--r--   0 smirolo    (501) staff       (20)    14494 2023-04-12 16:40:38.000000 djaodjin-signup-0.8.2/signup/static/js/djaodjin-password-strength.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    51604 2023-04-14 17:35:46.000000 djaodjin-signup-0.8.2/signup/static/js/djaodjin-resources-vue.js
+-rw-r--r--   0 smirolo    (501) staff       (20)     5924 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/static/js/djaodjin-resources.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    10225 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/static/js/djaodjin-signup-angular.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    13054 2023-04-14 19:06:38.000000 djaodjin-signup-0.8.2/signup/static/js/djaodjin-signup-vue.js
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.021294 djaodjin-signup-0.8.2/signup/templates/
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.036411 djaodjin-signup-0.8.2/signup/templates/accounts/
+-rw-r--r--   0 smirolo    (501) staff       (20)      291 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/templates/accounts/disabled.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      775 2023-03-16 16:54:13.000000 djaodjin-signup-0.8.2/signup/templates/accounts/login.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      102 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/templates/accounts/logout.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      796 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/templates/accounts/recover.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      755 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/templates/accounts/register.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      362 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/templates/accounts/reset.html
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.037139 djaodjin-signup-0.8.2/signup/templates/notification/
+-rw-r--r--   0 smirolo    (501) staff       (20)      247 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/templates/notification/password_reset.eml
+-rw-r--r--   0 smirolo    (501) staff       (20)      221 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/templates/notification/user_activated.eml
+-rw-r--r--   0 smirolo    (501) staff       (20)      207 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/templates/notification/user_registered.eml
+-rw-r--r--   0 smirolo    (501) staff       (20)      241 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/templates/notification/verification.eml
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.037848 djaodjin-signup-0.8.2/signup/templates/users/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1465 2023-03-02 23:05:43.000000 djaodjin-signup-0.8.2/signup/templates/users/index.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      259 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/templates/users/notifications.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     2856 2023-04-14 19:13:40.000000 djaodjin-signup-0.8.2/signup/templates/users/password.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     1839 2023-02-15 21:47:15.000000 djaodjin-signup-0.8.2/signup/templates/users/pubkey.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     5702 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/tests.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.038062 djaodjin-signup-0.8.2/signup/urls/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1551 2023-02-14 15:00:54.000000 djaodjin-signup-0.8.2/signup/urls/__init__.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.039838 djaodjin-signup-0.8.2/signup/urls/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1751 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/urls/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1541 2022-08-10 04:42:34.000000 djaodjin-signup-0.8.2/signup/urls/api/activate.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1926 2023-03-08 02:03:00.000000 djaodjin-signup-0.8.2/signup/urls/api/activities.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1857 2023-03-02 05:24:17.000000 djaodjin-signup-0.8.2/signup/urls/api/auth.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1906 2022-08-10 04:14:49.000000 djaodjin-signup-0.8.2/signup/urls/api/contacts.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1651 2022-08-10 04:15:39.000000 djaodjin-signup-0.8.2/signup/urls/api/keys.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1637 2022-08-10 04:16:27.000000 djaodjin-signup-0.8.2/signup/urls/api/tokens.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2165 2023-04-05 22:33:04.000000 djaodjin-signup-0.8.2/signup/urls/api/users.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.040894 djaodjin-signup-0.8.2/signup/urls/views/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1924 2022-10-19 16:04:48.000000 djaodjin-signup-0.8.2/signup/urls/views/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2545 2023-03-02 05:23:57.000000 djaodjin-signup-0.8.2/signup/urls/views/accounts.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1649 2023-03-04 00:46:08.000000 djaodjin-signup-0.8.2/signup/urls/views/contacts.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1469 2022-10-11 17:31:10.000000 djaodjin-signup-0.8.2/signup/urls/views/saml.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2031 2023-04-05 22:31:53.000000 djaodjin-signup-0.8.2/signup/urls/views/users.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     8894 2023-05-12 22:07:01.000000 djaodjin-signup-0.8.2/signup/utils.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4272 2023-02-15 03:45:50.000000 djaodjin-signup-0.8.2/signup/validators.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-18 23:23:16.042050 djaodjin-signup-0.8.2/signup/views/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:33.000000 djaodjin-signup-0.8.2/signup/views/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    16462 2023-05-18 22:43:56.000000 djaodjin-signup-0.8.2/signup/views/auth.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2739 2023-02-15 03:48:21.000000 djaodjin-signup-0.8.2/signup/views/contacts.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1903 2023-02-15 03:50:06.000000 djaodjin-signup-0.8.2/signup/views/saml.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    12802 2023-05-18 20:22:34.000000 djaodjin-signup-0.8.2/signup/views/users.py
```

### Comparing `djaodjin-signup-0.8.1/LICENSE.txt` & `djaodjin-signup-0.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/PKG-INFO` & `djaodjin-signup-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djaodjin-signup
-Version: 0.8.1
+Version: 0.8.2
 Summary: Django app for user authentication
 Author-email: The DjaoDjin Team <help@djaodjin.com>
 Maintainer-email: The DjaoDjin Team <help@djaodjin.com>
 License: BSD-2-Clause
 Project-URL: repository, https://github.com/djaodjin/djaodjin-signup
 Project-URL: documentation, https://djaodjin-signup.readthedocs.io/
 Project-URL: changelog, https://github.com/djaodjin/djaodjin-signup/changelog
```

### Comparing `djaodjin-signup-0.8.1/README.md` & `djaodjin-signup-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/djaodjin_signup.egg-info/PKG-INFO` & `djaodjin-signup-0.8.2/djaodjin_signup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djaodjin-signup
-Version: 0.8.1
+Version: 0.8.2
 Summary: Django app for user authentication
 Author-email: The DjaoDjin Team <help@djaodjin.com>
 Maintainer-email: The DjaoDjin Team <help@djaodjin.com>
 License: BSD-2-Clause
 Project-URL: repository, https://github.com/djaodjin/djaodjin-signup
 Project-URL: documentation, https://djaodjin-signup.readthedocs.io/
 Project-URL: changelog, https://github.com/djaodjin/djaodjin-signup/changelog
```

### Comparing `djaodjin-signup-0.8.1/djaodjin_signup.egg-info/SOURCES.txt` & `djaodjin-signup-0.8.2/djaodjin_signup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/pyproject.toml` & `djaodjin-signup-0.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/setup.py` & `djaodjin-signup-0.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/__init__.py` & `djaodjin-signup-0.8.2/signup/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """
 PEP 386-compliant version number for the signup django app.
 """
 
-__version__ = '0.8.1'
+__version__ = '0.8.2'
```

### Comparing `djaodjin-signup-0.8.1/signup/api/activities.py` & `djaodjin-signup-0.8.2/signup/api/activities.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/api/auth.py` & `djaodjin-signup-0.8.2/signup/api/auth.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/api/contacts.py` & `djaodjin-signup-0.8.2/signup/api/contacts.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/api/keys.py` & `djaodjin-signup-0.8.2/signup/api/keys.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from django.contrib.auth.hashers import make_password
 from django.core.exceptions import PermissionDenied
 from rest_framework import status
 from rest_framework.generics import GenericAPIView
 from rest_framework.response import Response
 from rest_framework.exceptions import ValidationError
 
+from ..backends.auth_ldap import is_ldap_user, set_ldap_pubkey
 from ..compat import gettext_lazy as _
 from ..docs import OpenAPIResponse, swagger_auto_schema
 from ..mixins import UserMixin
 from ..models import Credentials
 from ..serializers import (AuthenticatedUserPasswordSerializer,
     APIKeysSerializer, PublicKeySerializer, ValidationErrorSerializer)
 from ..utils import generate_random_slug
@@ -147,23 +148,26 @@
               "detail": "Public key updated successfully."
             }
         """
         #pylint:disable=unused-argument
         serializer = self.get_serializer(data=request.data)
         serializer.is_valid(raise_exception=True)
         password = serializer.validated_data.get('password')
-        if not request.user.check_password(password):
-            raise PermissionDenied(_("Incorrect credentials"))
         try:
-            self.user.set_pubkey(serializer.validated_data['pubkey'],
-                bind_password=serializer.validated_data['password'])
-            LOGGER.info("%s updated pubkey for %s.",
-                self.request.user, self.user, extra={
-                'event': 'update-pubkey', 'request': self.request,
-                'modified': self.user.username})
+            if is_ldap_user(self.user):
+                set_ldap_pubkey(self.user,
+                    serializer.validated_data['pubkey'],
+                    bind_password=password)
+                LOGGER.info("%s updated pubkey for %s.",
+                    self.request.user, self.user, extra={
+                    'event': 'update-pubkey', 'request': self.request,
+                    'modified': self.user.username})
+            else:
+                if not request.user.check_password(password):
+                    raise PermissionDenied(_("Incorrect credentials"))
         except AttributeError:
             raise ValidationError(
                 'Cannot store public key in the User model.')
         except PermissionDenied as err:
             raise ValidationError(str(err))
 
         return Response({'detail': _("Public key updated successfully.")})
```

### Comparing `djaodjin-signup-0.8.1/signup/api/tokens.py` & `djaodjin-signup-0.8.2/signup/api/tokens.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/api/users.py` & `djaodjin-signup-0.8.2/signup/api/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,21 +32,23 @@
 from rest_framework import generics, parsers, status
 from rest_framework.exceptions import ValidationError
 from rest_framework.response import Response
 from rest_framework.settings import api_settings
 
 
 from .. import filters, settings
+from ..backends.auth_ldap import is_ldap_user, set_ldap_password
 from ..compat import (force_str, gettext_lazy as _, reverse, six,
     urlparse, urlunparse)
 from ..decorators import check_has_credentials
 from ..docs import OpenAPIResponse, no_body, swagger_auto_schema
 from ..helpers import full_name_natural_split
 from ..mixins import ContactMixin, UserMixin
-from ..models import Contact, Credentials, Notification, OTPGenerator
+from ..models import (Contact, Credentials, Notification, OTPGenerator,
+    get_disabled_email_update)
 from ..serializers_overrides import UserSerializer, UserDetailSerializer
 from ..serializers import (OTPSerializer, OTPUpdateSerializer,
     PasswordChangeSerializer, NotificationsSerializer, UploadBlobSerializer,
     UserCreateSerializer, ValidationErrorSerializer)
 from ..utils import generate_random_code, get_picture_storage, handle_uniq_error
 
 
@@ -351,18 +353,14 @@
             serializer.validated_data.get('get_phone'))
         if phone:
             update_fields.update({'phone': phone})
         lang = serializer.validated_data.get('lang',
             serializer.validated_data.get('get_lang'))
         if lang:
             update_fields.update({'lang': lang})
-        for key in ('email',):
-            value = serializer.validated_data.get(key)
-            if value:
-                update_fields.update({key: value})
         with transaction.atomic():
             user = self.get_object()
             try:
                 if user.pk:
                     update_fields.update({'user': user})
                     if slug:
                         user.username = slug
@@ -371,17 +369,26 @@
                             full_name_natural_split(
                                 full_name, middle_initials=False)
                         user.first_name = first_name
                         if mid_name:
                             user.first_name = (
                                 first_name + " " + mid_name).strip()
                         user.last_name = last_name
-                    if serializer.validated_data.get('email'):
-                        user.email = serializer.validated_data.get('email')
+                    if get_disabled_email_update(user):
+                        serializer.validated_data.pop('email')
+                    else:
+                        email = serializer.validated_data.get('email')
+                        if email:
+                            user.email = email
                     user.save()
+                    update_fields.update({'email': user.email})
+                if 'email' not in update_fields:
+                    email = serializer.validated_data.get('email')
+                    if email:
+                        update_fields.update({'email': email})
                 Contact.objects.update_or_create(
                     slug=self.kwargs.get(self.lookup_url_kwarg),
                     defaults=update_fields)
             except IntegrityError as err:
                 handle_uniq_error(err)
         # A little patchy but it works. Otherwise we would need to override
         # `update` as well.
@@ -408,14 +415,15 @@
     filter_backends = (filters.SearchFilter, filters.OrderingFilter)
     serializer_class = UserSerializer
     queryset = Contact.objects.all().select_related('user')
     user_queryset = get_user_model().objects.filter(is_active=True)
 
     def as_user(self, contact):
         user_model = self.user_queryset.model
+        #pylint:disable=unused-variable
         first_name, unused, last_name = full_name_natural_split(
             contact.full_name)
         return user_model(username=contact.slug, email=contact.email,
             first_name=first_name, last_name=last_name)
 
     def get_users_queryset(self):
         return self.user_queryset.filter(contacts__isnull=True)
@@ -588,24 +596,25 @@
         user_model = self.user_queryset.model
         slug = serializer.validated_data.get('slug',
             serializer.validated_data.get('username'))
         full_name = serializer.validated_data.get('full_name',
             serializer.validated_data.get('get_full_name'))
         nick_name = serializer.validated_data.get('nick_name')
         if not nick_name:
+            #pylint:disable=unused-variable
             nick_name, unused1, unused2 = full_name_natural_split(
                 full_name, middle_initials=False)
         phone = serializer.validated_data.get('phone',
             serializer.validated_data.get('get_phone'))
         lang = serializer.validated_data.get('lang',
             serializer.validated_data.get('get_lang'))
         with transaction.atomic():
             try:
                 user = user_model.objects.get(
-                    email=serializer.validated_data.get('email'))
+                    email__iexact=serializer.validated_data.get('email'))
             except user_model.DoesNotExist:
                 user = None
             try:
                 contact = Contact.objects.create(
                     slug=slug,
                     full_name=full_name,
                     nick_name=nick_name,
@@ -649,14 +658,16 @@
             "results": [{
               "slug": "xia",
               "username": "xia",
               "printable_name": "Xia"
             }]
         }
     """
+    account_url_kwarg = 'profile'
+
     def get_queryset(self):
         return Contact.objects.filter(activities__account__slug=self.kwargs.get(
             self.account_url_kwarg)).select_related('user')
 
 
 class OTPChangeAPIView(UserMixin, generics.GenericAPIView):
 
@@ -778,19 +789,23 @@
         #pylint:disable=unused-argument
         instance = self.get_object()
         serializer = self.get_serializer(instance, data=request.data)
         serializer.is_valid(raise_exception=True)
 
         password = serializer.validated_data['password']
         new_password = serializer.validated_data.get('new_password')
-        if not self.request.user.check_password(password):
-            raise PermissionDenied(_("Incorrect credentials"))
         if new_password:
-            serializer.instance.set_password(new_password)
-            serializer.instance.save()
+            if is_ldap_user(serializer.instance):
+                set_ldap_password(serializer.instance, new_password,
+                    bind_password=password)
+            else:
+                if not self.request.user.check_password(password):
+                    raise PermissionDenied(_("Incorrect credentials"))
+                serializer.instance.set_password(new_password)
+                serializer.instance.save()
             # Updating the password logs out all other sessions for the user
             # except the current one if
             # django.contrib.auth.middleware.SessionAuthenticationMiddleware
             # is enabled.
             update_session_auth_hash(self.request, serializer.instance)
 
         return Response({'detail': _("Password updated successfully.")})
@@ -927,15 +942,15 @@
     parser_classes = (parsers.FormParser, parsers.MultiPartParser)
     serializer_class = UploadBlobSerializer
 
     def post(self, request, *args, **kwargs):
         #pylint:disable=unused-argument
         uploaded_file = request.data.get('file')
         if not uploaded_file:
-            return Response({'detail': "no location or file specified."},
+            return Response({'detail': _("no location or file specified.")},
                 status=status.HTTP_400_BAD_REQUEST)
 
         # tentatively extract file extension.
         parts = os.path.splitext(
             force_str(uploaded_file.name.replace('\\', '/')))
         ext = parts[-1].lower() if len(parts) > 1 else ""
         key_name = "%s%s" % (
```

### Comparing `djaodjin-signup-0.8.1/signup/auth.py` & `djaodjin-signup-0.8.2/signup/auth.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/authentication.py` & `djaodjin-signup-0.8.2/signup/authentication.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/backends/auth.py` & `djaodjin-signup-0.8.2/signup/backends/auth.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/backends/auth_ldap.py` & `djaodjin-signup-0.8.2/signup/backends/auth_ldap.py`

 * *Files 24% similar despite different names*

```diff
@@ -33,120 +33,133 @@
 AUTHENTICATION_BACKENDS = (
     'signup.backends.auth_ldap.LDAPBackend',
     'django.contrib.auth.backends.ModelBackend'
 )
 """
 import logging
 
-import ldap  # pip install python-ldap==3.1.0
+from django.conf import settings as django_settings
 from django.contrib.auth import get_user_model
 from django.core.exceptions import PermissionDenied
 from django.utils.encoding import force_bytes
 
 from .. import settings
 from ..compat import force_str
 
-
 LOGGER = logging.getLogger(__name__)
 
-
-class LDAPUser(object):
-
-    def __init__(self, backend, db_user=None):
-        self.backend = backend
-        self._dbuser = db_user
-
-    def __getattr__(self, name):
-        return getattr(self._dbuser, name)
-
-    def __str__(self):
-        return self._dbuser.__str__()
-
-    def _get_pk_val(self, meta=None):
-        #pylint:disable=protected-access
-        return self._dbuser._get_pk_val(meta=meta)
-
-    def _set_pk_val(self, value):
-        #pylint:disable=protected-access
-        return self._dbuser._set_pk_val(value)
-
-    pk = property(_get_pk_val, _set_pk_val) #pylint:disable=invalid-name
-
-    @staticmethod
-    def _get_bind_dn(user):
-        return settings.LDAP_USER_SEARCH_DN % {'user': force_str(user)}
-
-    def set_password(self, raw_password, bind_password=None):
-        bind_dn = self._get_bind_dn(self._dbuser.username)
-        ldap_connection = ldap.initialize(
-            settings.LDAP_SERVER_URI, bytes_mode=False)
+try:
+    import ldap  # pip install python-ldap>=3.1.0
+except ImportError:
+    LOGGER.warning("ldap module was not imported. LDAP login is disabled.")
+
+
+# Implementation Note:
+# `django.db.models.fields.related_lookups.get_normalized_value` will check
+# our model is an instance of `django.db.models.Model` so we might as well
+# make it an instance of `AbstractBaseUser`.
+# That works until queries are built by the ORM...
+
+def _get_bind_dn(user):
+    return settings.LDAP_USER_SEARCH_DN % {'user': force_str(user)}
+
+
+def is_ldap_user(user):
+    found = False
+    if ('signup.backends.auth_ldap.LDAPBackend'
+        in django_settings.AUTHENTICATION_BACKENDS):
+        bind_dn = _get_bind_dn(user.username)
         try:
-            ldap_connection.simple_bind_s(
-                force_str(bind_dn),
-                force_str(bind_password))
-            ldap_connection.passwd_s(
-                force_str(bind_dn),
-                oldpw=force_str(bind_password),
-                newpw=force_str(raw_password))
-        except ldap.LDAPError as err:
-            raise PermissionDenied(str(err))
+            ldap_connection = ldap.initialize(
+                settings.LDAP_SERVER_URI, bytes_mode=False)
+            resp = ldap_connection.search_s(
+                bind_dn, ldap.SCOPE_BASE) #pylint:disable=no-member
+            found = True
+        except ldap.LDAPError: #pylint:disable=no-member
+            found = False
         finally:
             ldap_connection.unbind_s()
+    return found
 
-    def set_pubkey(self, pubkey, bind_password=None):
-        bind_dn = self._get_bind_dn(self._dbuser.username)
-        ldap_connection = ldap.initialize(
-            settings.LDAP_SERVER_URI, bytes_mode=False)
-        try:
-            ldap_connection.simple_bind_s(
-                force_str(bind_dn),
-                force_str(bind_password))
-            ldap_connection.modify_s(force_str(bind_dn),
-                [(ldap.MOD_REPLACE, 'sshPublicKey',
-                  [force_bytes(pubkey)])])
-        except ldap.LDAPError as err:
-            raise PermissionDenied(str(err))
-        finally:
-            ldap_connection.unbind_s()
+
+def set_ldap_password(dbuser, raw_password, bind_password=None):
+    bind_dn = _get_bind_dn(dbuser.username)
+    ldap_connection = ldap.initialize(
+        settings.LDAP_SERVER_URI, bytes_mode=False)
+    try:
+        ldap_connection.simple_bind_s(
+            force_str(bind_dn),
+            force_str(bind_password))
+        ldap_connection.passwd_s(
+            force_str(bind_dn),
+            oldpw=force_str(bind_password),
+            newpw=force_str(raw_password))
+    except ldap.LDAPError as err: #pylint:disable=no-member
+        raise PermissionDenied(str(err))
+    finally:
+        ldap_connection.unbind_s()
+
+
+def set_ldap_pubkey(dbuser, pubkey, bind_password=None):
+    bind_dn = _get_bind_dn(dbuser.username)
+    ldap_connection = ldap.initialize(
+        settings.LDAP_SERVER_URI, bytes_mode=False)
+    try:
+        ldap_connection.simple_bind_s(
+            force_str(bind_dn),
+            force_str(bind_password))
+        ldap_connection.modify_s(force_str(bind_dn),
+            [(ldap.MOD_REPLACE, 'sshPublicKey', #pylint:disable=no-member
+              [force_bytes(pubkey)])])
+    except ldap.LDAPError as err:               #pylint:disable=no-member
+        raise PermissionDenied(str(err))
+    finally:
+        ldap_connection.unbind_s()
 
 
 class LDAPBackend(object):
     """
     Backend to authenticate a user through a LDAP server.
     """
     model = get_user_model()
 
-    @staticmethod
-    def _get_bind_dn(user):
-        return settings.LDAP_USER_SEARCH_DN % {'user': force_str(user)}
-
     def authenticate(self, request, username=None, password=None, **kwargs):
         #pylint:disable=unused-argument
         user = None
-        bind_dn = self._get_bind_dn(username)
+        bind_dn = _get_bind_dn(username)
         try:
             ldap_connection = ldap.initialize(
                 settings.LDAP_SERVER_URI, bytes_mode=False)
             ldap_connection.simple_bind_s(
                 force_str(bind_dn), force_str(password))
 
-            defaults = {}
+            resp = ldap_connection.search_s(
+                bind_dn, ldap.SCOPE_BASE) #pylint:disable=no-member
+            ldap_user = resp[0][1] if resp else {}
+            defaults = {
+                'first_name': force_str(ldap_user.get('sn', "")),
+                'last_name': force_str(ldap_user.get('cn', "")),
+                'email': force_str(ldap_user.get('mail', "")),
+                'password': "ldap" # prevent user from showing as inactive
+                                   # (see `has_invalid_password`).
+            }
             #pylint:disable=protected-access
             db_user, created = self.model._default_manager.get_or_create(**{
                 self.model.USERNAME_FIELD: username,
                 'defaults': defaults,
             })
             if created:
                 LOGGER.debug("created user '%s' in database.", username)
-            user = LDAPUser(self, db_user=db_user)
-        except ldap.LDAPError:
+            user = db_user
+        except ldap.LDAPError: #pylint:disable=no-member
             user = None
         finally:
             ldap_connection.unbind_s()
 
         return user
 
     def get_user(self, user_id):
         try:
-            return LDAPUser(self, db_user=self.model.objects.get(pk=user_id))
+            user = self.model.objects.get(pk=user_id)
+            return user
         except self.model.DoesNotExist:
             return None
```

### Comparing `djaodjin-signup-0.8.1/signup/backends/mfa.py` & `djaodjin-signup-0.8.2/signup/backends/mfa.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/backends/sts_credentials.py` & `djaodjin-signup-0.8.2/signup/backends/sts_credentials.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/compat.py` & `djaodjin-signup-0.8.2/signup/compat.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/decorators.py` & `djaodjin-signup-0.8.2/signup/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,17 +34,16 @@
 from django.contrib.auth.views import redirect_to_login
 from django.core.exceptions import PermissionDenied
 
 from . import settings, signals
 from .auth import validate_redirect
 from .compat import (available_attrs, gettext_lazy as _, is_authenticated,
     reverse, six)
-from .helpers import has_invalid_password
+from .helpers import get_accept_list, has_invalid_password
 from .models import Contact
-from .utils import get_accept_list
 
 
 def _insert_url(request, redirect_field_name=REDIRECT_FIELD_NAME,
                 inserted_url=None):
     '''Redirects to the *inserted_url* before going to the orginal
     request path.'''
     # This code is pretty much straightforward
```

### Comparing `djaodjin-signup-0.8.1/signup/docs.py` & `djaodjin-signup-0.8.2/signup/docs.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/filters.py` & `djaodjin-signup-0.8.2/signup/filters.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/forms.py` & `djaodjin-signup-0.8.2/signup/forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, Djaodjin Inc.
+# Copyright (c) 2023, Djaodjin Inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -33,14 +33,15 @@
 from django.contrib.auth.forms import (
     AuthenticationForm as AuthenticationBaseForm)
 from phonenumber_field.formfields import PhoneNumberField
 
 from . import settings, validators
 from .compat import gettext_lazy as _, six
 from .helpers import full_name_natural_split
+from .models import get_disabled_email_update
 from .utils import get_recaptcha_form_field
 
 
 class EmailField(forms.EmailField):
 
     default_validators = [validators.validate_email]
 
@@ -340,14 +341,16 @@
     class Meta:
         model = get_user_model()
         fields = ['username', 'full_name', 'email']
 
     def __init__(self, instance=None, **kwargs):
         super(UserForm, self).__init__(instance=instance, **kwargs)
         if instance:
+            if get_disabled_email_update(instance):
+                self.fields['email'].disabled = True
             # define other fields dynamically
             self.fields['phone'] = PhoneField(required=False)
             lang_code = settings.LANGUAGE_CODE
             contact = instance.contacts.order_by('pk').first()
             if contact:
                 self.fields['nick_name'].initial = contact.nick_name
                 self.fields['phone'].initial = contact.phone
```

### Comparing `djaodjin-signup-0.8.1/signup/helpers.py` & `djaodjin-signup-0.8.2/signup/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020, DjaoDjin inc.
+# Copyright (c) 2023, DjaoDjin inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -23,34 +23,35 @@
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import datetime
 
 from dateutil.parser import parse
 from django.utils.timezone import utc
 
+# Implementation Note: We cannot import `signup.settings` here otherwise
+# EXTRA_MIXIN is not setup properly (i.e. it uses the default one).
 from .compat import six
 
+def as_timestamp(dtime_at=None):
+    if not dtime_at:
+        dtime_at = datetime_or_now()
+    return int((
+        dtime_at - datetime.datetime(1970, 1, 1, tzinfo=utc)).total_seconds())
+
 
 def datetime_or_now(dtime_at=None):
     if not dtime_at:
         return datetime.datetime.utcnow().replace(tzinfo=utc)
     if isinstance(dtime_at, six.string_types):
         dtime_at = parse(dtime_at)
     if dtime_at.tzinfo is None:
         dtime_at = dtime_at.replace(tzinfo=utc)
     return dtime_at
 
 
-def as_timestamp(dtime_at=None):
-    if not dtime_at:
-        dtime_at = datetime_or_now()
-    return int((
-        dtime_at - datetime.datetime(1970, 1, 1, tzinfo=utc)).total_seconds())
-
-
 def full_name_natural_split(full_name, middle_initials=True):
     """
     This function splits a full name into a natural first name, last name
     and middle names.
     """
     parts = full_name.strip().split(' ')
     first_name = ""
@@ -70,14 +71,19 @@
             if middle_name:
                 mid_name += middle_name[0]
     else:
         mid_name = " ".join(parts)
     return first_name, mid_name, last_name
 
 
+def get_accept_list(request):
+    http_accept = request.META.get('HTTP_ACCEPT', '*/*')
+    return [item.strip() for item in http_accept.split(',')]
+
+
 def has_invalid_password(user):
     return not user.password or user.password.startswith('!')
 
 
 def update_context_urls(context, urls):
     if 'urls' in context:
         for key, val in six.iteritems(urls):
```

### Comparing `djaodjin-signup-0.8.1/signup/middleware.py` & `djaodjin-signup-0.8.2/signup/middleware.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/migrations/0001_v0_1_9.py` & `djaodjin-signup-0.8.2/signup/migrations/0001_v0_1_9.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/migrations/0002_0_2_0.py` & `djaodjin-signup-0.8.2/signup/migrations/0002_0_2_0.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/migrations/0003_0_2_1.py` & `djaodjin-signup-0.8.2/signup/migrations/0003_0_2_1.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/migrations/0004_0_2_6.py` & `djaodjin-signup-0.8.2/signup/migrations/0004_0_2_6.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/migrations/0005_0_2_8.py` & `djaodjin-signup-0.8.2/signup/migrations/0005_0_2_8.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/migrations/0006_v0_4_7.py` & `djaodjin-signup-0.8.2/signup/migrations/0006_v0_4_7.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/migrations/0007_v0_4_8.py` & `djaodjin-signup-0.8.2/signup/migrations/0007_v0_4_8.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/migrations/0008_v0_6_0.py` & `djaodjin-signup-0.8.2/signup/migrations/0008_v0_6_0.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/migrations/0009_v0_8_0.py` & `djaodjin-signup-0.8.2/signup/migrations/0009_v0_8_0.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/mixins.py` & `djaodjin-signup-0.8.2/signup/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,18 @@
                 self.request.resolver_match.route)
             look = re.match(pat, self.request.path.lstrip('/'))
             if look:
                 expected_path = '/' + look.group('expected_path')
                 extra =  look.group('extra')
                 if extra:
                     raise IncorrectPath(
-                        self.request.build_absolute_uri(expected_path))
+                        {'detail': (
+                         _("Incorrect path in URL. Expecting %(path)s") % {
+                        'path': self.request.build_absolute_uri(expected_path)}
+                    )})
         except AttributeError:
             pass # Django<=1.11 ResolverMatch does not have
                  # a route attribute.
 
         cleaned_data = {}
         if initial_data:
             cleaned_data = initial_data.copy()
@@ -213,32 +216,32 @@
             user = None
 
         return user, email
 
     def auth_check_disabled(self, user):
         auth_disabled = get_disabled_authentication(self.request, user)
         if auth_disabled:
-            raise AuthDisabled()
+            raise AuthDisabled(
+                {'detail': _("Authentication is disabled")})
 
     def check_user_throttles(self, request, user):
         """
         Rate-limit based on the user.
         """
         throttle = get_login_throttle()
         if throttle:
             throttle(request, self, user)
 
     def check_sso_required(self, email):
         # If the user cannot be found and we are not login
         # with an e-mail address, we cannot tell if we should
         # redirect to an SSO provider or not.
         if email:
-            domain = email.split('@')[-1]
             try:
-                delegate_auth = DelegateAuth.objects.get(domain=domain)
+                delegate_auth = DelegateAuth.objects.get_from_email(email)
                 raise SSORequired(delegate_auth)
             except DelegateAuth.DoesNotExist:
                 pass
 
     def auth_check_mfa(self, user, **cleaned_data):
         code = cleaned_data.get('code')
         if OTPGenerator.objects.filter(user=user).exists():
@@ -289,36 +292,38 @@
         # solely do so in POST HTTP requests.
         initial_data = self.prefetch_contact_info()
         LOGGER.debug("[run_pipeline] initial_data=%s", str(initial_data))
         cleaned_data = self.validate_inputs(initial_data)
         LOGGER.debug("[run_pipeline] cleaned_data=%s", str(cleaned_data))
         # Login, Verify: Find candidate User or Contact
         user, email = self.find_candidate(**cleaned_data)
-        LOGGER.debug("[run_pipeline] found_candidate user=%s, email=%s" % (
-            user, email))
+        LOGGER.debug("[run_pipeline] found_candidate user=%s, email=%s",
+            user, email)
         # Login, Verify: Check if auth is disabled for User, or
         # auth disabled globally if we only have a Contact
         self.auth_check_disabled(user)
         # Login, Verify: Auth rate-limiter
         self.check_user_throttles(self.request, user)
         # Login, Verify, Register:
         # Redirects if email requires SSO
         self.check_sso_required(email)
         # Login: If login by verifying e-mail or phone, send code
         #        Else check password
+        #pylint:disable=assignment-from-none
         user_with_backend = self.check_password(user, **cleaned_data)
 
         # Login, Verify: If required, check 2FA
         self.auth_check_mfa(user, **cleaned_data)
 
         # Register: Bot prevention verify e-mail if it looks suspicious.
         self.register_check_data(**cleaned_data)
         # Verify: If does not exist, create User from Contact
         # Register: Create User
         if not user_with_backend:
+            #pylint:disable=assignment-from-none
             user_with_backend = self.create_user(**cleaned_data)
         # Login, Verify, Register: Create session
         LOGGER.debug("[run_pipeline] create session for user_with_backend=%s",
             user_with_backend)
 
         self.create_session(user_with_backend)
         return user_with_backend
@@ -362,14 +367,15 @@
     def check_password(self, user, **cleaned_data):
         next_url = cleaned_data.get('next_url')
         email = cleaned_data.get('email')
         if not email:
             email = user.email
         # send link through e-mail
         if email:
+            #pylint:disable=unused-variable
             contact, unused = Contact.objects.prepare_email_verification(
                 email, user=user)
             send_verification_email(contact, self.request, next_url=next_url)
             raise VerifyRequired({'detail': _(
                     "We sent a one-time link to your e-mail address.")})
 
         raise serializers.ValidationError({
@@ -382,14 +388,15 @@
     """
     def check_password(self, user, **cleaned_data):
         next_url = cleaned_data.get('next_url')
 
         phone = cleaned_data.get('phone')
         # send link through phone
         if phone:
+            #pylint:disable=unused-variable
             contact, unused = Contact.objects.prepare_phone_verification(
                 phone, user=user)
             send_verification_phone(contact, self.request, next_url=next_url)
             raise VerifyRequired({'detail': _(
                     "We sent a one-time code to your phone.")})
 
         raise serializers.ValidationError({
@@ -419,15 +426,16 @@
         'street_address',
         'username',
     )
 
     def register_check_disabled(self):
         disabled_registration = get_disabled_registration(self.request)
         if disabled_registration:
-            raise RegistrationDisabled()
+            raise RegistrationDisabled(
+                {'detail': _("Registration is disabled")})
 
     def register_check_data(self, **cleaned_data):
         email = cleaned_data.get('email')
         if email:
             dynamic_validator = get_email_dynamic_validator()
             if dynamic_validator:
                 dynamic_validator(email)
@@ -508,15 +516,16 @@
 
 
     def check_password(self, user, **cleaned_data):
         #pylint:disable=unused-argument
         if (self.request.method.lower() == 'get' and
             (not user or has_invalid_password(user))):
             raise IncorrectUser({'email': _("Not found.")})
-        return None
+        return super(VerifyCompleteMixin, self).check_password(
+            user, **cleaned_data)
 
     def create_user(self, **cleaned_data):
         verification_key = self.kwargs.get(self.key_url_kwarg)
         full_name = cleaned_data.get('full_name', None)
         if not full_name:
             first_name = cleaned_data.get('first_name', "")
             last_name = cleaned_data.get('last_name', "")
@@ -611,14 +620,15 @@
                 self._user = self.request.user
             else:
                 kwargs = {self.user_field: slug}
                 self._user = get_object_or_404(self.user_queryset, **kwargs)
         return self._user
 
     def as_user(self, contact):
+        #pylint:disable=unused-variable
         first_name, unused, last_name = full_name_natural_split(
             contact.full_name)
         return self.queryset.model(username=contact.slug, email=contact.email,
             first_name=first_name, last_name=last_name)
 
     def get_context_data(self, **kwargs):
         context = super(UserMixin, self).get_context_data(**kwargs)
```

### Comparing `djaodjin-signup-0.8.1/signup/models.py` & `djaodjin-signup-0.8.2/signup/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,23 +39,23 @@
 from django.db import models, transaction, IntegrityError
 from django.template.defaultfilters import slugify
 from django.contrib.auth.hashers import check_password, make_password
 from phonenumber_field.modelfields import PhoneNumberField
 from rest_framework.exceptions import ValidationError as DRFValidationError
 
 from . import settings, signals
+from .backends.auth_ldap import is_ldap_user
 from .backends.mfa import EmailOTCBackend, PhoneOTCBackend
 from .compat import (gettext_lazy as _, import_string,
     python_2_unicode_compatible, six)
 from .helpers import (datetime_or_now, full_name_natural_split,
     has_invalid_password)
 from .utils import generate_random_slug, handle_uniq_error
 from .validators import validate_phone
 
-
 LOGGER = logging.getLogger(__name__)
 EMAIL_VERIFICATION_RE = re.compile('^%s$' % settings.EMAIL_VERIFICATION_PAT)
 
 
 def _get_extra_field_class():
     extra_class = settings.EXTRA_FIELD
     if extra_class is None:
@@ -124,15 +124,15 @@
                 username = generate_random_slug(
                     length=len(username_base) + 4, prefix=username_base + '-',
                     allowed_chars='0123456789')
                 trials = trials + 1
         raise err
 
     def create_user_from_phone(self, phone, password=None, **kwargs):
-        #pylint:disable=protected-access
+        #pylint:disable=protected-access,unused-argument
         field = self.model._meta.get_field('username')
         max_length = field.max_length
         prefix = 'user_'
         username = generate_random_slug(
             length=min(max_length - len(prefix), 40), prefix=prefix)
         try:
             field.run_validators(username)
@@ -316,21 +316,24 @@
             random_key = str(random.random()).encode('utf-8')
             salt = hashlib.sha1(random_key).hexdigest()[:5]
             verification_key = hashlib.sha1(
                 (salt+email).encode('utf-8')).hexdigest()
         # XXX The get() needs to be targeted at the write database in order
         # to avoid potential transaction consistency problems.
         contact = None
-        try:
-            if user:
-                contact = self.get(email=email, user=user)
-            else:
-                contact = self.get(email=email, user__isnull=True)
-        except self.model.DoesNotExist:
-            pass
+        if user:
+            try:
+                contact = self.get(email__iexact=email, user=user)
+            except self.model.DoesNotExist:
+                pass
+        if not contact:
+            try:
+                contact = self.get(email__iexact=email, user__isnull=True)
+            except self.model.DoesNotExist:
+                pass
         if not contact and user:
             contact = self.filter(email__isnull=True, user=user).first()
 
         if contact:
             created = False
             with transaction.atomic():
                 # We have to wrap in a transaction.atomic here, otherwise
@@ -764,33 +767,51 @@
         self.save()
 
     def provisioning_uri(self, issuer_name=None):
         return pyotp.totp.TOTP(self.priv_key).provisioning_uri(
             name=self.user.email, issuer_name=issuer_name)
 
 
+class DelegateAuthManager(models.Manager):
+
+    def get_from_email(self, email):
+        domain = email.split('@')[-1]
+        return super(DelegateAuthManager, self).get(domain=domain)
+
+
 @python_2_unicode_compatible
 class DelegateAuth(models.Model):
     """
     Authentication for users with e-mail addresses in these domains must be
     delegated to a SSO provider.
     """
+    objects = DelegateAuthManager()
+
     domain = models.CharField(max_length=100, unique=True,
         validators=[domain_name_validator, RegexValidator(URLValidator.host_re,
             _("Enter a valid 'domain', ex: example.com"), 'invalid')],
         help_text=_(
             _("fully qualified domain name at which the site is available")))
     provider = models.CharField(max_length=32)
     created_at = models.DateTimeField(auto_now_add=True,
         help_text=_("Date/time of creation (in ISO format)"))
 
     def __str__(self):
         return "%s/%s" % (self.provider, self.domain)
 
 
+def get_disabled_email_update(user):
+    try:
+        DelegateAuth.objects.get_from_email(user.email)
+        return True
+    except DelegateAuth.DoesNotExist:
+        pass
+    return is_ldap_user(user)
+
+
 def get_user_contact(user):
     if isinstance(settings.USER_CONTACT_CALLABLE, six.string_types):
         return import_string(settings.USER_CONTACT_CALLABLE)(user)
     if user:
         return Contact.objects.filter(
             models.Q(slug__iexact=user.username)
             | models.Q(email__iexact=user.email)).order_by(
```

### Comparing `djaodjin-signup-0.8.1/signup/serializers.py` & `djaodjin-signup-0.8.2/signup/serializers.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/serializers_overrides.py` & `djaodjin-signup-0.8.2/signup/serializers_overrides.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/settings.py` & `djaodjin-signup-0.8.2/signup/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         'fernet_fields.EncryptedCharField' if django.VERSION[0] < 4 else None),
     'EXTRA_FIELD': None,
     'EXTRA_MIXIN': object,
     'JWT_ALGORITHM': 'HS256',
     'JWT_SECRET_KEY': getattr(settings, 'SECRET_KEY'),
     'LDAP': {
         'SERVER_URI': None,
-        'USER_SERCH_DN': None
+        'USER_SEARCH_DN': None
     },
     'LOGIN_THROTTLE': None,
     'LOGOUT_CLEAR_COOKIES' : None,
     'MFA_MAX_ATTEMPTS': 3,
     'NOTIFICATION_TYPE': tuple([]),
     'NOTIFICATIONS_OPT_OUT': True,
     'PICTURE_STORAGE_CALLABLE': None,
@@ -117,15 +117,15 @@
 ENCRYPTED_FIELD = _SETTINGS.get('ENCRYPTED_FIELD')
 EXTRA_FIELD = _SETTINGS.get('EXTRA_FIELD')
 EXTRA_MIXIN = _SETTINGS.get('EXTRA_MIXIN')
 JWT_SECRET_KEY = _SETTINGS.get('JWT_SECRET_KEY')
 JWT_ALGORITHM = _SETTINGS.get('JWT_ALGORITHM')
 KEY_EXPIRATION = _SETTINGS.get('ACCOUNT_ACTIVATION_DAYS')
 LDAP_SERVER_URI = _SETTINGS.get('LDAP', {}).get('SERVER_URI', None)
-LDAP_USER_SEARCH_DN = _SETTINGS.get('LDAP', {}).get('USER_SERCH_DN', None)
+LDAP_USER_SEARCH_DN = _SETTINGS.get('LDAP', {}).get('USER_SEARCH_DN', None)
 
 #: A callable function, which is passed a triplet (request, view, user), and
 #: that throttles the HTTP request when there are too many attempts for that
 #: particular user to login.
 LOGIN_THROTTLE = _SETTINGS.get('LOGIN_THROTTLE')
 
 LOGOUT_CLEAR_COOKIES = _SETTINGS.get('LOGOUT_CLEAR_COOKIES')
```

### Comparing `djaodjin-signup-0.8.1/signup/signals.py` & `djaodjin-signup-0.8.2/signup/signals.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/static/js/djaodjin-password-strength.js` & `djaodjin-signup-0.8.2/signup/static/js/djaodjin-password-strength.js`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/static/js/djaodjin-resources-vue.js` & `djaodjin-signup-0.8.2/signup/static/js/djaodjin-resources-vue.js`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/static/js/djaodjin-resources.js` & `djaodjin-signup-0.8.2/signup/static/js/djaodjin-resources.js`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/static/js/djaodjin-signup-angular.js` & `djaodjin-signup-0.8.2/signup/static/js/djaodjin-signup-angular.js`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/static/js/djaodjin-signup-vue.js` & `djaodjin-signup-0.8.2/signup/static/js/djaodjin-signup-vue.js`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/templates/accounts/login.html` & `djaodjin-signup-0.8.2/signup/templates/accounts/login.html`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/templates/accounts/recover.html` & `djaodjin-signup-0.8.2/signup/templates/accounts/recover.html`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/templates/accounts/register.html` & `djaodjin-signup-0.8.2/signup/templates/accounts/register.html`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/templates/users/index.html` & `djaodjin-signup-0.8.2/signup/templates/users/index.html`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/templates/users/password.html` & `djaodjin-signup-0.8.2/signup/templates/users/password.html`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/templates/users/pubkey.html` & `djaodjin-signup-0.8.2/signup/templates/users/pubkey.html`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/tests.py` & `djaodjin-signup-0.8.2/signup/tests.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/urls/__init__.py` & `djaodjin-signup-0.8.2/signup/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/urls/api/__init__.py` & `djaodjin-signup-0.8.2/signup/urls/api/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/urls/api/activate.py` & `djaodjin-signup-0.8.2/signup/urls/api/activate.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/urls/api/activities.py` & `djaodjin-signup-0.8.2/signup/urls/api/activities.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/urls/api/auth.py` & `djaodjin-signup-0.8.2/signup/urls/api/auth.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/urls/api/contacts.py` & `djaodjin-signup-0.8.2/signup/urls/api/contacts.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/urls/api/keys.py` & `djaodjin-signup-0.8.2/signup/urls/api/keys.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/urls/api/tokens.py` & `djaodjin-signup-0.8.2/signup/urls/api/tokens.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/urls/api/users.py` & `djaodjin-signup-0.8.2/signup/urls/api/users.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/urls/views/__init__.py` & `djaodjin-signup-0.8.2/signup/urls/views/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/urls/views/accounts.py` & `djaodjin-signup-0.8.2/signup/urls/views/accounts.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/urls/views/contacts.py` & `djaodjin-signup-0.8.2/signup/urls/views/contacts.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/urls/views/saml.py` & `djaodjin-signup-0.8.2/signup/urls/views/saml.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/urls/views/users.py` & `djaodjin-signup-0.8.2/signup/urls/views/users.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/utils.py` & `djaodjin-signup-0.8.2/signup/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,19 +37,14 @@
 
 from . import settings
 from .compat import gettext_lazy as _, import_string, six
 
 LOGGER = logging.getLogger(__name__)
 
 
-def get_accept_list(request):
-    http_accept = request.META.get('HTTP_ACCEPT', '*/*')
-    return [item.strip() for item in http_accept.split(',')]
-
-
 def generate_random_code():
     return int(generate_random_slug(6, allowed_chars="0123456789"))
 
 
 def generate_random_slug(length=40, prefix=None,
                          allowed_chars="abcdef0123456789"):
     """
@@ -103,14 +98,57 @@
 def get_user_serializer():
     """
     Returns the serializer for the user model that is active in this project.
     """
     return import_string(settings.USER_SERIALIZER)
 
 
+def handle_uniq_error(err, renames=None):
+    """
+    Will raise a ``ValidationError`` with the appropriate error message.
+    """
+    field_name = None
+    err_msg = str(err).splitlines().pop()
+    # PostgreSQL unique constraint.
+    look = re.match(
+        r'DETAIL:\s+Key \(([a-z_]+)\)=\(.*\) already exists\.', err_msg)
+    if look:
+        field_name = look.group(1)
+    else:
+        look = re.match(
+          r'DETAIL:\s+Key \(lower\(([a-z_]+)::text\)\)=\(.*\) already exists\.',
+            err_msg)
+        if look:
+            field_name = look.group(1)
+        else:
+            # SQLite unique constraint.
+            look = re.match(
+                r'UNIQUE constraint failed: [a-z_]+\.([a-z_]+)', err_msg)
+            if look:
+                field_name = look.group(1)
+            else:
+                # On CentOS 7, installed sqlite 3.7.17
+                # returns differently-formatted error message.
+                look = re.match(
+                    r'column ([a-z_]+) is not unique', err_msg)
+                if look:
+                    field_name = look.group(1)
+    if field_name:
+        if renames and field_name in renames:
+            field_name = renames[field_name]
+        if field_name in ('email',):
+            # We treat these fields differently because translation of `this`
+            # is different depending on the `field_name`.
+            raise ValidationError({field_name:
+                _("This e-mail address is already taken.")})
+        raise ValidationError({field_name:
+            _("This %(field)s is already taken.") % {'field': field_name}})
+    raise err
+
+
 def printable_name(user):
     full_name = user.get_full_name()
     if full_name:
         return full_name
     return user.username
 
 
@@ -150,57 +188,14 @@
                 form.add_error(NON_FIELD_ERRORS, msg)
             else:
                 form.add_error(NON_FIELD_ERRORS,
                     _("No field '%(field)s': %(msg)s" % {
                     'field': field, 'msg': msg}))
 
 
-def handle_uniq_error(err, renames=None):
-    """
-    Will raise a ``ValidationError`` with the appropriate error message.
-    """
-    field_name = None
-    err_msg = str(err).splitlines().pop()
-    # PostgreSQL unique constraint.
-    look = re.match(
-        r'DETAIL:\s+Key \(([a-z_]+)\)=\(.*\) already exists\.', err_msg)
-    if look:
-        field_name = look.group(1)
-    else:
-        look = re.match(
-          r'DETAIL:\s+Key \(lower\(([a-z_]+)::text\)\)=\(.*\) already exists\.',
-            err_msg)
-        if look:
-            field_name = look.group(1)
-        else:
-            # SQLite unique constraint.
-            look = re.match(
-                r'UNIQUE constraint failed: [a-z_]+\.([a-z_]+)', err_msg)
-            if look:
-                field_name = look.group(1)
-            else:
-                # On CentOS 7, installed sqlite 3.7.17
-                # returns differently-formatted error message.
-                look = re.match(
-                    r'column ([a-z_]+) is not unique', err_msg)
-                if look:
-                    field_name = look.group(1)
-    if field_name:
-        if renames and field_name in renames:
-            field_name = renames[field_name]
-        if field_name in ('email',):
-            # We treat these fields differently because translation of `this`
-            # is different depending on the `field_name`.
-            raise ValidationError({field_name:
-                _("This e-mail address is already taken.")})
-        raise ValidationError({field_name:
-            _("This %(field)s is already taken.") % {'field': field_name}})
-    raise err
-
-
 def verify_token(token):
     try:
         payload = jwt.decode(
             token,
             settings.JWT_SECRET_KEY,
             algorithms=[settings.JWT_ALGORITHM],
             options={'verify_exp': True})
```

### Comparing `djaodjin-signup-0.8.1/signup/validators.py` & `djaodjin-signup-0.8.2/signup/validators.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/views/auth.py` & `djaodjin-signup-0.8.2/signup/views/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,18 @@
             context.update({'sso_required': err})
         except VerifyRequired as err:
             form = self.get_form()
             fill_form_errors(form, err)
             context = self.get_context_data(form=form)
         except AuthDisabled:
             context = {'disabled_authentication': True}
-
+        except exceptions.AuthenticationFailed as err:
+            form = self.get_form()
+            fill_form_errors(form, err)
+            context = self.get_context_data(form=form)
         if not context:
             context = self.get_context_data()
         return self.render_to_response(context)
 
 
 class SignupView(RegisterMixin, AuthResponseMixin, View):
     """
@@ -257,24 +260,24 @@
             self.run_pipeline()
             # We have an active user, so we are login them in directly.
             return HttpResponseRedirect(self.get_success_url())
         except SSORequired as err:
             form = self.get_form()
             context = self.get_context_data(form=form)
             context.update({'sso_required': err})
-        except OTPRequired as err:
+        except OTPRequired:
             form = self.get_mfa_form()
             context = self.get_context_data(form=form)
         except AuthDisabled:
             context = {'disabled_authentication': True}
         except RegistrationDisabled:
             context = {'disabled_registration': True}
-        except serializers.ValidationError as err:
+        except serializers.ValidationError:
             pass
-        except exceptions.AuthenticationFailed as err:
+        except exceptions.AuthenticationFailed:
             # Force registration
             pass
 
         if not context:
             context = self.get_context_data(form=self.get_form())
         return self.render_to_response(context)
 
@@ -334,15 +337,15 @@
         return initial
 
     def get_password_form(self):
         form_class = self.get_form_class()
         if not 'password' in form_class.base_fields:
             form_class = self.password_form_class
             form = form_class(**self.get_form_kwargs())
-            form._errors = ErrorDict()
+            form._errors = ErrorDict() #pylint:disable=protected-access
         else:
             form = form_class(**self.get_form_kwargs())
         return form
 
     def get(self, request, *args, **kwargs):
         return self.render_to_response(self.get_context_data())
```

### Comparing `djaodjin-signup-0.8.1/signup/views/contacts.py` & `djaodjin-signup-0.8.2/signup/views/contacts.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/views/saml.py` & `djaodjin-signup-0.8.2/signup/views/saml.py`

 * *Files identical despite different names*

### Comparing `djaodjin-signup-0.8.1/signup/views/users.py` & `djaodjin-signup-0.8.2/signup/views/users.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,16 @@
     profile. If a user is manager for an Organization subscribed to another
     Organization, she can access the product provided by that organization.
     """
     form_class = UserForm
     template_name = 'users/index.html'
 
     def form_valid(self, form):
-        contact = self.object.contacts.filter(email=self.object.email).first()
+        contact = self.object.contacts.filter(
+            email__iexact=self.object.email).first()
         if not contact:
             contact = self.object.contacts.order_by('pk').first()
         failed = False
         with transaction.atomic():
             # `form.save(commit=False)` will copy the form fields values
             # to the instance without committing to the database.
             # `update_db_row` will commit to the database.
@@ -141,15 +142,15 @@
             }})
             if has_invalid_password(self.object):
                 update_context_urls(context, {'user': {
                     'api_activate': reverse(
                         'api_user_activate', args=(self.object,)),
                 }})
             contact = context['user'].contacts.filter(
-                email=self.object.email).order_by('created_at').first()
+                email__iexact=self.object.email).order_by('created_at').first()
             if contact:
                 context.update({
                     'email_verified_at': contact.email_verified_at,
                     'phone_verified_at': contact.phone_verified_at
                 })
             context.update({
                 'otp_enabled': OTPGenerator.objects.filter(
@@ -268,14 +269,15 @@
         try:
             self.user.set_pubkey(form.cleaned_data['pubkey'],
                 bind_password=form.cleaned_data['password'])
             LOGGER.info("%s updated pubkey for %s.",
                 self.request.user, self.object, extra={
                 'event': 'update-pubkey', 'request': self.request,
                 'modified': self.object.username})
+            #pylint:disable=attribute-defined-outside-init
             self.object = self.user
         except AttributeError:
             form.add_error(None, "Cannot store public key in the User model.")
             return super(UserPublicKeyUpdateView, self).form_invalid(form)
         except PermissionDenied as err:
             form.add_error(None, str(err))
             return super(UserPublicKeyUpdateView, self).form_invalid(form)
```

