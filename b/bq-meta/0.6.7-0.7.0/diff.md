# Comparing `tmp/bq-meta-0.6.7.tar.gz` & `tmp/bq-meta-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bq-meta-0.6.7.tar", last modified: Tue Jan 31 18:56:04 2023, max compression
+gzip compressed data, was "bq-meta-0.7.0.tar", last modified: Fri May 19 17:46:19 2023, max compression
```

## Comparing `bq-meta-0.6.7.tar` & `bq-meta-0.7.0.tar`

### file list

```diff
@@ -1,37 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 18:56:04.293376 bq-meta-0.6.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-01-31 18:55:53.000000 bq-meta-0.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-01-31 18:56:04.293376 bq-meta-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-01-31 18:55:53.000000 bq-meta-0.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 18:56:04.289376 bq-meta-0.6.7/bq_meta/
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-01-31 18:55:53.000000 bq-meta-0.6.7/bq_meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-31 18:55:53.000000 bq-meta-0.6.7/bq_meta/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-01-31 18:55:53.000000 bq-meta-0.6.7/bq_meta/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-01-31 18:55:53.000000 bq-meta-0.6.7/bq_meta/bq_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-01-31 18:55:53.000000 bq-meta-0.6.7/bq_meta/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-01-31 18:55:53.000000 bq-meta-0.6.7/bq_meta/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-01-31 18:55:53.000000 bq-meta-0.6.7/bq_meta/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-01-31 18:55:53.000000 bq-meta-0.6.7/bq_meta/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-01-31 18:55:53.000000 bq-meta-0.6.7/bq_meta/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 18:56:04.293376 bq-meta-0.6.7/bq_meta/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 18:55:53.000000 bq-meta-0.6.7/bq_meta/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-01-31 18:55:53.000000 bq-meta-0.6.7/bq_meta/service/history_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-01-31 18:55:53.000000 bq-meta-0.6.7/bq_meta/service/project_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-01-31 18:55:53.000000 bq-meta-0.6.7/bq_meta/service/table_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-01-31 18:55:53.000000 bq-meta-0.6.7/bq_meta/service/template_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-01-31 18:55:53.000000 bq-meta-0.6.7/bq_meta/service/version_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 18:56:04.293376 bq-meta-0.6.7/bq_meta/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 18:55:53.000000 bq-meta-0.6.7/bq_meta/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-01-31 18:55:53.000000 bq-meta-0.6.7/bq_meta/util/bash_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-01-31 18:55:53.000000 bq-meta-0.6.7/bq_meta/util/num_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-01-31 18:55:53.000000 bq-meta-0.6.7/bq_meta/util/rich_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-01-31 18:55:53.000000 bq-meta-0.6.7/bq_meta/util/table_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-01-31 18:55:53.000000 bq-meta-0.6.7/bq_meta/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 18:56:04.289376 bq-meta-0.6.7/bq_meta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-01-31 18:56:04.000000 bq-meta-0.6.7/bq_meta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-01-31 18:56:04.000000 bq-meta-0.6.7/bq_meta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 18:56:04.000000 bq-meta-0.6.7/bq_meta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-31 18:56:04.000000 bq-meta-0.6.7/bq_meta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-31 18:56:04.000000 bq-meta-0.6.7/bq_meta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-31 18:56:04.000000 bq-meta-0.6.7/bq_meta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-01-31 18:55:53.000000 bq-meta-0.6.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-01-31 18:56:04.293376 bq-meta-0.6.7/setup.cfg
+drwxr-xr-x   0 pie        (502) staff       (20)        0 2023-05-19 17:46:19.869340 bq-meta-0.7.0/
+-rw-r--r--   0 pie        (502) staff       (20)    11340 2021-12-24 17:21:28.000000 bq-meta-0.7.0/LICENSE
+-rw-r--r--   0 pie        (502) staff       (20)       22 2023-05-19 17:39:54.000000 bq-meta-0.7.0/MANIFEST.in
+-rw-r--r--   0 pie        (502) staff       (20)     2861 2023-05-19 17:46:19.869428 bq-meta-0.7.0/PKG-INFO
+-rw-r--r--   0 pie        (502) staff       (20)     2307 2023-01-31 18:54:42.000000 bq-meta-0.7.0/README.md
+drwxr-xr-x   0 pie        (502) staff       (20)        0 2023-05-19 17:46:19.864492 bq-meta-0.7.0/bq_meta/
+-rw-r--r--   0 pie        (502) staff       (20)     2246 2022-07-26 16:17:15.000000 bq-meta-0.7.0/bq_meta/__init__.py
+-rw-r--r--   0 pie        (502) staff       (20)       66 2022-07-26 16:16:45.000000 bq-meta-0.7.0/bq_meta/__main__.py
+-rw-r--r--   0 pie        (502) staff       (20)     2354 2022-07-24 16:36:09.000000 bq-meta-0.7.0/bq_meta/auth.py
+-rw-r--r--   0 pie        (502) staff       (20)     2979 2023-05-19 17:39:54.000000 bq-meta-0.7.0/bq_meta/cli.py
+-rw-r--r--   0 pie        (502) staff       (20)      767 2023-05-19 17:39:54.000000 bq-meta-0.7.0/bq_meta/client.py
+-rw-r--r--   0 pie        (502) staff       (20)     2572 2022-09-11 07:24:49.000000 bq-meta-0.7.0/bq_meta/config.py
+-rw-r--r--   0 pie        (502) staff       (20)     2138 2023-05-19 17:39:54.000000 bq-meta-0.7.0/bq_meta/const.py
+-rw-r--r--   0 pie        (502) staff       (20)     2189 2023-05-19 17:39:54.000000 bq-meta-0.7.0/bq_meta/initialize.py
+-rw-r--r--   0 pie        (502) staff       (20)     8421 2023-05-19 17:40:01.000000 bq-meta-0.7.0/bq_meta/output.py
+drwxr-xr-x   0 pie        (502) staff       (20)        0 2023-05-19 17:46:19.866825 bq-meta-0.7.0/bq_meta/service/
+-rw-r--r--   0 pie        (502) staff       (20)        0 2022-07-27 07:58:04.000000 bq-meta-0.7.0/bq_meta/service/__init__.py
+-rw-r--r--   0 pie        (502) staff       (20)     1559 2023-05-19 17:39:54.000000 bq-meta-0.7.0/bq_meta/service/history_service.py
+-rw-r--r--   0 pie        (502) staff       (20)      992 2023-05-19 17:39:54.000000 bq-meta-0.7.0/bq_meta/service/project_service.py
+-rw-r--r--   0 pie        (502) staff       (20)      760 2023-05-19 17:39:54.000000 bq-meta-0.7.0/bq_meta/service/snippet_service.py
+-rw-r--r--   0 pie        (502) staff       (20)     2502 2023-05-19 17:39:54.000000 bq-meta-0.7.0/bq_meta/service/table_service.py
+-rw-r--r--   0 pie        (502) staff       (20)      852 2022-10-12 07:08:51.000000 bq-meta-0.7.0/bq_meta/service/version_service.py
+drwxr-xr-x   0 pie        (502) staff       (20)        0 2023-05-19 17:46:19.868174 bq-meta-0.7.0/bq_meta/snippets/
+-rw-r--r--   0 pie        (502) staff       (20)       95 2023-05-19 17:39:54.000000 bq-meta-0.7.0/bq_meta/snippets/dataset_size
+-rw-r--r--   0 pie        (502) staff       (20)      156 2023-05-19 17:39:54.000000 bq-meta-0.7.0/bq_meta/snippets/duplicate_count
+-rw-r--r--   0 pie        (502) staff       (20)      147 2023-05-19 17:39:54.000000 bq-meta-0.7.0/bq_meta/snippets/duplicate_rows
+-rw-r--r--   0 pie        (502) staff       (20)      324 2023-05-19 17:39:54.000000 bq-meta-0.7.0/bq_meta/snippets/month_size
+-rw-r--r--   0 pie        (502) staff       (20)      269 2023-05-19 17:39:54.000000 bq-meta-0.7.0/bq_meta/snippets/partition_size
+-rw-r--r--   0 pie        (502) staff       (20)       98 2023-05-19 17:39:54.000000 bq-meta-0.7.0/bq_meta/snippets/table_ddl
+drwxr-xr-x   0 pie        (502) staff       (20)        0 2023-05-19 17:46:19.869182 bq-meta-0.7.0/bq_meta/util/
+-rw-r--r--   0 pie        (502) staff       (20)        0 2022-07-27 07:58:16.000000 bq-meta-0.7.0/bq_meta/util/__init__.py
+-rw-r--r--   0 pie        (502) staff       (20)     1084 2022-07-28 20:39:16.000000 bq-meta-0.7.0/bq_meta/util/bash_util.py
+-rw-r--r--   0 pie        (502) staff       (20)      474 2023-01-29 20:27:09.000000 bq-meta-0.7.0/bq_meta/util/num_utils.py
+-rw-r--r--   0 pie        (502) staff       (20)     1201 2022-07-29 09:05:26.000000 bq-meta-0.7.0/bq_meta/util/rich_utils.py
+-rw-r--r--   0 pie        (502) staff       (20)      772 2022-07-28 21:05:28.000000 bq-meta-0.7.0/bq_meta/util/table_utils.py
+-rw-r--r--   0 pie        (502) staff       (20)     7810 2023-05-19 17:39:54.000000 bq-meta-0.7.0/bq_meta/window.py
+drwxr-xr-x   0 pie        (502) staff       (20)        0 2023-05-19 17:46:19.865391 bq-meta-0.7.0/bq_meta.egg-info/
+-rw-r--r--   0 pie        (502) staff       (20)     2861 2023-05-19 17:46:19.000000 bq-meta-0.7.0/bq_meta.egg-info/PKG-INFO
+-rw-r--r--   0 pie        (502) staff       (20)      939 2023-05-19 17:46:19.000000 bq-meta-0.7.0/bq_meta.egg-info/SOURCES.txt
+-rw-r--r--   0 pie        (502) staff       (20)        1 2023-05-19 17:46:19.000000 bq-meta-0.7.0/bq_meta.egg-info/dependency_links.txt
+-rw-r--r--   0 pie        (502) staff       (20)       44 2023-05-19 17:46:19.000000 bq-meta-0.7.0/bq_meta.egg-info/entry_points.txt
+-rw-r--r--   0 pie        (502) staff       (20)       87 2023-05-19 17:46:19.000000 bq-meta-0.7.0/bq_meta.egg-info/requires.txt
+-rw-r--r--   0 pie        (502) staff       (20)        8 2023-05-19 17:46:19.000000 bq-meta-0.7.0/bq_meta.egg-info/top_level.txt
+-rw-r--r--   0 pie        (502) staff       (20)      126 2021-12-30 16:55:35.000000 bq-meta-0.7.0/pyproject.toml
+-rw-r--r--   0 pie        (502) staff       (20)      829 2023-05-19 17:46:19.869792 bq-meta-0.7.0/setup.cfg
```

### Comparing `bq-meta-0.6.7/LICENSE` & `bq-meta-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bq-meta-0.6.7/PKG-INFO` & `bq-meta-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bq-meta
-Version: 0.6.7
+Version: 0.7.0
 Summary: BigQuery metadata
 Home-page: https://github.com/martintupy/bq-meta
 Author: Martin Tupy
 Author-email: id@martintupy.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bq-meta-0.6.7/README.md` & `bq-meta-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `bq-meta-0.6.7/bq_meta/__init__.py` & `bq-meta-0.7.0/bq_meta/__init__.py`

 * *Files identical despite different names*

