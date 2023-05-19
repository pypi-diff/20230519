# Comparing `tmp/crosscompute-0.9.4.4.tar.gz` & `tmp/crosscompute-0.9.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosscompute-0.9.4.4.tar", last modified: Tue May  9 13:27:43 2023, max compression
+gzip compressed data, was "crosscompute-0.9.4.8.tar", last modified: Fri May 19 19:43:47 2023, max compression
```

## Comparing `crosscompute-0.9.4.4.tar` & `crosscompute-0.9.4.8.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-09 13:27:43.789167 crosscompute-0.9.4.4/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1057 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/LICENSE.md
--rw-r--r--   0 rhh       (1000) rhh       (1000)     4968 2023-05-09 13:27:43.789167 crosscompute-0.9.4.4/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3704 2023-05-04 11:08:59.000000 crosscompute-0.9.4.4/README.md
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-09 13:27:43.769167 crosscompute-0.9.4.4/crosscompute/
--rw-r--r--   0 rhh       (1000) rhh       (1000)       22 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/__init__.py
--rw-rw-r--   0 rhh       (1000) rhh       (1000)       38 2022-08-15 04:38:47.000000 crosscompute-0.9.4.4/crosscompute/__main__.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-09 13:27:43.781167 crosscompute-0.9.4.4/crosscompute/assets/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1292 2023-04-26 18:11:29.000000 crosscompute-0.9.4.4/crosscompute/assets/automation.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      910 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/base.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      230 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/button-panel.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      183 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/checkbox-input-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      579 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/checkbox-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      628 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/checkbox-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      109 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/checkbox-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)    13520 2023-05-04 11:08:59.000000 crosscompute-0.9.4.4/crosscompute/assets/configuration.yml
--rw-r--r--   0 rhh       (1000) rhh       (1000)      224 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/default.css
--rw-r--r--   0 rhh       (1000) rhh       (1000)       48 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/embedded.css
--rw-r--r--   0 rhh       (1000) rhh       (1000)    22382 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/favicon.ico
--rw-r--r--   0 rhh       (1000) rhh       (1000)      765 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/file-input-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      165 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/file-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/file-input.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      737 2023-05-09 05:18:59.000000 crosscompute-0.9.4.4/crosscompute/assets/flex.css
--rw-r--r--   0 rhh       (1000) rhh       (1000)      180 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/frame-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/frame-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      138 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/image-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/image-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      156 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/json-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      139 2023-04-25 22:48:18.000000 crosscompute-0.9.4.4/crosscompute/assets/json-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      149 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/link-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/link-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)     2566 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/live.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      301 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/markdown-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      142 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/markdown-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      136 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/pdf-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      137 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/pdf-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)       64 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/pdf.css
--rw-r--r--   0 rhh       (1000) rhh       (1000)       53 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/printed.css
--rw-r--r--   0 rhh       (1000) rhh       (1000)       96 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/radio-input-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      575 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/radio-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      594 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/radio-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/radio-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      366 2023-05-04 11:08:59.000000 crosscompute-0.9.4.4/crosscompute/assets/root.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3271 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/step-body.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      874 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/step.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)       65 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/string-input-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      432 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/string-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      369 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/string-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      122 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/string-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1095 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/table-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      139 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/table-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      159 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/text-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      136 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/text-input.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      109 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/text-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      138 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/text-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)     2886 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/constants.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     5072 2023-04-01 20:58:16.000000 crosscompute-0.9.4.4/crosscompute/dependencies.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1055 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/exceptions.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-09 13:27:43.782167 crosscompute-0.9.4.4/crosscompute/macros/
--rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-08-15 04:38:47.000000 crosscompute-0.9.4.4/crosscompute/macros/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      717 2023-04-05 23:51:33.000000 crosscompute-0.9.4.4/crosscompute/macros/disk.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1530 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/macros/iterable.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1088 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/macros/log.py
--rw-rw-r--   0 rhh       (1000) rhh       (1000)      597 2022-08-15 04:38:47.000000 crosscompute-0.9.4.4/crosscompute/macros/package.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1349 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/macros/security.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-09 13:27:43.783167 crosscompute-0.9.4.4/crosscompute/routers/
--rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/routers/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     7021 2023-04-26 18:11:29.000000 crosscompute-0.9.4.4/crosscompute/routers/automation.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1142 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/routers/file.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3286 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/routers/root.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1240 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/routers/stream.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      523 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/routers/token.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-09 13:27:43.786167 crosscompute-0.9.4.4/crosscompute/routines/
--rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-08-15 04:38:47.000000 crosscompute-0.9.4.4/crosscompute/routines/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3195 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/routines/asset.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3457 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/routines/authorization.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     4806 2023-05-09 05:09:01.000000 crosscompute-0.9.4.4/crosscompute/routines/automation.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3537 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/routines/batch.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)    42419 2023-05-09 12:59:04.000000 crosscompute-0.9.4.4/crosscompute/routines/configuration.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     9409 2023-05-04 11:08:59.000000 crosscompute-0.9.4.4/crosscompute/routines/database.py
--rw-rw-r--   0 rhh       (1000) rhh       (1000)      914 2022-08-15 04:38:47.000000 crosscompute-0.9.4.4/crosscompute/routines/interface.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1404 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/routines/log.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1523 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/routines/mutation.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     6222 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/routines/printer.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     6803 2023-05-09 05:01:53.000000 crosscompute-0.9.4.4/crosscompute/routines/server.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     7390 2023-05-09 05:11:33.000000 crosscompute-0.9.4.4/crosscompute/routines/step.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      605 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/routines/uri.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)    30285 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/routines/variable.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)    28399 2023-05-09 13:25:17.000000 crosscompute-0.9.4.4/crosscompute/routines/work.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-09 13:27:43.787167 crosscompute-0.9.4.4/crosscompute/scripts/
--rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-08-15 04:38:47.000000 crosscompute-0.9.4.4/crosscompute/scripts/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3866 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/scripts/configure.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3829 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/scripts/launch.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1123 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/scripts/print.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1721 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/scripts/run.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     4065 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/scripts/serve.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1315 2023-05-09 05:07:31.000000 crosscompute-0.9.4.4/crosscompute/settings.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-09 13:27:43.770166 crosscompute-0.9.4.4/crosscompute.egg-info/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     4968 2023-05-09 13:27:43.000000 crosscompute-0.9.4.4/crosscompute.egg-info/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3437 2023-05-09 13:27:43.000000 crosscompute-0.9.4.4/crosscompute.egg-info/SOURCES.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-05-09 13:27:43.000000 crosscompute-0.9.4.4/crosscompute.egg-info/dependency_links.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)      831 2023-05-09 13:27:43.000000 crosscompute-0.9.4.4/crosscompute.egg-info/entry_points.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)      436 2023-05-09 13:27:43.000000 crosscompute-0.9.4.4/crosscompute.egg-info/requires.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)       13 2023-05-09 13:27:43.000000 crosscompute-0.9.4.4/crosscompute.egg-info/top_level.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2022-08-22 13:00:05.000000 crosscompute-0.9.4.4/crosscompute.egg-info/zip-safe
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3253 2023-05-09 13:27:43.790167 crosscompute-0.9.4.4/setup.cfg
--rw-rw-r--   0 rhh       (1000) rhh       (1000)       39 2022-08-15 04:38:47.000000 crosscompute-0.9.4.4/setup.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-09 13:27:43.788167 crosscompute-0.9.4.4/tests/
--rw-rw-r--   0 rhh       (1000) rhh       (1000)      168 2022-08-15 04:38:47.000000 crosscompute-0.9.4.4/tests/test_macros_iterable.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      428 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/tests/test_macros_security.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3759 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/tests/test_routines_configuration.py
--rw-rw-r--   0 rhh       (1000) rhh       (1000)     2285 2022-08-15 04:38:47.000000 crosscompute-0.9.4.4/tests/test_routines_variable.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      656 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/tests/test_routines_work.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-19 19:43:47.130337 crosscompute-0.9.4.8/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1057 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/LICENSE.md
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     4967 2023-05-19 19:43:47.130337 crosscompute-0.9.4.8/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3703 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/README.md
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-19 19:43:47.120337 crosscompute-0.9.4.8/crosscompute/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       22 2023-04-27 21:47:32.000000 crosscompute-0.9.4.8/crosscompute/__init__.py
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)       38 2022-01-21 18:22:22.000000 crosscompute-0.9.4.8/crosscompute/__main__.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-19 19:43:47.125337 crosscompute-0.9.4.8/crosscompute/assets/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    15561 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/LogoBrand-Horizontal-20230501.svg
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1630 2023-05-19 19:24:21.000000 crosscompute-0.9.4.8/crosscompute/assets/automation.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1006 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/base.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      230 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/assets/button-panel.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      183 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/assets/checkbox-input-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      579 2023-02-28 18:19:03.000000 crosscompute-0.9.4.8/crosscompute/assets/checkbox-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      749 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/checkbox-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      121 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/checkbox-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    13854 2023-05-19 19:17:25.000000 crosscompute-0.9.4.8/crosscompute/assets/configuration.yml
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      568 2023-05-19 19:41:05.000000 crosscompute-0.9.4.8/crosscompute/assets/default.css
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       48 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/assets/embedded.css
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    22382 2023-02-28 18:19:03.000000 crosscompute-0.9.4.8/crosscompute/assets/favicon.ico
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      765 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/assets/file-input-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      165 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/assets/file-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      737 2023-05-19 19:41:05.000000 crosscompute-0.9.4.8/crosscompute/assets/flex.css
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      108 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/frame-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       99 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/frame-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      138 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/assets/image-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-28 18:19:03.000000 crosscompute-0.9.4.8/crosscompute/assets/image-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      156 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/assets/json-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      139 2023-05-16 21:06:41.000000 crosscompute-0.9.4.8/crosscompute/assets/json-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      408 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/link-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       98 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/link-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     2556 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/live.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      323 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/markdown-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      148 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/markdown-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      136 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/assets/pdf-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      137 2023-05-16 21:07:00.000000 crosscompute-0.9.4.8/crosscompute/assets/pdf-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       64 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/assets/pdf.css
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       96 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/assets/radio-input-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      575 2023-02-28 18:19:03.000000 crosscompute-0.9.4.8/crosscompute/assets/radio-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      660 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/radio-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      118 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/radio-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      366 2023-05-15 19:34:28.000000 crosscompute-0.9.4.8/crosscompute/assets/root.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3275 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/step-body.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1021 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/step.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       65 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/assets/string-input-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      432 2023-02-28 18:19:03.000000 crosscompute-0.9.4.8/crosscompute/assets/string-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      479 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/string-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      128 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/string-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1095 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/assets/table-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      139 2023-05-16 21:07:09.000000 crosscompute-0.9.4.8/crosscompute/assets/table-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      159 2023-02-28 18:19:03.000000 crosscompute-0.9.4.8/crosscompute/assets/text-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      136 2023-02-28 18:19:03.000000 crosscompute-0.9.4.8/crosscompute/assets/text-input.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      131 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/text-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      144 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/assets/text-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3287 2023-05-19 19:17:57.000000 crosscompute-0.9.4.8/crosscompute/constants.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     5072 2023-03-30 19:34:16.000000 crosscompute-0.9.4.8/crosscompute/dependencies.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1055 2022-12-12 19:44:41.000000 crosscompute-0.9.4.8/crosscompute/exceptions.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-19 19:43:47.126337 crosscompute-0.9.4.8/crosscompute/macros/
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-01-21 18:22:22.000000 crosscompute-0.9.4.8/crosscompute/macros/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      717 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/macros/disk.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1551 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/macros/iterable.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1088 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/macros/log.py
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)      597 2022-03-14 16:37:10.000000 crosscompute-0.9.4.8/crosscompute/macros/package.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1349 2023-02-28 18:19:03.000000 crosscompute-0.9.4.8/crosscompute/macros/security.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-19 19:43:47.127337 crosscompute-0.9.4.8/crosscompute/routers/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-02-28 18:19:03.000000 crosscompute-0.9.4.8/crosscompute/routers/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     6373 2023-05-19 19:39:24.000000 crosscompute-0.9.4.8/crosscompute/routers/automation.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1142 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routers/file.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3451 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routers/root.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1240 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routers/stream.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      517 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routers/token.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-19 19:43:47.128337 crosscompute-0.9.4.8/crosscompute/routines/
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-01-21 18:22:22.000000 crosscompute-0.9.4.8/crosscompute/routines/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3195 2023-05-16 17:05:41.000000 crosscompute-0.9.4.8/crosscompute/routines/asset.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3401 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routines/authorization.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     4806 2023-05-15 19:34:28.000000 crosscompute-0.9.4.8/crosscompute/routines/automation.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3508 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routines/batch.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    43690 2023-05-19 19:19:15.000000 crosscompute-0.9.4.8/crosscompute/routines/configuration.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    10401 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routines/database.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1333 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routines/interface.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1428 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routines/log.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     2429 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routines/mutation.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     6177 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routines/printer.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     6803 2023-05-15 19:34:28.000000 crosscompute-0.9.4.8/crosscompute/routines/server.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     9981 2023-05-19 19:39:37.000000 crosscompute-0.9.4.8/crosscompute/routines/step.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      699 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routines/uri.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    30435 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routines/variable.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    28816 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/routines/work.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-19 19:43:47.129336 crosscompute-0.9.4.8/crosscompute/scripts/
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-01-21 18:22:22.000000 crosscompute-0.9.4.8/crosscompute/scripts/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3870 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/scripts/configure.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3846 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/scripts/launch.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1123 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/scripts/print.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1721 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/scripts/run.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     4065 2023-04-27 21:48:39.000000 crosscompute-0.9.4.8/crosscompute/scripts/serve.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1403 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/crosscompute/settings.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-19 19:43:47.120337 crosscompute-0.9.4.8/crosscompute.egg-info/
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)     4967 2023-05-19 19:43:47.000000 crosscompute-0.9.4.8/crosscompute.egg-info/PKG-INFO
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)     3449 2023-05-19 19:43:47.000000 crosscompute-0.9.4.8/crosscompute.egg-info/SOURCES.txt
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)        1 2023-05-19 19:43:47.000000 crosscompute-0.9.4.8/crosscompute.egg-info/dependency_links.txt
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)      831 2023-05-19 19:43:47.000000 crosscompute-0.9.4.8/crosscompute.egg-info/entry_points.txt
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)      427 2023-05-19 19:43:47.000000 crosscompute-0.9.4.8/crosscompute.egg-info/requires.txt
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)       13 2023-05-19 19:43:47.000000 crosscompute-0.9.4.8/crosscompute.egg-info/top_level.txt
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)        1 2022-01-21 22:12:56.000000 crosscompute-0.9.4.8/crosscompute.egg-info/zip-safe
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3257 2023-05-19 19:43:47.131337 crosscompute-0.9.4.8/setup.cfg
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)       39 2022-01-21 18:22:22.000000 crosscompute-0.9.4.8/setup.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-19 19:43:47.130337 crosscompute-0.9.4.8/tests/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      665 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/tests/test_constants.py
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)      168 2022-01-21 18:22:22.000000 crosscompute-0.9.4.8/tests/test_macros_iterable.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      428 2023-02-28 18:19:03.000000 crosscompute-0.9.4.8/tests/test_macros_security.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3759 2023-04-27 21:47:32.000000 crosscompute-0.9.4.8/tests/test_routines_configuration.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     2294 2023-05-19 19:03:42.000000 crosscompute-0.9.4.8/tests/test_routines_variable.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      656 2023-04-27 21:47:32.000000 crosscompute-0.9.4.8/tests/test_routines_work.py
```

### Comparing `crosscompute-0.9.4.4/LICENSE.md` & `crosscompute-0.9.4.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.4/PKG-INFO` & `crosscompute-0.9.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosscompute
-Version: 0.9.4.4
+Version: 0.9.4.8
 Summary: Automate your Jupyter notebooks and scripts as tools, reports, dashboards.
 Home-page: https://crosscompute.com
 Author: CrossCompute Inc.
 Author-email: support@crosscompute.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/crosscompute/crosscompute/issues
 Project-URL: Documentation, https://docs.crosscompute.com
@@ -78,17 +78,17 @@
 # Initialize configuration
 crosscompute
 
 # Serve automation
 crosscompute automate.yml
 ```
 
-Here are some tutorials and examples:
+Here are some examples and tutorials:
 
-- [Examples](https://crosscompute.net) [[source](https://github.com/crosscompute/crosscompute-examples)]
+- [Gallery](https://crosscompute.net) [[source](https://github.com/crosscompute/crosscompute-examples)]
 - [Documentation](https://docs.crosscompute.com) [[source](https://github.com/crosscompute/crosscompute-docs)]
 - [Forum](https://forum.crosscompute.com)
 
 ## Development
 
 ```bash
 # Clone repository
@@ -134,19 +134,19 @@
 source ~/.virtualenvs/crosscompute/bin/activate
 
 pip install crosscompute>=0.9.4
 ```
 
 ## Acknowledgments
 
+- [Kashfi Fahim](https://www.linkedin.com/in/kashfifahim)
 - [Olga Ryabtseva](https://www.linkedin.com/in/olga-creutzburg)
 - [Salah Ahmed](https://www.linkedin.com/in/salahspage)
 - [Rodrigo Guarachi](https://www.linkedin.com/in/rmguarachi)
 - [Polina Chernomaz](https://www.linkedin.com/in/polinac)
 - [Miguel Ángel Gordián](https://www.linkedin.com/in/miguelgordian)
 - [Noé Domínguez Porras](https://www.linkedin.com/in/noedominguez)
 - [Marta Moreno](https://www.linkedin.com/in/marta-moreno-07364b82)
 - [Ning Wei](https://www.linkedin.com/in/ning-wei-8152393b)
-- [Kashfi Fahim](https://www.linkedin.com/in/kashfifahim)
 - [Elaine Chan](https://www.linkedin.com/in/chanelaine)
 - [Aida Shoydokova](https://www.linkedin.com/in/ashoydok)
 - [Jennifer Ruda](https://www.linkedin.com/in/jruda)
```

