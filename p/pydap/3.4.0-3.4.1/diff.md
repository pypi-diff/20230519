# Comparing `tmp/pydap-3.4.0.tar.gz` & `tmp/pydap-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydap-3.4.0.tar", last modified: Fri Apr  7 23:16:09 2023, max compression
+gzip compressed data, was "pydap-3.4.1.tar", last modified: Fri May 19 19:24:45 2023, max compression
```

## Comparing `pydap-3.4.0.tar` & `pydap-3.4.1.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.222408 pydap-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-07 23:15:52.000000 pydap-3.4.0/CONTRIBUTORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-07 23:15:52.000000 pydap-3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-07 23:15:52.000000 pydap-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-04-07 23:15:52.000000 pydap-3.4.0/NEWS.md
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-07 23:16:09.222408 pydap-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-07 23:15:52.000000 pydap-3.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.202408 pydap-3.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/Special chars.odt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.202408 pydap-3.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/_static/default.css
--rw-r--r--   0 runner    (1001) docker     (123)    21148 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/client.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/developer.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15745 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/developer_data_model.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/developer_handlers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/developer_responses.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/developer_templating.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/handlers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/responses.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/server.rst
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-07 23:16:09.222408 pydap-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-07 23:15:52.000000 pydap-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.190408 pydap-3.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.206408 pydap-3.4.0/src/pydap/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.206408 pydap-3.4.0/src/pydap/apis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/apis/netcdf4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.206408 pydap-3.4.0/src/pydap/cas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/cas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/cas/esgf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/cas/get_cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/cas/urs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.206408 pydap-3.4.0/src/pydap/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.206408 pydap-3.4.0/src/pydap/handlers/csv/
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/handlers/csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23594 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/handlers/dap.py
--rw-r--r--   0 runner    (1001) docker     (123)    17787 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/handlers/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.206408 pydap-3.4.0/src/pydap/handlers/netcdf/
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/handlers/netcdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9930 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    23970 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.206408 pydap-3.4.0/src/pydap/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/parsers/das.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/parsers/dds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/parsers/dmr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/pycompat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.206408 pydap-3.4.0/src/pydap/responses/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/responses/ascii.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/responses/das.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/responses/dds.py
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/responses/dods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/responses/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.210408 pydap-3.4.0/src/pydap/responses/html/
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/responses/html/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.210408 pydap-3.4.0/src/pydap/responses/html/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/responses/html/templates/html.html
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/responses/html/templates/macros.html
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/responses/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/responses/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.210408 pydap-3.4.0/src/pydap/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/server/devel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/server/devel_ssl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.214408 pydap-3.4.0/src/pydap/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.214408 pydap-3.4.0/src/pydap/tests/dap_4_access/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/dap_4_access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/dap_4_access/analyze_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/dap_4_access/dap4_access_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.218408 pydap-3.4.0/src/pydap/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/data/coads_climatology.nc.dods
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/data/rainfall_time_malaysia.cdp.das
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/data/rainfall_time_malaysia.cdp.dds
--rw-r--r--   0 runner    (1001) docker     (123)  5673697 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/data/rainfall_time_malaysia.cdp.dods
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/data/test.01.das
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/data/test.01.dods
--rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_D1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_cas_esgf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_cas_urs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_constrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_dapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_handlers_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    22380 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_handlers_dap.py
--rw-r--r--   0 runner    (1001) docker     (123)    18572 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_handlers_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_handlers_netcdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_iter_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    16851 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_net.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_open_dap4_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_parsers_dap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_parsers_das.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_parsers_dds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_parsers_dmr.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_pydap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_responses_ascii.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_responses_das.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_responses_dds.py
--rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_responses_dods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_responses_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_responses_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_responses_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_responses_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_server_devel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_server_devel_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_special_chars.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_webtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_wsgi_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_wsgi_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_wsgi_ssf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.222408 pydap-3.4.0/src/pydap/wsgi/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/wsgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/wsgi/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/wsgi/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/wsgi/ssf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.222408 pydap-3.4.0/src/pydap/wsgi/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/wsgi/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/wsgi/templates/catalog.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/wsgi/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.222408 pydap-3.4.0/src/pydap/wsgi/templates/static/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/wsgi/templates/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.206408 pydap-3.4.0/src/pydap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-07 23:16:09.000000 pydap-3.4.0/src/pydap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-07 23:16:09.000000 pydap-3.4.0/src/pydap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:16:09.000000 pydap-3.4.0/src/pydap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-07 23:16:09.000000 pydap-3.4.0/src/pydap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-07 23:16:09.000000 pydap-3.4.0/src/pydap.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:16:08.000000 pydap-3.4.0/src/pydap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-07 23:16:09.000000 pydap-3.4.0/src/pydap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-07 23:16:09.000000 pydap-3.4.0/src/pydap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:45.968223 pydap-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-19 19:24:25.000000 pydap-3.4.1/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-19 19:24:25.000000 pydap-3.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-19 19:24:25.000000 pydap-3.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-05-19 19:24:25.000000 pydap-3.4.1/NEWS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-05-19 19:24:45.968223 pydap-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-19 19:24:25.000000 pydap-3.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:45.936223 pydap-3.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-19 19:24:25.000000 pydap-3.4.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-05-19 19:24:25.000000 pydap-3.4.1/docs/Special chars.odt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:45.936223 pydap-3.4.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-05-19 19:24:25.000000 pydap-3.4.1/docs/_static/default.css
+-rw-r--r--   0 runner    (1001) docker     (123)    21148 2023-05-19 19:24:25.000000 pydap-3.4.1/docs/client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-05-19 19:24:25.000000 pydap-3.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-19 19:24:25.000000 pydap-3.4.1/docs/developer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15745 2023-05-19 19:24:25.000000 pydap-3.4.1/docs/developer_data_model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-05-19 19:24:25.000000 pydap-3.4.1/docs/developer_handlers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-19 19:24:25.000000 pydap-3.4.1/docs/developer_responses.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-19 19:24:25.000000 pydap-3.4.1/docs/developer_templating.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-05-19 19:24:25.000000 pydap-3.4.1/docs/handlers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-05-19 19:24:25.000000 pydap-3.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-19 19:24:25.000000 pydap-3.4.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-19 19:24:25.000000 pydap-3.4.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-05-19 19:24:25.000000 pydap-3.4.1/docs/responses.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-05-19 19:24:25.000000 pydap-3.4.1/docs/server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-19 19:24:45.968223 pydap-3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-05-19 19:24:25.000000 pydap-3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:45.928223 pydap-3.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:45.940223 pydap-3.4.1/src/pydap/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:45.940223 pydap-3.4.1/src/pydap/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/apis/netcdf4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:45.940223 pydap-3.4.1/src/pydap/cas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/cas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/cas/esgf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/cas/get_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/cas/urs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:45.940223 pydap-3.4.1/src/pydap/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:45.944223 pydap-3.4.1/src/pydap/handlers/csv/
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/handlers/csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23882 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/handlers/dap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17787 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/handlers/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:45.944223 pydap-3.4.1/src/pydap/handlers/netcdf/
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/handlers/netcdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9930 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23970 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:45.944223 pydap-3.4.1/src/pydap/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/parsers/das.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/parsers/dds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/parsers/dmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/pycompat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:45.944223 pydap-3.4.1/src/pydap/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/responses/ascii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/responses/das.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/responses/dds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/responses/dods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/responses/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:45.944223 pydap-3.4.1/src/pydap/responses/html/
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/responses/html/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:45.944223 pydap-3.4.1/src/pydap/responses/html/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/responses/html/templates/html.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/responses/html/templates/macros.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/responses/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/responses/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:45.948223 pydap-3.4.1/src/pydap/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/server/devel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/server/devel_ssl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:45.956223 pydap-3.4.1/src/pydap/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:45.956223 pydap-3.4.1/src/pydap/tests/dap_4_access/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/dap_4_access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/dap_4_access/analyze_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/dap_4_access/dap4_access_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:45.964223 pydap-3.4.1/src/pydap/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/data/coads_climatology.nc.dods
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/data/rainfall_time_malaysia.cdp.das
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/data/rainfall_time_malaysia.cdp.dds
+-rw-r--r--   0 runner    (1001) docker     (123)  5673697 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/data/rainfall_time_malaysia.cdp.dods
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/data/test.01.das
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/data/test.01.dods
+-rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/test_D1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/test_cas_esgf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/test_cas_urs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/test_constrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/test_dapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/test_handlers_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23992 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/test_handlers_dap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18572 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/test_handlers_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/test_handlers_netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/test_iter_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16851 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/test_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/test_open_dap4_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/test_parsers_dap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/test_parsers_das.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-19 19:24:25.000000 pydap-3.4.1/src/pydap/tests/test_parsers_dds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-19 19:24:26.000000 pydap-3.4.1/src/pydap/tests/test_parsers_dmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-19 19:24:26.000000 pydap-3.4.1/src/pydap/tests/test_pydap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-19 19:24:26.000000 pydap-3.4.1/src/pydap/tests/test_responses_ascii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-19 19:24:26.000000 pydap-3.4.1/src/pydap/tests/test_responses_das.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-19 19:24:26.000000 pydap-3.4.1/src/pydap/tests/test_responses_dds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-05-19 19:24:26.000000 pydap-3.4.1/src/pydap/tests/test_responses_dods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-19 19:24:26.000000 pydap-3.4.1/src/pydap/tests/test_responses_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-05-19 19:24:26.000000 pydap-3.4.1/src/pydap/tests/test_responses_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-19 19:24:26.000000 pydap-3.4.1/src/pydap/tests/test_responses_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-19 19:24:26.000000 pydap-3.4.1/src/pydap/tests/test_responses_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-19 19:24:26.000000 pydap-3.4.1/src/pydap/tests/test_server_devel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-19 19:24:26.000000 pydap-3.4.1/src/pydap/tests/test_server_devel_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-19 19:24:26.000000 pydap-3.4.1/src/pydap/tests/test_special_chars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-19 19:24:26.000000 pydap-3.4.1/src/pydap/tests/test_webtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-19 19:24:26.000000 pydap-3.4.1/src/pydap/tests/test_wsgi_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-05-19 19:24:26.000000 pydap-3.4.1/src/pydap/tests/test_wsgi_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-05-19 19:24:26.000000 pydap-3.4.1/src/pydap/tests/test_wsgi_ssf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:45.968223 pydap-3.4.1/src/pydap/wsgi/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-19 19:24:26.000000 pydap-3.4.1/src/pydap/wsgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-05-19 19:24:26.000000 pydap-3.4.1/src/pydap/wsgi/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-05-19 19:24:26.000000 pydap-3.4.1/src/pydap/wsgi/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-05-19 19:24:26.000000 pydap-3.4.1/src/pydap/wsgi/ssf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:45.968223 pydap-3.4.1/src/pydap/wsgi/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-19 19:24:26.000000 pydap-3.4.1/src/pydap/wsgi/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-19 19:24:26.000000 pydap-3.4.1/src/pydap/wsgi/templates/catalog.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-19 19:24:26.000000 pydap-3.4.1/src/pydap/wsgi/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:45.968223 pydap-3.4.1/src/pydap/wsgi/templates/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-19 19:24:26.000000 pydap-3.4.1/src/pydap/wsgi/templates/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:45.940223 pydap-3.4.1/src/pydap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-05-19 19:24:45.000000 pydap-3.4.1/src/pydap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-19 19:24:45.000000 pydap-3.4.1/src/pydap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 19:24:45.000000 pydap-3.4.1/src/pydap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-19 19:24:45.000000 pydap-3.4.1/src/pydap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-19 19:24:45.000000 pydap-3.4.1/src/pydap.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 19:24:45.000000 pydap-3.4.1/src/pydap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-19 19:24:45.000000 pydap-3.4.1/src/pydap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 19:24:45.000000 pydap-3.4.1/src/pydap.egg-info/top_level.txt
```

### Comparing `pydap-3.4.0/CONTRIBUTORS.md` & `pydap-3.4.1/CONTRIBUTORS.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 pydap contributors (sorted alphabetically)
 ==========================================
 
 * Roberto De Almeida
 
 * Aleksandar Jelenak
 * Amanda Yoshiizumi  
