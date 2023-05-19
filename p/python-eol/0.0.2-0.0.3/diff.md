# Comparing `tmp/python_eol-0.0.2.tar.gz` & `tmp/python_eol-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_eol-0.0.2.tar", last modified: Mon May  1 07:25:15 2023, max compression
+gzip compressed data, was "python_eol-0.0.3.tar", last modified: Fri May 19 05:57:50 2023, max compression
```

## Comparing `python_eol-0.0.2.tar` & `python_eol-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-01 07:25:15.171445 python_eol-0.0.2/
--rw-rw-r--   0 martin    (1000) martin    (1000)      182 2023-05-01 07:24:31.000000 python_eol-0.0.2/.bumpversion.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)       28 2023-04-30 12:26:27.000000 python_eol-0.0.2/.flake8
--rw-rw-r--   0 martin    (1000) martin    (1000)      103 2023-04-30 15:47:31.000000 python_eol-0.0.2/.gitignore
--rw-rw-r--   0 martin    (1000) martin    (1000)      998 2023-05-01 07:21:13.000000 python_eol-0.0.2/.pre-commit-config.yaml
--rw-rw-r--   0 martin    (1000) martin    (1000)      303 2023-04-30 15:29:54.000000 python_eol-0.0.2/.pre-commit-hooks.yaml
--rw-rw-r--   0 martin    (1000) martin    (1000)     1062 2023-04-30 15:40:38.000000 python_eol-0.0.2/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)     1477 2023-05-01 07:25:15.171445 python_eol-0.0.2/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     1012 2023-05-01 07:21:13.000000 python_eol-0.0.2/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)     1894 2023-05-01 07:24:31.000000 python_eol-0.0.2/pyproject.toml
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-01 07:25:15.171445 python_eol-0.0.2/python_eol/
--rw-rw-r--   0 martin    (1000) martin    (1000)       74 2023-04-30 12:53:47.000000 python_eol-0.0.2/python_eol/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      646 2023-05-01 07:13:42.000000 python_eol-0.0.2/python_eol/_docker_utils.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1509 2023-04-24 16:42:44.000000 python_eol-0.0.2/python_eol/db.json
--rw-rw-r--   0 martin    (1000) martin    (1000)     3696 2023-05-01 05:45:39.000000 python_eol-0.0.2/python_eol/main.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-01 07:25:15.171445 python_eol-0.0.2/python_eol.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1477 2023-05-01 07:25:15.000000 python_eol-0.0.2/python_eol.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      469 2023-05-01 07:25:15.000000 python_eol-0.0.2/python_eol.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-05-01 07:25:15.000000 python_eol-0.0.2/python_eol.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       45 2023-05-01 07:25:15.000000 python_eol-0.0.2/python_eol.egg-info/entry_points.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       11 2023-05-01 07:25:15.000000 python_eol-0.0.2/python_eol.egg-info/top_level.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      109 2023-05-01 07:23:55.000000 python_eol-0.0.2/requirements-dev.in
--rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-05-01 07:25:15.171445 python_eol-0.0.2/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-01 07:25:15.171445 python_eol-0.0.2/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-04-30 06:43:54.000000 python_eol-0.0.2/tests/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1972 2023-05-01 07:12:56.000000 python_eol-0.0.2/tests/test_docker_utils.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3597 2023-05-01 07:12:48.000000 python_eol-0.0.2/tests/test_main.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1228 2023-04-30 17:26:09.000000 python_eol-0.0.2/tox.ini
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-19 05:57:50.569562 python_eol-0.0.3/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      182 2023-05-19 05:49:53.000000 python_eol-0.0.3/.bumpversion.cfg
+-rw-rw-r--   0 martin    (1000) martin    (1000)       28 2023-04-30 12:26:27.000000 python_eol-0.0.3/.flake8
+-rw-rw-r--   0 martin    (1000) martin    (1000)      103 2023-04-30 15:47:31.000000 python_eol-0.0.3/.gitignore
+-rw-rw-r--   0 martin    (1000) martin    (1000)      998 2023-05-19 05:49:30.000000 python_eol-0.0.3/.pre-commit-config.yaml
+-rw-rw-r--   0 martin    (1000) martin    (1000)      303 2023-04-30 15:29:54.000000 python_eol-0.0.3/.pre-commit-hooks.yaml
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1062 2023-04-30 15:40:38.000000 python_eol-0.0.3/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1725 2023-05-19 05:57:50.569562 python_eol-0.0.3/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1260 2023-05-19 05:49:19.000000 python_eol-0.0.3/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1894 2023-05-19 05:49:53.000000 python_eol-0.0.3/pyproject.toml
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-19 05:57:50.565562 python_eol-0.0.3/python_eol/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       74 2023-04-30 12:53:47.000000 python_eol-0.0.3/python_eol/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      646 2023-05-01 07:13:42.000000 python_eol-0.0.3/python_eol/_docker_utils.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      830 2023-05-19 05:42:08.000000 python_eol-0.0.3/python_eol/db.json
+-rw-rw-r--   0 martin    (1000) martin    (1000)      530 2023-05-19 05:42:08.000000 python_eol-0.0.3/python_eol/db_nep.json
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4009 2023-05-19 05:42:08.000000 python_eol-0.0.3/python_eol/main.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-19 05:57:50.565562 python_eol-0.0.3/python_eol.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1725 2023-05-19 05:57:50.000000 python_eol-0.0.3/python_eol.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      538 2023-05-19 05:57:50.000000 python_eol-0.0.3/python_eol.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-05-19 05:57:50.000000 python_eol-0.0.3/python_eol.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       45 2023-05-19 05:57:50.000000 python_eol-0.0.3/python_eol.egg-info/entry_points.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       11 2023-05-19 05:57:50.000000 python_eol-0.0.3/python_eol.egg-info/top_level.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      109 2023-05-01 07:23:55.000000 python_eol-0.0.3/requirements-dev.in
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-19 05:57:50.565562 python_eol-0.0.3/scripts/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1058 2023-05-19 05:45:01.000000 python_eol-0.0.3/scripts/eol_scraper.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1773 2023-05-19 05:45:01.000000 python_eol-0.0.3/scripts/nep_scraper.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-05-19 05:57:50.569562 python_eol-0.0.3/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-19 05:57:50.569562 python_eol-0.0.3/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-04-30 06:43:54.000000 python_eol-0.0.3/tests/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1972 2023-05-01 07:12:56.000000 python_eol-0.0.3/tests/test_docker_utils.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3959 2023-05-19 05:42:08.000000 python_eol-0.0.3/tests/test_main.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1302 2023-05-19 05:42:08.000000 python_eol-0.0.3/tox.ini
```

### Comparing `python_eol-0.0.2/.pre-commit-config.yaml` & `python_eol-0.0.3/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -29,11 +29,11 @@
     hooks:
       - id: black
   - repo: https://github.com/lyz-code/yamlfix/
     rev: 1.9.0
     hooks:
       - id: yamlfix
   - repo: https://github.com/mimre25/python-eol/
