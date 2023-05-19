# Comparing `tmp/cvat-cli-2.3.0.tar.gz` & `tmp/cvat-cli-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvat-cli-2.3.0.tar", last modified: Fri Dec 23 11:22:24 2022, max compression
+gzip compressed data, was "cvat-cli-2.4.0.tar", last modified: Thu Mar 16 09:13:42 2023, max compression
```

## Comparing `cvat-cli-2.3.0.tar` & `cvat-cli-2.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2022-12-23 11:22:24.793991 cvat-cli-2.3.0/
--rw-rw-r--   0 max       (1000) max       (1000)       47 2022-12-20 15:26:28.000000 cvat-cli-2.3.0/MANIFEST.in
--rw-rw-r--   0 max       (1000) max       (1000)     2325 2022-12-23 11:22:24.793991 cvat-cli-2.3.0/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)     1981 2022-12-20 15:26:28.000000 cvat-cli-2.3.0/README.md
--rw-rw-r--   0 max       (1000) max       (1000)      383 2022-12-20 15:26:28.000000 cvat-cli-2.3.0/pyproject.toml
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2022-12-23 11:22:24.793991 cvat-cli-2.3.0/requirements/
--rw-rw-r--   0 max       (1000) max       (1000)       30 2022-12-23 11:10:08.000000 cvat-cli-2.3.0/requirements/base.txt
--rw-rw-r--   0 max       (1000) max       (1000)       38 2022-12-23 11:22:24.793991 cvat-cli-2.3.0/setup.cfg
--rw-rw-r--   0 max       (1000) max       (1000)     1969 2022-12-20 15:26:28.000000 cvat-cli-2.3.0/setup.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2022-12-23 11:22:24.793991 cvat-cli-2.3.0/src/
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2022-12-23 11:22:24.793991 cvat-cli-2.3.0/src/cvat_cli/
--rw-rw-r--   0 max       (1000) max       (1000)        0 2022-12-20 15:26:28.000000 cvat-cli-2.3.0/src/cvat_cli/__init__.py
--rwxrwxr-x   0 max       (1000) max       (1000)     2151 2022-12-20 15:26:28.000000 cvat-cli-2.3.0/src/cvat_cli/__main__.py
--rw-rw-r--   0 max       (1000) max       (1000)     4784 2022-12-22 14:07:57.000000 cvat-cli-2.3.0/src/cvat_cli/cli.py
--rw-rw-r--   0 max       (1000) max       (1000)    12050 2022-12-21 19:40:57.000000 cvat-cli-2.3.0/src/cvat_cli/parser.py
--rw-rw-r--   0 max       (1000) max       (1000)       18 2022-12-23 11:10:08.000000 cvat-cli-2.3.0/src/cvat_cli/version.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2022-12-23 11:22:24.793991 cvat-cli-2.3.0/src/cvat_cli.egg-info/
--rw-rw-r--   0 max       (1000) max       (1000)     2325 2022-12-23 11:22:24.000000 cvat-cli-2.3.0/src/cvat_cli.egg-info/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)      402 2022-12-23 11:22:24.000000 cvat-cli-2.3.0/src/cvat_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 max       (1000) max       (1000)        1 2022-12-23 11:22:24.000000 cvat-cli-2.3.0/src/cvat_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 max       (1000) max       (1000)       52 2022-12-23 11:22:24.000000 cvat-cli-2.3.0/src/cvat_cli.egg-info/entry_points.txt
--rw-rw-r--   0 max       (1000) max       (1000)       30 2022-12-23 11:22:24.000000 cvat-cli-2.3.0/src/cvat_cli.egg-info/requires.txt
--rw-rw-r--   0 max       (1000) max       (1000)        9 2022-12-23 11:22:24.000000 cvat-cli-2.3.0/src/cvat_cli.egg-info/top_level.txt
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-16 09:13:42.886870 cvat-cli-2.4.0/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       47 2023-03-16 08:50:27.000000 cvat-cli-2.4.0/MANIFEST.in
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2325 2023-03-16 09:13:42.886870 cvat-cli-2.4.0/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1981 2023-03-16 08:50:27.000000 cvat-cli-2.4.0/README.md
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      383 2023-03-16 08:50:27.000000 cvat-cli-2.4.0/pyproject.toml
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-16 09:13:42.886870 cvat-cli-2.4.0/requirements/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       30 2023-03-16 08:50:27.000000 cvat-cli-2.4.0/requirements/base.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       38 2023-03-16 09:13:42.886870 cvat-cli-2.4.0/setup.cfg
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1969 2023-03-16 08:50:27.000000 cvat-cli-2.4.0/setup.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-16 09:13:42.886870 cvat-cli-2.4.0/src/
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-16 09:13:42.886870 cvat-cli-2.4.0/src/cvat_cli/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        0 2023-03-16 08:50:27.000000 cvat-cli-2.4.0/src/cvat_cli/__init__.py
+-rwxr-xr-x   0 andrey    (1000) andrey    (1000)     2151 2023-03-16 08:50:27.000000 cvat-cli-2.4.0/src/cvat_cli/__main__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     4805 2023-03-16 08:50:27.000000 cvat-cli-2.4.0/src/cvat_cli/cli.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13103 2023-03-16 08:50:27.000000 cvat-cli-2.4.0/src/cvat_cli/parser.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       18 2023-03-16 08:50:27.000000 cvat-cli-2.4.0/src/cvat_cli/version.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-16 09:13:42.886870 cvat-cli-2.4.0/src/cvat_cli.egg-info/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2325 2023-03-16 09:13:42.000000 cvat-cli-2.4.0/src/cvat_cli.egg-info/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      402 2023-03-16 09:13:42.000000 cvat-cli-2.4.0/src/cvat_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2023-03-16 09:13:42.000000 cvat-cli-2.4.0/src/cvat_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       52 2023-03-16 09:13:42.000000 cvat-cli-2.4.0/src/cvat_cli.egg-info/entry_points.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       30 2023-03-16 09:13:42.000000 cvat-cli-2.4.0/src/cvat_cli.egg-info/requires.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        9 2023-03-16 09:13:42.000000 cvat-cli-2.4.0/src/cvat_cli.egg-info/top_level.txt
```

### Comparing `cvat-cli-2.3.0/PKG-INFO` & `cvat-cli-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvat-cli
-Version: 2.3.0
+Version: 2.4.0
 Summary: Command-line client for CVAT
 Home-page: https://github.com/cvat-ai/cvat/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `cvat-cli-2.3.0/README.md` & `cvat-cli-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cvat-cli-2.3.0/setup.py` & `cvat-cli-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `cvat-cli-2.3.0/src/cvat_cli/__main__.py` & `cvat-cli-2.4.0/src/cvat_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `cvat-cli-2.3.0/src/cvat_cli/cli.py` & `cvat-cli-2.4.0/src/cvat_cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,17 @@
             for r in results:
                 print(r.id)
 
     def tasks_create(
         self,
         name: str,
         labels: List[Dict[str, str]],
-        resource_type: ResourceType,
         resources: Sequence[str],
         *,
+        resource_type: ResourceType = ResourceType.LOCAL,
         annotation_path: str = "",
         annotation_format: str = "CVAT XML 1.1",
         status_check_period: int = 2,
         dataset_repository_url: str = "",
         lfs: bool = False,
         **kwargs,
     ) -> None:
```

### Comparing `cvat-cli-2.3.0/src/cvat_cli/parser.py` & `cvat-cli-2.4.0/src/cvat_cli/parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # SPDX-License-Identifier: MIT
 
 import argparse
 import getpass
 import json
 import logging
 import os
+import textwrap
 from distutils.util import strtobool
 
 from cvat_sdk.core.proxies.tasks import ResourceType
 
 from .version import VERSION
 
 
@@ -86,18 +87,23 @@
     )
 
     #######################################################################
     # Create
     #######################################################################
     task_create_parser = task_subparser.add_parser(
         "create",
-        description="""Create a new CVAT task. To create a task, you need
-                    to specify labels using the --labels argument or
-                    attach the task to an existing project using the
-                    --project_id argument.""",
+        description=textwrap.dedent(
+            """\
+            Create a new CVAT task. To create a task, you need
+            to specify labels using the --labels argument or
+            attach the task to an existing project using the
+            --project_id argument.
+        """
+        ),
+        formatter_class=argparse.RawTextHelpFormatter,
     )
     task_create_parser.add_argument("name", type=str, help="name of the task")
     task_create_parser.add_argument(
         "resource_type",
         default="local",
         choices=list(ResourceType),
         type=parse_resource_type,
@@ -120,46 +126,64 @@
         "--chunk_size", default=None, type=int, help="the number of frames per chunk"
     )
     task_create_parser.add_argument(
         "--completion_verification_period",
         dest="status_check_period",
         default=2,
         type=float,
-        help="""number of seconds to wait until checking
-                if data compression finished (necessary before uploading annotations)""",
+        help=textwrap.dedent(
+            """\
+            number of seconds to wait until checking
+            if data compression finished (necessary before uploading annotations)
+        """
+        ),
     )
     task_create_parser.add_argument(
         "--copy_data",
         default=False,
         action="store_true",
-        help="""set the option to copy the data, only used when resource type is
-                share (default: %(default)s)""",
+        help=textwrap.dedent(
+            """\
+            set the option to copy the data, only used when resource type is
+            share (default: %(default)s)
+        """
+        ),
     )
     task_create_parser.add_argument(
         "--dataset_repository_url",
         default="",
         type=str,
-        help=(
-            "git repository to store annotations e.g."
-            " https://github.com/user/repos [annotation/<anno_file_name.zip>]"
+        help=textwrap.dedent(
+            """\
+            git repository to store annotations e.g.
+            https://github.com/user/repos [annotation/<anno_file_name.zip>]
+        """
         ),
     )
     task_create_parser.add_argument(
         "--frame_step",
         default=None,
         type=int,
-        help="""set the frame step option in the advanced configuration
-                when uploading image series or videos (default: %(default)s)""",
+        help=textwrap.dedent(
+            """\
+            set the frame step option in the advanced configuration
+            when uploading image series or videos (default: %(default)s)
+        """
+        ),
     )
     task_create_parser.add_argument(
         "--image_quality",
         default=70,
         type=int,
-        help="""set the image quality option in the advanced configuration
-                when creating tasks.(default: %(default)s)""",
+        help=textwrap.dedent(
+            """\
+            set the image quality option in the advanced configuration
+            when creating tasks.(default: %(default)s)
+        """
+        ),
     )
     task_create_parser.add_argument(
         "--labels",
         default="[]",
         type=parse_label_arg,
         help="string or file containing JSON labels specification",
     )
@@ -197,14 +221,34 @@
         "--use_cache", action="store_true", help="""use cache"""  # automatically sets default=False
     )
     task_create_parser.add_argument(
         "--use_zip_chunks",
         action="store_true",  # automatically sets default=False
         help="""zip chunks before sending them to the server""",
     )
+    task_create_parser.add_argument(
+        "--cloud_storage_id",
+        default=None,
+        type=int,
+        help="cloud storage ID if you would like to use data from cloud storage",
+    )
+    task_create_parser.add_argument(
+        "--filename_pattern",
+        type=str,
+        help=textwrap.dedent(
+            """\
+            pattern for filtering data from the manifest file for the upload.
+            Only shell-style wildcards are supported:
+            * - matches everything
+            ? - matches any single character
+            [seq] - matches any character in 'seq'
+            [!seq] - matches any character not in seq
+        """
+        ),
+    )
 
     #######################################################################
     # Delete
     #######################################################################
     delete_parser = task_subparser.add_parser("delete", description="Delete a CVAT task.")
     delete_parser.add_argument("task_ids", type=int, help="list of task IDs", nargs="+")
```

### Comparing `cvat-cli-2.3.0/src/cvat_cli.egg-info/PKG-INFO` & `cvat-cli-2.4.0/src/cvat_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvat-cli
-Version: 2.3.0
+Version: 2.4.0
 Summary: Command-line client for CVAT
 Home-page: https://github.com/cvat-ai/cvat/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

