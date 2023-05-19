# Comparing `tmp/m-abac-test-1.0.2.tar.gz` & `tmp/m-abac-test-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m-abac-test-1.0.2.tar", last modified: Mon May 15 09:22:40 2023, max compression
+gzip compressed data, was "m-abac-test-1.0.3.tar", last modified: Fri May 19 09:35:50 2023, max compression
```

## Comparing `m-abac-test-1.0.2.tar` & `m-abac-test-1.0.3.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:40.867016 m-abac-test-1.0.2/
--rw-r--r--   0 root         (0) root         (0)     1746 2023-05-15 09:22:40.866016 m-abac-test-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      620 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:40.807015 m-abac-test-1.0.2/m_abac_test.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1746 2023-05-15 09:22:40.000000 m-abac-test-1.0.2/m_abac_test.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3699 2023-05-15 09:22:40.000000 m-abac-test-1.0.2/m_abac_test.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 09:22:40.000000 m-abac-test-1.0.2/m_abac_test.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-15 09:22:40.000000 m-abac-test-1.0.2/m_abac_test.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-15 09:22:40.000000 m-abac-test-1.0.2/m_abac_test.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:40.797014 m-abac-test-1.0.2/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:40.797014 m-abac-test-1.0.2/mobio/libs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:40.810015 m-abac-test-1.0.2/mobio/libs/abac/
--rw-r--r--   0 root         (0) root         (0)       70 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:40.812015 m-abac-test-1.0.2/mobio/libs/abac/adapter/
--rw-r--r--   0 root         (0) root         (0)      267 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/adapter/__init__.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/adapter/adapter.py
--rw-r--r--   0 root         (0) root         (0)    15511 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/adapter/elasticsearch_adapter.py
--rw-r--r--   0 root         (0) root         (0)     8305 2023-05-15 09:21:38.000000 m-abac-test-1.0.2/mobio/libs/abac/call_api.py
--rw-r--r--   0 root         (0) root         (0)    12582 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/pdp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:40.816015 m-abac-test-1.0.2/mobio/libs/abac/policy/
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:40.819015 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      662 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:40.821015 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/boolean/
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/boolean/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1127 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/boolean/base.py
--rw-r--r--   0 root         (0) root         (0)     1107 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/boolean/check_bool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:40.828015 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/collection/
--rw-r--r--   0 root         (0) root         (0)      323 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/collection/__init__.py
--rw-r--r--   0 root         (0) root         (0)      629 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/collection/all_in.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/collection/all_not_in.py
--rw-r--r--   0 root         (0) root         (0)      638 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/collection/any_in.py
--rw-r--r--   0 root         (0) root         (0)      664 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/collection/any_not_in.py
--rw-r--r--   0 root         (0) root         (0)     1341 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/collection/base.py
--rw-r--r--   0 root         (0) root         (0)      754 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/collection/is_empty.py
--rw-r--r--   0 root         (0) root         (0)      602 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/collection/is_in.py
--rw-r--r--   0 root         (0) root         (0)      774 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/collection/is_not_empty.py
--rw-r--r--   0 root         (0) root         (0)      728 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/collection/is_not_in.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:40.835015 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/date_time/
--rw-r--r--   0 root         (0) root         (0)      243 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/date_time/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2520 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/date_time/base.py
--rw-r--r--   0 root         (0) root         (0)     1345 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/date_time/date_eq.py
--rw-r--r--   0 root         (0) root         (0)     1367 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/date_time/date_gt.py
--rw-r--r--   0 root         (0) root         (0)     1389 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/date_time/date_gte.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/date_time/date_lt.py
--rw-r--r--   0 root         (0) root         (0)     1380 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/date_time/date_lte.py
--rw-r--r--   0 root         (0) root         (0)     1363 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/date_time/date_neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:40.841015 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/day/
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/day/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1839 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/day/base.py
--rw-r--r--   0 root         (0) root         (0)     1004 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/day/day_eq.py
--rw-r--r--   0 root         (0) root         (0)      975 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/day/day_gt.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/day/day_gte.py
--rw-r--r--   0 root         (0) root         (0)      974 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/day/day_lt.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/day/day_lte.py
--rw-r--r--   0 root         (0) root         (0)      978 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/day/day_neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:40.844015 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/ip_address/
--rw-r--r--   0 root         (0) root         (0)       82 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/ip_address/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/ip_address/base.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:40.850015 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/numeric/
--rw-r--r--   0 root         (0) root         (0)      188 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/numeric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1450 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/numeric/base.py
--rw-r--r--   0 root         (0) root         (0)      853 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/numeric/eq.py
--rw-r--r--   0 root         (0) root         (0)      871 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/numeric/gt.py
--rw-r--r--   0 root         (0) root         (0)      895 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/numeric/gte.py
--rw-r--r--   0 root         (0) root         (0)      863 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/numeric/lt.py
--rw-r--r--   0 root         (0) root         (0)      886 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/numeric/lte.py
--rw-r--r--   0 root         (0) root         (0)      869 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/numeric/neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:40.854016 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/others/
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/others/__init__.py
--rw-r--r--   0 root         (0) root         (0)      963 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/others/base.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/others/exists.py
--rw-r--r--   0 root         (0) root         (0)      701 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/others/not_exists.py
--rw-r--r--   0 root         (0) root         (0)     2126 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:22:40.865016 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/string/
--rw-r--r--   0 root         (0) root         (0)      401 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/string/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/string/base.py
--rw-r--r--   0 root         (0) root         (0)     1213 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/string/contains.py
--rw-r--r--   0 root         (0) root         (0)     1245 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/string/ends_with.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/string/equals.py
--rw-r--r--   0 root         (0) root         (0)     1227 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/string/not_contains.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/string/not_ends_with.py
--rw-r--r--   0 root         (0) root         (0)     1214 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/string/not_equals.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/string/not_starts_with.py
--rw-r--r--   0 root         (0) root         (0)     1498 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/string/regex_match.py
--rw-r--r--   0 root         (0) root         (0)     1264 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/string/starts_with.py
--rw-r--r--   0 root         (0) root         (0)     1601 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     5812 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/policy.py
--rw-r--r--   0 root         (0) root         (0)     5139 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/policy/utils.py
--rw-r--r--   0 root         (0) root         (0)     2762 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/mobio/libs/abac/result_access.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-15 08:15:49.000000 m-abac-test-1.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 09:22:40.867016 m-abac-test-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     9779 2023-05-15 09:22:40.000000 m-abac-test-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.055878 m-abac-test-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-05-19 09:35:50.054878 m-abac-test-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      620 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.005876 m-abac-test-1.0.3/m_abac_test.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-05-19 09:35:49.000000 m-abac-test-1.0.3/m_abac_test.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3699 2023-05-19 09:35:49.000000 m-abac-test-1.0.3/m_abac_test.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 09:35:49.000000 m-abac-test-1.0.3/m_abac_test.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-05-19 09:35:49.000000 m-abac-test-1.0.3/m_abac_test.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-19 09:35:49.000000 m-abac-test-1.0.3/m_abac_test.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:49.996876 m-abac-test-1.0.3/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:49.996876 m-abac-test-1.0.3/mobio/libs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.007876 m-abac-test-1.0.3/mobio/libs/abac/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.009876 m-abac-test-1.0.3/mobio/libs/abac/adapter/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/adapter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/adapter/adapter.py
+-rw-r--r--   0 root         (0) root         (0)    15511 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/adapter/elasticsearch_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     8301 2023-05-19 09:33:30.000000 m-abac-test-1.0.3/mobio/libs/abac/call_api.py
+-rw-r--r--   0 root         (0) root         (0)    12709 2023-05-19 09:33:30.000000 m-abac-test-1.0.3/mobio/libs/abac/pdp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.012877 m-abac-test-1.0.3/mobio/libs/abac/policy/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.014876 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      662 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.016877 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/boolean/
+-rw-r--r--   0 root         (0) root         (0)       39 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/boolean/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/boolean/base.py
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/boolean/check_bool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.023877 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/
+-rw-r--r--   0 root         (0) root         (0)      323 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      629 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/all_in.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/all_not_in.py
+-rw-r--r--   0 root         (0) root         (0)      638 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/any_in.py
+-rw-r--r--   0 root         (0) root         (0)      664 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/any_not_in.py
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/base.py
+-rw-r--r--   0 root         (0) root         (0)      754 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/is_empty.py
+-rw-r--r--   0 root         (0) root         (0)      602 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/is_in.py
+-rw-r--r--   0 root         (0) root         (0)      774 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/is_not_empty.py
+-rw-r--r--   0 root         (0) root         (0)      728 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/is_not_in.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.030877 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/
+-rw-r--r--   0 root         (0) root         (0)      243 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2023-05-19 09:33:30.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/base.py
+-rw-r--r--   0 root         (0) root         (0)     1345 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_eq.py
+-rw-r--r--   0 root         (0) root         (0)     1367 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_gt.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_gte.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_lt.py
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_lte.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.035877 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/base.py
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/day_eq.py
+-rw-r--r--   0 root         (0) root         (0)      975 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/day_gt.py
+-rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/day_gte.py
+-rw-r--r--   0 root         (0) root         (0)      974 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/day_lt.py
+-rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/day_lte.py
+-rw-r--r--   0 root         (0) root         (0)      978 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/day_neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.038877 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/ip_address/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/ip_address/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/ip_address/base.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.043877 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/
+-rw-r--r--   0 root         (0) root         (0)      188 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/base.py
+-rw-r--r--   0 root         (0) root         (0)      853 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/eq.py
+-rw-r--r--   0 root         (0) root         (0)      871 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/gt.py
+-rw-r--r--   0 root         (0) root         (0)      895 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/gte.py
+-rw-r--r--   0 root         (0) root         (0)      863 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/lt.py
+-rw-r--r--   0 root         (0) root         (0)      886 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/lte.py
+-rw-r--r--   0 root         (0) root         (0)      869 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.045877 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/others/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/others/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      963 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/others/base.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/others/exists.py
+-rw-r--r--   0 root         (0) root         (0)      701 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/others/not_exists.py
+-rw-r--r--   0 root         (0) root         (0)     2126 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.053878 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/
+-rw-r--r--   0 root         (0) root         (0)      401 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/base.py
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/contains.py
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/ends_with.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/equals.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/not_contains.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/not_ends_with.py
+-rw-r--r--   0 root         (0) root         (0)     1214 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/not_equals.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/not_starts_with.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/regex_match.py
+-rw-r--r--   0 root         (0) root         (0)     1264 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/starts_with.py
+-rw-r--r--   0 root         (0) root         (0)     1601 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     6037 2023-05-19 09:33:30.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/policy.py
+-rw-r--r--   0 root         (0) root         (0)     5139 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3631 2023-05-19 09:33:30.000000 m-abac-test-1.0.3/mobio/libs/abac/result_access.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 09:35:50.055878 m-abac-test-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9779 2023-05-19 09:35:49.000000 m-abac-test-1.0.3/setup.py
```

### Comparing `m-abac-test-1.0.2/PKG-INFO` & `m-abac-test-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abac-test
-Version: 1.0.2
+Version: 1.0.3
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: ### ABAC Engine
```

### Comparing `m-abac-test-1.0.2/README.md` & `m-abac-test-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/m_abac_test.egg-info/PKG-INFO` & `m-abac-test-1.0.3/m_abac_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abac-test
-Version: 1.0.2
+Version: 1.0.3
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: ### ABAC Engine
```

### Comparing `m-abac-test-1.0.2/m_abac_test.egg-info/SOURCES.txt` & `m-abac-test-1.0.3/m_abac_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/adapter/elasticsearch_adapter.py` & `m-abac-test-1.0.3/mobio/libs/abac/adapter/elasticsearch_adapter.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/call_api.py` & `m-abac-test-1.0.3/mobio/libs/abac/call_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,16 +136,16 @@
         try:
             url = APIRequest.ADMIN_GET_LIST_STATEMENT.format(domain=Mobio.ADMIN_HOST)
             authorization = Mobio.MOBIO_TOKEN
             body_req = {
                 'user_ids': [account_id],
                 'team_ids': [],
                 'merchant_ids': [merchant_id],
-                'resources': [service + ":" + resource],
-                'actions': [resource + ":" + action]
+                'resources': service + ":" + resource,
+                'actions': resource + ":" + action
             }
             data_res = requests.post(
                 url,
                 json=body_req,
                 headers={
                     "Authorization": authorization,
                     "X-Merchant-ID": merchant_id,
```

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/pdp.py` & `m-abac-test-1.0.3/mobio/libs/abac/pdp.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,14 +218,15 @@
                             })
                             continue
                     else:
                         # nếu ko có field nào ở cấu hình policy nằm trong dữ liệu gửi lên thì cho qua
                         if statement.get("check_field") and statement.get("fields"):
                             if not Utils.field_in_body_request(statement.get("fields"), self.data_after):
                                 continue
+                    self.result_access.add_log_deny(statement)
                     result_deny = True
                     break
         except Exception as err:
             print("check_list_statement_is_deny err: {}".format(err))
             result_deny = False
         return result_deny
 
@@ -233,14 +234,15 @@
         result_allow = False
         try:
             for statement in list_statement:
                 statement["request_access"] = self.request_access
                 policy_schema = PolicySchema().load(statement)
                 if policy_schema.is_allowed():
                     result_allow = True
+                    self.result_access.add_log_allow(statement)
                     if self.access_level == PolicyDecisionPoint.AccessLevel.READ:
                         # tìm tất cả các cấu hình ẩn hiện field nếu có
                         if statement.get("fields"):
                             self.result_access.add_display_config({
                                 "effect": statement.get("effect"),
                                 "fields": statement.get("fields"),
                             })
```

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/base.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/boolean/base.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/boolean/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/boolean/check_bool.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/boolean/check_bool.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/collection/all_in.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/all_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/collection/all_not_in.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/all_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/collection/any_in.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/any_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/collection/any_not_in.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/any_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/collection/base.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/collection/is_empty.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/is_empty.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/collection/is_in.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/is_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/collection/is_not_empty.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/is_not_empty.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/collection/is_not_in.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/is_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/date_time/base.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 class DateCondition(ConditionBase, metaclass=ABCMeta):
     """
         Base class for string conditions
     """
 
     class DateFormat:
-        ISO_FORMAT = "%Y-%m-%d %H:%M:%S"
+        ISO_FORMAT = "%Y-%m-%dT%H:%M:%S.%sZ"
 
     def __init__(self, values, what, date_format=DateFormat.ISO_FORMAT, qualifier=ConditionBase.Qualifier.ForAnyValue, **kwargs):
         self.values = values
         self.what = what
         self.qualifier = qualifier
         self.date_format = date_format
```

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/date_time/date_eq.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/date_time/date_gt.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/date_time/date_gte.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/date_time/date_lt.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/date_time/date_lte.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/date_time/date_neq.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/day/base.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/day/day_eq.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/day_eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/day/day_gt.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/day_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/day/day_gte.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/day_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/day/day_lt.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/day_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/day/day_lte.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/day_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/day/day_neq.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/day_neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/ip_address/base.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/ip_address/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/numeric/base.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/numeric/eq.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/numeric/gt.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/numeric/gte.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/numeric/lt.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/numeric/lte.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/numeric/neq.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/others/base.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/others/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/others/exists.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/others/exists.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/others/not_exists.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/others/not_exists.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/schema.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/schema.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/string/base.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/string/contains.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/string/ends_with.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/ends_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/string/equals.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/equals.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/string/not_contains.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/not_contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/string/not_ends_with.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/not_ends_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/string/not_equals.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/not_equals.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/string/not_starts_with.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/not_starts_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/string/regex_match.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/regex_match.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/conditions/string/starts_with.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/starts_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/exceptions.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/exceptions.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/policy.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/policy.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,22 +16,22 @@
     """
         Policy class containing rules and targets
     """
 
     def __init__(
             self,
             effect: str,
-            action: list,
-            resource: list,
+            # action: list,
+            # resource: list,
             condition: dict,
             request_access: dict, **kwargs
     ):
         self.effect = effect
-        self.action = action
-        self.resource = resource
+        # self.action = action
+        # self.resource = resource
         self.condition = condition
         self.request_access = request_access
 
     def is_allowed(self):
         conditions = self.convert_condition()
         for condition in conditions:
             # print("condition: ", condition)
@@ -70,15 +70,19 @@
                 if what_check is None:
                     if if_exists:
                         have_condition_exclude = True
                         continue
                     raise GetValueNoneException("{} get value is None".format(cond_schema.get("field")))
                 values = []
                 for v in cond_schema.get("values"):
-                    values.append(self.get_value_from_variable(v))
+                    value_from_variable = self.get_value_from_variable(v)
+                    if isinstance(value_from_variable, list):
+                        values.extend(value_from_variable)
+                    else:
+                        values.append(value_from_variable)
                 list_condition.append({
                     **item,
                     "values": values,
                     "what": what_check,
                 })
         # if len(list_condition) == 0 and not have_condition_exclude:
         #     raise EmptyConditionException("no condition found")
@@ -128,16 +132,16 @@
 
 
 class PolicySchema(Schema):
     """
         JSON schema for policy
     """
     effect = fields.String(required=True, validate=validate.OneOf([AccessType.DENY_ACCESS, AccessType.ALLOW_ACCESS]))
-    action = fields.List(fields.String(required=True, allow_none=False),required=True, allow_none=False)
-    resource = fields.List(fields.String(required=True, allow_none=False),required=True, allow_none=False)
+    # action = fields.List(fields.String(required=True, allow_none=False),required=True, allow_none=False)
+    # resource = fields.List(fields.String(required=True, allow_none=False),required=True, allow_none=False)
     condition = fields.List(fields.Raw(required=True, allow_none=False), required=True, allow_none=False)
     request_access = fields.Dict(default={}, missing={}, allow_none=False)
 
     class Meta:
         unknown = EXCLUDE
 
     @post_load
```

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/policy/utils.py` & `m-abac-test-1.0.3/mobio/libs/abac/policy/utils.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.2/mobio/libs/abac/result_access.py` & `m-abac-test-1.0.3/mobio/libs/abac/result_access.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 class ResultAccess:
     def __init__(self):
         self.allow_access = False
         self.display_config = []
         self.filter_config = []
+        self.log_statement_deny = []
+        self.log_statement_allow = []
 
     def get_allow_access(self):
+        if self.allow_access:
+            print("statement_allow: {}".format(self.log_statement_allow))
+        else:
+            print("statement_deny: {}".format(self.log_statement_deny))
+
         return self.allow_access
 
     def set_allow_access(self, value: bool):
         self.allow_access = value
 
     def get_filter_config(self):
         """
@@ -69,7 +76,23 @@
         items = key_filter.split("#")
         return {
             "effect": items[0],
             "operator": items[1],
             "field": items[2],
             "qualifier": items[3],
         }
+    @classmethod
+    def convert_data_save_log(cls, value):
+        return {
+            'merchant_id': value.get('merchant_id'),
+            'policy_code': value.get('policy_code'),
+            'statement_id': value.get('statement_id'),
+            'effect': value.get('effect'),
+            'action': value.get('action'),
+            'resource': value.get('resource'),
+        }
+
+    def add_log_deny(self, value):
+        self.log_statement_deny.append(self.convert_data_save_log(value))
+
+    def add_log_allow(self, value):
+        self.log_statement_allow.append(self.convert_data_save_log(value))
```

### Comparing `m-abac-test-1.0.2/setup.py` & `m-abac-test-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         ]
         # with open(Requirements.requirements_path) as req_file:
         #     for line in req_file.read().splitlines():
         #         if not line.strip().startswith("#"):
         #             requirements.append(line)
         return requirements
 
-version_dev='1.0.2'
+version_dev='1.0.3'
 version_prod='1.0.0'
 
 run_mode='-test'
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
@@ -70,15 +70,15 @@
     # options={"bdist_wheel": {"universal": True}},
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.2',  # Required
+    version='1.0.3',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

