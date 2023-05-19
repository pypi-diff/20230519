# Comparing `tmp/elements-0.3.2.tar.gz` & `tmp/elements-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elements-0.3.2.tar", last modified: Mon Jul  5 19:11:55 2021, max compression
+gzip compressed data, was "elements-0.4.0.tar", last modified: Fri May 19 10:30:46 2023, max compression
```

## Comparing `elements-0.3.2.tar` & `elements-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,25 @@
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2021-07-05 19:11:55.095886 elements-0.3.2/
--rw-r-----   0 danijar  (322066) primarygroup (89939)      486 2021-07-05 19:11:55.095886 elements-0.3.2/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)       76 2021-04-21 22:19:36.000000 elements-0.3.2/README.md
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2021-07-05 19:11:55.095886 elements-0.3.2/elements/
--rw-r-----   0 danijar  (322066) primarygroup (89939)      374 2021-04-21 22:21:02.000000 elements-0.3.2/elements/__init__.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     5092 2021-06-30 01:59:41.000000 elements-0.3.2/elements/config.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      458 2021-04-21 22:21:02.000000 elements-0.3.2/elements/counter.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     4715 2021-06-03 20:26:01.000000 elements-0.3.2/elements/logger.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2887 2021-07-05 19:10:55.000000 elements-0.3.2/elements/parser.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      711 2021-04-22 16:07:35.000000 elements-0.3.2/elements/when.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2021-07-05 19:11:55.095886 elements-0.3.2/elements.egg-info/
--rw-r-----   0 danijar  (322066) primarygroup (89939)      486 2021-07-05 19:11:54.000000 elements-0.3.2/elements.egg-info/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)      292 2021-07-05 19:11:54.000000 elements-0.3.2/elements.egg-info/SOURCES.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2021-07-05 19:11:54.000000 elements-0.3.2/elements.egg-info/dependency_links.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       14 2021-07-05 19:11:54.000000 elements-0.3.2/elements.egg-info/requires.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        9 2021-07-05 19:11:54.000000 elements-0.3.2/elements.egg-info/top_level.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2021-07-05 19:11:55.095886 elements-0.3.2/setup.cfg
--rw-r-----   0 danijar  (322066) primarygroup (89939)      555 2021-07-05 19:11:39.000000 elements-0.3.2/setup.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-19 10:30:46.022923 elements-0.4.0/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1058 2023-05-19 09:08:34.000000 elements-0.4.0/LICENSE
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10156 2023-05-19 10:30:46.022923 elements-0.4.0/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     9796 2023-05-19 10:30:19.000000 elements-0.4.0/README.md
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-19 10:30:46.022923 elements-0.4.0/elements/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      303 2023-05-19 09:19:59.000000 elements-0.4.0/elements/__init__.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3109 2023-05-19 09:08:22.000000 elements-0.4.0/elements/checkpoint.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     5954 2023-05-19 09:08:01.000000 elements-0.4.0/elements/config.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      783 2023-05-19 09:10:31.000000 elements-0.4.0/elements/counter.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3237 2023-05-19 09:14:41.000000 elements-0.4.0/elements/flags.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    11498 2023-05-19 10:10:41.000000 elements-0.4.0/elements/logger.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     5456 2023-05-19 09:08:15.000000 elements-0.4.0/elements/path.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     6050 2023-05-19 09:07:53.000000 elements-0.4.0/elements/plotting.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1878 2023-05-19 09:07:56.000000 elements-0.4.0/elements/timer.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2958 2023-05-19 09:05:42.000000 elements-0.4.0/elements/usage.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1872 2023-05-19 09:06:23.000000 elements-0.4.0/elements/uuid.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1671 2023-05-19 09:06:29.000000 elements-0.4.0/elements/when.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-19 10:30:46.022923 elements-0.4.0/elements.egg-info/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10156 2023-05-19 10:30:45.000000 elements-0.4.0/elements.egg-info/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      413 2023-05-19 10:30:45.000000 elements-0.4.0/elements.egg-info/SOURCES.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2023-05-19 10:30:45.000000 elements-0.4.0/elements.egg-info/dependency_links.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       14 2023-05-19 10:30:45.000000 elements-0.4.0/elements.egg-info/requires.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        9 2023-05-19 10:30:45.000000 elements-0.4.0/elements.egg-info/top_level.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2023-05-19 10:30:46.022923 elements-0.4.0/setup.cfg
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      555 2023-05-19 09:09:01.000000 elements-0.4.0/setup.py
```

### Comparing `elements-0.3.2/elements/config.py` & `elements-0.4.0/elements/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,57 @@
+import io
 import json
 import re
 
