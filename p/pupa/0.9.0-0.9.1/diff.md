# Comparing `tmp/pupa-0.9.0.tar.gz` & `tmp/pupa-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pupa-0.9.0.tar", last modified: Wed Feb 14 05:14:54 2018, max compression
+gzip compressed data, was "dist/pupa-0.9.1.tar", last modified: Tue Oct 23 14:15:55 2018, max compression
```

## Comparing `pupa-0.9.0.tar` & `pupa-0.9.1.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2018-02-14 05:14:54.000000 pupa-0.9.0/
--rw-rw-r--   0 james     (1000) james     (1000)      401 2017-10-05 01:25:48.000000 pupa-0.9.0/README.md
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2018-02-14 05:14:54.000000 pupa-0.9.0/pupa/
--rw-rw-r--   0 james     (1000) james     (1000)     2427 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/models.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2018-02-14 05:14:54.000000 pupa-0.9.0/pupa/cli/
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2018-02-14 05:14:54.000000 pupa-0.9.0/pupa/cli/commands/
--rw-rw-r--   0 james     (1000) james     (1000)    13073 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/cli/commands/update.py
--rw-rw-r--   0 james     (1000) james     (1000)     1039 2018-01-11 17:44:38.000000 pupa-0.9.0/pupa/cli/commands/party.py
--rw-rw-r--   0 james     (1000) james     (1000)     4980 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/cli/commands/init.py
--rw-rw-r--   0 james     (1000) james     (1000)     2358 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/cli/commands/dbinit.py
--rw-rw-r--   0 james     (1000) james     (1000)        0 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/cli/commands/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)      409 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/cli/commands/base.py
--rw-rw-r--   0 james     (1000) james     (1000)        0 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/cli/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)     2419 2018-01-11 17:44:38.000000 pupa-0.9.0/pupa/cli/__main__.py
--rw-rw-r--   0 james     (1000) james     (1000)     1944 2018-01-26 16:27:12.000000 pupa-0.9.0/pupa/settings.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2018-02-14 05:14:54.000000 pupa-0.9.0/pupa/ext/
--rw-rw-r--   0 james     (1000) james     (1000)     4990 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/ext/ansistrm.py
--rw-rw-r--   0 james     (1000) james     (1000)        0 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/ext/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)     1353 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/admin.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2018-02-14 05:14:54.000000 pupa-0.9.0/pupa/migrations/
--rw-rw-r--   0 james     (1000) james     (1000)     1290 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/migrations/0002_auto_20150906_1458.py
--rw-rw-r--   0 james     (1000) james     (1000)     3335 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/migrations/0001_initial.py
--rw-rw-r--   0 james     (1000) james     (1000)      610 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/migrations/0005_auto_20170522_1935.py
--rw-rw-r--   0 james     (1000) james     (1000)      651 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/migrations/0006_identifier_jurisdiction.py
--rw-rw-r--   0 james     (1000) james     (1000)     1162 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/migrations/0003_auto_20151118_0408.py
--rw-rw-r--   0 james     (1000) james     (1000)        0 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/migrations/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)      869 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/migrations/0004_identifier.py
--rw-rw-r--   0 james     (1000) james     (1000)       43 2018-02-13 21:57:24.000000 pupa-0.9.0/pupa/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)     2526 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/exceptions.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2018-02-14 05:14:54.000000 pupa-0.9.0/pupa/tests/
--rw-rw-r--   0 james     (1000) james     (1000)        0 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/tests/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)      470 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/tests/django_settings.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2018-02-14 05:14:54.000000 pupa-0.9.0/pupa/tests/importers/
--rw-rw-r--   0 james     (1000) james     (1000)     5398 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/tests/importers/test_topsort.py
--rw-rw-r--   0 james     (1000) james     (1000)     7448 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/tests/importers/test_membership_importer.py
--rw-rw-r--   0 james     (1000) james     (1000)     6241 2018-01-26 16:27:12.000000 pupa-0.9.0/pupa/tests/importers/test_base_importer.py
--rw-rw-r--   0 james     (1000) james     (1000)        0 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/tests/importers/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)     8742 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/tests/importers/test_organization_importer.py
--rw-rw-r--   0 james     (1000) james     (1000)    20331 2018-02-13 21:53:50.000000 pupa-0.9.0/pupa/tests/importers/test_vote_event_importer.py
--rw-rw-r--   0 james     (1000) james     (1000)     4113 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/tests/importers/test_post_importer.py
--rw-rw-r--   0 james     (1000) james     (1000)     2693 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/tests/importers/test_jurisdiction_importer.py
--rw-rw-r--   0 james     (1000) james     (1000)    16025 2018-02-13 21:24:04.000000 pupa-0.9.0/pupa/tests/importers/test_bill_importer.py
--rw-rw-r--   0 james     (1000) james     (1000)     8448 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/tests/importers/test_people_importer.py
--rw-rw-r--   0 james     (1000) james     (1000)     9880 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/tests/importers/test_event_importer.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2018-02-14 05:14:54.000000 pupa-0.9.0/pupa/tests/scrape/
--rw-rw-r--   0 james     (1000) james     (1000)     2226 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/tests/scrape/test_jurisdiction_scrape.py
--rw-rw-r--   0 james     (1000) james     (1000)     6335 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/tests/scrape/test_bill_scrape.py
--rw-rw-r--   0 james     (1000) james     (1000)      620 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/tests/scrape/test_utils.py
--rw-rw-r--   0 james     (1000) james     (1000)     3363 2018-01-26 16:27:12.000000 pupa-0.9.0/pupa/tests/scrape/test_vote_event_scrape.py
--rw-rw-r--   0 james     (1000) james     (1000)     4410 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/tests/scrape/test_model_basics.py
--rw-rw-r--   0 james     (1000) james     (1000)        0 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/tests/scrape/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)     6230 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/tests/scrape/test_people_org_scrape.py
--rw-rw-r--   0 james     (1000) james     (1000)     4651 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/tests/scrape/test_event_scrape.py
--rw-rw-r--   0 james     (1000) james     (1000)     3604 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/tests/scrape/test_scraper.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2018-02-14 05:14:54.000000 pupa-0.9.0/pupa/utils/
--rw-rw-r--   0 james     (1000) james     (1000)     1886 2018-01-26 16:27:12.000000 pupa-0.9.0/pupa/utils/generic.py
--rw-rw-r--   0 james     (1000) james     (1000)      156 2018-01-26 16:27:12.000000 pupa-0.9.0/pupa/utils/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)     4925 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/utils/topsort.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2018-02-14 05:14:54.000000 pupa-0.9.0/pupa/importers/
--rw-rw-r--   0 james     (1000) james     (1000)     4601 2018-01-26 16:27:12.000000 pupa-0.9.0/pupa/importers/bills.py
--rw-rw-r--   0 james     (1000) james     (1000)     1039 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/importers/posts.py
--rw-rw-r--   0 james     (1000) james     (1000)     2765 2018-01-26 04:11:27.000000 pupa-0.9.0/pupa/importers/memberships.py
--rw-rw-r--   0 james     (1000) james     (1000)      738 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/importers/jurisdiction.py
--rw-rw-r--   0 james     (1000) james     (1000)      330 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/importers/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)    16242 2018-01-26 16:27:12.000000 pupa-0.9.0/pupa/importers/base.py
--rw-rw-r--   0 james     (1000) james     (1000)     4917 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/importers/organizations.py
--rw-rw-r--   0 james     (1000) james     (1000)     5205 2018-02-13 21:53:50.000000 pupa-0.9.0/pupa/importers/vote_events.py
--rw-rw-r--   0 james     (1000) james     (1000)     3223 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/importers/people.py
--rw-rw-r--   0 james     (1000) james     (1000)     4626 2018-01-26 16:27:12.000000 pupa-0.9.0/pupa/importers/events.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2018-02-14 05:14:54.000000 pupa-0.9.0/pupa/scrape/
--rw-rw-r--   0 james     (1000) james     (1000)     2894 2018-01-26 16:27:12.000000 pupa-0.9.0/pupa/scrape/vote_event.py
--rw-rw-r--   0 james     (1000) james     (1000)     1990 2018-01-11 17:44:39.000000 pupa-0.9.0/pupa/scrape/jurisdiction.py
--rw-rw-r--   0 james     (1000) james     (1000)     8642 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/scrape/popolo.py
--rw-rw-r--   0 james     (1000) james     (1000)      259 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/scrape/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)    10551 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/scrape/base.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2018-02-14 05:14:54.000000 pupa-0.9.0/pupa/scrape/schemas/
--rw-rw-r--   0 james     (1000) james     (1000)      988 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/scrape/schemas/organization.py
--rw-rw-r--   0 james     (1000) james     (1000)      783 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/scrape/schemas/person.py
--rw-rw-r--   0 james     (1000) james     (1000)      524 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/scrape/schemas/post.py
--rw-rw-r--   0 james     (1000) james     (1000)     1641 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/scrape/schemas/vote_event.py
--rw-rw-r--   0 james     (1000) james     (1000)      825 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/scrape/schemas/jurisdiction.py
--rw-rw-r--   0 james     (1000) james     (1000)        0 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/scrape/schemas/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)     2187 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/scrape/schemas/common.py
--rw-rw-r--   0 james     (1000) james     (1000)      832 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/scrape/schemas/membership.py
--rw-rw-r--   0 james     (1000) james     (1000)     5651 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/scrape/schemas/event.py
--rw-rw-r--   0 james     (1000) james     (1000)     4832 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/scrape/schemas/bill.py
--rw-rw-r--   0 james     (1000) james     (1000)     4917 2017-12-05 05:28:46.000000 pupa-0.9.0/pupa/scrape/event.py
--rw-rw-r--   0 james     (1000) james     (1000)     4688 2017-10-05 01:25:48.000000 pupa-0.9.0/pupa/scrape/bill.py
--rw-rw-r--   0 james     (1000) james     (1000)      678 2018-02-14 05:14:54.000000 pupa-0.9.0/PKG-INFO
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2018-02-14 05:14:54.000000 pupa-0.9.0/pupa.egg-info/
--rw-rw-r--   0 james     (1000) james     (1000)       47 2018-02-14 05:14:54.000000 pupa-0.9.0/pupa.egg-info/entry_points.txt
--rw-rw-r--   0 james     (1000) james     (1000)     2531 2018-02-14 05:14:54.000000 pupa-0.9.0/pupa.egg-info/SOURCES.txt
--rw-rw-r--   0 james     (1000) james     (1000)      165 2018-02-14 05:14:54.000000 pupa-0.9.0/pupa.egg-info/requires.txt
--rw-rw-r--   0 james     (1000) james     (1000)        1 2018-02-14 05:14:54.000000 pupa-0.9.0/pupa.egg-info/dependency_links.txt
--rw-rw-r--   0 james     (1000) james     (1000)        5 2018-02-14 05:14:54.000000 pupa-0.9.0/pupa.egg-info/top_level.txt
--rw-rw-r--   0 james     (1000) james     (1000)      678 2018-02-14 05:14:54.000000 pupa-0.9.0/pupa.egg-info/PKG-INFO
--rw-rw-r--   0 james     (1000) james     (1000)        1 2017-10-05 01:28:32.000000 pupa-0.9.0/pupa.egg-info/not-zip-safe
--rw-rw-r--   0 james     (1000) james     (1000)     1505 2017-12-05 05:28:46.000000 pupa-0.9.0/setup.py
--rw-rw-r--   0 james     (1000) james     (1000)      124 2018-02-14 05:14:54.000000 pupa-0.9.0/setup.cfg
+drwxr-xr-x   0 james      (501) staff       (20)        0 2018-10-23 14:15:55.000000 pupa-0.9.1/
+-rw-r--r--   0 james      (501) staff       (20)      664 2018-10-23 14:15:55.000000 pupa-0.9.1/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1517 2018-10-23 14:02:12.000000 pupa-0.9.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2018-10-23 14:15:55.000000 pupa-0.9.1/pupa/
+drwxr-xr-x   0 james      (501) staff       (20)        0 2018-10-23 14:15:55.000000 pupa-0.9.1/pupa/migrations/
+-rw-r--r--   0 james      (501) staff       (20)     1290 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/migrations/0002_auto_20150906_1458.py
+-rw-r--r--   0 james      (501) staff       (20)        0 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/migrations/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     1162 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/migrations/0003_auto_20151118_0408.py
+-rw-r--r--   0 james      (501) staff       (20)      651 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/migrations/0006_identifier_jurisdiction.py
+-rw-r--r--   0 james      (501) staff       (20)      869 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/migrations/0004_identifier.py
+-rw-r--r--   0 james      (501) staff       (20)     3335 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/migrations/0001_initial.py
+-rw-r--r--   0 james      (501) staff       (20)      610 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/migrations/0005_auto_20170522_1935.py
+-rw-r--r--   0 james      (501) staff       (20)     2427 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/models.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2018-10-23 14:15:55.000000 pupa-0.9.1/pupa/importers/
+-rw-r--r--   0 james      (501) staff       (20)     4626 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/importers/events.py
+-rw-r--r--   0 james      (501) staff       (20)     1039 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/importers/posts.py
+-rw-r--r--   0 james      (501) staff       (20)      330 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/importers/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     5205 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/importers/vote_events.py
+-rw-r--r--   0 james      (501) staff       (20)     3223 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/importers/people.py
+-rw-r--r--   0 james      (501) staff       (20)     4917 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/importers/organizations.py
+-rw-r--r--   0 james      (501) staff       (20)     4601 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/importers/bills.py
+-rw-r--r--   0 james      (501) staff       (20)    16242 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/importers/base.py
+-rw-r--r--   0 james      (501) staff       (20)      738 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/importers/jurisdiction.py
+-rw-r--r--   0 james      (501) staff       (20)     2765 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/importers/memberships.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2018-10-23 14:15:55.000000 pupa-0.9.1/pupa/ext/
+-rw-r--r--   0 james      (501) staff       (20)        0 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/ext/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     4990 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/ext/ansistrm.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2018-10-23 14:15:55.000000 pupa-0.9.1/pupa/tests/
+drwxr-xr-x   0 james      (501) staff       (20)        0 2018-10-23 14:15:55.000000 pupa-0.9.1/pupa/tests/importers/
+-rw-r--r--   0 james      (501) staff       (20)     2693 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/tests/importers/test_jurisdiction_importer.py
+-rw-r--r--   0 james      (501) staff       (20)    20331 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/tests/importers/test_vote_event_importer.py
+-rw-r--r--   0 james      (501) staff       (20)     6241 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/tests/importers/test_base_importer.py
+-rw-r--r--   0 james      (501) staff       (20)        0 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/tests/importers/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     4113 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/tests/importers/test_post_importer.py
+-rw-r--r--   0 james      (501) staff       (20)     8448 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/tests/importers/test_people_importer.py
+-rw-r--r--   0 james      (501) staff       (20)    16025 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/tests/importers/test_bill_importer.py
+-rw-r--r--   0 james      (501) staff       (20)     5398 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/tests/importers/test_topsort.py
+-rw-r--r--   0 james      (501) staff       (20)     9880 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/tests/importers/test_event_importer.py
+-rw-r--r--   0 james      (501) staff       (20)     7448 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/tests/importers/test_membership_importer.py
+-rw-r--r--   0 james      (501) staff       (20)     8742 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/tests/importers/test_organization_importer.py
+-rw-r--r--   0 james      (501) staff       (20)      470 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/tests/django_settings.py
+-rw-r--r--   0 james      (501) staff       (20)        0 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/tests/__init__.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2018-10-23 14:15:55.000000 pupa-0.9.1/pupa/tests/scrape/
+-rw-r--r--   0 james      (501) staff       (20)     6335 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/tests/scrape/test_bill_scrape.py
+-rw-r--r--   0 james      (501) staff       (20)      620 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/tests/scrape/test_utils.py
+-rw-r--r--   0 james      (501) staff       (20)     6230 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/tests/scrape/test_people_org_scrape.py
+-rw-r--r--   0 james      (501) staff       (20)     3604 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/tests/scrape/test_scraper.py
+-rw-r--r--   0 james      (501) staff       (20)        0 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/tests/scrape/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     4410 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/tests/scrape/test_model_basics.py
+-rw-r--r--   0 james      (501) staff       (20)     3363 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/tests/scrape/test_vote_event_scrape.py
+-rw-r--r--   0 james      (501) staff       (20)     2226 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/tests/scrape/test_jurisdiction_scrape.py
+-rw-r--r--   0 james      (501) staff       (20)     4651 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/tests/scrape/test_event_scrape.py
+-rw-r--r--   0 james      (501) staff       (20)       43 2018-10-23 14:15:02.000000 pupa-0.9.1/pupa/__init__.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2018-10-23 14:15:55.000000 pupa-0.9.1/pupa/utils/
+-rw-r--r--   0 james      (501) staff       (20)     1886 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/utils/generic.py
+-rw-r--r--   0 james      (501) staff       (20)      156 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/utils/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     4925 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/utils/topsort.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2018-10-23 14:15:55.000000 pupa-0.9.1/pupa/scrape/
+-rw-r--r--   0 james      (501) staff       (20)     4688 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/scrape/bill.py
+-rw-r--r--   0 james      (501) staff       (20)     4917 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/scrape/event.py
+-rw-r--r--   0 james      (501) staff       (20)      259 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/scrape/__init__.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2018-10-23 14:15:55.000000 pupa-0.9.1/pupa/scrape/schemas/
+-rw-r--r--   0 james      (501) staff       (20)     4832 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/scrape/schemas/bill.py
+-rw-r--r--   0 james      (501) staff       (20)      524 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/scrape/schemas/post.py
+-rw-r--r--   0 james      (501) staff       (20)     5651 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/scrape/schemas/event.py
+-rw-r--r--   0 james      (501) staff       (20)      783 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/scrape/schemas/person.py
+-rw-r--r--   0 james      (501) staff       (20)      988 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/scrape/schemas/organization.py
+-rw-r--r--   0 james      (501) staff       (20)        0 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/scrape/schemas/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     2187 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/scrape/schemas/common.py
+-rw-r--r--   0 james      (501) staff       (20)     1641 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/scrape/schemas/vote_event.py
+-rw-r--r--   0 james      (501) staff       (20)      832 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/scrape/schemas/membership.py
+-rw-r--r--   0 james      (501) staff       (20)      825 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/scrape/schemas/jurisdiction.py
+-rw-r--r--   0 james      (501) staff       (20)     2894 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/scrape/vote_event.py
+-rw-r--r--   0 james      (501) staff       (20)    10551 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/scrape/base.py
+-rw-r--r--   0 james      (501) staff       (20)     1990 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/scrape/jurisdiction.py
+-rw-r--r--   0 james      (501) staff       (20)     8642 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/scrape/popolo.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2018-10-23 14:15:55.000000 pupa-0.9.1/pupa/cli/
+-rw-r--r--   0 james      (501) staff       (20)        0 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/cli/__init__.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2018-10-23 14:15:55.000000 pupa-0.9.1/pupa/cli/commands/
+-rw-r--r--   0 james      (501) staff       (20)    13073 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/cli/commands/update.py
+-rw-r--r--   0 james      (501) staff       (20)        0 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/cli/commands/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     2358 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/cli/commands/dbinit.py
+-rw-r--r--   0 james      (501) staff       (20)     4980 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/cli/commands/init.py
+-rw-r--r--   0 james      (501) staff       (20)      409 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/cli/commands/base.py
+-rw-r--r--   0 james      (501) staff       (20)     1039 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/cli/commands/party.py
+-rw-r--r--   0 james      (501) staff       (20)     2419 2018-10-23 14:02:05.000000 pupa-0.9.1/pupa/cli/__main__.py
+-rw-r--r--   0 james      (501) staff       (20)     1353 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/admin.py
+-rw-r--r--   0 james      (501) staff       (20)     1944 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/settings.py
+-rw-r--r--   0 james      (501) staff       (20)     2526 2018-10-09 03:16:53.000000 pupa-0.9.1/pupa/exceptions.py
+-rw-r--r--   0 james      (501) staff       (20)      401 2018-10-09 03:16:53.000000 pupa-0.9.1/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2018-10-23 14:15:55.000000 pupa-0.9.1/pupa.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)        1 2018-10-09 03:50:21.000000 pupa-0.9.1/pupa.egg-info/not-zip-safe
+-rw-r--r--   0 james      (501) staff       (20)      664 2018-10-23 14:15:54.000000 pupa-0.9.1/pupa.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)       47 2018-10-23 14:15:54.000000 pupa-0.9.1/pupa.egg-info/entry_points.txt
+-rw-r--r--   0 james      (501) staff       (20)      177 2018-10-23 14:15:54.000000 pupa-0.9.1/pupa.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)        5 2018-10-23 14:15:54.000000 pupa-0.9.1/pupa.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)     2531 2018-10-23 14:15:54.000000 pupa-0.9.1/pupa.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2018-10-23 14:15:54.000000 pupa-0.9.1/pupa.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      124 2018-10-23 14:15:55.000000 pupa-0.9.1/setup.cfg
```

### Comparing `pupa-0.9.0/pupa/models.py` & `pupa-0.9.1/pupa/models.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/cli/commands/update.py` & `pupa-0.9.1/pupa/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/cli/commands/party.py` & `pupa-0.9.1/pupa/cli/commands/party.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/cli/commands/init.py` & `pupa-0.9.1/pupa/cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/cli/commands/dbinit.py` & `pupa-0.9.1/pupa/cli/commands/dbinit.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/cli/__main__.py` & `pupa-0.9.1/pupa/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/settings.py` & `pupa-0.9.1/pupa/settings.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/ext/ansistrm.py` & `pupa-0.9.1/pupa/ext/ansistrm.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/admin.py` & `pupa-0.9.1/pupa/admin.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/migrations/0002_auto_20150906_1458.py` & `pupa-0.9.1/pupa/migrations/0002_auto_20150906_1458.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/migrations/0001_initial.py` & `pupa-0.9.1/pupa/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/migrations/0005_auto_20170522_1935.py` & `pupa-0.9.1/pupa/migrations/0005_auto_20170522_1935.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/migrations/0006_identifier_jurisdiction.py` & `pupa-0.9.1/pupa/migrations/0006_identifier_jurisdiction.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/migrations/0003_auto_20151118_0408.py` & `pupa-0.9.1/pupa/migrations/0003_auto_20151118_0408.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/migrations/0004_identifier.py` & `pupa-0.9.1/pupa/migrations/0004_identifier.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/exceptions.py` & `pupa-0.9.1/pupa/exceptions.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/tests/importers/test_topsort.py` & `pupa-0.9.1/pupa/tests/importers/test_topsort.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/tests/importers/test_membership_importer.py` & `pupa-0.9.1/pupa/tests/importers/test_membership_importer.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/tests/importers/test_base_importer.py` & `pupa-0.9.1/pupa/tests/importers/test_base_importer.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/tests/importers/test_organization_importer.py` & `pupa-0.9.1/pupa/tests/importers/test_organization_importer.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/tests/importers/test_vote_event_importer.py` & `pupa-0.9.1/pupa/tests/importers/test_vote_event_importer.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/tests/importers/test_post_importer.py` & `pupa-0.9.1/pupa/tests/importers/test_post_importer.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/tests/importers/test_jurisdiction_importer.py` & `pupa-0.9.1/pupa/tests/importers/test_jurisdiction_importer.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/tests/importers/test_bill_importer.py` & `pupa-0.9.1/pupa/tests/importers/test_bill_importer.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/tests/importers/test_people_importer.py` & `pupa-0.9.1/pupa/tests/importers/test_people_importer.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/tests/importers/test_event_importer.py` & `pupa-0.9.1/pupa/tests/importers/test_event_importer.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/tests/scrape/test_jurisdiction_scrape.py` & `pupa-0.9.1/pupa/tests/scrape/test_jurisdiction_scrape.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/tests/scrape/test_bill_scrape.py` & `pupa-0.9.1/pupa/tests/scrape/test_bill_scrape.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/tests/scrape/test_utils.py` & `pupa-0.9.1/pupa/tests/scrape/test_utils.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/tests/scrape/test_vote_event_scrape.py` & `pupa-0.9.1/pupa/tests/scrape/test_vote_event_scrape.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/tests/scrape/test_model_basics.py` & `pupa-0.9.1/pupa/tests/scrape/test_model_basics.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/tests/scrape/test_people_org_scrape.py` & `pupa-0.9.1/pupa/tests/scrape/test_people_org_scrape.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/tests/scrape/test_event_scrape.py` & `pupa-0.9.1/pupa/tests/scrape/test_event_scrape.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/tests/scrape/test_scraper.py` & `pupa-0.9.1/pupa/tests/scrape/test_scraper.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/utils/generic.py` & `pupa-0.9.1/pupa/utils/generic.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/utils/topsort.py` & `pupa-0.9.1/pupa/utils/topsort.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/importers/bills.py` & `pupa-0.9.1/pupa/importers/bills.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/importers/posts.py` & `pupa-0.9.1/pupa/importers/posts.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/importers/memberships.py` & `pupa-0.9.1/pupa/importers/memberships.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/importers/jurisdiction.py` & `pupa-0.9.1/pupa/importers/jurisdiction.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/importers/base.py` & `pupa-0.9.1/pupa/importers/base.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/importers/organizations.py` & `pupa-0.9.1/pupa/importers/organizations.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/importers/vote_events.py` & `pupa-0.9.1/pupa/importers/vote_events.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/importers/people.py` & `pupa-0.9.1/pupa/importers/people.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/importers/events.py` & `pupa-0.9.1/pupa/importers/events.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/scrape/vote_event.py` & `pupa-0.9.1/pupa/scrape/vote_event.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/scrape/jurisdiction.py` & `pupa-0.9.1/pupa/scrape/jurisdiction.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/scrape/popolo.py` & `pupa-0.9.1/pupa/scrape/popolo.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/scrape/base.py` & `pupa-0.9.1/pupa/scrape/base.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/scrape/schemas/organization.py` & `pupa-0.9.1/pupa/scrape/schemas/organization.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/scrape/schemas/person.py` & `pupa-0.9.1/pupa/scrape/schemas/person.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/scrape/schemas/post.py` & `pupa-0.9.1/pupa/scrape/schemas/post.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/scrape/schemas/vote_event.py` & `pupa-0.9.1/pupa/scrape/schemas/vote_event.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/scrape/schemas/jurisdiction.py` & `pupa-0.9.1/pupa/scrape/schemas/jurisdiction.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/scrape/schemas/common.py` & `pupa-0.9.1/pupa/scrape/schemas/common.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/scrape/schemas/membership.py` & `pupa-0.9.1/pupa/scrape/schemas/membership.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/scrape/schemas/event.py` & `pupa-0.9.1/pupa/scrape/schemas/event.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/scrape/schemas/bill.py` & `pupa-0.9.1/pupa/scrape/schemas/bill.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/scrape/event.py` & `pupa-0.9.1/pupa/scrape/event.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa/scrape/bill.py` & `pupa-0.9.1/pupa/scrape/bill.py`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/PKG-INFO` & `pupa-0.9.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pupa
-Version: 0.9.0
+Version: 0.9.1
 Summary: scraping framework for muncipal data
 Home-page: https://github.com/opencivicdata/pupa/
 Author: James Turk
 Author-email: james@openstates.org
 License: BSD
-Description-Content-Type: UNKNOWN
 Description: UNKNOWN
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: dev
```

