# Comparing `tmp/github_repo_stats-0.1.1.tar.gz` & `tmp/github_repo_stats-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github_repo_stats-0.1.1.tar", last modified: Thu Apr 28 20:24:18 2022, max compression
+gzip compressed data, was "github_repo_stats-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `github_repo_stats-0.1.1.tar` & `github_repo_stats-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      589 2022-04-28 20:24:10.606469 github_repo_stats-0.1.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      636 2022-04-28 20:24:10.606469 github_repo_stats-0.1.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0     1846 2022-04-28 20:24:10.606469 github_repo_stats-0.1.1/.gitignore
--rw-r--r--   0        0        0     1072 2022-04-28 20:24:10.606469 github_repo_stats-0.1.1/LICENSE
--rw-r--r--   0        0        0     1955 2022-04-28 20:24:10.606469 github_repo_stats-0.1.1/README.md
--rw-r--r--   0        0        0      104 2022-04-28 20:24:10.606469 github_repo_stats-0.1.1/example.yaml
--rw-r--r--   0        0        0      850 2022-04-28 20:24:10.606469 github_repo_stats-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       79 2022-04-28 20:24:10.606469 github_repo_stats-0.1.1/requirements.in
--rw-r--r--   0        0        0     1825 2022-04-28 20:24:10.606469 github_repo_stats-0.1.1/requirements.txt
--rw-r--r--   0        0        0       30 2022-04-28 20:24:10.606469 github_repo_stats-0.1.1/src/gh_stats/__init__.py
--rw-r--r--   0        0        0     5829 2022-04-28 20:24:10.606469 github_repo_stats-0.1.1/src/gh_stats/cli.py
--rw-r--r--   0        0        0        0 2022-04-28 20:24:10.606469 github_repo_stats-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1777 2022-04-28 20:24:10.606469 github_repo_stats-0.1.1/tests/test_cli.py
--rw-r--r--   0        0        0      211 2022-04-28 20:24:10.606469 github_repo_stats-0.1.1/tox.ini
--rw-r--r--   0        0        0     2643 1970-01-01 00:00:00.000000 github_repo_stats-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      589 2023-05-19 15:45:03.105347 github_repo_stats-0.1.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      636 2023-05-19 15:45:03.105347 github_repo_stats-0.1.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1846 2023-05-19 15:45:03.105347 github_repo_stats-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1072 2023-05-19 15:45:03.105347 github_repo_stats-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1955 2023-05-19 15:45:03.105347 github_repo_stats-0.1.2/README.md
+-rw-r--r--   0        0        0      104 2023-05-19 15:45:03.105347 github_repo_stats-0.1.2/example.yaml
+-rw-r--r--   0        0        0      850 2023-05-19 15:45:03.105347 github_repo_stats-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       79 2023-05-19 15:45:03.105347 github_repo_stats-0.1.2/requirements.in
+-rw-r--r--   0        0        0    16482 2023-05-19 15:45:03.105347 github_repo_stats-0.1.2/requirements.txt
+-rw-r--r--   0        0        0       30 2023-05-19 15:45:03.105347 github_repo_stats-0.1.2/src/gh_stats/__init__.py
+-rw-r--r--   0        0        0     6566 2023-05-19 15:45:03.105347 github_repo_stats-0.1.2/src/gh_stats/cli.py
+-rw-r--r--   0        0        0        0 2023-05-19 15:45:03.105347 github_repo_stats-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     1777 2023-05-19 15:45:03.105347 github_repo_stats-0.1.2/tests/test_cli.py
+-rw-r--r--   0        0        0      211 2023-05-19 15:45:03.105347 github_repo_stats-0.1.2/tox.ini
+-rw-r--r--   0        0        0     2643 1970-01-01 00:00:00.000000 github_repo_stats-0.1.2/PKG-INFO
```

### Comparing `github_repo_stats-0.1.1/.github/workflows/publish.yml` & `github_repo_stats-0.1.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `github_repo_stats-0.1.1/.github/workflows/tests.yml` & `github_repo_stats-0.1.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `github_repo_stats-0.1.1/.gitignore` & `github_repo_stats-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `github_repo_stats-0.1.1/LICENSE` & `github_repo_stats-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `github_repo_stats-0.1.1/README.md` & `github_repo_stats-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `github_repo_stats-0.1.1/pyproject.toml` & `github_repo_stats-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dynamic = ["description"]
 requires-python=">=3.7"
 dependencies = [
     "pyyaml==6.0",
-    "requests==2.27.1",
-    "click==8.1.2",
-    "rich==12.2.0"
+    "requests==2.28.1",
+    "click==8.1.3",
+    "rich==12.5.1"
 ]
-version = "0.1.1"
+version = "0.1.2"
 
 [project.urls]
 Home = "https://migusgroup.com"
 Source = "https://github.com/The-Migus-Group/gh-repo-stats"
 
 [project.scripts]
 gh-stats = "gh_stats.cli:main"
```

