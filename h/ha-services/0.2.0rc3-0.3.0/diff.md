# Comparing `tmp/ha-services-0.2.0rc3.tar.gz` & `tmp/ha-services-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ha-services-0.2.0rc3.tar", last modified: Thu May 18 08:39:12 2023, max compression
+gzip compressed data, was "ha-services-0.3.0.tar", last modified: Fri May 19 20:09:04 2023, max compression
```

## Comparing `ha-services-0.2.0rc3.tar` & `ha-services-0.3.0.tar`

### file list

```diff
@@ -1,98 +1,103 @@
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.687547 ha-services-0.2.0rc3/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.683547 ha-services-0.2.0rc3/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.683547 ha-services-0.2.0rc3/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1476 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)     1239 2023-05-18 08:39:12.687547 ha-services-0.2.0rc3/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)      823 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/README.md
--rwxrwxr-x   0 jens      (1000) users      (100)     3052 2023-05-11 18:48:55.000000 ha-services-0.2.0rc3/cli.py
--rwxrwxr-x   0 jens      (1000) users      (100)     3052 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/dev-cli.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.683547 ha-services-0.2.0rc3/ha_services/
--rw-rw-r--   0 jens      (1000) users      (100)      168 2023-05-18 08:36:49.000000 ha-services-0.2.0rc3/ha_services/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      195 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/__main__.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.683547 ha-services-0.2.0rc3/ha_services/cli/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/cli/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     8343 2023-05-17 15:18:45.000000 ha-services-0.2.0rc3/ha_services/cli/cli_app.py
--rw-rw-r--   0 jens      (1000) users      (100)     7880 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/cli/dev.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.683547 ha-services-0.2.0rc3/ha_services/cli_tools/
--rw-rw-r--   0 jens      (1000) users      (100)      120 2023-05-11 06:15:16.000000 ha-services-0.2.0rc3/ha_services/cli_tools/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1364 2023-05-18 05:57:33.000000 ha-services-0.2.0rc3/ha_services/cli_tools/dict_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)     2529 2023-05-11 17:34:50.000000 ha-services-0.2.0rc3/ha_services/cli_tools/path_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)     3729 2023-05-11 20:05:42.000000 ha-services-0.2.0rc3/ha_services/cli_tools/rich_utils.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.683547 ha-services-0.2.0rc3/ha_services/cli_tools/test_utils/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc3/ha_services/cli_tools/test_utils/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1041 2023-05-18 04:39:33.000000 ha-services-0.2.0rc3/ha_services/cli_tools/test_utils/assertion.py
--rw-rw-r--   0 jens      (1000) users      (100)     1261 2023-05-18 04:14:32.000000 ha-services-0.2.0rc3/ha_services/cli_tools/test_utils/environment_fixtures.py
--rw-rw-r--   0 jens      (1000) users      (100)      820 2023-05-18 04:17:28.000000 ha-services-0.2.0rc3/ha_services/cli_tools/test_utils/mock_rich.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.683547 ha-services-0.2.0rc3/ha_services/cli_tools/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc3/ha_services/cli_tools/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      432 2023-05-18 05:10:52.000000 ha-services-0.2.0rc3/ha_services/cli_tools/tests/test_dict_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)      693 2023-05-11 07:38:00.000000 ha-services-0.2.0rc3/ha_services/cli_tools/tests/test_environ_fixtures.py
--rw-rw-r--   0 jens      (1000) users      (100)     1918 2023-05-11 07:37:29.000000 ha-services-0.2.0rc3/ha_services/cli_tools/tests/test_path_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)      164 2023-05-09 16:59:30.000000 ha-services-0.2.0rc3/ha_services/constants.py
--rw-rw-r--   0 jens      (1000) users      (100)     3437 2023-05-17 15:17:40.000000 ha-services-0.2.0rc3/ha_services/example.py
--rw-rw-r--   0 jens      (1000) users      (100)      240 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/log_setup.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.683547 ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/
--rw-rw-r--   0 jens      (1000) users      (100)       22 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1898 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/converter.py
--rw-rw-r--   0 jens      (1000) users      (100)     1061 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/data_classes.py
--rw-rw-r--   0 jens      (1000) users      (100)     4082 2023-05-18 04:39:33.000000 ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/mqtt.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.683547 ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2142 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/tests/test_converter.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.683547 ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/utilities/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/utilities/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      315 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/utilities/string_utils.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.687547 ha-services-0.2.0rc3/ha_services/systemd/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc3/ha_services/systemd/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     7252 2023-05-18 04:39:33.000000 ha-services-0.2.0rc3/ha_services/systemd/api.py
--rw-rw-r--   0 jens      (1000) users      (100)     3184 2023-05-18 04:39:33.000000 ha-services-0.2.0rc3/ha_services/systemd/data_classes.py
--rw-rw-r--   0 jens      (1000) users      (100)      505 2023-05-10 07:16:49.000000 ha-services-0.2.0rc3/ha_services/systemd/defaults.py
--rw-rw-r--   0 jens      (1000) users      (100)      320 2023-05-17 15:08:38.000000 ha-services-0.2.0rc3/ha_services/systemd/service_template.txt
--rw-rw-r--   0 jens      (1000) users      (100)     1794 2023-05-09 19:43:34.000000 ha-services-0.2.0rc3/ha_services/systemd/template.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.687547 ha-services-0.2.0rc3/ha_services/systemd/test_utils/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-18 04:08:42.000000 ha-services-0.2.0rc3/ha_services/systemd/test_utils/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2012 2023-05-18 05:54:08.000000 ha-services-0.2.0rc3/ha_services/systemd/test_utils/mock_systemd_info.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.687547 ha-services-0.2.0rc3/ha_services/systemd/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc3/ha_services/systemd/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     3387 2023-05-18 05:56:02.000000 ha-services-0.2.0rc3/ha_services/systemd/tests/test_api.py
--rw-rw-r--   0 jens      (1000) users      (100)     1482 2023-05-18 05:56:47.000000 ha-services-0.2.0rc3/ha_services/systemd/tests/test_data_classes.py
--rw-rw-r--   0 jens      (1000) users      (100)     3000 2023-05-18 06:02:23.000000 ha-services-0.2.0rc3/ha_services/systemd/tests/test_mock_systemd_info.py
--rw-rw-r--   0 jens      (1000) users      (100)      595 2023-05-18 06:01:09.000000 ha-services-0.2.0rc3/ha_services/systemd/tests/test_mock_systemd_info_mock_1.snapshot.toml
--rw-rw-r--   0 jens      (1000) users      (100)     2471 2023-05-09 19:43:34.000000 ha-services-0.2.0rc3/ha_services/systemd/tests/test_template.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.687547 ha-services-0.2.0rc3/ha_services/tests/
--rw-rw-r--   0 jens      (1000) users      (100)      262 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      217 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/tests/test_doctests.py
--rw-rw-r--   0 jens      (1000) users      (100)     2579 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/tests/test_project_setup.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.687547 ha-services-0.2.0rc3/ha_services/toml_settings/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/toml_settings/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     4234 2023-05-18 05:57:51.000000 ha-services-0.2.0rc3/ha_services/toml_settings/api.py
--rw-rw-r--   0 jens      (1000) users      (100)      220 2023-05-09 20:53:17.000000 ha-services-0.2.0rc3/ha_services/toml_settings/data_class_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)     1352 2023-05-11 19:53:35.000000 ha-services-0.2.0rc3/ha_services/toml_settings/debug.py
--rw-rw-r--   0 jens      (1000) users      (100)     3059 2023-05-09 20:53:17.000000 ha-services-0.2.0rc3/ha_services/toml_settings/deserialize.py
--rw-rw-r--   0 jens      (1000) users      (100)       56 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/toml_settings/exceptions.py
--rw-rw-r--   0 jens      (1000) users      (100)      728 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/toml_settings/sensible_editor.py
--rw-rw-r--   0 jens      (1000) users      (100)     1847 2023-05-18 06:01:57.000000 ha-services-0.2.0rc3/ha_services/toml_settings/serialize.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.687547 ha-services-0.2.0rc3/ha_services/toml_settings/test_utils/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-18 05:26:41.000000 ha-services-0.2.0rc3/ha_services/toml_settings/test_utils/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     3092 2023-05-18 08:32:52.000000 ha-services-0.2.0rc3/ha_services/toml_settings/test_utils/data_class_utils.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.687547 ha-services-0.2.0rc3/ha_services/toml_settings/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/toml_settings/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1383 2023-05-18 05:43:52.000000 ha-services-0.2.0rc3/ha_services/toml_settings/tests/fixtures.py
--rw-rw-r--   0 jens      (1000) users      (100)     1044 2023-05-17 15:20:34.000000 ha-services-0.2.0rc3/ha_services/toml_settings/tests/test_demo_settings.py
--rw-rw-r--   0 jens      (1000) users      (100)     5606 2023-05-18 06:01:57.000000 ha-services-0.2.0rc3/ha_services/toml_settings/tests/test_deserialize.py
--rw-rw-r--   0 jens      (1000) users      (100)     3172 2023-05-18 05:24:56.000000 ha-services-0.2.0rc3/ha_services/toml_settings/tests/test_serialize.py
--rw-rw-r--   0 jens      (1000) users      (100)     3205 2023-05-18 08:31:32.000000 ha-services-0.2.0rc3/ha_services/toml_settings/tests/test_test_utils.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.683547 ha-services-0.2.0rc3/ha_services.egg-info/
--rw-rw-r--   0 jens      (1000) users      (100)     1239 2023-05-18 08:39:12.000000 ha-services-0.2.0rc3/ha_services.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)     2868 2023-05-18 08:39:12.000000 ha-services-0.2.0rc3/ha_services.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1000) users      (100)        1 2023-05-18 08:39:12.000000 ha-services-0.2.0rc3/ha_services.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1000) users      (100)      105 2023-05-18 08:39:12.000000 ha-services-0.2.0rc3/ha_services.egg-info/entry_points.txt
--rw-rw-r--   0 jens      (1000) users      (100)      283 2023-05-18 08:39:12.000000 ha-services-0.2.0rc3/ha_services.egg-info/requires.txt
--rw-rw-r--   0 jens      (1000) users      (100)       12 2023-05-18 08:39:12.000000 ha-services-0.2.0rc3/ha_services.egg-info/top_level.txt
--rw-rw-r--   0 jens      (1000) users      (100)     4934 2023-05-09 17:58:58.000000 ha-services-0.2.0rc3/pyproject.toml
--rw-rw-r--   0 jens      (1000) users      (100)    53004 2023-05-18 06:04:30.000000 ha-services-0.2.0rc3/requirements.dev.txt
--rw-rw-r--   0 jens      (1000) users      (100)    22054 2023-05-18 06:04:13.000000 ha-services-0.2.0rc3/requirements.txt
--rw-rw-r--   0 jens      (1000) users      (100)       38 2023-05-18 08:39:12.687547 ha-services-0.2.0rc3/setup.cfg
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 20:09:04.271685 ha-services-0.3.0/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-05-09 16:39:25.000000 ha-services-0.3.0/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-05-09 16:39:25.000000 ha-services-0.3.0/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 20:09:04.267685 ha-services-0.3.0/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 20:09:04.267685 ha-services-0.3.0/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1476 2023-05-09 16:39:25.000000 ha-services-0.3.0/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-05-09 16:39:25.000000 ha-services-0.3.0/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)     6951 2023-05-19 20:09:04.271685 ha-services-0.3.0/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     6538 2023-05-18 14:20:06.000000 ha-services-0.3.0/README.md
+-rwxrwxr-x   0 jens      (1000) users      (100)     3052 2023-05-11 18:48:55.000000 ha-services-0.3.0/cli.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     3052 2023-05-09 16:39:25.000000 ha-services-0.3.0/dev-cli.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 20:09:04.267685 ha-services-0.3.0/ha_services/
+-rw-rw-r--   0 jens      (1000) users      (100)      165 2023-05-19 19:34:35.000000 ha-services-0.3.0/ha_services/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      195 2023-05-09 16:39:25.000000 ha-services-0.3.0/ha_services/__main__.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 20:09:04.267685 ha-services-0.3.0/ha_services/cli/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.3.0/ha_services/cli/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     8352 2023-05-19 19:35:24.000000 ha-services-0.3.0/ha_services/cli/cli_app.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7184 2023-05-19 19:56:41.000000 ha-services-0.3.0/ha_services/cli/dev.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 20:09:04.271685 ha-services-0.3.0/ha_services/cli_tools/
+-rw-rw-r--   0 jens      (1000) users      (100)      120 2023-05-11 06:15:16.000000 ha-services-0.3.0/ha_services/cli_tools/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1445 2023-05-19 19:49:27.000000 ha-services-0.3.0/ha_services/cli_tools/dev_tools.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1364 2023-05-18 05:57:33.000000 ha-services-0.3.0/ha_services/cli_tools/dict_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2529 2023-05-11 17:34:50.000000 ha-services-0.3.0/ha_services/cli_tools/path_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3729 2023-05-11 20:05:42.000000 ha-services-0.3.0/ha_services/cli_tools/rich_utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 20:09:04.271685 ha-services-0.3.0/ha_services/cli_tools/test_utils/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.3.0/ha_services/cli_tools/test_utils/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1048 2023-05-18 12:56:44.000000 ha-services-0.3.0/ha_services/cli_tools/test_utils/assertion.py
+-rw-rw-r--   0 jens      (1000) users      (100)      911 2023-05-18 09:57:15.000000 ha-services-0.3.0/ha_services/cli_tools/test_utils/cli_readme.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1261 2023-05-18 04:14:32.000000 ha-services-0.3.0/ha_services/cli_tools/test_utils/environment_fixtures.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4932 2023-05-18 14:16:23.000000 ha-services-0.3.0/ha_services/cli_tools/test_utils/rich_test_utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 20:09:04.271685 ha-services-0.3.0/ha_services/cli_tools/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.3.0/ha_services/cli_tools/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      432 2023-05-18 05:10:52.000000 ha-services-0.3.0/ha_services/cli_tools/tests/test_dict_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)      693 2023-05-11 07:38:00.000000 ha-services-0.3.0/ha_services/cli_tools/tests/test_environ_fixtures.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2220 2023-05-18 12:58:25.000000 ha-services-0.3.0/ha_services/cli_tools/tests/test_mock_rich.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1918 2023-05-11 07:37:29.000000 ha-services-0.3.0/ha_services/cli_tools/tests/test_path_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)      998 2023-05-19 19:18:58.000000 ha-services-0.3.0/ha_services/cli_tools/verbosity.py
+-rw-rw-r--   0 jens      (1000) users      (100)      164 2023-05-09 16:59:30.000000 ha-services-0.3.0/ha_services/constants.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3448 2023-05-19 19:30:01.000000 ha-services-0.3.0/ha_services/example.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 20:09:04.271685 ha-services-0.3.0/ha_services/mqtt4homeassistant/
+-rw-rw-r--   0 jens      (1000) users      (100)       22 2023-05-09 16:39:25.000000 ha-services-0.3.0/ha_services/mqtt4homeassistant/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1898 2023-05-09 16:39:25.000000 ha-services-0.3.0/ha_services/mqtt4homeassistant/converter.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1061 2023-05-09 16:39:25.000000 ha-services-0.3.0/ha_services/mqtt4homeassistant/data_classes.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4102 2023-05-19 19:30:59.000000 ha-services-0.3.0/ha_services/mqtt4homeassistant/mqtt.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 20:09:04.271685 ha-services-0.3.0/ha_services/mqtt4homeassistant/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.3.0/ha_services/mqtt4homeassistant/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2142 2023-05-09 16:39:25.000000 ha-services-0.3.0/ha_services/mqtt4homeassistant/tests/test_converter.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 20:09:04.271685 ha-services-0.3.0/ha_services/mqtt4homeassistant/utilities/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.3.0/ha_services/mqtt4homeassistant/utilities/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      315 2023-05-09 16:39:25.000000 ha-services-0.3.0/ha_services/mqtt4homeassistant/utilities/string_utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 20:09:04.271685 ha-services-0.3.0/ha_services/systemd/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.3.0/ha_services/systemd/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7252 2023-05-18 04:39:33.000000 ha-services-0.3.0/ha_services/systemd/api.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3184 2023-05-18 04:39:33.000000 ha-services-0.3.0/ha_services/systemd/data_classes.py
+-rw-rw-r--   0 jens      (1000) users      (100)      505 2023-05-10 07:16:49.000000 ha-services-0.3.0/ha_services/systemd/defaults.py
+-rw-rw-r--   0 jens      (1000) users      (100)      320 2023-05-17 15:08:38.000000 ha-services-0.3.0/ha_services/systemd/service_template.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     1794 2023-05-09 19:43:34.000000 ha-services-0.3.0/ha_services/systemd/template.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 20:09:04.271685 ha-services-0.3.0/ha_services/systemd/test_utils/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-18 04:08:42.000000 ha-services-0.3.0/ha_services/systemd/test_utils/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2012 2023-05-18 05:54:08.000000 ha-services-0.3.0/ha_services/systemd/test_utils/mock_systemd_info.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 20:09:04.271685 ha-services-0.3.0/ha_services/systemd/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.3.0/ha_services/systemd/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3387 2023-05-18 05:56:02.000000 ha-services-0.3.0/ha_services/systemd/tests/test_api.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1482 2023-05-18 05:56:47.000000 ha-services-0.3.0/ha_services/systemd/tests/test_data_classes.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3000 2023-05-18 06:02:23.000000 ha-services-0.3.0/ha_services/systemd/tests/test_mock_systemd_info.py
+-rw-rw-r--   0 jens      (1000) users      (100)      595 2023-05-18 06:01:09.000000 ha-services-0.3.0/ha_services/systemd/tests/test_mock_systemd_info_mock_1.snapshot.toml
+-rw-rw-r--   0 jens      (1000) users      (100)     2471 2023-05-09 19:43:34.000000 ha-services-0.3.0/ha_services/systemd/tests/test_template.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 20:09:04.271685 ha-services-0.3.0/ha_services/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)      296 2023-05-19 19:29:53.000000 ha-services-0.3.0/ha_services/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      217 2023-05-09 16:39:25.000000 ha-services-0.3.0/ha_services/tests/test_doctests.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2579 2023-05-09 16:39:25.000000 ha-services-0.3.0/ha_services/tests/test_project_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2949 2023-05-18 14:20:00.000000 ha-services-0.3.0/ha_services/tests/test_readme.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 20:09:04.271685 ha-services-0.3.0/ha_services/toml_settings/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.3.0/ha_services/toml_settings/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4234 2023-05-18 05:57:51.000000 ha-services-0.3.0/ha_services/toml_settings/api.py
+-rw-rw-r--   0 jens      (1000) users      (100)      220 2023-05-09 20:53:17.000000 ha-services-0.3.0/ha_services/toml_settings/data_class_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1352 2023-05-11 19:53:35.000000 ha-services-0.3.0/ha_services/toml_settings/debug.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3059 2023-05-09 20:53:17.000000 ha-services-0.3.0/ha_services/toml_settings/deserialize.py
+-rw-rw-r--   0 jens      (1000) users      (100)       56 2023-05-09 16:39:25.000000 ha-services-0.3.0/ha_services/toml_settings/exceptions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      728 2023-05-09 16:39:25.000000 ha-services-0.3.0/ha_services/toml_settings/sensible_editor.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1847 2023-05-18 06:01:57.000000 ha-services-0.3.0/ha_services/toml_settings/serialize.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 20:09:04.271685 ha-services-0.3.0/ha_services/toml_settings/test_utils/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-18 05:26:41.000000 ha-services-0.3.0/ha_services/toml_settings/test_utils/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1153 2023-05-18 13:05:47.000000 ha-services-0.3.0/ha_services/toml_settings/test_utils/cli_mock.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3092 2023-05-18 08:32:52.000000 ha-services-0.3.0/ha_services/toml_settings/test_utils/data_class_utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 20:09:04.271685 ha-services-0.3.0/ha_services/toml_settings/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.3.0/ha_services/toml_settings/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1383 2023-05-18 05:43:52.000000 ha-services-0.3.0/ha_services/toml_settings/tests/fixtures.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1044 2023-05-17 15:20:34.000000 ha-services-0.3.0/ha_services/toml_settings/tests/test_demo_settings.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5606 2023-05-18 06:01:57.000000 ha-services-0.3.0/ha_services/toml_settings/tests/test_deserialize.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3172 2023-05-18 05:24:56.000000 ha-services-0.3.0/ha_services/toml_settings/tests/test_serialize.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3205 2023-05-18 08:31:32.000000 ha-services-0.3.0/ha_services/toml_settings/tests/test_test_utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-19 20:09:04.267685 ha-services-0.3.0/ha_services.egg-info/
+-rw-rw-r--   0 jens      (1000) users      (100)     6951 2023-05-19 20:09:04.000000 ha-services-0.3.0/ha_services.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     3094 2023-05-19 20:09:04.000000 ha-services-0.3.0/ha_services.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        1 2023-05-19 20:09:04.000000 ha-services-0.3.0/ha_services.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      105 2023-05-19 20:09:04.000000 ha-services-0.3.0/ha_services.egg-info/entry_points.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      283 2023-05-19 20:09:04.000000 ha-services-0.3.0/ha_services.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       12 2023-05-19 20:09:04.000000 ha-services-0.3.0/ha_services.egg-info/top_level.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     4934 2023-05-09 17:58:58.000000 ha-services-0.3.0/pyproject.toml
+-rw-rw-r--   0 jens      (1000) users      (100)    53004 2023-05-18 06:04:30.000000 ha-services-0.3.0/requirements.dev.txt
+-rw-rw-r--   0 jens      (1000) users      (100)    22054 2023-05-18 06:04:13.000000 ha-services-0.3.0/requirements.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       38 2023-05-19 20:09:04.271685 ha-services-0.3.0/setup.cfg
```

### Comparing `ha-services-0.2.0rc3/.github/workflows/tests.yml` & `ha-services-0.3.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/cli.py` & `ha-services-0.3.0/cli.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/dev-cli.py` & `ha-services-0.3.0/dev-cli.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/cli/cli_app.py` & `ha-services-0.3.0/ha_services/cli/cli_app.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 from rich import print  # noqa
 from rich.console import Console
 from rich.traceback import install as rich_traceback_install
 from rich_click import RichGroup
 
 import ha_services
 from ha_services import __version__, constants
