# Comparing `tmp/hollihop_api_client-0.0.5.tar.gz` & `tmp/hollihop_api_client-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hollihop_api_client-0.0.5.tar", last modified: Thu May 18 12:20:59 2023, max compression
+gzip compressed data, was "hollihop_api_client-0.0.6.tar", last modified: Fri May 19 07:29:06 2023, max compression
```

## Comparing `hollihop_api_client-0.0.5.tar` & `hollihop_api_client-0.0.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 12:20:59.577074 hollihop_api_client-0.0.5/
--rw-r--r--   0 malts.tech   (501) staff       (20)     1073 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.5/LICENSE
--rw-r--r--   0 malts.tech   (501) staff       (20)     2401 2023-05-18 12:20:59.576937 hollihop_api_client-0.0.5/PKG-INFO
--rw-r--r--   0 malts.tech   (501) staff       (20)     1753 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.5/README.md
--rw-r--r--   0 malts.tech   (501) staff       (20)      716 2023-05-18 12:20:50.000000 hollihop_api_client-0.0.5/pyproject.toml
--rw-r--r--   0 malts.tech   (501) staff       (20)       38 2023-05-18 12:20:59.577110 hollihop_api_client-0.0.5/setup.cfg
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 12:20:59.568555 hollihop_api_client-0.0.5/src/
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 12:20:59.570217 hollihop_api_client-0.0.5/src/hollihop_api_client/
--rw-r--r--   0 malts.tech   (501) staff       (20)       94 2023-05-18 11:24:48.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/__init__.py
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 12:20:59.571833 hollihop_api_client-0.0.5/src/hollihop_api_client/api/
--rw-r--r--   0 malts.tech   (501) staff       (20)      138 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/api/__init__.py
--rw-r--r--   0 malts.tech   (501) staff       (20)      594 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/api/abc.py
--rw-r--r--   0 malts.tech   (501) staff       (20)     2667 2023-05-18 12:10:40.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/api/api.py
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 12:20:59.572280 hollihop_api_client-0.0.5/src/hollihop_api_client/base/
--rw-r--r--   0 malts.tech   (501) staff       (20)       63 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/base/__init__.py
--rw-r--r--   0 malts.tech   (501) staff       (20)      520 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/base/category.py
--rw-r--r--   0 malts.tech   (501) staff       (20)      836 2023-05-18 12:18:20.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/categories.py
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 12:20:59.573241 hollihop_api_client-0.0.5/src/hollihop_api_client/methods/
--rw-r--r--   0 malts.tech   (501) staff       (20)      315 2023-05-18 12:16:07.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/methods/__init__.py
--rw-r--r--   0 malts.tech   (501) staff       (20)     6766 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/methods/ed_unit_students.py
--rw-r--r--   0 malts.tech   (501) staff       (20)     6434 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/methods/ed_units.py
--rw-r--r--   0 malts.tech   (501) staff       (20)     2765 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/methods/leads.py
--rw-r--r--   0 malts.tech   (501) staff       (20)     1303 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/methods/locations.py
--rw-r--r--   0 malts.tech   (501) staff       (20)     1611 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/methods/offices.py
--rw-r--r--   0 malts.tech   (501) staff       (20)     1436 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/test.py
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 12:20:59.574627 hollihop_api_client-0.0.5/src/hollihop_api_client/tests/
--rw-r--r--   0 malts.tech   (501) staff       (20)        0 2023-03-11 10:01:33.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/tests/__init__.py
--rw-r--r--   0 malts.tech   (501) staff       (20)     1528 2023-03-12 11:14:09.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/tests/conftest.py
--rw-r--r--   0 malts.tech   (501) staff       (20)      474 2023-03-12 18:14:57.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/tests/test_ed_unit_students.py
--rw-r--r--   0 malts.tech   (501) staff       (20)      995 2023-03-12 11:19:09.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/tests/test_ed_units.py
--rw-r--r--   0 malts.tech   (501) staff       (20)      165 2023-03-12 11:17:10.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/tests/test_lead.py
--rw-r--r--   0 malts.tech   (501) staff       (20)      374 2023-03-12 11:16:33.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/tests/test_locations.py
--rw-r--r--   0 malts.tech   (501) staff       (20)      636 2023-03-12 11:15:54.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/tests/test_offices.py
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 12:20:59.574808 hollihop_api_client-0.0.5/src/hollihop_api_client/tools/
--rw-r--r--   0 malts.tech   (501) staff       (20)     3143 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/tools/__init__.py
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 12:20:59.569047 hollihop_api_client-0.0.5/src/hollihop_api_client/venv/
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 12:20:59.576752 hollihop_api_client-0.0.5/src/hollihop_api_client/venv/bin/
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      673 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/venv/bin/rst2html.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      795 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/venv/bin/rst2html4.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)     1130 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/venv/bin/rst2html5.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      872 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/venv/bin/rst2latex.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      695 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/venv/bin/rst2man.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      861 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/venv/bin/rst2odt.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      667 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      680 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      716 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/venv/bin/rst2s5.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      952 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/venv/bin/rst2xetex.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      681 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/venv/bin/rst2xml.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      749 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.5/src/hollihop_api_client/venv/bin/rstpep2html.py
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 12:20:59.570815 hollihop_api_client-0.0.5/src/hollihop_api_client.egg-info/
--rw-r--r--   0 malts.tech   (501) staff       (20)     2401 2023-05-18 12:20:59.000000 hollihop_api_client-0.0.5/src/hollihop_api_client.egg-info/PKG-INFO
--rw-r--r--   0 malts.tech   (501) staff       (20)     1709 2023-05-18 12:20:59.000000 hollihop_api_client-0.0.5/src/hollihop_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 malts.tech   (501) staff       (20)        1 2023-05-18 12:20:59.000000 hollihop_api_client-0.0.5/src/hollihop_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 malts.tech   (501) staff       (20)       20 2023-05-18 12:20:59.000000 hollihop_api_client-0.0.5/src/hollihop_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-19 07:29:06.755087 hollihop_api_client-0.0.6/
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1073 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.6/LICENSE
+-rw-r--r--   0 malts.tech   (501) staff       (20)     2401 2023-05-19 07:29:06.754950 hollihop_api_client-0.0.6/PKG-INFO
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1753 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.6/README.md
+-rw-r--r--   0 malts.tech   (501) staff       (20)      791 2023-05-19 07:28:56.000000 hollihop_api_client-0.0.6/pyproject.toml
+-rw-r--r--   0 malts.tech   (501) staff       (20)       38 2023-05-19 07:29:06.755125 hollihop_api_client-0.0.6/setup.cfg
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-19 07:29:06.749663 hollihop_api_client-0.0.6/src/
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-19 07:29:06.750682 hollihop_api_client-0.0.6/src/hollihop_api_client/
+-rw-r--r--   0 malts.tech   (501) staff       (20)       94 2023-05-18 11:24:48.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/__init__.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-19 07:29:06.751605 hollihop_api_client-0.0.6/src/hollihop_api_client/api/
+-rw-r--r--   0 malts.tech   (501) staff       (20)      138 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/api/__init__.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      598 2023-05-19 07:20:27.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/api/abc.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     2542 2023-05-19 07:22:09.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/api/api.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-19 07:29:06.751863 hollihop_api_client-0.0.6/src/hollihop_api_client/base/
+-rw-r--r--   0 malts.tech   (501) staff       (20)       63 2023-05-19 06:42:36.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/base/__init__.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      540 2023-05-19 06:42:33.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/base/category.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      936 2023-05-19 07:22:58.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/categories.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-19 07:29:06.752511 hollihop_api_client-0.0.6/src/hollihop_api_client/methods/
+-rw-r--r--   0 malts.tech   (501) staff       (20)      315 2023-05-18 12:16:07.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/methods/__init__.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     6845 2023-05-19 07:20:27.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/methods/ed_unit_students.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     6500 2023-05-19 07:20:27.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/methods/ed_units.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     2824 2023-05-19 07:20:27.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/methods/leads.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1320 2023-05-19 07:20:27.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/methods/locations.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1628 2023-05-19 07:20:27.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/methods/offices.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-19 07:29:06.753294 hollihop_api_client-0.0.6/src/hollihop_api_client/tests/
+-rw-r--r--   0 malts.tech   (501) staff       (20)        0 2023-03-11 10:01:33.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/tests/__init__.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1527 2023-05-19 07:20:27.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/tests/conftest.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      474 2023-03-12 18:14:57.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/tests/test_ed_unit_students.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      995 2023-03-12 11:19:09.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/tests/test_ed_units.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      165 2023-03-12 11:17:10.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/tests/test_lead.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      374 2023-03-12 11:16:33.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/tests/test_locations.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      636 2023-03-12 11:15:54.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/tests/test_offices.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-19 07:29:06.753397 hollihop_api_client-0.0.6/src/hollihop_api_client/tools/
+-rw-r--r--   0 malts.tech   (501) staff       (20)     3142 2023-05-19 07:20:27.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/tools/__init__.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-19 07:29:06.750111 hollihop_api_client-0.0.6/src/hollihop_api_client/venv/
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-19 07:29:06.754780 hollihop_api_client-0.0.6/src/hollihop_api_client/venv/bin/
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      673 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/venv/bin/rst2html.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      795 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/venv/bin/rst2html4.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)     1130 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/venv/bin/rst2html5.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      872 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/venv/bin/rst2latex.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      695 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/venv/bin/rst2man.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      861 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/venv/bin/rst2odt.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      667 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      680 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      716 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/venv/bin/rst2s5.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      952 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      681 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/venv/bin/rst2xml.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      749 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.6/src/hollihop_api_client/venv/bin/rstpep2html.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-19 07:29:06.751235 hollihop_api_client-0.0.6/src/hollihop_api_client.egg-info/
+-rw-r--r--   0 malts.tech   (501) staff       (20)     2401 2023-05-19 07:29:06.000000 hollihop_api_client-0.0.6/src/hollihop_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1723 2023-05-19 07:29:06.000000 hollihop_api_client-0.0.6/src/hollihop_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 malts.tech   (501) staff       (20)        1 2023-05-19 07:29:06.000000 hollihop_api_client-0.0.6/src/hollihop_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 malts.tech   (501) staff       (20)       38 2023-05-19 07:29:06.000000 hollihop_api_client-0.0.6/src/hollihop_api_client.egg-info/requires.txt
+-rw-r--r--   0 malts.tech   (501) staff       (20)       20 2023-05-19 07:29:06.000000 hollihop_api_client-0.0.6/src/hollihop_api_client.egg-info/top_level.txt
```

### Comparing `hollihop_api_client-0.0.5/LICENSE` & `hollihop_api_client-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.5/PKG-INFO` & `hollihop_api_client-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hollihop_api_client
-Version: 0.0.5
+Version: 0.0.6
 Summary: This library helps you easily create a python application with Hollihop API
 Author-email: Nicholas Maltseb <nmmaltsev@outlook.com>
 Project-URL: Homepage, https://github.com/nicholasChieftain/hollihop_api_client/
 Project-URL: Bug Tracker, https://github.com/nicholasChieftain/hollihop_api_client/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `hollihop_api_client-0.0.5/README.md` & `hollihop_api_client-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.5/pyproject.toml` & `hollihop_api_client-0.0.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hollihop_api_client"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Nicholas Maltseb", email="nmmaltsev@outlook.com" },
 ]
 description = "This library helps you easily create a python application with Hollihop API"
 readme = "README.md"
 requires-python = ">=3.10"
