# Comparing `tmp/cg_pytest_reporter-2023.5.17.942.tar.gz` & `tmp/cg_pytest_reporter-2023.5.18.1327.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cg_pytest_reporter-2023.5.17.942.tar", max compression
+gzip compressed data, was "cg_pytest_reporter-2023.5.18.1327.tar", max compression
```

## Comparing `cg_pytest_reporter-2023.5.17.942.tar` & `cg_pytest_reporter-2023.5.18.1327.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       21 2023-05-17 09:42:07.964449 cg_pytest_reporter-2023.5.17.942/README.md
--rw-r--r--   0        0        0      422 2023-05-17 09:42:07.964449 cg_pytest_reporter-2023.5.17.942/cg_pytest_reporter/__init__.py
--rw-r--r--   0        0        0    17620 2023-05-17 09:42:07.964449 cg_pytest_reporter-2023.5.17.942/cg_pytest_reporter/plugin.py
--rw-r--r--   0        0        0     1810 2023-05-17 09:42:33.186790 cg_pytest_reporter-2023.5.17.942/pyproject.toml
--rw-r--r--   0        0        0      405 1970-01-01 00:00:00.000000 cg_pytest_reporter-2023.5.17.942/PKG-INFO
+-rw-r--r--   0        0        0       21 2023-05-10 12:51:51.646282 cg_pytest_reporter-2023.5.18.1327/README.md
+-rw-r--r--   0        0        0      422 2023-05-16 10:13:24.236322 cg_pytest_reporter-2023.5.18.1327/cg_pytest_reporter/__init__.py
+-rw-r--r--   0        0        0    18890 2023-05-18 13:19:43.776409 cg_pytest_reporter-2023.5.18.1327/cg_pytest_reporter/plugin.py
+-rw-r--r--   0        0        0     1809 2023-05-18 13:27:13.393849 cg_pytest_reporter-2023.5.18.1327/pyproject.toml
+-rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 cg_pytest_reporter-2023.5.18.1327/setup.py
+-rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 cg_pytest_reporter-2023.5.18.1327/PKG-INFO
```

### Comparing `cg_pytest_reporter-2023.5.17.942/cg_pytest_reporter/plugin.py` & `cg_pytest_reporter-2023.5.18.1327/cg_pytest_reporter/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
     pytest -p no:cg-pytest-reporter
 """
 import json
 import typing as t
 import logging
 import dataclasses
+from fractions import Fraction
 
 import pytest
 import _pytest.nodes
 from _pytest.junitxml import mangle_test_address
 
 logger = logging.getLogger('cg_pytest_reporter')
 
@@ -102,26 +103,26 @@
 
 @dataclasses.dataclass
 class CgMarks:
     """Marks set on each test case by the `cg-pytest-reporter` plugin used when
     generating the report.
     """
     #: The name of the test suite.
-    suite_name: str | None
+    suite_name: t.Optional[str]
     #: The weight of the test suite.
-    suite_weight: int | float | None
+    suite_weight: t.Union[Fraction, int, float, None]
 
     #: The name of the test case.
-    name: str | None
+    name: t.Optional[str]
     #: The description of the test case.
-    description: str | None
+    description: t.Optional[str]
     #: The weight of the test case.
-    weight: int | float | None
+    weight: t.Union[Fraction, int, float, None]
     #: The reason the test failed.
-    reason: str | None
+    reason: t.Optional[str]
     #: The stdout produced while running the test.
     hide_stdout: bool
     #: The stderr produced while running the test.
     hide_stderr: bool
 
     @classmethod
     def from_item(cls, item: pytest.Item) -> 'CgMarks':
@@ -148,48 +149,48 @@
         )
 
     @classmethod
     def _get_suite_mark_value(
         cls,
         item: pytest.Item,
         name: str,
-    ) -> object | None:
+    ) -> t.Optional[object]:
         # It is not possible to add marks on the module level because you cannot
         # call a decorator on a module. So on the module level we allow a custom
         # name and weight by setting the `__cg_suite_{name,weight}__` variables
         # at the top level of the module.
         if isinstance(item.parent, pytest.Module):
             # Pytest offers no way to get the module object from a `Module` node.
             # pylint: disable=protected-access
             return getattr(item.parent._obj, f'__{name}__', None)
         else:
             return cls._get_mark_value(item.parent, name)
 
     @classmethod
     def _get_mark_value(
         cls,
-        item: _pytest.nodes.Node | None,
+        item: t.Optional[_pytest.nodes.Node],
         name: str,
-    ) -> object | None:
+    ) -> t.Optional[object]:
         if item is None:
             return None
-        mark: pytest.Mark | None = item.get_closest_marker(name)
+        mark: t.Optional[pytest.Mark] = item.get_closest_marker(name)
         if mark is None or not mark.args:
             return None
         return mark.args[0]
 
     @staticmethod
-    def _as_str(obj: object) -> str | None:
+    def _as_str(obj: object) -> t.Optional[str]:
         if isinstance(obj, str):
             return obj
         return None
 
     @staticmethod
-    def _as_num(obj: object) -> float | int | None:
-        if isinstance(obj, (int, float)):
+    def _as_num(obj: object) -> t.Union[Fraction, float, int, None]:
+        if isinstance(obj, (Fraction, int, float)):
             return obj
         return None
 
 
 class CGPytestReporterPlugin:
     """Implementation of the reporter plugin.
 
