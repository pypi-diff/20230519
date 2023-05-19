# Comparing `tmp/visual-compare-1.0.1.tar.gz` & `tmp/visual-compare-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visual-compare-1.0.1.tar", last modified: Tue May 16 07:00:00 2023, max compression
+gzip compressed data, was "visual-compare-1.0.2.tar", last modified: Fri May 19 07:11:45 2023, max compression
```

## Comparing `visual-compare-1.0.1.tar` & `visual-compare-1.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 07:00:00.314780 visual-compare-1.0.1/
--rw-rw-rw-   0        0        0     2023 2023-05-16 07:00:00.314780 visual-compare-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1206 2023-05-15 07:25:08.000000 visual-compare-1.0.1/README.md
--rw-rw-rw-   0        0        0      145 2023-05-16 07:00:00.314780 visual-compare-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1553 2023-05-16 06:59:52.000000 visual-compare-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:00:00.276193 visual-compare-1.0.1/visual_compare/
--rw-rw-rw-   0        0        0      376 2023-05-11 08:57:00.000000 visual-compare-1.0.1/visual_compare/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:00:00.294979 visual-compare-1.0.1/visual_compare/doc/
--rw-rw-rw-   0        0        0      378 2023-05-06 03:02:28.000000 visual-compare-1.0.1/visual_compare/doc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:00:00.296498 visual-compare-1.0.1/visual_compare/doc/image/
--rw-rw-rw-   0        0        0      378 2023-05-06 02:02:25.000000 visual-compare-1.0.1/visual_compare/doc/image/__init__.py
--rw-rw-rw-   0        0        0    29164 2023-05-11 09:04:51.000000 visual-compare-1.0.1/visual_compare/doc/image/compare_image.py
--rw-rw-rw-   0        0        0     3588 2023-05-15 02:33:50.000000 visual-compare-1.0.1/visual_compare/doc/image/image.py
--rw-rw-rw-   0        0        0     8588 2023-05-06 02:43:34.000000 visual-compare-1.0.1/visual_compare/doc/image/ocr.py
--rw-rw-rw-   0        0        0     2955 2023-05-12 09:18:28.000000 visual-compare-1.0.1/visual_compare/doc/match.py
--rw-rw-rw-   0        0        0      568 2023-05-12 10:32:40.000000 visual-compare-1.0.1/visual_compare/doc/models.py
--rw-rw-rw-   0        0        0     2164 2023-05-15 07:15:15.000000 visual-compare-1.0.1/visual_compare/doc/pdf.py
--rw-rw-rw-   0        0        0    12294 2023-05-09 03:42:47.000000 visual-compare-1.0.1/visual_compare/doc/pdf_test.py
--rw-rw-rw-   0        0        0    51498 2023-05-15 07:15:15.000000 visual-compare-1.0.1/visual_compare/doc/visual.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:00:00.310187 visual-compare-1.0.1/visual_compare/tests/
--rw-rw-rw-   0        0        0      378 2023-05-06 06:06:48.000000 visual-compare-1.0.1/visual_compare/tests/__init__.py
--rw-rw-rw-   0        0        0      376 2023-05-08 10:05:50.000000 visual-compare-1.0.1/visual_compare/tests/conftest.py
--rw-rw-rw-   0        0        0      714 2023-05-11 08:57:00.000000 visual-compare-1.0.1/visual_compare/tests/test_downloader.py
--rw-rw-rw-   0        0        0     1412 2023-05-15 02:03:24.000000 visual-compare-1.0.1/visual_compare/tests/test_image.py
--rw-rw-rw-   0        0        0     3005 2023-05-16 06:59:28.000000 visual-compare-1.0.1/visual_compare/tests/test_ocr.py
--rw-rw-rw-   0        0        0     2735 2023-05-15 09:34:23.000000 visual-compare-1.0.1/visual_compare/tests/test_paddle.py
--rw-rw-rw-   0        0        0      799 2023-05-15 07:04:57.000000 visual-compare-1.0.1/visual_compare/tests/test_pdf.py
--rw-rw-rw-   0        0        0      833 2023-05-15 10:16:35.000000 visual-compare-1.0.1/visual_compare/tests/test_torch.py
--rw-rw-rw-   0        0        0     2139 2023-05-15 07:17:08.000000 visual-compare-1.0.1/visual_compare/tests/test_visual.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:00:00.313252 visual-compare-1.0.1/visual_compare/utils/
--rw-rw-rw-   0        0        0      378 2023-05-06 02:26:53.000000 visual-compare-1.0.1/visual_compare/utils/__init__.py
--rw-rw-rw-   0        0        0     1002 2023-05-15 03:07:32.000000 visual-compare-1.0.1/visual_compare/utils/common.py
--rw-rw-rw-   0        0        0     1626 2023-05-11 09:04:51.000000 visual-compare-1.0.1/visual_compare/utils/downloader.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:00:00.288329 visual-compare-1.0.1/visual_compare.egg-info/
--rw-rw-rw-   0        0        0     2023 2023-05-16 07:00:00.000000 visual-compare-1.0.1/visual_compare.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1013 2023-05-16 07:00:00.000000 visual-compare-1.0.1/visual_compare.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 07:00:00.000000 visual-compare-1.0.1/visual_compare.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-08 07:02:46.000000 visual-compare-1.0.1/visual_compare.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      174 2023-05-16 07:00:00.000000 visual-compare-1.0.1/visual_compare.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-16 07:00:00.000000 visual-compare-1.0.1/visual_compare.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 07:11:45.724431 visual-compare-1.0.2/
+-rw-rw-rw-   0        0        0     2560 2023-05-19 07:11:45.724431 visual-compare-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1743 2023-05-19 06:57:05.000000 visual-compare-1.0.2/README.md
+-rw-rw-rw-   0        0        0      145 2023-05-19 07:11:45.724431 visual-compare-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1609 2023-05-19 06:57:05.000000 visual-compare-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 07:11:45.648483 visual-compare-1.0.2/visual_compare/
+-rw-rw-rw-   0        0        0      376 2023-05-11 08:57:00.000000 visual-compare-1.0.2/visual_compare/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 07:11:45.683529 visual-compare-1.0.2/visual_compare/doc/
+-rw-rw-rw-   0        0        0      378 2023-05-06 03:02:28.000000 visual-compare-1.0.2/visual_compare/doc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 07:11:45.690617 visual-compare-1.0.2/visual_compare/doc/image/
+-rw-rw-rw-   0        0        0      378 2023-05-06 02:02:25.000000 visual-compare-1.0.2/visual_compare/doc/image/__init__.py
+-rw-rw-rw-   0        0        0    30266 2023-05-19 06:57:05.000000 visual-compare-1.0.2/visual_compare/doc/image/compare_image.py
+-rw-rw-rw-   0        0        0     3984 2023-05-19 06:57:06.000000 visual-compare-1.0.2/visual_compare/doc/image/image.py
+-rw-rw-rw-   0        0        0    10447 2023-05-19 06:57:06.000000 visual-compare-1.0.2/visual_compare/doc/image/ocr.py
+-rw-rw-rw-   0        0        0     2955 2023-05-12 09:18:28.000000 visual-compare-1.0.2/visual_compare/doc/match.py
+-rw-rw-rw-   0        0        0      672 2023-05-19 06:57:06.000000 visual-compare-1.0.2/visual_compare/doc/models.py
+-rw-rw-rw-   0        0        0     2164 2023-05-15 07:15:15.000000 visual-compare-1.0.2/visual_compare/doc/pdf.py
+-rw-rw-rw-   0        0        0    12294 2023-05-09 03:42:47.000000 visual-compare-1.0.2/visual_compare/doc/pdf_test.py
+-rw-rw-rw-   0        0        0    58242 2023-05-19 06:57:06.000000 visual-compare-1.0.2/visual_compare/doc/visual.py
+drwxrwxrwx   0        0        0        0 2023-05-19 07:11:45.715790 visual-compare-1.0.2/visual_compare/tests/
+-rw-rw-rw-   0        0        0      378 2023-05-06 06:06:48.000000 visual-compare-1.0.2/visual_compare/tests/__init__.py
+-rw-rw-rw-   0        0        0      376 2023-05-08 10:05:50.000000 visual-compare-1.0.2/visual_compare/tests/conftest.py
+-rw-rw-rw-   0        0        0      714 2023-05-11 08:57:00.000000 visual-compare-1.0.2/visual_compare/tests/test_downloader.py
+-rw-rw-rw-   0        0        0     2241 2023-05-19 06:57:06.000000 visual-compare-1.0.2/visual_compare/tests/test_image.py
+-rw-rw-rw-   0        0        0     4216 2023-05-19 06:57:06.000000 visual-compare-1.0.2/visual_compare/tests/test_ocr.py
+-rw-rw-rw-   0        0        0     2735 2023-05-19 06:57:06.000000 visual-compare-1.0.2/visual_compare/tests/test_paddle.py
+-rw-rw-rw-   0        0        0      799 2023-05-15 07:04:57.000000 visual-compare-1.0.2/visual_compare/tests/test_pdf.py
+-rw-rw-rw-   0        0        0      833 2023-05-19 06:57:06.000000 visual-compare-1.0.2/visual_compare/tests/test_torch.py
+-rw-rw-rw-   0        0        0     2716 2023-05-19 06:57:06.000000 visual-compare-1.0.2/visual_compare/tests/test_visual.py
+drwxrwxrwx   0        0        0        0 2023-05-19 07:11:45.722400 visual-compare-1.0.2/visual_compare/utils/
+-rw-rw-rw-   0        0        0      378 2023-05-06 02:26:53.000000 visual-compare-1.0.2/visual_compare/utils/__init__.py
+-rw-rw-rw-   0        0        0     1002 2023-05-15 03:07:32.000000 visual-compare-1.0.2/visual_compare/utils/common.py
+-rw-rw-rw-   0        0        0     1626 2023-05-11 09:04:51.000000 visual-compare-1.0.2/visual_compare/utils/downloader.py
+drwxrwxrwx   0        0        0        0 2023-05-19 07:11:45.655555 visual-compare-1.0.2/visual_compare.egg-info/
+-rw-rw-rw-   0        0        0     2560 2023-05-19 07:11:45.000000 visual-compare-1.0.2/visual_compare.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1013 2023-05-19 07:11:45.000000 visual-compare-1.0.2/visual_compare.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 07:11:45.000000 visual-compare-1.0.2/visual_compare.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-08 07:02:46.000000 visual-compare-1.0.2/visual_compare.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      206 2023-05-19 07:11:45.000000 visual-compare-1.0.2/visual_compare.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-19 07:11:45.000000 visual-compare-1.0.2/visual_compare.egg-info/top_level.txt
```

### Comparing `visual-compare-1.0.1/PKG-INFO` & `visual-compare-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visual-compare
-Version: 1.0.1
+Version: 1.0.2
 Summary: Image and PDF Compare
 Home-page: https://github.com/cuidingyong/visual-compare
 Author: Dillon
 Author-email: cuidingyong@yeah.net
 License: MIT
 Keywords: visual compare image pdf diff
 Platform: UNKNOWN