+from . import path
+
 
 class Config(dict):
 
   SEP = '.'
   IS_PATTERN = re.compile(r'.*[^A-Za-z0-9_.-].*')
 
   def __init__(self, *args, **kwargs):
     mapping = dict(*args, **kwargs)
     mapping = self._flatten(mapping)
     mapping = self._ensure_keys(mapping)
     mapping = self._ensure_values(mapping)
     self._flat = mapping
     self._nested = self._nest(mapping)
     # Need to assign the values to the base class dictionary so that
-    # conversion to dict does not loose the content.
+    # conversion to dict does not lose the content.
     super().__init__(self._nested)
 
   @property
   def flat(self):
     return self._flat.copy()
 
+  def save(self, filename):
+    filename = path.Path(filename)
+    if filename.suffix == '.json':
+      filename.write(json.dumps(dict(self)))
+    elif filename.suffix in ('.yml', '.yaml'):
+      import ruamel.yaml as yaml
+      with io.StringIO() as stream:
+        yaml.safe_dump(dict(self), stream)
+        filename.write(stream.getvalue())
+    else:
+      raise NotImplementedError(filename.suffix)
+
+  @classmethod
+  def load(cls, filename):
+    filename = path.Path(filename)
+    if filename.suffix == '.json':
+      return cls(json.loads(filename.read_text()))
+    elif filename.suffix in ('.yml', '.yaml'):
+      import ruamel.yaml as yaml
+      return cls(yaml.safe_load(filename.read_text()))
+    else:
+      raise NotImplementedError(filename.suffix)
+
   def __contains__(self, name):
     try:
       self[name]
       return True
     except KeyError:
       return False
 
@@ -36,15 +62,18 @@
       return self[name]
     except KeyError:
       raise AttributeError(name)
 
   def __getitem__(self, name):
     result = self._nested
     for part in name.split(self.SEP):
-      result = result[part]
+      try:
+        result = result[part]
+      except TypeError:
+        raise KeyError
     if isinstance(result, dict):
       result = type(self)(result)
     return result
 
   def __setattr__(self, key, value):
     if key.startswith('_'):
       return super().__setattr__(key, value)
@@ -93,15 +122,15 @@
             if float(int(new)) != new:
               message = f"Cannot convert fractional float {new} to int."
               raise ValueError(message)
           result[key] = type(old)(new)
         except (ValueError, TypeError):
           raise TypeError(
               f"Cannot convert '{new}' to type '{type(old).__name__}' " +
-              f"of value '{old}' for key '{key}'.")
+              f"for key '{key}' with previous value '{old}'.")
     return type(self)(result)
 
   def _flatten(self, mapping):
     result = {}
     for key, value in mapping.items():
       if isinstance(value, dict):
         for k, v in self._flatten(value).items():
```

### Comparing `elements-0.3.2/elements/parser.py` & `elements-0.4.0/elements/flags.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import re
 import sys
 
-from .config import Config
+from . import config
 
 
-class FlagParser:
+class Flags:
 
   def __init__(self, *args, **kwargs):
-    self._config = Config(*args, **kwargs)
+    self._config = config.Config(*args, **kwargs)
 
-  def parse(self, argv=None, exit_on_help=True):
-    config, remaining = self.parse_known(argv, exit_on_help)
+  def parse(self, argv=None, help_exits=True):
+    parsed, remaining = self.parse_known(argv)
     for flag in remaining:
       if flag.startswith('--'):
         raise ValueError(f"Flag '{flag}' did not match any config keys.")
     assert not remaining, remaining
-    return config
+    return parsed
 
-  def parse_known(self, argv=None, exit_on_help=True):
+  def parse_known(self, argv=None, help_exits=False):
     if argv is None:
       argv = sys.argv[1:]
     if '--help' in argv:
       print('\nHelp:')
       lines = str(self._config).split('\n')[2:]
       print('\n'.join('--' + re.sub(r'[:,\[\]]', '', x) for x in lines))
