# Comparing `tmp/pyrecdp-1.0.1b202305161.tar.gz` & `tmp/pyrecdp-1.0.1b202305181.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrecdp-1.0.1b202305161.tar", last modified: Tue May 16 22:43:44 2023, max compression
+gzip compressed data, was "pyrecdp-1.0.1b202305181.tar", last modified: Fri May 19 16:51:25 2023, max compression
```

## Comparing `pyrecdp-1.0.1b202305161.tar` & `pyrecdp-1.0.1b202305181.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:43:44.478421 pyrecdp-1.0.1b202305161/
--rw-r--r--   0 root         (0) root         (0)    94051 2023-05-05 19:05:00.000000 pyrecdp-1.0.1b202305161/LICENSE
--rw-r--r--   0 root         (0) root         (0)      189 2023-05-05 19:05:00.000000 pyrecdp-1.0.1b202305161/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8860 2023-05-16 22:43:44.478421 pyrecdp-1.0.1b202305161/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8315 2023-05-05 19:05:00.000000 pyrecdp-1.0.1b202305161/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:43:44.470421 pyrecdp-1.0.1b202305161/ScalaProcessUtils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:00.000000 pyrecdp-1.0.1b202305161/ScalaProcessUtils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:43:44.470421 pyrecdp-1.0.1b202305161/pyrecdp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:43:44.470421 pyrecdp-1.0.1b202305161/pyrecdp/ScalaProcessUtils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/ScalaProcessUtils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/ScalaProcessUtils/spark-defaults.conf
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/ScalaProcessUtils/spark-env.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:43:44.470421 pyrecdp-1.0.1b202305161/pyrecdp/ScalaProcessUtils/target/
--rw-r--r--   0 root         (0) root         (0)   114879 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar
--rw-r--r--   0 root         (0) root         (0)     1001 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:43:44.474421 pyrecdp-1.0.1b202305161/pyrecdp/autofe/
--rw-r--r--   0 root         (0) root         (0)     3070 2023-05-16 21:58:12.000000 pyrecdp-1.0.1b202305161/pyrecdp/autofe/AutoFE.py
--rw-r--r--   0 root         (0) root         (0)    13396 2023-05-15 23:17:43.000000 pyrecdp-1.0.1b202305161/pyrecdp/autofe/BasePipeline.py
--rw-r--r--   0 root         (0) root         (0)     4459 2023-05-15 23:17:43.000000 pyrecdp-1.0.1b202305161/pyrecdp/autofe/FeatureEstimator.py
--rw-r--r--   0 root         (0) root         (0)     3106 2023-05-15 23:17:43.000000 pyrecdp-1.0.1b202305161/pyrecdp/autofe/FeatureProfiler.py
--rw-r--r--   0 root         (0) root         (0)     2915 2023-05-08 20:26:24.000000 pyrecdp-1.0.1b202305161/pyrecdp/autofe/FeatureWrangler.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-08 21:49:59.000000 pyrecdp-1.0.1b202305161/pyrecdp/autofe/RelationalBuilder.py
--rw-r--r--   0 root         (0) root         (0)      218 2023-05-08 21:21:08.000000 pyrecdp-1.0.1b202305161/pyrecdp/autofe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:43:44.474421 pyrecdp-1.0.1b202305161/pyrecdp/core/
--rw-r--r--   0 root         (0) root         (0)      186 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1394 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/core/dataframe.py
--rw-r--r--   0 root         (0) root         (0)     2849 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/core/di_graph.py
--rw-r--r--   0 root         (0) root         (0)     5696 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/core/schema.py
--rw-r--r--   0 root         (0) root         (0)     5860 2023-05-12 21:35:22.000000 pyrecdp-1.0.1b202305161/pyrecdp/core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:43:44.474421 pyrecdp-1.0.1b202305161/pyrecdp/datasets/
--rw-r--r--   0 root         (0) root         (0)     2942 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/datasets/CESM_breast_cancer.py
--rw-r--r--   0 root         (0) root         (0)      358 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      680 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/datasets/amazon_product_review.py
--rw-r--r--   0 root         (0) root         (0)     4186 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/datasets/base_api.py
--rw-r--r--   0 root         (0) root         (0)      288 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/datasets/download.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/datasets/ibm_fraud_detect.py
--rw-r--r--   0 root         (0) root         (0)     1208 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/datasets/nyc_taxi.py
--rw-r--r--   0 root         (0) root         (0)      905 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/datasets/outbrain.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/datasets/pretrained.py
--rw-r--r--   0 root         (0) root         (0)      428 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/datasets/twitter_recsys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:43:44.474421 pyrecdp-1.0.1b202305161/pyrecdp/primitives/
--rw-r--r--   0 root         (0) root         (0)       76 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:43:44.474421 pyrecdp-1.0.1b202305161/pyrecdp/primitives/engines/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-01 06:07:04.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/engines/__init__.py
--rw-r--r--   0 root         (0) root         (0)       93 2023-03-01 06:17:33.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/engines/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:43:44.474421 pyrecdp-1.0.1b202305161/pyrecdp/primitives/estimators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/estimators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2091 2023-05-13 22:10:56.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/estimators/base.py
--rw-r--r--   0 root         (0) root         (0)     2656 2023-05-12 20:38:27.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/estimators/lightgbm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:43:44.474421 pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/
--rw-r--r--   0 root         (0) root         (0)     1855 2023-05-13 20:11:42.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/base.py
--rw-r--r--   0 root         (0) root         (0)      269 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/binned.py
--rw-r--r--   0 root         (0) root         (0)     1171 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/category.py
--rw-r--r--   0 root         (0) root         (0)     1620 2023-05-12 03:42:22.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/datetime.py
--rw-r--r--   0 root         (0) root         (0)     1398 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/drop.py
--rw-r--r--   0 root         (0) root         (0)     4047 2023-05-12 20:27:56.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/encode.py
--rw-r--r--   0 root         (0) root         (0)     1221 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/feature_transform.py
--rw-r--r--   0 root         (0) root         (0)     1334 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/featuretools_adaptor.py
--rw-r--r--   0 root         (0) root         (0)     1180 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/fillna.py
--rw-r--r--   0 root         (0) root         (0)     4666 2023-05-12 20:55:11.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/geograph.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-05-13 21:52:17.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/name.py
--rw-r--r--   0 root         (0) root         (0)     3100 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/nlp.py
--rw-r--r--   0 root         (0) root         (0)     4720 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/relation.py
--rw-r--r--   0 root         (0) root         (0)     2975 2023-05-05 19:42:48.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:43:44.474421 pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/
--rw-r--r--   0 root         (0) root         (0)      111 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5810 2023-05-15 23:17:43.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/base.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/category.py
--rw-r--r--   0 root         (0) root         (0)      351 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/custom.py
--rw-r--r--   0 root         (0) root         (0)     1929 2023-05-15 23:17:43.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/data.py
--rw-r--r--   0 root         (0) root         (0)     3291 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/dataframe.py
--rw-r--r--   0 root         (0) root         (0)      758 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/drop.py
--rw-r--r--   0 root         (0) root         (0)     3522 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/encode.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/featuretools_adaptor.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/fillna.py
--rw-r--r--   0 root         (0) root         (0)      682 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/geograph.py
--rw-r--r--   0 root         (0) root         (0)     1376 2023-05-08 22:20:11.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/merge.py
--rw-r--r--   0 root         (0) root         (0)      709 2023-05-09 20:16:39.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/name.py
--rw-r--r--   0 root         (0) root         (0)      712 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/tuple.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-05-09 20:16:35.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:43:44.474421 pyrecdp-1.0.1b202305161/pyrecdp/primitives/profilers/
--rw-r--r--   0 root         (0) root         (0)      157 2023-05-08 18:34:18.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/profilers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5563 2023-05-15 23:17:43.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/profilers/statics.py
--rw-r--r--   0 root         (0) root         (0)     4363 2023-05-12 03:42:15.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/profilers/type_infer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:43:44.474421 pyrecdp-1.0.1b202305161/pyrecdp/primitives/spark_data_processor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/spark_data_processor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54029 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/spark_data_processor/data_processor.py
--rw-r--r--   0 root         (0) root         (0)     8145 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/spark_data_processor/encoder.py
--rw-r--r--   0 root         (0) root         (0)     8115 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/primitives/spark_data_processor/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:43:44.474421 pyrecdp-1.0.1b202305161/pyrecdp/widgets/
--rw-r--r--   0 root         (0) root         (0)     1092 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/widgets/BaseWidget.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/widgets/PlotWidget.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/widgets/ProfilerWidget.py
--rw-r--r--   0 root         (0) root         (0)      821 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/widgets/TabWidget.py
--rw-r--r--   0 root         (0) root         (0)     2103 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/widgets/TableViewWidget.py
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:43:44.478421 pyrecdp-1.0.1b202305161/pyrecdp/widgets/templates/
--rw-r--r--   0 root         (0) root         (0)      989 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/widgets/templates/base.html
--rw-r--r--   0 root         (0) root         (0)       85 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/widgets/templates/error.html
--rw-r--r--   0 root         (0) root         (0)      260 2023-05-11 22:08:36.000000 pyrecdp-1.0.1b202305161/pyrecdp/widgets/templates/interactions.html
--rw-r--r--   0 root         (0) root         (0)     1340 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/widgets/templates/overview.html
--rw-r--r--   0 root         (0) root         (0)     7110 2023-05-15 23:17:43.000000 pyrecdp-1.0.1b202305161/pyrecdp/widgets/templates/scripts.html
--rw-r--r--   0 root         (0) root         (0)    16515 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/widgets/templates/styles.html
--rw-r--r--   0 root         (0) root         (0)     9250 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/widgets/templates/variables.html
--rw-r--r--   0 root         (0) root         (0)      166 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305161/pyrecdp/widgets/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:43:44.470421 pyrecdp-1.0.1b202305161/pyrecdp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8860 2023-05-16 22:43:44.000000 pyrecdp-1.0.1b202305161/pyrecdp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3454 2023-05-16 22:43:44.000000 pyrecdp-1.0.1b202305161/pyrecdp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 22:43:44.000000 pyrecdp-1.0.1b202305161/pyrecdp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-13 19:42:06.000000 pyrecdp-1.0.1b202305161/pyrecdp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      203 2023-05-16 22:43:44.000000 pyrecdp-1.0.1b202305161/pyrecdp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-05-16 22:43:44.000000 pyrecdp-1.0.1b202305161/pyrecdp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-16 22:43:44.478421 pyrecdp-1.0.1b202305161/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1457 2023-05-16 22:43:31.000000 pyrecdp-1.0.1b202305161/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.897554 pyrecdp-1.0.1b202305181/
+-rw-r--r--   0 root         (0) root         (0)    94051 2023-05-05 19:05:00.000000 pyrecdp-1.0.1b202305181/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      189 2023-05-05 19:05:00.000000 pyrecdp-1.0.1b202305181/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10481 2023-05-19 16:51:25.897554 pyrecdp-1.0.1b202305181/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-05-05 19:05:00.000000 pyrecdp-1.0.1b202305181/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.889553 pyrecdp-1.0.1b202305181/ScalaProcessUtils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:00.000000 pyrecdp-1.0.1b202305181/ScalaProcessUtils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.889553 pyrecdp-1.0.1b202305181/pyrecdp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.889553 pyrecdp-1.0.1b202305181/pyrecdp/ScalaProcessUtils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/ScalaProcessUtils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/ScalaProcessUtils/spark-defaults.conf
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/ScalaProcessUtils/spark-env.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.893554 pyrecdp-1.0.1b202305181/pyrecdp/ScalaProcessUtils/target/
+-rw-r--r--   0 root         (0) root         (0)   114879 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.893554 pyrecdp-1.0.1b202305181/pyrecdp/autofe/
+-rw-r--r--   0 root         (0) root         (0)     4010 2023-05-19 16:51:22.000000 pyrecdp-1.0.1b202305181/pyrecdp/autofe/AutoFE.py
+-rw-r--r--   0 root         (0) root         (0)    13436 2023-05-18 19:47:36.000000 pyrecdp-1.0.1b202305181/pyrecdp/autofe/BasePipeline.py
+-rw-r--r--   0 root         (0) root         (0)     4496 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/autofe/FeatureEstimator.py
+-rw-r--r--   0 root         (0) root         (0)     3106 2023-05-15 23:17:43.000000 pyrecdp-1.0.1b202305181/pyrecdp/autofe/FeatureProfiler.py
+-rw-r--r--   0 root         (0) root         (0)     3008 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/autofe/FeatureWrangler.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-08 21:49:59.000000 pyrecdp-1.0.1b202305181/pyrecdp/autofe/RelationalBuilder.py
+-rw-r--r--   0 root         (0) root         (0)      218 2023-05-08 21:21:08.000000 pyrecdp-1.0.1b202305181/pyrecdp/autofe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.893554 pyrecdp-1.0.1b202305181/pyrecdp/core/
+-rw-r--r--   0 root         (0) root         (0)      186 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      742 2023-05-19 16:40:19.000000 pyrecdp-1.0.1b202305181/pyrecdp/core/dataframe.py
+-rw-r--r--   0 root         (0) root         (0)     2849 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/core/di_graph.py
+-rw-r--r--   0 root         (0) root         (0)     5696 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/core/schema.py
+-rw-r--r--   0 root         (0) root         (0)     6420 2023-05-18 19:26:45.000000 pyrecdp-1.0.1b202305181/pyrecdp/core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.893554 pyrecdp-1.0.1b202305181/pyrecdp/datasets/
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/datasets/CESM_breast_cancer.py
+-rw-r--r--   0 root         (0) root         (0)      358 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      680 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/datasets/amazon_product_review.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/datasets/base_api.py
+-rw-r--r--   0 root         (0) root         (0)      288 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/datasets/download.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/datasets/ibm_fraud_detect.py
+-rw-r--r--   0 root         (0) root         (0)     1208 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/datasets/nyc_taxi.py
+-rw-r--r--   0 root         (0) root         (0)      905 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/datasets/outbrain.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/datasets/pretrained.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/datasets/twitter_recsys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.893554 pyrecdp-1.0.1b202305181/pyrecdp/primitives/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.893554 pyrecdp-1.0.1b202305181/pyrecdp/primitives/engines/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-01 06:07:04.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/engines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       93 2023-03-01 06:17:33.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/engines/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.893554 pyrecdp-1.0.1b202305181/pyrecdp/primitives/estimators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/estimators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2091 2023-05-13 22:10:56.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/estimators/base.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-05-12 20:38:27.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/estimators/lightgbm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.893554 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/
+-rw-r--r--   0 root         (0) root         (0)     1855 2023-05-13 20:11:42.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      234 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/base.py
+-rw-r--r--   0 root         (0) root         (0)      269 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/binned.py
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/category.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-05-12 03:42:22.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/datetime.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/drop.py
+-rw-r--r--   0 root         (0) root         (0)     4047 2023-05-12 20:27:56.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/encode.py
+-rw-r--r--   0 root         (0) root         (0)     1221 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/feature_transform.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/featuretools_adaptor.py
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/fillna.py
+-rw-r--r--   0 root         (0) root         (0)     4666 2023-05-12 20:55:11.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/geograph.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-05-13 21:52:17.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/name.py
+-rw-r--r--   0 root         (0) root         (0)     3100 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/nlp.py
+-rw-r--r--   0 root         (0) root         (0)     4720 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/relation.py
+-rw-r--r--   0 root         (0) root         (0)     2975 2023-05-05 19:42:48.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.893554 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6028 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/base.py
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/category.py
+-rw-r--r--   0 root         (0) root         (0)      351 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/custom.py
+-rw-r--r--   0 root         (0) root         (0)     1929 2023-05-15 23:17:43.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/data.py
+-rw-r--r--   0 root         (0) root         (0)     3291 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/dataframe.py
+-rw-r--r--   0 root         (0) root         (0)      758 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/drop.py
+-rw-r--r--   0 root         (0) root         (0)     3940 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/encode.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/featuretools_adaptor.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/fillna.py
+-rw-r--r--   0 root         (0) root         (0)      682 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/geograph.py
+-rw-r--r--   0 root         (0) root         (0)     1376 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/merge.py
+-rw-r--r--   0 root         (0) root         (0)      709 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/name.py
+-rw-r--r--   0 root         (0) root         (0)      712 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.893554 pyrecdp-1.0.1b202305181/pyrecdp/primitives/profilers/
+-rw-r--r--   0 root         (0) root         (0)      157 2023-05-08 18:34:18.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/profilers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5674 2023-05-19 16:42:22.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/profilers/statics.py
+-rw-r--r--   0 root         (0) root         (0)     4398 2023-05-18 18:54:28.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/profilers/type_infer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.893554 pyrecdp-1.0.1b202305181/pyrecdp/primitives/spark_data_processor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/spark_data_processor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54029 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/spark_data_processor/data_processor.py
+-rw-r--r--   0 root         (0) root         (0)     8145 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/spark_data_processor/encoder.py
+-rw-r--r--   0 root         (0) root         (0)     8115 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/primitives/spark_data_processor/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.897554 pyrecdp-1.0.1b202305181/pyrecdp/widgets/
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/BaseWidget.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/PlotWidget.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/ProfilerWidget.py
+-rw-r--r--   0 root         (0) root         (0)      821 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/TabWidget.py
+-rw-r--r--   0 root         (0) root         (0)     2103 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/TableViewWidget.py
+-rw-r--r--   0 root         (0) root         (0)      221 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.897554 pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/
+-rw-r--r--   0 root         (0) root         (0)      989 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/base.html
+-rw-r--r--   0 root         (0) root         (0)       85 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/error.html
+-rw-r--r--   0 root         (0) root         (0)      260 2023-05-11 22:08:36.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/interactions.html
+-rw-r--r--   0 root         (0) root         (0)     1340 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/overview.html
+-rw-r--r--   0 root         (0) root         (0)     7110 2023-05-15 23:17:43.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/scripts.html
+-rw-r--r--   0 root         (0) root         (0)    16515 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/styles.html
+-rw-r--r--   0 root         (0) root         (0)     9250 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/variables.html
+-rw-r--r--   0 root         (0) root         (0)      166 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305181/pyrecdp/widgets/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 16:51:25.889553 pyrecdp-1.0.1b202305181/pyrecdp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10481 2023-05-19 16:51:25.000000 pyrecdp-1.0.1b202305181/pyrecdp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3454 2023-05-19 16:51:25.000000 pyrecdp-1.0.1b202305181/pyrecdp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 16:51:25.000000 pyrecdp-1.0.1b202305181/pyrecdp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-13 19:42:06.000000 pyrecdp-1.0.1b202305181/pyrecdp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      221 2023-05-19 16:51:25.000000 pyrecdp-1.0.1b202305181/pyrecdp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-19 16:51:25.000000 pyrecdp-1.0.1b202305181/pyrecdp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 16:51:25.897554 pyrecdp-1.0.1b202305181/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1486 2023-05-18 19:00:07.000000 pyrecdp-1.0.1b202305181/setup.py
```

### Comparing `pyrecdp-1.0.1b202305161/LICENSE` & `pyrecdp-1.0.1b202305181/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/PKG-INFO` & `pyrecdp-1.0.1b202305181/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: pyrecdp
-Version: 1.0.1b202305161
-Summary: A data processing bundle for spark based recommender system operations
-Home-page: https://github.com/intel/e2eAIOK/
-Author: INTEL AIA
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # RecDP v2.0
 
 # INTRODUCTION
 
 ## Problem Statement
 
 Data Preparation is an essential step to build AI pipelines 
