# Comparing `tmp/jobbergate-cli-3.5.0a2.tar.gz` & `tmp/jobbergate_cli-3.5.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate-cli-3.5.0a2.tar", max compression
+gzip compressed data, was "jobbergate_cli-3.5.0a3.tar", max compression
```

## Comparing `jobbergate-cli-3.5.0a2.tar` & `jobbergate_cli-3.5.0a3.tar`

### file list

```diff
@@ -1,36 +1,35 @@
--rw-r--r--   0        0        0     1082 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/LICENSE
--rw-r--r--   0        0        0     1065 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/README.rst
--rw-r--r--   0        0        0      801 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/__init__.py
--rw-r--r--   0        0        0     1112 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/application_base.py
--rw-r--r--   0        0        0    11271 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/auth.py
--rw-r--r--   0        0        0     3614 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/compat.py
--rw-r--r--   0        0        0     4355 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/config.py
--rw-r--r--   0        0        0     1139 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/constants.py
--rw-r--r--   0        0        0     3112 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/exceptions.py
--rw-r--r--   0        0        0     1134 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/jobberappslib.py
--rw-r--r--   0        0        0     1095 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/logging.py
--rw-r--r--   0        0        0     6510 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/main.py
--rw-r--r--   0        0        0     7002 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/render.py
--rw-r--r--   0        0        0     7348 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/requests.py
--rw-r--r--   0        0        0     6006 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/schemas.py
--rw-r--r--   0        0        0       66 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/__init__.py
--rw-r--r--   0        0        0       66 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/applications/__init__.py
--rw-r--r--   0        0        0    10132 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/applications/app.py
--rw-r--r--   0        0        0     1725 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/applications/application_base.py
--rw-r--r--   0        0        0     1558 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/applications/application_helpers.py
--rw-r--r--   0        0        0    13800 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/applications/questions.py
--rw-r--r--   0        0        0    10292 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/applications/tools.py
--rw-r--r--   0        0        0       61 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/clusters/__init__.py
--rw-r--r--   0        0        0      728 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/clusters/app.py
--rw-r--r--   0        0        0     3284 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/clusters/tools.py
--rw-r--r--   0        0        0       64 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/job_scripts/__init__.py
--rw-r--r--   0        0        0    10067 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/job_scripts/app.py
--rw-r--r--   0        0        0     5519 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/job_scripts/tools.py
--rw-r--r--   0        0        0       68 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/job_submissions/__init__.py
--rw-r--r--   0        0        0     6502 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/job_submissions/app.py
--rw-r--r--   0        0        0     4167 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/job_submissions/tools.py
--rw-r--r--   0        0        0     1370 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/text_tools.py
--rw-r--r--   0        0        0     3524 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/jobbergate_cli/time_loop.py
--rw-r--r--   0        0        0     2531 2023-04-27 21:34:05.378925 jobbergate-cli-3.5.0a2/pyproject.toml
--rw-r--r--   0        0        0     2542 2023-04-27 21:34:23.553271 jobbergate-cli-3.5.0a2/setup.py
--rw-r--r--   0        0        0     2824 2023-04-27 21:34:23.553738 jobbergate-cli-3.5.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/LICENSE
+-rw-r--r--   0        0        0     1065 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/README.rst
+-rw-r--r--   0        0        0      801 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/__init__.py
+-rw-r--r--   0        0        0     1112 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/application_base.py
+-rw-r--r--   0        0        0    11271 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/auth.py
+-rw-r--r--   0        0        0     4414 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/compat.py
+-rw-r--r--   0        0        0     4355 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/config.py
+-rw-r--r--   0        0        0     1139 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/constants.py
+-rw-r--r--   0        0        0     3112 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/exceptions.py
+-rw-r--r--   0        0        0     1134 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/jobberappslib.py
+-rw-r--r--   0        0        0     1095 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/logging.py
+-rw-r--r--   0        0        0     6510 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/main.py
+-rw-r--r--   0        0        0     7523 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/render.py
+-rw-r--r--   0        0        0     7348 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/requests.py
+-rw-r--r--   0        0        0     6084 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/schemas.py
+-rw-r--r--   0        0        0       66 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/__init__.py
+-rw-r--r--   0        0        0       66 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/applications/__init__.py
+-rw-r--r--   0        0        0    11778 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/applications/app.py
+-rw-r--r--   0        0        0     1725 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/applications/application_base.py
+-rw-r--r--   0        0        0     1558 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/applications/application_helpers.py
+-rw-r--r--   0        0        0    13800 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/applications/questions.py
+-rw-r--r--   0        0        0    11471 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/applications/tools.py
+-rw-r--r--   0        0        0       61 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/clusters/__init__.py
+-rw-r--r--   0        0        0      728 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/clusters/app.py
+-rw-r--r--   0        0        0     3284 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/clusters/tools.py
+-rw-r--r--   0        0        0       64 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/job_scripts/__init__.py
+-rw-r--r--   0        0        0    11693 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/job_scripts/app.py
+-rw-r--r--   0        0        0     6750 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/job_scripts/tools.py
+-rw-r--r--   0        0        0       68 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/job_submissions/__init__.py
+-rw-r--r--   0        0        0     7123 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/job_submissions/app.py
+-rw-r--r--   0        0        0     4167 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/job_submissions/tools.py
+-rw-r--r--   0        0        0     1370 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/text_tools.py
+-rw-r--r--   0        0        0     3524 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/jobbergate_cli/time_loop.py
+-rw-r--r--   0        0        0     2531 2023-05-09 14:04:30.775206 jobbergate_cli-3.5.0a3/pyproject.toml
+-rw-r--r--   0        0        0     2923 1970-01-01 00:00:00.000000 jobbergate_cli-3.5.0a3/PKG-INFO
```

### Comparing `jobbergate-cli-3.5.0a2/LICENSE` & `jobbergate_cli-3.5.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a2/README.rst` & `jobbergate_cli-3.5.0a3/README.rst`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/__init__.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/application_base.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/application_base.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/auth.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/auth.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/compat.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/compat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 """
 Provide compatibility to the previous version of Jobbergate CLI for users who have automation or are
 familiar with the old commands
 """
 
 import typer
 
+from jobbergate_cli.subapps.applications.app import archive as archive_application
 from jobbergate_cli.subapps.applications.app import create as create_application
 from jobbergate_cli.subapps.applications.app import delete as delete_application
 from jobbergate_cli.subapps.applications.app import download_files as download_files_application
 from jobbergate_cli.subapps.applications.app import get_one as get_application
 from jobbergate_cli.subapps.applications.app import list_all as list_applications
+from jobbergate_cli.subapps.applications.app import restore as restore_application
 from jobbergate_cli.subapps.applications.app import update as update_application
+from jobbergate_cli.subapps.job_scripts.app import archive as archive_job_script
 from jobbergate_cli.subapps.job_scripts.app import create as create_job_script
 from jobbergate_cli.subapps.job_scripts.app import delete as delete_job_script
 from jobbergate_cli.subapps.job_scripts.app import download_files as download_files_job_script
 from jobbergate_cli.subapps.job_scripts.app import get_one as get_job_script
 from jobbergate_cli.subapps.job_scripts.app import list_all as list_job_scripts
+from jobbergate_cli.subapps.job_scripts.app import restore as restore_job_script
 from jobbergate_cli.subapps.job_scripts.app import update as update_job_script
 from jobbergate_cli.subapps.job_submissions.app import create as create_job_submission
 from jobbergate_cli.subapps.job_submissions.app import delete as delete_job_submission
 from jobbergate_cli.subapps.job_submissions.app import get_one as get_job_submission
 from jobbergate_cli.subapps.job_submissions.app import list_all as list_job_submissions
 
 
@@ -39,14 +43,22 @@
         help="GET an Application.",
     )(get_application)
     app.command(
         name="create-application",
         help="CREATE an Application.",
     )(create_application)
     app.command(
+        name="archive-application",
+        help="ARCHIVE an Application.",
+    )(archive_application)
+    app.command(
+        name="restore-application",
+        help="RESTORE an Application.",
+    )(restore_application)
+    app.command(
         name="delete-application",
         help="DELETE an Application.",
     )(delete_application)
     app.command(
         name="update-application",
         help="UPDATE an Application.",
     )(update_application)
@@ -65,14 +77,22 @@
         help="GET a job script",
     )(get_job_script)
     app.command(
         name="create-job-script",
         help="CREATE a job script",
     )(create_job_script)
     app.command(
+        name="archive-job-script",
+        help="ARCHIVE a Job Script.",
+    )(archive_job_script)
+    app.command(
+        name="restore-job-script",
+        help="RESTORE a Job Script.",
+    )(restore_job_script)
+    app.command(
         name="update-job-script",
         help="UPDATE a job script",
     )(update_job_script)
     app.command(
         name="delete-job-script",
         help="DELETE a job script",
     )(delete_job_script)
```

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/config.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/config.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/constants.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/constants.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/exceptions.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/jobberappslib.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/jobberappslib.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/logging.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/logging.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/main.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/main.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/render.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/render.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import json
 from typing import Any, Dict, List, Optional, Union, cast
 
 import pydantic
 from rich import print_json
 from rich.console import Console
 from rich.panel import Panel
