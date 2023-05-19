# Comparing `tmp/eulertools-0.8.0.tar.gz` & `tmp/eulertools-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eulertools-0.8.0.tar", max compression
+gzip compressed data, was "eulertools-0.9.0.tar", max compression
```

## Comparing `eulertools-0.8.0.tar` & `eulertools-0.9.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7652 2023-05-09 19:41:34.782813 eulertools-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0     2679 2023-05-17 15:25:07.529316 eulertools-0.8.0/README.rst
--rw-r--r--   0        0        0     2693 2023-05-17 15:25:59.778268 eulertools-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-09 19:41:34.789309 eulertools-0.8.0/src/eulertools/__init__.py
--rw-r--r--   0        0        0       22 2023-05-17 15:25:59.781326 eulertools-0.8.0/src/eulertools/__version__.py
--rw-r--r--   0        0        0     2881 2023-05-15 13:24:16.965570 eulertools-0.8.0/src/eulertools/compare.py
--rw-r--r--   0        0        0      871 2023-05-16 21:00:03.640220 eulertools-0.8.0/src/eulertools/generate.py
--rw-r--r--   0        0        0     3376 2023-05-17 13:06:15.125067 eulertools-0.8.0/src/eulertools/main.py
--rw-r--r--   0        0        0     3175 2023-05-17 13:06:15.125983 eulertools-0.8.0/src/eulertools/run.py
--rw-r--r--   0        0        0      969 2023-05-17 15:25:07.672109 eulertools-0.8.0/src/eulertools/statement.py
--rw-r--r--   0        0        0     2586 2023-05-15 13:30:41.006142 eulertools-0.8.0/src/eulertools/time.py
--rw-r--r--   0        0        0     6121 2023-05-17 15:25:08.070232 eulertools-0.8.0/src/eulertools/utils.py
--rw-r--r--   0        0        0     3519 1970-01-01 00:00:00.000000 eulertools-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-05-09 19:41:34.782813 eulertools-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0     2709 2023-05-19 09:12:00.518889 eulertools-0.9.0/README.rst
+-rw-r--r--   0        0        0     2693 2023-05-19 09:23:51.856605 eulertools-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-09 19:41:34.789309 eulertools-0.9.0/src/eulertools/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-19 09:24:03.037423 eulertools-0.9.0/src/eulertools/__version__.py
+-rw-r--r--   0        0        0     2881 2023-05-15 13:24:16.965570 eulertools-0.9.0/src/eulertools/compare.py
+-rw-r--r--   0        0        0      871 2023-05-16 21:00:03.640220 eulertools-0.9.0/src/eulertools/generate.py
+-rw-r--r--   0        0        0     3549 2023-05-18 13:32:14.231507 eulertools-0.9.0/src/eulertools/main.py
+-rw-r--r--   0        0        0     3555 2023-05-18 16:50:57.283677 eulertools-0.9.0/src/eulertools/run.py
+-rw-r--r--   0        0        0      939 2023-05-17 15:31:23.939637 eulertools-0.9.0/src/eulertools/statement.py
+-rw-r--r--   0        0        0     2626 2023-05-18 11:36:19.700674 eulertools-0.9.0/src/eulertools/time.py
+-rw-r--r--   0        0        0     6947 2023-05-18 16:44:27.428929 eulertools-0.9.0/src/eulertools/utils.py
+-rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 eulertools-0.9.0/PKG-INFO
```

### Comparing `eulertools-0.8.0/LICENSE.txt` & `eulertools-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eulertools-0.8.0/README.rst` & `eulertools-0.9.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -34,31 +34,33 @@
 Installation
 ^^^^^^^^^^^^
 
 The easiest way is to use `pipx`_ to install ``eulertools``.
 
 .. code:: console
 
-   $ pipx install yamk
+   $ pipx install eulertools
 
 This is the only officially supported way of installing it.
 As ``eulertools`` require python 3.11+, please make sure that
 this is the version used by your system, or use a tool like
 `pyenv`_ to create a shell with such a python version.
 
 Usage
 ^^^^^
 
 ``eulertools`` provides a cli command called ``euler``, which has the following subcommands:
 
-compare: compare the timings between different languages
-generate: generate a template for a new problem from the language template
-run: run (and test) problems for various language implementations
-statement: show the problem statement and the hint for the solution
-time: run the timings for a specific problem
+::
+
+    compare: Compare the timings between different languages
+    generate: Generate a template for a new problem from the language template
+    run: Run (and test) problems for various language implementations
+    statement: Show the problem statement and the hint for the solution
+    time: Run the timings for a specific problem
 
 For the required project structure, please view the detailed `Documentation`_.
 
 Links
 -----
 
 - `Documentation`_