@@ -214,9 +198,7 @@
 
 ## LICENSE
 * Apache 2.0
 
 ## Dependency
 * Spark 3.x
 * python 3.*
-
-
```

### Comparing `pyrecdp-1.0.1b202305161/README.md` & `pyrecdp-1.0.1b202305181/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,204 +1,219 @@
-# RecDP v2.0
-
-# INTRODUCTION
-
-## Problem Statement
-
-Data Preparation is an essential step to build AI pipelines 
-* key data preparation capabilities: data connector, cleaning, sampling, joining, profiling, feature engineering, low-code/no-code UI, lineage etc. 
-* exploration of optimal Data preparation consumes majority of Data Science time
-
-## Solution with RecDP v2.0
-
-* Auto pipeline
-    * only 3 lines of codes required
-* Pipeline Generator
-    * Data Profiling:
-        * Auto anomalies detection
-        * Auto missing value impute
-        * Profiling Visualizzation        
-    * Feature Wrangling:
-        * feature transformation(datetime, geo_info, text_nlp, url, etc.)
-        * multiple data auto joining
-        * feature cross(aggregation transformation - sum, avg, count, etc.)
-    * export pipeline as JSON file, can be import to other data platform
-* Pipeline Runner:
-    * spark engine: convert pipeline to spark codes to run
-    * pandas engine: convert pipeline to pandas codes to run
-    * sql engine: convert pipeline to sql
-* DataLoader:
-    * parquet, csv, json, database
-* FeatureWriter - ML/DL connector:
-    * Data Lineage
-    * Feature Store
-    * numpy, csv, parquet, dgl / pyG graph
-![RecDP v2.0 Overview](resources/recdp_intro.png)
-
-## This solution is intended for
-citizen data scientists, enterprise users, independent software vendor and partial of cloud service provider.
-
-# Getting Start
-## setup with pip
-```
-git clone --single-branch --branch RecDP_v2.0 https://github.com/intel-innersource/frameworks.bigdata.AIDK.git
-cd frameworks.bigdata.AIDK/RecDP
-# install dependencies
-apt-get update -y &&  DEBIAN_FRONTEND=noninteractive apt-get install -y python3 python3-pip python-is-python3 graphviz
-DEBIAN_FRONTEND=noninteractive apt-get install -y openjdk-8-jre
-# install recdp
-python setup.py sdist
-pip install dist/pyrecdp-1.0.1.tar.gz
-
-sh start-jupyter.sh
-# open browser with http://hostname:8888
-```
-
-## run
-![nyc taxi demo](https://github.com/intel-innersource/frameworks.bigdata.AIDK/assets/4355494/03d8c2fe-de47-41f9-9fef-8513bc4aaf42)
-
-## modify pipeline (add user defined function or remove operation)
-``` python
-def filter_with_cond(df):
-    df = df[df['Year'] <= 2018]
-    return df
-operation = {
-    "children": [6], # will to append this new op
-    "next": [7], # who will be connected to this new op
-    "inline_function": filter_with_cond, # function
-}
-pipeline.add_operation(operation)
-```
-``` python
-operation = {
-    "idx": 6, # OP id to be deleted
-    "next": [10] # who is connected to the to_be_deleted op
-}
-pipeline.delete_operation(operation)
-```
-
-## export pipeline
-``` python
-pipeline.export(file_path = "exported_pipeline.json")
-```
-``` json
-{
-    "0": {
-        "children": null,
-        "op": "DataFrame",
-        "config": "main_table"
-    },
-    "1": {
-        "children": [0],
-        "op": "type_infer",
-        "config": [
-            ["pickup_datetime",["is_string","is_datetime"]],
-            ["pickup_longitude",["is_numeric","is_float"]],
-            ["pickup_latitude",["is_numeric","is_float"]],
-            ["dropoff_longitude",["is_numeric","is_float"]],
-            ["dropoff_latitude",["is_numeric","is_float"]],
-            ["passenger_count",["is_numeric","is_int64","is_integer","is_categorical"]]
-        ]
-    },
-    "2": {
-        "children": [1],
-        "op": "tuple",
-        "config": {
-            "src": ["pickup_latitude","pickup_longitude"],"dst": "pickup_coordinates"
-        }
-    },
-    "3": {
-        "children": [2],
-        "op": "tuple",
-        "config": {
-            "src": ["dropoff_latitude","dropoff_longitude"],"dst": "dropoff_coordinates"
-        }
-    },
-    "4": {
-        "children": [3],
-        "op": "fillna",
-        "config": {
-            "pickup_longitude": -1,
-            "pickup_latitude": -1,
-            "dropoff_longitude": -1,
-            "dropoff_latitude": -1,
-            "passenger_count": -1
-        }
-    },
-    "5": {
-        "children": [4],
-        "op": "datetime_feature",
-        "config": {
-            "pickup_datetime": [
-                ["pickup_datetime__day",["featuretools.primitives.standard.transform.datetime.day", "Day"]],
-                ["pickup_datetime__month",["featuretools.primitives.standard.transform.datetime.month","Month"]],
-                ["pickup_datetime__weekday",["featuretools.primitives.standard.transform.datetime.weekday","Weekday"]],
-                ["pickup_datetime__year",["featuretools.primitives.standard.transform.datetime.year","Year"]],
-                ["pickup_datetime__hour",["featuretools.primitives.standard.transform.datetime.hour","Hour"]]
-            ]
-        }
-    },
-    "6": {
-        "children": [5],
-        "op": "haversine",
-        "config": {
-            "['pickup_coordinates', 'dropoff_coordinates']": ["haversine_pickup_coordinates_dropoff_coordinates",["featuretools.primitives.standard.transform.latlong.haversine","Haversine"]]
-        }
-    },
-    "7": {
-        "children": [6],
-        "op": "drop",
-        "config": [
-            "pickup_datetime",
-            "pickup_coordinates",
-            "dropoff_coordinates"
-        ]
-    },
-    "8": {
-        "children": [7],
-        "op": "lightgbm",
-        "config": {
-            "label": "fare_amount",
-            "metrics": "rmse",
-            "objective": "regression",
-            "model_file": "lightgbm_regression_label.mdl",
-            "method": "predict"
-        }
-    }
-}
-```
-
-
-## Quick Example
-* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/de044d606e6cdc44d3005db2a0ae968d/recdp_fare_prediction.ipynb) - [nyc taxi fare](examples/notebooks/autofe/demo/nyc_taxi_workflow_train.ipynb) - geographic, datetime, lgbm regression
-
-* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/2b8acb3eda73028635072352560139ba/recdp_fraud_detect.ipynb) - [IBM Card Transaction Fraud Detect](examples/notebooks/autofe/demo/fraud_detect_train.ipynb) - onehot encode, lgbm, binary classification 
-
-* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/b039b8c0a40fec951b1b09c3fbb93a7b/recdp_social_media.ipynb) - [twitter recsys](examples/notebooks/autofe/demo/twitter_workflow_test.ipynb) - text nlp, datetime feature engineering  
-
-* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/1e08668ab0e15e1e98c592f284d79dad/recdp_click_through_rate_multiple_tables.ipynb) - [outbrain](examples/notebooks/autofe/demo/outbrain_ctr_workflow_test.ipynb) - multiple table joining
-
-* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/2f942c30dbf9b63a64cc819a61966e34/recdp_rating_prediction_amazon_review.ipynb) - [amazon product review](examples/notebooks/autofe/demo/amazon_product_review_test.ipynb) - text nlp, datetime, feature-cross
-
-# More Examples - completed example including training
-
-## Auto Feature Engineering vs. featuretools
-* [NYC Taxi fare auto data prepration](examples/notebooks/autofe/FeatureWrangler.ipynb): An example to show how RecDP_v2.0 automatically generating datetime and geo features upon 55M records. Tested with both Spark and Pandas(featuretools) as compute engine, show 21x speedup by spark.
-
-## load PIPELINE and execute
-* [twitter pipeline re-load and execute](examples/notebooks/autofe/demo/custom_pipeline_twitter.ipynb): An example to show how RecDP_v2.0 reload pipeline from json and do execution - use RecDP as compute engine.
-
-## Realtime Inference pipeline
-* [nyc taxi fare](examples/notebooks/autofe/demo/nyc_taxi_workflow_predict.ipynb) - geographic, datetime feature engineering, lgbm
-
-## Data Profiler Examples
-* [NYC Taxi fare Profiler](resources/FeatureProfiler_NYC.png): An example to show RecDP_v2.0 to profile data, including infer the potential data type, generate data distribution charts.
-
-* [twitter Profiler](resources/FeatureProfiler_recsys.png): An example to show RecDP_v2.0 to profile data, including infer the potential data type, generate data distribution charts.
-
-
-## LICENSE
-* Apache 2.0
-
-## Dependency
-* Spark 3.x
-* python 3.*
+Metadata-Version: 2.1
+Name: pyrecdp
+Version: 1.0.1b202305181
+Summary: A data processing bundle for spark based recommender system operations
+Home-page: https://github.com/intel/e2eAIOK/
+Author: INTEL AIA
+License: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/
+Description: # RecDP v2.0
+        
+        # INTRODUCTION
+        
+        ## Problem Statement
+        
+        Data Preparation is an essential step to build AI pipelines 
+        * key data preparation capabilities: data connector, cleaning, sampling, joining, profiling, feature engineering, low-code/no-code UI, lineage etc. 
+        * exploration of optimal Data preparation consumes majority of Data Science time
+        
+        ## Solution with RecDP v2.0
+        
+        * Auto pipeline
+            * only 3 lines of codes required
+        * Pipeline Generator
+            * Data Profiling:
+                * Auto anomalies detection
+                * Auto missing value impute
+                * Profiling Visualizzation        
+            * Feature Wrangling:
+                * feature transformation(datetime, geo_info, text_nlp, url, etc.)
+                * multiple data auto joining
+                * feature cross(aggregation transformation - sum, avg, count, etc.)
+            * export pipeline as JSON file, can be import to other data platform
+        * Pipeline Runner:
+            * spark engine: convert pipeline to spark codes to run
+            * pandas engine: convert pipeline to pandas codes to run
+            * sql engine: convert pipeline to sql
+        * DataLoader:
+            * parquet, csv, json, database
+        * FeatureWriter - ML/DL connector:
+            * Data Lineage
+            * Feature Store
+            * numpy, csv, parquet, dgl / pyG graph
+        ![RecDP v2.0 Overview](resources/recdp_intro.png)
+        
+        ## This solution is intended for
+        citizen data scientists, enterprise users, independent software vendor and partial of cloud service provider.
+        
+        # Getting Start
+        ## setup with pip
+        ```
+        git clone --single-branch --branch RecDP_v2.0 https://github.com/intel-innersource/frameworks.bigdata.AIDK.git
+        cd frameworks.bigdata.AIDK/RecDP
+        # install dependencies
+        apt-get update -y &&  DEBIAN_FRONTEND=noninteractive apt-get install -y python3 python3-pip python-is-python3 graphviz
+        DEBIAN_FRONTEND=noninteractive apt-get install -y openjdk-8-jre
+        # install recdp
+        python setup.py sdist
+        pip install dist/pyrecdp-1.0.1.tar.gz
+        
+        sh start-jupyter.sh
+        # open browser with http://hostname:8888
+        ```
+        
+        ## run
+        ![nyc taxi demo](https://github.com/intel-innersource/frameworks.bigdata.AIDK/assets/4355494/03d8c2fe-de47-41f9-9fef-8513bc4aaf42)
+        
+        ## modify pipeline (add user defined function or remove operation)
+        ``` python
+        def filter_with_cond(df):
+            df = df[df['Year'] <= 2018]
+            return df
+        operation = {
+            "children": [6], # will to append this new op
+            "next": [7], # who will be connected to this new op
+            "inline_function": filter_with_cond, # function
+        }
+        pipeline.add_operation(operation)
+        ```
+        ``` python
+        operation = {
+            "idx": 6, # OP id to be deleted
+            "next": [10] # who is connected to the to_be_deleted op
+        }
+        pipeline.delete_operation(operation)
+        ```
+        
+        ## export pipeline
+        ``` python
+        pipeline.export(file_path = "exported_pipeline.json")
+        ```
+        ``` json
+        {
+            "0": {
+                "children": null,
+                "op": "DataFrame",
+                "config": "main_table"
+            },
+            "1": {
+                "children": [0],
+                "op": "type_infer",
+                "config": [
+                    ["pickup_datetime",["is_string","is_datetime"]],
+                    ["pickup_longitude",["is_numeric","is_float"]],
+                    ["pickup_latitude",["is_numeric","is_float"]],
+                    ["dropoff_longitude",["is_numeric","is_float"]],
+                    ["dropoff_latitude",["is_numeric","is_float"]],
+                    ["passenger_count",["is_numeric","is_int64","is_integer","is_categorical"]]
+                ]
+            },
+            "2": {
+                "children": [1],
+                "op": "tuple",
+                "config": {
+                    "src": ["pickup_latitude","pickup_longitude"],"dst": "pickup_coordinates"
+                }
+            },
+            "3": {
+                "children": [2],
+                "op": "tuple",
+                "config": {
+                    "src": ["dropoff_latitude","dropoff_longitude"],"dst": "dropoff_coordinates"
+                }
+            },
+            "4": {
+                "children": [3],
+                "op": "fillna",
+                "config": {
+                    "pickup_longitude": -1,
+                    "pickup_latitude": -1,
+                    "dropoff_longitude": -1,
+                    "dropoff_latitude": -1,
+                    "passenger_count": -1
+                }
+            },
+            "5": {
+                "children": [4],
+                "op": "datetime_feature",
+                "config": {
+                    "pickup_datetime": [
+                        ["pickup_datetime__day",["featuretools.primitives.standard.transform.datetime.day", "Day"]],
+                        ["pickup_datetime__month",["featuretools.primitives.standard.transform.datetime.month","Month"]],
+                        ["pickup_datetime__weekday",["featuretools.primitives.standard.transform.datetime.weekday","Weekday"]],
+                        ["pickup_datetime__year",["featuretools.primitives.standard.transform.datetime.year","Year"]],
+                        ["pickup_datetime__hour",["featuretools.primitives.standard.transform.datetime.hour","Hour"]]
+                    ]
+                }
+            },
+            "6": {
+                "children": [5],
+                "op": "haversine",
+                "config": {
+                    "['pickup_coordinates', 'dropoff_coordinates']": ["haversine_pickup_coordinates_dropoff_coordinates",["featuretools.primitives.standard.transform.latlong.haversine","Haversine"]]
+                }
+            },
+            "7": {
+                "children": [6],
+                "op": "drop",
+                "config": [
+                    "pickup_datetime",
+                    "pickup_coordinates",
+                    "dropoff_coordinates"
+                ]
+            },
+            "8": {
+                "children": [7],
+                "op": "lightgbm",
+                "config": {
+                    "label": "fare_amount",
+                    "metrics": "rmse",
+                    "objective": "regression",
+                    "model_file": "lightgbm_regression_label.mdl",
+                    "method": "predict"
+                }
+            }
+        }
+        ```
+        
+        
+        ## Quick Example
+        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/de044d606e6cdc44d3005db2a0ae968d/recdp_fare_prediction.ipynb) - [nyc taxi fare](examples/notebooks/autofe/demo/nyc_taxi_workflow_train.ipynb) - geographic, datetime, lgbm regression
+        
+        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/2b8acb3eda73028635072352560139ba/recdp_fraud_detect.ipynb) - [IBM Card Transaction Fraud Detect](examples/notebooks/autofe/demo/fraud_detect_train.ipynb) - onehot encode, lgbm, binary classification 
+        
+        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/b039b8c0a40fec951b1b09c3fbb93a7b/recdp_social_media.ipynb) - [twitter recsys](examples/notebooks/autofe/demo/twitter_workflow_test.ipynb) - text nlp, datetime feature engineering  
+        
+        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/1e08668ab0e15e1e98c592f284d79dad/recdp_click_through_rate_multiple_tables.ipynb) - [outbrain](examples/notebooks/autofe/demo/outbrain_ctr_workflow_test.ipynb) - multiple table joining
+        
+        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/2f942c30dbf9b63a64cc819a61966e34/recdp_rating_prediction_amazon_review.ipynb) - [amazon product review](examples/notebooks/autofe/demo/amazon_product_review_test.ipynb) - text nlp, datetime, feature-cross
+        
+        # More Examples - completed example including training
+        
+        ## Auto Feature Engineering vs. featuretools
+        * [NYC Taxi fare auto data prepration](examples/notebooks/autofe/FeatureWrangler.ipynb): An example to show how RecDP_v2.0 automatically generating datetime and geo features upon 55M records. Tested with both Spark and Pandas(featuretools) as compute engine, show 21x speedup by spark.
+        
+        ## load PIPELINE and execute
+        * [twitter pipeline re-load and execute](examples/notebooks/autofe/demo/custom_pipeline_twitter.ipynb): An example to show how RecDP_v2.0 reload pipeline from json and do execution - use RecDP as compute engine.
+        
+        ## Realtime Inference pipeline
+        * [nyc taxi fare](examples/notebooks/autofe/demo/nyc_taxi_workflow_predict.ipynb) - geographic, datetime feature engineering, lgbm
+        
+        ## Data Profiler Examples
+        * [NYC Taxi fare Profiler](resources/FeatureProfiler_NYC.png): An example to show RecDP_v2.0 to profile data, including infer the potential data type, generate data distribution charts.
+        
+        * [twitter Profiler](resources/FeatureProfiler_recsys.png): An example to show RecDP_v2.0 to profile data, including infer the potential data type, generate data distribution charts.
+        
+        
+        ## LICENSE
+        * Apache 2.0
+        
+        ## Dependency
+        * Spark 3.x
+        * python 3.*
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
```

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/ScalaProcessUtils/spark-defaults.conf` & `pyrecdp-1.0.1b202305181/pyrecdp/ScalaProcessUtils/spark-defaults.conf`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar` & `pyrecdp-1.0.1b202305181/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/__init__.py` & `pyrecdp-1.0.1b202305181/pyrecdp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/autofe/AutoFE.py` & `pyrecdp-1.0.1b202305181/pyrecdp/autofe/AutoFE.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,42 +24,63 @@
             config = {
                 'model_file': 'autofe_lightgbm.mdl',
                 'objective': infer_problem_type(pipeline.dataset[pipeline.main_table][label]),
                 'model_name': 'lightgbm'}
             self.auto_pipeline['estimator'] = FeatureEstimator(data_pipeline = pipeline, config = config)
 
     def fit_transform(self, engine_type = 'pandas', no_cache = False, *args, **kwargs):
