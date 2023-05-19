# Comparing `tmp/arg-econ-data-0.0.8.tar.gz` & `tmp/arg-econ-data-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arg-econ-data-0.0.8.tar", last modified: Wed Apr 27 16:16:45 2022, max compression
+gzip compressed data, was "arg-econ-data-0.0.9.tar", last modified: Fri Apr 29 15:42:51 2022, max compression
```

## Comparing `arg-econ-data-0.0.8.tar` & `arg-econ-data-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2022-04-27 16:16:45.199037 arg-econ-data-0.0.8/
--rw-rw-rw-   0        0        0      128 2022-04-27 16:16:45.198039 arg-econ-data-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-04-27 16:16:45.183037 arg-econ-data-0.0.8/arg_econ_data/
--rw-rw-rw-   0        0        0    14579 2022-04-27 16:15:02.000000 arg-econ-data-0.0.8/arg_econ_data/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-27 16:16:45.197038 arg-econ-data-0.0.8/arg_econ_data.egg-info/
--rw-rw-rw-   0        0        0      128 2022-04-27 16:16:44.000000 arg-econ-data-0.0.8/arg_econ_data.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2022-04-27 16:16:45.000000 arg-econ-data-0.0.8/arg_econ_data.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-27 16:16:44.000000 arg-econ-data-0.0.8/arg_econ_data.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2022-04-27 16:16:45.000000 arg-econ-data-0.0.8/arg_econ_data.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-04-27 16:16:45.000000 arg-econ-data-0.0.8/arg_econ_data.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2022-04-20 15:28:18.000000 arg-econ-data-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-04-27 16:16:45.199037 arg-econ-data-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      333 2022-04-27 16:15:59.000000 arg-econ-data-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-04-29 15:42:51.821090 arg-econ-data-0.0.9/
+-rw-rw-rw-   0        0        0      128 2022-04-29 15:42:51.821090 arg-econ-data-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-04-29 15:42:51.801098 arg-econ-data-0.0.9/arg_econ_data/
+-rw-rw-rw-   0        0        0    26213 2022-04-29 15:40:15.000000 arg-econ-data-0.0.9/arg_econ_data/__init__.py
+drwxrwxrwx   0        0        0        0 2022-04-29 15:42:51.819089 arg-econ-data-0.0.9/arg_econ_data.egg-info/
+-rw-rw-rw-   0        0        0      128 2022-04-29 15:42:51.000000 arg-econ-data-0.0.9/arg_econ_data.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2022-04-29 15:42:51.000000 arg-econ-data-0.0.9/arg_econ_data.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-04-29 15:42:51.000000 arg-econ-data-0.0.9/arg_econ_data.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2022-04-29 15:42:51.000000 arg-econ-data-0.0.9/arg_econ_data.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2022-04-29 15:42:51.000000 arg-econ-data-0.0.9/arg_econ_data.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2022-04-29 14:12:54.000000 arg-econ-data-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-04-29 15:42:51.822090 arg-econ-data-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      333 2022-04-29 15:42:34.000000 arg-econ-data-0.0.9/setup.py
```