```

### Comparing `eulertools-0.8.0/pyproject.toml` & `eulertools-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 skip_empty = true
 
 [tool.poetry]
 name = "eulertools"
-version = "0.8.0"
+version = "0.9.0"
 description = "Multilanguage competitive coding toolbox"
 authors = [
     "Stephanos Kuma <stephanos@kuma.ai>",
 ]
 
 license = "LGPL-3.0+"
 readme = "README.rst"
```

### Comparing `eulertools-0.8.0/src/eulertools/compare.py` & `eulertools-0.9.0/src/eulertools/compare.py`

 * *Files identical despite different names*

### Comparing `eulertools-0.8.0/src/eulertools/generate.py` & `eulertools-0.9.0/src/eulertools/generate.py`

 * *Files identical despite different names*

### Comparing `eulertools-0.8.0/src/eulertools/main.py` & `eulertools-0.9.0/src/eulertools/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     generate_parser = subparsers.add_parser("generate", parents=[parent_parser])
     language_specific(generate_parser)
     problem_specific(generate_parser)
 
     run_parser = subparsers.add_parser("run", parents=[parent_parser])
     language_specific(run_parser)
     problem_specific(run_parser)
+    run_parser.add_argument("-u", "--update", action="store_true")
 
     time_parser = subparsers.add_parser("time", parents=[parent_parser])
     language_specific(time_parser)
     problem_specific(time_parser)
     time_parser.add_argument("-t", "--times", type=int, default=10)
     time_parser.add_argument("-u", "--update", action="store_true")
 
@@ -88,15 +89,20 @@
         filter_languages(options.languages) if hasattr(options, "languages") else []
     )
     options.problems = filter_problems(options.problems)
     match options.command:
         case "generate":
             Generate(options.languages, options.problems).run()
         case "run":
-            Run(options.languages, options.problems, options.verbosity).run()
+            Run(
+                options.languages,
+                options.problems,
+                options.verbosity,
+                run_update=options.update,
+            ).run()
         case "time":
             Time(
                 options.languages,
                 options.problems,
                 options.times,
                 options.verbosity,
                 run_update=options.update,
```

### Comparing `eulertools-0.8.0/src/eulertools/run.py` & `eulertools-0.9.0/src/eulertools/run.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,51 @@
 import subprocess
 from itertools import product
 
-from eulertools.utils import Language, Modes, get_answers, get_solution
+from eulertools.utils import (
+    Language,
+    Modes,
+    get_answers,
+    get_line_answer,
+    get_solution,
+    update_answers,
+)
 
 
 class Run:
     def __init__(
         self,
         languages: list[Language],
         problems: list[str],
         verbosity: int,
         *,
+        run_update: bool = False,
         times: int = 1,
         mode: str = Modes.RUN,
     ):
         self.languages = languages
         self.problems = problems
         self.mode = mode
         self.times = times
         self.verbosity = verbosity
+        self.expected_answers = get_answers()
+        self.run_update = run_update
 
     def run(self) -> dict[Language, dict[str, dict[int, list[int]]]]:
         output: dict[Language, dict[str, dict[int, list[int]]]] = {}
         success = True
         for language, problem in product(self.languages, self.problems):
             run_success, timings = self.run_single_problem(language, problem)
             if run_success is not None:
                 success = success and run_success
                 output.setdefault(language, {})[problem] = timings
         if not success:
             raise RuntimeError("Some tests failed")
+        if self.run_update:
+            update_answers(self.expected_answers)
         return output
 
     def run_single_problem(
         self, language: Language, problem: str
     ) -> tuple[bool | None, dict[int, list[int]]]:
         solution = get_solution(language, problem)
         if not solution.exists():
@@ -44,37 +56,41 @@
         )
         output = raw_output.stdout.decode()
         if self.verbosity > 3:
             print(output)
         actual_answers: dict[int, set[str]] = {}
         timings: dict[int, list[int]] = {}
         for line in output.splitlines():
-            output_type, run_id, value = line.split(maxsplit=2)
-            key = int(run_id)
+            output_type, run_id, value = get_line_answer(line)
             if output_type == "Time":
-                timings.setdefault(key, []).append(int(value) or 1)
+                timings.setdefault(run_id, []).append(int(value) or 1)
             elif output_type == "Answer":
-                actual_answers.setdefault(key, set()).add(value)
-        expected_answers = get_answers(problem)
+                actual_answers.setdefault(run_id, set()).add(value)
+        expected_answers = self.expected_answers.setdefault(problem, {})
         success = True
-        if self.mode != Modes.TIMING and len(actual_answers) != len(expected_answers):
+        if missing_answers := {
+            answer for answer in expected_answers if answer not in actual_answers
+        }:
             success = False