+dependencies = [
+    'phonenumbers >= 8.3.11',
+    'requests >= 2.30.0',
+]
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
     "Operating System :: MacOS",
     "Operating System :: POSIX :: Linux"
 ]
```

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client/api/abc.py` & `hollihop_api_client-0.0.6/src/hollihop_api_client/api/abc.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from abc import ABC, abstractmethod
-from typing import NoReturn, TYPE_CHECKING
+from typing import TYPE_CHECKING, NoReturn
 
 if TYPE_CHECKING:
     from requests import Response
 
-from categories import APICategories
+from hollihop_api_client.categories import APICategories
 
 
 class AbstractAPI(ABC, APICategories):
     @abstractmethod
     def request(
             self,
             method: str,
             http_method: str = 'GET',
             data: None | dict = None,
-            ) -> None | dict:
+    ) -> None | dict:
         pass
 
     @abstractmethod
     def _validate_response(
             self,
             response: "Response"
-            ) -> (None | dict) | NoReturn:
+    ) -> (None | dict) | NoReturn:
         pass
 
 
 __all__ = ['AbstractAPI']
```

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client/api/api.py` & `hollihop_api_client-0.0.6/src/hollihop_api_client/api/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from typing import NoReturn, TYPE_CHECKING
 
 from requests import Response, Session, get
 
