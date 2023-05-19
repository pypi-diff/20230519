# Comparing `tmp/hippogym-2.0.0a1.tar.gz` & `tmp/hippogym-2.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hippogym-2.0.0a1.tar", last modified: Mon Apr 24 11:33:40 2023, max compression
+gzip compressed data, was "hippogym-2.0.0a2.tar", last modified: Fri May 19 17:35:49 2023, max compression
```

## Comparing `hippogym-2.0.0a1.tar` & `hippogym-2.0.0a2.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.832371 hippogym-2.0.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.812371 hippogym-2.0.0a1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.816371 hippogym-2.0.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/.github/workflows/python-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/.github/workflows/python-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/.github/workflows/python_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/.github/workflows/python_tests_end_to_end.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-24 11:33:40.832371 hippogym-2.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.816371 hippogym-2.0.0a1/StepFiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/StepFiles/exampleConsent.html
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/StepFiles/exampleQuiz.html
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/StepFiles/exampleSurvey.html
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/StepFiles/exampleThank.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.816371 hippogym-2.0.0a1/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    19099 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/assets/class_diagram.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.824371 hippogym-2.0.0a1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    14736 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/docs/UML_class_diagram.uxf
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/docs/backend_success_example.png
--rw-r--r--   0 runner    (1001) docker     (123)  6002564 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/docs/lunar_human_demo.gif
--rw-r--r--   0 runner    (1001) docker     (123)  1863460 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/docs/minigrid_human_demo.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.824371 hippogym-2.0.0a1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/examples/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/examples/hcraft_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/examples/lunar_lander.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/examples/minigrid_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.828371 hippogym-2.0.0a1/img/
--rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/img/icon_dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/img/icon_light.png
--rw-r--r--   0 runner    (1001) docker     (123)    46665 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/img/logo_horizontal.png
--rw-r--r--   0 runner    (1001) docker     (123)    44138 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/img/logo_vertical.png
--rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/img/words_horizontal.png
--rw-r--r--   0 runner    (1001) docker     (123)    21835 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/img/words_vertical.png
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/requirements-examples.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 11:33:40.832371 hippogym-2.0.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.812371 hippogym-2.0.0a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.828371 hippogym-2.0.0a1/src/hippogym/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/bucketer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/communicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/hippogym.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.828371 hippogym-2.0.0a1/src/hippogym/trialsteps/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/trialsteps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/trialsteps/gymstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/trialsteps/trialstep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.828371 hippogym-2.0.0a1/src/hippogym/ui_elements/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/ui_elements/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.828371 hippogym-2.0.0a1/src/hippogym/ui_elements/building_blocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/ui_elements/building_blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/ui_elements/building_blocks/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/ui_elements/building_blocks/slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/ui_elements/control_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/ui_elements/game_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/ui_elements/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/ui_elements/info_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/ui_elements/text_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/src/hippogym/ui_elements/ui_element.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.828371 hippogym-2.0.0a1/src/hippogym.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-24 11:33:40.000000 hippogym-2.0.0a1/src/hippogym.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-24 11:33:40.000000 hippogym-2.0.0a1/src/hippogym.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 11:33:40.000000 hippogym-2.0.0a1/src/hippogym.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-24 11:33:40.000000 hippogym-2.0.0a1/src/hippogym.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-24 11:33:40.000000 hippogym-2.0.0a1/src/hippogym.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 11:33:40.000000 hippogym-2.0.0a1/src/hippogym.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       60 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/start.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.832371 hippogym-2.0.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.832371 hippogym-2.0.0a1/tests/end_to_end/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/end_to_end/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/end_to_end/custom_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/end_to_end/test_crafting.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/end_to_end/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/end_to_end/test_minigrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/fakes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.832371 hippogym-2.0.0a1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/unit/test_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/unit/test_events_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/unit/test_hippogym.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:40.832371 hippogym-2.0.0a1/tests/unit/ui_elements/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/unit/ui_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/unit/ui_elements/test_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/unit/ui_elements/test_slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-24 11:33:17.000000 hippogym-2.0.0a1/tests/unit/ui_elements/test_ui_element.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:49.969657 hippogym-2.0.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:49.937657 hippogym-2.0.0a2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:49.941657 hippogym-2.0.0a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/.github/workflows/python-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/.github/workflows/python-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/.github/workflows/python_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/.github/workflows/python_tests_end_to_end.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-19 17:35:49.969657 hippogym-2.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:49.945657 hippogym-2.0.0a2/StepFiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/StepFiles/exampleConsent.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/StepFiles/exampleQuiz.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/StepFiles/exampleSurvey.html
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/StepFiles/exampleThank.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:49.945657 hippogym-2.0.0a2/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    19099 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/assets/class_diagram.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:49.953657 hippogym-2.0.0a2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    14736 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/docs/UML_class_diagram.uxf
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/docs/backend_success_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)  6002564 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/docs/lunar_human_demo.gif
+-rw-r--r--   0 runner    (1001) docker     (123)  1863460 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/docs/minigrid_human_demo.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:49.957657 hippogym-2.0.0a2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/examples/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/examples/hcraft_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/examples/lunar_lander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/examples/minigrid_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:49.957657 hippogym-2.0.0a2/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/img/icon_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/img/icon_light.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46665 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/img/logo_horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44138 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/img/logo_vertical.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/img/words_horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21835 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/img/words_vertical.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/requirements-examples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 17:35:49.969657 hippogym-2.0.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:49.937657 hippogym-2.0.0a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:49.961657 hippogym-2.0.0a2/src/hippogym/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/src/hippogym/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/src/hippogym/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/src/hippogym/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/src/hippogym/bucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/src/hippogym/communicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/src/hippogym/event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/src/hippogym/hippogym.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/src/hippogym/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/src/hippogym/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/src/hippogym/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/src/hippogym/trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:49.965657 hippogym-2.0.0a2/src/hippogym/trialsteps/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/src/hippogym/trialsteps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/src/hippogym/trialsteps/gymstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/src/hippogym/trialsteps/trialstep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:49.965657 hippogym-2.0.0a2/src/hippogym/ui_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/src/hippogym/ui_elements/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:49.965657 hippogym-2.0.0a2/src/hippogym/ui_elements/building_blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/src/hippogym/ui_elements/building_blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/src/hippogym/ui_elements/building_blocks/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/src/hippogym/ui_elements/building_blocks/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/src/hippogym/ui_elements/control_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/src/hippogym/ui_elements/game_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/src/hippogym/ui_elements/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/src/hippogym/ui_elements/info_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/src/hippogym/ui_elements/text_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/src/hippogym/ui_elements/ui_element.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:49.965657 hippogym-2.0.0a2/src/hippogym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-19 17:35:49.000000 hippogym-2.0.0a2/src/hippogym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-19 17:35:49.000000 hippogym-2.0.0a2/src/hippogym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 17:35:49.000000 hippogym-2.0.0a2/src/hippogym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-19 17:35:49.000000 hippogym-2.0.0a2/src/hippogym.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-19 17:35:49.000000 hippogym-2.0.0a2/src/hippogym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-19 17:35:49.000000 hippogym-2.0.0a2/src/hippogym.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       58 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/start.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:49.965657 hippogym-2.0.0a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:49.969657 hippogym-2.0.0a2/tests/end_to_end/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/tests/end_to_end/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/tests/end_to_end/custom_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/tests/end_to_end/test_crafting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/tests/end_to_end/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/tests/end_to_end/test_minigrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/tests/fakes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:49.969657 hippogym-2.0.0a2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/tests/unit/test_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/tests/unit/test_events_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/tests/unit/test_hippogym.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:49.969657 hippogym-2.0.0a2/tests/unit/ui_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/tests/unit/ui_elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/tests/unit/ui_elements/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/tests/unit/ui_elements/test_slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-19 17:35:27.000000 hippogym-2.0.0a2/tests/unit/ui_elements/test_ui_element.py
```

### Comparing `hippogym-2.0.0a1/.github/workflows/python-coverage.yml` & `hippogym-2.0.0a2/.github/workflows/python-coverage.yml`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/.github/workflows/python-pypi.yml` & `hippogym-2.0.0a2/.github/workflows/python-pypi.yml`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/.github/workflows/python_tests.yml` & `hippogym-2.0.0a2/.github/workflows/python_tests.yml`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/.github/workflows/python_tests_end_to_end.yml` & `hippogym-2.0.0a2/.github/workflows/python_tests_end_to_end.yml`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/.gitignore` & `hippogym-2.0.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/LICENSE` & `hippogym-2.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/PKG-INFO` & `hippogym-2.0.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hippogym
-Version: 2.0.0a1
+Version: 2.0.0a2
 Author-email: Nick Nissen <nnissen@ualberta.ca>, Mathïs Fédérico <mathfederico@gmail.com>
 License: Apache-2.0
 Project-URL: Home-page, https://hippogym.irll.net
 Project-URL: Source, https://github.com/IRLL/HIPPO_Gym
 Project-URL: Documentation, https://hippogym.irll.net/
 Keywords: gym,human,loop,reinforcement,learning
 Requires-Python: >=3.8