### Comparing `github_repo_stats-0.1.1/src/gh_stats/cli.py` & `github_repo_stats-0.1.2/src/gh_stats/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,41 +4,56 @@
 from pathlib import Path
 
 import click
 import requests
 import yaml
 from rich.console import Console
 from rich.table import Table
+from typing import Union
+
+
+def check_response(response, repo) -> Union[str, dict]:
+    if response.status_code == 200:
+        return response.json()
+    else:
+        print(f"Repo {repo} returned this error: ", response.text)
 
 
 def get_repo_data(headers: dict, owner: str, repo: str) -> dict:
     """Fetches all data required for output for each repo"""
-    # TODO: Handle missing data if non-200 response
-    resp_data = requests.get(
-        f"https://api.github.com/repos/{owner}/{repo}", headers=headers
-    ).json()
 
-    views = requests.get(
+    resp_data, views, clones = None, None, None
+
+    resp = requests.get(f"https://api.github.com/repos/{owner}/{repo}", headers=headers)
+
+    resp_data = check_response(resp, repo)
+
+    views_resp = requests.get(
         f"https://api.github.com/repos/{owner}/{repo}/traffic/views", headers=headers
-    ).json()
+    )
+
+    views = check_response(views_resp, repo)
 
-    clones = requests.get(
+    clones_resp = requests.get(
         f"https://api.github.com/repos/{owner}/{repo}/traffic/clones", headers=headers
-    ).json()
+    )
+
+    clones = check_response(clones_resp, repo)
 
-    return {
-        "Repo": f"{owner}/{repo}",
-        "Forks": resp_data["forks_count"],
-        "Stars": resp_data["stargazers_count"],
-        "Watchers": resp_data["watchers_count"],
-        "Clones Total": clones["count"],
-        "Clones Unique": clones["uniques"],
-        "Views Total": views["count"],
-        "Views Unique": views["uniques"],
-    }
+    if all([resp_data, views, clones]):
+        return {
+            "Repo": f"{owner}/{repo}",
+            "Forks": resp_data["forks_count"],
+            "Stars": resp_data["stargazers_count"],
+            "Watchers": resp_data["watchers_count"],
+            "Clones Total": clones["count"],
+            "Clones Unique": clones["uniques"],
+            "Views Total": views["count"],
+            "Views Unique": views["uniques"],
+        }
 
 
 def parse_repos_list_from_yaml(file) -> dict:
     """Parses the YAML file and converts to Python objects"""
     with open(file) as yaml_file:
         return yaml.safe_load(yaml_file)
 
@@ -61,15 +76,15 @@
     help="Yaml representation of Repos to Pull",
 )
 @click.option("-o", "--org", help="Pull stats for all repos owned by Org")
 @click.option("-u", "--user", help="Pull stats for all repos owned by User")
 @click.option(
     "-f", "--output-file", type=Path, help="Output file path. Only supports CSV or JSON"
 )
