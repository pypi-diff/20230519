# Comparing `tmp/sealights-python-agent-1.0.5.tar.gz` & `tmp/sealights-python-agent-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sealights-python-agent-1.0.5.tar", last modified: Sun Jul 10 11:37:14 2022, max compression
+gzip compressed data, was "dist/sealights-python-agent-1.0.6.tar", last modified: Tue Aug 30 13:30:03 2022, max compression
```

## Comparing `sealights-python-agent-1.0.5.tar` & `sealights-python-agent-1.0.6.tar`

### file list

```diff
@@ -1,305 +1,306 @@
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/
--rw-r--r--   0 jenkins    (498) jenkins    (497)    13769 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/admin.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/bootstrap/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1171 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/bootstrap/sitecustomize.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/bootstrap/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/common/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     8417 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/common/configuration_manager.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1787 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/common/environment_variables_resolver.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2676 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/common/config_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2395 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/common/constants.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/common/autoupgrade/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3132 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/common/autoupgrade/autoupgrade_manager.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/common/autoupgrade/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/common/token/
--rw-r--r--   0 jenkins    (498) jenkins    (497)      353 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/common/token/token_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1328 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/common/token/token_parser.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/common/token/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/common/http/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     9695 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/common/http/backend_proxy.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2422 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/common/http/sl_routes.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1838 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/common/http/requests_wrapper.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/common/http/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/common/build_session/
--rw-r--r--   0 jenkins    (498) jenkins    (497)      343 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/common/build_session/build_session_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/common/build_session/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/common/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/common/log/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2923 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/common/log/sealights_logging.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/common/log/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     5183 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/utils.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/test_listener/
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/test_listener/queues/
--rw-r--r--   0 jenkins    (498) jenkins    (497)      821 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/queues/events_queue.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/queues/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      940 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/queues/footprints_queue.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/test_listener/web_frameworks/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1280 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/web_frameworks/bottle_framework.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1260 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/web_frameworks/flask_framework.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)       51 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/web_frameworks/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/test_listener/coloring/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1396 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/coloring/requests_helper.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2218 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/coloring/selenium_helper.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      682 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/coloring/urllib2_helper.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)       68 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/coloring/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/test_listener/managers/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4899 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/managers/code_coverage_manager.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3191 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/managers/agent_manager.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     7483 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/managers/footprints_manager.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2791 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/managers/events_manager.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/managers/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      453 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/footprints_collector.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2551 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/sealights_api.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/test_listener/services/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     6000 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/services/footprints_service.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1162 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/services/events_service.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/services/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1026 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/line_footprints_collector.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      744 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/utils.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3654 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/method_footprints_collector.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/test_listener/integrations/
--rw-r--r--   0 jenkins    (498) jenkins    (497)      560 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/integrations/freezegun_patcher.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2792 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/integrations/multiprocessing_patcher.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      779 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/integrations/pytest_xdist_helper.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4928 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/integrations/unittest_helper.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4371 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/integrations/nose_helper.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     6774 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/integrations/pytest_helper.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/integrations/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/test_listener/entities/
--rw-r--r--   0 jenkins    (498) jenkins    (497)      239 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/entities/upload_reports_request.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      130 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/entities/footprint_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      308 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/entities/footprints_request.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      337 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/entities/events_request.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      410 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/entities/start_execution_request.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      388 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/entities/logs_request.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      608 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/entities/upload_reports_metadata.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      223 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/entities/test_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/entities/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      197 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/entities/file_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      223 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/entities/app_data.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/test_listener/executors/
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/test_listener/executors/test_frameworks/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1402 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/executors/test_frameworks/agent_execution.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1958 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/executors/test_frameworks/pytest_execution.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1135 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/executors/test_frameworks/unittest_execution.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/executors/test_frameworks/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1200 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/executors/test_frameworks/nose_execution.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2175 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/executors/upload_reports.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      395 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/executors/end_execution.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      836 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/executors/start_execution.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2068 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/executors/run.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      849 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/executors/send_footprints.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/executors/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      523 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/executors/anonymous_execution.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1604 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/test_listener/state_tracker.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3113 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/build_scanner/
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/build_scanner/scm/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     7711 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/build_scanner/scm/git_integration.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2517 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/build_scanner/scm/scm_info.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/build_scanner/scm/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1581 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/build_scanner/file_scanner.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2412 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/build_scanner/visitors.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     5864 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/build_scanner/app.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2281 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/build_scanner/ast_utils.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3794 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/build_scanner/method_hasher.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/build_scanner/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/build_scanner/entities/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2327 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/build_scanner/entities/environment_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/build_scanner/entities/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/build_scanner/entities/v3/
--rw-r--r--   0 jenkins    (498) jenkins    (497)      263 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/build_scanner/entities/v3/build_mapping_request.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      620 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/build_scanner/entities/v3/method_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)       91 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/build_scanner/entities/v3/code_element_with_hash.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/build_scanner/entities/v3/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      625 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/build_scanner/entities/v3/file_data.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/build_scanner/executors/
--rw-r--r--   0 jenkins    (498) jenkins    (497)      652 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/build_scanner/executors/build.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1836 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/build_scanner/executors/config.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/build_scanner/executors/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      625 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/init.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/packages/
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/packages/blinker/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4479 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/blinker/_utilities.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    16341 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/blinker/base.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     9223 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/blinker/_saferef.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      322 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/blinker/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/packages/requests/
--rw-r--r--   0 jenkins    (498) jenkins    (497)    22041 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/requests/adapters.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3456 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/requests/exceptions.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1003 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/requests/packages.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    35166 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/requests/models.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      441 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/requests/__version__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      475 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/requests/certs.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     6402 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/requests/api.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      757 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/requests/hooks.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    18430 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/requests/cookies.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    10207 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/requests/auth.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    33321 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/requests/utils.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4071 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/requests/help.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1096 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/requests/_internal_utils.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     5039 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/requests/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4188 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/requests/status_codes.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3005 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/requests/structures.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2081 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/requests/compat.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    29835 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/requests/sessions.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    32452 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/six.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/packages/certifi/
--rw-r--r--   0 jenkins    (498) jenkins    (497)   276001 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/certifi/cacert.pem
--rw-r--r--   0 jenkins    (498) jenkins    (497)      243 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/certifi/__main__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)       96 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/certifi/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2537 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/certifi/core.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/packages/jwt/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     9186 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/jwt/api_jws.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      963 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/jwt/exceptions.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1914 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/jwt/jwks_client.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     8025 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/jwt/api_jwt.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    22392 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/jwt/algorithms.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3114 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/jwt/api_jwk.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3993 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/jwt/utils.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1605 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/jwt/help.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1548 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/jwt/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/packages/astunparse/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1222 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/astunparse/__main__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    20121 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/astunparse/unparser36.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1435 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/astunparse/printer.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    26742 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/astunparse/unparser.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      466 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/astunparse/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    20676 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/astunparse/unparser37.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/packages/astor/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2917 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/astor/string_repr.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    32032 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/astor/code_gen.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        6 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/astor/VERSION
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3268 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/astor/file_util.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     7373 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/astor/source_repr.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     6542 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/astor/node_util.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2291 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/astor/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     6741 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/astor/rtrip.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     6020 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/astor/tree_walk.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3191 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/astor/op_util.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      204 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/astor/codegen.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)   107685 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/typing_extensions.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/packages/importlib_metadata/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1862 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/importlib_metadata/_adapters.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2166 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/importlib_metadata/_text.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      743 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/importlib_metadata/_collections.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1826 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/importlib_metadata/_compat.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2895 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/importlib_metadata/_functools.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1154 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/importlib_metadata/_meta.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/importlib_metadata/py.typed
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2068 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/importlib_metadata/_itertools.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    30533 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/importlib_metadata/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     8425 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/zipp.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/packages/click/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1353 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/click/_textwrap.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     9167 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/click/exceptions.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    16063 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/click/testing.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    35114 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/click/types.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    23451 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/click/_termui_impl.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    18810 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/click/_compat.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3201 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/click/_unicodefun.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     7860 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/click/_winconsole.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1983 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/click/globals.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    18956 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/click/utils.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    19066 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/click/parser.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3243 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/click/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)   111454 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/click/core.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    14901 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/click/decorators.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     9706 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/click/formatting.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    18003 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/click/shell_completion.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    28873 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/click/termui.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/
--rw-r--r--   0 jenkins    (498) jenkins    (497)    11076 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/cd.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3384 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/legacy.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    13303 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/models.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/assets/
--rw-r--r--   0 jenkins    (498) jenkins    (497)    25485 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/assets/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/cli/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     9364 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/cli/normalizer.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/cli/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    20303 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/api.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/py.typed
--rw-r--r--   0 jenkins    (498) jenkins    (497)       80 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/version.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    18191 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/md.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     9308 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/utils.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1790 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    19449 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/constant.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/packages/semantic_version/
--rw-r--r--   0 jenkins    (498) jenkins    (497)    48115 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/semantic_version/base.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      546 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/semantic_version/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3510 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/semantic_version/django_fields.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/packages/idna/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3374 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/idna/codec.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1881 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/idna/intranges.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)   204400 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/idna/uts46data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)       21 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/idna/package_data.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    44025 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/idna/idnadata.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      849 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/idna/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    12795 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/idna/core.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      321 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/idna/compat.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     8217 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/exceptions.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    28276 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/response.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     8579 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/fields.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    39013 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/connectionpool.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)       63 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/_version.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    19786 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/poolmanager.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    10811 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/_collections.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2440 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/filepost.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    20070 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/connection.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     5758 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     6895 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/ssltransport.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3510 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/response.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1605 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/proxy.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    17165 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/ssl_.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     5404 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/wait.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    10003 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/timeout.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4901 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/connection.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      498 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/queue.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4225 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/request.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    22001 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/retry.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1155 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    14057 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/url.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     5985 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/request.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/contrib/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     4538 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/contrib/ntlmpool.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/contrib/_securetransport/
--rw-r--r--   0 jenkins    (498) jenkins    (497)    13922 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    17632 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    34433 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/contrib/securetransport.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    16901 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/contrib/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      957 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)    11010 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/contrib/appengine.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     7097 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/contrib/socks.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2763 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/packages/
--rw-r--r--   0 jenkins    (498) jenkins    (497)    34666 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/packages/six.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/packages/backports/
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1417 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/packages/backports/makefile.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/packages/backports/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/urllib3/packages/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/python_agent/packages/freezegun/
--rw-r--r--   0 jenkins    (498) jenkins    (497)    25911 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/freezegun/api.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      421 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/freezegun/_async.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)      302 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/python_agent/packages/freezegun/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)     2305 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/LICENSE.txt
-drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/sealights_python_agent.egg-info/
--rw-r--r--   0 jenkins    (498) jenkins    (497)        1 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/sealights_python_agent.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (498) jenkins    (497)       95 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/sealights_python_agent.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (498) jenkins    (497)    11818 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/sealights_python_agent.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (498) jenkins    (497)      386 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/sealights_python_agent.egg-info/requires.txt
--rw-r--r--   0 jenkins    (498) jenkins    (497)       13 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/sealights_python_agent.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3655 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/sealights_python_agent.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (498) jenkins    (497)      433 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/requirements.txt
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1891 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/CHANGES.rst
--rw-r--r--   0 jenkins    (498) jenkins    (497)     1043 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/README.rst
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3655 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/PKG-INFO
--rw-r--r--   0 jenkins    (498) jenkins    (497)     3799 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/setup.py
--rw-r--r--   0 jenkins    (498) jenkins    (497)       67 2022-07-10 11:37:14.000000 sealights-python-agent-1.0.5/setup.cfg
--rw-r--r--   0 jenkins    (498) jenkins    (497)      138 2022-07-10 11:37:13.000000 sealights-python-agent-1.0.5/MANIFEST.in
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    13769 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/admin.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/bootstrap/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1171 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/bootstrap/sitecustomize.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/bootstrap/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/common/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     8417 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/configuration_manager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1787 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/environment_variables_resolver.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2740 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/config_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2767 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/constants.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/common/autoupgrade/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3132 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/autoupgrade/autoupgrade_manager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/autoupgrade/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/common/token/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      353 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/token/token_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1328 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/token/token_parser.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/token/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/common/http/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     7672 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/http/backend_proxy.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2422 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/http/sl_routes.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1838 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/http/requests_wrapper.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/http/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/common/build_session/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      343 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/build_session/build_session_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/build_session/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/common/log/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2923 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/log/sealights_logging.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/common/log/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     5183 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/utils.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/test_listener/
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/test_listener/queues/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      821 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/queues/events_queue.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/queues/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      940 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/queues/footprints_queue.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/test_listener/web_frameworks/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1280 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/web_frameworks/bottle_framework.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1260 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/web_frameworks/flask_framework.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       51 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/web_frameworks/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/test_listener/coloring/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1396 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/coloring/requests_helper.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2218 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/coloring/selenium_helper.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      682 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/coloring/urllib2_helper.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       68 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/coloring/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/test_listener/managers/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4000 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/managers/tia_manager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4899 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/managers/code_coverage_manager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2989 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/managers/agent_manager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     7483 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/managers/footprints_manager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2791 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/managers/events_manager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/managers/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      453 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/footprints_collector.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2551 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/sealights_api.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/test_listener/services/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     6000 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/services/footprints_service.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1200 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/services/events_service.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/services/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1026 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/line_footprints_collector.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      744 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/utils.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3654 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/method_footprints_collector.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/test_listener/integrations/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      560 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/integrations/freezegun_patcher.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2806 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/integrations/multiprocessing_patcher.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      779 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/integrations/pytest_xdist_helper.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4928 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/integrations/unittest_helper.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4371 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/integrations/nose_helper.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     6774 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/integrations/pytest_helper.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/integrations/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/test_listener/entities/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      239 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/entities/upload_reports_request.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      130 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/entities/footprint_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      308 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/entities/footprints_request.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      417 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/entities/events_request.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      410 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/entities/start_execution_request.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      388 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/entities/logs_request.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      608 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/entities/upload_reports_metadata.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      223 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/entities/test_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/entities/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      197 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/entities/file_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      223 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/entities/app_data.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/test_frameworks/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1402 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/test_frameworks/agent_execution.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1958 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/test_frameworks/pytest_execution.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1135 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/test_frameworks/unittest_execution.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/test_frameworks/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1200 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/test_frameworks/nose_execution.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2175 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/upload_reports.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      395 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/end_execution.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      836 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/start_execution.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2068 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/run.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      849 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/send_footprints.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      523 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/executors/anonymous_execution.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1604 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/test_listener/state_tracker.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3113 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/scm/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     7711 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/scm/git_integration.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2517 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/scm/scm_info.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/scm/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1581 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/file_scanner.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2419 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/visitors.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     5864 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/app.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2281 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/ast_utils.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3794 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/method_hasher.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/entities/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2327 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/entities/environment_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/entities/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/entities/v3/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      263 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/entities/v3/build_mapping_request.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      620 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/entities/v3/method_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       91 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/entities/v3/code_element_with_hash.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/entities/v3/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      625 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/entities/v3/file_data.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/executors/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      652 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/executors/build.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1836 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/executors/config.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/build_scanner/executors/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      632 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/init.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/blinker/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4479 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/blinker/_utilities.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    16341 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/blinker/base.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     9223 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/blinker/_saferef.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      322 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/blinker/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    22041 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/adapters.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3456 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/exceptions.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1003 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/packages.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    35166 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/models.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      441 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/__version__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      475 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/certs.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     6402 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/api.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      757 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/hooks.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    18430 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/cookies.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    10207 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/auth.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    33321 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/utils.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4071 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/help.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1096 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/_internal_utils.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     5039 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4188 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/status_codes.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3005 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/structures.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2081 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/compat.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    29835 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/requests/sessions.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    32452 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/six.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/certifi/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)   276001 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/certifi/cacert.pem
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      243 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/certifi/__main__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       96 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/certifi/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2537 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/certifi/core.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/jwt/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     9186 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/jwt/api_jws.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      963 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/jwt/exceptions.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1914 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/jwt/jwks_client.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     8025 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/jwt/api_jwt.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    22392 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/jwt/algorithms.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3114 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/jwt/api_jwk.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3993 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/jwt/utils.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1605 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/jwt/help.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1548 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/jwt/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/astunparse/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1222 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astunparse/__main__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    20121 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astunparse/unparser36.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1435 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astunparse/printer.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    26742 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astunparse/unparser.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      466 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astunparse/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    20676 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astunparse/unparser37.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/astor/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2917 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astor/string_repr.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    32032 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astor/code_gen.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        6 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astor/VERSION
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3268 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astor/file_util.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     7373 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astor/source_repr.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     6542 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astor/node_util.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2291 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astor/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     6741 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astor/rtrip.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     6020 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astor/tree_walk.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3191 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astor/op_util.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      204 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/astor/codegen.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)   107685 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/typing_extensions.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1862 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_adapters.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2166 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_text.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      743 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_collections.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1826 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_compat.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2895 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_functools.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1154 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_meta.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/py.typed
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2068 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_itertools.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    30533 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     8425 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/zipp.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/click/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1353 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/_textwrap.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     9167 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/exceptions.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    16063 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/testing.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    35114 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/types.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    23451 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/_termui_impl.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    18810 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/_compat.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3201 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/_unicodefun.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     7860 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/_winconsole.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1983 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/globals.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    18956 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/utils.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    19066 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/parser.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3243 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)   111454 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/core.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    14901 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/decorators.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     9706 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/formatting.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    18003 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/shell_completion.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    28873 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/click/termui.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    11076 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/cd.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3384 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/legacy.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    13303 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/models.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/assets/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    25485 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/assets/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/cli/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     9364 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/cli/normalizer.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/cli/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    20303 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/api.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/py.typed
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       80 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/version.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    18191 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/md.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     9308 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/utils.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1790 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    19449 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/constant.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/semantic_version/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    48115 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/semantic_version/base.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      546 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/semantic_version/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3510 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/semantic_version/django_fields.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/idna/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3374 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/idna/codec.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1881 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/idna/intranges.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)   204400 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/idna/uts46data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       21 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/idna/package_data.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    44025 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/idna/idnadata.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      849 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/idna/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    12795 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/idna/core.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      321 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/idna/compat.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     8217 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/exceptions.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    28276 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/response.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     8579 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/fields.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    39013 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/connectionpool.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       63 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/_version.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    19786 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/poolmanager.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    10811 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/_collections.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2440 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/filepost.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    20070 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/connection.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     5758 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     6895 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/ssltransport.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3510 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/response.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1605 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/proxy.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    17165 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/ssl_.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     5404 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/wait.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    10003 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/timeout.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4901 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/connection.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      498 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/queue.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4225 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/request.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    22001 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/retry.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1155 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    14057 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/url.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     5985 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/request.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     4538 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/ntlmpool.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/_securetransport/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    13922 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    17632 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    34433 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/securetransport.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    16901 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      957 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    11010 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/appengine.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     7097 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/socks.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2763 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/packages/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    34666 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/packages/six.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/packages/backports/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1417 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/urllib3/packages/__init__.py
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/python_agent/packages/freezegun/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    25911 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/freezegun/api.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      421 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/freezegun/_async.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      302 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/python_agent/packages/freezegun/__init__.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     2305 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/LICENSE.txt
+drwxr-xr-x   0 jenkins    (498) jenkins    (497)        0 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/sealights_python_agent.egg-info/
+-rw-r--r--   0 jenkins    (498) jenkins    (497)        1 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/sealights_python_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       95 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/sealights_python_agent.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (498) jenkins    (497)    11869 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/sealights_python_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      386 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/sealights_python_agent.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       13 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/sealights_python_agent.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3717 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/sealights_python_agent.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      433 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/requirements.txt
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1992 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/CHANGES.rst
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     1004 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/README.rst
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3717 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/PKG-INFO
+-rw-r--r--   0 jenkins    (498) jenkins    (497)     3808 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/setup.py
+-rw-r--r--   0 jenkins    (498) jenkins    (497)       67 2022-08-30 13:30:03.000000 sealights-python-agent-1.0.6/setup.cfg
+-rw-r--r--   0 jenkins    (498) jenkins    (497)      138 2022-08-30 13:30:02.000000 sealights-python-agent-1.0.6/MANIFEST.in
```

### Comparing `sealights-python-agent-1.0.5/python_agent/admin.py` & `sealights-python-agent-1.0.6/python_agent/admin.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/bootstrap/sitecustomize.py` & `sealights-python-agent-1.0.6/python_agent/bootstrap/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/common/configuration_manager.py` & `sealights-python-agent-1.0.6/python_agent/common/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/common/environment_variables_resolver.py` & `sealights-python-agent-1.0.6/python_agent/common/environment_variables_resolver.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/common/config_data.py` & `sealights-python-agent-1.0.6/python_agent/common/config_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from python_agent.common import constants
-from python_agent.common.constants import DEFAULT_WORKSPACEPATH
+from python_agent.common.constants import DEFAULT_WORKSPACEPATH, TestSelectionStatus
 from python_agent.utils import to_str_obj
 
 class ScmConfigArgs(object):
     def __init__(self, scm_provider, scm_version, scm_base_url, scm_type):
         self.scmProvider = scm_provider
         self.scmVersion = scm_version
         self.scmBaseUrl = scm_base_url
