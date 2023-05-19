# Comparing `tmp/llama-cli-1.0.18.tar.gz` & `tmp/llama-cli-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama-cli-1.0.18.tar", last modified: Fri May 19 08:18:02 2023, max compression
+gzip compressed data, was "/u/83/lehtint6/data/Documents/git/llama-cli/dist/tmp192loksv/llama-cli-1.0.6.tar", last modified: Thu Oct 14 16:00:41 2021, max compression
```

## Comparing `llama-cli-1.0.18.tar` & `llama-cli-1.0.6.tar`

### file list

```diff
@@ -1,49 +1,37 @@
-drwxr-xr-x   0 lehtint6 (1496283) domain users (70000)        0 2023-05-19 08:18:02.521009 llama-cli-1.0.18/
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1057 2022-03-21 09:43:33.000000 llama-cli-1.0.18/LICENSE
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     8224 2023-05-19 08:18:02.521009 llama-cli-1.0.18/PKG-INFO
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     7763 2022-05-10 09:41:30.000000 llama-cli-1.0.18/README.md
-drwxr-xr-x   0 lehtint6 (1496283) domain users (70000)        0 2023-05-19 08:18:02.513009 llama-cli-1.0.18/llama/
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     2890 2023-05-19 08:15:16.000000 llama-cli-1.0.18/llama/Config.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     6017 2023-02-02 09:02:50.000000 llama-cli-1.0.18/llama/Filters.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     4525 2022-09-21 04:51:26.000000 llama-cli-1.0.18/llama/LlamaApi.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)    11762 2022-03-29 14:03:16.000000 llama-cli-1.0.18/llama/LlamaStats.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     5833 2022-05-11 11:49:12.000000 llama-cli-1.0.18/llama/ProgSnap2.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     2232 2023-05-17 16:58:42.000000 llama-cli-1.0.18/llama/__init__.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)       56 2022-03-21 09:43:33.000000 llama-cli-1.0.18/llama/__main__.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     2495 2023-05-17 16:55:40.000000 llama-cli-1.0.18/llama/anonymize.py
-drwxr-xr-x   0 lehtint6 (1496283) domain users (70000)        0 2023-05-19 08:18:02.517009 llama-cli-1.0.18/llama/common/
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)      840 2022-03-28 05:53:39.000000 llama-cli-1.0.18/llama/common/__init__.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     3193 2022-05-11 07:55:45.000000 llama-cli-1.0.18/llama/common/dataframes.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1226 2023-04-05 09:01:02.000000 llama-cli-1.0.18/llama/common/files.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)      478 2022-03-21 09:43:33.000000 llama-cli-1.0.18/llama/common/input.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)       90 2022-03-28 05:53:24.000000 llama-cli-1.0.18/llama/common/series.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     3826 2023-02-02 08:48:49.000000 llama-cli-1.0.18/llama/exclude.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     2208 2023-05-17 17:22:44.000000 llama-cli-1.0.18/llama/fetch.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1438 2023-02-02 06:27:14.000000 llama-cli-1.0.18/llama/list.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1357 2022-09-21 04:52:26.000000 llama-cli-1.0.18/llama/operations.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     3209 2022-03-28 10:02:06.000000 llama-cli-1.0.18/llama/plotting.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)      968 2022-05-10 08:25:28.000000 llama-cli-1.0.18/llama/privacy.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)      188 2022-03-21 09:43:33.000000 llama-cli-1.0.18/llama/shell.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1029 2022-03-21 09:43:33.000000 llama-cli-1.0.18/llama/sources.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)      891 2023-04-05 09:49:58.000000 llama-cli-1.0.18/llama/status.py
-drwxr-xr-x   0 lehtint6 (1496283) domain users (70000)        0 2023-05-19 08:18:02.517009 llama-cli-1.0.18/llama/types/
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     6188 2023-05-17 17:19:22.000000 llama-cli-1.0.18/llama/types/AbstractApi.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)      563 2022-03-21 09:43:33.000000 llama-cli-1.0.18/llama/types/AbstractDjangoApi.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     2603 2022-09-20 17:46:57.000000 llama-cli-1.0.18/llama/types/AcosJsonApi.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     5678 2023-05-17 17:30:57.000000 llama-cli-1.0.18/llama/types/AplusApi.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     6727 2022-09-21 04:49:19.000000 llama-cli-1.0.18/llama/types/MongodumpApi.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1393 2022-04-06 09:09:27.000000 llama-cli-1.0.18/llama/types/__init__.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)      606 2022-04-06 11:05:43.000000 llama-cli-1.0.18/llama/types/acosjson.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)      865 2022-03-21 09:43:33.000000 llama-cli-1.0.18/llama/types/aplus.py
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1564 2022-07-12 07:13:28.000000 llama-cli-1.0.18/llama/types/mongodump.py
-drwxr-xr-x   0 lehtint6 (1496283) domain users (70000)        0 2023-05-19 08:18:02.521009 llama-cli-1.0.18/llama_cli.egg-info/
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     8224 2023-05-19 08:18:02.000000 llama-cli-1.0.18/llama_cli.egg-info/PKG-INFO
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)      909 2023-05-19 08:18:02.000000 llama-cli-1.0.18/llama_cli.egg-info/SOURCES.txt
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)        1 2023-05-19 08:18:02.000000 llama-cli-1.0.18/llama_cli.egg-info/dependency_links.txt
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)       37 2023-05-19 08:18:02.000000 llama-cli-1.0.18/llama_cli.egg-info/entry_points.txt
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)       33 2023-05-19 08:18:02.000000 llama-cli-1.0.18/llama_cli.egg-info/requires.txt
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)        6 2023-05-19 08:18:02.000000 llama-cli-1.0.18/llama_cli.egg-info/top_level.txt
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)      100 2022-03-21 09:43:33.000000 llama-cli-1.0.18/pyproject.toml
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)      669 2023-05-19 08:18:02.521009 llama-cli-1.0.18/setup.cfg
-drwxr-xr-x   0 lehtint6 (1496283) domain users (70000)        0 2023-05-19 08:18:02.521009 llama-cli-1.0.18/test/
--rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1627 2022-07-12 20:58:09.000000 llama-cli-1.0.18/test/test_filters.py
+drwxr-xr-x   0 lehtint6 (1496283) domain users (70000)        0 2021-10-14 16:00:41.000000 llama-cli-1.0.6/
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)      100 2021-10-13 15:30:09.000000 llama-cli-1.0.6/pyproject.toml
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     3873 2021-10-14 12:06:41.000000 llama-cli-1.0.6/README.md
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)      608 2021-10-14 16:00:41.000000 llama-cli-1.0.6/setup.cfg
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     4330 2021-10-14 16:00:41.000000 llama-cli-1.0.6/PKG-INFO
+drwxr-xr-x   0 lehtint6 (1496283) domain users (70000)        0 2021-10-14 16:00:41.000000 llama-cli-1.0.6/llama/
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1082 2021-10-12 11:07:59.000000 llama-cli-1.0.6/llama/status.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     2201 2021-10-14 11:10:07.000000 llama-cli-1.0.6/llama/__init__.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     4510 2021-10-14 15:49:53.000000 llama-cli-1.0.6/llama/exclude.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)      496 2021-10-14 15:25:56.000000 llama-cli-1.0.6/llama/operations.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)       56 2021-10-14 11:10:47.000000 llama-cli-1.0.6/llama/__main__.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1333 2021-10-13 11:57:12.000000 llama-cli-1.0.6/llama/anonymize.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     2292 2021-10-14 15:51:00.000000 llama-cli-1.0.6/llama/Llama.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1691 2021-10-14 15:31:49.000000 llama-cli-1.0.6/llama/fetch.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1350 2021-10-12 11:07:11.000000 llama-cli-1.0.6/llama/list.py
+drwxr-xr-x   0 lehtint6 (1496283) domain users (70000)        0 2021-10-14 16:00:41.000000 llama-cli-1.0.6/llama/types/
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)      938 2021-10-13 10:28:34.000000 llama-cli-1.0.6/llama/types/__init__.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)      865 2021-08-14 14:07:15.000000 llama-cli-1.0.6/llama/types/aplus.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     6482 2021-10-14 15:22:50.000000 llama-cli-1.0.6/llama/types/AbstractApi.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     4922 2021-10-14 15:53:52.000000 llama-cli-1.0.6/llama/types/AplusApi.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)      606 2021-08-28 03:31:01.000000 llama-cli-1.0.6/llama/types/AbstractDjangoApi.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1029 2021-08-18 09:08:13.000000 llama-cli-1.0.6/llama/sources.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     2528 2021-10-14 13:03:54.000000 llama-cli-1.0.6/llama/config.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)      968 2021-08-24 06:57:58.000000 llama-cli-1.0.6/llama/privacy.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     4151 2021-10-14 15:56:38.000000 llama-cli-1.0.6/llama/Filters.py
+drwxr-xr-x   0 lehtint6 (1496283) domain users (70000)        0 2021-10-14 16:00:41.000000 llama-cli-1.0.6/llama/common/
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)      400 2021-08-28 10:30:28.000000 llama-cli-1.0.6/llama/common/__init__.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1048 2021-10-13 07:36:47.000000 llama-cli-1.0.6/llama/common/files.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)      478 2021-08-14 07:41:23.000000 llama-cli-1.0.6/llama/common/input.py
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     1057 2021-10-14 06:40:25.000000 llama-cli-1.0.6/LICENSE
+drwxr-xr-x   0 lehtint6 (1496283) domain users (70000)        0 2021-10-14 16:00:41.000000 llama-cli-1.0.6/llama_cli.egg-info/
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)       38 2021-10-14 16:00:41.000000 llama-cli-1.0.6/llama_cli.egg-info/entry_points.txt
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)        6 2021-10-14 16:00:41.000000 llama-cli-1.0.6/llama_cli.egg-info/top_level.txt
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)        1 2021-10-14 16:00:41.000000 llama-cli-1.0.6/llama_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)     4330 2021-10-14 16:00:41.000000 llama-cli-1.0.6/llama_cli.egg-info/PKG-INFO
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)      659 2021-10-14 16:00:41.000000 llama-cli-1.0.6/llama_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 lehtint6 (1496283) domain users (70000)       16 2021-10-14 16:00:41.000000 llama-cli-1.0.6/llama_cli.egg-info/requires.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `llama-cli-1.0.18/LICENSE` & `llama-cli-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `llama-cli-1.0.18/llama/__init__.py` & `llama-cli-1.0.6/llama/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import sys
 from .common import find, require
