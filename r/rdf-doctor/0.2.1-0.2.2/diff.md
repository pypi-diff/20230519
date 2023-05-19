# Comparing `tmp/rdf_doctor-0.2.1-py3-none-any.whl.zip` & `tmp/rdf_doctor-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,28 +1,16 @@
-Zip file size: 35064 bytes, number of entries: 26
+Zip file size: 28305 bytes, number of entries: 14
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-20 08:28 doctor/__init__.py
--rw-r--r--  2.0 unx      619 b- defN 23-May-18 06:15 doctor/consts.py
+-rw-r--r--  2.0 unx      619 b- defN 23-May-19 04:24 doctor/consts.py
 -rw-r--r--  2.0 unx    22796 b- defN 23-May-18 06:06 doctor/doctor.py
 -rw-r--r--  2.0 unx    20305 b- defN 23-Apr-28 02:45 doctor/reference/correct-prefixes.tsv
 -rw-r--r--  2.0 unx    36944 b- defN 23-Apr-20 08:28 doctor/reference/rdf-config-prefixes.tsv
 -rw-r--r--  2.0 unx    21257 b- defN 23-Apr-20 08:28 doctor/reference/rdf-config-prefixes.yaml
 -rw-r--r--  2.0 unx      596 b- defN 23-Apr-28 06:16 doctor/reference/refine-classes.tsv
 -rw-r--r--  2.0 unx      678 b- defN 23-May-16 00:01 doctor/reference/refine-prefixes.tsv
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-20 08:28 tests/__init__.py
--rw-r--r--  2.0 unx     1122 b- defN 23-Apr-20 08:28 tests/test_fingerprint.py
--rw-r--r--  2.0 unx     2264 b- defN 23-Apr-20 08:28 tests/test_get_class_comparison_result.py
--rw-r--r--  2.0 unx     1511 b- defN 23-May-17 05:47 tests/test_get_command_line_args.py
--rw-r--r--  2.0 unx     1606 b- defN 23-Apr-20 08:28 tests/test_get_fingerprint_comparison_result.py
--rw-r--r--  2.0 unx     1224 b- defN 23-Apr-20 08:28 tests/test_get_input_classes.py
--rw-r--r--  2.0 unx      867 b- defN 23-Apr-20 08:28 tests/test_get_input_format.py
--rw-r--r--  2.0 unx     1717 b- defN 23-Apr-27 07:05 tests/test_get_input_prefixes.py
--rw-r--r--  2.0 unx      880 b- defN 23-Apr-26 07:37 tests/test_get_prefix_comparison_result.py
--rw-r--r--  2.0 unx     1178 b- defN 23-Apr-26 07:37 tests/test_get_prefix_reuse_percentage.py
--rw-r--r--  2.0 unx     3423 b- defN 23-Apr-28 07:39 tests/test_get_suggested_qname.py
--rw-r--r--  2.0 unx    10048 b- defN 23-May-16 00:26 tests/test_validate_command_line_args.py
--rw-r--r--  2.0 unx     1061 b- defN 23-May-18 06:27 rdf_doctor-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     6136 b- defN 23-May-18 06:27 rdf_doctor-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-18 06:27 rdf_doctor-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-May-18 06:27 rdf_doctor-0.2.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-May-18 06:27 rdf_doctor-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2286 b- defN 23-May-18 06:27 rdf_doctor-0.2.1.dist-info/RECORD
-26 files, 138675 bytes uncompressed, 31326 bytes compressed:  77.4%
+-rw-r--r--  2.0 unx     1061 b- defN 23-May-19 04:30 rdf_doctor-0.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6257 b- defN 23-May-19 04:30 rdf_doctor-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-19 04:30 rdf_doctor-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 23-May-19 04:30 rdf_doctor-0.2.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-May-19 04:30 rdf_doctor-0.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1191 b- defN 23-May-19 04:30 rdf_doctor-0.2.2.dist-info/RECORD
+14 files, 111855 bytes uncompressed, 26307 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -18,62 +18,26 @@
 
 Filename: doctor/reference/refine-classes.tsv
 Comment: 
 
 Filename: doctor/reference/refine-prefixes.tsv
 Comment: 
 
