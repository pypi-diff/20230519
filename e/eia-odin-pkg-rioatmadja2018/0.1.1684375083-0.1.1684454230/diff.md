# Comparing `tmp/eia-odin-pkg-rioatmadja2018-0.1.1684375083.tar.gz` & `tmp/eia-odin-pkg-rioatmadja2018-0.1.1684454230.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eia-odin-pkg-rioatmadja2018-0.1.1684375083.tar", last modified: Thu May 18 01:58:03 2023, max compression
+gzip compressed data, was "eia-odin-pkg-rioatmadja2018-0.1.1684454230.tar", last modified: Thu May 18 23:57:10 2023, max compression
```

## Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083.tar` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 01:58:03.957424 eia-odin-pkg-rioatmadja2018-0.1.1684375083/
--rw-r--r--   0 debian    (1000) debian    (1000)     1800 2023-05-18 01:58:03.957424 eia-odin-pkg-rioatmadja2018-0.1.1684375083/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)     1445 2023-04-26 16:19:11.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/README.md
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 01:58:03.945423 eia-odin-pkg-rioatmadja2018-0.1.1684375083/cronjob/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-05-05 04:31:42.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/cronjob/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)     4750 2023-05-18 01:57:25.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/cronjob/forecast_padd_weekly_pricing.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1438 2023-05-14 15:58:45.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/cronjob/update_odin_db.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 01:58:03.945423 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-26 16:17:16.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/__init__.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 01:58:03.949423 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/crude_oil/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/crude_oil/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)      789 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/crude_oil/consumption_sales.py
--rw-r--r--   0 debian    (1000) debian    (1000)     2176 2023-05-04 06:19:24.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/crude_oil/import_export.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1252 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/crude_oil/movements.py
--rw-r--r--   0 debian    (1000) debian    (1000)      888 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/crude_oil/pricing.py
--rw-r--r--   0 debian    (1000) debian    (1000)      879 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/crude_oil/production.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1234 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/crude_oil/refining_processing.py
--rw-r--r--   0 debian    (1000) debian    (1000)     4067 2023-05-10 03:19:22.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/crude_oil/stocks.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 01:58:03.949423 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/db/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/db/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)     8279 2023-05-11 16:13:42.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/db/odin_db.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 01:58:03.953423 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/utils/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-26 18:20:07.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/utils/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)     5718 2023-05-18 01:57:25.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/utils/aws_resources.py
--rw-r--r--   0 debian    (1000) debian    (1000)      534 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/utils/browser.py
--rw-r--r--   0 debian    (1000) debian    (1000)     3853 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/utils/constants.py
--rw-r--r--   0 debian    (1000) debian    (1000)      389 2023-05-14 07:07:07.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/utils/credentials.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1004 2023-04-28 03:34:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/utils/facets.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1590 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/utils/tools.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 01:58:03.953423 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia_odin_pkg_rioatmadja2018.egg-info/
--rw-r--r--   0 debian    (1000) debian    (1000)     1800 2023-05-18 01:58:03.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia_odin_pkg_rioatmadja2018.egg-info/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)     1988 2023-05-18 01:58:03.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia_odin_pkg_rioatmadja2018.egg-info/SOURCES.txt
--rw-r--r--   0 debian    (1000) debian    (1000)        1 2023-05-18 01:58:03.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia_odin_pkg_rioatmadja2018.egg-info/dependency_links.txt
--rw-r--r--   0 debian    (1000) debian    (1000)       41 2023-05-18 01:58:03.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia_odin_pkg_rioatmadja2018.egg-info/requires.txt
--rw-r--r--   0 debian    (1000) debian    (1000)       38 2023-05-18 01:58:03.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia_odin_pkg_rioatmadja2018.egg-info/top_level.txt
--rw-r--r--   0 debian    (1000) debian    (1000)        1 2023-05-18 01:57:55.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia_odin_pkg_rioatmadja2018.egg-info/zip-safe
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 01:58:03.953423 eia-odin-pkg-rioatmadja2018-0.1.1684375083/images/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-26 16:17:11.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/images/__init__.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 01:58:03.957424 eia-odin-pkg-rioatmadja2018-0.1.1684375083/lambda_funcs/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/lambda_funcs/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)     3241 2023-05-14 06:18:32.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/lambda_funcs/lambda_function.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1645 2023-05-10 06:22:42.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/lambda_funcs/lambda_function_bulk_import.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1295 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/lambda_funcs/lambda_function_consumption_sales.py
--rw-r--r--   0 debian    (1000) debian    (1000)     3533 2023-05-04 06:41:42.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/lambda_funcs/lambda_function_crude_oil_bulk_old_ver.py
--rw-r--r--   0 debian    (1000) debian    (1000)      822 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/lambda_funcs/lambda_function_import_export.py
--rw-r--r--   0 debian    (1000) debian    (1000)      790 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/lambda_funcs/lambda_function_movements.py
--rw-r--r--   0 debian    (1000) debian    (1000)     5829 2023-05-14 06:18:32.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/lambda_funcs/lambda_function_petroleum_stocks.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1268 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/lambda_funcs/lambda_function_productions.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1332 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/lambda_funcs/lambda_function_refining_processing.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1225 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/lambda_funcs/lambda_function_stocks.py
--rw-r--r--   0 debian    (1000) debian    (1000)      821 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/lambda_funcs/lambda_function_weekly_pricing.py
--rw-r--r--   0 debian    (1000) debian    (1000)       38 2023-05-18 01:58:03.957424 eia-odin-pkg-rioatmadja2018-0.1.1684375083/setup.cfg
--rw-r--r--   0 debian    (1000) debian    (1000)     1562 2023-04-26 16:26:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/setup.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 01:58:03.957424 eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/__init__.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 01:58:03.957424 eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/functionals/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/functionals/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)      885 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/functionals/test_odin_crude_oil_bulk_imports.py
--rw-r--r--   0 debian    (1000) debian    (1000)     2854 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/functionals/test_odin_db.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1687 2023-05-11 16:13:42.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/functionals/test_odin_petroleum_stocks.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 01:58:03.957424 eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/integrations/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/integrations/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1270 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/integrations/test_crude_oil_file_conversition.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 01:58:03.957424 eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/units/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/units/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)      438 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/units/test_crude_oil_consumption_sales.py
--rw-r--r--   0 debian    (1000) debian    (1000)      731 2023-05-04 06:19:24.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/units/test_crude_oil_import_export.py
--rw-r--r--   0 debian    (1000) debian    (1000)      475 2023-04-30 22:13:11.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/units/test_crude_oil_movements.py
--rw-r--r--   0 debian    (1000) debian    (1000)      879 2023-04-28 03:34:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/units/test_crude_oil_production.py
--rw-r--r--   0 debian    (1000) debian    (1000)      602 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/units/test_crude_oil_refining_processing.py
--rw-r--r--   0 debian    (1000) debian    (1000)     2444 2023-05-10 03:19:22.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/units/test_crude_oil_stocks.py
--rw-r--r--   0 debian    (1000) debian    (1000)      992 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/units/test_crude_oil_weekly_price.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 23:57:10.934280 eia-odin-pkg-rioatmadja2018-0.1.1684454230/
+-rw-r--r--   0 debian    (1000) debian    (1000)     1800 2023-05-18 23:57:10.934280 eia-odin-pkg-rioatmadja2018-0.1.1684454230/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)     1445 2023-04-26 16:19:11.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/README.md
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 23:57:10.906280 eia-odin-pkg-rioatmadja2018-0.1.1684454230/cronjob/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-05-05 04:31:42.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/cronjob/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     4750 2023-05-18 01:57:25.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/cronjob/forecast_padd_weekly_pricing.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     2682 2023-05-18 02:27:03.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/cronjob/update_odin_db.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 23:57:10.906280 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-26 16:17:16.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/__init__.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 23:57:10.910280 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/crude_oil/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/crude_oil/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      789 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/crude_oil/consumption_sales.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     2176 2023-05-04 06:19:24.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/crude_oil/import_export.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1252 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/crude_oil/movements.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      888 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/crude_oil/pricing.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      879 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/crude_oil/production.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1234 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/crude_oil/refining_processing.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     4067 2023-05-10 03:19:22.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/crude_oil/stocks.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 23:57:10.910280 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/db/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/db/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     8279 2023-05-11 16:13:42.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/db/odin_db.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 23:57:10.910280 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/utils/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-26 18:20:07.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/utils/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     5718 2023-05-18 01:57:25.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/utils/aws_resources.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      534 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/utils/browser.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     3853 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/utils/constants.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      389 2023-05-14 07:07:07.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/utils/credentials.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1004 2023-04-28 03:34:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/utils/facets.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1590 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/utils/tools.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 23:57:10.914280 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia_odin_pkg_rioatmadja2018.egg-info/
+-rw-r--r--   0 debian    (1000) debian    (1000)     1800 2023-05-18 23:57:10.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia_odin_pkg_rioatmadja2018.egg-info/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)     1988 2023-05-18 23:57:10.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia_odin_pkg_rioatmadja2018.egg-info/SOURCES.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)        1 2023-05-18 23:57:10.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia_odin_pkg_rioatmadja2018.egg-info/dependency_links.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)       41 2023-05-18 23:57:10.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia_odin_pkg_rioatmadja2018.egg-info/requires.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)       38 2023-05-18 23:57:10.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia_odin_pkg_rioatmadja2018.egg-info/top_level.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)        1 2023-05-18 23:57:01.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia_odin_pkg_rioatmadja2018.egg-info/zip-safe
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 23:57:10.914280 eia-odin-pkg-rioatmadja2018-0.1.1684454230/images/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-26 16:17:11.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/images/__init__.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 23:57:10.922280 eia-odin-pkg-rioatmadja2018-0.1.1684454230/lambda_funcs/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/lambda_funcs/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     3241 2023-05-14 06:18:32.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/lambda_funcs/lambda_function.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1645 2023-05-10 06:22:42.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/lambda_funcs/lambda_function_bulk_import.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1295 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/lambda_funcs/lambda_function_consumption_sales.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     3533 2023-05-04 06:41:42.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/lambda_funcs/lambda_function_crude_oil_bulk_old_ver.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      822 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/lambda_funcs/lambda_function_import_export.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      790 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/lambda_funcs/lambda_function_movements.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     5829 2023-05-14 06:18:32.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/lambda_funcs/lambda_function_petroleum_stocks.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1268 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/lambda_funcs/lambda_function_productions.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1332 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/lambda_funcs/lambda_function_refining_processing.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1225 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/lambda_funcs/lambda_function_stocks.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      821 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/lambda_funcs/lambda_function_weekly_pricing.py
+-rw-r--r--   0 debian    (1000) debian    (1000)       38 2023-05-18 23:57:10.934280 eia-odin-pkg-rioatmadja2018-0.1.1684454230/setup.cfg
+-rw-r--r--   0 debian    (1000) debian    (1000)     1562 2023-04-26 16:26:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/setup.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 23:57:10.922280 eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/__init__.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 23:57:10.930280 eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/functionals/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/functionals/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      885 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/functionals/test_odin_crude_oil_bulk_imports.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     2854 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/functionals/test_odin_db.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1687 2023-05-11 16:13:42.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/functionals/test_odin_petroleum_stocks.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 23:57:10.934280 eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/integrations/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/integrations/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1270 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/integrations/test_crude_oil_file_conversition.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-18 23:57:10.934280 eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/units/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/units/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      438 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/units/test_crude_oil_consumption_sales.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      731 2023-05-04 06:19:24.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/units/test_crude_oil_import_export.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      475 2023-04-30 22:13:11.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/units/test_crude_oil_movements.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      879 2023-04-28 03:34:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/units/test_crude_oil_production.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      602 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/units/test_crude_oil_refining_processing.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     2444 2023-05-10 03:19:22.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/units/test_crude_oil_stocks.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      992 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/units/test_crude_oil_weekly_price.py
```

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/PKG-INFO` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eia-odin-pkg-rioatmadja2018
-Version: 0.1.1684375083
+Version: 0.1.1684454230
 Summary: Python Wheels to interact with the EIA APIs
 Author: Rio Atmadja
 Author-email: rioatmadja2018@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8