+from ha_services.cli_tools.verbosity import OPTION_KWARGS_VERBOSE, setup_logging
 from ha_services.example import DemoSettings, SystemdServiceInfo, publish_forever
-from ha_services.log_setup import basic_log_setup
 from ha_services.mqtt4homeassistant.data_classes import MqttSettings
 from ha_services.mqtt4homeassistant.mqtt import get_connected_client
 from ha_services.systemd.api import ServiceControl
 from ha_services.toml_settings.api import TomlSettings
 
 
 logger = logging.getLogger(__name__)
@@ -76,37 +76,37 @@
 ######################################################################################################
 
 SETTINGS_DIR_NAME = 'ha-services'
 SETTINGS_FILE_NAME = 'ha-services-demo'
 
 
 @click.command()
-@click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_TRUE)
-def edit_settings(debug):
+@click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
+def edit_settings(verbosity: int):
     """
     Edit the settings file. On first call: Create the default one.
     """
-    basic_log_setup(debug=debug)
+    setup_logging(verbosity=verbosity)
     TomlSettings(
         dir_name=SETTINGS_DIR_NAME,
         file_name=SETTINGS_FILE_NAME,
         settings_dataclass=DemoSettings(),
     ).open_in_editor()
 
 
 cli.add_command(edit_settings)
 
 
 @click.command()