@@ -39,15 +39,16 @@
         self.commitHistoryLength = constants.DEFAULT_COMMIT_LOG_SIZE
         self.tokenFile = None
         self.buildSessionIdFile = None
         self.covReport = None
         self.perTest = True
         self.interval = constants.INTERVAL_IN_MILLISECONDS
         self.intervalSeconds = constants.INTERVAL_IN_SECONDS
-        self.testSelection = {"enable":True, "interval":constants.TEST_RECOMMENDATION.interval_sec, "timeout":constants.TEST_RECOMMENDATION.timeout_sec}
+        self.testSelection = {"enable": True, "interval": constants.TEST_RECOMMENDATION.interval_sec, "timeout": constants.TEST_RECOMMENDATION.timeout_sec}
+        self.testSelectionStatus = None
         self.test_selection_enable = True
         self.isDisabled = False
 
     def apply_scm_args(self, scm_args):
         """
         Overrides scm properties by not None values of scm_args
         None scm_args are ignored
```

### Comparing `sealights-python-agent-1.0.5/python_agent/common/constants.py` & `sealights-python-agent-1.0.6/python_agent/common/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from enum import Enum
+
 import os
 import sys
 
 PREFIXES = ["sl.", "sl_", "SL.", "SL_"]
 TOKEN_FILE = "sltoken.txt"
 BUILD_SESSION_ID_FILE = "buildSessionId.txt"
 CONFIG_ENV_VARIABLE = "sl_configuration"
@@ -71,13 +73,22 @@
     "kwargannotation" : None
 }
 
 class TEST_RECOMMENDATION(object):
     timeout_sec = 60
     interval_sec = 5
     RSS = 'recommendationSetStatus'
-    RSS_NOT_READY = 'notready'
+    RSS_NOT_READY = 'notReady'
     RSS_NO_HISTORY = 'noHistory'
     RSS_READY = 'ready'
     RSS_ERROR = 'error'
+    RSS_WONT_BE_READY = 'wontBeReady'
     TEST_SELECTION_ENABLED = "testSelectionEnabled"
 
+
+class TestSelectionStatus(str, Enum):
+    RECOMMENDED_TESTS = "recommendedTests"
+    DISABLED = "disabled"
+    DISABLED_BY_CONFIGURATION = "disabledByConfiguration"
+    RECOMMENDATIONS_TIMEOUT = "recommendationsTimeout"
+    RECOMMENDATIONS_TIMEOUT_SERVER = "recommendationsTimeoutOnServer"
+    ERROR = "error"
```

### Comparing `sealights-python-agent-1.0.5/python_agent/common/autoupgrade/autoupgrade_manager.py` & `sealights-python-agent-1.0.6/python_agent/common/autoupgrade/autoupgrade_manager.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/common/token/token_parser.py` & `sealights-python-agent-1.0.6/python_agent/common/token/token_parser.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/common/http/backend_proxy.py` & `sealights-python-agent-1.0.6/python_agent/common/http/backend_proxy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import json
 import logging
-import time
 
+from python_agent import __package_name__ as PACKAGE_NAME
+from python_agent import __version__ as VERSION
 from python_agent.common.build_session.build_session_data import BuildSessionData
 from python_agent.common.http.requests_wrapper import Requests
 from python_agent.common.http.sl_routes import SLRoutes
 from python_agent.packages import requests
-from python_agent import __package_name__ as PACKAGE_NAME
-from python_agent import __version__ as VERSION
 from python_agent.packages.requests import HTTPError
 
-from python_agent.common.constants import TEST_RECOMMENDATION
-
 log = logging.getLogger(__name__)
 
 
 class BackendProxy(object):
 
     def __init__(self, config_data):
         self.requests = Requests(config_data)
@@ -140,63 +137,25 @@
             else:
                 log.warning("Failed getting remote configuration. Error: %s" % str(e))
         except Exception as e:
             log.warning("Failed getting remote configuration. Error: %s" % str(e))
 
         return {}
 
-    def get_recommendations(self, config_data):
-        interval_sec = config_data.testSelection["interval"]
-        timeout_sec = config_data.testSelection["timeout"]
-        test_recommendations = {
-            "testSelectionEnabled": False,
-            "recommendedTests": [],
-            "excludedTests": []
-        }
-        if (config_data.testSelection["enable"]):
-            if (interval_sec < 0):
-                interval_sec = TEST_RECOMMENDATION.interval_sec
-            if (timeout_sec < 0):
-                timeout_sec = TEST_RECOMMENDATION.timeout_sec
-            if (timeout_sec == 0 or interval_sec == 0):
-                test_recommendations = self.try_get_recommendations(config_data.buildSessionId) or dict()
-                return test_recommendations
-            
-            n_retry = 0
-            while timeout_sec > 0:
-                test_recommendations = self.try_get_recommendations(config_data.buildSessionId) or dict()
-                if not (self.is_selection_enabled_and_not_ready(test_recommendations)):
-                    return test_recommendations
-                n_retry += 1
-                time.sleep(interval_sec)
-                timeout_sec -= interval_sec
-                log.debug("Failed to receive test recommendations. remain %d retry" % (timeout_sec / interval_sec))
-            else:
-                log.warning("did not get test recommendations after %d tries and %d seconds" % (n_retry, timeout_sec))
-                return test_recommendations
-        else:
-            log.warning("Test recommendations disabled")
-            return test_recommendations
-
     def try_get_recommendations(self, build_session_id):
         url = SLRoutes.test_exclusions_v3(build_session_id, self.config_data.testStage)
         try:
             response = self.requests.get(url)
             response.raise_for_status()
             return response.json()
 
         except Exception as e:
             log.warning("failed get recommendation tests from server URL: %s. Error: %s" % (url, str(e)))
             return {}
 
-    def is_selection_enabled_and_not_ready(self, test_recommendations):
-        return test_recommendations.get(TEST_RECOMMENDATION.TEST_SELECTION_ENABLED) and\
-               test_recommendations.get(TEST_RECOMMENDATION.RSS) and\
-               test_recommendations[TEST_RECOMMENDATION.RSS].lower() == TEST_RECOMMENDATION.RSS_NOT_READY
-
     def get_build_session_from_labid(self, labid):
         url = SLRoutes.lab_ids_active_build_session_v1(labid)
         try:
             response = self.requests.get(url)
             response.raise_for_status()
             build_session_dict = response.json()
             return self._create_build_session_data(build_session_dict)
```

### Comparing `sealights-python-agent-1.0.5/python_agent/common/http/sl_routes.py` & `sealights-python-agent-1.0.6/python_agent/common/http/sl_routes.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/common/http/requests_wrapper.py` & `sealights-python-agent-1.0.6/python_agent/common/http/requests_wrapper.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/common/log/sealights_logging.py` & `sealights-python-agent-1.0.6/python_agent/common/log/sealights_logging.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/utils.py` & `sealights-python-agent-1.0.6/python_agent/utils.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/queues/events_queue.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/queues/events_queue.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/queues/footprints_queue.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/queues/footprints_queue.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/web_frameworks/bottle_framework.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/web_frameworks/bottle_framework.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/web_frameworks/flask_framework.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/web_frameworks/flask_framework.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/coloring/requests_helper.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/coloring/requests_helper.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/coloring/selenium_helper.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/coloring/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/coloring/urllib2_helper.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/coloring/urllib2_helper.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/managers/code_coverage_manager.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/managers/code_coverage_manager.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/managers/agent_manager.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/managers/agent_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from python_agent.common.http.backend_proxy import BackendProxy
 from python_agent.packages.six import add_metaclass
 from python_agent.test_listener.integrations.freezegun_patcher import FreezeGunPatcher
 from python_agent.test_listener.integrations.pytest_xdist_helper import override_xdist_exit_timeout
 from python_agent.test_listener.managers.events_manager import EventsManager
 from python_agent.test_listener.managers.footprints_manager import FootprintsManager
+from python_agent.test_listener.managers.tia_manager import TIAManager
 from python_agent.test_listener.state_tracker import StateTracker
 from python_agent.test_listener.utils import Singleton
 
 log = logging.getLogger(__name__)
 
 @add_metaclass(Singleton)
 class AgentManager(object):
@@ -26,28 +27,24 @@
         self.config_data = config_data
         self.is_master = is_master
         self.pid = os.getpid()
         self.backend_proxy = BackendProxy(config_data)
         self.state_tracker = StateTracker(config_data)
         self.footprints_manager = FootprintsManager(config_data, self.backend_proxy)
         self.events_manager = EventsManager(config_data, self.backend_proxy)
+        self.tia_manager = TIAManager(config_data)
         self.footprints_manager.start()
         self.events_manager.start()
         atexit.register(self.shutdown)
         self.agent_started()
         self.register_integrations()
         # self.register_uwsgi_at_exit()
 
     def get_excluded_tests(self):
-        test_recommendations = self.backend_proxy.get_recommendations(self.config_data)
-        if (self.config_data.testSelection["enable"] and
-                test_recommendations.get('testSelectionEnabled', False) and
-                len(test_recommendations.get('excludedTests', [])) > 0):
-            return test_recommendations.get('excludedTests', [])
-        return []
+        return self.tia_manager.get_excluded_tests()
 
     def create_execution_id(self):
         return str(uuid.uuid4())
 
     def push_event(self, event):
         event["timestamp"] = int(round(time.time() * 1000))
         self.events_manager.push_event(event)
```

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/managers/footprints_manager.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/managers/footprints_manager.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/managers/events_manager.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/managers/events_manager.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/sealights_api.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/sealights_api.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/services/footprints_service.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/services/footprints_service.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/services/events_service.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/services/events_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,13 +13,13 @@
 
     def send_events(self, events):
         try:
             log.info("Sending Events. Number Of Events: %s" % len(events))
             environment_data = EnvironmentData(self.config_data.labId, self.config_data.testStage)
             events_request = EventsRequest(self.config_data.customerId, self.config_data.appName,
                                            self.config_data.branchName, self.config_data.buildName, environment_data,
-                                           events)
+                                           events, self.config_data.testSelectionStatus)
             self.backend_proxy.send_events(events_request)
             log.info("Sent Events to Server. Number Of Events: %s" % len(events))
         except Exception as e:
             log.exception("Failed Sending Events. Number Of Events: %s. error: %s" % (len(events), str(e)))
             raise
```

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/line_footprints_collector.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/line_footprints_collector.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/utils.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/utils.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/method_footprints_collector.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/method_footprints_collector.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/integrations/freezegun_patcher.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/integrations/freezegun_patcher.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/integrations/multiprocessing_patcher.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/integrations/multiprocessing_patcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # An attribute that will be set on the module to indicate that it has been
 # monkey-patched.
 
 PATCHED_MARKER = "_coverage$patched"
 
 
-if sys.version_info >= (3, 4):
+if tuple(sys.version_info) >= (3, 4):
     OriginalProcess = multiprocessing.process.BaseProcess
 else:
     OriginalProcess = multiprocessing.Process
 
 original_bootstrap = OriginalProcess._bootstrap
 
 
@@ -54,15 +54,15 @@
     This involves aggressive monkey-patching.
 
     """
 
     if hasattr(multiprocessing, PATCHED_MARKER):
         return
 
