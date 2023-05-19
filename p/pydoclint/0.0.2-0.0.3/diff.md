# Comparing `tmp/pydoclint-0.0.2.tar.gz` & `tmp/pydoclint-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoclint-0.0.2.tar", last modified: Tue May 16 08:41:01 2023, max compression
+gzip compressed data, was "pydoclint-0.0.3.tar", last modified: Fri May 19 06:24:32 2023, max compression
```

## Comparing `pydoclint-0.0.2.tar` & `pydoclint-0.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:41:01.770929 pydoclint-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-16 08:40:48.000000 pydoclint-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-05-16 08:41:01.770929 pydoclint-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-05-16 08:40:48.000000 pydoclint-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:41:01.770929 pydoclint-0.0.2/pydoclint/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/flake8_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/internal_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/method_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:41:01.770929 pydoclint-0.0.2/pydoclint/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/utils/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/utils/astTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/utils/return_yield_raise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/utils/walk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/violation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:41:01.770929 pydoclint-0.0.2/pydoclint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-05-16 08:41:01.000000 pydoclint-0.0.2/pydoclint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-16 08:41:01.000000 pydoclint-0.0.2/pydoclint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:41:01.000000 pydoclint-0.0.2/pydoclint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-16 08:41:01.000000 pydoclint-0.0.2/pydoclint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-16 08:41:01.000000 pydoclint-0.0.2/pydoclint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 08:41:01.000000 pydoclint-0.0.2/pydoclint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-16 08:41:01.774929 pydoclint-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-16 08:40:48.000000 pydoclint-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:41:01.770929 pydoclint-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-05-16 08:40:48.000000 pydoclint-0.0.2/tests/test_arg.py
--rw-r--r--   0 runner    (1001) docker     (123)    20192 2023-05-16 08:40:48.000000 pydoclint-0.0.2/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:24:32.877374 pydoclint-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-19 06:24:18.000000 pydoclint-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-05-19 06:24:32.877374 pydoclint-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-05-19 06:24:18.000000 pydoclint-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:24:32.873373 pydoclint-0.0.3/pydoclint/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/flake8_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:24:32.877374 pydoclint-0.0.3/pydoclint/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/utils/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/utils/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/utils/astTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/utils/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/utils/internal_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/utils/method_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/utils/return_yield_raise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/utils/violation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/utils/walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12357 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pydoclint/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:24:32.873373 pydoclint-0.0.3/pydoclint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-05-19 06:24:32.000000 pydoclint-0.0.3/pydoclint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-19 06:24:32.000000 pydoclint-0.0.3/pydoclint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 06:24:32.000000 pydoclint-0.0.3/pydoclint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-19 06:24:32.000000 pydoclint-0.0.3/pydoclint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-19 06:24:32.000000 pydoclint-0.0.3/pydoclint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 06:24:32.000000 pydoclint-0.0.3/pydoclint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-19 06:24:18.000000 pydoclint-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-19 06:24:32.877374 pydoclint-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-19 06:24:18.000000 pydoclint-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:24:32.877374 pydoclint-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21080 2023-05-19 06:24:18.000000 pydoclint-0.0.3/tests/test_main.py
```

### Comparing `pydoclint-0.0.2/LICENSE` & `pydoclint-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.2/PKG-INFO` & `pydoclint-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoclint
-Version: 0.0.2
+Version: 0.0.3
 Summary: A linter to check arguments in Python docstrings
 Home-page: https://github.com/jsh9/pydoclint
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
@@ -23,19 +23,23 @@
 Here is a comparison of linting time on some famous Python projects:
 
 |                                                              | pydoclint | darglint                          |
 | ------------------------------------------------------------ | --------- | --------------------------------- |
 | [numpy](https://github.com/numpy/numpy)                      | 2.0 sec   | 49 min 9 sec (1,475x slower)      |
 | [scikit-learn](https://github.com/scikit-learn/scikit-learn) | 2.4 sec   | 3 hr 5 min 33 sec (4,639x slower) |
 
-Currently, _pydoclint_ only works when you write your docstrings in the
-[numpy stlyle](https://numpydoc.readthedocs.io/en/latest/format.html). Support
-for the
-[Google style](https://www.sphinx-doc.org/en/master/usage/extensions/example_google.html)
-docstrings will be added soon.
+Currently, _pydoclint_ supports two docstring styles:
+
+- The [numpy stlyle](https://numpydoc.readthedocs.io/en/latest/format.html)
+- The
+  [Google style](https://www.sphinx-doc.org/en/master/usage/extensions/example_google.html)
+
+Support for the
+[Sphinx style](https://sphinx-rtd-tutorial.readthedocs.io/en/latest/docstrings.html)
+may be added in the future if there are requests for it.
 
 Another note: this linter and [pydocstyle](https://github.com/PyCQA/pydocstyle)
 serves complementary purposes. It is recommended that you use both together.
 
 ## 1. Installation
 
 ```
@@ -154,15 +158,30 @@
 pydoclint --exclude='\.git|\.tox|tests/data' <FOLDER_NAME>
 ```
 
 This option is only available in the native command-line mode. If you use
 _pydoclint_ within _flake8_, you can use _flake8_'s
 [`--exclude` option](https://flake8.pycqa.org/en/latest/user/options.html#cmdoption-flake8-exclude).
 
-### 4.3. `--check-type-hint` (shortform: `-th`, default: `True`)
+### 4.3. `--style`
+
+Which style of docstring is your code base using. Right now there are two
+available choices: `numpy` and `google`. The default value is `numpy`.
+
+```
+pydoclint --style=google <FILE_OR_FOLDER>
+```
+
+or
+
+```
+flake8 --style=google <FILE_OR_FOLDER>
+```
+
+### 4.4. `--check-type-hint` (shortform: `-th`, default: `True`)
 
 If `True`, the type hints in the docstring and in the Python code need to
 exactly match.
 
 To turn this optoin on/off, do this:
 
 ```
@@ -171,15 +190,15 @@
 
 or
 
 ```
 flake8 --check-type-hint=False <FILE_OR_FOLDER>
 ```
 
-### 4.4. `--check-arg-order` (shortform: `-ao`, default: `True`)
+### 4.5. `--check-arg-order` (shortform: `-ao`, default: `True`)
 
 If `True`, the input argument order in the docstring needs to match that in the
 function signature.
 
 To turn this optoin on/off, do this:
 
 ```
@@ -188,15 +207,15 @@
 
 or
 
 ```
 flake8 --check-arg-order=False <FILE_OR_FOLDER>
 ```
 
-### 4.5. `--skip-checking-short-docstrings` (shortform: `-scsd`, default: `True`)
+### 4.6. `--skip-checking-short-docstrings` (shortform: `-scsd`, default: `True`)
 
 If `True`, `pydoclint` won't check functions that have only a short description
 in their docstring.
 
 To turn this optoin on/off, do this:
 
 ```
@@ -205,12 +224,12 @@
 
 or
 
 ```
 flake8 --skip-checking-short-docstrings=False <FILE_OR_FOLDER>
 ```
 
-### 4.6. `--skip-checking-raises` (shortform: `-scr`, default: `False`)
+### 4.7. `--skip-checking-raises` (shortform: `-scr`, default: `False`)
 
 If `True`, _pydoclint_ won't report `DOC501` or `DOC502` if there are `raise`
 statements in the function/method but there aren't any "raises" sections in the
 docstring (or vice versa).
```

### Comparing `pydoclint-0.0.2/README.md` & `pydoclint-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,23 @@
 Here is a comparison of linting time on some famous Python projects:
 
 |                                                              | pydoclint | darglint                          |
 | ------------------------------------------------------------ | --------- | --------------------------------- |
 | [numpy](https://github.com/numpy/numpy)                      | 2.0 sec   | 49 min 9 sec (1,475x slower)      |
 | [scikit-learn](https://github.com/scikit-learn/scikit-learn) | 2.4 sec   | 3 hr 5 min 33 sec (4,639x slower) |
 
-Currently, _pydoclint_ only works when you write your docstrings in the
-[numpy stlyle](https://numpydoc.readthedocs.io/en/latest/format.html). Support
-for the
-[Google style](https://www.sphinx-doc.org/en/master/usage/extensions/example_google.html)
-docstrings will be added soon.
+Currently, _pydoclint_ supports two docstring styles:
+
+- The [numpy stlyle](https://numpydoc.readthedocs.io/en/latest/format.html)
+- The
+  [Google style](https://www.sphinx-doc.org/en/master/usage/extensions/example_google.html)
+
+Support for the
+[Sphinx style](https://sphinx-rtd-tutorial.readthedocs.io/en/latest/docstrings.html)
+may be added in the future if there are requests for it.
 
 Another note: this linter and [pydocstyle](https://github.com/PyCQA/pydocstyle)
 serves complementary purposes. It is recommended that you use both together.
 
 ## 1. Installation
 
 ```
@@ -141,15 +145,30 @@
 pydoclint --exclude='\.git|\.tox|tests/data' <FOLDER_NAME>
 ```
 
 This option is only available in the native command-line mode. If you use
 _pydoclint_ within _flake8_, you can use _flake8_'s
 [`--exclude` option](https://flake8.pycqa.org/en/latest/user/options.html#cmdoption-flake8-exclude).
 
-### 4.3. `--check-type-hint` (shortform: `-th`, default: `True`)
+### 4.3. `--style`
+
+Which style of docstring is your code base using. Right now there are two
+available choices: `numpy` and `google`. The default value is `numpy`.
+
+```
+pydoclint --style=google <FILE_OR_FOLDER>
+```
+
+or
+
+```
+flake8 --style=google <FILE_OR_FOLDER>
+```
+
+### 4.4. `--check-type-hint` (shortform: `-th`, default: `True`)
 
 If `True`, the type hints in the docstring and in the Python code need to
 exactly match.
 
 To turn this optoin on/off, do this:
 
 ```
@@ -158,15 +177,15 @@
 
 or
 
 ```
 flake8 --check-type-hint=False <FILE_OR_FOLDER>
 ```
 
-### 4.4. `--check-arg-order` (shortform: `-ao`, default: `True`)
+### 4.5. `--check-arg-order` (shortform: `-ao`, default: `True`)
 
 If `True`, the input argument order in the docstring needs to match that in the
 function signature.
 
 To turn this optoin on/off, do this:
 
 ```
@@ -175,15 +194,15 @@
 
 or
 
 ```
 flake8 --check-arg-order=False <FILE_OR_FOLDER>
 ```
 
-### 4.5. `--skip-checking-short-docstrings` (shortform: `-scsd`, default: `True`)
+### 4.6. `--skip-checking-short-docstrings` (shortform: `-scsd`, default: `True`)
 
 If `True`, `pydoclint` won't check functions that have only a short description
 in their docstring.
 
 To turn this optoin on/off, do this:
 
 ```
@@ -192,12 +211,12 @@
 
 or
 
 ```
 flake8 --skip-checking-short-docstrings=False <FILE_OR_FOLDER>
 ```
 
-### 4.6. `--skip-checking-raises` (shortform: `-scr`, default: `False`)
+### 4.7. `--skip-checking-raises` (shortform: `-scr`, default: `False`)
 
 If `True`, _pydoclint_ won't report `DOC501` or `DOC502` if there are `raise`
 statements in the function/method but there aren't any "raises" sections in the
 docstring (or vice versa).
```

### Comparing `pydoclint-0.0.2/pydoclint/arg.py` & `pydoclint-0.0.3/pydoclint/utils/arg.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import ast
-from typing import List, Set
+from typing import List, Optional, Set
 
+from docstring_parser.common import DocstringParam
 from numpydoc.docscrape import Parameter
 
 from pydoclint.utils.annotation import parseAnnotation
 
 
 class Arg:
     """
@@ -57,20 +58,29 @@
 
     @classmethod
     def fromNumpydocParam(cls, param: Parameter) -> 'Arg':
         """Construct an Arg object from a Numpydoc Parameter object"""
         return Arg(name=param.name, typeHint=param.type)
 
     @classmethod
+    def fromGoogleParsedParam(cls, param: DocstringParam) -> 'Arg':
+        """Construct an Arg object from a GoogleParser Parameter object"""
+        return Arg(name=param.arg_name, typeHint=cls._str(param.type_name))
+
+    @classmethod
     def fromAstArg(cls, astArg: ast.arg) -> 'Arg':
         """Construct an Arg object from a Python AST argument object"""
         anno = astArg.annotation
         typeHint: str = '' if anno is None else parseAnnotation(anno)
         return Arg(name=astArg.arg, typeHint=typeHint)
 
+    @classmethod
+    def _str(cls, typeName: Optional[str]) -> str:
+        return '' if typeName is None else typeName
+
 
 class ArgList:
     """
     A class to hold a list of `Arg` objects.
 
     This class also defines some behaviors of an argument list, such as
     equality, length calculation, etc.
```

### Comparing `pydoclint-0.0.2/pydoclint/flake8_entry.py` & `pydoclint-0.0.3/pydoclint/flake8_entry.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,20 @@
 
     def __init__(self, tree: ast.AST) -> None:
         self._tree = tree
 
     @classmethod
     def add_options(cls, parser):  # noqa: D102
         parser.add_option(
+            '--style',
+            action='store',
+            default='numpy',
+            help='Which style of docstring is your code base using',
+        )
+        parser.add_option(
             '-th',
             '--check-type-hint',
             action='store',
             default='True',
             help='Whether to check type hints in the docstring',
         )
         parser.add_option(
@@ -52,33 +58,40 @@
     def parse_options(cls, options):  # noqa: D102
         cls.check_type_hint = options.check_type_hint
         cls.check_arg_order = options.check_arg_order
         cls.skip_checking_short_docstrings = (
             options.skip_checking_short_docstrings
         )
         cls.skip_checking_raises = options.skip_checking_raises
+        cls.style = options.style
 
     def run(self) -> Generator[Tuple[int, int, str, Any], None, None]:
         """Run the linter and yield the violation information"""
         checkTypeHint = self._bool('--check-type-hint', self.check_type_hint)
         checkArgOrder = self._bool('--check-arg-order', self.check_arg_order)
         skipCheckingShortDocstrings = self._bool(
             '--skip-checking-short-docstrings',
             self.skip_checking_short_docstrings,
         )
         skipCheckingRaises = self._bool(
             '--skip-checking-raises',
             self.skip_checking_raises,
         )
 
+        if self.style not in {'numpy', 'google'}:
+            raise ValueError(
+                'Invalid value for "--style": must be "numpy" or "google"'
+            )
+
         v = Visitor(
             checkTypeHint=checkTypeHint,
             checkArgOrder=checkArgOrder,
             skipCheckingShortDocstrings=skipCheckingShortDocstrings,
             skipCheckingRaises=skipCheckingRaises,
+            style=self.style,
         )
         v.visit(self._tree)
         violationInfo = [_.getInfoForFlake8() for _ in v.violations]
         for line, colOffset, msg in violationInfo:
             yield line, colOffset, msg, type(self)
 
     @classmethod
```

### Comparing `pydoclint-0.0.2/pydoclint/main.py` & `pydoclint-0.0.3/pydoclint/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 import ast
 import re
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple
 
 import click
 
-from pydoclint.violation import Violation
+from pydoclint.utils.violation import Violation
 from pydoclint.visitor import Visitor
 
 
+def validateStyleValue(
+        context: click.Context,
+        param: click.Parameter,
+        value: Optional[str],
+) -> Optional[str]:
+    """Validate the value of the 'style' option"""
+    if value not in {'numpy', 'google'}:
+        raise click.BadParameter('"--style" must be "numpy" or "google"')
+
+    return value
+
+
 @click.command(
     context_settings={'help_option_names': ['-h', '--help']},
     # While Click does set this field automatically using the docstring, mypyc
     # (annoyingly) strips them, so we need to set it here too.
     help='Yes',
 )
 @click.option(
@@ -36,14 +48,22 @@
     help=(
         'Regex pattern to exclude files/folders. Please add quotes (both'
         ' double and single quotes are fine) around the regex in the'
         ' command line.'
     ),
 )
 @click.option(
+    '--style',
+    type=str,
+    show_default=True,
+    default='numpy',
+    callback=validateStyleValue,
+    help='',
+)
+@click.option(
     '-th',
     '--check-type-hint',
     type=bool,
     show_default=True,
     default=True,
     help='Whether to check type hints in docstrings',
 )
@@ -84,14 +104,15 @@
     is_eager=True,
 )
 @click.pass_context
 def main(
         ctx: click.Context,
         quiet: bool,
         exclude: str,
+        style: str,
         src: Optional[str],
         paths: Tuple[str, ...],
         check_type_hint: bool,
         check_arg_order: bool,
         skip_checking_short_docstrings: bool,
         skip_checking_raises: bool,
 ) -> None:
@@ -110,14 +131,15 @@
             main.get_usage(ctx) + "\n\nOne of 'paths' or 'src' is required."
         )
         ctx.exit(1)
 
     violationsInAllFiles: Dict[str, List[Violation]] = _checkPaths(
         quiet=quiet,
         exclude=exclude,
+        style=style,
         paths=paths,
         checkTypeHint=check_type_hint,
         checkArgOrder=check_arg_order,
         skipCheckingShortDocstrings=skip_checking_short_docstrings,
         skipCheckingRaises=skip_checking_raises,
     )
 
@@ -153,14 +175,15 @@
             click.echo(click.style('🎉 No violations 🎉', fg='green', bold=True))
 
         ctx.exit(0)
 
 
 def _checkPaths(
         paths: Tuple[str, ...],
+        style: str = 'numpy',
         checkTypeHint: bool = True,
         checkArgOrder: bool = True,
         skipCheckingShortDocstrings: bool = True,
         skipCheckingRaises: bool = False,
         quiet: bool = False,
         exclude: str = '',
 ) -> Dict[str, List[Violation]]:
@@ -186,36 +209,39 @@
             continue
 
         if not quiet:
             click.echo(click.style(filename, fg='cyan', bold=True))
 
         violationsInThisFile: List[Violation] = _checkFile(
             filename,
+            style=style,
             checkTypeHint=checkTypeHint,
             checkArgOrder=checkArgOrder,
             skipCheckingShortDocstrings=skipCheckingShortDocstrings,
             skipCheckingRaises=skipCheckingRaises,
         )
         allViolations[filename.as_posix()] = violationsInThisFile
 
     return allViolations
 
 
 def _checkFile(
         filename: Path,
+        style: str = 'numpy',
         checkTypeHint: bool = True,
         checkArgOrder: bool = True,
         skipCheckingShortDocstrings: bool = True,
         skipCheckingRaises: bool = False,
 ) -> List[Violation]:
     with open(filename) as fp:
         src: str = ''.join(fp.readlines())
 
     tree: ast.Module = ast.parse(src)
     visitor = Visitor(
+        style=style,
         checkTypeHint=checkTypeHint,
         checkArgOrder=checkArgOrder,
         skipCheckingShortDocstrings=skipCheckingShortDocstrings,
         skipCheckingRaises=skipCheckingRaises,
     )
     visitor.visit(tree)
     return visitor.violations
```

### Comparing `pydoclint-0.0.2/pydoclint/utils/annotation.py` & `pydoclint-0.0.3/pydoclint/utils/annotation.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.2/pydoclint/utils/return_yield_raise.py` & `pydoclint-0.0.3/pydoclint/utils/return_yield_raise.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.2/pydoclint/utils/walk.py` & `pydoclint-0.0.3/pydoclint/utils/walk.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.2/pydoclint/violation.py` & `pydoclint-0.0.3/pydoclint/utils/violation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import types
 from typing import Tuple
 
-from pydoclint.internal_error import InternalError
+from pydoclint.utils.internal_error import InternalError
 
 VIOLATION_CODES = types.MappingProxyType({
     101: 'Docstring contains fewer arguments than in function signature.',
     102: 'Docstring contains more arguments than in function signature.',
     103: (  # noqa: PAR001
         'Docstring arguments are different from function arguments.'
         ' (Or did you miss the space between the argument name'
```

### Comparing `pydoclint-0.0.2/pydoclint/visitor.py` & `pydoclint-0.0.3/pydoclint/visitor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import ast
 from typing import List, Optional, Set
 
-from numpydoc.docscrape import NumpyDocString, Parameter
-
-from pydoclint.arg import Arg, ArgList
-from pydoclint.method_type import MethodType
+from pydoclint.utils.arg import Arg, ArgList
 from pydoclint.utils.astTypes import FuncOrAsyncFuncDef
+from pydoclint.utils.doc import Doc
 from pydoclint.utils.generic import (
     collectFuncArgs,
     detectMethodType,
     generateMsgPrefix,
     getDocstring,
-    isShortDocstring,
 )
+from pydoclint.utils.method_type import MethodType
 from pydoclint.utils.return_yield_raise import (
     hasGeneratorAsReturnAnnotation,
     hasRaiseStatements,
     hasReturnAnnotation,
     hasReturnStatements,
     hasYieldStatements,
 )
-from pydoclint.violation import Violation
+from pydoclint.utils.violation import Violation
 
 
 class Visitor(ast.NodeVisitor):
     """A class to recursively visit all the nodes in a parsed module"""
 
     def __init__(
             self,
+            style: str = 'numpy',
             checkTypeHint: bool = True,
             checkArgOrder: bool = True,
             skipCheckingShortDocstrings: bool = True,
             skipCheckingRaises: bool = False,
     ) -> None:
+        self.style: str = style
         self.checkTypeHint: bool = checkTypeHint
         self.checkArgOrder: bool = checkArgOrder
         self.skipCheckingShortDocstrings: bool = skipCheckingShortDocstrings
         self.skipCheckingRaises: bool = skipCheckingRaises
 
         self.parent: Optional[ast.AST] = None  # keep track of parent node
         self.violations: List[Violation] = []
@@ -86,23 +86,16 @@
             # or pydocstyle (https://www.pydocstyle.org/en/stable/)
             # to determine whether a function needs a docstring.
             argViolations = []
             returnViolations = []
             yieldViolations = []
             raiseViolations = []
         else:
-            # Note: a NumpyDocString object has the following sections:
-            # *  {'Signature': '', 'Summary': [''], 'Extended Summary': [],
-            # *  'Parameters': [], 'Returns': [], 'Yields': [], 'Receives': [],
-            # *  'Raises': [], 'Warns': [], 'Other Parameters': [],
-            # *  'Attributes': [], 'Methods': [], 'See Also': [], 'Notes': [],
-            # *  'Warnings': [], 'References': '', 'Examples': '', 'index': {}}
-            doc: NumpyDocString = NumpyDocString(docstring)
-
-            isShort: bool = isShortDocstring(doc)
+            doc: Doc = Doc(docstring=docstring, style=self.style)
+            isShort: bool = doc.isShortDocstring
             if self.skipCheckingShortDocstrings and isShort:
                 argViolations = []
                 returnViolations = []
                 yieldViolations = []
                 raiseViolations = []
             else:
                 argViolations = self.checkArguments(node, parent_, doc)
@@ -118,15 +111,15 @@
                     else:
                         raiseViolations = []
 
             if isClassConstructor:
                 # Re-check return violations because the rules are
                 # different for class constructors.
                 returnViolations = self.checkReturnsInClassConstructor(
-                    parent=parent_, nonEmptyDocStruct=doc
+                    parent=parent_, doc=doc
                 )
 
         self.violations.extend(argViolations)
         self.violations.extend(returnViolations)
         self.violations.extend(yieldViolations)
         self.violations.extend(raiseViolations)
 
@@ -137,94 +130,57 @@
     def visit_AsyncFunctionDef(self, node: ast.AsyncFunctionDef):  # noqa: D102
         # Treat async functions similarly to regular ones
         self.visit_FunctionDef(node)
 
     def visit_Raise(self, node: ast.Raise):  # noqa: D102
         self.generic_visit(node)
 
-    def checkArguments(
+    def checkArguments(  # noqa: C901
             self,
             node: FuncOrAsyncFuncDef,
             parent_: ast.AST,
-            docstringStruct: NumpyDocString,
+            doc: Doc,
     ) -> List[Violation]:
         """
         Check input arguments of the function.
 
         Parameters
         ----------
         node : FuncOrAsyncFuncDef
             The current function node.  It can be a regular function
             or an async function.
         parent_ : ast.AST
             The parent of the current node, which can be another function,
             a class, etc.
-        docstringStruct : NumpyDocString
+        doc : Doc
             The parsed docstring structure.
 
         Returns
         -------
         List[Violation]
             A list of argument violations
         """
-        argList: List[ast.arg] = collectFuncArgs(node)
+        astArgList: List[ast.arg] = collectFuncArgs(node)
 
         isMethod: bool = isinstance(parent_, ast.ClassDef)
         msgPrefix: str = generateMsgPrefix(node, parent_, appendColon=True)
 
         if isMethod:
             mType: MethodType = detectMethodType(node)
             if mType in {MethodType.INSTANCE_METHOD, MethodType.CLASS_METHOD}:
-                argList = argList[1:]  # no need to document `self` and `cls`
-
-        docArgList: List[Parameter] = docstringStruct.get('Parameters', [])
-
-        return self.validateDocArgs(
-            docArgList=docArgList,
-            actualArgs=argList,
-            node=node,
-            msgPrefix=msgPrefix,
-        )
-
-    def validateDocArgs(  # noqa: C901
-            self,
-            docArgList: List[Parameter],
-            actualArgs: List[ast.arg],
-            node: FuncOrAsyncFuncDef,
-            msgPrefix: str,
-    ) -> List[Violation]:
-        """
-        Validate the argument list in the docstring against the "actual"
-        arguments (the argument list in the function signature).
-
-        Parameters
-        ----------
-        docArgList : List[Parameter]
-            The argument list from the docstring
-        actualArgs : List[ast.arg]
-            The argument list from the function signature
-        node : FuncOrAsyncFuncDef
-            The current function node
-        msgPrefix : str
-            The prefix to be used in the violation message
+                astArgList = astArgList[1:]  # no need to document self/cls
 
-        Returns
-        -------
-        List[Violation]
-            A list of argument violations. It can be empty.
-        """
         lineNum: int = node.lineno
-
         v101 = Violation(code=101, line=lineNum, msgPrefix=msgPrefix)
         v102 = Violation(code=102, line=lineNum, msgPrefix=msgPrefix)
         v104 = Violation(code=104, line=lineNum, msgPrefix=msgPrefix)
         v105 = Violation(code=105, line=lineNum, msgPrefix=msgPrefix)
 
-        docArgs = ArgList([Arg.fromNumpydocParam(_) for _ in docArgList])
-        funcArgs = ArgList([Arg.fromAstArg(_) for _ in actualArgs])
+        docArgs = doc.argList
+        funcArgs = ArgList([Arg.fromAstArg(_) for _ in astArgList])
 
         if docArgs.length() == 0 and funcArgs.length() == 0:
             return []
 
         violations: List[Violation] = []
         if docArgs.length() < funcArgs.length():
             violations.append(v101)
@@ -285,28 +241,28 @@
         return violations
 
     @classmethod
     def checkReturns(
             cls,
             node: FuncOrAsyncFuncDef,
             parent: ast.AST,
-            nonEmptyDocStruct: NumpyDocString,
+            doc: Doc,
     ) -> List[Violation]:
         """Check return statement & return type annotation of this function"""
         lineNum: int = node.lineno
         msgPrefix = generateMsgPrefix(node, parent, appendColon=False)
 
         v201 = Violation(code=201, line=lineNum, msgPrefix=msgPrefix)
         v202 = Violation(code=202, line=lineNum, msgPrefix=msgPrefix)
 
         hasReturnStmt: bool = hasReturnStatements(node)
         hasReturnAnno: bool = hasReturnAnnotation(node)
         hasGenAsRetAnno: bool = hasGeneratorAsReturnAnnotation(node)
 
-        docstringHasReturnSection = bool(nonEmptyDocStruct.get('Returns'))
+        docstringHasReturnSection: bool = doc.hasReturnsSection
 
         violations: List[Violation] = []
         if not docstringHasReturnSection:
             if hasReturnStmt or (hasReturnAnno and not hasGenAsRetAnno):
                 # If "Generator[...]" is put in the return type annotation,
                 # we don't need a "Returns" section in the docstring. Instead,
                 # we need a "Yields" section.
@@ -317,22 +273,19 @@
 
         return violations
 
     @classmethod
     def checkReturnsInClassConstructor(
             cls,
             parent: ast.ClassDef,
-            nonEmptyDocStruct: NumpyDocString,
+            doc: Doc,
     ) -> List[Violation]:
         """Check the presence of a "Returns" section in class docstring"""
         violations: List[Violation] = []
-
-        docstringHasReturnSection = bool(nonEmptyDocStruct.get('Returns'))
-
-        if docstringHasReturnSection:
+        if doc.hasReturnsSection:
             violations.append(
                 Violation(
                     code=302,
                     line=parent.lineno,
                     msgPrefix=f'Class `{parent.name}`:',
                 )
             )
@@ -340,27 +293,28 @@
         return violations
 
     @classmethod
     def checkYields(
             cls,
             node: FuncOrAsyncFuncDef,
             parent: ast.AST,
-            nonEmptyDocStruct: NumpyDocString,
+            doc: Doc,
     ) -> List[Violation]:
         """Check violations on 'yield' statements or 'Generator' annotation"""
         violations: List[Violation] = []
 
         lineNum: int = node.lineno
         msgPrefix = generateMsgPrefix(node, parent, appendColon=False)
 
         v401 = Violation(code=401, line=lineNum, msgPrefix=msgPrefix)
         v402 = Violation(code=402, line=lineNum, msgPrefix=msgPrefix)
         v403 = Violation(code=403, line=lineNum, msgPrefix=msgPrefix)
 
-        docstringHasYieldsSection = bool(nonEmptyDocStruct.get('Yields'))
+        docstringHasYieldsSection: bool = doc.hasYieldsSection
+
         hasYieldStmt: bool = hasYieldStatements(node)
         hasGenAsRetAnno: bool = hasGeneratorAsReturnAnnotation(node)
 
         if not docstringHasYieldsSection:
             if hasGenAsRetAnno:
                 violations.append(v401)
 
@@ -374,26 +328,26 @@
         return violations
 
     @classmethod
     def checkRaises(
             cls,
             node: FuncOrAsyncFuncDef,
             parent: ast.AST,
-            nonEmptyDocStruct: NumpyDocString,
+            doc: Doc,
     ) -> List[Violation]:
         """Check violations on 'raise' statements"""
         violations: List[Violation] = []
 
         lineNum: int = node.lineno
         msgPrefix = generateMsgPrefix(node, parent, appendColon=False)
 
         v501 = Violation(code=501, line=lineNum, msgPrefix=msgPrefix)
         v502 = Violation(code=502, line=lineNum, msgPrefix=msgPrefix)
 
-        docstringHasRaisesSection = bool(nonEmptyDocStruct.get('Raises'))
+        docstringHasRaisesSection: bool = doc.hasRaisesSection
         hasRaiseStmt: bool = hasRaiseStatements(node)
 
         if hasRaiseStmt and not docstringHasRaisesSection:
             violations.append(v501)
 
         if not hasRaiseStmt and docstringHasRaisesSection:
             violations.append(v502)
```

### Comparing `pydoclint-0.0.2/pydoclint.egg-info/PKG-INFO` & `pydoclint-0.0.3/pydoclint.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoclint
-Version: 0.0.2
+Version: 0.0.3
 Summary: A linter to check arguments in Python docstrings
 Home-page: https://github.com/jsh9/pydoclint
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
@@ -23,19 +23,23 @@
 Here is a comparison of linting time on some famous Python projects:
 
 |                                                              | pydoclint | darglint                          |
 | ------------------------------------------------------------ | --------- | --------------------------------- |
 | [numpy](https://github.com/numpy/numpy)                      | 2.0 sec   | 49 min 9 sec (1,475x slower)      |
 | [scikit-learn](https://github.com/scikit-learn/scikit-learn) | 2.4 sec   | 3 hr 5 min 33 sec (4,639x slower) |
 
-Currently, _pydoclint_ only works when you write your docstrings in the
-[numpy stlyle](https://numpydoc.readthedocs.io/en/latest/format.html). Support
-for the
-[Google style](https://www.sphinx-doc.org/en/master/usage/extensions/example_google.html)
-docstrings will be added soon.
+Currently, _pydoclint_ supports two docstring styles:
+
+- The [numpy stlyle](https://numpydoc.readthedocs.io/en/latest/format.html)
+- The
+  [Google style](https://www.sphinx-doc.org/en/master/usage/extensions/example_google.html)
+
+Support for the
+[Sphinx style](https://sphinx-rtd-tutorial.readthedocs.io/en/latest/docstrings.html)
+may be added in the future if there are requests for it.
 
 Another note: this linter and [pydocstyle](https://github.com/PyCQA/pydocstyle)
 serves complementary purposes. It is recommended that you use both together.
 
 ## 1. Installation
 
 ```
@@ -154,15 +158,30 @@
 pydoclint --exclude='\.git|\.tox|tests/data' <FOLDER_NAME>
 ```
 
 This option is only available in the native command-line mode. If you use
 _pydoclint_ within _flake8_, you can use _flake8_'s
 [`--exclude` option](https://flake8.pycqa.org/en/latest/user/options.html#cmdoption-flake8-exclude).
 
-### 4.3. `--check-type-hint` (shortform: `-th`, default: `True`)
+### 4.3. `--style`
+
+Which style of docstring is your code base using. Right now there are two
+available choices: `numpy` and `google`. The default value is `numpy`.
+
+```
+pydoclint --style=google <FILE_OR_FOLDER>
+```
+
+or
+
+```
+flake8 --style=google <FILE_OR_FOLDER>
+```
+
+### 4.4. `--check-type-hint` (shortform: `-th`, default: `True`)
 
 If `True`, the type hints in the docstring and in the Python code need to
 exactly match.
 
 To turn this optoin on/off, do this:
 
 ```
@@ -171,15 +190,15 @@
 
 or
 
 ```
 flake8 --check-type-hint=False <FILE_OR_FOLDER>
 ```
 
-### 4.4. `--check-arg-order` (shortform: `-ao`, default: `True`)
+### 4.5. `--check-arg-order` (shortform: `-ao`, default: `True`)
 
 If `True`, the input argument order in the docstring needs to match that in the
 function signature.
 
 To turn this optoin on/off, do this:
 
 ```
@@ -188,15 +207,15 @@
 
 or
 
 ```
 flake8 --check-arg-order=False <FILE_OR_FOLDER>
 ```
 
-### 4.5. `--skip-checking-short-docstrings` (shortform: `-scsd`, default: `True`)
+### 4.6. `--skip-checking-short-docstrings` (shortform: `-scsd`, default: `True`)
 
 If `True`, `pydoclint` won't check functions that have only a short description
 in their docstring.
 
 To turn this optoin on/off, do this:
 
 ```
@@ -205,12 +224,12 @@
 
 or
 
 ```
 flake8 --skip-checking-short-docstrings=False <FILE_OR_FOLDER>
 ```
 
-### 4.6. `--skip-checking-raises` (shortform: `-scr`, default: `False`)
+### 4.7. `--skip-checking-raises` (shortform: `-scr`, default: `False`)
 
 If `True`, _pydoclint_ won't report `DOC501` or `DOC502` if there are `raise`
 statements in the function/method but there aren't any "raises" sections in the
 docstring (or vice versa).
```

### Comparing `pydoclint-0.0.2/pydoclint.egg-info/SOURCES.txt` & `pydoclint-0.0.3/pydoclint.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 pydoclint/__init__.py
-pydoclint/arg.py
 pydoclint/flake8_entry.py
-pydoclint/internal_error.py
 pydoclint/main.py
-pydoclint/method_type.py
-pydoclint/violation.py
 pydoclint/visitor.py
 pydoclint.egg-info/PKG-INFO
 pydoclint.egg-info/SOURCES.txt
 pydoclint.egg-info/dependency_links.txt
 pydoclint.egg-info/entry_points.txt
 pydoclint.egg-info/requires.txt
 pydoclint.egg-info/top_level.txt
 pydoclint/utils/__init__.py
 pydoclint/utils/annotation.py
+pydoclint/utils/arg.py
 pydoclint/utils/astTypes.py
+pydoclint/utils/doc.py
 pydoclint/utils/generic.py
+pydoclint/utils/internal_error.py
+pydoclint/utils/method_type.py
 pydoclint/utils/return_yield_raise.py
+pydoclint/utils/violation.py
 pydoclint/utils/walk.py
-tests/test_arg.py
 tests/test_main.py
```

### Comparing `pydoclint-0.0.2/setup.cfg` & `pydoclint-0.0.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pydoclint
-version = 0.0.2
+version = 0.0.3
 description = A linter to check arguments in Python docstrings
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jsh9/pydoclint
 license = MIT
 license_file = LICENSE
 classifiers = 
@@ -14,14 +14,15 @@
 
 [options]
 packages = find:
 install_requires = 
 	flake8>=4
 	click>=8.0.0
 	numpydoc>=1.5.0
+	docstring_parser>=0.15
 python_requires = >=3.8
 
 [options.packages.find]
 exclude = 
 	tests*
 	testing*
```

### Comparing `pydoclint-0.0.2/tests/test_main.py` & `pydoclint-0.0.3/tests/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,49 +178,58 @@
     'true_false',
     'false_true',
     'false_false',
 ]
 
 
 @pytest.mark.parametrize(
-    'filename, option',
+    'style, filename, option',
     list(
         itertools.product(
+            ['numpy', 'google'],
             ['function.py', 'classmethod.py', 'method.py', 'staticmethod.py'],
             options,
         ),
     ),
 )
 def testArguments(
+        style: str,
         filename: str,
         option: str,
 ) -> None:
     optionDict: Dict[str, bool] = optionDictLookup[option]
     expectedViolations: List[str] = expectedViolationsLookup[option]
 
     expectedViolationsCopy = copy.deepcopy(expectedViolations)
     if filename == 'function.py':
         _tweakViolationMsgForFunctions(expectedViolationsCopy)
 
     violations = _checkFile(
-        filename=DATA_DIR / f'args/{filename}',
+        filename=DATA_DIR / f'{style}/args/{filename}',
         checkTypeHint=optionDict['checkTypeHint'],
         checkArgOrder=optionDict['checkArgOrder'],
+        style=style,
     )
     assert list(map(str, violations)) == expectedViolationsCopy
 
 
 @pytest.mark.parametrize(
-    'filename',
-    ['function.py', 'classmethod.py', 'method.py', 'staticmethod.py'],
+    'style, filename',
+    list(
+        itertools.product(
+            ['numpy', 'google'],
+            ['function.py', 'classmethod.py', 'method.py', 'staticmethod.py'],
+        ),
+    ),
 )
-def testReturns(filename: str) -> None:
+def testReturns(style: str, filename: str) -> None:
     violations = _checkFile(
-        filename=DATA_DIR / f'returns/{filename}',
+        filename=DATA_DIR / f'{style}/returns/{filename}',
         skipCheckingShortDocstrings=False,
+        style=style,
     )
 
     expectedViolations: List[str] = [
         'DOC201: Method `MyClass.func1_3` does not have a return section in '
         'docstring ',
         'DOC201: Method `MyClass.func1_5` does not have a return section in '
         'docstring ',
@@ -286,30 +295,44 @@
     'docstring: [arg1: , arg2: , arg3: ]. Arguments in the docstring but not in '
     'the function signature: [var1: int, var2: str].',
     'DOC201: Function `func3` does not have a return section in docstring ',
 ]
 
 
 @pytest.mark.parametrize(
-    'skipCheckingShortDocstrings, expected',
-    [(True, expected_True), (False, expected_False)],
+    'style, skipCheckingShortDocstrings, expected',
+    [
+        ('numpy', True, expected_True),
+        ('numpy', False, expected_False),
+        ('google', True, expected_True),
+        ('google', False, expected_False),
+    ],
 )
 def testSkipCheckingShortDocstrings(
+        style: str,
         skipCheckingShortDocstrings: bool,
         expected: List[str],
 ) -> None:
     violations = _checkFile(
-        filename=DATA_DIR / 'short_docstrings/cases.py',
+        filename=DATA_DIR / f'{style}/short_docstrings/cases.py',
         skipCheckingShortDocstrings=skipCheckingShortDocstrings,
+        style=style,
     )
     assert list(map(str, violations)) == expected
 
 
-def testInit() -> None:
-    violations = _checkFile(filename=DATA_DIR / 'init/init.py')
+@pytest.mark.parametrize(
+    'style',
+    ['numpy', 'google'],
+)
+def testInit(style: str) -> None:
+    violations = _checkFile(
+        filename=DATA_DIR / f'{style}/init/init.py',
+        style=style,
+    )
     expected = [
         'DOC301: Class `A`: __init__() should not have a docstring; please combine it '
         'with the docstring of the class ',
         'DOC302: Class `B`: The docstring for the class does not need a "Returns" '
         'sections ',
         'DOC105: Method `C.__init__`: Argument names match, but type hints do not '
         'match ',
@@ -322,51 +345,64 @@
         'the function signature: [var1: list, var2: dict].',
         'DOC302: Class `D`: The docstring for the class does not need a "Returns" '
         'sections ',
     ]
     assert list(map(str, violations)) == expected
 
 
-def testYields() -> None:
-    violations = _checkFile(filename=DATA_DIR / 'yields/cases.py')
+@pytest.mark.parametrize('style', ['numpy', 'google'])
+def testYields(style: str) -> None:
+    violations = _checkFile(
+        filename=DATA_DIR / f'{style}/yields/cases.py',
+        style=style,
+    )
     expected = [
         'DOC401: Method `A.method1` returns a Generator, but the docstring does not '
         'have a "Yields" section ',
         'DOC402: Method `A.method1` has "yield" statements, but the docstring does '
         'not have a "Yields" section ',
         'DOC402: Method `A.method2` has "yield" statements, but the docstring does '
         'not have a "Yields" section ',
         'DOC403: Method `A.method3` has a "Yields" section in the docstring, but '
         'there are no "yield" statements or a Generator return annotation ',
     ]
     assert list(map(str, violations)) == expected
 
 
-@pytest.mark.parametrize('skipRaisesCheck', [False, True])
-def testRaises(skipRaisesCheck: bool) -> None:
+@pytest.mark.parametrize(
+    'style, skipRaisesCheck',
+    itertools.product(
+        ['numpy', 'google'],
+        [False, True],
+    ),
+)
+def testRaises(style: str, skipRaisesCheck: bool) -> None:
     violations = _checkFile(
-        filename=DATA_DIR / 'raises/cases.py',
+        filename=DATA_DIR / f'{style}/raises/cases.py',
         skipCheckingRaises=skipRaisesCheck,
+        style=style,
     )
     expected0 = [
         'DOC501: Method `B.func1` has "raise" statements, but the docstring does not '
         'have a "Raises" section ',
         'DOC502: Method `B.func5` has a "Raises" section in the docstring, but there '
         'are not "raise" statements in the body ',
         'DOC502: Method `B.func7` has a "Raises" section in the docstring, but there '
         'are not "raise" statements in the body ',
     ]
     expected1 = []
     expected = expected1 if skipRaisesCheck else expected0
     assert list(map(str, violations)) == expected
 
 
-def testStarsInArgumentList() -> None:
+@pytest.mark.parametrize('style', ['numpy', 'google'])
+def testStarsInArgumentList(style: str) -> None:
     violations = _checkFile(
-        filename=DATA_DIR / 'star_args/cases.py',
+        filename=DATA_DIR / f'{style}/star_args/cases.py',
+        style=style,
     )
     expected = [
         'DOC103: Function `func2`: Docstring arguments are different from function '
         'arguments. (Or did you miss the space between the argument name and the ":" '
         'in the docstring?). Arguments in the function signature but not in the '
         'docstring: [**kwargs: ]. Arguments in the docstring but not in the function '
         'signature: [kwargs: ].',
@@ -397,10 +433,11 @@
     This is a placeholder test for testing the `playground.py` file.
 
     When you want to quickly test something, you can add contents into
     tests/data/playground.py and run this test function.
     """
     violations = _checkFile(
         filename=DATA_DIR / 'playground.py',
+        style='google',
     )
     expected = []
     assert list(map(str, violations)) == expected
```