@@ -71,7 +71,28 @@
 assert is_diff is True
 ```
 
  Result as follows
 
 ![2.jpg](https://github.com/cuidingyong/visual-compare/raw/main/files/result/2.jpg)
 
+### Compare images with OCR ###
+
+```python
+from visual_compare.doc.visual import Visual
+
+def get_path(filename):
+    image_base = '../../files/images/'
+    return image_base + filename
+
+reference_image = get_path('123.png')
+test_image = get_path('124.png')
+vt = Visual()
+is_diff, res = vt.compare_images(reference_image, test_image, force_ocr=True, lang=['ch_sim', 'en'])
+print(res)
+assert is_diff is True
+```
+
+ Result as follows
+
+![3.jpg](https://github.com/cuidingyong/visual-compare/raw/main/files/result/3.jpg)
+
```

### Comparing `visual-compare-1.0.1/README.md` & `visual-compare-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -47,8 +47,29 @@
 is_diff, res = vt.compare_images(reference_image, test_image, mask=mask)
 print(res)
 assert is_diff is True
 ```
 
  Result as follows
 
-![2.jpg](https://github.com/cuidingyong/visual-compare/raw/main/files/result/2.jpg)
+![2.jpg](https://github.com/cuidingyong/visual-compare/raw/main/files/result/2.jpg)
+
+### Compare images with OCR ###
+
+```python
+from visual_compare.doc.visual import Visual
+
+def get_path(filename):
+    image_base = '../../files/images/'
+    return image_base + filename
+
+reference_image = get_path('123.png')
+test_image = get_path('124.png')
+vt = Visual()
+is_diff, res = vt.compare_images(reference_image, test_image, force_ocr=True, lang=['ch_sim', 'en'])
+print(res)
+assert is_diff is True
+```
+
+ Result as follows
+
+![3.jpg](https://github.com/cuidingyong/visual-compare/raw/main/files/result/3.jpg)
```

### Comparing `visual-compare-1.0.1/setup.py` & `visual-compare-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="visual-compare",
-    version="1.0.1",
+    version="1.0.2",
     description="Image and PDF Compare",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cuidingyong/visual-compare",
     author="Dillon",
     author_email="cuidingyong@yeah.net",
     license="MIT",
@@ -37,11 +37,13 @@
         "imutils~=0.5.4",
         "scikit-image~=0.20",
         "pytesseract~=0.3.10",
         "parsimonious~=0.10",
         "PyMuPDF~=1.22",
         "pyzbar~=0.1.9",
         "pylibdmtx~=0.1.10",
