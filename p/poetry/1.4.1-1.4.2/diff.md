# Comparing `tmp/poetry-1.4.1.tar.gz` & `tmp/poetry-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry-1.4.1.tar", max compression
+gzip compressed data, was "poetry-1.4.2.tar", max compression
```

## Comparing `poetry-1.4.1.tar` & `poetry-1.4.2.tar`

### file list

```diff
@@ -1,672 +1,674 @@
--rw-r--r--   0        0        0     1070 2023-03-19 14:44:45.078395 poetry-1.4.1/LICENSE
--rw-r--r--   0        0        0     4547 2023-03-19 14:44:45.078395 poetry-1.4.1/README.md
--rw-r--r--   0        0        0     5180 2023-03-19 14:44:45.090396 poetry-1.4.1/pyproject.toml
--rw-r--r--   0        0        0      146 2023-03-19 14:44:45.090396 poetry-1.4.1/src/poetry/__main__.py
--rw-r--r--   0        0        0      342 2023-03-19 14:44:45.090396 poetry-1.4.1/src/poetry/__version__.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.090396 poetry-1.4.1/src/poetry/config/__init__.py
--rw-r--r--   0        0        0     9688 2023-03-19 14:44:45.090396 poetry-1.4.1/src/poetry/config/config.py
--rw-r--r--   0        0        0      261 2023-03-19 14:44:45.090396 poetry-1.4.1/src/poetry/config/config_source.py
--rw-r--r--   0        0        0     1018 2023-03-19 14:44:45.090396 poetry-1.4.1/src/poetry/config/dict_config_source.py
--rw-r--r--   0        0        0     2338 2023-03-19 14:44:45.090396 poetry-1.4.1/src/poetry/config/file_config_source.py
--rw-r--r--   0        0        0      339 2023-03-19 14:44:45.090396 poetry-1.4.1/src/poetry/config/source.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.090396 poetry-1.4.1/src/poetry/console/__init__.py
--rw-r--r--   0        0        0    12765 2023-03-19 14:44:45.090396 poetry-1.4.1/src/poetry/console/application.py
--rw-r--r--   0        0        0      615 2023-03-19 14:44:45.090396 poetry-1.4.1/src/poetry/console/command_loader.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/__init__.py
--rw-r--r--   0        0        0      915 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/about.py
--rw-r--r--   0        0        0    10289 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/add.py
--rw-r--r--   0        0        0     1081 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/build.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/cache/__init__.py
--rw-r--r--   0        0        0     2411 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/cache/clear.py
--rw-r--r--   0        0        0      634 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/cache/list.py
--rw-r--r--   0        0        0     3366 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/check.py
--rw-r--r--   0        0        0     1118 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/command.py
--rw-r--r--   0        0        0    11052 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/config.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/debug/__init__.py
--rw-r--r--   0        0        0      764 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/debug/info.py
--rw-r--r--   0        0        0     4459 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/debug/resolve.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/env/__init__.py
--rw-r--r--   0        0        0     2310 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/env/info.py
--rw-r--r--   0        0        0      822 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/env/list.py
--rw-r--r--   0        0        0     1478 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/env/remove.py
--rw-r--r--   0        0        0      706 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/env/use.py
--rw-r--r--   0        0        0      544 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/env_command.py
--rw-r--r--   0        0        0     3372 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/group_command.py
--rw-r--r--   0        0        0    17297 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/init.py
--rw-r--r--   0        0        0     6470 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/install.py
--rw-r--r--   0        0        0      907 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/installer_command.py
--rw-r--r--   0        0        0     1738 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/lock.py
--rw-r--r--   0        0        0     3047 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/new.py
--rw-r--r--   0        0        0     2784 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/publish.py
--rw-r--r--   0        0        0     5013 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/remove.py
--rw-r--r--   0        0        0     2697 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/run.py
--rw-r--r--   0        0        0      786 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/search.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/self/__init__.py
--rw-r--r--   0        0        0     1262 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/self/add.py
--rw-r--r--   0        0        0      973 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/self/install.py
--rw-r--r--   0        0        0      642 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/self/lock.py
--rw-r--r--   0        0        0      607 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/self/remove.py
--rw-r--r--   0        0        0     4493 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/self/self_command.py
--rw-r--r--   0        0        0     1209 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/self/show/__init__.py
--rw-r--r--   0        0        0     4096 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/self/show/plugins.py
--rw-r--r--   0        0        0     1802 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/self/update.py
--rw-r--r--   0        0        0     1527 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/shell.py
--rw-r--r--   0        0        0    19612 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/show.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/source/__init__.py
--rw-r--r--   0        0        0     3128 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/source/add.py
--rw-r--r--   0        0        0     1133 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/source/remove.py
--rw-r--r--   0        0        0     1755 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/source/show.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/source/update.py
--rw-r--r--   0        0        0     1773 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/update.py
--rw-r--r--   0        0        0     3775 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/commands/version.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/events/__init__.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/events/console_events.py
--rw-r--r--   0        0        0      122 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/io/__init__.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/io/inputs/__init__.py
--rw-r--r--   0        0        0     2582 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/io/inputs/run_argv_input.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/logging/__init__.py
--rw-r--r--   0        0        0       99 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/logging/filters.py
--rw-r--r--   0        0        0      336 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/logging/formatters/__init__.py
--rw-r--r--   0        0        0      788 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/logging/formatters/builder_formatter.py
--rw-r--r--   0        0        0      132 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/logging/formatters/formatter.py
--rw-r--r--   0        0        0     1026 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/logging/io_formatter.py
--rw-r--r--   0        0        0      718 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/console/logging/io_handler.py
--rw-r--r--   0        0        0      134 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/exceptions.py
--rw-r--r--   0        0        0    10059 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/factory.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/inspection/__init__.py
--rw-r--r--   0        0        0    21835 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/inspection/info.py
--rw-r--r--   0        0        0      114 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/installation/__init__.py
--rw-r--r--   0        0        0      430 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/installation/base_installer.py
--rw-r--r--   0        0        0     8853 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/installation/chef.py
--rw-r--r--   0        0        0     8029 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/installation/chooser.py
--rw-r--r--   0        0        0    34730 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/installation/executor.py
--rw-r--r--   0        0        0    19912 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/installation/installer.py
--rw-r--r--   0        0        0      979 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/installation/noop_installer.py
--rw-r--r--   0        0        0      262 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/installation/operations/__init__.py
--rw-r--r--   0        0        0      906 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/installation/operations/install.py
--rw-r--r--   0        0        0     1315 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/installation/operations/operation.py
--rw-r--r--   0        0        0      959 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/installation/operations/uninstall.py
--rw-r--r--   0        0        0     1540 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/installation/operations/update.py
--rw-r--r--   0        0        0    10103 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/installation/pip_installer.py
--rw-r--r--   0        0        0     3497 2023-03-19 14:44:45.094397 poetry-1.4.1/src/poetry/installation/wheel_installer.py
--rw-r--r--   0        0        0     1311 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/json/__init__.py
--rw-r--r--   0        0        0     1552 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/json/schemas/poetry.json
--rw-r--r--   0        0        0      310 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/layouts/__init__.py
--rw-r--r--   0        0        0     6072 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/layouts/layout.py
--rw-r--r--   0        0        0      202 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/layouts/src.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/layouts/standard.py
--rw-r--r--   0        0        0     1657 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/locations.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/masonry/__init__.py
--rw-r--r--   0        0        0      497 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/masonry/api.py
--rw-r--r--   0        0        0      129 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/masonry/builders/__init__.py
--rw-r--r--   0        0        0     9599 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/masonry/builders/editable.py
--rw-r--r--   0        0        0      467 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/mixology/__init__.py
--rw-r--r--   0        0        0     1555 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/mixology/assignment.py
--rw-r--r--   0        0        0    10186 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/mixology/failure.py
--rw-r--r--   0        0        0    15346 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/mixology/incompatibility.py
--rw-r--r--   0        0        0     1903 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/mixology/incompatibility_cause.py
--rw-r--r--   0        0        0     7080 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/mixology/partial_solution.py
--rw-r--r--   0        0        0      676 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/mixology/result.py
--rw-r--r--   0        0        0      211 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/mixology/set_relation.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/mixology/solutions/__init__.py
--rw-r--r--   0        0        0      214 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/mixology/solutions/providers/__init__.py
--rw-r--r--   0        0        0     1091 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/mixology/solutions/providers/python_requirement_solution_provider.py
--rw-r--r--   0        0        0      189 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/mixology/solutions/solutions/__init__.py
--rw-r--r--   0        0        0     2281 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/mixology/solutions/solutions/python_requirement_solution.py
--rw-r--r--   0        0        0     6904 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/mixology/term.py
--rw-r--r--   0        0        0    19826 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/mixology/version_solver.py
--rw-r--r--   0        0        0      273 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/packages/__init__.py
--rw-r--r--   0        0        0     1297 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/packages/dependency_package.py
--rw-r--r--   0        0        0    17314 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/packages/locker.py
--rw-r--r--   0        0        0      921 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/packages/package_collection.py
--rw-r--r--   0        0        0      185 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/plugins/__init__.py
--rw-r--r--   0        0        0      687 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/plugins/application_plugin.py
--rw-r--r--   0        0        0      435 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/plugins/base_plugin.py
--rw-r--r--   0        0        0      484 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/plugins/plugin.py
--rw-r--r--   0        0        0     2567 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/plugins/plugin_manager.py
--rw-r--r--   0        0        0     2114 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/poetry.py
--rw-r--r--   0        0        0      112 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/publishing/__init__.py
--rw-r--r--   0        0        0     2893 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/publishing/publisher.py
--rw-r--r--   0        0        0    12483 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/publishing/uploader.py
--rw-r--r--   0        0        0       99 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/puzzle/__init__.py
--rw-r--r--   0        0        0      799 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/puzzle/exceptions.py
--rw-r--r--   0        0        0    40439 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/puzzle/provider.py
--rw-r--r--   0        0        0    11539 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/puzzle/solver.py
--rw-r--r--   0        0        0     5124 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/puzzle/transaction.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/py.typed
--rw-r--r--   0        0        0      198 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/repositories/__init__.py
--rw-r--r--   0        0        0      833 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/repositories/abstract_repository.py
--rw-r--r--   0        0        0     2553 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/repositories/cached_repository.py
--rw-r--r--   0        0        0      125 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/repositories/exceptions.py
--rw-r--r--   0        0        0    11550 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/repositories/http_repository.py
--rw-r--r--   0        0        0    10342 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/repositories/installed_repository.py
--rw-r--r--   0        0        0     4474 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/repositories/legacy_repository.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/repositories/link_sources/__init__.py
--rw-r--r--   0        0        0     3835 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/repositories/link_sources/base.py
--rw-r--r--   0        0        0     1955 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/repositories/link_sources/html.py
--rw-r--r--   0        0        0     1227 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/repositories/link_sources/json.py
--rw-r--r--   0        0        0      841 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/repositories/lockfile_repository.py
--rw-r--r--   0        0        0     8452 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/repositories/pypi_repository.py
--rw-r--r--   0        0        0     3978 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/repositories/repository.py
--rw-r--r--   0        0        0     4783 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/repositories/repository_pool.py
--rw-r--r--   0        0        0      753 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/repositories/single_page_repository.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/utils/__init__.py
--rw-r--r--   0        0        0     1639 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/utils/_compat.py
--rw-r--r--   0        0        0    16540 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/utils/authenticator.py
--rw-r--r--   0        0        0     5509 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/utils/cache.py
--rw-r--r--   0        0        0      115 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/utils/constants.py
--rw-r--r--   0        0        0     6993 2023-03-19 14:44:45.098397 poetry-1.4.1/src/poetry/utils/dependency_specification.py
--rw-r--r--   0        0        0    67576 2023-03-19 14:44:45.102397 poetry-1.4.1/src/poetry/utils/env.py
--rw-r--r--   0        0        0     1848 2023-03-19 14:44:45.102397 poetry-1.4.1/src/poetry/utils/extras.py
--rw-r--r--   0        0        0     7416 2023-03-19 14:44:45.102397 poetry-1.4.1/src/poetry/utils/helpers.py
--rw-r--r--   0        0        0     7339 2023-03-19 14:44:45.102397 poetry-1.4.1/src/poetry/utils/password_manager.py
--rw-r--r--   0        0        0      406 2023-03-19 14:44:45.102397 poetry-1.4.1/src/poetry/utils/patterns.py
--rw-r--r--   0        0        0     1463 2023-03-19 14:44:45.102397 poetry-1.4.1/src/poetry/utils/pip.py
--rw-r--r--   0        0        0    12143 2023-03-19 14:44:45.102397 poetry-1.4.1/src/poetry/utils/setup_reader.py
--rw-r--r--   0        0        0     4290 2023-03-19 14:44:45.102397 poetry-1.4.1/src/poetry/utils/shell.py
--rw-r--r--   0        0        0      446 2023-03-19 14:44:45.102397 poetry-1.4.1/src/poetry/utils/source.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.102397 poetry-1.4.1/src/poetry/vcs/__init__.py
--rw-r--r--   0        0        0       95 2023-03-19 14:44:45.102397 poetry-1.4.1/src/poetry/vcs/git/__init__.py
--rw-r--r--   0        0        0    15755 2023-03-19 14:44:45.102397 poetry-1.4.1/src/poetry/vcs/git/backend.py
--rw-r--r--   0        0        0     1771 2023-03-19 14:44:45.102397 poetry-1.4.1/src/poetry/vcs/git/system.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.102397 poetry-1.4.1/src/poetry/version/__init__.py
--rw-r--r--   0        0        0     1573 2023-03-19 14:44:45.102397 poetry-1.4.1/src/poetry/version/version_selector.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/__init__.py
--rw-r--r--   0        0        0      274 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/compat.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/config/__init__.py
--rw-r--r--   0        0        0     2265 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/config/test_config.py
--rw-r--r--   0        0        0    13346 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/__init__.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/__init__.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/cache/__init__.py
--rw-r--r--   0        0        0     1458 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/cache/conftest.py
--rw-r--r--   0        0        0     2237 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/cache/test_clear.py
--rw-r--r--   0        0        0      816 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/cache/test_list.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/debug/__init__.py
--rw-r--r--   0        0        0     1776 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/debug/test_resolve.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/env/__init__.py
--rw-r--r--   0        0        0     2336 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/env/conftest.py
--rw-r--r--   0        0        0     1077 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/env/helpers.py
--rw-r--r--   0        0        0     1374 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/env/test_info.py
--rw-r--r--   0        0        0     2030 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/env/test_list.py
--rw-r--r--   0        0        0     2880 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/env/test_remove.py
--rw-r--r--   0        0        0     4387 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/env/test_use.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/self/__init__.py
--rw-r--r--   0        0        0     2333 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/self/conftest.py
--rw-r--r--   0        0        0       65 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/self/fixtures/poetry-1.0.5-darwin.sha256sum
--rw-r--r--   0        0        0     1041 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/self/fixtures/poetry-1.0.5-darwin.tar.gz
--rw-r--r--   0        0        0     7167 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/self/test_add_plugins.py
--rw-r--r--   0        0        0     3015 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/self/test_remove_plugins.py
--rw-r--r--   0        0        0     5665 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/self/test_show_plugins.py
--rw-r--r--   0        0        0     2160 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/self/test_update.py
--rw-r--r--   0        0        0     1069 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/self/utils.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/source/__init__.py
--rw-r--r--   0        0        0     1716 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/source/conftest.py
--rw-r--r--   0        0        0     3035 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/source/test_add.py
--rw-r--r--   0        0        0     1254 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/source/test_remove.py
--rw-r--r--   0        0        0     2102 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/source/test_show.py
--rw-r--r--   0        0        0      827 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/test_about.py
--rw-r--r--   0        0        0    56270 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/test_add.py
--rw-r--r--   0        0        0     1258 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/test_build.py
--rw-r--r--   0        0        0     2012 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/test_check.py
--rw-r--r--   0        0        0     8649 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/test_config.py
--rw-r--r--   0        0        0    29495 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/test_init.py
--rw-r--r--   0        0        0    10196 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/test_install.py
--rw-r--r--   0        0        0    10247 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/test_lock.py
--rw-r--r--   0        0        0     5943 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/test_new.py
--rw-r--r--   0        0        0     3698 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/test_publish.py
--rw-r--r--   0        0        0     9026 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/test_remove.py
--rw-r--r--   0        0        0     6178 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/test_run.py
--rw-r--r--   0        0        0     2560 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/test_search.py
--rw-r--r--   0        0        0     2332 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/test_shell.py
--rw-r--r--   0        0        0    65807 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/test_show.py
--rw-r--r--   0        0        0     1633 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/test_update.py
--rw-r--r--   0        0        0     2486 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/commands/test_version.py
--rw-r--r--   0        0        0     5047 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/conftest.py
--rw-r--r--   0        0        0     3120 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/console/test_application.py
--rw-r--r--   0        0        0       22 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/fixtures/build_system_requires_not_available/README.rst
--rw-r--r--   0        0        0      676 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/fixtures/build_system_requires_not_available/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/fixtures/build_system_requires_not_available/simple_project/__init__.py
--rw-r--r--   0        0        0     1168 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/fixtures/complete.toml
--rw-r--r--   0        0        0      424 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/fixtures/deleted_directory_dependency/poetry.lock
--rw-r--r--   0        0        0      234 2023-03-19 14:44:45.102397 poetry-1.4.1/tests/fixtures/deleted_directory_dependency/pyproject.toml
--rw-r--r--   0        0        0      446 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/deleted_file_dependency/poetry.lock
--rw-r--r--   0        0        0      234 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/deleted_file_dependency/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/directory/project_with_transitive_directory_dependencies/project_with_transitive_directory_dependencies/__init__.py
--rw-r--r--   0        0        0      418 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/directory/project_with_transitive_directory_dependencies/pyproject.toml
--rw-r--r--   0        0        0      574 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/directory/project_with_transitive_directory_dependencies/setup.py
--rw-r--r--   0        0        0      234 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/directory/project_with_transitive_file_dependencies/inner-directory-project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/directory/project_with_transitive_file_dependencies/project_with_transitive_file_dependencies/__init__.py
--rw-r--r--   0        0        0      385 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/directory/project_with_transitive_file_dependencies/pyproject.toml
--rw-r--r--   0        0        0     1116 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1003 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/distributions/demo-0.1.0.tar.gz
--rw-r--r--   0        0        0     1552 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/distributions/demo-0.1.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0       22 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/excluded_subpackage/README.rst
--rw-r--r--   0        0        0       59 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/excluded_subpackage/example/__init__.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/excluded_subpackage/example/test/__init__.py
--rw-r--r--   0        0        0      159 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/excluded_subpackage/example/test/excluded.py
--rw-r--r--   0        0        0      329 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/excluded_subpackage/pyproject.toml
--rw-r--r--   0        0        0       22 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/extended_project/README.rst
--rw-r--r--   0        0        0      362 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/extended_project/build.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/extended_project/extended_project/__init__.py
--rw-r--r--   0        0        0      652 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/extended_project/pyproject.toml
--rw-r--r--   0        0        0       22 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/extended_project_without_setup/README.rst
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/extended_project_without_setup/build.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/extended_project_without_setup/extended_project/__init__.py
--rw-r--r--   0        0        0      756 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/extended_project_without_setup/pyproject.toml
--rw-r--r--   0        0        0       18 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/extended_with_no_setup/README.md
--rw-r--r--   0        0        0      852 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/extended_with_no_setup/build.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/extended_with_no_setup/extended/__init__.py
--rw-r--r--   0        0        0      888 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/extended_with_no_setup/extended/extended.c
--rw-r--r--   0        0        0      559 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/extended_with_no_setup/pyproject.toml
--rw-r--r--   0        0        0       59 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/demo/demo/__init__.py
--rw-r--r--   0        0        0      226 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/demo/demo.egg-info/PKG-INFO
--rw-r--r--   0        0        0      164 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/demo/demo.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/demo/demo.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       43 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/demo/demo.egg-info/requires.txt
--rw-r--r--   0        0        0        5 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/demo/demo.egg-info/top_level.txt
--rw-r--r--   0        0        0      429 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/demo/setup.py
--rw-r--r--   0        0        0       93 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/namespace-package-one/namespace_package/__init__.py
--rw-r--r--   0        0        0       50 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/namespace-package-one/namespace_package/one/__init__.py
--rw-r--r--   0        0        0      402 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/namespace-package-one/setup.py
--rw-r--r--   0        0        0       59 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/no-dependencies/demo/__init__.py
--rw-r--r--   0        0        0      214 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/no-dependencies/demo.egg-info/PKG-INFO
--rw-r--r--   0        0        0      137 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/no-dependencies/demo.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/no-dependencies/demo.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        5 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/no-dependencies/demo.egg-info/top_level.txt
--rw-r--r--   0        0        0      329 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/no-dependencies/setup.py
--rw-r--r--   0        0        0       59 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/no-version/demo/__init__.py
--rw-r--r--   0        0        0      696 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/no-version/setup.py
--rw-r--r--   0        0        0      254 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/PKG-INFO
--rw-r--r--   0        0        0      164 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       43 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/requires.txt
--rw-r--r--   0        0        0        5 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/top_level.txt
--rw-r--r--   0        0        0       59 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/non-canonical-name/demo/__init__.py
--rw-r--r--   0        0        0      429 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/non-canonical-name/setup.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/poetry-plugin/poetry_plugin/__init__.py
--rw-r--r--   0        0        0      349 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/poetry-plugin/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/poetry-plugin2/subdir/poetry_plugin/__init__.py
--rw-r--r--   0        0        0      349 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/poetry-plugin2/subdir/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/prerelease/prerelease/__init__.py
--rw-r--r--   0        0        0      268 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/prerelease/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/pyproject-demo/demo/__init__.py
--rw-r--r--   0        0        0      275 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/pyproject-demo/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/subdirectories/one/one/__init__.py
--rw-r--r--   0        0        0      244 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/subdirectories/one/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/subdirectories/one-copy/one/__init__.py
--rw-r--r--   0        0        0      244 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/subdirectories/one-copy/pyproject.toml
--rw-r--r--   0        0        0      252 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/subdirectories/two/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/git/github.com/demo/subdirectories/two/two/__init__.py
--rw-r--r--   0        0        0       34 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/incompatible_lock/poetry.lock
--rw-r--r--   0        0        0      320 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/incompatible_lock/pyproject.toml
--rw-r--r--   0        0        0      378 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/inspection/demo/pyproject.toml
--rw-r--r--   0        0        0      225 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/inspection/demo_no_setup_pkg_info_no_deps/PKG-INFO
--rw-r--r--   0        0        0      461 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/inspection/demo_no_setup_pkg_info_no_deps/pyproject.toml
--rw-r--r--   0        0        0      225 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/inspection/demo_only_requires_txt.egg-info/PKG-INFO
--rw-r--r--   0        0        0       64 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/inspection/demo_only_requires_txt.egg-info/requires.txt
--rw-r--r--   0        0        0      300 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/inspection/demo_poetry_package/pyproject.toml
--rw-r--r--   0        0        0      225 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/inspection/demo_with_obsolete_egg_info/demo-0.1.0.egg-info/PKG-INFO
--rw-r--r--   0        0        0       64 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/inspection/demo_with_obsolete_egg_info/demo-0.1.0.egg-info/requires.txt
--rw-r--r--   0        0        0      378 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/inspection/demo_with_obsolete_egg_info/pyproject.toml
--rw-r--r--   0        0        0       26 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/invalid_lock/poetry.lock
--rw-r--r--   0        0        0      320 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/invalid_lock/pyproject.toml
--rw-r--r--   0        0        0      392 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/invalid_pyproject/pyproject.toml
--rw-r--r--   0        0        0      423 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/missing_directory_dependency/poetry.lock
--rw-r--r--   0        0        0      299 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/missing_directory_dependency/pyproject.toml
--rw-r--r--   0        0        0      445 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/missing_file_dependency/poetry.lock
--rw-r--r--   0        0        0      324 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/missing_file_dependency/pyproject.toml
--rw-r--r--   0        0        0       32 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/no_name_project/README.rst
--rw-r--r--   0        0        0      306 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/no_name_project/pyproject.toml
--rw-r--r--   0        0        0      780 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/old_lock/poetry.lock
--rw-r--r--   0        0        0      320 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/old_lock/pyproject.toml
--rw-r--r--   0        0        0      448 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/old_lock_path_dependency/poetry.lock
--rw-r--r--   0        0        0      336 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/old_lock_path_dependency/pyproject.toml
--rw-r--r--   0        0        0      247 2023-03-19 14:44:45.106397 poetry-1.4.1/tests/fixtures/old_lock_path_dependency/quix/pyproject.toml
--rw-r--r--   0        0        0     6674 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/outdated_lock/poetry.lock
--rw-r--r--   0        0        0      311 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/outdated_lock/pyproject.toml
--rw-r--r--   0        0        0      309 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/private_pyproject/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/project_with_extras/project_with_extras/__init__.py
--rw-r--r--   0        0        0      402 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/project_with_extras/pyproject.toml
--rw-r--r--   0        0        0      881 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/project_with_git_dev_dependency/pyproject.toml
--rw-r--r--   0        0        0      893 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/project_with_local_dependencies/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/project_with_multi_constraints_dependency/project/__init__.py
--rw-r--r--   0        0        0      394 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/project_with_multi_constraints_dependency/pyproject.toml
--rw-r--r--   0        0        0      264 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/project_with_nested_local/bar/pyproject.toml
--rw-r--r--   0        0        0      262 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/project_with_nested_local/foo/pyproject.toml
--rw-r--r--   0        0        0      324 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/project_with_nested_local/pyproject.toml
--rw-r--r--   0        0        0      221 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/project_with_nested_local/quix/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/project_with_setup/my_package/__init__.py
--rw-r--r--   0        0        0      239 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/PKG-INFO
--rw-r--r--   0        0        0      201 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       38 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/requires.txt
--rw-r--r--   0        0        0       11 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/top_level.txt
--rw-r--r--   0        0        0      416 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/project_with_setup/setup.py
--rw-r--r--   0        0        0       22 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/sample_project/README.rst
--rw-r--r--   0        0        0     1493 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/sample_project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/scripts/README.md
--rw-r--r--   0        0        0      400 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/scripts/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/scripts/scripts/__init__.py
--rw-r--r--   0        0        0      557 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/scripts/scripts/check_argv0.py
--rw-r--r--   0        0        0      122 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/scripts/scripts/exit_code.py
--rw-r--r--   0        0        0      128 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/scripts/scripts/return_code.py
--rw-r--r--   0        0        0       22 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/simple_project/README.rst
--rw-r--r--   0        0        0     1320 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1106 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/simple_project/dist/simple_project-1.2.3.tar.gz
--rw-r--r--   0        0        0      775 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/simple_project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/simple_project/simple_project/__init__.py
--rw-r--r--   0        0        0     6669 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/up_to_date_lock/poetry.lock
--rw-r--r--   0        0        0      311 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/up_to_date_lock/pyproject.toml
--rw-r--r--   0        0        0     1722 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/wheel_with_no_requires_dist/demo-0.1.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1062 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with-include/LICENSE
--rw-r--r--   0        0        0       22 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with-include/README.rst
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with-include/extra_dir/README.md
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with-include/extra_dir/__init__.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with-include/extra_dir/sub_pkg/__init__.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with-include/extra_dir/sub_pkg/vcs_excluded.txt
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with-include/extra_dir/vcs_excluded.txt
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with-include/for_wheel_only/__init__.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with-include/my_module.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with-include/notes.txt
--rw-r--r--   0        0        0       59 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with-include/package_with_include/__init__.py
--rw-r--r--   0        0        0     1259 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with-include/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with-include/src/src_package/__init__.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with-include/tests/__init__.py
--rw-r--r--   0        0        0      153 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with_conditional_path_deps/demo_one/pyproject.toml
--rw-r--r--   0        0        0      153 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with_conditional_path_deps/demo_two/pyproject.toml
--rw-r--r--   0        0        0      257 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with_conditional_path_deps/pyproject.toml
--rw-r--r--   0        0        0       22 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with_default_source/README.rst
--rw-r--r--   0        0        0     1412 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with_default_source/pyproject.toml
--rw-r--r--   0        0        0       22 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with_local_config/README.rst
--rw-r--r--   0        0        0       48 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with_local_config/poetry.toml
--rw-r--r--   0        0        0     1327 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with_local_config/pyproject.toml
--rw-r--r--   0        0        0       28 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with_multiple_readme_files/README-1.rst
--rw-r--r--   0        0        0       20 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with_multiple_readme_files/README-2.rst
--rw-r--r--   0        0        0       79 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with_multiple_readme_files/my_package/__init__.py
--rw-r--r--   0        0        0      286 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with_multiple_readme_files/pyproject.toml
--rw-r--r--   0        0        0      421 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with_non_default_multiple_secondary_sources/pyproject.toml
--rw-r--r--   0        0        0      404 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with_non_default_multiple_sources/pyproject.toml
--rw-r--r--   0        0        0      335 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with_non_default_secondary_source/pyproject.toml
--rw-r--r--   0        0        0      318 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with_non_default_source/pyproject.toml
--rw-r--r--   0        0        0       22 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with_two_default_sources/README.rst
--rw-r--r--   0        0        0     1496 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/fixtures/with_two_default_sources/pyproject.toml
--rw-r--r--   0        0        0     8775 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/helpers.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/inspection/__init__.py
--rw-r--r--   0        0        0     7664 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/inspection/test_info.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/__init__.py
--rw-r--r--   0        0        0      636 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/extras-with-dependencies.test
--rw-r--r--   0        0        0      602 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/extras.test
--rw-r--r--   0        0        0      455 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/install-no-dev.test
--rw-r--r--   0        0        0       95 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/no-dependencies.test
--rw-r--r--   0        0        0     4217 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/old-lock.test
--rw-r--r--   0        0        0      206 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/remove.test
--rw-r--r--   0        0        0      206 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/update-with-lock.test
--rw-r--r--   0        0        0      770 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/update-with-locked-extras.test
--rw-r--r--   0        0        0      366 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/with-category-change.test
--rw-r--r--   0        0        0      446 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/with-conditional-dependency.test
--rw-r--r--   0        0        0      563 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/with-dependencies-extras.test
--rw-r--r--   0        0        0      685 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/with-dependencies-nested-extras.test
--rw-r--r--   0        0        0      331 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/with-dependencies.test
--rw-r--r--   0        0        0     2276 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/with-directory-dependency-poetry-transitive.test
--rw-r--r--   0        0        0      634 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/with-directory-dependency-poetry.test
--rw-r--r--   0        0        0      695 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/with-directory-dependency-setuptools.test
--rw-r--r--   0        0        0      525 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/with-duplicate-dependencies-update.test
--rw-r--r--   0        0        0      931 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/with-duplicate-dependencies.test
--rw-r--r--   0        0        0     1451 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/with-file-dependency-transitive.test
--rw-r--r--   0        0        0      712 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/with-file-dependency.test
--rw-r--r--   0        0        0      824 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/with-multiple-updates.test
--rw-r--r--   0        0        0      523 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/with-optional-dependencies.test
--rw-r--r--   0        0        0      637 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/with-platform-dependencies.test
--rw-r--r--   0        0        0      333 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/with-prereleases.test
--rw-r--r--   0        0        0     4894 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/with-pypi-repository.test
--rw-r--r--   0        0        0      478 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/with-python-versions.test
--rw-r--r--   0        0        0     1200 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/with-same-version-url-dependencies.test
--rw-r--r--   0        0        0      651 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/with-sub-dependencies.test
--rw-r--r--   0        0        0      722 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/with-url-dependency.test
--rw-r--r--   0        0        0      762 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/with-vcs-dependency-with-extras.test
--rw-r--r--   0        0        0      527 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/with-vcs-dependency-without-ref.test
--rw-r--r--   0        0        0      496 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/fixtures/with-wheel-dependency-no-requires-dist.test
--rw-r--r--   0        0        0     7380 2023-03-19 14:44:45.110398 poetry-1.4.1/tests/installation/test_chef.py
--rw-r--r--   0        0        0    11061 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/installation/test_chooser.py
--rw-r--r--   0        0        0    35670 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/installation/test_executor.py
--rw-r--r--   0        0        0    78885 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/installation/test_installer.py
--rw-r--r--   0        0        0    56712 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/installation/test_installer_old.py
--rw-r--r--   0        0        0     8776 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/installation/test_pip_installer.py
--rw-r--r--   0        0        0     2706 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/installation/test_wheel_installer.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/integration/__init__.py
--rw-r--r--   0        0        0    10929 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/integration/test_utils_vcs_git.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/json/__init__.py
--rw-r--r--   0        0        0      316 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/json/fixtures/source/complete_invalid.toml
--rw-r--r--   0        0        0      349 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/json/fixtures/source/complete_valid.toml
--rw-r--r--   0        0        0      696 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/json/test_schema_sources.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/masonry/builders/__init__.py
--rw-r--r--   0        0        0       22 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/masonry/builders/fixtures/excluded_subpackage/README.rst
--rw-r--r--   0        0        0       59 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/masonry/builders/fixtures/excluded_subpackage/example/__init__.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/masonry/builders/fixtures/excluded_subpackage/example/test/__init__.py
--rw-r--r--   0        0        0      176 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/masonry/builders/fixtures/excluded_subpackage/example/test/excluded.py
--rw-r--r--   0        0        0      329 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/masonry/builders/fixtures/excluded_subpackage/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/masonry/builders/fixtures/pep_561_stub_only/pkg-stubs/__init__.pyi
--rw-r--r--   0        0        0       83 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/masonry/builders/fixtures/pep_561_stub_only/pkg-stubs/module.pyi
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/masonry/builders/fixtures/pep_561_stub_only/pkg-stubs/subpkg/__init__.pyi
--rw-r--r--   0        0        0      261 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/masonry/builders/fixtures/pep_561_stub_only/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/__init__.pyi
--rw-r--r--   0        0        0       83 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/module.pyi
--rw-r--r--   0        0        0        8 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/py.typed
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/subpkg/__init__.pyi
--rw-r--r--   0        0        0      291 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pyproject.toml
--rw-r--r--   0        0        0      294 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/masonry/builders/fixtures/pep_561_stub_only_src/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/masonry/builders/fixtures/pep_561_stub_only_src/src/pkg-stubs/__init__.pyi
--rw-r--r--   0        0        0       83 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/masonry/builders/fixtures/pep_561_stub_only_src/src/pkg-stubs/module.pyi
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/masonry/builders/fixtures/pep_561_stub_only_src/src/pkg-stubs/subpkg/__init__.pyi
--rw-r--r--   0        0        0    10539 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/masonry/builders/test_editable_builder.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/mixology/__init__.py
--rw-r--r--   0        0        0     2132 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/mixology/helpers.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/mixology/solutions/__init__.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/mixology/solutions/providers/__init__.py
--rw-r--r--   0        0        0     1433 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/mixology/solutions/providers/test_python_requirement_solution_provider.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/mixology/solutions/solutions/__init__.py
--rw-r--r--   0        0        0     1462 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/mixology/solutions/solutions/test_python_requirement_solution.py
--rw-r--r--   0        0        0      109 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/mixology/version_solver/__init__.py
--rw-r--r--   0        0        0     1066 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/mixology/version_solver/conftest.py
--rw-r--r--   0        0        0     6820 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/mixology/version_solver/test_backtracking.py
--rw-r--r--   0        0        0     4294 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/mixology/version_solver/test_basic_graph.py
--rw-r--r--   0        0        0     4399 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/mixology/version_solver/test_dependency_cache.py
--rw-r--r--   0        0        0     1145 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/mixology/version_solver/test_python_constraint.py
--rw-r--r--   0        0        0     5170 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/mixology/version_solver/test_unsolvable.py
--rw-r--r--   0        0        0     7606 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/mixology/version_solver/test_with_lock.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/packages/__init__.py
--rw-r--r--   0        0        0    30069 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/packages/test_locker.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/plugins/__init__.py
--rw-r--r--   0        0        0     3030 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/plugins/test_plugin_manager.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/publishing/__init__.py
--rw-r--r--   0        0        0     6280 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/publishing/test_publisher.py
--rw-r--r--   0        0        0     4646 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/publishing/test_uploader.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/puzzle/__init__.py
--rw-r--r--   0        0        0      528 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/puzzle/conftest.py
--rw-r--r--   0        0        0    24339 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/puzzle/test_provider.py
--rw-r--r--   0        0        0   121407 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/puzzle/test_solver.py
--rw-r--r--   0        0        0     5495 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/puzzle/test_transaction.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.114398 poetry-1.4.1/tests/repositories/__init__.py
--rw-r--r--   0        0        0    16009 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/cleo-0.7.6.dist-info/METADATA
--rw-r--r--   0        0        0      110 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/directory_pep_610-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0       81 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/directory_pep_610-1.2.3.dist-info/direct_url.json
--rw-r--r--   0        0        0      719 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-2.3.4.dist-info/METADATA
--rw-r--r--   0        0        0      731 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-with-import-2.3.4.dist-info/METADATA
--rw-r--r--   0        0        0       10 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-with-import.pth
--rw-r--r--   0        0        0       18 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable.pth
--rw-r--r--   0        0        0      119 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable_directory_pep_610-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0      105 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable_directory_pep_610-1.2.3.dist-info/direct_url.json
--rw-r--r--   0        0        0      105 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/file_pep_610-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0      182 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/file_pep_610-1.2.3.dist-info/direct_url.json
--rw-r--r--   0        0        0     1306 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/foo-0.1.0-py3.8.egg
--rw-r--r--   0        0        0      104 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0      159 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610-1.2.3.dist-info/direct_url.json
--rw-r--r--   0        0        0      125 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610_no_requested_version-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0      141 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610_no_requested_version-1.2.3.dist-info/direct_url.json
--rw-r--r--   0        0        0      117 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610_subdirectory-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0      200 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610_subdirectory-1.2.3.dist-info/direct_url.json
--rw-r--r--   0        0        0      719 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/standard-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0        9 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/standard.pth
--rw-r--r--   0        0        0      104 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/url_pep_610-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0      102 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/url_pep_610-1.2.3.dist-info/direct_url.json
--rw-r--r--   0        0        0      717 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/bender-2.0.5.dist-info/METADATA
--rw-r--r--   0        0        0       20 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/bender.pth
--rw-r--r--   0        0        0      710 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/lib64-2.3.4.dist-info/METADATA
--rw-r--r--   0        0        0      717 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/src/bender/bender.egg-info/PKG-INFO
--rw-r--r--   0        0        0     8866 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/src/pendulum/pendulum.egg-info/PKG-INFO
--rw-r--r--   0        0        0       87 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/src/pendulum/pendulum.egg-info/requires.txt
--rw-r--r--   0        0        0     9020 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/installed/vendor/py3.7/attrs-19.3.0.dist-info/METADATA
--rw-r--r--   0        0        0      731 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/legacy/absolute.html
--rw-r--r--   0        0        0      790 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/legacy/black.html
--rw-r--r--   0        0        0     1455 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/legacy/clikit.html
--rw-r--r--   0        0        0      746 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/legacy/discord-py.html
--rw-r--r--   0        0        0      759 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/legacy/futures-partial-yank.html
--rw-r--r--   0        0        0      747 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/legacy/futures.html
--rw-r--r--   0        0        0      625 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/legacy/invalid-version.html
--rw-r--r--   0        0        0     1433 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/legacy/ipython.html
--rw-r--r--   0        0        0      917 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/legacy/isort.html
--rw-r--r--   0        0        0      333 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/legacy/jupyter.html
--rw-r--r--   0        0        0      348 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/legacy/missing-version.html
--rw-r--r--   0        0        0      401 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/legacy/pastel.html
--rw-r--r--   0        0        0      534 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/legacy/poetry-test-py2-py3-metadata-merge.html
--rw-r--r--   0        0        0      802 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/legacy/pytest.html
--rw-r--r--   0        0        0      467 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/legacy/python-language-server.html
--rw-r--r--   0        0        0      941 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/legacy/pyyaml.html
--rw-r--r--   0        0        0      687 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/legacy/relative.html
--rw-r--r--   0        0        0      473 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/legacy/tomlkit.html
--rw-r--r--   0        0        0    18499 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/SQLAlchemy-1.2.12.tar.gz
--rw-r--r--   0        0        0     9634 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/Twisted-18.9.0.tar.bz2
--rw-r--r--   0        0        0     1940 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/black-19.10b0-py36-none-any.whl
--rw-r--r--   0        0        0    14949 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/black-21.11b0-py3-none-any.whl
--rw-r--r--   0        0        0    78701 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/cleo-1.0.0a5-py3-none-any.whl
--rw-r--r--   0        0        0     2329 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/clikit-0.2.4-py2.py3-none-any.whl
--rw-r--r--   0        0        0     2290 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/discord.py-2.0.0-py3-none-any.whl
--rw-r--r--   0        0        0    15847 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0-py2-none-any.whl
--rw-r--r--   0        0        0    18359 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0.tar.gz
--rw-r--r--   0        0        0    31809 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/importlib_metadata-1.7.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0    23473 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py2-none-any.whl
--rw-r--r--   0        0        0    23475 2023-03-19 14:44:45.118399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py3-none-any.whl
--rw-r--r--   0        0        0    15795 2023-03-19 14:44:45.122399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0.tar.gz
--rw-r--r--   0        0        0    22352 2023-03-19 14:44:45.122399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/ipython-7.5.0-py3-none-any.whl
--rw-r--r--   0        0        0    45393 2023-03-19 14:44:45.122399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py2-none-any.whl
--rw-r--r--   0        0        0    45352 2023-03-19 14:44:45.122399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py3-none-any.whl
--rw-r--r--   0        0        0    56070 2023-03-19 14:44:45.122399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4.tar.gz
--rw-r--r--   0        0        0     2736 2023-03-19 14:44:45.122399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0    12916 2023-03-19 14:44:45.122399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0.tar.gz
--rw-r--r--   0        0        0     4490 2023-03-19 14:44:45.122399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/pastel-0.1.0.tar.gz
--rw-r--r--   0        0        0   464992 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/poetry_core-1.5.0-py3-none-any.whl
--rw-r--r--   0        0        0     1213 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py2-none-any.whl
--rw-r--r--   0        0        0     1218 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py3-none-any.whl
--rw-r--r--   0        0        0     3691 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/pytest-3.5.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0     3708 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/pytest-3.5.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0    54076 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/python-language-server-0.21.2.tar.gz
--rw-r--r--   0        0        0    29813 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.2.tar.gz
--rw-r--r--   0        0        0    29864 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.3.tar.gz
--rw-r--r--   0        0        0     5700 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/zipp-3.5.0-py3-none-any.whl
--rw-r--r--   0        0        0     3421 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/attrs/17.4.0.json
--rw-r--r--   0        0        0      856 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/attrs.json
--rw-r--r--   0        0        0    62683 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/black/19.10b0.json
--rw-r--r--   0        0        0     5924 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/black/21.11b0.json
--rw-r--r--   0        0        0     1709 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/black.json
--rw-r--r--   0        0        0     2298 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/cachecontrol/0.12.5.json
--rw-r--r--   0        0        0     2425 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/cachecontrol.json
--rw-r--r--   0        0        0     3035 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/cleo/1.0.0a5.json
--rw-r--r--   0        0        0     3745 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/clikit/0.2.4.json
--rw-r--r--   0        0        0      997 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/clikit.json
--rw-r--r--   0        0        0     2922 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/colorama/0.3.9.json
--rw-r--r--   0        0        0      867 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/colorama.json
--rw-r--r--   0        0        0     4035 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/discord-py/2.0.0.json
--rw-r--r--   0        0        0     2944 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/funcsigs/1.0.2.json
--rw-r--r--   0        0        0      867 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/funcsigs.json
--rw-r--r--   0        0        0     3838 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/hbmqtt/0.9.6.json
--rw-r--r--   0        0        0    14437 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/hbmqtt.json
--rw-r--r--   0        0        0     5331 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/importlib-metadata/1.7.0.json
--rw-r--r--   0        0        0     1065 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/importlib-metadata.json
--rw-r--r--   0        0        0     5984 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/ipython/4.1.0rc1.json
--rw-r--r--   0        0        0    21476 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/isort/4.3.4.json
--rw-r--r--   0        0        0     1221 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/isort.json
--rw-r--r--   0        0        0     3969 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/jupyter/1.0.0.json
--rw-r--r--   0        0        0     1217 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/jupyter.json
--rw-r--r--   0        0        0     2931 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/lockfile/0.12.2.json
--rw-r--r--   0        0        0      871 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/lockfile.json
--rw-r--r--   0        0        0     3552 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/more-itertools/4.1.0.json
--rw-r--r--   0        0        0     1284 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/more-itertools.json
--rw-r--r--   0        0        0     2328 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/pluggy/0.6.0.json
--rw-r--r--   0        0        0      470 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/pluggy.json
--rw-r--r--   0        0        0     3180 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/poetry/0.12.4.json
--rw-r--r--   0        0        0     3555 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/poetry-core/1.5.0.json
--rw-r--r--   0        0        0      897 2023-03-19 14:44:45.126399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/poetry-core.json
--rw-r--r--   0        0        0     4561 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/poetry.json
--rw-r--r--   0        0        0     3095 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/py/1.5.3.json
--rw-r--r--   0        0        0      837 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/py.json
--rw-r--r--   0        0        0      931 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/pygame-music-grid.json
--rw-r--r--   0        0        0     4469 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/pylev/1.3.0.json
--rw-r--r--   0        0        0      495 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/pylev.json
--rw-r--r--   0        0        0     6933 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/pytest/3.5.0.json
--rw-r--r--   0        0        0     7555 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/pytest/3.5.1.json
--rw-r--r--   0        0        0      857 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/pytest.json
--rw-r--r--   0        0        0    14143 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/pyyaml/3.13.0.json
--rw-r--r--   0        0        0     7805 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/pyyaml.json
--rw-r--r--   0        0        0     3142 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/requests/2.18.4.json
--rw-r--r--   0        0        0    67409 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/requests.json
--rw-r--r--   0        0        0     5315 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/setuptools/39.2.0.json
--rw-r--r--   0        0        0      875 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/setuptools.json
--rw-r--r--   0        0        0     2387 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/six/1.11.0.json
--rw-r--r--   0        0        0      846 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/six.json
--rw-r--r--   0        0        0     8870 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/sqlalchemy/1.2.12.json
--rw-r--r--   0        0        0      484 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/sqlalchemy.json
--rw-r--r--   0        0        0     6109 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/toga.json
--rw-r--r--   0        0        0    11126 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/tomlkit/0.5.3.json
--rw-r--r--   0        0        0     1892 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/tomlkit.json
--rw-r--r--   0        0        0     3184 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/trackpy/0.4.1.json
--rw-r--r--   0        0        0      838 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/trackpy.json
--rw-r--r--   0        0        0    11606 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/twisted/18.9.0.json
--rw-r--r--   0        0        0      477 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/twisted.json
--rw-r--r--   0        0        0     5188 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/zipp/3.5.0.json
--rw-r--r--   0        0        0      907 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/zipp.json
--rw-r--r--   0        0        0   224197 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/pypi.org/search/search.html
--rw-r--r--   0        0        0     3407 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/fixtures/single-page/jax_releases.html
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/link_sources/__init__.py
--rw-r--r--   0        0        0     3108 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/link_sources/test_base.py
--rw-r--r--   0        0        0     2999 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/link_sources/test_html.py
--rw-r--r--   0        0        0    10674 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/test_installed_repository.py
--rw-r--r--   0        0        0    17165 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/test_legacy_repository.py
--rw-r--r--   0        0        0     1772 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/test_lockfile_repository.py
--rw-r--r--   0        0        0    11351 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/test_pypi_repository.py
--rw-r--r--   0        0        0     2321 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/test_repository.py
--rw-r--r--   0        0        0     9148 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/test_repository_pool.py
--rw-r--r--   0        0        0     1982 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/repositories/test_single_page_repository.py
--rw-r--r--   0        0        0    11419 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/test_factory.py
--rw-r--r--   0        0        0      399 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/test_helpers.py
--rw-r--r--   0        0        0     1551 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/types.py
--rw-r--r--   0        0        0        0 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/utils/__init__.py
--rw-r--r--   0        0        0      379 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/utils/conftest.py
--rw-r--r--   0        0        0      604 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/utils/fixtures/pyproject.toml
--rw-r--r--   0        0        0      371 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/utils/fixtures/setups/ansible/requirements.txt
--rw-r--r--   0        0        0    10765 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/utils/fixtures/setups/ansible/setup.py
--rw-r--r--   0        0        0      271 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/utils/fixtures/setups/extras_require_with_vars/setup.py
--rw-r--r--   0        0        0     2581 2023-03-19 14:44:45.130399 poetry-1.4.1/tests/utils/fixtures/setups/flask/setup.py
--rw-r--r--   0        0        0     1353 2023-03-19 14:44:45.134400 poetry-1.4.1/tests/utils/fixtures/setups/pendulum/setup.py
--rw-r--r--   0        0        0    11825 2023-03-19 14:44:45.134400 poetry-1.4.1/tests/utils/fixtures/setups/pyyaml/setup.py
--rw-r--r--   0        0        0     3366 2023-03-19 14:44:45.134400 poetry-1.4.1/tests/utils/fixtures/setups/requests/setup.py
--rw-r--r--   0        0        0      290 2023-03-19 14:44:45.134400 poetry-1.4.1/tests/utils/fixtures/setups/setuptools_setup/setup.py
--rw-r--r--   0        0        0     6272 2023-03-19 14:44:45.134400 poetry-1.4.1/tests/utils/fixtures/setups/sqlalchemy/setup.py
--rw-r--r--   0        0        0      302 2023-03-19 14:44:45.134400 poetry-1.4.1/tests/utils/fixtures/setups/with-setup-cfg/setup.cfg
--rw-r--r--   0        0        0       75 2023-03-19 14:44:45.134400 poetry-1.4.1/tests/utils/fixtures/setups/with-setup-cfg/setup.py
--rw-r--r--   0        0        0      339 2023-03-19 14:44:45.134400 poetry-1.4.1/tests/utils/fixtures/setups/with-setup-cfg-attr/setup.cfg
--rw-r--r--   0        0        0       75 2023-03-19 14:44:45.134400 poetry-1.4.1/tests/utils/fixtures/setups/with-setup-cfg-attr/setup.py
--rw-r--r--   0        0        0    19220 2023-03-19 14:44:45.134400 poetry-1.4.1/tests/utils/test_authenticator.py
--rw-r--r--   0        0        0     5581 2023-03-19 14:44:45.134400 poetry-1.4.1/tests/utils/test_cache.py
--rw-r--r--   0        0        0     4079 2023-03-19 14:44:45.134400 poetry-1.4.1/tests/utils/test_dependency_specification.py
--rw-r--r--   0        0        0    50347 2023-03-19 14:44:45.134400 poetry-1.4.1/tests/utils/test_env.py
--rw-r--r--   0        0        0     1625 2023-03-19 14:44:45.134400 poetry-1.4.1/tests/utils/test_env_site.py
--rw-r--r--   0        0        0     2241 2023-03-19 14:44:45.134400 poetry-1.4.1/tests/utils/test_extras.py
--rw-r--r--   0        0        0     5126 2023-03-19 14:44:45.134400 poetry-1.4.1/tests/utils/test_helpers.py
--rw-r--r--   0        0        0     7260 2023-03-19 14:44:45.134400 poetry-1.4.1/tests/utils/test_password_manager.py
--rw-r--r--   0        0        0     1077 2023-03-19 14:44:45.134400 poetry-1.4.1/tests/utils/test_patterns.py
--rw-r--r--   0        0        0     1012 2023-03-19 14:44:45.134400 poetry-1.4.1/tests/utils/test_pip.py
--rw-r--r--   0        0        0     6613 2023-03-19 14:44:45.134400 poetry-1.4.1/tests/utils/test_setup_reader.py
--rw-r--r--   0        0        0     1025 2023-03-19 14:44:45.134400 poetry-1.4.1/tests/utils/test_source.py
--rw-r--r--   0        0        0     7099 1970-01-01 00:00:00.000000 poetry-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-02 16:01:45.129953 poetry-1.4.2/LICENSE
+-rw-r--r--   0        0        0     4547 2023-04-02 16:01:45.129953 poetry-1.4.2/README.md
+-rw-r--r--   0        0        0     5180 2023-04-02 16:01:45.145953 poetry-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0      146 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/__main__.py
+-rw-r--r--   0        0        0      342 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/__version__.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/config/__init__.py
+-rw-r--r--   0        0        0     9688 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/config/config.py
+-rw-r--r--   0        0        0      261 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/config/config_source.py
+-rw-r--r--   0        0        0     1018 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/config/dict_config_source.py
+-rw-r--r--   0        0        0     2338 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/config/file_config_source.py
+-rw-r--r--   0        0        0      339 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/config/source.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/__init__.py
+-rw-r--r--   0        0        0    12765 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/application.py
+-rw-r--r--   0        0        0      615 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/command_loader.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/__init__.py
+-rw-r--r--   0        0        0      915 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/about.py
+-rw-r--r--   0        0        0    10289 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/add.py
+-rw-r--r--   0        0        0     1081 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/build.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/cache/__init__.py
+-rw-r--r--   0        0        0     2411 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/cache/clear.py
+-rw-r--r--   0        0        0      634 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/cache/list.py
+-rw-r--r--   0        0        0     3366 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/check.py
+-rw-r--r--   0        0        0     1118 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/command.py
+-rw-r--r--   0        0        0    11052 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/config.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/debug/__init__.py
+-rw-r--r--   0        0        0      764 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/debug/info.py
+-rw-r--r--   0        0        0     4459 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/debug/resolve.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/env/__init__.py
+-rw-r--r--   0        0        0     2310 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/env/info.py
+-rw-r--r--   0        0        0      822 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/env/list.py
+-rw-r--r--   0        0        0     1478 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/env/remove.py
+-rw-r--r--   0        0        0      706 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/env/use.py
+-rw-r--r--   0        0        0      544 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/env_command.py
+-rw-r--r--   0        0        0     3372 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/group_command.py
+-rw-r--r--   0        0        0    17297 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/init.py
+-rw-r--r--   0        0        0     6470 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/install.py
+-rw-r--r--   0        0        0      907 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/installer_command.py
+-rw-r--r--   0        0        0     1738 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/lock.py
+-rw-r--r--   0        0        0     3047 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/new.py
+-rw-r--r--   0        0        0     2784 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/publish.py
+-rw-r--r--   0        0        0     5013 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/remove.py
+-rw-r--r--   0        0        0     2697 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/run.py
+-rw-r--r--   0        0        0      786 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/search.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/self/__init__.py
+-rw-r--r--   0        0        0     1262 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/self/add.py
+-rw-r--r--   0        0        0      973 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/self/install.py
+-rw-r--r--   0        0        0      642 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/self/lock.py
+-rw-r--r--   0        0        0      607 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/self/remove.py
+-rw-r--r--   0        0        0     4493 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/self/self_command.py
+-rw-r--r--   0        0        0     1209 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/self/show/__init__.py
+-rw-r--r--   0        0        0     4096 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/self/show/plugins.py
+-rw-r--r--   0        0        0     1802 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/self/update.py
+-rw-r--r--   0        0        0     1527 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/shell.py
+-rw-r--r--   0        0        0    19612 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/show.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/source/__init__.py
+-rw-r--r--   0        0        0     3128 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/source/add.py
+-rw-r--r--   0        0        0     1133 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/source/remove.py
+-rw-r--r--   0        0        0     1755 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/source/show.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/source/update.py
+-rw-r--r--   0        0        0     1773 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/update.py
+-rw-r--r--   0        0        0     3775 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/commands/version.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/events/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/events/console_events.py
+-rw-r--r--   0        0        0      122 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/io/inputs/__init__.py
+-rw-r--r--   0        0        0     2582 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/io/inputs/run_argv_input.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/logging/__init__.py
+-rw-r--r--   0        0        0       99 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/logging/filters.py
+-rw-r--r--   0        0        0      336 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/logging/formatters/__init__.py
+-rw-r--r--   0        0        0      788 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/logging/formatters/builder_formatter.py
+-rw-r--r--   0        0        0      132 2023-04-02 16:01:45.145953 poetry-1.4.2/src/poetry/console/logging/formatters/formatter.py
+-rw-r--r--   0        0        0     1026 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/console/logging/io_formatter.py
+-rw-r--r--   0        0        0      718 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/console/logging/io_handler.py
+-rw-r--r--   0        0        0      134 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/exceptions.py
+-rw-r--r--   0        0        0    10059 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/factory.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/inspection/__init__.py
+-rw-r--r--   0        0        0    21835 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/inspection/info.py
+-rw-r--r--   0        0        0      114 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/installation/__init__.py
+-rw-r--r--   0        0        0      430 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/installation/base_installer.py
+-rw-r--r--   0        0        0     8853 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/installation/chef.py
+-rw-r--r--   0        0        0     8029 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/installation/chooser.py
+-rw-r--r--   0        0        0    35199 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/installation/executor.py
+-rw-r--r--   0        0        0    19912 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/installation/installer.py
+-rw-r--r--   0        0        0      979 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/installation/noop_installer.py
+-rw-r--r--   0        0        0      262 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/installation/operations/__init__.py
+-rw-r--r--   0        0        0      906 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/installation/operations/install.py
+-rw-r--r--   0        0        0     1315 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/installation/operations/operation.py
+-rw-r--r--   0        0        0      959 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/installation/operations/uninstall.py
+-rw-r--r--   0        0        0     1540 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/installation/operations/update.py
+-rw-r--r--   0        0        0    10103 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/installation/pip_installer.py
+-rw-r--r--   0        0        0     3736 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/installation/wheel_installer.py
+-rw-r--r--   0        0        0     1311 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/json/__init__.py
+-rw-r--r--   0        0        0     1552 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/json/schemas/poetry.json
+-rw-r--r--   0        0        0      310 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/layouts/__init__.py
+-rw-r--r--   0        0        0     6072 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/layouts/layout.py
+-rw-r--r--   0        0        0      202 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/layouts/src.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/layouts/standard.py
+-rw-r--r--   0        0        0     1657 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/locations.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/masonry/__init__.py
+-rw-r--r--   0        0        0      497 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/masonry/api.py
+-rw-r--r--   0        0        0      129 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/masonry/builders/__init__.py
+-rw-r--r--   0        0        0     9599 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/masonry/builders/editable.py
+-rw-r--r--   0        0        0      467 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/mixology/__init__.py
+-rw-r--r--   0        0        0     1555 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/mixology/assignment.py
+-rw-r--r--   0        0        0    10186 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/mixology/failure.py
+-rw-r--r--   0        0        0    15346 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/mixology/incompatibility.py
+-rw-r--r--   0        0        0     1903 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/mixology/incompatibility_cause.py
+-rw-r--r--   0        0        0     7080 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/mixology/partial_solution.py
+-rw-r--r--   0        0        0      676 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/mixology/result.py
+-rw-r--r--   0        0        0      211 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/mixology/set_relation.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/mixology/solutions/__init__.py
+-rw-r--r--   0        0        0      214 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/mixology/solutions/providers/__init__.py
+-rw-r--r--   0        0        0     1091 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/mixology/solutions/providers/python_requirement_solution_provider.py
+-rw-r--r--   0        0        0      189 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/mixology/solutions/solutions/__init__.py
+-rw-r--r--   0        0        0     2281 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/mixology/solutions/solutions/python_requirement_solution.py
+-rw-r--r--   0        0        0     6904 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/mixology/term.py
+-rw-r--r--   0        0        0    19826 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/mixology/version_solver.py
+-rw-r--r--   0        0        0      273 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/packages/__init__.py
+-rw-r--r--   0        0        0     1297 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/packages/dependency_package.py
+-rw-r--r--   0        0        0    17314 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/packages/locker.py
+-rw-r--r--   0        0        0      921 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/packages/package_collection.py
+-rw-r--r--   0        0        0      185 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/plugins/__init__.py
+-rw-r--r--   0        0        0      687 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/plugins/application_plugin.py
+-rw-r--r--   0        0        0      435 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/plugins/base_plugin.py
+-rw-r--r--   0        0        0      484 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/plugins/plugin.py
+-rw-r--r--   0        0        0     2567 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/plugins/plugin_manager.py
+-rw-r--r--   0        0        0     2114 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/poetry.py
+-rw-r--r--   0        0        0      112 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/publishing/__init__.py
+-rw-r--r--   0        0        0     2893 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/publishing/publisher.py
+-rw-r--r--   0        0        0    12483 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/publishing/uploader.py
+-rw-r--r--   0        0        0       99 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/puzzle/__init__.py
+-rw-r--r--   0        0        0      799 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/puzzle/exceptions.py
+-rw-r--r--   0        0        0    40439 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/puzzle/provider.py
+-rw-r--r--   0        0        0    11539 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/puzzle/solver.py
+-rw-r--r--   0        0        0     5124 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/puzzle/transaction.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/py.typed
+-rw-r--r--   0        0        0      198 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/repositories/__init__.py
+-rw-r--r--   0        0        0      833 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/repositories/abstract_repository.py
+-rw-r--r--   0        0        0     2553 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/repositories/cached_repository.py
+-rw-r--r--   0        0        0      125 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/repositories/exceptions.py
+-rw-r--r--   0        0        0    11550 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/repositories/http_repository.py
+-rw-r--r--   0        0        0    10342 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/repositories/installed_repository.py
+-rw-r--r--   0        0        0     4474 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/repositories/legacy_repository.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/repositories/link_sources/__init__.py
+-rw-r--r--   0        0        0     3835 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/repositories/link_sources/base.py
+-rw-r--r--   0        0        0     1955 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/repositories/link_sources/html.py
+-rw-r--r--   0        0        0     1227 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/repositories/link_sources/json.py
+-rw-r--r--   0        0        0      841 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/repositories/lockfile_repository.py
+-rw-r--r--   0        0        0     8452 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/repositories/pypi_repository.py
+-rw-r--r--   0        0        0     3978 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/repositories/repository.py
+-rw-r--r--   0        0        0     4783 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/repositories/repository_pool.py
+-rw-r--r--   0        0        0      753 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/repositories/single_page_repository.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/utils/__init__.py
+-rw-r--r--   0        0        0     1639 2023-04-02 16:01:45.149953 poetry-1.4.2/src/poetry/utils/_compat.py
+-rw-r--r--   0        0        0    16540 2023-04-02 16:01:45.153953 poetry-1.4.2/src/poetry/utils/authenticator.py
+-rw-r--r--   0        0        0     5509 2023-04-02 16:01:45.153953 poetry-1.4.2/src/poetry/utils/cache.py
+-rw-r--r--   0        0        0      115 2023-04-02 16:01:45.153953 poetry-1.4.2/src/poetry/utils/constants.py
+-rw-r--r--   0        0        0     6993 2023-04-02 16:01:45.153953 poetry-1.4.2/src/poetry/utils/dependency_specification.py
+-rw-r--r--   0        0        0    67563 2023-04-02 16:01:45.153953 poetry-1.4.2/src/poetry/utils/env.py
+-rw-r--r--   0        0        0     1848 2023-04-02 16:01:45.153953 poetry-1.4.2/src/poetry/utils/extras.py
+-rw-r--r--   0        0        0     7416 2023-04-02 16:01:45.153953 poetry-1.4.2/src/poetry/utils/helpers.py
+-rw-r--r--   0        0        0     7339 2023-04-02 16:01:45.153953 poetry-1.4.2/src/poetry/utils/password_manager.py
+-rw-r--r--   0        0        0      406 2023-04-02 16:01:45.153953 poetry-1.4.2/src/poetry/utils/patterns.py
+-rw-r--r--   0        0        0     1463 2023-04-02 16:01:45.153953 poetry-1.4.2/src/poetry/utils/pip.py
+-rw-r--r--   0        0        0    12143 2023-04-02 16:01:45.153953 poetry-1.4.2/src/poetry/utils/setup_reader.py
+-rw-r--r--   0        0        0     4290 2023-04-02 16:01:45.153953 poetry-1.4.2/src/poetry/utils/shell.py
+-rw-r--r--   0        0        0      446 2023-04-02 16:01:45.153953 poetry-1.4.2/src/poetry/utils/source.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.153953 poetry-1.4.2/src/poetry/vcs/__init__.py
+-rw-r--r--   0        0        0       95 2023-04-02 16:01:45.153953 poetry-1.4.2/src/poetry/vcs/git/__init__.py
+-rw-r--r--   0        0        0    16101 2023-04-02 16:01:45.153953 poetry-1.4.2/src/poetry/vcs/git/backend.py
+-rw-r--r--   0        0        0     1771 2023-04-02 16:01:45.153953 poetry-1.4.2/src/poetry/vcs/git/system.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.153953 poetry-1.4.2/src/poetry/version/__init__.py
+-rw-r--r--   0        0        0     1573 2023-04-02 16:01:45.153953 poetry-1.4.2/src/poetry/version/version_selector.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/__init__.py
+-rw-r--r--   0        0        0      274 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/compat.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/config/__init__.py
+-rw-r--r--   0        0        0     2265 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/config/test_config.py
+-rw-r--r--   0        0        0    13346 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/cache/__init__.py
+-rw-r--r--   0        0        0     1458 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/cache/conftest.py
+-rw-r--r--   0        0        0     2237 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/cache/test_clear.py
+-rw-r--r--   0        0        0      816 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/cache/test_list.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/debug/__init__.py
+-rw-r--r--   0        0        0     1776 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/debug/test_resolve.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/env/__init__.py
+-rw-r--r--   0        0        0     2336 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/env/conftest.py
+-rw-r--r--   0        0        0     1077 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/env/helpers.py
+-rw-r--r--   0        0        0     1374 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/env/test_info.py
+-rw-r--r--   0        0        0     2030 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/env/test_list.py
+-rw-r--r--   0        0        0     2880 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/env/test_remove.py
+-rw-r--r--   0        0        0     4387 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/env/test_use.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/self/__init__.py
+-rw-r--r--   0        0        0     2333 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/self/conftest.py
+-rw-r--r--   0        0        0       65 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/self/fixtures/poetry-1.0.5-darwin.sha256sum
+-rw-r--r--   0        0        0     1041 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/self/fixtures/poetry-1.0.5-darwin.tar.gz
+-rw-r--r--   0        0        0     7167 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/self/test_add_plugins.py
+-rw-r--r--   0        0        0     3015 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/self/test_remove_plugins.py
+-rw-r--r--   0        0        0     5665 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/self/test_show_plugins.py
+-rw-r--r--   0        0        0     2160 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/self/test_update.py
+-rw-r--r--   0        0        0     1069 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/self/utils.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/source/__init__.py
+-rw-r--r--   0        0        0     1716 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/source/conftest.py
+-rw-r--r--   0        0        0     3035 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/source/test_add.py
+-rw-r--r--   0        0        0     1254 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/source/test_remove.py
+-rw-r--r--   0        0        0     2102 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/source/test_show.py
+-rw-r--r--   0        0        0      827 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/test_about.py
+-rw-r--r--   0        0        0    56270 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/test_add.py
+-rw-r--r--   0        0        0     1258 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/test_build.py
+-rw-r--r--   0        0        0     2012 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/test_check.py
+-rw-r--r--   0        0        0     8649 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/test_config.py
+-rw-r--r--   0        0        0    29495 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/test_init.py
+-rw-r--r--   0        0        0    10196 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/test_install.py
+-rw-r--r--   0        0        0    10247 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/test_lock.py
+-rw-r--r--   0        0        0     5943 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/test_new.py
+-rw-r--r--   0        0        0     3698 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/test_publish.py
+-rw-r--r--   0        0        0     9026 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/test_remove.py
+-rw-r--r--   0        0        0     6178 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/test_run.py
+-rw-r--r--   0        0        0     2560 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/test_search.py
+-rw-r--r--   0        0        0     2332 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/test_shell.py
+-rw-r--r--   0        0        0    65807 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/test_show.py
+-rw-r--r--   0        0        0     1633 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/test_update.py
+-rw-r--r--   0        0        0     2486 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/commands/test_version.py
+-rw-r--r--   0        0        0     5047 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/conftest.py
+-rw-r--r--   0        0        0     3120 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/console/test_application.py
+-rw-r--r--   0        0        0       22 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/fixtures/build_system_requires_not_available/README.rst
+-rw-r--r--   0        0        0      676 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/fixtures/build_system_requires_not_available/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/fixtures/build_system_requires_not_available/simple_project/__init__.py
+-rw-r--r--   0        0        0     1168 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/fixtures/complete.toml
+-rw-r--r--   0        0        0      424 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/fixtures/deleted_directory_dependency/poetry.lock
+-rw-r--r--   0        0        0      234 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/fixtures/deleted_directory_dependency/pyproject.toml
+-rw-r--r--   0        0        0      446 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/fixtures/deleted_file_dependency/poetry.lock
+-rw-r--r--   0        0        0      234 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/fixtures/deleted_file_dependency/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/fixtures/directory/project_with_transitive_directory_dependencies/project_with_transitive_directory_dependencies/__init__.py
+-rw-r--r--   0        0        0      418 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/fixtures/directory/project_with_transitive_directory_dependencies/pyproject.toml
+-rw-r--r--   0        0        0      574 2023-04-02 16:01:45.153953 poetry-1.4.2/tests/fixtures/directory/project_with_transitive_directory_dependencies/setup.py
+-rw-r--r--   0        0        0      234 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/directory/project_with_transitive_file_dependencies/inner-directory-project/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/directory/project_with_transitive_file_dependencies/project_with_transitive_file_dependencies/__init__.py
+-rw-r--r--   0        0        0      385 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/directory/project_with_transitive_file_dependencies/pyproject.toml
+-rw-r--r--   0        0        0     1116 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1003 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/distributions/demo-0.1.0.tar.gz
+-rw-r--r--   0        0        0     1552 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/distributions/demo-0.1.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1169 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/distributions/demo_invalid_record-0.1.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1307 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/distributions/demo_invalid_record2-0.1.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0       22 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/excluded_subpackage/README.rst
+-rw-r--r--   0        0        0       59 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/excluded_subpackage/example/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/excluded_subpackage/example/test/__init__.py
+-rw-r--r--   0        0        0      159 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/excluded_subpackage/example/test/excluded.py
+-rw-r--r--   0        0        0      329 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/excluded_subpackage/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/extended_project/README.rst
+-rw-r--r--   0        0        0      362 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/extended_project/build.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/extended_project/extended_project/__init__.py
+-rw-r--r--   0        0        0      652 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/extended_project/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/extended_project_without_setup/README.rst
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/extended_project_without_setup/build.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/extended_project_without_setup/extended_project/__init__.py
+-rw-r--r--   0        0        0      756 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/extended_project_without_setup/pyproject.toml
+-rw-r--r--   0        0        0       18 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/extended_with_no_setup/README.md
+-rw-r--r--   0        0        0      852 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/extended_with_no_setup/build.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/extended_with_no_setup/extended/__init__.py
+-rw-r--r--   0        0        0      888 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/extended_with_no_setup/extended/extended.c
+-rw-r--r--   0        0        0      559 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/extended_with_no_setup/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/demo/demo/__init__.py
+-rw-r--r--   0        0        0      226 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/demo/demo.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      164 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/demo/demo.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/demo/demo.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       43 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/demo/demo.egg-info/requires.txt
+-rw-r--r--   0        0        0        5 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/demo/demo.egg-info/top_level.txt
+-rw-r--r--   0        0        0      429 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/demo/setup.py
+-rw-r--r--   0        0        0       93 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/namespace-package-one/namespace_package/__init__.py
+-rw-r--r--   0        0        0       50 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/namespace-package-one/namespace_package/one/__init__.py
+-rw-r--r--   0        0        0      402 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/namespace-package-one/setup.py
+-rw-r--r--   0        0        0       59 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/no-dependencies/demo/__init__.py
+-rw-r--r--   0        0        0      214 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/no-dependencies/demo.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      137 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/no-dependencies/demo.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/no-dependencies/demo.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        5 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/no-dependencies/demo.egg-info/top_level.txt
+-rw-r--r--   0        0        0      329 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/no-dependencies/setup.py
+-rw-r--r--   0        0        0       59 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/no-version/demo/__init__.py
+-rw-r--r--   0        0        0      696 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/no-version/setup.py
+-rw-r--r--   0        0        0      254 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      164 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       43 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/requires.txt
+-rw-r--r--   0        0        0        5 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/top_level.txt
+-rw-r--r--   0        0        0       59 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/non-canonical-name/demo/__init__.py
+-rw-r--r--   0        0        0      429 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/non-canonical-name/setup.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/poetry-plugin/poetry_plugin/__init__.py
+-rw-r--r--   0        0        0      349 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/poetry-plugin/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/poetry-plugin2/subdir/poetry_plugin/__init__.py
+-rw-r--r--   0        0        0      349 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/poetry-plugin2/subdir/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/prerelease/prerelease/__init__.py
+-rw-r--r--   0        0        0      268 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/prerelease/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/pyproject-demo/demo/__init__.py
+-rw-r--r--   0        0        0      275 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/pyproject-demo/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/subdirectories/one/one/__init__.py
+-rw-r--r--   0        0        0      244 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/subdirectories/one/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/subdirectories/one-copy/one/__init__.py
+-rw-r--r--   0        0        0      244 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/subdirectories/one-copy/pyproject.toml
+-rw-r--r--   0        0        0      252 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/subdirectories/two/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/git/github.com/demo/subdirectories/two/two/__init__.py
+-rw-r--r--   0        0        0       34 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/incompatible_lock/poetry.lock
+-rw-r--r--   0        0        0      320 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/incompatible_lock/pyproject.toml
+-rw-r--r--   0        0        0      378 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/inspection/demo/pyproject.toml
+-rw-r--r--   0        0        0      225 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/inspection/demo_no_setup_pkg_info_no_deps/PKG-INFO
+-rw-r--r--   0        0        0      461 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/inspection/demo_no_setup_pkg_info_no_deps/pyproject.toml
+-rw-r--r--   0        0        0      225 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/inspection/demo_only_requires_txt.egg-info/PKG-INFO
+-rw-r--r--   0        0        0       64 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/inspection/demo_only_requires_txt.egg-info/requires.txt
+-rw-r--r--   0        0        0      300 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/inspection/demo_poetry_package/pyproject.toml
+-rw-r--r--   0        0        0      225 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/inspection/demo_with_obsolete_egg_info/demo-0.1.0.egg-info/PKG-INFO
+-rw-r--r--   0        0        0       64 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/inspection/demo_with_obsolete_egg_info/demo-0.1.0.egg-info/requires.txt
+-rw-r--r--   0        0        0      378 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/inspection/demo_with_obsolete_egg_info/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/invalid_lock/poetry.lock
+-rw-r--r--   0        0        0      320 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/invalid_lock/pyproject.toml
+-rw-r--r--   0        0        0      392 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/invalid_pyproject/pyproject.toml
+-rw-r--r--   0        0        0      423 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/missing_directory_dependency/poetry.lock
+-rw-r--r--   0        0        0      299 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/missing_directory_dependency/pyproject.toml
+-rw-r--r--   0        0        0      445 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/missing_file_dependency/poetry.lock
+-rw-r--r--   0        0        0      324 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/missing_file_dependency/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/no_name_project/README.rst
+-rw-r--r--   0        0        0      306 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/no_name_project/pyproject.toml
+-rw-r--r--   0        0        0      780 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/old_lock/poetry.lock
+-rw-r--r--   0        0        0      320 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/old_lock/pyproject.toml
+-rw-r--r--   0        0        0      448 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/old_lock_path_dependency/poetry.lock
+-rw-r--r--   0        0        0      336 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/old_lock_path_dependency/pyproject.toml
+-rw-r--r--   0        0        0      247 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/old_lock_path_dependency/quix/pyproject.toml
+-rw-r--r--   0        0        0     6674 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/outdated_lock/poetry.lock
+-rw-r--r--   0        0        0      311 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/outdated_lock/pyproject.toml
+-rw-r--r--   0        0        0      309 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/private_pyproject/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/project_with_extras/project_with_extras/__init__.py
+-rw-r--r--   0        0        0      402 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/project_with_extras/pyproject.toml
+-rw-r--r--   0        0        0      881 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/project_with_git_dev_dependency/pyproject.toml
+-rw-r--r--   0        0        0      893 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/project_with_local_dependencies/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/project_with_multi_constraints_dependency/project/__init__.py
+-rw-r--r--   0        0        0      394 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/project_with_multi_constraints_dependency/pyproject.toml
+-rw-r--r--   0        0        0      264 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/project_with_nested_local/bar/pyproject.toml
+-rw-r--r--   0        0        0      262 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/project_with_nested_local/foo/pyproject.toml
+-rw-r--r--   0        0        0      324 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/project_with_nested_local/pyproject.toml
+-rw-r--r--   0        0        0      221 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/project_with_nested_local/quix/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/project_with_setup/my_package/__init__.py
+-rw-r--r--   0        0        0      239 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/project_with_setup/project_with_setup.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      201 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/project_with_setup/project_with_setup.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/project_with_setup/project_with_setup.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       38 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/project_with_setup/project_with_setup.egg-info/requires.txt
+-rw-r--r--   0        0        0       11 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/project_with_setup/project_with_setup.egg-info/top_level.txt
+-rw-r--r--   0        0        0      416 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/project_with_setup/setup.py
+-rw-r--r--   0        0        0       22 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/sample_project/README.rst
+-rw-r--r--   0        0        0     1493 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/sample_project/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/scripts/README.md
+-rw-r--r--   0        0        0      400 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/scripts/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/scripts/scripts/__init__.py
+-rw-r--r--   0        0        0      557 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/scripts/scripts/check_argv0.py
+-rw-r--r--   0        0        0      122 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/scripts/scripts/exit_code.py
+-rw-r--r--   0        0        0      128 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/scripts/scripts/return_code.py
+-rw-r--r--   0        0        0       22 2023-04-02 16:01:45.157953 poetry-1.4.2/tests/fixtures/simple_project/README.rst
+-rw-r--r--   0        0        0     1320 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1106 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/simple_project/dist/simple_project-1.2.3.tar.gz
+-rw-r--r--   0        0        0      775 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/simple_project/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/simple_project/simple_project/__init__.py
+-rw-r--r--   0        0        0     6669 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/up_to_date_lock/poetry.lock
+-rw-r--r--   0        0        0      311 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/up_to_date_lock/pyproject.toml
+-rw-r--r--   0        0        0     1722 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/wheel_with_no_requires_dist/demo-0.1.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1062 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with-include/LICENSE
+-rw-r--r--   0        0        0       22 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with-include/README.rst
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with-include/extra_dir/README.md
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with-include/extra_dir/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with-include/extra_dir/sub_pkg/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with-include/extra_dir/sub_pkg/vcs_excluded.txt
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with-include/extra_dir/vcs_excluded.txt
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with-include/for_wheel_only/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with-include/my_module.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with-include/notes.txt
+-rw-r--r--   0        0        0       59 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with-include/package_with_include/__init__.py
+-rw-r--r--   0        0        0     1259 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with-include/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with-include/src/src_package/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with-include/tests/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with_conditional_path_deps/demo_one/pyproject.toml
+-rw-r--r--   0        0        0      153 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with_conditional_path_deps/demo_two/pyproject.toml
+-rw-r--r--   0        0        0      257 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with_conditional_path_deps/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with_default_source/README.rst
+-rw-r--r--   0        0        0     1412 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with_default_source/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with_local_config/README.rst
+-rw-r--r--   0        0        0       48 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with_local_config/poetry.toml
+-rw-r--r--   0        0        0     1327 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with_local_config/pyproject.toml
+-rw-r--r--   0        0        0       28 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with_multiple_readme_files/README-1.rst
+-rw-r--r--   0        0        0       20 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with_multiple_readme_files/README-2.rst
+-rw-r--r--   0        0        0       79 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with_multiple_readme_files/my_package/__init__.py
+-rw-r--r--   0        0        0      286 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with_multiple_readme_files/pyproject.toml
+-rw-r--r--   0        0        0      421 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with_non_default_multiple_secondary_sources/pyproject.toml
+-rw-r--r--   0        0        0      404 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with_non_default_multiple_sources/pyproject.toml
+-rw-r--r--   0        0        0      335 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with_non_default_secondary_source/pyproject.toml
+-rw-r--r--   0        0        0      318 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with_non_default_source/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with_two_default_sources/README.rst
+-rw-r--r--   0        0        0     1496 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/fixtures/with_two_default_sources/pyproject.toml
+-rw-r--r--   0        0        0     8775 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/helpers.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/inspection/__init__.py
+-rw-r--r--   0        0        0     7664 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/inspection/test_info.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/__init__.py
+-rw-r--r--   0        0        0      636 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/extras-with-dependencies.test
+-rw-r--r--   0        0        0      602 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/extras.test
+-rw-r--r--   0        0        0      455 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/install-no-dev.test
+-rw-r--r--   0        0        0       95 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/no-dependencies.test
+-rw-r--r--   0        0        0     4217 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/old-lock.test
+-rw-r--r--   0        0        0      206 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/remove.test
+-rw-r--r--   0        0        0      206 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/update-with-lock.test
+-rw-r--r--   0        0        0      770 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/update-with-locked-extras.test
+-rw-r--r--   0        0        0      366 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/with-category-change.test
+-rw-r--r--   0        0        0      446 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/with-conditional-dependency.test
+-rw-r--r--   0        0        0      563 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/with-dependencies-extras.test
+-rw-r--r--   0        0        0      685 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/with-dependencies-nested-extras.test
+-rw-r--r--   0        0        0      331 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/with-dependencies.test
+-rw-r--r--   0        0        0     2276 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/with-directory-dependency-poetry-transitive.test
+-rw-r--r--   0        0        0      634 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/with-directory-dependency-poetry.test
+-rw-r--r--   0        0        0      695 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/with-directory-dependency-setuptools.test
+-rw-r--r--   0        0        0      525 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/with-duplicate-dependencies-update.test
+-rw-r--r--   0        0        0      931 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/with-duplicate-dependencies.test
+-rw-r--r--   0        0        0     1451 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/with-file-dependency-transitive.test
+-rw-r--r--   0        0        0      712 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/with-file-dependency.test
+-rw-r--r--   0        0        0      824 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/with-multiple-updates.test
+-rw-r--r--   0        0        0      523 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/with-optional-dependencies.test
+-rw-r--r--   0        0        0      637 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/with-platform-dependencies.test
+-rw-r--r--   0        0        0      333 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/with-prereleases.test
+-rw-r--r--   0        0        0     4894 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/with-pypi-repository.test
+-rw-r--r--   0        0        0      478 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/with-python-versions.test
+-rw-r--r--   0        0        0     1200 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/with-same-version-url-dependencies.test
+-rw-r--r--   0        0        0      651 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/with-sub-dependencies.test
+-rw-r--r--   0        0        0      722 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/with-url-dependency.test
+-rw-r--r--   0        0        0      762 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/with-vcs-dependency-with-extras.test
+-rw-r--r--   0        0        0      527 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/with-vcs-dependency-without-ref.test
+-rw-r--r--   0        0        0      496 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/fixtures/with-wheel-dependency-no-requires-dist.test
+-rw-r--r--   0        0        0     7427 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/test_chef.py
+-rw-r--r--   0        0        0    11061 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/test_chooser.py
+-rw-r--r--   0        0        0    37483 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/test_executor.py
+-rw-r--r--   0        0        0    78885 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/test_installer.py
+-rw-r--r--   0        0        0    56712 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/test_installer_old.py
+-rw-r--r--   0        0        0     8776 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/test_pip_installer.py
+-rw-r--r--   0        0        0     2706 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/installation/test_wheel_installer.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/integration/__init__.py
+-rw-r--r--   0        0        0    11884 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/integration/test_utils_vcs_git.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/json/__init__.py
+-rw-r--r--   0        0        0      316 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/json/fixtures/source/complete_invalid.toml
+-rw-r--r--   0        0        0      349 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/json/fixtures/source/complete_valid.toml
+-rw-r--r--   0        0        0      696 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/json/test_schema_sources.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/masonry/builders/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/masonry/builders/fixtures/excluded_subpackage/README.rst
+-rw-r--r--   0        0        0       59 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/masonry/builders/fixtures/excluded_subpackage/example/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/masonry/builders/fixtures/excluded_subpackage/example/test/__init__.py
+-rw-r--r--   0        0        0      176 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/masonry/builders/fixtures/excluded_subpackage/example/test/excluded.py
+-rw-r--r--   0        0        0      329 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/masonry/builders/fixtures/excluded_subpackage/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/masonry/builders/fixtures/pep_561_stub_only/pkg-stubs/__init__.pyi
+-rw-r--r--   0        0        0       83 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/masonry/builders/fixtures/pep_561_stub_only/pkg-stubs/module.pyi
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/masonry/builders/fixtures/pep_561_stub_only/pkg-stubs/subpkg/__init__.pyi
+-rw-r--r--   0        0        0      261 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/masonry/builders/fixtures/pep_561_stub_only/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/__init__.pyi
+-rw-r--r--   0        0        0       83 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/module.pyi
+-rw-r--r--   0        0        0        8 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/py.typed
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/subpkg/__init__.pyi
+-rw-r--r--   0        0        0      291 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pyproject.toml
+-rw-r--r--   0        0        0      294 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/masonry/builders/fixtures/pep_561_stub_only_src/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/masonry/builders/fixtures/pep_561_stub_only_src/src/pkg-stubs/__init__.pyi
+-rw-r--r--   0        0        0       83 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/masonry/builders/fixtures/pep_561_stub_only_src/src/pkg-stubs/module.pyi
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/masonry/builders/fixtures/pep_561_stub_only_src/src/pkg-stubs/subpkg/__init__.pyi
+-rw-r--r--   0        0        0    10539 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/masonry/builders/test_editable_builder.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.161953 poetry-1.4.2/tests/mixology/__init__.py
+-rw-r--r--   0        0        0     2132 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/mixology/helpers.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/mixology/solutions/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/mixology/solutions/providers/__init__.py
+-rw-r--r--   0        0        0     1433 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/mixology/solutions/providers/test_python_requirement_solution_provider.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/mixology/solutions/solutions/__init__.py
+-rw-r--r--   0        0        0     1462 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/mixology/solutions/solutions/test_python_requirement_solution.py
+-rw-r--r--   0        0        0      109 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/mixology/version_solver/__init__.py
+-rw-r--r--   0        0        0     1066 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/mixology/version_solver/conftest.py
+-rw-r--r--   0        0        0     6820 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/mixology/version_solver/test_backtracking.py
+-rw-r--r--   0        0        0     4294 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/mixology/version_solver/test_basic_graph.py
+-rw-r--r--   0        0        0     4399 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/mixology/version_solver/test_dependency_cache.py
+-rw-r--r--   0        0        0     1145 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/mixology/version_solver/test_python_constraint.py
+-rw-r--r--   0        0        0     5170 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/mixology/version_solver/test_unsolvable.py
+-rw-r--r--   0        0        0     7606 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/mixology/version_solver/test_with_lock.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/packages/__init__.py
+-rw-r--r--   0        0        0    30069 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/packages/test_locker.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/plugins/__init__.py
+-rw-r--r--   0        0        0     3030 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/plugins/test_plugin_manager.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/publishing/__init__.py
+-rw-r--r--   0        0        0     6280 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/publishing/test_publisher.py
+-rw-r--r--   0        0        0     4646 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/publishing/test_uploader.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/puzzle/__init__.py
+-rw-r--r--   0        0        0      528 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/puzzle/conftest.py
+-rw-r--r--   0        0        0    24339 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/puzzle/test_provider.py
+-rw-r--r--   0        0        0   121407 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/puzzle/test_solver.py
+-rw-r--r--   0        0        0     5495 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/puzzle/test_transaction.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/__init__.py
+-rw-r--r--   0        0        0    16009 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/cleo-0.7.6.dist-info/METADATA
+-rw-r--r--   0        0        0      110 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/directory_pep_610-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0       81 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/directory_pep_610-1.2.3.dist-info/direct_url.json
+-rw-r--r--   0        0        0      719 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-2.3.4.dist-info/METADATA
+-rw-r--r--   0        0        0      731 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-with-import-2.3.4.dist-info/METADATA
+-rw-r--r--   0        0        0       10 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-with-import.pth
+-rw-r--r--   0        0        0       18 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable.pth
+-rw-r--r--   0        0        0      119 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable_directory_pep_610-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0      105 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable_directory_pep_610-1.2.3.dist-info/direct_url.json
+-rw-r--r--   0        0        0      105 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/file_pep_610-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0      182 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/file_pep_610-1.2.3.dist-info/direct_url.json
+-rw-r--r--   0        0        0     1306 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/foo-0.1.0-py3.8.egg
+-rw-r--r--   0        0        0      104 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0      159 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610-1.2.3.dist-info/direct_url.json
+-rw-r--r--   0        0        0      125 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610_no_requested_version-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0      141 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610_no_requested_version-1.2.3.dist-info/direct_url.json
+-rw-r--r--   0        0        0      117 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610_subdirectory-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0      200 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610_subdirectory-1.2.3.dist-info/direct_url.json
+-rw-r--r--   0        0        0      719 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/standard-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0        9 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/standard.pth
+-rw-r--r--   0        0        0      104 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/url_pep_610-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0      102 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/url_pep_610-1.2.3.dist-info/direct_url.json
+-rw-r--r--   0        0        0      717 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/bender-2.0.5.dist-info/METADATA
+-rw-r--r--   0        0        0       20 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/bender.pth
+-rw-r--r--   0        0        0      710 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/lib64-2.3.4.dist-info/METADATA
+-rw-r--r--   0        0        0      717 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/src/bender/bender.egg-info/PKG-INFO
+-rw-r--r--   0        0        0     8866 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/src/pendulum/pendulum.egg-info/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/src/pendulum/pendulum.egg-info/requires.txt
+-rw-r--r--   0        0        0     9020 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/installed/vendor/py3.7/attrs-19.3.0.dist-info/METADATA
+-rw-r--r--   0        0        0      731 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/legacy/absolute.html
+-rw-r--r--   0        0        0      790 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/legacy/black.html
+-rw-r--r--   0        0        0     1455 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/legacy/clikit.html
+-rw-r--r--   0        0        0      746 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/legacy/discord-py.html
+-rw-r--r--   0        0        0      759 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/legacy/futures-partial-yank.html
+-rw-r--r--   0        0        0      747 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/legacy/futures.html
+-rw-r--r--   0        0        0      625 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/legacy/invalid-version.html
+-rw-r--r--   0        0        0     1433 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/legacy/ipython.html
+-rw-r--r--   0        0        0      917 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/legacy/isort.html
+-rw-r--r--   0        0        0      333 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/legacy/jupyter.html
+-rw-r--r--   0        0        0      348 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/legacy/missing-version.html
+-rw-r--r--   0        0        0      401 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/legacy/pastel.html
+-rw-r--r--   0        0        0      534 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/legacy/poetry-test-py2-py3-metadata-merge.html
+-rw-r--r--   0        0        0      802 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/legacy/pytest.html
+-rw-r--r--   0        0        0      467 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/legacy/python-language-server.html
+-rw-r--r--   0        0        0      941 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/legacy/pyyaml.html
+-rw-r--r--   0        0        0      687 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/legacy/relative.html
+-rw-r--r--   0        0        0      473 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/legacy/tomlkit.html
+-rw-r--r--   0        0        0    18499 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/SQLAlchemy-1.2.12.tar.gz
+-rw-r--r--   0        0        0     9634 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/Twisted-18.9.0.tar.bz2
+-rw-r--r--   0        0        0     1940 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/black-19.10b0-py36-none-any.whl
+-rw-r--r--   0        0        0    14949 2023-04-02 16:01:45.165953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/black-21.11b0-py3-none-any.whl
+-rw-r--r--   0        0        0    78701 2023-04-02 16:01:45.169953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/cleo-1.0.0a5-py3-none-any.whl
+-rw-r--r--   0        0        0     2329 2023-04-02 16:01:45.169953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/clikit-0.2.4-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     2290 2023-04-02 16:01:45.169953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/discord.py-2.0.0-py3-none-any.whl
+-rw-r--r--   0        0        0    15847 2023-04-02 16:01:45.169953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0-py2-none-any.whl
+-rw-r--r--   0        0        0    18359 2023-04-02 16:01:45.169953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0.tar.gz
+-rw-r--r--   0        0        0    31809 2023-04-02 16:01:45.169953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/importlib_metadata-1.7.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    23473 2023-04-02 16:01:45.169953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py2-none-any.whl
+-rw-r--r--   0        0        0    23475 2023-04-02 16:01:45.169953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py3-none-any.whl
+-rw-r--r--   0        0        0    15795 2023-04-02 16:01:45.169953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0.tar.gz
+-rw-r--r--   0        0        0    22352 2023-04-02 16:01:45.169953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/ipython-7.5.0-py3-none-any.whl
+-rw-r--r--   0        0        0    45393 2023-04-02 16:01:45.169953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py2-none-any.whl
+-rw-r--r--   0        0        0    45352 2023-04-02 16:01:45.169953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py3-none-any.whl
+-rw-r--r--   0        0        0    56070 2023-04-02 16:01:45.169953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4.tar.gz
+-rw-r--r--   0        0        0     2736 2023-04-02 16:01:45.169953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    12916 2023-04-02 16:01:45.169953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0.tar.gz
+-rw-r--r--   0        0        0     4490 2023-04-02 16:01:45.169953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/pastel-0.1.0.tar.gz
+-rw-r--r--   0        0        0   464992 2023-04-02 16:01:45.173953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/poetry_core-1.5.0-py3-none-any.whl
+-rw-r--r--   0        0        0     1213 2023-04-02 16:01:45.173953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py2-none-any.whl
+-rw-r--r--   0        0        0     1218 2023-04-02 16:01:45.173953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py3-none-any.whl
+-rw-r--r--   0        0        0     3691 2023-04-02 16:01:45.173953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/pytest-3.5.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     3708 2023-04-02 16:01:45.173953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/pytest-3.5.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    54076 2023-04-02 16:01:45.173953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/python-language-server-0.21.2.tar.gz
+-rw-r--r--   0        0        0    29813 2023-04-02 16:01:45.173953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.2.tar.gz
+-rw-r--r--   0        0        0    29864 2023-04-02 16:01:45.173953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.3.tar.gz
+-rw-r--r--   0        0        0     5700 2023-04-02 16:01:45.173953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/zipp-3.5.0-py3-none-any.whl
+-rw-r--r--   0        0        0     3421 2023-04-02 16:01:45.173953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/attrs/17.4.0.json
+-rw-r--r--   0        0        0      856 2023-04-02 16:01:45.173953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/attrs.json
+-rw-r--r--   0        0        0    62683 2023-04-02 16:01:45.173953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/black/19.10b0.json
+-rw-r--r--   0        0        0     5924 2023-04-02 16:01:45.173953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/black/21.11b0.json
+-rw-r--r--   0        0        0     1709 2023-04-02 16:01:45.173953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/black.json
+-rw-r--r--   0        0        0     2298 2023-04-02 16:01:45.173953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/cachecontrol/0.12.5.json
+-rw-r--r--   0        0        0     2425 2023-04-02 16:01:45.173953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/cachecontrol.json
+-rw-r--r--   0        0        0     3035 2023-04-02 16:01:45.173953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/cleo/1.0.0a5.json
+-rw-r--r--   0        0        0     3745 2023-04-02 16:01:45.173953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/clikit/0.2.4.json
+-rw-r--r--   0        0        0      997 2023-04-02 16:01:45.173953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/clikit.json
+-rw-r--r--   0        0        0     2922 2023-04-02 16:01:45.173953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/colorama/0.3.9.json
+-rw-r--r--   0        0        0      867 2023-04-02 16:01:45.173953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/colorama.json
+-rw-r--r--   0        0        0     4035 2023-04-02 16:01:45.173953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/discord-py/2.0.0.json
+-rw-r--r--   0        0        0     2944 2023-04-02 16:01:45.173953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/funcsigs/1.0.2.json
+-rw-r--r--   0        0        0      867 2023-04-02 16:01:45.173953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/funcsigs.json
+-rw-r--r--   0        0        0     3838 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/hbmqtt/0.9.6.json
+-rw-r--r--   0        0        0    14437 2023-04-02 16:01:45.173953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/hbmqtt.json
+-rw-r--r--   0        0        0     5331 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/importlib-metadata/1.7.0.json
+-rw-r--r--   0        0        0     1065 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/importlib-metadata.json
+-rw-r--r--   0        0        0     5984 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/ipython/4.1.0rc1.json
+-rw-r--r--   0        0        0    21476 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/isort/4.3.4.json
+-rw-r--r--   0        0        0     1221 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/isort.json
+-rw-r--r--   0        0        0     3969 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/jupyter/1.0.0.json
+-rw-r--r--   0        0        0     1217 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/jupyter.json
+-rw-r--r--   0        0        0     2931 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/lockfile/0.12.2.json
+-rw-r--r--   0        0        0      871 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/lockfile.json
+-rw-r--r--   0        0        0     3552 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/more-itertools/4.1.0.json
+-rw-r--r--   0        0        0     1284 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/more-itertools.json
+-rw-r--r--   0        0        0     2328 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/pluggy/0.6.0.json
+-rw-r--r--   0        0        0      470 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/pluggy.json
+-rw-r--r--   0        0        0     3180 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/poetry/0.12.4.json
+-rw-r--r--   0        0        0     3555 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/poetry-core/1.5.0.json
+-rw-r--r--   0        0        0      897 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/poetry-core.json
+-rw-r--r--   0        0        0     4561 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/poetry.json
+-rw-r--r--   0        0        0     3095 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/py/1.5.3.json
+-rw-r--r--   0        0        0      837 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/py.json
+-rw-r--r--   0        0        0      931 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/pygame-music-grid.json
+-rw-r--r--   0        0        0     4469 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/pylev/1.3.0.json
+-rw-r--r--   0        0        0      495 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/pylev.json
+-rw-r--r--   0        0        0     6933 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/pytest/3.5.0.json
+-rw-r--r--   0        0        0     7555 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/pytest/3.5.1.json
+-rw-r--r--   0        0        0      857 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/pytest.json
+-rw-r--r--   0        0        0    14143 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/pyyaml/3.13.0.json
+-rw-r--r--   0        0        0     7805 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/pyyaml.json
+-rw-r--r--   0        0        0     3142 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/requests/2.18.4.json
+-rw-r--r--   0        0        0    67409 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/requests.json
+-rw-r--r--   0        0        0     5315 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/setuptools/39.2.0.json
+-rw-r--r--   0        0        0      875 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/setuptools.json
+-rw-r--r--   0        0        0     2387 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/six/1.11.0.json
+-rw-r--r--   0        0        0      846 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/six.json
+-rw-r--r--   0        0        0     8870 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/sqlalchemy/1.2.12.json
+-rw-r--r--   0        0        0      484 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/sqlalchemy.json
+-rw-r--r--   0        0        0     6109 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/toga.json
+-rw-r--r--   0        0        0    11126 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/tomlkit/0.5.3.json
+-rw-r--r--   0        0        0     1892 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/tomlkit.json
+-rw-r--r--   0        0        0     3184 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/trackpy/0.4.1.json
+-rw-r--r--   0        0        0      838 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/trackpy.json
+-rw-r--r--   0        0        0    11606 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/twisted/18.9.0.json
+-rw-r--r--   0        0        0      477 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/twisted.json
+-rw-r--r--   0        0        0     5188 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/zipp/3.5.0.json
+-rw-r--r--   0        0        0      907 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/zipp.json
+-rw-r--r--   0        0        0   224197 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/pypi.org/search/search.html
+-rw-r--r--   0        0        0     3407 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/fixtures/single-page/jax_releases.html
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/link_sources/__init__.py
+-rw-r--r--   0        0        0     3108 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/link_sources/test_base.py
+-rw-r--r--   0        0        0     2999 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/link_sources/test_html.py
+-rw-r--r--   0        0        0    10674 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/test_installed_repository.py
+-rw-r--r--   0        0        0    17165 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/test_legacy_repository.py
+-rw-r--r--   0        0        0     1772 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/test_lockfile_repository.py
+-rw-r--r--   0        0        0    11351 2023-04-02 16:01:45.177953 poetry-1.4.2/tests/repositories/test_pypi_repository.py
+-rw-r--r--   0        0        0     2321 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/repositories/test_repository.py
+-rw-r--r--   0        0        0     9148 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/repositories/test_repository_pool.py
+-rw-r--r--   0        0        0     1982 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/repositories/test_single_page_repository.py
+-rw-r--r--   0        0        0    11419 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/test_factory.py
+-rw-r--r--   0        0        0      399 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/test_helpers.py
+-rw-r--r--   0        0        0     1551 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/types.py
+-rw-r--r--   0        0        0        0 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/__init__.py
+-rw-r--r--   0        0        0      379 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/conftest.py
+-rw-r--r--   0        0        0      604 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/fixtures/pyproject.toml
+-rw-r--r--   0        0        0      371 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/fixtures/setups/ansible/requirements.txt
+-rw-r--r--   0        0        0    10765 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/fixtures/setups/ansible/setup.py
+-rw-r--r--   0        0        0      271 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/fixtures/setups/extras_require_with_vars/setup.py
+-rw-r--r--   0        0        0     2581 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/fixtures/setups/flask/setup.py
+-rw-r--r--   0        0        0     1353 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/fixtures/setups/pendulum/setup.py
+-rw-r--r--   0        0        0    11825 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/fixtures/setups/pyyaml/setup.py
+-rw-r--r--   0        0        0     3366 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/fixtures/setups/requests/setup.py
+-rw-r--r--   0        0        0      290 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/fixtures/setups/setuptools_setup/setup.py
+-rw-r--r--   0        0        0     6272 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/fixtures/setups/sqlalchemy/setup.py
+-rw-r--r--   0        0        0      302 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/fixtures/setups/with-setup-cfg/setup.cfg
+-rw-r--r--   0        0        0       75 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/fixtures/setups/with-setup-cfg/setup.py
+-rw-r--r--   0        0        0      339 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/fixtures/setups/with-setup-cfg-attr/setup.cfg
+-rw-r--r--   0        0        0       75 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/fixtures/setups/with-setup-cfg-attr/setup.py
+-rw-r--r--   0        0        0    19220 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/test_authenticator.py
+-rw-r--r--   0        0        0     5581 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/test_cache.py
+-rw-r--r--   0        0        0     4079 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/test_dependency_specification.py
+-rw-r--r--   0        0        0    51146 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/test_env.py
+-rw-r--r--   0        0        0     1625 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/test_env_site.py
+-rw-r--r--   0        0        0     2241 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/test_extras.py
+-rw-r--r--   0        0        0     5126 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/test_helpers.py
+-rw-r--r--   0        0        0     7260 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/test_password_manager.py
+-rw-r--r--   0        0        0     1077 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/test_patterns.py
+-rw-r--r--   0        0        0     1012 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/test_pip.py
+-rw-r--r--   0        0        0     6613 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/test_setup_reader.py
+-rw-r--r--   0        0        0     1025 2023-04-02 16:01:45.181953 poetry-1.4.2/tests/utils/test_source.py
+-rw-r--r--   0        0        0     7099 1970-01-01 00:00:00.000000 poetry-1.4.2/PKG-INFO
```

### Comparing `poetry-1.4.1/LICENSE` & `poetry-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/README.md` & `poetry-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/pyproject.toml` & `poetry-1.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry"
-version = "1.4.1"
+version = "1.4.2"
 description = "Python dependency management and packaging made easy."
 authors = [
     "Sébastien Eustace <sebastien@eustace.io>",
 ]
 maintainers = [
     "Arun Babu Neelicattu <arun.neelicattu@gmail.com>",
     "Bjorn Neergaard <bjorn@neersighted.com>",
```

### Comparing `poetry-1.4.1/src/poetry/config/config.py` & `poetry-1.4.2/src/poetry/config/config.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/config/dict_config_source.py` & `poetry-1.4.2/src/poetry/config/dict_config_source.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/config/file_config_source.py` & `poetry-1.4.2/src/poetry/config/file_config_source.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/application.py` & `poetry-1.4.2/src/poetry/console/application.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/command_loader.py` & `poetry-1.4.2/src/poetry/console/command_loader.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/about.py` & `poetry-1.4.2/src/poetry/console/commands/about.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/add.py` & `poetry-1.4.2/src/poetry/console/commands/add.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/build.py` & `poetry-1.4.2/src/poetry/console/commands/build.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/cache/clear.py` & `poetry-1.4.2/src/poetry/console/commands/cache/clear.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/cache/list.py` & `poetry-1.4.2/src/poetry/console/commands/cache/list.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/check.py` & `poetry-1.4.2/src/poetry/console/commands/check.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/command.py` & `poetry-1.4.2/src/poetry/console/commands/command.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/config.py` & `poetry-1.4.2/src/poetry/console/commands/config.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/debug/info.py` & `poetry-1.4.2/src/poetry/console/commands/debug/info.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/debug/resolve.py` & `poetry-1.4.2/src/poetry/console/commands/debug/resolve.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/env/info.py` & `poetry-1.4.2/src/poetry/console/commands/env/info.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/env/list.py` & `poetry-1.4.2/src/poetry/console/commands/env/list.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/env/remove.py` & `poetry-1.4.2/src/poetry/console/commands/env/remove.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/env/use.py` & `poetry-1.4.2/src/poetry/console/commands/env/use.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/env_command.py` & `poetry-1.4.2/src/poetry/console/commands/env_command.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/group_command.py` & `poetry-1.4.2/src/poetry/console/commands/group_command.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/init.py` & `poetry-1.4.2/src/poetry/console/commands/init.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/install.py` & `poetry-1.4.2/src/poetry/console/commands/install.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/installer_command.py` & `poetry-1.4.2/src/poetry/console/commands/installer_command.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/lock.py` & `poetry-1.4.2/src/poetry/console/commands/lock.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/new.py` & `poetry-1.4.2/src/poetry/console/commands/new.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/publish.py` & `poetry-1.4.2/src/poetry/console/commands/publish.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/remove.py` & `poetry-1.4.2/src/poetry/console/commands/remove.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/run.py` & `poetry-1.4.2/src/poetry/console/commands/run.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/search.py` & `poetry-1.4.2/src/poetry/console/commands/search.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/self/add.py` & `poetry-1.4.2/src/poetry/console/commands/self/add.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/self/install.py` & `poetry-1.4.2/src/poetry/console/commands/self/install.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/self/lock.py` & `poetry-1.4.2/src/poetry/console/commands/self/lock.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/self/remove.py` & `poetry-1.4.2/src/poetry/console/commands/self/remove.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/self/self_command.py` & `poetry-1.4.2/src/poetry/console/commands/self/self_command.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/self/show/__init__.py` & `poetry-1.4.2/src/poetry/console/commands/self/show/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/self/show/plugins.py` & `poetry-1.4.2/src/poetry/console/commands/self/show/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/self/update.py` & `poetry-1.4.2/src/poetry/console/commands/self/update.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/shell.py` & `poetry-1.4.2/src/poetry/console/commands/shell.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/show.py` & `poetry-1.4.2/src/poetry/console/commands/show.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/source/add.py` & `poetry-1.4.2/src/poetry/console/commands/source/add.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/source/remove.py` & `poetry-1.4.2/src/poetry/console/commands/source/remove.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/source/show.py` & `poetry-1.4.2/src/poetry/console/commands/source/show.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/update.py` & `poetry-1.4.2/src/poetry/console/commands/update.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/commands/version.py` & `poetry-1.4.2/src/poetry/console/commands/version.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/io/inputs/run_argv_input.py` & `poetry-1.4.2/src/poetry/console/io/inputs/run_argv_input.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/logging/formatters/builder_formatter.py` & `poetry-1.4.2/src/poetry/console/logging/formatters/builder_formatter.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/logging/io_formatter.py` & `poetry-1.4.2/src/poetry/console/logging/io_formatter.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/console/logging/io_handler.py` & `poetry-1.4.2/src/poetry/console/logging/io_handler.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/factory.py` & `poetry-1.4.2/src/poetry/factory.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/inspection/info.py` & `poetry-1.4.2/src/poetry/inspection/info.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/installation/chef.py` & `poetry-1.4.2/src/poetry/installation/chef.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/installation/chooser.py` & `poetry-1.4.2/src/poetry/installation/chooser.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/installation/executor.py` & `poetry-1.4.2/src/poetry/installation/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,14 +201,22 @@
                 [task.cancel() for task in tasks]
                 self._executor.shutdown(wait=True)
 
                 break
 
         for warning in self._yanked_warnings:
             self._io.write_error_line(f"<warning>Warning: {warning}</warning>")
+        for path, issues in self._wheel_installer.invalid_wheels.items():
+            formatted_issues = "\n".join(issues)
+            warning = (
+                f"Validation of the RECORD file of {path.name} failed."
+                " Please report to the maintainers of that package so they can fix"
+                f" their build process. Details:\n{formatted_issues}\n"
+            )
+            self._io.write_error_line(f"<warning>Warning: {warning}</warning>")
 
         return 1 if self._shutdown else 0
 
     @staticmethod
     def _get_max_workers(desired_max_workers: int | None = None) -> int:
         # This should be directly handled by ThreadPoolExecutor
         # however, on some systems the number of CPUs cannot be determined
```

### Comparing `poetry-1.4.1/src/poetry/installation/installer.py` & `poetry-1.4.2/src/poetry/installation/installer.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/installation/noop_installer.py` & `poetry-1.4.2/src/poetry/installation/noop_installer.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/installation/operations/install.py` & `poetry-1.4.2/src/poetry/installation/operations/install.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/installation/operations/operation.py` & `poetry-1.4.2/src/poetry/installation/operations/operation.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/installation/operations/uninstall.py` & `poetry-1.4.2/src/poetry/installation/operations/uninstall.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/installation/operations/update.py` & `poetry-1.4.2/src/poetry/installation/operations/update.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/installation/pip_installer.py` & `poetry-1.4.2/src/poetry/installation/pip_installer.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/installation/wheel_installer.py` & `poetry-1.4.2/src/poetry/installation/wheel_installer.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 from installer import install
 from installer.destinations import SchemeDictionaryDestination
 from installer.sources import WheelFile
+from installer.sources import _WheelFileValidationError
 
 from poetry.__version__ import __version__
 from poetry.utils._compat import WINDOWS
 
 
 if TYPE_CHECKING:
     from typing import BinaryIO
@@ -89,20 +90,25 @@
         schemes = self._env.paths
         schemes["headers"] = schemes["include"]
 
         self._destination = WheelDestination(
             schemes, interpreter=self._env.python, script_kind=script_kind
         )
 
+        self.invalid_wheels: dict[Path, list[str]] = {}
+
     def enable_bytecode_compilation(self, enable: bool = True) -> None:
         self._destination.bytecode_optimization_levels = (-1,) if enable else ()
 
     def install(self, wheel: Path) -> None:
         with WheelFile.open(wheel) as source:
-            source.validate_record()
+            try:
+                source.validate_record()
+            except _WheelFileValidationError as e:
+                self.invalid_wheels[wheel] = e.issues
             install(
                 source=source,
                 destination=self._destination.for_source(source),
                 # Additional metadata that is generated by the installation tool.
                 additional_metadata={
                     "INSTALLER": f"Poetry {__version__}".encode(),
                 },
```

### Comparing `poetry-1.4.1/src/poetry/json/__init__.py` & `poetry-1.4.2/src/poetry/json/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/json/schemas/poetry.json` & `poetry-1.4.2/src/poetry/json/schemas/poetry.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/layouts/layout.py` & `poetry-1.4.2/src/poetry/layouts/layout.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/locations.py` & `poetry-1.4.2/src/poetry/locations.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/masonry/builders/editable.py` & `poetry-1.4.2/src/poetry/masonry/builders/editable.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/mixology/assignment.py` & `poetry-1.4.2/src/poetry/mixology/assignment.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/mixology/failure.py` & `poetry-1.4.2/src/poetry/mixology/failure.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/mixology/incompatibility.py` & `poetry-1.4.2/src/poetry/mixology/incompatibility.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/mixology/incompatibility_cause.py` & `poetry-1.4.2/src/poetry/mixology/incompatibility_cause.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/mixology/partial_solution.py` & `poetry-1.4.2/src/poetry/mixology/partial_solution.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/mixology/result.py` & `poetry-1.4.2/src/poetry/mixology/result.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/mixology/solutions/providers/python_requirement_solution_provider.py` & `poetry-1.4.2/src/poetry/mixology/solutions/providers/python_requirement_solution_provider.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/mixology/solutions/solutions/python_requirement_solution.py` & `poetry-1.4.2/src/poetry/mixology/solutions/solutions/python_requirement_solution.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/mixology/term.py` & `poetry-1.4.2/src/poetry/mixology/term.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/mixology/version_solver.py` & `poetry-1.4.2/src/poetry/mixology/version_solver.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/packages/dependency_package.py` & `poetry-1.4.2/src/poetry/packages/dependency_package.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/packages/locker.py` & `poetry-1.4.2/src/poetry/packages/locker.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/packages/package_collection.py` & `poetry-1.4.2/src/poetry/packages/package_collection.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/plugins/application_plugin.py` & `poetry-1.4.2/src/poetry/plugins/application_plugin.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/plugins/plugin_manager.py` & `poetry-1.4.2/src/poetry/plugins/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/poetry.py` & `poetry-1.4.2/src/poetry/poetry.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/publishing/publisher.py` & `poetry-1.4.2/src/poetry/publishing/publisher.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/publishing/uploader.py` & `poetry-1.4.2/src/poetry/publishing/uploader.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/puzzle/exceptions.py` & `poetry-1.4.2/src/poetry/puzzle/exceptions.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/puzzle/provider.py` & `poetry-1.4.2/src/poetry/puzzle/provider.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/puzzle/solver.py` & `poetry-1.4.2/src/poetry/puzzle/solver.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/puzzle/transaction.py` & `poetry-1.4.2/src/poetry/puzzle/transaction.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/repositories/abstract_repository.py` & `poetry-1.4.2/src/poetry/repositories/abstract_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/repositories/cached_repository.py` & `poetry-1.4.2/src/poetry/repositories/cached_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/repositories/http_repository.py` & `poetry-1.4.2/src/poetry/repositories/http_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/repositories/installed_repository.py` & `poetry-1.4.2/src/poetry/repositories/installed_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/repositories/legacy_repository.py` & `poetry-1.4.2/src/poetry/repositories/legacy_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/repositories/link_sources/base.py` & `poetry-1.4.2/src/poetry/repositories/link_sources/base.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/repositories/link_sources/html.py` & `poetry-1.4.2/src/poetry/repositories/link_sources/html.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/repositories/link_sources/json.py` & `poetry-1.4.2/src/poetry/repositories/link_sources/json.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/repositories/lockfile_repository.py` & `poetry-1.4.2/src/poetry/repositories/lockfile_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/repositories/pypi_repository.py` & `poetry-1.4.2/src/poetry/repositories/pypi_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/repositories/repository.py` & `poetry-1.4.2/src/poetry/repositories/repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/repositories/repository_pool.py` & `poetry-1.4.2/src/poetry/repositories/repository_pool.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/repositories/single_page_repository.py` & `poetry-1.4.2/src/poetry/repositories/single_page_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/utils/_compat.py` & `poetry-1.4.2/src/poetry/utils/_compat.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/utils/authenticator.py` & `poetry-1.4.2/src/poetry/utils/authenticator.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/utils/cache.py` & `poetry-1.4.2/src/poetry/utils/cache.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/utils/dependency_specification.py` & `poetry-1.4.2/src/poetry/utils/dependency_specification.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/utils/env.py` & `poetry-1.4.2/src/poetry/utils/env.py`

 * *Files 0% similar despite different names*

```diff
@@ -1533,17 +1533,16 @@
                     stderr=stderr,
                     input=encode(input_),
                     check=True,
                     env=env,
                     **kwargs,
                 ).stdout
             elif call:
-                return subprocess.call(
-                    cmd, stdout=subprocess.PIPE, stderr=stderr, env=env, **kwargs
-                )
+                assert stderr != subprocess.PIPE
+                return subprocess.call(cmd, stderr=stderr, env=env, **kwargs)
             else:
                 output = subprocess.check_output(cmd, stderr=stderr, env=env, **kwargs)
         except CalledProcessError as e:
             raise EnvCommandError(e, input=input_)
 
         return decode(output)
```

### Comparing `poetry-1.4.1/src/poetry/utils/extras.py` & `poetry-1.4.2/src/poetry/utils/extras.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/utils/helpers.py` & `poetry-1.4.2/src/poetry/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/utils/password_manager.py` & `poetry-1.4.2/src/poetry/utils/password_manager.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/utils/pip.py` & `poetry-1.4.2/src/poetry/utils/pip.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/utils/setup_reader.py` & `poetry-1.4.2/src/poetry/utils/setup_reader.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/utils/shell.py` & `poetry-1.4.2/src/poetry/utils/shell.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/vcs/git/backend.py` & `poetry-1.4.2/src/poetry/vcs/git/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import dataclasses
 import logging
 import re
 
 from pathlib import Path
 from subprocess import CalledProcessError
 from typing import TYPE_CHECKING
+from urllib.parse import urljoin
 
 from dulwich import porcelain
 from dulwich.client import HTTPUnauthorized
 from dulwich.client import get_transport_and_path
 from dulwich.config import ConfigFile
 from dulwich.config import parse_submodules
 from dulwich.errors import NotGitRepository
@@ -327,24 +328,32 @@
     def _clone_submodules(cls, repo: Repo) -> None:
         """
         Helper method to identify configured submodules and clone them recursively.
         """
         repo_root = Path(repo.path)
         modules_config = repo_root.joinpath(".gitmodules")
 
+        # A relative URL by definition starts with ../ or ./
+        relative_submodule_regex = re.compile(r"^\.{1,2}/")
+
         if modules_config.exists():
             config = ConfigFile.from_path(str(modules_config))
 
             url: bytes
             path: bytes
             submodules = parse_submodules(config)
+
             for path, url, name in submodules:
                 path_relative = Path(path.decode("utf-8"))
                 path_absolute = repo_root.joinpath(path_relative)
 
+                url_string = url.decode("utf-8")
+                if relative_submodule_regex.search(url_string):
+                    url_string = urljoin(f"{Git.get_remote_url(repo)}/", url_string)
+
                 source_root = path_absolute.parent
                 source_root.mkdir(parents=True, exist_ok=True)
 
                 with repo:
                     try:
                         revision = repo.open_index()[path].sha.decode("utf-8")
                     except KeyError:
@@ -353,15 +362,15 @@
                             name,
                             repo.path,
                             path,
                         )
                         continue
 
                 cls.clone(
-                    url=url.decode("utf-8"),
+                    url=url_string,
                     source_root=source_root,
                     name=path_relative.name,
                     revision=revision,
                     clean=path_absolute.exists()
                     and not path_absolute.joinpath(".git").is_dir(),
                 )
