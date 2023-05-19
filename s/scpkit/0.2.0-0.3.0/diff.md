# Comparing `tmp/scpkit-0.2.0.tar.gz` & `tmp/scpkit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scpkit-0.2.0.tar", last modified: Fri Apr 28 19:53:59 2023, max compression
+gzip compressed data, was "scpkit-0.3.0.tar", last modified: Fri May 19 18:56:08 2023, max compression
```

## Comparing `scpkit-0.2.0.tar` & `scpkit-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:53:59.817956 scpkit-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-28 19:53:48.000000 scpkit-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-28 19:53:59.817956 scpkit-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-04-28 19:53:48.000000 scpkit-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 19:53:48.000000 scpkit-0.2.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:53:59.813955 scpkit-0.2.0/scpkit/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 19:53:48.000000 scpkit-0.2.0/scpkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-28 19:53:48.000000 scpkit-0.2.0/scpkit/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:53:59.817956 scpkit-0.2.0/scpkit/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:53:48.000000 scpkit-0.2.0/scpkit/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-04-28 19:53:48.000000 scpkit-0.2.0/scpkit/src/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-28 19:53:48.000000 scpkit-0.2.0/scpkit/src/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-28 19:53:48.000000 scpkit-0.2.0/scpkit/src/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-28 19:53:48.000000 scpkit-0.2.0/scpkit/src/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:53:59.813955 scpkit-0.2.0/scpkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-28 19:53:59.000000 scpkit-0.2.0/scpkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-28 19:53:59.000000 scpkit-0.2.0/scpkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:53:59.000000 scpkit-0.2.0/scpkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-28 19:53:59.000000 scpkit-0.2.0/scpkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:53:59.000000 scpkit-0.2.0/scpkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 19:53:59.000000 scpkit-0.2.0/scpkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 19:53:59.000000 scpkit-0.2.0/scpkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-28 19:53:59.817956 scpkit-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 19:53:48.000000 scpkit-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:53:59.817956 scpkit-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-04-28 19:53:48.000000 scpkit-0.2.0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:56:08.132303 scpkit-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 18:55:59.000000 scpkit-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-19 18:56:08.132303 scpkit-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-19 18:55:59.000000 scpkit-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 18:55:59.000000 scpkit-0.3.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:56:08.132303 scpkit-0.3.0/scpkit/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 18:55:59.000000 scpkit-0.3.0/scpkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-19 18:55:59.000000 scpkit-0.3.0/scpkit/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:56:08.132303 scpkit-0.3.0/scpkit/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:55:59.000000 scpkit-0.3.0/scpkit/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-19 18:55:59.000000 scpkit-0.3.0/scpkit/src/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-19 18:55:59.000000 scpkit-0.3.0/scpkit/src/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-19 18:55:59.000000 scpkit-0.3.0/scpkit/src/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-19 18:55:59.000000 scpkit-0.3.0/scpkit/src/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:56:08.132303 scpkit-0.3.0/scpkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-19 18:56:08.000000 scpkit-0.3.0/scpkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-19 18:56:08.000000 scpkit-0.3.0/scpkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:56:08.000000 scpkit-0.3.0/scpkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-19 18:56:08.000000 scpkit-0.3.0/scpkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:56:07.000000 scpkit-0.3.0/scpkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-19 18:56:08.000000 scpkit-0.3.0/scpkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 18:56:08.000000 scpkit-0.3.0/scpkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-19 18:56:08.132303 scpkit-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 18:55:59.000000 scpkit-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:56:08.132303 scpkit-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-19 18:55:59.000000 scpkit-0.3.0/tests/test.py
```

### Comparing `scpkit-0.2.0/LICENSE` & `scpkit-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scpkit-0.2.0/PKG-INFO` & `scpkit-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scpkit
-Version: 0.2.0
+Version: 0.3.0
 Summary: This package helps consolidate service control policies in AWS
 Home-page: https://www.aquia.us
 Author: Aquia
 Author-email: info@aquia.us
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/aquia-inc/scpkit/issues
 Project-URL: Source, https://github.com/aquia-inc/scpkit