-@click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_TRUE)
-def print_settings(debug):
+@click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
+def print_settings(verbosity: int):
     """
     Display (anonymized) MQTT server username and password
     """
-    basic_log_setup(debug=debug)
+    setup_logging(verbosity=verbosity)
     TomlSettings(
         dir_name=SETTINGS_DIR_NAME,
         file_name=SETTINGS_FILE_NAME,
         settings_dataclass=DemoSettings(),
     ).print_settings()
 
 
@@ -114,83 +114,83 @@
 
 
 ######################################################################################################
 # Manage systemd service commands:
 
 
 @click.command()
-@click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_TRUE)
-def debug_systemd_config(debug):
+@click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
+def systemd_debug(verbosity: int):
     """
     Print Systemd service template + context + rendered file content.
     """
-    basic_log_setup(debug=debug)
+    setup_logging(verbosity=verbosity)
     toml_settings = TomlSettings(
         dir_name=SETTINGS_DIR_NAME,
         file_name=SETTINGS_FILE_NAME,
         settings_dataclass=DemoSettings(),
     )
     user_settings: DemoSettings = toml_settings.get_user_settings(debug=True)
     systemd_settings: SystemdServiceInfo = user_settings.systemd
 
     ServiceControl(info=systemd_settings).debug_systemd_config()
 
 
