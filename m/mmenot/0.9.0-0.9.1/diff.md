# Comparing `tmp/mmenot-0.9.0-py3-none-any.whl.zip` & `tmp/mmenot-0.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,18 @@
-Zip file size: 23338 bytes, number of entries: 15
--rw-r--r--  2.0 unx        0 b- defN 23-May-18 12:46 mmenot/__init__.py
+Zip file size: 24230 bytes, number of entries: 16
+-rw-r--r--  2.0 unx        0 b- defN 23-May-19 09:36 mmenot/__init__.py
 -rw-r--r--  2.0 unx     2935 b- defN 23-May-17 06:09 mmenot/exporter.py
 -rw-r--r--  2.0 unx     5489 b- defN 23-May-17 06:09 mmenot/labels.py
 -rw-r--r--  2.0 unx     5930 b- defN 23-May-18 12:45 mmenot/loops.py
--rw-r--r--  2.0 unx     5198 b- defN 23-May-18 12:45 mmenot/pruner.py
+-rw-r--r--  2.0 unx     1456 b- defN 23-May-19 09:31 mmenot/patches.py
+-rw-r--r--  2.0 unx     5458 b- defN 23-May-19 09:31 mmenot/pruner.py
 -rw-r--r--  2.0 unx      633 b- defN 23-May-17 06:09 mmenot/runner.py
 -rw-r--r--  2.0 unx     3034 b- defN 23-May-17 06:09 mmenot/tester.py
 -rw-r--r--  2.0 unx     4989 b- defN 23-May-17 06:09 mmenot/trainer.py
 -rw-r--r--  2.0 unx    11638 b- defN 23-May-18 12:45 mmenot/utils.py
--rw-rw-rw-  2.0 unx    11338 b- defN 23-May-18 12:46 mmenot-0.9.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    13960 b- defN 23-May-18 12:46 mmenot-0.9.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-18 12:46 mmenot-0.9.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      139 b- defN 23-May-18 12:46 mmenot-0.9.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-May-18 12:46 mmenot-0.9.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1134 b- defN 23-May-18 12:46 mmenot-0.9.0.dist-info/RECORD
-15 files, 66516 bytes uncompressed, 21496 bytes compressed:  67.7%
+-rw-rw-rw-  2.0 unx    11338 b- defN 23-May-19 09:36 mmenot-0.9.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14257 b- defN 23-May-19 09:36 mmenot-0.9.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-19 09:36 mmenot-0.9.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      139 b- defN 23-May-19 09:36 mmenot-0.9.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-May-19 09:36 mmenot-0.9.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1208 b- defN 23-May-19 09:36 mmenot-0.9.1.dist-info/RECORD
+16 files, 68603 bytes uncompressed, 22278 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: mmenot/labels.py
 Comment: 
 
 Filename: mmenot/loops.py
 Comment: 
 
+Filename: mmenot/patches.py
+Comment: 
+
 Filename: mmenot/pruner.py
 Comment: 
 
 Filename: mmenot/runner.py
 Comment: 
 
 Filename: mmenot/tester.py
@@ -21,26 +24,26 @@
 
 Filename: mmenot/trainer.py
 Comment: 
 
 Filename: mmenot/utils.py
 Comment: 
 
-Filename: mmenot-0.9.0.dist-info/LICENSE
+Filename: mmenot-0.9.1.dist-info/LICENSE
 Comment: 
 
-Filename: mmenot-0.9.0.dist-info/METADATA
+Filename: mmenot-0.9.1.dist-info/METADATA
 Comment: 
 
-Filename: mmenot-0.9.0.dist-info/WHEEL
+Filename: mmenot-0.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: mmenot-0.9.0.dist-info/entry_points.txt
+Filename: mmenot-0.9.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: mmenot-0.9.0.dist-info/top_level.txt
+Filename: mmenot-0.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: mmenot-0.9.0.dist-info/RECORD
+Filename: mmenot-0.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mmenot/pruner.py

```diff
@@ -4,14 +4,25 @@
 import torch
 from mmengine.config import Config
 from mmengine.config import DictAction
 
 from mmenot.loops import EpochBasedPruningLoop  # pylint: disable=unused-import
 from mmenot.runner import PruningRunner
 
+# apply patches.
+try:
+    # pylint: disable=C0412
+    import mmseg.models.decode_heads.decode_head
+
+    from mmenot.patches import loss_by_feat
+
+    mmseg.models.decode_heads.decode_head.BaseDecodeHead.loss_by_feat = loss_by_feat
+except ImportError:
+    pass
+
 
 def parse_args():  # pylint: disable=missing-function-docstring
     parser = argparse.ArgumentParser(description='Prune a model')
     parser.add_argument('config', help='train config file path')
     parser.add_argument('--checkpoint', type=str, default='', help='path to checkpoint, overrides model config')
     parser.add_argument(
         '--pruning-type',
```