```

### Comparing `scpkit-0.2.0/README.md` & `scpkit-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `scpkit-0.2.0/scpkit/main.py` & `scpkit-0.3.0/scpkit/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """SCPkit
 Usage:
-    main.py (validate | merge) [--sourcefiles sourcefiles] [--profile profile] [ --outdir outdir] [--validate-after-merge] [--readable]
+    main.py (validate | merge) [--sourcefiles sourcefiles] [--profile profile] [ --outdir outdir] [--validate-after-merge] [--readable] [--console]
 
 Options:
     -h --help                   Show this screen.
     --version                   Show version.
     --sourcefiles sourcefiles   Directory path to SCP files in json format or a single SCP file
     --outdir outdir             Directory to write new SCP files [Default: ./]
     --profile profile           AWS profile name
     --validate-after-merge      Validate the policies after merging them
     --readable                  Leave indentation and some whitespace to make the SCPs readable
+    --console                   Adds Log to console
 """
 from docopt import docopt
 from .src.validate import validate_policies
 from .src.merge import scp_merge
 from .src.util import get_files_in_dir
 
 def main():
@@ -23,12 +24,12 @@
 
     arguments['scps'] = get_files_in_dir(arguments["sourcefiles"])
 
     if arguments.get("merge"):
         scp_merge(**arguments)
 
     if arguments.get("validate"):
-        validate_policies(arguments['scps'], arguments['profile'], arguments['outdir'])
+        validate_policies(arguments['scps'], arguments['profile'], arguments['outdir'], arguments['console'])
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `scpkit-0.2.0/scpkit/src/merge.py` & `scpkit-0.3.0/scpkit/src/merge.py`

 * *Files identical despite different names*

### Comparing `scpkit-0.2.0/scpkit/src/model.py` & `scpkit-0.3.0/scpkit/src/model.py`

 * *Files identical despite different names*

### Comparing `scpkit-0.2.0/scpkit/src/util.py` & `scpkit-0.3.0/scpkit/src/util.py`

 * *Files identical despite different names*

### Comparing `scpkit-0.2.0/scpkit/src/validate.py` & `scpkit-0.3.0/scpkit/src/validate.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,23 +24,33 @@
 
     Returns:
         [object]: client session for specific aws service (eg. accessanalyzer)
     """
     return session.client(service)
 
 
-def validate_policies(scps, profile, outdir=None):
+def validate_policies(scps, profile, outdir=None, console=False):
     """Validates SCPs 
 
     Args:
         scps (list of objects): SCP objects  
         profile (object): AWS profile name
     """
     access_analyzer = create_client(create_session(profile), "accessanalyzer")
 
     for scp in scps:
+        if(console):
+            print(f"🧪 Validate SCP: {scp.name}")
         scp.validate(access_analyzer)
         if scp.findings:
+            if(console):
+                print(f"    🚨 Error(s) in {scp.name}:")
+                for finding in scp.findings:
+                    print(f"       {finding['issueCode']} - {finding['findingDetails']}")
             if outdir:
                 scp.write_findings_for_scp(outdir)
+                if(console):
+                    print("    ℹ️  More details check log file {outdir}/{scp.name}-findings.json")
             else:
                 print(scp.findings_json)
+                if(console):
+                    print(f"   ℹ️  More details check log file ./{scp.name}-findings.json")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scpkit-0.2.0/scpkit.egg-info/PKG-INFO` & `scpkit-0.3.0/scpkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scpkit
-Version: 0.2.0
+Version: 0.3.0
 Summary: This package helps consolidate service control policies in AWS
 Home-page: https://www.aquia.us
 Author: Aquia
 Author-email: info@aquia.us
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/aquia-inc/scpkit/issues
 Project-URL: Source, https://github.com/aquia-inc/scpkit
```

### Comparing `scpkit-0.2.0/setup.cfg` & `scpkit-0.3.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 project_urls = 
 	Bug Tracker = https://github.com/aquia-inc/scpkit/issues
 	Source = https://github.com/aquia-inc/scpkit
 description = This package helps consolidate service control policies in AWS
 license = Apache License 2.0
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 0.2.0
+version = 0.3.0
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = file: requirements.txt
```

### Comparing `scpkit-0.2.0/tests/test.py` & `scpkit-0.3.0/tests/test.py`

 * *Files identical despite different names*

