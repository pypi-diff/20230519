# Comparing `tmp/propan-0.1.1.0.tar.gz` & `tmp/propan-0.1.1.1.tar.gz`

## Comparing `propan-0.1.1.0.tar` & `propan-0.1.1.1.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 propan-0.1.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.1.0/SECURITY.md
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 propan-0.1.1.0/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 propan-0.1.1.0/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.1.0/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 propan-0.1.1.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/rabbit/header.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/rabbit/topic.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/redis/direct.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.1.0/examples/redis/pattern.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/__about__.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/__main__.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/py.typed
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/__init__.py
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/model/__init__.py
--rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/model/broker_usecase.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/model/schemas.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/model/utils.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0    11019 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0     7300 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/redis/__init__.py
--rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/redis/redis_broker.py
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/redis/redis_broker.pyi
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/brokers/redis/schemas.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/__init__.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/app.py
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/main.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/startproject/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/startproject/app.py
--rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/startproject/core.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/startproject/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/startproject/async_app/__init__.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/startproject/async_app/app.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/startproject/async_app/core.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/startproject/async_app/nats.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/startproject/async_app/rabbit.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/startproject/async_app/redis.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/startproject/sync_app/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/startproject/sync_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/fastapi/rabbit/router.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/fastapi/rabbit/router.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/fastapi/redis/__init__.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/fastapi/redis/router.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/fastapi/redis/router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/log/__init__.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/log/formatter.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/log/logging.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/test/__init__.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/test/rabbit.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/test/redis.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/test/utils.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/utils/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/utils/classes.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/utils/functions.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/utils/context/main.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.1.0/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.1.0/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.1.0/scripts/publish.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.1.0/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.1.0/scripts/test.sh
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 propan-0.1.1.0/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.1.0/LICENSE
--rw-r--r--   0        0        0    12114 2020-02-02 00:00:00.000000 propan-0.1.1.0/README.md
--rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 propan-0.1.1.0/pyproject.toml
--rw-r--r--   0        0        0    15563 2020-02-02 00:00:00.000000 propan-0.1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 propan-0.1.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.1.1/SECURITY.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 propan-0.1.1.1/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.1.1/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.1.1/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 propan-0.1.1.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.1.1/examples/redis/pattern.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/__about__.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/__main__.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/py.typed
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/brokers/__init__.py
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/brokers/model/__init__.py
+-rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/brokers/model/broker_usecase.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/brokers/model/schemas.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/brokers/model/utils.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0    11020 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0     7300 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     7854 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/cli/__init__.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/cli/app.py
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/cli/main.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/log/__init__.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/log/formatter.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/log/logging.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/test/__init__.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/test/redis.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/test/utils.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/utils/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/utils/classes.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/utils/functions.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/utils/context/main.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.1.1/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.1.1/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.1.1/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.1.1/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.1.1/scripts/test.sh
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 propan-0.1.1.1/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.1.1/LICENSE
+-rw-r--r--   0        0        0    12147 2020-02-02 00:00:00.000000 propan-0.1.1.1/README.md
+-rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 propan-0.1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    15596 2020-02-02 00:00:00.000000 propan-0.1.1.1/PKG-INFO
```

### Comparing `propan-0.1.1.0/CONTRIBUTING.md` & `propan-0.1.1.1/CONTRIBUTING.md`

 * *Files 3% similar despite different names*

```diff
@@ -40,70 +40,79 @@
 If you create a Python file that imports and uses Propan, and run it with the Python from your local environment, it will use your local Propan source code.
 
 And if you update that local Propan source code, as it is installed with `-e`, when you run that Python file again, it will use the fresh version of Propan you just edited.
 
 That way, you don't have to "install" your local version to be able to test every change.
 
 To use your local Propan cli type:
+
 ```bash
-$ python -m propan ...
+python -m propan ...
 ```
 
 ### Tests
 