### Comparing `crosscompute-0.9.4.4/README.md` & `crosscompute-0.9.4.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,17 @@
 # Initialize configuration
 crosscompute
 
 # Serve automation
 crosscompute automate.yml
 ```
 
-Here are some tutorials and examples:
+Here are some examples and tutorials:
 
-- [Examples](https://crosscompute.net) [[source](https://github.com/crosscompute/crosscompute-examples)]
+- [Gallery](https://crosscompute.net) [[source](https://github.com/crosscompute/crosscompute-examples)]
 - [Documentation](https://docs.crosscompute.com) [[source](https://github.com/crosscompute/crosscompute-docs)]
 - [Forum](https://forum.crosscompute.com)
 
 ## Development
 
 ```bash
 # Clone repository
@@ -104,19 +104,19 @@
 source ~/.virtualenvs/crosscompute/bin/activate
 
 pip install crosscompute>=0.9.4
 ```
 
 ## Acknowledgments
 
+- [Kashfi Fahim](https://www.linkedin.com/in/kashfifahim)
 - [Olga Ryabtseva](https://www.linkedin.com/in/olga-creutzburg)
 - [Salah Ahmed](https://www.linkedin.com/in/salahspage)
 - [Rodrigo Guarachi](https://www.linkedin.com/in/rmguarachi)
 - [Polina Chernomaz](https://www.linkedin.com/in/polinac)
 - [Miguel Ángel Gordián](https://www.linkedin.com/in/miguelgordian)
 - [Noé Domínguez Porras](https://www.linkedin.com/in/noedominguez)
 - [Marta Moreno](https://www.linkedin.com/in/marta-moreno-07364b82)
 - [Ning Wei](https://www.linkedin.com/in/ning-wei-8152393b)
-- [Kashfi Fahim](https://www.linkedin.com/in/kashfifahim)
 - [Elaine Chan](https://www.linkedin.com/in/chanelaine)
 - [Aida Shoydokova](https://www.linkedin.com/in/ashoydok)
 - [Jennifer Ruda](https://www.linkedin.com/in/jruda)
```

### Comparing `crosscompute-0.9.4.4/crosscompute/assets/automation.html` & `crosscompute-0.9.4.8/crosscompute/assets/automation.html`

 * *Files 14% similar despite different names*

```diff
@@ -6,41 +6,49 @@
 <meta name="description" property="og:description" content="{{ description }}">
 <meta name="image" property="og:image" content="{{ host_uri }}{{ root_uri }}/favicon.ico" />
 <meta property="og:url" content="{{ host_uri }}{{ root_uri }}{{ uri }}" />
 <meta name="twitter:card" content="summary">
 {% endblock %}
 
 {% block header_html %}
-{% if not for_embed %}
-<a href="{{ root_uri or '/' }}">Root</a> &gt;
-<a href="{{ root_uri }}{{ uri }}">{{ name }}</a>
+{% if not for_embed and not for_print %}
+<nav class="_breadcrumb" aria-label="breadcrumb">
+<ul>
+<li><a href="{{ copyright_uri }}" target="_blank">{{ copyright_name }}</a></li>
+<li><a href="{{ root_uri or '/' }}">Automations</a></li>
+<li><a href="{{ root_uri }}{{ uri }}" aria-current="page">{{ name }}</a></li>
+</ul>
+</nav>
 {% endif %}
 {% endblock %}
 
 {% block main_html %}
 {% if step_name != 'none' %}
 {{ super() -}}
 {% endif %}
 {% endblock %}
 
 {% block footer_html %}
-{% if not for_embed %}
+{% if not for_embed and not for_print %}
 <ul class="_batches">
 {% for batch_definition in batch_definitions %}
 {% set absolute_batch_uri = root_uri + uri + batch_definition.uri %}
 <li>
 {{ batch_definition.name }}
 <a href="{{ absolute_batch_uri }}/i">input</a>
 <a href="{{ absolute_batch_uri }}/o">output</a>
 {% if automation_definition.variable_definitions_by_step_name['print'] %}
 <a href="{{ absolute_batch_uri }}/p">print</a>
 {% endif %}
 </li>
 {% endfor %}
 </ul>
 {% endif %}
+{% if not for_embed and attribution_text %}
+<p class="_attribution">{{ attribution_text | safe }}</p>
+{% endif %}
 {% endblock %}
 
 {% block body_js %}
 {% include 'step-body.js' %}
 {{ super() -}}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,17 +1,23 @@
 {% extends live_template_path %} {% block head_html %} {{ super() -}}
 
 
 
 
- {% endblock %} {% block header_html %} {% if not for_embed %} Root > {{_name
-}} {% endif %} {% endblock %} {% block main_html %} {% if step_name != 'none'
-%} {{ super() -}} {% endif %} {% endblock %} {% block footer_html %} {% if not
-for_embed %}
+ {% endblock %} {% block header_html %} {% if not for_embed and not for_print
+%}
+    * {{_copyright_name_}}
+    * Automations
+    * {{_name_}}
+ {% endif %} {% endblock %} {% block main_html %} {% if step_name != 'none' %}
+{{ super() -}} {% endif %} {% endblock %} {% block footer_html %} {% if not
+for_embed and not for_print %}
     * {% for batch_definition in batch_definitions %} {% set absolute_batch_uri
       = root_uri + uri + batch_definition.uri %}
     * {{ batch_definition.name }} input output {% if
       automation_definition.variable_definitions_by_step_name['print'] %} print
       {% endif %}
     * {% endfor %}
+{% endif %} {% if not for_embed and attribution_text %}
+{{ attribution_text | safe }}
 {% endif %} {% endblock %} {% block body_js %} {% include 'step-body.js' %} {
 { super() -}} {% endblock %}
```

### Comparing `crosscompute-0.9.4.4/crosscompute/assets/checkbox-input.html` & `crosscompute-0.9.4.8/crosscompute/assets/checkbox-input.html`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.4/crosscompute/assets/checkbox-output-header.js` & `crosscompute-0.9.4.8/crosscompute/assets/checkbox-output-header.js`

 * *Files 21% similar despite different names*

#### js-beautify {}

```diff
@@ -1,24 +1,22 @@
-async function refreshCheckbox(elementId, dataUri) {
-    let d;
-    try {
-        const r = await fetch(dataUri + '.json');
-        d = await r.json();
-    } catch {
-        return;
+async function refreshCheckbox(elementId, dataUri, dataValue, dataConfiguration) {
+    const x = dataValue,
+        options = dataConfiguration?.['options'],
+        l = document.getElementById(elementId),
+        vs = x !== undefined ? x.split('\n') : [];
+    if (options !== undefined) {
+        const hs = [],
+            i = l.dataset.variable;
+        for (let j = 0; j < options.length; j++) {
+            const o = options[j],
+                v = o.value,
+                n = o.name || v,
+                w = vs.includes(v) ? ' checked' : '';
+            hs.push(`<div><input type="checkbox" id="${i}-${j}" name="${i}" value="${v}"${w}> <label for="${i}-${j}">${n}</label></div>`);
+        }
+        l.innerHTML = hs.join('\n');
+    } else if (vs.length) {
+        for (const g of l.querySelectorAll('input')) {
+            g.checked = vs.includes(g.value);
+        }
     }
-    const l = document.getElementById(elementId),
-        i = l.dataset.variable,
-        hs = [],
-        {
-            options
-        } = d.configuration,
-        vs = d.value.split('\n');
-    for (let j = 0; j < options.length; j++) {
-        const option = options[j],
-            v = option.value,
-            n = option.name || v,
-            x = vs.includes(v) ? ' checked' : '';
-        hs.push(`<div><input type="checkbox" id="${i}-${j}" name="${i}" value="${v}"${x}> <label for="${i}-${j}">${n}</label></div>`);
-    }
-    l.innerHTML = hs.join('\n');
 }
```

### Comparing `crosscompute-0.9.4.4/crosscompute/assets/configuration.yml` & `crosscompute-0.9.4.8/crosscompute/assets/configuration.yml`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,23 @@
 # Documentation: https://docs.crosscompute.com
 # Forum: https://forum.crosscompute.com
 # Gallery: https://crosscompute.net
 
 # crosscompute version determines how this file is interpreted (required)
 crosscompute: 0.0.0
 