-cli.add_command(debug_systemd_config)
+cli.add_command(systemd_debug)
 
 
 @click.command()
-@click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_TRUE)
-def setup_systemd_service(debug):
+@click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
+def systemd_setup(verbosity: int):
     """
     Write Systemd service file, enable it and (re-)start the service. (May need sudo)
     """
-    basic_log_setup(debug=debug)
+    setup_logging(verbosity=verbosity)
     toml_settings = TomlSettings(
         dir_name=SETTINGS_DIR_NAME,
         file_name=SETTINGS_FILE_NAME,
         settings_dataclass=DemoSettings(),
     )
     user_settings: DemoSettings = toml_settings.get_user_settings(debug=True)
     systemd_settings: SystemdServiceInfo = user_settings.systemd
 
     ServiceControl(info=systemd_settings).setup_and_restart_systemd_service()
 
 
-cli.add_command(setup_systemd_service)
+cli.add_command(systemd_setup)
 
 
 @click.command()
-@click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_TRUE)
-def remove_systemd_service(debug):
+@click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
+def systemd_remove(verbosity: int):
     """
     Write Systemd service file, enable it and (re-)start the service. (May need sudo)
     """
-    basic_log_setup(debug=debug)
+    setup_logging(verbosity=verbosity)
     toml_settings = TomlSettings(
         dir_name=SETTINGS_DIR_NAME,
         file_name=SETTINGS_FILE_NAME,
         settings_dataclass=DemoSettings(),
     )
     user_settings: DemoSettings = toml_settings.get_user_settings(debug=True)
     systemd_settings: SystemdServiceInfo = user_settings.systemd
 
     ServiceControl(info=systemd_settings).remove_systemd_service()
 
 