### Comparing `bq-meta-0.6.7/bq_meta/auth.py` & `bq-meta-0.7.0/bq_meta/auth.py`

 * *Files identical despite different names*

### Comparing `bq-meta-0.6.7/bq_meta/cli.py` & `bq-meta-0.7.0/bq_meta/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 import click
 from rich.console import Console
 from rich.panel import Panel
 from rich.text import Text
 from google.cloud.bigquery.table import TableReference
 
 from bq_meta import const, output
-from bq_meta.bq_client import BqClient
+from bq_meta.client import Client
 from bq_meta.config import Config
 from bq_meta.initialize import initialize
 from bq_meta.service.history_service import HistoryService
 from bq_meta.service.project_service import ProjectService
 from bq_meta.service.table_service import TableService
-from bq_meta.service.template_service import TemplateService
+from bq_meta.service.snippet_service import SnippetService
 from bq_meta.service.version_service import VersionService
 from bq_meta.util import table_utils
 from bq_meta.window import Window
 
 
 @click.command()
 @click.argument("full_table_id", required=False)
@@ -35,20 +35,20 @@
     fetch_projects: bool,
 ):
     """BiqQuery metadata"""
 
     ctx = click.get_current_context()
     console = Console(theme=const.theme, soft_wrap=True, force_interactive=True)
     config = Config()