+# copyright declares who owns the rights to this work
+copyright_name: CrossCompute
+copyright_uri: https://crosscompute.com
+copyright_year: 2023
+attribution_text: >-
+  [![CrossCompute](/assets/logo.svg)]({copyright_uri}) © {copyright_year}.
+  Made with the
+  [CrossCompute Software Development Kit](https://docs.crosscompute.com).
+
 # name summarizes what your automation does
 name: Automation X
 
 # slug customizes the automation uri
 slug: automation-x
 
 # title sets the page title
@@ -297,16 +306,16 @@
   # image is the container used to run your scripts when using podman engine
   image: python
 
   # packages are installed in the container when using podman engine
   packages:
     # id is the name of the package as defined in the package manager
     # manager is the name of a package manager such as apt, dnf, npm, pip
-    - id: chromium
-      manager: apt
+    - id: matplotlib
+      manager: pip
 
   # ports expose server processes running in your scripts
   ports:
     # id should correspond to a log or debug variable id that uses frame view;
     # number is the port on which your script server process is listening
     - id: demo
       number: 8888
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `crosscompute-0.9.4.4/crosscompute/assets/favicon.ico` & `crosscompute-0.9.4.8/crosscompute/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.4/crosscompute/assets/file-input-header.js` & `crosscompute-0.9.4.8/crosscompute/assets/file-input-header.js`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.4/crosscompute/assets/flex.css` & `crosscompute-0.9.4.8/crosscompute/assets/flex.css`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.4/crosscompute/assets/live.html` & `crosscompute-0.9.4.8/crosscompute/assets/live.html`

 * *Files 10% similar despite different names*

```diff
@@ -8,33 +8,34 @@
   const ys = xs[k];
   if (ys === undefined) {
     xs[k] = [v];
   } else {
     ys.push(v);
   }
 }
-function registerCallback(variableId, f) {
-  register(callbacks, variableId, f);
+function registerCallback(i, f) {
+  register(callbacks, i, f);
 }
 </script>
 {% endblock %}
 
 {% block body_js %}
 {% if step_name != 'input' %}
-async function refreshVariable(variableId) {
-  await runEach(functions[variableId]);
-  await runEach(callbacks[variableId]);
+async function refreshVariable(i, v, c) {
+  const d = {v, c};
+  await runEach(functions[i], d);
+  await runEach(callbacks[i], d);
 {% if not with_restart and not has_interval %}
-  if (variableId == 'return_code') {
+  if (i == 'return_code') {
     mutationStream.close();
   }
 {% endif %}
 }
-async function runEach(xs) {
-  await Promise.all((xs || []).map(_ => _()));
+async function runEach(fs, v, c) {
+  await Promise.all((fs || []).map(_ => _(v, c)));
 }
 {% endif %}
 {{ super() -}}
 {% if with_restart or is_done == 0 %}
 {% if with_restart %}
 async function refreshPage() {
   const { status } = await fetch(location.href, { method: 'head' });
@@ -73,24 +74,24 @@
     }
   };
   mutationStream.onmessage = async ({ data }) => {
     d = JSON.parse(data);
 {% if with_restart %}
     if (
       d.server_time != {{ server_time }} ||
-      d.configurations.length ||
-      d.templates.length
+      d.configurations ||
+      d.templates
     ) {
       refreshPage();
-    } else if (d.styles.length) {
+    } else if (d.styles) {
       refreshStyle();
     }
 {% endif %}
 {% if step_name != 'input' %}
-    await Promise.all(d.variables.map(_ => refreshVariable(_.id)));
+    await Promise.all((d.variables || []).map(({ i, v, c }) => refreshVariable(i, v, c)));
 {% endif %}
     mutationTime = d.mutation_time;
   };
 }
 let mutationStream, mutationTimeout, mutationTime = {{ mutation_time }}, retrySeconds = 1;
 setupMutationStream();
 {% endif %}
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
 {% extends base_template_path %} {% block head_html %} {{ super() -}}
  {% endblock %} {% block body_js %} {% if step_name != 'input' %} async
-function refreshVariable(variableId) { await runEach(functions[variableId]);
-await runEach(callbacks[variableId]); {% if not with_restart and not
-has_interval %} if (variableId == 'return_code') { mutationStream.close(); } {%
-endif %} } async function runEach(xs) { await Promise.all((xs || []).map(_ => _
-())); } {% endif %} {{ super() -}} {% if with_restart or is_done == 0 %} {% if
+function refreshVariable(i, v, c) { const d = {v, c}; await runEach(functions
+[i], d); await runEach(callbacks[i], d); {% if not with_restart and not
+has_interval %} if (i == 'return_code') { mutationStream.close(); } {% endif %}
+} async function runEach(fs, v, c) { await Promise.all((fs || []).map(_ => _(v,
+c))); } {% endif %} {{ super() -}} {% if with_restart or is_done == 0 %} {% if
 with_restart %} async function refreshPage() { const { status } = await fetch
 (location.href, { method: 'head' }); switch (status) { case 200:
 location.reload(); break; case 404: location.href = '{{ root_uri or '/' }}';
 break; default: setTimeout(refreshPage, 1000); } } function refreshStyle()
 { const { origin } = location; for (var l of document.getElementsByTagName
 ('link')) { if (l.rel !== 'stylesheet' || new URL(l.href).origin !== origin)
 { continue; } l.href += '?' + Date.now(); } } {% endif %} function
 setupMutationStream() { mutationStream = new EventSource(rootUri + '/streams{
 { mutation_uri }}?t=' + mutationTime); mutationStream.onopen = () =>
 { retrySeconds = 1; }; mutationStream.onerror = () => { mutationStream.close();
 clearTimeout(mutationTimeout); mutationTimeout = setTimeout
 (setupMutationStream, retrySeconds); if (retrySeconds < 60) { retrySeconds *=
 2; } }; mutationStream.onmessage = async ({ data }) => { d = JSON.parse(data);
 {% if with_restart %} if ( d.server_time != {{ server_time }} ||
-d.configurations.length || d.templates.length ) { refreshPage(); } else if
-(d.styles.length) { refreshStyle(); } {% endif %} {% if step_name != 'input' %}
-await Promise.all(d.variables.map(_ => refreshVariable(_.id))); {% endif %}
-mutationTime = d.mutation_time; }; } let mutationStream, mutationTimeout,
+d.configurations || d.templates ) { refreshPage(); } else if (d.styles)
+{ refreshStyle(); } {% endif %} {% if step_name != 'input' %} await Promise.all
+((d.variables || []).map(({ i, v, c }) => refreshVariable(i, v, c))); {% endif
+%} mutationTime = d.mutation_time; }; } let mutationStream, mutationTimeout,
 mutationTime = {{ mutation_time }}, retrySeconds = 1; setupMutationStream(); {%
 endif %} {% endblock %}
```

### Comparing `crosscompute-0.9.4.4/crosscompute/assets/radio-input.html` & `crosscompute-0.9.4.8/crosscompute/assets/radio-input.html`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.4/crosscompute/assets/step-body.js` & `crosscompute-0.9.4.8/crosscompute/assets/step-body.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -3,16 +3,15 @@
     if template_count == 1 %
 }
 document.querySelectorAll('._continue').forEach(function(l) {
     if (!l.onclick) {
         l.onclick = runAutomation;
     }
 }); {
-    %
-    else %
+    % elif design_name != 'none' %
 }
 async function showNext() {
     let newElement, isThis = false;
     if (newTemplateIndex >= 0) {
         templateIndices.push(newTemplateIndex);
     }
     while (!isThis) {
@@ -120,16 +119,16 @@
     return d;
 }
 const GET_DATA_BY_VIEW_NAME = {}; {
     %
     if step_name != 'input' %
 }
 
-function registerFunction(variableId, f) {
-    register(functions, variableId, f);
+function registerFunction(i, f) {
+    register(functions, i, f);
 }
 const functions = {}; {
     %
     if step_name == 'log' %
 }
 registerFunction('return_code', function() {
     location = location.href.slice(0, -1) + 'o';
```

### Comparing `crosscompute-0.9.4.4/crosscompute/assets/table-output-header.js` & `crosscompute-0.9.4.8/crosscompute/assets/table-output-header.js`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.4/crosscompute/constants.py` & `crosscompute-0.9.4.8/crosscompute/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from datetime import datetime
 from enum import IntEnum
 from os import getenv
 from pathlib import Path
 
 
 class Status(IntEnum):
 
@@ -50,29 +51,38 @@
 ID_LENGTH = 32
 TOKEN_LENGTH = 32
 
 
 AUTOMATION_NAME = 'Automation X'
 AUTOMATION_VERSION = '0.0.0'
 AUTOMATION_PATH = Path('automate.yml')
+COPYRIGHT_NAME = 'CrossCompute'
+COPYRIGHT_URI = 'https://crosscompute.com'
+COPYRIGHT_YEAR = datetime.now().year
+ATTRIBUTION_TEXT = '''
+[![CrossCompute](/assets/logo.svg)]({copyright_uri}) © {copyright_year}.
+Made with the
+[CrossCompute Software Development Kit](https://docs.crosscompute.com).
+'''.strip()
+LOGO_PATH = ASSETS_FOLDER / 'LogoBrand-Horizontal-20230501.svg'
 
 
 HOST = '127.0.0.1'
 PORT = 7000
 DISK_DEBOUNCE_IN_MILLISECONDS = 1600
 DISK_STEP_IN_MILLISECONDS = 50
 
 
 AUTOMATION_ROUTE = '/a/{automation_slug}'
 BATCH_ROUTE = '/b/{batch_slug}'
 STEP_ROUTE = '/{step_code}'
 VARIABLE_ROUTE = '/{variable_id}'
 FILES_ROUTE = '/files.json'
 STREAM_ROUTE = '/streams'
-STYLE_ROUTE = '/styles/{style_name}.css'
+STYLE_ROUTE = '/assets/{style_name}.css'
 MUTATION_ROUTE = '/mutations{uri}.json'
 PORT_ROUTE = '/ports{uri}'
 
 
 PRINTER_NAMES = 'pdf',
 
 
@@ -93,16 +103,16 @@
 STEP_NAMES = 'input', 'output', 'log', 'debug', 'print'
 STEP_NAME_BY_CODE = {_[0]: _ for _ in STEP_NAMES}
 STEP_CODE_BY_NAME = {k: v for v, k in STEP_NAME_BY_CODE.items()}
 MAXIMUM_MUTATION_AGE_IN_SECONDS = 180
 
 
 VARIABLE_ID_PATTERN = re.compile(r'[a-zA-Z0-9-_ ]+$')
-VARIABLE_ID_TEMPLATE_PATTERN = re.compile(r'{ *([a-zA-Z0-9-_| ]+?) *}')
 VARIABLE_ID_WHITELIST_PATTERN = re.compile(r'{ *(ROOT_URI) *}')
+VARIABLE_ID_TEMPLATE_PATTERN = re.compile(r'{ *([a-zA-Z0-9-_| ]+?) *}')
 CACHED_FILE_SIZE_LIMIT_IN_BYTES = 1024
 MAXIMUM_FILE_CACHE_LENGTH = 256
 
 
 MINIMUM_PORT = int(getenv('CROSSCOMPUTE_MINIMUM_PORT', 1024))
 MAXIMUM_PORT = int(getenv('CROSSCOMPUTE_MAXIMUM_PORT', 65535))
 PROXY_URI = getenv('CROSSCOMPUTE_PROXY_URI', '')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `crosscompute-0.9.4.4/crosscompute/dependencies.py` & `crosscompute-0.9.4.8/crosscompute/dependencies.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.4/crosscompute/exceptions.py` & `crosscompute-0.9.4.8/crosscompute/exceptions.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.4/crosscompute/macros/disk.py` & `crosscompute-0.9.4.8/crosscompute/macros/disk.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.4/crosscompute/macros/iterable.py` & `crosscompute-0.9.4.8/crosscompute/macros/iterable.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,13 +43,13 @@
             normalized_v = normalize(v)
             is_match = compare(normalized_value, normalized_v)
         return is_match
 
     return next(filter(is_match, items))
 
 
-def get_unique_order(items):
-    return list(dict.fromkeys(items))
+def get_unique_order(texts):
+    return list(dict.fromkeys([_.strip() for _ in texts]))
 
 
 def extend_uniquely(old_items, new_items):
     old_items.extend(_ for _ in new_items if _ not in old_items)
```

### Comparing `crosscompute-0.9.4.4/crosscompute/macros/log.py` & `crosscompute-0.9.4.8/crosscompute/macros/log.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.4/crosscompute/macros/package.py` & `crosscompute-0.9.4.8/crosscompute/macros/package.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.4/crosscompute/macros/security.py` & `crosscompute-0.9.4.8/crosscompute/macros/security.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.4/crosscompute/routers/automation.py` & `crosscompute-0.9.4.8/crosscompute/routers/automation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-from logging import getLogger
 from pathlib import Path
 from time import time
 
 from fastapi import APIRouter, Depends, Request, Response, HTTPException
 from fastapi.responses import FileResponse
 from invisibleroads_macros_disk import make_random_folder
 
 from ..constants import (
     Task,
     AUTOMATION_ROUTE,
     BATCH_ROUTE,
     ID_LENGTH,
-    MUTATION_ROUTE,
     STEP_ROUTE,
     VARIABLE_ROUTE)
 from ..dependencies import (
     AuthorizationGuardFactory,
     get_automation_definition,
     get_batch_definition,
     get_data_by_id,
@@ -24,21 +22,26 @@
 from ..routines.authorization import AuthorizationGuard
 from ..routines.batch import DiskBatch
 from ..routines.configuration import (
     AutomationDefinition,
     BatchDefinition,
     VariableDefinition)
 from ..routines.step import (
+    get_automation_response_dictionary,
+    get_layout_settings,
     get_step_response_dictionary)
+from ..routines.uri import (
+    get_host_uri)
 from ..routines.variable import (
     load_file_text,
     remove_variable_data)
 from ..settings import (
     TemplateResponse,
     site,
+    template_globals,
     template_path_by_id)
 
 
 router = APIRouter()
 
 
 @router.get(
@@ -47,34 +50,54 @@
 async def see_automation(
     request: Request, response: Response,
     automation_definition: AutomationDefinition = Depends(
         get_automation_definition),
     guard: AuthorizationGuard = Depends(
         AuthorizationGuardFactory('see_automation')),
 ):
-    automation_uri = automation_definition.uri
-    design_name = automation_definition.get_design_name('automation')
-    if design_name == 'none':
-        d = {
-            'css_uris': automation_definition.css_uris, 'is_done': 1,
-            'mutation_uri': MUTATION_ROUTE.format(uri=automation_uri)}
-    else:
-        d = get_step_response_dictionary(
-            automation_definition, automation_definition.batch_definitions[0],
-            design_name, request.query_params)
-    request_uri = request.url
+    d = get_automation_response_dictionary(
+        automation_definition, template_globals['root_uri'],
+        request.query_params)
     return TemplateResponse(template_path_by_id['automation'], {
-        'request': request, 'title_text': automation_definition.title,
+        'request': request,
+        'title_text': automation_definition.title,
         'description': automation_definition.description,
-        'host_uri': request_uri.scheme + '://' + request_uri.netloc,
-        'name': automation_definition.name, 'uri': automation_uri,
         'automation_definition': automation_definition,
-        'step_name': design_name,
         'batch_definitions': guard.get_batch_definitions(
             automation_definition),
+        'host_uri': get_host_uri(request),
+        'mutation_time': time(),
+    } | d, headers=response.headers)
+
+
+@router.get(
+    AUTOMATION_ROUTE + BATCH_ROUTE + STEP_ROUTE,
+    tags=['automation'])
+async def see_automation_batch_step(
+    request: Request,
+    response: Response,
+    automation_definition: AutomationDefinition = Depends(
+        get_automation_definition),
+    batch_definition: BatchDefinition = Depends(get_batch_definition),
+    step_name: str = Depends(get_step_name),
+    guard: AuthorizationGuard = Depends(
+        AuthorizationGuardFactory('see_batch')),
+):
+    request_params = request.query_params
+    layout_settings = get_layout_settings(
+        automation_definition.get_design_name(step_name), request_params)
+    d = get_step_response_dictionary(
+        automation_definition, batch_definition, step_name,
+        template_globals['root_uri'], layout_settings, request_params)
+    return TemplateResponse(template_path_by_id['step'], {
+        'request': request,
+        'title_text': batch_definition.name,
+        'automation_definition': automation_definition,
+        'batch_definition': batch_definition,
+        'step_name': step_name,
         'mutation_time': time(),
     } | d, headers=response.headers)
 
 
 @router.post(
     AUTOMATION_ROUTE + '.json',
     tags=['automation'])
@@ -104,54 +127,14 @@
         'log') else 'o'
     return {
         'batch_slug': batch_definition.name,
         'step_code': step_code}
 
 
 @router.get(
-    AUTOMATION_ROUTE + BATCH_ROUTE,
-    tags=['automation'])
-async def see_automation_batch(
-    request: Request,
-    response: Response,
-    guard: AuthorizationGuard = Depends(
-        AuthorizationGuardFactory('see_batch')),
-):
-    return TemplateResponse(template_path_by_id['batch'], {
-        'request': request,
-    }, headers=response.headers)
-
-
-@router.get(
-    AUTOMATION_ROUTE + BATCH_ROUTE + STEP_ROUTE,
-    tags=['automation'])
-async def see_automation_batch_step(
-    request: Request,
-    response: Response,
-    automation_definition: AutomationDefinition = Depends(
-        get_automation_definition),
-    batch_definition: BatchDefinition = Depends(get_batch_definition),
-    step_name: str = Depends(get_step_name),
-    guard: AuthorizationGuard = Depends(
-        AuthorizationGuardFactory('see_batch')),
-):
-    page_dictionary = get_step_response_dictionary(
-        automation_definition, batch_definition, step_name,
-        request.query_params)
-    return TemplateResponse(template_path_by_id['step'], {
-        'request': request,
-        'title_text': batch_definition.name,
-        'automation_definition': automation_definition,
-        'batch_definition': batch_definition,
-        'step_name': step_name,
-        'mutation_time': time(),
-    } | page_dictionary, headers=response.headers)
-
-
-@router.get(
     AUTOMATION_ROUTE + BATCH_ROUTE + STEP_ROUTE + VARIABLE_ROUTE + '.json',
     tags=['automation'])
 async def see_automation_batch_step_variable_json(
     automation_definition: AutomationDefinition = Depends(
         get_automation_definition),
     batch_definition: BatchDefinition = Depends(get_batch_definition),
     variable_definition: VariableDefinition = Depends(
@@ -163,20 +146,20 @@
     variable_data = batch.load_data(variable_definition)
     if 'error' in variable_data:
         raise HTTPException(status_code=404)
     if 'path' in variable_data:
         variable_value = load_file_text(variable_data['path'])
     else:
         variable_value = variable_data['value']
-    variable_configuration = batch.get_variable_configuration(
+    data_configuration = batch.get_data_configuration(
         variable_definition).copy()
-    variable_configuration.pop('path', None)
+    data_configuration.pop('path', None)
     return {
         'value': variable_value,
-        'configuration': variable_configuration}
+        'configuration': data_configuration}
 
 
 @router.get(
     AUTOMATION_ROUTE + BATCH_ROUTE + STEP_ROUTE + VARIABLE_ROUTE,
     tags=['automation'])
 async def see_automation_batch_step_variable(
     response: Response,
@@ -195,10 +178,7 @@
     if 'path' in variable_data:
         r = FileResponse(
             variable_data['path'], headers=response.headers)
     else:
         r = Response(str(
             variable_data['value']), headers=response.headers)
     return r
-
-
-L = getLogger(__name__)
```

### Comparing `crosscompute-0.9.4.4/crosscompute/routers/file.py` & `crosscompute-0.9.4.8/crosscompute/routers/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 async def add_files_json(files: list[UploadFile]):
     file_dictionaries = []
     folder = Path(make_random_folder(FILES_FOLDER))
     for file_index, async_file in enumerate(files):
         name = async_file.filename
         path = folder / str(file_index)
         content_type = async_file.content_type
-        with open(path, 'wb') as f:
+        with path.open('wb') as f:
             f.write(await async_file.read())
         file_dictionaries.append({
             'name': name,
             'type': content_type,
             'size': path.stat().st_size,
             'extension': guess_extension(content_type)})
         L.info(f'saved {name} in {path}')
-    with open(folder / 'files.json', 'wt') as f:
+    with (folder / 'files.json').open('wt') as f:
         json.dump(sorted(file_dictionaries, key=lambda _: _['name']), f)
     return {'uri': f'/f/{folder.name}'}
 
 
 L = getLogger(__name__)
```

### Comparing `crosscompute-0.9.4.4/crosscompute/routers/root.py` & `crosscompute-0.9.4.8/crosscompute/routers/root.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from fastapi import APIRouter, Depends, HTTPException, Request, Response
 from fastapi.responses import FileResponse
 
 from ..constants import (
     ASSETS_FOLDER,
     AUTOMATION_ROUTE,
     BATCH_ROUTE,
+    LOGO_PATH,
     MUTATION_ROUTE,
     STEP_ROUTE,
     STYLE_ROUTE)
 from ..dependencies import (
     AuthorizationGuardFactory,
     get_automation_definition,
     get_batch_definition)
@@ -61,28 +62,33 @@
         AuthorizationGuardFactory('see_root')),
 ):
     'Render root with a list of available automations'
     configuration = site['configuration']
     return TemplateResponse(template_path_by_id['root'], {
         'request': request,
         'title_text': site['name'],
-        'css_uris': configuration.css_uris,
         'automation_definitions': guard.get_automation_definitions(
             configuration),
+        'css_uris': configuration.css_uris,
         'mutation_uri': MUTATION_ROUTE.format(uri=''),
         'mutation_time': time(),
     }, headers=response.headers)
 
 
 @router.get('/favicon.ico', tags=['root'])
 async def see_icon(response: Response):
     return FileResponse(
         ASSETS_FOLDER / 'favicon.ico', headers=response.headers)
 
 
+@router.get('/assets/logo.svg', tags=['root'])
+async def see_logo(response: Response):
+    return FileResponse(LOGO_PATH, headers=response.headers)
+
+
 @router.get(STYLE_ROUTE, tags=['root'])
 async def see_style(request: Request, response: Response):
     return get_style_response(
         site['configuration'], request.url.path, response.headers)
 
 
 @router.get(AUTOMATION_ROUTE + STYLE_ROUTE, tags=['root'])
```

### Comparing `crosscompute-0.9.4.4/crosscompute/routers/stream.py` & `crosscompute-0.9.4.8/crosscompute/routers/stream.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# TODO: Add guard
 import asyncio
 import json
 
 from fastapi import APIRouter, Query
 from sse_starlette.sse import EventSourceResponse
 
 from ..constants import (
@@ -17,27 +18,26 @@
 @router.get(
     STREAM_ROUTE + MUTATION_ROUTE.format(uri='{reference_uri:path}'),
     tags=['stream'])
 async def see_mutation_stream(
     reference_uri: str,
     old_time: float = Query(default=0, alias='t'),
 ):
-    # TODO: Consider adding guard
     live_uris = site['uris']
     file_changes = site['changes']
 
     async def loop():
         live_uris.append(reference_uri)
         reference_time = old_time
         try:
             while True:
                 await asyncio.sleep(1)
                 d = get_mutation(file_changes, reference_uri, reference_time)
-                if d['configurations'] or d['variables'] or d[
-                        'templates'] or d['styles']:
+                if d.get('configurations') or d.get('variables') or d.get(
+                        'templates') or d.get('styles'):
                     reference_time = d['mutation_time']
                     yield {'data': json.dumps(d)}
         except asyncio.CancelledError:
             live_uris.remove(reference_uri)
 
     return EventSourceResponse(
         loop(), ping_message_factory=lambda: {'comment': ''})
```

### Comparing `crosscompute-0.9.4.4/crosscompute/routers/token.py` & `crosscompute-0.9.4.8/crosscompute/routers/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,9 +15,8 @@
     time_in_seconds: int,
     guard: AuthorizationGuard = Depends(
         AuthorizationGuardFactory('add_token')),
 ):
     token = guard.put(identities, time_in_seconds)
     return {
         'access_token': token,
-        'token_type': 'bearer',
-    }
+        'token_type': 'bearer'}
```

### Comparing `crosscompute-0.9.4.4/crosscompute/routines/asset.py` & `crosscompute-0.9.4.8/crosscompute/routines/asset.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.4/crosscompute/routines/authorization.py` & `crosscompute-0.9.4.8/crosscompute/routines/authorization.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-from logging import getLogger
 from types import FunctionType
 
 from ..macros.iterable import find_item
 from ..routines.batch import DiskBatch
 from ..settings import site
 
 
@@ -101,10 +100,7 @@
     if not isinstance(value2, list):
         value2 = [value2]
     for v1 in value1:
         for v2 in value2:
             if v1 == v2:
                 return True
     return False
-
-
-L = getLogger(__name__)
```

### Comparing `crosscompute-0.9.4.4/crosscompute/routines/automation.py` & `crosscompute-0.9.4.8/crosscompute/routines/automation.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.4/crosscompute/routines/batch.py` & `crosscompute-0.9.4.8/crosscompute/routines/batch.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,49 +10,25 @@
 from ..exceptions import (
     CrossComputeDataError)
 from ..settings import (
     template_globals)
 from .interface import Batch
 from .variable import (
     get_data_from,
+    load_file_json,
     load_variable_data)
 
 
 class DiskBatch(Batch):
 
     def __init__(self, automation_definition, batch_definition):
         self.automation_definition = automation_definition
         self.batch_definition = batch_definition
         self.folder = automation_definition.folder / batch_definition.folder
 
-    def get_variable_configuration(self, variable_definition):
-        folder = self.folder
-        variable_configuration = variable_definition.configuration.copy()
-        if 'path' in variable_configuration:
-            relative_path = variable_configuration['path']
-            is_customized = True
-        else:
-            relative_path = str(variable_definition.path) + '.configuration'
-            is_customized = False
-        step_name = variable_definition.step_name
-        path = folder / step_name / relative_path
-        if not is_customized and not path.exists():
-            return variable_configuration
-        try:
-            with path.open('rt') as f:
-                d = json.load(f)
-            variable_configuration.update(d)
-        except OSError:
-            L.error('path not found %s', format_path(path))
-        except json.JSONDecodeError:
-            L.error('must be json %s', format_path(path))
-        except TypeError:
-            L.error('must contain a dictionary %s', format_path(path))
-        return variable_configuration
-
     def load_data_from(self, request_params, variable_definition):
         return get_data_from(
             request_params, variable_definition,
         ) or self.load_data(variable_definition)
 
     def load_data(self, variable_definition):
         variable_path = variable_definition.path
@@ -74,24 +50,47 @@
         batch_uri = self.batch_definition.uri
         step_code = STEP_CODE_BY_NAME[variable_definition.step_name]
         step_uri = STEP_ROUTE.format(step_code=step_code)
         variable_uri = VARIABLE_ROUTE.format(
             variable_id=variable_definition.id)
         return root_uri + automation_uri + batch_uri + step_uri + variable_uri
 
+    def get_data_configuration(self, variable_definition):
+        folder = self.folder
+        variable_configuration = variable_definition.configuration.copy()
+        if 'path' in variable_configuration:
+            relative_path = variable_configuration['path']
+            is_customized = True
+        else:
+            relative_path = str(variable_definition.path) + '.configuration'
+            is_customized = False
+        step_name = variable_definition.step_name
+        path = folder / step_name / relative_path
+        if not is_customized and not path.exists():
+            return variable_configuration
+        try:
+            d = load_file_json(path)
+            variable_configuration.update(d)
+        except OSError:
+            L.error('path "%s" was not found', format_path(path))
+        except json.JSONDecodeError:
+            L.error('path "%s" must contain json', format_path(path))
+        except TypeError:
+            L.error('path "%s" must contain a dictionary', format_path(path))
+        return variable_configuration
+
     def is_done(self):
         if self.automation_definition.interval_timedelta:
             return False
         batch_definition = self.batch_definition
         if hasattr(batch_definition, 'is_done'):
             return True
         path = self.folder / 'debug' / 'variables.dictionary'
         try:
-            with path.open('rt') as f:
-                d = json.load(f)
+            d = load_file_json(path)
             is_done = 'return_code' in d
         except (OSError, ValueError):
             return False
         if is_done:
             batch_definition.is_done = True
         return is_done
```

### Comparing `crosscompute-0.9.4.4/crosscompute/routines/configuration.py` & `crosscompute-0.9.4.8/crosscompute/routines/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 # TODO: Save to ini, toml
-import json
 import shutil
 from collections import Counter, defaultdict
 from configparser import ConfigParser
 from datetime import datetime, timedelta
 from logging import getLogger
 from os import environ
 from os.path import basename, relpath, splitext
 from pathlib import Path
 from string import Template
 from time import time
 
 import tomli
 from invisibleroads_macros_log import format_path
 from invisibleroads_macros_text import format_name, format_slug
+from invisibleroads_macros_web.markdown import (
+    get_html_from_markdown,
+    remove_single_paragraph)
 from nbconvert import PythonExporter
 from nbformat import read as load_notebook, NO_CONVERT
 from ruamel.yaml import YAML
 from ruamel.yaml.error import YAMLError
 
 from .. import __version__
 from ..constants import (
     Status,
+    ATTRIBUTION_TEXT,
     AUTOMATION_NAME,
     AUTOMATION_ROUTE,
     AUTOMATION_VERSION,
     BATCH_ROUTE,
     BUTTON_TEXT_BY_ID,
+    COPYRIGHT_NAME,
+    COPYRIGHT_URI,
+    COPYRIGHT_YEAR,
     DEBUG_VARIABLE_DICTIONARIES,
     DESIGN_NAMES_BY_PAGE_ID,
     INTERVAL_UNIT_NAMES,
     PACKAGE_MANAGER_NAMES,
     PRINTER_NAMES,
     STEP_NAMES,
     STYLE_ROUTE,
@@ -49,14 +55,15 @@
     view_by_name)
 from .printer import (
     initialize_printer_by_name)
 from .variable import (
     format_text,
     get_data_by_id_from_folder,
     initialize_view_by_name,
+    load_file_json,
     YIELD_DATA_BY_ID_BY_EXTENSION)
 
 
 class Definition(dict):
     '''
     A definition validates and preserves the original dictionary while adding
     computed attributes.
@@ -159,15 +166,15 @@
             validate_batch_identifiers,
             validate_batch_configuration]
 
     def get_status(self):
         status = Status.NEW
         path = self.folder / 'debug' / 'variables.dictionary'
         if path.exists():
-            d = json.load(path.open('rt'))
+            d = load_file_json(path)
             return_code = d['return_code']
             status = Status.DONE if return_code == 0 else Status.FAILED
         return status
 
 
 class DatasetDefinition(Definition):
 
@@ -285,20 +292,19 @@
     save_raw_configuration = {
         'yaml': save_raw_configuration_yaml,
     }[configuration_format]
     return save_raw_configuration(configuration_path, configuration)
 
 
 def save_raw_configuration_yaml(configuration_path, configuration):
-    # TODO: Add --- at top
     yaml = YAML()
     yaml.explicit_start = True
     yaml.indent(mapping=2, sequence=4, offset=2)
     try:
-        with open(configuration_path, 'wt') as configuration_file:
+        with configuration_path.open('wt') as configuration_file:
             yaml.dump(configuration, configuration_file)
     except (OSError, YAMLError) as e:
         raise CrossComputeConfigurationError(e)
     return configuration_path
 
 
 def load_configuration(configuration_path, index=0, group_definitions=[]):
@@ -331,66 +337,79 @@
 def load_raw_configuration_ini(configuration_path, with_comments=False):
     configuration = ConfigParser()
     try:
         paths = configuration.read(configuration_path)
     except (OSError, UnicodeDecodeError) as e:
         raise CrossComputeConfigurationError(e)
     if not paths:
-        raise CrossComputeConfigurationError(f'{configuration_path} not found')
+        raise CrossComputeConfigurationError(
+            f'configuration path "{configuration_path}" was not found')
     return dict(configuration)
 
 
 def load_raw_configuration_toml(configuration_path, with_comments=False):
     try:
-        with open(configuration_path, 'rt') as configuration_file:
+        with configuration_path.open('rt') as configuration_file:
             configuration = tomli.load(configuration_file)
     except (OSError, UnicodeDecodeError) as e:
         raise CrossComputeConfigurationError(e)
     return configuration
 
 
 def load_raw_configuration_yaml(configuration_path, with_comments=False):
     yaml = YAML(typ='rt' if with_comments else 'safe')
     try:
-        with open(configuration_path, 'rt') as configuration_file:
+        with configuration_path.open('rt') as configuration_file:
             configuration = yaml.load(configuration_file)
     except (OSError, YAMLError) as e:
         raise CrossComputeConfigurationError(e)
     return configuration or {}
 
 
 def validate_protocol(configuration):
     if 'crosscompute' not in configuration:
-        raise CrossComputeError('crosscompute expected')
+        raise CrossComputeError(
+            'crosscompute was not found in the configuration')
     protocol_version = configuration['crosscompute'].strip()
     if not protocol_version:
-        raise CrossComputeConfigurationError('crosscompute version required')
+        raise CrossComputeConfigurationError(
+            'crosscompute version is required')
     elif not is_equivalent_version(
             protocol_version, __version__, version_depth=3):
         raise CrossComputeConfigurationError(
             f'crosscompute version {protocol_version} is not compatible with '
             f'{__version__}; pip install crosscompute=={protocol_version}')
     return {}
 
 
 def validate_automation_identifiers(configuration):
-    index = configuration.index
-    name = configuration.get('name', make_automation_name(index))
+    name = configuration.get('name', make_automation_name(configuration.index))
     slug = configuration.get('slug', format_slug(name))
-    title = configuration.get('title', name)
-    description = configuration.get('description', name)
-    version = configuration.get('version', AUTOMATION_VERSION)
-    uri = AUTOMATION_ROUTE.format(automation_slug=slug)
+    copyright_name = configuration.get('copyright_name', COPYRIGHT_NAME)
+    copyright_uri = configuration.get('copyright_uri', COPYRIGHT_URI)
+    copyright_year = configuration.get('copyright_year', COPYRIGHT_YEAR)
+    attribution_text = remove_single_paragraph(get_html_from_markdown(
+        configuration.get('attribution_text', ATTRIBUTION_TEXT).format(
+            name=name,
+            copyright_name=copyright_name,
+            copyright_uri=copyright_uri,
+            copyright_year=copyright_year,
+        ), extras=[
+            'target-blank-links',
+        ]))
     return {
         'name': name,
         'slug': slug,
-        'title': title,
-        'description': description,
-        'version': version,
-        'uri': uri}
+        'title': configuration.get('title', name),
+        'description': configuration.get('description', name),
+        'version': configuration.get('version', AUTOMATION_VERSION),
+        'uri': AUTOMATION_ROUTE.format(automation_slug=slug),
+        'copyright_name': copyright_name,
+        'copyright_uri': copyright_uri,
+        'attribution_text': attribution_text}
 
 
 def validate_imports(configuration):
     automation_configurations = [configuration]
     folder = configuration.folder
     group_definitions = getattr(configuration, 'group_definitions', [])
     import_configurations = get_dictionaries(configuration, 'imports')
@@ -400,26 +419,25 @@
             try:
                 automation_configuration = load_configuration(
                     path, index=i, group_definitions=group_definitions)
             except CrossComputeConfigurationFormatError as e:
                 raise CrossComputeConfigurationError(e)
             import_configuration['path'] = path
         else:
-            raise CrossComputeConfigurationError(
-                'path required for each import')
+            raise CrossComputeConfigurationError('import path is required')
         import_configurations.extend(
             automation_configuration.import_configurations)
         automation_configurations.extend(
             automation_configuration.automation_definitions)
     automation_definitions = [
         _ for _ in automation_configurations if 'output' in _]
     assert_unique_values([
-        _.name for _ in automation_definitions], 'duplicate name {x}')
+        _.name for _ in automation_definitions], 'automation name "{x}"')
     assert_unique_values([
-        _.slug for _ in automation_definitions], 'duplicate slug {x}')
+        _.slug for _ in automation_definitions], 'automation slug "{x}"')
     return {
         'import_configurations': import_configurations,
         'automation_definitions': automation_definitions}
 
 
 def validate_variables(configuration):
     variable_definitions_by_step_name = {}
@@ -432,30 +450,31 @@
             step_configuration, 'variables')
         if step_name == 'debug':
             variable_dictionaries[:0] = DEBUG_VARIABLE_DICTIONARIES
         variable_definitions = [VariableDefinition(
             _, step_name=step_name) for _ in variable_dictionaries]
         assert_unique_values([
             _.id for _ in variable_definitions
-        ], f'duplicate variable id {{x}} in {step_name}')
+        ], f'variable id "{{x}}" in {step_name}')
         variable_definitions_by_step_name[step_name] = variable_definitions
         view_names.update(_.view_name for _ in variable_definitions)
     L.debug('view_names = %s', list(view_names))
     return {
         'variable_definitions_by_step_name': variable_definitions_by_step_name,
         '___view_names': view_names}
 
 
 def validate_variable_views(configuration):
     initialize_view_by_name()
     for view_name in configuration.___view_names:
         try:
             View = view_by_name[view_name]
         except KeyError:
-            raise CrossComputeConfigurationError(f'{view_name} not installed')
+            raise CrossComputeConfigurationError(
+                f'view "{view_name}" is not installed')
         environment_variable_ids = get_environment_variable_ids(
             View.environment_variable_definitions)
         if environment_variable_ids:
             L.debug('%s.environment_variable_ids = %s', view_name, list(
                 environment_variable_ids))
     return {}
 
@@ -466,15 +485,15 @@
     for step_name in STEP_NAMES:
         step_configuration = get_dictionary(configuration, step_name)
         template_definitions = [TemplateDefinition(
             _, automation_folder=automation_folder, step_name=step_name,
         ) for _ in get_dictionaries(step_configuration, 'templates')]
         assert_unique_values([
             _.path for _ in template_definitions
-        ], f'duplicate template path {{x}} in {step_name}')
+        ], f'template path "{{x}}" in {step_name}')
         template_definitions_by_step_name[step_name] = template_definitions
     return {
         'template_definitions_by_step_name': template_definitions_by_step_name}
 
 
 def validate_batches(configuration):
     batch_definitions = []
@@ -482,21 +501,21 @@
     automation_folder = configuration.folder
     variable_definitions = configuration.get_variable_definitions('input')
     for raw_batch_definition in raw_batch_definitions:
         batch_definitions.extend(get_batch_definitions(
             raw_batch_definition, automation_folder, variable_definitions))
     if 'output' in configuration and not batch_definitions:
         raise CrossComputeConfigurationError(
-            'no batches configured; please define at least one batch')
+            'no batches are configured; you must define at least one batch')
     assert_unique_values([
-        _.folder for _ in batch_definitions], 'duplicate batch folder {x}')
+        _.folder for _ in batch_definitions], 'batch folder "{x}"')
     assert_unique_values([
-        _.name for _ in batch_definitions], 'duplicate batch name {x}')
+        _.name for _ in batch_definitions], 'batch name "{x}"')
     assert_unique_values([
-        _.uri for _ in batch_definitions], 'duplicate batch uri {x}')
+        _.uri for _ in batch_definitions], 'batch uri "{x}"')
     return {'batch_definitions': batch_definitions}
 
 
 def validate_environment(configuration):
     d = get_dictionary(configuration, 'environment')
     package_ids_by_manager_name = get_package_ids_by_manager_name(
         get_dictionaries(d, 'packages'))
@@ -504,15 +523,15 @@
         d, configuration.get_variable_definitions('log')
         + configuration.get_variable_definitions('debug'))
     environment_variable_ids = get_environment_variable_ids(get_dictionaries(
         d, 'variables'))
     batch_concurrency_name = d.get('batch', 'thread').lower()
     if batch_concurrency_name not in ('process', 'thread', 'single'):
         raise CrossComputeConfigurationError(
-            f'"{batch_concurrency_name}" batch concurrency is not supported')
+            f'batch concurrency "{batch_concurrency_name}" is not supported')
     interval_timedelta, is_interval_strict = get_interval_pack(d.get(
         'interval', '').strip())
     return {
         'engine_name': get_engine_name(d),
         'parent_image_name': d.get('image', 'python').strip(),
         'package_ids_by_manager_name': package_ids_by_manager_name,
         'port_definitions': port_definitions,
@@ -549,15 +568,15 @@
         style_definition = StyleDefinition(raw_style_definition)
         style_uri = style_definition.uri
         if '//' not in style_uri:
             style_path = style_definition.path
             path = automation_folder / style_path
             if not path.exists():
                 raise CrossComputeConfigurationError(
-                    f'{path} not found for style')
+                    f'style path "{path}" was not found')
             style_name = format_slug(
                 f'{splitext(style_path)[0]}-{reference_time}')
             style_uri = STYLE_ROUTE.format(style_name=style_name)
             if automation_index > 0:
                 style_uri = automation_uri + style_uri
             style_definition.path = style_path
             style_definition.uri = style_uri
@@ -621,61 +640,68 @@
         'group_definitions': group_definitions}
 
 
 def validate_template_identifiers(template_dictionary):
     try:
         template_path = template_dictionary['path']
     except KeyError as e:
-        raise CrossComputeConfigurationError(f'{e} required for each template')
+        raise CrossComputeConfigurationError(
+            f'{e} is required for each template')
     automation_folder = template_dictionary.automation_folder
     template_path = Path(template_path)
     if not (automation_folder / template_path).exists():
         raise CrossComputeConfigurationError(
-            f'could not find template {template_path}')
+            f'template path "{template_path}" was not found')
     return {
         'path': template_path,
         'expression': template_dictionary.get('expression', '')}
 
 
 def validate_variable_identifiers(variable_dictionary):
     try:
         variable_id = variable_dictionary['id']
         view_name = variable_dictionary['view']
         variable_path = variable_dictionary['path']
     except KeyError as e:
-        raise CrossComputeConfigurationError(f'{e} required for each variable')
+        raise CrossComputeConfigurationError(
+            f'{e} is required for each variable')
     if not VARIABLE_ID_PATTERN.match(variable_id):
         raise CrossComputeConfigurationError(
             f'{variable_id} is not a valid variable id; please use only '
             'lowercase, uppercase, numbers, hyphens, underscores and spaces')
     if variable_dictionary.step_name == 'print':
         if view_name in ['link']:
             pass
         elif view_name not in PRINTER_NAMES:
             raise CrossComputeConfigurationError(
-                f'{view_name} is not a supported printer')
+                f'printer "{view_name}" is not supported')
         elif view_name not in printer_by_name:
             raise CrossComputeConfigurationError(
                 f'pip install crosscompute-printers-{view_name}')
     if relpath(variable_path).startswith('..'):
         raise CrossComputeConfigurationError(
-            f'path {variable_path} for variable {variable_id} must be within '
-            'the folder')
+            f'variable "{variable_id}" path "{variable_path}" must be within '
+            'the automation folder')
     label = variable_dictionary.get('label', format_name(variable_id)).strip()
     return {
         'id': variable_id,
         'view_name': view_name,
         'path': Path(variable_path),
         'label': label}
 
 
 def validate_variable_configuration(variable_dictionary):
     # TODO: Validate variable view configurations
     c = get_dictionary(
         variable_dictionary, 'configuration')
+    if 'path' in c:
+        p = c['path']
+        if not p.endswith('.json'):
+            raise CrossComputeConfigurationError(
+                f'variable configuration path "{p}" suffix must be ".json"')
     if variable_dictionary.step_name == 'print':
         variable_id = variable_dictionary.id
         view_name = variable_dictionary.view_name
         if view_name == 'link':
             pass
         else:
             process_header_footer_options(variable_id, c)
@@ -684,15 +710,16 @@
 
 
 def validate_batch_identifiers(batch_dictionary):
     is_run = batch_dictionary.is_run
     try:
         folder = get_scalar_text(batch_dictionary, 'folder')
     except KeyError as e:
-        raise CrossComputeConfigurationError(f'{e} required for each batch')
+        raise CrossComputeConfigurationError(
+            f'{e} is required for each batch')
     name = get_scalar_text(batch_dictionary, 'name', basename(folder))
     slug = get_scalar_text(batch_dictionary, 'slug', name)
     data_by_id = batch_dictionary.data_by_id
     if data_by_id and not is_run:
         try:
             folder = format_text(folder, data_by_id)
             name = format_text(name, data_by_id)
@@ -731,25 +758,25 @@
     dataset_reference = get_dictionary(dataset_dictionary, 'reference')
     reference_path = get_folder_plus_path(dataset_reference)
     if reference_path:
         source_path = automation_folder / reference_path
         if not source_path.exists():
             if source_path.is_symlink():
                 raise CrossComputeConfigurationError(
-                    f'invalid symlink for dataset reference {reference_path}')
+                    f'dataset reference link "{reference_path}" is invalid')
             elif source_path.name == 'runs':
                 source_path.mkdir(parents=True)
             else:
                 raise CrossComputeConfigurationError(
-                    f'could not find dataset reference {reference_path}')
+                    f'dataset reference path "{reference_path}" was not found')
         target_path = dataset_dictionary.path
         if target_path.exists() and not target_path.is_symlink():
             raise CrossComputeConfigurationError(
-                'refusing to overwrite existing dataset; please delete '
-                f'{target_path} from the disk as defined')
+                'dataset path conflicts with existing dataset; please delete '
+                f'"{target_path}" from the disk to continue')
     return {'reference': dataset_reference}
 
 
 def validate_script_identifiers(script_dictionary):
     folder = script_dictionary.get('folder', '.').strip()
     method_count = 0
 
@@ -760,190 +787,192 @@
         command = None
 
     if 'path' in script_dictionary:
         path = Path(script_dictionary['path'].strip())
         suffix = path.suffix
         if suffix not in ['.ipynb', '.py']:
             raise CrossComputeConfigurationError(
-                f'{suffix} not supported for script path')
+                f'script path suffix "{suffix}" is not supported')
         method_count += 1
     else:
         path = None
 
     if 'function' in script_dictionary:
         method_count += 1
 
     if method_count > 1:
         raise CrossComputeConfigurationError(
-            'set script command or path or function')
+            'script command or path or function is required')
     return {'folder': Path(folder), 'command': command, 'path': path}
 
 
 def validate_package_identifiers(package_dictionary):
     try:
         package_id = package_dictionary['id']
         manager_name = package_dictionary['manager']
     except KeyError as e:
-        raise CrossComputeConfigurationError(f'{e} required for each package')
+        raise CrossComputeConfigurationError(
+            f'{e} is required for each package')
     if manager_name not in PACKAGE_MANAGER_NAMES:
         raise CrossComputeConfigurationError(
-            f'"{manager_name}" manager is not supported')
-    return {
-        'id': package_id,
-        'manager_name': manager_name}
+            f'manager "{manager_name}" is not supported')
+    return {'id': package_id, 'manager_name': manager_name}
 
 
 def validate_port_identifiers(port_dictionary):
     try:
         port_id = port_dictionary['id']
         port_number = port_dictionary['number']
     except KeyError as e:
-        raise CrossComputeConfigurationError(f'{e} required for each port')
+        raise CrossComputeConfigurationError(
+            f'{e} is required for each port')
     try:
         port_number = int(port_number)
     except ValueError:
         raise CrossComputeConfigurationError(
-            f'{port_number} must be an integer')
+            f'port number "{port_number}" must be an integer')
     return {
         'id': port_id,
         'number': port_number}
 
 
 def validate_style_identifiers(style_dictionary):
     uri = style_dictionary.get('uri', '').strip()
     path = style_dictionary.get('path', '').strip()
     if not uri and not path:
-        raise CrossComputeConfigurationError(
-            'uri or path required for each style')
+        raise CrossComputeConfigurationError('style uri or path is required')
     return {'uri': uri, 'path': Path(path)}
 
 
 def validate_page_identifiers(page_dictionary):
     try:
         page_id = page_dictionary['id']
     except KeyError as e:
-        raise CrossComputeConfigurationError(f'{e} required for each page')
+        raise CrossComputeConfigurationError(
+            f'{e} is required for each page')
     if page_id not in DESIGN_NAMES_BY_PAGE_ID:
         raise CrossComputeConfigurationError(
-            f'{page_id} page not supported for page configuration')
+            f'page "{page_id}" is not supported')
     return {'id': page_id}
 
 
 def validate_page_configuration(page_dictionary):
     page_configuration = get_dictionary(page_dictionary, 'configuration')
     page_id = page_dictionary['id']
     design_name = page_configuration.get('design')
     design_names = DESIGN_NAMES_BY_PAGE_ID[page_id]
     if design_name not in design_names:
         raise CrossComputeConfigurationError(
-            f'"{design_name}" design not supported for {page_id} page')
+            f'design "{design_name}" is not supported for page "{page_id}"')
     return {'configuration': page_configuration}
 
 
 def validate_button_identifiers(button_dictionary):
     try:
         button_id = button_dictionary['id']
     except KeyError as e:
-        raise CrossComputeConfigurationError(f'{e} required for each button')
+        raise CrossComputeConfigurationError(
+            f'{e} is required for each button')
     if button_id not in BUTTON_TEXT_BY_ID:
         raise CrossComputeConfigurationError(
-            f'{button_id} button not supported for button configuration')
+            f'button id "{button_id}" is not supported')
     return {'id': button_id}
 
 
 def validate_button_configuration(button_dictionary):
     button_configuration = get_dictionary(button_dictionary, 'configuration')
     return {'configuration': button_configuration}
 
 
 def validate_token_identifiers(token_dictionary):
     try:
         token_path = token_dictionary['path']
     except KeyError as e:
-        raise CrossComputeConfigurationError(f'{e} required for each token')
+        raise CrossComputeConfigurationError(f'{e} is required for each token')
     path = Path(token_dictionary.automation_folder, token_path)
     suffix = path.suffix
     if suffix == '.yml':
         d = load_raw_configuration_yaml(path)
     else:
         raise CrossComputeConfigurationError(
-            f'{suffix} not supported for token paths')
+            f'token path suffix "{suffix}" is not supported')
     identities_by_token = {}
     for token, identities in d.items():
         token = str(token)
         variable_match = VARIABLE_ID_TEMPLATE_PATTERN.match(token)
         if variable_match:
             variable_id = variable_match.group(1)
             try:
                 token = environ[variable_id]
             except KeyError:
                 e = CrossComputeConfigurationError(
-                    f'{variable_id} is missing in the environment')
+                    f'environment variable "{variable_id}" is missing')
                 e.path = path
                 raise e
         identities_by_token[token] = identities
     return {'identities_by_token': identities_by_token}
 
 
 def validate_group_identifiers(group_dictionary):
     try:
         group_configuration = group_dictionary['configuration']
     except KeyError as e:
-        raise CrossComputeConfigurationError(f'{e} required for each group')
+        raise CrossComputeConfigurationError(f'{e} is required for each group')
     group_permissions = [PermissionDefinition(_) for _ in get_dictionaries(
         group_dictionary, 'permissions')]
     return {
         'configuration': group_configuration or {},
         'permissions': group_permissions}
 
 
 def validate_permission_identifiers(permission_dictionary):
     try:
         permission_id = permission_dictionary['id']
     except KeyError as e:
         raise CrossComputeConfigurationError(
-            f'{e} required for each permission')
+            f'{e} is required for each permission')
     if permission_id not in PERMISSION_IDS:
         raise CrossComputeConfigurationError(
-            f'"{permission_id}" permission not supported')
+            f'permission id "{permission_id}" is not supported')
     permission_action = permission_dictionary.get('action', 'accept')
     if permission_action not in PERMISSION_ACTIONS:
         raise CrossComputeConfigurationError(
-            f'"{permission_action}" action not supported')
+            f'permission action "{permission_action}" is not supported')
     return {'id': permission_id, 'action': permission_action}
 
 
 def get_configuration_format(path):
-    file_extension = path.suffix
+    suffix = path.suffix
     try:
         configuration_format = {
             '.cfg': 'ini',
             '.ini': 'ini',
             '.toml': 'toml',
             '.yaml': 'yaml',
             '.yml': 'yaml',
-        }[file_extension]
+        }[suffix]
     except KeyError:
         raise CrossComputeConfigurationFormatError((
-            f'{file_extension} format not supported for automation '
-            'configuration').lstrip())
+            f'automation configuration suffix "{suffix}" '
+            'is not supported'
+        ).lstrip())
     return configuration_format
 
 
 def get_engine_name(environment_dictionary):
     engine_name = environment_dictionary.get('engine', 'unsafe').strip()
     if engine_name == 'podman':
         if not shutil.which('podman'):
             L.warning('podman is not available on this machine')
     elif engine_name == 'unsafe':
         L.warning(
             'using engine=unsafe; use engine=podman for untrusted code')
     else:
         raise CrossComputeConfigurationError(
-            f'"{engine_name}" engine is not supported')
+            f'engine "{engine_name}" is not supported')
     return engine_name
 
 
 def get_package_ids_by_manager_name(package_dictionaries):
     package_ids_by_manager_name = defaultdict(set)
     package_definitions = [PackageDefinition(_) for _ in package_dictionaries]
     for package_definition in package_definitions:
@@ -958,69 +987,69 @@
     for port_definition in port_definitions:
         port_id = port_definition.id
         try:
             variable_definition = find_item(
                 variable_definitions, 'id', port_id)
         except StopIteration:
             raise CrossComputeConfigurationError(
-                f'{port_id} port must have a matching variable definition')
+                f'port "{port_id}" must have a matching variable definition')
         step_name = variable_definition.step_name
         if step_name not in ['log', 'debug']:
             raise CrossComputeConfigurationError(
-                f'{port_id} port must correspond to a log or debug variable')
+                f'port "{port_id}" must correspond to a log or debug variable')
         port_definition.step_name = step_name
     return port_definitions
 
 
 def get_environment_variable_ids(environment_variable_definitions):
     variable_ids = set()
     for environment_variable_definition in environment_variable_definitions:
         try:
             variable_id = environment_variable_definition['id']
         except KeyError as e:
             raise CrossComputeConfigurationError(
-                f'{e} required for each environment variable')
+                f'{e} is required for each environment variable')
         try:
             environ[variable_id]
         except KeyError:
             raise CrossComputeConfigurationError(
-                f'{variable_id} is missing in the environment as defined')
+                f'environment variable "{variable_id}" is missing')
         variable_ids.add(variable_id)
     return variable_ids
 
 
 def get_interval_pack(interval_text):
     if not interval_text:
         return None, None
     try:
         count, name = interval_text.split(maxsplit=1)
         count = int(count)
     except ValueError:
         raise CrossComputeConfigurationError(
-            f'unparseable interval "{interval_text}"; '
-            f'expected something like "30 minutes"')
+            f'interval "{interval_text}" is not parsable; '
+            f'something like "30 minutes" was expected')
     for unit_name in INTERVAL_UNIT_NAMES:
         if name.startswith(unit_name[:-1]):
             break
     else:
-        unit_names_text = ' '.join(INTERVAL_UNIT_NAMES)
+        unit_names_text = ' or '.join(INTERVAL_UNIT_NAMES)
         raise CrossComputeConfigurationError(
-            f'unsupported interval unit "{name}" in "{interval_text}"; '
-            f'expected {unit_names_text}')
+            f'interval "{interval_text}" unit "{name}" is not supported; '
+            f'{unit_names_text} was expected')
     is_strict = True if '!' in name else False
     return timedelta(**{unit_name: count}), is_strict
 
 
 def get_scalar_text(d, key, default=None):
     value = d.get(key) or default
     if value is None:
         raise KeyError(key)
     if isinstance(value, dict):
         raise CrossComputeConfigurationError(
-            f'surround {key} with quotes since it begins with a {{')
+            f'"{key}" must be surrounded with quotes when it begins with a {{')
     return value
 
 
 def get_batch_definitions(
         raw_batch_definition, automation_folder, variable_definitions):
     batch_definitions = []
     raw_batch_definition = BatchDefinition(raw_batch_definition)
@@ -1033,21 +1062,21 @@
             automation_folder / reference_folder / 'input',
             variable_definitions)
     else:
         reference_data_by_id = {}
 
     if 'path' in batch_configuration:
         batch_configuration_path = Path(batch_configuration['path'])
-        file_extension = batch_configuration_path.suffix
+        suffix = batch_configuration_path.suffix
         try:
-            yield_data_by_id = YIELD_DATA_BY_ID_BY_EXTENSION[file_extension]
+            yield_data_by_id = YIELD_DATA_BY_ID_BY_EXTENSION[suffix]
         except KeyError:
             raise CrossComputeConfigurationError((
-                f'{file_extension} format not supported for batch '
-                'configuration').lstrip())
+                f'batch configuration suffix "{suffix}" is not supported'
+            ).lstrip())
         for configuration_data_by_id in yield_data_by_id(
                 automation_folder / batch_configuration_path,
                 variable_definitions):
             data_by_id = reference_data_by_id | configuration_data_by_id
             batch_definitions.append(BatchDefinition(
                 raw_batch_definition, data_by_id=data_by_id))
     else:
@@ -1069,57 +1098,61 @@
 
 def process_page_number_options(variable_id, print_configuration):
     k = 'page-number'
     d = get_dictionary(print_configuration, k)
     location = d.get('location')
     if location and location not in ['header', 'footer']:
         raise CrossComputeConfigurationError(
-            f'print variable {variable_id} configuration {k} '
-            f'location {location} not supported')
+            f'print variable "{variable_id}" configuration "{k}" '
+            f'location "{location}" is not supported')
     alignment = d.get('alignment')
     if alignment and alignment not in ['left', 'center', 'right']:
         raise CrossComputeConfigurationError(
-            f'print variable {variable_id} configuration {k} '
-            f'alignment {alignment} not supported')
+            f'print variable "{variable_id}" configuration "{k}" '
+            f'alignment "{alignment}" is not supported')
 
 
 def get_folder_plus_path(d):
     folder = d.get('folder', '').strip()
     path = d.get('path', '').strip()
     if not folder and not path:
         return
     return Path(folder, path)
 
 
 def get_dictionaries(d, key):
     values = get_list(d, key)
     for value in values:
         if not isinstance(value, dict):
-            raise CrossComputeConfigurationError(f'{key} must be dictionaries')
+            raise CrossComputeConfigurationError(
+                f'"{key}" must be dictionaries')
     return values
 
 
 def get_dictionary(d, key):
     value = d.get(key, {})
     if not isinstance(value, dict):
-        raise CrossComputeConfigurationError(f'{key} must be a dictionary')
+        raise CrossComputeConfigurationError(
+            f'"{key}" must be a dictionary')
     return value
 
 
 def get_list(d, key):
     value = d.get(key, [])
     if not isinstance(value, list):
-        raise CrossComputeConfigurationError(f'{key} must be a list')
+        raise CrossComputeConfigurationError(
+            f'"{key}" must be a list')
     return value
 
 
 def assert_unique_values(xs, message):
     for x, count in Counter(xs).items():
         if count > 1:
-            raise CrossComputeConfigurationError(message.format(x=x))
+            raise CrossComputeConfigurationError(
+                message.format(x=x) + ' is not unique')
 
 
 RUN_PY = Template('''\
 from inspect import signature
 from os import getenv
 from pathlib import Path
 
@@ -1139,16 +1172,14 @@
 
 
 PERMISSION_IDS = [
     'add_token',
     'see_root',
     'see_automation',
     'see_batch',
-    'run_automation',
-]
+    'run_automation']
 PERMISSION_ACTIONS = [
     'accept',
-    'match',
-]
+    'match']
 
 
 L = getLogger(__name__)
```

### Comparing `crosscompute-0.9.4.4/crosscompute/routines/database.py` & `crosscompute-0.9.4.8/crosscompute/routines/database.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 import shlex
+from copy import deepcopy
 from logging import getLogger
 from os.path import isfile
 from pathlib import Path
 from time import time
 
 from invisibleroads_macros_disk import is_path_in_folder
 from watchfiles import Change, DefaultFilter
 
 from ..constants import (
     Info,
     BATCH_ROUTE,
+    MAXIMUM_FILE_CACHE_LENGTH,
     STEP_CODE_BY_NAME,
     STEP_ROUTE)
+from ..exceptions import CrossComputeDataError
+from ..macros.disk import FileCache
 from .configuration import (
     get_folder_plus_path)
+from .variable import (
+    load_file_json,
+    load_variable_data)
 
 
 class DiskDatabase():
 
     def __init__(self, configuration, changes, with_restart):
         self._configuration = configuration
         self._changes = changes
         self._memory = learn(configuration, with_restart)
 
     def grok(self, paths):
         changed_infos = []
-        variable_ids = []
         for path in paths:
             try:
                 infos = self.get(path)
             except KeyError:
                 continue
-            for info in infos:
-                if info['code'] == Info.VARIABLE:
-                    variable_id = info['id']
-                    if info['id'] in variable_ids:
-                        continue
-                    variable_ids.append(variable_id)
-                changed_infos.append(info)
+            changed_infos.extend(infos)
         if changed_infos:
             self._changes[time()] = changed_infos
         L.debug(changed_infos)
         return changed_infos
 
     def get(self, path):
         path = Path(path)
@@ -74,24 +74,43 @@
     def add(self, path, info):
         path = Path(path).absolute()
         if not path.exists() or path.is_file():
             d = self._infos_by_path
         elif path.is_dir() and info['code'] == Info.DATASET:
             d = self._infos_by_folder
         else:
-            L.warning(f'{path} must be a file')
+            L.warning('path "%s" must be a file', path)
             return
         if path not in d:
             d[path] = []
         d[path].append(info)
 
     def get(self, path):
         path = Path(path).absolute()
-        if path in self._infos_by_path:
-            return self._infos_by_path[path]
+        infos_by_path = self._infos_by_path
+        if path in infos_by_path:
+            infos = deepcopy(infos_by_path[path])
+            for info in infos:
+                if info['code'] != Info.VARIABLE or info['step'] == 'i':
+                    continue
+                if info.get('is_configuration'):
+                    try:
+                        info['configuration'] = FILE_JSON_CACHE[path]
+                    except OSError:
+                        pass
+                elif info['view'] in [
+                    'string', 'number', 'password', 'email', 'text',
+                    'markdown', 'radio', 'checkbox', 'frame',
+                ]:
+                    try:
+                        info['value'] = load_variable_data(
+                            path, info['id'])['value']
+                    except (CrossComputeDataError, KeyError):
+                        pass
+            return infos
         for folder, infos in self._infos_by_folder.items():
             if folder in path.parents:
                 return infos
         raise KeyError
 
 
 class PositiveFileFilter(DefaultFilter):
@@ -102,23 +121,23 @@
         return is_positive and is_file and super().__call__(change, path)
 
 
 def learn(configuration, with_restart):
     memory = DiskMemory()
     add_variable_infos(memory, configuration)
     if with_restart:
-        add_code_infos(memory, configuration)
+        add_configuration_infos(memory, configuration)
         add_script_infos(memory, configuration)
         add_dataset_infos(memory, configuration)
         add_template_infos(memory, configuration)
         add_style_infos(memory, configuration)
     return memory
 
 
-def add_code_infos(memory, configuration):
+def add_configuration_infos(memory, configuration):
     info = {'code': Info.CONFIGURATION}
     # Get automation configuration paths
     memory.add(configuration.path, info)
     for import_configuration in configuration.import_configurations:
         memory.add(import_configuration['path'], info)
     # Get batch configuration paths
     for automation_definition in configuration.automation_definitions:
@@ -189,26 +208,27 @@
     d = automation_definition.variable_definitions_by_step_name
     for step_name, variable_definitions in d.items():
         step_code = STEP_CODE_BY_NAME[step_name]
         step_uri = STEP_ROUTE.format(step_code=step_code)
         folder = absolute_batch_folder / step_name
         for variable_definition in variable_definitions:
             variable_id = variable_definition.id
+            variable_view = variable_definition.view_name
             if variable_id != 'return_code':
                 info_uri = uri + step_uri
             else:
                 info_uri = uri
             variable_info = info | {
                 'id': variable_id, 'uri': info_uri, 'step': step_code}
             variable_configuration = variable_definition.configuration
             if 'path' in variable_configuration:
                 path = folder / variable_configuration['path']
-                memory.add(path, variable_info)
+                memory.add(path, variable_info | {'is_configuration': 1})
             path = folder / variable_definition.path
-            memory.add(path, variable_info)
+            memory.add(path, variable_info | {'view': variable_view})
 
 
 def add_template_infos(memory, configuration):
     info = {'code': Info.TEMPLATE}
     for automation_definition in configuration.automation_definitions:
         automation_folder = automation_definition.folder
         automation_uri = automation_definition.uri
@@ -235,8 +255,11 @@
         for style_definition in automation_definition.style_definitions:
             if 'path' not in style_definition:
                 continue
             path = automation_folder / style_definition['path']
             memory.add(path, info)
 
 
+FILE_JSON_CACHE = FileCache(
+    load_file_data=load_file_json,
+    maximum_length=MAXIMUM_FILE_CACHE_LENGTH)
 L = getLogger(__name__)
```

### Comparing `crosscompute-0.9.4.4/crosscompute/routines/log.py` & `crosscompute-0.9.4.8/crosscompute/routines/log.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 from logging import (
-    basicConfig, getLogger, CRITICAL, DEBUG, ERROR, INFO, WARNING)
+    basicConfig,
+    getLogger,
+    CRITICAL,
+    DEBUG,
+    ERROR,
+    INFO,
+    WARNING)
 
 
 def configure_argument_parser_for_logging(argument_parser):
     argument_parser.add_argument(
         '--quiet', '-q', dest='quietness', action='count', default=0,
         help='decrease logging level; stack as -qq')
     argument_parser.add_argument(
```

### Comparing `crosscompute-0.9.4.4/crosscompute/routines/mutation.py` & `crosscompute-0.9.4.8/crosscompute/routines/mutation.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,37 +6,74 @@
 from ..settings import (
     template_globals)
 from .uri import (
     get_step_code)
 
 
 def get_mutation(file_changes, reference_uri, old_time):
-    configurations, variables, templates, styles = [], [], [], []
-    new_time = time()
-    step_code = get_step_code(reference_uri)
+    variable_by_id, configurations, templates, styles = {}, [], [], []
+    new_time, step_code = time(), get_step_code(reference_uri)
     for t, infos in file_changes.copy().items():
         if new_time - t > MAXIMUM_MUTATION_AGE_IN_SECONDS:
             try:
                 del file_changes[t]
             except KeyError:
                 pass
         if t <= old_time:
             continue
         for info in infos:
-            code = info['code']
-            if code == Info.CONFIGURATION:
-                configurations.append({})
-            elif code == Info.VARIABLE and info['step'] != 'i':
-                if reference_uri.startswith(info['uri']):
-                    # TODO: Send value if authorized
-                    variables.append({'id': info['id']})
-            elif code == Info.TEMPLATE:
-                if 'step' in info and info['step'] != step_code:
-                    continue
-                if reference_uri.startswith(info['uri']):
-                    templates.append({})
-            elif code == Info.STYLE:
-                styles.append({})
-    return {
-        'configurations': configurations, 'variables': variables,
-        'templates': templates, 'styles': styles, 'mutation_time': new_time,
+            categorize_mutation(
+                info, reference_uri, step_code, variable_by_id,
+                configurations, templates, styles)
+    d = {
+        'mutation_time': new_time,
         'server_time': template_globals['server_time']}
+    if configurations:
+        d['configurations'] = configurations
+    if variable_by_id:
+        d['variables'] = list(variable_by_id.values())
+    if templates:
+        d['templates'] = templates
+    if styles:
+        d['styles'] = styles
+    return d
+
+
+def categorize_mutation(
+        info, reference_uri, step_code, variable_by_id,
+        configurations, templates, styles):
+    match info['code']:
+        case Info.CONFIGURATION:
+            configurations.append({})
+        case Info.VARIABLE:
+            if is_irrelevant_variable(info, reference_uri):
+                return
+            variable_id = info['id']
+            d = {'i': variable_id}
+            if 'value' in info:
+                d['v'] = info['value']
+            if 'configuration' in info:
+                d['c'] = info['configuration']
+            variable_by_id[variable_id] = variable_by_id.get(
+                variable_id, {}) | d
+        case Info.TEMPLATE:
+            if is_irrelevant_template(info, step_code, reference_uri):
+                return
+            templates.append({})
+        case Info.STYLE:
+            styles.append({})
+
+
+def is_irrelevant_variable(info, reference_uri):
+    if info['step'] == 'i':
+        return True
+    if not reference_uri.startswith(info['uri']):
+        return True
+    return False
+
+
+def is_irrelevant_template(info, step_code, reference_uri):
+    if info.get('step') != step_code:
+        return True
+    if not reference_uri.startswith(info['uri']):
+        return True
+    return False
```

### Comparing `crosscompute-0.9.4.4/crosscompute/routines/printer.py` & `crosscompute-0.9.4.8/crosscompute/routines/printer.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,25 +49,20 @@
             view_name,
             print_configurations,
         ) in print_configurations_by_view_name.items():
             packs_by_view_name[view_name].append((
                 batch_dictionaries, print_configurations))
 
     def run(self):
-        is_draft = self.is_draft
-        if is_draft:
-            for draft_path in self._pack_by_path:
-                if draft_path.is_symlink():
-                    remove_path(draft_path)
+        self._save_link_configurations()
         for view_name, packs in self._packs_by_view_name.items():
             Printer = printer_by_name[view_name]
-            printer = Printer(self.server_uri, is_draft)
+            printer = Printer(self.server_uri, self.is_draft)
             for batch_dictionaries, print_configurations in packs:
                 printer.render(batch_dictionaries, print_configurations)
-        self._save_link_configurations()
         self.reset()
 
     def _get_batch_dictionaries(
             self, automation_definition, batch_definitions):
         batch_dictionaries = []
         automation_folder = automation_definition.folder
         automation_uri = automation_definition.uri
@@ -95,15 +90,19 @@
                     pack_by_path[draft_path] = print_folder, print_name
                 elif view_name == 'link':
                     link_packs.append((draft_folder, print_definition))
         return batch_dictionaries
 
     def _save_link_configurations(self):
         pack_by_path = self._pack_by_path
-        if not self.is_draft:
+        if self.is_draft:
+            for draft_path in pack_by_path:
+                if draft_path.is_symlink():
+                    remove_path(draft_path)
+        else:
             for draft_path, (
                 print_folder, print_name,
             ) in pack_by_path.items():
                 symlink(print_folder / print_name, remove_path(draft_path))
         for (
             draft_folder, variable_definition,
         ) in self._link_packs:
```

### Comparing `crosscompute-0.9.4.4/crosscompute/routines/server.py` & `crosscompute-0.9.4.8/crosscompute/routines/server.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.4/crosscompute/routines/step.py` & `crosscompute-0.9.4.8/crosscompute/routines/step.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,61 @@
 from functools import partial
 from html.parser import HTMLParser
 from itertools import count
 from logging import getLogger
 
-from invisibleroads_macros_web.markdown import get_html_from_markdown
+from invisibleroads_macros_web.markdown import (
+    get_html_from_markdown,
+    remove_parent_paragraphs)
 
 from ..constants import (
     BUTTON_TEXT_BY_ID,
     MUTATION_ROUTE,
     STEP_CODE_BY_NAME,
     STEP_ROUTE,
     VARIABLE_ID_TEMPLATE_PATTERN,
     VARIABLE_ID_WHITELIST_PATTERN)
-from ..macros.iterable import find_item, get_unique_order
-from ..settings import template_globals
+from ..macros.iterable import find_item
 from .asset import asset_storage
 from .batch import DiskBatch
+from .configuration import AutomationDefinition
 from .variable import Element, VariableView
 
 
 class TemplateFilter(HTMLParser):
 
-    def __init__(self, render_html, template_index, *args, **kwargs):
+    def __init__(self, root_uri, render_html, template_index, *args, **kwargs):
+        self.render_text = partial(render_text, root_uri=root_uri)
         self.render_html = partial(render_html, template_index=template_index)
         self.in_script = False
         self.template_parts = []
         super().__init__(*args, **kwargs)
 
     def handle_starttag(self, tag, attrs):
         if tag == 'script':
             self.in_script = True
-        attribute_strings = [f'{k}="{v}"' for k, v in attrs]
+        attribute_strings = []
+        for k, v in attrs:
+            v = VARIABLE_ID_WHITELIST_PATTERN.sub(self.render_text, v)
+            attribute_strings.append(f'{k}="{v}"')
         attributes_string = ' ' + ' '.join(
             attribute_strings) if attribute_strings else ''
         self.template_parts.append(f'<{tag}{attributes_string}>')
 
     def handle_endtag(self, tag):
         if tag == 'script':
             self.in_script = False
         self.template_parts.append(f'</{tag}>')
 
     def handle_data(self, data):
         in_script = self.in_script
-        render_html = self.render_html
         if in_script:
-            data = VARIABLE_ID_WHITELIST_PATTERN.sub(render_html, data)
+            data = VARIABLE_ID_WHITELIST_PATTERN.sub(self.render_text, data)
         else:
-            data = VARIABLE_ID_TEMPLATE_PATTERN.sub(render_html, data)
+            data = VARIABLE_ID_TEMPLATE_PATTERN.sub(self.render_html, data)
         self.template_parts.append(data)
 
     def process(self, text):
         self.template_parts = []
         self.feed(text)
         return ''.join(self.template_parts)
 
@@ -60,127 +65,202 @@
     automation_uri = automation_definition.uri
     batch_uri = batch_definition.uri
     step_code = STEP_CODE_BY_NAME[step_name]
     step_uri = STEP_ROUTE.format(step_code=step_code)
     return automation_uri + batch_uri + step_uri
 
 
+def get_automation_response_dictionary(
+        automation_definition, root_uri, request_params):
+    automation_uri = automation_definition.uri
+    step_name = automation_definition.get_design_name('automation')
+    if step_name == 'none':
+        layout_settings = get_layout_settings(step_name, request_params)
+        d = {
+            'css_uris': automation_definition.css_uris,
+            'css_texts': get_css_texts(layout_settings),
+            'is_done': 1,
+            'mutation_uri': MUTATION_ROUTE.format(uri=automation_uri)}
+    else:
+        layout_settings = get_layout_settings(
+            automation_definition.get_design_name(step_name), request_params)
+        d = get_step_response_dictionary(
+            automation_definition, automation_definition.batch_definitions[0],
+            step_name, root_uri, layout_settings, request_params)
+    return {
+        'copyright_name': automation_definition.copyright_name,
+        'copyright_uri': automation_definition.copyright_uri,
+        'attribution_text': automation_definition.attribution_text,
+        'name': automation_definition.name,
+        'uri': automation_uri,
+        'step_name': step_name,
+    } | d
+
+
 def get_step_response_dictionary(
-        automation_definition, batch_definition, step_name, request_params):
+        automation_definition, batch_definition, step_name, root_uri,
+        layout_settings, request_params):
     variable_definitions = automation_definition.get_variable_definitions(
         step_name, with_all=True)
     batch = DiskBatch(automation_definition, batch_definition)
     m = {
         'css_uris': automation_definition.css_uris.copy(), 'css_texts': [],
         'js_uris': [], 'js_texts': []}
-    design_name = automation_definition.get_design_name(step_name)
-    for_embed = '_embed' in request_params
-    for_print = '_print' in request_params
     render_html = partial(
-        render_variable_html, variable_definitions=variable_definitions,
-        batch=batch, m=m, variable_index=count(),
-        root_uri=template_globals['root_uri'], request_params=request_params,
+        render_variable_html, batch=batch, step_name=step_name,
+        variable_definitions=variable_definitions, variable_index=count(),
         button_text_by_id=automation_definition.button_text_by_id,
-        step_name=step_name, design_name=design_name, for_print=for_print)
+        root_uri=root_uri, layout_settings=layout_settings,
+        request_params=request_params, m=m)
     main_text, template_count = get_main_pack(
-        automation_definition, step_name, render_html)
+        automation_definition, step_name, root_uri, render_html,
+        layout_settings)
     mutation_reference_uri = get_automation_batch_step_uri(
         automation_definition, batch_definition, step_name)