```

### Comparing `poetry-1.4.1/src/poetry/vcs/git/system.py` & `poetry-1.4.2/src/poetry/vcs/git/system.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/src/poetry/version/version_selector.py` & `poetry-1.4.2/src/poetry/version/version_selector.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/config/test_config.py` & `poetry-1.4.2/tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/conftest.py` & `poetry-1.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/cache/conftest.py` & `poetry-1.4.2/tests/console/commands/cache/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/cache/test_clear.py` & `poetry-1.4.2/tests/console/commands/cache/test_clear.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/cache/test_list.py` & `poetry-1.4.2/tests/console/commands/cache/test_list.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/debug/test_resolve.py` & `poetry-1.4.2/tests/console/commands/debug/test_resolve.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/env/conftest.py` & `poetry-1.4.2/tests/console/commands/env/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/env/helpers.py` & `poetry-1.4.2/tests/console/commands/env/helpers.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/env/test_info.py` & `poetry-1.4.2/tests/console/commands/env/test_info.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/env/test_list.py` & `poetry-1.4.2/tests/console/commands/env/test_list.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/env/test_remove.py` & `poetry-1.4.2/tests/console/commands/env/test_remove.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/env/test_use.py` & `poetry-1.4.2/tests/console/commands/env/test_use.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/self/conftest.py` & `poetry-1.4.2/tests/console/commands/self/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/self/fixtures/poetry-1.0.5-darwin.tar.gz` & `poetry-1.4.2/tests/console/commands/self/fixtures/poetry-1.0.5-darwin.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/self/test_add_plugins.py` & `poetry-1.4.2/tests/console/commands/self/test_add_plugins.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/self/test_remove_plugins.py` & `poetry-1.4.2/tests/console/commands/self/test_remove_plugins.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/self/test_show_plugins.py` & `poetry-1.4.2/tests/console/commands/self/test_show_plugins.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/self/test_update.py` & `poetry-1.4.2/tests/console/commands/self/test_update.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/self/utils.py` & `poetry-1.4.2/tests/console/commands/self/utils.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/source/conftest.py` & `poetry-1.4.2/tests/console/commands/source/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/source/test_add.py` & `poetry-1.4.2/tests/console/commands/source/test_add.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/source/test_remove.py` & `poetry-1.4.2/tests/console/commands/source/test_remove.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/source/test_show.py` & `poetry-1.4.2/tests/console/commands/source/test_show.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/test_about.py` & `poetry-1.4.2/tests/console/commands/test_about.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/test_add.py` & `poetry-1.4.2/tests/console/commands/test_add.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/test_build.py` & `poetry-1.4.2/tests/console/commands/test_build.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/test_check.py` & `poetry-1.4.2/tests/console/commands/test_check.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/test_config.py` & `poetry-1.4.2/tests/console/commands/test_config.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/test_init.py` & `poetry-1.4.2/tests/console/commands/test_init.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/test_install.py` & `poetry-1.4.2/tests/console/commands/test_install.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/test_lock.py` & `poetry-1.4.2/tests/console/commands/test_lock.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/test_new.py` & `poetry-1.4.2/tests/console/commands/test_new.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/test_publish.py` & `poetry-1.4.2/tests/console/commands/test_publish.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/test_remove.py` & `poetry-1.4.2/tests/console/commands/test_remove.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/test_run.py` & `poetry-1.4.2/tests/console/commands/test_run.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/test_search.py` & `poetry-1.4.2/tests/console/commands/test_search.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/test_shell.py` & `poetry-1.4.2/tests/console/commands/test_shell.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/test_show.py` & `poetry-1.4.2/tests/console/commands/test_show.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/test_update.py` & `poetry-1.4.2/tests/console/commands/test_update.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/commands/test_version.py` & `poetry-1.4.2/tests/console/commands/test_version.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/conftest.py` & `poetry-1.4.2/tests/console/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/console/test_application.py` & `poetry-1.4.2/tests/console/test_application.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/build_system_requires_not_available/pyproject.toml` & `poetry-1.4.2/tests/fixtures/build_system_requires_not_available/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/complete.toml` & `poetry-1.4.2/tests/fixtures/complete.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/directory/project_with_transitive_directory_dependencies/setup.py` & `poetry-1.4.2/tests/fixtures/directory/project_with_transitive_directory_dependencies/setup.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl` & `poetry-1.4.2/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/distributions/demo-0.1.0.tar.gz` & `poetry-1.4.2/tests/fixtures/distributions/demo-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/distributions/demo-0.1.2-py2.py3-none-any.whl` & `poetry-1.4.2/tests/fixtures/distributions/demo-0.1.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/extended_project/pyproject.toml` & `poetry-1.4.2/tests/fixtures/extended_project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/extended_project_without_setup/pyproject.toml` & `poetry-1.4.2/tests/fixtures/extended_project_without_setup/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/extended_with_no_setup/build.py` & `poetry-1.4.2/tests/fixtures/extended_with_no_setup/build.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/extended_with_no_setup/extended/extended.c` & `poetry-1.4.2/tests/fixtures/extended_with_no_setup/extended/extended.c`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/extended_with_no_setup/pyproject.toml` & `poetry-1.4.2/tests/fixtures/extended_with_no_setup/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/git/github.com/demo/no-version/setup.py` & `poetry-1.4.2/tests/fixtures/git/github.com/demo/no-version/setup.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/old_lock/poetry.lock` & `poetry-1.4.2/tests/fixtures/old_lock/poetry.lock`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/outdated_lock/poetry.lock` & `poetry-1.4.2/tests/fixtures/outdated_lock/poetry.lock`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/project_with_git_dev_dependency/pyproject.toml` & `poetry-1.4.2/tests/fixtures/project_with_git_dev_dependency/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/project_with_local_dependencies/pyproject.toml` & `poetry-1.4.2/tests/fixtures/project_with_local_dependencies/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/sample_project/pyproject.toml` & `poetry-1.4.2/tests/fixtures/sample_project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/scripts/scripts/check_argv0.py` & `poetry-1.4.2/tests/fixtures/scripts/scripts/check_argv0.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl` & `poetry-1.4.2/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/simple_project/dist/simple_project-1.2.3.tar.gz` & `poetry-1.4.2/tests/fixtures/simple_project/dist/simple_project-1.2.3.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/simple_project/pyproject.toml` & `poetry-1.4.2/tests/fixtures/simple_project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/up_to_date_lock/poetry.lock` & `poetry-1.4.2/tests/fixtures/up_to_date_lock/poetry.lock`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/wheel_with_no_requires_dist/demo-0.1.0-py2.py3-none-any.whl` & `poetry-1.4.2/tests/fixtures/wheel_with_no_requires_dist/demo-0.1.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/with-include/LICENSE` & `poetry-1.4.2/tests/fixtures/with-include/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/with-include/pyproject.toml` & `poetry-1.4.2/tests/fixtures/with-include/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/with_default_source/pyproject.toml` & `poetry-1.4.2/tests/fixtures/with_default_source/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/with_local_config/pyproject.toml` & `poetry-1.4.2/tests/fixtures/with_local_config/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/fixtures/with_two_default_sources/pyproject.toml` & `poetry-1.4.2/tests/fixtures/with_two_default_sources/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/helpers.py` & `poetry-1.4.2/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/inspection/test_info.py` & `poetry-1.4.2/tests/inspection/test_info.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/fixtures/extras-with-dependencies.test` & `poetry-1.4.2/tests/installation/fixtures/extras-with-dependencies.test`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/fixtures/extras.test` & `poetry-1.4.2/tests/installation/fixtures/extras.test`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/fixtures/old-lock.test` & `poetry-1.4.2/tests/installation/fixtures/old-lock.test`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/fixtures/update-with-locked-extras.test` & `poetry-1.4.2/tests/installation/fixtures/update-with-locked-extras.test`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/fixtures/with-dependencies-extras.test` & `poetry-1.4.2/tests/installation/fixtures/with-dependencies-extras.test`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/fixtures/with-dependencies-nested-extras.test` & `poetry-1.4.2/tests/installation/fixtures/with-dependencies-nested-extras.test`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/fixtures/with-directory-dependency-poetry-transitive.test` & `poetry-1.4.2/tests/installation/fixtures/with-directory-dependency-poetry-transitive.test`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/fixtures/with-directory-dependency-poetry.test` & `poetry-1.4.2/tests/installation/fixtures/with-directory-dependency-poetry.test`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/fixtures/with-directory-dependency-setuptools.test` & `poetry-1.4.2/tests/installation/fixtures/with-directory-dependency-setuptools.test`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/fixtures/with-duplicate-dependencies-update.test` & `poetry-1.4.2/tests/installation/fixtures/with-duplicate-dependencies-update.test`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/fixtures/with-duplicate-dependencies.test` & `poetry-1.4.2/tests/installation/fixtures/with-duplicate-dependencies.test`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/fixtures/with-file-dependency-transitive.test` & `poetry-1.4.2/tests/installation/fixtures/with-file-dependency-transitive.test`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/fixtures/with-file-dependency.test` & `poetry-1.4.2/tests/installation/fixtures/with-file-dependency.test`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/fixtures/with-multiple-updates.test` & `poetry-1.4.2/tests/installation/fixtures/with-multiple-updates.test`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/fixtures/with-optional-dependencies.test` & `poetry-1.4.2/tests/installation/fixtures/with-optional-dependencies.test`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/fixtures/with-platform-dependencies.test` & `poetry-1.4.2/tests/installation/fixtures/with-platform-dependencies.test`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/fixtures/with-pypi-repository.test` & `poetry-1.4.2/tests/installation/fixtures/with-pypi-repository.test`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/fixtures/with-same-version-url-dependencies.test` & `poetry-1.4.2/tests/installation/fixtures/with-same-version-url-dependencies.test`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/fixtures/with-sub-dependencies.test` & `poetry-1.4.2/tests/installation/fixtures/with-sub-dependencies.test`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/fixtures/with-url-dependency.test` & `poetry-1.4.2/tests/installation/fixtures/with-url-dependency.test`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/fixtures/with-vcs-dependency-with-extras.test` & `poetry-1.4.2/tests/installation/fixtures/with-vcs-dependency-with-extras.test`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/fixtures/with-vcs-dependency-without-ref.test` & `poetry-1.4.2/tests/installation/fixtures/with-vcs-dependency-without-ref.test`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/test_chef.py` & `poetry-1.4.2/tests/installation/test_chef.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,17 @@
     )
 
     archives = chef.get_cached_archives_for_link(
         Link("https://files.python-poetry.org/demo-0.1.0.tar.gz")
     )
 
     assert archives