-from .Config import Config, TIME_KEY, PERSON_KEY, GRADE_KEY
+from .config import Config
+from .Llama import Llama
 from . import status
 from . import sources
 from . import list
 from . import privacy
 from . import exclude
 from . import fetch
 from . import anonymize
-from . import shell
-from .LlamaApi import LlamaApi
-from .LlamaStats import LlamaStats
+
+VERSION = '1.0.0'
 
 COMMANDS = [
   {
     'cmd': 'status',
     'desc': 'Show the working tree status',
     'require': ['config'],
     'call': status.command,
@@ -51,23 +51,24 @@
     'cmd': 'anonymize',
     'desc': 'Export anonymized data',
     'require': ['config', 'source'],
     'call': anonymize.command,
   },
   {
     'cmd': 'shell',
-    'desc': 'Open python REPL with \'llama\' instance to export data',
-    'call': shell.command,
+    'desc': 'Open python REPL with \'llama\' instance to fetched data',
+    'require': ['config', 'source'],
+    'call': status.shell,
   }
 ]
 
 def llama_cli(cmd, args):
   definition = find(COMMANDS, lambda c: c['cmd'] == cmd)
   require(definition, 'Unknown command')
-  config = Config()
+  config = Config(VERSION)
   requirements = definition.get('require', [])
   if 'config' in requirements:
     require(config.exists, 'The working directory has no configuration (.llama)')
   if 'source' in requirements:
     require(config.sources, 'First, use command \'source\' to configure a data source')
   require(definition.get('call', None), 'FATAL: command missing implementation', 1)
   definition['call'](args, config)
