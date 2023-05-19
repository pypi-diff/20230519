# Comparing `tmp/chrislab-0.5.2.tar.gz` & `tmp/chrislab-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrislab-0.5.2.tar", last modified: Thu May 18 18:31:14 2023, max compression
+gzip compressed data, was "chrislab-0.5.3.tar", last modified: Fri May 19 20:53:27 2023, max compression
```

## Comparing `chrislab-0.5.2.tar` & `chrislab-0.5.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:31:14.963521 chrislab-0.5.2/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2023-05-14 13:51:34.000000 chrislab-0.5.2/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)      830 2023-05-18 18:31:14.963521 chrislab-0.5.2/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      291 2023-05-14 13:51:34.000000 chrislab-0.5.2/README.md
--rw-rw-r--   0 chris     (1000) chris     (1000)       81 2023-05-14 13:51:34.000000 chrislab-0.5.2/pyproject.toml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1203 2023-05-18 18:31:14.963521 chrislab-0.5.2/setup.cfg
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:31:14.959521 chrislab-0.5.2/src/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:31:14.959521 chrislab-0.5.2/src/chrislab/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/chrislab/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:31:14.959521 chrislab-0.5.2/src/chrislab/common/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/chrislab/common/__init__.py
--rwxrwxr-x   0 chris     (1000) chris     (1000)     7852 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/chrislab/common/downloader.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    12638 2023-05-16 05:20:42.000000 chrislab-0.5.2/src/chrislab/common/tokenizer_korbert.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    13164 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/chrislab/common/util.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:31:14.959521 chrislab-0.5.2/src/chrislab/language/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/chrislab/language/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1316 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/chrislab/language/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    14142 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/chrislab/language/converter.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     9408 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/chrislab/language/evaluater.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    39567 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/chrislab/language/finetuner.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6833 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/chrislab/language/modeling.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    14491 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/chrislab/language/predictor.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:31:14.959521 chrislab-0.5.2/src/chrislab.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)      830 2023-05-18 18:31:14.000000 chrislab-0.5.2/src/chrislab.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     1420 2023-05-18 18:31:14.000000 chrislab-0.5.2/src/chrislab.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-18 18:31:14.000000 chrislab-0.5.2/src/chrislab.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      164 2023-05-18 18:31:14.000000 chrislab-0.5.2/src/chrislab.egg-info/entry_points.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      249 2023-05-18 18:31:14.000000 chrislab-0.5.2/src/chrislab.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       17 2023-05-18 18:31:14.000000 chrislab-0.5.2/src/chrislab.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-18 18:31:14.000000 chrislab-0.5.2/src/chrislab.egg-info/zip-safe
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:31:14.963521 chrislab-0.5.2/src/nlpbook/
--rw-rw-r--   0 chris     (1000) chris     (1000)       95 2023-05-18 12:07:19.000000 chrislab-0.5.2/src/nlpbook/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     8521 2023-05-18 18:19:49.000000 chrislab-0.5.2/src/nlpbook/arguments.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:31:14.963521 chrislab-0.5.2/src/nlpbook/cls/
--rw-rw-r--   0 chris     (1000) chris     (1000)       59 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/cls/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     8870 2023-05-18 17:57:18.000000 chrislab-0.5.2/src/nlpbook/cls/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5208 2023-05-18 14:04:27.000000 chrislab-0.5.2/src/nlpbook/cls/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2674 2023-05-18 17:12:36.000000 chrislab-0.5.2/src/nlpbook/cls/task.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2246 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/data_utils.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3438 2023-05-18 17:45:48.000000 chrislab-0.5.2/src/nlpbook/factory.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:31:14.963521 chrislab-0.5.2/src/nlpbook/generation/
--rw-rw-r--   0 chris     (1000) chris     (1000)      170 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/generation/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4280 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/generation/arguments.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5371 2023-05-18 08:22:09.000000 chrislab-0.5.2/src/nlpbook/generation/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      882 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/generation/deploy.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1293 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/generation/task.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      653 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/metrics.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:31:14.963521 chrislab-0.5.2/src/nlpbook/ner/
--rw-rw-r--   0 chris     (1000) chris     (1000)       48 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/ner/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     8882 2023-05-18 17:57:18.000000 chrislab-0.5.2/src/nlpbook/ner/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    11551 2023-05-18 17:55:00.000000 chrislab-0.5.2/src/nlpbook/ner/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     8528 2023-05-18 16:39:33.000000 chrislab-0.5.2/src/nlpbook/ner/task.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:31:14.963521 chrislab-0.5.2/src/nlpbook/paircls/
--rw-rw-r--   0 chris     (1000) chris     (1000)       62 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/paircls/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2656 2023-05-18 08:22:04.000000 chrislab-0.5.2/src/nlpbook/paircls/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      641 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/paircls/deploy.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:31:14.963521 chrislab-0.5.2/src/nlpbook/qa/
--rw-rw-r--   0 chris     (1000) chris     (1000)      146 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/qa/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4984 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/qa/arguments.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    17104 2023-05-18 08:22:15.000000 chrislab-0.5.2/src/nlpbook/qa/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      639 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/qa/deploy.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2072 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/qa/task.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     8635 2023-05-18 15:44:30.000000 chrislab-0.5.2/src/nlpbook/utils.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-19 20:53:27.904633 chrislab-0.5.3/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2023-05-14 13:51:34.000000 chrislab-0.5.3/LICENSE
+-rw-rw-r--   0 chris     (1000) chris     (1000)      830 2023-05-19 20:53:27.904633 chrislab-0.5.3/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      291 2023-05-14 13:51:34.000000 chrislab-0.5.3/README.md
+-rw-rw-r--   0 chris     (1000) chris     (1000)       81 2023-05-14 13:51:34.000000 chrislab-0.5.3/pyproject.toml
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1203 2023-05-19 20:53:27.908633 chrislab-0.5.3/setup.cfg
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-19 20:53:27.900633 chrislab-0.5.3/src/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-19 20:53:27.900633 chrislab-0.5.3/src/chrislab/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/chrislab/__init__.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-19 20:53:27.904633 chrislab-0.5.3/src/chrislab/common/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/chrislab/common/__init__.py
+-rwxrwxr-x   0 chris     (1000) chris     (1000)     7852 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/chrislab/common/downloader.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    12638 2023-05-16 05:20:42.000000 chrislab-0.5.3/src/chrislab/common/tokenizer_korbert.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    13273 2023-05-19 19:44:22.000000 chrislab-0.5.3/src/chrislab/common/util.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-19 20:53:27.904633 chrislab-0.5.3/src/chrislab/language/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/chrislab/language/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1316 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/chrislab/language/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    14142 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/chrislab/language/converter.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9408 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/chrislab/language/evaluater.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    39567 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/chrislab/language/finetuner.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6833 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/chrislab/language/modeling.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    14491 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/chrislab/language/predictor.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-19 20:53:27.904633 chrislab-0.5.3/src/chrislab.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      830 2023-05-19 20:53:27.000000 chrislab-0.5.3/src/chrislab.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1420 2023-05-19 20:53:27.000000 chrislab-0.5.3/src/chrislab.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-19 20:53:27.000000 chrislab-0.5.3/src/chrislab.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      164 2023-05-19 20:53:27.000000 chrislab-0.5.3/src/chrislab.egg-info/entry_points.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      249 2023-05-19 20:53:27.000000 chrislab-0.5.3/src/chrislab.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       17 2023-05-19 20:53:27.000000 chrislab-0.5.3/src/chrislab.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-19 20:53:27.000000 chrislab-0.5.3/src/chrislab.egg-info/zip-safe
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-19 20:53:27.904633 chrislab-0.5.3/src/nlpbook/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       95 2023-05-18 12:07:19.000000 chrislab-0.5.3/src/nlpbook/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8521 2023-05-19 20:24:27.000000 chrislab-0.5.3/src/nlpbook/arguments.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-19 20:53:27.904633 chrislab-0.5.3/src/nlpbook/cls/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       59 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/cls/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8870 2023-05-18 17:57:18.000000 chrislab-0.5.3/src/nlpbook/cls/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5209 2023-05-19 20:51:20.000000 chrislab-0.5.3/src/nlpbook/cls/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2674 2023-05-18 17:12:36.000000 chrislab-0.5.3/src/nlpbook/cls/task.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2246 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/data_utils.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3438 2023-05-18 17:45:48.000000 chrislab-0.5.3/src/nlpbook/factory.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-19 20:53:27.904633 chrislab-0.5.3/src/nlpbook/generation/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      170 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/generation/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4280 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/generation/arguments.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5371 2023-05-18 08:22:09.000000 chrislab-0.5.3/src/nlpbook/generation/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      882 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/generation/deploy.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1293 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/generation/task.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      653 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/metrics.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-19 20:53:27.904633 chrislab-0.5.3/src/nlpbook/ner/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       48 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/ner/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8942 2023-05-19 20:51:19.000000 chrislab-0.5.3/src/nlpbook/ner/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    12626 2023-05-19 20:51:20.000000 chrislab-0.5.3/src/nlpbook/ner/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8534 2023-05-18 18:36:43.000000 chrislab-0.5.3/src/nlpbook/ner/task.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-19 20:53:27.904633 chrislab-0.5.3/src/nlpbook/paircls/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       62 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/paircls/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2656 2023-05-18 08:22:04.000000 chrislab-0.5.3/src/nlpbook/paircls/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      641 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/paircls/deploy.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-19 20:53:27.904633 chrislab-0.5.3/src/nlpbook/qa/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      146 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/qa/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4984 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/qa/arguments.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    17104 2023-05-18 08:22:15.000000 chrislab-0.5.3/src/nlpbook/qa/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      639 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/qa/deploy.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2072 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/qa/task.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8635 2023-05-18 15:44:30.000000 chrislab-0.5.3/src/nlpbook/utils.py
```

### Comparing `chrislab-0.5.2/LICENSE` & `chrislab-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/PKG-INFO` & `chrislab-0.5.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrislab
-Version: 0.5.2
+Version: 0.5.3
 Summary: An advanced tool for doing experimental study.
 Home-page: https://github.com/chrisjihee/chrislab
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chrislab-0.5.2/setup.cfg` & `chrislab-0.5.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chrislab
-version = 0.5.2
+version = 0.5.3
 author = Jihee Ryu
 author_email = chrisjihee@naver.com
 url = https://github.com/chrisjihee/chrislab
 description = An advanced tool for doing experimental study.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