-    bq_client = BqClient(console, config)
-    project_service = ProjectService(console, config, bq_client)
-    table_service = TableService(console, config, bq_client, project_service)
-    template_service = TemplateService()
+    client = Client(console, config)
+    project_service = ProjectService(console, config, client)
+    table_service = TableService(console, config, client, project_service)
+    snippet_service = SnippetService()
     history_service = HistoryService(console, config, table_service)
-    window = Window(console, config, history_service, table_service, template_service)
+    window = Window(console, config, history_service, table_service, snippet_service)
     table = None
     
     if os.path.exists(const.BQ_META_HOME):
         version_service = VersionService()
         version_service.update_config(config)
 
     if init:
```

### Comparing `bq-meta-0.6.7/bq_meta/config.py` & `bq-meta-0.7.0/bq_meta/config.py`

 * *Files identical despite different names*

### Comparing `bq-meta-0.6.7/bq_meta/const.py` & `bq-meta-0.7.0/bq_meta/const.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 DEFAULT_BQ_META_HOME = f"{Path.home()}/.config/bq-meta"
 
 BQ_META_HOME = os.getenv("BQ_META_HOME", DEFAULT_BQ_META_HOME)
 BQ_META_CONFIG = f"{BQ_META_HOME}/config.yaml"
 BQ_META_PROJECTS = f"{BQ_META_HOME}/projects"
 BQ_META_HISTORY = f"{BQ_META_HOME}/history"