```

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/README.md` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/README.md`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/cronjob/forecast_padd_weekly_pricing.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/cronjob/forecast_padd_weekly_pricing.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/crude_oil/consumption_sales.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/crude_oil/consumption_sales.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/crude_oil/import_export.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/crude_oil/import_export.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/crude_oil/movements.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/crude_oil/movements.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/crude_oil/pricing.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/crude_oil/pricing.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/crude_oil/production.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/crude_oil/production.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/crude_oil/refining_processing.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/crude_oil/refining_processing.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/crude_oil/stocks.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/crude_oil/stocks.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/db/odin_db.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/db/odin_db.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/utils/aws_resources.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/utils/aws_resources.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/utils/browser.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/utils/browser.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/utils/constants.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/utils/constants.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/utils/facets.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/utils/facets.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia/utils/tools.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia/utils/tools.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia_odin_pkg_rioatmadja2018.egg-info/PKG-INFO` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia_odin_pkg_rioatmadja2018.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eia-odin-pkg-rioatmadja2018
-Version: 0.1.1684375083
+Version: 0.1.1684454230
 Summary: Python Wheels to interact with the EIA APIs
 Author: Rio Atmadja
 Author-email: rioatmadja2018@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8
```

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/eia_odin_pkg_rioatmadja2018.egg-info/SOURCES.txt` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/eia_odin_pkg_rioatmadja2018.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/lambda_funcs/lambda_function.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/lambda_funcs/lambda_function.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/lambda_funcs/lambda_function_bulk_import.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/lambda_funcs/lambda_function_bulk_import.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/lambda_funcs/lambda_function_consumption_sales.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/lambda_funcs/lambda_function_consumption_sales.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/lambda_funcs/lambda_function_crude_oil_bulk_old_ver.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/lambda_funcs/lambda_function_crude_oil_bulk_old_ver.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/lambda_funcs/lambda_function_import_export.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/lambda_funcs/lambda_function_import_export.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/lambda_funcs/lambda_function_movements.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/lambda_funcs/lambda_function_movements.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/lambda_funcs/lambda_function_petroleum_stocks.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/lambda_funcs/lambda_function_petroleum_stocks.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/lambda_funcs/lambda_function_productions.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/lambda_funcs/lambda_function_productions.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/lambda_funcs/lambda_function_refining_processing.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/lambda_funcs/lambda_function_refining_processing.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/lambda_funcs/lambda_function_stocks.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/lambda_funcs/lambda_function_stocks.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/lambda_funcs/lambda_function_weekly_pricing.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/lambda_funcs/lambda_function_weekly_pricing.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/setup.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/setup.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/functionals/test_odin_crude_oil_bulk_imports.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/functionals/test_odin_crude_oil_bulk_imports.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/functionals/test_odin_db.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/functionals/test_odin_db.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/functionals/test_odin_petroleum_stocks.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/functionals/test_odin_petroleum_stocks.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/integrations/test_crude_oil_file_conversition.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/integrations/test_crude_oil_file_conversition.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/units/test_crude_oil_import_export.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/units/test_crude_oil_import_export.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/units/test_crude_oil_production.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/units/test_crude_oil_production.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/units/test_crude_oil_refining_processing.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/units/test_crude_oil_refining_processing.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/units/test_crude_oil_stocks.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/units/test_crude_oil_stocks.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684375083/tests/units/test_crude_oil_weekly_price.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684454230/tests/units/test_crude_oil_weekly_price.py`

 * *Files identical despite different names*