+        print("AutoFE started to execute data")
         ret_df = None
         if self.auto_pipeline['relational']:
             pipeline = self.auto_pipeline['relational']
             ret_df = pipeline.fit_transform(engine_type, data = ret_df)
             print("AutoFE started to profile data")
 
         if self.auto_pipeline['estimator']:
             pipeline = self.auto_pipeline['estimator']
             ret_df = pipeline.fit_transform(engine_type, data = ret_df)
         return ret_df
     
-    def profile(self, engine_type):
+    def profile(self, engine_type = 'pandas'):
         if isinstance(self.auto_pipeline['profiler'], type(None)):
             return "feature profile support for multiple table is WIP"
         return self.auto_pipeline['profiler'].visualize_analyze(engine_type)
 
     def feature_importance(self):
         import pandas as pd
         if isinstance(self.auto_pipeline['estimator'], type(None)):
             return "feature estimator support for multiple table is WIP"
         fe_imp_dict = self.auto_pipeline['estimator'].get_feature_importance()
         feat_importances = pd.Series([i[1] for i in fe_imp_dict], [i[0] for i in fe_imp_dict])
-        return feat_importances.plot(kind='barh')
+        feat_importances = feat_importances[feat_importances > 0].sort_values()
+        height = int(len(feat_importances) * 0.5)
+        return feat_importances.plot(kind='barh', figsize=(15,height))
 
     def plot(self):
         if self.auto_pipeline['relational']:
             return self.auto_pipeline['relational'].plot()
         else:
-            return self.auto_pipeline['estimator'].plot()        
+            return self.auto_pipeline['estimator'].plot()
         
-    def get_transformed_cache(self):
+    def get_transformed_data(self):
         if self.auto_pipeline['relational']:
             return self.auto_pipeline['relational'].get_transformed_cache()
         else:
-            return self.auto_pipeline['estimator'].get_transformed_cache()
+            ret_df = self.auto_pipeline['estimator'].get_transformed_cache()
+            return ret_df
+        
+    def get_feature_list(self):
+        fe_imp_dict = self.auto_pipeline['estimator'].get_feature_importance()
+        feature_list = [i[0] for i in fe_imp_dict if i[1] > 0]
+        return feature_list
+    
+    def add_operation(self, config):
+        if self.auto_pipeline['relational']:
+            return self.auto_pipeline['relational'].add_operation(config)
+        else:
+            return self.auto_pipeline['estimator'].add_operation(config)
+        
+    def delete_operation(self, idx):
+        if self.auto_pipeline['relational']:
+            return self.auto_pipeline['relational'].delete_operation(idx)
+        else:
+            return self.auto_pipeline['estimator'].delete_operation(idx)
```

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/autofe/BasePipeline.py` & `pyrecdp-1.0.1b202305181/pyrecdp/autofe/BasePipeline.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import logging
 import graphviz
 import json
 from pyrecdp.core.utils import Timer, sample_read, deepcopy
 from pyspark.sql import DataFrame as SparkDataFrame
 from pyspark import RDD as SparkRDD
 from IPython.display import display
+from tqdm import tqdm
 
 logging.basicConfig(format='%(asctime)s %(levelname)s:%(message)s', level=logging.ERROR, datefmt='%I:%M:%S')
 logger = logging.getLogger(__name__)
 
 class BasePipeline:
     def __init__(self, dataset, label, *args, **kwargs):
         # properties
@@ -76,17 +77,23 @@
         else:
             self.supplementary = None
         self.rdp = None
      
     def fit_analyze(self, *args, **kwargs):
         child = list(self.pipeline.keys())[-1]
         max_id = child
+        to_run = []
         for i in range(len(self.generators)):
             for generator in self.generators[i]:
-                self.pipeline, child, max_id = generator.fit_prepare(self.pipeline, [child], max_id)
+                to_run.append(generator)
+        
+        pbar = tqdm(to_run, total=len(to_run))
+        for generator in pbar:
+            pbar.set_description(f"{generator.__class__.__name__}")
+            self.pipeline, child, max_id = generator.fit_prepare(self.pipeline, [child], max_id)
         return child, max_id
 
     def __repr__(self):
         return repr(self.pipeline)
 
     def export(self, file_path = None):
         json_object = self.pipeline.json_dump()
@@ -116,93 +123,85 @@
             if actual_op:
                 executable_pipeline[idx] = actual_op
                 executable_sequence.append(executable_pipeline[idx])
         return executable_pipeline, executable_sequence
     
     def add_operation(self, config):
         # check if below keys are existing
-        # children: who is its child
-        # next: who is will use this operation
-        # inline_function: the function to process data
-        example = """
-            def add_one_print(df):
-                df['col_1'] = df['col_1'] + 1
-                display(df)
-                return df
-            {
-                "children": [7],
-                "next": [8],
-                "inline_function": add_one_print,
-            }"""
-        try:
-            children = config["children"]
-            next = config["next"]
-            inline_function = config["inline_function"]
-        except:
-            raise ValueError(f"please follow this example to create customer operator: {example}")
+        # config can be either a dict or function defininition
+        pipeline_chain = self.to_chain()
+        if not hasattr(self, 'transformed_end_idx'):            
+            leaf_child = pipeline_chain[-1]
+        else:
+            leaf_child = self.pipeline[self.transformed_end_idx].children[0]
+        
+        if not isinstance(config, dict):
+            op = config
+            config = {
+                "children": [leaf_child],
+                "inline_function": op,
+            }        
+        children = config["children"]
+        inline_function = config["inline_function"]
+        
         if not isinstance(children, list):
             children = [children]
-        if not isinstance(next, list):
-            next = [next]
-        if len(children) > 1 and len(next) > 1:
-            raise NotImplementedError("Current we didn't support add operation to case that children and next are all multiple operators.")
         
         # get current max operator id
         max_idx = self.pipeline.get_max_idx()
         cur_idx = max_idx + 1
         
         config = {
             "func_name": inline_function,
         }
         self.pipeline[cur_idx] = Operation(
             cur_idx, children, output = None, op = "custom_operator", config = config)
-        for idx in next:
-            # replace next's children with new added operator
-            children_in_next = self.pipeline[idx].children
-            found = {}
-            for id, child in enumerate(children_in_next):
-                if child in children:
-                    found[id] = cur_idx
-            for k, v in found.items():
-                self.pipeline[idx].children[k] = v
-        display(self.plot())
-
-    def delete_operation(self, config):
-        example = """
-            config = {
-                "idx": 7,
-                "next": [8]
-            }"""
-        try:
-            cur_idx = config["idx"]
-            next = config["next"]
-        except:
-            raise ValueError(f"please follow this example to create customer operator: {example}")
-        if not isinstance(next, list):
-            next = [next]
-            
-        children = self.pipeline[cur_idx].children
-        if len(children) > 1 and len(next) > 1:
-            raise NotImplementedError("Current we didn't support add operation to case that children and next are all multiple operators.")
-        
-        if len(next) == 1:
-            self.pipeline[next[0]].children = children
-        else:            
+        
+        # we need to find nexts
+        for to_replace_child in children:
+            next = []
+            for idx in pipeline_chain:
+                if self.pipeline[idx].children and to_replace_child in self.pipeline[idx].children:
+                    next.append(idx)
             for idx in next:
                 # replace next's children with new added operator
                 children_in_next = self.pipeline[idx].children
                 found = {}
                 for id, child in enumerate(children_in_next):
-                    if child == cur_idx:
-                        found[id] = children[0]
+                    if child == to_replace_child:
+                        found[id] = cur_idx
                 for k, v in found.items():
                     self.pipeline[idx].children[k] = v
+
+    def delete_operation(self, id):
+        cur_idx = id
+        pipeline_chain = self.to_chain()
+        children = self.pipeline[cur_idx].children    
+        # we need to find nexts
+        for to_replace_child in children:
+            next = []
+            for idx in pipeline_chain:
+                if self.pipeline[idx].children and to_replace_child in self.pipeline[idx].children:
+                    next.append(idx)
+            if len(next) == 1:
+                self.pipeline[next[0]].children = children
+            else:            
+                for idx in next:
+                    # replace next's children with new added operator
+                    children_in_next = self.pipeline[idx].children
+                    found = {}
+                    for id, child in enumerate(children_in_next):
+                        if child == cur_idx:
+                            found[id] = to_replace_child
+                    for k, v in found.items():
+                        self.pipeline[idx].children[k] = v
+        if hasattr(self, 'transformed_end_idx'):
+            self.transformed_end_idx = children[0]
         del self.pipeline[cur_idx]
-        display(self.plot())        
-           
+          
     def plot(self):
         f = graphviz.Digraph(format='svg')
         edges = []
         nodes = []
         f.attr(fontsize='10')
         def add_escape(input):
             input = input.replace('<', '\<').replace('>', '\>')
```

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/autofe/FeatureEstimator.py` & `pyrecdp-1.0.1b202305181/pyrecdp/autofe/FeatureEstimator.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         else:
             raise NotImplementedError(f"Unsupport input datapipeline is {data_pipeline}")
         if label is None and method != 'predict':
             raise ValueError("Unable to find label for this pipeline, please provide it through API")
         
         max_idx = self.pipeline.get_max_idx()
         leaf_idx = self.pipeline.convert_to_node_chain()[-1]
