# Comparing `tmp/pkgmt-0.5.0.tar.gz` & `tmp/pkgmt-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgmt-0.5.0.tar", last modified: Fri Apr 28 17:13:47 2023, max compression
+gzip compressed data, was "pkgmt-0.5.1.tar", last modified: Fri May 19 18:51:22 2023, max compression
```

## Comparing `pkgmt-0.5.0.tar` & `pkgmt-0.5.1.tar`

### file list

```diff
@@ -1,58 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:47.865345 pkgmt-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-04-28 17:13:33.000000 pkgmt-0.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-28 17:13:33.000000 pkgmt-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-28 17:13:33.000000 pkgmt-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-28 17:13:47.865345 pkgmt-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-28 17:13:33.000000 pkgmt-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-28 17:13:33.000000 pkgmt-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-28 17:13:47.865345 pkgmt-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-28 17:13:33.000000 pkgmt-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:47.861345 pkgmt-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:47.865345 pkgmt-0.5.0/src/pkgmt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:47.865345 pkgmt-0.5.0/src/pkgmt/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:47.865345 pkgmt-0.5.0/src/pkgmt/assets/template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:47.861345 pkgmt-0.5.0/src/pkgmt/assets/template/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:47.865345 pkgmt-0.5.0/src/pkgmt/assets/template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/assets/template/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/assets/template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/assets/template/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/assets/template/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/assets/template/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/assets/template/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/assets/template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:47.861345 pkgmt-0.5.0/src/pkgmt/assets/template/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:47.865345 pkgmt-0.5.0/src/pkgmt/assets/template/src/name/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/assets/template/src/name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/assets/template/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:47.865345 pkgmt-0.5.0/src/pkgmt/assets/template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/assets/template/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/links.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/new.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:47.865345 pkgmt-0.5.0/src/pkgmt/versioner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/versioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/versioner/abstractversioner.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/versioner/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/versioner/versionernonsetup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-28 17:13:33.000000 pkgmt-0.5.0/src/pkgmt/versioner/versionersetup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:47.865345 pkgmt-0.5.0/src/pkgmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-28 17:13:47.000000 pkgmt-0.5.0/src/pkgmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-28 17:13:47.000000 pkgmt-0.5.0/src/pkgmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 17:13:47.000000 pkgmt-0.5.0/src/pkgmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-28 17:13:47.000000 pkgmt-0.5.0/src/pkgmt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-28 17:13:47.000000 pkgmt-0.5.0/src/pkgmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 17:13:47.000000 pkgmt-0.5.0/src/pkgmt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:22.379885 pkgmt-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-05-19 18:51:06.000000 pkgmt-0.5.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-19 18:51:06.000000 pkgmt-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-19 18:51:06.000000 pkgmt-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-19 18:51:22.379885 pkgmt-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-19 18:51:06.000000 pkgmt-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-19 18:51:06.000000 pkgmt-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-19 18:51:22.379885 pkgmt-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-19 18:51:06.000000 pkgmt-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:22.375885 pkgmt-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:22.375885 pkgmt-0.5.1/src/pkgmt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:22.379885 pkgmt-0.5.1/src/pkgmt/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:22.379885 pkgmt-0.5.1/src/pkgmt/assets/template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:22.379885 pkgmt-0.5.1/src/pkgmt/assets/template/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:22.379885 pkgmt-0.5.1/src/pkgmt/assets/template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:22.375885 pkgmt-0.5.1/src/pkgmt/assets/template/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:22.379885 pkgmt-0.5.1/src/pkgmt/assets/template/src/name/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/src/name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:22.379885 pkgmt-0.5.1/src/pkgmt/assets/template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/assets/template/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:22.379885 pkgmt-0.5.1/src/pkgmt/versioner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/versioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/versioner/abstractversioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/versioner/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/versioner/versionernonsetup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-19 18:51:06.000000 pkgmt-0.5.1/src/pkgmt/versioner/versionersetup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:51:22.379885 pkgmt-0.5.1/src/pkgmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-19 18:51:22.000000 pkgmt-0.5.1/src/pkgmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-19 18:51:22.000000 pkgmt-0.5.1/src/pkgmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:51:22.000000 pkgmt-0.5.1/src/pkgmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-19 18:51:22.000000 pkgmt-0.5.1/src/pkgmt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-19 18:51:22.000000 pkgmt-0.5.1/src/pkgmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 18:51:22.000000 pkgmt-0.5.1/src/pkgmt.egg-info/top_level.txt
```

### Comparing `pkgmt-0.5.0/CHANGELOG.md` & `pkgmt-0.5.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # CHANGELOG
 