-@click.option("-t", "--auth-token", help="GitHb Access Token")
+@click.option("-t", "--auth-token", help="GitHub Access Token")
 def main(repos, org, user, output_file, auth_token):
     """Fetch GitHub repo stats!
 
     REQUIRES either a repos yaml file, an org name, or a user's name.
 
     Typical usage:
     \n\t$ gh-stats -r example.yaml
@@ -96,84 +111,90 @@
     else:
         raise ValueError("Please provide a yaml file, owner, or user.")
 
     final_data = []
     for repo_owner in repos_dict["Owners"]:
         key = next(iter(repo_owner))
         for repo in repo_owner[key]:
-            final_data.append(get_repo_data(HEADERS, key, repo))
+            data = get_repo_data(HEADERS, key, repo)
 
-    if output_file:
-        file_path = Path(output_file)
+            if data:
+                final_data.append(data)
 
-        if file_path.suffix == ".csv":
-            print("Creating CSV")
-            with open(file_path, "w", newline="") as file:
-                writer = csv.DictWriter(
-                    file,
-                    fieldnames=[
-                        "Repo",
-                        "Forks",
-                        "Stars",
-                        "Watchers",
-                        "Clones Total",
-                        "Clones Unique",
-                        "Views Total",
-                        "Views Unique",
-                    ],
-                )
-                writer.writeheader()
+    if final_data:
 
-                for data in final_data:
-                    writer.writerow(
-                        {
-                            "Repo": data["Repo"],
-                            "Forks": data["Forks"],
-                            "Stars": data["Stars"],
-                            "Watchers": data["Watchers"],
-                            "Clones Total": data["Clones Total"],
-                            "Clones Unique": data["Clones Unique"],
-                            "Views Total": data["Views Total"],
-                            "Views Unique": data["Views Unique"],
-                        }
+        if output_file:
+            file_path = Path(output_file)
+
+            if file_path.suffix == ".csv":
+                print("Creating CSV")
+                with open(file_path, "w", newline="") as file:
+                    writer = csv.DictWriter(
+                        file,
+                        fieldnames=[
+                            "Repo",
+                            "Forks",
+                            "Stars",
+                            "Watchers",
+                            "Clones Total",
+                            "Clones Unique",
+                            "Views Total",
+                            "Views Unique",
+                        ],
                     )
+                    writer.writeheader()
 
-            print("CSV file created.")
+                    for data in final_data:
+                        writer.writerow(
+                            {
+                                "Repo": data["Repo"],
+                                "Forks": data["Forks"],
+                                "Stars": data["Stars"],
+                                "Watchers": data["Watchers"],
+                                "Clones Total": data["Clones Total"],
+                                "Clones Unique": data["Clones Unique"],
+                                "Views Total": data["Views Total"],
+                                "Views Unique": data["Views Unique"],
+                            }
+                        )
+
+                print("CSV file created.")
+
+            elif file_path.suffix == ".json":
+                print("Creating JSON")
+                with open(file_path, "w") as file:
+                    file_data = {"Data": [data for data in final_data]}
+                    file.write(json.dumps(file_data, indent=4))
 
-        elif file_path.suffix == ".json":
-            print("Creating JSON")
-            with open(file_path, "w") as file:
-                file_data = {"Data": [data for data in final_data]}
-                file.write(json.dumps(file_data, indent=4))
+            else:
+                raise ValueError("Output file must be CSV or JSON")
 
         else:
-            raise ValueError("Output file must be CSV or JSON")
 
-    else:
-        table = Table(title="GitHub Stats")
-        table.add_column("Repo")
-        table.add_column("Forks", justify="center")
-        table.add_column("Stars", justify="center")
-        table.add_column("Watchers", justify="center")
-        table.add_column("Clones Total", justify="center")
-        table.add_column("Clones Unique", justify="center")
-        table.add_column("Views Total", justify="center")
-        table.add_column("Views Unique", justify="center")
-
-        for data in final_data:
-            table.add_row(
-                str(data["Repo"]),
-                str(data["Forks"]),
-                str(data["Stars"]),
-                str(data["Watchers"]),
-                str(data["Clones Total"]),
-                str(data["Clones Unique"]),
-                str(data["Views Total"]),
-                str(data["Views Unique"]),
-            )
+            table = Table(title="GitHub Stats")
+            table.add_column("Repo")
+            table.add_column("Forks", justify="center")
+            table.add_column("Stars", justify="center")
+            table.add_column("Watchers", justify="center")
+            table.add_column("Clones Total", justify="center")
+            table.add_column("Clones Unique", justify="center")
+            table.add_column("Views Total", justify="center")
+            table.add_column("Views Unique", justify="center")
+
+            for data in final_data:
+                table.add_row(
+                    str(data["Repo"]),
+                    str(data["Forks"]),
+                    str(data["Stars"]),
+                    str(data["Watchers"]),
+                    str(data["Clones Total"]),
+                    str(data["Clones Unique"]),
+                    str(data["Views Total"]),
+                    str(data["Views Unique"]),
+                )
 
-        console = Console()
-        console.print(table)
+            console = Console()
+            console.print(table)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `github_repo_stats-0.1.1/tests/test_cli.py` & `github_repo_stats-0.1.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `github_repo_stats-0.1.1/PKG-INFO` & `github_repo_stats-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: github_repo_stats
-Version: 0.1.1
+Version: 0.1.2
 Summary: Fetch your GH Repo stats
 Author-email: Ricky White <ricky@migusgroup.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: pyyaml==6.0
-Requires-Dist: requests==2.27.1
-Requires-Dist: click==8.1.2
-Requires-Dist: rich==12.2.0
+Requires-Dist: requests==2.28.1
+Requires-Dist: click==8.1.3
+Requires-Dist: rich==12.5.1
 Project-URL: Home, https://migusgroup.com
 Project-URL: Source, https://github.com/The-Migus-Group/gh-repo-stats
 
 ![PyPI Version](https://img.shields.io/pypi/v/github-repo-stats) ![License](https://img.shields.io/github/license/the-migus-group/github-repo-stats) ![Python Versions](https://img.shields.io/pypi/pyversions/github-repo-stats)
 
 # GitHub Repo Stats
```