-    return {
-        'css_uris': get_unique_order(m['css_uris']),
-        'css_text': get_css_text(design_name, for_embed, for_print, m),
+    return layout_settings | {
+        'css_uris': m['css_uris'],
+        'css_texts': get_css_texts(layout_settings) + m['css_texts'],
+        'js_uris': m['js_uris'],
+        'js_texts': m['js_texts'],
         'main_text': main_text, 'template_count': template_count,
-        'js_uris': get_unique_order(m['js_uris']),
-        'js_text': '\n'.join(get_unique_order(m['js_texts'])),
-        'for_embed': for_embed, 'for_print': for_print,
-        'has_interval': automation_definition.interval_timedelta is not None,
         'is_done': batch.is_done(),
+        'has_interval': automation_definition.interval_timedelta is not None,
         'mutation_uri': MUTATION_ROUTE.format(uri=mutation_reference_uri)}
 
 
+def render_text(match, root_uri):
+    matching_inner_text = match.group(1)
+    if matching_inner_text == 'ROOT_URI':
+        return root_uri
+    matching_outer_text = match.group(0)
+    return matching_outer_text
+
+
 def render_variable_html(
-        match, variable_definitions, batch, m, variable_index, template_index,
-        root_uri, request_params, button_text_by_id, step_name, design_name,
-        for_print):
+        match, batch, step_name, variable_definitions, variable_index,
+        template_index, button_text_by_id, root_uri, layout_settings,
+        request_params, m):
     matching_inner_text = match.group(1)
     if matching_inner_text == 'ROOT_URI':
         return root_uri
     elif matching_inner_text == 'BUTTON_PANEL':
         return get_button_panel_html(template_index, button_text_by_id)
     terms = matching_inner_text.split('|')
     variable_id = terms[0].strip()
     try:
         variable_definition = find_item(
             variable_definitions, 'id', variable_id)
     except StopIteration:
         L.warning(
-            '%s variable in template but not in configuration', variable_id)
+            'variable "%s" is in the template but is missing from the '
+            'configuration',
+            variable_id)
         matching_outer_text = match.group(0)
         return matching_outer_text
     view = VariableView.get_from(variable_definition)
     mode_name = variable_definition.get('mode', step_name)
     element = Element(
-        f'v{next(variable_index)}', request_params, mode_name, design_name,
-        for_print, terms[1:])
+        f'v{next(variable_index)}', mode_name, request_params,
+        layout_settings, terms[1:])
     page_dictionary = view.render(batch, element)
     for k, v in m.items():
         v.extend(_.strip() for _ in page_dictionary[k])
     return page_dictionary['main_text']
 
 