-from hollihop_api_client.categories import APICategories
-
 from .abc import AbstractAPI
 
 
 class HolliHopAPIError(Exception):
     _response_not_ok = '''Запрос к {url} не выполнен.
     Статус код {status_code}.
     {error_message}'''
@@ -37,30 +35,29 @@
 
 
 class HolliHopAPI(AbstractAPI):
     __api_version__ = 'Api/V2/'
 
     def __init__(
             self,
-            domain: str = None,
-            api_key: str = None
+            domain: str | None = None,
+            api_key: str | None = None
     ):
         if api_key is None:
             raise HolliHopAPIError(
                 error_message='Не указан ключ доступа к API'
             )
         if domain is None:
             raise HolliHopAPIError(
                 error_message='Не указан домен для доступа к API'
             )
         self._domain = domain
         self._api_key = api_key
 
         super().__init__(self)
-        self.categories = APICategories(self)
 
     def request(
             self,
             method: str,
             http_method: str = 'GET',
             data: dict | None = None
     ) -> None | dict:
@@ -80,15 +77,14 @@
     def _validate_response(
             self,
             response: Response,
     ) -> (None | dict) | NoReturn:
         if response.status_code == 200:
             return response.json()
         else:
-            print(response.json())
             raise HolliHopAPIError(
                 response.url,
                 response.status_code,
                 'Ошибка выполнения запроса'
             )