-#### Pytests
+#### Pytest
+
 To run tests with your current Propan application and Python environment use:
 
 ```bash
 $ pytest tests
 # or
 $ bash ./scripts/test.sh
 # with coverage output
 $ bash ./scripts/test-cov.sh
 ```
 
 There are some *pytest marks* at project:
+
 * **slow**
 * **rabbit**
 * **nats**
 * **all**
 
 Default *pytest* calling runs "not slow" tests.
 
 To run all tests use:
 
 ```bash
-$ pytest -m 'all'
+pytest -m 'all'
 ```
 
 Also if you didn't up local rabbit or nats intance, run tests without that dependencies
 
 ```bash
-$ pytest -m 'not rabbit and not nats'
+pytest -m 'not rabbit and not nats'
 ```
 
 To run all tests based on RabbitMQ, NATS or another dependencies you should run first following *docker-compose.yml*
 
 ```yaml
 version: "3"
 
 services:
   rabbit:
     image: rabbitmq
     ports:
       - 5672:5672
-  
+
+  redis:
+    image: redis
+    ports:
+      - 6379:6379
+
   nats:
     image: nats
     ports:
       - 4222:4222
+      - 8222:8222  # management
 ```
 
 ```bash
-$ docker compose up -d
+docker compose up -d
 ```
 
 #### Hatch
 
 If you are using **hatch** use following environments to run tests:
 
 ##### **TEST**
@@ -129,8 +138,8 @@
 $ hatch run test-last:run
 
 # Run all tests at python 3.11
 $ hatch run test-last:run-all
 
 # Run all tests at python 3.11 and show coverage
 $ hatch run test-last:cov
-```
+```
```

### Comparing `propan-0.1.1.0/SECURITY.md` & `propan-0.1.1.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/.github/workflows/documentation.yml` & `propan-0.1.1.1/.github/workflows/documentation.yml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
           python-version: 3.x
       - uses: actions/cache@v2
         with:
           key: ${{ github.ref }}
           path: .cache
       - run: pip install mkdocs-material mkdocs-static-i18n mdx-include mkdocs-markdownextradata-plugin
       - working-directory: ./docs
-        run: mkdocs gh-deploy --force
+        run: mkdocs gh-deploy --force
```

### Comparing `propan-0.1.1.0/.github/workflows/publish_coverage.yml` & `propan-0.1.1.1/.github/workflows/publish_coverage.yml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   smokeshow:
     if: ${{ github.event.workflow_run.conclusion == 'success' }}
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/setup-python@v4
         with:
-          python-version: '3.9'
+          python-version: "3.9"
 
       - run: pip install smokeshow
 
       - uses: dawidd6/action-download-artifact@v2.26.0
         with:
           workflow: tests.yml
           commit: ${{ github.event.workflow_run.head_sha }}
@@ -28,8 +28,8 @@
       - run: smokeshow upload coverage-html
         env:
           SMOKESHOW_GITHUB_STATUS_DESCRIPTION: Coverage {coverage-percentage}
           SMOKESHOW_GITHUB_COVERAGE_THRESHOLD: 70
           SMOKESHOW_GITHUB_CONTEXT: coverage
           SMOKESHOW_GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
           SMOKESHOW_GITHUB_PR_HEAD_SHA: ${{ github.event.workflow_run.head_sha }}
-          SMOKESHOW_AUTH_KEY: ${{ secrets.SMOKESHOW_AUTH_KEY }}
+          SMOKESHOW_AUTH_KEY: ${{ secrets.SMOKESHOW_AUTH_KEY }}
```

### Comparing `propan-0.1.1.0/.github/workflows/publish_pypi.yml` & `propan-0.1.1.1/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/.github/workflows/tests.yml` & `propan-0.1.1.1/.github/workflows/tests.yml`

 * *Files 3% similar despite different names*

```diff
@@ -10,26 +10,31 @@
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
       fail-fast: false
-    
+
     services:
       rabbitmq:
         image: rabbitmq
         ports:
           - 5672:5672