+from rich.prompt import Confirm
 from rich.table import Table
 
 from jobbergate_cli.schemas import JobbergateContext, ListResponseEnvelope
 from jobbergate_cli.text_tools import dedent
 from jobbergate_cli.text_tools import indent as indent_text
 
 
@@ -86,14 +87,27 @@
         text = indent_text(text, prefix="  ")
     console = Console()
     console.print()
     console.print(Panel(text, **panel_kwargs))
     console.print()
 
 
+def terminal_confirm(*args, question: str = "Are you sure you want to continue?", **kwargs) -> bool:
+    """
+    Print a nicely formatted message as output to the user using a ``rich`` ``Panel``.
+
+    :param: *args:    Arguments for nested ``terminal_message``
+    :param: *kwargs:  Arguments for nested ``terminal_message``
+    :param: question: The text for the confirmation question
+    """
+    terminal_message(*args, **kwargs)
+    result = Confirm().ask(question)
+    return result
+
+
 def render_json(data: Any):
     """
     Print nicely formatted representation of a JSON serializable python primitive.
     """
     console = Console()
     console.print()
     console.print_json(json.dumps(data))
```

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/requests.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/requests.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/schemas.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
 
     id: int
     application_name: str
     application_identifier: Optional[str] = None
     application_description: Optional[str] = None
     application_owner_email: str
     application_uploaded: bool
+    is_archived: Optional[bool] = None
     created_at: Optional[datetime] = None
     updated_at: Optional[datetime] = None
     application_config: Optional[str] = None
     application_source_file: Optional[str] = None
     application_templates: Optional[Dict[str, str]] = None
 
 
@@ -120,14 +121,15 @@
 
     id: int
     application_id: int
     job_script_name: str
     job_script_description: Optional[str] = None
     job_script_files: JobScriptFiles
     job_script_owner_email: str
+    is_archived: Optional[bool] = None
     created_at: Optional[datetime] = None
     updated_at: Optional[datetime] = None
 
 
 class JobSubmissionResponse(pydantic.BaseModel, extra=pydantic.Extra.ignore):
     """
     Describes the format of data for job_submissions retrieved from the Jobbergate API endpoints.
```

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/applications/app.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/applications/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,30 +6,38 @@
 from textwrap import dedent
 from typing import Any, Dict, Optional, cast
 
 import typer
 
 from jobbergate_cli.constants import OV_CONTACT, SortOrder
 from jobbergate_cli.exceptions import handle_abort