-      exit_on_help and sys.exit()
+      help_exits and sys.exit()
     parsed = {}
     remaining = []
     key = None
     vals = None
     for arg in argv:
       if arg.startswith('--'):
         if key:
@@ -40,54 +40,63 @@
           key, vals = arg, []
       else:
         if key:
           vals.append(arg)
         else:
           remaining.append(arg)
     self._submit_entry(key, vals, parsed, remaining)
-    return self._config.update(parsed), remaining
+    parsed = self._config.update(parsed)
+    return parsed, remaining
 
   def _submit_entry(self, key, vals, parsed, remaining):
+    if not key and not vals:
+      return
     if not key:
       vals = ', '.join(f"'{x}'" for x in vals)
-      raise ValueError(f"Values {vals} were not preceeded by any flag.")
+      raise ValueError(f"Values {vals} were not preceded by any flag.")
     name = key[len('--'):]
     if '=' in name:
       remaining.extend([key] + vals)
       return
-    if self._config.IS_PATTERN.match(name):
+    if self._config.IS_PATTERN.fullmatch(name):
       pattern = re.compile(name)
-      keys = {k for k in self._config.flat if pattern.match(k)}
+      keys = {k for k in self._config.flat if pattern.fullmatch(k)}
     elif name in self._config:
       keys = [name]
     else:
       keys = []
     if not keys:
       remaining.extend([key] + vals)
       return
     if not vals:
       raise ValueError(f"Flag '{key}' was not followed by any values.")
     for key in keys:
-      parsed[key] = parse_flag_value(self._config[key], vals, key)
-
+      parsed[key] = self._parse_flag_value(self._config[key], vals, key)
 
-def parse_flag_value(default, value, key):
-  value = value if isinstance(value, (tuple, list)) else (value,)
-  if isinstance(default, (tuple, list)):
-    if len(value) == 1 and ',' in value[0]:
-      value = value[0].split(',')
-    return tuple(parse_flag_value(default[0], [x], key) for x in value)
-  assert len(value) == 1, value
-  value = str(value[0])
-  if default is None:
-    return value
-  if isinstance(default, bool):
-    try:
-      return bool(['False', 'True'].index(value))
-    except ValueError:
-      raise TypeError(f"Expected bool but got '{value}' for key '{key}'.")
-  if isinstance(default, int):
-    value = float(value)  # Allow scientific notation for integers.
-    if float(int(value)) != value:
-      raise TypeError(f"Expected int but got float '{value}' for key '{key}'.")
-    return int(value)
-  return type(default)(value)
+  def _parse_flag_value(self, default, value, key):
+    value = value if isinstance(value, (tuple, list)) else (value,)
+    if isinstance(default, (tuple, list)):
+      if len(value) == 1 and ',' in value[0]:
+        value = value[0].split(',')
+      return tuple(self._parse_flag_value(default[0], [x], key) for x in value)
+    assert len(value) == 1, value
+    value = str(value[0])
+    if default is None:
+      return value
+    if isinstance(default, bool):
+      try:
+        return bool(['False', 'True'].index(value))
+      except ValueError:
+        message = f"Expected bool but got '{value}' for key '{key}'."
+        raise TypeError(message)
+    if isinstance(default, int):
+      try:
+        value = float(value)  # Allow scientific notation for integers.
+        assert float(int(value)) == value
+      except (TypeError, AssertionError):
+        message = f"Expected int but got float '{value}' for key '{key}'."
+        raise TypeError(message)
+      return int(value)
+    if isinstance(default, dict):
+      raise TypeError(
+          f"Key '{key}' refers to a whole dict. Please speicfy a subkey.")
+    return type(default)(value)
```

### Comparing `elements-0.3.2/setup.py` & `elements-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 import pathlib
 
 
 setuptools.setup(
     name='elements',
-    version='0.3.2',
+    version='0.4.0',
     description='Building blocks for productive research.',
     url='http://github.com/danijar/elements',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     packages=['elements'],
     install_requires=['numpy', 'imageio'],
     classifiers=[
```