```

### Comparing `hippogym-2.0.0a1/README.md` & `hippogym-2.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/StepFiles/exampleConsent.html` & `hippogym-2.0.0a2/StepFiles/exampleConsent.html`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/StepFiles/exampleQuiz.html` & `hippogym-2.0.0a2/StepFiles/exampleQuiz.html`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/StepFiles/exampleSurvey.html` & `hippogym-2.0.0a2/StepFiles/exampleSurvey.html`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/assets/class_diagram.pdf` & `hippogym-2.0.0a2/assets/class_diagram.pdf`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/config.yml` & `hippogym-2.0.0a2/config.yml`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/docs/UML_class_diagram.uxf` & `hippogym-2.0.0a2/docs/UML_class_diagram.uxf`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/docs/backend_success_example.png` & `hippogym-2.0.0a2/docs/backend_success_example.png`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/docs/lunar_human_demo.gif` & `hippogym-2.0.0a2/docs/lunar_human_demo.gif`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/docs/minigrid_human_demo.gif` & `hippogym-2.0.0a2/docs/minigrid_human_demo.gif`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/examples/grid.py` & `hippogym-2.0.0a2/examples/grid.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/examples/hcraft_example.py` & `hippogym-2.0.0a2/examples/hcraft_example.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/examples/lunar_lander.py` & `hippogym-2.0.0a2/examples/lunar_lander.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         super().reset()
 
 
 class LunarLanderV2Step(GymStep):
     def __init__(self, agent, experiment_name: str):
         self.info_panel = InfoPanel(
             text="Use keyboard to play the game",
-            items=["s = down", "a = left", "d = right"],
+            items=[u"\u2193"" = down", u"\u2190"" = left", u"\u2192" " = right"],
         )
         self.control_panel = ControlPanel(buttons=standard_controls)
         self.recorder = JsonRecorder(
             records_path="records", experiment_name=experiment_name
         )
         self.score = 0
         super().__init__(
```