```

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client/base/category.py` & `hollihop_api_client-0.0.6/src/hollihop_api_client/base/category.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from api import AbstractAPI
+    from hollihop_api_client.api import AbstractAPI
 
 
 class BaseCategory:
     def __init__(self, api: 'AbstractAPI'):
         self.api = api
 
     @classmethod
```

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client/categories.py` & `hollihop_api_client-0.0.6/src/hollihop_api_client/categories.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-from methods import (
-    LocationsCategory,
-    OfficesCategory,
-    EdUnitsCategory,
-    StudentsCategory,
-    LeadsCategory
-)
-
 from typing import TYPE_CHECKING
 
+from hollihop_api_client.methods import (EdUnitsCategory, LeadsCategory,
+                                         LocationsCategory, OfficesCategory,
+                                         StudentsCategory)
+
 if TYPE_CHECKING:
-    from api import AbstractAPI
+    from hollihop_api_client.api import AbstractAPI
 
 
 class APICategories:
     def __init__(self, api: 'AbstractAPI'):
         self.api = api
 
     @property
```

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client/methods/ed_unit_students.py` & `hollihop_api_client-0.0.6/src/hollihop_api_client/methods/ed_unit_students.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-from base import BaseCategory
-from typing import TYPE_CHECKING, Any
-import phonenumbers
-
 from dataclasses import dataclass, field
-from datetime import datetime, time, date, timedelta
+from datetime import date, datetime, time, timedelta
+from typing import TYPE_CHECKING, Any
 
-from methods.ed_units import EdUnit
+import phonenumbers
 
-from tools import dict_to_camel, dict_to_snake
+from hollihop_api_client.base import BaseCategory
+from hollihop_api_client.methods.ed_units import EdUnit
+from hollihop_api_client.tools import dict_to_camel, dict_to_snake
 
 if TYPE_CHECKING:
-    from api import AbstractAPI
+    from hollihop_api_client.api import AbstractAPI
 
 
 def replace_spaces(from_str: str):
     return from_str.replace('\xa0', ' ')
 
 
 @dataclass
```

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client/methods/ed_units.py` & `hollihop_api_client-0.0.6/src/hollihop_api_client/methods/ed_units.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-from pprint import pprint
-
-from base import BaseCategory
-from typing import TYPE_CHECKING, Any, List
-
 from dataclasses import dataclass, field
 from datetime import datetime, time
+from typing import TYPE_CHECKING, Any, List
 
-from tools import dict_to_camel, dict_to_snake
+from hollihop_api_client.base import BaseCategory
+from hollihop_api_client.tools import dict_to_camel, dict_to_snake
 
 if TYPE_CHECKING:
-    from api import AbstractAPI
+    from hollihop_api_client.api import AbstractAPI
 
 
 @dataclass
 class ScheduleItem:
     begin_date: None | datetime = None
     begin_time: None | str = None
     classroom_id: None | int = None
@@ -133,21 +130,23 @@
     fiscal_info: FiscalInfo | list = None
     teacher_prices: None | list[TeacherPrice] = None
     price_values: None | list = None
     assignee: None | dict = None
 
     def __post_init__(self):
         if not self.schedule_items is None:
-            self.schedule_items = [ScheduleItem(**_) for _ in self.schedule_items]
+            self.schedule_items = [ScheduleItem(
+                **_) for _ in self.schedule_items]
         if not self.days is None:
             self.days = [Day(**_) for _ in self.days]
         if not self.fiscal_info is None:
             self.fiscal_info = FiscalInfo(**self.fiscal_info)
         if not self.teacher_prices is None:
-            self.teacher_prices = [TeacherPrice(**_) for _ in self.teacher_prices]
+            self.teacher_prices = [TeacherPrice(
+                **_) for _ in self.teacher_prices]
 
 
 @dataclass(frozen=True)
 class Statuses:
     Reserve = 'Reserve'
     Forming = 'Forming'
     Working = 'Working'
```

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client/methods/leads.py` & `hollihop_api_client-0.0.6/src/hollihop_api_client/methods/leads.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from base import BaseCategory
-from typing import TYPE_CHECKING, Any
-
 from dataclasses import dataclass, field
 from datetime import datetime
+from typing import TYPE_CHECKING, Any
 
-from tools import dict_to_camel, dict_to_snake
+from hollihop_api_client.base import BaseCategory
+from hollihop_api_client.tools import dict_to_camel, dict_to_snake
 
 if TYPE_CHECKING:
-    from api import AbstractAPI
+    from hollihop_api_client.api import AbstractAPI
 
 
 @dataclass
 class Agent:
     first_name: str | None = None
     last_name: str | None = None
     is_customer: bool | None = None
```

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client/methods/locations.py` & `hollihop_api_client-0.0.6/src/hollihop_api_client/methods/locations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,55 +1,53 @@
-from base import BaseCategory
-from typing import TYPE_CHECKING, Any
-
 from dataclasses import dataclass, field
+from typing import TYPE_CHECKING, Any
 
-from tools import dict_to_camel, dict_to_snake
+from hollihop_api_client.base import BaseCategory
+from hollihop_api_client.tools import dict_to_camel, dict_to_snake
 
 if TYPE_CHECKING:
-    from api import AbstractAPI
+    from hollihop_api_client.api import AbstractAPI
 
 
 @dataclass
 class Location:
     id: None | int
     name: None | str
 
 
-@dataclass 
+@dataclass
 class Locations:
     locations: list[Location] = field(default_factory=list)
 
 
 class LocationsCategory(BaseCategory):
 
     def __init__(self, api: 'AbstractAPI'):
         self.api = api
 
     def get_locations(
             self,
             id: None | int = None,
             name: None | str = None
-            ) -> list[Location]:
+    ) -> list[Location]:
         data = dict_to_camel(self.handle_parameters(locals()))
 
         response = self.api.request(
-                method='GetLocations',
-                http_method='GET',
-                data=data
-                )
+            method='GetLocations',
+            http_method='GET',
+            data=data
+        )
 
         response = dict_to_snake(response)
 
         return [Location(**_) for _ in Locations(**response).locations]
-    
+
     def get_all_locations_name(self) -> list[str]:
         locations = self.get_locations()
         return [location.name for location in locations]
 
     def get_all_locations_id(self) -> list[int]:
         locations = self.get_locations()
         return [location.id for location in locations]
 
 
 __all__ = ['LocationsCategory']
-
```

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client/methods/offices.py` & `hollihop_api_client-0.0.6/src/hollihop_api_client/methods/offices.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from base import BaseCategory
-from typing import TYPE_CHECKING, Any
-
 from dataclasses import dataclass, field
 from datetime import timezone
+from typing import TYPE_CHECKING, Any
 
-from tools import dict_to_camel, dict_to_snake
+from hollihop_api_client.base import BaseCategory
+from hollihop_api_client.tools import dict_to_camel, dict_to_snake
 
 if TYPE_CHECKING:
-    from api import AbstractAPI
+    from hollihop_api_client.api import AbstractAPI
 
 
 @dataclass
 class Office:
     id: None | int = None
     name: None | str = None
     location: None | str = None
@@ -19,15 +18,15 @@
     email: None | str = None
     phone: None | str = None
     no_classrooms: None | bool = None
     time_zone: None | timezone = None
     license: None | str = None
 
 
-@dataclass 
+@dataclass
 class Offices:
     offices: list[Office] = field(default_factory=list)
 
 
 class OfficesCategory(BaseCategory):
 
     def __init__(self, api: 'AbstractAPI'):
@@ -35,31 +34,30 @@
 
     def get_offices(
             self,
             id: None | int = None,
             location_id: None | int = None,
             name: None | str = None,
             license: None | str = None
-            ) -> list[Office]:
+    ) -> list[Office]:
         data = dict_to_camel(self.handle_parameters(locals()))
 
         response = self.api.request(
-                method='GetOffices',
-                http_method='GET',
-                data=data
-                )
+            method='GetOffices',
+            http_method='GET',
+            data=data
+        )
 
         response = dict_to_snake(response)
 
         return [Office(**_) for _ in Offices(**response).offices]
-    
+
     def get_all_offices_name(self) -> list[str]:
         offices = self.get_offices()
         return [office.name for office in offices]
 
     def get_all_offices_id(self) -> list[int]:
         offices = self.get_offices()
         return [office.id for office in offices]
 
 
 __all__ = ['OfficesCategory']
-
```

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client/tests/conftest.py` & `hollihop_api_client-0.0.6/src/hollihop_api_client/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 from dataclasses import dataclass
 from datetime import datetime
 
 import pytest