-        "Wand~=0.6.11"
+        "Wand~=0.6.11",
+        "pydantic~=1.8.2",
+        "deepdiff~=6.3.0"
     ],
     zip_safe=False,
 )
```

### Comparing `visual-compare-1.0.1/visual_compare/doc/image/compare_image.py` & `visual-compare-1.0.2/visual_compare/doc/image/compare_image.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,23 +17,24 @@
 import re
 import sys
 import tempfile
 import time
 from os.path import splitext, split
 
 import cv2
+import easyocr
 import fitz
 import numpy as np
 import pytesseract
 from pytesseract import Output
 
+from visual_compare.utils.common import is_url
 from visual_compare.utils.downloader import download_file_from_url
 from .ocr import EastTextExtractor
-from ..match import MatchPdf
-from visual_compare.utils.common import is_url
+from ..models import Contour
 
 logger = logging.getLogger(__name__)
 
 EAST_CONFIDENCE = 0.5
 
 
 class CompareImage(object):
@@ -49,24 +50,28 @@
         self.placeholder_file = kwargs.pop('placeholder_file', None)
         self.mask = kwargs.pop('mask', None)
         self.contains_barcodes = kwargs.pop('contains_barcodes', False)
         self.get_pdf_content = kwargs.pop('get_pdf_content', False)
         self.force_ocr = kwargs.pop('force_ocr', False)
         self.ocr_engine = kwargs.pop('ocr_engine', 'tesseract')
         self.DPI = int(kwargs.pop('DPI', 200))
+        self.lang = kwargs.pop('lang', 'en')
+        self.contrast_ths = kwargs.pop('contrast_ths', 0.4)
+        self.adjust_contrast = kwargs.pop('adjust_contrast', 0.6)
         if is_url(image):
             self.image = download_file_from_url(image)
         else:
             self.image = str(image)
         self.path, self.filename = split(self.image)
         self.filename_without_extension, self.extension = splitext(self.filename)
         self.opencv_images = []
         self.placeholders = []
         self.placeholder_mask = None
         self.text_content = []
+        self.ocr_text_contents = []
         # self.pdf_content = []
         self.placeholder_frame_width = 10
         self.tmp_directory = tempfile.TemporaryDirectory()
         self.diff_images = []
         self.threshold_images = []
         self.barcodes = []
         self.re_rendered_for_ocr = False
@@ -137,14 +142,37 @@
                     width_list.append(d['width'][j])
                     height_list.append(d['height'][j])
                     conf_list.append(d['conf'][j])
             self.text_content.append(
                 {'text': text_list, 'left': left_list, 'top': top_list, 'width': width_list, 'height': height_list,
                  'conf': conf_list})
 
+    def get_ocr_text_content(self):
+        # self.increase_resolution_for_ocr()
+        for i in range(len(self.opencv_images)):
+            ocr_text_content = []
+            cv_image = self.opencv_images[i]
+            gray_image = cv2.cvtColor(cv_image, cv2.COLOR_BGR2GRAY)
+            threshold_image = cv2.threshold(gray_image, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)[1]
+            reader = easyocr.Reader(self.lang)
+            text_list = reader.readtext(threshold_image, contrast_ths=self.contrast_ths,
+                                        adjust_contrast=self.adjust_contrast)
+            # eo = EasyOcr(self.lang)
+            # text_list = eo.get_image_text_and_coordinate(threshold_image)
+            for text in text_list:
+                na = np.array(text[0]).astype(np.int32)
+                x, y, w, h = cv2.boundingRect(na)
+                # try:
+                #     x, y, w, h = cv2.boundingRect(na)
+                # except Exception as e:
+                #     print(e)
+                ct = Contour(text=text[1], x=x, y=y, width=w, height=h)
+                ocr_text_content.append(ct)
+            self.ocr_text_contents.append(ocr_text_content)
+
     def increase_resolution_for_ocr(self):
         # experimental: IF OCR is used and DPI is lower than self.MINIMUM_OCR_RESOLUTION DPI, re-render with self.MINIMUM_OCR_RESOLUTION DPI
         if self.DPI < self.MINIMUM_OCR_RESOLUTION:
             logger.info("Re-Render document for OCR at {} DPI as current resolution is only {} DPI".format(
                 self.MINIMUM_OCR_RESOLUTION, self.DPI))
             if self.extension == '.pdf':
                 self.convert_mupdf_to_opencv_image(resolution=self.MINIMUM_OCR_RESOLUTION)
@@ -172,30 +200,23 @@
         for frame in self.opencv_images:
             text = self.east_text_extractor.get_image_text(frame)
             self.text_content.append(text)
 
     def identify_placeholders(self):
         placeholders = None
         if self.placeholder_file is not None:
-            if isinstance(self.placeholder_file, list):
-                placeholders = []
-                for pf in self.placeholder_file:
-                    if self.is_image(pf):
-                        mi = MatchPdf(self.opencv_images[0], pf)
-                        placeholders.extend(mi.mask)
-            elif isinstance(self.placeholders, str):
-                try:
-                    with open(self.placeholder_file, 'r') as f:
-                        placeholders = json.load(f)
-                except IOError as err:
-                    logger.error("Placeholder File %s is not accessible", self.placeholder_file)
-                    logger.error("I/O error: {0}".format(err))
-                except:
-                    logger.error("Unexpected error:", sys.exc_info()[0])
-                    raise
+            try:
+                with open(self.placeholder_file, 'r') as f:
+                    placeholders = json.load(f)
+            except IOError as err:
+                logger.error("Placeholder File %s is not accessible", self.placeholder_file)
+                logger.error("I/O error: {0}".format(err))
+            except:
+                logger.error("Unexpected error:", sys.exc_info()[0])
+                raise
         elif self.mask is not None:
             if isinstance(self.mask, dict):
                 placeholders = self.mask
             elif isinstance(self.mask, list):
                 placeholders = self.mask
             elif isinstance(self.mask, str):
                 try:
@@ -512,14 +533,16 @@
                 self.opencv_images.append(img)
 
     def load_text_content_and_identify_masks(self):
         if (self.placeholder_file is not None) or (self.mask is not None):
             self.identify_placeholders()
         if self.contains_barcodes is True:
             self.identify_barcodes()
+        if self.force_ocr:
+            self.get_ocr_text_content()
         if self.placeholders:
             print('Identified Masks: {}'.format(self.placeholders))
 
     def get_text_content_from_mupdf(self):
         pass
 
     def convert_pywand_to_opencv_image(self, resolution=None):