+## 0.5.1 (2023-05-19)
+
+* [Feature] Add `tests/conftest.py` to package template ([#7](https://github.com/ploomber/pkgmt/issues/7))
+* [Feature] Add `.github/pull_request_template.md` to package template ([#13](https://github.com/ploomber/pkgmt/issues/13))
+* [Feature] Improvements to `.github/workflows/ci.yml` in package template ([#6](https://github.com/ploomber/pkgmt/issues/6))
+* [Feature] Add `pyproject.toml` to package template ([#10](https://github.com/ploomber/pkgmt/issues/10))
+* [Fix] Fix GitHub handle expansion when username contains `_` or `-`
+* [Fix] Fix harcoded path in `MANIFEST.in` in package template ([#28](https://github.com/ploomber/pkgmt/issues/28))
+
 ## 0.5.0 (2023-04-28)
 
 * [API Change] `pkgmt version` halts if there are uncommitted changes
 
 ## 0.4.2 (2023-04-28)
 
 *No changes*
```

### Comparing `pkgmt-0.5.0/LICENSE` & `pkgmt-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.0/README.md` & `pkgmt-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.0/setup.py` & `pkgmt-0.5.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,16 @@
     # dependencies for linting and formatting
     "black",
     "nbqa",
     "flake8",
     "jupytext",
     # ensure we have a valid IPython version since
     # black needs it
-    "ipython<=8.12.0; python_version == '3.8'",
+    "ipython<=8.12.0; python_version <= '3.8'",
+    "ipython",
 ]
 
 
 DEV = [
     "pytest",
     "twine",
     # optional dependency for test module
```

### Comparing `pkgmt-0.5.0/src/pkgmt/assets/template/.gitignore` & `pkgmt-0.5.1/src/pkgmt/assets/template/.gitignore`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.0/src/pkgmt/assets/template/setup.py` & `pkgmt-0.5.1/src/pkgmt/assets/template/setup.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.0/src/pkgmt/assets/template/tasks.py` & `pkgmt-0.5.1/src/pkgmt/assets/template/tasks.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.0/src/pkgmt/changelog.py` & `pkgmt-0.5.1/src/pkgmt/changelog.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         r"([^\[])#([0-9]+)",
         r"\1[#\2](" + url + r"\2)",
         text,
     )
 
 
 def _replace_handles_with_links(text):
-    pattern = r"(?<!\[)@(\w+)(?!\]\(https:\/\/github\.com\/\w+\))"
+    pattern = r"(?<!\[)@([\w\-_]+)(?!\]\(https:\/\/github\.com\/\w+\))"
     repl = r"[\g<0>](https://github.com/\g<1>)"
     return re.sub(pattern, repl, text)
 
 
 def _expand_github_from_text(text):
     """Convert strings with the #{number} format into their"""
     cfg = config.load()
```

### Comparing `pkgmt-0.5.0/src/pkgmt/cli.py` & `pkgmt-0.5.1/src/pkgmt/cli.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.0/src/pkgmt/config.py` & `pkgmt-0.5.1/src/pkgmt/config.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.0/src/pkgmt/dependencies.py` & `pkgmt-0.5.1/src/pkgmt/dependencies.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.0/src/pkgmt/deprecation.py` & `pkgmt-0.5.1/src/pkgmt/deprecation.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.0/src/pkgmt/dev.py` & `pkgmt-0.5.1/src/pkgmt/dev.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.0/src/pkgmt/formatting.py` & `pkgmt-0.5.1/src/pkgmt/formatting.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.0/src/pkgmt/github.py` & `pkgmt-0.5.1/src/pkgmt/github.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.0/src/pkgmt/hook.py` & `pkgmt-0.5.1/src/pkgmt/hook.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.0/src/pkgmt/links.py` & `pkgmt-0.5.1/src/pkgmt/links.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.0/src/pkgmt/new.py` & `pkgmt-0.5.1/src/pkgmt/new.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,11 +19,18 @@
         # so we trick it
         path = p.parent / "template"
 
     shutil.copytree(path, name)
 
     root = Path(name)
 
-    for file in ("README.md", "setup.py", "tasks.py", "MANIFEST.in"):
+    for file in (
+        "README.md",
+        "setup.py",
+        "tasks.py",
+        "MANIFEST.in",
+        "pyproject.toml",
+        ".github/workflows/ci.yml",
+    ):
         render_inplace(root / file, name=name)
 
     os.rename(root / "src" / "name", root / "src" / name)
```

### Comparing `pkgmt-0.5.0/src/pkgmt/test.py` & `pkgmt-0.5.1/src/pkgmt/test.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.0/src/pkgmt/versioneer.py` & `pkgmt-0.5.1/src/pkgmt/versioneer.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.0/src/pkgmt/versioner/abstractversioner.py` & `pkgmt-0.5.1/src/pkgmt/versioner/abstractversioner.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.0/src/pkgmt/versioner/util.py` & `pkgmt-0.5.1/src/pkgmt/versioner/util.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.0/src/pkgmt/versioner/versionernonsetup.py` & `pkgmt-0.5.1/src/pkgmt/versioner/versionernonsetup.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.0/src/pkgmt/versioner/versionersetup.py` & `pkgmt-0.5.1/src/pkgmt/versioner/versionersetup.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.5.0/src/pkgmt.egg-info/SOURCES.txt` & `pkgmt-0.5.1/src/pkgmt.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -28,18 +28,21 @@
 src/pkgmt.egg-info/requires.txt
 src/pkgmt.egg-info/top_level.txt
 src/pkgmt/assets/__init__.py
 src/pkgmt/assets/template/.gitignore
 src/pkgmt/assets/template/CHANGELOG.md
 src/pkgmt/assets/template/MANIFEST.in
 src/pkgmt/assets/template/README.md
+src/pkgmt/assets/template/pyproject.toml
 src/pkgmt/assets/template/setup.cfg
 src/pkgmt/assets/template/setup.py
 src/pkgmt/assets/template/tasks.py
+src/pkgmt/assets/template/.github/pull_request_template.md
 src/pkgmt/assets/template/.github/workflows/ci.yml
 src/pkgmt/assets/template/src/name/__init__.py
+src/pkgmt/assets/template/tests/conftest.py
 src/pkgmt/assets/template/tests/test_sample.py
 src/pkgmt/versioner/__init__.py
 src/pkgmt/versioner/abstractversioner.py
 src/pkgmt/versioner/util.py
 src/pkgmt/versioner/versionernonsetup.py
 src/pkgmt/versioner/versionersetup.py
```