@@ -204,14 +205,17 @@
     report to the given file descriptor.
     """
 
     _config: pytest.Config
     _fd: int
     _file: t.BinaryIO
 
+    _points_achieved: Fraction = Fraction(0, 1)
+    _points_possible: Fraction = Fraction(0, 1)
+
     def __init__(self, config: pytest.Config) -> None:
         self._config = config
 
         fd = config.getoption('--cg-pytest-fd', default=None)
         if fd is None:
             self._fd = 1
         else:
@@ -274,14 +278,15 @@
 
         data = json_dumps(message) + '\n'
         if len(data) > MESSAGE_SIZE_LIMIT:
             self._limit_message_size(message)
             data = json_dumps(message) + '\n'
 
         self._file.write(data.encode('utf8'))
+        self._update_score(report)
 
     def _mk_test_suite(self, report: pytest.TestReport) -> TestSuiteResult:
         *suite_name_parts, case_name = mangle_test_address(report.nodeid)
         suite_name = '.'.join(suite_name_parts)
 
         test_suite: TestSuiteResult = {
             'id': suite_name,
@@ -329,22 +334,51 @@
                 # If it is a tuple it has 3 elements: a path, a line number, and
                 # the actual reason.
                 reason = longrepr[2]
             else:
                 reason = report.longreprtext
             test_case['reason'] = reason
 
-        # if status == 'failure':
         if report.capstdout and not marks.hide_stdout:
             test_case['stdout'] = report.capstdout
         if report.capstderr and not marks.hide_stderr:
             test_case['stderr'] = report.capstderr
 
         return test_case
 
+    def _update_score(self, report: pytest.TestReport) -> None:
+        if report.outcome == 'skipped':
+            return
+
+        # pylint: disable=protected-access
+        marks = t.cast(CgMarks, report._cg_marks)
+        weight = Fraction(1, 1)
+
+        if marks.weight is not None:
+            weight *= Fraction(marks.weight)
+        if marks.suite_weight is not None:
+            weight *= Fraction(marks.suite_weight)
+
+        self._points_possible += weight
+        if report.outcome == 'passed':
+            self._points_achieved += weight
+
+    def pytest_terminal_summary(self, *_) -> None:
+        """Write the final achieved score to the structured output.
+
+        This uses the same format as the Custom Test step.
+        """
+        if self._points_possible == 0:
+            points = Fraction(0)
+        else:
+            points = self._points_achieved / self._points_possible
+
+        message = {'tag': 'points', 'points': str(points)}
+        self._file.write(json_dumps(message).encode('utf8'))
+
     @staticmethod
     def _limit_message_size(message: UnitTestMessage) -> None:
         """Edits the message in place to ensure it will not be dropped.
 
         If all of the following fields do not fit, an exception is raised. All
         of these fields, except for case status which is already very limited in
         the size it needs, are directly controlled by the teacher.
@@ -358,16 +392,17 @@
         that the smaller one of stdout and stderr is included, and finally the
         other one as well.
         """
         def jsonlen(obj: object) -> int:
             return len(json_dumps(obj))
 
         def field_length(
-            dct: t.Mapping[str, object], field: str
-        ) -> int | None:
+            dct: t.Mapping[str, object],
+            field: str,
+        ) -> t.Optional[int]:
             val = dct.get(field)
             if val is None:
                 return None
 
             length = len(f'"{field}":')
             if isinstance(val, str):
                 # Add 2 for the quotes.
```

### Comparing `cg_pytest_reporter-2023.5.17.942/pyproject.toml` & `cg_pytest_reporter-2023.5.18.1327/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "cg-pytest-reporter"
-version = "2023.05.17.0942"
+version = "2023.05.18.1327"
 description = ""
 authors = ["CodeGrade <info@codegrade.com>"]
 readme = "README.md"
 packages = [{include = "cg_pytest_reporter"}]
 
 [tool.poetry.plugins.pytest11]
 cg_pytest_reporter = "cg_pytest_reporter.plugin"
 
 [tool.poetry.dependencies]
-python = "^3.10"
-pytest = ">=7.3.1"
+python = "^3.8"
+pytest = ">=7.0.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.2.0"
 pylint = "^2.17.4"
 yapf = "^0.33.0"
 isort = "^5.12.0"
```