```

### Comparing `visual-compare-1.0.1/visual_compare/doc/image/image.py` & `visual-compare-1.0.2/visual_compare/doc/image/image.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,21 +7,21 @@
    Author:          dingyong.cui
    date：           2023/5/6
 -------------------------------------------------
    Change Activity:
                     2023/5/6
 -------------------------------------------------
 """
+import os
 from typing import Union
 
 import cv2
 import numpy
-import os
 
-from visual_compare.doc.models import Mask
+from visual_compare.doc.models import Mask, Contour
 from visual_compare.utils.common import is_url
 from visual_compare.utils.downloader import download_file_from_url
 
 
 class Image:
 
     def __init__(self, image: str):
@@ -41,14 +41,46 @@
         return self.image.shape[1]
 
     @property
     def height(self):
         return self.image.shape[0]
 
 
+class OcrImage:
+
+    def __init__(self, text: str, x: int, y: int, width: int, height: int):
+        self.text = text
+        self.x = x
+        self.y = y
+        self.width = width
+        self.height = height
+        self._identical = False
+
+    @property
+    def identical(self):
+        return self._identical
+
+    def equal(self, other: Contour, strip: bool = True, space_remove: bool = True, coordinate_eq: bool = False):
+        self._identical = False
+        if strip:
+            self.text = self.text.strip()
+            other.text = other.text.strip()
+        if space_remove:
+            self.text = self.text.replace(' ', '')
+            other.text = other.text.replace(' ', '')
+        if coordinate_eq:
+            if self.x != other.x or self.y != other.y or self.width != other.width or self.height != other.height:
+                return False
+        if self.text == other.text:
+            self._identical = True
+            return True
+        else:
+            return False
+
+
 class MatchImg:
 
     def __init__(self, threshold=0.95, match_method=cv2.TM_CCOEFF_NORMED):
         self.threshold = threshold
         self.match_method = match_method
         self.match = []
 
@@ -68,35 +100,21 @@
     @staticmethod
     def uniform_channel(img):
         if img.shape[2] == 4:
             img = img[:, :, :3]
 
         return img
 
-    # def parse_mask(self, source: str, temp: str, threshold=None, match_method=cv2.TM_CCOEFF_NORMED,
-    #                mask_type='coordinates', page: Union[str, int] = 'all'):
-    #     source_img = Image(source)
-    #     temp_img = Image(temp)
-    # 
-    #     mask_list = []
-    #     match_list = self.match_temp(source_img.image, temp_img.image, threshold, match_method)
-    #     for m in match_list:
-    #         mask = Mask(type=mask_type, page=1, x=m[0], y=m[1], width=temp_img.width, height=temp_img.height)
-    #         mask_list.append(mask.dict())
-    # 
-    #     return mask_list
-
     def parse_mask(self, source: Union[str, list], temp: Union[str, list], threshold=None,
                    match_method=cv2.TM_CCOEFF_NORMED, mask_type='coordinates'):
         if isinstance(source, str):
             source = [source]
         if isinstance(temp, str):
             temp = [temp]
         for i, s in enumerate(source):
-            # sii = Image(s)
             for t in temp:
                 ti = Image(t)
                 match_list = self.match_temp(s, ti.image, threshold, match_method)
                 if match_list:
                     self.collect(match_list, ti.width, ti.height, mask_type, i + 1)
 
         return self.match
```

### Comparing `visual-compare-1.0.1/visual_compare/doc/image/ocr.py` & `visual-compare-1.0.2/visual_compare/doc/image/ocr.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 import cv2
 import numpy as np
 import pytesseract
 from imutils.object_detection import non_max_suppression
 import urllib
 import re
 import unicodedata
+from pytesseract import Output
+
+from visual_compare.doc.models import Contour
 
 PYTESSERACT_CONFIDENCE = 20
 
 
 def remove_control_characters(s):
     return "".join(ch for ch in s if unicodedata.category(ch)[0] != "C")
 
@@ -33,14 +36,56 @@
     layer_names = ('feature_fusion/Conv_7/Sigmoid', 'feature_fusion/concat_3',)
 
     def __init__(self, east=None):
         pkg_east_model = resource_filename(__name__, 'data/frozen_east_text_detection.pb')
         self.east = east or pkg_east_model
         self._load_assets()
 
+    def get_image_text_and_coordinate(self,
+                                      image,
+                                      width=480,
+                                      height=480,
+                                      conf_threshold=0.2,
+                                      **kwargs):
+        loaded_image = image
+
+        image, width, height, ratio_width, ratio_height = self._resize_image(
+            loaded_image, width, height
+        )
+        scores, geometry = self._compute_scores_geometry(image, width, height)
+
+        # decoding results from the model
+        rectangles, confidences = box_extractor(scores, geometry, conf_threshold)
+
+        # find contours of all rectangles
+        mask = np.zeros((height, width), dtype=np.uint8)
+        for i in range(len(rectangles)):
+            x1, y1, x2, y2 = rectangles[i]
+            cv2.rectangle(mask, (x1, y1), (x2, y2), 255, -1)
+
+        contours, hierarchy = cv2.findContours(mask, cv2.RETR_LIST, cv2.CHAIN_APPROX_SIMPLE)
+        results = []
+        for i in range(len(contours) - 1, -1, -1):
+            x, y, w, h = cv2.boundingRect(contours[i])
+            start_x = int(x * ratio_width)
+            start_y = int(y * ratio_height)
+            end_x = int((x + w) * ratio_width)
+            end_y = int((y + h) * ratio_height)
+            # ROI to be recognized
+            roi = loaded_image[start_y:end_y, start_x:end_x]
+
+            # recognizing text
+            config = '-l jpn --oem 1 --psm 7'
+            text = str(pytesseract.image_to_string(roi, config=config))
+
+            ct = Contour(text=text, x=start_x, y=start_y, width=end_x - start_x, height=end_y - start_y)
+            results.append(ct)
+
+        return results
+
     def get_image_text(self,
                        image,
                        width=480,
                        height=480,
                        numbers=True,
                        confThreshold=0.2,
                        nmsThreshold=0.1,
@@ -55,16 +100,15 @@
             loaded_image, width, height
         )
         scores, geometry = self._compute_scores_geometry(image, width, height)
 
         # decoding results from the model
         rectangles, confidences = box_extractor(scores, geometry, confThreshold)
 
-        # find countur of all rectangles
-
+        # find contours of all rectangles
         mask = np.zeros((height, width), dtype=np.uint8)
         for i in range(len(rectangles)):
             x1, y1, x2, y2 = rectangles[i]
             cv2.rectangle(mask, (x1, y1), (x2, y2), 255, -1)
 
         contours, hierarchy = cv2.findContours(mask, cv2.RETR_LIST, cv2.CHAIN_APPROX_SIMPLE)
         results = {'text': [], 'left': [], 'top': [], 'width': [], 'height': []}
@@ -86,43 +130,45 @@
             results['left'].append(start_x)
             results['top'].append(start_y)
             results['width'].append(end_x - start_x)
             results['height'].append(end_y - start_y)
 
         return results
 
-    def _load_image(self, image):
+    @staticmethod
+    def _load_image(image):
         return cv2.imread(image)
 
-    def _resize_image(self, image, width, height):
+    @staticmethod
+    def _resize_image(image, width, height):
         (H, W) = image.shape[:2]
 
         (newW, newH) = (width, height)
         ratio_width = W / float(newW)
         ratio_height = H / float(newH)
 
         # resize the image and grab the new image dimensions
         resized_image = cv2.resize(image, (newW, newH))
-        (H, W) = resized_image.shape[:2]
-        return (resized_image, height, width, ratio_width, ratio_height)
+        # (H, W) = resized_image.shape[:2]
+        return resized_image, height, width, ratio_width, ratio_height
 
     def _compute_scores_geometry(self, image, width, height):
         # construct a blob from the image and then perform a forward pass of
         # the model to obtain the two output layer sets
         blob = cv2.dnn.blobFromImage(
             image, 1.0, (width, height), (123.68, 116.78, 103.94), swapRB=True, crop=False
         )
         start = time.time()
         self.east_net.setInput(blob)
         (scores, geometry) = self.east_net.forward(self.layer_names)
         end = time.time()
 
         # show timing information on text prediction
         print('[INFO] text detection took {:.6f} seconds'.format(end - start))
-        return (scores, geometry)
+        return scores, geometry
 
     def _load_assets(self):
         self._get_east()
         start = time.time()
         self.east_net = cv2.dnn.readNet(self.east)
         end = time.time()
         print('[INFO] Loaded EAST text detector {:.6f} seconds ...'.format(end - start))
```

### Comparing `visual-compare-1.0.1/visual_compare/doc/match.py` & `visual-compare-1.0.2/visual_compare/doc/match.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.1/visual_compare/doc/pdf.py` & `visual-compare-1.0.2/visual_compare/doc/pdf.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.1/visual_compare/doc/pdf_test.py` & `visual-compare-1.0.2/visual_compare/doc/pdf_test.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.1/visual_compare/doc/visual.py` & `visual-compare-1.0.2/visual_compare/doc/visual.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import fitz
 import imutils
 import numpy as np
 import pytesseract
 from skimage import metrics
 
 from visual_compare.doc.image.compare_image import CompareImage
+from visual_compare.doc.models import Contour
 from visual_compare.utils.common import is_url, check_file_exist
 
 logger = logging.getLogger(__name__)
 
 
 class Visual(object):
     ROBOT_LIBRARY_VERSION = 0.2
@@ -46,19 +47,23 @@
     FONT_COLOR = (255, 0, 0)
     LINE_TYPE = 2
     THRESHOLD = 0.95
     REFERENCE_LABEL = "Expected Result (Reference)"
     CANDIDATE_LABEL = "Actual Result (Candidate)"
     OCR_ENGINE = "tesseract"
     MOVEMENT_DETECTION = "classic"
+    LANG_DEFAULT = 'en'
+    CONTRAST_THS_DEFAULT = 0.4
+    ADJUST_CONTRAST_DEFAULT = 0.6
 
     def __init__(self, threshold: float = 0.0000, dpi: int = DPI_DEFAULT,
                  take_screenshots: bool = False,
                  show_diff: bool = False, ocr_engine: str = OCR_ENGINE, movement_detection: str = MOVEMENT_DETECTION,
-                 watermark_file: str = None, screenshot_dir: str = None, screenshot_format: str = 'jpg', **kwargs):
+                 watermark_file: str = None, screenshot_dir: str = None, screenshot_format: str = 'jpg',
+                 lang: list = None, contrast_ths: float = None, adjust_contrast: float = None, **kwargs):
         """
         | =Arguments= | =Description= |
         | ``take_screenshots`` | Shall screenshots be taken also for passed comparisons.   |
         | ``show_diff`` | Shall a diff screenshot be added showing differences in black and white  |
         | ``screenshot_format`` | Image format of screenshots, ``jpg`` or ``png`` |
         | ``DPI`` | Resolution in which documents are rendered before comparison, only relevant for ``pdf``, ``ps`` and ``pcl``. Images will be compared in their original resolution |
         | ``watermark_file`` | Path to an image/document or a folder containing multiple images. They shall only contain a ```solid black`` area of the parts that shall be ignored for doc comparisons |
@@ -81,19 +86,26 @@
         self.screenshot_format = screenshot_format
         try:
             self.screenshot_dir = Path(screenshot_dir)
         except TypeError:
             self.screenshot_dir = Path.cwd() / Path("screenshots/")
         if not (self.screenshot_format == 'jpg' or self.screenshot_format == 'png'):
             self.screenshot_format = 'jpg'
+        self.lang = self.LANG_DEFAULT
+        if lang:
+            self.lang = lang
+        self.contrast_ths = self.CONTRAST_THS_DEFAULT
+        if contrast_ths:
+            self.contrast_ths = contrast_ths
+        self.adjust_contrast = self.ADJUST_CONTRAST_DEFAULT
+        if adjust_contrast:
+            self.adjust_contrast = adjust_contrast
 
         self._is_different = False
 
-        # self.check_exist([reference_image, test_image])
-
         self.reference_image = None
         self.test_image = None
 
     @property
     def is_different(self):
         return self._is_different
 
@@ -132,15 +144,17 @@
         return mask if len(mask) > 0 else None
 
     def compare_images(self, reference_image: str, test_image: str, placeholder_file: Union[str, list] = None,
                        mask: Union[str, dict, list] = None, check_text_content: bool = False,
                        move_tolerance: int = None, contains_barcodes: bool = False, get_pdf_content: bool = False,
                        force_ocr: bool = False, dpi: int = None, watermark_file: str = None,
                        ignore_watermarks: bool = None, ocr_engine: str = None, resize_candidate: bool = False,
-                       blur: bool = False, threshold: float = None, **kwargs):
+                       blur: bool = False, lang: list = None, threshold: float = None, contrast_ths: float = None,
+                       adjust_contrast: float = None, coordinate_eq: bool = False, strip: bool = True,
+                       space_remove: bool = True, **kwargs):
         """Compares the documents/images ``reference_image`` and ``test_image``.
 
         Result is passed if no doc differences are detected.
 
         | =Arguments= | =Description= |
         | ``reference_image`` | Path or URL of the Reference Image/Document, your expected result. May be .pdf, .ps, .pcl or image files |
         | ``test_image`` | Path or URL of the Candidate Image/Document, that's the one you want to test. May be .pdf, .ps, .pcl or image files |
@@ -178,41 +192,51 @@
             watermark_file = self.watermark_file
         if ignore_watermarks is None:
             ignore_watermarks = os.getenv('IGNORE_WATERMARKS', False)
         if ocr_engine is None:
             ocr_engine = self.ocr_engine
         if threshold is None:
             threshold = self.threshold
+        if lang is None:
+            lang = self.lang
+        if contrast_ths is None:
+            contrast_ths = self.contrast_ths
+        if adjust_contrast is None:
+            adjust_contrast = self.adjust_contrast
 
         if mask:
             threshold = threshold + 0.0001
 
         compare_options = {'get_pdf_content': get_pdf_content, 'ignore_watermarks': ignore_watermarks,
                            'check_text_content': check_text_content, 'contains_barcodes': contains_barcodes,
                            'force_ocr': force_ocr, 'move_tolerance': move_tolerance, 'watermark_file': watermark_file,
                            'ocr_engine': ocr_engine, 'resize_candidate': resize_candidate, 'blur': blur,
-                           'threshold': threshold}
+                           'threshold': threshold, 'coordinate_eq': coordinate_eq, 'strip': strip,
+                           'space_remove': space_remove}
 
         if (os.path.isfile(reference_image) is False) and (is_url(reference_image) is False):
             raise AssertionError(
                 'The reference file does not exist: {}'.format(reference_image))
 
         if (os.path.isfile(test_image) is False) and (is_url(test_image) is False):
             raise AssertionError(
                 'The candidate file does not exist: {}'.format(test_image))
 
         with futures.ThreadPoolExecutor(max_workers=2) as parallel_executor:
             reference_future = parallel_executor.submit(CompareImage, reference_image,
                                                         placeholder_file=placeholder_file,
                                                         contains_barcodes=contains_barcodes,
                                                         get_pdf_content=get_pdf_content, DPI=self.DPI,
-                                                        force_ocr=force_ocr, mask=mask, ocr_engine=ocr_engine)
+                                                        force_ocr=force_ocr, mask=mask, ocr_engine=ocr_engine,
+                                                        lang=lang, contrast_ths=contrast_ths,
+                                                        adjust_contrast=adjust_contrast)
             candidate_future = parallel_executor.submit(
                 CompareImage, test_image, contains_barcodes=contains_barcodes, get_pdf_content=get_pdf_content,
-                DPI=self.DPI)
+                DPI=self.DPI, force_ocr=force_ocr, lang=lang, contrast_ths=contrast_ths,
+                adjust_contrast=adjust_contrast)
             reference_compare_image = reference_future.result()
             candidate_compare_image = candidate_future.result()
 
         tic = time.perf_counter()
         if reference_compare_image.placeholders:
             candidate_compare_image.placeholders = reference_compare_image.placeholders
             with futures.ThreadPoolExecutor(max_workers=2) as parallel_executor:
@@ -241,28 +265,41 @@
                     compare_collection[i], "_candidate_page_" + str(i + 1))
             raise AssertionError(
                 'Reference File and Candidate File have different number of pages')
 
         check_difference_results = []
         with futures.ThreadPoolExecutor(max_workers=8) as parallel_executor:
             for i, (reference, candidate) in enumerate(zip(reference_collection, compare_collection)):
-                if get_pdf_content:
+                if force_ocr:
                     try:
-                        reference_pdf_content = reference_compare_image.mu_pdf_doc[i]
-                        candidate_pdf_content = candidate_compare_image.mu_pdf_doc[i]
-                    except:
-                        reference_pdf_content = reference_compare_image.mu_pdf_doc[0]
-                        candidate_pdf_content = candidate_compare_image.mu_pdf_doc[0]
+                        reference_text_content = reference_compare_image.ocr_text_contents[i]
+                        candidate_text_content = candidate_compare_image.ocr_text_contents[i]
+                    except IndexError:
+                        reference_text_content = reference_compare_image.ocr_text_contents[0]
+                        candidate_text_content = candidate_compare_image.ocr_text_contents[0]
+                    # print('reference -> ', reference_text_content)
+                    # print('candidate -> ', candidate_text_content)
+                    check_difference_results.append(parallel_executor.submit(
+                        self.check_for_ocr_differences, reference, candidate, i, detected_differences,
+                        screenshot_names, compare_options, reference_text_content, candidate_text_content))
                 else:
-                    reference_pdf_content = None
-                    candidate_pdf_content = None
-                check_difference_results.append(parallel_executor.submit(
-                    self.check_for_differences, reference, candidate, i, detected_differences, screenshot_names,
-                    compare_options,
-                    reference_pdf_content, candidate_pdf_content))
+                    if get_pdf_content:
+                        try:
+                            reference_pdf_content = reference_compare_image.mu_pdf_doc[i]
+                            candidate_pdf_content = candidate_compare_image.mu_pdf_doc[i]
+                        except IndexError:
+                            reference_pdf_content = reference_compare_image.mu_pdf_doc[0]
+                            candidate_pdf_content = candidate_compare_image.mu_pdf_doc[0]
+                    else:
+                        reference_pdf_content = None
+                        candidate_pdf_content = None
+                    check_difference_results.append(parallel_executor.submit(
+                        self.check_for_differences, reference, candidate, i, detected_differences, screenshot_names,
+                        compare_options,
+                        reference_pdf_content, candidate_pdf_content))
         for result in check_difference_results:
             if result.exception() is not None:
                 raise result.exception()
         if reference_compare_image.barcodes:
             if reference_compare_image.barcodes != candidate_compare_image.barcodes:
                 detected_differences.append(True)
                 logger.error(
@@ -526,16 +563,18 @@
             gray_a, gray_b, gaussian_weights=True, full=True)
         score = abs(1 - score)
 
         if score > compare_options['threshold']:
 
             diff = (diff * 255).astype("uint8")
 
-            thresh = cv2.threshold(diff, 0, 255,
-                                   cv2.THRESH_BINARY_INV | cv2.THRESH_OTSU)[1]
+            # thresh = cv2.threshold(diff, 0, 255,
+            #                        cv2.THRESH_BINARY_INV | cv2.THRESH_OTSU)[1]
+            thresh = cv2.threshold(diff, 127, 255,
+                                   cv2.THRESH_BINARY_INV)[1]
 
             reference_with_rect, candidate_with_rect, contours = self.get_images_with_highlighted_differences(
                 thresh, reference.copy(), candidate.copy(), extension=int(os.getenv('EXTENSION', 2)))
 
             cv2.putText(reference_with_rect, self.REFERENCE_LABEL, self.BOTTOM_LEFT_CORNER_OF_TEXT,
                         self.FONT, self.FONT_SCALE, self.FONT_COLOR, self.LINE_TYPE)
             cv2.putText(candidate_with_rect, self.CANDIDATE_LABEL, self.BOTTOM_LEFT_CORNER_OF_TEXT,
@@ -862,14 +901,99 @@
                                         print(
                                             "This is within the allowed range of ", move_tolerance, " pixels")
                                         self.add_screenshot_to_log(self.overlay_two_images(
                                             diff_area_reference, diff_area_candidate), "_diff_area_blended")
             if images_are_equal is not True:
                 detected_differences.append(True)
 
+    def check_for_ocr_differences(self, reference, candidate, i, detected_differences, screenshot_names,
+                                  compare_options, reference_text_content, candidate_text_content):
+        # reference_collections = reference_compare_image.opencv_images
+        # candidate_collections = candidate_compare_image.opencv_images
+        # reference_text_contents = reference_compare_image.ocr_text_contents
+        # candidate_text_contents = candidate_compare_image.ocr_text_contents
+        # for i in range(len(reference_collections)):
+        coordinate_eq = compare_options['coordinate_eq']
+        strip = compare_options['strip']
+        space_remove = compare_options['space_remove']
+        image_contents_are_equal = True
+        while image_contents_are_equal:
+            image_contents_are_equal, reference_text_content, candidate_text_content = self.get_parts_of_different(
+                reference_text_content, candidate_text_content, coordinate_eq, strip, space_remove)
+
+        reference_with_rect = self.highlight_differences(reference.copy(), reference_text_content)
+        candidate_with_rect = self.highlight_differences(candidate.copy(), candidate_text_content)
+
+        cv2.putText(reference_with_rect, self.REFERENCE_LABEL, self.BOTTOM_LEFT_CORNER_OF_TEXT,
+                    self.FONT, self.FONT_SCALE, self.FONT_COLOR, self.LINE_TYPE)
+        cv2.putText(candidate_with_rect, self.CANDIDATE_LABEL, self.BOTTOM_LEFT_CORNER_OF_TEXT,
+                    self.FONT, self.FONT_SCALE, self.FONT_COLOR, self.LINE_TYPE)
+
+        if reference_with_rect.shape[0] != candidate_with_rect.shape[0] or reference_with_rect.shape[1] != \
+                candidate_with_rect.shape[1]:
+            candidate_with_rect = cv2.resize(
+                candidate_with_rect, (reference_with_rect.shape[1], reference_with_rect.shape[0]))
+        screenshot_name = self.add_screenshot_to_log(np.concatenate(
+            (reference_with_rect, candidate_with_rect), axis=1), "_page_" + str(i + 1) + "_rectangles_concat")
+        screenshot_names.append(screenshot_name)
+
+        if len(reference_text_content) > 0 or len(candidate_text_content) > 0:
+            detected_differences.append(True)
+
+    @staticmethod
+    def highlight_differences(image, contents):
+        for c in contents:
+            cv2.rectangle(image, (c.x, c.y), (c.x + c.width, c.y + c.height), (0, 0, 255), 4)
+
+        return image
+
+    @staticmethod
+    def get_parts_of_different(reference, candidate, coordinate_eq, strip, space_remove):
+        eq_flag = False
+        ref_res, can_res = [], []
+        la, lb = len(reference) + 1, len(candidate) + 1
+        dp = [[0 for _ in range(lb)] for _ in range(la)]
+        max_num = 0
+        max_i = 0
+        max_j = 0
+        for i in range(la - 1):
+            for j in range(lb - 1):
+                if equal(reference[i], candidate[j], coordinate_eq=coordinate_eq, strip=strip,
+                         space_remove=space_remove):
+                    dp[i + 1][j + 1] = dp[i][j] + 1
+                    if eq_flag is False:
+                        eq_flag = True
+                if dp[i + 1][j + 1] > max_num:
+                    max_num = dp[i + 1][j + 1]
+                    max_i = i + 1
+                    max_j = j + 1
+        ref_res.extend(reference[0:max_i - max_num])
+        ref_res.extend(reference[max_i:])
+        can_res.extend(candidate[0:max_j - max_num])
+        can_res.extend(candidate[max_j:])
+
+        return eq_flag, ref_res, can_res
+
+
+def equal(reference: Contour, candidate: Contour, strip: bool = True, space_remove: bool = True,
+          coordinate_eq: bool = False) -> bool:
+    if strip:
+        reference.text = reference.text.strip()
+        candidate.text = candidate.text.strip()
+    if space_remove:
+        reference.text = reference.text.replace(' ', '')
+        candidate.text = candidate.text.replace(' ', '')
+    if coordinate_eq:
+        if reference.x != candidate.x or reference.y != candidate.y or reference.width != candidate.width or reference.height != candidate.height:
+            return False
+    if reference.text == candidate.text:
+        return True
+    else:
+        return False
+
 
 def make_text(words):
     """Return text string output of get_text("words").
     Word items are sorted for reading sequence left to right,
     top to bottom.
     """
     line_dict = {}  # key: vertical coordinate, value: list of words
```