### Comparing `pupa-0.9.0/pupa.egg-info/SOURCES.txt` & `pupa-0.9.1/pupa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pupa-0.9.0/pupa.egg-info/PKG-INFO` & `pupa-0.9.1/pupa.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pupa
-Version: 0.9.0
+Version: 0.9.1
 Summary: scraping framework for muncipal data
 Home-page: https://github.com/opencivicdata/pupa/
 Author: James Turk
 Author-email: james@openstates.org
 License: BSD
-Description-Content-Type: UNKNOWN
 Description: UNKNOWN
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: dev
```

### Comparing `pupa-0.9.0/setup.py` & `pupa-0.9.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,24 +16,24 @@
       platforms=['any'],
       zip_safe=False,
       entry_points='''[console_scripts]
 pupa = pupa.cli.__main__:main''',
       install_requires=[
           'Django>=1.11',
           'opencivicdata>=2.1.0',
-          'dj_database_url==0.3.0',
+          'dj_database_url>=0.3.0',
           'scrapelib>=1.0',
-          'jsonschema==2.6.0',
-          'psycopg2',
+          'jsonschema>=2.6.0',
+          'psycopg2-binary',
           'pytz',
       ],
       extras_require={
           'dev': [
             'mock',
-            'pytest',
+            'pytest>=3.6',
             'pytest-cov',
             'pytest-django',
             'coveralls',
             'flake8',
           ],
       },
       classifiers=["Development Status :: 4 - Beta",
```

