# Comparing `tmp/openai_pygenerator-0.0.9.tar.gz` & `tmp/openai_pygenerator-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_pygenerator-0.0.9.tar", last modified: Thu May 18 09:12:12 2023, max compression
+gzip compressed data, was "openai_pygenerator-0.1.0.tar", last modified: Fri May 19 15:54:07 2023, max compression
```

## Comparing `openai_pygenerator-0.0.9.tar` & `openai_pygenerator-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:12:12.929755 openai_pygenerator-0.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:12:12.925755 openai_pygenerator-0.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:12:12.929755 openai_pygenerator-0.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-18 09:11:53.000000 openai_pygenerator-0.0.9/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-18 09:11:53.000000 openai_pygenerator-0.0.9/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-18 09:11:53.000000 openai_pygenerator-0.0.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-18 09:12:12.929755 openai_pygenerator-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-18 09:11:53.000000 openai_pygenerator-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:53.000000 openai_pygenerator-0.0.9/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-18 09:11:53.000000 openai_pygenerator-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-18 09:11:53.000000 openai_pygenerator-0.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-18 09:12:12.929755 openai_pygenerator-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-18 09:11:53.000000 openai_pygenerator-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:12:12.929755 openai_pygenerator-0.0.9/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:53.000000 openai_pygenerator-0.0.9/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:12:12.929755 openai_pygenerator-0.0.9/src/openai_pygenerator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-18 09:12:12.000000 openai_pygenerator-0.0.9/src/openai_pygenerator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-18 09:12:12.000000 openai_pygenerator-0.0.9/src/openai_pygenerator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 09:12:12.000000 openai_pygenerator-0.0.9/src/openai_pygenerator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-18 09:12:12.000000 openai_pygenerator-0.0.9/src/openai_pygenerator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 09:12:12.000000 openai_pygenerator-0.0.9/src/openai_pygenerator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-18 09:11:53.000000 openai_pygenerator-0.0.9/src/openai_pygenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:12:12.929755 openai_pygenerator-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-18 09:11:53.000000 openai_pygenerator-0.0.9/tests/test_gpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:54:07.641098 openai_pygenerator-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:54:07.637098 openai_pygenerator-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:54:07.641098 openai_pygenerator-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21334 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-19 15:54:07.641098 openai_pygenerator-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/mypy-tests.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-19 15:54:07.641098 openai_pygenerator-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:54:07.641098 openai_pygenerator-0.1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/src/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:54:07.641098 openai_pygenerator-0.1.0/src/openai_pygenerator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-19 15:54:07.000000 openai_pygenerator-0.1.0/src/openai_pygenerator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-19 15:54:07.000000 openai_pygenerator-0.1.0/src/openai_pygenerator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:54:07.000000 openai_pygenerator-0.1.0/src/openai_pygenerator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-19 15:54:07.000000 openai_pygenerator-0.1.0/src/openai_pygenerator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-19 15:54:07.000000 openai_pygenerator-0.1.0/src/openai_pygenerator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:54:07.000000 openai_pygenerator-0.1.0/src/openai_pygenerator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/src/openai_pygenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:54:07.641098 openai_pygenerator-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/tests/test_gpt.py
```

### Comparing `openai_pygenerator-0.0.9/.github/workflows/python-package.yml` & `openai_pygenerator-0.1.0/.github/workflows/python-package.yml`

 * *Files 14% similar despite different names*

```diff
@@ -23,18 +23,15 @@
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        python -m pip install flake8 pytest
-        if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
-    - name: Lint with flake8
+        pip install .[dev]
+    - name: Pre-commit tests
       run: |
-        # stop the build if there are Python syntax errors or undefined names
-        flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
-        # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
-        flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
+        export PYTHONPATH="./src"
+        pre-commit run --all-files
     - name: Test with pytest
       run: |
         pytest
```

### Comparing `openai_pygenerator-0.0.9/.github/workflows/python-publish.yml` & `openai_pygenerator-0.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `openai_pygenerator-0.0.9/LICENSE.txt` & `openai_pygenerator-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openai_pygenerator-0.0.9/pyproject.toml` & `openai_pygenerator-0.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [build-system]
-requires = ["setuptools>=61.0", "setuptools_scm[toml]>=6.2", "openai>=0.27"]
+requires = ["setuptools>=61.0", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "src/version.py"
 
+[tool.pytest.ini_options]
+pythonpath = "src"
+
 [project]
 name = "openai_pygenerator"
 dynamic = ["version"]
 
 authors = [
   { name="Steve Phelps", email="sphelps@sphelps.net" },
 ]
```

### Comparing `openai_pygenerator-0.0.9/tests/test_gpt.py` & `openai_pygenerator-0.1.0/tests/test_gpt.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,21 @@
-from typing import Iterable
+from typing import Callable, Iterable
 
 import pytest
 from openai.error import APIError, RateLimitError
 from openai.openai_object import OpenAIObject
 
-from src.openai_pygenerator import GPT_MAX_RETRIES, generate_completions
+from openai_pygenerator import (
+    GPT_MAX_RETRIES,
+    ChatSession,
+    Conversation,
+    gpt_completions,
+    transcript,
+    user_message,
+)
 
 
 def aio(text: str) -> OpenAIObject:
     result = OpenAIObject()
     result["message"] = text
     return result
 
@@ -38,15 +45,15 @@
 def test_generate_completion(mock_openai, mock_sleep, error):
     mock_openai.side_effect = [
         error,
         error,
         MockChoices(["Test completion 1", "Test completion 2"]),
     ]
 
-    completions = list(generate_completions([]))
+    completions = list(gpt_completions([]))
 
     assert completions == ["Test completion 1", "Test completion 2"]
     assert mock_sleep.call_count == 2
 
 
 @pytest.mark.parametrize(
     "error",
@@ -55,10 +62,48 @@
         APIError("Gateway Timeout", http_status=524),
     ],
 )
 def test_generate_completion_error(mock_openai, mock_sleep, error):
     mock_openai.side_effect = [error] * GPT_MAX_RETRIES
 
     with pytest.raises(Exception):
-        _ = list(generate_completions([]))
+        _ = list(gpt_completions([]))
 
     assert mock_sleep.call_count == GPT_MAX_RETRIES
+
+
+def test_user_message():
+    test_message = "test"
+    result = user_message(test_message)
+    assert result["role"] == "user"
+    assert result["content"] == test_message
+
+
+def test_transcript():
+    def test_message(i: int) -> str:
+        return f"message{i}"
+
+    test_messages = [user_message(test_message(i)) for i in range(10)]
+    result = list(transcript(iter(test_messages)))
+    for i in range(10):
+        assert result[i] == test_message(i)
+
+
+def test_chat_session():
+    def completer(response: str) -> Callable[[Conversation, int], Conversation]:
+        def mock_complete(_history: Conversation, _n: int) -> Conversation:
+            yield {"role": "assistant", "content": response}
+
+        return mock_complete
+
+    session = ChatSession(completer("response1"))
+    result = session.ask("First question")
+    assert result == "response1"
+    session._generate = completer("response2")  # pylint: disable=protected-access
+    result = session.ask("Second question")
+    assert result == "response2"
+    assert session.transcript == [
+        "First question",
+        "response1",
+        "Second question",
+        "response2",
+    ]
```

