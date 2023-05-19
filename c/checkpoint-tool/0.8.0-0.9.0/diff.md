# Comparing `tmp/checkpoint_tool-0.8.0.tar.gz` & `tmp/checkpoint_tool-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkpoint_tool-0.8.0.tar", max compression
+gzip compressed data, was "checkpoint_tool-0.9.0.tar", max compression
```

## Comparing `checkpoint_tool-0.8.0.tar` & `checkpoint_tool-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     7552 2023-05-18 18:03:10.920597 checkpoint_tool-0.8.0/README.md
--rw-r--r--   0        0        0      608 2023-05-09 01:50:05.066517 checkpoint_tool-0.8.0/checkpoint/__init__.py
--rw-r--r--   0        0        0     2514 2023-05-18 16:34:53.180387 checkpoint_tool-0.8.0/checkpoint/app.py
--rw-r--r--   0        0        0     4517 2023-05-18 16:13:03.919978 checkpoint_tool-0.8.0/checkpoint/database.py
--rw-r--r--   0        0        0     7245 2023-05-18 16:35:39.947857 checkpoint_tool-0.8.0/checkpoint/graph.py
--rw-r--r--   0        0        0    11597 2023-05-18 18:02:36.761898 checkpoint_tool-0.8.0/checkpoint/task.py
--rw-r--r--   0        0        0     1391 2023-05-18 04:14:19.815251 checkpoint_tool-0.8.0/checkpoint/types.py
--rw-r--r--   0        0        0      677 2023-05-18 18:06:47.844143 checkpoint_tool-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     8357 1970-01-01 00:00:00.000000 checkpoint_tool-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     7809 2023-05-19 01:36:04.901914 checkpoint_tool-0.9.0/README.md
+-rw-r--r--   0        0        0      668 2023-05-19 00:24:23.655244 checkpoint_tool-0.9.0/checkpoint/__init__.py
+-rw-r--r--   0        0        0     2514 2023-05-18 16:34:53.180387 checkpoint_tool-0.9.0/checkpoint/app.py
+-rw-r--r--   0        0        0     4517 2023-05-19 00:54:25.356853 checkpoint_tool-0.9.0/checkpoint/database.py
+-rw-r--r--   0        0        0     7245 2023-05-18 16:35:39.947857 checkpoint_tool-0.9.0/checkpoint/graph.py
+-rw-r--r--   0        0        0    13251 2023-05-19 01:27:03.643064 checkpoint_tool-0.9.0/checkpoint/task.py
+-rw-r--r--   0        0        0     1391 2023-05-18 04:14:19.815251 checkpoint_tool-0.9.0/checkpoint/types.py
+-rw-r--r--   0        0        0      677 2023-05-19 01:28:43.016375 checkpoint_tool-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     8614 1970-01-01 00:00:00.000000 checkpoint_tool-0.9.0/PKG-INFO
```

### Comparing `checkpoint_tool-0.8.0/README.md` & `checkpoint_tool-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -182,14 +182,22 @@
 which is then compressed with `gzip`.
 The compression level can be changed as follows (defaults to 9).
 ```python
 class NoCompressionTask(Task, compress_level=0):
     ...
 ```
 
+### Job scheduling and prefixes
+To run task on job schedulers, one can add prefix to the call of task.
+```python
+
+class TaskWithJobScheduler(Task, job_prefix=['jbsub', '-tty', '-queue x86_1h', '-cores 16+1', '-mem 64g', '-require a100_80gb']):
+    ...
+```
+
 ### Data directories
 
 Use `task.task_directory` to get a fresh path dedicated to each task.
 The directory is automatically created at
 `{$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.{task_name}/data/{task_id}`
 and the contents of the directory are cleared at each task call and persist until the task is cleared.
 ```python
```