-    rev: v0.0.2
+    rev: v0.0.3
     hooks:
       - id: python-eol-check
         args: [--fail-close-to-eol]
```

### Comparing `python_eol-0.0.2/LICENSE` & `python_eol-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_eol-0.0.2/PKG-INFO` & `python_eol-0.0.3/python_eol.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: python_eol
-Version: 0.0.2
+Name: python-eol
+Version: 0.0.3
 Summary: Simple tool to check if python version is past EOL
 Author-email: Martin Imre <martinimre25@gmail.com>
 Project-URL: Source, https://github.com/mimre25/python-eol
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
@@ -28,20 +28,27 @@
 ## Usage
 Simply invoke `eol` from your command line
 ```sh
 eol
 ```
 **Options**:
 ```sh
+usage: eol [-h] [--fail-close-to-eol] [--check-docker-files] [--nep29]
+
+eol check if your python version is beyond end of life
+
+options:
+  -h, --help            show this help message and exit
   --fail-close-to-eol   Fail if the python version is close to eol instead of just warn
   --check-docker-files  Search for Dockerfile (**/*Dockerfile*) and check the python versions specified inside them
+  --nep29               Use NEP0029 end of life policy
 ```
 
 ## Pre-commit-hook
 Add the following to your `.pre-commit-config.yaml`:
 ```yaml
 repos:
   - repo: https://github.com/mimre25/python-eol/
-    rev: v0.0.2
+    rev: v0.0.3
     hooks:
       - id: python-eol-check
 ```