-
+        self.transformed_end_idx = -1
         
         if self.pipeline[leaf_idx].op not in ["lightgbm"]:
             model_name = config['model_name']
             objective = config['objective']
             if objective == 'binary':
                 config['metrics'] = 'auc'
             elif objective == 'regression':
```

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/autofe/FeatureProfiler.py` & `pyrecdp-1.0.1b202305181/pyrecdp/autofe/FeatureProfiler.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/autofe/FeatureWrangler.py` & `pyrecdp-1.0.1b202305181/pyrecdp/autofe/FeatureWrangler.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,8 +53,9 @@
             max_id = cur_id
             child = cur_id
             sampled_data = sampled_data[self.feature_columns]
         
         # firstly, call data profiler to analyze data
         for generator in self.data_profiler:
             self.pipeline, child, max_id = generator.fit_prepare(self.pipeline, [child], max_id, sampled_data)
+        print("Feature List generated, using analyzed feature tags to create data pipeline")
         return super().fit_analyze(*args, **kwargs)
```

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/autofe/RelationalBuilder.py` & `pyrecdp-1.0.1b202305181/pyrecdp/autofe/RelationalBuilder.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/core/di_graph.py` & `pyrecdp-1.0.1b202305181/pyrecdp/core/di_graph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/core/schema.py` & `pyrecdp-1.0.1b202305181/pyrecdp/core/schema.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/core/utils.py` & `pyrecdp-1.0.1b202305181/pyrecdp/core/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -35,27 +35,46 @@
         b_list = b.tolist()
     elif isinstance(b, list):
         b_list = b
     a_dict = dict((i, 0) for i in a_list)
     [a_list.append(i) for i in b_list if i not in a_dict]
     return np.array(a_list)
 
-def increment_encoder(encoder, dict_path):
+def get_encoder_np(encoder, dict_path):
+    if isinstance(dict_path, type(None)):
+        return encoder
+    dirname = os.path.dirname(dict_path)
+    if not os.path.exists(dict_path):
+        return encoder
+    encoder.classes_ = np.load(dict_path)    
+    return encoder
+
+def save_encoder_np(encoder, dict_path):
+    if isinstance(dict_path, type(None)):
+        return
     dirname = os.path.dirname(dict_path)
     if not os.path.exists(dirname):
         os.mkdir(dirname)
-    if os.path.exists(dict_path):
-        saved_dict = np.load(dict_path)
-        # update dict
-        ret = sequenced_union1d(encoder.classes_, saved_dict)
-        encoder.classes_ = ret
-    # save dictionary
     np.save(dict_path, encoder.classes_)
-    
-    return encoder
+
+def get_encoder_df(dict_path):
+    if isinstance(dict_path, type(None)):
+        return None
+    dirname = os.path.dirname(dict_path)
+    if not os.path.exists(dict_path):
+        return None
+    return pd.read_parquet(dict_path)
+
+def save_encoder_df(encoder, dict_path):
+    if isinstance(dict_path, type(None)):
+        return
+    dirname = os.path.dirname(dict_path)
+    if not os.path.exists(dirname):
+        os.mkdir(dirname)
+    encoder.to_parquet(dict_path)
     
 def deepcopy(dict_df):
     return copy.deepcopy(dict_df)
     
 def get_sample_indices_pd(indices, target_num_rows):
     if isinstance(indices, pd.DataFrame):
         indices = indices.notna()