-def get_css_text(design_name, for_embed, for_print, m):
-    css_texts = []
-    if for_embed:
-        css_texts.append(EMBEDDED_CSS)
-    elif for_print:
-        css_texts.append(PRINTED_CSS)
-    else:
-        css_texts.append(DEFAULT_CSS)
-    if design_name == 'flex':
-        css_texts.append(FLEX_CSS)
-    return '\n'.join(css_texts + get_unique_order(m['css_texts']))
-
-
-def get_main_pack(automation_definition, step_name, render_html):
-    a = automation_definition
+def get_main_pack(
+        a: AutomationDefinition, step_name, root_uri, render_html,
+        layout_settings):
     template_definitions = a.template_definitions_by_step_name[step_name]
-    with_button_panel = step_name == 'input' or len(template_definitions) > 1
-    button_text_by_id = a.button_text_by_id
-
-    def format_template(text, i=0, x=''):
-        l_ = ' _live' if not i and not x else ''
-        x_ = f' data-expression="{x}"' if x else ''
-        g = TemplateFilter(render_html, template_index=i).process(text)
-        h = get_html_from_markdown(g)
-        if with_button_panel and 'class="_continue"' not in h:
-            h += '\n' + get_button_panel_html(i, button_text_by_id)
-        return f'<div id="_t{i}" class="_template{l_}"{x_}>\n{h}\n</div>'
-
-    if not template_definitions:
-        variable_definitions = a.get_variable_definitions(step_name)
-        variable_ids = (_.id for _ in variable_definitions)
-        text = '\n'.join('{%s}' % _ for _ in variable_ids)
-        return format_template(text), 1
+    template_count = len(template_definitions)
+    format_html = partial(
+        format_template_html,
+        root_uri=root_uri,
+        render_html=render_html,
+        with_button_panel=get_with_button_panel(
+            layout_settings, step_name, template_count),
+        button_text_by_id=a.button_text_by_id)
+    if not template_count:
+        template_text = make_template_text(a, step_name)
+        return format_html(
+            template_text, template_index=0, template_expression=''), 1
     parts = []
     automation_folder = a.folder