### Comparing `checkpoint_tool-0.8.0/checkpoint/__init__.py` & `checkpoint_tool-0.9.0/checkpoint/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,16 @@
     - Automatic cache/data management (source code change detection, cache/data dependency tracking).
     - Task queue with rate limits.
 
 Limitations:
     - No priority-based scheduling.
 """
 from .types import Context
-from .task import infer_task_type, Task, TaskLike, Req, Requires, RequiresList, RequiresDict, Const
+from .task import infer_task_type, Task, SinkTask, SourceTask, TaskLike, Req, Requires, RequiresList, RequiresDict, Const
 
 
 __EXPORT__ = [
-        infer_task_type, Task, Req, Requires, RequiresList, RequiresDict, Const, TaskLike,
+        infer_task_type, Task, SinkTask, SourceTask,
+        Const, TaskLike,
+        Req, Requires, RequiresList, RequiresDict,
         Context
         ]
```

### Comparing `checkpoint_tool-0.8.0/checkpoint/app.py` & `checkpoint_tool-0.9.0/checkpoint/app.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.8.0/checkpoint/database.py` & `checkpoint_tool-0.9.0/checkpoint/database.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.8.0/checkpoint/graph.py` & `checkpoint_tool-0.9.0/checkpoint/graph.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.8.0/checkpoint/task.py` & `checkpoint_tool-0.9.0/checkpoint/task.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from __future__ import annotations
 from abc import ABC, abstractmethod
 from collections.abc import Iterable
+from re import sub
 from typing import Callable, Generic, Mapping, Protocol, Sequence, Type, TypeVar, Any, cast
 from typing_extensions import ParamSpec, Self, get_origin, overload
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
 from concurrent.futures import Executor
 import ast
 import logging
 import inspect
 import json
 import shutil
 
+
 from .types import Json, TaskKey, Context
 from .database import Database
 from .graph import TaskGraph, run_task_graph
 
 
 LOGGER = logging.getLogger(__name__)
 
@@ -32,20 +34,22 @@
 class TaskConfig(Generic[P, R]):
     """ Information specific to a task class (not instance) """
     def __init__(
             self,
             task_class: Type[TaskType[P, R]],
             channels: tuple[str, ...],
             compress_level: int,
+            job_prefix: list[str] | None,
             ) -> None:
 
         self.task_class = task_class
         self.name = _serialize_function(task_class)
         self.db = Database.make(name=self.name, compress_level=compress_level)
         self.channels = (self.name,) + channels
+        self.job_prefix = job_prefix
         self.worker_registry: dict[Json, TaskWorker[R]] = {}
 
         source = inspect.getsource(task_class)
         formatted_source = ast.unparse(ast.parse(source))
         self.source_timestamp = self.db.update_source_if_necessary(formatted_source)
 
     def clear_all(self) -> None:
@@ -97,17 +101,44 @@
         except KeyError:
             return None
 
     def set_result(self) -> None:
         db = self.config.db
         if self.directory.exists():
             shutil.rmtree(self.directory)
-        out = self.instance.run_task()
+        out = self.run_instance_task()
         db.save(self.arg_key, out)
 
+    def run_instance_task(self) -> R:
+        job_prefix = self.config.job_prefix
+        if job_prefix is None:
+            return self.instance.run_task()
+        else:
+            import subprocess
+            import tempfile
+            import cloudpickle
+            import gzip
+            import sys
+            with tempfile.TemporaryDirectory() as dir_ref:
+                worker_path = Path(dir_ref) / 'worker.pkl'
+                result_path = Path(dir_ref) / 'result.pkl'
+                pycmd = f"""import gzip, cloudpickle
+                    worker = cloudpickle.load(gzip.open("{worker_path}", "rb"))
+                    res = worker.instance.run_task()
+                    cloudpickle.dump(res, gzip.open("{result_path}", "wb"))
+                """.replace('\n', ';')
+                with gzip.open(worker_path, 'wb') as worker_ref:
+                    cloudpickle.dump(self, worker_ref)
+                res = subprocess.run([*job_prefix, sys.executable, '-c', pycmd], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+                print(res.stdout.decode(), end='')
+                print(res.stderr.decode(), end='', file=sys.stderr)
+                res.check_returncode()
+                with gzip.open(result_path, 'rb') as result_ref:
+                    return cloudpickle.load(result_ref)
+
     @property
     def _directory_uninit(self) -> Path:
         _, arg_str = self.to_tuple()
         return self.config.db.get_data_directory(arg_str)
 
     @property
     def directory(self) -> Path:
@@ -150,24 +181,25 @@
             assert all(isinstance(q, str) for q in channels)
         elif _channel is None:
             channels = tuple()
         else:
             raise ValueError('Invalid channel value:', _channel)
 
         compress_level = kwargs.pop('compress_level', 9)
+        job_prefix = kwargs.pop('job_prefix', None)
 
         # Fill missing requirement
         ann = inspect.get_annotations(cls, eval_str=True)
         for k, v in ann.items():
             if get_origin(v) is Req and getattr(cls, k, None) is None:
                 req = Req()
                 req.__set_name__(None, k)
                 setattr(cls, k, req)
 
-        cls._task_config = TaskConfig(task_class=cls, channels=channels, compress_level=compress_level)
+        cls._task_config = TaskConfig(task_class=cls, channels=channels, compress_level=compress_level, job_prefix=job_prefix)
         super().__init_subclass__(**kwargs)
 
     def __init__(self, *args: P.args, **kwargs: P.kwargs) -> None:
         self._task_worker: TaskWorker[R] = TaskWorker.make(
                 self._task_config, self, *args, **kwargs
                 )
 
@@ -345,7 +377,17 @@
 Task = TaskType[..., R]
 TaskLike = Task[R] | Const[R] | _MappedTask[Any, R]
 
 
 Requires = Req[TaskLike[R], R]
 RequiresList = Req[Sequence[TaskLike[R]], list[R]]
 RequiresDict = Req[Mapping[K, TaskLike[R]], dict[K, R]]
+
+
+class SourceTask(TaskType[[], R]):
+    def build_task(self) -> None:
+        pass
+
+
+class SinkTask(TaskType[P, None]):
+    def run_task(self) -> None:
+        pass
```

### Comparing `checkpoint_tool-0.8.0/checkpoint/types.py` & `checkpoint_tool-0.9.0/checkpoint/types.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.8.0/pyproject.toml` & `checkpoint_tool-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkpoint-tool"
-version = "0.8.0"
+version = "0.9.0"
 description = "A lightweight workflow management tool written in pure Python"
 authors = ["Kohei Miyaguchi <koheimiyaguchi@gmail.com>"]
 license = "MIT License"
 homepage = "https://github.com/koheimiya/checkpoint"
 repository = "https://github.com/koheimiya/checkpoint"
 readme = "README.md"
 packages = [{include = "checkpoint"}]
```

### Comparing `checkpoint_tool-0.8.0/PKG-INFO` & `checkpoint_tool-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkpoint-tool
-Version: 0.8.0
+Version: 0.9.0
 Summary: A lightweight workflow management tool written in pure Python
 Home-page: https://github.com/koheimiya/checkpoint
 License: MIT
 Author: Kohei Miyaguchi
 Author-email: koheimiyaguchi@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -203,14 +203,22 @@
 which is then compressed with `gzip`.
 The compression level can be changed as follows (defaults to 9).
 ```python
 class NoCompressionTask(Task, compress_level=0):
     ...
 ```
 
+### Job scheduling and prefixes
+To run task on job schedulers, one can add prefix to the call of task.
+```python
+
+class TaskWithJobScheduler(Task, job_prefix=['jbsub', '-tty', '-queue x86_1h', '-cores 16+1', '-mem 64g', '-require a100_80gb']):
+    ...
+```
+
 ### Data directories
 
 Use `task.task_directory` to get a fresh path dedicated to each task.
 The directory is automatically created at
 `{$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.{task_name}/data/{task_id}`
 and the contents of the directory are cleared at each task call and persist until the task is cleared.
 ```python
```