```

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/datasets/CESM_breast_cancer.py` & `pyrecdp-1.0.1b202305181/pyrecdp/datasets/CESM_breast_cancer.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/datasets/amazon_product_review.py` & `pyrecdp-1.0.1b202305181/pyrecdp/datasets/amazon_product_review.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/datasets/base_api.py` & `pyrecdp-1.0.1b202305181/pyrecdp/datasets/base_api.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/datasets/ibm_fraud_detect.py` & `pyrecdp-1.0.1b202305181/pyrecdp/datasets/ibm_fraud_detect.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/datasets/nyc_taxi.py` & `pyrecdp-1.0.1b202305181/pyrecdp/datasets/nyc_taxi.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/datasets/outbrain.py` & `pyrecdp-1.0.1b202305181/pyrecdp/datasets/outbrain.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/estimators/base.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/estimators/base.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/estimators/lightgbm.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/estimators/lightgbm.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/__init__.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/category.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/category.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from .base import BaseFeatureGenerator as super_class
 import pandas as pd
 from pyrecdp.core import SeriesSchema
 from pyrecdp.primitives.operations import Operation
+import copy
 
 class CategoryFeatureGenerator(super_class):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     def fit_prepare(self, pipeline, children, max_idx):
         is_useful = False
         pa_schema = pipeline[children[0]].output
         feature_in_out = {}
         folder = 'pipeline_default'
+        ret_pa_schema = copy.deepcopy(pa_schema)
         for pa_field in pa_schema:
             if pa_field.is_categorical_and_string:
                 feature = pa_field.name
                 out_schema = SeriesSchema(f"{feature}__idx", pd.CategoricalDtype())
                 feature_in_out[feature] = (f"{folder}/{feature}_categorify_dict", out_schema.name)
                 is_useful = True
-                pa_schema.append(out_schema)
+                ret_pa_schema.append(out_schema)
         if is_useful:
             cur_idx = max_idx + 1
             config = feature_in_out
-            pipeline[cur_idx] = Operation(cur_idx, children, pa_schema, op = 'categorify', config = config)
+            pipeline[cur_idx] = Operation(cur_idx, children, ret_pa_schema, op = 'categorify', config = config)
             return pipeline, cur_idx, cur_idx
         else:
             return pipeline, children[0], max_idx
```

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/datetime.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/datetime.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/drop.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/drop.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/encode.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/encode.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/feature_transform.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/feature_transform.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/featuretools_adaptor.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/featuretools_adaptor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/fillna.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/fillna.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/geograph.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/geograph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/name.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/name.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/nlp.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/nlp.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/relation.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/relation.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/generators/type.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/generators/type.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/base.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,18 @@
     @staticmethod
     def load(idx, dump_dict):
         obj = Operation(idx, dump_dict['children'], None, dump_dict['op'], dump_dict['config'])
         return obj
 
 class BaseOperation:
     def __init__(self, op_base):
+        # option1: for get_function_pd use
+        if not isinstance(op_base, Operation):
+            op_base = Operation(-1, None, [], f'{self.__class__.__name__}', op_base)
+        # option2: complete usage in recdp
         self.op = op_base
         self.cache = None
         self.support_spark_dataframe = False
         self.support_spark_rdd = False
         self.fast_without_dpp = False
        
     def __repr__(self) -> str:
```

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/category.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/tuple.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 from .base import BaseOperation
-import pandas as pd
-from pyspark.sql import DataFrame as SparkDataFrame
-from pyrecdp.core.utils import increment_encoder
-import copy
 
-class CategorifyOperation(BaseOperation):
+class TupleOperation(BaseOperation):        
     def __init__(self, op_base):
         super().__init__(op_base)
-        self.feature_in_out = op_base.config
         self.support_spark_dataframe = False
-        self.support_spark_rdd = False
-    
+        self.support_spark_rdd = True
+        self.feature_in = self.op.config['src']
+        self.feature_out = self.op.config['dst']
+
     def get_function_pd(self):
-        feature_in_out = copy.deepcopy(self.feature_in_out)
-        def categorify(df):
-            from sklearn.preprocessing import LabelEncoder
-            import numpy
-            import os
-            for feature, (dict_path, feature_out) in feature_in_out.items():
-                encoder = LabelEncoder()
-                encoder.fit(df[feature])
-                encoder = increment_encoder(encoder, dict_path)
-                df[f"{feature_out}"] = pd.Series(encoder.transform(df[feature]))
-                
+        feature_in = self.feature_in.copy()
+        feature_out = self.feature_out
+        def process(df):
+            df[feature_out] = df[feature_in].apply(tuple, axis=1)
             return df
-        return categorify
+        return process
+
+    def get_function_spark(self, rdp):
+        raise NotImplementedError(f"CoordinatesOperation spark dataframe is not supported yet.")
```

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/data.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/data.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/dataframe.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/drop.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/drop.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pyspark.sql import DataFrame as SparkDataFrame
 from pyspark import RDD
 import copy
  
 class DropOperation(BaseOperation):
     def __init__(self, op_base):
         super().__init__(op_base)
-        self.feature_in = op_base.config
+        self.feature_in = self.op.config
         self.support_spark_dataframe = True
         self.support_spark_rdd = True
         self.fast_without_dpp = True
 
     def get_function_pd(self):
         feature_in = copy.deepcopy(self.feature_in)
         def drop_useless_feature(df):
```

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/featuretools_adaptor.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/featuretools_adaptor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .base import BaseOperation
 import copy
 from pyrecdp.core.utils import class_name_fix
 
 class FeaturetoolsOperation(BaseOperation):
     def __init__(self, op_base):
         super().__init__(op_base)
-        self.feature_in_out_map = op_base.config
+        self.feature_in_out_map = self.op.config
         self.support_spark_dataframe = False
         self.support_spark_rdd = True
 
     def get_function_pd(self):
         feature_in_out_map = copy.deepcopy(self.feature_in_out_map)
         def generate_ft_feature(df):
             for in_feat_name, ops in feature_in_out_map.items():
```

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/fillna.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/fillna.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .base import BaseOperation
 import copy
 
 class FillNaOperation(BaseOperation):
     def __init__(self, op_base):
         super().__init__(op_base)
-        self._fillna_feature_map = op_base.config
+        self._fillna_feature_map = self.op.config
         self.support_spark_dataframe = True
         self.support_spark_rdd = True
     
     def get_function_pd(self):
         _fillna_feature_map = copy.deepcopy(self._fillna_feature_map)
         def fill_na(df):
             df.fillna(_fillna_feature_map, inplace=True, downcast=False)
```

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/geograph.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/geograph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/merge.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/merge.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .base import BaseOperation
 import pandas as pd
 
 class MergeOperation(BaseOperation):
     def __init__(self, op_base):
         super().__init__(op_base)
-        self.config = op_base.config
+        self.config = self.op.config
         
     def execute_pd(self, pipeline):
         if self.cache is not None:
             return
         
         if len(self.op.children) != 2:
             raise ValueError("merge operation only accept num_children as 2")
```

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/name.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/name.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .base import BaseOperation
 import copy
 
 class RenameOperation(BaseOperation):
     def __init__(self, op_base):
         super().__init__(op_base)
-        self.renamed = op_base.config
+        self.renamed = self.op.config
         self.support_spark_dataframe = True
         self.support_spark_rdd = True
         self.fast_without_dpp = True
         
     def get_function_pd(self):
         renamed = copy.deepcopy(self.renamed)
         def rename(df):
```

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/operations/type.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/operations/type.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pyrecdp.core import SeriesSchema
 import pandas as pd
 import copy
 
 class TypeInferOperation(BaseOperation):
     def __init__(self, op_base):
         super().__init__(op_base)
-        self.astype_feature_map = op_base.config
+        self.astype_feature_map = self.op.config
         self.support_spark_dataframe = False
         self.support_spark_rdd = True
 
     def get_function_pd(self):
         astype_feature_map = copy.deepcopy(self.astype_feature_map)
         def type_infer(df):
             for feature in astype_feature_map:
```

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/profilers/statics.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/profilers/statics.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 from pyrecdp.core import SeriesSchema
 from pyrecdp.core.utils import is_text_series
 from pyrecdp.core.utils import Timer
 import pandas as pd
 import numpy as np
+from tqdm import tqdm
+from pyrecdp.core.dataframe import DataFrameAPI
 
 def draw_xy_scatter_plot(xy_scatter_features, feature_data, y, row_height, n_plot_per_row):
     from plotly.subplots import make_subplots
     import plotly.graph_objs as go
     import math
     
     n_feat = len(xy_scatter_features)
     n_row = math.ceil(n_feat / n_plot_per_row)
     n_col = n_plot_per_row if n_feat > n_plot_per_row else n_feat
     subplot_titles = xy_scatter_features
 
     fig_list = make_subplots(rows=n_row, cols=n_col, subplot_titles  = subplot_titles, y_title = y.name)
 
-    indices = y.notna()
-    if indices.size > 1000:
-        frac = 1000/indices.size
-        mask = pd.Series(np.random.choice(a=[False, True], size=(indices.size), p=[1-frac, frac]))
-        indices = indices & mask
+    X = DataFrameAPI().instiate(feature_data)
+    sampled_data = X.may_sample(nrows = 1000)
+    y = sampled_data[y.name]
 
-    for idx, c_name in enumerate(xy_scatter_features):
-        feature = feature_data[c_name]
+    for idx, c_name in tqdm(enumerate(xy_scatter_features), total=len(xy_scatter_features)):
+        feature = sampled_data[c_name]
         # if string, wrap when too long
         sch = SeriesSchema(feature)
         is_feature_string = True if (sch.is_string or sch.is_categorical_and_string) else False
         
         if is_feature_string:
-            tmp = feature[indices].str.slice(0, 12, 1)
-            fig = go.Scatter(x=tmp, y=y[indices], mode='markers', name=c_name, showlegend=False)
+            tmp = feature.str.slice(0, 12, 1)
+            fig = go.Scatter(x=tmp, y=y, mode='markers', name=c_name, showlegend=False)
         else:
-            fig = go.Scatter(x=feature[indices], y=y[indices], mode='markers', name=c_name, showlegend=False)
+            fig = go.Scatter(x=feature, y=y, mode='markers', name=c_name, showlegend=False)
 
         fig_list.add_trace(fig, row = int(idx / n_plot_per_row) + 1, col = ((idx % n_plot_per_row) + 1))
 
+    print("prepare xy scatter subplot completed, start to add them as one global plot")
     fig_list.update_layout(height=row_height * n_row, width=400 * n_col)
+    print("prepare xy scatter plot completed")
     
     return fig_list
 
 def draw_mapbox_plot(mapbox_scatter_features, feature_data):
     import plotly.graph_objs as go
 
     from shapely.geometry import MultiPoint
