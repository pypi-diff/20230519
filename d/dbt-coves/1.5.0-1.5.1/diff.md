# Comparing `tmp/dbt_coves-1.5.0.tar.gz` & `tmp/dbt_coves-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_coves-1.5.0.tar", max compression
+gzip compressed data, was "dbt_coves-1.5.1.tar", max compression
```

## Comparing `dbt_coves-1.5.0.tar` & `dbt_coves-1.5.1.tar`

### file list

```diff
@@ -1,58 +1,59 @@
--rw-r--r--   0        0        0    11357 2022-11-12 20:16:42.866709 dbt_coves-1.5.0/LICENSE
--rw-r--r--   0        0        0    21746 2023-05-02 13:59:26.100559 dbt_coves-1.5.0/README.md
--rw-r--r--   0        0        0       22 2023-05-18 12:04:27.911193 dbt_coves-1.5.0/dbt_coves/__init__.py
--rw-r--r--   0        0        0        0 2022-11-12 20:16:42.867324 dbt_coves-1.5.0/dbt_coves/config/__init__.py
--rw-r--r--   0        0        0     9689 2023-04-25 20:50:24.122865 dbt_coves-1.5.0/dbt_coves/config/config.py
--rw-r--r--   0        0        0        0 2022-11-12 20:16:42.867500 dbt_coves-1.5.0/dbt_coves/core/__init__.py
--rw-r--r--   0        0        0      650 2022-11-12 20:16:42.867579 dbt_coves-1.5.0/dbt_coves/core/exceptions.py
--rw-r--r--   0        0        0     7398 2023-05-18 12:03:26.474660 dbt_coves-1.5.0/dbt_coves/core/main.py
--rw-r--r--   0        0        0        0 2022-11-12 20:16:42.867724 dbt_coves-1.5.0/dbt_coves/tasks/__init__.py
--rw-r--r--   0        0        0     3008 2023-05-18 12:03:26.475205 dbt_coves-1.5.0/dbt_coves/tasks/base.py
--rw-r--r--   0        0        0     4994 2023-05-02 13:59:26.103829 dbt_coves-1.5.0/dbt_coves/tasks/dbt/main.py
--rw-r--r--   0        0        0        0 2022-11-12 20:16:42.867965 dbt_coves-1.5.0/dbt_coves/tasks/extract/__init__.py
--rw-r--r--   0        0        0    12303 2023-05-15 17:37:04.477439 dbt_coves-1.5.0/dbt_coves/tasks/extract/airbyte.py
--rw-r--r--   0        0        0      475 2023-03-23 11:02:15.327281 dbt_coves-1.5.0/dbt_coves/tasks/extract/base.py
--rw-r--r--   0        0        0     4512 2023-03-23 11:02:15.327681 dbt_coves-1.5.0/dbt_coves/tasks/extract/fivetran.py
--rw-r--r--   0        0        0      963 2023-03-23 11:02:15.328185 dbt_coves-1.5.0/dbt_coves/tasks/extract/main.py
--rw-r--r--   0        0        0        0 2022-11-12 20:16:42.868244 dbt_coves-1.5.0/dbt_coves/tasks/generate/__init__.py
--rw-r--r--   0        0        0    18472 2023-05-16 15:07:22.657626 dbt_coves-1.5.0/dbt_coves/tasks/generate/base.py
--rw-r--r--   0        0        0     1520 2023-05-16 11:48:11.708991 dbt_coves-1.5.0/dbt_coves/tasks/generate/main.py
--rw-r--r--   0        0        0    10562 2023-03-23 11:02:15.329609 dbt_coves-1.5.0/dbt_coves/tasks/generate/metadata.py
--rw-r--r--   0        0        0     8880 2023-03-30 13:55:57.611879 dbt_coves-1.5.0/dbt_coves/tasks/generate/properties.py
--rw-r--r--   0        0        0    13955 2023-05-18 12:03:26.475513 dbt_coves-1.5.0/dbt_coves/tasks/generate/sources.py
--rw-r--r--   0        0        0     2653 2023-03-23 11:02:15.330706 dbt_coves-1.5.0/dbt_coves/tasks/generate/templates.py
--rw-r--r--   0        0        0        0 2022-11-12 20:16:42.868885 dbt_coves-1.5.0/dbt_coves/tasks/load/__init__.py
--rw-r--r--   0        0        0    25682 2023-05-15 17:37:04.477626 dbt_coves-1.5.0/dbt_coves/tasks/load/airbyte.py
--rw-r--r--   0        0        0     2259 2023-05-05 11:02:21.127260 dbt_coves-1.5.0/dbt_coves/tasks/load/base.py
--rw-r--r--   0        0        0    18390 2023-05-15 17:37:04.478119 dbt_coves-1.5.0/dbt_coves/tasks/load/fivetran.py
--rw-r--r--   0        0        0      946 2023-03-23 11:02:15.332754 dbt_coves-1.5.0/dbt_coves/tasks/load/main.py
--rw-r--r--   0        0        0        0 2022-11-12 20:16:42.869156 dbt_coves-1.5.0/dbt_coves/tasks/setup/__init__.py
--rw-r--r--   0        0        0     1744 2023-03-23 11:02:15.333279 dbt_coves-1.5.0/dbt_coves/tasks/setup/all.py
--rw-r--r--   0        0        0     4294 2023-05-18 12:03:26.475924 dbt_coves-1.5.0/dbt_coves/tasks/setup/dbt.py
--rw-r--r--   0        0        0     6689 2023-03-23 11:02:15.334243 dbt_coves-1.5.0/dbt_coves/tasks/setup/git.py
--rw-r--r--   0        0        0     1329 2023-05-08 19:28:33.430793 dbt_coves-1.5.0/dbt_coves/tasks/setup/main.py
--rw-r--r--   0        0        0     1615 2023-05-08 19:28:33.431036 dbt_coves-1.5.0/dbt_coves/tasks/setup/pre_commit.py
--rw-r--r--   0        0        0    10142 2023-03-23 11:02:15.335712 dbt_coves-1.5.0/dbt_coves/tasks/setup/ssh.py
--rw-r--r--   0        0        0      845 2023-05-08 19:28:33.431214 dbt_coves-1.5.0/dbt_coves/tasks/setup/templates/pre_commit/copier.yml
--rw-r--r--   0        0        0     2110 2023-05-08 19:28:33.431340 dbt_coves-1.5.0/dbt_coves/tasks/setup/templates/pre_commit/{% if use_sqlfluff or use_yamllint or use_dbt_checkpoint %}pre-commit-config.yaml{% endif %}.jinja
--rw-r--r--   0        0        0       75 2023-05-08 19:28:33.431660 dbt_coves-1.5.0/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluffignore{% endif %}
--rw-r--r--   0        0        0     2743 2023-05-08 19:28:33.431853 dbt_coves-1.5.0/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluff{% endif %}.jinja
--rw-r--r--   0        0        0      668 2023-05-08 19:28:33.432263 dbt_coves-1.5.0/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_yamllint %}.yamllint{% endif %}
--rw-r--r--   0        0        0      102 2023-05-08 19:28:33.432386 dbt_coves-1.5.0/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{{ _copier_conf.answers_file }}-precommit.yaml.jinja
--rw-r--r--   0        0        0     1371 2023-05-08 19:28:33.432813 dbt_coves-1.5.0/dbt_coves/tasks/setup/utils.py
--rw-r--r--   0        0        0      255 2023-03-23 11:02:15.337399 dbt_coves-1.5.0/dbt_coves/templates/model_props.yml
--rw-r--r--   0        0        0      214 2023-03-23 11:02:15.337740 dbt_coves-1.5.0/dbt_coves/templates/source_props.yml
--rw-r--r--   0        0        0     1201 2023-03-23 11:02:15.338064 dbt_coves-1.5.0/dbt_coves/templates/staging_model.sql
--rw-r--r--   0        0        0      495 2023-03-23 11:02:15.338292 dbt_coves-1.5.0/dbt_coves/templates/staging_model_props.yml
--rw-r--r--   0        0        0        0 2022-11-12 20:16:42.870019 dbt_coves-1.5.0/dbt_coves/ui/__init__.py
--rw-r--r--   0        0        0     1202 2022-11-12 20:16:42.870090 dbt_coves-1.5.0/dbt_coves/ui/traceback.py
--rw-r--r--   0        0        0        0 2022-11-12 20:16:42.870149 dbt_coves-1.5.0/dbt_coves/utils/__init__.py
--rw-r--r--   0        0        0    11270 2023-05-15 17:37:04.478455 dbt_coves-1.5.0/dbt_coves/utils/api_caller.py
--rw-r--r--   0        0        0    14725 2023-05-18 12:03:26.476318 dbt_coves-1.5.0/dbt_coves/utils/flags.py
--rw-r--r--   0        0        0     1132 2023-03-23 11:02:15.340252 dbt_coves-1.5.0/dbt_coves/utils/jinja.py
--rw-r--r--   0        0        0      785 2023-03-23 11:02:15.340489 dbt_coves-1.5.0/dbt_coves/utils/log.py
--rw-r--r--   0        0        0      791 2023-03-23 11:02:15.341162 dbt_coves-1.5.0/dbt_coves/utils/shell.py
--rw-r--r--   0        0        0     1010 2023-03-23 11:02:15.341786 dbt_coves-1.5.0/dbt_coves/utils/yaml.py
--rw-r--r--   0        0        0     3573 2023-05-18 12:04:23.598551 dbt_coves-1.5.0/pyproject.toml
--rw-r--r--   0        0        0    24184 1970-01-01 00:00:00.000000 dbt_coves-1.5.0/setup.py
--rw-r--r--   0        0        0    23804 1970-01-01 00:00:00.000000 dbt_coves-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/LICENSE
+-rw-r--r--   0        0        0    21746 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/README.md
+-rw-r--r--   0        0        0       22 2023-05-19 17:40:19.080273 dbt_coves-1.5.1/dbt_coves/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/config/__init__.py
+-rw-r--r--   0        0        0     9689 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/config/config.py
+-rw-r--r--   0        0        0        0 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/core/__init__.py
+-rw-r--r--   0        0        0      650 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/core/exceptions.py
+-rw-r--r--   0        0        0     8193 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/core/main.py
+-rw-r--r--   0        0        0        0 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/__init__.py
+-rw-r--r--   0        0        0     3008 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/base.py
+-rw-r--r--   0        0        0     5056 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/dbt/main.py
+-rw-r--r--   0        0        0        0 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/extract/__init__.py
+-rw-r--r--   0        0        0    12365 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/extract/airbyte.py
+-rw-r--r--   0        0        0      475 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/extract/base.py
+-rw-r--r--   0        0        0     4574 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/extract/fivetran.py
+-rw-r--r--   0        0        0      963 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/extract/main.py
+-rw-r--r--   0        0        0        0 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/generate/__init__.py
+-rw-r--r--   0        0        0    18472 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/generate/base.py
+-rw-r--r--   0        0        0     1520 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/generate/main.py
+-rw-r--r--   0        0        0    10624 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/generate/metadata.py
+-rw-r--r--   0        0        0     8942 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/generate/properties.py
+-rw-r--r--   0        0        0    14017 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/generate/sources.py
+-rw-r--r--   0        0        0     2715 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/generate/templates.py
+-rw-r--r--   0        0        0        0 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/load/__init__.py
+-rw-r--r--   0        0        0    25744 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/load/airbyte.py
+-rw-r--r--   0        0        0     2259 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/load/base.py
+-rw-r--r--   0        0        0    18452 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/load/fivetran.py
+-rw-r--r--   0        0        0      946 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/load/main.py
+-rw-r--r--   0        0        0        0 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/__init__.py
+-rw-r--r--   0        0        0     2004 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/all.py
+-rw-r--r--   0        0        0      494 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/base.py
+-rw-r--r--   0        0        0     4287 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/dbt.py
+-rw-r--r--   0        0        0     6751 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/git.py
+-rw-r--r--   0        0        0     1266 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/main.py
+-rw-r--r--   0        0        0     1664 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/pre_commit.py
+-rw-r--r--   0        0        0    10262 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/ssh.py
+-rw-r--r--   0        0        0      845 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/templates/pre_commit/copier.yml
+-rw-r--r--   0        0        0     2110 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/templates/pre_commit/{% if use_sqlfluff or use_yamllint or use_dbt_checkpoint %}pre-commit-config.yaml{% endif %}.jinja
+-rw-r--r--   0        0        0       75 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluffignore{% endif %}
+-rw-r--r--   0        0        0     2743 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluff{% endif %}.jinja
+-rw-r--r--   0        0        0      668 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_yamllint %}.yamllint{% endif %}
+-rw-r--r--   0        0        0      102 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{{ _copier_conf.answers_file }}-precommit.yaml.jinja
+-rw-r--r--   0        0        0     1371 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/utils.py
+-rw-r--r--   0        0        0      255 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/templates/model_props.yml
+-rw-r--r--   0        0        0      214 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/templates/source_props.yml
+-rw-r--r--   0        0        0     1201 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/templates/staging_model.sql
+-rw-r--r--   0        0        0      495 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/templates/staging_model_props.yml
+-rw-r--r--   0        0        0        0 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/ui/__init__.py
+-rw-r--r--   0        0        0     1202 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/ui/traceback.py
+-rw-r--r--   0        0        0        0 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/utils/__init__.py
+-rw-r--r--   0        0        0    11270 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/utils/api_caller.py
+-rw-r--r--   0        0        0    14725 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/utils/flags.py
+-rw-r--r--   0        0        0     1132 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/utils/jinja.py
+-rw-r--r--   0        0        0      785 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/utils/log.py
+-rw-r--r--   0        0        0      791 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/utils/shell.py
+-rw-r--r--   0        0        0     1765 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/utils/tracking.py
+-rw-r--r--   0        0        0     1010 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/utils/yaml.py
+-rw-r--r--   0        0        0     3606 2023-05-19 17:40:19.076274 dbt_coves-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0    23695 1970-01-01 00:00:00.000000 dbt_coves-1.5.1/PKG-INFO
```

### Comparing `dbt_coves-1.5.0/LICENSE` & `dbt_coves-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.0/README.md` & `dbt_coves-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.0/dbt_coves/config/config.py` & `dbt_coves-1.5.1/dbt_coves/config/config.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.0/dbt_coves/core/exceptions.py` & `dbt_coves-1.5.1/dbt_coves/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.0/dbt_coves/core/main.py` & `dbt_coves-1.5.1/dbt_coves/core/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,15 @@
 import argparse