```

### Comparing `llama-cli-1.0.18/llama/common/files.py` & `llama-cli-1.0.6/llama/common/files.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,31 +12,25 @@
 def ensure_dir(path):
   if type(path) != str:
     p = path[0]
     for i in range(0, len(path) - 1):
       mkdir(p)
       p = os.path.join(p, path[i + 1])
 
-def read_any(path, txt=False):
+def read_text(path):
   file_name = path_to_file_name(path)
   if not os.path.isfile(file_name):
     return None
-  with open(file_name, 'r' if txt else 'rb') as f:
+  with open(file_name) as f:
     return f.read()
 
-def write_any(path, data, txt=False):
-  ensure_dir(path)
-  with open(path_to_file_name(path), 'w' if txt else 'wb') as f:
-    f.write(data)
-
-def read_text(path):
-  return read_any(path, txt=True)
-
 def write_text(path, text):
-  write_any(path, text, txt=True)
+  ensure_dir(path)
+  with open(path_to_file_name(path), 'w') as f:
+    f.write(text)
 
 def read_json(path):
   text = read_text(path)
   return json.loads(text) if text else None
 
 def write_json(path, data):
   write_text(path, json.dumps(data, indent=2))
```

### Comparing `llama-cli-1.0.18/llama/exclude.py` & `llama-cli-1.0.6/llama/exclude.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,27 @@
+import re
 from .types import get_sources_with_tables
 from .list import print_sources
 from .Filters import Filters