+* [Anthony Baxter](anthonybaxter)
 * Beto Dealmeida, Roberto De Almeida
 * Christian Skarby  
 * Daniel Gray
 * Danny  
 * Edward Hartnett  
+* [Fedor Baart](https://github.com/SiggyF)
+* [Filipe Fernandes](https://github.com/ocefpaf)
 * Frédéric Laliberté  
 * Ghislain Antony Vaillant  
 * Hugo  
 * James Gallagher  
 * James Hiebert  
+* [Jonas Gliß](https://github.com/jgliss)
 * Juan Luis Cano Rodríguez  
 * Lewis John McGibbney
+* [Massimo Di Stefano](epifanio)
 * Michael Bunsen  
 * Mike McCann
+* [Nathan Carlson](nathanlcarlson)
 * Nathan Potter  
 * Niklas Griessbaum
+* [Owen Littlejohns](https://github.com/owenlittlejohns)
 * Ray Bell  
 * Rich Signell  
 * Ryan Abernathey  
 * Sebastian Krieger  
 * Shreyas Cholia  
 * Stephan Hoyer
 * Tobias Kölling  
 * Tom Kralidis  
 * Will Holmgren  
-* [SiggyF](https://github.com/SiggyF)
-* [ocefpaf](https://github.com/ocefpaf)
-* anthonybaxter  
-* epifanio  
-* nathanlcarlson
```

### Comparing `pydap-3.4.0/LICENSE` & `pydap-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/NEWS.md` & `pydap-3.4.1/NEWS.md`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/PKG-INFO` & `pydap-3.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydap
-Version: 3.4.0
+Version: 3.4.1
 Summary: An implementation of the Data Access Protocol.
 Home-page: http://pydap.org/
 Author: Roberto De Almeida
 Author-email: roberto@dealmeida.net
 Maintainer: James Hiebert
 Maintainer-email: james@hiebert.name
 License: MIT
```

### Comparing `pydap-3.4.0/README.md` & `pydap-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/docs/Makefile` & `pydap-3.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/docs/Special chars.odt` & `pydap-3.4.1/docs/Special chars.odt`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/docs/_static/default.css` & `pydap-3.4.1/docs/_static/default.css`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/docs/client.rst` & `pydap-3.4.1/docs/client.rst`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/docs/conf.py` & `pydap-3.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/docs/developer.rst` & `pydap-3.4.1/docs/developer.rst`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/docs/developer_data_model.rst` & `pydap-3.4.1/docs/developer_data_model.rst`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/docs/developer_handlers.rst` & `pydap-3.4.1/docs/developer_handlers.rst`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/docs/developer_responses.rst` & `pydap-3.4.1/docs/developer_responses.rst`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/docs/developer_templating.rst` & `pydap-3.4.1/docs/developer_templating.rst`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/docs/handlers.rst` & `pydap-3.4.1/docs/handlers.rst`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/docs/index.rst` & `pydap-3.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/docs/license.rst` & `pydap-3.4.1/docs/license.rst`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/docs/make.bat` & `pydap-3.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/docs/responses.rst` & `pydap-3.4.1/docs/responses.rst`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/docs/server.rst` & `pydap-3.4.1/docs/server.rst`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/setup.py` & `pydap-3.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/apis/netcdf4.py` & `pydap-3.4.1/src/pydap/apis/netcdf4.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/cas/esgf.py` & `pydap-3.4.1/src/pydap/cas/esgf.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/cas/get_cookies.py` & `pydap-3.4.1/src/pydap/cas/get_cookies.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/cas/urs.py` & `pydap-3.4.1/src/pydap/cas/urs.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/client.py` & `pydap-3.4.1/src/pydap/client.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/exceptions.py` & `pydap-3.4.1/src/pydap/exceptions.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/handlers/csv/__init__.py` & `pydap-3.4.1/src/pydap/handlers/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/handlers/dap.py` & `pydap-3.4.1/src/pydap/handlers/dap.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,26 +124,32 @@
         else:
             self.add_dap2_proxies()
 
     def add_dap4_proxies(self):
         # remove any projection from the base_url, leaving selections
         for var in walk(self.dataset, pydap.model.BaseType):
             var.data = BaseProxyDap4(self.base_url, var.name, var.dtype, var.shape,
-                                     application=self.application, session=self.session)
+                                     application=self.application, session=self.session,
+                                     timeout=self.timeout)
         for var in walk(self.dataset, pydap.model.GridType):
             var.set_output_grid(self.output_grid)
 
     def add_dap2_proxies(self):
         # now add data proxies
         for var in walk(self.dataset, pydap.model.BaseType):
             var.data = BaseProxyDap2(self.base_url, var.id, var.dtype, var.shape,
-                                     application=self.application, session=self.session)
+                                     application=self.application, session=self.session,
+                                     timeout=self.timeout)
         for var in walk(self.dataset, pydap.model.SequenceType):
             template = copy.copy(var)
-            var.data = SequenceProxy(self.base_url, template, application=self.application, session=self.session)
+            var.data = SequenceProxy(self.base_url,
+                                     template,
+                                     application=self.application,
+                                     session=self.session,
+                                     timeout=self.timeout)
 
         # apply projections
         for var in self.projection:
             target = self.dataset
             while var:
                 token, index = var.pop(0)
                 target = target[token]
```

### Comparing `pydap-3.4.0/src/pydap/handlers/lib.py` & `pydap-3.4.1/src/pydap/handlers/lib.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/handlers/netcdf/__init__.py` & `pydap-3.4.1/src/pydap/handlers/netcdf/__init__.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/lib.py` & `pydap-3.4.1/src/pydap/lib.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/model.py` & `pydap-3.4.1/src/pydap/model.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/net.py` & `pydap-3.4.1/src/pydap/net.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/parsers/__init__.py` & `pydap-3.4.1/src/pydap/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/parsers/das.py` & `pydap-3.4.1/src/pydap/parsers/das.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/parsers/dds.py` & `pydap-3.4.1/src/pydap/parsers/dds.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/parsers/dmr.py` & `pydap-3.4.1/src/pydap/parsers/dmr.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/pycompat.py` & `pydap-3.4.1/src/pydap/pycompat.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/responses/ascii.py` & `pydap-3.4.1/src/pydap/responses/ascii.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/responses/das.py` & `pydap-3.4.1/src/pydap/responses/das.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/responses/dds.py` & `pydap-3.4.1/src/pydap/responses/dds.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/responses/dods.py` & `pydap-3.4.1/src/pydap/responses/dods.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/responses/error.py` & `pydap-3.4.1/src/pydap/responses/error.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/responses/html/__init__.py` & `pydap-3.4.1/src/pydap/responses/html/__init__.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/responses/html/templates/html.html` & `pydap-3.4.1/src/pydap/responses/html/templates/html.html`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/responses/html/templates/macros.html` & `pydap-3.4.1/src/pydap/responses/html/templates/macros.html`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/responses/lib.py` & `pydap-3.4.1/src/pydap/responses/lib.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/responses/version.py` & `pydap-3.4.1/src/pydap/responses/version.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/server/devel.py` & `pydap-3.4.1/src/pydap/server/devel.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/server/devel_ssl.py` & `pydap-3.4.1/src/pydap/server/devel_ssl.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/dap_4_access/analyze_log.py` & `pydap-3.4.1/src/pydap/tests/dap_4_access/analyze_log.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/dap_4_access/dap4_access_test.py` & `pydap-3.4.1/src/pydap/tests/dap_4_access/dap4_access_test.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/data/rainfall_time_malaysia.cdp.das` & `pydap-3.4.1/src/pydap/tests/data/rainfall_time_malaysia.cdp.das`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/data/rainfall_time_malaysia.cdp.dds` & `pydap-3.4.1/src/pydap/tests/data/rainfall_time_malaysia.cdp.dds`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/data/rainfall_time_malaysia.cdp.dods` & `pydap-3.4.1/src/pydap/tests/data/rainfall_time_malaysia.cdp.dods`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/datasets.py` & `pydap-3.4.1/src/pydap/tests/datasets.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_D1.py` & `pydap-3.4.1/src/pydap/tests/test_D1.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_cas_esgf.py` & `pydap-3.4.1/src/pydap/tests/test_cas_esgf.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_cas_urs.py` & `pydap-3.4.1/src/pydap/tests/test_cas_urs.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_client.py` & `pydap-3.4.1/src/pydap/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_constrain.py` & `pydap-3.4.1/src/pydap/tests/test_constrain.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_dapper.py` & `pydap-3.4.1/src/pydap/tests/test_dapper.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_exceptions.py` & `pydap-3.4.1/src/pydap/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_handlers_csv.py` & `pydap-3.4.1/src/pydap/tests/test_handlers_csv.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_handlers_dap.py` & `pydap-3.4.1/src/pydap/tests/test_handlers_dap.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Test the DAP handler, which forms the core of the client."""
 
 import numpy as np
+import pydap.model
 from pydap.model import StructureType, GridType, DatasetType, BaseType
 from pydap.handlers.lib import BaseHandler, ConstraintExpression
 from pydap.handlers.dap import DAPHandler, BaseProxyDap2, SequenceProxy
-from pydap.handlers.dap import find_pattern_in_string_iter
+from pydap.handlers.dap import find_pattern_in_string_iter, walk
 from pydap.tests.datasets import (
     SimpleSequence, SimpleGrid, SimpleArray, VerySimpleSequence)
 
 import unittest
 try:
     from unittest.mock import patch
 except ImportError:
@@ -236,14 +237,52 @@
             "http://localhost:8001/?cast[1]", self.app2).dataset
 
         self.assertEqual(dataset.cast.data.slice, (slice(1, 2, 1),))
         self.assertEqual(
             [tuple(row) for row in dataset.cast.iterdata()], [
                 ('2', 200, 10, 500, 1, 15, 35, 100)])
 
+    def test_custom_timeout_BaseProxyDap2(self):
+        dataset = DAPHandler("http://localhost:8001/",
+                             self.app1,
+                             timeout=300).dataset
+
+        for var in walk(dataset, pydap.model.BaseType):
+            assert var.data.timeout == 300
+
+    def test_custom_timeout_SequenceProxy(self):
+        dataset = DAPHandler("http://localhost:8001/",
+                             self.app2,
+                             timeout=300).dataset
+        for var in walk(dataset, pydap.model.SequenceType):
+            assert var.data.timeout == 300
+
+    def test_custom_timeout_BaseProxyDap4(self):
+
+        # monkeypatch DAP4 dataset init (since there is
+        # no DAP4 test dataset available, we only
+        # need the DAP4 proxy to be instantiated as such
+        # to test assignment of custom timeout).
+        # See DAPHandler.make_dataset call in __init__
+        # We only need DAPHandler.add_proxies to handle
+        # case add_dap4_proxies for the timeout test
+        # ToDo: This hack should be removed once a proper DAP4 test setup
+        # is in place
+        from _pytest.monkeypatch import MonkeyPatch
+        mp = MonkeyPatch()
+        mp.setattr(DAPHandler, "dataset_from_dap4",
+                   DAPHandler.dataset_from_dap2)
+
+        dataset = DAPHandler("http://localhost:8001/",
+                             self.app1,
+                             timeout=300,
+                             protocol='dap4').dataset
+
+        for var in walk(dataset, pydap.model.BaseType):
+            assert var.data.timeout == 300
 
 class TestBaseProxy(unittest.TestCase):
 
     """Test `BaseProxy` objects."""
 
     def setUp(self):
         """Create a WSGI app"""
```

### Comparing `pydap-3.4.0/src/pydap/tests/test_handlers_lib.py` & `pydap-3.4.1/src/pydap/tests/test_handlers_lib.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_handlers_netcdf.py` & `pydap-3.4.1/src/pydap/tests/test_handlers_netcdf.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_iter_data.py` & `pydap-3.4.1/src/pydap/tests/test_iter_data.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_lib.py` & `pydap-3.4.1/src/pydap/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_model.py` & `pydap-3.4.1/src/pydap/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_net.py` & `pydap-3.4.1/src/pydap/tests/test_net.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_open_dap4_url.py` & `pydap-3.4.1/src/pydap/tests/test_open_dap4_url.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_parsers.py` & `pydap-3.4.1/src/pydap/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_parsers_dap.py` & `pydap-3.4.1/src/pydap/tests/test_parsers_dap.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_parsers_das.py` & `pydap-3.4.1/src/pydap/tests/test_parsers_das.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_parsers_dds.py` & `pydap-3.4.1/src/pydap/tests/test_parsers_dds.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_parsers_dmr.py` & `pydap-3.4.1/src/pydap/tests/test_parsers_dmr.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_responses_ascii.py` & `pydap-3.4.1/src/pydap/tests/test_responses_ascii.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_responses_das.py` & `pydap-3.4.1/src/pydap/tests/test_responses_das.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_responses_dds.py` & `pydap-3.4.1/src/pydap/tests/test_responses_dds.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_responses_dods.py` & `pydap-3.4.1/src/pydap/tests/test_responses_dods.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_responses_error.py` & `pydap-3.4.1/src/pydap/tests/test_responses_error.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_responses_html.py` & `pydap-3.4.1/src/pydap/tests/test_responses_html.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_responses_lib.py` & `pydap-3.4.1/src/pydap/tests/test_responses_lib.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_responses_version.py` & `pydap-3.4.1/src/pydap/tests/test_responses_version.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_server_devel.py` & `pydap-3.4.1/src/pydap/tests/test_server_devel.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_server_devel_ssl.py` & `pydap-3.4.1/src/pydap/tests/test_server_devel_ssl.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_special_chars.py` & `pydap-3.4.1/src/pydap/tests/test_special_chars.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_wsgi_app.py` & `pydap-3.4.1/src/pydap/tests/test_wsgi_app.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_wsgi_functions.py` & `pydap-3.4.1/src/pydap/tests/test_wsgi_functions.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/tests/test_wsgi_ssf.py` & `pydap-3.4.1/src/pydap/tests/test_wsgi_ssf.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/wsgi/app.py` & `pydap-3.4.1/src/pydap/wsgi/app.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/wsgi/functions.py` & `pydap-3.4.1/src/pydap/wsgi/functions.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/wsgi/ssf.py` & `pydap-3.4.1/src/pydap/wsgi/ssf.py`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/wsgi/templates/base.html` & `pydap-3.4.1/src/pydap/wsgi/templates/base.html`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/wsgi/templates/catalog.xml` & `pydap-3.4.1/src/pydap/wsgi/templates/catalog.xml`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/wsgi/templates/index.html` & `pydap-3.4.1/src/pydap/wsgi/templates/index.html`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap/wsgi/templates/static/style.css` & `pydap-3.4.1/src/pydap/wsgi/templates/static/style.css`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap.egg-info/PKG-INFO` & `pydap-3.4.1/src/pydap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydap
-Version: 3.4.0
+Version: 3.4.1
 Summary: An implementation of the Data Access Protocol.
 Home-page: http://pydap.org/
 Author: Roberto De Almeida
 Author-email: roberto@dealmeida.net
 Maintainer: James Hiebert
 Maintainer-email: james@hiebert.name
 License: MIT
```

### Comparing `pydap-3.4.0/src/pydap.egg-info/SOURCES.txt` & `pydap-3.4.1/src/pydap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap.egg-info/entry_points.txt` & `pydap-3.4.1/src/pydap.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pydap-3.4.0/src/pydap.egg-info/requires.txt` & `pydap-3.4.1/src/pydap.egg-info/requires.txt`

 * *Files identical despite different names*

