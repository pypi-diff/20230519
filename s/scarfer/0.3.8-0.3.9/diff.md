# Comparing `tmp/scarfer-0.3.8.tar.gz` & `tmp/scarfer-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scarfer-0.3.8.tar", last modified: Sun May  7 14:35:05 2023, max compression
+gzip compressed data, was "scarfer-0.3.9.tar", last modified: Fri May 19 13:58:16 2023, max compression
```

## Comparing `scarfer-0.3.8.tar` & `scarfer-0.3.9.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 hesa      (1000) hesa      (1000)        0 2023-05-07 14:35:05.296931 scarfer-0.3.8/
--rw-r--r--   0 hesa      (1000) hesa      (1000)      268 2023-04-26 16:41:20.000000 scarfer-0.3.8/DESCRIPTION.md
-drwxr-xr-x   0 hesa      (1000) hesa      (1000)        0 2023-05-07 14:35:05.292931 scarfer-0.3.8/LICENSES/
--rw-r--r--   0 hesa      (1000) hesa      (1000)    34670 2023-04-26 16:41:20.000000 scarfer-0.3.8/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0 hesa      (1000) hesa      (1000)      111 2023-04-26 16:41:20.000000 scarfer-0.3.8/MANIFEST.in
--rw-r--r--   0 hesa      (1000) hesa      (1000)     1126 2023-05-07 14:35:05.296931 scarfer-0.3.8/PKG-INFO
--rw-r--r--   0 hesa      (1000) hesa      (1000)     3007 2023-05-01 14:57:15.000000 scarfer-0.3.8/README.md
--rw-r--r--   0 hesa      (1000) hesa      (1000)        1 2023-04-26 16:41:20.000000 scarfer-0.3.8/requirements-dev.txt
--rw-r--r--   0 hesa      (1000) hesa      (1000)       37 2023-04-26 16:41:20.000000 scarfer-0.3.8/requirements.txt
-drwxr-xr-x   0 hesa      (1000) hesa      (1000)        0 2023-05-07 14:35:05.292931 scarfer-0.3.8/scarfer/
--rwxr-xr-x   0 hesa      (1000) hesa      (1000)    13731 2023-05-07 14:34:56.000000 scarfer-0.3.8/scarfer/__main__.py
--rw-r--r--   0 hesa      (1000) hesa      (1000)     6761 2023-04-26 16:41:20.000000 scarfer-0.3.8/scarfer/analyzer.py
--rw-r--r--   0 hesa      (1000) hesa      (1000)      237 2023-05-07 14:34:56.000000 scarfer-0.3.8/scarfer/config.py
--rw-r--r--   0 hesa      (1000) hesa      (1000)      612 2023-04-26 16:41:20.000000 scarfer-0.3.8/scarfer/filter_utils.py
-drwxr-xr-x   0 hesa      (1000) hesa      (1000)        0 2023-05-07 14:35:05.292931 scarfer-0.3.8/scarfer/format/
--rw-r--r--   0 hesa      (1000) hesa      (1000)        0 2023-04-26 16:41:20.000000 scarfer-0.3.8/scarfer/format/__init__.py
--rw-r--r--   0 hesa      (1000) hesa      (1000)      672 2023-04-26 16:41:20.000000 scarfer-0.3.8/scarfer/format/factory.py
--rw-r--r--   0 hesa      (1000) hesa      (1000)     1122 2023-04-26 16:41:20.000000 scarfer-0.3.8/scarfer/format/format_json.py
--rw-r--r--   0 hesa      (1000) hesa      (1000)      968 2023-04-26 16:41:20.000000 scarfer-0.3.8/scarfer/format/format_markdown.py
--rw-r--r--   0 hesa      (1000) hesa      (1000)     2572 2023-04-26 16:41:20.000000 scarfer-0.3.8/scarfer/format/format_text.py
--rw-r--r--   0 hesa      (1000) hesa      (1000)      190 2023-04-26 16:41:20.000000 scarfer-0.3.8/scarfer/format/format_yaml.py
--rw-r--r--   0 hesa      (1000) hesa      (1000)     1141 2023-04-26 16:41:20.000000 scarfer-0.3.8/scarfer/format/interface.py
--rw-r--r--   0 hesa      (1000) hesa      (1000)     4438 2023-05-01 14:54:06.000000 scarfer-0.3.8/scarfer/scan_interface.py
-drwxr-xr-x   0 hesa      (1000) hesa      (1000)        0 2023-05-07 14:35:05.296931 scarfer-0.3.8/scarfer/var/
--rw-r--r--   0 hesa      (1000) hesa      (1000)     2927 2023-05-07 14:34:56.000000 scarfer-0.3.8/scarfer/var/default-exclude-files.txt
--rw-r--r--   0 hesa      (1000) hesa      (1000)     3113 2023-04-26 16:41:20.000000 scarfer-0.3.8/scarfer/var/normalized-scan.json
-drwxr-xr-x   0 hesa      (1000) hesa      (1000)        0 2023-05-07 14:35:05.292931 scarfer-0.3.8/scarfer.egg-info/
--rw-r--r--   0 hesa      (1000) hesa      (1000)     1126 2023-05-07 14:35:05.000000 scarfer-0.3.8/scarfer.egg-info/PKG-INFO
--rw-r--r--   0 hesa      (1000) hesa      (1000)      685 2023-05-07 14:35:05.000000 scarfer-0.3.8/scarfer.egg-info/SOURCES.txt
--rw-r--r--   0 hesa      (1000) hesa      (1000)        1 2023-05-07 14:35:05.000000 scarfer-0.3.8/scarfer.egg-info/dependency_links.txt
--rw-r--r--   0 hesa      (1000) hesa      (1000)       51 2023-05-07 14:35:05.000000 scarfer-0.3.8/scarfer.egg-info/entry_points.txt
--rw-r--r--   0 hesa      (1000) hesa      (1000)       44 2023-05-07 14:35:05.000000 scarfer-0.3.8/scarfer.egg-info/requires.txt
--rw-r--r--   0 hesa      (1000) hesa      (1000)       23 2023-05-07 14:35:05.000000 scarfer-0.3.8/scarfer.egg-info/top_level.txt
--rw-r--r--   0 hesa      (1000) hesa      (1000)       38 2023-05-07 14:35:05.296931 scarfer-0.3.8/setup.cfg
--rw-r--r--   0 hesa      (1000) hesa      (1000)     1937 2023-04-26 16:41:20.000000 scarfer-0.3.8/setup.py
+drwxrwxr-x   0 hesa      (1001) hesa      (1001)        0 2023-05-19 13:58:16.946464 scarfer-0.3.9/
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)      268 2022-12-20 17:51:14.000000 scarfer-0.3.9/DESCRIPTION.md
+drwxrwxr-x   0 hesa      (1001) hesa      (1001)        0 2023-05-19 13:58:16.946464 scarfer-0.3.9/LICENSES/
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)    34670 2022-12-20 17:51:14.000000 scarfer-0.3.9/LICENSES/GPL-3.0-or-later.txt
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)      111 2023-05-06 15:02:55.000000 scarfer-0.3.9/MANIFEST.in
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)     1106 2023-05-19 13:58:16.946464 scarfer-0.3.9/PKG-INFO
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)     3007 2023-05-06 15:02:55.000000 scarfer-0.3.9/README.md
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)        1 2022-12-20 17:51:14.000000 scarfer-0.3.9/requirements-dev.txt
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)       37 2023-05-06 15:02:56.000000 scarfer-0.3.9/requirements.txt
+drwxrwxr-x   0 hesa      (1001) hesa      (1001)        0 2023-05-19 13:58:16.946464 scarfer-0.3.9/scarfer/
+-rwxrwxr-x   0 hesa      (1001) hesa      (1001)    13733 2023-05-19 13:46:23.000000 scarfer-0.3.9/scarfer/__main__.py
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)     6921 2023-05-19 13:40:07.000000 scarfer-0.3.9/scarfer/analyzer.py
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)      237 2023-05-19 13:48:54.000000 scarfer-0.3.9/scarfer/config.py
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)      612 2023-05-06 15:02:56.000000 scarfer-0.3.9/scarfer/filter_utils.py
+drwxrwxr-x   0 hesa      (1001) hesa      (1001)        0 2023-05-19 13:58:16.946464 scarfer-0.3.9/scarfer/format/
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)        0 2022-12-20 17:51:14.000000 scarfer-0.3.9/scarfer/format/__init__.py
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)      672 2023-05-06 15:02:56.000000 scarfer-0.3.9/scarfer/format/factory.py
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)     1122 2023-05-06 15:02:56.000000 scarfer-0.3.9/scarfer/format/format_json.py
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)      968 2023-05-06 15:02:56.000000 scarfer-0.3.9/scarfer/format/format_markdown.py
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)     2642 2023-05-19 13:40:07.000000 scarfer-0.3.9/scarfer/format/format_text.py
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)      155 2023-05-19 13:40:07.000000 scarfer-0.3.9/scarfer/format/format_utils.py
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)      190 2022-12-20 17:51:14.000000 scarfer-0.3.9/scarfer/format/format_yaml.py
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)     1141 2023-05-06 15:02:56.000000 scarfer-0.3.9/scarfer/format/interface.py
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)     4438 2023-05-06 15:02:56.000000 scarfer-0.3.9/scarfer/scan_interface.py
+drwxrwxr-x   0 hesa      (1001) hesa      (1001)        0 2023-05-19 13:58:16.946464 scarfer-0.3.9/scarfer/var/
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)     2968 2023-05-19 13:40:07.000000 scarfer-0.3.9/scarfer/var/default-exclude-files.txt
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)     3113 2023-05-06 15:02:56.000000 scarfer-0.3.9/scarfer/var/normalized-scan.json
+drwxrwxr-x   0 hesa      (1001) hesa      (1001)        0 2023-05-19 13:58:16.946464 scarfer-0.3.9/scarfer.egg-info/
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)     1106 2023-05-19 13:58:16.000000 scarfer-0.3.9/scarfer.egg-info/PKG-INFO
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)      716 2023-05-19 13:58:16.000000 scarfer-0.3.9/scarfer.egg-info/SOURCES.txt
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)        1 2023-05-19 13:58:16.000000 scarfer-0.3.9/scarfer.egg-info/dependency_links.txt
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)       50 2023-05-19 13:58:16.000000 scarfer-0.3.9/scarfer.egg-info/entry_points.txt
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)       44 2023-05-19 13:58:16.000000 scarfer-0.3.9/scarfer.egg-info/requires.txt
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)       23 2023-05-19 13:58:16.000000 scarfer-0.3.9/scarfer.egg-info/top_level.txt
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)       38 2023-05-19 13:58:16.946464 scarfer-0.3.9/setup.cfg
+-rw-rw-r--   0 hesa      (1001) hesa      (1001)     1937 2023-05-06 15:02:56.000000 scarfer-0.3.9/setup.py
```

### Comparing `scarfer-0.3.8/LICENSES/GPL-3.0-or-later.txt` & `scarfer-0.3.9/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `scarfer-0.3.8/PKG-INFO` & `scarfer-0.3.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 Metadata-Version: 2.1
 Name: scarfer
-Version: 0.3.8
-Summary: UNKNOWN
+Version: 0.3.9
 Home-page: https://github.com/hesa/scarfer
 Author: Henrik Sanklef
 Author-email: hesa@sandklef.com
-License: UNKNOWN
-Description: Scarfer outputs compliance related information from a scan report.
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
@@ -22,7 +18,10 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSES/GPL-3.0-or-later.txt
+
+Scarfer outputs compliance related information from a scan report.
```