-cli.add_command(remove_systemd_service)
+cli.add_command(systemd_remove)
 
 
 @click.command()
-@click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_TRUE)
-def systemd_status(debug):
+@click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
+def systemd_status(verbosity: int):
     """
     Display status of systemd service. (May need sudo)
     """
-    basic_log_setup(debug=debug)
+    setup_logging(verbosity=verbosity)
     toml_settings = TomlSettings(
         dir_name=SETTINGS_DIR_NAME,
         file_name=SETTINGS_FILE_NAME,
         settings_dataclass=DemoSettings(),
     )
     user_settings: DemoSettings = toml_settings.get_user_settings(debug=True)
     systemd_settings: SystemdServiceInfo = user_settings.systemd
@@ -198,20 +198,20 @@
     ServiceControl(info=systemd_settings).status()
 
 
 cli.add_command(systemd_status)
 
 
 @click.command()
-@click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_TRUE)
-def systemd_stop(debug):
+@click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
+def systemd_stop(verbosity: int):
     """
     Stops the systemd service. (May need sudo)
     """
-    basic_log_setup(debug=debug)
+    setup_logging(verbosity=verbosity)
     toml_settings = TomlSettings(
         dir_name=SETTINGS_DIR_NAME,
         file_name=SETTINGS_FILE_NAME,
         settings_dataclass=DemoSettings(),
     )
     user_settings: DemoSettings = toml_settings.get_user_settings(debug=True)
     systemd_settings: SystemdServiceInfo = user_settings.systemd
@@ -222,20 +222,20 @@
 cli.add_command(systemd_stop)
 
 ######################################################################################################
 # MQTT DEMO commands:
 
 
 @click.command()
-@click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_FALSE)
-def test_mqtt_connection(debug):
+@click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
+def test_mqtt_connection(verbosity: int):
     """
     Test connection to MQTT Server
     """
-    basic_log_setup(debug=debug)
+    setup_logging(verbosity=verbosity)
     toml_settings = TomlSettings(
         dir_name=SETTINGS_DIR_NAME,
         file_name=SETTINGS_FILE_NAME,
         settings_dataclass=DemoSettings(),
     )
     user_settings: DemoSettings = toml_settings.get_user_settings(debug=True)
 
@@ -247,30 +247,29 @@
     print('\n[green]Test succeed[/green], bye ;)')
 
 
 cli.add_command(test_mqtt_connection)
 
 
 @click.command()
-@click.option('--verbose/--no-verbose', **OPTION_ARGS_DEFAULT_TRUE)
-@click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_FALSE)
-def publish_loop(verbose, debug):
+@click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
+def publish_loop(verbosity: int):
     """
     Publish data via MQTT for Home Assistant (endless loop)
     """
-    basic_log_setup(debug=debug)
+    setup_logging(verbosity=verbosity)
     toml_settings = TomlSettings(
         dir_name=SETTINGS_DIR_NAME,
         file_name=SETTINGS_FILE_NAME,
         settings_dataclass=DemoSettings(),
     )
     user_settings: DemoSettings = toml_settings.get_user_settings(debug=True)
 
     try:
-        publish_forever(user_settings=user_settings, verbose=verbose)
+        publish_forever(user_settings=user_settings, verbosity=verbosity)
     except KeyboardInterrupt:
         print('Bye, bye')
 
 
 cli.add_command(publish_loop)
```

### Comparing `ha-services-0.2.0rc3/ha_services/cli/dev.py` & `ha-services-0.3.0/ha_services/cli/dev.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from manageprojects.utilities.subprocess_utils import verbose_check_call
 from manageprojects.utilities.version_info import print_version
 from rich import print  # noqa; noqa
 from rich_click import RichGroup
 
 import ha_services
 from ha_services import constants