```

### Comparing `python_eol-0.0.2/README.md` & `python_eol-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -15,20 +15,27 @@
 ## Usage
 Simply invoke `eol` from your command line
 ```sh
 eol
 ```
 **Options**:
 ```sh
+usage: eol [-h] [--fail-close-to-eol] [--check-docker-files] [--nep29]
+
+eol check if your python version is beyond end of life
+
+options:
+  -h, --help            show this help message and exit
   --fail-close-to-eol   Fail if the python version is close to eol instead of just warn
   --check-docker-files  Search for Dockerfile (**/*Dockerfile*) and check the python versions specified inside them
+  --nep29               Use NEP0029 end of life policy
 ```
 
 ## Pre-commit-hook
 Add the following to your `.pre-commit-config.yaml`:
 ```yaml
 repos:
   - repo: https://github.com/mimre25/python-eol/
-    rev: v0.0.2
+    rev: v0.0.3
     hooks:
       - id: python-eol-check
 ```
```

### Comparing `python_eol-0.0.2/pyproject.toml` & `python_eol-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python_eol"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   {name = "Martin Imre", email = "martinimre25@gmail.com"}
 ]
 description = "Simple tool to check if python version is past EOL"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `python_eol-0.0.2/python_eol/_docker_utils.py` & `python_eol-0.0.3/python_eol/_docker_utils.py`

 * *Files identical despite different names*

### Comparing `python_eol-0.0.2/python_eol/main.py` & `python_eol-0.0.3/python_eol/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,52 +17,52 @@
 
 
 def _get_major_minor() -> str:
     major, minor, patch = platform.python_version_tuple()
     return f"{major}.{minor}"
 
 
-def _get_db_file_path() -> Path:
+def _get_db_file_path(*, nep_mode: bool = False) -> Path:
     major, minor, _ = platform.python_version_tuple()
-
+    filename = "db.json" if not nep_mode else "db_nep.json"
     if int(major) == 3 and int(minor) >= 9:  # noqa: PLR2004
         import importlib.resources
 
         data_path = importlib.resources.files("python_eol")
-        db_file = f"{data_path}/db.json"
+        db_file = f"{data_path}/{filename}"
     else:
         import pkg_resources  # pragma: no cover
 
         db_file = pkg_resources.resource_filename(
             "python_eol",
-            "db.json",
+            filename,
         )  # pragma: no cover
 
     return Path(db_file)
 
 
 def _check_eol(
     python_version: str,
     version_info: dict[str, dict[str, Any]],
     *,
     fail_close_to_eol: bool = False,
     prefix: str = "",
 ) -> int:
     my_version_info = version_info[python_version]
     today = date.today()
-    eol_date = date.fromisoformat(my_version_info["eol"])
+    eol_date = date.fromisoformat(my_version_info["End of Life"])
     time_to_eol = eol_date - today
 
     if time_to_eol.days < 0:
         logger.error(f"{prefix}Python {python_version} is beyond end of life")
         return 1
     if time_to_eol.days < EOL_WARN_DAYS:
         msg = (
             f"{prefix}Python {python_version} is going to "
-            f"be end of life in 2 months {eol_date}"
+            f"be end of life within the next 2 months ({eol_date})"
         )
 
         if fail_close_to_eol:
             logger.error(msg)
             return 1
         else:
             logger.warning(msg)
@@ -70,20 +70,21 @@
     return 0
 
 
 def _check_python_eol(
     *,
     fail_close_to_eol: bool = False,
     check_docker_files: bool = False,
+    nep_mode: bool = False,
 ) -> int:
-    db_file = _get_db_file_path()
+    db_file = _get_db_file_path(nep_mode=nep_mode)
     with db_file.open() as f:
         eol_data = json.load(f)
 
-    version_info = {entry["cycle"]: entry for entry in eol_data}
+    version_info = {entry["Version"]: entry for entry in eol_data}
 
     my_version = _get_major_minor()
 
     docker_res = 0
     if check_docker_files:
         for path in _find_docker_files():
             version = _extract_python_version_from_docker_file(path)
@@ -116,22 +117,28 @@
         "--check-docker-files",
         action="store_true",
         help=(
             "Search for Dockerfile (**/*Dockerfile*) and check "
             "the python versions specified inside them"
         ),
     )
+    parser.add_argument(
+        "--nep29",
+        action="store_true",
+        help=("Use NEP0029 end of life policy"),
+    )
     return parser
 
 
 def main() -> int:
     """Run main entry point."""
     parser = _get_argparser()
     args, unknown_args = parser.parse_known_args()
     return _check_python_eol(
         fail_close_to_eol=args.fail_close_to_eol,
         check_docker_files=args.check_docker_files,
+        nep_mode=args.nep29,
     )
 
 
 if __name__ == "__main__":
     raise SystemExit(main())