-from dotenv import load_dotenv
-
 from api import HolliHopAPI
+from dotenv import load_dotenv
 
 
 @dataclass
 class TestData:
     test_city_name: str
     test_city_id: int
     test_office_name: str
```

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client/tests/test_ed_units.py` & `hollihop_api_client-0.0.6/src/hollihop_api_client/tests/test_ed_units.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client/tests/test_offices.py` & `hollihop_api_client-0.0.6/src/hollihop_api_client/tests/test_offices.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client/tools/__init__.py` & `hollihop_api_client-0.0.6/src/hollihop_api_client/tools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from functools import lru_cache
 from typing import Any
 
-
 keyword_tuple = ('False', 'await', 'else', 'import', 'pass',
                  'None', 'break', 'except', 'in', 'raise',
                  'True', 'class', 'finally', 'is', 'return',
                  'and', 'continue', 'for', 'lambda', 'try',
                  'as', 'def', 'from', 'nonlocal', 'while',
                  'assert', 'del', 'global', 'not', 'with',
                  'async', 'elif', 'if', 'or', 'yield',
```

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client/venv/bin/rst2html.py` & `hollihop_api_client-0.0.6/src/hollihop_api_client/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client/venv/bin/rst2html4.py` & `hollihop_api_client-0.0.6/src/hollihop_api_client/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client/venv/bin/rst2html5.py` & `hollihop_api_client-0.0.6/src/hollihop_api_client/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client/venv/bin/rst2latex.py` & `hollihop_api_client-0.0.6/src/hollihop_api_client/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client/venv/bin/rst2man.py` & `hollihop_api_client-0.0.6/src/hollihop_api_client/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client/venv/bin/rst2odt.py` & `hollihop_api_client-0.0.6/src/hollihop_api_client/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client/venv/bin/rst2odt_prepstyles.py` & `hollihop_api_client-0.0.6/src/hollihop_api_client/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client/venv/bin/rst2pseudoxml.py` & `hollihop_api_client-0.0.6/src/hollihop_api_client/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client/venv/bin/rst2s5.py` & `hollihop_api_client-0.0.6/src/hollihop_api_client/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client/venv/bin/rst2xetex.py` & `hollihop_api_client-0.0.6/src/hollihop_api_client/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client/venv/bin/rst2xml.py` & `hollihop_api_client-0.0.6/src/hollihop_api_client/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client/venv/bin/rstpep2html.py` & `hollihop_api_client-0.0.6/src/hollihop_api_client/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client.egg-info/PKG-INFO` & `hollihop_api_client-0.0.6/src/hollihop_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hollihop-api-client
-Version: 0.0.5
+Version: 0.0.6
 Summary: This library helps you easily create a python application with Hollihop API
 Author-email: Nicholas Maltseb <nmmaltsev@outlook.com>
 Project-URL: Homepage, https://github.com/nicholasChieftain/hollihop_api_client/
 Project-URL: Bug Tracker, https://github.com/nicholasChieftain/hollihop_api_client/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `hollihop_api_client-0.0.5/src/hollihop_api_client.egg-info/SOURCES.txt` & `hollihop_api_client-0.0.6/src/hollihop_api_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 LICENSE
 README.md
 pyproject.toml
 src/hollihop_api_client/__init__.py
 src/hollihop_api_client/categories.py
-src/hollihop_api_client/test.py
 src/hollihop_api_client.egg-info/PKG-INFO
 src/hollihop_api_client.egg-info/SOURCES.txt
 src/hollihop_api_client.egg-info/dependency_links.txt
+src/hollihop_api_client.egg-info/requires.txt
 src/hollihop_api_client.egg-info/top_level.txt
 src/hollihop_api_client/api/__init__.py
 src/hollihop_api_client/api/abc.py
 src/hollihop_api_client/api/api.py
 src/hollihop_api_client/base/__init__.py
 src/hollihop_api_client/base/category.py
 src/hollihop_api_client/methods/__init__.py
```

