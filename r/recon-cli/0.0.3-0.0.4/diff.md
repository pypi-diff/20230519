# Comparing `tmp/recon_cli-0.0.3.tar.gz` & `tmp/recon_cli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recon_cli-0.0.3.tar", last modified: Fri May 19 03:28:00 2023, max compression
+gzip compressed data, was "recon_cli-0.0.4.tar", last modified: Fri May 19 15:27:15 2023, max compression
```

## Comparing `recon_cli-0.0.3.tar` & `recon_cli-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0       51 2023-05-19 03:28:00.000000 recon_cli-0.0.3/.flake8
--rw-r--r--   0        0        0      231 2023-05-19 03:28:00.000000 recon_cli-0.0.3/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0      655 2023-05-19 03:28:00.000000 recon_cli-0.0.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      625 2023-05-19 03:28:00.000000 recon_cli-0.0.3/.github/workflows/tox.yml
--rw-r--r--   0        0        0      948 2023-05-19 03:28:00.000000 recon_cli-0.0.3/.gitignore
--rw-r--r--   0        0        0      563 2023-05-19 03:28:00.000000 recon_cli-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1069 2023-05-19 03:28:00.000000 recon_cli-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0     1225 2023-05-19 03:28:00.000000 recon_cli-0.0.3/README.md
--rw-r--r--   0        0        0      938 2023-05-19 03:28:00.000000 recon_cli-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      104 2023-05-19 03:28:00.000000 recon_cli-0.0.3/recon/__init__.py
--rw-r--r--   0        0        0     4306 2023-05-19 03:28:00.000000 recon_cli-0.0.3/recon/__main__.py
--rw-r--r--   0        0        0     9837 2023-05-19 03:28:00.000000 recon_cli-0.0.3/recon/reconcile.py
--rw-r--r--   0        0        0      364 2023-05-19 03:28:00.000000 recon_cli-0.0.3/recon/utils.py
--rw-r--r--   0        0        0     1058 2023-05-19 03:28:00.000000 recon_cli-0.0.3/requirements.txt
--rw-r--r--   0        0        0        0 2023-05-19 03:28:00.000000 recon_cli-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     3113 2023-05-19 03:28:00.000000 recon_cli-0.0.3/tests/test_main.py
--rw-r--r--   0        0        0      385 2023-05-19 03:28:00.000000 recon_cli-0.0.3/tox.ini
--rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 recon_cli-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       51 2023-05-19 15:27:15.000000 recon_cli-0.0.4/.flake8
+-rw-r--r--   0        0        0      231 2023-05-19 15:27:15.000000 recon_cli-0.0.4/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0      655 2023-05-19 15:27:15.000000 recon_cli-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      625 2023-05-19 15:27:15.000000 recon_cli-0.0.4/.github/workflows/tox.yml
+-rw-r--r--   0        0        0      948 2023-05-19 15:27:15.000000 recon_cli-0.0.4/.gitignore
+-rw-r--r--   0        0        0      563 2023-05-19 15:27:15.000000 recon_cli-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1069 2023-05-19 15:27:15.000000 recon_cli-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     7231 2023-05-19 15:27:15.000000 recon_cli-0.0.4/README.md
+-rw-r--r--   0        0        0      970 2023-05-19 15:27:15.000000 recon_cli-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-05-19 15:27:15.000000 recon_cli-0.0.4/recon/__init__.py
+-rw-r--r--   0        0        0       35 2023-05-19 15:27:15.000000 recon_cli-0.0.4/recon/__main__.py
+-rw-r--r--   0        0        0     4283 2023-05-19 15:27:15.000000 recon_cli-0.0.4/recon/main.py
+-rw-r--r--   0        0        0    10351 2023-05-19 15:27:15.000000 recon_cli-0.0.4/recon/reconcile.py
+-rw-r--r--   0        0        0      364 2023-05-19 15:27:15.000000 recon_cli-0.0.4/recon/utils.py
+-rw-r--r--   0        0        0     1058 2023-05-19 15:27:15.000000 recon_cli-0.0.4/requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-19 15:27:15.000000 recon_cli-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     3113 2023-05-19 15:27:15.000000 recon_cli-0.0.4/tests/test_main.py
+-rw-r--r--   0        0        0      374 2023-05-19 15:27:15.000000 recon_cli-0.0.4/tox.ini
+-rw-r--r--   0        0        0     8042 1970-01-01 00:00:00.000000 recon_cli-0.0.4/PKG-INFO
```

### Comparing `recon_cli-0.0.3/.github/workflows/publish.yml` & `recon_cli-0.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.3/.github/workflows/tox.yml` & `recon_cli-0.0.4/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.3/.gitignore` & `recon_cli-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.3/.pre-commit-config.yaml` & `recon_cli-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.3/LICENSE.txt` & `recon_cli-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.3/pyproject.toml` & `recon_cli-0.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "recon-cli"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Mynhardt Burger", email="mynhardt+recon@gmail.com" },
 ]
-description = "Simple reconciliation of two lists based on a common field"
+description = "Simple command line tool to reconcile datasets"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Financial and Insurance Industry",
@@ -23,14 +23,17 @@
 
 [project.optional-dependencies]
 test = [
     "pytest >=2.7.3",
     "pytest-cov",
 ]
 
+[project.scripts]
+recon = "recon.main:app"
+
 [project.urls]
 "Homepage" = "https://github.com/mynhardtburger/recon-cli"
 
 [tool.flit.module]
 name = "recon"
 
 [tool.isort]