```

### Comparing `chrislab-0.5.2/src/chrislab/common/downloader.py` & `chrislab-0.5.3/src/chrislab/common/downloader.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/src/chrislab/common/tokenizer_korbert.py` & `chrislab-0.5.3/src/chrislab/common/tokenizer_korbert.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/src/chrislab/common/util.py` & `chrislab-0.5.3/src/chrislab/common/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 def cuda_visible_devices(gpus=None):
     if gpus:
         os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
         os.environ["CUDA_VISIBLE_DEVICES"] = gpus
     return os.environ.get("CUDA_VISIBLE_DEVICES")
 
 
+def set_tokenizers_parallelism(value=False):
+    os.environ["TOKENIZERS_PARALLELISM"] = f"{value}".lower()
+
+
 def num_cuda_devices():
     from torch.cuda import _device_count_nvml
     nvml_count = _device_count_nvml()
     if nvml_count >= 0:
         return nvml_count
     else:
         return torch.cuda.device_count()
```

### Comparing `chrislab-0.5.2/src/chrislab/language/cli.py` & `chrislab-0.5.3/src/chrislab/language/cli.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/src/chrislab/language/converter.py` & `chrislab-0.5.3/src/chrislab/language/converter.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/src/chrislab/language/evaluater.py` & `chrislab-0.5.3/src/chrislab/language/evaluater.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/src/chrislab/language/finetuner.py` & `chrislab-0.5.3/src/chrislab/language/finetuner.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/src/chrislab/language/modeling.py` & `chrislab-0.5.3/src/chrislab/language/modeling.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/src/chrislab/language/predictor.py` & `chrislab-0.5.3/src/chrislab/language/predictor.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/src/chrislab.egg-info/PKG-INFO` & `chrislab-0.5.3/src/chrislab.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrislab
-Version: 0.5.2
+Version: 0.5.3
 Summary: An advanced tool for doing experimental study.
 Home-page: https://github.com/chrisjihee/chrislab
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chrislab-0.5.2/src/chrislab.egg-info/SOURCES.txt` & `chrislab-0.5.3/src/chrislab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/src/nlpbook/arguments.py` & `chrislab-0.5.3/src/nlpbook/arguments.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/src/nlpbook/cls/cli.py` & `chrislab-0.5.3/src/nlpbook/cls/cli.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/src/nlpbook/cls/corpus.py` & `chrislab-0.5.3/src/nlpbook/cls/corpus.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         assert args.data.home, f"No data_home: {args.data.home}"
         assert args.data.name, f"No data_name: {args.data.name}"
         data_file_dict: dict = args.data.files.to_dict()
         assert split in data_file_dict, f"No '{split}' split in data_file: should be one of {list(data_file_dict.keys())}"
         assert data_file_dict[split], f"No data_file for '{split}' split: {args.data.files}"
         text_data_path: Path = Path(args.data.home) / args.data.name / data_file_dict[split]
         cache_data_path = text_data_path \