-    for i, template_definition in enumerate(template_definitions):
+    for template_index, template_definition in enumerate(template_definitions):
         path = automation_folder / template_definition.path
-        with path.open('rt') as f:
-            text = f.read().strip()
-        parts.append(format_template(text, i, template_definition.expression))
-    return '\n'.join(parts), len(template_definitions)
+        try:
+            with path.open('rt') as f:
+                text = f.read().strip()
+        except IOError:
+            L.error('template path "%s" was not found', path)
+            continue
+        parts.append(format_html(
+            text, template_index, template_definition.expression))
+    return '\n'.join(parts), template_count
 
 
 def get_button_panel_html(template_index, button_text_by_id):
     return BUTTON_PANEL_HTML.render({
         'template_index': template_index,
         'button_text_by_id': BUTTON_TEXT_BY_ID | button_text_by_id})
 
 
+def get_layout_settings(design_name, request_params):
+    return {
+        'design_name': design_name,
+        'for_embed': '_embed' in request_params,
+        'for_print': '_print' in request_params}
+
+
+def get_css_texts(layout_settings):
+    css_texts = []
+    if layout_settings['for_embed']:
+        css_texts.append(EMBEDDED_CSS)
+    else:
+        css_texts.append(DEFAULT_CSS)
+    if layout_settings['design_name'] == 'flex':
+        css_texts.append(FLEX_CSS)
+    return css_texts
+
+
+def get_with_button_panel(layout_settings, step_name, template_count):
+    if layout_settings['design_name'] == 'none':
+        return False
+    if layout_settings['for_print']:
+        return False
+    if step_name != 'input' and template_count <= 1:
+        return False
+    return True
+
+
+def make_template_text(automation_definition, step_name):
+    variable_definitions = automation_definition.get_variable_definitions(
+        step_name)
+    variable_ids = (_.id for _ in variable_definitions)
+    return ' '.join('{%s}' % _ for _ in variable_ids)
+
+
+def format_template_html(
+        text, template_index, template_expression, root_uri, render_html,
+        with_button_panel, button_text_by_id):
+    l_ = ' _live' if not template_index and not template_expression else ''
+    x_ = (
+        f' data-expression="{template_expression}"'
+        if template_expression else '')
+    h = get_html_from_markdown(text)
+    h = TemplateFilter(
+        root_uri, render_html, template_index=template_index).process(h)
+    h = remove_parent_paragraphs(h)
+    if with_button_panel and 'class="_continue"' not in h:
+        h += '\n' + get_button_panel_html(template_index, button_text_by_id)
+    return (
+        f'<div id="_t{template_index}" class="_template{l_}"{x_}>'
+        f'\n{h}\n</div>')
+
+
 L = getLogger(__name__)
 
 
 EMBEDDED_CSS = asset_storage.load_raw_text('embedded.css')