+from ha_services.cli_tools.dev_tools import _run_tox, _run_unittest_cli
+from ha_services.cli_tools.verbosity import OPTION_KWARGS_VERBOSE
 
 
 logger = logging.getLogger(__name__)
 
 
 PACKAGE_ROOT = Path(ha_services.__file__).parent.parent
 assert_is_file(PACKAGE_ROOT / 'pyproject.toml')
@@ -55,34 +57,34 @@
     epilog=constants.CLI_EPILOG,
 )
 def cli():
     pass
 
 
 @click.command()
-@click.option('--verbose/--no-verbose', **OPTION_ARGS_DEFAULT_FALSE)
-def mypy(verbose: bool = True):
+@click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
+def mypy(verbosity: int):
     """Run Mypy (configured in pyproject.toml)"""
-    verbose_check_call('mypy', '.', cwd=PACKAGE_ROOT, verbose=verbose, exit_on_error=True)
+    verbose_check_call('mypy', '.', cwd=PACKAGE_ROOT, verbose=verbosity > 0, exit_on_error=True)
 
 
 cli.add_command(mypy)
 
 
 @click.command()
-@click.option('--verbose/--no-verbose', **OPTION_ARGS_DEFAULT_FALSE)
-def coverage(verbose: bool = True):
+@click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
+def coverage(verbosity: int):
     """
     Run and show coverage.
     """
-    verbose_check_call('coverage', 'run', verbose=verbose, exit_on_error=True)
-    verbose_check_call('coverage', 'combine', '--append', verbose=verbose, exit_on_error=True)
-    verbose_check_call('coverage', 'report', '--fail-under=30', verbose=verbose, exit_on_error=True)
-    verbose_check_call('coverage', 'xml', verbose=verbose, exit_on_error=True)
-    verbose_check_call('coverage', 'json', verbose=verbose, exit_on_error=True)
+    verbose_check_call('coverage', 'run', verbose=verbosity > 0, exit_on_error=True)
+    verbose_check_call('coverage', 'combine', '--append', verbose=verbosity > 0, exit_on_error=True)
+    verbose_check_call('coverage', 'report', '--fail-under=30', verbose=verbosity > 0, exit_on_error=True)
+    verbose_check_call('coverage', 'xml', verbose=verbosity > 0, exit_on_error=True)
+    verbose_check_call('coverage', 'json', verbose=verbosity > 0, exit_on_error=True)
 
 
 cli.add_command(coverage)
 
 
 @click.command()
 def install():
@@ -173,33 +175,33 @@
 
 
 cli.add_command(publish)
 
 
 @click.command()
 @click.option('--color/--no-color', **OPTION_ARGS_DEFAULT_TRUE)
-@click.option('--verbose/--no-verbose', **OPTION_ARGS_DEFAULT_FALSE)
-def fix_code_style(color: bool = True, verbose: bool = False):
+@click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
+def fix_code_style(color: bool, verbosity: int):
     """
     Fix code style of all ha_services source code files via darker
     """
-    code_style.fix(package_root=PACKAGE_ROOT, color=color, verbose=verbose)
+    code_style.fix(package_root=PACKAGE_ROOT, color=color, verbose=verbosity > 0)
 
 
 cli.add_command(fix_code_style)
 
 
 @click.command()
 @click.option('--color/--no-color', **OPTION_ARGS_DEFAULT_TRUE)
-@click.option('--verbose/--no-verbose', **OPTION_ARGS_DEFAULT_FALSE)
-def check_code_style(color: bool = True, verbose: bool = False):
+@click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
+def check_code_style(color: bool, verbosity: int):
     """
     Check code style by calling darker + flake8
     """
-    code_style.check(package_root=PACKAGE_ROOT, color=color, verbose=verbose)
+    code_style.check(package_root=PACKAGE_ROOT, color=color, verbose=verbosity > 0)
 
 
 cli.add_command(check_code_style)
 
 
 @click.command()
 def update_test_snapshot_files():
@@ -228,63 +230,25 @@
     new_files = len(list(iter_snapshot_files()))
     print(f'{new_files} test snapshot files created, ok.\n')
 
 
 cli.add_command(update_test_snapshot_files)
 
 
-def _run_unittest_cli(extra_env=None, verbose=True, exit_after_run=True):
-    """
-    Call the origin unittest CLI and pass all args to it.
-    """
-    if extra_env is None:
-        extra_env = dict()
-
-    extra_env.update(
-        dict(
-            PYTHONUNBUFFERED='1',
-            PYTHONWARNINGS='always',
-        )
-    )
-
-    args = sys.argv[2:]
-    if not args:
-        if verbose:
-            args = ('--verbose', '--locals', '--buffer')
-        else:
-            args = ('--locals', '--buffer')
-
-    verbose_check_call(
-        sys.executable,
-        '-m',
-        'unittest',
-        *args,
-        timeout=15 * 60,
-        extra_env=extra_env,
-    )
-    if exit_after_run:
-        sys.exit(0)
-
-
 @click.command()  # Dummy command
 def test():
     """
     Run unittests
     """
     _run_unittest_cli()
 
 
 cli.add_command(test)
 
 
-def _run_tox():
-    verbose_check_call(sys.executable, '-m', 'tox', *sys.argv[2:])
-    sys.exit(0)
-
-
 @click.command()  # Dummy "tox" command
 def tox():
     """
     Run tox
     """
     _run_tox()
```

### Comparing `ha-services-0.2.0rc3/ha_services/cli_tools/dict_utils.py` & `ha-services-0.3.0/ha_services/cli_tools/dict_utils.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/cli_tools/path_utils.py` & `ha-services-0.3.0/ha_services/cli_tools/path_utils.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/cli_tools/rich_utils.py` & `ha-services-0.3.0/ha_services/cli_tools/rich_utils.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/cli_tools/test_utils/assertion.py` & `ha-services-0.3.0/ha_services/cli_tools/test_utils/assertion.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,8 +24,8 @@
             content='\n\n'.join(missing),
         )
         raise AssertionError(f'assert_in(): {len(missing)} parts not found in content, see output above')
 
 
 def assert_startswith(text, prefix):
     if not text.startswith(prefix):
