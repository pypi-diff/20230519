# Comparing `tmp/dwiqc-0.1.4-py2.py3-none-any.whl.zip` & `tmp/dwiqc-0.1.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 21853 bytes, number of entries: 20
+Zip file size: 21780 bytes, number of entries: 20
 -rw-r--r--  2.0 unx      225 b- defN 23-May-19 13:23 dwiqc/__init__.py
--rw-r--r--  2.0 unx      247 b- defN 23-May-19 13:23 dwiqc/__version__.py
+-rw-r--r--  2.0 unx      247 b- defN 23-May-19 14:20 dwiqc/__version__.py
 -rw-r--r--  2.0 unx       62 b- defN 23-May-19 13:24 dwiqc/cli/__init__.py
 -rw-r--r--  2.0 unx     6651 b- defN 23-May-15 18:24 dwiqc/cli/get.py
 -rw-r--r--  2.0 unx     5273 b- defN 23-May-19 13:31 dwiqc/cli/process.py
 -rw-r--r--  2.0 unx      160 b- defN 23-May-15 18:24 dwiqc/config/__init__.py
 -rw-r--r--  2.0 unx      274 b- defN 23-May-15 18:24 dwiqc/config/dwiqc.yaml
 -rw-r--r--  2.0 unx       98 b- defN 23-May-19 13:27 dwiqc/state/__init__.py
 -rw-r--r--  2.0 unx     1892 b- defN 23-May-19 13:26 dwiqc/tasks/__init__.py
--rw-r--r--  2.0 unx     9512 b- defN 23-May-18 16:50 dwiqc/tasks/prequal.py
--rw-r--r--  2.0 unx     3765 b- defN 23-May-18 15:54 dwiqc/tasks/prequal_EQ.py
--rw-r--r--  2.0 unx     6247 b- defN 23-May-18 16:32 dwiqc/tasks/qsiprep.py
--rw-r--r--  2.0 unx     3836 b- defN 23-May-16 18:34 dwiqc/tasks/qsiprep_EQ.py
+-rw-r--r--  2.0 unx     9470 b- defN 23-May-19 13:47 dwiqc/tasks/prequal.py
+-rw-r--r--  2.0 unx     3697 b- defN 23-May-19 13:51 dwiqc/tasks/prequal_EQ.py
+-rw-r--r--  2.0 unx     6193 b- defN 23-May-19 13:48 dwiqc/tasks/qsiprep.py
+-rw-r--r--  2.0 unx     3782 b- defN 23-May-19 13:49 dwiqc/tasks/qsiprep_EQ.py
 -rw-r--r--  2.0 unx    12888 b- defN 23-May-19 13:31 dwiqc/xnat/__init__.py
--rwxr-xr-x  2.0 unx     4039 b- defN 23-May-19 13:33 dwiqc-0.1.4.data/scripts/dwiqc.py
--rw-r--r--  2.0 unx     1541 b- defN 23-May-19 13:33 dwiqc-0.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx      293 b- defN 23-May-19 13:33 dwiqc-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-19 13:33 dwiqc-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-May-19 13:33 dwiqc-0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1559 b- defN 23-May-19 13:33 dwiqc-0.1.4.dist-info/RECORD
-20 files, 58678 bytes uncompressed, 19341 bytes compressed:  67.0%
+-rwxr-xr-x  2.0 unx     4016 b- defN 23-May-19 14:21 dwiqc-0.1.5.data/scripts/dwiQC.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-May-19 14:21 dwiqc-0.1.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx      388 b- defN 23-May-19 14:21 dwiqc-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-19 14:21 dwiqc-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-May-19 14:21 dwiqc-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1559 b- defN 23-May-19 14:21 dwiqc-0.1.5.dist-info/RECORD
+20 files, 58532 bytes uncompressed, 19268 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -36,26 +36,26 @@
 
 Filename: dwiqc/tasks/qsiprep_EQ.py
 Comment: 
 
 Filename: dwiqc/xnat/__init__.py
 Comment: 
 
-Filename: dwiqc-0.1.4.data/scripts/dwiqc.py
+Filename: dwiqc-0.1.5.data/scripts/dwiQC.py
 Comment: 
 