-    if sys.version_info >= (3, 4):
+    if tuple(sys.version_info) >= (3, 4):
         OriginalProcess._bootstrap = ProcessWithCoverage._bootstrap
     else:
         multiprocessing.Process = ProcessWithCoverage
 
     # When spawning processes rather than forking them, we have no state in the
     # new process.  We sneak in there with a Stowaway: we stuff one of our own
     # objects into the data that gets pickled and sent to the sub-process. When
```

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/integrations/pytest_xdist_helper.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/integrations/pytest_xdist_helper.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/integrations/unittest_helper.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/integrations/unittest_helper.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/integrations/nose_helper.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/integrations/nose_helper.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/integrations/pytest_helper.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/integrations/pytest_helper.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/entities/upload_reports_metadata.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/entities/upload_reports_metadata.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/executors/test_frameworks/agent_execution.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/executors/test_frameworks/agent_execution.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/executors/test_frameworks/pytest_execution.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/executors/test_frameworks/pytest_execution.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/executors/test_frameworks/unittest_execution.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/executors/test_frameworks/unittest_execution.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/executors/test_frameworks/nose_execution.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/executors/test_frameworks/nose_execution.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/executors/upload_reports.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/executors/upload_reports.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/executors/start_execution.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/executors/start_execution.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/executors/run.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/executors/run.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/executors/send_footprints.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/executors/send_footprints.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/executors/anonymous_execution.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/executors/anonymous_execution.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/test_listener/state_tracker.py` & `sealights-python-agent-1.0.6/python_agent/test_listener/state_tracker.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/__init__.py` & `sealights-python-agent-1.0.6/python_agent/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from python_agent.packages import urllib3
 from python_agent.packages.urllib3.exceptions import InsecureRequestWarning
 from logging.config import dictConfig
 
 urllib3.disable_warnings(InsecureRequestWarning)
 
-__version__ = "1.0.5"
+__version__ = "1.0.6"
 __package_name__ = "sealights-python-agent"
 
 
 LOG_CONF = {
     'version': 1,
     'disable_existing_loggers': False,
     'formatters': {
```