+import pathlib
 import sys
+import uuid
 from typing import List
 
 import pyfiglet
 from dbt import tracking, version
-
-try:
-    from dbt.flags import PROFILES_DIR
-
-    VARS_DEFAULT_IS_STR = False
-except ImportError:
-    from dbt.cli.resolvers import default_profiles_dir
-
-    PROFILES_DIR = default_profiles_dir()
-    VARS_DEFAULT_IS_STR = True
 from rich.console import Console
 
 from dbt_coves import __version__
 from dbt_coves.config.config import DbtCovesConfig
 from dbt_coves.core.exceptions import MissingCommand, MissingDbtProject
 from dbt_coves.tasks.base import BaseTask
 from dbt_coves.tasks.dbt.main import RunDbtTask
@@ -25,14 +17,25 @@
 from dbt_coves.tasks.generate.main import GenerateTask
 from dbt_coves.tasks.load.main import LoadTask
 from dbt_coves.tasks.setup.main import SetupTask
 from dbt_coves.ui.traceback import DbtCovesTraceback
 from dbt_coves.utils.flags import DbtCovesFlags
 from dbt_coves.utils.log import LOGGER as logger
 from dbt_coves.utils.log import log_manager
+from dbt_coves.utils.yaml import open_yaml, save_yaml
+
+try:
+    from dbt.flags import PROFILES_DIR
+
+    VARS_DEFAULT_IS_STR = False
+except ImportError:
+    from dbt.cli.resolvers import default_profiles_dir
+
+    PROFILES_DIR = default_profiles_dir()
+    VARS_DEFAULT_IS_STR = True
 
 console = Console()
 
 parser = argparse.ArgumentParser(
     prog="dbt-coves",
     formatter_class=argparse.RawTextHelpFormatter,
     description="CLI tool for dbt users applying analytics engineering best practices.",
@@ -181,14 +184,21 @@
     "--static-parser",
     action="store_true",
     default=False,
     help="Use the static parser.",
     dest="STATIC_PARSER",
 )
 
+base_subparser.add_argument(
+    "--disable-tracking",
+    action="store_true",
+    default=False,
+    help="Disable command usage tracking. We don't store any user information.",
+)
+
 sub_parsers = parser.add_subparsers(title="dbt-coves commands", dest="task")
 
 # Register subcommands
 [
     task.register_parser(sub_parsers, base_subparser)
     for task in [GenerateTask, SetupTask, ExtractTask, LoadTask, RunDbtTask]
 ]
@@ -209,14 +219,15 @@
     coves_config = None
     if task_cls.needs_config:
         coves_config = DbtCovesConfig(main_parser)
         coves_config.load_config()
 
     if main_parser.log_level == "debug":
         log_manager.set_debug()
+    _gen_get_app_uuid(main_parser.args)
     return task_cls.get_instance(main_parser, coves_config=coves_config).run()
 
 
 def main(parser: argparse.ArgumentParser = parser, test_cli_args: List[str] = list()) -> int:
     tracking.do_not_track()
 
     exit_code = 0
@@ -248,9 +259,23 @@
         return 1
 
     if exit_code > 0:
         logger.error("[red]The process did not complete successfully.")
     return exit_code
 
 
+def _gen_get_app_uuid(args):
+    dbt_coves_homepath = pathlib.Path("~/.dbt-coves/").expanduser()
+    dbt_coves_homepath.mkdir(exist_ok=True)
+    uuid_path = dbt_coves_homepath / ".user.yml"
+    try:
+        existent_uuid = open_yaml(uuid_path).get("id")
+        args.uuid = existent_uuid
+    except FileNotFoundError:
+        dbt_coves_uuid = str(uuid.uuid4())
+        dbt_coves_user = {"id": dbt_coves_uuid}
+        save_yaml(uuid_path, dbt_coves_user)
+        args.uuid = dbt_coves_uuid
+
+
 if __name__ == "__main__":
     exit(main())
```

### Comparing `dbt_coves-1.5.0/dbt_coves/tasks/base.py` & `dbt_coves-1.5.1/dbt_coves/tasks/base.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.0/dbt_coves/tasks/dbt/main.py` & `dbt_coves-1.5.1/dbt_coves/tasks/dbt/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import tempfile
 from pathlib import Path
 
 from rich.console import Console
 from rich.text import Text
 
 from dbt_coves.tasks.base import NonDbtBaseConfiguredTask
+from dbt_coves.utils.tracking import trackable
 
 console = Console()
 
 
 class RunDbtException(Exception):
     pass
 
@@ -53,14 +54,15 @@
             type=str,
             nargs="+",
             help="dbt command to run, i.e. 'run -s model_name'",
         )
 
         return ext_subparser
 
+    @trackable
     def run(self) -> int:
         project_dir = self.get_config_value("project_dir")
         if not project_dir:
             project_dir = os.environ.get("DBT_PROJECT_DIR", os.environ.get("DATACOVES__DBT_HOME"))
         if not project_dir:
             console.print("[red]No dbt project specified[/red].")
             return -1
```

### Comparing `dbt_coves-1.5.0/dbt_coves/tasks/extract/airbyte.py` & `dbt_coves-1.5.1/dbt_coves/tasks/extract/airbyte.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 import pathlib
 from copy import copy
 
 from rich.console import Console
 
 from dbt_coves.utils.api_caller import AirbyteApiCaller
+from dbt_coves.utils.tracking import trackable
 
 from .base import BaseExtractTask
 
 # from dbt_coves.utils import airbyte_api
 
 console = Console()
 NON_EXTRACT_KEYS = ["icon", "breakingChange"]
@@ -48,14 +49,15 @@
             "--port",
             type=str,
             help="Airbyte's API port, i.e. '8001'",
         )
         subparser.set_defaults(cls=cls, which="airbyte")
         return subparser
 
+    @trackable
     def run(self):
         self.extraction_results = {
             "sources": set(),
             "destinations": set(),
             "connections": set(),
         }
```

### Comparing `dbt_coves-1.5.0/dbt_coves/tasks/extract/fivetran.py` & `dbt_coves-1.5.1/dbt_coves/tasks/extract/fivetran.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pathlib import Path
 
 import questionary
 from rich.console import Console
 
 from dbt_coves.utils.api_caller import FivetranApiCaller
+from dbt_coves.utils.tracking import trackable
 from dbt_coves.utils.yaml import open_yaml
 
 from .base import BaseExtractTask
 
 console = Console()
 
 
@@ -48,14 +49,15 @@
         )
         subparser.set_defaults(cls=cls, which="fivetran")
         return subparser
 
     def get_config_value(self, key):
         return self.coves_config.integrated["extract"]["fivetran"][key]
 
+    @trackable
     def run(self) -> int:
         self.extraction_results = set()
 
         extract_destination = self.get_config_value("path")
         self.api_key = self.get_config_value("api_key")
         self.api_secret = self.get_config_value("api_secret")
         api_credentials_path = self.get_config_value("credentials")
```

### Comparing `dbt_coves-1.5.0/dbt_coves/tasks/extract/main.py` & `dbt_coves-1.5.1/dbt_coves/tasks/extract/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.0/dbt_coves/tasks/generate/base.py` & `dbt_coves-1.5.1/dbt_coves/tasks/generate/base.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.0/dbt_coves/tasks/generate/main.py` & `dbt_coves-1.5.1/dbt_coves/tasks/generate/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.0/dbt_coves/tasks/generate/metadata.py` & `dbt_coves-1.5.1/dbt_coves/tasks/generate/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pathlib import Path
 
 import questionary
 from questionary import Choice
 from rich.console import Console
 
 from dbt_coves.utils.jinja import render_template