-Filename: dwiqc-0.1.4.dist-info/LICENSE
+Filename: dwiqc-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: dwiqc-0.1.4.dist-info/METADATA
+Filename: dwiqc-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: dwiqc-0.1.4.dist-info/WHEEL
+Filename: dwiqc-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: dwiqc-0.1.4.dist-info/top_level.txt
+Filename: dwiqc-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: dwiqc-0.1.4.dist-info/RECORD
+Filename: dwiqc-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dwiqc/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'dwiqc'
 __description__ = 'Quality Assurance Pipeline for Diffusion MR Data'
 __url__ = 'https://github.com/harvard-nrg/dwiqc'
-__version__ = '0.1.4'
+__version__ = '0.1.5'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## dwiqc/tasks/prequal.py

```diff
@@ -3,26 +3,26 @@
 
 import subprocess
 import os
 import logging
 from bids import BIDSLayout
 import sys
 import json
-sys.path.insert(0, '/n/home_fasse/dasay/dwiqc/dwiqc/tasks')
-import setup# as tasks
+import dwiqc
+import dwiqc.tasks as tasks
 import shutil
 from executors.models import Job
 
 
 logger = logging.getLogger(__name__)
 
 
 # pull in some parameters from the BaseTask class in the __init__.py directory
 
-class Task(setup.BaseTask):
+class Task(tasks.BaseTask):
 	def __init__(self, sub, ses, run, bids, outdir, tempdir=None, pipenv=None):
 		self._sub = sub
 		self._ses = ses
 		self._run = run
 		self._bids = bids
 		self._layout = BIDSLayout(bids)
 		super().__init__(outdir, tempdir, pipenv)
```

## dwiqc/tasks/prequal_EQ.py

```diff
@@ -1,17 +1,15 @@
 
-import PyPDF2
 import shutil
 import os
 import time
 import sys
 sys.path.insert(0, os.path.join(os.environ['MODULESHOME'], "init"))
 from env_modules_python import module
-sys.path.insert(0, '/n/home_fasse/dasay/dwiqc/dwiqc/tasks')
-import setup as tasks
+import dwiqc.tasks as tasks
 import logging
 import subprocess
 import json
 from executors.models import Job
 
 
 old_out = sys.stdout
```

## dwiqc/tasks/qsiprep.py

```diff
@@ -4,16 +4,15 @@
 import subprocess
 import os
 import logging
 from bids import BIDSLayout
 import sys
 import json
 import nibabel as nib
-sys.path.insert(0, '/n/home_fasse/dasay/dwiqc/dwiqc/tasks')
-import setup as tasks
+import dwiqc.tasks as tasks
 sys.path.insert(0, os.path.join(os.environ['MODULESHOME'], "init"))
 from env_modules_python import module
 import shutil
 from executors.models import Job
 
 
 module('load', 'cuda/9.1.85-fasrc01')
```

## dwiqc/tasks/qsiprep_EQ.py

```diff
@@ -1,16 +1,15 @@
 
 
 import shutil
 import os
 import sys
 sys.path.insert(0, os.path.join(os.environ['MODULESHOME'], "init"))
 from env_modules_python import module
-sys.path.insert(0, '/n/home_fasse/dasay/dwiqc/dwiqc/tasks')
-import setup as tasks
+import dwiqc.tasks as tasks
 import logging
 import subprocess
 import json
 from executors.models import Job
 
 old_out = sys.stdout
```

## Comparing `dwiqc-0.1.4.data/scripts/dwiqc.py` & `dwiqc-0.1.5.data/scripts/dwiQC.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 
 
 
 import sys
 #sys.path.insert(0, '/n/home_fasse/dasay/dwiqc/dwiqc/cli')
 #sys.path.insert(0, '/n/home_fasse/dasay/dwiqc/dwiqc/config')
 import dwiqc
-from dwiqc import cli
+import dwiqc.cli as cli
 import logging
 import argparse as ap
-#import dwiqc.cli as cli
 #import dwiqc.config as config
 
 logger = logging.getLogger(__name__)