### Comparing `sealights-python-agent-1.0.5/python_agent/build_scanner/scm/git_integration.py` & `sealights-python-agent-1.0.6/python_agent/build_scanner/scm/git_integration.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/build_scanner/scm/scm_info.py` & `sealights-python-agent-1.0.6/python_agent/build_scanner/scm/scm_info.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/build_scanner/file_scanner.py` & `sealights-python-agent-1.0.6/python_agent/build_scanner/file_scanner.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/build_scanner/visitors.py` & `sealights-python-agent-1.0.6/python_agent/build_scanner/visitors.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def visit_Lambda(self, node):
         if not hasattr(node, "name"):
             node.name = "(Anonymous)"
         self.file_data.methods.append(self.method_hasher.build_method(self.file_data, node.name, node))
         self.generic_visit(node)
 
     def visit_AsyncFunctionDef(self, node):
-        if sys.version_info >= (3, 7) and node.col_offset == 0:
+        if tuple(sys.version_info) >= (3, 7) and node.col_offset == 0:
             # python 3.7 fixed the col_offset to be 0 instead of 6 for async methods
             # we're setting it as 6 to be consistent with the rest of the 3.x versions
             # reference - https://github.com/python/cpython/pull/4175/files
             node.col_offset = 6
         self.file_data.methods.append(self.method_hasher.build_method(self.file_data, node.name, node))
         self.generic_visit(node)