-            print(f"🔴 Running {problem}... Not the expected number of answers.")
+            print(
+                f"🔴 Running {problem}... Missing answers with keys {missing_answers}."
+            )
         for key, values in actual_answers.items():
             if len(values) != 1:
                 success = False
                 print(
                     f"🔴 Running {language.name}/{problem}/{key}... Not deterministic answer."
                 )
             value = values.pop()
             if key not in expected_answers:
                 if self.mode != Modes.TIMING:
                     print(
                         f"🟠 Running {language.name}/{problem}/{key}... new response: {value}"
                     )
+                expected_answers[key] = value
             elif value != expected_answers[key]:
                 success = False
                 print(
                     f"🔴 Running {language.name}/{problem}/{key}... expected: {expected_answers[key]}, got: {value}"
                 )
             elif self.mode != Modes.TIMING:
                 print(f"🟢 Running {language.name}/{problem}/{key}... {value}")
```

### Comparing `eulertools-0.8.0/src/eulertools/statement.py` & `eulertools-0.9.0/src/eulertools/statement.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,16 +10,14 @@
         for problem in self.problems:
             self.show_statement(problem)
 
     def show_statement(self, problem: str) -> None:
         statement = get_statement(problem)["common"]
         if title := statement.get("title", ""):
             print(ANSIEscape.OKGREEN, title, ANSIEscape.ENDC, sep="")
-            print(
-                ANSIEscape.OKGREEN, "~" * len(title), ANSIEscape.ENDC, sep=""
-            )
+            print(ANSIEscape.OKGREEN, "~" * len(title), ANSIEscape.ENDC, sep="")
         print(statement["description"].strip())
         if self.show_hints and (hint := statement.get("hint")):
             print("")
             print(ANSIEscape.OKBLUE, "Hint", ANSIEscape.ENDC, sep="")
             print(ANSIEscape.OKBLUE, "~" * len("Hint"), ANSIEscape.ENDC, sep="")
             print(hint.strip())
```

### Comparing `eulertools-0.8.0/src/eulertools/time.py` & `eulertools-0.9.0/src/eulertools/time.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,17 @@
         self.verbosity = verbosity
         self.run_update = run_update
         self.timings = {language: get_timings(language) for language in languages}
 
     def run(self) -> None:
         for language, problem in product(self.languages, self.problems):
             self.time_single_problem(language, problem)
+        if self.run_update:
+            for language in self.languages:
+                update_timings(language, self.timings[language])
 
     def time_single_problem(self, language: Language, problem: str) -> None:
         self.timings[language].setdefault(problem, {})
         solution = get_solution(language, problem)
         if not solution.exists():
             return
 
@@ -59,16 +62,14 @@
             new_timing = new_timings[key]
             self.timings[language][problem][key] = new_timing
             print(f"Old timing: {old_timing}")
             if self.verbosity > 0:
                 print("New timings:")
                 for i, timing in enumerate(raw_timing):
                     print(f"* Run {i + 1} took: {Timing.from_nanoseconds(timing)}")
-            if self.run_update:
-                update_timings(language, self.timings[language])
             prefix = "New" if old_timing is not None else "Initial"
             print(f"{prefix} timing: {new_timing}")
             if self.verbosity > 1 and old_timing is not None:
                 old_nanoseconds = old_timing.nanoseconds
                 new_nanoseconds = new_timing.nanoseconds
                 change = 100 * (old_nanoseconds - new_nanoseconds) / old_nanoseconds
                 print(f"Performance difference: {change:.2f}%")
```

### Comparing `eulertools-0.8.0/src/eulertools/utils.py` & `eulertools-0.9.0/src/eulertools/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -115,57 +115,79 @@
 
 
 def get_template(language: Language) -> Path:
     return language.path.joinpath(".leet", "solution.jinja")
 
 
 def get_solution(language: Language, problem: str) -> Path:
-    return language.path.joinpath(
-        "src", "solutions", f"{problem}.{language.extension}"
-    )
+    return language.path.joinpath("src", "solutions", f"{problem}.{language.extension}")
 
 
 def get_statement(problem: str) -> dict[str, Any]:
     return SettingsParser(_get_statement(problem)).data
 
 
 def get_settings() -> dict[str, Any]:
     return SettingsParser(_get_settings()).data
 
 
