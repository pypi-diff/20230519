# Comparing `tmp/httpie-3.2.1.tar.gz` & `tmp/httpie-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpie-3.2.1.tar", last modified: Fri May  6 07:10:35 2022, max compression
+gzip compressed data, was "httpie-3.2.2.tar", last modified: Fri May 19 21:40:41 2023, max compression
```

## Comparing `httpie-3.2.1.tar` & `httpie-3.2.2.tar`

### file list

```diff
@@ -1,224 +1,277 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.069795 httpie-3.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1788 2022-05-06 07:10:04.000000 httpie-3.2.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (121)    26210 2022-05-06 07:10:04.000000 httpie-3.2.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1534 2022-05-06 07:10:04.000000 httpie-3.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-05-06 07:10:04.000000 httpie-3.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5544 2022-05-06 07:10:35.069795 httpie-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4260 2022-05-06 07:10:04.000000 httpie-3.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.049795 httpie-3.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)    82870 2022-05-06 07:10:04.000000 httpie-3.2.1/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.049795 httpie-3.2.1/extras/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.049795 httpie-3.2.1/extras/man/
--rw-r--r--   0 runner    (1001) docker     (121)    14728 2022-05-06 07:10:04.000000 httpie-3.2.1/extras/man/http.1
--rw-r--r--   0 runner    (1001) docker     (121)     2352 2022-05-06 07:10:04.000000 httpie-3.2.1/extras/man/httpie.1
--rw-r--r--   0 runner    (1001) docker     (121)    14731 2022-05-06 07:10:04.000000 httpie-3.2.1/extras/man/https.1
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.053795 httpie-3.2.1/httpie/
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/adapters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.053795 httpie-3.2.1/httpie/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23136 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/cli/argparser.py
--rw-r--r--   0 runner    (1001) docker     (121)     7991 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/cli/argtypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3340 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    28652 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/cli/definition.py
--rw-r--r--   0 runner    (1001) docker     (121)     2390 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/cli/dicts.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    11052 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/cli/nested_json.py
--rw-r--r--   0 runner    (1001) docker     (121)     7732 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (121)     7179 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/cli/requestitems.py
--rw-r--r--   0 runner    (1001) docker     (121)     2151 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    13324 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3500 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     5005 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     6726 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/cookies.py
--rw-r--r--   0 runner    (1001) docker     (121)    10442 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    11805 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/downloads.py
--rw-r--r--   0 runner    (1001) docker     (121)     1385 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.053795 httpie-3.2.1/httpie/internal/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-05-06 07:10:25.000000 httpie-3.2.1/httpie/internal/__build_channel__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/internal/daemon_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     3406 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/internal/daemons.py
--rw-r--r--   0 runner    (1001) docker     (121)     5178 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/internal/update_warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.053795 httpie-3.2.1/httpie/legacy/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2905 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/legacy/v3_1_0_session_cookie_format.py
--rw-r--r--   0 runner    (1001) docker     (121)     2078 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/legacy/v3_2_0_session_header_format.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.057795 httpie-3.2.1/httpie/manager/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1752 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/manager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5371 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/manager/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2023 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/manager/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1142 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/manager/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.057795 httpie-3.2.1/httpie/manager/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/manager/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/manager/tasks/check_updates.py
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/manager/tasks/export_args.py
--rw-r--r--   0 runner    (1001) docker     (121)     8526 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/manager/tasks/plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)     2686 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/manager/tasks/sessions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6167 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.057795 httpie-3.2.1/httpie/output/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/output/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.057795 httpie-3.2.1/httpie/output/formatters/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/output/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13002 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/output/formatters/colors.py
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/output/formatters/headers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1123 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/output/formatters/json.py
--rw-r--r--   0 runner    (1001) docker     (121)     2505 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/output/formatters/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.057795 httpie-3.2.1/httpie/output/lexers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/output/lexers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      517 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/output/lexers/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     3044 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/output/lexers/http.py
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/output/lexers/json.py
--rw-r--r--   0 runner    (1001) docker     (121)     1672 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/output/lexers/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/output/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1763 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/output/processing.py
--rw-r--r--   0 runner    (1001) docker     (121)     8155 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/output/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.057795 httpie-3.2.1/httpie/output/ui/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/output/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1276 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/output/ui/man_pages.py
--rw-r--r--   0 runner    (1001) docker     (121)     7226 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/output/ui/palette.py
--rw-r--r--   0 runner    (1001) docker     (121)     6565 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/output/ui/rich_help.py
--rw-r--r--   0 runner    (1001) docker     (121)     2294 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/output/ui/rich_palette.py
--rw-r--r--   0 runner    (1001) docker     (121)     3980 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/output/ui/rich_progress.py
--rw-r--r--   0 runner    (1001) docker     (121)      972 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/output/ui/rich_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/output/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6515 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/output/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.057795 httpie-3.2.1/httpie/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4529 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/plugins/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2123 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/plugins/builtin.py
--rw-r--r--   0 runner    (1001) docker     (121)     4049 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/plugins/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/plugins/registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     9705 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/sessions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2891 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/ssl_.py
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/status.py
--rw-r--r--   0 runner    (1001) docker     (121)     7744 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/uploads.py
--rw-r--r--   0 runner    (1001) docker     (121)     9137 2022-05-06 07:10:04.000000 httpie-3.2.1/httpie/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.053795 httpie-3.2.1/httpie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5544 2022-05-06 07:10:34.000000 httpie-3.2.1/httpie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6236 2022-05-06 07:10:35.000000 httpie-3.2.1/httpie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-06 07:10:34.000000 httpie-3.2.1/httpie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-05-06 07:10:34.000000 httpie-3.2.1/httpie.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-05-06 07:10:34.000000 httpie-3.2.1/httpie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-05-06 07:10:34.000000 httpie-3.2.1/httpie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-05-06 07:10:35.069795 httpie-3.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3283 2022-05-06 07:10:04.000000 httpie-3.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.061795 httpie-3.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.061795 httpie-3.2.1/tests/client_certs/
--rw-r--r--   0 runner    (1001) docker     (121)     1939 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/client_certs/client.crt
--rw-r--r--   0 runner    (1001) docker     (121)     3243 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/client_certs/client.key
--rw-r--r--   0 runner    (1001) docker     (121)     5182 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/client_certs/client.pem
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.061795 httpie-3.2.1/tests/client_certs/password_protected/
--rw-r--r--   0 runner    (1001) docker     (121)     2546 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/client_certs/password_protected/client.key
--rw-r--r--   0 runner    (1001) docker     (121)     1594 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/client_certs/password_protected/client.pem
--rw-r--r--   0 runner    (1001) docker     (121)     2359 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.061795 httpie-3.2.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)     2091 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.049795 httpie-3.2.1/tests/fixtures/session_data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.065795 httpie-3.2.1/tests/fixtures/session_data/new/
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/session_data/new/cookies_dict.json
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/session_data/new/cookies_dict_dev_version.json
--rw-r--r--   0 runner    (1001) docker     (121)      811 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/session_data/new/cookies_dict_with_extras.json
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/session_data/new/empty_cookies_dict.json
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/session_data/new/empty_cookies_list.json
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/session_data/new/empty_headers_dict.json
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/session_data/new/empty_headers_list.json
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/session_data/new/headers_cookies_dict_mixed.json
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/session_data/new/headers_dict.json
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/session_data/new/headers_dict_extras.json
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/session_data/new/headers_list.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.065795 httpie-3.2.1/tests/fixtures/session_data/old/
--rw-r--r--   0 runner    (1001) docker     (121)      558 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/session_data/old/cookies_dict.json
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/session_data/old/cookies_dict_dev_version.json
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/session_data/old/cookies_dict_with_extras.json
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/session_data/old/empty_cookies_dict.json
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/session_data/old/empty_cookies_list.json
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/session_data/old/empty_headers_dict.json
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/session_data/old/empty_headers_list.json
--rw-r--r--   0 runner    (1001) docker     (121)      613 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/session_data/old/headers_cookies_dict_mixed.json
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/session_data/old/headers_dict.json
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/session_data/old/headers_dict_extras.json
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/session_data/old/headers_list.json
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/test.bin
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/test.json
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/test_with_dupe_keys.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.049795 httpie-3.2.1/tests/fixtures/xmldata/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.065795 httpie-3.2.1/tests/fixtures/xmldata/invalid/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/invalid/cyclic.xml
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/invalid/external.xml
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/invalid/external_file.xml
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/invalid/not-xml.xml
--rw-r--r--   0 runner    (1001) docker     (121)   103050 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/invalid/quadratic.xml
--rw-r--r--   0 runner    (1001) docker     (121)      875 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/invalid/xalan_exec.xsl
--rw-r--r--   0 runner    (1001) docker     (121)      695 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/invalid/xalan_write.xsl
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/invalid/xmlbomb.xml
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/invalid/xmlbomb2.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.065795 httpie-3.2.1/tests/fixtures/xmldata/valid/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/valid/custom-header.xml
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/valid/custom-header_formatted.xml
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/valid/dtd_formatted.xml
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/valid/dtd_raw.xml
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/valid/simple-ns_formatted.xml
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/valid/simple-ns_raw.xml
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/valid/simple-single-tag_formatted.xml
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/valid/simple-single-tag_raw.xml
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/valid/simple-standalone-no_formatted.xml
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/valid/simple-standalone-no_raw.xml
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/valid/simple-standalone-yes_formatted.xml
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/valid/simple-standalone-yes_raw.xml
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/valid/simple_formatted.xml
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/valid/simple_raw.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.069795 httpie-3.2.1/tests/fixtures/xmldata/xhtml/
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/xhtml/xhtml_formatted.xml
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/xhtml/xhtml_formatted_python_less_than_3.8.xml
--rw-r--r--   0 runner    (1001) docker     (121)      942 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/fixtures/xmldata/xhtml/xhtml_raw.xml
--rw-r--r--   0 runner    (1001) docker     (121)     5176 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     3689 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_auth_plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)     1986 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_binary.py
--rw-r--r--   0 runner    (1001) docker     (121)    14285 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2025 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_cli_ui.py
--rw-r--r--   0 runner    (1001) docker     (121)     2322 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3882 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_compress.py
--rw-r--r--   0 runner    (1001) docker     (121)     3773 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1876 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_cookie.py
--rw-r--r--   0 runner    (1001) docker     (121)     7191 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_cookie_on_redirects.py
--rw-r--r--   0 runner    (1001) docker     (121)     4908 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)     9739 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_downloads.py
--rw-r--r--   0 runner    (1001) docker     (121)     6761 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (121)     2392 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2678 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_exit_status.py
--rw-r--r--   0 runner    (1001) docker     (121)    10076 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_httpie.py
--rw-r--r--   0 runner    (1001) docker     (121)     4403 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_httpie_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    18678 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (121)     1979 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_offline.py
--rw-r--r--   0 runner    (1001) docker     (121)    20821 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_output.py
--rw-r--r--   0 runner    (1001) docker     (121)     2085 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_parser_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     5674 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_plugins_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     3580 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_redirects.py
--rw-r--r--   0 runner    (1001) docker     (121)     1159 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_regressions.py
--rw-r--r--   0 runner    (1001) docker     (121)    27010 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_sessions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7343 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (121)     4523 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (121)     3992 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_tokens.py
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_transport_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     6608 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_update_warnings.py
--rw-r--r--   0 runner    (1001) docker     (121)    12899 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_uploads.py
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_windows.py
--rw-r--r--   0 runner    (1001) docker     (121)     2869 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/test_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.069795 httpie-3.2.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (121)    12983 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4482 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/utils/http_server.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 07:10:35.069795 httpie-3.2.1/tests/utils/matching/
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/utils/matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2596 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/utils/matching/parsing.py
--rw-r--r--   0 runner    (1001) docker     (121)     5827 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/utils/matching/test_matching.py
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/utils/matching/tokens.py
--rw-r--r--   0 runner    (1001) docker     (121)     6572 2022-05-06 07:10:04.000000 httpie-3.2.1/tests/utils/plugins_cli.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.180986 httpie-3.2.2/
+-rw-r--r--   0 jakub      (501) staff       (20)     1788 2023-05-19 19:11:41.000000 httpie-3.2.2/AUTHORS.md
+-rw-r--r--   0 jakub      (501) staff       (20)    26389 2023-05-19 21:34:11.000000 httpie-3.2.2/CHANGELOG.md
+-rw-r--r--   0 jakub      (501) staff       (20)     1534 2023-05-19 19:11:41.000000 httpie-3.2.2/LICENSE
+-rw-r--r--   0 jakub      (501) staff       (20)      173 2023-05-19 19:11:41.000000 httpie-3.2.2/MANIFEST.in
+-rw-r--r--   0 jakub      (501) staff       (20)     6069 2023-05-19 21:40:41.181066 httpie-3.2.2/PKG-INFO
+-rw-r--r--   0 jakub      (501) staff       (20)     4805 2023-05-19 19:11:41.000000 httpie-3.2.2/README.md
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.143676 httpie-3.2.2/docs/
+-rw-r--r--   0 jakub      (501) staff       (20)    84094 2023-05-19 19:11:41.000000 httpie-3.2.2/docs/README.md
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.139762 httpie-3.2.2/extras/
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.144352 httpie-3.2.2/extras/man/
+-rw-r--r--   0 jakub      (501) staff       (20)    14728 2023-05-19 19:11:41.000000 httpie-3.2.2/extras/man/http.1
+-rw-r--r--   0 jakub      (501) staff       (20)     2352 2023-05-19 19:11:41.000000 httpie-3.2.2/extras/man/httpie.1
+-rw-r--r--   0 jakub      (501) staff       (20)    14731 2023-05-19 19:11:41.000000 httpie-3.2.2/extras/man/https.1
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.147056 httpie-3.2.2/httpie/
+-rw-r--r--   0 jakub      (501) staff       (20)      178 2023-05-19 21:29:36.000000 httpie-3.2.2/httpie/__init__.py
+-rw-r--r--   0 jakub      (501) staff       (20)      394 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/__main__.py
+-rw-r--r--   0 jakub      (501) staff       (20)      448 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/adapters.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.149166 httpie-3.2.2/httpie/cli/
+-rw-r--r--   0 jakub      (501) staff       (20)        0 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/cli/__init__.py
+-rw-r--r--   0 jakub      (501) staff       (20)    23136 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/cli/argparser.py
+-rw-r--r--   0 jakub      (501) staff       (20)     7991 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/cli/argtypes.py
+-rw-r--r--   0 jakub      (501) staff       (20)     3246 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/cli/constants.py
+-rw-r--r--   0 jakub      (501) staff       (20)    28690 2023-05-19 20:23:49.000000 httpie-3.2.2/httpie/cli/definition.py
+-rw-r--r--   0 jakub      (501) staff       (20)     2317 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/cli/dicts.py
+-rw-r--r--   0 jakub      (501) staff       (20)       38 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/cli/exceptions.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.149755 httpie-3.2.2/httpie/cli/nested_json/
+-rw-r--r--   0 jakub      (501) staff       (20)      497 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/cli/nested_json/__init__.py
+-rw-r--r--   0 jakub      (501) staff       (20)      745 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/cli/nested_json/errors.py
+-rw-r--r--   0 jakub      (501) staff       (20)     4341 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/cli/nested_json/interpret.py
+-rw-r--r--   0 jakub      (501) staff       (20)     5431 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/cli/nested_json/parse.py
+-rw-r--r--   0 jakub      (501) staff       (20)     1912 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/cli/nested_json/tokens.py
+-rw-r--r--   0 jakub      (501) staff       (20)     7732 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/cli/options.py
+-rw-r--r--   0 jakub      (501) staff       (20)     7546 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/cli/requestitems.py
+-rw-r--r--   0 jakub      (501) staff       (20)     2151 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/cli/utils.py
+-rw-r--r--   0 jakub      (501) staff       (20)    13126 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/client.py
+-rw-r--r--   0 jakub      (501) staff       (20)     3500 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/compat.py
+-rw-r--r--   0 jakub      (501) staff       (20)     5005 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/config.py
+-rw-r--r--   0 jakub      (501) staff       (20)     6739 2023-05-19 19:25:58.000000 httpie-3.2.2/httpie/context.py
+-rw-r--r--   0 jakub      (501) staff       (20)     1069 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/cookies.py
+-rw-r--r--   0 jakub      (501) staff       (20)    10450 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/core.py
+-rw-r--r--   0 jakub      (501) staff       (20)    11805 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/downloads.py
+-rw-r--r--   0 jakub      (501) staff       (20)     1385 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/encoding.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.150316 httpie-3.2.2/httpie/internal/
+-rw-r--r--   0 jakub      (501) staff       (20)       22 2023-05-19 21:40:38.000000 httpie-3.2.2/httpie/internal/__build_channel__.py
+-rw-r--r--   0 jakub      (501) staff       (20)        0 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/internal/__init__.py
+-rw-r--r--   0 jakub      (501) staff       (20)     1521 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/internal/daemon_runner.py
+-rw-r--r--   0 jakub      (501) staff       (20)     3403 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/internal/daemons.py
+-rw-r--r--   0 jakub      (501) staff       (20)     5178 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/internal/update_warnings.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.150675 httpie-3.2.2/httpie/legacy/
+-rw-r--r--   0 jakub      (501) staff       (20)        0 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/legacy/__init__.py
+-rw-r--r--   0 jakub      (501) staff       (20)     2905 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/legacy/v3_1_0_session_cookie_format.py
+-rw-r--r--   0 jakub      (501) staff       (20)     2078 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/legacy/v3_2_0_session_header_format.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.151273 httpie-3.2.2/httpie/manager/
+-rw-r--r--   0 jakub      (501) staff       (20)        0 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/manager/__init__.py
+-rw-r--r--   0 jakub      (501) staff       (20)     1707 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/manager/__main__.py
+-rw-r--r--   0 jakub      (501) staff       (20)     5371 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/manager/cli.py
+-rw-r--r--   0 jakub      (501) staff       (20)     2001 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/manager/compat.py
+-rw-r--r--   0 jakub      (501) staff       (20)     1142 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/manager/core.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.151968 httpie-3.2.2/httpie/manager/tasks/
+-rw-r--r--   0 jakub      (501) staff       (20)      384 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/manager/tasks/__init__.py
+-rw-r--r--   0 jakub      (501) staff       (20)      362 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/manager/tasks/check_updates.py
+-rw-r--r--   0 jakub      (501) staff       (20)      701 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/manager/tasks/export_args.py
+-rw-r--r--   0 jakub      (501) staff       (20)     8526 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/manager/tasks/plugins.py
+-rw-r--r--   0 jakub      (501) staff       (20)     2686 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/manager/tasks/sessions.py
+-rw-r--r--   0 jakub      (501) staff       (20)     6347 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/models.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.152739 httpie-3.2.2/httpie/output/
+-rw-r--r--   0 jakub      (501) staff       (20)        0 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/output/__init__.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.153353 httpie-3.2.2/httpie/output/formatters/
+-rw-r--r--   0 jakub      (501) staff       (20)        0 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/output/formatters/__init__.py
+-rw-r--r--   0 jakub      (501) staff       (20)    13002 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/output/formatters/colors.py
+-rw-r--r--   0 jakub      (501) staff       (20)      552 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/output/formatters/headers.py
+-rw-r--r--   0 jakub      (501) staff       (20)     1123 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/output/formatters/json.py
+-rw-r--r--   0 jakub      (501) staff       (20)     2505 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/output/formatters/xml.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.154030 httpie-3.2.2/httpie/output/lexers/
+-rw-r--r--   0 jakub      (501) staff       (20)        0 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/output/lexers/__init__.py
+-rw-r--r--   0 jakub      (501) staff       (20)      517 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/output/lexers/common.py
+-rw-r--r--   0 jakub      (501) staff       (20)     3044 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/output/lexers/http.py
+-rw-r--r--   0 jakub      (501) staff       (20)      851 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/output/lexers/json.py
+-rw-r--r--   0 jakub      (501) staff       (20)     1672 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/output/lexers/metadata.py
+-rw-r--r--   0 jakub      (501) staff       (20)     1400 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/output/models.py
+-rw-r--r--   0 jakub      (501) staff       (20)     1763 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/output/processing.py
+-rw-r--r--   0 jakub      (501) staff       (20)     8155 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/output/streams.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.154926 httpie-3.2.2/httpie/output/ui/
+-rw-r--r--   0 jakub      (501) staff       (20)        0 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/output/ui/__init__.py
+-rw-r--r--   0 jakub      (501) staff       (20)     1276 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/output/ui/man_pages.py
+-rw-r--r--   0 jakub      (501) staff       (20)     7226 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/output/ui/palette.py
+-rw-r--r--   0 jakub      (501) staff       (20)     6565 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/output/ui/rich_help.py
+-rw-r--r--   0 jakub      (501) staff       (20)     2294 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/output/ui/rich_palette.py
+-rw-r--r--   0 jakub      (501) staff       (20)     3980 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/output/ui/rich_progress.py
+-rw-r--r--   0 jakub      (501) staff       (20)      973 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/output/ui/rich_utils.py
+-rw-r--r--   0 jakub      (501) staff       (20)     1066 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/output/utils.py
+-rw-r--r--   0 jakub      (501) staff       (20)     6515 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/output/writer.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.155575 httpie-3.2.2/httpie/plugins/
+-rw-r--r--   0 jakub      (501) staff       (20)      299 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/plugins/__init__.py
+-rw-r--r--   0 jakub      (501) staff       (20)     4529 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/plugins/base.py
+-rw-r--r--   0 jakub      (501) staff       (20)     2123 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/plugins/builtin.py
+-rw-r--r--   0 jakub      (501) staff       (20)     4049 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/plugins/manager.py
+-rw-r--r--   0 jakub      (501) staff       (20)      560 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/plugins/registry.py
+-rw-r--r--   0 jakub      (501) staff       (20)     9705 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/sessions.py
+-rw-r--r--   0 jakub      (501) staff       (20)     3287 2023-05-19 20:16:48.000000 httpie-3.2.2/httpie/ssl_.py
+-rw-r--r--   0 jakub      (501) staff       (20)      987 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/status.py
+-rw-r--r--   0 jakub      (501) staff       (20)     7744 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/uploads.py
+-rw-r--r--   0 jakub      (501) staff       (20)     9147 2023-05-19 19:11:41.000000 httpie-3.2.2/httpie/utils.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.147697 httpie-3.2.2/httpie.egg-info/
+-rw-r--r--   0 jakub      (501) staff       (20)     6069 2023-05-19 21:40:41.000000 httpie-3.2.2/httpie.egg-info/PKG-INFO
+-rw-r--r--   0 jakub      (501) staff       (20)     9005 2023-05-19 21:40:41.000000 httpie-3.2.2/httpie.egg-info/SOURCES.txt
+-rw-r--r--   0 jakub      (501) staff       (20)        1 2023-05-19 21:40:41.000000 httpie-3.2.2/httpie.egg-info/dependency_links.txt
+-rw-r--r--   0 jakub      (501) staff       (20)      113 2023-05-19 21:40:41.000000 httpie-3.2.2/httpie.egg-info/entry_points.txt
+-rw-r--r--   0 jakub      (501) staff       (20)      574 2023-05-19 21:40:41.000000 httpie-3.2.2/httpie.egg-info/requires.txt
+-rw-r--r--   0 jakub      (501) staff       (20)        7 2023-05-19 21:40:41.000000 httpie-3.2.2/httpie.egg-info/top_level.txt
+-rw-r--r--   0 jakub      (501) staff       (20)      217 2023-05-19 21:40:41.181322 httpie-3.2.2/setup.cfg
+-rw-r--r--   0 jakub      (501) staff       (20)     3283 2023-05-19 19:11:41.000000 httpie-3.2.2/setup.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.160982 httpie-3.2.2/tests/
+-rw-r--r--   0 jakub      (501) staff       (20)      150 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/README.md
+-rw-r--r--   0 jakub      (501) staff       (20)        0 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/__init__.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.169072 httpie-3.2.2/tests/__pycache__/
+-rw-r--r--   0 jakub      (501) staff       (20)      151 2023-05-19 21:32:49.000000 httpie-3.2.2/tests/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)     4216 2023-05-19 21:32:49.000000 httpie-3.2.2/tests/__pycache__/conftest.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    28700 2023-05-19 21:32:49.000000 httpie-3.2.2/tests/__pycache__/test_auth.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    21564 2023-05-19 21:32:49.000000 httpie-3.2.2/tests/__pycache__/test_auth_plugins.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)     9935 2023-05-19 21:32:49.000000 httpie-3.2.2/tests/__pycache__/test_binary.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    70391 2023-05-19 21:32:49.000000 httpie-3.2.2/tests/__pycache__/test_cli.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)     3898 2023-05-19 21:32:49.000000 httpie-3.2.2/tests/__pycache__/test_cli_ui.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)     3757 2023-05-19 21:32:49.000000 httpie-3.2.2/tests/__pycache__/test_cli_utils.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    22263 2023-05-19 21:32:49.000000 httpie-3.2.2/tests/__pycache__/test_compress.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    17375 2023-05-19 21:32:49.000000 httpie-3.2.2/tests/__pycache__/test_config.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)     4473 2023-05-19 21:32:49.000000 httpie-3.2.2/tests/__pycache__/test_cookie.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    15170 2023-05-19 21:32:49.000000 httpie-3.2.2/tests/__pycache__/test_cookie_on_redirects.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    30163 2023-05-19 21:32:49.000000 httpie-3.2.2/tests/__pycache__/test_defaults.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    31002 2023-05-19 21:32:49.000000 httpie-3.2.2/tests/__pycache__/test_downloads.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    34771 2023-05-19 21:32:49.000000 httpie-3.2.2/tests/__pycache__/test_encoding.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    11969 2023-05-19 21:32:50.000000 httpie-3.2.2/tests/__pycache__/test_errors.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    18735 2023-05-19 21:32:50.000000 httpie-3.2.2/tests/__pycache__/test_exit_status.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    63500 2023-05-19 21:32:50.000000 httpie-3.2.2/tests/__pycache__/test_httpie.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    23438 2023-05-19 21:32:50.000000 httpie-3.2.2/tests/__pycache__/test_httpie_cli.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    24508 2023-05-19 21:32:50.000000 httpie-3.2.2/tests/__pycache__/test_json.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)     3596 2023-05-19 21:32:50.000000 httpie-3.2.2/tests/__pycache__/test_meta.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    12336 2023-05-19 21:32:50.000000 httpie-3.2.2/tests/__pycache__/test_offline.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    80142 2023-05-19 21:32:50.000000 httpie-3.2.2/tests/__pycache__/test_output.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)     3621 2023-05-19 21:32:50.000000 httpie-3.2.2/tests/__pycache__/test_parser_schema.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    26627 2023-05-19 21:32:50.000000 httpie-3.2.2/tests/__pycache__/test_plugins_cli.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    21133 2023-05-19 21:32:50.000000 httpie-3.2.2/tests/__pycache__/test_redirects.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)     5626 2023-05-19 21:32:50.000000 httpie-3.2.2/tests/__pycache__/test_regressions.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    89851 2023-05-19 21:32:50.000000 httpie-3.2.2/tests/__pycache__/test_sessions.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    24650 2023-05-19 21:32:50.000000 httpie-3.2.2/tests/__pycache__/test_ssl.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    17060 2023-05-19 21:32:50.000000 httpie-3.2.2/tests/__pycache__/test_stream.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    10284 2023-05-19 21:32:50.000000 httpie-3.2.2/tests/__pycache__/test_tokens.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)     4692 2023-05-19 21:32:50.000000 httpie-3.2.2/tests/__pycache__/test_transport_plugin.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    25101 2023-05-19 21:32:50.000000 httpie-3.2.2/tests/__pycache__/test_update_warnings.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    64627 2023-05-19 21:32:50.000000 httpie-3.2.2/tests/__pycache__/test_uploads.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)     3161 2023-05-19 21:32:50.000000 httpie-3.2.2/tests/__pycache__/test_windows.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)     7515 2023-05-19 21:32:50.000000 httpie-3.2.2/tests/__pycache__/test_xml.cpython-311-pytest-7.3.1.pyc
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.169731 httpie-3.2.2/tests/client_certs/
+-rw-r--r--   0 jakub      (501) staff       (20)     1939 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/client_certs/client.crt
+-rw-r--r--   0 jakub      (501) staff       (20)     3243 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/client_certs/client.key
+-rw-r--r--   0 jakub      (501) staff       (20)     5182 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/client_certs/client.pem
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.170039 httpie-3.2.2/tests/client_certs/password_protected/
+-rw-r--r--   0 jakub      (501) staff       (20)     2546 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/client_certs/password_protected/client.key
+-rw-r--r--   0 jakub      (501) staff       (20)     1594 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/client_certs/password_protected/client.pem
+-rw-r--r--   0 jakub      (501) staff       (20)     2359 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/conftest.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.171149 httpie-3.2.2/tests/fixtures/
+-rw-r--r--   0 jakub      (501) staff       (20)      109 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/.editorconfig
+-rw-r--r--   0 jakub      (501) staff       (20)     2091 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/__init__.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.171286 httpie-3.2.2/tests/fixtures/__pycache__/
+-rw-r--r--   0 jakub      (501) staff       (20)     3613 2023-05-19 21:32:49.000000 httpie-3.2.2/tests/fixtures/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.141324 httpie-3.2.2/tests/fixtures/session_data/
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.172799 httpie-3.2.2/tests/fixtures/session_data/new/
+-rw-r--r--   0 jakub      (501) staff       (20)      668 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/session_data/new/cookies_dict.json
+-rw-r--r--   0 jakub      (501) staff       (20)      668 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/session_data/new/cookies_dict_dev_version.json
+-rw-r--r--   0 jakub      (501) staff       (20)      811 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/session_data/new/cookies_dict_with_extras.json
+-rw-r--r--   0 jakub      (501) staff       (20)      283 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/session_data/new/empty_cookies_dict.json
+-rw-r--r--   0 jakub      (501) staff       (20)      283 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/session_data/new/empty_cookies_list.json
+-rw-r--r--   0 jakub      (501) staff       (20)      283 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/session_data/new/empty_headers_dict.json
+-rw-r--r--   0 jakub      (501) staff       (20)      283 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/session_data/new/empty_headers_list.json
+-rw-r--r--   0 jakub      (501) staff       (20)      829 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/session_data/new/headers_cookies_dict_mixed.json
+-rw-r--r--   0 jakub      (501) staff       (20)      438 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/session_data/new/headers_dict.json
+-rw-r--r--   0 jakub      (501) staff       (20)      803 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/session_data/new/headers_dict_extras.json
+-rw-r--r--   0 jakub      (501) staff       (20)      438 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/session_data/new/headers_list.json
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.174284 httpie-3.2.2/tests/fixtures/session_data/old/
+-rw-r--r--   0 jakub      (501) staff       (20)      558 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/session_data/old/cookies_dict.json
+-rw-r--r--   0 jakub      (501) staff       (20)      563 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/session_data/old/cookies_dict_dev_version.json
+-rw-r--r--   0 jakub      (501) staff       (20)      701 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/session_data/old/cookies_dict_with_extras.json
+-rw-r--r--   0 jakub      (501) staff       (20)      277 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/session_data/old/empty_cookies_dict.json
+-rw-r--r--   0 jakub      (501) staff       (20)      277 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/session_data/old/empty_cookies_list.json
+-rw-r--r--   0 jakub      (501) staff       (20)      277 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/session_data/old/empty_headers_dict.json
+-rw-r--r--   0 jakub      (501) staff       (20)      277 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/session_data/old/empty_headers_list.json
+-rw-r--r--   0 jakub      (501) staff       (20)      613 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/session_data/old/headers_cookies_dict_mixed.json
+-rw-r--r--   0 jakub      (501) staff       (20)      326 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/session_data/old/headers_dict.json
+-rw-r--r--   0 jakub      (501) staff       (20)      691 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/session_data/old/headers_dict_extras.json
+-rw-r--r--   0 jakub      (501) staff       (20)      438 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/session_data/old/headers_list.json
+-rw-r--r--   0 jakub      (501) staff       (20)     1150 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/test.bin
+-rw-r--r--   0 jakub      (501) staff       (20)      168 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/test.json
+-rw-r--r--   0 jakub      (501) staff       (20)      211 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/test.txt
+-rw-r--r--   0 jakub      (501) staff       (20)       36 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/test_with_dupe_keys.json
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.141610 httpie-3.2.2/tests/fixtures/xmldata/
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.175583 httpie-3.2.2/tests/fixtures/xmldata/invalid/
+-rw-r--r--   0 jakub      (501) staff       (20)       81 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/invalid/cyclic.xml
+-rw-r--r--   0 jakub      (501) staff       (20)      102 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/invalid/external.xml
+-rw-r--r--   0 jakub      (501) staff       (20)      104 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/invalid/external_file.xml
+-rw-r--r--   0 jakub      (501) staff       (20)       11 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/invalid/not-xml.xml
+-rw-r--r--   0 jakub      (501) staff       (20)   103050 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/invalid/quadratic.xml
+-rw-r--r--   0 jakub      (501) staff       (20)      875 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/invalid/xalan_exec.xsl
+-rw-r--r--   0 jakub      (501) staff       (20)      695 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/invalid/xalan_write.xsl
+-rw-r--r--   0 jakub      (501) staff       (20)      183 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/invalid/xmlbomb.xml
+-rw-r--r--   0 jakub      (501) staff       (20)       88 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/invalid/xmlbomb2.xml
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.177361 httpie-3.2.2/tests/fixtures/xmldata/valid/
+-rw-r--r--   0 jakub      (501) staff       (20)      179 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/valid/custom-header.xml
+-rw-r--r--   0 jakub      (501) staff       (20)      177 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/valid/custom-header_formatted.xml
+-rw-r--r--   0 jakub      (501) staff       (20)      210 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/valid/dtd_formatted.xml
+-rw-r--r--   0 jakub      (501) staff       (20)      198 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/valid/dtd_raw.xml
+-rw-r--r--   0 jakub      (501) staff       (20)      152 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/valid/simple-ns_formatted.xml
+-rw-r--r--   0 jakub      (501) staff       (20)      137 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/valid/simple-ns_raw.xml
+-rw-r--r--   0 jakub      (501) staff       (20)        5 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/valid/simple-single-tag_formatted.xml
+-rw-r--r--   0 jakub      (501) staff       (20)        8 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/valid/simple-single-tag_raw.xml
+-rw-r--r--   0 jakub      (501) staff       (20)       87 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/valid/simple-standalone-no_formatted.xml
+-rw-r--r--   0 jakub      (501) staff       (20)       86 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/valid/simple-standalone-no_raw.xml
+-rw-r--r--   0 jakub      (501) staff       (20)       88 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/valid/simple-standalone-yes_formatted.xml
+-rw-r--r--   0 jakub      (501) staff       (20)       87 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/valid/simple-standalone-yes_raw.xml
+-rw-r--r--   0 jakub      (501) staff       (20)      122 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/valid/simple_formatted.xml
+-rw-r--r--   0 jakub      (501) staff       (20)      108 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/valid/simple_raw.xml
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.177781 httpie-3.2.2/tests/fixtures/xmldata/xhtml/
+-rw-r--r--   0 jakub      (501) staff       (20)      986 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/xhtml/xhtml_formatted.xml
+-rw-r--r--   0 jakub      (501) staff       (20)      986 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/xhtml/xhtml_formatted_python_less_than_3.8.xml
+-rw-r--r--   0 jakub      (501) staff       (20)      942 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/fixtures/xmldata/xhtml/xhtml_raw.xml
+-rw-r--r--   0 jakub      (501) staff       (20)     5176 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_auth.py
+-rw-r--r--   0 jakub      (501) staff       (20)     3689 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_auth_plugins.py
+-rw-r--r--   0 jakub      (501) staff       (20)     1986 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_binary.py
+-rw-r--r--   0 jakub      (501) staff       (20)    14285 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_cli.py
+-rw-r--r--   0 jakub      (501) staff       (20)     2025 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_cli_ui.py
+-rw-r--r--   0 jakub      (501) staff       (20)     2322 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_cli_utils.py
+-rw-r--r--   0 jakub      (501) staff       (20)     3882 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_compress.py
+-rw-r--r--   0 jakub      (501) staff       (20)     3773 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_config.py
+-rw-r--r--   0 jakub      (501) staff       (20)     1876 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_cookie.py
+-rw-r--r--   0 jakub      (501) staff       (20)     7191 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_cookie_on_redirects.py
+-rw-r--r--   0 jakub      (501) staff       (20)     4908 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_defaults.py
+-rw-r--r--   0 jakub      (501) staff       (20)     9739 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_downloads.py
+-rw-r--r--   0 jakub      (501) staff       (20)     6761 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_encoding.py
+-rw-r--r--   0 jakub      (501) staff       (20)     2392 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_errors.py
+-rw-r--r--   0 jakub      (501) staff       (20)     2678 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_exit_status.py
+-rw-r--r--   0 jakub      (501) staff       (20)    10076 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_httpie.py
+-rw-r--r--   0 jakub      (501) staff       (20)     4403 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_httpie_cli.py
+-rw-r--r--   0 jakub      (501) staff       (20)    18699 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_json.py
+-rw-r--r--   0 jakub      (501) staff       (20)      570 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_meta.py
+-rw-r--r--   0 jakub      (501) staff       (20)     1979 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_offline.py
+-rw-r--r--   0 jakub      (501) staff       (20)    20821 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_output.py
+-rw-r--r--   0 jakub      (501) staff       (20)     2085 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_parser_schema.py
+-rw-r--r--   0 jakub      (501) staff       (20)     5784 2023-05-19 21:28:50.000000 httpie-3.2.2/tests/test_plugins_cli.py
+-rw-r--r--   0 jakub      (501) staff       (20)     3580 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_redirects.py
+-rw-r--r--   0 jakub      (501) staff       (20)     1159 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_regressions.py
+-rw-r--r--   0 jakub      (501) staff       (20)    27603 2023-05-19 21:37:53.000000 httpie-3.2.2/tests/test_sessions.py
+-rw-r--r--   0 jakub      (501) staff       (20)     7357 2023-05-19 20:16:48.000000 httpie-3.2.2/tests/test_ssl.py
+-rw-r--r--   0 jakub      (501) staff       (20)     4523 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_stream.py
+-rw-r--r--   0 jakub      (501) staff       (20)     3992 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_tokens.py
+-rw-r--r--   0 jakub      (501) staff       (20)     1229 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_transport_plugin.py
+-rw-r--r--   0 jakub      (501) staff       (20)     6608 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_update_warnings.py
+-rw-r--r--   0 jakub      (501) staff       (20)    12899 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_uploads.py
+-rw-r--r--   0 jakub      (501) staff       (20)      956 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_windows.py
+-rw-r--r--   0 jakub      (501) staff       (20)     2869 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/test_xml.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.178435 httpie-3.2.2/tests/utils/
+-rw-r--r--   0 jakub      (501) staff       (20)    12983 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/utils/__init__.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.179212 httpie-3.2.2/tests/utils/__pycache__/
+-rw-r--r--   0 jakub      (501) staff       (20)    22192 2023-05-19 21:32:49.000000 httpie-3.2.2/tests/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    10260 2023-05-19 21:32:49.000000 httpie-3.2.2/tests/utils/__pycache__/http_server.cpython-311.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)    14010 2023-05-19 21:32:49.000000 httpie-3.2.2/tests/utils/__pycache__/plugins_cli.cpython-311.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)     4482 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/utils/http_server.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.179930 httpie-3.2.2/tests/utils/matching/
+-rw-r--r--   0 jakub      (501) staff       (20)     1004 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/utils/matching/__init__.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2023-05-19 21:40:41.180828 httpie-3.2.2/tests/utils/matching/__pycache__/
+-rw-r--r--   0 jakub      (501) staff       (20)     1618 2023-05-19 21:32:50.000000 httpie-3.2.2/tests/utils/matching/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)     4378 2023-05-19 21:32:50.000000 httpie-3.2.2/tests/utils/matching/__pycache__/parsing.cpython-311.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)     8225 2023-05-19 21:32:50.000000 httpie-3.2.2/tests/utils/matching/__pycache__/test_matching.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)     1675 2023-05-19 21:32:50.000000 httpie-3.2.2/tests/utils/matching/__pycache__/tokens.cpython-311.pyc
+-rw-r--r--   0 jakub      (501) staff       (20)     2596 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/utils/matching/parsing.py
+-rw-r--r--   0 jakub      (501) staff       (20)     5827 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/utils/matching/test_matching.py
+-rw-r--r--   0 jakub      (501) staff       (20)     1106 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/utils/matching/tokens.py
+-rw-r--r--   0 jakub      (501) staff       (20)     6572 2023-05-19 19:11:41.000000 httpie-3.2.2/tests/utils/plugins_cli.py
```

### Comparing `httpie-3.2.1/AUTHORS.md` & `httpie-3.2.2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/CHANGELOG.md` & `httpie-3.2.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Change Log
 
 This document records all notable changes to [HTTPie](https://httpie.io).
 This project adheres to [Semantic Versioning](https://semver.org/).
 
+## [3.2.2](https://github.com/httpie/httpie/compare/3.2.1...3.2.2) (2022-05-19)
+
+- Fixed compatibility with urllib3 2.0.0. ([#1499](https://github.com/httpie/httpie/issue/1499))
+
 ## [3.2.1](https://github.com/httpie/httpie/compare/3.1.0...3.2.1) (2022-05-06)
 
 - Improved support for determining auto-streaming when the `Content-Type` header includes encoding information. ([#1383](https://github.com/httpie/httpie/pull/1383))
 - Fixed the display of the crash happening in the secondary process for update checks. ([#1388](https://github.com/httpie/httpie/issues/1388))
 
 ## [3.2.0](https://github.com/httpie/httpie/compare/3.1.0...3.2.0) (2022-05-05)
```

### Comparing `httpie-3.2.1/LICENSE` & `httpie-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/PKG-INFO` & `httpie-3.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: httpie
-Version: 3.2.1
+Version: 3.2.2
 Summary: HTTPie: modern, user-friendly command-line HTTP client for the API era.
 Home-page: https://httpie.io/
-Download-URL: https://github.com/httpie/httpie/archive/3.2.1.tar.gz
+Download-URL: https://github.com/httpie/httpie/archive/3.2.2.tar.gz
 Author: Jakub Roztocil
 Author-email: jakub@roztocil.co
 License: BSD
 Project-URL: GitHub, https://github.com/httpie/httpie
 Project-URL: Twitter, https://twitter.com/httpie
 Project-URL: Discord, https://httpie.io/discord
 Project-URL: Documentation, https://httpie.io/docs
 Project-URL: Online Demo, https://httpie.io/run
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
@@ -29,38 +28,58 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS.md
 
-<br/>
-<a href="https://httpie.io" target="blank_">
-    <img height="100" alt="HTTPie" src="https://raw.githubusercontent.com/httpie/httpie/master/docs/httpie-logo.svg" />
-</a>
-<br/>
+<h2 align="center">
+    <a href="https://httpie.io" target="blank_">
+        <img height="100" alt="HTTPie" src="https://raw.githubusercontent.com/httpie/httpie/master/docs/httpie-logo.svg" />
+    </a>
+    <br>
+    HTTPie for Terminal: human-friendly CLI HTTP client for the API era
+</h2>
+
+<div align="center">
+
+[![HTTPie for Desktop](https://img.shields.io/static/v1?label=HTTPie&message=for%20Desktop&color=4B78E6)](https://httpie.io/product)
+[![](https://img.shields.io/static/v1?label=HTTPie&message=for%20Web%20%26%20Mobile&color=73DC8C)](https://httpie.io/app)
+[![](https://img.shields.io/static/v1?label=HTTPie&message=for%20Terminal&color=FA9BFA)](https://httpie.io/cli)
+[![Twitter](https://img.shields.io/twitter/follow/httpie?style=flat&color=%234B78E6&logoColor=%234B78E6)](https://twitter.com/httpie)
+[![Chat](https://img.shields.io/discord/725351238698270761?style=flat&label=Chat%20on%20Discord&color=%23FA9BFA)](https://httpie.io/discord)
+
+</div>
+
+
+<div align="center">
 
-# HTTPie: human-friendly CLI HTTP client for the API era
+[![Docs](https://img.shields.io/badge/stable%20docs-httpie.io%2Fdocs%2Fcli-brightgreen?style=flat&color=%2373DC8C&label=Docs)](https://httpie.org/docs/cli)
+[![Latest version](https://img.shields.io/pypi/v/httpie.svg?style=flat&label=Latest&color=%234B78E6&logo=&logoColor=white)](https://pypi.python.org/pypi/httpie)
+[![Build](https://img.shields.io/github/actions/workflow/status/httpie/httpie/tests.yml?branch=master&color=%23FA9BFA&label=Build)](https://github.com/httpie/httpie/actions)
+[![Coverage](https://img.shields.io/codecov/c/github/httpie/httpie?style=flat&label=Coverage&color=%2373DC8C)](https://codecov.io/gh/httpie/httpie)
+
+</div>
 
 HTTPie (pronounced _aitch-tee-tee-pie_) is a command-line HTTP client.
 Its goal is to make CLI interaction with web services as human-friendly as possible.
 HTTPie is designed for testing, debugging, and generally interacting with APIs & HTTP servers.
 The `http` & `https` commands allow for creating and sending arbitrary HTTP requests.
 They use simple and natural syntax and provide formatted and colorized output.
 
-[![Docs](https://img.shields.io/badge/stable%20docs-httpie.io%2Fdocs-brightgreen?style=flat&color=%2373DC8C&label=Docs)](https://httpie.org/docs)
-[![Latest version](https://img.shields.io/pypi/v/httpie.svg?style=flat&label=Latest&color=%234B78E6&logo=&logoColor=white)](https://pypi.python.org/pypi/httpie)
-[![Build](https://img.shields.io/github/workflow/status/httpie/httpie/Build?color=%23FA9BFA&label=Build)](https://github.com/httpie/httpie/actions)
-[![Coverage](https://img.shields.io/codecov/c/github/httpie/httpie?style=flat&label=Coverage&color=%2373DC8C)](https://codecov.io/gh/httpie/httpie)
-[![Twitter](https://img.shields.io/twitter/follow/httpie?style=flat&color=%234B78E6&logoColor=%234B78E6)](https://twitter.com/httpie)
-[![Chat](https://img.shields.io/badge/chat-Discord-brightgreen?style=flat&label=Chat%20on&color=%23FA9BFA)](https://httpie.io/discord)
+<div align="center">
 
 <img src="https://raw.githubusercontent.com/httpie/httpie/master/docs/httpie-animation.gif" alt="HTTPie in action" width="100%"/>
 
 
+</div>
+
+
+
+
 ## We lost 54k GitHub stars
 
 Please note we recently accidentally made this repo private for a moment, and GitHub deleted our community that took a decade to build. Read the full story here: https://httpie.io/blog/stardust
 
 ![](docs/stardust.png)
 
 
@@ -84,33 +103,33 @@
 [See all features →](https://httpie.io/docs)
 
 ## Examples
 
 Hello World:
 
 ```bash
-$ https httpie.io/hello
+https httpie.io/hello
 ```
 
 Custom [HTTP method](https://httpie.io/docs#http-method), [HTTP headers](https://httpie.io/docs#http-headers) and [JSON](https://httpie.io/docs#json) data:
 
 ```bash
-$ http PUT pie.dev/put X-API-Token:123 name=John
+http PUT pie.dev/put X-API-Token:123 name=John
 ```
 
 Build and print a request without sending it using [offline mode](https://httpie.io/docs#offline-mode):
 
 ```bash
-$ http --offline pie.dev/post hello=offline
+http --offline pie.dev/post hello=offline
 ```
 
 Use [GitHub API](https://developer.github.com/v3/issues/comments/#create-a-comment) to post a comment on an [Issue](https://github.com/httpie/httpie/issues/83) with [authentication](https://httpie.io/docs#authentication):
 
 ```bash
-$ http -a USERNAME POST https://api.github.com/repos/httpie/httpie/issues/83/comments body='HTTPie is awesome! :heart:'
+http -a USERNAME POST https://api.github.com/repos/httpie/httpie/issues/83/comments body='HTTPie is awesome! :heart:'
 ```
 
 [See more examples →](https://httpie.io/docs#examples)
 
 ## Community & support
 
 - Visit the [HTTPie website](https://httpie.io) for full documentation and useful links.
@@ -121,9 +140,7 @@
 - Subscribe to the [HTTPie newsletter](https://httpie.io) for occasional updates.
 
 ## Contributing
 
 Have a look through existing [Issues](https://github.com/httpie/httpie/issues) and [Pull Requests](https://github.com/httpie/httpie/pulls) that you could help with. If you'd like to request a feature or report a bug, please [create a GitHub Issue](https://github.com/httpie/httpie/issues) using one of the templates provided.
 
 [See contribution guide →](https://github.com/httpie/httpie/blob/master/CONTRIBUTING.md)
-
-
```

#### html2text {}

```diff
@@ -1,71 +1,82 @@
-Metadata-Version: 2.1 Name: httpie Version: 3.2.1 Summary: HTTPie: modern,
+Metadata-Version: 2.1 Name: httpie Version: 3.2.2 Summary: HTTPie: modern,
 user-friendly command-line HTTP client for the API era. Home-page: https://
-httpie.io/ Download-URL: https://github.com/httpie/httpie/archive/3.2.1.tar.gz
+httpie.io/ Download-URL: https://github.com/httpie/httpie/archive/3.2.2.tar.gz
 Author: Jakub Roztocil Author-email: jakub@roztocil.co License: BSD Project-
 URL: GitHub, https://github.com/httpie/httpie Project-URL: Twitter, https://
 twitter.com/httpie Project-URL: Discord, https://httpie.io/discord Project-URL:
 Documentation, https://httpie.io/docs Project-URL: Online Demo, https://
-httpie.io/run Platform: UNKNOWN Classifier: Development Status :: 5 -
-Production/Stable Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 :: Only Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-System Administrators Classifier: License :: OSI Approved :: BSD License
-Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic :: Software
-Development Classifier: Topic :: System :: Networking Classifier: Topic ::
-Terminals Classifier: Topic :: Text Processing Classifier: Topic :: Utilities
-Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
-dev Provides-Extra: test License-File: LICENSE License-File: AUTHORS.md
-[HTTPie]
-# HTTPie: human-friendly CLI HTTP client for the API era HTTPie (pronounced
-_aitch-tee-tee-pie_) is a command-line HTTP client. Its goal is to make CLI
-interaction with web services as human-friendly as possible. HTTPie is designed
-for testing, debugging, and generally interacting with APIs & HTTP servers. The
-`http` & `https` commands allow for creating and sending arbitrary HTTP
-requests. They use simple and natural syntax and provide formatted and
-colorized output. [![Docs](https://img.shields.io/badge/stable%20docs-
-httpie.io%2Fdocs-brightgreen?style=flat&color=%2373DC8C&label=Docs)](https://
-httpie.org/docs) [![Latest version](https://img.shields.io/pypi/v/
-httpie.svg?style=flat&label=Latest&color=%234B78E6&logo=&logoColor=white)]
+httpie.io/run Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 :: Only Classifier: Environment :: Console Classifier: Intended
+Audience :: Developers Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: BSD License Classifier: Topic ::
+Internet :: WWW/HTTP Classifier: Topic :: Software Development Classifier:
+Topic :: System :: Networking Classifier: Topic :: Terminals Classifier: Topic
+:: Text Processing Classifier: Topic :: Utilities Requires-Python: >=3.7
+Description-Content-Type: text/markdown Provides-Extra: dev Provides-Extra:
+test License-File: LICENSE License-File: AUTHORS.md
+                                ***** [HTTPie]
+   HTTPie for Terminal: human-friendly CLI HTTP client for the API era *****
+             [![HTTPie for Desktop](https://img.shields.io/static/
+v1?label=HTTPie&message=for%20Desktop&color=4B78E6)](https://httpie.io/product)
+                      [![](https://img.shields.io/static/
+   v1?label=HTTPie&message=for%20Web%20%26%20Mobile&color=73DC8C)](https://
+              httpie.io/app) [![](https://img.shields.io/static/
+v1?label=HTTPie&message=for%20Terminal&color=FA9BFA)](https://httpie.io/cli) [!
+               [Twitter](https://img.shields.io/twitter/follow/
+ httpie?style=flat&color=%234B78E6&logoColor=%234B78E6)](https://twitter.com/
+               httpie) [![Chat](https://img.shields.io/discord/
+   725351238698270761?style=flat&label=Chat%20on%20Discord&color=%23FA9BFA)]
+                          (https://httpie.io/discord)
+  [![Docs](https://img.shields.io/badge/stable%20docs-httpie.io%2Fdocs%2Fcli-
+ brightgreen?style=flat&color=%2373DC8C&label=Docs)](https://httpie.org/docs/
+            cli) [![Latest version](https://img.shields.io/pypi/v/
+  httpie.svg?style=flat&label=Latest&color=%234B78E6&logo=&logoColor=white)]
 (https://pypi.python.org/pypi/httpie) [![Build](https://img.shields.io/github/
-workflow/status/httpie/httpie/Build?color=%23FA9BFA&label=Build)](https://
-github.com/httpie/httpie/actions) [![Coverage](https://img.shields.io/codecov/
-c/github/httpie/httpie?style=flat&label=Coverage&color=%2373DC8C)](https://
-codecov.io/gh/httpie/httpie) [![Twitter](https://img.shields.io/twitter/follow/
-httpie?style=flat&color=%234B78E6&logoColor=%234B78E6)](https://twitter.com/
-httpie) [![Chat](https://img.shields.io/badge/chat-Discord-
-brightgreen?style=flat&label=Chat%20on&color=%23FA9BFA)](https://httpie.io/
-discord) [HTTPie in action] ## We lost 54k GitHub stars Please note we recently
-accidentally made this repo private for a moment, and GitHub deleted our
-community that took a decade to build. Read the full story here: https://
-httpie.io/blog/stardust ![](docs/stardust.png) ## Getting started -
-[Installation instructions â](https://httpie.io/docs#installation) - [Full
-documentation â](https://httpie.io/docs) ## Features - Expressive and
-intuitive syntax - Formatted and colorized terminal output - Built-in JSON
-support - Forms and file uploads - HTTPS, proxies, and authentication -
-Arbitrary request data - Custom headers - Persistent sessions - `wget`-like
-downloads [See all features â](https://httpie.io/docs) ## Examples Hello
-World: ```bash $ https httpie.io/hello ``` Custom [HTTP method](https://
-httpie.io/docs#http-method), [HTTP headers](https://httpie.io/docs#http-
-headers) and [JSON](https://httpie.io/docs#json) data: ```bash $ http PUT
-pie.dev/put X-API-Token:123 name=John ``` Build and print a request without
-sending it using [offline mode](https://httpie.io/docs#offline-mode): ```bash $
-http --offline pie.dev/post hello=offline ``` Use [GitHub API](https://
-developer.github.com/v3/issues/comments/#create-a-comment) to post a comment on
-an [Issue](https://github.com/httpie/httpie/issues/83) with [authentication]
-(https://httpie.io/docs#authentication): ```bash $ http -a USERNAME POST https:
-//api.github.com/repos/httpie/httpie/issues/83/comments body='HTTPie is
-awesome! :heart:' ``` [See more examples â](https://httpie.io/docs#examples)
-## Community & support - Visit the [HTTPie website](https://httpie.io) for full
-documentation and useful links. - Join our [Discord server](https://httpie.io/
-discord) is to ask questions, discuss features, and for general API chat. -
-Tweet at [@httpie](https://twitter.com/httpie) on Twitter. - Use
-[StackOverflow](https://stackoverflow.com/questions/tagged/httpie) to ask
-questions and include a `httpie` tag. - Create [GitHub Issues](https://
-github.com/httpie/httpie/issues) for bug reports and feature requests. -
-Subscribe to the [HTTPie newsletter](https://httpie.io) for occasional updates.
-## Contributing Have a look through existing [Issues](https://github.com/
-httpie/httpie/issues) and [Pull Requests](https://github.com/httpie/httpie/
-pulls) that you could help with. If you'd like to request a feature or report a
-bug, please [create a GitHub Issue](https://github.com/httpie/httpie/issues)
-using one of the templates provided. [See contribution guide â](https://
-github.com/httpie/httpie/blob/master/CONTRIBUTING.md)
+                    actions/workflow/status/httpie/httpie/
+   tests.yml?branch=master&color=%23FA9BFA&label=Build)](https://github.com/
+ httpie/httpie/actions) [![Coverage](https://img.shields.io/codecov/c/github/
+ httpie/httpie?style=flat&label=Coverage&color=%2373DC8C)](https://codecov.io/
+                               gh/httpie/httpie)
+HTTPie (pronounced _aitch-tee-tee-pie_) is a command-line HTTP client. Its goal
+is to make CLI interaction with web services as human-friendly as possible.
+HTTPie is designed for testing, debugging, and generally interacting with APIs
+& HTTP servers. The `http` & `https` commands allow for creating and sending
+arbitrary HTTP requests. They use simple and natural syntax and provide
+formatted and colorized output.
+                              [HTTPie in action]
+## We lost 54k GitHub stars Please note we recently accidentally made this repo
+private for a moment, and GitHub deleted our community that took a decade to
+build. Read the full story here: https://httpie.io/blog/stardust ![](docs/
+stardust.png) ## Getting started - [Installation instructions â](https://
+httpie.io/docs#installation) - [Full documentation â](https://httpie.io/docs)
+## Features - Expressive and intuitive syntax - Formatted and colorized
+terminal output - Built-in JSON support - Forms and file uploads - HTTPS,
+proxies, and authentication - Arbitrary request data - Custom headers -
+Persistent sessions - `wget`-like downloads [See all features â](https://
+httpie.io/docs) ## Examples Hello World: ```bash https httpie.io/hello ```
+Custom [HTTP method](https://httpie.io/docs#http-method), [HTTP headers](https:
+//httpie.io/docs#http-headers) and [JSON](https://httpie.io/docs#json) data:
+```bash http PUT pie.dev/put X-API-Token:123 name=John ``` Build and print a
+request without sending it using [offline mode](https://httpie.io/docs#offline-
+mode): ```bash http --offline pie.dev/post hello=offline ``` Use [GitHub API]
+(https://developer.github.com/v3/issues/comments/#create-a-comment) to post a
+comment on an [Issue](https://github.com/httpie/httpie/issues/83) with
+[authentication](https://httpie.io/docs#authentication): ```bash http -
+a USERNAME POST https://api.github.com/repos/httpie/httpie/issues/83/comments
+body='HTTPie is awesome! :heart:' ``` [See more examples â](https://
+httpie.io/docs#examples) ## Community & support - Visit the [HTTPie website]
+(https://httpie.io) for full documentation and useful links. - Join our
+[Discord server](https://httpie.io/discord) is to ask questions, discuss
+features, and for general API chat. - Tweet at [@httpie](https://twitter.com/
+httpie) on Twitter. - Use [StackOverflow](https://stackoverflow.com/questions/
+tagged/httpie) to ask questions and include a `httpie` tag. - Create [GitHub
+Issues](https://github.com/httpie/httpie/issues) for bug reports and feature
+requests. - Subscribe to the [HTTPie newsletter](https://httpie.io) for
+occasional updates. ## Contributing Have a look through existing [Issues]
+(https://github.com/httpie/httpie/issues) and [Pull Requests](https://
+github.com/httpie/httpie/pulls) that you could help with. If you'd like to
+request a feature or report a bug, please [create a GitHub Issue](https://
+github.com/httpie/httpie/issues) using one of the templates provided. [See
+contribution guide â](https://github.com/httpie/httpie/blob/master/
+CONTRIBUTING.md)
```

### Comparing `httpie-3.2.1/README.md` & `httpie-3.2.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,51 @@
-<br/>
-<a href="https://httpie.io" target="blank_">
-    <img height="100" alt="HTTPie" src="https://raw.githubusercontent.com/httpie/httpie/master/docs/httpie-logo.svg" />
-</a>
-<br/>
+<h2 align="center">
+    <a href="https://httpie.io" target="blank_">
+        <img height="100" alt="HTTPie" src="https://raw.githubusercontent.com/httpie/httpie/master/docs/httpie-logo.svg" />
+    </a>
+    <br>
+    HTTPie for Terminal: human-friendly CLI HTTP client for the API era
+</h2>
+
+<div align="center">
+
+[![HTTPie for Desktop](https://img.shields.io/static/v1?label=HTTPie&message=for%20Desktop&color=4B78E6)](https://httpie.io/product)
+[![](https://img.shields.io/static/v1?label=HTTPie&message=for%20Web%20%26%20Mobile&color=73DC8C)](https://httpie.io/app)
+[![](https://img.shields.io/static/v1?label=HTTPie&message=for%20Terminal&color=FA9BFA)](https://httpie.io/cli)
+[![Twitter](https://img.shields.io/twitter/follow/httpie?style=flat&color=%234B78E6&logoColor=%234B78E6)](https://twitter.com/httpie)
+[![Chat](https://img.shields.io/discord/725351238698270761?style=flat&label=Chat%20on%20Discord&color=%23FA9BFA)](https://httpie.io/discord)
+
+</div>
+
+
+<div align="center">
+
+[![Docs](https://img.shields.io/badge/stable%20docs-httpie.io%2Fdocs%2Fcli-brightgreen?style=flat&color=%2373DC8C&label=Docs)](https://httpie.org/docs/cli)
+[![Latest version](https://img.shields.io/pypi/v/httpie.svg?style=flat&label=Latest&color=%234B78E6&logo=&logoColor=white)](https://pypi.python.org/pypi/httpie)
+[![Build](https://img.shields.io/github/actions/workflow/status/httpie/httpie/tests.yml?branch=master&color=%23FA9BFA&label=Build)](https://github.com/httpie/httpie/actions)
+[![Coverage](https://img.shields.io/codecov/c/github/httpie/httpie?style=flat&label=Coverage&color=%2373DC8C)](https://codecov.io/gh/httpie/httpie)
 
-# HTTPie: human-friendly CLI HTTP client for the API era
+</div>
 
 HTTPie (pronounced _aitch-tee-tee-pie_) is a command-line HTTP client.
 Its goal is to make CLI interaction with web services as human-friendly as possible.
 HTTPie is designed for testing, debugging, and generally interacting with APIs & HTTP servers.
 The `http` & `https` commands allow for creating and sending arbitrary HTTP requests.
 They use simple and natural syntax and provide formatted and colorized output.
 
-[![Docs](https://img.shields.io/badge/stable%20docs-httpie.io%2Fdocs-brightgreen?style=flat&color=%2373DC8C&label=Docs)](https://httpie.org/docs)
-[![Latest version](https://img.shields.io/pypi/v/httpie.svg?style=flat&label=Latest&color=%234B78E6&logo=&logoColor=white)](https://pypi.python.org/pypi/httpie)
-[![Build](https://img.shields.io/github/workflow/status/httpie/httpie/Build?color=%23FA9BFA&label=Build)](https://github.com/httpie/httpie/actions)
-[![Coverage](https://img.shields.io/codecov/c/github/httpie/httpie?style=flat&label=Coverage&color=%2373DC8C)](https://codecov.io/gh/httpie/httpie)
-[![Twitter](https://img.shields.io/twitter/follow/httpie?style=flat&color=%234B78E6&logoColor=%234B78E6)](https://twitter.com/httpie)
-[![Chat](https://img.shields.io/badge/chat-Discord-brightgreen?style=flat&label=Chat%20on&color=%23FA9BFA)](https://httpie.io/discord)
+<div align="center">
 
 <img src="https://raw.githubusercontent.com/httpie/httpie/master/docs/httpie-animation.gif" alt="HTTPie in action" width="100%"/>
 
 
+</div>
+
+
+
+
 ## We lost 54k GitHub stars
 
 Please note we recently accidentally made this repo private for a moment, and GitHub deleted our community that took a decade to build. Read the full story here: https://httpie.io/blog/stardust
 
 ![](docs/stardust.png)
 
 
@@ -49,33 +69,33 @@
 [See all features →](https://httpie.io/docs)
 
 ## Examples
 
 Hello World:
 
 ```bash
-$ https httpie.io/hello
+https httpie.io/hello
 ```
 
 Custom [HTTP method](https://httpie.io/docs#http-method), [HTTP headers](https://httpie.io/docs#http-headers) and [JSON](https://httpie.io/docs#json) data:
 
 ```bash
-$ http PUT pie.dev/put X-API-Token:123 name=John
+http PUT pie.dev/put X-API-Token:123 name=John
 ```
 
 Build and print a request without sending it using [offline mode](https://httpie.io/docs#offline-mode):
 
 ```bash
-$ http --offline pie.dev/post hello=offline
+http --offline pie.dev/post hello=offline
 ```
 
 Use [GitHub API](https://developer.github.com/v3/issues/comments/#create-a-comment) to post a comment on an [Issue](https://github.com/httpie/httpie/issues/83) with [authentication](https://httpie.io/docs#authentication):
 
 ```bash
-$ http -a USERNAME POST https://api.github.com/repos/httpie/httpie/issues/83/comments body='HTTPie is awesome! :heart:'
+http -a USERNAME POST https://api.github.com/repos/httpie/httpie/issues/83/comments body='HTTPie is awesome! :heart:'
 ```
 
 [See more examples →](https://httpie.io/docs#examples)
 
 ## Community & support
 
 - Visit the [HTTPie website](https://httpie.io) for full documentation and useful links.
```

#### html2text {}

```diff
@@ -1,55 +1,65 @@
-
-[HTTPie]
-# HTTPie: human-friendly CLI HTTP client for the API era HTTPie (pronounced
-_aitch-tee-tee-pie_) is a command-line HTTP client. Its goal is to make CLI
-interaction with web services as human-friendly as possible. HTTPie is designed
-for testing, debugging, and generally interacting with APIs & HTTP servers. The
-`http` & `https` commands allow for creating and sending arbitrary HTTP
-requests. They use simple and natural syntax and provide formatted and
-colorized output. [![Docs](https://img.shields.io/badge/stable%20docs-
-httpie.io%2Fdocs-brightgreen?style=flat&color=%2373DC8C&label=Docs)](https://
-httpie.org/docs) [![Latest version](https://img.shields.io/pypi/v/
-httpie.svg?style=flat&label=Latest&color=%234B78E6&logo=&logoColor=white)]
+                                ***** [HTTPie]
+   HTTPie for Terminal: human-friendly CLI HTTP client for the API era *****
+             [![HTTPie for Desktop](https://img.shields.io/static/
+v1?label=HTTPie&message=for%20Desktop&color=4B78E6)](https://httpie.io/product)
+                      [![](https://img.shields.io/static/
+   v1?label=HTTPie&message=for%20Web%20%26%20Mobile&color=73DC8C)](https://
+              httpie.io/app) [![](https://img.shields.io/static/
+v1?label=HTTPie&message=for%20Terminal&color=FA9BFA)](https://httpie.io/cli) [!
+               [Twitter](https://img.shields.io/twitter/follow/
+ httpie?style=flat&color=%234B78E6&logoColor=%234B78E6)](https://twitter.com/
+               httpie) [![Chat](https://img.shields.io/discord/
+   725351238698270761?style=flat&label=Chat%20on%20Discord&color=%23FA9BFA)]
+                          (https://httpie.io/discord)
+  [![Docs](https://img.shields.io/badge/stable%20docs-httpie.io%2Fdocs%2Fcli-
+ brightgreen?style=flat&color=%2373DC8C&label=Docs)](https://httpie.org/docs/
+            cli) [![Latest version](https://img.shields.io/pypi/v/
+  httpie.svg?style=flat&label=Latest&color=%234B78E6&logo=&logoColor=white)]
 (https://pypi.python.org/pypi/httpie) [![Build](https://img.shields.io/github/
-workflow/status/httpie/httpie/Build?color=%23FA9BFA&label=Build)](https://
-github.com/httpie/httpie/actions) [![Coverage](https://img.shields.io/codecov/
-c/github/httpie/httpie?style=flat&label=Coverage&color=%2373DC8C)](https://
-codecov.io/gh/httpie/httpie) [![Twitter](https://img.shields.io/twitter/follow/
-httpie?style=flat&color=%234B78E6&logoColor=%234B78E6)](https://twitter.com/
-httpie) [![Chat](https://img.shields.io/badge/chat-Discord-
-brightgreen?style=flat&label=Chat%20on&color=%23FA9BFA)](https://httpie.io/
-discord) [HTTPie in action] ## We lost 54k GitHub stars Please note we recently
-accidentally made this repo private for a moment, and GitHub deleted our
-community that took a decade to build. Read the full story here: https://
-httpie.io/blog/stardust ![](docs/stardust.png) ## Getting started -
-[Installation instructions â](https://httpie.io/docs#installation) - [Full
-documentation â](https://httpie.io/docs) ## Features - Expressive and
-intuitive syntax - Formatted and colorized terminal output - Built-in JSON
-support - Forms and file uploads - HTTPS, proxies, and authentication -
-Arbitrary request data - Custom headers - Persistent sessions - `wget`-like
-downloads [See all features â](https://httpie.io/docs) ## Examples Hello
-World: ```bash $ https httpie.io/hello ``` Custom [HTTP method](https://
-httpie.io/docs#http-method), [HTTP headers](https://httpie.io/docs#http-
-headers) and [JSON](https://httpie.io/docs#json) data: ```bash $ http PUT
-pie.dev/put X-API-Token:123 name=John ``` Build and print a request without
-sending it using [offline mode](https://httpie.io/docs#offline-mode): ```bash $
-http --offline pie.dev/post hello=offline ``` Use [GitHub API](https://
-developer.github.com/v3/issues/comments/#create-a-comment) to post a comment on
-an [Issue](https://github.com/httpie/httpie/issues/83) with [authentication]
-(https://httpie.io/docs#authentication): ```bash $ http -a USERNAME POST https:
-//api.github.com/repos/httpie/httpie/issues/83/comments body='HTTPie is
-awesome! :heart:' ``` [See more examples â](https://httpie.io/docs#examples)
-## Community & support - Visit the [HTTPie website](https://httpie.io) for full
-documentation and useful links. - Join our [Discord server](https://httpie.io/
-discord) is to ask questions, discuss features, and for general API chat. -
-Tweet at [@httpie](https://twitter.com/httpie) on Twitter. - Use
-[StackOverflow](https://stackoverflow.com/questions/tagged/httpie) to ask
-questions and include a `httpie` tag. - Create [GitHub Issues](https://
-github.com/httpie/httpie/issues) for bug reports and feature requests. -
-Subscribe to the [HTTPie newsletter](https://httpie.io) for occasional updates.
-## Contributing Have a look through existing [Issues](https://github.com/
-httpie/httpie/issues) and [Pull Requests](https://github.com/httpie/httpie/
-pulls) that you could help with. If you'd like to request a feature or report a
-bug, please [create a GitHub Issue](https://github.com/httpie/httpie/issues)
-using one of the templates provided. [See contribution guide â](https://
-github.com/httpie/httpie/blob/master/CONTRIBUTING.md)
+                    actions/workflow/status/httpie/httpie/
+   tests.yml?branch=master&color=%23FA9BFA&label=Build)](https://github.com/
+ httpie/httpie/actions) [![Coverage](https://img.shields.io/codecov/c/github/
+ httpie/httpie?style=flat&label=Coverage&color=%2373DC8C)](https://codecov.io/
+                               gh/httpie/httpie)
+HTTPie (pronounced _aitch-tee-tee-pie_) is a command-line HTTP client. Its goal
+is to make CLI interaction with web services as human-friendly as possible.
+HTTPie is designed for testing, debugging, and generally interacting with APIs
+& HTTP servers. The `http` & `https` commands allow for creating and sending
+arbitrary HTTP requests. They use simple and natural syntax and provide
+formatted and colorized output.
+                              [HTTPie in action]
+## We lost 54k GitHub stars Please note we recently accidentally made this repo
+private for a moment, and GitHub deleted our community that took a decade to
+build. Read the full story here: https://httpie.io/blog/stardust ![](docs/
+stardust.png) ## Getting started - [Installation instructions â](https://
+httpie.io/docs#installation) - [Full documentation â](https://httpie.io/docs)
+## Features - Expressive and intuitive syntax - Formatted and colorized
+terminal output - Built-in JSON support - Forms and file uploads - HTTPS,
+proxies, and authentication - Arbitrary request data - Custom headers -
+Persistent sessions - `wget`-like downloads [See all features â](https://
+httpie.io/docs) ## Examples Hello World: ```bash https httpie.io/hello ```
+Custom [HTTP method](https://httpie.io/docs#http-method), [HTTP headers](https:
+//httpie.io/docs#http-headers) and [JSON](https://httpie.io/docs#json) data:
+```bash http PUT pie.dev/put X-API-Token:123 name=John ``` Build and print a
+request without sending it using [offline mode](https://httpie.io/docs#offline-
+mode): ```bash http --offline pie.dev/post hello=offline ``` Use [GitHub API]
+(https://developer.github.com/v3/issues/comments/#create-a-comment) to post a
+comment on an [Issue](https://github.com/httpie/httpie/issues/83) with
+[authentication](https://httpie.io/docs#authentication): ```bash http -
+a USERNAME POST https://api.github.com/repos/httpie/httpie/issues/83/comments
+body='HTTPie is awesome! :heart:' ``` [See more examples â](https://
+httpie.io/docs#examples) ## Community & support - Visit the [HTTPie website]
+(https://httpie.io) for full documentation and useful links. - Join our
+[Discord server](https://httpie.io/discord) is to ask questions, discuss
+features, and for general API chat. - Tweet at [@httpie](https://twitter.com/
+httpie) on Twitter. - Use [StackOverflow](https://stackoverflow.com/questions/
+tagged/httpie) to ask questions and include a `httpie` tag. - Create [GitHub
+Issues](https://github.com/httpie/httpie/issues) for bug reports and feature
+requests. - Subscribe to the [HTTPie newsletter](https://httpie.io) for
+occasional updates. ## Contributing Have a look through existing [Issues]
+(https://github.com/httpie/httpie/issues) and [Pull Requests](https://
+github.com/httpie/httpie/pulls) that you could help with. If you'd like to
+request a feature or report a bug, please [create a GitHub Issue](https://
+github.com/httpie/httpie/issues) using one of the templates provided. [See
+contribution guide â](https://github.com/httpie/httpie/blob/master/
+CONTRIBUTING.md)
```

### Comparing `httpie-3.2.1/docs/README.md` & `httpie-3.2.2/docs/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -211,14 +211,29 @@
 ```
 
 ```bash
 # Upgrade httpie
 $ pacman -Syu
 ```
 
+#### Single binary executables
+
+Get the standalone HTTPie Linux executables when you don't want to go through the full installation process
+
+```bash
+# Install httpie
+$ https --download packages.httpie.io/binaries/linux/http-latest -o http
+$ chmod +x ./http
+```
+
+```bash
+# Upgrade httpie
+$ https --download packages.httpie.io/binaries/linux/http-latest -o http
+```
+
 ### FreeBSD
 
 #### FreshPorts
 
 ```bash
 # Install httpie
 $ pkg install www/py-httpie
@@ -231,44 +246,47 @@
 
 <!-- /GENERATED SECTION -->
 
 </div>
 
 ### Unstable version
 
-You can also install the latest unreleased development version directly from the `master` branch on GitHub.
-It is a work-in-progress of a future stable release so the experience might be not as smooth.
+If you want to try out the latest version of HTTPie that hasn't been officially released yet, you can install the development or unstable version directly from the master branch on GitHub. However, keep in mind that the development version is a work in progress and may not be as reliable as the stable version.
 
-You can install it on Linux, macOS, Windows, or FreeBSD with `pip`:
+You can use the following command to install the development version of HTTPie on Linux, macOS, Windows, or FreeBSD operating systems. With this command, the code present in the `master` branch is downloaded and installed using `pip`.
 
 ```bash
 $ python -m pip install --upgrade https://github.com/httpie/httpie/archive/master.tar.gz
 ```
 
-Or on macOS, and Linux, with Homebrew:
+There are other ways to install the development version of HTTPie on macOS and Linux.
+
+You can install it using Homebrew by running the following commands:
 
 ```bash
 $ brew uninstall --force httpie
 $ brew install --HEAD httpie
 ```
 
-And even on macOS, and Linux, with Snapcraft:
+You can install it using Snapcraft by running the following commands:
 
 ```bash
 $ snap remove httpie
 $ snap install httpie --edge
 ```
 
-Verify that now you have the [current development version identifier](https://github.com/httpie/httpie/blob/master/httpie/__init__.py#L6) with the `.dev0` suffix, for example:
+To verify the installation, you can compare the [version identifier on GitHub](https://github.com/httpie/httpie/blob/master/httpie/__init__.py#L6) with the one available on your machine. You can check the version of HTTPie on your machine by using the command `http --version`.
 
 ```bash
 $ http --version
 # 3.X.X.dev0
 ```
 
+Note that on your machine, the version name will have the `.dev0` suffix.
+
 ## Usage
 
 Hello World:
 
 ```bash
 $ https httpie.io/hello
 ```
@@ -1434,15 +1452,16 @@
 
 ```bash
 $ http --proxy=http:http://user:pass@10.10.1.10:3128 example.org
 ```
 
 ### Environment variables
 
-You can also configure proxies by environment variables `ALL_PROXY`, `HTTP_PROXY` and `HTTPS_PROXY`, and the underlying [Requests library](https://python-requests.org/) will pick them up.
+You can also configure proxies by environment variables `ALL_PROXY`, `HTTP_PROXY` and `HTTPS_PROXY`, and the underlying
+[Requests library](https://requests.readthedocs.io/en/latest/) will pick them up.
 If you want to disable proxies configured through the environment variables for certain hosts, you can specify them in `NO_PROXY`.
 
 In your `~/.bash_profile`:
 
 ```bash
 export HTTP_PROXY=http://10.10.1.10:3128
 export HTTPS_PROXY=https://10.10.1.10:1080
@@ -2375,20 +2394,17 @@
 ```
 
 ### Best practices
 
 The default behavior of automatically reading `stdin` is typically not desirable during non-interactive invocations.
 You most likely want to use the `--ignore-stdin` option to disable it.
 
-It is a common *gotcha* that without this option HTTPie seemingly hangs.
-What happens is that when HTTPie is invoked, for example, from a cron job, `stdin` is not connected to a terminal.
-Therefore, the rules for [redirected input](#redirected-input) apply, i.e. HTTPie starts to read it expecting that the request body will be passed through.
-And since there’s neither data nor `EOF`, it will get stuck. So unless you’re piping some data to HTTPie, the `--ignore-stdin` flag should be used in scripts.
+It's important to note that without the `--ignore-stdin` option, HTTPie may appear to have stopped working (hang). This happens because, in situations where HTTPie is invoked outside of an interactive session, such as from a cron job, `stdin` is not connected to a terminal. This means that the rules for [redirected input](#redirected-input) will be followed. When `stdin` is redirected, HTTPie assumes that the input will contain the request body, and it waits for the input to be provided. But, since there is neither any input data nor an end-of-file (`EOF`) signal, HTTPie gets stuck. To avoid this problem, the `--ignore-stdin` flag should be used in scripts, unless data is being piped to HTTPie.
 
-Also, it might be good to set a connection `--timeout` limit to prevent your program from hanging if the server never responds.
+To prevent your program from becoming unresponsive when the server fails to respond, it's a good idea to use the `--timeout` option to set a connection timeout limit.
 
 ## Plugin manager
 
 HTTPie offers extensibility through a [plugin API](https://github.com/httpie/httpie/blob/master/httpie/plugins/base.py),
 and there are dozens of plugins available to try!
 They add things like new authentication methods ([akamai/httpie-edgegrid](https://github.com/akamai/httpie-edgegrid)),
 transport mechanisms ([httpie/httpie-unixsocket](https://github.com/httpie/httpie-unixsocket)),
@@ -2406,15 +2422,15 @@
 
 #### `httpie cli check-updates`
 
 You can check whether a new update is available for your system by running `httpie cli check-updates`:
 
 ```bash-termible
 $ httpie cli check-updates
-````
+```
 
 #### `httpie cli export-args`
 
 `httpie cli export-args` command can expose the parser specification of `http`/`https` commands
 (like an API definition) to outside tools so that they can use this to build better interactions
 over them (e.g., offer auto-complete).
 
@@ -2534,15 +2550,15 @@
 
 ### Related projects
 
 #### Dependencies
 
 Under the hood, HTTPie uses these two amazing libraries:
 
-- [Requests](https://python-requests.org) — Python HTTP library for humans
+- [Requests](https://requests.readthedocs.io/en/latest/) — Python HTTP library for humans
 - [Pygments](https://pygments.org/) — Python syntax highlighter
 
 #### HTTPie friends
 
 HTTPie plays exceptionally well with the following tools:
 
 - [http-prompt](https://github.com/httpie/http-prompt) — an interactive shell for HTTPie featuring autocomplete and command syntax highlighting
```

### Comparing `httpie-3.2.1/extras/man/http.1` & `httpie-3.2.2/extras/man/http.1`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/extras/man/httpie.1` & `httpie-3.2.2/extras/man/httpie.1`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/extras/man/https.1` & `httpie-3.2.2/extras/man/https.1`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/cli/argparser.py` & `httpie-3.2.2/httpie/cli/argparser.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/cli/argtypes.py` & `httpie-3.2.2/httpie/cli/argtypes.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/cli/constants.py` & `httpie-3.2.2/httpie/cli/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -128,14 +128,7 @@
 OUTPUT_OPTIONS_DEFAULT_OFFLINE = OUT_REQ_HEAD + OUT_REQ_BODY
 
 
 class RequestType(enum.Enum):
     FORM = enum.auto()
     MULTIPART = enum.auto()
     JSON = enum.auto()
-
-
-EMPTY_STRING = ''
-OPEN_BRACKET = '['
-CLOSE_BRACKET = ']'
-BACKSLASH = '\\'
-HIGHLIGHTER = '^'
```

### Comparing `httpie-3.2.1/httpie/cli/definition.py` & `httpie-3.2.2/httpie/cli/definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
                                   SORTED_FORMAT_OPTIONS_STRING,
                                   UNSORTED_FORMAT_OPTIONS_STRING, RequestType)
 from httpie.cli.options import ParserSpec, Qualifiers, to_argparse
 from httpie.output.formatters.colors import (AUTO_STYLE, DEFAULT_STYLE, BUNDLED_STYLES,
                                              get_available_styles)
 from httpie.plugins.builtin import BuiltinAuthPlugin
 from httpie.plugins.registry import plugin_manager
-from httpie.ssl_ import AVAILABLE_SSL_VERSION_ARG_MAPPING, DEFAULT_SSL_CIPHERS
+from httpie.ssl_ import AVAILABLE_SSL_VERSION_ARG_MAPPING, DEFAULT_SSL_CIPHERS_STRING
 
 options = ParserSpec(
     'http',
     description=f'{__doc__.strip()} <https://httpie.io>',
     epilog="""
     For every --OPTION there is also a --no-OPTION that reverts OPTION
     to its default value.
@@ -828,17 +828,17 @@
 )
 ssl.add_argument(
     '--ciphers',
     short_help='A string in the OpenSSL cipher list format.',
     help=f"""
 
     A string in the OpenSSL cipher list format. By default, the following
-    is used:
+    ciphers are used on your system:
 
-    {DEFAULT_SSL_CIPHERS}
+    {DEFAULT_SSL_CIPHERS_STRING}
 
     """,
 )
 ssl.add_argument(
     '--cert',
     default=None,
     type=readable_file_arg,
```

### Comparing `httpie-3.2.1/httpie/cli/dicts.py` & `httpie-3.2.2/httpie/cli/dicts.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,11 +88,7 @@
 
 class MultipartRequestDataDict(MultiValueOrderedDict):
     pass
 
 
 class RequestFilesDict(RequestDataDict):
     pass
-
-
-class NestedJSONArray(list):
-    """Denotes a top-level JSON array."""
```

### Comparing `httpie-3.2.1/httpie/cli/options.py` & `httpie-3.2.2/httpie/cli/options.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/cli/requestitems.py` & `httpie-3.2.2/httpie/cli/requestitems.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .dicts import (
     BaseMultiDict, MultipartRequestDataDict, RequestDataDict,
     RequestFilesDict, HTTPHeadersDict, RequestJSONDataDict,
     RequestQueryParamsDict,
 )
 from .exceptions import ParseError
 from .nested_json import interpret_nested_json
-from ..utils import get_content_type, load_json_preserve_order_and_dupe_keys, split
+from ..utils import get_content_type, load_json_preserve_order_and_dupe_keys, split_iterable
 
 
 class RequestItems:
 
     def __init__(self, request_type: Optional[RequestType] = None):
         self.headers = HTTPHeadersDict()
         self.request_type = request_type
@@ -74,33 +74,36 @@
                 instance.data,
             ),
             SEPARATOR_GROUP_NESTED_JSON_ITEMS: (
                 process_data_nested_json_embed_args,
                 instance.data,
             ),
             SEPARATOR_DATA_RAW_JSON: (
-                json_only(instance, process_data_raw_json_embed_arg),
+                convert_json_value_to_form_if_needed(
+                    in_json_mode=instance.is_json,
+                    processor=process_data_raw_json_embed_arg
+                ),
                 instance.data,
             ),
             SEPARATOR_DATA_EMBED_RAW_JSON_FILE: (
-                json_only(instance, process_data_embed_raw_json_file_arg),
+                convert_json_value_to_form_if_needed(
+                    in_json_mode=instance.is_json,
+                    processor=process_data_embed_raw_json_file_arg,
+                ),
                 instance.data,
             ),
         }
 
         if instance.is_json:
-            json_item_args, request_item_args = split(
-                request_item_args,
-                lambda arg: arg.sep in SEPARATOR_GROUP_NESTED_JSON_ITEMS
+            json_item_args, request_item_args = split_iterable(
+                iterable=request_item_args,
+                key=lambda arg: arg.sep in SEPARATOR_GROUP_NESTED_JSON_ITEMS
             )
             if json_item_args:
-                pairs = [
-                    (arg.key, rules[arg.sep][0](arg))
-                    for arg in json_item_args
-                ]
+                pairs = [(arg.key, rules[arg.sep][0](arg)) for arg in json_item_args]
                 processor_func, target_dict = rules[SEPARATOR_GROUP_NESTED_JSON_ITEMS]
                 value = processor_func(pairs)
                 target_dict.update(value)
 
         # Then handle all other items.
         for arg in request_item_args:
             processor_func, target_dict = rules[arg.sep]
@@ -155,45 +158,46 @@
     return (
         os.path.basename(filename),
         f,
         mime_type or get_content_type(filename),
     )
 
 
-def process_data_item_arg(arg: KeyValueArg) -> str:
-    return arg.value
-
-
-def process_data_embed_file_contents_arg(arg: KeyValueArg) -> str:
-    return load_text_file(arg)
+def convert_json_value_to_form_if_needed(in_json_mode: bool, processor: Callable[[KeyValueArg], JSONType]) -> Callable[[], str]:
+    """
+    We allow primitive values to be passed to forms via JSON key/value syntax.
 
+    But complex values lead to an error because there’s no clear way to serialize them.
 
-def json_only(items: RequestItems, func: Callable[[KeyValueArg], JSONType]) -> str:
-    if items.is_json:
-        return func
+    """
+    if in_json_mode:
+        return processor
 
-    @functools.wraps(func)
+    @functools.wraps(processor)
     def wrapper(*args, **kwargs) -> str:
         try:
-            ret = func(*args, **kwargs)
+            output = processor(*args, **kwargs)
         except ParseError:
-            ret = None
-
-        # If it is a basic type, then allow it
-        if isinstance(ret, (str, int, float)):
-            return str(ret)
+            output = None
+        if isinstance(output, (str, int, float)):
+            return str(output)
         else:
-            raise ParseError(
-                'Can\'t use complex JSON value types with '
-                '--form/--multipart.'
-            )
+            raise ParseError('Cannot use complex JSON value types with --form/--multipart.')
 
     return wrapper
 
 
+def process_data_item_arg(arg: KeyValueArg) -> str:
+    return arg.value
+
+
+def process_data_embed_file_contents_arg(arg: KeyValueArg) -> str:
+    return load_text_file(arg)
+
+
 def process_data_embed_raw_json_file_arg(arg: KeyValueArg) -> JSONType:
     contents = load_text_file(arg)
     value = load_json(arg, contents)
     return value
 
 
 def process_data_raw_json_embed_arg(arg: KeyValueArg) -> JSONType:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `httpie-3.2.1/httpie/cli/utils.py` & `httpie-3.2.2/httpie/cli/utils.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/client.py` & `httpie-3.2.2/httpie/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 from time import monotonic
 from typing import Any, Dict, Callable, Iterable
 from urllib.parse import urlparse, urlunparse
 
 import requests
 # noinspection PyPackageRequirements
 import urllib3
+
 from . import __version__
 from .adapters import HTTPieHTTPAdapter
+from .cli.constants import HTTP_OPTIONS
+from .cli.dicts import HTTPHeadersDict
+from .cli.nested_json import unwrap_top_level_list_if_needed
 from .context import Environment
-from .cli.constants import EMPTY_STRING, HTTP_OPTIONS
-from .cli.dicts import HTTPHeadersDict, NestedJSONArray
 from .encoding import UTF8
 from .models import RequestsMessage
 from .plugins.registry import plugin_manager
 from .sessions import get_httpie_session
 from .ssl_ import AVAILABLE_SSL_VERSION_ARG_MAPPING, HTTPieCertificate, HTTPieHTTPSAdapter
 from .uploads import (
     compress_request, prepare_request_body,
@@ -301,29 +303,21 @@
             'false': False,
         }.get(args.verify.lower(), args.verify),
         'cert': cert,
     }
 
 
 def json_dict_to_request_body(data: Dict[str, Any]) -> str:
-    # Propagate the top-level list if there is only one
-    # item in the object, with an en empty key.
-    if len(data) == 1:
-        [(key, value)] = data.items()
-        if isinstance(value, NestedJSONArray):
-            assert key == EMPTY_STRING
-            data = value
-
+    data = unwrap_top_level_list_if_needed(data)
     if data:
         data = json.dumps(data)
     else:
         # We need to set data to an empty string to prevent requests
         # from assigning an empty list to `response.request.data`.
         data = ''
-
     return data
 
 
 def make_request_kwargs(
     env: Environment,
     args: argparse.Namespace,
     base_headers: HTTPHeadersDict = None,
```

### Comparing `httpie-3.2.1/httpie/compat.py` & `httpie-3.2.2/httpie/compat.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/config.py` & `httpie-3.2.2/httpie/config.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/context.py` & `httpie-3.2.2/httpie/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         config = self._config
         if not config:
             self._config = config = Config(directory=self.config_dir)
             if not config.is_new():
                 try:
                     config.load()
                 except ConfigFileError as e:
-                    self.log_error(e, level='warning')
+                    self.log_error(e, level=LogLevel.WARNING)
         return config
 
     @property
     def devnull(self) -> IO:
         if self._devnull is None:
             self._devnull = open(os.devnull, 'w+')
         return self._devnull
@@ -170,15 +170,15 @@
     def log_error(self, msg: str, level: LogLevel = LogLevel.ERROR) -> None:
         if self.stdout_isatty and self.quiet >= LOG_LEVEL_DISPLAY_THRESHOLDS[level]:
             stderr = self.stderr  # Not directly /dev/null, since stderr might be mocked
         else:
             stderr = self._orig_stderr
         rich_console = self._make_rich_console(file=stderr, force_terminal=stderr.isatty())
         rich_console.print(
-            f'\n{self.program_name}: {level}: {msg}\n\n',
+            f'\n{self.program_name}: {level.value}: {msg}\n\n',
             style=LOG_LEVEL_COLORS[level],
             markup=False,
             highlight=False,
             soft_wrap=True
         )
 
     def apply_warnings_filter(self) -> None:
```

### Comparing `httpie-3.2.1/httpie/cookies.py` & `httpie-3.2.2/httpie/cookies.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/core.py` & `httpie-3.2.2/httpie/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import requests
 from pygments import __version__ as pygments_version
 from requests import __version__ as requests_version
 
 from . import __version__ as httpie_version
 from .cli.constants import OUT_REQ_BODY
-from .cli.nested_json import HTTPieSyntaxError
+from .cli.nested_json import NestedJSONSyntaxError
 from .client import collect_messages
 from .context import Environment, LogLevel
 from .downloads import Downloader
 from .models import (
     RequestsMessageKind,
     OutputOptions
 )
@@ -74,15 +74,15 @@
     exit_status = ExitStatus.SUCCESS
 
     try:
         parsed_args = parser.parse_args(
             args=args,
             env=env,
         )
-    except HTTPieSyntaxError as exc:
+    except NestedJSONSyntaxError as exc:
         env.stderr.write(str(exc) + "\n")
         if include_traceback:
             raise
         exit_status = ExitStatus.ERROR
     except KeyboardInterrupt:
         env.stderr.write('\n')
         if include_traceback:
```

### Comparing `httpie-3.2.1/httpie/downloads.py` & `httpie-3.2.2/httpie/downloads.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/encoding.py` & `httpie-3.2.2/httpie/encoding.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/internal/daemon_runner.py` & `httpie-3.2.2/httpie/internal/daemon_runner.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/internal/daemons.py` & `httpie-3.2.2/httpie/internal/daemons.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 This module provides an interface to spawn a detached task to be
-runned with httpie.internal.daemon_runner on a separate process. It is
+run with httpie.internal.daemon_runner on a separate process. It is
 based on DVC's daemon system.
 https://github.com/iterative/dvc/blob/main/dvc/daemon.py
 """
 
 import inspect
 import os
 import platform
```

### Comparing `httpie-3.2.1/httpie/internal/update_warnings.py` & `httpie-3.2.2/httpie/internal/update_warnings.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/legacy/v3_1_0_session_cookie_format.py` & `httpie-3.2.2/httpie/legacy/v3_1_0_session_cookie_format.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/legacy/v3_2_0_session_header_format.py` & `httpie-3.2.2/httpie/legacy/v3_2_0_session_header_format.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/manager/__main__.py` & `httpie-3.2.2/httpie/manager/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,14 @@
         return ExitStatus.ERROR
 
 
 def program():
     try:
         exit_status = main()
     except KeyboardInterrupt:
-        from httpie.status import ExitStatus
         exit_status = ExitStatus.ERROR_CTRL_C
 
     return exit_status
 
 
 if __name__ == '__main__':  # pragma: nocover
     sys.exit(program())
```

### Comparing `httpie-3.2.1/httpie/manager/cli.py` & `httpie-3.2.2/httpie/manager/cli.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/manager/compat.py` & `httpie-3.2.2/httpie/manager/compat.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,14 @@
         if _check_pip_version(pip_location):
             return pip_location
 
     raise SystemError("Couldn't find 'pip' executable. Please ensure that pip in your system is available.")
 
 
 def _run_pip_subprocess(pip_executable: List[str], args: List[str]) -> bytes:
-    import subprocess
 
     cmd = [*pip_executable, *args]
     try:
         process = subprocess.run(
             cmd,
             check=True,
             shell=False,
```

### Comparing `httpie-3.2.1/httpie/manager/core.py` & `httpie-3.2.2/httpie/manager/core.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/manager/tasks/export_args.py` & `httpie-3.2.2/httpie/manager/tasks/export_args.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/manager/tasks/plugins.py` & `httpie-3.2.2/httpie/manager/tasks/plugins.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/manager/tasks/sessions.py` & `httpie-3.2.2/httpie/manager/tasks/sessions.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/models.py` & `httpie-3.2.2/httpie/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     OUT_RESP_BODY,
     OUT_RESP_HEAD,
     OUT_RESP_META
 )
 from .compat import cached_property
 from .utils import split_cookies, parse_content_type_header
 
-
 ELAPSED_TIME_LABEL = 'Elapsed time'
 
 
 class HTTPMessage:
     """Abstract class for HTTP messages."""
 
     def __init__(self, orig):
@@ -63,35 +62,18 @@
 
     def iter_body(self, chunk_size=1):
         return self._orig.iter_content(chunk_size=chunk_size)
 
     def iter_lines(self, chunk_size):
         return ((line, b'\n') for line in self._orig.iter_lines(chunk_size))
 
-    # noinspection PyProtectedMember
     @property
     def headers(self):
-        try:
-            raw = self._orig.raw
-            if getattr(raw, '_original_response', None):
-                raw_version = raw._original_response.version
-            else:
-                raw_version = raw.version
-        except AttributeError:
-            # Assume HTTP/1.1
-            raw_version = 11
-        version = {
-            9: '0.9',
-            10: '1.0',
-            11: '1.1',
-            20: '2.0',
-        }[raw_version]
-
         original = self._orig
-        status_line = f'HTTP/{version} {original.status_code} {original.reason}'
+        status_line = f'HTTP/{self.version} {original.status_code} {original.reason}'
         headers = [status_line]
         headers.extend(
             ': '.join(header)
             for header in original.headers.items()
             if header[0] != 'Set-Cookie'
         )
         headers.extend(
@@ -113,14 +95,40 @@
         # data['Body time'] = str(round(time_since_headers_parsed, 5)) + 's'
         data[ELAPSED_TIME_LABEL] = str(round(time_elapsed, 10)) + 's'
         return '\n'.join(
             f'{key}: {value}'
             for key, value in data.items()
         )
 
+    @property
+    def version(self) -> str:
+        """
+        Return the HTTP version used by the server, e.g. '1.1'.
+
+        Assume HTTP/1.1 if version is not available.
+
+        """
+        mapping = {
+            9: '0.9',
+            10: '1.0',
+            11: '1.1',
+            20: '2.0',
+        }
+        fallback = 11
+        version = None
+        try:
+            raw = self._orig.raw
+            if getattr(raw, '_original_response', None):
+                version = raw._original_response.version
+            else:
+                version = raw.version
+        except AttributeError:
+            pass
+        return mapping[version or fallback]
+
 
 class HTTPRequest(HTTPMessage):
     """A :class:`requests.models.Request` wrapper."""
 
     def iter_body(self, chunk_size):
         yield self.body
```

### Comparing `httpie-3.2.1/httpie/output/formatters/colors.py` & `httpie-3.2.2/httpie/output/formatters/colors.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/output/formatters/headers.py` & `httpie-3.2.2/httpie/output/formatters/headers.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/output/formatters/json.py` & `httpie-3.2.2/httpie/output/formatters/json.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/output/formatters/xml.py` & `httpie-3.2.2/httpie/output/formatters/xml.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/output/lexers/common.py` & `httpie-3.2.2/httpie/output/lexers/common.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/output/lexers/http.py` & `httpie-3.2.2/httpie/output/lexers/http.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/output/lexers/json.py` & `httpie-3.2.2/httpie/output/lexers/json.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/output/lexers/metadata.py` & `httpie-3.2.2/httpie/output/lexers/metadata.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/output/models.py` & `httpie-3.2.2/httpie/output/models.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/output/processing.py` & `httpie-3.2.2/httpie/output/processing.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/output/streams.py` & `httpie-3.2.2/httpie/output/streams.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/output/ui/man_pages.py` & `httpie-3.2.2/httpie/output/ui/man_pages.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/output/ui/palette.py` & `httpie-3.2.2/httpie/output/ui/palette.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/output/ui/rich_help.py` & `httpie-3.2.2/httpie/output/ui/rich_help.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/output/ui/rich_palette.py` & `httpie-3.2.2/httpie/output/ui/rich_palette.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/output/ui/rich_progress.py` & `httpie-3.2.2/httpie/output/ui/rich_progress.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/output/ui/rich_utils.py` & `httpie-3.2.2/httpie/output/ui/rich_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 @contextmanager
 def enable_highlighter(
     console: Console,
     highlighter: Highlighter,
 ) -> Iterator[Console]:
-    """Enable a higlighter temporarily."""
+    """Enable a highlighter temporarily."""
 
     original_highlighter = console.highlighter
     try:
         console.highlighter = highlighter
         yield console
     finally:
         console.highlighter = original_highlighter
```

### Comparing `httpie-3.2.1/httpie/output/utils.py` & `httpie-3.2.2/httpie/output/utils.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/output/writer.py` & `httpie-3.2.2/httpie/output/writer.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/plugins/base.py` & `httpie-3.2.2/httpie/plugins/base.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/plugins/builtin.py` & `httpie-3.2.2/httpie/plugins/builtin.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/plugins/manager.py` & `httpie-3.2.2/httpie/plugins/manager.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/plugins/registry.py` & `httpie-3.2.2/httpie/plugins/registry.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/sessions.py` & `httpie-3.2.2/httpie/sessions.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/ssl_.py` & `httpie-3.2.2/httpie/ssl_.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import ssl
 from typing import NamedTuple, Optional
 
 from httpie.adapters import HTTPAdapter
 # noinspection PyPackageRequirements
 from urllib3.util.ssl_ import (
-    DEFAULT_CIPHERS, create_urllib3_context,
+    create_urllib3_context,
     resolve_ssl_version,
 )
 
 
-DEFAULT_SSL_CIPHERS = DEFAULT_CIPHERS
 SSL_VERSION_ARG_MAPPING = {
     'ssl2.3': 'PROTOCOL_SSLv23',
     'ssl3': 'PROTOCOL_SSLv3',
     'tls1': 'PROTOCOL_TLSv1',
     'tls1.1': 'PROTOCOL_TLSv1_1',
     'tls1.2': 'PROTOCOL_TLSv1_2',
     'tls1.3': 'PROTOCOL_TLSv1_3',
@@ -77,20 +76,30 @@
             ssl_version=resolve_ssl_version(ssl_version),
             # Since we are using a custom SSL context, we need to pass this
             # here manually, even though it’s also passed to the connection
             # in `super().cert_verify()`.
             cert_reqs=ssl.CERT_REQUIRED if verify else ssl.CERT_NONE
         )
 
+    @classmethod
+    def get_default_ciphers_names(cls):
+        return [cipher['name'] for cipher in cls._create_ssl_context(verify=False).get_ciphers()]
+
 
 def _is_key_file_encrypted(key_file):
     """Detects if a key file is encrypted or not.
 
     Copy of the internal urllib function (urllib3.util.ssl_)"""
 
     with open(key_file, "r") as f:
         for line in f:
             # Look for Proc-Type: 4,ENCRYPTED
             if "ENCRYPTED" in line:
                 return True
 
     return False
+
+
+# We used to import the default set of TLS ciphers from urllib3, but they removed it.
+# Instead, now urllib3 uses the list of ciphers configured by the system.
+# <https://github.com/httpie/httpie/pull/1501>
+DEFAULT_SSL_CIPHERS_STRING = ':'.join(HTTPieHTTPSAdapter.get_default_ciphers_names())
```

### Comparing `httpie-3.2.1/httpie/status.py` & `httpie-3.2.2/httpie/status.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/uploads.py` & `httpie-3.2.2/httpie/uploads.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/httpie/utils.py` & `httpie-3.2.2/httpie/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,15 +241,15 @@
                 path,
                 py_version_short=f'{major}.{minor}'
             )
     else:
         yield as_site(path)
 
 
-def split(iterable: Iterable[T], key: Callable[[T], bool]) -> Tuple[List[T], List[T]]:
+def split_iterable(iterable: Iterable[T], key: Callable[[T], bool]) -> Tuple[List[T], List[T]]:
     left, right = [], []
     for item in iterable:
         if key(item):
             left.append(item)
         else:
             right.append(item)
     return left, right
@@ -273,15 +273,15 @@
 
 @contextmanager
 def open_with_lockfile(file: Path, *args, **kwargs) -> Generator[IO[Any], None, None]:
     file_id = base64.b64encode(os.fsencode(file)).decode()
     target_file = Path(tempfile.gettempdir()) / file_id
 
     # Have an atomic-like touch here, so we'll tighten the possibility of
-    # a race occuring between multiple processes accessing the same file.
+    # a race occurring between multiple processes accessing the same file.
     try:
         target_file.touch(exist_ok=False)
     except FileExistsError as exc:
         raise LockFileError("Can't modify a locked file.") from exc
 
     try:
         with open(file, *args, **kwargs) as stream:
```

### Comparing `httpie-3.2.1/httpie.egg-info/PKG-INFO` & `httpie-3.2.2/httpie.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: httpie
-Version: 3.2.1
+Version: 3.2.2
 Summary: HTTPie: modern, user-friendly command-line HTTP client for the API era.
 Home-page: https://httpie.io/
-Download-URL: https://github.com/httpie/httpie/archive/3.2.1.tar.gz
+Download-URL: https://github.com/httpie/httpie/archive/3.2.2.tar.gz
 Author: Jakub Roztocil
 Author-email: jakub@roztocil.co
 License: BSD
 Project-URL: GitHub, https://github.com/httpie/httpie
 Project-URL: Twitter, https://twitter.com/httpie
 Project-URL: Discord, https://httpie.io/discord
 Project-URL: Documentation, https://httpie.io/docs
 Project-URL: Online Demo, https://httpie.io/run
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
@@ -29,38 +28,58 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS.md
 
-<br/>
-<a href="https://httpie.io" target="blank_">
-    <img height="100" alt="HTTPie" src="https://raw.githubusercontent.com/httpie/httpie/master/docs/httpie-logo.svg" />
-</a>
-<br/>
+<h2 align="center">
+    <a href="https://httpie.io" target="blank_">
+        <img height="100" alt="HTTPie" src="https://raw.githubusercontent.com/httpie/httpie/master/docs/httpie-logo.svg" />
+    </a>
+    <br>
+    HTTPie for Terminal: human-friendly CLI HTTP client for the API era
+</h2>
+
+<div align="center">
+
+[![HTTPie for Desktop](https://img.shields.io/static/v1?label=HTTPie&message=for%20Desktop&color=4B78E6)](https://httpie.io/product)
+[![](https://img.shields.io/static/v1?label=HTTPie&message=for%20Web%20%26%20Mobile&color=73DC8C)](https://httpie.io/app)
+[![](https://img.shields.io/static/v1?label=HTTPie&message=for%20Terminal&color=FA9BFA)](https://httpie.io/cli)
+[![Twitter](https://img.shields.io/twitter/follow/httpie?style=flat&color=%234B78E6&logoColor=%234B78E6)](https://twitter.com/httpie)
+[![Chat](https://img.shields.io/discord/725351238698270761?style=flat&label=Chat%20on%20Discord&color=%23FA9BFA)](https://httpie.io/discord)
+
+</div>
+
+
+<div align="center">
 
-# HTTPie: human-friendly CLI HTTP client for the API era
+[![Docs](https://img.shields.io/badge/stable%20docs-httpie.io%2Fdocs%2Fcli-brightgreen?style=flat&color=%2373DC8C&label=Docs)](https://httpie.org/docs/cli)
+[![Latest version](https://img.shields.io/pypi/v/httpie.svg?style=flat&label=Latest&color=%234B78E6&logo=&logoColor=white)](https://pypi.python.org/pypi/httpie)
+[![Build](https://img.shields.io/github/actions/workflow/status/httpie/httpie/tests.yml?branch=master&color=%23FA9BFA&label=Build)](https://github.com/httpie/httpie/actions)
+[![Coverage](https://img.shields.io/codecov/c/github/httpie/httpie?style=flat&label=Coverage&color=%2373DC8C)](https://codecov.io/gh/httpie/httpie)
+
+</div>
 
 HTTPie (pronounced _aitch-tee-tee-pie_) is a command-line HTTP client.
 Its goal is to make CLI interaction with web services as human-friendly as possible.
 HTTPie is designed for testing, debugging, and generally interacting with APIs & HTTP servers.
 The `http` & `https` commands allow for creating and sending arbitrary HTTP requests.
 They use simple and natural syntax and provide formatted and colorized output.
 
-[![Docs](https://img.shields.io/badge/stable%20docs-httpie.io%2Fdocs-brightgreen?style=flat&color=%2373DC8C&label=Docs)](https://httpie.org/docs)
-[![Latest version](https://img.shields.io/pypi/v/httpie.svg?style=flat&label=Latest&color=%234B78E6&logo=&logoColor=white)](https://pypi.python.org/pypi/httpie)
-[![Build](https://img.shields.io/github/workflow/status/httpie/httpie/Build?color=%23FA9BFA&label=Build)](https://github.com/httpie/httpie/actions)
-[![Coverage](https://img.shields.io/codecov/c/github/httpie/httpie?style=flat&label=Coverage&color=%2373DC8C)](https://codecov.io/gh/httpie/httpie)
-[![Twitter](https://img.shields.io/twitter/follow/httpie?style=flat&color=%234B78E6&logoColor=%234B78E6)](https://twitter.com/httpie)
-[![Chat](https://img.shields.io/badge/chat-Discord-brightgreen?style=flat&label=Chat%20on&color=%23FA9BFA)](https://httpie.io/discord)
+<div align="center">
 
 <img src="https://raw.githubusercontent.com/httpie/httpie/master/docs/httpie-animation.gif" alt="HTTPie in action" width="100%"/>
 
 
+</div>
+
+
+
+
 ## We lost 54k GitHub stars
 
 Please note we recently accidentally made this repo private for a moment, and GitHub deleted our community that took a decade to build. Read the full story here: https://httpie.io/blog/stardust
 
 ![](docs/stardust.png)
 
 
@@ -84,33 +103,33 @@
 [See all features →](https://httpie.io/docs)
 
 ## Examples
 
 Hello World:
 
 ```bash
-$ https httpie.io/hello
+https httpie.io/hello
 ```
 
 Custom [HTTP method](https://httpie.io/docs#http-method), [HTTP headers](https://httpie.io/docs#http-headers) and [JSON](https://httpie.io/docs#json) data:
 
 ```bash
-$ http PUT pie.dev/put X-API-Token:123 name=John
+http PUT pie.dev/put X-API-Token:123 name=John
 ```
 
 Build and print a request without sending it using [offline mode](https://httpie.io/docs#offline-mode):
 
 ```bash
-$ http --offline pie.dev/post hello=offline
+http --offline pie.dev/post hello=offline
 ```
 
 Use [GitHub API](https://developer.github.com/v3/issues/comments/#create-a-comment) to post a comment on an [Issue](https://github.com/httpie/httpie/issues/83) with [authentication](https://httpie.io/docs#authentication):
 
 ```bash
-$ http -a USERNAME POST https://api.github.com/repos/httpie/httpie/issues/83/comments body='HTTPie is awesome! :heart:'
+http -a USERNAME POST https://api.github.com/repos/httpie/httpie/issues/83/comments body='HTTPie is awesome! :heart:'
 ```
 
 [See more examples →](https://httpie.io/docs#examples)
 
 ## Community & support
 
 - Visit the [HTTPie website](https://httpie.io) for full documentation and useful links.
@@ -121,9 +140,7 @@
 - Subscribe to the [HTTPie newsletter](https://httpie.io) for occasional updates.
 
 ## Contributing
 
 Have a look through existing [Issues](https://github.com/httpie/httpie/issues) and [Pull Requests](https://github.com/httpie/httpie/pulls) that you could help with. If you'd like to request a feature or report a bug, please [create a GitHub Issue](https://github.com/httpie/httpie/issues) using one of the templates provided.
 
 [See contribution guide →](https://github.com/httpie/httpie/blob/master/CONTRIBUTING.md)
-
-
```

#### html2text {}

```diff
@@ -1,71 +1,82 @@
-Metadata-Version: 2.1 Name: httpie Version: 3.2.1 Summary: HTTPie: modern,
+Metadata-Version: 2.1 Name: httpie Version: 3.2.2 Summary: HTTPie: modern,
 user-friendly command-line HTTP client for the API era. Home-page: https://
-httpie.io/ Download-URL: https://github.com/httpie/httpie/archive/3.2.1.tar.gz
+httpie.io/ Download-URL: https://github.com/httpie/httpie/archive/3.2.2.tar.gz
 Author: Jakub Roztocil Author-email: jakub@roztocil.co License: BSD Project-
 URL: GitHub, https://github.com/httpie/httpie Project-URL: Twitter, https://
 twitter.com/httpie Project-URL: Discord, https://httpie.io/discord Project-URL:
 Documentation, https://httpie.io/docs Project-URL: Online Demo, https://
-httpie.io/run Platform: UNKNOWN Classifier: Development Status :: 5 -
-Production/Stable Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 :: Only Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-System Administrators Classifier: License :: OSI Approved :: BSD License
-Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic :: Software
-Development Classifier: Topic :: System :: Networking Classifier: Topic ::
-Terminals Classifier: Topic :: Text Processing Classifier: Topic :: Utilities
-Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
-dev Provides-Extra: test License-File: LICENSE License-File: AUTHORS.md
-[HTTPie]
-# HTTPie: human-friendly CLI HTTP client for the API era HTTPie (pronounced
-_aitch-tee-tee-pie_) is a command-line HTTP client. Its goal is to make CLI
-interaction with web services as human-friendly as possible. HTTPie is designed
-for testing, debugging, and generally interacting with APIs & HTTP servers. The
-`http` & `https` commands allow for creating and sending arbitrary HTTP
-requests. They use simple and natural syntax and provide formatted and
-colorized output. [![Docs](https://img.shields.io/badge/stable%20docs-
-httpie.io%2Fdocs-brightgreen?style=flat&color=%2373DC8C&label=Docs)](https://
-httpie.org/docs) [![Latest version](https://img.shields.io/pypi/v/
-httpie.svg?style=flat&label=Latest&color=%234B78E6&logo=&logoColor=white)]
+httpie.io/run Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 :: Only Classifier: Environment :: Console Classifier: Intended
+Audience :: Developers Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: BSD License Classifier: Topic ::
+Internet :: WWW/HTTP Classifier: Topic :: Software Development Classifier:
+Topic :: System :: Networking Classifier: Topic :: Terminals Classifier: Topic
+:: Text Processing Classifier: Topic :: Utilities Requires-Python: >=3.7
+Description-Content-Type: text/markdown Provides-Extra: dev Provides-Extra:
+test License-File: LICENSE License-File: AUTHORS.md
+                                ***** [HTTPie]
+   HTTPie for Terminal: human-friendly CLI HTTP client for the API era *****
+             [![HTTPie for Desktop](https://img.shields.io/static/
+v1?label=HTTPie&message=for%20Desktop&color=4B78E6)](https://httpie.io/product)
+                      [![](https://img.shields.io/static/
+   v1?label=HTTPie&message=for%20Web%20%26%20Mobile&color=73DC8C)](https://
+              httpie.io/app) [![](https://img.shields.io/static/
+v1?label=HTTPie&message=for%20Terminal&color=FA9BFA)](https://httpie.io/cli) [!
+               [Twitter](https://img.shields.io/twitter/follow/
+ httpie?style=flat&color=%234B78E6&logoColor=%234B78E6)](https://twitter.com/
+               httpie) [![Chat](https://img.shields.io/discord/
+   725351238698270761?style=flat&label=Chat%20on%20Discord&color=%23FA9BFA)]
+                          (https://httpie.io/discord)
+  [![Docs](https://img.shields.io/badge/stable%20docs-httpie.io%2Fdocs%2Fcli-
+ brightgreen?style=flat&color=%2373DC8C&label=Docs)](https://httpie.org/docs/
+            cli) [![Latest version](https://img.shields.io/pypi/v/
+  httpie.svg?style=flat&label=Latest&color=%234B78E6&logo=&logoColor=white)]
 (https://pypi.python.org/pypi/httpie) [![Build](https://img.shields.io/github/
-workflow/status/httpie/httpie/Build?color=%23FA9BFA&label=Build)](https://
-github.com/httpie/httpie/actions) [![Coverage](https://img.shields.io/codecov/
-c/github/httpie/httpie?style=flat&label=Coverage&color=%2373DC8C)](https://
-codecov.io/gh/httpie/httpie) [![Twitter](https://img.shields.io/twitter/follow/
-httpie?style=flat&color=%234B78E6&logoColor=%234B78E6)](https://twitter.com/
-httpie) [![Chat](https://img.shields.io/badge/chat-Discord-
-brightgreen?style=flat&label=Chat%20on&color=%23FA9BFA)](https://httpie.io/
-discord) [HTTPie in action] ## We lost 54k GitHub stars Please note we recently
-accidentally made this repo private for a moment, and GitHub deleted our
-community that took a decade to build. Read the full story here: https://
-httpie.io/blog/stardust ![](docs/stardust.png) ## Getting started -
-[Installation instructions â](https://httpie.io/docs#installation) - [Full
-documentation â](https://httpie.io/docs) ## Features - Expressive and
-intuitive syntax - Formatted and colorized terminal output - Built-in JSON
-support - Forms and file uploads - HTTPS, proxies, and authentication -
-Arbitrary request data - Custom headers - Persistent sessions - `wget`-like
-downloads [See all features â](https://httpie.io/docs) ## Examples Hello
-World: ```bash $ https httpie.io/hello ``` Custom [HTTP method](https://
-httpie.io/docs#http-method), [HTTP headers](https://httpie.io/docs#http-
-headers) and [JSON](https://httpie.io/docs#json) data: ```bash $ http PUT
-pie.dev/put X-API-Token:123 name=John ``` Build and print a request without
-sending it using [offline mode](https://httpie.io/docs#offline-mode): ```bash $
-http --offline pie.dev/post hello=offline ``` Use [GitHub API](https://
-developer.github.com/v3/issues/comments/#create-a-comment) to post a comment on
-an [Issue](https://github.com/httpie/httpie/issues/83) with [authentication]
-(https://httpie.io/docs#authentication): ```bash $ http -a USERNAME POST https:
-//api.github.com/repos/httpie/httpie/issues/83/comments body='HTTPie is
-awesome! :heart:' ``` [See more examples â](https://httpie.io/docs#examples)
-## Community & support - Visit the [HTTPie website](https://httpie.io) for full
-documentation and useful links. - Join our [Discord server](https://httpie.io/
-discord) is to ask questions, discuss features, and for general API chat. -
-Tweet at [@httpie](https://twitter.com/httpie) on Twitter. - Use
-[StackOverflow](https://stackoverflow.com/questions/tagged/httpie) to ask
-questions and include a `httpie` tag. - Create [GitHub Issues](https://
-github.com/httpie/httpie/issues) for bug reports and feature requests. -
-Subscribe to the [HTTPie newsletter](https://httpie.io) for occasional updates.
-## Contributing Have a look through existing [Issues](https://github.com/
-httpie/httpie/issues) and [Pull Requests](https://github.com/httpie/httpie/
-pulls) that you could help with. If you'd like to request a feature or report a
-bug, please [create a GitHub Issue](https://github.com/httpie/httpie/issues)
-using one of the templates provided. [See contribution guide â](https://
-github.com/httpie/httpie/blob/master/CONTRIBUTING.md)
+                    actions/workflow/status/httpie/httpie/
+   tests.yml?branch=master&color=%23FA9BFA&label=Build)](https://github.com/
+ httpie/httpie/actions) [![Coverage](https://img.shields.io/codecov/c/github/
+ httpie/httpie?style=flat&label=Coverage&color=%2373DC8C)](https://codecov.io/
+                               gh/httpie/httpie)
+HTTPie (pronounced _aitch-tee-tee-pie_) is a command-line HTTP client. Its goal
+is to make CLI interaction with web services as human-friendly as possible.
+HTTPie is designed for testing, debugging, and generally interacting with APIs
+& HTTP servers. The `http` & `https` commands allow for creating and sending
+arbitrary HTTP requests. They use simple and natural syntax and provide
+formatted and colorized output.
+                              [HTTPie in action]
+## We lost 54k GitHub stars Please note we recently accidentally made this repo
+private for a moment, and GitHub deleted our community that took a decade to
+build. Read the full story here: https://httpie.io/blog/stardust ![](docs/
+stardust.png) ## Getting started - [Installation instructions â](https://
+httpie.io/docs#installation) - [Full documentation â](https://httpie.io/docs)
+## Features - Expressive and intuitive syntax - Formatted and colorized
+terminal output - Built-in JSON support - Forms and file uploads - HTTPS,
+proxies, and authentication - Arbitrary request data - Custom headers -
+Persistent sessions - `wget`-like downloads [See all features â](https://
+httpie.io/docs) ## Examples Hello World: ```bash https httpie.io/hello ```
+Custom [HTTP method](https://httpie.io/docs#http-method), [HTTP headers](https:
+//httpie.io/docs#http-headers) and [JSON](https://httpie.io/docs#json) data:
+```bash http PUT pie.dev/put X-API-Token:123 name=John ``` Build and print a
+request without sending it using [offline mode](https://httpie.io/docs#offline-
+mode): ```bash http --offline pie.dev/post hello=offline ``` Use [GitHub API]
+(https://developer.github.com/v3/issues/comments/#create-a-comment) to post a
+comment on an [Issue](https://github.com/httpie/httpie/issues/83) with
+[authentication](https://httpie.io/docs#authentication): ```bash http -
+a USERNAME POST https://api.github.com/repos/httpie/httpie/issues/83/comments
+body='HTTPie is awesome! :heart:' ``` [See more examples â](https://
+httpie.io/docs#examples) ## Community & support - Visit the [HTTPie website]
+(https://httpie.io) for full documentation and useful links. - Join our
+[Discord server](https://httpie.io/discord) is to ask questions, discuss
+features, and for general API chat. - Tweet at [@httpie](https://twitter.com/
+httpie) on Twitter. - Use [StackOverflow](https://stackoverflow.com/questions/
+tagged/httpie) to ask questions and include a `httpie` tag. - Create [GitHub
+Issues](https://github.com/httpie/httpie/issues) for bug reports and feature
+requests. - Subscribe to the [HTTPie newsletter](https://httpie.io) for
+occasional updates. ## Contributing Have a look through existing [Issues]
+(https://github.com/httpie/httpie/issues) and [Pull Requests](https://
+github.com/httpie/httpie/pulls) that you could help with. If you'd like to
+request a feature or report a bug, please [create a GitHub Issue](https://
+github.com/httpie/httpie/issues) using one of the templates provided. [See
+contribution guide â](https://github.com/httpie/httpie/blob/master/
+CONTRIBUTING.md)
```

### Comparing `httpie-3.2.1/httpie.egg-info/requires.txt` & `httpie-3.2.2/httpie.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/setup.py` & `httpie-3.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/client_certs/client.crt` & `httpie-3.2.2/tests/client_certs/client.crt`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/client_certs/client.key` & `httpie-3.2.2/tests/client_certs/client.key`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/client_certs/client.pem` & `httpie-3.2.2/tests/client_certs/client.pem`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/client_certs/password_protected/client.key` & `httpie-3.2.2/tests/client_certs/password_protected/client.key`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/client_certs/password_protected/client.pem` & `httpie-3.2.2/tests/client_certs/password_protected/client.pem`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/conftest.py` & `httpie-3.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/fixtures/__init__.py` & `httpie-3.2.2/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/fixtures/session_data/new/cookies_dict.json` & `httpie-3.2.2/tests/fixtures/session_data/new/cookies_dict.json`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/fixtures/session_data/new/cookies_dict_dev_version.json` & `httpie-3.2.2/tests/fixtures/session_data/new/cookies_dict_dev_version.json`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/fixtures/session_data/new/cookies_dict_with_extras.json` & `httpie-3.2.2/tests/fixtures/session_data/new/cookies_dict_with_extras.json`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/fixtures/session_data/new/headers_cookies_dict_mixed.json` & `httpie-3.2.2/tests/fixtures/session_data/new/headers_cookies_dict_mixed.json`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/fixtures/session_data/new/headers_dict_extras.json` & `httpie-3.2.2/tests/fixtures/session_data/new/headers_dict_extras.json`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/fixtures/session_data/old/cookies_dict.json` & `httpie-3.2.2/tests/fixtures/session_data/old/cookies_dict.json`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/fixtures/session_data/old/cookies_dict_dev_version.json` & `httpie-3.2.2/tests/fixtures/session_data/old/cookies_dict_dev_version.json`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/fixtures/session_data/old/cookies_dict_with_extras.json` & `httpie-3.2.2/tests/fixtures/session_data/old/cookies_dict_with_extras.json`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/fixtures/session_data/old/headers_cookies_dict_mixed.json` & `httpie-3.2.2/tests/fixtures/session_data/old/headers_cookies_dict_mixed.json`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/fixtures/session_data/old/headers_dict_extras.json` & `httpie-3.2.2/tests/fixtures/session_data/old/headers_dict_extras.json`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/fixtures/test.bin` & `httpie-3.2.2/tests/fixtures/test.bin`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/fixtures/xmldata/invalid/quadratic.xml` & `httpie-3.2.2/tests/fixtures/xmldata/invalid/quadratic.xml`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/fixtures/xmldata/invalid/xalan_exec.xsl` & `httpie-3.2.2/tests/fixtures/xmldata/invalid/xalan_exec.xsl`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/fixtures/xmldata/invalid/xalan_write.xsl` & `httpie-3.2.2/tests/fixtures/xmldata/invalid/xalan_write.xsl`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/fixtures/xmldata/xhtml/xhtml_formatted.xml` & `httpie-3.2.2/tests/fixtures/xmldata/xhtml/xhtml_formatted.xml`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/fixtures/xmldata/xhtml/xhtml_formatted_python_less_than_3.8.xml` & `httpie-3.2.2/tests/fixtures/xmldata/xhtml/xhtml_formatted_python_less_than_3.8.xml`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/fixtures/xmldata/xhtml/xhtml_raw.xml` & `httpie-3.2.2/tests/fixtures/xmldata/xhtml/xhtml_raw.xml`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_auth.py` & `httpie-3.2.2/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_auth_plugins.py` & `httpie-3.2.2/tests/test_auth_plugins.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_binary.py` & `httpie-3.2.2/tests/test_binary.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_cli.py` & `httpie-3.2.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_cli_ui.py` & `httpie-3.2.2/tests/test_cli_ui.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_cli_utils.py` & `httpie-3.2.2/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_compress.py` & `httpie-3.2.2/tests/test_compress.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_config.py` & `httpie-3.2.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_cookie.py` & `httpie-3.2.2/tests/test_cookie.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_cookie_on_redirects.py` & `httpie-3.2.2/tests/test_cookie_on_redirects.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_defaults.py` & `httpie-3.2.2/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_downloads.py` & `httpie-3.2.2/tests/test_downloads.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_encoding.py` & `httpie-3.2.2/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_errors.py` & `httpie-3.2.2/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_exit_status.py` & `httpie-3.2.2/tests/test_exit_status.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_httpie.py` & `httpie-3.2.2/tests/test_httpie.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_httpie_cli.py` & `httpie-3.2.2/tests/test_httpie_cli.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_json.py` & `httpie-3.2.2/tests/test_json.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 
 import pytest
 import responses
 
 from httpie.cli.constants import PRETTY_MAP
 from httpie.cli.exceptions import ParseError
-from httpie.cli.nested_json import HTTPieSyntaxError
+from httpie.cli.nested_json import NestedJSONSyntaxError
 from httpie.output.formatters.colors import ColorFormatter
 from httpie.utils import JsonDictPreservingDuplicateKeys
 
 from .fixtures import (
     FILE_CONTENT,
     FILE_PATH,
     JSON_FILE_CONTENT,
@@ -153,15 +153,15 @@
     with pytest.raises(ParseError) as cm:
         http(
             request_type,
             httpbin + '/post',
             f'option:={json.dumps(value)}',
         )
 
-    cm.match("Can't use complex JSON value types")
+    cm.match('Cannot use complex JSON value types')
 
 
 @pytest.mark.parametrize(
     'input_json, expected_json',
     [
         # Examples taken from https://www.w3.org/TR/html-json-forms/
         (
@@ -504,72 +504,72 @@
         ),
         (
             ['foo[bar][1]\\[142241[]:=2'],
             "HTTPie Syntax Error: Expecting '['\nfoo[bar][1]\\[142241[]\n           ^^^^^^^^",
         ),
         (
             ['foo=1', 'foo[key]:=2'],
-            "HTTPie Type Error: Can't perform 'key' based access on 'foo' which has a type of 'string' but this operation requires a type of 'object'.\nfoo[key]\n   ^^^^^",
+            "HTTPie Type Error: Cannot perform 'key' based access on 'foo' which has a type of 'string' but this operation requires a type of 'object'.\nfoo[key]\n   ^^^^^",
         ),
         (
             ['foo=1', 'foo[0]:=2'],
-            "HTTPie Type Error: Can't perform 'index' based access on 'foo' which has a type of 'string' but this operation requires a type of 'array'.\nfoo[0]\n   ^^^",
+            "HTTPie Type Error: Cannot perform 'index' based access on 'foo' which has a type of 'string' but this operation requires a type of 'array'.\nfoo[0]\n   ^^^",
         ),
         (
             ['foo=1', 'foo[]:=2'],
-            "HTTPie Type Error: Can't perform 'append' based access on 'foo' which has a type of 'string' but this operation requires a type of 'array'.\nfoo[]\n   ^^",
+            "HTTPie Type Error: Cannot perform 'append' based access on 'foo' which has a type of 'string' but this operation requires a type of 'array'.\nfoo[]\n   ^^",
         ),
         (
             ['data[key]=value', 'data[key 2]=value 2', 'data[0]=value'],
-            "HTTPie Type Error: Can't perform 'index' based access on 'data' which has a type of 'object' but this operation requires a type of 'array'.\ndata[0]\n    ^^^",
+            "HTTPie Type Error: Cannot perform 'index' based access on 'data' which has a type of 'object' but this operation requires a type of 'array'.\ndata[0]\n    ^^^",
         ),
         (
             ['data[key]=value', 'data[key 2]=value 2', 'data[]=value'],
-            "HTTPie Type Error: Can't perform 'append' based access on 'data' which has a type of 'object' but this operation requires a type of 'array'.\ndata[]\n    ^^",
+            "HTTPie Type Error: Cannot perform 'append' based access on 'data' which has a type of 'object' but this operation requires a type of 'array'.\ndata[]\n    ^^",
         ),
         (
             [
                 'foo[bar][baz][5]:=[1,2,3]',
                 'foo[bar][baz][5][]:=4',
                 'foo[bar][baz][key][]:=5',
             ],
-            "HTTPie Type Error: Can't perform 'key' based access on 'foo[bar][baz]' which has a type of 'array' but this operation requires a type of 'object'.\nfoo[bar][baz][key][]\n             ^^^^^",
+            "HTTPie Type Error: Cannot perform 'key' based access on 'foo[bar][baz]' which has a type of 'array' but this operation requires a type of 'object'.\nfoo[bar][baz][key][]\n             ^^^^^",
         ),
         (
             ['foo[-10]:=[1,2]'],
             'HTTPie Value Error: Negative indexes are not supported.\nfoo[-10]\n    ^^^',
         ),
         (
             ['foo[0]:=1', 'foo[]:=2', 'foo[\\2]:=3'],
-            "HTTPie Type Error: Can't perform 'key' based access on 'foo' which has a type of 'array' but this operation requires a type of 'object'.\nfoo[\\2]\n   ^^^^",
+            "HTTPie Type Error: Cannot perform 'key' based access on 'foo' which has a type of 'array' but this operation requires a type of 'object'.\nfoo[\\2]\n   ^^^^",
         ),
         (
             ['foo[\\1]:=2', 'foo[5]:=3'],
-            "HTTPie Type Error: Can't perform 'index' based access on 'foo' which has a type of 'object' but this operation requires a type of 'array'.\nfoo[5]\n   ^^^",
+            "HTTPie Type Error: Cannot perform 'index' based access on 'foo' which has a type of 'object' but this operation requires a type of 'array'.\nfoo[5]\n   ^^^",
         ),
         (
             ['x=y', '[]:=2'],
-            "HTTPie Type Error: Can't perform 'append' based access on '' which has a type of 'object' but this operation requires a type of 'array'.",
+            "HTTPie Type Error: Cannot perform 'append' based access on '' which has a type of 'object' but this operation requires a type of 'array'.",
         ),
         (
             ['[]:=2', 'x=y'],
-            "HTTPie Type Error: Can't perform 'key' based access on '' which has a type of 'array' but this operation requires a type of 'object'.",
+            "HTTPie Type Error: Cannot perform 'key' based access on '' which has a type of 'array' but this operation requires a type of 'object'.",
         ),
         (
             [':=[1,2,3]', '[]:=4'],
-            "HTTPie Type Error: Can't perform 'append' based access on '' which has a type of 'object' but this operation requires a type of 'array'.",
+            "HTTPie Type Error: Cannot perform 'append' based access on '' which has a type of 'object' but this operation requires a type of 'array'.",
         ),
         (
             ['[]:=4', ':=[1,2,3]'],
-            "HTTPie Type Error: Can't perform 'key' based access on '' which has a type of 'array' but this operation requires a type of 'object'.",
+            "HTTPie Type Error: Cannot perform 'key' based access on '' which has a type of 'array' but this operation requires a type of 'object'.",
         ),
     ],
 )
 def test_nested_json_errors(input_json, expected_error, httpbin):
-    with pytest.raises(HTTPieSyntaxError) as exc:
+    with pytest.raises(NestedJSONSyntaxError) as exc:
         http(httpbin + '/post', *input_json)
 
     exc_lines = str(exc.value).splitlines()
     expected_lines = expected_error.splitlines()
     if len(expected_lines) == 1:
         # When the error offsets are not important, we'll just compare the actual
         # error message.
```

### Comparing `httpie-3.2.1/tests/test_meta.py` & `httpie-3.2.2/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_offline.py` & `httpie-3.2.2/tests/test_offline.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_output.py` & `httpie-3.2.2/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_parser_schema.py` & `httpie-3.2.2/tests/test_parser_schema.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_plugins_cli.py` & `httpie-3.2.2/tests/test_plugins_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,14 +113,16 @@
     assert result.exit_status == ExitStatus.ERROR
     assert (
         result.stderr.splitlines()[-1].strip()
         == f"Can't uninstall '{dummy_plugin.name}': package is not installed"
     )
 
 
+# TODO: Make this work on CI (stopped working at some point)
+@pytest.mark.skip(reason='Doesn’t work in CI')
 @pytest.mark.requires_installation
 def test_plugins_upgrade(httpie_plugins, httpie_plugins_success, dummy_plugin):
     httpie_plugins_success("install", dummy_plugin.path)
 
     # Make a new version of the plugin
     dummy_plugin.version = '2.0.0'
     dummy_plugin.build()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `httpie-3.2.1/tests/test_redirects.py` & `httpie-3.2.2/tests/test_redirects.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_regressions.py` & `httpie-3.2.2/tests/test_regressions.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_sessions.py` & `httpie-3.2.2/tests/test_sessions.py`

 * *Files 1% similar despite different names*

```diff
@@ -442,15 +442,15 @@
     def test_get_expired_cookies_manages_multiple_cookie_headers(self, cookies, now, expected_expired):
         assert get_expired_cookies(cookies, now=now) == expected_expired
 
 
 class TestCookieStorage(CookieTestBase):
 
     @pytest.mark.parametrize(
-        'new_cookies, new_cookies_dict, expected',
+        ['specified_cookie_header', 'new_cookies_dict', 'expected_effective_cookie_header'],
         [(
             'new=bar',
             {'new': 'bar'},
             'cookie1=foo; cookie2=foo; new=bar'
         ),
             (
             'new=bar;chocolate=milk',
@@ -459,39 +459,54 @@
         ),
             (
             'new=bar; chocolate=milk',
             {'new': 'bar', 'chocolate': 'milk'},
             'chocolate=milk; cookie1=foo; cookie2=foo; new=bar'
         ),
             (
-            'new=bar;; chocolate=milk;;;',
+            'new=bar; chocolate=milk',
             {'new': 'bar', 'chocolate': 'milk'},
-            'cookie1=foo; cookie2=foo; new=bar'
+            'cookie1=foo; cookie2=foo; new=bar; chocolate=milk'
         ),
             (
             'new=bar; chocolate=milk;;;',
             {'new': 'bar', 'chocolate': 'milk'},
             'chocolate=milk; cookie1=foo; cookie2=foo; new=bar'
         )
         ]
     )
-    def test_existing_and_new_cookies_sent_in_request(self, new_cookies, new_cookies_dict, expected, httpbin):
+    def test_existing_and_new_cookies_sent_in_request(
+        self,
+        specified_cookie_header,
+        new_cookies_dict,
+        expected_effective_cookie_header,
+        httpbin,
+    ):
         r = http(
             '--session', str(self.session_path),
             '--print=H',
             httpbin.url,
-            'Cookie:' + new_cookies,
+            'Cookie:' + specified_cookie_header,
         )
-        # Note: cookies in response are in alphabetical order
-        assert f'Cookie: {expected}' in r
+        parsed_request_headers = {  # noqa
+            name: value for name, value in [
+                line.split(': ', 1)
+                for line in r.splitlines()
+                if line and ':' in line
+            ]
+        }
+        # Note: cookies in the request are in an undefined order.
+        expected_request_cookie_set = set(expected_effective_cookie_header.split('; '))
+        actual_request_cookie_set = set(parsed_request_headers['Cookie'].split('; '))
+        assert actual_request_cookie_set == expected_request_cookie_set
 
         updated_session = json.loads(self.session_path.read_text(encoding=UTF8))
+        assert 'Cookie' not in updated_session['headers']
         for name, value in new_cookies_dict.items():
-            assert name, value in updated_session['cookies']
-            assert 'Cookie' not in updated_session['headers']
+            assert updated_session['cookies'][name]['value'] == value
 
     @pytest.mark.parametrize(
         'cli_cookie, set_cookie, expected',
         [(
             '',
             '/cookies/set/cookie1/bar',
             'bar'
```

### Comparing `httpie-3.2.1/tests/test_ssl.py` & `httpie-3.2.2/tests/test_ssl.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pytest
 import pytest_httpbin.certs
 import requests.exceptions
 import urllib3
 
 from unittest import mock
 
-from httpie.ssl_ import AVAILABLE_SSL_VERSION_ARG_MAPPING, DEFAULT_SSL_CIPHERS
+from httpie.ssl_ import AVAILABLE_SSL_VERSION_ARG_MAPPING, DEFAULT_SSL_CIPHERS_STRING
 from httpie.status import ExitStatus
 
 from .utils import HTTP_OK, TESTS_ROOT, IS_PYOPENSSL, http
 
 
 try:
     # Handle OpenSSL errors, if installed.
@@ -142,15 +142,15 @@
             http(httpbin_secure.url + '/get', '--verify', __file__)
 
 
 def test_ciphers(httpbin_secure):
     r = http(
         httpbin_secure.url + '/get',
         '--ciphers',
-        DEFAULT_SSL_CIPHERS,
+        DEFAULT_SSL_CIPHERS_STRING,
     )
     assert HTTP_OK in r
 
 
 @pytest.mark.skipif(IS_PYOPENSSL, reason='pyOpenSSL uses a different message format.')
 def test_ciphers_none_can_be_selected(httpbin_secure):
     r = http(
```

### Comparing `httpie-3.2.1/tests/test_stream.py` & `httpie-3.2.2/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_tokens.py` & `httpie-3.2.2/tests/test_tokens.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_transport_plugin.py` & `httpie-3.2.2/tests/test_transport_plugin.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_update_warnings.py` & `httpie-3.2.2/tests/test_update_warnings.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_uploads.py` & `httpie-3.2.2/tests/test_uploads.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_windows.py` & `httpie-3.2.2/tests/test_windows.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/test_xml.py` & `httpie-3.2.2/tests/test_xml.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/utils/__init__.py` & `httpie-3.2.2/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/utils/http_server.py` & `httpie-3.2.2/tests/utils/http_server.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/utils/matching/__init__.py` & `httpie-3.2.2/tests/utils/matching/__init__.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/utils/matching/parsing.py` & `httpie-3.2.2/tests/utils/matching/parsing.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/utils/matching/test_matching.py` & `httpie-3.2.2/tests/utils/matching/test_matching.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/utils/matching/tokens.py` & `httpie-3.2.2/tests/utils/matching/tokens.py`

 * *Files identical despite different names*

### Comparing `httpie-3.2.1/tests/utils/plugins_cli.py` & `httpie-3.2.2/tests/utils/plugins_cli.py`

 * *Files identical despite different names*