### Comparing `visual-compare-1.0.1/visual_compare/tests/test_downloader.py` & `visual-compare-1.0.2/visual_compare/tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.1/visual_compare/tests/test_image.py` & `visual-compare-1.0.2/visual_compare/tests/test_image.py`

 * *Files 26% similar despite different names*

```diff
@@ -40,7 +40,23 @@
     def test_parse_mask1(self):
         from visual_compare.doc.image.compare_image import CompareImage
         img = self.get_path('111.pdf')
         img1 = CompareImage(img).opencv_images
         img11 = self.get_path('333.png')
         res = self.cls().parse_mask(img1, img11)
         print(res)
+
+    def test_ocr_image_equal(self):
+        from visual_compare.doc.image.image import OcrImage
+        from visual_compare.doc.models import Contour
+        ct1 = Contour(text='w ア イ ア ル\n', x=1317, y=932, width=30, height=18)
+        ct2 = Contour(text='w アイ アル\n', x=1318, y=933, width=30, height=18)
+        oi = OcrImage(**ct1.dict())
+        assert oi.equal(ct2) is True
+
+    def test_ocr_image_not_equal(self):
+        from visual_compare.doc.image.image import OcrImage
+        from visual_compare.doc.models import Contour
+        ct1 = Contour(text='w ア イ ア ル\n', x=1317, y=932, width=30, height=18)
+        ct2 = Contour(text='w アイ アル\n', x=1318, y=933, width=30, height=18)
+        oi = OcrImage(**ct1.dict())
+        assert oi.equal(ct2, coordinate_eq=True) is False
```