```

## Comparing `dwiqc-0.1.4.dist-info/LICENSE` & `dwiqc-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dwiqc-0.1.4.dist-info/RECORD` & `dwiqc-0.1.5.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 dwiqc/__init__.py,sha256=MZJhUZKhHHoZ2w_GeoFCITk1m_0ASdRw_ZaeDixFEPU,225
-dwiqc/__version__.py,sha256=OGe0WHcttQjUj2yaL-eo5DW7yfmgDCLPPsIbnak2COo,247
+dwiqc/__version__.py,sha256=YUc8aPHVKYcL0bNu62DvwwXlBDIy2t13wD1eV0X2_H0,247
 dwiqc/cli/__init__.py,sha256=zGIm7lrjh3wA191D-VjQBZNjSlspFUx148VwDNQGaTk,62
 dwiqc/cli/get.py,sha256=6ixaBdwEgY_GXh8L-_3QDY4MEsNqSJgXle_mxW99mlk,6651
 dwiqc/cli/process.py,sha256=X4eUXf-jRuOR_3cVQ0FfcDXmNPVQzILH35uGAtz9upE,5273
 dwiqc/config/__init__.py,sha256=k_w5JzoJN_7R7eI_sIJxHA4FQQHs0_KGf-6jsbG4Xs8,160
 dwiqc/config/dwiqc.yaml,sha256=x8gKMFZyChdzvNX3GthRe0eWvyKDDL5itXo0kLWVfd0,274
 dwiqc/state/__init__.py,sha256=NaRifw26bI3F1J9BqeLa-KLSzEPq2m_UNhMbXdmPdh4,98
 dwiqc/tasks/__init__.py,sha256=LnlN7iYjpqiBic2ihFrM-_h7m8FD_N7Beh7UIwKyGZ8,1892
-dwiqc/tasks/prequal.py,sha256=2yy5D0CeBpAOK0GHyvikxnr9cqzSE3zcApCsJ01zHnk,9512
-dwiqc/tasks/prequal_EQ.py,sha256=t5dgnC4Kbids-Ny3RK93wUJguBwjQ2fNZQuTZspq_Bk,3765
-dwiqc/tasks/qsiprep.py,sha256=LureiZSkkfCi87XTiNAn29AezzzzfFSsBBA3K8ntd5I,6247
-dwiqc/tasks/qsiprep_EQ.py,sha256=R0rGR2HBL5fLHN5L52i1N73B2yvYvmAlnv6XOxCGH3Q,3836
+dwiqc/tasks/prequal.py,sha256=w3vpr53Qrs75Ke6MZTw_jlfMZ6aHWoyFM6yWnC9Bqtg,9470
+dwiqc/tasks/prequal_EQ.py,sha256=LZOrTSqjVz2Zr7p0FUdkCUUFxjE3pjpi1TayZktbIek,3697
+dwiqc/tasks/qsiprep.py,sha256=RS8M07BO7ngImbUl1uaOSwPu1BF3NOB_-NhVcuP8vVc,6193
+dwiqc/tasks/qsiprep_EQ.py,sha256=JWildptHsuyJVj7ZYMFlWWYvsAIszJpWk1a0m05JM-Q,3782
 dwiqc/xnat/__init__.py,sha256=Hp0cHw98fDnOmG6sWJ1HI_DFck0h6fiV5VshQa_HTYI,12888
-dwiqc-0.1.4.data/scripts/dwiqc.py,sha256=wx1qmjd-a5vZgzs8UfEodbpVyXnQkD7OAD6xXFhOpbA,4039
-dwiqc-0.1.4.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-dwiqc-0.1.4.dist-info/METADATA,sha256=ghqKMBDKMLGhR7kMqP4Y-dOwTcR-SBmmBkDMEiKjAqI,293
-dwiqc-0.1.4.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-dwiqc-0.1.4.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
-dwiqc-0.1.4.dist-info/RECORD,,
+dwiqc-0.1.5.data/scripts/dwiQC.py,sha256=Z-Xt04-T9n4ZixWY_1O4gL3Oc7Em0ewwfLcktOlTsUw,4016
+dwiqc-0.1.5.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+dwiqc-0.1.5.dist-info/METADATA,sha256=lmSvO-R4V_yHqsa__-5G7fBxJPzloA8LboUhemhqEJ8,388
+dwiqc-0.1.5.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+dwiqc-0.1.5.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
+dwiqc-0.1.5.dist-info/RECORD,,
```