-from jobbergate_cli.render import StyleMapper, render_list_results, render_single_result, terminal_message
+from jobbergate_cli.render import (
+    StyleMapper,
+    render_list_results,
+    render_single_result,
+    terminal_confirm,
+    terminal_message,
+)
 from jobbergate_cli.requests import make_request
 from jobbergate_cli.schemas import JobbergateContext, ListResponseEnvelope
 from jobbergate_cli.subapps.applications.tools import (
+    change_archive_status,
     fetch_application_data,
     load_default_config,
     save_application_files,
     upload_application,
 )
 
 
 # TODO: move hidden field logic to the API
 HIDDEN_FIELDS = [
     "application_config",
     "application_source_file",
     "application_templates",
+    "is_archived",
     "created_at",
     "updated_at",
 ]
 
 ID_NOTE = """
 
     This id represents the primary key of the application in the database. It
@@ -61,14 +69,15 @@
 
 @app.command("list")
 @handle_abort
 def list_all(
     ctx: typer.Context,
     show_all: bool = typer.Option(False, "--all", help="Show all applications, even the ones without identifier"),
     user_only: bool = typer.Option(False, "--user", help="Show only applications owned by the current user"),
+    include_archived: bool = typer.Option(False, help="Show archived applications as well"),
     search: Optional[str] = typer.Option(None, help="Apply a search term to results"),
     sort_order: SortOrder = typer.Option(SortOrder.UNSORTED, help="Specify sort order"),
     sort_field: Optional[str] = typer.Option(None, help="The field by which results should be sorted"),
 ):
     """
     Show available applications
     """
@@ -77,14 +86,15 @@
     # Make static type checkers happy
     assert jg_ctx is not None
     assert jg_ctx.client is not None
 
     params: Dict[str, Any] = dict(
         all=show_all,
         user=user_only,
+        include_archived=include_archived,
     )
     if search is not None:
         params["search"] = search
     if sort_order is not SortOrder.UNSORTED:
         params["sort_ascending"] = SortOrder is SortOrder.ASCENDING
     if sort_field is not None:
         params["sort_field"] = sort_field
@@ -103,15 +113,15 @@
         ),
     )
     render_list_results(
         jg_ctx,
         envelope,
         title="Applications List",
         style_mapper=style_mapper,
-        hidden_fields=HIDDEN_FIELDS,
+        hidden_fields=HIDDEN_FIELDS + (["is_archived"] if include_archived else []),
     )
 
 
 @app.command()
 @handle_abort
 def get_one(
     ctx: typer.Context,
@@ -291,18 +301,41 @@
 @handle_abort
 def delete(
     ctx: typer.Context,
     id: int = typer.Option(
         ...,
         help=f"the specific id of the application to delete. {ID_NOTE}",
     ),
+    confirm: bool = typer.Option(
+        None,
+        "--confirm",
+        "-y",
+        help="If supplied, do not ask for confirmation; just delete.",
+    ),
 ):
     """
     Delete an existing application.
     """
+    if not confirm and not terminal_confirm(
+        """
+        [yellow]Any files uploaded for this Application will be completely removed.
+        Any references to it in other items will also be removed.
+        """,
+        subject="Deleting is permanent!",
+        color="red",
+    ):
+        terminal_message(
+            """
+            No application was deleted.
+            """,
+            subject="Aborted",
+            color="yellow",
+        )
+        return
+
     jg_ctx: JobbergateContext = ctx.obj
 
     # Make static type checkers happy
     assert jg_ctx.client is not None
 
     # Delete the upload. The API will also remove the application data files
     make_request(
@@ -320,14 +353,47 @@
         """,
         subject="Application delete succeeded",
     )
 
 
 @app.command()
 @handle_abort