-PRINTED_CSS = asset_storage.load_raw_text('printed.css')
 DEFAULT_CSS = asset_storage.load_raw_text('default.css')
 FLEX_CSS = asset_storage.load_raw_text('flex.css')
 BUTTON_PANEL_HTML = asset_storage.load_jinja_text('button-panel.html')
```

### Comparing `crosscompute-0.9.4.4/crosscompute/routines/uri.py` & `crosscompute-0.9.4.8/crosscompute/routines/uri.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,10 +21,15 @@
 def get_step_code(uri):
     match = STEP_PATTERN.search(uri)
     if not match:
         return
     return match.group(1)
 
 
+def get_host_uri(request):
+    uri = request.url
+    return uri.scheme + '://' + uri.netloc
+
+
 AUTOMATION_PATTERN = re.compile(r'/a/([^/]+)')
 BATCH_PATTERN = re.compile(r'/b/([^/]+)')
 STEP_PATTERN = re.compile(r'/([%s])$' % ''.join(STEP_CODE_BY_NAME.keys()))
```

### Comparing `crosscompute-0.9.4.4/crosscompute/routines/variable.py` & `crosscompute-0.9.4.8/crosscompute/routines/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 from os import symlink
 from urllib.request import urlretrieve as download_uri
 
 from importlib_metadata import entry_points
 from invisibleroads_macros_log import format_path
 from invisibleroads_macros_text import format_slug
 from invisibleroads_macros_web.escape import (
-    escape_quotes_html,
-    escape_quotes_js)
+    escape_quotes_html)
 
 from ..constants import (
     CACHED_FILE_SIZE_LIMIT_IN_BYTES,
     FILES_FOLDER,
     FILES_ROUTE,
     MAXIMUM_FILE_CACHE_LENGTH,
     VARIABLE_ID_TEMPLATE_PATTERN)
@@ -67,18 +66,17 @@
 from .interface import Batch
 
 
 @dataclass(repr=False, eq=False, order=False, frozen=True)
 class Element():
 
     id: str
-    request_params: str
     mode_name: str
-    design_name: str
-    for_print: bool
+    request_params: str
+    layout_settings: dict
     function_names: list[str]
 
 
 class VariableView():
 
     view_name = 'variable'
     environment_variable_definitions = []
@@ -90,15 +88,15 @@
 
     @classmethod
     def get_from(Class, variable_definition):
         view_name = variable_definition.view_name
         try:
             View = view_by_name[view_name]
         except KeyError:
-            L.error('%s view not installed', view_name)
+            L.error('view "%s" is not installed', view_name)
             View = Class
         return View(variable_definition)
 
     def parse(self, data):
         return data
 
     def process(self, path):
@@ -107,15 +105,15 @@
     def render(self, b: Batch, x: Element):
         if x.mode_name == 'input':
             render = self.render_input
         else:
             render = self.render_output
         page_dictionary = render(b, x)
         main_text = page_dictionary['main_text']
-        if x.design_name != 'none':
+        if x.layout_settings['design_name'] != 'none':
             if main_text.endswith('</a>') or main_text.endswith('</span>'):
                 tag_name = 'span'
             else:
                 tag_name = 'div'
             main_text = add_label_html(
                 main_text, self.variable_definition, x.id)
             page_dictionary['main_text'] = '<%s class="_view">\n%s\n</%s>' % (
@@ -142,30 +140,30 @@
 class LinkView(VariableView):
 
     view_name = 'link'
 
     def render_output(self, b: Batch, x: Element):
         variable_definition = self.variable_definition
         variable_id = self.variable_id
-        element_id = x.id
         data_uri = b.get_data_uri(variable_definition, x)
-        c = b.get_variable_configuration(variable_definition)
+        c = b.get_data_configuration(variable_definition)
+        element_id = x.id
         file_name = c.get('file-name', self.variable_path.name)
         link_text = c.get('link-text', file_name)
         main_text = (
             f'<a id="{element_id}" href="{data_uri}" '
             f'class="_{x.mode_name} _{self.view_name} {variable_id}" '
-            f'download="{escape_quotes_html(file_name)}">'
+            f'download="{escape_quotes_html(file_name)}" '
+            f'data-text="{escape_quotes_html(link_text)}">'
             f'{link_text}</a>')
         js_texts = [
             LINK_OUTPUT_HEADER_JS,
             LINK_OUTPUT_JS.substitute({
                 'variable_id': variable_id,
-                'element_id': element_id,
-                'link_text': escape_quotes_js(link_text)})]
+                'element_id': element_id})]
         return {
             'css_uris': [], 'css_texts': [], 'js_uris': [],
             'js_texts': js_texts, 'main_text': main_text}
 
 
 class StringView(VariableView):
 
@@ -185,45 +183,46 @@
             value = ''
         return value
 
     def render_input(self, b: Batch, x: Element):
         variable_definition = self.variable_definition
         variable_id = self.variable_id
         view_name = self.view_name
-        element_id = x.id
         value = self.get_value(b, x)
-        c = b.get_variable_configuration(variable_definition)
+        c = b.get_data_configuration(variable_definition)
+        element_id = x.id
         main_text = STRING_INPUT_HTML.render({
             'element_id': element_id,
             'mode_name': x.mode_name,
             'view_name': view_name,
             'variable_id': variable_id,
             'value': escape_quotes_html(value),
             'input_type': self.input_type,
             'suggestions': c.get('suggestions', [])})
         js_texts = [
             STRING_INPUT_HEADER_JS.substitute({'view_name': view_name})]
         return {
             'css_uris': [], 'css_texts': [], 'js_uris': [],
-            'main_text': main_text, 'js_texts': js_texts}
+            'js_texts': js_texts, 'main_text': main_text}
 
     def render_output(self, b: Batch, x: Element):
         value = self.get_value(b, x)
         try:
             value = apply_functions(
                 value, x.function_names, self.function_by_name)
         except KeyError as e:
-            L.error('%s function not supported for %s', e, self.view_name)
+            L.error(
+                'function "%s" not supported for view "%s"', e, self.view_name)
         variable_definition = self.variable_definition
         variable_id = self.variable_id
-        element_id = x.id
         data_uri = b.get_data_uri(variable_definition, x)
+        element_id = x.id
         main_text = (
-            f'<span id="{x.id}" '
-            f'class="_{x.mode_name} _{self.view_name} {self.variable_id}">'
+            f'<span id="{element_id}" '
+            f'class="_{x.mode_name} _{self.view_name} {variable_id}">'
             f'{value}</span>')
         js_texts = [
             STRING_OUTPUT_HEADER_JS,
             STRING_OUTPUT_JS.substitute({
                 'variable_id': variable_id,
                 'element_id': element_id,
                 'data_uri': data_uri})]
@@ -261,19 +260,20 @@
 
 class TextView(VariableView):
 
     view_name = 'text'
 
     def render_input(self, b: Batch, x: Element):
         variable_definition = self.variable_definition
-        data = get_data_from(x.request_params, variable_definition)
-        value = data.get('value', '')
         variable_id = self.variable_id
         view_name = self.view_name
+        data_uri = b.get_data_uri(variable_definition, x)
+        data = get_data_from(x.request_params, variable_definition)
         element_id = x.id
+        value = data.get('value', '')
         main_text = TEXT_INPUT_HTML.substitute({
             'element_id': element_id,
             'mode_name': x.mode_name,
             'view_name': view_name,
             'variable_id': variable_id,
             'attribute_string': '' if value else ' disabled',
             'value': value})
@@ -281,27 +281,27 @@
             STRING_OUTPUT_HEADER_JS,
             STRING_INPUT_HEADER_JS.substitute({'view_name': view_name})]
         if not value:
             js_texts.extend([
                 TEXT_OUTPUT_HEADER_JS,
                 TEXT_INPUT_JS.substitute({
                     'element_id': element_id,
-                    'data_uri': b.get_data_uri(variable_definition, x)})])
+                    'data_uri': data_uri})])
         return {
             'css_uris': [], 'css_texts': [], 'js_uris': [],
-            'main_text': main_text, 'js_texts': js_texts}
+            'js_texts': js_texts, 'main_text': main_text}
 
     def render_output(self, b: Batch, x: Element):
         variable_definition = self.variable_definition
         variable_id = self.variable_id
-        element_id = x.id
         data_uri = b.get_data_uri(variable_definition, x)