```

### Comparing `recon_cli-0.0.3/recon/__main__.py` & `recon_cli-0.0.4/recon/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 
 
 def main(
     left: Annotated[
         Path,
         typer.Argument(
             default=...,
-            help="Path to the left dataset.",
+            help="Path to the left dataset (csv|xlsx).",
             show_default=False,
             exists=True,
             file_okay=True,
             dir_okay=False,
             writable=False,
             readable=True,
             resolve_path=True,
         ),
     ],
     right: Annotated[
         Path,
         typer.Argument(
             default=...,
-            help="Path to the right dataset.",
+            help="Path to the right dataset (csv|xlsx).",
             show_default=False,
             exists=True,
             file_okay=True,
             dir_okay=False,
             writable=False,
             readable=True,
             resolve_path=True,
@@ -88,15 +88,15 @@
             rich_help_panel="Input options",
         ),
     ] = "Sheet1",
     output_file: Annotated[
         str,
         typer.Option(
             default=...,
-            help="Path to save results (in xlsx format) to.",
+            help="Path to save results to (xlsx).",
             show_default=False,
             rich_help_panel="Output options",
         ),
     ] = "",
     std_out: Annotated[
         bool,
         typer.Option(
@@ -141,18 +141,17 @@
         progress.add_task(description="Reconciling...", total=None)
 
         if info_only:
             recon.info()
             raise typer.Exit()
 
         if std_out:
-            recon.to_stdout(["all_data"])
+            recon.to_stdout(["all"])
             raise typer.Exit()
 
         if output_file:
-            recon.to_xlsx(output_file, ["all_data"])
+            recon.to_xlsx(output_file, ["all"])
             print(f"Recon results saved to '{output_file}'.")
             raise typer.Exit()
 
 
-if __name__ == "__main__":
-    typer.run(main)
+app = typer.run(main)
```

### Comparing `recon_cli-0.0.3/recon/reconcile.py` & `recon_cli-0.0.4/recon/reconcile.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,22 +14,23 @@
 
 FilePath = Union[str, "PathLike[str]"]
 Suffixes = Union[
     list[Union[str, None]], tuple[str, None], tuple[None, str], tuple[str, str]
 ]
 
 RECON_COMPONENTS = Literal[
-    "left_both",
-    "right_both",
     "left_only",
     "right_only",
     "left_duplicate",
     "right_duplicate",
+    "left_both",
+    "right_both",
+    "left",
+    "right",
     "both",
-    "data_map",
     "all_data",
     "all",
 ]
 
 
 Relationship = Enum(
     "Relationship", ["ONE_TO_ONE", "ONE_TO_MANY", "MANY_TO_ONE", "MANY_TO_MANY", "NONE"]
@@ -41,25 +42,39 @@
         self.left: pd.DataFrame
         self.right: pd.DataFrame
         self.left_on: str
         self.right_on: str
 
         self.suffixes: tuple[str, str]
 
-        self.output_dispatch = [
+        self._output_dispatch = [
             "left_only",
             "right_only",
             "left_duplicate",
             "right_duplicate",
             "left_both",
             "right_both",
             "left",
             "right",
+            "both",
+            "all_data",
         ]
-        """Set of property names available for export."""
+        """List of property names available for output."""
+
+        self._all = [
+            "left_only",
+            "right_only",
+            "left_duplicate",
+            "right_duplicate",
+            "left_both",
+            "right_both",
+            "left",
+            "right",
+        ]
+        """List of property names represented by "all"."""
 
     def _map_column_names(self):
         left_columns = set(self.left.reset_index(names="index").columns)
         right_columns = set(self.right.reset_index(names="index").columns)
         common_columns = left_columns & right_columns
         left_only = left_columns - right_columns
         right_only = right_columns - left_columns
@@ -200,30 +215,37 @@
         Right: {right_stats}
         Relationship: {self.relationship} ({self.left_on}:{self.right_on})
         """
         )
         print(report)
 
     def to_xlsx(
-        self, path: FilePath, recon_components: list[RECON_COMPONENTS], **kwargs
+        self,
+        path: FilePath,
+        recon_components: list[RECON_COMPONENTS] = ["all"],
+        **kwargs,
     ) -> None:
-        write_list = (
-            self.output_dispatch if "all_data" in recon_components else recon_components
-        )
+        if recon_components == ["all"]:
+            write_list = self._all
+        else:
+            write_list = [x for x in recon_components if x in self._output_dispatch]
 
         with pd.ExcelWriter(path, **kwargs) as writer:
             for component in write_list:
                 getattr(self, component).to_excel(
                     writer, sheet_name=component, index_label="index"
                 )
 
-    def to_stdout(self, recon_components: list[RECON_COMPONENTS], **kwargs) -> None:
-        write_list = (
-            self.output_dispatch if "all_data" in recon_components else recon_components
-        )
+    def to_stdout(
+        self, recon_components: list[RECON_COMPONENTS] = ["all"], **kwargs
+    ) -> None:
+        if recon_components == ["all"]:
+            write_list = self._all
+        else:
+            write_list = [x for x in recon_components if x in self._output_dispatch]
 
         print("--------- START ----------")
         for component in write_list:
             print(f"--------- {component} ----------")
             getattr(self, component).to_csv(sys.stdout, index_label="index", **kwargs)
         print("--------- END ----------")
```

### Comparing `recon_cli-0.0.3/requirements.txt` & `recon_cli-0.0.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `recon_cli-0.0.3/tests/test_main.py` & `recon_cli-0.0.4/tests/test_main.py`

 * *Files identical despite different names*