+def archive(
+    ctx: typer.Context,
+    id: int = typer.Option(
+        ...,
+        help=f"the specific id of the application to archive. {ID_NOTE}",
+    ),
+):
+    """
+    Archive an existing application.
+
+    An application that is archived will not appear in lists by default. This is a way to
+    effectively hide an application from view.
+    """
+    change_archive_status(ctx.obj, id, True)
+
+
+@app.command()
+@handle_abort
+def restore(
+    ctx: typer.Context,
+    id: int = typer.Option(
+        ...,
+        help=f"the specific id of the application to restore from the archive. {ID_NOTE}",
+    ),
+):
+    """
+    Restore an archived application.
+    """
+    change_archive_status(ctx.obj, id, False)
+
+
+@app.command()
+@handle_abort
 def download_files(
     ctx: typer.Context,
     id: Optional[int] = typer.Option(
         None,
         help=f"The specific id of the application. {ID_NOTE}",
     ),
     identifier: Optional[str] = typer.Option(
```

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/applications/application_base.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/applications/application_base.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/applications/application_helpers.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/applications/application_helpers.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/applications/questions.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/applications/questions.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/applications/tools.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/applications/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from jobbergate_cli.constants import (
     JOBBERGATE_APPLICATION_CONFIG,
     JOBBERGATE_APPLICATION_CONFIG_FILE_NAME,
     JOBBERGATE_APPLICATION_MODULE_FILE_NAME,
     JOBBERGATE_APPLICATION_SUPPORTED_FILES,
 )
 from jobbergate_cli.exceptions import Abort
+from jobbergate_cli.render import terminal_message
 from jobbergate_cli.requests import make_request
 from jobbergate_cli.schemas import ApplicationResponse, JobbergateApplicationConfig, JobbergateContext
 from jobbergate_cli.subapps.applications.application_base import JobbergateApplicationBase
 from jobbergate_cli.subapps.applications.questions import gather_param_values
 
 
 def load_default_config() -> Dict[str, Any]:
@@ -269,7 +270,41 @@
     :param: supplied_params: Pre-set values for the parameters. Any questions about these values will be skipped.
     :param: fast_mode:       If true, do not ask the user questions. Just use supplied_params or defaults
     :returns: The configuration values collected from the user by executing the application
     """
     app_params = gather_param_values(app_module, supplied_params=supplied_params, fast_mode=fast_mode)
     app_config.application_config.update(**app_params)
     return app_params
+
+
+def change_archive_status(
+    jg_ctx: JobbergateContext,
+    application_id: int,
+    should_archive: bool,
+):
+    """
+    Change the "is_archived" status of an application.
+
+    :param: jg_ctx:           The JobbergateContext. Needed to access the Httpx client with which to make API calls
+    :param: application_id:   The id of the application for which to change the archived status
+    :param: should_archive:   If true, archive the application. Otherwise restore it.
+    """
+    # Make static type checkers happy
+    assert jg_ctx.client is not None
+
+    message_stub = "archive" if should_archive else "restore"
+    make_request(
+        jg_ctx.client,
+        f"/jobbergate/applications/{application_id}",
+        "PUT",
+        expected_status=200,
+        expect_response=False,
+        abort_message=f"Request to {message_stub} application was not accepted by the API",
+        support=True,
+        json=dict(is_archived=should_archive),
+    )
+    terminal_message(
+        f"""
+        The application was successfully {message_stub}d.
+        """,
+        subject=f"Application {message_stub} succeeded",
+    )
```

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/clusters/app.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/clusters/app.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/clusters/tools.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/clusters/tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/job_scripts/app.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/job_scripts/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,42 @@
 import pathlib
 from typing import Any, Dict, List, Optional, cast
 
 import typer
 
 from jobbergate_cli.constants import SortOrder
 from jobbergate_cli.exceptions import Abort, handle_abort
-from jobbergate_cli.render import StyleMapper, render_json, render_list_results, render_single_result, terminal_message
+from jobbergate_cli.render import (
+    StyleMapper,
+    render_json,
+    render_list_results,
+    render_single_result,
+    terminal_confirm,
+    terminal_message,
+)
 from jobbergate_cli.requests import make_request
 from jobbergate_cli.schemas import JobbergateContext, JobScriptResponse, ListResponseEnvelope
-from jobbergate_cli.subapps.job_scripts.tools import create_job_script, download_job_script_files, fetch_job_script_data
+from jobbergate_cli.subapps.job_scripts.tools import (
+    change_archive_status,
+    create_job_script,
+    download_job_script_files,
+    fetch_job_script_data,
+)
 from jobbergate_cli.subapps.job_submissions.app import HIDDEN_FIELDS as JOB_SUBMISSION_HIDDEN_FIELDS
 from jobbergate_cli.subapps.job_submissions.tools import create_job_submission
 from jobbergate_cli.text_tools import dedent
 
 
 # move hidden field logic to the API
 HIDDEN_FIELDS = [
     "created_at",
     "updated_at",
     "job_script_data_as_string",
     "job_script_files",
+    "is_archived",
 ]
 
 
 style_mapper = StyleMapper(
     id="green",
     job_script_name="cyan",
 )
@@ -37,14 +50,15 @@
 
 
 @app.command("list")
 @handle_abort
 def list_all(
     ctx: typer.Context,
     show_all: bool = typer.Option(False, "--all", help="Show all job scripts, even the ones owned by others"),
+    include_archived: bool = typer.Option(False, help="Show archived job_scripts as well"),
     search: Optional[str] = typer.Option(None, help="Apply a search term to results"),
     sort_order: SortOrder = typer.Option(SortOrder.UNSORTED, help="Specify sort order"),
     sort_field: Optional[str] = typer.Option(None, help="The field by which results should be sorted"),
     from_application_id: Optional[int] = typer.Option(
         None,
         help="Filter job-scripts by the application-id they were created from.",
     ),
@@ -54,15 +68,15 @@
     """
     jg_ctx: JobbergateContext = ctx.obj
 
     # Make static type checkers happy
     assert jg_ctx is not None
     assert jg_ctx.client is not None
 
-    params: Dict[str, Any] = dict(all=show_all)
+    params: Dict[str, Any] = dict(all=show_all, include_archived=include_archived)
     if search is not None:
         params["search"] = search
     if sort_order is not SortOrder.UNSORTED:
         params["sort_ascending"] = SortOrder is SortOrder.ASCENDING
     if sort_field is not None:
         params["sort_field"] = sort_field
     if from_application_id is not None:
@@ -82,15 +96,15 @@
         ),
     )
     render_list_results(
         jg_ctx,
         envelope,
         title="Job Scripts List",
         style_mapper=style_mapper,
-        hidden_fields=HIDDEN_FIELDS,
+        hidden_fields=HIDDEN_FIELDS + (["is_archived"] if include_archived else []),
     )
 
 
 @app.command()
 @handle_abort
 def get_one(
     ctx: typer.Context,
@@ -268,18 +282,41 @@
 @handle_abort
 def delete(
     ctx: typer.Context,
     id: int = typer.Option(
         ...,
         help="The id of the job script to delete",
     ),
+    confirm: bool = typer.Option(
+        None,
+        "--confirm",
+        "-y",
+        help="If supplied, do not ask for confirmation; just delete.",
+    ),
 ):
     """
     Delete an existing job script.
     """
+    if not confirm and not terminal_confirm(
+        """
+        [yellow]Any files uploaded for this Job Script will be completely removed.
+        Any references to it in other items will also be removed.
+        """,
+        subject="Deleting is permanent!",
+        color="red",
+    ):
+        terminal_message(
+            """
+            No job_script was deleted.
+            """,
+            subject="Aborted",
+            color="yellow",
+        )
+        return
+
     jg_ctx: JobbergateContext = ctx.obj
 
     # Make static type checkers happy
     assert jg_ctx.client is not None
 
     make_request(
         jg_ctx.client,
@@ -293,14 +330,47 @@
         "The job script was successfully deleted.",
         subject="Job script delete succeeded",
     )
 
 
 @app.command()
 @handle_abort
+def archive(
+    ctx: typer.Context,
+    id: int = typer.Option(
+        ...,
+        help="the specific id of the job_script to archive.",
+    ),
+):
+    """
+    Archive an existing job_script.
+
+    A job_script that is archived will not appear in lists by default. This is a way to
+    effectively hide a job_script from view.
+    """
+    change_archive_status(ctx.obj, id, True)
+
+
+@app.command()
+@handle_abort
+def restore(
+    ctx: typer.Context,
+    id: int = typer.Option(
+        ...,
+        help="the specific id of the job_script to restore from the archive.",
+    ),
+):
+    """
+    Restore an archived job_script.
+    """
+    change_archive_status(ctx.obj, id, False)
+
+
+@app.command()
+@handle_abort
 def show_files(
     ctx: typer.Context,
     id: int = typer.Option(int, help="The specific id of the job script."),
     plain: bool = typer.Option(False, help="Show the files in plain text."),
 ):
     """
     Show the files for a single job script by id.
```

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/job_scripts/tools.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/job_scripts/tools.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import json
 import pathlib
 from typing import Any, Dict, List, Optional, cast
 
 from loguru import logger
 
 from jobbergate_cli.exceptions import Abort
+from jobbergate_cli.render import terminal_message
 from jobbergate_cli.requests import make_request
 from jobbergate_cli.schemas import JobbergateContext, JobScriptCreateRequestData, JobScriptResponse
 from jobbergate_cli.subapps.applications.tools import execute_application, fetch_application_data, load_application_data
 
 
 def validate_parameter_file(parameter_path: pathlib.Path) -> Dict[str, Any]:
     """
@@ -157,7 +158,42 @@
     """
     result = fetch_job_script_data(jg_ctx, id)
     downloaded_files = save_job_script_files(
         job_script_data=result,
         destination_path=pathlib.Path.cwd(),
     )
     return downloaded_files
+
+
+def change_archive_status(
+    jg_ctx: JobbergateContext,
+    job_script_id: int,
+    should_archive: bool,
+):
+    """
+    Change the "is_archived" status of a job_script.
+
+    :param: jg_ctx:           The JobbergateContext. Needed to access the Httpx client with which to make API calls
+    :param:  job_script_id:   The id of the job_script for which to change the archived status
+    :param: should_archive:   If true, archive the job_script. Otherwise restore it.
+    """
+    # Make static type checkers happy
+    assert jg_ctx.client is not None
+
+    message_stub = "archive" if should_archive else "restore"
+    make_request(
+        jg_ctx.client,
+        f"/jobbergate/job-scripts/{job_script_id}",
+        "PUT",
+        expected_status=200,
+        expect_response=False,
+        abort_message=f"Request to {message_stub} job_script was not accepted by the API",
+        support=True,
+        json=dict(is_archived=should_archive),
+    )
+    message_stub = "archive" if should_archive else "restore"
+    terminal_message(
+        f"""
+        The job_script was successfully {message_stub}d.
+        """,
+        subject=f"Job Script {message_stub} succeeded",
+    )
```

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/job_submissions/app.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/job_submissions/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,21 @@
 from textwrap import dedent
 from typing import Any, Dict, Optional, cast
 
 import typer
 
 from jobbergate_cli.constants import SortOrder
 from jobbergate_cli.exceptions import handle_abort
-from jobbergate_cli.render import StyleMapper, render_list_results, render_single_result, terminal_message
+from jobbergate_cli.render import (
+    StyleMapper,
+    render_list_results,
+    render_single_result,
+    terminal_confirm,
+    terminal_message,
+)
 from jobbergate_cli.requests import make_request
 from jobbergate_cli.schemas import JobbergateContext, ListResponseEnvelope
 from jobbergate_cli.subapps.job_scripts.tools import download_job_script_files
 from jobbergate_cli.subapps.job_submissions.tools import create_job_submission, fetch_job_submission_data
 
 
 # move hidden field logic to the API
@@ -192,18 +198,40 @@
 @handle_abort
 def delete(
     ctx: typer.Context,
     id: int = typer.Option(
         ...,
         help="The id of the job submission to delete",
     ),
+    confirm: bool = typer.Option(
+        None,
+        "--confirm",
+        "-y",
+        help="If supplied, do not ask for confirmation; just delete.",
+    ),
 ):
     """
     Delete an existing job submission.
     """
+    if not confirm and not terminal_confirm(
+        """
+        [yellow]Job Submissons are a historical record and should not usually be deleted.
+        """,
+        subject="Deleting is permanent!",
+        color="red",
+    ):
+        terminal_message(
+            """
+            No job_submission was deleted.
+            """,
+            subject="Aborted",
+            color="yellow",
+        )
+        return
+
     jg_ctx: JobbergateContext = ctx.obj
 
     # Make static type checkers happy
     assert jg_ctx.client is not None, "Client is uninitialized"
 
     make_request(
         jg_ctx.client,
```

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/subapps/job_submissions/tools.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/subapps/job_submissions/tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/text_tools.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/text_tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a2/jobbergate_cli/time_loop.py` & `jobbergate_cli-3.5.0a3/jobbergate_cli/time_loop.py`

 * *Files identical despite different names*

### Comparing `jobbergate-cli-3.5.0a2/pyproject.toml` & `jobbergate_cli-3.5.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-cli"
-version = "3.5.0-alpha.2"
+version = "3.5.0-alpha.3"
 description = "Jobbergate CLI Client"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 packages = [ { include = "jobbergate_cli" } ]
 classifiers = [
```

### Comparing `jobbergate-cli-3.5.0a2/PKG-INFO` & `jobbergate_cli-3.5.0a3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: jobbergate-cli
-Version: 3.5.0a2
+Version: 3.5.0a3
 Summary: Jobbergate CLI Client
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.6.2,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: PyYAML (>=5.4.1,<6.0.0)
 Requires-Dist: boto3 (>=1.18.64,<2.0.0)
 Requires-Dist: click (>=8.0.1,<9.0.0)
 Requires-Dist: httpx (>=0.22.0,<0.23.0)
 Requires-Dist: importlib-metadata (>=4.2,<5.0)
 Requires-Dist: inquirer (>=2.7.0,<3.0.0)
```