-    assert set(archives) == set(distributions.glob("demo-0.1.*"))
+    assert set(archives) == set(distributions.glob("*.whl")) | set(
+        distributions.glob("*.tar.gz")
+    )
 
 
 def test_get_cache_directory_for_link(config: Config, config_cache_dir: Path):
     chef = Chef(
         config,
         MockEnv(
             marker_env={"interpreter_name": "cpython", "interpreter_version": "3.8.3"}
```

### Comparing `poetry-1.4.1/tests/installation/test_chooser.py` & `poetry-1.4.2/tests/installation/test_chooser.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/test_executor.py` & `poetry-1.4.2/tests/installation/test_executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,30 +125,30 @@
     pool = RepositoryPool()
     pool.add_repository(MockRepository())
 
     return pool
 
 
 @pytest.fixture()
-def mock_file_downloads(http: type[httpretty.httpretty]) -> None:
+def mock_file_downloads(
+    http: type[httpretty.httpretty], fixture_dir: FixtureDirGetter
+) -> None:
     def callback(
         request: HTTPrettyRequest, uri: str, headers: dict[str, Any]
     ) -> list[int | dict[str, Any] | str]:
         name = Path(urlparse(uri).path).name
 
         fixture = Path(__file__).parent.parent.joinpath(
             "repositories/fixtures/pypi.org/dists/" + name
         )
 
         if not fixture.exists():
-            if name == "demo-0.1.0.tar.gz":
-                fixture = Path(__file__).parent.parent.joinpath(
-                    "fixtures/distributions/demo-0.1.0.tar.gz"
-                )
-            else:
+            fixture = fixture_dir("distributions") / name
+
+            if not fixture.exists():
                 fixture = Path(__file__).parent.parent.joinpath(
                     "fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl"
                 )
 
         return [200, headers, fixture.read_bytes()]
 
     http.register_uri(
@@ -338,14 +338,74 @@
         assert expected in error
         assert error.count("is yanked") == 1
     else:
         assert expected not in error
         assert error.count("yanked") == 0
 
 
+def test_execute_prints_warning_for_invalid_wheels(
+    config: Config,
+    pool: RepositoryPool,
+    io: BufferedIO,
+    tmp_dir: str,
+    mock_file_downloads: None,
+    env: MockEnv,
+):
+    config.merge({"cache-dir": tmp_dir})
+
+    executor = Executor(env, pool, config, io)
+
+    base_url = "https://files.pythonhosted.org/"
+    wheel1 = "demo_invalid_record-0.1.0-py2.py3-none-any.whl"
+    wheel2 = "demo_invalid_record2-0.1.0-py2.py3-none-any.whl"
+    return_code = executor.execute(
+        [
+            Install(
+                Package(
+                    "demo-invalid-record",
+                    "0.1.0",
+                    source_type="url",
+                    source_url=f"{base_url}/{wheel1}",
+                )
+            ),
+            Install(
+                Package(
+                    "demo-invalid-record2",
+                    "0.1.0",
+                    source_type="url",
+                    source_url=f"{base_url}/{wheel2}",
+                )
+            ),
+        ]
+    )
+
+    warning1 = f"""\
+<warning>Warning: Validation of the RECORD file of {wheel1} failed.\
+ Please report to the maintainers of that package so they can fix their build process.\
+ Details:
+In .*?{wheel1}, demo/__init__.py is not mentioned in RECORD
+In .*?{wheel1}, demo_invalid_record-0.1.0.dist-info/WHEEL is not mentioned in RECORD
+"""
+
+    warning2 = f"""\
+<warning>Warning: Validation of the RECORD file of {wheel2} failed.\
+ Please report to the maintainers of that package so they can fix their build process.\
+ Details:
+In .*?{wheel2}, hash / size of demo_invalid_record2-0.1.0.dist-info/METADATA didn't\
+ match RECORD
+"""
+
+    output = io.fetch_output()
+    error = io.fetch_error()
+    assert return_code == 0, f"\noutput: {output}\nerror: {error}\n"
+    assert re.match(f"{warning1}\n{warning2}", error) or re.match(
+        f"{warning2}\n{warning1}", error
+    ), error
+
+
 def test_execute_shows_skipped_operations_if_verbose(
     config: Config,
     pool: RepositoryPool,
     io: BufferedIO,
     config_cache_dir: Path,
     env: MockEnv,
 ):
```

### Comparing `poetry-1.4.1/tests/installation/test_installer.py` & `poetry-1.4.2/tests/installation/test_installer.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/test_installer_old.py` & `poetry-1.4.2/tests/installation/test_installer_old.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/test_pip_installer.py` & `poetry-1.4.2/tests/installation/test_pip_installer.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/installation/test_wheel_installer.py` & `poetry-1.4.2/tests/installation/test_wheel_installer.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/integration/test_utils_vcs_git.py` & `poetry-1.4.2/tests/integration/test_utils_vcs_git.py`

 * *Files 12% similar despite different names*

```diff
@@ -236,14 +236,38 @@
         )
 
     assert submodule_package_directory.exists()
     assert submodule_package_directory.joinpath("README.md").exists()
     assert len(list(submodule_package_directory.glob("*"))) > 1
 
 
+def test_git_clone_clones_submodules_with_relative_urls(source_url: str) -> None:
+    with Git.clone(url=source_url, branch="relative_submodule") as repo:
+        submodule_package_directory = (
+            Path(repo.path) / "submodules" / "relative-url-submodule"
+        )
+
+    assert submodule_package_directory.exists()
+    assert submodule_package_directory.joinpath("README.md").exists()
+    assert len(list(submodule_package_directory.glob("*"))) > 1
+
+
+def test_git_clone_clones_submodules_with_relative_urls_and_explicit_base(
+    source_url: str,
+) -> None:
+    with Git.clone(url=source_url, branch="relative_submodule") as repo:
+        submodule_package_directory = (
+            Path(repo.path) / "submodules" / "relative-url-submodule-with-base"
+        )
+
+    assert submodule_package_directory.exists()
+    assert submodule_package_directory.joinpath("README.md").exists()
+    assert len(list(submodule_package_directory.glob("*"))) > 1
+
+
 def test_system_git_fallback_on_http_401(
     mocker: MockerFixture,
     source_url: str,
 ) -> None:
     spy = mocker.spy(Git, "_clone_legacy")
     mocker.patch.object(Git, "_clone", side_effect=HTTPUnauthorized(None, None))
```

### Comparing `poetry-1.4.1/tests/json/test_schema_sources.py` & `poetry-1.4.2/tests/json/test_schema_sources.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/masonry/builders/test_editable_builder.py` & `poetry-1.4.2/tests/masonry/builders/test_editable_builder.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/mixology/helpers.py` & `poetry-1.4.2/tests/mixology/helpers.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/mixology/solutions/providers/test_python_requirement_solution_provider.py` & `poetry-1.4.2/tests/mixology/solutions/providers/test_python_requirement_solution_provider.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/mixology/solutions/solutions/test_python_requirement_solution.py` & `poetry-1.4.2/tests/mixology/solutions/solutions/test_python_requirement_solution.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/mixology/version_solver/conftest.py` & `poetry-1.4.2/tests/mixology/version_solver/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/mixology/version_solver/test_backtracking.py` & `poetry-1.4.2/tests/mixology/version_solver/test_backtracking.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/mixology/version_solver/test_basic_graph.py` & `poetry-1.4.2/tests/mixology/version_solver/test_basic_graph.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/mixology/version_solver/test_dependency_cache.py` & `poetry-1.4.2/tests/mixology/version_solver/test_dependency_cache.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/mixology/version_solver/test_python_constraint.py` & `poetry-1.4.2/tests/mixology/version_solver/test_python_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/mixology/version_solver/test_unsolvable.py` & `poetry-1.4.2/tests/mixology/version_solver/test_unsolvable.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/mixology/version_solver/test_with_lock.py` & `poetry-1.4.2/tests/mixology/version_solver/test_with_lock.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/packages/test_locker.py` & `poetry-1.4.2/tests/packages/test_locker.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/plugins/test_plugin_manager.py` & `poetry-1.4.2/tests/plugins/test_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/publishing/test_publisher.py` & `poetry-1.4.2/tests/publishing/test_publisher.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/publishing/test_uploader.py` & `poetry-1.4.2/tests/publishing/test_uploader.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/puzzle/conftest.py` & `poetry-1.4.2/tests/puzzle/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/puzzle/test_provider.py` & `poetry-1.4.2/tests/puzzle/test_provider.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/puzzle/test_solver.py` & `poetry-1.4.2/tests/puzzle/test_solver.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/puzzle/test_transaction.py` & `poetry-1.4.2/tests/puzzle/test_transaction.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/cleo-0.7.6.dist-info/METADATA` & `poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/cleo-0.7.6.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-2.3.4.dist-info/METADATA` & `poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-2.3.4.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-with-import-2.3.4.dist-info/METADATA` & `poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-with-import-2.3.4.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/foo-0.1.0-py3.8.egg` & `poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/foo-0.1.0-py3.8.egg`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/standard-1.2.3.dist-info/METADATA` & `poetry-1.4.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/standard-1.2.3.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/bender-2.0.5.dist-info/METADATA` & `poetry-1.4.2/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/bender-2.0.5.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/lib64-2.3.4.dist-info/METADATA` & `poetry-1.4.2/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/lib64-2.3.4.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/installed/src/bender/bender.egg-info/PKG-INFO` & `poetry-1.4.2/tests/repositories/fixtures/installed/src/bender/bender.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/installed/src/pendulum/pendulum.egg-info/PKG-INFO` & `poetry-1.4.2/tests/repositories/fixtures/installed/src/pendulum/pendulum.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/installed/vendor/py3.7/attrs-19.3.0.dist-info/METADATA` & `poetry-1.4.2/tests/repositories/fixtures/installed/vendor/py3.7/attrs-19.3.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/legacy/absolute.html` & `poetry-1.4.2/tests/repositories/fixtures/legacy/absolute.html`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/legacy/black.html` & `poetry-1.4.2/tests/repositories/fixtures/legacy/black.html`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/legacy/clikit.html` & `poetry-1.4.2/tests/repositories/fixtures/legacy/clikit.html`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/legacy/discord-py.html` & `poetry-1.4.2/tests/repositories/fixtures/legacy/discord-py.html`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/legacy/futures-partial-yank.html` & `poetry-1.4.2/tests/repositories/fixtures/legacy/futures-partial-yank.html`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/legacy/futures.html` & `poetry-1.4.2/tests/repositories/fixtures/legacy/futures.html`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/legacy/invalid-version.html` & `poetry-1.4.2/tests/repositories/fixtures/legacy/invalid-version.html`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/legacy/ipython.html` & `poetry-1.4.2/tests/repositories/fixtures/legacy/ipython.html`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/legacy/isort.html` & `poetry-1.4.2/tests/repositories/fixtures/legacy/isort.html`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/legacy/poetry-test-py2-py3-metadata-merge.html` & `poetry-1.4.2/tests/repositories/fixtures/legacy/poetry-test-py2-py3-metadata-merge.html`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/legacy/pytest.html` & `poetry-1.4.2/tests/repositories/fixtures/legacy/pytest.html`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/legacy/pyyaml.html` & `poetry-1.4.2/tests/repositories/fixtures/legacy/pyyaml.html`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/legacy/relative.html` & `poetry-1.4.2/tests/repositories/fixtures/legacy/relative.html`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/SQLAlchemy-1.2.12.tar.gz` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/SQLAlchemy-1.2.12.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/Twisted-18.9.0.tar.bz2` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/Twisted-18.9.0.tar.bz2`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/black-19.10b0-py36-none-any.whl` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/black-19.10b0-py36-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/black-21.11b0-py3-none-any.whl` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/black-21.11b0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/cleo-1.0.0a5-py3-none-any.whl` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/cleo-1.0.0a5-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/clikit-0.2.4-py2.py3-none-any.whl` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/clikit-0.2.4-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/discord.py-2.0.0-py3-none-any.whl` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/discord.py-2.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0-py2-none-any.whl` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0-py2-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0.tar.gz` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/importlib_metadata-1.7.0-py2.py3-none-any.whl` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/importlib_metadata-1.7.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py2-none-any.whl` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py2-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py3-none-any.whl` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0.tar.gz` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/ipython-7.5.0-py3-none-any.whl` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/ipython-7.5.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py2-none-any.whl` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py2-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py3-none-any.whl` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4.tar.gz` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0-py2.py3-none-any.whl` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0.tar.gz` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/pastel-0.1.0.tar.gz` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/pastel-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/poetry_core-1.5.0-py3-none-any.whl` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/poetry_core-1.5.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py2-none-any.whl` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py2-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py3-none-any.whl` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/pytest-3.5.0-py2.py3-none-any.whl` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/pytest-3.5.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/pytest-3.5.1-py2.py3-none-any.whl` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/pytest-3.5.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/python-language-server-0.21.2.tar.gz` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/python-language-server-0.21.2.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.2.tar.gz` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.2.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.3.tar.gz` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.3.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/dists/zipp-3.5.0-py3-none-any.whl` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/dists/zipp-3.5.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/attrs/17.4.0.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/attrs/17.4.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/attrs.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/attrs.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/black/19.10b0.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/black/19.10b0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/black/21.11b0.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/black/21.11b0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/black.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/black.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/cachecontrol/0.12.5.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/cachecontrol/0.12.5.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/cachecontrol.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/cachecontrol.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/cleo/1.0.0a5.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/cleo/1.0.0a5.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/clikit/0.2.4.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/clikit/0.2.4.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/clikit.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/clikit.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/colorama/0.3.9.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/colorama/0.3.9.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/colorama.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/colorama.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/discord-py/2.0.0.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/discord-py/2.0.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/funcsigs/1.0.2.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/funcsigs/1.0.2.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/funcsigs.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/funcsigs.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/hbmqtt/0.9.6.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/hbmqtt/0.9.6.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/hbmqtt.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/hbmqtt.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/importlib-metadata/1.7.0.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/importlib-metadata/1.7.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/importlib-metadata.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/importlib-metadata.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/ipython/4.1.0rc1.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/ipython/4.1.0rc1.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/isort/4.3.4.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/isort/4.3.4.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/isort.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/isort.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/jupyter/1.0.0.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/jupyter/1.0.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/jupyter.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/jupyter.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/lockfile/0.12.2.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/lockfile/0.12.2.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/lockfile.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/lockfile.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/more-itertools/4.1.0.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/more-itertools/4.1.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/more-itertools.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/more-itertools.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/pluggy/0.6.0.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/pluggy/0.6.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/poetry/0.12.4.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/poetry/0.12.4.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/poetry-core/1.5.0.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/poetry-core/1.5.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/poetry-core.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/poetry-core.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/poetry.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/poetry.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/py/1.5.3.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/py/1.5.3.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/py.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/py.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/pygame-music-grid.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/pygame-music-grid.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/pylev/1.3.0.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/pylev/1.3.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/pytest/3.5.0.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/pytest/3.5.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/pytest/3.5.1.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/pytest/3.5.1.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/pytest.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/pytest.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/pyyaml/3.13.0.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/pyyaml/3.13.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/pyyaml.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/pyyaml.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/requests/2.18.4.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/requests/2.18.4.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/requests.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/requests.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/setuptools/39.2.0.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/setuptools/39.2.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/setuptools.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/setuptools.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/six/1.11.0.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/six/1.11.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/six.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/six.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/sqlalchemy/1.2.12.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/sqlalchemy/1.2.12.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/toga.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/toga.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/tomlkit/0.5.3.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/tomlkit/0.5.3.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/tomlkit.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/tomlkit.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/trackpy/0.4.1.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/trackpy/0.4.1.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/trackpy.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/trackpy.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/twisted/18.9.0.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/twisted/18.9.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/zipp/3.5.0.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/zipp/3.5.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/json/zipp.json` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/json/zipp.json`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/pypi.org/search/search.html` & `poetry-1.4.2/tests/repositories/fixtures/pypi.org/search/search.html`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/fixtures/single-page/jax_releases.html` & `poetry-1.4.2/tests/repositories/fixtures/single-page/jax_releases.html`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/link_sources/test_base.py` & `poetry-1.4.2/tests/repositories/link_sources/test_base.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/link_sources/test_html.py` & `poetry-1.4.2/tests/repositories/link_sources/test_html.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/test_installed_repository.py` & `poetry-1.4.2/tests/repositories/test_installed_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/test_legacy_repository.py` & `poetry-1.4.2/tests/repositories/test_legacy_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/test_lockfile_repository.py` & `poetry-1.4.2/tests/repositories/test_lockfile_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/test_pypi_repository.py` & `poetry-1.4.2/tests/repositories/test_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/test_repository.py` & `poetry-1.4.2/tests/repositories/test_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/test_repository_pool.py` & `poetry-1.4.2/tests/repositories/test_repository_pool.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/repositories/test_single_page_repository.py` & `poetry-1.4.2/tests/repositories/test_single_page_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/test_factory.py` & `poetry-1.4.2/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/types.py` & `poetry-1.4.2/tests/types.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/utils/fixtures/pyproject.toml` & `poetry-1.4.2/tests/utils/fixtures/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/utils/fixtures/setups/ansible/setup.py` & `poetry-1.4.2/tests/utils/fixtures/setups/ansible/setup.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/utils/fixtures/setups/flask/setup.py` & `poetry-1.4.2/tests/utils/fixtures/setups/flask/setup.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/utils/fixtures/setups/pendulum/setup.py` & `poetry-1.4.2/tests/utils/fixtures/setups/pendulum/setup.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/utils/fixtures/setups/pyyaml/setup.py` & `poetry-1.4.2/tests/utils/fixtures/setups/pyyaml/setup.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/utils/fixtures/setups/requests/setup.py` & `poetry-1.4.2/tests/utils/fixtures/setups/requests/setup.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/utils/fixtures/setups/sqlalchemy/setup.py` & `poetry-1.4.2/tests/utils/fixtures/setups/sqlalchemy/setup.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/utils/test_authenticator.py` & `poetry-1.4.2/tests/utils/test_authenticator.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/utils/test_cache.py` & `poetry-1.4.2/tests/utils/test_cache.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/utils/test_dependency_specification.py` & `poetry-1.4.2/tests/utils/test_dependency_specification.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/utils/test_env.py` & `poetry-1.4.2/tests/utils/test_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import os
 import subprocess
 import sys
 
 from pathlib import Path
+from threading import Thread
 from typing import TYPE_CHECKING
 from typing import Any
 
 import pytest
 import tomlkit
 
 from poetry.core.constraints.version import Version
@@ -1005,14 +1006,39 @@
     with pytest.raises(EnvCommandError) as error:
         tmp_venv.run("python", "-")
     subprocess.check_output.assert_called_once()
     assert "some output" in str(error.value)
     assert "some error" in str(error.value)
 
 
+@pytest.mark.parametrize("out", ["sys.stdout", "sys.stderr"])
+def test_call_does_not_block_on_full_pipe(
+    tmp_path: Path, tmp_venv: VirtualEnv, out: str
+):
+    """see https://github.com/python-poetry/poetry/issues/7698"""
+    script = tmp_path / "script.py"
+    script.write_text(
+        f"""\
+import sys
+for i in range(10000):
+    print('just print a lot of text to fill the buffer', file={out})
+"""
+    )
+
+    def target(result: list[int]) -> None:
+        result.append(tmp_venv.run("python", str(script), call=True))
+
+    results = []
+    # use a separate thread, so that the test does not block in case of error
+    thread = Thread(target=target, args=(results,))
+    thread.start()
+    thread.join(1)  # must not block
+    assert results and results[0] == 0
+
+
 def test_run_python_script_called_process_error(
     tmp_dir: str, tmp_venv: VirtualEnv, mocker: MockerFixture
 ):
     mocker.patch(
         "subprocess.run",
         side_effect=subprocess.CalledProcessError(
             42, "some_command", "some output", "some error"
```

### Comparing `poetry-1.4.1/tests/utils/test_env_site.py` & `poetry-1.4.2/tests/utils/test_env_site.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/utils/test_extras.py` & `poetry-1.4.2/tests/utils/test_extras.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/utils/test_helpers.py` & `poetry-1.4.2/tests/utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/utils/test_password_manager.py` & `poetry-1.4.2/tests/utils/test_password_manager.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/utils/test_patterns.py` & `poetry-1.4.2/tests/utils/test_patterns.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/utils/test_pip.py` & `poetry-1.4.2/tests/utils/test_pip.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/utils/test_setup_reader.py` & `poetry-1.4.2/tests/utils/test_setup_reader.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/tests/utils/test_source.py` & `poetry-1.4.2/tests/utils/test_source.py`

 * *Files identical despite different names*

### Comparing `poetry-1.4.1/PKG-INFO` & `poetry-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry
-Version: 1.4.1
+Version: 1.4.2
 Summary: Python dependency management and packaging made easy.
 Home-page: https://python-poetry.org/
 License: MIT
 Keywords: packaging,dependency,poetry
 Author: Sébastien Eustace
 Author-email: sebastien@eustace.io
 Maintainer: Arun Babu Neelicattu
```