-from .common import require, input_selection
+from .common import count, require, input_selection
+
+def parse_exclusion(pattern):
+  result = re.match(r'^(-)?(\d+:)?(#?[\w ]+)?(\.[\w ]+)?(=[\w ]+)?$', pattern)
+  if not result:
+    return None
+  re_groups = result.groups()
+  table_id = re_groups[2] and re_groups[2].startswith('#')
+  return {
+    'reverse': re_groups[0] == '-',
+    'source': int(re_groups[1][:-1]) if re_groups[1] else None,
+    'table_by_id': table_id,
+    'table': re_groups[2][1:] if table_id else re_groups[2],
+    'column': re_groups[3][1:] if re_groups[3] else None,
+    'value': re_groups[4][1:] if re_groups[4] else None,
+  }
 
 def format_exclusion(spec):
   reverse = '-' if spec['reverse'] else ''
   source = f'{spec["source"]}:' if not spec['source'] is None else ''
   table = f'{"#" if spec["table_by_id"] else ""}{spec["table"]}' if spec['table'] else ''
   column = f'.{spec["column"]}' if spec['column'] else ''
   value = f'={spec["value"]}' if spec['value'] else ''
@@ -43,15 +59,15 @@
     exc = config.exclude[i]
     config.set_exclude(e for j, e in enumerate(config.exclude) if j != i)
     print(f'Removed exclusion: {format_exclusion(exc)}')
   elif args == ['apply']:
     fl = Filters(config.exclude)
     print_sources(fl.filter(get_sources_with_tables(config)))
   else:
-    exc = Filters.parse(' '.join(args[1:]))
+    exc = parse_exclusion(' '.join(args[1:]))
     require(exc, 'Invalid exclude pattern')
     if exc['source']:
       require(0 <= exc['source'] < len(config.sources), 'Invalid source index')
     fl = Filters([exc])
     if fl.has_person_filters():
       _, sources = next(fl.person_filter_columns(get_sources_with_tables(config)))
       print_sources(sources)
@@ -65,11 +81,14 @@
       config.set_exclude(config.exclude + [exc])
       print(f'Added exclusion: {format_exclusion(exc)}')
 
 def status(config):
   lines = []
   if config.exclude:
     lines.append(' '.join(['Exclude:'] + [format_exclusion(e) for e in config.exclude]))
-    ps = Filters.person_status()
-    if ps:
-      lines.append(f'{ps["included"]}/{ps["total"]} ({ps["percent"]}%) persons included')
+  persons = Filters.person_status()
+  if persons:
+    total = len(persons)
+    included = count(p for p in persons if p['included'])
+    percent = round(100 * included / total)
+    lines.append(f'{included}/{total} ({percent}%) persons included')
   return '\n'.join(lines) if lines else None
```

### Comparing `llama-cli-1.0.18/llama/fetch.py` & `llama-cli-1.0.6/llama/fetch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,39 @@
 from .types import get_sources_with_tables
 from .Filters import Filters
-from .common import require
+from .common import write_json
 
-def get_filtered_table_rows(select_filter, config):
+def get_filtered_table_rows(config):
   fl = Filters(config.exclude)
-  for s in select_filter.filter(fl.filter(get_sources_with_tables(config))):
+  for s in fl.filter(get_sources_with_tables(config)):
     for t in s['tables']:
       rows, _ = s['api'].fetch_rows(t, only_cache=True)
       if rows is None:
         print(f'Skipping {t["name"]}: fetch rows first')
       else:
         yield s, t, rows
 
 def command(args, config):
-  target = args[0] if len(args) > 0 else None
-  if not target in ('rows', 'files', 'filesfix', 'meta'):
+  if not args in (['rows'], ['files'], ['meta']):
     print('Fetches learning data from sources\n')
-    print('usage: llama fetch <target> [<select>]\n')
-    print('   target    rows     new table rows')
-    print('             files    new file attachments for rows')
-    print('             meta     new meta attachments for rows')
-    print('   select    [-][source:](#table_id|partial_table_name)')
-    return
-  fls = Filters([], inclusive=True)
-  if len(args) > 1:
-    select = Filters.parse(' '.join(args[1:]), columns=False)
-    require(select, 'Invalid select pattern')
-    fls.add([select])
-  if target == 'rows':
+    print('usage: llama fetch <target>\n')
+    print('   rows      new table rows')
+    print('   files     new file attachments for rows')
+    print('   meta      new meta attachments for rows')
+  elif args == ['rows']:
     sources = get_sources_with_tables(config)
     fl = Filters(config.exclude)
     persons = fl.person_select(sources, config.privacy == 'none') if fl.has_person_filters() else None
