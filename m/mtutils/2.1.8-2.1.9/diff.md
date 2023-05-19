# Comparing `tmp/mtutils-2.1.8.tar.gz` & `tmp/mtutils-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mtutils-2.1.8.tar", last modified: Thu Jul 14 07:37:57 2022, max compression
+gzip compressed data, was "dist\mtutils-2.1.9.tar", last modified: Thu Jul 14 08:06:49 2022, max compression
```

## Comparing `mtutils-2.1.8.tar` & `mtutils-2.1.9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxrwx   0        0        0        0 2022-07-14 07:37:57.265512 mtutils-2.1.8/
--rw-rw-rw-   0        0        0      240 2022-07-14 07:37:57.265512 mtutils-2.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-07-14 07:37:57.214648 mtutils-2.1.8/mtutils/
--rw-rw-rw-   0        0        0       52 2022-06-17 06:57:37.000000 mtutils-2.1.8/mtutils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-14 07:37:57.220632 mtutils-2.1.8/mtutils/assets/
--rw-rw-rw-   0        0        0        0 2022-07-11 03:40:27.000000 mtutils-2.1.8/mtutils/assets/__init__.py
--rw-rw-rw-   0        0        0     4946 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/assets/color_list.py
--rw-rw-rw-   0        0        0    67701 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/assets/det.json
-drwxrwxrwx   0        0        0        0 2022-07-14 07:37:57.221629 mtutils-2.1.8/mtutils/assets/evaluator/
--rw-rw-rw-   0        0        0        0 2022-06-17 06:40:45.000000 mtutils-2.1.8/mtutils/assets/evaluator/__init__.py
--rw-rw-rw-   0        0        0     9331 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/assets/everytime3p.jpg
--rw-rw-rw-   0        0        0     6924 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/assets/mc.json
--rw-rw-rw-   0        0        0     7917 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/assets/ml.json
-drwxrwxrwx   0        0        0        0 2022-07-14 07:37:57.221629 mtutils-2.1.8/mtutils/lib/
--rw-rw-rw-   0        0        0      330 2022-06-17 07:31:58.000000 mtutils-2.1.8/mtutils/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-14 07:37:57.226643 mtutils-2.1.8/mtutils/lib/data/
--rw-rw-rw-   0        0        0       97 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/lib/data/__init__.py
--rw-rw-rw-   0        0        0    19650 2022-07-13 10:14:38.000000 mtutils-2.1.8/mtutils/lib/data/base.py
--rw-rw-rw-   0        0        0     3252 2022-06-14 01:41:22.000000 mtutils-2.1.8/mtutils/lib/data/class_mapper.py
--rw-rw-rw-   0        0        0    12093 2022-06-13 06:02:47.000000 mtutils-2.1.8/mtutils/lib/data/format.py
--rw-rw-rw-   0        0        0     6896 2022-06-14 01:41:22.000000 mtutils-2.1.8/mtutils/lib/data/info.py
--rw-rw-rw-   0        0        0     3676 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/lib/data/saver.py
-drwxrwxrwx   0        0        0        0 2022-07-14 07:37:57.231627 mtutils-2.1.8/mtutils/lib/evaluator/
--rw-rw-rw-   0        0        0      230 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/lib/evaluator/__init__.py
--rw-rw-rw-   0        0        0     7205 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/lib/evaluator/base.py
--rw-rw-rw-   0        0        0    14287 2022-06-17 06:40:45.000000 mtutils-2.1.8/mtutils/lib/evaluator/detection.py
--rw-rw-rw-   0        0        0     2187 2022-06-23 08:24:31.000000 mtutils-2.1.8/mtutils/lib/evaluator/multi_class.py
--rw-rw-rw-   0        0        0    13941 2022-06-17 06:40:45.000000 mtutils-2.1.8/mtutils/lib/evaluator/multi_label.py
-drwxrwxrwx   0        0        0        0 2022-07-14 07:37:57.235619 mtutils-2.1.8/mtutils/lib/labelme/
--rw-rw-rw-   0        0        0       82 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/lib/labelme/__init__.py
--rw-rw-rw-   0        0        0     3051 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/lib/labelme/labelme.py
--rw-rw-rw-   0        0        0      614 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/lib/labelme/main.py
--rw-rw-rw-   0        0        0     3040 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/lib/labelme/polygon.py
--rw-rw-rw-   0        0        0     1191 2022-06-17 06:40:45.000000 mtutils-2.1.8/mtutils/lib/labelme/utils.py
-drwxrwxrwx   0        0        0        0 2022-07-14 07:37:57.241604 mtutils-2.1.8/mtutils/lib/processing/
--rw-rw-rw-   0        0        0      225 2022-06-17 06:40:45.000000 mtutils-2.1.8/mtutils/lib/processing/__init__.py
--rw-rw-rw-   0        0        0     4742 2022-06-17 06:40:45.000000 mtutils-2.1.8/mtutils/lib/processing/array_processing.py
--rw-rw-rw-   0        0        0     8211 2022-06-17 06:40:45.000000 mtutils-2.1.8/mtutils/lib/processing/box_processing.py
--rw-rw-rw-   0        0        0    11906 2022-06-17 06:40:45.000000 mtutils-2.1.8/mtutils/lib/processing/circle_processing.py
--rw-rw-rw-   0        0        0    44238 2022-07-11 05:56:15.000000 mtutils-2.1.8/mtutils/lib/processing/image_processing.py
--rw-rw-rw-   0        0        0     3721 2022-06-17 06:40:45.000000 mtutils-2.1.8/mtutils/lib/processing/math_processing.py
--rw-rw-rw-   0        0        0     6131 2022-07-14 07:37:36.000000 mtutils-2.1.8/mtutils/lib/processing/multi_processing.py
--rw-rw-rw-   0        0        0      389 2022-06-17 06:40:45.000000 mtutils-2.1.8/mtutils/lib/processing/net_processing.py
-drwxrwxrwx   0        0        0        0 2022-07-14 07:37:57.249555 mtutils-2.1.8/mtutils/lib/utils/
--rw-rw-rw-   0        0        0      439 2022-06-17 06:40:45.000000 mtutils-2.1.8/mtutils/lib/utils/__init__.py
--rw-rw-rw-   0        0        0     2204 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/lib/utils/add_utils.py
-drwxrwxrwx   0        0        0        0 2022-07-14 07:37:57.254541 mtutils-2.1.8/mtutils/lib/utils/classifier_eval/
--rw-rw-rw-   0        0        0       98 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/lib/utils/classifier_eval/__init__.py
--rw-rw-rw-   0        0        0    33004 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/lib/utils/classifier_eval/eval_metrics.py
--rw-rw-rw-   0        0        0     4463 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/lib/utils/classifier_eval/example.py
--rw-rw-rw-   0        0        0     3104 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/lib/utils/classifier_eval/plot_confusion_matrix.py
--rw-rw-rw-   0        0        0     2852 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/lib/utils/classifier_eval/tmp_file.py
--rw-rw-rw-   0        0        0     1121 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/lib/utils/classifier_eval/utils.py
--rw-rw-rw-   0        0        0     2220 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/lib/utils/coding_related.py
--rw-rw-rw-   0        0        0     1490 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/lib/utils/eva_utils.py
--rw-rw-rw-   0        0        0      657 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/lib/utils/id_related.py
--rw-rw-rw-   0        0        0    18973 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/lib/utils/mean_ap.py
--rw-rw-rw-   0        0        0     1330 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/lib/utils/path_related.py
--rw-rw-rw-   0        0        0     1320 2022-06-13 01:26:21.000000 mtutils-2.1.8/mtutils/lib/utils/torch_utils.py
--rw-rw-rw-   0        0        0    46941 2022-07-13 08:48:56.000000 mtutils-2.1.8/mtutils/lib/utils/utils.py
--rw-rw-rw-   0        0        0      169 2022-06-17 07:11:18.000000 mtutils-2.1.8/mtutils/mttest.py
-drwxrwxrwx   0        0        0        0 2022-07-14 07:37:57.254541 mtutils-2.1.8/mtutils/tests/
--rw-rw-rw-   0        0        0        0 2022-06-17 06:40:45.000000 mtutils-2.1.8/mtutils/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-14 07:37:57.256561 mtutils-2.1.8/mtutils/tests/test_data/
--rw-rw-rw-   0        0        0        0 2022-06-17 06:40:45.000000 mtutils-2.1.8/mtutils/tests/test_data/__init__.py
--rw-rw-rw-   0        0        0     6193 2022-06-17 07:09:18.000000 mtutils-2.1.8/mtutils/tests/test_data/test_data.py
-drwxrwxrwx   0        0        0        0 2022-07-14 07:37:57.257557 mtutils-2.1.8/mtutils/tests/test_utils/
--rw-rw-rw-   0        0        0        0 2022-06-17 06:40:45.000000 mtutils-2.1.8/mtutils/tests/test_utils/__init__.py
--rw-rw-rw-   0        0        0    14186 2022-06-17 07:09:11.000000 mtutils-2.1.8/mtutils/tests/test_utils/test_utils.py
-drwxrwxrwx   0        0        0        0 2022-07-14 07:37:57.263521 mtutils-2.1.8/mtutils.egg-info/
--rw-rw-rw-   0        0        0      240 2022-07-14 07:37:56.000000 mtutils-2.1.8/mtutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2124 2022-07-14 07:37:56.000000 mtutils-2.1.8/mtutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-14 07:37:56.000000 mtutils-2.1.8/mtutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-07-14 07:37:56.000000 mtutils-2.1.8/mtutils.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       50 2022-07-14 07:37:56.000000 mtutils-2.1.8/mtutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-07-14 07:37:56.000000 mtutils-2.1.8/mtutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-07-14 07:37:57.265512 mtutils-2.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1273 2022-07-14 07:37:54.000000 mtutils-2.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-07-14 08:06:49.552017 mtutils-2.1.9/
+-rw-rw-rw-   0        0        0      240 2022-07-14 08:06:49.551043 mtutils-2.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-07-14 08:06:49.513490 mtutils-2.1.9/mtutils/
+-rw-rw-rw-   0        0        0       52 2022-06-17 06:57:37.000000 mtutils-2.1.9/mtutils/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-14 08:06:49.516804 mtutils-2.1.9/mtutils/assets/
+-rw-rw-rw-   0        0        0        0 2022-07-11 03:40:27.000000 mtutils-2.1.9/mtutils/assets/__init__.py
+-rw-rw-rw-   0        0        0     4946 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/assets/color_list.py
+-rw-rw-rw-   0        0        0    67701 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/assets/det.json
+drwxrwxrwx   0        0        0        0 2022-07-14 08:06:49.517801 mtutils-2.1.9/mtutils/assets/evaluator/
+-rw-rw-rw-   0        0        0        0 2022-06-17 06:40:45.000000 mtutils-2.1.9/mtutils/assets/evaluator/__init__.py
+-rw-rw-rw-   0        0        0     9331 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/assets/everytime3p.jpg
+-rw-rw-rw-   0        0        0     6924 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/assets/mc.json
+-rw-rw-rw-   0        0        0     7917 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/assets/ml.json
+drwxrwxrwx   0        0        0        0 2022-07-14 08:06:49.518799 mtutils-2.1.9/mtutils/lib/
+-rw-rw-rw-   0        0        0      330 2022-06-17 07:31:58.000000 mtutils-2.1.9/mtutils/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-14 08:06:49.521791 mtutils-2.1.9/mtutils/lib/data/
+-rw-rw-rw-   0        0        0       97 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/lib/data/__init__.py
+-rw-rw-rw-   0        0        0    19650 2022-07-13 10:14:38.000000 mtutils-2.1.9/mtutils/lib/data/base.py
+-rw-rw-rw-   0        0        0     3252 2022-06-14 01:41:22.000000 mtutils-2.1.9/mtutils/lib/data/class_mapper.py
+-rw-rw-rw-   0        0        0    12093 2022-06-13 06:02:47.000000 mtutils-2.1.9/mtutils/lib/data/format.py
+-rw-rw-rw-   0        0        0     6896 2022-06-14 01:41:22.000000 mtutils-2.1.9/mtutils/lib/data/info.py
+-rw-rw-rw-   0        0        0     3676 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/lib/data/saver.py
+drwxrwxrwx   0        0        0        0 2022-07-14 08:06:49.524902 mtutils-2.1.9/mtutils/lib/evaluator/
+-rw-rw-rw-   0        0        0      230 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/lib/evaluator/__init__.py
+-rw-rw-rw-   0        0        0     7205 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/lib/evaluator/base.py
+-rw-rw-rw-   0        0        0    14287 2022-06-17 06:40:45.000000 mtutils-2.1.9/mtutils/lib/evaluator/detection.py
+-rw-rw-rw-   0        0        0     2187 2022-06-23 08:24:31.000000 mtutils-2.1.9/mtutils/lib/evaluator/multi_class.py
+-rw-rw-rw-   0        0        0    13941 2022-06-17 06:40:45.000000 mtutils-2.1.9/mtutils/lib/evaluator/multi_label.py
+drwxrwxrwx   0        0        0        0 2022-07-14 08:06:49.527918 mtutils-2.1.9/mtutils/lib/labelme/
+-rw-rw-rw-   0        0        0       82 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/lib/labelme/__init__.py
+-rw-rw-rw-   0        0        0     3051 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/lib/labelme/labelme.py
+-rw-rw-rw-   0        0        0      614 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/lib/labelme/main.py
+-rw-rw-rw-   0        0        0     3040 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/lib/labelme/polygon.py
+-rw-rw-rw-   0        0        0     1191 2022-06-17 06:40:45.000000 mtutils-2.1.9/mtutils/lib/labelme/utils.py
+drwxrwxrwx   0        0        0        0 2022-07-14 08:06:49.534899 mtutils-2.1.9/mtutils/lib/processing/
+-rw-rw-rw-   0        0        0      225 2022-06-17 06:40:45.000000 mtutils-2.1.9/mtutils/lib/processing/__init__.py
+-rw-rw-rw-   0        0        0     4742 2022-06-17 06:40:45.000000 mtutils-2.1.9/mtutils/lib/processing/array_processing.py
+-rw-rw-rw-   0        0        0     8211 2022-06-17 06:40:45.000000 mtutils-2.1.9/mtutils/lib/processing/box_processing.py
+-rw-rw-rw-   0        0        0    11906 2022-06-17 06:40:45.000000 mtutils-2.1.9/mtutils/lib/processing/circle_processing.py
+-rw-rw-rw-   0        0        0    44238 2022-07-11 05:56:15.000000 mtutils-2.1.9/mtutils/lib/processing/image_processing.py
+-rw-rw-rw-   0        0        0     3721 2022-06-17 06:40:45.000000 mtutils-2.1.9/mtutils/lib/processing/math_processing.py
+-rw-rw-rw-   0        0        0     6188 2022-07-14 08:02:36.000000 mtutils-2.1.9/mtutils/lib/processing/multi_processing.py
+-rw-rw-rw-   0        0        0      389 2022-06-17 06:40:45.000000 mtutils-2.1.9/mtutils/lib/processing/net_processing.py
+drwxrwxrwx   0        0        0        0 2022-07-14 08:06:49.539886 mtutils-2.1.9/mtutils/lib/utils/
+-rw-rw-rw-   0        0        0      439 2022-06-17 06:40:45.000000 mtutils-2.1.9/mtutils/lib/utils/__init__.py
+-rw-rw-rw-   0        0        0     2204 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/lib/utils/add_utils.py
+drwxrwxrwx   0        0        0        0 2022-07-14 08:06:49.544038 mtutils-2.1.9/mtutils/lib/utils/classifier_eval/
+-rw-rw-rw-   0        0        0       98 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/lib/utils/classifier_eval/__init__.py
+-rw-rw-rw-   0        0        0    33004 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/lib/utils/classifier_eval/eval_metrics.py
+-rw-rw-rw-   0        0        0     4463 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/lib/utils/classifier_eval/example.py
+-rw-rw-rw-   0        0        0     3104 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/lib/utils/classifier_eval/plot_confusion_matrix.py
+-rw-rw-rw-   0        0        0     2852 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/lib/utils/classifier_eval/tmp_file.py
+-rw-rw-rw-   0        0        0     1121 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/lib/utils/classifier_eval/utils.py
+-rw-rw-rw-   0        0        0     2220 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/lib/utils/coding_related.py
+-rw-rw-rw-   0        0        0     1490 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/lib/utils/eva_utils.py
+-rw-rw-rw-   0        0        0      657 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/lib/utils/id_related.py
+-rw-rw-rw-   0        0        0    18973 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/lib/utils/mean_ap.py
+-rw-rw-rw-   0        0        0     1330 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/lib/utils/path_related.py
+-rw-rw-rw-   0        0        0     1320 2022-06-13 01:26:21.000000 mtutils-2.1.9/mtutils/lib/utils/torch_utils.py
+-rw-rw-rw-   0        0        0    46941 2022-07-13 08:48:56.000000 mtutils-2.1.9/mtutils/lib/utils/utils.py
+-rw-rw-rw-   0        0        0      169 2022-06-17 07:11:18.000000 mtutils-2.1.9/mtutils/mttest.py
+drwxrwxrwx   0        0        0        0 2022-07-14 08:06:49.544038 mtutils-2.1.9/mtutils/tests/
+-rw-rw-rw-   0        0        0        0 2022-06-17 06:40:45.000000 mtutils-2.1.9/mtutils/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-14 08:06:49.545059 mtutils-2.1.9/mtutils/tests/test_data/
+-rw-rw-rw-   0        0        0        0 2022-06-17 06:40:45.000000 mtutils-2.1.9/mtutils/tests/test_data/__init__.py
+-rw-rw-rw-   0        0        0     6193 2022-06-17 07:09:18.000000 mtutils-2.1.9/mtutils/tests/test_data/test_data.py
+drwxrwxrwx   0        0        0        0 2022-07-14 08:06:49.546057 mtutils-2.1.9/mtutils/tests/test_utils/
+-rw-rw-rw-   0        0        0        0 2022-06-17 06:40:45.000000 mtutils-2.1.9/mtutils/tests/test_utils/__init__.py
+-rw-rw-rw-   0        0        0    14186 2022-06-17 07:09:11.000000 mtutils-2.1.9/mtutils/tests/test_utils/test_utils.py
+drwxrwxrwx   0        0        0        0 2022-07-14 08:06:49.550047 mtutils-2.1.9/mtutils.egg-info/
+-rw-rw-rw-   0        0        0      240 2022-07-14 08:06:49.000000 mtutils-2.1.9/mtutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2124 2022-07-14 08:06:49.000000 mtutils-2.1.9/mtutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-07-14 08:06:49.000000 mtutils-2.1.9/mtutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-07-14 08:06:49.000000 mtutils-2.1.9/mtutils.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       50 2022-07-14 08:06:49.000000 mtutils-2.1.9/mtutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2022-07-14 08:06:49.000000 mtutils-2.1.9/mtutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-07-14 08:06:49.552017 mtutils-2.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1273 2022-07-14 08:06:48.000000 mtutils-2.1.9/setup.py
```

### Comparing `mtutils-2.1.8/mtutils/assets/color_list.py` & `mtutils-2.1.9/mtutils/assets/color_list.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/assets/det.json` & `mtutils-2.1.9/mtutils/assets/det.json`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/assets/everytime3p.jpg` & `mtutils-2.1.9/mtutils/assets/everytime3p.jpg`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/assets/mc.json` & `mtutils-2.1.9/mtutils/assets/mc.json`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/assets/ml.json` & `mtutils-2.1.9/mtutils/assets/ml.json`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/data/base.py` & `mtutils-2.1.9/mtutils/lib/data/base.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/data/class_mapper.py` & `mtutils-2.1.9/mtutils/lib/data/class_mapper.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/data/format.py` & `mtutils-2.1.9/mtutils/lib/data/format.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/data/info.py` & `mtutils-2.1.9/mtutils/lib/data/info.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/data/saver.py` & `mtutils-2.1.9/mtutils/lib/data/saver.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/evaluator/base.py` & `mtutils-2.1.9/mtutils/lib/evaluator/base.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/evaluator/detection.py` & `mtutils-2.1.9/mtutils/lib/evaluator/detection.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/evaluator/multi_class.py` & `mtutils-2.1.9/mtutils/lib/evaluator/multi_class.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/evaluator/multi_label.py` & `mtutils-2.1.9/mtutils/lib/evaluator/multi_label.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/labelme/labelme.py` & `mtutils-2.1.9/mtutils/lib/labelme/labelme.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/labelme/main.py` & `mtutils-2.1.9/mtutils/lib/labelme/main.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/labelme/polygon.py` & `mtutils-2.1.9/mtutils/lib/labelme/polygon.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/labelme/utils.py` & `mtutils-2.1.9/mtutils/lib/labelme/utils.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/processing/array_processing.py` & `mtutils-2.1.9/mtutils/lib/processing/array_processing.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/processing/box_processing.py` & `mtutils-2.1.9/mtutils/lib/processing/box_processing.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/processing/circle_processing.py` & `mtutils-2.1.9/mtutils/lib/processing/circle_processing.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/processing/image_processing.py` & `mtutils-2.1.9/mtutils/lib/processing/image_processing.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/processing/math_processing.py` & `mtutils-2.1.9/mtutils/lib/processing/math_processing.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/processing/multi_processing.py` & `mtutils-2.1.9/mtutils/lib/processing/multi_processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,33 +28,37 @@
 
     print(f"{len(share_list)} / {total_size}")
     
     min_time = (time.time() - start_time) / max(1, len(share_list)) * (total_size - max(1, len(share_list))) / 60
     print(f"time passed: {(time.time() - start_time)/ 60} min      time left: {min_time} min")
 
 