-Filename: tests/__init__.py
+Filename: rdf_doctor-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: tests/test_fingerprint.py
+Filename: rdf_doctor-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: tests/test_get_class_comparison_result.py
+Filename: rdf_doctor-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: tests/test_get_command_line_args.py
+Filename: rdf_doctor-0.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: tests/test_get_fingerprint_comparison_result.py
+Filename: rdf_doctor-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: tests/test_get_input_classes.py
-Comment: 
-
-Filename: tests/test_get_input_format.py
-Comment: 
-
-Filename: tests/test_get_input_prefixes.py
-Comment: 
-
-Filename: tests/test_get_prefix_comparison_result.py
-Comment: 
-
-Filename: tests/test_get_prefix_reuse_percentage.py
-Comment: 
-
-Filename: tests/test_get_suggested_qname.py
-Comment: 
-
-Filename: tests/test_validate_command_line_args.py
-Comment: 
-
-Filename: rdf_doctor-0.2.1.dist-info/LICENSE
-Comment: 
-
-Filename: rdf_doctor-0.2.1.dist-info/METADATA
-Comment: 
-
-Filename: rdf_doctor-0.2.1.dist-info/WHEEL
-Comment: 
-
-Filename: rdf_doctor-0.2.1.dist-info/entry_points.txt
-Comment: 
-
-Filename: rdf_doctor-0.2.1.dist-info/top_level.txt
-Comment: 
-
-Filename: rdf_doctor-0.2.1.dist-info/RECORD
+Filename: rdf_doctor-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doctor/consts.py

```diff
@@ -1,8 +1,8 @@
-VERSION = "0.2.1"
+VERSION = "0.2.2"
 
 # Report export format
 REPORT_FORMAT_SHEX = "shex"
 REPORT_FORMAT_MD = "md"               # same as markdown
 REPORT_FORMAT_MARKDOWN = "markdown"   # same as md
 
 # Target classes
```

## Comparing `rdf_doctor-0.2.1.dist-info/LICENSE` & `rdf_doctor-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rdf_doctor-0.2.1.dist-info/METADATA` & `rdf_doctor-0.2.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,55 +1,53 @@
 Metadata-Version: 2.1
 Name: rdf-doctor
-Version: 0.2.1
+Version: 0.2.2
 Summary: Validate RDF data, report problems, and support creation of more accurate data
 Home-page: https://github.com/dbcls/rdf-doctor
 Author: DBCLS
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Flask (==2.3.2)
+Requires-Dist: Flask (>=2.2.5)
 Requires-Dist: Flask-Cors (==3.0.9)
 Requires-Dist: rdflib (==6.3.1)
 Requires-Dist: SPARQLWrapper (==2.0.0)
 Requires-Dist: wlighter (==1.0.1)
 Requires-Dist: shexer (==2.2.0)
 Requires-Dist: unidecode (>=1.3.6)
 
 # rdf-doctor
+[![Pyversions](https://img.shields.io/pypi/pyversions/rdf-doctor.svg)](https://pypi.python.org/pypi/rdf-doctor)
 
 ## Motivation
-
 DBCLS has conducted to convert various life science databases to RDF and support it. This development will enable us to provide a high-quality dataset that better links existing RDF datasets stored in the RDF portal site and newly developed RDF.
 
 ## Requirements
 ```
 (1) Operating system
 Linux (CentOS 7 or later or Ubuntu 20.04 or later), macOS 12 Monterey or later
 
 (2) Software development language
 Python
 
 (3) Operating system environment
 Main memory: 32 GB or less
 Hard disk: 2TB or less
 ```
-## Install
 
+## Install
 ```
 pip install rdf-doctor
 ```
 
-
 ## Command Line Interface
-
 ```
 $ rdf-doctor --help
 usage: rdf-doctor -i RDF-FILE [Options]
 
 Home page: https://github.com/dbcls/rdf-doctor
 
 optional arguments:
@@ -64,18 +62,17 @@
   -c URL [URL ...], --classes URL [URL ...]
                         set the target classes to be inspected to one of: all (defalut) or URL1, URL2,...
 ```
 
 ## See Also
 - [1] https://github.com/DaniFdezAlvarez/shexer
 - [2] http://shex.io/shex-primer/#combined-constraints
-- [3] https://docs.openrefine.org/next/manual/cellediting#fingerprinting
+- [3] https://openrefine.org/docs/technical-reference/clustering-in-depth#fingerprint
 
 ## Example
-
 ```
 $ rdf-doctor -i example.nt
 PREFIX : <http://weso.es/shapes/>
 
 :Person  [<http://purl.obolibrary.org/obo/>~]  AND   # 5 instances
 {
    <http://www.w3.org/1999/02/22-rdf-syntax-ns#type>  [<http://xmlns.com/foaf/0.1/Person>]  ;          # 100.0 % (5 instances).
```