-    for s in fls.filter(fl.filter(sources)):
+    for s in fl.filter(sources):
       for t in s['tables']:
         columns_rm = [c['key'] for c in t['columns_rm']] if 'columns_rm' in t else None
         s['api'].fetch_rows(t, config.privacy == 'none', False, persons, columns_rm)
-  elif target in ('files', 'filesfix'):
-    for source, table, rows in get_filtered_table_rows(fls, config):
-      for r in source['api'].fetch_files(
-        table,
-        rows,
-        include_personal=config.privacy == 'none',
-        fix_privacy=target == 'filesfix'
-      ):
+  elif args == ['files']:
+    for source, table, rows in get_filtered_table_rows(config):
+      for r in source['api'].fetch_files(table, rows, config.privacy == 'none'):
         if r['cached']:
           print(f'* Cached file {"/".join(r["path"])}')
-  elif target == 'meta':
-    for source, table, rows in get_filtered_table_rows(fls, config):
+  elif args == ['meta']:
+    for source, table, rows in get_filtered_table_rows(config):
       for r in source['api'].fetch_meta(table, rows, config.privacy == 'none'):
         if r['cached']:
           print(f'* Cached meta {"/".join(r["path"])}')
```

### Comparing `llama-cli-1.0.18/llama/list.py` & `llama-cli-1.0.6/llama/list.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from .types import enumerate_sources
 from .operations import last_time
 from .common import count
-from .Filters import Filters
 
 def format_source(i, name):
   return f'{i:d}: {name}'
 
 def format_table(id, name, columns):
   return f'#{id} "{name}".[{",".join(c["key"] for c in columns)}]'
 
@@ -28,11 +27,9 @@
       for t in tables:
         print(format_table(t['id'], t['name'], t['columns']), end=' ')
         rows, _ = api.fetch_rows(t, only_cache=True)
         rows_n = 0 if rows is None else rows.shape[0]
         if not rows is None and count(api.file_columns(t, rows)) > 0:
           file_n = count(api.fetch_files(t, rows, only_cache=True))
           print(f'{rows_n} rows, {file_n} files, last {last_time(rows)}')
-        elif rows_n > 0:
-          print(f'{rows_n} rows, last {last_time(rows)}')
         else:
-          print('0 rows fetched')
+          print(f'{rows_n} rows, last {last_time(rows)}')
```

### Comparing `llama-cli-1.0.18/llama/privacy.py` & `llama-cli-1.0.6/llama/privacy.py`

 * *Files identical despite different names*

### Comparing `llama-cli-1.0.18/llama/sources.py` & `llama-cli-1.0.6/llama/sources.py`

 * *Files identical despite different names*

### Comparing `llama-cli-1.0.18/llama/status.py` & `llama-cli-1.0.6/llama/status.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from .types import enumerate_sources
-from .common import require
 from . import exclude
 from . import privacy
+from .types import enumerate_sources
+from .common import require
+from .Llama import Llama
 
 def status_sources(config):
   if not config.sources:
     return "No data sources configured"
   lines = []
   for i, src, api in enumerate_sources(config):
     tables, cached = api.list_tables(only_cache=True)
-    lines.append(f'{i:d}: {src["name"]} [{src["type"]}]')
+    lines.append(f'{i:d}: {src["name"]} [{src["id"]}]')
     if cached:
       lines.append(f'   {len(tables)} tables')
     else:
       lines.append('   No table list loaded, use "list" command')
   return '\n'.join(lines)
 
 def status(config):
@@ -26,7 +27,14 @@
     privacy.status(config)
   ]
   return '\n'.join(l for l in lines if not l is None)
 
 def command(args, config):
   require(args == [], 'Unknown command')
   print(status(config))
+
+def shell(args, config):
+  require(args == [], 'Unknown command')
+  import code
+  code.interact('Use "llama" to access data', local={
+    'llama': Llama(config),
+  })
```

### Comparing `llama-cli-1.0.18/llama/types/AbstractApi.py` & `llama-cli-1.0.6/llama/types/AbstractApi.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import os
 import time
 import io
 import json
 import requests
 import pandas
-from ..Config import STORAGE_DIR, TIME_KEY, PERSON_KEY
-from ..operations import ensure_column_types
-from ..common import read_json, write_json, read_csv, write_csv, read_any, write_any
+from ..common import read_json, write_json, read_csv, write_csv, read_text, write_text
+from ..config import PERSON_KEY, STORAGE_DIR, EXPORT_DIR, TIME_KEY
 
 class AbstractApi:
 
   TABLE_LIST_JSON = '{source_id}-tables.json'
   TABLE_CSV = '{source_id}-{table_id}-rows.csv'
   TABLE_DIR = '{source_id}-{table_id}'
   ITEM_DIR = '{user_id}-{time}'