-def multi_process(main_fun, para_fun=None, total_size=None, max_pool_num=8, catch_exception=True, method=None, data=None):
+def multi_process(main_fun, para_fun, total_size=None, max_pool_num=8, catch_exception=True, method=None):
     """_summary_
 
     Args:
         main_fun (func): main function
         para_fun (func): fun(id) is the input data
         total_size (int): total number of inputs
         max_pool_num (int, optional): worker number. Defaults to 8.
         catch_exception (bool, optional): if True, a try-except will be applied. Defaults to True.
         method (str, optional): method to setup multiprocessing, could be one of ['spawn', 'fork', 'forkserver']. Defaults to None.
         data(list): data to be handled
 
     Returns:
         _type_: _description_
     """
-    if para_fun is None and data is not None:
+    
+
+    if hasattr(para_fun, '__getitem__') and hasattr(para_fun, '__len__'):
+        # is data
+        if total_size is None:
+            total_size = len(para_fun)
+        data = para_fun
         para_fun = lambda idx: data[idx]
-    if total_size is None and data is not None:
-        total_size = len(data)
 
     if method is not None:
         multiprocessing.set_start_method(method, force=True)
         # multiprocessing.set_start_method('spawn')
     print(f"Current Multiprocessing Method: {multiprocessing.get_start_method()}")
 
     start_time = time.time()