```

### Comparing `sealights-python-agent-1.0.5/python_agent/build_scanner/app.py` & `sealights-python-agent-1.0.6/python_agent/build_scanner/app.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/build_scanner/ast_utils.py` & `sealights-python-agent-1.0.6/python_agent/build_scanner/ast_utils.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/build_scanner/method_hasher.py` & `sealights-python-agent-1.0.6/python_agent/build_scanner/method_hasher.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/build_scanner/entities/environment_data.py` & `sealights-python-agent-1.0.6/python_agent/build_scanner/entities/environment_data.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/build_scanner/entities/v3/method_data.py` & `sealights-python-agent-1.0.6/python_agent/build_scanner/entities/v3/method_data.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/build_scanner/entities/v3/file_data.py` & `sealights-python-agent-1.0.6/python_agent/build_scanner/entities/v3/file_data.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/build_scanner/executors/build.py` & `sealights-python-agent-1.0.6/python_agent/build_scanner/executors/build.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/build_scanner/executors/config.py` & `sealights-python-agent-1.0.6/python_agent/build_scanner/executors/config.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/init.py` & `sealights-python-agent-1.0.6/python_agent/init.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from python_agent.test_listener.managers.agent_manager import AgentManager
 
 
 def init():
     try:
         admin.init()
     except SystemExit as e:
-        if sys.version_info >= (3, 0):
+        if tuple(sys.version_info) >= (3, 0):
             threading.current_thread = utils.trace(threading.current_thread, AgentManager().get_trace_function())
         else:
             threading.currentThread = utils.trace(threading.currentThread, AgentManager().get_trace_function())
 
 
 if 'uwsgi' in sys.modules:
     import uwsgidecorators
```

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/blinker/_utilities.py` & `sealights-python-agent-1.0.6/python_agent/packages/blinker/_utilities.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/blinker/base.py` & `sealights-python-agent-1.0.6/python_agent/packages/blinker/base.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/blinker/_saferef.py` & `sealights-python-agent-1.0.6/python_agent/packages/blinker/_saferef.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/requests/adapters.py` & `sealights-python-agent-1.0.6/python_agent/packages/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/requests/exceptions.py` & `sealights-python-agent-1.0.6/python_agent/packages/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/requests/packages.py` & `sealights-python-agent-1.0.6/python_agent/packages/requests/packages.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/requests/models.py` & `sealights-python-agent-1.0.6/python_agent/packages/requests/models.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/requests/api.py` & `sealights-python-agent-1.0.6/python_agent/packages/requests/api.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/requests/hooks.py` & `sealights-python-agent-1.0.6/python_agent/packages/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/requests/cookies.py` & `sealights-python-agent-1.0.6/python_agent/packages/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/requests/auth.py` & `sealights-python-agent-1.0.6/python_agent/packages/requests/auth.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/requests/utils.py` & `sealights-python-agent-1.0.6/python_agent/packages/requests/utils.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/requests/help.py` & `sealights-python-agent-1.0.6/python_agent/packages/requests/help.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/requests/_internal_utils.py` & `sealights-python-agent-1.0.6/python_agent/packages/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/requests/__init__.py` & `sealights-python-agent-1.0.6/python_agent/packages/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/requests/status_codes.py` & `sealights-python-agent-1.0.6/python_agent/packages/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/requests/structures.py` & `sealights-python-agent-1.0.6/python_agent/packages/requests/structures.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/requests/compat.py` & `sealights-python-agent-1.0.6/python_agent/packages/requests/compat.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/requests/sessions.py` & `sealights-python-agent-1.0.6/python_agent/packages/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/six.py` & `sealights-python-agent-1.0.6/python_agent/packages/six.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/certifi/cacert.pem` & `sealights-python-agent-1.0.6/python_agent/packages/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/certifi/core.py` & `sealights-python-agent-1.0.6/python_agent/packages/certifi/core.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/jwt/api_jws.py` & `sealights-python-agent-1.0.6/python_agent/packages/jwt/api_jws.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/jwt/exceptions.py` & `sealights-python-agent-1.0.6/python_agent/packages/jwt/exceptions.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/jwt/jwks_client.py` & `sealights-python-agent-1.0.6/python_agent/packages/jwt/jwks_client.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/jwt/api_jwt.py` & `sealights-python-agent-1.0.6/python_agent/packages/jwt/api_jwt.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/jwt/algorithms.py` & `sealights-python-agent-1.0.6/python_agent/packages/jwt/algorithms.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/jwt/api_jwk.py` & `sealights-python-agent-1.0.6/python_agent/packages/jwt/api_jwk.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/jwt/utils.py` & `sealights-python-agent-1.0.6/python_agent/packages/jwt/utils.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/jwt/help.py` & `sealights-python-agent-1.0.6/python_agent/packages/jwt/help.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/jwt/__init__.py` & `sealights-python-agent-1.0.6/python_agent/packages/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/astunparse/__main__.py` & `sealights-python-agent-1.0.6/python_agent/packages/astunparse/__main__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/astunparse/unparser36.py` & `sealights-python-agent-1.0.6/python_agent/packages/astunparse/unparser36.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/astunparse/printer.py` & `sealights-python-agent-1.0.6/python_agent/packages/astunparse/printer.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/astunparse/unparser.py` & `sealights-python-agent-1.0.6/python_agent/packages/astunparse/unparser.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/astunparse/unparser37.py` & `sealights-python-agent-1.0.6/python_agent/packages/astunparse/unparser37.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/astor/string_repr.py` & `sealights-python-agent-1.0.6/python_agent/packages/astor/string_repr.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/astor/code_gen.py` & `sealights-python-agent-1.0.6/python_agent/packages/astor/code_gen.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/astor/file_util.py` & `sealights-python-agent-1.0.6/python_agent/packages/astor/file_util.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/astor/source_repr.py` & `sealights-python-agent-1.0.6/python_agent/packages/astor/source_repr.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/astor/node_util.py` & `sealights-python-agent-1.0.6/python_agent/packages/astor/node_util.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/astor/__init__.py` & `sealights-python-agent-1.0.6/python_agent/packages/astor/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/astor/rtrip.py` & `sealights-python-agent-1.0.6/python_agent/packages/astor/rtrip.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/astor/tree_walk.py` & `sealights-python-agent-1.0.6/python_agent/packages/astor/tree_walk.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/astor/op_util.py` & `sealights-python-agent-1.0.6/python_agent/packages/astor/op_util.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/typing_extensions.py` & `sealights-python-agent-1.0.6/python_agent/packages/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/importlib_metadata/_adapters.py` & `sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/importlib_metadata/_text.py` & `sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/importlib_metadata/_collections.py` & `sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/importlib_metadata/_compat.py` & `sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/importlib_metadata/_functools.py` & `sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/importlib_metadata/_meta.py` & `sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/importlib_metadata/_itertools.py` & `sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/importlib_metadata/__init__.py` & `sealights-python-agent-1.0.6/python_agent/packages/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/zipp.py` & `sealights-python-agent-1.0.6/python_agent/packages/zipp.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/click/_textwrap.py` & `sealights-python-agent-1.0.6/python_agent/packages/click/_textwrap.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/click/exceptions.py` & `sealights-python-agent-1.0.6/python_agent/packages/click/exceptions.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/click/testing.py` & `sealights-python-agent-1.0.6/python_agent/packages/click/testing.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/click/types.py` & `sealights-python-agent-1.0.6/python_agent/packages/click/types.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/click/_termui_impl.py` & `sealights-python-agent-1.0.6/python_agent/packages/click/_termui_impl.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/click/_compat.py` & `sealights-python-agent-1.0.6/python_agent/packages/click/_compat.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/click/_unicodefun.py` & `sealights-python-agent-1.0.6/python_agent/packages/click/_unicodefun.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/click/_winconsole.py` & `sealights-python-agent-1.0.6/python_agent/packages/click/_winconsole.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/click/globals.py` & `sealights-python-agent-1.0.6/python_agent/packages/click/globals.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/click/utils.py` & `sealights-python-agent-1.0.6/python_agent/packages/click/utils.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/click/parser.py` & `sealights-python-agent-1.0.6/python_agent/packages/click/parser.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/click/__init__.py` & `sealights-python-agent-1.0.6/python_agent/packages/click/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/click/core.py` & `sealights-python-agent-1.0.6/python_agent/packages/click/core.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/click/decorators.py` & `sealights-python-agent-1.0.6/python_agent/packages/click/decorators.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/click/formatting.py` & `sealights-python-agent-1.0.6/python_agent/packages/click/formatting.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/click/shell_completion.py` & `sealights-python-agent-1.0.6/python_agent/packages/click/shell_completion.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/click/termui.py` & `sealights-python-agent-1.0.6/python_agent/packages/click/termui.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/cd.py` & `sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/cd.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/legacy.py` & `sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/legacy.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/models.py` & `sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/models.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/assets/__init__.py` & `sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/cli/normalizer.py` & `sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/cli/normalizer.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/api.py` & `sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/api.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/md.py` & `sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/md.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/utils.py` & `sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/utils.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/__init__.py` & `sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/charset_normalizer/constant.py` & `sealights-python-agent-1.0.6/python_agent/packages/charset_normalizer/constant.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/semantic_version/base.py` & `sealights-python-agent-1.0.6/python_agent/packages/semantic_version/base.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/semantic_version/__init__.py` & `sealights-python-agent-1.0.6/python_agent/packages/semantic_version/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/semantic_version/django_fields.py` & `sealights-python-agent-1.0.6/python_agent/packages/semantic_version/django_fields.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/idna/codec.py` & `sealights-python-agent-1.0.6/python_agent/packages/idna/codec.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/idna/intranges.py` & `sealights-python-agent-1.0.6/python_agent/packages/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/idna/uts46data.py` & `sealights-python-agent-1.0.6/python_agent/packages/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/idna/idnadata.py` & `sealights-python-agent-1.0.6/python_agent/packages/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/idna/__init__.py` & `sealights-python-agent-1.0.6/python_agent/packages/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/idna/core.py` & `sealights-python-agent-1.0.6/python_agent/packages/idna/core.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/exceptions.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/response.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/fields.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/connectionpool.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/poolmanager.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/_collections.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/filepost.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/connection.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/ssl_match_hostname.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/ssltransport.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/response.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/proxy.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/ssl_.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/wait.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/timeout.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/connection.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/request.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/retry.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/__init__.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/util/url.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/request.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/contrib/ntlmpool.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/contrib/_securetransport/low_level.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/contrib/_securetransport/bindings.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/contrib/securetransport.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/contrib/pyopenssl.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/contrib/_appengine_environ.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/contrib/appengine.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/contrib/socks.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/__init__.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/packages/six.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/urllib3/packages/backports/makefile.py` & `sealights-python-agent-1.0.6/python_agent/packages/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/python_agent/packages/freezegun/api.py` & `sealights-python-agent-1.0.6/python_agent/packages/freezegun/api.py`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/LICENSE.txt` & `sealights-python-agent-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sealights-python-agent-1.0.5/sealights_python_agent.egg-info/SOURCES.txt` & `sealights-python-agent-1.0.6/sealights_python_agent.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -237,14 +237,15 @@
 python_agent/test_listener/integrations/pytest_xdist_helper.py
 python_agent/test_listener/integrations/unittest_helper.py
 python_agent/test_listener/managers/__init__.py
 python_agent/test_listener/managers/agent_manager.py
 python_agent/test_listener/managers/code_coverage_manager.py
 python_agent/test_listener/managers/events_manager.py
 python_agent/test_listener/managers/footprints_manager.py