## Comparing `mmenot-0.9.0.dist-info/LICENSE` & `mmenot-0.9.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mmenot-0.9.0.dist-info/METADATA` & `mmenot-0.9.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: mmenot
-Version: 0.9.0
+Version: 0.9.1
+Summary: ENOT Framework integration package for OpenMMLab codebase
 Author-email: ENOT LLC <enot@enot.ai>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -200,22 +201,25 @@
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
+Project-URL: homepage, https://enot.ai
+Project-URL: documentation, https://enot-autodl.rtd.enot.ai/en/latest/openmmlab/mmenot.html
 Keywords: AI,ENOT,Pruning,MMDetection,MMSegmentation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mmengine (>=0.7.2)
 Requires-Dist: mmcv (>=2.0.0)
 Requires-Dist: mmdeploy (>=1.0.0)
 Requires-Dist: onnx
 Requires-Dist: numpy
 Requires-Dist: enot-latency-server
@@ -226,7 +230,8 @@
 Requires-Dist: pre-commit ; extra == 'dev'
 Requires-Dist: isort ; extra == 'dev'
 Provides-Extra: mmdet
 Requires-Dist: mmdet (>=3.0.0) ; extra == 'mmdet'
 Provides-Extra: mmseg
 Requires-Dist: mmsegmentation (>=1.0.0) ; extra == 'mmseg'
 
+ENOT Framework integration package for OpenMMLab codebase.
```

## Comparing `mmenot-0.9.0.dist-info/RECORD` & `mmenot-0.9.1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 mmenot/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mmenot/exporter.py,sha256=WlClJ-jvcR3KxfkZaUy8gWZ-SepMkkwz6tL_wLgUDpk,2935
 mmenot/labels.py,sha256=jk9YVE-hSYInKWjkj0PylF-Gnr_4saQVH-Xdb6jne7E,5489
 mmenot/loops.py,sha256=BT7O0v3MAMttPTeQQ27bi6JtYN_CHo6JFzRkY80VTrA,5930
-mmenot/pruner.py,sha256=QgMr3iOY6vwep5WGE9F6GUIiDFGcZjgLwy5fFknfoR4,5198
+mmenot/patches.py,sha256=4cwAotsPxAKP7CbkvgeBMif9QgPi4jRLl4fYFfJw-dM,1456
+mmenot/pruner.py,sha256=Bvy5dhwKZC0KEQtNy-IZo4lWf-Pg8e_RtKQK7f2pKpU,5458
 mmenot/runner.py,sha256=VnKZwKBB8xPtVldUX-7DdEpYdh4wVjiUArEBV4PdbjM,633
 mmenot/tester.py,sha256=5ckHo9Isn_-H2p_47A2-yvc_CyZJHaZjMjFNs6mtVeM,3034
 mmenot/trainer.py,sha256=aTZd3qEZ7oifWXhq31foz9xkWTCQbjCOeDnMzJF8mfg,4989
 mmenot/utils.py,sha256=vOHB0qDSkFWPl7YbR_KlCCmFh9p1SX-ThcPW0WYgWwM,11638
-mmenot-0.9.0.dist-info/LICENSE,sha256=iWLEJUustLjDYQcmBAwQmj0-kh3XqQi2kHpvDIc8suA,11338
-mmenot-0.9.0.dist-info/METADATA,sha256=BFbihm2o9y9drmGdV5bppfrG1rLAWdzQ9b_sBwphinw,13960
-mmenot-0.9.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mmenot-0.9.0.dist-info/entry_points.txt,sha256=9T5dLAFO5XGe0IOG2cvWvzRc4apXIGgBi4k3mTdRtj8,139
-mmenot-0.9.0.dist-info/top_level.txt,sha256=WV_L47You9buX7kgIYAYhqcdL8TrWmexP6IEWqH2R_4,7
-mmenot-0.9.0.dist-info/RECORD,,
+mmenot-0.9.1.dist-info/LICENSE,sha256=iWLEJUustLjDYQcmBAwQmj0-kh3XqQi2kHpvDIc8suA,11338
+mmenot-0.9.1.dist-info/METADATA,sha256=Yfh_sTkGMk4Usp3tG3wZYw7THsccEJVVKSbWHtnySGo,14257
+mmenot-0.9.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mmenot-0.9.1.dist-info/entry_points.txt,sha256=9T5dLAFO5XGe0IOG2cvWvzRc4apXIGgBi4k3mTdRtj8,139
+mmenot-0.9.1.dist-info/top_level.txt,sha256=WV_L47You9buX7kgIYAYhqcdL8TrWmexP6IEWqH2R_4,7
+mmenot-0.9.1.dist-info/RECORD,,
```