-  META_JSON = 'meta.json'
 
   REQUEST_DELAY = 1 #sec
 
   def __init__(self, source_id):
     self.source_id = source_id
 
   def list_tables(self, try_cache=True, only_cache=False):
@@ -41,102 +39,109 @@
         new_rows = self.fetch_rows_csv(table, rows, include_personal, select_persons, exclude_columns)
         if not new_rows is None:
           write_csv(self.table_csv_name(table['id']), new_rows)
           rows = new_rows
           self.fetch_delay()
     else:
       self.fetch_delay()
-    ensure_column_types(rows)
+    rows[TIME_KEY] = pandas.to_datetime(rows[TIME_KEY])
     return rows, cached
 
-  def fetch_files(self, table, rows, include_personal=False, only_cache=False, fix_privacy=False):
+  def fetch_files(self, table, rows, include_personal=False, only_cache=False):
     file_cols = self.file_columns(table, rows)
     table_dir = self.table_dir_name(table['id'])
     for _, row in rows.iterrows():
       item_dir = self.item_dir_name(row)
       for c in file_cols:
         path = (STORAGE_DIR, table_dir, item_dir, c)
         content, cached = self.cached_or_fetch(
-          lambda: read_any(path),
+          lambda: read_text(path),
           lambda: self.fetch_file(table, row, c, include_personal),
-          lambda r: write_any(path, r),
+          lambda r: write_text(path, r),
           True,
           only_cache
         )
-        if fix_privacy and cached:
-          write_any(path, self.fix_file_privacy(table, row, c, content))
         if not content is None and not cached:
           self.fetch_delay()
         yield { 'row': row, 'col': c, 'path': path, 'content': content, 'cached': cached }
 
   def fetch_meta(self, table, rows, include_personal=False, only_cache=False):
     table_dir = self.table_dir_name(table['id'])
     for _, row in rows.iterrows():
       item_dir = self.item_dir_name(row)
-      path = (STORAGE_DIR, table_dir, item_dir, self.META_JSON)
+      path = (STORAGE_DIR, table_dir, item_dir, 'meta.json')
       content, cached = self.cached_json_or_fetch(
         lambda: self.fetch_meta_json(table, row, include_personal),
         path,
         True,
         only_cache
       )
       if not content is None and not cached:
         self.fetch_delay()
       yield { 'row': row, 'path': path, 'content': content, 'cached': cached }
 
-  def export_rows(self, table, rows, person_map, metas=False, volatile_columns=None):
-    data = self.drop_for_export(table, rows, volatile_columns)
+  def write_export(self, table, rows, person_map):
+    data = self.drop_for_export(table, rows)
     data[PERSON_KEY] = data[PERSON_KEY].map(person_map)
     data = data.dropna(subset=[PERSON_KEY]).reset_index(drop=True)
     table_dir = self.table_dir_name(table['id'])
     file_cols = self.file_columns(table, rows)
     def rewrite_files(row):
       item_dir = self.item_dir_name(row)
       for c in file_cols:
         row[c] = os.path.join(table_dir, item_dir, c)
       return row
     data = data.apply(rewrite_files, 1)
-    if metas:
-      data['RowMeta'] = [
-        os.path.join(table_dir, self.item_dir_name(row), self.META_JSON)
-        for _, row in data.iterrows()
-      ]
-    return data
+    write_csv(self.table_csv_name(table['id'], export=True), data)
+  
+  def get_export_rows(self, table):
+    return read_csv(self.table_csv_name(table['id'], export=True))
+
+  def get_export_files(self, table, rows):
+    file_cols = self.file_columns(table, rows)
+    table_dir = self.table_dir_name(table['id'])
+    for _, row in rows.iterrows():
+      item_dir = self.item_dir_name(row)
+      for c in file_cols:
+        path = (EXPORT_DIR, table_dir, item_dir, c)
+        yield { 'row': row, 'col': c, 'path': path, 'content': read_json(path) }
+
+  def get_export_meta(self, table, rows):
+    table_dir = self.table_dir_name(table['id'])
+    for _, row in rows.iterrows():
+      path = (EXPORT_DIR, table_dir, self.item_dir_name(row), 'meta.json')
+      yield { 'row': row, 'path': path, 'content': read_text(path) }
 
   def fetch_tables_json(self):
     raise NotImplementedError()
 
   def fetch_rows_csv(self, table, old_rows, include_personal, select_persons, exclude_columns):