-      
+
       redis:
         image: redis
         ports:
           - 6379:6379
 
+      nats:
+        image: nats
+        ports:
+          - 4222:4222
+
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           cache: "pip"
@@ -59,15 +64,15 @@
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
 
       - uses: actions/setup-python@v4
         with:
-          python-version: '3.8'
+          python-version: "3.8"
           cache: "pip"
           cache-dependency-path: pyproject.toml
 
       - name: Get coverage files
         uses: actions/download-artifact@v3
         with:
           name: coverage
@@ -83,21 +88,20 @@
       - name: Store coverage html
         uses: actions/upload-artifact@v3
         with:
           name: coverage-html
           path: htmlcov
 
   # https://github.com/marketplace/actions/alls-green#why
-  check:  # This job does nothing and is only used for the branch protection
-
+  check: # This job does nothing and is only used for the branch protection
     if: always()
 
     needs:
       - coverage-combine
 
     runs-on: ubuntu-latest
 
     steps:
       - name: Decide whether the needed jobs succeeded or failed
         uses: re-actors/alls-green@release/v1
         with:
-          jobs: ${{ toJSON(needs) }}
+          jobs: ${{ toJSON(needs) }}
```

### Comparing `propan-0.1.1.0/examples/3_lifespan_events.py` & `propan-0.1.1.1/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/examples/4_cli_attributes_promotion.py` & `propan-0.1.1.1/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/examples/5_publishing.py` & `propan-0.1.1.1/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/examples/6_arguments_casting.py` & `propan-0.1.1.1/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/examples/7_handler_errors_processing.py` & `propan-0.1.1.1/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/examples/dependencies/1_dependency_injection.py` & `propan-0.1.1.1/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.1.1/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.1.1/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.1.1/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.1.1/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/examples/dependencies/7_annotated.py` & `propan-0.1.1.1/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.1.1/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.1.1/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.1.1/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.1.1/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/examples/http_frameworks_integrations/quart.py` & `propan-0.1.1.1/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.1.1/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.1.1/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/examples/rabbit/direct.py` & `propan-0.1.1.1/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/examples/rabbit/fanout.py` & `propan-0.1.1.1/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/examples/rabbit/header.py` & `propan-0.1.1.1/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/examples/rabbit/topic.py` & `propan-0.1.1.1/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/examples/redis/direct.py` & `propan-0.1.1.1/examples/redis/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/examples/redis/pattern.py` & `propan-0.1.1.1/examples/redis/pattern.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/__init__.py` & `propan-0.1.1.1/propan/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/annotations.py` & `propan-0.1.1.1/propan/annotations.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/types.py` & `propan-0.1.1.1/propan/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/brokers/push_back_watcher.py` & `propan-0.1.1.1/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/brokers/model/broker_usecase.py` & `propan-0.1.1.1/propan/brokers/model/broker_usecase.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/brokers/model/schemas.py` & `propan-0.1.1.1/propan/brokers/model/schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,9 +64,10 @@
 
 
 @pydantic_dataclass
 class PropanMessage:
     body: bytes
     raw_message: Any
     content_type: Optional[str] = None
+    reply_to: str = ""
     headers: AnyDict = Field(default_factory=dict)
     message_id: str = Field(default_factory=lambda: str(uuid4()))
```

### Comparing `propan-0.1.1.0/propan/brokers/model/utils.py` & `propan-0.1.1.1/propan/brokers/model/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/brokers/nats/nats_broker.py` & `propan-0.1.1.1/propan/brokers/nats/nats_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.1.1/propan/brokers/nats/nats_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.1.1/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/brokers/nats/schemas.py` & `propan-0.1.1.1/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.1.1/propan/brokers/rabbit/rabbit_broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
         log_fmt: Optional[str] = None,
         **kwargs: AnyDict,
     ) -> None:
         super().__init__(*args, log_fmt=log_fmt, **kwargs)
         self._max_consumers = consumers
 
         self._channel = None