-            .with_stem(text_data_path.stem + f"-by-{tokenizer.__class__.__name__}-with-{args.model.max_seq_length}") \
+            .with_stem(text_data_path.stem + f"-by-{tokenizer.__class__.__name__}-as-{args.model.max_seq_length}seq") \
             .with_suffix(".cache")
         cache_lock_path = cache_data_path.with_suffix(".lock")
 
         with FileLock(cache_lock_path):
             if os.path.exists(cache_data_path) and args.data.caching:
                 start = time.time()
                 self.features = torch.load(cache_data_path)
```

### Comparing `chrislab-0.5.2/src/nlpbook/cls/task.py` & `chrislab-0.5.3/src/nlpbook/cls/task.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/src/nlpbook/data_utils.py` & `chrislab-0.5.3/src/nlpbook/data_utils.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/src/nlpbook/factory.py` & `chrislab-0.5.3/src/nlpbook/factory.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/src/nlpbook/generation/arguments.py` & `chrislab-0.5.3/src/nlpbook/generation/arguments.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/src/nlpbook/generation/corpus.py` & `chrislab-0.5.3/src/nlpbook/generation/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/src/nlpbook/generation/deploy.py` & `chrislab-0.5.3/src/nlpbook/generation/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/src/nlpbook/generation/task.py` & `chrislab-0.5.3/src/nlpbook/generation/task.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/src/nlpbook/metrics.py` & `chrislab-0.5.3/src/nlpbook/metrics.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/src/nlpbook/ner/cli.py` & `chrislab-0.5.3/src/nlpbook/ner/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from typer import Typer
 
 import nlpbook
 from chrisbase.io import JobTimer, err_hr
 from nlpbook.arguments import TrainerArguments, ServerArguments, TesterArguments, RuntimeChecking
 from nlpbook.ner.corpus import NERCorpus, NERDataset
 from nlpbook.ner.task import NERTask
-from transformers import BertConfig, BertForTokenClassification, BertTokenizer
+from transformers import BertConfig, BertForTokenClassification, PreTrainedTokenizerFast, AutoTokenizer
 from transformers.modeling_outputs import TokenClassifierOutput
 
 app = Typer()
 logger = logging.getLogger("nlpbook")
 
 
 @app.command()