### Comparing `hippogym-2.0.0a1/examples/minigrid_example.py` & `hippogym-2.0.0a2/examples/minigrid_example.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import gymnasium as gym
 from minigrid.minigrid_env import MiniGridEnv
 from minigrid.core.actions import Actions
 
 from hippogym import HippoGym, HumanAgent
 from hippogym.ui_elements import InfoPanel, ControlPanel, Button
 from hippogym.trialsteps import GymStep
-
+from hippogym.recorder import JsonRecorder
 
 logging.basicConfig(level=logging.DEBUG)
 LOGGER = logging.getLogger(__name__)
 
 
 class HumanValue(Enum):
     LEFT = "left"
@@ -30,16 +30,25 @@
     PICKUP = "pickup"
     DROP = "drop"
     END = "end"
 
 
 class MiniGridStep(GymStep):
     def __init__(self, agent):
-        self.info_panel = InfoPanel()
-
+        self.info_panel = InfoPanel(text="Use keyboard to play the game",
+                                    items = ["ArrowRight = Right,"+
+                                            "ArrowLeft = Left",
+                                            "ArrowUp = Up, "+
+                                            "Space = Toggle",
+                                            "c = Pickup, "+
+                                            "v = Drop",
+                                            "Enter = End"])
+        self.recorder = JsonRecorder(
+                    records_path="records", experiment_name="minigrid_human"
+                )
         buttons_params = {
             HumanValue.LEFT: {"icon": "FaArrowLeft"},
             HumanValue.RIGHT: {"icon": "FaArrowRight"},
             HumanValue.UP: {"icon": "FaArrowUp"},
             HumanValue.TOGGLE: {"icon": "IoToggle"},
             HumanValue.PICKUP: {"icon": "GiCardPickup"},
             HumanValue.DROP: {"icon": "GiDropWeapon"},
@@ -68,30 +77,41 @@
         observation,
         action,
         new_observation,
         reward: float,
         done: bool,
         info: dict,
     ) -> None:
-        if done:
-            self.info_panel.update(key_value={"Score": reward})
-            self.score = 0
-            return
+
 
         observation_msg = f"Step={self.env.step_count}, Reward={reward}"
         observation_msg = f"[{observation_msg}]"
         self.score += reward
         self.info_panel.update(
             key_value={
                 "Score": self.score,
                 "Reward": reward,
                 "Observation": observation_msg,
             },
         )
 
+
+        if done:
+            self.info_panel.update(key_value={"Score": reward})
+            self.recorder.record(
+                data = {
+                "episode": episode,
+                "steps": self.env.step_count,
+                "reward" : reward,
+            },
+                user_id=self.user_id,
+            )
+            self.score = 0
+            return
+
     def send_render(self):
         rgb_frame = self.env.get_frame(tile_size=64, agent_pov=True)
         render = self.render_window.convert_numpy_array_to_base64(rgb_frame)
         self.render_window.update(image=render)
 
 
 def build_experiment() -> HippoGym:
```

### Comparing `hippogym-2.0.0a1/img/icon_dark.png` & `hippogym-2.0.0a2/img/icon_dark.png`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/img/icon_light.png` & `hippogym-2.0.0a2/img/icon_light.png`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/img/logo_horizontal.png` & `hippogym-2.0.0a2/img/logo_horizontal.png`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/img/logo_vertical.png` & `hippogym-2.0.0a2/img/logo_vertical.png`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/img/words_horizontal.png` & `hippogym-2.0.0a2/img/words_horizontal.png`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/img/words_vertical.png` & `hippogym-2.0.0a2/img/words_vertical.png`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/pyproject.toml` & `hippogym-2.0.0a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/src/hippogym/agent.py` & `hippogym-2.0.0a2/src/hippogym/agent.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/src/hippogym/bucketer.py` & `hippogym-2.0.0a2/src/hippogym/bucketer.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/src/hippogym/communicator.py` & `hippogym-2.0.0a2/src/hippogym/communicator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import json
 import ssl
 from logging import getLogger
 from multiprocessing import Queue
 from typing import TYPE_CHECKING, Callable, Optional, Tuple, Union
-
+import os
 from websockets.server import WebSocketServerProtocol, serve
 
 if TYPE_CHECKING:
     from hippogym.hippogym import HippoGym
 
 
 LOGGER = getLogger(__name__)
@@ -146,23 +146,19 @@
             event_handler (EventHandler): Handler to transcribe messages into HippoGym events.
         """
         while out_q.empty():
             await asyncio.sleep(0.01)
         return out_q.get()
 
 
-async def start_non_ssl_server(handler: Callable, host: str, port: int) -> None:
-    """Start a non-ssl WebSocket server.
 