-        self.handlers = []
 
         self.__max_queue_len = 4
         self.__max_exchange_len = 4
 
     async def close(self) -> None:
         if self._channel is not None:
             await self._channel.close()
@@ -232,14 +231,15 @@
     @staticmethod
     async def _parse_message(
         message: aio_pika.message.IncomingMessage,
     ) -> PropanMessage:
         return PropanMessage(
             body=message.body,
             headers=message.headers,
+            reply_to=message.reply_to or "",
             message_id=message.message_id,
             content_type=message.content_type or "",
             raw_message=message,
         )
 
     def _process_message(
         self, func: Callable[[PropanMessage], T], watcher: Optional[BaseWatcher]
@@ -256,18 +256,18 @@
                     on_success=pika_message.ack,
                     on_error=pika_message.nack,
                     on_max=pika_message.reject,
                 )
 
             async with context:
                 r = await func(message)
-                if message.raw_message.reply_to:
+                if message.reply_to:
                     await self.publish(
                         message=r,
-                        routing_key=pika_message.reply_to,
+                        routing_key=message.reply_to,
                         correlation_id=pika_message.correlation_id,
                     )
 
                 return r
 
         return wrapper
```

### Comparing `propan-0.1.1.0/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.1.1/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/brokers/rabbit/schemas.py` & `propan-0.1.1.1/propan/brokers/rabbit/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/brokers/redis/redis_broker.py` & `propan-0.1.1.1/propan/brokers/redis/redis_broker.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,16 +74,16 @@
         watcher: Optional[BaseWatcher],
     ) -> Callable[[PropanMessage], T]:
         @wraps(func)
         async def wrapper(message: PropanMessage) -> T:
             r = await func(message)
 
             msg = message.raw_message
-            if isinstance(msg, RedisMessage) and msg.reply_to:
-                await self.publish(r or "", msg.reply_to)
+            if isinstance(msg, RedisMessage) and message.reply_to:
+                await self.publish(r or "", message.reply_to)
 
             return r
 
         return wrapper
 
     def handle(
         self,
@@ -188,14 +188,15 @@
                 body=data,
                 raw_message=message,
             )
         else:
             msg = PropanMessage(
                 body=obj.data,
                 content_type=obj.headers.get("content-type", ""),
+                reply_to=obj.reply_to,
                 headers=obj.headers,
                 raw_message=obj,
             )
 
         return msg
 
     async def _decode_message(self, message: PropanMessage) -> DecodedMessage:
```

### Comparing `propan-0.1.1.0/propan/brokers/redis/redis_broker.pyi` & `propan-0.1.1.1/propan/brokers/redis/redis_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/brokers/redis/schemas.py` & `propan-0.1.1.1/propan/brokers/redis/schemas.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 from dataclasses import dataclass
 from typing import Any, Dict, Optional
 
 from pydantic import BaseModel, Field
 from redis.asyncio.client import PubSub
 
 from propan.brokers.model.schemas import BaseHandler
-from propan.types import AnyCallable
 
 
 @dataclass
 class Handler(BaseHandler):
-    callback: AnyCallable
     channel: str
     pattern: bool = False
 
     task: Optional["asyncio.Task[Any]"] = None
     subscription: Optional[PubSub] = None