@@ -26,21 +26,22 @@
     nlpbook.set_logger()
     args_file = Path(args_file)
     assert args_file.exists(), f"No args_file: {args_file}"
     args: TrainerArguments = TrainerArguments.from_json(args_file.read_text()).show()
     nlpbook.set_seed(args)
 
     with JobTimer(f"chrialab.nlpbook.ner train {args_file}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
-        nlpbook.download_downstream_dataset(args)
-        err_hr(c='-')
+        if args.data.redownload:
+            nlpbook.download_downstream_dataset(args)
+            err_hr(c='-')
 
         corpus = NERCorpus(args)
-        # tokenizer: PreTrainedTokenizerFast = AutoTokenizer.from_pretrained(args.model.pretrained, do_lower_case=False, use_fast=True)
-        # assert isinstance(tokenizer, PreTrainedTokenizerFast), f"tokenizer is not PreTrainedTokenizerFast: {type(tokenizer)}"
-        tokenizer: BertTokenizer = BertTokenizer.from_pretrained(args.model.pretrained, do_lower_case=False)
+        tokenizer: PreTrainedTokenizerFast = AutoTokenizer.from_pretrained(args.model.pretrained, do_lower_case=False, use_fast=True)
+        assert isinstance(tokenizer, PreTrainedTokenizerFast), f"tokenizer is not PreTrainedTokenizerFast: {type(tokenizer)}"
+        # tokenizer: BertTokenizer = BertTokenizer.from_pretrained(args.model.pretrained, do_lower_case=False)
         train_dataset = NERDataset("train", args=args, corpus=corpus, tokenizer=tokenizer)
         train_dataloader = DataLoader(train_dataset,
                                       batch_size=args.hardware.batch_size,
                                       num_workers=args.hardware.cpu_workers,
                                       sampler=RandomSampler(train_dataset, replacement=False),
                                       collate_fn=nlpbook.data_collator,
                                       drop_last=False)
@@ -86,17 +87,17 @@
         logger.info(f"Using finetuned checkpoint file at {checkpoint_path}")
         err_hr(c='-')
 
         nlpbook.download_downstream_dataset(args)
         err_hr(c='-')
 
         corpus = NERCorpus(args)
-        # tokenizer: PreTrainedTokenizerFast = AutoTokenizer.from_pretrained(args.model.pretrained, do_lower_case=False, use_fast=True)
-        # assert isinstance(tokenizer, PreTrainedTokenizerFast), f"tokenizer is not PreTrainedTokenizerFast: {type(tokenizer)}"
-        tokenizer: BertTokenizer = BertTokenizer.from_pretrained(args.model.pretrained, do_lower_case=False)
+        tokenizer: PreTrainedTokenizerFast = AutoTokenizer.from_pretrained(args.model.pretrained, do_lower_case=False, use_fast=True)
+        assert isinstance(tokenizer, PreTrainedTokenizerFast), f"tokenizer is not PreTrainedTokenizerFast: {type(tokenizer)}"
+        # tokenizer: BertTokenizer = BertTokenizer.from_pretrained(args.model.pretrained, do_lower_case=False)
         test_dataset = NERDataset("test", args=args, corpus=corpus, tokenizer=tokenizer)
         test_dataloader = DataLoader(test_dataset,
                                      batch_size=args.hardware.batch_size,
                                      num_workers=args.hardware.cpu_workers,
                                      sampler=SequentialSampler(test_dataset),
                                      collate_fn=nlpbook.data_collator,
                                      drop_last=False)
@@ -130,17 +131,17 @@
     with JobTimer(f"chrialab.nlpbook serve_ner {args_file}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
         checkpoint_path = args.output.dir_path / args.model.finetuning_name
         assert checkpoint_path.exists(), f"No checkpoint file: {checkpoint_path}"
         checkpoint: dict = torch.load(checkpoint_path, map_location=torch.device("cpu"))
         logger.info(f"Using finetuned checkpoint file at {checkpoint_path}")
         err_hr(c='-')
 
-        # tokenizer: PreTrainedTokenizerFast = AutoTokenizer.from_pretrained(args.model.pretrained, do_lower_case=False, use_fast=True)
-        # assert isinstance(tokenizer, PreTrainedTokenizerFast), f"tokenizer is not PreTrainedTokenizerFast: {type(tokenizer)}"
-        tokenizer: BertTokenizer = BertTokenizer.from_pretrained(args.model.pretrained, do_lower_case=False)
+        tokenizer: PreTrainedTokenizerFast = AutoTokenizer.from_pretrained(args.model.pretrained, do_lower_case=False, use_fast=True)
+        assert isinstance(tokenizer, PreTrainedTokenizerFast), f"tokenizer is not PreTrainedTokenizerFast: {type(tokenizer)}"
+        # tokenizer: BertTokenizer = BertTokenizer.from_pretrained(args.model.pretrained, do_lower_case=False)
         label_map_path: Path = args.output.dir_path / "label_map.txt"
         assert label_map_path.exists(), f"No downstream label file: {label_map_path}"
         labels = label_map_path.read_text().splitlines(keepends=False)
         id_to_label = {idx: label for idx, label in enumerate(labels)}
 
         pretrained_model_config = BertConfig.from_pretrained(
             args.model.pretrained,
```

### Comparing `chrislab-0.5.2/src/nlpbook/ner/corpus.py` & `chrislab-0.5.3/src/nlpbook/ner/corpus.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,259 +1,184 @@
 import logging
 import os
 import re
 import time
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from pathlib import Path
-from typing import List, Optional
+from typing import List, Optional, ClassVar
 
 import torch
+from dataclasses_json import DataClassJsonMixin
 from filelock import FileLock
 from torch.utils.data.dataset import Dataset
 
-from chrisbase.io import make_parent_dir
-from nlpbook.arguments import TrainerArguments, TesterArguments
-from transformers import BertTokenizer
-from transformers.tokenization_utils_base import PaddingStrategy, TruncationStrategy
+from chrisbase.io import make_parent_dir, files, merge_dicts
+from nlpbook.arguments import TesterArguments
+from transformers import PreTrainedTokenizerFast
+from transformers.tokenization_utils_base import CharSpan
+from transformers.tokenization_utils_base import PaddingStrategy, TruncationStrategy, BatchEncoding
 
 logger = logging.getLogger("nlpbook")
 
-# 자체 제작 NER 코퍼스 기준의 레이블 시퀀스를 만들기 위한 ID 체계
-# 나 는 삼성 에 입사 했다
-# O O 기관 O O O > [CLS] O O 기관 O O O [SEP] [PAD] [PAD] ...
 NER_CLS_TOKEN = "[CLS]"
 NER_SEP_TOKEN = "[SEP]"
 NER_PAD_TOKEN = "[PAD]"
 NER_MASK_TOKEN = "[MASK]"
 NER_PAD_ID = 2
 
 
 @dataclass
-class NERExample:
+class EntityInText(DataClassJsonMixin):
+    pattern: ClassVar[re.Pattern] = re.compile('<([^<>]+?):([A-Z]{2,3})>')
     text: str
-    label: Optional[str] = None
+    label: str
+    offset: tuple[int, int]
+
+    @staticmethod
+    def from_match(m: re.Match, s: str) -> tuple["EntityInText", str]:
+        x = m.group(1)
+        y = m.group(2)
+        z = (m.start(), m.start() + len(x))
+        e = EntityInText(text=x, label=y, offset=z)
+        s = s[:m.start()] + m.group(1) + s[m.end():]
+        return e, s
+
+    def to_offset_lable_dict(self) -> dict[int, str]:
+        offset_list = [(self.offset[0], f"B-{self.label}")]
+        for i in range(self.offset[0] + 1, self.offset[1]):
+            offset_list.append((i, f"I-{self.label}"))
+        return dict(offset_list)
+
+
+@dataclass
+class NERExampleForKLUE(DataClassJsonMixin):
+    origin: str = field(default_factory=str)
+    entity_list: list[EntityInText] = field(default_factory=list)
+    character_list: list[tuple[str, str]] = field(default_factory=list)
 
 
 @dataclass
 class NERFeatures:
     input_ids: List[int]
     attention_mask: Optional[List[int]] = None
     token_type_ids: Optional[List[int]] = None
     label_ids: Optional[List[int]] = None
 
 
 class NERCorpus:
-
-    def __init__(
-            self,
-            args: TrainerArguments | TesterArguments,
-    ):
+    def __init__(self, args: TesterArguments):
         self.args = args
 
-    def get_examples(self, data_path):
-        logger.info(f"loading data from {data_path}...")
+    def get_examples(self, data_path: Path) -> List[NERExampleForKLUE]:
         examples = []
-        for line in open(data_path, "r", encoding="utf-8").readlines():
-            text, label = line.split("\u241E")
-            examples.append(NERExample(text=text, label=label))
+        with data_path.open(encoding="utf-8") as inp:
+            for line in inp.readlines():
+                examples.append(NERExampleForKLUE.from_json(line))
+        logger.info(f"Loaded {len(examples)} {examples[0].__class__.__name__} from {data_path}")
         return examples
 
     def get_labels(self):
         label_map_path = make_parent_dir(self.args.output.dir_path / "label_map.txt")
         if not label_map_path.exists():
-            logger.info("processing NER tag dictionary...")
-            os.makedirs(self.args.model.finetuning_home, exist_ok=True)
             ner_tags = []
-            regex_ner = re.compile('<(.+?):[A-Z]{3}>')
-            train_corpus_path = self.args.data.home / self.args.data.name / "train.txt"
-            target_sentences = [line.split("\u241E")[1].strip()
-                                for line in train_corpus_path.open("r", encoding="utf-8").readlines()]
-            for target_sentence in target_sentences:
-                regex_filter_res = regex_ner.finditer(target_sentence)
-                for match_item in regex_filter_res:
-                    ner_tag = match_item[0][-4:-1]
-                    if ner_tag not in ner_tags:
-                        ner_tags.append(ner_tag)
+            train_data_path: Path = self.args.data.home / self.args.data.name / self.args.data.files.train
+            with train_data_path.open(encoding="utf-8") as inp:
+                for line in inp.readlines():
+                    for x in NERExampleForKLUE.from_json(line).entity_list:
+                        if x.label not in ner_tags:
+                            ner_tags.append(x.label)
             b_tags = [f"B-{ner_tag}" for ner_tag in ner_tags]
             i_tags = [f"I-{ner_tag}" for ner_tag in ner_tags]
             labels = [NER_CLS_TOKEN, NER_SEP_TOKEN, NER_PAD_TOKEN, NER_MASK_TOKEN, "O"] + b_tags + i_tags
             with label_map_path.open("w", encoding="utf-8") as f:
-                for tag in labels:
-                    f.writelines(tag + "\n")
+                f.writelines([x + "\n" for x in labels])
         else:
-            labels = [tag.strip() for tag in open(label_map_path, "r", encoding="utf-8").readlines()]
+            labels = [label.strip() for label in label_map_path.open(encoding="utf-8").readlines()]
+        logger.info(f"Loaded {len(labels)} labels from {label_map_path}")
         return labels
 
     @property
     def num_labels(self):
         return len(self.get_labels())
 
 
-def _process_target_sentence(
-        tokens: List[str],
-        origin_sentence: str,
-        target_sentence: str,
-        max_length: int,
-        label_map: dict,
-        tokenizer: BertTokenizer,
-        cls_token_at_end: Optional[bool] = False,
-):
-    """
-    target_sentence = "―<효진:PER> 역의 <김환희:PER>(<14:NOH>)가 특히 인상적이었다."
-    tokens = ["―", "효", "##진", "역", "##의", "김", "##환", "##희",
-              "(", "14", ")", "가", "특히", "인상", "##적이", "##었다", "."]
-    label_sequence = ['O', 'B-PER', 'I-PER', 'O', 'O', 'B-PER', 'I-PER', 'I-PER', 'O',
-                      'B-NOH', 'O', 'O', 'O', 'O', 'O', 'O', 'O']
-    """
-    if "[UNK]" in tokens:
-        processed_tokens = []
-        basic_tokens = tokenizer.basic_tokenizer.tokenize(origin_sentence)
-        for basic_token in basic_tokens:
-            current_tokens = tokenizer.tokenize(basic_token)
-            if "[UNK]" in current_tokens:
-                # [UNK] 복원
-                processed_tokens.append(basic_token)
-            else:
-                processed_tokens.extend(current_tokens)
-    else:
-        processed_tokens = tokens
-
-    prefix_sum_of_token_start_index, sum = [0], 0
-    for i, token in enumerate(processed_tokens):
-        if token.startswith("##"):
-            sum += len(token) - 2
-        else:
-            sum += len(token)
-        prefix_sum_of_token_start_index.append(sum)
-
-    regex_ner = re.compile('<(.+?):[A-Z]{3}>')  # NER Tag가 2자리 문자면 {3} -> {2}로 변경 (e.g. LOC -> LC) 인경우
-    regex_filter_res = regex_ner.finditer(target_sentence.replace(" ", ""))
-
-    list_of_ner_tag = []
-    list_of_ner_text = []
-    list_of_tuple_ner_start_end = []
-
-    count_of_match = 0
-    for match_item in regex_filter_res:
-        ner_tag = match_item[0][-4:-1]  # <4일간:DUR> -> DUR
-        ner_text = match_item[1]  # <4일간:DUR> -> 4일간
-        start_index = match_item.start() - 6 * count_of_match  # delete previous '<, :, 3 words tag name, >'
-        end_index = match_item.end() - 6 - 6 * count_of_match
-
-        list_of_ner_tag.append(ner_tag)
-        list_of_ner_text.append(ner_text)
-        list_of_tuple_ner_start_end.append((start_index, end_index))
-        count_of_match += 1
-
-    label_sequence = []
-    entity_index = 0
-    is_entity_still_B = True
-
-    for tup in zip(processed_tokens, prefix_sum_of_token_start_index):
-        token, index = tup
-
-        if entity_index < len(list_of_tuple_ner_start_end):
-            start, end = list_of_tuple_ner_start_end[entity_index]
-
-            if end < index:  # 엔티티 범위보다 현재 seq pos가 더 크면 다음 엔티티를 꺼내서 체크
-                is_entity_still_B = True
-                entity_index = entity_index + 1 if entity_index + 1 < len(list_of_tuple_ner_start_end) else entity_index
-                start, end = list_of_tuple_ner_start_end[entity_index]
-
-            if start <= index and index < end:  # <13일:DAT>까지 -> ('▁13', 10, 'B-DAT') ('일까지', 12, 'I-DAT') 이런 경우가 포함됨, 포함 안시키려면 토큰의 length도 계산해서 제어해야함
-                entity_tag = list_of_ner_tag[entity_index]
-                if is_entity_still_B is True:
-                    entity_tag = 'B-' + entity_tag
-                    label_sequence.append(entity_tag)
-                    is_entity_still_B = False
-                else:
-                    entity_tag = 'I-' + entity_tag
-                    label_sequence.append(entity_tag)
-            else:
-                is_entity_still_B = True
-                entity_tag = 'O'
-                label_sequence.append(entity_tag)
-        else:
-            entity_tag = 'O'
-            label_sequence.append(entity_tag)
-
-    # truncation
-    label_sequence = label_sequence[:max_length - 2]
-
-    # add special tokens
-    if cls_token_at_end:
-        label_sequence = label_sequence + [NER_CLS_TOKEN, NER_SEP_TOKEN]
-    else:
-        label_sequence = [NER_CLS_TOKEN] + label_sequence + [NER_SEP_TOKEN]
-
-    # padding
-    pad_length = max(max_length - len(label_sequence), 0)
-    pad_sequence = [NER_PAD_TOKEN] * pad_length
-    label_sequence += pad_sequence
-
-    # encoding
-    label_ids = [label_map[label] for label in label_sequence]
-    return label_ids
+def _decide_span_label(span: CharSpan, offset_to_label: dict[int, str]):
+    for x in [offset_to_label[i] for i in range(span.start, span.end)]:
+        if x.startswith("B-") or x.startswith("I-"):
+            return x
+    return "O"
 
 
 def _convert_examples_to_ner_features(
-        examples: List[NERExample],
-        tokenizer: BertTokenizer,
-        args: TrainerArguments,
+        examples: List[NERExampleForKLUE],
+        tokenizer: PreTrainedTokenizerFast,
+        args: TesterArguments,
         label_list: List[str],
         cls_token_at_end: Optional[bool] = False,
+        num_show_example: int = 3,
 ):
     """
     `cls_token_at_end` define the location of the CLS token:
             - False (Default, BERT/XLM pattern): [CLS] + A + [SEP] + B + [SEP]
             - True (XLNet/GPT pattern): A + [SEP] + B + [SEP] + [CLS]
     """
-    label_map = {label: i for i, label in enumerate(label_list)}
+    label_to_id = {label: i for i, label in enumerate(label_list)}
     id_to_label = {i: label for i, label in enumerate(label_list)}
 
-    features = []
+    features: list[NERFeatures] = []
     for example in examples:
-        tokens = tokenizer.tokenize(example.text)
-        inputs = tokenizer._encode_plus(
-            tokens,
-            max_length=args.model.max_seq_length,
-            truncation_strategy=TruncationStrategy.LONGEST_FIRST,
-            padding_strategy=PaddingStrategy.MAX_LENGTH,
-        )
-        label_ids = _process_target_sentence(
-            tokens=tokens,
-            origin_sentence=example.text,
-            target_sentence=example.label,
-            max_length=args.model.max_seq_length,
-            label_map=label_map,
-            tokenizer=tokenizer,
-            cls_token_at_end=cls_token_at_end,
-        )
+        example: NERExampleForKLUE = example
+        offset_to_label: dict[int, str] = {i: y for i, (_, y) in enumerate(example.character_list)}
+        inputs: BatchEncoding = tokenizer.encode_plus(example.origin,
+                                                      max_length=args.model.max_seq_length,
+                                                      truncation=TruncationStrategy.LONGEST_FIRST,
+                                                      padding=PaddingStrategy.MAX_LENGTH)
+        input_tokens: List[str] = inputs.tokens()
+        # out_hr()
+        # print(f"offset_to_label        = {offset_to_label}")
+        # out_hr()
+        # print(f"input_tokens           = {inputs.tokens()}")
+        # out_hr()
+        # for key in inputs.keys():
+        #     print(f"inputs[{key:14s}] = {inputs[key]}")
+        # out_hr()
+
+        label_list: list[str] = []
+        for i in range(args.model.max_seq_length):
+            token = input_tokens[i]
+            token_span: CharSpan = inputs.token_to_chars(i)
+            if token_span:
+                token_label = _decide_span_label(token_span, offset_to_label)
+                label_list.append(token_label)
+                # token_str = example.origin[token_span.start:token_span.end]
+                # print('\t'.join(map(str, [i, token, token_span, token_str, token_label])))
+            else:
+                label_list.append(token)
+                # print('\t'.join(map(str, [i, token, token_span])))
+        label_ids: list[int] = [label_to_id[label] for label in label_list]
         features.append(NERFeatures(**inputs, label_ids=label_ids))
-
-    for i, example in enumerate(examples[:3]):
-        logger.info("*** Example ***")
-        logger.info("sentence: %s" % (example.text))
-        logger.info("target: %s" % (example.label))
-        logger.info("tokens: %s" % (" ".join(tokenizer.convert_ids_to_tokens(features[i].input_ids))))
-        logger.info("label: %s" % (" ".join([id_to_label[label_id] for label_id in features[i].label_ids])))
-        logger.info("features: %s" % features[i])
+        # print(f"label_list             = {label_list}")
+        # out_hr()
+        # print(f"label_ids              = {label_ids}")
+        # print(f"features               = {features[-1]}")
+
+    for i, example in enumerate(examples[:num_show_example]):
+        logger.info("  === [Example %d] ===" % (i + 1))
+        logger.info("  = sentence : %s" % example.origin)
+        logger.info("  = entities : %s" % example.entity_list)
+        logger.info("  = tokens   : %s" % (" ".join(tokenizer.convert_ids_to_tokens(features[i].input_ids))))
+        logger.info("  = labels   : %s" % (" ".join([id_to_label[label_id] for label_id in features[i].label_ids])))
+        logger.info("  = features : %s" % features[i])
+        logger.info("  === ")
 
     return features
 
 
 class NERDataset(Dataset):
-    def __init__(
-            self,
-            split: str,
-            args: TrainerArguments | TesterArguments,
-            tokenizer: BertTokenizer,
-            corpus: NERCorpus,
-            convert_examples_to_features_fn=_convert_examples_to_ner_features,
-    ):
+    def __init__(self, split: str, args: TesterArguments, tokenizer: PreTrainedTokenizerFast, corpus: NERCorpus):
         assert corpus, "corpus is not valid"
         self.corpus = corpus
 
         assert args.data.home, f"No data_home: {args.data.home}"
         assert args.data.name, f"No data_name: {args.data.name}"
         data_file_dict: dict = args.data.files.to_dict()
         assert split in data_file_dict, f"No '{split}' split in data_file: should be one of {list(data_file_dict.keys())}"
@@ -269,21 +194,100 @@
                 start = time.time()
                 self.features = torch.load(cache_data_path)
                 logger.info(f"Loading features from cached file at {cache_data_path} [took {time.time() - start:.3f} s]")
             else:
                 assert text_data_path.exists() and text_data_path.is_file(), f"No data_text_path: {text_data_path}"
                 logger.info(f"Creating features from dataset file at {text_data_path}")
                 examples = self.corpus.get_examples(text_data_path)
-                self.features = convert_examples_to_features_fn(examples, tokenizer, args, label_list=self.corpus.get_labels())
+                self.features = _convert_examples_to_ner_features(examples, tokenizer, args, label_list=self.corpus.get_labels())
                 start = time.time()
-                logger.info("Saving features into cached file, it could take a lot of time...")
                 torch.save(self.features, cache_data_path)
                 logger.info(f"Saving features into cached file at {cache_data_path} [took {time.time() - start:.3f} s]")
 
     def __len__(self):
         return len(self.features)
 
     def __getitem__(self, i):
         return self.features[i]
 
     def get_labels(self):
         return self.corpus.get_labels()
+
+
+def _parse_tagged(origin: str, tagged: str, debug: bool = False) -> Optional[NERExampleForKLUE]:
+    entity_list: list[EntityInText] = []
+    if debug:
+        print(f"* origin: {origin}")
+        print(f"  tagged: {tagged}")
+    restored = tagged[:]
+    no_problem = True
+    offset_labels = {i: "O" for i in range(len(origin))}
+    while True:
+        match: re.Match = EntityInText.pattern.search(restored)
+        if not match:
+            break
+        entity, restored = EntityInText.from_match(match, restored)
+        extracted = origin[entity.offset[0]:entity.offset[1]]
+        if entity.text == extracted:
+            entity_list.append(entity)
+            offset_labels = merge_dicts(offset_labels, entity.to_offset_lable_dict())
+        else:
+            no_problem = False
+        if debug:
+            print(f"  = {entity} -> {extracted}")
+            # print(f"    {offset_labels}")
+    if debug:
+        print(f"  --------------------")
+    character_list = [(origin[i], offset_labels[i]) for i in range(len(origin))]
+    if restored != origin:
+        no_problem = False
+    return NERExampleForKLUE(origin, entity_list, character_list) if no_problem else None
+
+
+def convert_kmou_format(infile: str | Path, outfile: str | Path, debug: bool = False):
+    with Path(infile).open(encoding="utf-8") as inp, Path(outfile).open("w", encoding="utf-8") as out:
+        for line in inp.readlines():
+            origin, tagged = line.strip().split("\u241E")
+            parsed: Optional[NERExampleForKLUE] = _parse_tagged(origin, tagged, debug=debug)
+            if parsed:
+                out.write(parsed.to_json(ensure_ascii=False) + "\n")
+
+
+def convert_klue_format(infile: str | Path, outfile: str | Path, debug: bool = False):
+    with Path(infile) as inp, Path(outfile).open("w", encoding="utf-8") as out:
+        raw_text = inp.read_text(encoding="utf-8").strip()
+        raw_docs = re.split(r"\n\t?\n", raw_text)
+        for raw_doc in raw_docs:
+            raw_lines = raw_doc.splitlines()
+            num_header = 0
+            for line in raw_lines:
+                if not line.startswith("##"):
+                    break
+                num_header += 1
+            head_lines = raw_lines[:num_header]
+            body_lines = raw_lines[num_header:]
+
+            origin = ''.join(x.split("\t")[0] for x in body_lines)
+            tagged = head_lines[-1].split("\t")[1].strip()
+            parsed: Optional[NERExampleForKLUE] = _parse_tagged(origin, tagged, debug=debug)
+            if parsed:
+                character_list_from_head = parsed.character_list
+                character_list_from_body = [tuple(x.split("\t")) for x in body_lines]
+                if character_list_from_head == character_list_from_body:
+                    out.write(parsed.to_json(ensure_ascii=False) + "\n")
+                elif debug:
+                    print(f"* origin: {origin}")
+                    print(f"  tagged: {tagged}")
+                    for a, b in zip(character_list_from_head, character_list_from_body):
+                        if a != b:
+                            print(f"  = {a[0]}:{a[1]} <=> {b[0]}:{b[1]}")
+                    print(f"  ====================")
+
+
+if __name__ == "__main__":
+    for path in files("data/kmou-ner-full/*.txt"):
+        print(f"[FILE]: {path}")
+        convert_kmou_format(path, path.with_suffix(".jsonl"), debug=True)
+
+    # for path in files("data/klue-ner/*.tsv"):
+    #     print(f"[FILE]: {path}")
+    #     convert_klue_format(path, path.with_suffix(".jsonl"), debug=True)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `chrislab-0.5.2/src/nlpbook/ner/task.py` & `chrislab-0.5.3/src/nlpbook/ner/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,28 +42,29 @@
         return {"loss": outputs.loss, "acc": acc}
 
     def validation_step(self, inputs, batch_idx):
         outputs: TokenClassifierOutput = self.model(**inputs)
         preds = outputs.logits.argmax(dim=-1)
         labels = inputs["labels"]
         acc = accuracy(preds, labels, ignore_index=NER_PAD_ID)
-        self.log("train_loss", self.train_loss, prog_bar=True, logger=False, on_step=False, on_epoch=True)
-        self.log("train_acc", self.train_acc, prog_bar=True, logger=False, on_step=False, on_epoch=True)
-        self.log("val_loss", outputs.loss, prog_bar=True, logger=False, on_step=False, on_epoch=True)
-        self.log("val_acc", acc, prog_bar=True, logger=False, on_step=False, on_epoch=True)
-        self.log("global_step", self.trainer.lightning_module.global_step * 1.0, prog_bar=True, logger=False, on_step=True, on_epoch=False)
+        global_step = self.trainer.lightning_module.global_step * 1.0
+        self.log(prog_bar=True, logger=False, on_epoch=True, name="global_step", value=global_step)
+        self.log(prog_bar=True, logger=False, on_epoch=True, name="train_loss", value=self.train_loss)
+        self.log(prog_bar=True, logger=False, on_epoch=True, name="train_acc", value=self.train_acc)
+        self.log(prog_bar=True, logger=False, on_epoch=True, name="val_loss", value=outputs.loss)
+        self.log(prog_bar=True, logger=False, on_epoch=True, name="val_acc", value=acc)
         return {"val_loss": outputs.loss, "val_acc": acc}
 
     def test_step(self, inputs, batch_idx):
         outputs: TokenClassifierOutput = self.model(**inputs)
         preds = outputs.logits.argmax(dim=-1)
         labels = inputs["labels"]
         acc = accuracy(preds, labels, ignore_index=NER_PAD_ID)
-        self.log("test_loss", outputs.loss, prog_bar=False, logger=True, on_step=False, on_epoch=True)
-        self.log("test_acc", acc, prog_bar=False, logger=True, on_step=False, on_epoch=True)
+        self.log(prog_bar=False, logger=True, on_epoch=True, name="test_loss", value=outputs.loss)
+        self.log(prog_bar=False, logger=True, on_epoch=True, name="test_acc", value=acc)
         return {"test_loss": outputs.loss, "test_acc": acc}
 
     def x_validation_epoch_end(
             self, outputs: List[Dict[str, torch.Tensor]], data_type: str = "valid", write_predictions: bool = False
     ) -> None:
         """When validation step ends, either token- or character-level predicted
         labels are aligned with the original character-level labels and then
```

### Comparing `chrislab-0.5.2/src/nlpbook/paircls/corpus.py` & `chrislab-0.5.3/src/nlpbook/paircls/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/src/nlpbook/paircls/deploy.py` & `chrislab-0.5.3/src/nlpbook/paircls/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/src/nlpbook/qa/arguments.py` & `chrislab-0.5.3/src/nlpbook/qa/arguments.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/src/nlpbook/qa/corpus.py` & `chrislab-0.5.3/src/nlpbook/qa/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/src/nlpbook/qa/deploy.py` & `chrislab-0.5.3/src/nlpbook/qa/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/src/nlpbook/qa/task.py` & `chrislab-0.5.3/src/nlpbook/qa/task.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.2/src/nlpbook/utils.py` & `chrislab-0.5.3/src/nlpbook/utils.py`

 * *Files identical despite different names*