+        element_id = x.id
         main_text = (
-            f'<span id="{x.id}" '
-            f'class="_{x.mode_name} _{self.view_name} {self.variable_id}">'
+            f'<span id="{element_id}" '
+            f'class="_{x.mode_name} _{self.view_name} {variable_id}">'
             '</span>')
         js_texts = [
             STRING_OUTPUT_HEADER_JS,
             TEXT_OUTPUT_HEADER_JS,
             TEXT_OUTPUT_JS.substitute({
                 'variable_id': variable_id,
                 'element_id': element_id,
@@ -315,19 +315,19 @@
 
     view_name = 'markdown'
     js_uris = ['https://cdn.jsdelivr.net/npm/marked/marked.min.js']
 
     def render_output(self, b: Batch, x: Element):
         variable_definition = self.variable_definition
         variable_id = self.variable_id
-        element_id = x.id
         data_uri = b.get_data_uri(variable_definition, x)
+        element_id = x.id
         main_text = (
-            f'<span id="{x.id}" '
-            f'class="_{x.mode_name} _{self.view_name} {self.variable_id}">'
+            f'<span id="{element_id}" '
+            f'class="_{x.mode_name} _{self.view_name} {variable_id}">'
             '</span>')
         js_texts = [
             STRING_OUTPUT_HEADER_JS,
             MARKDOWN_OUTPUT_HEADER_JS,
             MARKDOWN_OUTPUT_JS.substitute({
                 'variable_id': variable_id,
                 'element_id': element_id,
@@ -340,18 +340,18 @@
 class ImageView(VariableView):
 
     view_name = 'image'
 
     def render_output(self, b: Batch, x: Element):
         variable_definition = self.variable_definition
         variable_id = self.variable_id
-        element_id = x.id
         data_uri = b.get_data_uri(variable_definition, x)
+        element_id = x.id
         main_text = (
-            f'<img id="{x.id}" '
+            f'<img id="{element_id}" '
             f'class="_{x.mode_name} _{self.view_name} {variable_id}" '
             f'src="{data_uri}" alt="">')
         # TODO: Show spinner on error
         js_texts = [
             IMAGE_OUTPUT_HEADER_JS,
             IMAGE_OUTPUT_JS.substitute({
                 'variable_id': variable_id,
@@ -366,24 +366,25 @@
 
     view_name = 'radio'
 
     def render_input(self, b: Batch, x: Element):
         variable_definition = self.variable_definition
         variable_id = self.variable_id
         view_name = self.view_name
-        element_id = x.id
-        c = b.get_variable_configuration(variable_definition)
+        c = b.get_data_configuration(variable_definition)
         data = b.load_data_from(x.request_params, variable_definition)
+        element_id = x.id
         value = data.get('value', '')
         main_text = RADIO_INPUT_HTML.render({
             'element_id': element_id,
             'mode_name': x.mode_name,
             'view_name': view_name,
             'variable_id': variable_id,
-            'options': get_configuration_options(c, [value]),
+            'options': get_configuration_options(
+                c, [value] if value != '' else []),
             'value': value})
         js_texts = [
             RADIO_INPUT_HEADER_JS.substitute({'view_name': view_name})]
         if variable_definition.step_name != 'input':
             data_uri = b.get_data_uri(variable_definition, x)
             js_texts.extend([
                 RADIO_OUTPUT_HEADER_JS,
@@ -396,21 +397,21 @@
 
 
 class CheckboxView(VariableView):
 
     view_name = 'checkbox'
 
     def render_input(self, b: Batch, x: Element):
-        element_id = x.id
         view_name = self.view_name
         variable_id = self.variable_id
         variable_definition = self.variable_definition
-        c = b.get_variable_configuration(variable_definition)
+        c = b.get_data_configuration(variable_definition)
         data = b.load_data_from(x.request_params, variable_definition)
-        values = data.get('value', '').splitlines()
+        element_id = x.id
+        values = data.get('value', '').strip().splitlines()
         main_text = CHECKBOX_INPUT_HTML.render({
             'element_id': element_id,
             'mode_name': x.mode_name,
             'view_name': view_name,
             'variable_id': variable_id,
             'options': get_configuration_options(c, values),
             'values': values})
@@ -432,16 +433,16 @@
 class TableView(VariableView):
 
     view_name = 'table'
 
     def render_output(self, b: Batch, x: Element):
         variable_definition = self.variable_definition
         variable_id = self.variable_id
-        element_id = x.id
         data_uri = b.get_data_uri(variable_definition, x)
+        element_id = x.id
         main_text = (
             f'<table id="{element_id}" '
             f'class="_{x.mode_name} _{self.view_name} {variable_id}">'
             '<thead/><tbody/></table>')
         js_texts = [
             TABLE_OUTPUT_HEADER_JS,
             TABLE_OUTPUT_JS.substitute({
@@ -456,17 +457,17 @@
 class FrameView(VariableView):
 
     view_name = 'frame'
 
     def render_output(self, b: Batch, x: Element):
         variable_definition = self.variable_definition
         variable_id = self.variable_id
-        element_id = x.id
         data_uri = b.get_data_uri(variable_definition, x)
         data = b.load_data(variable_definition)
+        element_id = x.id
         if 'value' in data:
             value = data['value']
         else:
             value = ''
         main_text = (
             f'<iframe id="{element_id}" '
             f'class="_{x.mode_name} _{self.view_name} {variable_id}" '
@@ -505,16 +506,16 @@
 
     view_name = 'pdf'
     css_texts = [PDF_CSS]
 
     def render_output(self, b: Batch, x: Element):
         variable_definition = self.variable_definition
         variable_id = self.variable_id
-        element_id = x.id
         data_uri = b.get_data_uri(variable_definition, x)
+        element_id = x.id
         js_texts = [
             PDF_OUTPUT_HEADER_JS,
             PDF_OUTPUT_JS.substitute({
                 'variable_id': variable_id,
                 'element_id': element_id,
                 'data_uri': data_uri})]
         main_text = (
@@ -528,19 +529,19 @@
 
 
 class FileView(VariableView):
 
     view_name = 'file'
 
     def render_input(self, b: Batch, x: Element):
-        element_id = x.id
         view_name = self.view_name
         variable_id = self.variable_id
         variable_definition = self.variable_definition
-        c = b.get_variable_configuration(variable_definition)
+        c = b.get_data_configuration(variable_definition)
+        element_id = x.id
         mime_types = c.get('mime-types', [])
         root_uri = template_globals['root_uri']
         js_texts = [
             FILE_INPUT_HEADER_JS.substitute({
                 'view_name': view_name,
                 'files_uri': root_uri + FILES_ROUTE})]
         main_text = FILE_INPUT_HTML.substitute({
@@ -561,25 +562,25 @@
 
 
 def save_variable_data(target_path, data_by_id, variable_definitions):
     target_path.parent.mkdir(parents=True, exist_ok=True)
     variable_data_by_id = get_variable_data_by_id(
         variable_definitions, data_by_id)
     if target_path.suffix == '.dictionary':
-        with open(target_path, 'wt') as input_file:
+        with target_path.open('wt') as input_file:
             variable_value_by_id = get_variable_value_by_id(
                 variable_data_by_id)
             json.dump(variable_value_by_id, input_file)
     elif len(variable_data_by_id) > 1:
         raise CrossComputeConfigurationError(
             'use file extension .dictionary for multiple variables')
     else:
         variable_id, variable_data = list(variable_data_by_id.items())[0]
         if 'value' in variable_data:
-            open(target_path, 'wt').write(variable_data['value'])
+            target_path.open('wt').write(variable_data['value'])
         elif 'path' in variable_data:
             shutil.copy(variable_data['path'], target_path)
         elif 'uri' in variable_data:
             variable_uri = variable_data['uri']
             if variable_uri.startswith(
                 'http://'
             ) or variable_uri.startswith('https://'):
@@ -590,16 +591,15 @@
             variable_definitions, 'id', variable_id)
         variable_view = VariableView.get_from(variable_definition)
         variable_view.process(target_path)
 
 
 def link_files(path_template, variable_uri):
     folder = FILES_FOLDER / variable_uri.replace('/f/', '')
-    with open(folder / 'files.json', 'rt') as f:
-        file_dictionaries = json.load(f)
+    file_dictionaries = load_file_json(folder / 'files.json')
     for file_index, file_dictionary in enumerate(file_dictionaries):
         file_path = folder / str(file_index)
         file_extension = file_dictionary['extension']
         target_path = str(path_template).format(
             index=file_index, extension=file_extension)
         symlink(file_path, target_path)
         L.debug(f'linked {file_path} to {target_path}')
@@ -766,22 +766,22 @@
 
 def load_file_data(path):
     if not path.exists():
         raise CrossComputeDataError(f'could not find {format_path(path)}')
     suffix = path.suffix
     if suffix == '.dictionary':
         return load_dictionary_data(path)
-    if suffix == '.txt':
+    if suffix in ['.md', '.txt']:
         return load_text_data(path)
     return {'path': path}
 
 
 def load_dictionary_data(path):
     try:
-        value = json.load(path.open('rt'))
+        value = load_file_json(path)
     except (json.JSONDecodeError, OSError) as e:
         raise CrossComputeDataError(
             f'could not load {format_path(path)}: {e}')
     if not isinstance(value, dict):
         raise CrossComputeDataError(
             f'expected dictionary in {format_path(path)}')
     return {'value': value}
@@ -798,14 +798,20 @@
     return {'value': value}
 
 
 def load_file_text(path):
     return path.read_text().rstrip()
 
 
+def load_file_json(path):
+    with path.open('rt') as f:
+        d = json.load(f)
+    return d
+
+
 def get_variable_data_by_id(
         variable_definitions, data_by_id, with_exceptions=True):
     variable_data_by_id = {}
     for variable_definition in variable_definitions:
         variable_id = variable_definition.id
         if None in data_by_id:
             variable_data = data_by_id[None]
```

### Comparing `crosscompute-0.9.4.4/crosscompute/routines/work.py` & `crosscompute-0.9.4.8/crosscompute/routines/work.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,34 +100,38 @@
             'return_code': return_code}})
 
 
 class UnsafeEngine(AbstractEngine):
 
     def prepare(self, automation_definition):
         # TODO: Consider having a separate venv for each automation
+        automation_folder = automation_definition.folder
         d = automation_definition.package_ids_by_manager_name
         try:
             for manager_name, package_ids in d.items():
-                subprocess.run([
-                    manager_name, 'install'] + list(package_ids), check=True)
-        except subprocess.CalledProcessError:
-            raise CrossComputeExecutionError()
+                subprocess.run(
+                    [manager_name, 'install'] + list(package_ids),
+                    cwd=automation_folder,
+                    check=True)
+        except (OSError, subprocess.CalledProcessError) as e:
+            raise CrossComputeExecutionError(
+                'could not install packages: %s' % e)
         for s in automation_definition.script_definitions:
             s.get_command_string()
 
     def run(self, automation_definition, batch_folder, custom_environment):
         step_folder_by_name = _get_step_folder_by_name(
             automation_definition.folder, batch_folder)
         script_definitions = automation_definition.script_definitions
         script_environment = _prepare_script_environment(
             step_folder_by_name, custom_environment, with_path=True)
         debug_folder = step_folder_by_name['debug_folder']
         o_path = debug_folder / 'stdout.txt'
         e_path = debug_folder / 'stderr.txt'
-        with open(o_path, 'wt') as o_file, open(e_path, 'w+t') as e_file:
+        with o_path.open('wt') as o_file, e_path.open('w+t') as e_file:
             for script_definition in script_definitions:
                 return_code = _run_script(
                     script_definition, step_folder_by_name,
                     script_environment, o_file, e_file)
         return return_code
 
 
@@ -240,18 +244,18 @@
             except URLError:
                 L.error(f'could not download dataset from {reference_uri}')
 
 
 def process_loop(
         automation_definitions, automation_tasks, live_uris, file_changes,
         user_environment, server_uri, with_rebuild):
-    for a in automation_definitions:
-        prepare_automation(a, with_rebuild)
-        for b in a.batch_definitions:
-            prepare_batch(a, b)
+    thread = Thread(
+        target=prepare_loop, args=(automation_definitions, with_rebuild),
+        daemon=True)
+    thread.start()
     try:
         while True:
             sleep(1)
             try:
                 automation_task = _get_automation_task(
                     automation_tasks, automation_definitions, live_uris,
                     file_changes, user_environment)
@@ -261,14 +265,22 @@
                 target=_process_task, args=automation_task + (server_uri,),
                 daemon=True)
             thread.start()
     except KeyboardInterrupt:
         pass
 
 
+def prepare_loop(automation_definitions, with_rebuild):
+    for a in automation_definitions:
+        for b in a.batch_definitions:
+            prepare_batch(a, b)
+    for a in automation_definitions:
+        prepare_automation(a, with_rebuild)
+
+
 def prepare_automation(automation_definition, with_rebuild=True):
     engine = get_script_engine(automation_definition.engine_name, with_rebuild)
     engine.prepare(automation_definition)
 
 
 def prepare_batch(automation_definition, batch_definition):
     variable_definitions = automation_definition.get_variable_definitions(
```

### Comparing `crosscompute-0.9.4.4/crosscompute/scripts/configure.py` & `crosscompute-0.9.4.8/crosscompute/scripts/configure.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         L.warning('%s already exists', formatted_configuration_path)
         question = '\033[1moverwrite? yes or [no]:\033[0m '
         participle = 'overwritten'
     else:
         question = 'save? yes or [no]: '
         participle = 'saved'
     if not input(question).lower() == 'yes':
-        L.warning('%s not %s', formatted_configuration_path, participle)
+        L.warning('%s was not %s', formatted_configuration_path, participle)
         raise SystemExit
     try:
         save_raw_configuration(configuration_path, configuration)
     except CrossComputeError as e:
         L.error(e)
         raise SystemExit
     L.info('%s %s', formatted_configuration_path, participle)
```

### Comparing `crosscompute-0.9.4.4/crosscompute/scripts/launch.py` & `crosscompute-0.9.4.8/crosscompute/scripts/launch.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,16 @@
 
 
 def _get_automation_from(args):
     path_or_folder = args.path_or_folder
     try:
         automation = DiskAutomation.load(path_or_folder or '.')
     except CrossComputeConfigurationNotFoundError:
-        L.info('existing configuration not found; configuring new automation')
+        L.info(
+            'existing configuration was not found; configuring new automation')
         print()
         path = configure_with(args)
         automation = DiskAutomation.load(path)
     except CrossComputeError as e:
         L.error(e)
         raise SystemExit
     return automation
```

### Comparing `crosscompute-0.9.4.4/crosscompute/scripts/print.py` & `crosscompute-0.9.4.8/crosscompute/scripts/print.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.4/crosscompute/scripts/run.py` & `crosscompute-0.9.4.8/crosscompute/scripts/run.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.4/crosscompute/scripts/serve.py` & `crosscompute-0.9.4.8/crosscompute/scripts/serve.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.4/crosscompute/settings.py` & `crosscompute-0.9.4.8/crosscompute/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     PathTemplateLoader,
     RelativeTemplateEnvironment)
 from invisibleroads_macros_web.starlette import (
     TemplateResponseFactory)
 
 from .constants import (
     TEMPLATE_PATH_BY_ID)
+from .macros.iterable import get_unique_order
 
 
 multiprocessing_context = mp.get_context('fork')
 StoppableProcess = partial(
     invisibleroads_macros_process.StoppableProcess,
     multiprocessing_context.Process)
 site = {
@@ -30,14 +31,15 @@
 template_path_by_id = TEMPLATE_PATH_BY_ID.copy()
 template_environment = RelativeTemplateEnvironment(
     loader=PathTemplateLoader(),
     autoescape=True,
     trim_blocks=True,
     lstrip_blocks=True)
 template_globals = template_environment.globals = {
+    'get_unique_order': get_unique_order,
     'base_template_path': template_path_by_id['base'],
     'live_template_path': template_path_by_id['live'],
     'google_analytics_id': '',
     'server_time': 0,
     'root_uri': '',
     'with_restart': True}
 TemplateResponse = TemplateResponseFactory(
```

### Comparing `crosscompute-0.9.4.4/crosscompute.egg-info/PKG-INFO` & `crosscompute-0.9.4.8/crosscompute.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosscompute
-Version: 0.9.4.4
+Version: 0.9.4.8
 Summary: Automate your Jupyter notebooks and scripts as tools, reports, dashboards.
 Home-page: https://crosscompute.com
 Author: CrossCompute Inc.
 Author-email: support@crosscompute.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/crosscompute/crosscompute/issues
 Project-URL: Documentation, https://docs.crosscompute.com
@@ -78,17 +78,17 @@
 # Initialize configuration
 crosscompute
 
 # Serve automation
 crosscompute automate.yml
 ```
 
-Here are some tutorials and examples:
+Here are some examples and tutorials:
 
-- [Examples](https://crosscompute.net) [[source](https://github.com/crosscompute/crosscompute-examples)]
+- [Gallery](https://crosscompute.net) [[source](https://github.com/crosscompute/crosscompute-examples)]
 - [Documentation](https://docs.crosscompute.com) [[source](https://github.com/crosscompute/crosscompute-docs)]
 - [Forum](https://forum.crosscompute.com)
 
 ## Development
 
 ```bash
 # Clone repository
@@ -134,19 +134,19 @@
 source ~/.virtualenvs/crosscompute/bin/activate
 
 pip install crosscompute>=0.9.4
 ```
 
 ## Acknowledgments
 
+- [Kashfi Fahim](https://www.linkedin.com/in/kashfifahim)
 - [Olga Ryabtseva](https://www.linkedin.com/in/olga-creutzburg)
 - [Salah Ahmed](https://www.linkedin.com/in/salahspage)
 - [Rodrigo Guarachi](https://www.linkedin.com/in/rmguarachi)
 - [Polina Chernomaz](https://www.linkedin.com/in/polinac)
 - [Miguel Ángel Gordián](https://www.linkedin.com/in/miguelgordian)
 - [Noé Domínguez Porras](https://www.linkedin.com/in/noedominguez)
 - [Marta Moreno](https://www.linkedin.com/in/marta-moreno-07364b82)
 - [Ning Wei](https://www.linkedin.com/in/ning-wei-8152393b)
-- [Kashfi Fahim](https://www.linkedin.com/in/kashfifahim)
 - [Elaine Chan](https://www.linkedin.com/in/chanelaine)
 - [Aida Shoydokova](https://www.linkedin.com/in/ashoydok)
 - [Jennifer Ruda](https://www.linkedin.com/in/jruda)
```

### Comparing `crosscompute-0.9.4.4/crosscompute.egg-info/SOURCES.txt` & `crosscompute-0.9.4.8/crosscompute.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 crosscompute.egg-info/PKG-INFO
 crosscompute.egg-info/SOURCES.txt
 crosscompute.egg-info/dependency_links.txt
 crosscompute.egg-info/entry_points.txt
 crosscompute.egg-info/requires.txt
 crosscompute.egg-info/top_level.txt
 crosscompute.egg-info/zip-safe
+crosscompute/assets/LogoBrand-Horizontal-20230501.svg
 crosscompute/assets/automation.html
 crosscompute/assets/base.html
 crosscompute/assets/button-panel.html
 crosscompute/assets/checkbox-input-header.js
 crosscompute/assets/checkbox-input.html
 crosscompute/assets/checkbox-output-header.js
 crosscompute/assets/checkbox-output.js
 crosscompute/assets/configuration.yml
 crosscompute/assets/default.css
 crosscompute/assets/embedded.css
 crosscompute/assets/favicon.ico
 crosscompute/assets/file-input-header.js
 crosscompute/assets/file-input.html
-crosscompute/assets/file-input.js
 crosscompute/assets/flex.css
 crosscompute/assets/frame-output-header.js
 crosscompute/assets/frame-output.js
 crosscompute/assets/image-output-header.js
 crosscompute/assets/image-output.js
 crosscompute/assets/json-output-header.js
 crosscompute/assets/json-output.js
@@ -40,15 +40,14 @@
 crosscompute/assets/link-output.js
 crosscompute/assets/live.html
 crosscompute/assets/markdown-output-header.js
 crosscompute/assets/markdown-output.js
 crosscompute/assets/pdf-output-header.js
 crosscompute/assets/pdf-output.js
 crosscompute/assets/pdf.css
-crosscompute/assets/printed.css
 crosscompute/assets/radio-input-header.js
 crosscompute/assets/radio-input.html
 crosscompute/assets/radio-output-header.js
 crosscompute/assets/radio-output.js
 crosscompute/assets/root.html
 crosscompute/assets/step-body.js
 crosscompute/assets/step.html
@@ -92,12 +91,13 @@
 crosscompute/routines/work.py
 crosscompute/scripts/__init__.py
 crosscompute/scripts/configure.py
 crosscompute/scripts/launch.py
 crosscompute/scripts/print.py
 crosscompute/scripts/run.py
 crosscompute/scripts/serve.py
+tests/test_constants.py
 tests/test_macros_iterable.py
 tests/test_macros_security.py
 tests/test_routines_configuration.py
 tests/test_routines_variable.py
 tests/test_routines_work.py
```

### Comparing `crosscompute-0.9.4.4/crosscompute.egg-info/entry_points.txt` & `crosscompute-0.9.4.8/crosscompute.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.4/setup.cfg` & `crosscompute-0.9.4.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosscompute
-version = 0.9.4.4
+version = 0.9.4.8
 description = Automate your Jupyter notebooks and scripts as tools, reports, dashboards.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://crosscompute.com
 author = CrossCompute Inc.
 author_email = support@crosscompute.com
 license = MIT
@@ -36,34 +36,34 @@
 	fastapi
 	importlib-metadata >= 6.6.0
 	invisibleroads-macros-disk >= 1.3.0
 	invisibleroads-macros-log >= 1.0.6
 	invisibleroads-macros-process >= 0.2.0
 	invisibleroads-macros-security >= 1.0.3
 	invisibleroads-macros-text >= 1.1.2
-	invisibleroads-macros-web[jinja,markdown,starlette] >= 0.3.0
+	invisibleroads-macros-web[jinja,markdown,starlette] >= 0.3.3
 	jinja2
-	markdown
 	nbconvert
 	nbformat
 	python-multipart
 	requests
 	ruamel.yaml
 	sse-starlette
 	tomli
-	uvicorn >= 0.21.1
+	uvicorn >= 0.22.0
 	watchfiles
 zip_safe = True
 
 [options.package_data]
 crosscompute = 
 	assets/*.css
 	assets/*.html
 	assets/*.ico
 	assets/*.js
+	assets/*.svg
 	assets/*.yml
 
 [options.entry_points]
 console_scripts = 
 	crosscompute = crosscompute.scripts.launch:do
 crosscompute.views = 
 	link = crosscompute.routines.variable.LinkView
```

### Comparing `crosscompute-0.9.4.4/tests/test_routines_configuration.py` & `crosscompute-0.9.4.8/tests/test_routines_configuration.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.4/tests/test_routines_variable.py` & `crosscompute-0.9.4.8/tests/test_routines_variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,16 @@
     json.dump({'a': 1}, path.open('wt'))
     assert load_file_data(path)['value']['a'] == 1
 
     path = tmp_path / 'x.txt'
     path.write_text('whee')
     assert load_file_data(path)['value'] == 'whee'
 
-    path = tmp_path / 'x.md'
-    path.write_text('whee')
+    path = tmp_path / 'x.json'
+    json.dump({}, path.open('wt'))
     assert load_file_data(path)['path'] == path
 
 
 def test_load_dictionary_data(tmp_path):
     path = tmp_path / 'x.dictionary'
 
     with raises(CrossComputeDataError):
```

### Comparing `crosscompute-0.9.4.4/tests/test_routines_work.py` & `crosscompute-0.9.4.8/tests/test_routines_work.py`

 * *Files identical despite different names*