```

### Comparing `propan-0.1.1.0/propan/cli/app.py` & `propan-0.1.1.1/propan/cli/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/cli/main.py` & `propan-0.1.1.1/propan/cli/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/cli/startproject/core.py` & `propan-0.1.1.1/propan/cli/startproject/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/cli/startproject/async_app/app.py` & `propan-0.1.1.1/propan/cli/startproject/async_app/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/cli/startproject/async_app/core.py` & `propan-0.1.1.1/propan/cli/startproject/async_app/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/cli/startproject/async_app/nats.py` & `propan-0.1.1.1/propan/cli/startproject/async_app/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/cli/startproject/async_app/rabbit.py` & `propan-0.1.1.1/propan/cli/startproject/async_app/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/cli/startproject/async_app/redis.py` & `propan-0.1.1.1/propan/cli/startproject/async_app/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/cli/supervisors/basereload.py` & `propan-0.1.1.1/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/cli/supervisors/multiprocess.py` & `propan-0.1.1.1/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/cli/supervisors/utils.py` & `propan-0.1.1.1/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/cli/supervisors/watchfiles.py` & `propan-0.1.1.1/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/cli/utils/imports.py` & `propan-0.1.1.1/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/cli/utils/logs.py` & `propan-0.1.1.1/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/cli/utils/parser.py` & `propan-0.1.1.1/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/fastapi/core/route.py` & `propan-0.1.1.1/propan/fastapi/core/route.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/fastapi/core/router.py` & `propan-0.1.1.1/propan/fastapi/core/router.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/fastapi/rabbit/router.pyi` & `propan-0.1.1.1/propan/fastapi/rabbit/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/fastapi/redis/router.pyi` & `propan-0.1.1.1/propan/fastapi/redis/router.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -69,19 +69,17 @@
     def add_api_mq_route(  # type: ignore[override]
         self,
         channel: str,
         *,
         endpoint: AnyCallable,
         name: Optional[str] = None,
         pattern: bool = False,
-        retry: Union[bool, int] = False,
     ) -> None:
         pass
     def event(  # type: ignore[override]
         self,
         channel: str,
         *,
         pattern: bool = False,
-        retry: Union[bool, int] = False,
         name: Optional[str] = None,
     ) -> None:
         pass
```

### Comparing `propan-0.1.1.0/propan/log/formatter.py` & `propan-0.1.1.1/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/log/logging.py` & `propan-0.1.1.1/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/test/rabbit.py` & `propan-0.1.1.1/propan/test/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/test/redis.py` & `propan-0.1.1.1/propan/test/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/test/utils.py` & `propan-0.1.1.1/propan/test/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/utils/functions.py` & `propan-0.1.1.1/propan/utils/functions.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/utils/context/main.py` & `propan-0.1.1.1/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/propan/utils/context/types.py` & `propan-0.1.1.1/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/LICENSE` & `propan-0.1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/README.md` & `propan-0.1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -132,17 +132,19 @@
 ---
 
 ## Quickstart
 
 Install using `pip`:
 
 ```shell
-$ pip install "propan[async-rabbit]"
+pip install "propan[async-rabbit]"
 # or
-$ pip install "propan[async-nats]"
+pip install "propan[async-nats]"
+# or
+pip install "propan[async-redis]"
 ```
 
 ### Basic usage
 
 Create an application with the following code at `serve.py`:
 
 ```python
@@ -162,15 +164,15 @@
     '''Handle all default exchange messages with `test` routing key'''
     print(body)
 ```
 
 And just run it:
 
 ```shell
-$ propan run serve:app
+propan run serve:app
 ```
 
 ---
 
 ## Type casting
 
 Propan uses `pydantic` to cast incoming function arguments to types according to their annotation.
```

#### html2text {}

```diff
@@ -50,30 +50,30 @@
 declare *channel*, *queues*, *exchanges* by yourself. Also, you need to manage
 *connection*, *message*, *queue* context to avoid any troubles. It is not a bad
 way, but it can be much easier. ```python from propan import PropanApp,
 RabbitBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
 PropanApp(broker) @broker.handle("test_queue") async def base_handler(body):
 print(body) ``` This is the **Propan** declarative way to write the same code.
 That is so much easier, isn't it? --- ## Quickstart Install using `pip`:
-```shell $ pip install "propan[async-rabbit]" # or $ pip install "propan[async-
-nats]" ``` ### Basic usage Create an application with the following code at
-`serve.py`: ```python from propan import PropanApp from propan import
-RabbitBroker # from propan import RedisBroker # from propan import NatsBroker
-broker = RabbitBroker("amqp://guest:guest@localhost:5672/") # broker =
-NatsBroker("nats://localhost:4222") # broker = RedisBroker("redis://localhost:
-6379") app = PropanApp(broker) @broker.handle("test") async def base_handler
-(body): '''Handle all default exchange messages with `test` routing key'''
-print(body) ``` And just run it: ```shell $ propan run serve:app ``` --- ##
-Type casting Propan uses `pydantic` to cast incoming function arguments to
-types according to their annotation. ```python from pydantic import BaseModel
-from propan import PropanApp, Context, RabbitBroker broker = RabbitBroker
-("amqp://guest:guest@localhost:5672/") app = PropanApp(broker) class
-SimpleMessage(BaseModel): key: int @broker.handle("test2") async def
-second_handler(body: SimpleMessage): assert isinstance(body.key, int) ``` --
-- ## Dependencies **Propan** a has dependencies management policy close to
+```shell pip install "propan[async-rabbit]" # or pip install "propan[async-
+nats]" # or pip install "propan[async-redis]" ``` ### Basic usage Create an
+application with the following code at `serve.py`: ```python from propan import
+PropanApp from propan import RabbitBroker # from propan import RedisBroker #
+from propan import NatsBroker broker = RabbitBroker("amqp://guest:
+guest@localhost:5672/") # broker = NatsBroker("nats://localhost:4222") # broker
+= RedisBroker("redis://localhost:6379") app = PropanApp(broker) @broker.handle
+("test") async def base_handler(body): '''Handle all default exchange messages
+with `test` routing key''' print(body) ``` And just run it: ```shell propan run
+serve:app ``` --- ## Type casting Propan uses `pydantic` to cast incoming
+function arguments to types according to their annotation. ```python from
+pydantic import BaseModel from propan import PropanApp, Context, RabbitBroker
+broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp
+(broker) class SimpleMessage(BaseModel): key: int @broker.handle("test2") async
+def second_handler(body: SimpleMessage): assert isinstance(body.key, int) ``` -
+-- ## Dependencies **Propan** a has dependencies management policy close to
 `pytest fixtures`. You can specify in functions arguments which dependencies
 you would to use. Framework passes them from the global Context object. Already
 existed context fields are: *app*, *broker*, *context* (itself), *logger* and
 *message*. If you call not existing field, raises *pydantic.ValidationError*
 value. But you can specify your own dependencies, call dependencies functions
 (like `Fastapi Depends`) and [more](https://github.com/Lancetnik/Propan/tree/
 main/examples/dependencies). ```python import aio_pika from propan import
```

### Comparing `propan-0.1.1.0/pyproject.toml` & `propan-0.1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.0/PKG-INFO` & `propan-0.1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.1.1.0
+Version: 0.1.1.1
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-Expression: MIT
@@ -207,17 +207,19 @@
 ---
 
 ## Quickstart
 
 Install using `pip`:
 
 ```shell
-$ pip install "propan[async-rabbit]"
+pip install "propan[async-rabbit]"
 # or
-$ pip install "propan[async-nats]"
+pip install "propan[async-nats]"
+# or
+pip install "propan[async-redis]"
 ```
 
 ### Basic usage
 
 Create an application with the following code at `serve.py`:
 
 ```python
@@ -237,15 +239,15 @@
     '''Handle all default exchange messages with `test` routing key'''
     print(body)
 ```
 
 And just run it:
 
 ```shell
-$ propan run serve:app
+propan run serve:app
 ```
 
 ---
 
 ## Type casting
 
 Propan uses `pydantic` to cast incoming function arguments to types according to their annotation.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propan Version: 0.1.1.0 Summary: Propan framework:
+Metadata-Version: 2.1 Name: propan Version: 0.1.1.1 Summary: Propan framework:
 the simplest way to work with a messaging queues Project-URL: Homepage, https:/
 /lancetnik.github.io/Propan/ Project-URL: Documentation, https://
 lancetnik.github.io/Propan/ Project-URL: Tracker, https://github.com/Lancetnik/
 Propan/issues Project-URL: Source, https://github.com/Lancetnik/Propan Author-
 email: Pastukhov Nikita
 yandex.ru> License-Expression: MIT License-File: LICENSE Keywords:
 framework,message brokers,rabbitmq Classifier: Development Status :: 5 -
@@ -96,30 +96,30 @@
 declare *channel*, *queues*, *exchanges* by yourself. Also, you need to manage
 *connection*, *message*, *queue* context to avoid any troubles. It is not a bad
 way, but it can be much easier. ```python from propan import PropanApp,
 RabbitBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
 PropanApp(broker) @broker.handle("test_queue") async def base_handler(body):
 print(body) ``` This is the **Propan** declarative way to write the same code.
 That is so much easier, isn't it? --- ## Quickstart Install using `pip`:
-```shell $ pip install "propan[async-rabbit]" # or $ pip install "propan[async-
-nats]" ``` ### Basic usage Create an application with the following code at
-`serve.py`: ```python from propan import PropanApp from propan import
-RabbitBroker # from propan import RedisBroker # from propan import NatsBroker
-broker = RabbitBroker("amqp://guest:guest@localhost:5672/") # broker =
-NatsBroker("nats://localhost:4222") # broker = RedisBroker("redis://localhost:
-6379") app = PropanApp(broker) @broker.handle("test") async def base_handler
-(body): '''Handle all default exchange messages with `test` routing key'''
-print(body) ``` And just run it: ```shell $ propan run serve:app ``` --- ##
-Type casting Propan uses `pydantic` to cast incoming function arguments to
-types according to their annotation. ```python from pydantic import BaseModel
-from propan import PropanApp, Context, RabbitBroker broker = RabbitBroker
-("amqp://guest:guest@localhost:5672/") app = PropanApp(broker) class
-SimpleMessage(BaseModel): key: int @broker.handle("test2") async def
-second_handler(body: SimpleMessage): assert isinstance(body.key, int) ``` --
-- ## Dependencies **Propan** a has dependencies management policy close to
+```shell pip install "propan[async-rabbit]" # or pip install "propan[async-
+nats]" # or pip install "propan[async-redis]" ``` ### Basic usage Create an
+application with the following code at `serve.py`: ```python from propan import
+PropanApp from propan import RabbitBroker # from propan import RedisBroker #
+from propan import NatsBroker broker = RabbitBroker("amqp://guest:
+guest@localhost:5672/") # broker = NatsBroker("nats://localhost:4222") # broker
+= RedisBroker("redis://localhost:6379") app = PropanApp(broker) @broker.handle
+("test") async def base_handler(body): '''Handle all default exchange messages
+with `test` routing key''' print(body) ``` And just run it: ```shell propan run
+serve:app ``` --- ## Type casting Propan uses `pydantic` to cast incoming
+function arguments to types according to their annotation. ```python from
+pydantic import BaseModel from propan import PropanApp, Context, RabbitBroker
+broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp
+(broker) class SimpleMessage(BaseModel): key: int @broker.handle("test2") async
+def second_handler(body: SimpleMessage): assert isinstance(body.key, int) ``` -
+-- ## Dependencies **Propan** a has dependencies management policy close to
 `pytest fixtures`. You can specify in functions arguments which dependencies
 you would to use. Framework passes them from the global Context object. Already
 existed context fields are: *app*, *broker*, *context* (itself), *logger* and
 *message*. If you call not existing field, raises *pydantic.ValidationError*
 value. But you can specify your own dependencies, call dependencies functions
 (like `Fastapi Depends`) and [more](https://github.com/Lancetnik/Propan/tree/
 main/examples/dependencies). ```python import aio_pika from propan import
```