+from dbt_coves.utils.tracking import trackable
 
 from .base import BaseGenerateTask
 
 console = Console()
 
 
 class GenerateMetadataTask(BaseGenerateTask):
@@ -250,14 +251,15 @@
                     action = "create"
             else:
                 action = "create"
 
             self.generate_or_append_metadata(rel, csv_path, options, action, existing_rows)
             self.metadata_files_processed.add(csv_path)
 
+    @trackable
     def run(self):
         self.no_prompt = self.get_config_value("no_prompt")
         config_database = self.get_config_value("database")
         self.db = config_database or self.config.credentials.database
 
         with self.adapter.connection_named("master"):
             filtered_schemas = self.get_schemas()
```

### Comparing `dbt_coves-1.5.0/dbt_coves/tasks/generate/properties.py` & `dbt_coves-1.5.1/dbt_coves/tasks/generate/properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pathlib import Path
 
 import questionary
 from questionary import Choice
 from rich.console import Console
 
 from dbt_coves.utils.jinja import render_template
+from dbt_coves.utils.tracking import trackable
 
 from .base import BaseGenerateTask
 
 console = Console()
 
 
 class GeneratePropertiesException(Exception):
@@ -237,14 +238,15 @@
             templates_folder,
             update_strategy,
             "model",
             destination,
             "model_props.yml",
         )
 
+    @trackable
     def run(self):
         self.no_prompt = self.get_config_value("no_prompt")
         self.get_metadata()
         with self.adapter.connection_named("master"):
             dbt_models = self.list_from_dbt_ls("json")
             manifest = self.load_manifest_nodes()
             models = self.select_models(dbt_models)
```

### Comparing `dbt_coves-1.5.0/dbt_coves/tasks/generate/sources.py` & `dbt_coves-1.5.1/dbt_coves/tasks/generate/sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pathlib import Path
 
 import questionary
 from questionary import Choice
 from rich.console import Console
 
 from dbt_coves.utils.jinja import render_template, render_template_file
+from dbt_coves.utils.tracking import trackable
 
 from .base import BaseGenerateTask
 
 console = Console()
 
 
 class GenerateSourcesTask(BaseGenerateTask):
@@ -330,14 +331,15 @@
                 }
                 metadata_key = self.get_metadata_map_key(metadata_map_key_data)
                 # Get metadata info or default and assign to the field.
                 metadata_info = metadata.get(metadata_key)
                 if metadata_info:
                     data[col][item].update(metadata_info)
 
+    @trackable
     def run(self):
         self.no_prompt = self.get_config_value("no_prompt")
         config_database = self.get_config_value("database")
         self.db = config_database or self.config.credentials.database
 
         self.get_metadata()
```

### Comparing `dbt_coves-1.5.0/dbt_coves/tasks/generate/templates.py` & `dbt_coves-1.5.1/dbt_coves/tasks/generate/templates.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pathlib import Path
 
 import questionary
 from rich import console
 
 import dbt_coves
 from dbt_coves.tasks.base import BaseConfiguredTask
+from dbt_coves.utils.tracking import trackable
 
 console = console.Console()
 
 
 class GenerateTemplatesException(Exception):
     pass
 
@@ -35,14 +36,15 @@
             shutil.copyfile(dbtcoves_template_path, destination_template_path)
             console.print(f"Generated [green]{destination_template_path}[/green]")
         except OSError as e:
             raise GenerateTemplatesException(
                 f"Couldn't generate {template_name} template file: {e}"
             )
 
+    @trackable
     def run(self):
         options = {"overwrite_all": False}
         dbtcoves_templates_path = Path(dbt_coves.__file__).parent / "templates"
 
         dbt_project_path = self.config.project_root
         templates_destination_path = (
             dbt_project_path
```

### Comparing `dbt_coves-1.5.0/dbt_coves/tasks/load/airbyte.py` & `dbt_coves-1.5.1/dbt_coves/tasks/load/airbyte.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from os import path
 
 import questionary
 from rich.console import Console
 from slugify import slugify
 
 from dbt_coves.utils.api_caller import AirbyteApiCaller, AirbyteApiCallerException
+from dbt_coves.utils.tracking import trackable
 
 from .base import BaseLoadTask
 
 console = Console()
 
 
 class AirbyteLoaderException(Exception):
@@ -64,14 +65,15 @@
         )
         subparser.add_argument("--secrets-project", type=str, help="Secret credentials project")
         subparser.add_argument("--secrets-tags", type=str, help="Secret credentials tags")
         subparser.add_argument("--secrets-key", type=str, help="Secret credentials key")
         subparser.set_defaults(cls=cls, which="airbyte")
         return subparser
 
+    @trackable
     def run(self):
         self.loading_results = {
             "sources": {"updated": [], "created": []},
             "destinations": {"updated": [], "created": []},
             "connections": {"updated": [], "created": []},
         }
         self.load_destination = self.get_config_value("path")
```

### Comparing `dbt_coves-1.5.0/dbt_coves/tasks/load/base.py` & `dbt_coves-1.5.1/dbt_coves/tasks/load/base.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.0/dbt_coves/tasks/load/fivetran.py` & `dbt_coves-1.5.1/dbt_coves/tasks/load/fivetran.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pathlib import Path
 
 import questionary
 from rich.console import Console
 
 from dbt_coves.utils.api_caller import FivetranApiCaller
+from dbt_coves.utils.tracking import trackable
 from dbt_coves.utils.yaml import open_yaml
 
 from .base import BaseLoadTask
 
 console = Console()
 
 
@@ -69,14 +70,15 @@
             for activity, result in result_dict.items():
                 if len(result) > 0:
                     console.print(
                         f"{obj_type.capitalize()} {activity}: "
                         f"[green]{', '.join(result)}[/green]"
                     )
 
+    @trackable
     def run(self) -> int:
         self.load_results = {
             "groups": {"created": set()},
             "destinations": {"created": set(), "updated": set()},
             "connectors": {"created": set(), "updated": set()},
             "schemas": {"updated": set()},
             "tables": {"updated": set()},
```

### Comparing `dbt_coves-1.5.0/dbt_coves/tasks/load/main.py` & `dbt_coves-1.5.1/dbt_coves/tasks/load/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.0/dbt_coves/tasks/setup/dbt.py` & `dbt_coves-1.5.1/dbt_coves/tasks/setup/dbt.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 import os
 from pathlib import Path
 
 from rich.console import Console
 
 from dbt_coves.config.config import DbtCovesConfig
-from dbt_coves.tasks.base import NonDbtBaseTask
+from dbt_coves.tasks.setup.base import BaseSetupTask
 from dbt_coves.utils.shell import run_and_capture_cwd
+from dbt_coves.utils.tracking import trackable
 
 from .utils import file_exists, print_row
 
 console = Console()
 
 
-class SetupDbtTask(NonDbtBaseTask):
+class SetupDbtTask(BaseSetupTask):
     """
     Task that runs ssh key generation, git repo clone and db connection setup
     """
 
     @classmethod
     def register_parser(cls, sub_parsers, base_subparser):
         subparser = sub_parsers.add_parser(
             "dbt",
             parents=[base_subparser],
             help="Set up dbt for dbt-coves project",
         )
         subparser.set_defaults(cls=cls, which="dbt")
         return subparser
 
-    @classmethod
-    def run(cls) -> int:
-        config_folder = cls.get_config_folder(mandatory=False)
-        cls.dbt_init(config_folder)
-        cls.dbt_debug(config_folder)
-        cls.dbt_deps(config_folder)
+    @trackable
+    def run(self) -> int:
+        config_folder = self.get_config_folder(mandatory=False)
+        self.dbt_init(config_folder)
+        self.dbt_debug(config_folder)
+        self.dbt_deps(config_folder)
         return 0
 
-    @classmethod
-    def get_config_folder(cls, mandatory=True):
+    def get_config_folder(self, mandatory=True):
         workspace_path = os.environ.get("WORKSPACE_PATH", Path.cwd())
         return DbtCovesConfig.get_config_folder(workspace_path=workspace_path, mandatory=mandatory)
 
-    @classmethod
-    def dbt_debug(cls, config_folder=None):
+    def dbt_debug(self, config_folder=None):
         if not config_folder:
-            config_folder = cls.get_config_folder(mandatory=False)
+            config_folder = self.get_config_folder(mandatory=False)
 
         if config_folder:
             dbt_project_yaml_path = Path(config_folder.parent) / "dbt_project.yml"
         else:
             dbt_project_yaml_path = file_exists(Path(os.getcwd()), "dbt_project.yml")
 
         debug_status = "[red]FAIL[/red]"
@@ -61,18 +60,17 @@
             "dbt debug",
             debug_status,
             new_section=True,
         )
         if output.returncode > 0:
             raise Exception("dbt debug error. Check logs.")
 
-    @classmethod
-    def dbt_init(cls, config_folder=None):
+    def dbt_init(self, config_folder=None):
         if not config_folder:
-            config_folder = cls.get_config_folder(mandatory=False)
+            config_folder = self.get_config_folder(mandatory=False)
 
         if config_folder:
             dbt_project_yaml_path = Path(config_folder.parent) / "dbt_project.yml"
         else:
             dbt_project_yaml_path = file_exists(Path.cwd(), "dbt_project.yml")
 
         if not dbt_project_yaml_path:
@@ -92,18 +90,17 @@
                 "dbt init",
                 init_status,
                 new_section=True,
             )
         else:
             raise Exception("dbt init error. Check logs.")
 
-    @classmethod
-    def dbt_deps(cls, config_folder=None):
+    def dbt_deps(self, config_folder=None):
         if not config_folder:
-            config_folder = cls.get_config_folder(mandatory=False)
+            config_folder = self.get_config_folder(mandatory=False)
 
         if config_folder:
             dbt_project_yaml_path = Path(config_folder.parent) / "dbt_project.yml"
         else:
             dbt_project_yaml_path = file_exists(Path(os.getcwd()), "dbt_project.yml")
 
         if dbt_project_yaml_path.exists():
```

### Comparing `dbt_coves-1.5.0/dbt_coves/tasks/setup/git.py` & `dbt_coves-1.5.1/dbt_coves/tasks/setup/git.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import os
 from pathlib import Path
 from urllib.parse import urlparse
 
 import questionary
 from rich.console import Console
 
-from dbt_coves.tasks.base import NonDbtBaseTask
+from dbt_coves.tasks.setup.base import BaseSetupTask
 from dbt_coves.utils.shell import run, run_and_capture
+from dbt_coves.utils.tracking import trackable
 
 from .utils import print_row
 
 console = Console()
 
 
 class SetupGitException(Exception):
     pass
 
 
-class SetupGitTask(NonDbtBaseTask):
+class SetupGitTask(BaseSetupTask):
     """
     Task that runs ssh key generation, git repo clone and db connection setup
     """
 
     key_column_with = 50
     value_column_with = 30
 
@@ -37,20 +38,21 @@
             help="Configure Git without user intervention",
             action="store_true",
             default=False,
         )
         subparser.set_defaults(cls=cls, which="git")
         return subparser
 