-BQ_META_TEMPLATES = f"{BQ_META_HOME}/templates"
+BQ_META_SNIPPETS = f"{BQ_META_HOME}/snippets"
 
 BQ_META_DISABLE_COLORS = os.getenv("BQ_META_DISABLE_COLORS", "False").lower() in ("true", "1", "t")
 BQ_META_SKIN = os.getenv("BQ_META_SKIN")
 
 default_skin = {
     "request": "gold3",
     "info": "green",
```

### Comparing `bq-meta-0.6.7/bq_meta/initialize.py` & `bq-meta-0.7.0/bq_meta/initialize.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+import bq_meta
+
 from pathlib import Path
 
 from rich.console import Console, Group, NewLine
 from rich.panel import Panel
 from rich.prompt import Prompt
 from rich.text import Text
 
 from bq_meta import const
 from bq_meta.auth import Auth
 from bq_meta.config import Config
 from bq_meta.service.project_service import ProjectService
+from distutils.dir_util import copy_tree
 
 
 def initialize(config: Config, console: Console, project_service: ProjectService):
     bq_meta_home = Prompt.ask(
         Text("", style=const.darker_style).append("Enter bq_meta home path", style=const.request_style),
         default=const.DEFAULT_BQ_META_HOME,
         console=console,
@@ -23,14 +26,18 @@
     Path(const.BQ_META_CONFIG).touch()
     config.write_default()
     _print_created(console, const.BQ_META_CONFIG)
     Path(const.BQ_META_PROJECTS).touch()
     _print_created(console, const.BQ_META_PROJECTS)
     Path(const.BQ_META_HISTORY).touch()
     _print_created(console, const.BQ_META_HISTORY)
+    Path(const.BQ_META_SNIPPETS).mkdir(parents=True, exist_ok=True)
+    _print_created(console, const.BQ_META_SNIPPETS)
+    Path(bq_meta.__file__).resolve().parent
+    copy_tree(Path(bq_meta.__file__).resolve().parent / "snippets", const.BQ_META_SNIPPETS)
 
     Prompt.ask(
         Text("", style=const.darker_style).append("Login to google account", style=const.request_style),
         choices=None,
         default="Press enter",
         console=console,
     )
```

### Comparing `bq-meta-0.6.7/bq_meta/output.py` & `bq-meta-0.7.0/bq_meta/output.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from typing import List, Optional
+
 from google.cloud import bigquery
 from packaging import version
 from rich.align import Align
 from rich.box import SIMPLE
 from rich.columns import Columns
 from rich.console import Group, NewLine, RenderableType
 from rich.layout import Layout
 from rich.panel import Panel
 from rich.rule import Rule
+from rich.syntax import Syntax
 from rich.table import Table
 from rich.text import Text
 from rich.tree import Tree
-from rich.syntax import Syntax
+
 from bq_meta import const
 from bq_meta.config import Config
 from bq_meta.util import table_utils
 from bq_meta.util.num_utils import bytes_fmt, num_fmt
 from bq_meta.window import Hint
 
 title = """
@@ -67,22 +69,29 @@
     if renderable:
         content = Panel(renderable, border_style=const.darker_style)
     else:
         content = Panel(NewLine(), border_style=const.darker_style)
     return Layout(content, name="content")
 
 
-def hints_layout(hints: List[Hint]) -> Layout:
+def hints_layout(hints: List[Hint], bottom_hints: List[Hint]) -> Layout:
+    hints_layout = Layout(name="hints")
     separator = Rule(style=const.darker_style)
     hints_list = []
     for hint in hints:
         text = Text(f"{hint.name} ({hint.key})", style="default")
         hints_list.extend([text, separator])
-    panel = Panel(Group(*hints_list), box=const.box_left_rounded, style=const.darker_style)
-    return Layout(panel, size=30)
+    top = Layout(Group(*hints_list))
+    bottom_hints_list = []
+    for bottom_hint in bottom_hints:
+        text = Text(f"{bottom_hint.name} ({bottom_hint.key})", style="default")
+        bottom_hints_list.extend([separator, text])
+    bottom = Layout(Align(Group(*bottom_hints_list, fit=False), vertical="bottom"))
+    hints_layout.split_column(top, bottom)
+    return Layout(Panel(hints_layout, box=const.box_left_rounded, style=const.darker_style), size=30)
 
 
 def get_config_info(config: Config) -> Group:
     return Group(text_tuple("Account", config.account))
 
 
 def get_schema_output(table: bigquery.Table) -> Group:
@@ -90,17 +99,17 @@
     tree = Tree(Text(table.full_table_id, const.key_style))
     table = Table(box=SIMPLE, show_header=False)
     table_utils.scheme_tree(schema, tree)
     table_utils.scheme_table(schema, table)
     return Group(Rule("Schema", style=const.darker_style), Columns([tree, table]))
 
 
-def get_template_output(template: str) -> Group:
-    syntax = Syntax(template, lexer="SqlJinjaLexer", line_numbers=True)
-    return Group(Rule("Rendered template", style=const.darker_style), syntax)
+def get_snippet_output(snippet: str) -> Group:
+    syntax = Syntax(snippet, lexer="SqlLexer", line_numbers=True, theme="ansi_dark")
+    return Group(Rule("Snippet", style=const.darker_style), syntax)
 
 
 # fmt: off
 def get_table_output(table: bigquery.Table) -> Group:
     total_logical_bytes = bytes_fmt(int(table._properties.get("numTotalLogicalBytes", 0)))
     active_logical_bytes = bytes_fmt(int(table._properties.get("numActiveLogicalBytes", 0)))
     long_term_logical_bytes = bytes_fmt(int(table._properties.get("numLongTermLogicalBytes", 0)))
@@ -129,14 +138,15 @@
             "Table ID": table.full_table_id,
             "Friendly name": table.friendly_name,
             "Created": created,
             "Last modified": modified,
             "Table expiry": expiry,
             "Data location": table.location,
             "Data location": table.location,
+            "Description": table.description,
         }),
         Rule(style=const.darker_style),
         table_tuple({
             "Table type": table.table_type,
             "Partitioned by": partitioned_by,
             "Partitioned on field": partitioned_field,
             "Partition expiry": table.partition_expiration,
```

### Comparing `bq-meta-0.6.7/bq_meta/service/history_service.py` & `bq-meta-0.7.0/bq_meta/service/history_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 class HistoryService:
     def __init__(self, console: Console, config: Config, table_service: TableService) -> None:
         self.console = console
         self.config = config
         self.table_service = table_service
         self.history_path = const.BQ_META_HISTORY
 
-    def list_history(self) -> List[str]:
+    def list_tables(self) -> List[str]:
         projects = open(self.history_path, "r").read().splitlines()
         return projects
 
     def save_table(self, table: Table):
-        history = self.list_history()
+        history = self.list_tables()
         try:
             history.remove(table.full_table_id)
         except ValueError:
             pass
         history.append(table.full_table_id)
         with open(self.history_path, "w") as f:
             f.write("\n".join(history))
 
     def pick_table(self, live: Optional[Live]) -> Optional[Table]:
-        history = self.list_history()
+        history = self.list_tables()
         from_history = bash_util.pick_one(history, live)
         table = None
         if from_history:
             table_ref = TableReference.from_string(from_history.replace(":", "."))
             project_id = table_ref.project
             dataset_id = table_ref.dataset_id
             table_id = table_ref.table_id
```

### Comparing `bq-meta-0.6.7/bq_meta/service/project_service.py` & `bq-meta-0.7.0/bq_meta/service/project_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from typing import List
 
 from bq_meta import const
-from bq_meta.bq_client import BqClient
+from bq_meta.client import Client
 from bq_meta.config import Config
 from rich.console import Console
 
 from bq_meta.util.rich_utils import progress
 
 
 class ProjectService:
-    def __init__(self, console: Console, config: Config, bq_client: BqClient) -> None:
+    def __init__(self, console: Console, config: Config, client: Client) -> None:
         self.console = console
         self.config = config
-        self.bq_client = bq_client
+        self.client = client
         self.projects_path = const.BQ_META_PROJECTS
 
     def list_projects(self) -> List[str]:
         projects = open(self.projects_path, "r").read().splitlines()
         return projects
 
     def fetch_projects(self):
         projects_ids = ["bigquery-public-data"]  # add bq public datasets explicitly, for testing purposes
-        iterator = self.bq_client.client.list_projects()
+        iterator = self.client.bq_client.list_projects()
         for project in progress(self.console, "projects", iterator):
             projects_ids.append(project.project_id)
 
         with open(self.projects_path, "w") as f:
             f.write("\n".join(projects_ids))
```

### Comparing `bq-meta-0.6.7/bq_meta/service/table_service.py` & `bq-meta-0.7.0/bq_meta/service/table_service.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from typing import Optional
 
-from bq_meta.bq_client import BqClient
+from bq_meta.client import Client
 from bq_meta.config import Config
 from bq_meta.service.project_service import ProjectService
 from bq_meta.util import bash_util
 from bq_meta.util.rich_utils import progress
 from google.cloud import bigquery
 from rich.console import Console
 from rich.live import Live
 
 
 class TableService:
     def __init__(
         self,
         console: Console,
         config: Config,
-        bq_client: BqClient,
+        client: Client,
         project_service: ProjectService,
     ):
         self.console = console
         self.config = config
-        self.bq_client = bq_client
+        self.client = client
         self.project_service = project_service
 
     def get_table(
         self,
         project_id: Optional[str] = None,
         dataset_id: Optional[str] = None,
         table_id: Optional[str] = None,
@@ -33,32 +33,32 @@
         table = None
         project_id = project_id if project_id else self._pick_project_id(live)
         if project_id:
             dataset_id = dataset_id if dataset_id else self._pick_dataset_id(project_id, live)
         if dataset_id:
             table_id = table_id if table_id else self._pick_table_id(project_id, dataset_id, live)
         if table_id:
-            table = self.bq_client.client.get_table(f"{project_id}.{dataset_id}.{table_id}")
+            table = self.client.bq_client.get_table(f"{project_id}.{dataset_id}.{table_id}")
         return table
 
     def get_fresh_table(self, table: bigquery.Table) -> bigquery.Table:
-        return self.bq_client.client.get_table(f"{table.project}.{table.dataset_id}.{table.table_id}")
+        return self.client.bq_client.get_table(f"{table.project}.{table.dataset_id}.{table.table_id}")
 
     # ======================   Pick   ======================
 
     def _pick_project_id(self, live: Optional[Live]) -> Optional[str]:
         project_ids = self.project_service.list_projects()
         return bash_util.pick_one(project_ids, live)
 
     def _pick_dataset_id(self, project_id: str, live: Optional[Live]) -> Optional[str]:
         dataset_ids = []
-        iterator = self.bq_client.client.list_datasets(project=project_id)
+        iterator = self.client.bq_client.list_datasets(project=project_id)
         for dataset in progress(self.console, "datasets", iterator):
             dataset_ids.append(dataset.dataset_id)
         return bash_util.pick_one(dataset_ids, live)
 
     def _pick_table_id(self, project_id: str, dataset_id: str, live: Optional[Live]) -> Optional[str]:
         table_ids = []
-        iterator = self.bq_client.client.list_tables(f"{project_id}.{dataset_id}")
+        iterator = self.client.bq_client.list_tables(f"{project_id}.{dataset_id}")
         for table in progress(self.console, "tables", iterator):
             table_ids.append(table.table_id)
         return bash_util.pick_one(table_ids, live)
```

### Comparing `bq-meta-0.6.7/bq_meta/service/version_service.py` & `bq-meta-0.7.0/bq_meta/service/version_service.py`

 * *Files identical despite different names*

### Comparing `bq-meta-0.6.7/bq_meta/util/bash_util.py` & `bq-meta-0.7.0/bq_meta/util/bash_util.py`

 * *Files identical despite different names*

### Comparing `bq-meta-0.6.7/bq_meta/util/rich_utils.py` & `bq-meta-0.7.0/bq_meta/util/rich_utils.py`

 * *Files identical despite different names*

### Comparing `bq-meta-0.6.7/bq_meta/util/table_utils.py` & `bq-meta-0.7.0/bq_meta/util/table_utils.py`

 * *Files identical despite different names*

### Comparing `bq-meta-0.6.7/bq_meta/window.py` & `bq-meta-0.7.0/bq_meta/window.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,99 +14,104 @@
 from rich.live import Live
 from rich.panel import Panel
 
 from bq_meta import const, output
 from bq_meta.config import Config
 from bq_meta.service.history_service import HistoryService
 from bq_meta.service.table_service import TableService
-from bq_meta.service.template_service import TemplateService
+from bq_meta.service.snippet_service import SnippetService
 from bq_meta.util import bash_util
 from bq_meta.util.rich_utils import flash_panel
 
 
 class View(Enum):
     empty = 1
     table = 2
     schema = 3
-    template = 4
+    snippets = 4
 
 
 @dataclass
 class Hint:
     key: str
     name: str
 
 
 hint_open = Hint("o", "Open new table")
 hint_refresh = Hint("r", "Refresh table")
 hint_table = Hint("t", "Show table")
 hint_schema = Hint("s", "Show schema")
-hint_template = Hint("ctrl-t", "Show templates")
+hint_snippets = Hint("p", "Show snippets")
 hint_console = Hint("c", "Open in console")
 hint_history = Hint("h", "Show history")
 hint_quit = Hint("q", "Quit")
 
-all_hints = [hint_open, hint_refresh, hint_table, hint_schema, hint_template, hint_console, hint_history, hint_quit]
+all_hints = [hint_open, hint_refresh, hint_table, hint_schema, hint_snippets, hint_console, hint_history]
 
 
 class Window:
     def __init__(
         self,
         console: Console,
         config: Config,
         history_service: HistoryService,
         table_service: TableService,
-        template_service: TemplateService,
+        snippet_service: SnippetService,
     ):
         self.console = console
         self.config = config
         self.history_service = history_service
         self.table_service = table_service
-        self.template_service = template_service
+        self.snippet_service = snippet_service
         self.table: Optional[bigquery.Table] = None
         self.project_id: Optional[str] = None
         self.dataset_id: Optional[str] = None
         self.layout: Layout = Layout()
         self.content: Optional[RenderableType] = None
         self.view: View = View.empty
         self.hints: List[str] = []
+        self.bottom_hints: List[str] = [hint_quit]
         self.values: List[str] = []
         self.selected_value: Optional[str] = None
-        self.template: Optional[str] = None
+        self.snippet: Optional[str] = None
 
     def live_window(self, table: Optional[bigquery.Table]):
         self.now = datetime.utcnow()
         self.table = table
         with Live(self.layout, auto_refresh=False, screen=True, transient=True) as live:
             self._loop(live)
 
-    def _update_content(self):
+    def _update_content(self, live: Live):
         match self.view:
             case View.empty:
-                self.hints = [hint_open, hint_history, hint_quit]
+                self.hints = [hint_open, hint_history]
             case View.table if self.table:
                 self.hints = all_hints
                 self.values = []
                 self.selected_value = None
                 self.content = output.get_table_output(self.table)
                 self._update_table(self.table)
             case View.schema if self.table:
                 self.hints = all_hints
                 self.values = []
                 self.selected_value = None
-                self.content = output.get_schema_output(self.table)
-            case View.template if self.table:
+                live.stop()
+                with self.console.pager():
+                    self.console.print(output.get_schema_output(self.table))
+                self.view = View.table
+                live.start()
+            case View.snippets if self.table:
                 self.hints = all_hints
-                self.template = self.template_service.get_template(self.selected_value, self.table)
-                self.content = output.get_template_output(self.template)
+                self.snippet = self.snippet_service.get_snippet(self.selected_value, self.table)
+                self.content = output.get_snippet_output(self.snippet)
 
     def _update_panel(self, live: Live) -> None:
         window_layout = Layout(name="window")
         body_layout = Layout(name="body")
-        hints_layout = output.hints_layout(self.hints)
+        hints_layout = output.hints_layout(self.hints, self.bottom_hints)
         content_layout = output.content_layout(self.content)
         list_layout = output.list_layout(self.values, self.selected_value)
         header_layout = output.header_layout(self.config)
         body_layout.split_row(hints_layout, content_layout, list_layout)
         window_layout.split_column(header_layout, body_layout)
         self.panel = Panel(
             title=self.now.strftime("%Y-%m-%d %H:%M:%S UTC"),
@@ -127,15 +132,15 @@
             self.dataset_id = table.dataset_id
             self.history_service.save_table(table)
 
     def _loop(self, live: Live):
         """
         Loop listening on specific keypress, updating live CLI
         """
-        self._update_content()
+        self._update_content(live)
         self._update_panel(live)
         char = readchar.readkey()
         match char:
 
             case "t" | key.BACKSPACE | key.ESC:
                 self.view = View.table
                 self.selected_value = None
@@ -183,29 +188,29 @@
             # Show schema view
             case "s" if self.table:
                 self.view = View.schema
 
             # Open google console
             case "c" if self.table:
                 match self.view:
-                    case View.template:
+                    case View.snippets:
                         url = f"https://console.cloud.google.com/bigquery?p={self.table.project}&d={self.table.dataset_id}&t={self.table.table_id}"
-                        pyperclip.copy(self.template)
+                        pyperclip.copy(self.snippet)
                         webbrowser.open(url)
 
                     case _:
                         url = f"https://console.cloud.google.com/bigquery?p={self.table.project}&d={self.table.dataset_id}&t={self.table.table_id}&page=table"
                         webbrowser.open(url)
 
-            # Show template view
-            case key.CTRL_T if self.table:
-                self.view = View.template
-                templates = self.template_service.list_templates()
-                self.values = templates
-                self.selected_value = templates[0] if templates else None
+            # Show snippets view
+            case "p" if self.table:
+                self.view = View.snippets
+                snippets = self.snippet_service.list_snippets()
+                self.values = snippets
+                self.selected_value = snippets[0] if snippets else None
 
             # Quit program
             case "q":
                 live.stop()
                 click.get_current_context().exit()
 
         # Infinite loop, until quitted (q)
```

### Comparing `bq-meta-0.6.7/bq_meta.egg-info/PKG-INFO` & `bq-meta-0.7.0/bq_meta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bq-meta
-Version: 0.6.7
+Version: 0.7.0
 Summary: BigQuery metadata
 Home-page: https://github.com/martintupy/bq-meta
 Author: Martin Tupy
 Author-email: id@martintupy.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bq-meta-0.6.7/bq_meta.egg-info/SOURCES.txt` & `bq-meta-0.7.0/bq_meta.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 bq_meta/__init__.py
 bq_meta/__main__.py
 bq_meta/auth.py
-bq_meta/bq_client.py
 bq_meta/cli.py
+bq_meta/client.py
 bq_meta/config.py
 bq_meta/const.py
 bq_meta/initialize.py
 bq_meta/output.py
 bq_meta/window.py
 bq_meta.egg-info/PKG-INFO
 bq_meta.egg-info/SOURCES.txt
 bq_meta.egg-info/dependency_links.txt
 bq_meta.egg-info/entry_points.txt
 bq_meta.egg-info/requires.txt
 bq_meta.egg-info/top_level.txt
 bq_meta/service/__init__.py
 bq_meta/service/history_service.py
 bq_meta/service/project_service.py
+bq_meta/service/snippet_service.py
 bq_meta/service/table_service.py
-bq_meta/service/template_service.py
 bq_meta/service/version_service.py
+bq_meta/snippets/dataset_size
+bq_meta/snippets/duplicate_count
+bq_meta/snippets/duplicate_rows
+bq_meta/snippets/month_size
+bq_meta/snippets/partition_size
+bq_meta/snippets/table_ddl
 bq_meta/util/__init__.py
 bq_meta/util/bash_util.py
 bq_meta/util/num_utils.py
 bq_meta/util/rich_utils.py
 bq_meta/util/table_utils.py
```

### Comparing `bq-meta-0.6.7/setup.cfg` & `bq-meta-0.7.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bq-meta
-version = 0.6.7
+version = 0.7.0
 description = BigQuery metadata
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/martintupy/bq-meta
 author = Martin Tupy
 author_email = id@martintupy.com
 license = Apache-2.0
@@ -24,14 +24,15 @@
 	google-cloud-bigquery
 	jinja2
 	pyperclip
 	pyyaml
 	readchar
 	rich
 python_requires = >=3.10
+include_package_data = True
 
 [options.entry_points]
 console_scripts = bq-meta = bq_meta.cli:cli
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