### Comparing `visual-compare-1.0.1/visual_compare/tests/test_ocr.py` & `visual-compare-1.0.2/visual_compare/tests/test_ocr.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,17 +8,19 @@
    date：           2023/5/12
 -------------------------------------------------
    Change Activity:
                     2023/5/12
 -------------------------------------------------
 """
 import cv2
+import numpy
 from pytesseract import pytesseract
 
 from visual_compare.doc.image.compare_image import CompareImage
+from visual_compare.doc.image.ocr import EastTextExtractor
 
 
 class TestOcr:
 
     def setup(self):
         # from visual_compare.doc.visual_test import VisualTest
         # self.cls = VisualTest
@@ -60,23 +62,48 @@
              'conf': conf_list})
         print(text_content)
 
     def test_torch(self):
         import torch
         pth_file = r'C:\Users\dingyong.cui\.EasyOCR\model\japanese_g2.pth'
         net = torch.load(pth_file, map_location=torch.device('cpu'))
-        print(net['model'])
         for k, v in dict(net).items():
             print(k)
             print(v)
 
     def test_x(self):
         import easyocr
-        img1 = self.get_path('1.jpg')
+        # img1 = self.get_path('1.jpg')
+        img1 = self.get_path('y11.png')
+        img2 = self.get_path('y11.png')
         img_np = cv2.imread(img1)
         img_gray = cv2.cvtColor(img_np, cv2.COLOR_BGR2GRAY)
         # 阈值二进制 - > 127 设置为255(白)，否则0(黑) -> 淡白得更白,淡黑更黑
-        _, img_thresh = cv2.threshold(img_gray, 170, 255, cv2.THRESH_BINARY)
-        # 图像 OCR 识别
-        reader = easyocr.Reader(['ja', 'en'], detector=True, recognizer=True)
-        text = reader.readtext(img_thresh, detail=0, batch_size=1, paragraph=True)
-        print(text)
+        _, img_thresh = cv2.threshold(img_gray, 127, 255, cv2.THRESH_BINARY | cv2.THRESH_OTSU)
+
+        # img = cv2.rectangle(img_np, (20, 8), (96, 36), (0, 0, 255), 4)
+        # cv2.imshow('test', img)
+        # cv2.waitKey(0)
+
+        # 图像 OCR 识别 paragraph-是否返回匹配度
+        # reader = easyocr.Reader(['en', 'ja'], detector=True, recognizer=True)
+        reader = easyocr.Reader(['en', 'ja'], detector=True, recognizer=True)
+        text1 = reader.readtext(img_thresh, detail=1, batch_size=1, paragraph=False, contrast_ths=0.5,
+                                adjust_contrast=0.8)
+
+        img_np2 = cv2.imread(img2)
+        img_gray2 = cv2.cvtColor(img_np2, cv2.COLOR_BGR2GRAY)
+        # 阈值二进制 - > 127 设置为255(白)，否则0(黑) -> 淡白得更白,淡黑更黑
+        _, img_thresh2 = cv2.threshold(img_gray2, 170, 255, cv2.THRESH_BINARY | cv2.THRESH_OTSU)
+        text2 = reader.readtext(img_thresh2, detail=1, batch_size=1, paragraph=True)
+        print(text1)
+        print(text2)
+
+    def test_1(self):
+        img1 = self.get_path('y11.png')
+        oi = CompareImage(img1).opencv_images[0]
+        x = EastTextExtractor().get_image_text_and_coordinate(oi)
+        print(x)
+
+    def test_0(self):
+        cnt = numpy.array([[53, 89], [281, 89], [281, 109], [53, 109]])
+        cv2.boundingRect(cnt)
```

### Comparing `visual-compare-1.0.1/visual_compare/tests/test_paddle.py` & `visual-compare-1.0.2/visual_compare/tests/test_paddle.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.1/visual_compare/tests/test_pdf.py` & `visual-compare-1.0.2/visual_compare/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.1/visual_compare/tests/test_torch.py` & `visual-compare-1.0.2/visual_compare/tests/test_torch.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.1/visual_compare/tests/test_visual.py` & `visual-compare-1.0.2/visual_compare/tests/test_visual.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,27 +19,14 @@
         from visual_compare.doc.visual import Visual
         self.cls = Visual
         self.image_base = '../../files/images/'
 
     def get_path(self, filename):
         return self.image_base + filename
 
-    def test_check_exist(self):
-        img1 = self.get_path('123.png')
-        img11 = self.get_path('000.png')
-        self.cls().check_exist([img1, img11])
-
-    def test_check_exist_fail(self):
-        img1 = self.get_path('123.png')
-        img11 = self.get_path('00000.png')
-        try:
-            self.cls().check_exist([img1, img11])
-        except AssertionError as e:
-            print(e)
-
     def test_generate_mask(self):
         reference_image = self.get_path('123.png')
         mask_images = self.get_path('000.png')
         res = self.cls().generate_mask(reference_image, mask_images)
         print(res)
 
     def test_generate_mask_pages(self):
@@ -61,7 +48,33 @@
         mask_images = self.get_path('000.png')
         img2 = self.get_path('124.png')
         cls = self.cls()
         mask = cls.generate_mask(img1, mask_images)
         is_diff, res = cls.compare_images(img1, img2, mask=mask)
         print(res)
         assert is_diff is True
+
+    def test_compare_images_with_mask1(self):
+        img1 = self.get_path('008.jpg')
+        mask_images = self.get_path('007.png')
+        img2 = self.get_path('009.jpg')
+        cls = self.cls()
+        mask = cls.generate_mask(img1, mask_images)
+        is_diff, res = cls.compare_images(img1, img2, mask=mask)
+        print(res)
+        assert is_diff is True
+
+    def test_compare_images_with_force_ocr(self):
+        img1 = self.get_path('y1.png')
+        img2 = self.get_path('y2.png')
+        cls = self.cls()
+        is_diff, res = cls.compare_images(img1, img2, force_ocr=True, lang=['ja', 'en'])
+        print(res)
+        assert is_diff is True
+
+    def test_compare_images_with_force_ocr_and_ch(self):
+        img1 = self.get_path('123.png')
+        img2 = self.get_path('124.png')
+        cls = self.cls()
+        is_diff, res = cls.compare_images(img1, img2, force_ocr=True, lang=['ch_sim', 'en'])
+        print(res)
+        assert is_diff is True
```

### Comparing `visual-compare-1.0.1/visual_compare/utils/common.py` & `visual-compare-1.0.2/visual_compare/utils/common.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.1/visual_compare/utils/downloader.py` & `visual-compare-1.0.2/visual_compare/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.1/visual_compare.egg-info/PKG-INFO` & `visual-compare-1.0.2/visual_compare.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visual-compare
-Version: 1.0.1
+Version: 1.0.2
 Summary: Image and PDF Compare
 Home-page: https://github.com/cuidingyong/visual-compare
 Author: Dillon
 Author-email: cuidingyong@yeah.net
 License: MIT
 Keywords: visual compare image pdf diff
 Platform: UNKNOWN
@@ -71,7 +71,28 @@
 assert is_diff is True
 ```
 
  Result as follows
 
 ![2.jpg](https://github.com/cuidingyong/visual-compare/raw/main/files/result/2.jpg)
 
+### Compare images with OCR ###
+
+```python
+from visual_compare.doc.visual import Visual
+
+def get_path(filename):
+    image_base = '../../files/images/'
+    return image_base + filename
+
+reference_image = get_path('123.png')
+test_image = get_path('124.png')
+vt = Visual()
+is_diff, res = vt.compare_images(reference_image, test_image, force_ocr=True, lang=['ch_sim', 'en'])
+print(res)
+assert is_diff is True
+```
+
+ Result as follows
+
+![3.jpg](https://github.com/cuidingyong/visual-compare/raw/main/files/result/3.jpg)
+
```

### Comparing `visual-compare-1.0.1/visual_compare.egg-info/SOURCES.txt` & `visual-compare-1.0.2/visual_compare.egg-info/SOURCES.txt`

 * *Files identical despite different names*