+python_agent/test_listener/managers/tia_manager.py
 python_agent/test_listener/queues/__init__.py
 python_agent/test_listener/queues/events_queue.py
 python_agent/test_listener/queues/footprints_queue.py
 python_agent/test_listener/services/__init__.py
 python_agent/test_listener/services/events_service.py
 python_agent/test_listener/services/footprints_service.py
 python_agent/test_listener/web_frameworks/__init__.py
```

### Comparing `sealights-python-agent-1.0.5/sealights_python_agent.egg-info/PKG-INFO` & `sealights-python-agent-1.0.6/sealights_python_agent.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sealights-python-agent
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python Agent
 Home-page: https://github.com/Sealights/SL.OnPremise.Agents.Python
 Author: Shai Cantor
 Author-email: shai@sealights.io
 License: Other/Proprietary License
 Keywords: sealights python agent setuptools development
 Platform: UNKNOWN
@@ -25,17 +25,14 @@
 
 The sealights-python-agent package integrates with the Sealights Quality Intelligence Platform.
 
 
 ****************
 Language Support
 ****************
-* Python 2.7
-* Python 3.4
-* Python 3.5
 * Python 3.6
 * Python 3.7
 
 
 ************
 Installation
 ************
@@ -80,14 +77,18 @@
 
         $ sl-python unit2 --teststage "Unit Tests" <your args...>
 
 
 Changes
 =======
 
