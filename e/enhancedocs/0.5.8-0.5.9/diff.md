# Comparing `tmp/enhancedocs-0.5.8.tar.gz` & `tmp/enhancedocs-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhancedocs-0.5.8.tar", max compression
+gzip compressed data, was "enhancedocs-0.5.9.tar", max compression
```

## Comparing `enhancedocs-0.5.8.tar` & `enhancedocs-0.5.9.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0    11341 2023-05-14 19:26:34.235742 enhancedocs-0.5.8/LICENSE
--rw-r--r--   0        0        0     1030 2023-05-14 19:26:34.235742 enhancedocs-0.5.8/README.md
--rw-r--r--   0        0        0      474 2023-05-14 19:26:34.235742 enhancedocs-0.5.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 19:26:34.235742 enhancedocs-0.5.8/src/enhancedocs/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 19:26:34.235742 enhancedocs-0.5.8/src/enhancedocs/commands/__init__.py
--rw-r--r--   0        0        0      167 2023-05-14 19:26:34.235742 enhancedocs-0.5.8/src/enhancedocs/commands/alpha/__init__.py
--rw-r--r--   0        0        0      148 2023-05-14 19:26:34.235742 enhancedocs-0.5.8/src/enhancedocs/commands/alpha/projects/__init__.py
--rw-r--r--   0        0        0     1645 2023-05-14 19:26:34.235742 enhancedocs-0.5.8/src/enhancedocs/commands/alpha/projects/create.py
--rw-r--r--   0        0        0     2802 2023-05-14 19:26:34.235742 enhancedocs-0.5.8/src/enhancedocs/commands/ask.py
--rw-r--r--   0        0        0     1315 2023-05-14 19:26:34.235742 enhancedocs-0.5.8/src/enhancedocs/commands/build.py
--rw-r--r--   0        0        0     1885 2023-05-14 19:26:34.235742 enhancedocs-0.5.8/src/enhancedocs/commands/push.py
--rw-r--r--   0        0        0     1151 2023-05-14 19:26:34.235742 enhancedocs-0.5.8/src/enhancedocs/config.py
--rw-r--r--   0        0        0      481 2023-05-14 19:26:34.235742 enhancedocs-0.5.8/src/enhancedocs/main.py
--rw-r--r--   0        0        0     1447 2023-05-14 19:26:34.235742 enhancedocs-0.5.8/src/enhancedocs/utils.py
--rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 enhancedocs-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-05-19 15:13:16.608054 enhancedocs-0.5.9/LICENSE
+-rw-r--r--   0        0        0     1030 2023-05-19 15:13:16.608054 enhancedocs-0.5.9/README.md
+-rw-r--r--   0        0        0      474 2023-05-19 15:13:16.612054 enhancedocs-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-19 15:13:16.612054 enhancedocs-0.5.9/src/enhancedocs/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 15:13:16.612054 enhancedocs-0.5.9/src/enhancedocs/commands/__init__.py
+-rw-r--r--   0        0        0      223 2023-05-19 15:13:16.612054 enhancedocs-0.5.9/src/enhancedocs/commands/alpha/__init__.py
+-rw-r--r--   0        0        0      149 2023-05-19 15:13:16.612054 enhancedocs-0.5.9/src/enhancedocs/commands/alpha/projects/__init__.py
+-rw-r--r--   0        0        0     1647 2023-05-19 15:13:16.612054 enhancedocs-0.5.9/src/enhancedocs/commands/alpha/projects/create.py
+-rw-r--r--   0        0        0      141 2023-05-19 15:13:16.612054 enhancedocs-0.5.9/src/enhancedocs/commands/alpha/sources/__init__.py
+-rw-r--r--   0        0        0      775 2023-05-19 15:13:16.612054 enhancedocs-0.5.9/src/enhancedocs/commands/alpha/sources/web.py
+-rw-r--r--   0        0        0     2802 2023-05-19 15:13:16.612054 enhancedocs-0.5.9/src/enhancedocs/commands/ask.py
+-rw-r--r--   0        0        0     1315 2023-05-19 15:13:16.612054 enhancedocs-0.5.9/src/enhancedocs/commands/build.py
+-rw-r--r--   0        0        0     1885 2023-05-19 15:13:16.612054 enhancedocs-0.5.9/src/enhancedocs/commands/push.py
+-rw-r--r--   0        0        0     1151 2023-05-19 15:13:16.612054 enhancedocs-0.5.9/src/enhancedocs/config.py
+-rw-r--r--   0        0        0      481 2023-05-19 15:13:16.612054 enhancedocs-0.5.9/src/enhancedocs/main.py
+-rw-r--r--   0        0        0     1447 2023-05-19 15:13:16.612054 enhancedocs-0.5.9/src/enhancedocs/utils.py
+-rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 enhancedocs-0.5.9/PKG-INFO
```

### Comparing `enhancedocs-0.5.8/LICENSE` & `enhancedocs-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.8/README.md` & `enhancedocs-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.8/src/enhancedocs/commands/alpha/projects/create.py` & `enhancedocs-0.5.9/src/enhancedocs/commands/alpha/projects/create.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,8 +37,8 @@
             response = requests.put(f'{api_base_url}/projects/{project["_id"]}/source/web',
                                     json={"url": url},
                                     headers=headers,
                                     )
             response.raise_for_status()
         except requests.exceptions.RequestException as err:
             raise click.ClickException(str(err))
-        click.echo(f'Project {name} has been sucesfully created')
+        click.echo(f'Project {name} has been successfully created')
```

### Comparing `enhancedocs-0.5.8/src/enhancedocs/commands/ask.py` & `enhancedocs-0.5.9/src/enhancedocs/commands/ask.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.8/src/enhancedocs/commands/build.py` & `enhancedocs-0.5.9/src/enhancedocs/commands/build.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.8/src/enhancedocs/commands/push.py` & `enhancedocs-0.5.9/src/enhancedocs/commands/push.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.8/src/enhancedocs/config.py` & `enhancedocs-0.5.9/src/enhancedocs/config.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.8/src/enhancedocs/utils.py` & `enhancedocs-0.5.9/src/enhancedocs/utils.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.8/PKG-INFO` & `enhancedocs-0.5.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enhancedocs
-Version: 0.5.8
+Version: 0.5.9
 Summary: EnhanceDocs Command Line Interface (CLI)
 License: Apache-2.0
 Author: Alvaro Molina
 Author-email: alw3ys@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