-def get_answers(problem: str) -> dict[int, str]:
+def get_line_timing(line: str) -> tuple[str, int, Timing]:
+    problem_part, mode_id, timing = line.split(maxsplit=2)
+    return problem_part, int(mode_id), Timing.from_nanoseconds(int(timing))
+
+
+def get_line_answer(line: str) -> tuple[str, int, str]:
+    problem_part, mode_id, *answers = line.split(maxsplit=2)
+    if len(answers) == 0:
+        answer = ""
+    elif len(answers) == 1:
+        answer = answers[0]
+    else:
+        raise RuntimeError("Too many answers")
+    return problem_part, int(mode_id), answer
+
+
+def get_answers() -> dict[str, dict[int, str]]:
     answers = _get_answers()
-    output: dict[int, str] = {}
+    output: dict[str, dict[int, str]] = {}
     for line in answers.read_text().splitlines():
-        if line.startswith(problem):
-            problem_part, mode_id, answer = line.split(maxsplit=2)
-            output[int(mode_id)] = answer
+        problem, mode_id, answer = get_line_answer(line)
+        output.setdefault(problem, {})[mode_id] = answer
     return output
 
 
 def get_timings(language: Language) -> dict[str, dict[int, Timing]]:
     timings = _get_timings(language)
     output: dict[str, dict[int, Timing]] = {}
     for line in timings.read_text().splitlines():
-        problem, key, timing = line.split()
-        output.setdefault(problem, {})[int(key)] = Timing.from_nanoseconds(int(timing))
+        problem, mode_id, timing = get_line_timing(line)
+        output.setdefault(problem, {})[mode_id] = timing
     return output
 
 
 def get_context(language: Language, problem: str) -> dict[str, str]:
     statement = get_statement(problem)
     return {
         "problem": problem,
         "title": statement["common"].get("title", ""),
         "method": statement["common"].get("method", ""),
         "args": statement.get(language.name, {}).get("args", ""),
         "rtype": statement.get(language.name, {}).get("rtype", ""),
     }
 
 
+def update_answers(answers: dict[str, dict[int, str]]) -> None:
+    answers_path = _get_answers()
+    with answers_path.open("w") as file:
+        for problem in sorted(answers):
+            for key in sorted(answers[problem]):
+                answer = answers[problem][key]
+                file.write(f"{problem} {key} {answer}\n")
+
+
 def update_timings(language: Language, timings: dict[str, dict[int, Timing]]) -> None:
     timings_path = _get_timings(language)
     with timings_path.open("w") as file:
         for problem in sorted(timings):
             for key in sorted(timings[problem]):
                 timing = timings[problem][key]
                 file.write(f"{problem} {key} {timing.nanoseconds}\n")
@@ -185,15 +207,17 @@
 def get_all_problems() -> list[str]:
     statement_dir = _get_statements_dir()
     return sorted(file.stem for file in statement_dir.iterdir())
 
 
 def get_all_keyed_problems() -> list[tuple[str, int]]:
     output = [
-        (problem, key) for problem in get_all_problems() for key in get_answers(problem)
+        (problem, key)
+        for problem, problem_info in get_answers().items()
+        for key in problem_info
     ]
     return sorted(output)
 
 
 def filter_languages(parsed_languages: list[str]) -> list[Language]:
     language_strings = get_all_languages()
     return [
```

### Comparing `eulertools-0.8.0/PKG-INFO` & `eulertools-0.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eulertools
-Version: 0.8.0
+Version: 0.9.0
 Summary: Multilanguage competitive coding toolbox
 Home-page: https://eulertools.readthedocs.io/en/latest/
 License: LGPL-3.0+
 Keywords: leetcode,topcoder,project_euler
 Author: Stephanos Kuma
 Author-email: stephanos@kuma.ai
 Requires-Python: >=3.11,<4.0
@@ -55,31 +55,33 @@
 Installation
 ^^^^^^^^^^^^
 
 The easiest way is to use `pipx`_ to install ``eulertools``.
 
 .. code:: console
 
-   $ pipx install yamk
+   $ pipx install eulertools
 
 This is the only officially supported way of installing it.
 As ``eulertools`` require python 3.11+, please make sure that
 this is the version used by your system, or use a tool like
 `pyenv`_ to create a shell with such a python version.
 
 Usage
 ^^^^^
 
 ``eulertools`` provides a cli command called ``euler``, which has the following subcommands:
 
-compare: compare the timings between different languages
-generate: generate a template for a new problem from the language template
-run: run (and test) problems for various language implementations
-statement: show the problem statement and the hint for the solution
-time: run the timings for a specific problem
+::
+
+    compare: Compare the timings between different languages
+    generate: Generate a template for a new problem from the language template
+    run: Run (and test) problems for various language implementations
+    statement: Show the problem statement and the hint for the solution
+    time: Run the timings for a specific problem
 
 For the required project structure, please view the detailed `Documentation`_.
 
 Links
 -----
 
 - `Documentation`_
```