-        raise AssertionError(f'{text!r} does not starts with: {prefix!r}')
+        raise AssertionError(f'{prefix=!r} is not at the beginning of: {text!r}')
```

### Comparing `ha-services-0.2.0rc3/ha_services/cli_tools/test_utils/environment_fixtures.py` & `ha-services-0.3.0/ha_services/cli_tools/test_utils/environment_fixtures.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/cli_tools/tests/test_environ_fixtures.py` & `ha-services-0.3.0/ha_services/cli_tools/tests/test_environ_fixtures.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/cli_tools/tests/test_path_utils.py` & `ha-services-0.3.0/ha_services/cli_tools/tests/test_path_utils.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/example.py` & `ha-services-0.3.0/ha_services/example.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,21 +57,21 @@
     # Information about the MQTT server:
     mqtt: dataclasses = dataclasses.field(default_factory=MqttSettings)
 
     # Example "app" data:
     app: dataclasses = dataclasses.field(default_factory=MqttExampleValues)
 
 
-def publish_forever(*, user_settings: DemoSettings, verbose):
+def publish_forever(*, user_settings: DemoSettings, verbosity: int):
     """
     Publish "something" to MQTT server. It's just a DEMO ;)
     """
     publisher = HaMqttPublisher(
         settings=user_settings.mqtt,
-        verbose=verbose,
+        verbosity=verbosity,
         config_count=1,  # Send every time the config
     )
 
     while True:
         # Just collect something that we can send:
         usage = resource.getrusage(resource.RUSAGE_SELF)
         values = [
```

### Comparing `ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/converter.py` & `ha-services-0.3.0/ha_services/mqtt4homeassistant/converter.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/data_classes.py` & `ha-services-0.3.0/ha_services/mqtt4homeassistant/data_classes.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/mqtt.py` & `ha-services-0.3.0/ha_services/mqtt4homeassistant/mqtt.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,38 +18,38 @@
 def get_client_id():
     hostname = socket.gethostname()
     client_id = f'ha_services v{__version__} on {hostname}'
     return client_id
 
 
 class OnConnectCallback:
-    def __init__(self, verbose: bool = True):
-        self.verbose = verbose
+    def __init__(self, verbosity: int):
+        self.verbosity = verbosity
 
     def __call__(self, client, userdata, flags, rc):
-        if self.verbose:
+        if self.verbosity:
             print(f'MQTT broker connect result code: {rc}', end=' ')
 
         if rc == 0:
-            if self.verbose:
+            if self.verbosity:
                 print('[green]OK')
         else:
             print('\n[red]MQTT Connection not successful!')
             print('[yellow]Please check your credentials\n')
             raise RuntimeError(f'MQTT connection result code {rc} is not 0')
 
-        if self.verbose:
+        if self.verbosity:
             print(f'\t{userdata=}')
             print(f'\t{flags=}')
 
 
-def get_connected_client(settings: MqttSettings, verbose: bool = True, timeout=10):
+def get_connected_client(settings: MqttSettings, verbosity: int, timeout=10):
     client_id = get_client_id()
 
-    if verbose:
+    if verbosity:
         print(f'\nConnect [cyan]{settings.host}:{settings.port}[/cyan] as "[magenta]{client_id}[/magenta]"', end='...')
 
     socket.setdefaulttimeout(timeout)  # Sadly: Timeout will not used in getaddrinfo()!
     try:
         info = socket.getaddrinfo(settings.host, settings.port)
     except socket.gaierror as err:
         human_error(
@@ -57,53 +57,53 @@
             title=f'[red]Error get address info from: [cyan]{settings.host}:{settings.port}[/cyan]',
             exception=err,
             exit_code=1,
         )
     else:
         if not info:
             print('[red]Resolve error: No info!')
-        elif verbose:
+        elif verbosity:
             print('Host/port test [green]OK')
 
     mqttc = mqtt.Client(client_id=client_id)
-    mqttc.on_connect = OnConnectCallback(verbose=verbose)
+    mqttc.on_connect = OnConnectCallback(verbosity=verbosity)
     mqttc.enable_logger(logger=logger)
 
     if settings.user_name and settings.password:
-        if verbose:
+        if verbosity:
             print(
                 f'login with user: {anonymize(settings.user_name)} password:{anonymize(settings.password)}',
                 end='...',
             )
         mqttc.username_pw_set(settings.user_name, settings.password)
 
     mqttc.connect(settings.host, port=settings.port)
 
-    if verbose:
+    if verbosity:
         print('[green]OK')
     return mqttc
 
 
 class HaMqttPublisher:
-    def __init__(self, settings: MqttSettings, verbose: bool = True, config_count: int = 10):
-        self.verbose = verbose
-        self.mqttc = get_connected_client(settings=settings, verbose=verbose)
+    def __init__(self, settings: MqttSettings, verbosity: int = 0, config_count: int = 10):
+        self.verbosity = verbosity
+        self.mqttc = get_connected_client(settings=settings, verbosity=verbosity)
         self.mqttc.loop_start()
 
         self.config_count = config_count
         self.send_count = 0
 
     def publish(self, *, topic: str, payload: dict) -> None:
-        if self.verbose:
+        if self.verbosity:
             print('_' * 100)
             print(f'[yellow]Publish MQTT topic: [blue]{topic} [grey](Send count: {self.send_count})')
             pprint(payload)
 
         info: mqtt.MQTTMessageInfo = self.mqttc.publish(topic=topic, payload=json.dumps(payload))
-        if self.verbose:
+        if self.verbosity:
             print('publish result:', info)
 
     def publish2homeassistant(self, *, ha_mqtt_payload: HaMqttPayload) -> None:
         log_prefix = f'{self.send_count=} ({self.config_count=})'
 
         if self.send_count == 0 or self.send_count % self.config_count == 0:
             logger.debug(f'{log_prefix} send {len(ha_mqtt_payload.configs)} configs')
```

### Comparing `ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/tests/test_converter.py` & `ha-services-0.3.0/ha_services/mqtt4homeassistant/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/systemd/api.py` & `ha-services-0.3.0/ha_services/systemd/api.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/systemd/data_classes.py` & `ha-services-0.3.0/ha_services/systemd/data_classes.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/systemd/template.py` & `ha-services-0.3.0/ha_services/systemd/template.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/systemd/test_utils/mock_systemd_info.py` & `ha-services-0.3.0/ha_services/systemd/test_utils/mock_systemd_info.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/systemd/tests/test_api.py` & `ha-services-0.3.0/ha_services/systemd/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/systemd/tests/test_data_classes.py` & `ha-services-0.3.0/ha_services/systemd/tests/test_data_classes.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/systemd/tests/test_mock_systemd_info.py` & `ha-services-0.3.0/ha_services/systemd/tests/test_mock_systemd_info.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/systemd/tests/test_mock_systemd_info_mock_1.snapshot.toml` & `ha-services-0.3.0/ha_services/systemd/tests/test_mock_systemd_info_mock_1.snapshot.toml`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/systemd/tests/test_template.py` & `ha-services-0.3.0/ha_services/systemd/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/tests/test_project_setup.py` & `ha-services-0.3.0/ha_services/tests/test_project_setup.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/toml_settings/api.py` & `ha-services-0.3.0/ha_services/toml_settings/api.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/toml_settings/debug.py` & `ha-services-0.3.0/ha_services/toml_settings/debug.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/toml_settings/deserialize.py` & `ha-services-0.3.0/ha_services/toml_settings/deserialize.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/toml_settings/sensible_editor.py` & `ha-services-0.3.0/ha_services/toml_settings/sensible_editor.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/toml_settings/serialize.py` & `ha-services-0.3.0/ha_services/toml_settings/serialize.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/toml_settings/test_utils/data_class_utils.py` & `ha-services-0.3.0/ha_services/toml_settings/test_utils/data_class_utils.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/toml_settings/tests/fixtures.py` & `ha-services-0.3.0/ha_services/toml_settings/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/toml_settings/tests/test_demo_settings.py` & `ha-services-0.3.0/ha_services/toml_settings/tests/test_demo_settings.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/toml_settings/tests/test_deserialize.py` & `ha-services-0.3.0/ha_services/toml_settings/tests/test_deserialize.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/toml_settings/tests/test_serialize.py` & `ha-services-0.3.0/ha_services/toml_settings/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services/toml_settings/tests/test_test_utils.py` & `ha-services-0.3.0/ha_services/toml_settings/tests/test_test_utils.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/ha_services.egg-info/SOURCES.txt` & `ha-services-0.3.0/ha_services.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,35 +8,38 @@
 requirements.dev.txt
 requirements.txt
 .github/workflows/tests.yml
 ha_services/__init__.py
 ha_services/__main__.py
 ha_services/constants.py
 ha_services/example.py
-ha_services/log_setup.py
 ha_services.egg-info/PKG-INFO
 ha_services.egg-info/SOURCES.txt
 ha_services.egg-info/dependency_links.txt
 ha_services.egg-info/entry_points.txt
 ha_services.egg-info/requires.txt
 ha_services.egg-info/top_level.txt
 ha_services/cli/__init__.py
 ha_services/cli/cli_app.py
 ha_services/cli/dev.py
 ha_services/cli_tools/__init__.py
+ha_services/cli_tools/dev_tools.py
 ha_services/cli_tools/dict_utils.py
 ha_services/cli_tools/path_utils.py
 ha_services/cli_tools/rich_utils.py
+ha_services/cli_tools/verbosity.py
 ha_services/cli_tools/test_utils/__init__.py
 ha_services/cli_tools/test_utils/assertion.py
+ha_services/cli_tools/test_utils/cli_readme.py
 ha_services/cli_tools/test_utils/environment_fixtures.py
-ha_services/cli_tools/test_utils/mock_rich.py
+ha_services/cli_tools/test_utils/rich_test_utils.py
 ha_services/cli_tools/tests/__init__.py
 ha_services/cli_tools/tests/test_dict_utils.py
 ha_services/cli_tools/tests/test_environ_fixtures.py
+ha_services/cli_tools/tests/test_mock_rich.py
 ha_services/cli_tools/tests/test_path_utils.py
 ha_services/mqtt4homeassistant/__init__.py
 ha_services/mqtt4homeassistant/converter.py
 ha_services/mqtt4homeassistant/data_classes.py
 ha_services/mqtt4homeassistant/mqtt.py
 ha_services/mqtt4homeassistant/tests/__init__.py
 ha_services/mqtt4homeassistant/tests/test_converter.py
@@ -55,23 +58,25 @@
 ha_services/systemd/tests/test_data_classes.py
 ha_services/systemd/tests/test_mock_systemd_info.py
 ha_services/systemd/tests/test_mock_systemd_info_mock_1.snapshot.toml
 ha_services/systemd/tests/test_template.py
 ha_services/tests/__init__.py
 ha_services/tests/test_doctests.py
 ha_services/tests/test_project_setup.py
+ha_services/tests/test_readme.py
 ha_services/toml_settings/__init__.py
 ha_services/toml_settings/api.py
 ha_services/toml_settings/data_class_utils.py
 ha_services/toml_settings/debug.py
 ha_services/toml_settings/deserialize.py
 ha_services/toml_settings/exceptions.py
 ha_services/toml_settings/sensible_editor.py
 ha_services/toml_settings/serialize.py
 ha_services/toml_settings/test_utils/__init__.py
+ha_services/toml_settings/test_utils/cli_mock.py
 ha_services/toml_settings/test_utils/data_class_utils.py
 ha_services/toml_settings/tests/__init__.py
 ha_services/toml_settings/tests/fixtures.py
 ha_services/toml_settings/tests/test_demo_settings.py
 ha_services/toml_settings/tests/test_deserialize.py
 ha_services/toml_settings/tests/test_serialize.py
 ha_services/toml_settings/tests/test_test_utils.py
```

### Comparing `ha-services-0.2.0rc3/pyproject.toml` & `ha-services-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/requirements.dev.txt` & `ha-services-0.3.0/requirements.dev.txt`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc3/requirements.txt` & `ha-services-0.3.0/requirements.txt`

 * *Files identical despite different names*