```

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/profilers/type_infer.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/profilers/type_infer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from pyrecdp.core import SeriesSchema
 from pyrecdp.primitives.operations import Operation
 import pandas as pd
 import numpy as np
 from pandas.api import types as pdt
 import copy
 from featuretools.primitives.base import TransformPrimitive
+from tqdm import tqdm
 
 def try_category(s):
     if pdt.is_categorical_dtype(s) and not pdt.is_bool_dtype(s):
         return False
     n_unique = s.nunique()
     total_len = len(s)
     threshold = (total_len / 5)
@@ -101,24 +102,24 @@
 class TypeInferFeatureGenerator():
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
    
     def fit_prepare(self, pipeline, children, max_idx, df):
         ret_pa_fields = []
         pa_schema = pipeline[children[0]].output
-        for pa_field, feature_name in zip(pa_schema, df.columns):
+        for pa_field, feature_name in tqdm(zip(pa_schema, df.columns), total=len(df.columns)):
             config = {}
             if try_datetime(df[feature_name]):
-                config['is_datetime'] = True            
-            elif try_numeric(df[feature_name]):
+                config['is_datetime'] = True
+            if try_category(df[feature_name]):
+                config['is_categorical'] = True
+            if try_numeric(df[feature_name]):
                 config['is_numeric'] = True
             elif try_re_numeric(df[feature_name]):
                 config['is_re_numeric'] = True
-            elif try_category(df[feature_name]):
-                config['is_categorical'] = True
             config['is_list_string'] = try_list_string(df[feature_name])
             if config['is_list_string'] is False:
                 skip = ('is_numeric' in config and config['is_numeric']) or ('is_re_numeric' in config and config['is_re_numeric'])
                 if not skip:
                     config['is_onehot'] = try_onehot(df[feature_name])
             
             pa_field.copy_config_from(config)
```

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/spark_data_processor/data_processor.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/spark_data_processor/data_processor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/spark_data_processor/encoder.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/spark_data_processor/encoder.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/primitives/spark_data_processor/utils.py` & `pyrecdp-1.0.1b202305181/pyrecdp/primitives/spark_data_processor/utils.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/widgets/BaseWidget.py` & `pyrecdp-1.0.1b202305181/pyrecdp/widgets/BaseWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/widgets/TabWidget.py` & `pyrecdp-1.0.1b202305181/pyrecdp/widgets/TabWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/widgets/TableViewWidget.py` & `pyrecdp-1.0.1b202305181/pyrecdp/widgets/TableViewWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/widgets/templates/base.html` & `pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/base.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/widgets/templates/overview.html` & `pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/overview.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/widgets/templates/scripts.html` & `pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/scripts.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/widgets/templates/styles.html` & `pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/styles.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp/widgets/templates/variables.html` & `pyrecdp-1.0.1b202305181/pyrecdp/widgets/templates/variables.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp.egg-info/PKG-INFO` & `pyrecdp-1.0.1b202305181/pyrecdp.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,222 +1,219 @@
 Metadata-Version: 2.1
 Name: pyrecdp
