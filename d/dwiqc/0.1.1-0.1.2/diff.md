# Comparing `tmp/dwiqc-0.1.1-py2.py3-none-any.whl.zip` & `tmp/dwiqc-0.1.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3503 bytes, number of entries: 6
--rwxr-xr-x  2.0 unx     4063 b- defN 23-May-18 18:01 dwiqc-0.1.1.data/scripts/dwiQC.py
--rw-r--r--  2.0 unx     1541 b- defN 23-May-18 18:01 dwiqc-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      337 b- defN 23-May-18 18:01 dwiqc-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-18 18:01 dwiqc-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-18 18:01 dwiqc-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      465 b- defN 23-May-18 18:01 dwiqc-0.1.1.dist-info/RECORD
-6 files, 6517 bytes uncompressed, 2661 bytes compressed:  59.2%
+Zip file size: 3492 bytes, number of entries: 6
+-rwxr-xr-x  2.0 unx     4028 b- defN 23-May-18 18:40 dwiqc-0.1.2.data/scripts/dwiQC.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-May-18 18:40 dwiqc-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      337 b- defN 23-May-18 18:40 dwiqc-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-18 18:40 dwiqc-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-18 18:40 dwiqc-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      465 b- defN 23-May-18 18:40 dwiqc-0.1.2.dist-info/RECORD
+6 files, 6482 bytes uncompressed, 2650 bytes compressed:  59.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: dwiqc-0.1.1.data/scripts/dwiQC.py
+Filename: dwiqc-0.1.2.data/scripts/dwiQC.py
 Comment: 
 
-Filename: dwiqc-0.1.1.dist-info/LICENSE
+Filename: dwiqc-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: dwiqc-0.1.1.dist-info/METADATA
+Filename: dwiqc-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: dwiqc-0.1.1.dist-info/WHEEL
+Filename: dwiqc-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: dwiqc-0.1.1.dist-info/top_level.txt
+Filename: dwiqc-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: dwiqc-0.1.1.dist-info/RECORD
+Filename: dwiqc-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `dwiqc-0.1.1.data/scripts/dwiQC.py` & `dwiqc-0.1.2.data/scripts/dwiQC.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #!python
 
 
 
 
 import sys
-sys.path.insert(0, '/n/home_fasse/dasay/dwiqc/dwiqc/cli')
-sys.path.insert(0, '/n/home_fasse/dasay/dwiqc/dwiqc/config')
-import get
-import process
+#sys.path.insert(0, '/n/home_fasse/dasay/dwiqc/dwiqc/cli')
+#sys.path.insert(0, '/n/home_fasse/dasay/dwiqc/dwiqc/config')
+import dwiqc.cli as cli
 import logging
 import argparse as ap
 #import dwiqc.cli as cli
 #import dwiqc.config as config
 
 logger = logging.getLogger(__name__)
 
@@ -41,15 +40,15 @@
         help='XNAT host')
     parser_get.add_argument('--xnat-user',
         help='XNAT username')
     parser_get.add_argument('--xnat-pass',
         help='XNAT password')
     parser_get.add_argument('--dry-run', action='store_true',
         help='Do not execute any jobs')
-    parser_get.set_defaults(func=get.do) #(func=cli.get.do)
+    parser_get.set_defaults(func=cli.get.do)
 
     # process mode
     parser_process = subparsers.add_parser('process', help='process -h')
     parser_process.add_argument('--partition', default='fasse_gpu',
         help='Job scheduler partition')
     parser_process.add_argument('--scheduler', default=None,
         help='Choose a specific job scheduler')
@@ -81,21 +80,21 @@
         help='XNAT username')
     parser_process.add_argument('--xnat-pass',
         help='XNAT password')
     parser_process.add_argument('--artifacts-dir',
         help='Location for generated assessors and resources')
     parser_process.add_argument('--xnat-upload', action='store_true',
         help='Upload results to XNAT over REST API')
-    parser_process.set_defaults(func=process.do) #(func=cli.process.do)
+    parser_process.set_defaults(func=cli.process.do)
 
     args = parser.parse_args()
 
 
     configure_logging(args.verbose)
-    #logger.info('Welcome to dwiQC version %s', dwiqc.version())
+    logger.info('Welcome to dwiQC version %s', dwiqc.version())
 
     # fire parser_*.set_defaults(func=<function>)
     args.func(args)
 
 def configure_logging(verbose):
     level = logging.INFO
     if verbose:
```

## Comparing `dwiqc-0.1.1.dist-info/LICENSE` & `dwiqc-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