-    Args:
-        handler (Callable): Function to serve on the websocket.
-        host (str): Host of the websocket server.
-        port (int): Port of the websocket server.
-    """
-    async with serve(handler, host, port) as websocket:
+
+async def start_non_ssl_server(handler: Callable, host: str, port: int) -> None:
+    host = os.environ.get('HIPPOGYM_HOST', host)
+    async with serve(handler, host=host, port='5000') as websocket:
         LOGGER.info("Non-SSL websocket started at %s:%i", host, port)
         await websocket.serve_forever()
 
 
 class SSLCertificate:
     certfile: str = "fullchain.pem"
     privkey: str = "privkey.pem"
```

### Comparing `hippogym-2.0.0a1/src/hippogym/event_handler.py` & `hippogym-2.0.0a2/src/hippogym/event_handler.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/src/hippogym/hippogym.py` & `hippogym-2.0.0a2/src/hippogym/hippogym.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/src/hippogym/log.py` & `hippogym-2.0.0a2/src/hippogym/log.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/src/hippogym/message_handler.py` & `hippogym-2.0.0a2/src/hippogym/message_handler.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/src/hippogym/trial.py` & `hippogym-2.0.0a2/src/hippogym/trial.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/src/hippogym/trialsteps/gymstep.py` & `hippogym-2.0.0a2/src/hippogym/trialsteps/gymstep.py`

 * *Files 18% similar despite different names*

```diff
@@ -36,15 +36,18 @@
         )
         if ui_elements is None:
             ui_elements = []
         if self.render_window not in ui_elements:
             ui_elements.append(self.render_window)
         super().__init__(ui_elements)
         if isinstance(env, str):
-            env = gym.make(env, **kwargs)
+            if "LunarLander" in str(self):
+                env = gym.make(env, render_mode="rgb_array", **kwargs)
+            else:
+                env = gym.make(env, **kwargs)
         self.env = env
         self.agent = agent
         self.agent.set_spaces(self.env.observation_space, self.env.action_space)
 
         self.stop = False
         self.run_from_start = run_from_start
         self.running = self.run_from_start
@@ -140,14 +143,17 @@
         if len(reset_data) == 2 and isinstance(reset_data[1], dict):
             return reset_data
         observation = reset_data
         info = {}
         return observation, info
 
     def send_render(self):
-        rgb_array = self.env.render(mode="rgb_array")
+        if "LunarLander" in str(self):
+            rgb_array = self.env.render()
+        else:
+            rgb_array = self.env.render(mode="rgb_array")
         try:
             rgb_array = np.array(rgb_array)
         except:
             raise TypeError("Env render should output a numpy array.")
         render = self.render_window.convert_numpy_array_to_base64(rgb_array)
         self.render_window.update(image=render)
```

### Comparing `hippogym-2.0.0a1/src/hippogym/trialsteps/trialstep.py` & `hippogym-2.0.0a2/src/hippogym/trialsteps/trialstep.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/src/hippogym/ui_elements/__init__.py` & `hippogym-2.0.0a2/src/hippogym/ui_elements/__init__.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/src/hippogym/ui_elements/building_blocks/button.py` & `hippogym-2.0.0a2/src/hippogym/ui_elements/building_blocks/button.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/src/hippogym/ui_elements/building_blocks/slider.py` & `hippogym-2.0.0a2/src/hippogym/ui_elements/building_blocks/slider.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/src/hippogym/ui_elements/control_panel.py` & `hippogym-2.0.0a2/src/hippogym/ui_elements/control_panel.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/src/hippogym/ui_elements/game_window.py` & `hippogym-2.0.0a2/src/hippogym/ui_elements/game_window.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/src/hippogym/ui_elements/grid.py` & `hippogym-2.0.0a2/src/hippogym/ui_elements/grid.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/src/hippogym/ui_elements/info_panel.py` & `hippogym-2.0.0a2/src/hippogym/ui_elements/info_panel.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/src/hippogym/ui_elements/text_box.py` & `hippogym-2.0.0a2/src/hippogym/ui_elements/text_box.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/src/hippogym/ui_elements/ui_element.py` & `hippogym-2.0.0a2/src/hippogym/ui_elements/ui_element.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/src/hippogym.egg-info/PKG-INFO` & `hippogym-2.0.0a2/src/hippogym.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hippogym
-Version: 2.0.0a1
+Version: 2.0.0a2
 Author-email: Nick Nissen <nnissen@ualberta.ca>, Mathïs Fédérico <mathfederico@gmail.com>
 License: Apache-2.0
 Project-URL: Home-page, https://hippogym.irll.net
 Project-URL: Source, https://github.com/IRLL/HIPPO_Gym
 Project-URL: Documentation, https://hippogym.irll.net/
 Keywords: gym,human,loop,reinforcement,learning
 Requires-Python: >=3.8
```

### Comparing `hippogym-2.0.0a1/src/hippogym.egg-info/SOURCES.txt` & `hippogym-2.0.0a2/src/hippogym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/tests/end_to_end/custom_checks.py` & `hippogym-2.0.0a2/tests/end_to_end/custom_checks.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/tests/fakes.py` & `hippogym-2.0.0a2/tests/fakes.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/tests/unit/test_event_handler.py` & `hippogym-2.0.0a2/tests/unit/test_event_handler.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/tests/unit/test_events_dispatch.py` & `hippogym-2.0.0a2/tests/unit/test_events_dispatch.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/tests/unit/test_hippogym.py` & `hippogym-2.0.0a2/tests/unit/test_hippogym.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/tests/unit/ui_elements/test_button.py` & `hippogym-2.0.0a2/tests/unit/ui_elements/test_button.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/tests/unit/ui_elements/test_slider.py` & `hippogym-2.0.0a2/tests/unit/ui_elements/test_slider.py`

 * *Files identical despite different names*

### Comparing `hippogym-2.0.0a1/tests/unit/ui_elements/test_ui_element.py` & `hippogym-2.0.0a2/tests/unit/ui_elements/test_ui_element.py`

 * *Files identical despite different names*