+    @trackable
     def run(self, workspace_path=Path.cwd()) -> int:
-        self._run_git_config()
-        self._run_git_clone(workspace_path)
+        self.run_git_config()
+        self.run_git_clone(workspace_path)
         return 0
 
-    def _run_git_config(self):
+    def run_git_config(self):
         config_status = "[red]MISSING[/red]"
 
         email_output = run_and_capture(["git", "config", "--global", "--get", "user.email"])
         email_exists = email_output.returncode == 0 and email_output.stdout
         email = email_output.stdout.replace("\n", "")
 
         name_output = run_and_capture(["git", "config", "--global", "--get", "user.name"])
@@ -92,15 +94,15 @@
                     return 1
                 email_output = run_and_capture(["git", "config", "--global", "user.email", email])
                 if email_output.returncode != 0:
                     console.print("Could not set user.email")
                     return 1
                 console.print("[green]:heavy_check_mark: Git user configured successfully.")
 
-    def _run_git_clone(self, workspace_path):
+    def run_git_clone(self, workspace_path):
         repo_url = ""
         cloned_status = "[red]MISSING[/red]"
         cloned_exists = Path(workspace_path, ".git").exists()
         if cloned_exists:
             cloned_status = "[green]FOUND :heavy_check_mark:[/green]"
         print_row("Checking for git repo", cloned_status, new_section=True)
```

### Comparing `dbt_coves-1.5.0/dbt_coves/tasks/setup/pre_commit.py` & `dbt_coves-1.5.1/dbt_coves/tasks/setup/pre_commit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from pathlib import Path
 
 import copier
 import questionary
 from rich.console import Console
 
+from dbt_coves.utils.tracking import trackable
+
 from .main import NonDbtBaseTask
 from .utils import get_dbt_projects, get_git_root
 
 console = Console()
 
 
 class SetupPrecommitException(Exception):
@@ -25,21 +27,21 @@
             "precommit",
             parents=[base_subparser],
             help="Set up pre-commit for dbt-coves project",
         )
         subparser.set_defaults(cls=cls, which="precommit")
         return subparser
 
-    @classmethod
-    def run(cls) -> int:
-        cls.setup_precommit()
+    @trackable
+    def run(self) -> int:
+        self.setup_precommit()
         return 0
 
     @classmethod
-    def setup_precommit(cls):
+    def setup_precommit(self):
         repo_root = get_git_root()
         dbt_project_paths = get_dbt_projects(repo_root)
         if not dbt_project_paths:
             raise SetupPrecommitException(
                 "Your repository doesn't contain any dbt project where to install pre-commit into"
             )
         data = {}
```

### Comparing `dbt_coves-1.5.0/dbt_coves/tasks/setup/ssh.py` & `dbt_coves-1.5.1/dbt_coves/tasks/setup/ssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from subprocess import CalledProcessError
 
 import questionary
 from rich.console import Console
 
 from dbt_coves.tasks.base import NonDbtBaseTask
 from dbt_coves.utils.shell import run_and_capture, shell_run
+from dbt_coves.utils.tracking import trackable
 
 from .utils import print_row
 
 console = Console()
 
 
 class SetupSSHException(Exception):
@@ -39,15 +40,15 @@
             action="store_true",
             default=False,
         )
         subparser.set_defaults(cls=cls, which="ssh")
         cls.arg_parser = base_subparser
         return subparser
 
-    def run(self) -> int:
+    def setup_ssh(self):
         ssh_status = "[red]MISSING[/red]"
         ssh_configured = False
         ssh_keys_dir = "~/.ssh/"
         self.ssh_keys_dir_abs = os.path.abspath(Path(ssh_keys_dir).expanduser())
 
         provided_key_path = f"{self.ssh_keys_dir_abs}/id_datacoves"
 
@@ -113,14 +114,18 @@
             return 0
         else:
             raise Exception(
                 "You must first configure you SSH key in your Git server"
                 "then rerun 'dbt-coves setup'"
             )
 
+    @trackable
+    def run(self) -> int:
+        return self.setup_ssh()
+
     def generate_ecdsa_keys(self, key_path_abs):
         try:
             return shell_run(args=["ssh-keygen", "-q", "-t", "ecdsa", "-f", key_path_abs])
         except CalledProcessError as e:
             raise SetupSSHException(e.output)
 
     def generate_ecdsa_public_key(self, private_path_abs):
```

### Comparing `dbt_coves-1.5.0/dbt_coves/tasks/setup/templates/pre_commit/copier.yml` & `dbt_coves-1.5.1/dbt_coves/tasks/setup/templates/pre_commit/copier.yml`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.0/dbt_coves/tasks/setup/templates/pre_commit/{% if use_sqlfluff or use_yamllint or use_dbt_checkpoint %}pre-commit-config.yaml{% endif %}.jinja` & `dbt_coves-1.5.1/dbt_coves/tasks/setup/templates/pre_commit/{% if use_sqlfluff or use_yamllint or use_dbt_checkpoint %}pre-commit-config.yaml{% endif %}.jinja`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.0/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluff{% endif %}.jinja` & `dbt_coves-1.5.1/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluff{% endif %}.jinja`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.0/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_yamllint %}.yamllint{% endif %}` & `dbt_coves-1.5.1/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_yamllint %}.yamllint{% endif %}`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.0/dbt_coves/tasks/setup/utils.py` & `dbt_coves-1.5.1/dbt_coves/tasks/setup/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.0/dbt_coves/templates/staging_model.sql` & `dbt_coves-1.5.1/dbt_coves/templates/staging_model.sql`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.0/dbt_coves/ui/traceback.py` & `dbt_coves-1.5.1/dbt_coves/ui/traceback.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.0/dbt_coves/utils/api_caller.py` & `dbt_coves-1.5.1/dbt_coves/utils/api_caller.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.0/dbt_coves/utils/flags.py` & `dbt_coves-1.5.1/dbt_coves/utils/flags.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.0/dbt_coves/utils/jinja.py` & `dbt_coves-1.5.1/dbt_coves/utils/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.0/dbt_coves/utils/log.py` & `dbt_coves-1.5.1/dbt_coves/utils/log.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.0/dbt_coves/utils/shell.py` & `dbt_coves-1.5.1/dbt_coves/utils/shell.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.0/dbt_coves/utils/yaml.py` & `dbt_coves-1.5.1/dbt_coves/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.0/pyproject.toml` & `dbt_coves-1.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt_coves"
-version = "1.5.0"
+version = "1.5.1"
 description = "CLI tool for dbt users adopting analytics engineering best practices."
 authors = ["Datacoves <hello@datacoves.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Information Technology",
@@ -39,14 +39,15 @@
 dbt-core = ">=1.1,<1.6"
 bumpversion = "^0.6.0"
 typing_extensions = { version = "^4.0", python = "^3.7" }
 ruamel-yaml = "^0.17.21"
 db-dtypes = "^1.0.5"
 copier = "6.0.0"
 gitpython = "^3.1.31"
+mixpanel = "^4.10.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 mypy = "^0.991"
 towncrier = "^22.12.0"
 pytest-mock = "^3.6.1"
@@ -117,12 +118,12 @@
 markers = ["datafiles"]
 
 [tool.black]
 line-length = 100
 target-version=['py37', 'py38', 'py39', 'py310', 'py311']
 
 [tool.isort]
-known_third_party=["copier", "dbt", "dotenv", "git", "google", "jinja2", "pretty_errors", "pydantic", "pyfiglet", "pytest", "questionary", "redshift_connector", "requests", "rich", "ruamel", "slugify", "snowflake"]
+known_third_party=["copier", "dbt", "dotenv", "git", "google", "jinja2", "mixpanel", "pretty_errors", "pydantic", "pyfiglet", "pytest", "questionary", "redshift_connector", "requests", "rich", "ruamel", "slugify", "snowflake"]
 line_length=100
 multi_line_output=3
 include_trailing_comma=true
 profile="black"
```

### Comparing `dbt_coves-1.5.0/setup.py` & `dbt_coves-1.5.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,639 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: dbt-coves
+Version: 1.5.1
+Summary: CLI tool for dbt users adopting analytics engineering best practices.
+Home-page: https://datacoves.com
+License: Apache 2.0
+Keywords: data engineering,analytics engineering,dbt,ETL,data modelling
+Author: Datacoves
+Author-email: hello@datacoves.com
+Requires-Python: >=3.7.2,<3.11
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Code Generators
+Requires-Dist: Jinja2 (>2.11.2)
+Requires-Dist: PyYAML (>=5.4.1)
+Requires-Dist: bumpversion (>=0.6.0,<0.7.0)
+Requires-Dist: click (>=8.0.3,<9.0.0)
+Requires-Dist: copier (==6.0.0)
+Requires-Dist: db-dtypes (>=1.0.5,<2.0.0)
+Requires-Dist: dbt-core (>=1.1,<1.6)
+Requires-Dist: gitpython (>=3.1.31,<4.0.0)
+Requires-Dist: luddite (>=1.0.1,<2.0.0)
+Requires-Dist: mixpanel (>=4.10.0,<5.0.0)
+Requires-Dist: packaging (>=20.8,<22.0)
+Requires-Dist: pretty-errors (>=1.2.19,<2.0.0)
+Requires-Dist: pydantic (>=1.8,<2.0)
+Requires-Dist: pyfiglet (>=0.8.post1,<0.9)
+Requires-Dist: python-slugify (<9.0.0)
+Requires-Dist: questionary (>=1.9.0,<2.0.0)
+Requires-Dist: rich (>=10.4,<14.0)
+Requires-Dist: ruamel-yaml (>=0.17.21,<0.18.0)
+Requires-Dist: typing_extensions (>=4.0,<5.0) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: yamlloader (>=1.0.0,<2.0.0)
+Project-URL: Documentation, https://datacoves.gitbook.io/dbt-coves/
+Project-URL: Repository, https://github.com/datacoves/dbt-coves
+Description-Content-Type: text/markdown
 