-Version: 1.0.1b202305161
+Version: 1.0.1b202305181
 Summary: A data processing bundle for spark based recommender system operations
 Home-page: https://github.com/intel/e2eAIOK/
 Author: INTEL AIA
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/
+Description: # RecDP v2.0
+        
+        # INTRODUCTION
+        
+        ## Problem Statement
+        
+        Data Preparation is an essential step to build AI pipelines 
+        * key data preparation capabilities: data connector, cleaning, sampling, joining, profiling, feature engineering, low-code/no-code UI, lineage etc. 
+        * exploration of optimal Data preparation consumes majority of Data Science time
+        
+        ## Solution with RecDP v2.0
+        
+        * Auto pipeline
+            * only 3 lines of codes required
+        * Pipeline Generator
+            * Data Profiling:
+                * Auto anomalies detection
+                * Auto missing value impute
+                * Profiling Visualizzation        
+            * Feature Wrangling:
+                * feature transformation(datetime, geo_info, text_nlp, url, etc.)
+                * multiple data auto joining
+                * feature cross(aggregation transformation - sum, avg, count, etc.)
+            * export pipeline as JSON file, can be import to other data platform
+        * Pipeline Runner:
+            * spark engine: convert pipeline to spark codes to run
+            * pandas engine: convert pipeline to pandas codes to run
+            * sql engine: convert pipeline to sql
+        * DataLoader:
+            * parquet, csv, json, database
+        * FeatureWriter - ML/DL connector:
+            * Data Lineage
+            * Feature Store
+            * numpy, csv, parquet, dgl / pyG graph
+        ![RecDP v2.0 Overview](resources/recdp_intro.png)
+        
+        ## This solution is intended for
+        citizen data scientists, enterprise users, independent software vendor and partial of cloud service provider.
+        
+        # Getting Start
+        ## setup with pip
+        ```
+        git clone --single-branch --branch RecDP_v2.0 https://github.com/intel-innersource/frameworks.bigdata.AIDK.git
+        cd frameworks.bigdata.AIDK/RecDP
+        # install dependencies
+        apt-get update -y &&  DEBIAN_FRONTEND=noninteractive apt-get install -y python3 python3-pip python-is-python3 graphviz
+        DEBIAN_FRONTEND=noninteractive apt-get install -y openjdk-8-jre
+        # install recdp
+        python setup.py sdist
+        pip install dist/pyrecdp-1.0.1.tar.gz
+        
+        sh start-jupyter.sh
+        # open browser with http://hostname:8888
+        ```
+        
+        ## run
+        ![nyc taxi demo](https://github.com/intel-innersource/frameworks.bigdata.AIDK/assets/4355494/03d8c2fe-de47-41f9-9fef-8513bc4aaf42)
+        
+        ## modify pipeline (add user defined function or remove operation)
+        ``` python
+        def filter_with_cond(df):
+            df = df[df['Year'] <= 2018]
+            return df
+        operation = {
+            "children": [6], # will to append this new op
+            "next": [7], # who will be connected to this new op
+            "inline_function": filter_with_cond, # function
+        }
+        pipeline.add_operation(operation)
+        ```
+        ``` python
+        operation = {
+            "idx": 6, # OP id to be deleted
+            "next": [10] # who is connected to the to_be_deleted op
+        }
+        pipeline.delete_operation(operation)
+        ```
+        
+        ## export pipeline
+        ``` python
+        pipeline.export(file_path = "exported_pipeline.json")
+        ```
+        ``` json
+        {
+            "0": {
+                "children": null,
+                "op": "DataFrame",
+                "config": "main_table"
+            },
+            "1": {
+                "children": [0],
+                "op": "type_infer",
+                "config": [
+                    ["pickup_datetime",["is_string","is_datetime"]],
+                    ["pickup_longitude",["is_numeric","is_float"]],
+                    ["pickup_latitude",["is_numeric","is_float"]],
+                    ["dropoff_longitude",["is_numeric","is_float"]],
+                    ["dropoff_latitude",["is_numeric","is_float"]],
+                    ["passenger_count",["is_numeric","is_int64","is_integer","is_categorical"]]
+                ]
+            },
+            "2": {
+                "children": [1],
+                "op": "tuple",
+                "config": {
+                    "src": ["pickup_latitude","pickup_longitude"],"dst": "pickup_coordinates"
+                }
+            },
+            "3": {
+                "children": [2],
+                "op": "tuple",
+                "config": {
+                    "src": ["dropoff_latitude","dropoff_longitude"],"dst": "dropoff_coordinates"
+                }
+            },
+            "4": {
+                "children": [3],
+                "op": "fillna",
+                "config": {
+                    "pickup_longitude": -1,
+                    "pickup_latitude": -1,
+                    "dropoff_longitude": -1,
+                    "dropoff_latitude": -1,
+                    "passenger_count": -1
+                }
+            },
+            "5": {
+                "children": [4],
+                "op": "datetime_feature",
+                "config": {
+                    "pickup_datetime": [
+                        ["pickup_datetime__day",["featuretools.primitives.standard.transform.datetime.day", "Day"]],
+                        ["pickup_datetime__month",["featuretools.primitives.standard.transform.datetime.month","Month"]],
+                        ["pickup_datetime__weekday",["featuretools.primitives.standard.transform.datetime.weekday","Weekday"]],
+                        ["pickup_datetime__year",["featuretools.primitives.standard.transform.datetime.year","Year"]],
+                        ["pickup_datetime__hour",["featuretools.primitives.standard.transform.datetime.hour","Hour"]]
+                    ]
+                }
+            },
+            "6": {
+                "children": [5],
+                "op": "haversine",
+                "config": {
+                    "['pickup_coordinates', 'dropoff_coordinates']": ["haversine_pickup_coordinates_dropoff_coordinates",["featuretools.primitives.standard.transform.latlong.haversine","Haversine"]]
+                }
+            },
+            "7": {
+                "children": [6],
+                "op": "drop",
+                "config": [
+                    "pickup_datetime",
+                    "pickup_coordinates",
+                    "dropoff_coordinates"
+                ]
+            },
+            "8": {
+                "children": [7],
+                "op": "lightgbm",
+                "config": {
+                    "label": "fare_amount",
+                    "metrics": "rmse",
+                    "objective": "regression",
+                    "model_file": "lightgbm_regression_label.mdl",
+                    "method": "predict"
+                }
+            }
+        }
+        ```
+        
+        
+        ## Quick Example
+        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/de044d606e6cdc44d3005db2a0ae968d/recdp_fare_prediction.ipynb) - [nyc taxi fare](examples/notebooks/autofe/demo/nyc_taxi_workflow_train.ipynb) - geographic, datetime, lgbm regression
+        
+        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/2b8acb3eda73028635072352560139ba/recdp_fraud_detect.ipynb) - [IBM Card Transaction Fraud Detect](examples/notebooks/autofe/demo/fraud_detect_train.ipynb) - onehot encode, lgbm, binary classification 
+        
+        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/b039b8c0a40fec951b1b09c3fbb93a7b/recdp_social_media.ipynb) - [twitter recsys](examples/notebooks/autofe/demo/twitter_workflow_test.ipynb) - text nlp, datetime feature engineering  
+        
+        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/1e08668ab0e15e1e98c592f284d79dad/recdp_click_through_rate_multiple_tables.ipynb) - [outbrain](examples/notebooks/autofe/demo/outbrain_ctr_workflow_test.ipynb) - multiple table joining
+        
+        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/2f942c30dbf9b63a64cc819a61966e34/recdp_rating_prediction_amazon_review.ipynb) - [amazon product review](examples/notebooks/autofe/demo/amazon_product_review_test.ipynb) - text nlp, datetime, feature-cross
+        
+        # More Examples - completed example including training
+        
+        ## Auto Feature Engineering vs. featuretools
+        * [NYC Taxi fare auto data prepration](examples/notebooks/autofe/FeatureWrangler.ipynb): An example to show how RecDP_v2.0 automatically generating datetime and geo features upon 55M records. Tested with both Spark and Pandas(featuretools) as compute engine, show 21x speedup by spark.
+        
+        ## load PIPELINE and execute
+        * [twitter pipeline re-load and execute](examples/notebooks/autofe/demo/custom_pipeline_twitter.ipynb): An example to show how RecDP_v2.0 reload pipeline from json and do execution - use RecDP as compute engine.
+        
+        ## Realtime Inference pipeline
+        * [nyc taxi fare](examples/notebooks/autofe/demo/nyc_taxi_workflow_predict.ipynb) - geographic, datetime feature engineering, lgbm
+        
+        ## Data Profiler Examples
+        * [NYC Taxi fare Profiler](resources/FeatureProfiler_NYC.png): An example to show RecDP_v2.0 to profile data, including infer the potential data type, generate data distribution charts.
+        
+        * [twitter Profiler](resources/FeatureProfiler_recsys.png): An example to show RecDP_v2.0 to profile data, including infer the potential data type, generate data distribution charts.
+        
+        
+        ## LICENSE
+        * Apache 2.0
+        
+        ## Dependency
+        * Spark 3.x
+        * python 3.*
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# RecDP v2.0
-
-# INTRODUCTION
-
-## Problem Statement
-
-Data Preparation is an essential step to build AI pipelines 
-* key data preparation capabilities: data connector, cleaning, sampling, joining, profiling, feature engineering, low-code/no-code UI, lineage etc. 
-* exploration of optimal Data preparation consumes majority of Data Science time
-
-## Solution with RecDP v2.0
-
-* Auto pipeline
-    * only 3 lines of codes required
-* Pipeline Generator
-    * Data Profiling:
-        * Auto anomalies detection
-        * Auto missing value impute
-        * Profiling Visualizzation        
-    * Feature Wrangling:
-        * feature transformation(datetime, geo_info, text_nlp, url, etc.)
-        * multiple data auto joining
-        * feature cross(aggregation transformation - sum, avg, count, etc.)
-    * export pipeline as JSON file, can be import to other data platform
-* Pipeline Runner:
-    * spark engine: convert pipeline to spark codes to run
-    * pandas engine: convert pipeline to pandas codes to run
-    * sql engine: convert pipeline to sql
-* DataLoader:
-    * parquet, csv, json, database
-* FeatureWriter - ML/DL connector:
-    * Data Lineage
-    * Feature Store
-    * numpy, csv, parquet, dgl / pyG graph
-![RecDP v2.0 Overview](resources/recdp_intro.png)
-
-## This solution is intended for
-citizen data scientists, enterprise users, independent software vendor and partial of cloud service provider.
-
-# Getting Start
-## setup with pip
-```
-git clone --single-branch --branch RecDP_v2.0 https://github.com/intel-innersource/frameworks.bigdata.AIDK.git
-cd frameworks.bigdata.AIDK/RecDP
-# install dependencies
-apt-get update -y &&  DEBIAN_FRONTEND=noninteractive apt-get install -y python3 python3-pip python-is-python3 graphviz
-DEBIAN_FRONTEND=noninteractive apt-get install -y openjdk-8-jre
-# install recdp
-python setup.py sdist
-pip install dist/pyrecdp-1.0.1.tar.gz
-
-sh start-jupyter.sh
-# open browser with http://hostname:8888
-```
-
-## run
-![nyc taxi demo](https://github.com/intel-innersource/frameworks.bigdata.AIDK/assets/4355494/03d8c2fe-de47-41f9-9fef-8513bc4aaf42)
-
-## modify pipeline (add user defined function or remove operation)
-``` python
-def filter_with_cond(df):
-    df = df[df['Year'] <= 2018]
-    return df
-operation = {
-    "children": [6], # will to append this new op
-    "next": [7], # who will be connected to this new op
-    "inline_function": filter_with_cond, # function
-}
-pipeline.add_operation(operation)
-```
-``` python
-operation = {
-    "idx": 6, # OP id to be deleted
-    "next": [10] # who is connected to the to_be_deleted op
-}
-pipeline.delete_operation(operation)
-```
-
-## export pipeline
-``` python
-pipeline.export(file_path = "exported_pipeline.json")
-```
-``` json
-{
-    "0": {
-        "children": null,
-        "op": "DataFrame",
-        "config": "main_table"
-    },
-    "1": {
-        "children": [0],
-        "op": "type_infer",
-        "config": [
-            ["pickup_datetime",["is_string","is_datetime"]],
-            ["pickup_longitude",["is_numeric","is_float"]],
-            ["pickup_latitude",["is_numeric","is_float"]],
-            ["dropoff_longitude",["is_numeric","is_float"]],
-            ["dropoff_latitude",["is_numeric","is_float"]],
-            ["passenger_count",["is_numeric","is_int64","is_integer","is_categorical"]]
-        ]
-    },
-    "2": {
-        "children": [1],
-        "op": "tuple",
-        "config": {
-            "src": ["pickup_latitude","pickup_longitude"],"dst": "pickup_coordinates"
-        }
-    },
-    "3": {
-        "children": [2],
-        "op": "tuple",
-        "config": {
-            "src": ["dropoff_latitude","dropoff_longitude"],"dst": "dropoff_coordinates"
-        }
-    },
-    "4": {
-        "children": [3],
-        "op": "fillna",
-        "config": {
-            "pickup_longitude": -1,
-            "pickup_latitude": -1,
-            "dropoff_longitude": -1,
-            "dropoff_latitude": -1,
-            "passenger_count": -1
-        }
-    },
-    "5": {
-        "children": [4],
-        "op": "datetime_feature",
-        "config": {
-            "pickup_datetime": [
-                ["pickup_datetime__day",["featuretools.primitives.standard.transform.datetime.day", "Day"]],
-                ["pickup_datetime__month",["featuretools.primitives.standard.transform.datetime.month","Month"]],
-                ["pickup_datetime__weekday",["featuretools.primitives.standard.transform.datetime.weekday","Weekday"]],
-                ["pickup_datetime__year",["featuretools.primitives.standard.transform.datetime.year","Year"]],
-                ["pickup_datetime__hour",["featuretools.primitives.standard.transform.datetime.hour","Hour"]]
-            ]
-        }
-    },
-    "6": {
-        "children": [5],
-        "op": "haversine",
-        "config": {
-            "['pickup_coordinates', 'dropoff_coordinates']": ["haversine_pickup_coordinates_dropoff_coordinates",["featuretools.primitives.standard.transform.latlong.haversine","Haversine"]]
-        }
-    },
-    "7": {
-        "children": [6],
-        "op": "drop",
-        "config": [
-            "pickup_datetime",
-            "pickup_coordinates",
-            "dropoff_coordinates"
-        ]
-    },
-    "8": {
-        "children": [7],
-        "op": "lightgbm",
-        "config": {
-            "label": "fare_amount",
-            "metrics": "rmse",
-            "objective": "regression",
-            "model_file": "lightgbm_regression_label.mdl",
-            "method": "predict"
-        }
-    }
-}
-```
-
-
-## Quick Example
-* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/de044d606e6cdc44d3005db2a0ae968d/recdp_fare_prediction.ipynb) - [nyc taxi fare](examples/notebooks/autofe/demo/nyc_taxi_workflow_train.ipynb) - geographic, datetime, lgbm regression
-
-* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/2b8acb3eda73028635072352560139ba/recdp_fraud_detect.ipynb) - [IBM Card Transaction Fraud Detect](examples/notebooks/autofe/demo/fraud_detect_train.ipynb) - onehot encode, lgbm, binary classification 
-
-* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/b039b8c0a40fec951b1b09c3fbb93a7b/recdp_social_media.ipynb) - [twitter recsys](examples/notebooks/autofe/demo/twitter_workflow_test.ipynb) - text nlp, datetime feature engineering  
-
-* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/1e08668ab0e15e1e98c592f284d79dad/recdp_click_through_rate_multiple_tables.ipynb) - [outbrain](examples/notebooks/autofe/demo/outbrain_ctr_workflow_test.ipynb) - multiple table joining
-
-* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/2f942c30dbf9b63a64cc819a61966e34/recdp_rating_prediction_amazon_review.ipynb) - [amazon product review](examples/notebooks/autofe/demo/amazon_product_review_test.ipynb) - text nlp, datetime, feature-cross
-
-# More Examples - completed example including training
-
-## Auto Feature Engineering vs. featuretools
-* [NYC Taxi fare auto data prepration](examples/notebooks/autofe/FeatureWrangler.ipynb): An example to show how RecDP_v2.0 automatically generating datetime and geo features upon 55M records. Tested with both Spark and Pandas(featuretools) as compute engine, show 21x speedup by spark.
-
-## load PIPELINE and execute
-* [twitter pipeline re-load and execute](examples/notebooks/autofe/demo/custom_pipeline_twitter.ipynb): An example to show how RecDP_v2.0 reload pipeline from json and do execution - use RecDP as compute engine.
-
-## Realtime Inference pipeline
-* [nyc taxi fare](examples/notebooks/autofe/demo/nyc_taxi_workflow_predict.ipynb) - geographic, datetime feature engineering, lgbm
-
-## Data Profiler Examples
-* [NYC Taxi fare Profiler](resources/FeatureProfiler_NYC.png): An example to show RecDP_v2.0 to profile data, including infer the potential data type, generate data distribution charts.
-
-* [twitter Profiler](resources/FeatureProfiler_recsys.png): An example to show RecDP_v2.0 to profile data, including infer the potential data type, generate data distribution charts.
-
-
-## LICENSE
-* Apache 2.0
-
-## Dependency
-* Spark 3.x
-* python 3.*
-
-
```

### Comparing `pyrecdp-1.0.1b202305161/pyrecdp.egg-info/SOURCES.txt` & `pyrecdp-1.0.1b202305181/pyrecdp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305161/setup.py` & `pyrecdp-1.0.1b202305181/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools.command.install import install
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name="pyrecdp",
-    version="1.0.1b202305161",
+    version="1.0.1b202305181",
     author="INTEL AIA",
     description=
     "A data processing bundle for spark based recommender system operations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = "https://github.com/intel/e2eAIOK/",
     project_urls={
@@ -46,9 +46,10 @@
         "shapely",
         "graphviz",
         "requests",
         "distro",
         "pyspark==3.3.1",
         "lightgbm",
         "jupyterlab",
-        "matplotlib"
+        "matplotlib",
+        "category_encoders"
         ])
```