-    # MUST use default keys if appropriate columns: TIME_KEY, PERSON_KEY, GRADE_KEY
     # Should optimize the queries to extend previous data, if possible.
     raise NotImplementedError()
   
   def fetch_meta_json(self, table, row, include_personal):
     raise NotImplementedError()
 
   def file_columns(self, table, rows):
     raise NotImplementedError()
 
   def fetch_file(self, table, row, col_name, include_personal):
     raise NotImplementedError()
 
-  def fix_file_privacy(self, table, row, col_name, content):
-    raise NotImplementedError()
-
   def drop_for_export(self, table, rows):
     raise NotImplementedError()
 
   def table_list_json_name(self):
     return (
       self.TABLE_LIST_JSON.format(source_id=self.source_id),
     )
 
-  def table_csv_name(self, table_id):
+  def table_csv_name(self, table_id, export=False):
     return (
-      STORAGE_DIR,
+      EXPORT_DIR if export else STORAGE_DIR,
       self.TABLE_CSV.format(source_id=self.source_id, table_id=table_id),
     )
 
   def table_dir_name(self, table_id):
     return self.TABLE_DIR.format(source_id=self.source_id, table_id=table_id)
 
   def item_dir_name(self, row):
```

### Comparing `llama-cli-1.0.18/llama/types/AbstractDjangoApi.py` & `llama-cli-1.0.6/llama/types/AbstractDjangoApi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .AbstractApi import AbstractApi
+from ..common import read_json, write_json
 
 class AbstractDjangoApi(AbstractApi):
 
   def __init__(self, source_id, token):
     super().__init__(source_id)
     self.token = token
```

### Comparing `llama-cli-1.0.18/llama/types/AplusApi.py` & `llama-cli-1.0.6/llama/types/AplusApi.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,43 @@
-import os
 import re
-from ..Config import PERSON_KEY, GRADE_KEY
+from ..config import PERSON_KEY
 from .AbstractDjangoApi import AbstractDjangoApi
 
 class AplusApi(AbstractDjangoApi):
 
   API_URL = '{host}/api/v2/'
   COURSE_LIST = '{url}courses/'
   EXERCISE_LIST = '{url}courses/{course_id:d}/exercises/'
   SUBMISSION_ROWS = '{url}courses/{course_id:d}/submissiondata/?exercise_id={exercise_id:d}&best=no&format=csv'
   SUBMISSION_DETAILS = '{url}submissions/{submission_id:d}'
 
   STATUS_KEY = 'Status'
+  GRADE_KEY = 'Grade'
   PENALTY_KEY = 'Penalty'
   PSEUDO_USER_KEY = 'UserID'
   PSEUDO_ITEM_KEY = 'SubmissionID'
-  REMOVE_KEYS = [PSEUDO_USER_KEY, STATUS_KEY, 'ExerciseID', 'Category', 'Exercise', 'Graded', 'GraderEmail', 'Notified', 'NSeen', '_aplus_group', '__grader_lang']
+  REMOVE_KEYS = [PSEUDO_USER_KEY, STATUS_KEY, PENALTY_KEY, 'ExerciseID', 'Category', 'Exercise', 'Graded', 'GraderEmail', 'Notified', 'NSeen', '_aplus_group', '__grader_lang']
   REMOVE_PERSONAL_KEYS = ['StudentID', 'Email']
   REMOVE_AT_EXPORT = [PSEUDO_ITEM_KEY] + REMOVE_PERSONAL_KEYS
   META_KEYS = ['exercise', 'submission_time', 'grading_time', 'grade', 'late_penalty_applied', 'feedback', 'grading_data']
   FILE_KEY_REGEXP = r'^file\d+$'
   FILE_VAL_REGEXP = r'^https:\/\/[^?]+'
-  PERSONAL_FILE_REGEXP = r'^.*filename=\"[^\"]+\.(txt|py|java|scala|c|cpp|js|mat)\".*$'
-  PERSONAL_REGEXP = r'# (Nimi|Opiskelijanumero): [\w -]*'
+  PERSONAL_REGEXP = r'^# (Nimi|Opiskelijanumero): .*$'
 
   @classmethod
   def create(cls, host, token):
     url = cls.API_URL.format(host=f'{"" if "://" in host else "https://"}{host}')
     return AplusApi(url, token), url
 
   def __init__(self, url, token, course_id=None):
     super().__init__(course_id, token)
     self.url = url
     self.course_id = course_id
     self.file_key_re = re.compile(self.FILE_KEY_REGEXP)
     self.file_val_re = re.compile(self.FILE_VAL_REGEXP)