@@ -65,14 +69,15 @@
         pool = Pool(max_pool_num)
         for index in range(total_size):
             paras = para_fun(index)
             pool.apply_async(func=single_process, args=(main_fun, paras, share_list, share_lock, total_size, start_time, catch_exception))
         pool.close()
         pool.join()
         result_list = list(share_list)
+
     else:
         result_list = list()
         for index in tqdm(range(total_size)):
             res = main_fun(para_fun(index))
             result_list.append(res)
     print(f"total time: {(time.time() - start_time) / 60} min     mean time {(time.time() - start_time) / max(1, len(result_list))} s")
     return result_list
```

### Comparing `mtutils-2.1.8/mtutils/lib/utils/add_utils.py` & `mtutils-2.1.9/mtutils/lib/utils/add_utils.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/utils/classifier_eval/eval_metrics.py` & `mtutils-2.1.9/mtutils/lib/utils/classifier_eval/eval_metrics.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/utils/classifier_eval/example.py` & `mtutils-2.1.9/mtutils/lib/utils/classifier_eval/example.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/utils/classifier_eval/plot_confusion_matrix.py` & `mtutils-2.1.9/mtutils/lib/utils/classifier_eval/plot_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/utils/classifier_eval/tmp_file.py` & `mtutils-2.1.9/mtutils/lib/utils/classifier_eval/tmp_file.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/utils/classifier_eval/utils.py` & `mtutils-2.1.9/mtutils/lib/utils/classifier_eval/utils.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/utils/coding_related.py` & `mtutils-2.1.9/mtutils/lib/utils/coding_related.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/utils/eva_utils.py` & `mtutils-2.1.9/mtutils/lib/utils/eva_utils.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/utils/id_related.py` & `mtutils-2.1.9/mtutils/lib/utils/id_related.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/utils/mean_ap.py` & `mtutils-2.1.9/mtutils/lib/utils/mean_ap.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/utils/path_related.py` & `mtutils-2.1.9/mtutils/lib/utils/path_related.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/utils/torch_utils.py` & `mtutils-2.1.9/mtutils/lib/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/lib/utils/utils.py` & `mtutils-2.1.9/mtutils/lib/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/tests/test_data/test_data.py` & `mtutils-2.1.9/mtutils/tests/test_data/test_data.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils/tests/test_utils/test_utils.py` & `mtutils-2.1.9/mtutils/tests/test_utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/mtutils.egg-info/SOURCES.txt` & `mtutils-2.1.9/mtutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mtutils-2.1.8/setup.py` & `mtutils-2.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import setuptools
 from setuptools import find_packages, setup
 from numpy.distutils.core import setup
 from numpy.distutils.misc_util import Configuration
 from os.path import join, dirname, realpath
 
-str_version = '2.1.8'
+str_version = '2.1.9'
 
 
 
 def configuration(parent_package='', top_path=''):
     # this will automatically build the scattering extensions, using the
     # setup.py files located in their subdirectories
     config = Configuration(None, parent_package, top_path)
```