```

### Comparing `python_eol-0.0.2/python_eol.egg-info/PKG-INFO` & `python_eol-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: python-eol
-Version: 0.0.2
+Name: python_eol
+Version: 0.0.3
 Summary: Simple tool to check if python version is past EOL
 Author-email: Martin Imre <martinimre25@gmail.com>
 Project-URL: Source, https://github.com/mimre25/python-eol
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
@@ -28,20 +28,27 @@
 ## Usage
 Simply invoke `eol` from your command line
 ```sh
 eol
 ```
 **Options**:
 ```sh
+usage: eol [-h] [--fail-close-to-eol] [--check-docker-files] [--nep29]
+
+eol check if your python version is beyond end of life
+
+options:
+  -h, --help            show this help message and exit
   --fail-close-to-eol   Fail if the python version is close to eol instead of just warn
   --check-docker-files  Search for Dockerfile (**/*Dockerfile*) and check the python versions specified inside them
+  --nep29               Use NEP0029 end of life policy
 ```
 
 ## Pre-commit-hook
 Add the following to your `.pre-commit-config.yaml`:
 ```yaml
 repos:
   - repo: https://github.com/mimre25/python-eol/
-    rev: v0.0.2
+    rev: v0.0.3
     hooks:
       - id: python-eol-check
 ```
```

### Comparing `python_eol-0.0.2/tests/test_docker_utils.py` & `python_eol-0.0.3/tests/test_docker_utils.py`

 * *Files identical despite different names*

### Comparing `python_eol-0.0.2/tests/test_main.py` & `python_eol-0.0.3/tests/test_main.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,27 +39,38 @@
 
 mock_py311 = pytest.mark.usefixtures("_mock_py311")
 
 
 def test_get_argparser() -> None:
     parser = _get_argparser()
     args, kwargs = parser.parse_known_args(
-        ["--fail-close-to-eol"],
+        ["--fail-close-to-eol", "--check-docker-files", "--nep29"],
     )
 
     assert args.fail_close_to_eol is True
+    assert args.check_docker_files is True
+    assert args.nep29 is True
 
 
 def test_get_argparser2() -> None:
     parser = _get_argparser()
     args, kwargs = parser.parse_known_args(
         [],
     )
 
     assert args.fail_close_to_eol is False
+    assert args.check_docker_files is False
+    assert args.nep29 is False
+
+
+@mock_py37
+@freeze_time("2021-12-27")
+def test_ep_mode() -> None:
+    result = _check_python_eol(nep_mode=True)
+    assert result == 1
 
 
 @mock_py37
 @freeze_time("2023-04-30")
 @pytest.mark.parametrize("fail_close_to_eol", [True, False])
 def test_check_python_eol(
     fail_close_to_eol: bool,
@@ -128,9 +139,12 @@
         mocked_find_docker_files.return_value = [p]
         result = _check_python_eol(
             fail_close_to_eol=fail_close_to_eol,
             check_docker_files=True,
         )
         assert result == expected_return_status
 
-    msg = f"{p}: Python 3.7 is going to be end of life in 2 months 2023-06-27"
+    msg = (
+        f"{p}: Python 3.7 is going to be end of life within the next 2 months"
+        " (2023-06-27)"
+    )
     assert caplog.record_tuples == [("python_eol.main", log_level, msg)]
```

### Comparing `python_eol-0.0.2/tox.ini` & `python_eol-0.0.3/tox.ini`

 * *Files 20% similar despite different names*

```diff
@@ -22,34 +22,35 @@
 commands =
     {[testenv]commands}
     coverage report --fail-under 80
 
 [testenv:ruff]
 skip_install = true
 deps = ruff
-commands = ruff check .
+commands = ruff check python_eol/ tests/
 
 [testenv:black]
 skip_install = true
 deps = black
 commands = black --check python_eol/ tests/
 
 [testenv:flake8]
 skip_install = true
 deps = flake8
-commands = flake8
+max-line-length = 88
+commands = flake8 python_eol/ tests/
 
 [testenv:mypy]
 skip_install = true
 deps =
   mypy
   types-setuptools
   types-freezegun
   pytest
-commands = mypy .
+commands = mypy python_eol/ tests/
 
 [testenv:yamlfix]
 skip_install = true
 deps = yamlfix
 commands = yamlfix .
 
 [testenv:lint]
```