-    self.personal_file_re = re.compile(self.PERSONAL_FILE_REGEXP, flags=re.I)
     self.personal_re = re.compile(self.PERSONAL_REGEXP, flags=re.I | re.M)
 
   def list_courses(self):
     courses = self.get_paged_json(self.COURSE_LIST.format(url=self.url))
     courses.sort(key=lambda c: c['id'], reverse=True)
     return courses  
 
@@ -51,52 +49,49 @@
         entry = {
           'module_id': m['id'],
           'module_name': self.en_name(m['display_name']),
           'id': e['id'],
           'name': self.en_name(e['display_name']),
           'max_points': e['max_points'],
           'max_submissions': e['max_submissions'],
-          'difficulty': e.get('difficulty'),
         }
         self.fetch_delay()
         details = self.fetch_json(e['url'])
         form = (details.get('exercise_info') or {}).get('form_spec', [])
         entry['columns'] = [{ 'key': f['key'] } for f in form if f['type'] != 'static']
         tables.append(entry)
     return tables
 
   def fetch_rows_csv(self, table, old_rows, include_personal, select_persons, exclude_columns):
 
     # NOTE: A-plus does not offer filtering by time or id to extend previously fetched rows
     if not old_rows is None:
-      print(f'* Cached {table["name"]}: to update, remove {os.path.join(*self.table_csv_name(table["id"]))}')
+      print(f'* Cached {table["name"]}: to update, remove {self.table_csv_name(table["id"])}')
       return None
 
     url = self.SUBMISSION_ROWS.format(url=self.url, course_id=self.course_id, exercise_id=table['id'])
     data = self.fetch_csv(url)
     
     # Reject rows where status NOT 'ready'
     if self.STATUS_KEY in data:
       data = data[data[self.STATUS_KEY] == 'ready']
 
     # Filter rows by persons
     if not select_persons is None:
-      data = data[data[self.PSEUDO_USER_KEY].astype(str).isin(select_persons)]
+      data = data[data[self.PSEUDO_USER_KEY].isin(select_persons)]
 
     # Cancel late penalties to keep all grades comparable
     def cancel_apply(row):
       if row[self.PENALTY_KEY] > 0:
-        row[GRADE_KEY] /= row[self.PENALTY_KEY]
+        row[self.GRADE_KEY] /= row[self.PENALTY_KEY]
       return row
     if self.PENALTY_KEY in data:
       data = data.apply(cancel_apply, 1)
 
-    # Use default column keys:
-    # TIME_KEY matches
-    # GRADE_KEY matches
+    # Use default column keys, TIME_KEY matches
     data[PERSON_KEY] = data[self.PSEUDO_USER_KEY]
 
     # Filter extra columns
     rm_cols = self.REMOVE_KEYS
     if not include_personal:
       rm_cols.extend(self.REMOVE_PERSONAL_KEYS)
     if exclude_columns:
@@ -105,37 +100,26 @@
 
   def file_columns(self, table, rows):
     return [c for c in rows.columns if self.file_key_re.match(c)]
   
   def fetch_file(self, table, row, col_name, include_personal):
     url_match = self.file_val_re.match(row[col_name])
     if url_match:
-      r = self.fetch(url_match.group(0))
-      cd = r.headers.get('content-disposition')
-      if not include_personal and self.personal_file_re.match(cd):
-        return self.personal_re.sub('', r.text).encode()
-      return r.content
+      content = self.fetch(url_match.group(0)).text
+      if not include_personal:
+        content = self.personal_re.sub('', content)
+      return content
     return None
 
-  def fix_file_privacy(self, table, row, col_name, content):
-    try:
-      return self.personal_re.sub('', content.decode()).encode()
-    except UnicodeDecodeError:
-      return self.fetch_file(table, row, col_name, False)
-
   def fetch_meta_json(self, table, row, include_personal):
     url = self.SUBMISSION_DETAILS.format(url=self.url, submission_id=row[self.PSEUDO_ITEM_KEY])
     data = self.fetch_json(url)
     return { k: data.get(k) for k in self.META_KEYS }
 
-  def drop_for_export(self, table, rows, volatile_columns):
-    pere = self.personal_re
-    for name in volatile_columns or []:
-      if name in rows.columns:
-        rows[name] = rows[name].apply(lambda s: pere.sub('', str(s)) if s else s)
+  def drop_for_export(self, table, rows):
     return rows.drop(columns=[c for c in rows.columns if c in self.REMOVE_AT_EXPORT])
 
   @staticmethod
   def en_name(name):
     return ''.join(
       (p[3:] if p.startswith('en:') else p).replace('  ', ' ')
       for p in name.split('|')
```

### Comparing `llama-cli-1.0.18/llama/types/aplus.py` & `llama-cli-1.0.6/llama/types/aplus.py`

 * *Files identical despite different names*