### Comparing `scarfer-0.3.8/README.md` & `scarfer-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `scarfer-0.3.8/scarfer/__main__.py` & `scarfer-0.3.9/scarfer/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,15 +354,15 @@
             formatted_data_list.append(formatter.format_copyright_summary(filtered_files, settings))
         if args['license_summary']:
             formatted_data_list.append(formatter.format_license_summary(filtered_files, settings))
         formatted_data = "\n".join(formatted_data_list)
     elif args['cumulative']:
         formatted_data = formatter.format_cumulative(filtered_files, settings)
     elif args['output_fixes']:
-        formatted_data = formatter.format_fixes(reader.fixes(), settings)
+        formatted_data = formatter.format_fixes(analyzer.fixes(), settings)
     else:
         formatted_data = formatter.format(filtered_files, settings)
 
     # Print the data
     print(formatted_data)
 
 if __name__ == '__main__':
```

### Comparing `scarfer-0.3.8/scarfer/analyzer.py` & `scarfer-0.3.9/scarfer/analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,21 @@
         self.schema = None
 
     def _apply_filter_file(self, filt, f):
         if filt.type == ScanReportFilterType.FILE:
             ret = re.search(filt.expr, f['path'])
             return ret != None
         elif filt.type == ScanReportFilterType.LICENSE:
-            for l in f['license']['expressions']:
-                if re.search(filt.expr,l):
-                    return True
+            if len(f['license']['expressions']) == 0:
+                if filt.expr == "missing":
+                    return  True
+            else:
+                for l in f['license']['expressions']:
+                    if re.search(filt.expr,l):
+                        return True
             return False
         else:
             raise(ScanReportException("Unsupported filter type. This is weird."))
             
 
     def _apply_filters_file(self, f, filters, filter_on_files):
```

### Comparing `scarfer-0.3.8/scarfer/filter_utils.py` & `scarfer-0.3.9/scarfer/filter_utils.py`

 * *Files identical despite different names*

### Comparing `scarfer-0.3.8/scarfer/format/factory.py` & `scarfer-0.3.9/scarfer/format/factory.py`

 * *Files identical despite different names*

### Comparing `scarfer-0.3.8/scarfer/format/format_json.py` & `scarfer-0.3.9/scarfer/format/format_json.py`

 * *Files identical despite different names*

### Comparing `scarfer-0.3.8/scarfer/format/format_markdown.py` & `scarfer-0.3.9/scarfer/format/format_markdown.py`

 * *Files identical despite different names*

### Comparing `scarfer-0.3.8/scarfer/format/format_text.py` & `scarfer-0.3.9/scarfer/format/format_text.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from scarfer.format.interface import FormatInterface
+from scarfer.format.format_utils import summarize_license
 import os
 
 class TextFormatter(FormatInterface):
 
     def _format_file(self, f, settings):
         ret = []
         