+1.0.6 (2022-08-30)
+--------------------
+* Fixed "TIA Not Supported" Indicator for Test Optimization
+
 1.0.5 (2022-07-05)
 --------------------
 * Dropped support for Python 2.7, 3.4 and 3.5.
 * Upgraded dependencies
 * Using coverage.py 6
 * Bugfix: build session ids and lab ids were not encoded
```

### Comparing `sealights-python-agent-1.0.5/CHANGES.rst` & `sealights-python-agent-1.0.6/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changes
 =======
 
+1.0.6 (2022-08-30)
+--------------------
+* Fixed "TIA Not Supported" Indicator for Test Optimization
+
 1.0.5 (2022-07-05)
 --------------------
 * Dropped support for Python 2.7, 3.4 and 3.5.
 * Upgraded dependencies
 * Using coverage.py 6
 * Bugfix: build session ids and lab ids were not encoded
```

### Comparing `sealights-python-agent-1.0.5/README.rst` & `sealights-python-agent-1.0.6/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 
 The sealights-python-agent package integrates with the Sealights Quality Intelligence Platform.
 
 
 ****************
 Language Support
 ****************
-* Python 2.7
-* Python 3.4
-* Python 3.5
 * Python 3.6
 * Python 3.7
 
 
 ************
 Installation
 ************
```

### Comparing `sealights-python-agent-1.0.5/PKG-INFO` & `sealights-python-agent-1.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sealights-python-agent
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python Agent
 Home-page: https://github.com/Sealights/SL.OnPremise.Agents.Python
 Author: Shai Cantor
 Author-email: shai@sealights.io
 License: Other/Proprietary License
 Keywords: sealights python agent setuptools development
 Platform: UNKNOWN
@@ -25,17 +25,14 @@
 
 The sealights-python-agent package integrates with the Sealights Quality Intelligence Platform.
 
 
 ****************
 Language Support
 ****************
-* Python 2.7
-* Python 3.4
-* Python 3.5
 * Python 3.6
 * Python 3.7
 
 
 ************
 Installation
 ************
@@ -80,14 +77,18 @@
 
         $ sl-python unit2 --teststage "Unit Tests" <your args...>
 
 
 Changes
 =======
 
+1.0.6 (2022-08-30)
+--------------------
+* Fixed "TIA Not Supported" Indicator for Test Optimization
+
 1.0.5 (2022-07-05)
 --------------------
 * Dropped support for Python 2.7, 3.4 and 3.5.
 * Upgraded dependencies
 * Using coverage.py 6
 * Bugfix: build session ids and lab ids were not encoded
```

### Comparing `sealights-python-agent-1.0.5/setup.py` & `sealights-python-agent-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,18 @@
     changes = f.read()
 
 with open(path.join(here, 'requirements.txt')) as f:
     requirements = f.read().splitlines()
     # python 3.3 use case where dependencies are read as bytes of the form b'APScheduler==3.0.6'
     requirements = [requirement.decode() if isinstance(requirement, bytes) else requirement for requirement in requirements]
 
-if sys.version_info >= (3, 7):
-    install_requires = [requirements, "coverage==6.4"]
+if tuple(sys.version_info) >= (3, 7):
+    install_requires = requirements + ["coverage==6.4"]
 else:
-    install_requires = [requirements, "coverage==6.2"]
+    install_requires = requirements + ["coverage==6.2"]
 
 setup(
     name=python_agent.__package_name__,
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
```