-packages = \
-['dbt_coves',
- 'dbt_coves.config',
- 'dbt_coves.core',
- 'dbt_coves.tasks',
- 'dbt_coves.tasks.dbt',
- 'dbt_coves.tasks.extract',
- 'dbt_coves.tasks.generate',
- 'dbt_coves.tasks.load',
- 'dbt_coves.tasks.setup',
- 'dbt_coves.ui',
- 'dbt_coves.utils']
-
-package_data = \
-{'': ['*'],
- 'dbt_coves': ['templates/*'],
- 'dbt_coves.tasks.setup': ['templates/pre_commit/*',
-                           'templates/pre_commit/{{ dbt_project_dir }}/*']}
-
-install_requires = \
-['Jinja2>2.11.2',
- 'PyYAML>=5.4.1',
- 'bumpversion>=0.6.0,<0.7.0',
- 'click>=8.0.3,<9.0.0',
- 'copier==6.0.0',
- 'db-dtypes>=1.0.5,<2.0.0',
- 'dbt-core>=1.1,<1.6',
- 'gitpython>=3.1.31,<4.0.0',
- 'luddite>=1.0.1,<2.0.0',
- 'packaging>=20.8,<22.0',
- 'pretty-errors>=1.2.19,<2.0.0',
- 'pydantic>=1.8,<2.0',
- 'pyfiglet>=0.8.post1,<0.9',
- 'python-slugify<9.0.0',
- 'questionary>=1.9.0,<2.0.0',
- 'rich>=10.4,<14.0',
- 'ruamel-yaml>=0.17.21,<0.18.0',
- 'yamlloader>=1.0.0,<2.0.0']
-
-extras_require = \
-{':python_version >= "3.7" and python_version < "4.0"': ['typing_extensions>=4.0,<5.0']}
-
-entry_points = \
-{'console_scripts': ['dbt-coves = dbt_coves.core.main:main']}
-
-setup_kwargs = {
-    'name': 'dbt-coves',
-    'version': '1.5.0',
-    'description': 'CLI tool for dbt users adopting analytics engineering best practices.',
-    'long_description': '# dbt-coves\n\n## Sponsor\n\n<picture>\n  <source media="(prefers-color-scheme: dark)" srcset="images/datacoves-dark.png">\n  <img alt="Datacoves" src="images/datacoves-light.png" width="150">\n</picture>\n\nHosted VS Code, dbt-core, SqlFluff, and Airflow, find out more at [Datacoves.com](https://datacoves.com/product).\n\n## What is dbt-coves?\n\ndbt-coves is a CLI tool that automates certain tasks for [dbt](https://www.getdbt.com), making life simpler for the dbt user.\n\ndbt-coves generates dbt sources, staging models and property(yml) files by analyzing information from the data warehouse and creating the necessary files (sql and yml).\n\nFinally, dbt-coves includes functionality to bootstrap a dbt project and to extract and load configurations from Airbyte.\n\n## Supported dbt versions\n\n| Version | Status           |\n| ------- | ---------------- |\n| \\< 1.0  | ❌ Not supported |\n| >= 1.0  | ✅ Tested        |\n\nFrom `dbt-coves` 1.4.0 onwards, our major and minor versions match those of [dbt-core](https://github.com/dbt-labs/dbt-core).\nThis means we release a new major/minor version once it\'s dbt-core equivalent is tested.\nPatch suffix (1.4.X) is exclusive to our continuous development and does not reflect a version match with dbt\n\n## Supported adapters\n\n| Feature                           | Snowflake | Redshift  | BigQuery  |\n| --------------------------------- | --------- | --------- | --------- |\n| dbt project setup                 | ✅ Tested | ✅ Tested | ✅ Tested |\n| source model (sql) generation     | ✅ Tested | ✅ Tested | ✅ Tested |\n| model properties (yml) generation | ✅ Tested | ✅ Tested | ✅ Tested |\n\nNOTE: Other database adapters may work, although we have not tested them. Feel free to try them and let us know so we can update the table above.\n\n### Here\\\'s the tool in action\n\n[![image](https://cdn.loom.com/sessions/thumbnails/74062cf71cbe4898805ca508ea2d9455-1624905546029-with-play.gif)](https://www.loom.com/share/74062cf71cbe4898805ca508ea2d9455)\n\n# Installation\n\n```console\npip install dbt-coves\n```\n\nWe recommend using [python\nvirtualenvs](https://docs.python.org/3/tutorial/venv.html) and create\none separate environment per project.\n\n# Command Reference\n\nFor a complete list of options, please run:\n\n```console\ndbt-coves -h\ndbt-coves <command> -h\n```\n\n## Environment setup\n\nSetting up your environment can be done in two different ways:\n\nRuns a set of scripts in your local environment to configure your project components: `ssh keys`, `git` and `dbt`\n\n```console\ndbt-coves setup all\n```\n\nYou can configure individual components:\n\nSet up `git` repository of dbt-coves project\n\n```console\ndbt-coves setup git\n```\n\nSetup `dbt` within the project (delegates to dbt init)\n\n```console\ndbt-coves setup dbt\n```\n\nSet up SSH Keys for dbt project. Supports the argument `--open_ssl_public_key` which generates an extra Public Key in Open SSL format, useful for configuring certain providers (i.e. Snowflake authentication)\n\n```console\ndbt-coves setup ssh\n```\n\n## Models generation\n\n```console\ndbt-coves generate <resource>\n```\n\nWhere _\\<resource\\>_ could be _sources_, _properties_ or _metadata_.\n\n```console\ndbt-coves generate sources\n```\n\nThis command will generate the dbt source configuration as well as the initial dbt staging model(s). It will look in the database defined in your `profiles.yml` file or you can pass the `--database` argument or set up default configuration options (see below)\n\n```console\ndbt-coves generate sources --database raw\n```\n\nSupports Jinja templates to adjust how the resources are generated. See below for examples.\n\nEvery `dbt-coves generate <resource>` supports `--no-prompt` flag, which will silently generate all sources/models/properties/metadata without asking anything to the user.\n\n### Source Generation Arguments\n\ndbt-coves can be used to create the initial staging models. It will do the following:\n\n1. Create / Update the source yml file\n2. Create the initial staging model(sql) file and offer to flatten VARIANT(JSON) fields\n3. Create the staging model\'s property(yml) file.\n\n`dbt-coves generate sources` supports the following args:\n\nSee full list in help\n\n```console\ndbt-coves generate sources -h\n```\n\n```console\n--database\n# Database to inspect\n```\n\n```console\n--schemas\n# Schema(s) to inspect. Accepts wildcards (must be enclosed in quotes if used)\n```\n\n```console\n--select-relations\n# List of relations where raw data resides. The parameter must be enclosed in quotes. Accepts wildcards.\n```\n\n```console\n--exclude-relations\n# Filter relation(s) to exclude from source file(s) generation. The parameter must be enclosed in quotes. Accepts wildcards.\n```\n\n```console\n--sources-destination\n# Where sources yml files will be generated, default: \'models/staging/{{schema}}/sources.yml\'\n```\n\n```console\n--models-destination\n# Where models sql files will be generated, default: \'models/staging/{{schema}}/{{relation}}.sql\'\n```\n\n```console\n--model-props-destination\n# Where models yml files will be generated, default: \'models/staging/{{schema}}/{{relation}}.yml\'\n```\n\n```console\n--update-strategy\n# Action to perform when a property file already exists: \'update\', \'recreate\', \'fail\', \'ask\' (per file)\n```\n\n```console\n--templates-folder\n# Folder with jinja templates that override default sources generation templates, i.e. \'templates\'\n```\n\n```console\n--metadata\n# Path to csv file containing metadata, i.e. \'metadata.csv\'\n```\n\n```console\n--no-prompt\n# Silently generate source dbt models\n```\n\n### Properties Generation Arguments\n\nYou can use dbt-coves to generate and update the properties(yml) file for a given dbt model(sql) file.\n\n`dbt-coves generate properties` supports the following args:\n\n```console\n--destination\n# Where models yml files will be generated, default: \'{{model_folder_path}}/{{model_file_name}}.yml\'\n```\n\n```console\n--update-strategy\n# Action to perform when a property file already exists: \'update\', \'recreate\', \'fail\', \'ask\' (per file)\n```\n\n```console\n-s --select\n# Filter model(s) to generate property file(s)\n```\n\n```console\n--exclude\n# Filter model(s) to exclude from property file(s) generation\n```\n\n```console\n--selector\n# Specify dbt selector for more complex model filtering\n```\n\n```console\n--templates-folder\n# Folder with jinja templates that override default properties generation templates, i.e. \'templates\'\n```\n\n```console\n--metadata\n# Path to csv file containing metadata, i.e. \'metadata.csv\'\n```\n\n```console\n--no-prompt\n# Silently generate dbt models property files\n```\n\nNote: `--select (or -s)`, `--exclude` and `--selector` work exactly as `dbt ls` selectors do. For usage details, visit [dbt list docs](https://docs.getdbt.com/reference/commands/list)\n\n### Metadata Generation Arguments\n\nYou can use dbt-coves to generate the metadata file(s) containing the basic structure of the csv that can be used in the above `dbt-coves generate sources/properties` commands.\nUsage of these metadata files can be found in [metadata](https://github.com/datacoves/dbt-coves#metadata) below.\n\n`dbt-coves generate metadata` supports the following args:\n\n```console\n--database\n# Database to inspect\n```\n\n```console\n--schemas\n# Schema(s) to inspect. Accepts wildcards (must be enclosed in quotes if used)\n```\n\n```console\n--select-relations\n# List of relations where raw data resides. The parameter must be enclosed in quotes. Accepts wildcards.\n```\n\n```console\n--exclude-relations\n# Filter relation(s) to exclude from source file(s) generation. The parameter must be enclosed in quotes. Accepts wildcards.\n```\n\n```console\n--destination\n# Where csv file(s) will be generated, default: \'metadata.csv\'\n# Supports using the Jinja tags `{{relation}}` and `{{schema}}`\n# if creating one csv per relation/table in schema, i.e: "metadata/{{relation}}.csv"\n```\n\n```console\n--no-prompt\n# Silently generate metadata\n```\n\n### Metadata\n\ndbt-coves supports the argument `--metadata` which allows users to specify a csv file containing field types and descriptions to be used when creating the staging models and property files.\n\n```console\ndbt-coves generate sources --metadata metadata.csv\n```\n\nMetadata format:\nYou can download a [sample csv file](sample_metadata.csv) as reference\n\n| database | schema | relation                          | column          | key  | type    | description                                     |\n| -------- | ------ | --------------------------------- | --------------- | ---- | ------- | ----------------------------------------------- |\n| raw      | raw    | \\_airbyte_raw_country_populations | \\_airbyte_data  | Year | integer | Year of country population measurement          |\n| raw      | raw    | \\_airbyte_raw_country_populations | \\_airbyte_data  |      | variant | Airbyte data columns (VARIANT) in Snowflake     |\n| raw      | raw    | \\_airbyte_raw_country_populations | \\_airbyte_ab_id |      | varchar | Airbyte unique identifier used during data load |\n\n## Extract configuration from Airbyte\n\n```console\ndbt-coves extract airbyte\n```\n\nExtracts the configuration from your Airbyte sources, connections and destinations (excluding credentials) and stores it in the specified folder. The main goal of this feature is to keep track of the configuration changes in your git repo, and rollback to a specific version when needed.\n\nFull usage example:\n\n```console\ndbt-coves extract airbyte --host http://airbyte-server --port 8001 --path /config/workspace/load/airbyte\n```\n\n## Load configuration to Airbyte\n\n```console\ndbt-coves load airbyte\n```\n\nLoads the Airbyte configuration generated with `dbt-coves extract airbyte` on an Airbyte server. Secrets folder needs to be specified separately. You can use [git-secret](https://git-secret.io/) to encrypt secrets and make them part of your git repo.\n\n### Loading secrets\n\nSecret credentials can be approached in two different ways: locally or remotely (through a provider/manager).\n\nIn order to load encrypted fields locally:\n\n```console\ndbt-coves load airbyte --secrets-path /path/to/secret/directory\n\n# This directory must have \'sources\', \'destinations\' and \'connections\' folders nested inside, and inside them the respective JSON files with unencrypted fields.\n# Naming convention: JSON unencrypted secret files must be named exactly as the extracted ones.\n```\n\nTo load encrypted fields through a manager (in this case we are connecting to Datacoves\' Service Credentials):\n\n```console\n--secrets-manager datacoves\n```\n\n```console\n--secrets-url https://api.datacoves.localhost/service-credentials/airbyte\n```\n\n```console\n--secrets-token <secret token>\n```\n\nFull usage example:\n\n```console\ndbt-coves load airbyte --host http://airbyte-server --port 8001 --path /config/workspace/load/airbyte --secrets-path /config/workspace/secrets\n```\n\n## Extract configuration from Fivetran\n\n```console\ndbt-coves extract fivetran\n```\n\nExtracts the configuration from your Fivetran destinations and connectors (excluding credentials) and stores it in the specified folder. The main goal of this feature is to keep track of the configuration changes in your git repo, and rollback to a specific version when needed.\n\nFull usage example:\n\n```console\ndbt-coves extract fivetran --credentials /config/workspace/secrets/fivetran/credentials.yml --path /config/workspace/load/fivetran\n```\n\n## Load configuration to Fivetran\n\n```console\ndbt-coves load fivetran\n```\n\nLoads the Fivetran configuration generated with `dbt-coves extract fivetran` on a Fivetran instance. Secrets folder needs to be specified separately. You can use [git-secret](https://git-secret.io/) to encrypt secrets and make them part of your git repo.\n\n### Credentials\n\nIn order for extract/load fivetran to work properly, you need to provide an api key-secret pair (you can generate them [here](https://fivetran.com/account/settings/account)).\n\nThese credentials can be used with `--api-key [key] --api-secret [secret]`, or specyfing a YML file with `--credentials /path/to/credentials.yml`. The required structure of this file is the following:\n\n```yaml\naccount_name: # Any name, used by dbt-coves to ask which to use when more than one is found\n  api_key: [key]\n  api_secret: [secret]\naccount_name_2:\n  api_key: [key]\n  api_secret: [secret]\n```\n\nThis YML file approach allows you to both work with multiple Fivetran accounts, and treat this credentials file as a secret.\n\n> :warning: **Warning**: --api-key/secret and --credentials flags are mutually exclusive, don\'t use them together.\n\n### Loading secrets\n\nSecret credentials can be approached via `--secrets-path` flag\n\n```console\ndbt-coves load fivetran --secrets-path /path/to/secret/directory\n```\n\n#### Field naming convention\n\nAlthough secret files can have any name, unencrypted JSON files must follow a simple structure:\n\n- Keys should match their corresponding Fivetran destination ID: two words automatically generated by Fivetran, which can be found in previously extracted data.\n- Inside those keys, a nested dictionary of which fields should be overwritten\n\nFor example:\n\n```json\n{\n  "extract_muscle": {\n    // Internal ID that Fivetran gave to a Snowflake warehouse Destination\n    "password": "[PASSWORD]" // Field:Value pair\n  },\n  "centre_straighten": {\n    "password": "[PASSWORD]"\n  }\n}\n```\n\n## Run dbt commands\n\n```shell\ndbt-coves dbt <arguments> -- <command>\n```\n\nRun dbt commands on special environments such as Airflow, or CI workers, with the possibility of changing dbt project location and activating a specific virtual environment in which running commands.\n\n### Arguments\n\n`dbt-coves dbt` supports the following arguments\n\n```shell\n--project-dir\n# Path of the dbt project where command will be executed, i.e.: /opt/user/dbt_project\n```\n\n```shell\n--virtualenv\n# Virtual environment path. i.e.: /opt/user/virtualenvs/airflow\n```\n\n### Sample usage\n\n```shell\ndbt-coves dbt --project-dir /opt/user/dbt_project --virtualenv /opt/user/virtualenvs/airflow -- run -s model --vars \\"{key: value}\\"\n# Make sure to escape special characters such as quotation marks\n# Double dash (--) between <arguments> and <command> are mandatory\n```\n\n# Settings\n\ndbt-coves will read settings from `.dbt_coves/config.yml`. A standard settings files could look like\nthis:\n\n```yaml\ngenerate:\n  sources:\n    database: "RAW" # Database where to look for source tables\n    schemas: # List of schema names where to look for source tables\n      - RAW\n    select_relations: # list of relations where raw data resides\n      - TABLE_1\n      - TABLE_2\n    exclude_relations: # Filter relation(s) to exclude from source file(s) generation\n      - TABLE_1\n      - TABLE_2\n    sources_destination: "models/staging/{{schema}}/{{schema}}.yml" # Where sources yml files will be generated\n    models_destination: "models/staging/{{schema}}/{{relation}}.sql" # Where models sql files will be generated\n    model_props_destination: "models/staging/{{schema}}/{{relation}}.yml" # Where models yml files will be generated\n    update_strategy: ask # Action to perform when a property file already exists. Options: update, recreate, fail, ask (per file)\n    templates_folder: ".dbt_coves/templates" # Folder where source generation jinja templates are located. Override default templates creating  source_props.yml, source_model_props.yml, and source_model.sql under this folder\n    metadata: "metadata.csv" # Path to csv file containing metadata\n\n  properties:\n    destination: "{{model_folder_path}}/{{model_file_name}}.yml" # Where models yml files will be generated\n    # You can specify a different path by declaring it explicitly, i.e.: "models/staging/{{model_file_name}}.yml"\n    update-strategy: ask # Action to perform when a property file already exists. Options: update, recreate, fail, ask (per file)\n    select: "models/staging/bays" # Filter model(s) to generate property file(s)\n    exclude: "models/staging/bays/test_bay" # Filter model(s) to generate property file(s)\n    selector: "selectors/bay_selector.yml" # Specify dbt selector for more complex model filtering\n    templates_folder: ".dbt_coves/templates" # Folder where source generation jinja templates are located. Override default template creating model_props.yml under this folder\n    metadata: "metadata.csv" # Path to csv file containing metadata\n\n  metadata:\n    database: RAW # Database where to look for source tables\n    schemas: # List of schema names where to look for source tables\n      - RAW\n    select_relations: # list of relations where raw data resides\n      - TABLE_1\n      - TABLE_2\n    exclude_relations: # Filter relation(s) to exclude from source file(s) generation\n      - TABLE_1\n      - TABLE_2\n    destination: # Where metadata file will be generated, default: \'metadata.csv\'\n\nextract:\n  airbyte:\n    path: /config/workspace/load/airbyte # Where json files will be generated\n    host: http://airbyte-server # Airbyte\'s API hostname\n    port: 8001 # Airbyte\'s API port\n  fivetran:\n    path: /config/workspace/load/fivetran # Where Fivetran export will be generated\n    api_key: [KEY] # Fivetran API Key\n    api_secret: [SECRET] # Fivetran API Secret\n    credentials: /opt/fivetran_credentials.yml # Fivetran set of key:secret pairs\n    # \'api_key\' + \'api_secret\' are mutually exclusive with \'credentials\', use one or the other\n\nload:\n  airbyte:\n    path: /config/workspace/load\n    host: http://airbyte-server\n    port: 8001\n    secrets_manager: datacoves # (optional) Secret credentials provider (secrets_path OR secrets_manager should be used, can\'t load secrets locally and remotely at the same time)\n    secrets_path: /config/workspace/secrets # (optional) Secret files location if secrets_manager was not specified\n    secrets_url: https://api.datacoves.localhost/service-credentials/airbyte # Secrets url if secrets_manager is datacoves\n    secrets_token: <TOKEN> # Secrets auth token if secrets_manager is datacoves\n  fivetran:\n    path: /config/workspace/load/fivetran # Where previous Fivetran export resides, subject of import\n    api_key: [KEY] # Fivetran API Key\n    api_secret: [SECRET] # Fivetran API Secret\n    secrets_path: /config/workspace/secrets/fivetran # Fivetran secret fields\n    credentials: /opt/fivetran_credentials.yml # Fivetran set of key:secret pairs\n    # \'api_key\' + \'api_secret\' are mutually exclusive with \'credentials\', use one or the other\n```\n\n## Override generation templates\n\nCustomizing generated models and model properties requires placing\ntemplate files under the `.dbt-coves/templates` folder.\n\nThere are different variables available in the templates:\n\n- `adapter_name` refers to the Adapter\'s class name being used by the target, e.g. `SnowflakeAdapter` when using [Snowflake](https://github.com/dbt-labs/dbt-snowflake/blob/21b52127e7d221db8b92114aae066fb8a7151bba/dbt/adapters/snowflake/impl.py#L33).\n- `columns` contains the list of relation columns that don\'t contain nested (JSON) data, it\'s type is `List[Item]`.\n- `nested` contains a dict of nested columns, grouped by column name, it\'s type is `Dict[column_name, Dict[nested_key, Item]]`.\n\n`Item` is a `dict` with the keys `id`, `name`, `type`, and `description`, where `id` contains an slugified id generated from `name`.\n\n### dbt-coves generate sources\n\n#### Source property file (.yml) template\n\nThis file is used to create the sources yml file\n\n[source_props.yml](dbt_coves/templates/source_props.yml)\n\n#### Staging model file (.sql) template\n\nThis file is used to create the staging model (sql) files.\n\n[staging_model.sql](dbt_coves/templates/staging_model.sql)\n\n#### Staging model property file (.yml) template\n\nThis file is used to create the model properties (yml) file\n\n[staging_model_props.yml](dbt_coves/templates/staging_model_props.yml)\n\n### dbt-coves generate properties\n\nThis file is used to create the properties (yml) files for models\n\n[model_props.yml](dbt_coves/templates/model_props.yml)\n\n# Thanks\n\nThe project main structure was inspired by [dbt-sugar](https://github.com/bitpicky/dbt-sugar). Special thanks to [Bastien Boutonnet](https://github.com/bastienboutonnet) for the great work done.\n\n# Authors\n\n- Sebastian Sassi [\\@sebasuy](https://twitter.com/sebasuy) -- [Datacoves](https://datacoves.com/)\n- Noel Gomez [\\@noel_g](https://twitter.com/noel_g) -- [Datacoves](https://datacoves.com/)\n- Bruno Antonellini -- [Datacoves](https://datacoves.com/)\n\n# About\n\nLearn more about [Datacoves](https://datacoves.com).\n\n⚠️ **dbt-coves is still in development, make sure to test it for your dbt project version and DW before using in production and please submit any issues you find. We also welcome any contributions from the community**\n\n# Metrics\n\n[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/datacoves/dbt-coves/graphs/commit-activity)\n[![PyPI version\nfury.io](https://badge.fury.io/py/dbt-coves.svg)](https://pypi.python.org/pypi/dbt-coves/)\n[![Code\nStyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n[![Imports:\nisort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)\n[![Imports:\npython](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue)](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue)\n[![Build](https://github.com/datacoves/dbt-coves/actions/workflows/main_ci.yml/badge.svg)](https://github.com/datacoves/dbt-coves/actions/workflows/main_ci.yml/badge.svg)\n\n<!-- [![codecov](https://codecov.io/gh/datacoves/dbt-coves/branch/main/graph/badge.svg?token=JB0E0LZDW1)](https://codecov.io/gh/datacoves/dbt-coves) -->\n\n[![Maintainability](https://api.codeclimate.com/v1/badges/1e6a887de605ef8e0eca/maintainability)](https://codeclimate.com/github/datacoves/dbt-coves/maintainability)\n[![Downloads](https://pepy.tech/badge/dbt-coves)](https://pepy.tech/project/dbt-coves)\n',
-    'author': 'Datacoves',
-    'author_email': 'hello@datacoves.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://datacoves.com',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.2,<3.11',
+# dbt-coves
+
+## Sponsor
+
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="images/datacoves-dark.png">
+  <img alt="Datacoves" src="images/datacoves-light.png" width="150">
+</picture>
+
+Hosted VS Code, dbt-core, SqlFluff, and Airflow, find out more at [Datacoves.com](https://datacoves.com/product).
+
+## What is dbt-coves?
+
+dbt-coves is a CLI tool that automates certain tasks for [dbt](https://www.getdbt.com), making life simpler for the dbt user.
+
+dbt-coves generates dbt sources, staging models and property(yml) files by analyzing information from the data warehouse and creating the necessary files (sql and yml).
+
+Finally, dbt-coves includes functionality to bootstrap a dbt project and to extract and load configurations from Airbyte.
+
+## Supported dbt versions
+
+| Version | Status           |
+| ------- | ---------------- |
+| \< 1.0  | ❌ Not supported |
+| >= 1.0  | ✅ Tested        |
+
+From `dbt-coves` 1.4.0 onwards, our major and minor versions match those of [dbt-core](https://github.com/dbt-labs/dbt-core).
+This means we release a new major/minor version once it's dbt-core equivalent is tested.
+Patch suffix (1.4.X) is exclusive to our continuous development and does not reflect a version match with dbt
+
+## Supported adapters
+
+| Feature                           | Snowflake | Redshift  | BigQuery  |
+| --------------------------------- | --------- | --------- | --------- |
+| dbt project setup                 | ✅ Tested | ✅ Tested | ✅ Tested |
+| source model (sql) generation     | ✅ Tested | ✅ Tested | ✅ Tested |
+| model properties (yml) generation | ✅ Tested | ✅ Tested | ✅ Tested |
+
+NOTE: Other database adapters may work, although we have not tested them. Feel free to try them and let us know so we can update the table above.
+
+### Here\'s the tool in action
+
+[![image](https://cdn.loom.com/sessions/thumbnails/74062cf71cbe4898805ca508ea2d9455-1624905546029-with-play.gif)](https://www.loom.com/share/74062cf71cbe4898805ca508ea2d9455)
+
+# Installation
+
+```console
+pip install dbt-coves
+```
+
+We recommend using [python
+virtualenvs](https://docs.python.org/3/tutorial/venv.html) and create
+one separate environment per project.
+
+# Command Reference
+
+For a complete list of options, please run:
+
+```console
+dbt-coves -h
+dbt-coves <command> -h
+```
+
+## Environment setup
+
+Setting up your environment can be done in two different ways:
+
+Runs a set of scripts in your local environment to configure your project components: `ssh keys`, `git` and `dbt`
+
+```console
+dbt-coves setup all
+```
+
+You can configure individual components:
+
+Set up `git` repository of dbt-coves project
+
+```console
+dbt-coves setup git
+```
+
+Setup `dbt` within the project (delegates to dbt init)
+
+```console
+dbt-coves setup dbt
+```
+
+Set up SSH Keys for dbt project. Supports the argument `--open_ssl_public_key` which generates an extra Public Key in Open SSL format, useful for configuring certain providers (i.e. Snowflake authentication)
+
+```console
+dbt-coves setup ssh
+```
+
+## Models generation
+
+```console
+dbt-coves generate <resource>
+```
+
+Where _\<resource\>_ could be _sources_, _properties_ or _metadata_.
+
+```console
+dbt-coves generate sources
+```
+
+This command will generate the dbt source configuration as well as the initial dbt staging model(s). It will look in the database defined in your `profiles.yml` file or you can pass the `--database` argument or set up default configuration options (see below)
+
+```console
+dbt-coves generate sources --database raw
+```
+
+Supports Jinja templates to adjust how the resources are generated. See below for examples.
+
+Every `dbt-coves generate <resource>` supports `--no-prompt` flag, which will silently generate all sources/models/properties/metadata without asking anything to the user.
+
+### Source Generation Arguments
+
+dbt-coves can be used to create the initial staging models. It will do the following:
+
+1. Create / Update the source yml file
+2. Create the initial staging model(sql) file and offer to flatten VARIANT(JSON) fields
+3. Create the staging model's property(yml) file.
+
+`dbt-coves generate sources` supports the following args:
+
+See full list in help
+
+```console
+dbt-coves generate sources -h
+```
+
+```console
+--database
+# Database to inspect
+```
+
+```console
+--schemas
+# Schema(s) to inspect. Accepts wildcards (must be enclosed in quotes if used)
+```
+
+```console
+--select-relations
+# List of relations where raw data resides. The parameter must be enclosed in quotes. Accepts wildcards.
+```
+
+```console
+--exclude-relations
+# Filter relation(s) to exclude from source file(s) generation. The parameter must be enclosed in quotes. Accepts wildcards.
+```
+
+```console
+--sources-destination
+# Where sources yml files will be generated, default: 'models/staging/{{schema}}/sources.yml'
+```
+
+```console
+--models-destination
+# Where models sql files will be generated, default: 'models/staging/{{schema}}/{{relation}}.sql'
+```
+
+```console
+--model-props-destination
+# Where models yml files will be generated, default: 'models/staging/{{schema}}/{{relation}}.yml'
+```
+
+```console
+--update-strategy
+# Action to perform when a property file already exists: 'update', 'recreate', 'fail', 'ask' (per file)
+```
+
+```console
+--templates-folder
+# Folder with jinja templates that override default sources generation templates, i.e. 'templates'
+```
+
+```console
+--metadata
+# Path to csv file containing metadata, i.e. 'metadata.csv'
+```
+
+```console
+--no-prompt
+# Silently generate source dbt models
+```
+
+### Properties Generation Arguments
+
+You can use dbt-coves to generate and update the properties(yml) file for a given dbt model(sql) file.
+
+`dbt-coves generate properties` supports the following args:
+
+```console
+--destination
+# Where models yml files will be generated, default: '{{model_folder_path}}/{{model_file_name}}.yml'
+```
+
+```console
+--update-strategy
+# Action to perform when a property file already exists: 'update', 'recreate', 'fail', 'ask' (per file)
+```
+
+```console
+-s --select
+# Filter model(s) to generate property file(s)
+```
+
+```console
+--exclude
+# Filter model(s) to exclude from property file(s) generation
+```
+
+```console
+--selector
+# Specify dbt selector for more complex model filtering
+```
+
+```console
+--templates-folder
+# Folder with jinja templates that override default properties generation templates, i.e. 'templates'
+```
+
+```console
+--metadata
+# Path to csv file containing metadata, i.e. 'metadata.csv'
+```
+
+```console
+--no-prompt
+# Silently generate dbt models property files
+```
+
+Note: `--select (or -s)`, `--exclude` and `--selector` work exactly as `dbt ls` selectors do. For usage details, visit [dbt list docs](https://docs.getdbt.com/reference/commands/list)
+
+### Metadata Generation Arguments
+
+You can use dbt-coves to generate the metadata file(s) containing the basic structure of the csv that can be used in the above `dbt-coves generate sources/properties` commands.
+Usage of these metadata files can be found in [metadata](https://github.com/datacoves/dbt-coves#metadata) below.
+
+`dbt-coves generate metadata` supports the following args:
+
+```console
+--database
+# Database to inspect
+```
+
+```console
+--schemas
+# Schema(s) to inspect. Accepts wildcards (must be enclosed in quotes if used)
+```
+
+```console
+--select-relations
+# List of relations where raw data resides. The parameter must be enclosed in quotes. Accepts wildcards.
+```
+
+```console
+--exclude-relations
+# Filter relation(s) to exclude from source file(s) generation. The parameter must be enclosed in quotes. Accepts wildcards.
+```
+
+```console
+--destination
+# Where csv file(s) will be generated, default: 'metadata.csv'
+# Supports using the Jinja tags `{{relation}}` and `{{schema}}`
+# if creating one csv per relation/table in schema, i.e: "metadata/{{relation}}.csv"
+```
+
+```console
+--no-prompt
+# Silently generate metadata
+```
+
+### Metadata
+
+dbt-coves supports the argument `--metadata` which allows users to specify a csv file containing field types and descriptions to be used when creating the staging models and property files.
+
+```console
+dbt-coves generate sources --metadata metadata.csv
+```
+
+Metadata format:
+You can download a [sample csv file](sample_metadata.csv) as reference
+
+| database | schema | relation                          | column          | key  | type    | description                                     |
+| -------- | ------ | --------------------------------- | --------------- | ---- | ------- | ----------------------------------------------- |
+| raw      | raw    | \_airbyte_raw_country_populations | \_airbyte_data  | Year | integer | Year of country population measurement          |
+| raw      | raw    | \_airbyte_raw_country_populations | \_airbyte_data  |      | variant | Airbyte data columns (VARIANT) in Snowflake     |
+| raw      | raw    | \_airbyte_raw_country_populations | \_airbyte_ab_id |      | varchar | Airbyte unique identifier used during data load |
+
+## Extract configuration from Airbyte
+
+```console
+dbt-coves extract airbyte
+```
+
+Extracts the configuration from your Airbyte sources, connections and destinations (excluding credentials) and stores it in the specified folder. The main goal of this feature is to keep track of the configuration changes in your git repo, and rollback to a specific version when needed.
+
+Full usage example:
+
+```console
+dbt-coves extract airbyte --host http://airbyte-server --port 8001 --path /config/workspace/load/airbyte
+```
+
+## Load configuration to Airbyte
+
+```console
+dbt-coves load airbyte
+```
+
+Loads the Airbyte configuration generated with `dbt-coves extract airbyte` on an Airbyte server. Secrets folder needs to be specified separately. You can use [git-secret](https://git-secret.io/) to encrypt secrets and make them part of your git repo.
+
+### Loading secrets
+
+Secret credentials can be approached in two different ways: locally or remotely (through a provider/manager).
+
+In order to load encrypted fields locally:
+
+```console
+dbt-coves load airbyte --secrets-path /path/to/secret/directory
+
+# This directory must have 'sources', 'destinations' and 'connections' folders nested inside, and inside them the respective JSON files with unencrypted fields.
+# Naming convention: JSON unencrypted secret files must be named exactly as the extracted ones.
+```
+
+To load encrypted fields through a manager (in this case we are connecting to Datacoves' Service Credentials):
+
+```console
+--secrets-manager datacoves
+```
+
+```console
+--secrets-url https://api.datacoves.localhost/service-credentials/airbyte
+```
+
+```console
+--secrets-token <secret token>
+```
+
+Full usage example:
+
+```console
+dbt-coves load airbyte --host http://airbyte-server --port 8001 --path /config/workspace/load/airbyte --secrets-path /config/workspace/secrets
+```
+
+## Extract configuration from Fivetran
+
+```console
+dbt-coves extract fivetran
+```
+
+Extracts the configuration from your Fivetran destinations and connectors (excluding credentials) and stores it in the specified folder. The main goal of this feature is to keep track of the configuration changes in your git repo, and rollback to a specific version when needed.
+
+Full usage example:
+
+```console
+dbt-coves extract fivetran --credentials /config/workspace/secrets/fivetran/credentials.yml --path /config/workspace/load/fivetran
+```
+
+## Load configuration to Fivetran
+
+```console
+dbt-coves load fivetran
+```
+
+Loads the Fivetran configuration generated with `dbt-coves extract fivetran` on a Fivetran instance. Secrets folder needs to be specified separately. You can use [git-secret](https://git-secret.io/) to encrypt secrets and make them part of your git repo.
+
+### Credentials
+
+In order for extract/load fivetran to work properly, you need to provide an api key-secret pair (you can generate them [here](https://fivetran.com/account/settings/account)).
+
+These credentials can be used with `--api-key [key] --api-secret [secret]`, or specyfing a YML file with `--credentials /path/to/credentials.yml`. The required structure of this file is the following:
+
+```yaml
+account_name: # Any name, used by dbt-coves to ask which to use when more than one is found
+  api_key: [key]
+  api_secret: [secret]
+account_name_2:
+  api_key: [key]
+  api_secret: [secret]
+```
+
+This YML file approach allows you to both work with multiple Fivetran accounts, and treat this credentials file as a secret.
+
+> :warning: **Warning**: --api-key/secret and --credentials flags are mutually exclusive, don't use them together.
+
+### Loading secrets
+
+Secret credentials can be approached via `--secrets-path` flag
+
+```console
+dbt-coves load fivetran --secrets-path /path/to/secret/directory
+```
+
+#### Field naming convention
+
+Although secret files can have any name, unencrypted JSON files must follow a simple structure:
+
+- Keys should match their corresponding Fivetran destination ID: two words automatically generated by Fivetran, which can be found in previously extracted data.
+- Inside those keys, a nested dictionary of which fields should be overwritten
+
+For example:
+
+```json
+{
+  "extract_muscle": {
+    // Internal ID that Fivetran gave to a Snowflake warehouse Destination
+    "password": "[PASSWORD]" // Field:Value pair
+  },
+  "centre_straighten": {
+    "password": "[PASSWORD]"
+  }
 }
+```
+
+## Run dbt commands
+
+```shell
+dbt-coves dbt <arguments> -- <command>
+```
+
+Run dbt commands on special environments such as Airflow, or CI workers, with the possibility of changing dbt project location and activating a specific virtual environment in which running commands.
+
+### Arguments
+
+`dbt-coves dbt` supports the following arguments
+
+```shell
+--project-dir
+# Path of the dbt project where command will be executed, i.e.: /opt/user/dbt_project
+```
+
+```shell
+--virtualenv
+# Virtual environment path. i.e.: /opt/user/virtualenvs/airflow
+```
+
+### Sample usage
+
+```shell
+dbt-coves dbt --project-dir /opt/user/dbt_project --virtualenv /opt/user/virtualenvs/airflow -- run -s model --vars \"{key: value}\"
+# Make sure to escape special characters such as quotation marks
+# Double dash (--) between <arguments> and <command> are mandatory
+```
+
+# Settings
+
+dbt-coves will read settings from `.dbt_coves/config.yml`. A standard settings files could look like
+this:
+
+```yaml
+generate:
+  sources:
+    database: "RAW" # Database where to look for source tables
+    schemas: # List of schema names where to look for source tables
+      - RAW
+    select_relations: # list of relations where raw data resides
+      - TABLE_1
+      - TABLE_2
+    exclude_relations: # Filter relation(s) to exclude from source file(s) generation
+      - TABLE_1
+      - TABLE_2
+    sources_destination: "models/staging/{{schema}}/{{schema}}.yml" # Where sources yml files will be generated
+    models_destination: "models/staging/{{schema}}/{{relation}}.sql" # Where models sql files will be generated
+    model_props_destination: "models/staging/{{schema}}/{{relation}}.yml" # Where models yml files will be generated
+    update_strategy: ask # Action to perform when a property file already exists. Options: update, recreate, fail, ask (per file)
+    templates_folder: ".dbt_coves/templates" # Folder where source generation jinja templates are located. Override default templates creating  source_props.yml, source_model_props.yml, and source_model.sql under this folder
+    metadata: "metadata.csv" # Path to csv file containing metadata
+
+  properties:
+    destination: "{{model_folder_path}}/{{model_file_name}}.yml" # Where models yml files will be generated
+    # You can specify a different path by declaring it explicitly, i.e.: "models/staging/{{model_file_name}}.yml"
+    update-strategy: ask # Action to perform when a property file already exists. Options: update, recreate, fail, ask (per file)
+    select: "models/staging/bays" # Filter model(s) to generate property file(s)
+    exclude: "models/staging/bays/test_bay" # Filter model(s) to generate property file(s)
+    selector: "selectors/bay_selector.yml" # Specify dbt selector for more complex model filtering
+    templates_folder: ".dbt_coves/templates" # Folder where source generation jinja templates are located. Override default template creating model_props.yml under this folder
+    metadata: "metadata.csv" # Path to csv file containing metadata
+
+  metadata:
+    database: RAW # Database where to look for source tables
+    schemas: # List of schema names where to look for source tables
+      - RAW
+    select_relations: # list of relations where raw data resides
+      - TABLE_1
+      - TABLE_2
+    exclude_relations: # Filter relation(s) to exclude from source file(s) generation
+      - TABLE_1
+      - TABLE_2
+    destination: # Where metadata file will be generated, default: 'metadata.csv'
+
+extract:
+  airbyte:
+    path: /config/workspace/load/airbyte # Where json files will be generated
+    host: http://airbyte-server # Airbyte's API hostname
+    port: 8001 # Airbyte's API port
+  fivetran:
+    path: /config/workspace/load/fivetran # Where Fivetran export will be generated
+    api_key: [KEY] # Fivetran API Key
+    api_secret: [SECRET] # Fivetran API Secret
+    credentials: /opt/fivetran_credentials.yml # Fivetran set of key:secret pairs
+    # 'api_key' + 'api_secret' are mutually exclusive with 'credentials', use one or the other
+
+load:
+  airbyte:
+    path: /config/workspace/load
+    host: http://airbyte-server
+    port: 8001
+    secrets_manager: datacoves # (optional) Secret credentials provider (secrets_path OR secrets_manager should be used, can't load secrets locally and remotely at the same time)
+    secrets_path: /config/workspace/secrets # (optional) Secret files location if secrets_manager was not specified
+    secrets_url: https://api.datacoves.localhost/service-credentials/airbyte # Secrets url if secrets_manager is datacoves
+    secrets_token: <TOKEN> # Secrets auth token if secrets_manager is datacoves
+  fivetran:
+    path: /config/workspace/load/fivetran # Where previous Fivetran export resides, subject of import
+    api_key: [KEY] # Fivetran API Key
+    api_secret: [SECRET] # Fivetran API Secret
+    secrets_path: /config/workspace/secrets/fivetran # Fivetran secret fields
+    credentials: /opt/fivetran_credentials.yml # Fivetran set of key:secret pairs
+    # 'api_key' + 'api_secret' are mutually exclusive with 'credentials', use one or the other
+```
+
+## Override generation templates
+
+Customizing generated models and model properties requires placing
+template files under the `.dbt-coves/templates` folder.
+
+There are different variables available in the templates:
+
+- `adapter_name` refers to the Adapter's class name being used by the target, e.g. `SnowflakeAdapter` when using [Snowflake](https://github.com/dbt-labs/dbt-snowflake/blob/21b52127e7d221db8b92114aae066fb8a7151bba/dbt/adapters/snowflake/impl.py#L33).
+- `columns` contains the list of relation columns that don't contain nested (JSON) data, it's type is `List[Item]`.
+- `nested` contains a dict of nested columns, grouped by column name, it's type is `Dict[column_name, Dict[nested_key, Item]]`.
+
+`Item` is a `dict` with the keys `id`, `name`, `type`, and `description`, where `id` contains an slugified id generated from `name`.
+
+### dbt-coves generate sources
+
+#### Source property file (.yml) template
+
+This file is used to create the sources yml file
+
+[source_props.yml](dbt_coves/templates/source_props.yml)
+
+#### Staging model file (.sql) template
+
+This file is used to create the staging model (sql) files.
+
+[staging_model.sql](dbt_coves/templates/staging_model.sql)
+
+#### Staging model property file (.yml) template
+
+This file is used to create the model properties (yml) file
+
+[staging_model_props.yml](dbt_coves/templates/staging_model_props.yml)
+
+### dbt-coves generate properties
+
+This file is used to create the properties (yml) files for models
+
+[model_props.yml](dbt_coves/templates/model_props.yml)
+
+# Thanks
+
+The project main structure was inspired by [dbt-sugar](https://github.com/bitpicky/dbt-sugar). Special thanks to [Bastien Boutonnet](https://github.com/bastienboutonnet) for the great work done.
+
+# Authors
+
+- Sebastian Sassi [\@sebasuy](https://twitter.com/sebasuy) -- [Datacoves](https://datacoves.com/)
+- Noel Gomez [\@noel_g](https://twitter.com/noel_g) -- [Datacoves](https://datacoves.com/)
+- Bruno Antonellini -- [Datacoves](https://datacoves.com/)
+
+# About
+
+Learn more about [Datacoves](https://datacoves.com).
+
+⚠️ **dbt-coves is still in development, make sure to test it for your dbt project version and DW before using in production and please submit any issues you find. We also welcome any contributions from the community**
+
+# Metrics
+
+[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/datacoves/dbt-coves/graphs/commit-activity)
+[![PyPI version
+fury.io](https://badge.fury.io/py/dbt-coves.svg)](https://pypi.python.org/pypi/dbt-coves/)
+[![Code
+Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+[![Imports:
+isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Imports:
+python](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue)](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue)
+[![Build](https://github.com/datacoves/dbt-coves/actions/workflows/main_ci.yml/badge.svg)](https://github.com/datacoves/dbt-coves/actions/workflows/main_ci.yml/badge.svg)
+
+<!-- [![codecov](https://codecov.io/gh/datacoves/dbt-coves/branch/main/graph/badge.svg?token=JB0E0LZDW1)](https://codecov.io/gh/datacoves/dbt-coves) -->
 
+[![Maintainability](https://api.codeclimate.com/v1/badges/1e6a887de605ef8e0eca/maintainability)](https://codeclimate.com/github/datacoves/dbt-coves/maintainability)
+[![Downloads](https://pepy.tech/badge/dbt-coves)](https://pepy.tech/project/dbt-coves)
 
-setup(**setup_kwargs)
```