@@ -48,21 +49,23 @@
         return f'{os.linesep.join(excluded)}{os.linesep}{os.linesep.join(missing)}'
 
     def format_cumulative(self, report, settings={}):
         ret = []
         cumulative = report['cumulative']
         ret.append(f"Cumulative license: {cumulative['license']}")
         return "\n".join(ret)
-        
+
+    
+    
     def format_license_summary(self, report, settings={}):
         license_summary = set()
         for f in report['files']:
             for l in f['license']['expressions']:
                 license_summary.add(l)
-        return f'License:\n { " AND ".join(license_summary)}\n'
+        return f'License:\n {summarize_license(list(license_summary))}\n'
 
     def format_copyright_summary(self, report, settings={}):
         copyright_summary = set()
         for f in report['files']:
             for l in f['copyrights']:
                 copyright_summary.add(l)
         c_list = list(copyright_summary)
```

### Comparing `scarfer-0.3.8/scarfer/format/interface.py` & `scarfer-0.3.9/scarfer/format/interface.py`

 * *Files identical despite different names*

### Comparing `scarfer-0.3.8/scarfer/scan_interface.py` & `scarfer-0.3.9/scarfer/scan_interface.py`

 * *Files identical despite different names*

### Comparing `scarfer-0.3.8/scarfer/var/default-exclude-files.txt` & `scarfer-0.3.9/scarfer/var/default-exclude-files.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 config\.status
 autom4te\.cache/
 \.timestamp
 ~
 \.deps/
 ChangeLog[\.\-\w]*
 Changelog[\.\-\w]*
+CHANGELOG[\.\-\w]*
 README[\.\-\w]*
 ABOUT[\.\-\w]*
 FAQ[\.\-\w]*
 TODO[\.\-\w]*
-MANIFEST
+MANIFEST[\.\-\w]*
 BUILD[\.\-\w]*
 USAGE[\.\-\w]*
 OWNERS[\.\-\w]*
 BUILD[\.\-\w]*
 WORKSPACE[\.\-\w]*
 COPYING.[\.\-\w]*
 INSTALL
@@ -35,14 +36,15 @@
 CODEOWNER.[\.\-\w]*
 
 # test code
 tests/
 test/
 __test__/
 __tests__/
+\.coveragerc
 
 # documentation
 doc/
 docs/
 
 # example
 /examples/
```

### Comparing `scarfer-0.3.8/scarfer/var/normalized-scan.json` & `scarfer-0.3.9/scarfer/var/normalized-scan.json`

 * *Files identical despite different names*

### Comparing `scarfer-0.3.8/scarfer.egg-info/PKG-INFO` & `scarfer-0.3.9/scarfer.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 Metadata-Version: 2.1
 Name: scarfer
-Version: 0.3.8
-Summary: UNKNOWN
+Version: 0.3.9
 Home-page: https://github.com/hesa/scarfer
 Author: Henrik Sanklef
 Author-email: hesa@sandklef.com
-License: UNKNOWN
-Description: Scarfer outputs compliance related information from a scan report.
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
@@ -22,7 +18,10 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSES/GPL-3.0-or-later.txt
+
+Scarfer outputs compliance related information from a scan report.
```

### Comparing `scarfer-0.3.8/scarfer.egg-info/SOURCES.txt` & `scarfer-0.3.9/scarfer.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -17,11 +17,12 @@
 scarfer.egg-info/requires.txt
 scarfer.egg-info/top_level.txt
 scarfer/format/__init__.py
 scarfer/format/factory.py
 scarfer/format/format_json.py
 scarfer/format/format_markdown.py
 scarfer/format/format_text.py
+scarfer/format/format_utils.py
 scarfer/format/format_yaml.py
 scarfer/format/interface.py
 scarfer/var/default-exclude-files.txt
 scarfer/var/normalized-scan.json
```

### Comparing `scarfer-0.3.8/setup.py` & `scarfer-0.3.9/setup.py`

 * *Files identical despite different names*

