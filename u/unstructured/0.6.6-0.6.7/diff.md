# Comparing `tmp/unstructured-0.6.6.tar.gz` & `tmp/unstructured-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.6.6.tar", last modified: Fri May 12 17:49:05 2023, max compression
+gzip compressed data, was "unstructured-0.6.7.tar", last modified: Fri May 19 17:33:22 2023, max compression
```

## Comparing `unstructured-0.6.6.tar` & `unstructured-0.6.7.tar`

### file list

```diff
@@ -1,108 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:05.018533 unstructured-0.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-05-12 17:48:53.000000 unstructured-0.6.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    21142 2023-05-12 17:49:05.018533 unstructured-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16877 2023-05-12 17:48:53.000000 unstructured-0.6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-12 17:49:05.022533 unstructured-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-12 17:48:53.000000 unstructured-0.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:04.994531 unstructured-0.6.6/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:48:53.000000 unstructured-0.6.6/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:04.994531 unstructured-0.6.6/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:48:53.000000 unstructured-0.6.6/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-12 17:48:53.000000 unstructured-0.6.6/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-12 17:48:53.000000 unstructured-0.6.6/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-12 17:48:53.000000 unstructured-0.6.6/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-12 17:48:53.000000 unstructured-0.6.6/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:04.998531 unstructured-0.6.6/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:04.998531 unstructured-0.6.6/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:04.998531 unstructured-0.6.6/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:05.002532 unstructured-0.6.6/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:05.002532 unstructured-0.6.6/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:05.002532 unstructured-0.6.6/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:05.002532 unstructured-0.6.6/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27999 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:05.002532 unstructured-0.6.6/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:05.014532 unstructured-0.6.6/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:05.014532 unstructured-0.6.6/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/odt.py
--rw-r--r--   0 runner    (1001) docker     (123)    12755 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/text_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:05.018533 unstructured-0.6.6/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/staging/baseplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:04.998531 unstructured-0.6.6/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21142 2023-05-12 17:49:04.000000 unstructured-0.6.6/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-12 17:49:04.000000 unstructured-0.6.6/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:49:04.000000 unstructured-0.6.6/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-12 17:49:04.000000 unstructured-0.6.6/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-12 17:49:04.000000 unstructured-0.6.6/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-12 17:49:04.000000 unstructured-0.6.6/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.594192 unstructured-0.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-05-19 17:33:13.000000 unstructured-0.6.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    21203 2023-05-19 17:33:22.594192 unstructured-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16906 2023-05-19 17:33:13.000000 unstructured-0.6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-19 17:33:22.598192 unstructured-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-19 17:33:14.000000 unstructured-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.582192 unstructured-0.6.7/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:14.000000 unstructured-0.6.7/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.582192 unstructured-0.6.7/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:14.000000 unstructured-0.6.7/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-19 17:33:14.000000 unstructured-0.6.7/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-19 17:33:14.000000 unstructured-0.6.7/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-19 17:33:14.000000 unstructured-0.6.7/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-19 17:33:14.000000 unstructured-0.6.7/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.582192 unstructured-0.6.7/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.586192 unstructured-0.6.7/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.586192 unstructured-0.6.7/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.586192 unstructured-0.6.7/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.586192 unstructured-0.6.7/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.586192 unstructured-0.6.7/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.586192 unstructured-0.6.7/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24164 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.586192 unstructured-0.6.7/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.594192 unstructured-0.6.7/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.594192 unstructured-0.6.7/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/odt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/text_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.594192 unstructured-0.6.7/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/staging/baseplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.586192 unstructured-0.6.7/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21203 2023-05-19 17:33:22.000000 unstructured-0.6.7/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-19 17:33:22.000000 unstructured-0.6.7/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 17:33:22.000000 unstructured-0.6.7/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-19 17:33:22.000000 unstructured-0.6.7/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-19 17:33:22.000000 unstructured-0.6.7/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-19 17:33:22.000000 unstructured-0.6.7/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.6.6/LICENSE.md` & `unstructured-0.6.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/PKG-INFO` & `unstructured-0.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.6.6
+Version: 0.6.7
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -186,31 +186,32 @@
         you can also uninstall the hooks with `pre-commit uninstall`.
         
         ## :clap: Quick Tour
         
         You can run this [Colab notebook](https://colab.research.google.com/drive/1U8VCjY2-x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below.
         
         The following examples show how to get started with the `unstructured` library.
-        You can parse **TXT**, **HTML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**,
-        **ODT**, **PPT**, **PPTX**, **JPG**,
+        
+        You can parse **TXT**, **HTML**, **XML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**,
+        **XLSX**, **ODT**, **PPT**, **PPTX**, **JPG**,
         and **PNG** documents with one line of code!
         <br></br>
         See our [documentation page](https://unstructured-io.github.io/unstructured) for a full description
         of the features in the library.
         
         ### Document Parsing
         
         The easiest way to parse a document in unstructured is to use the `partition` brick. If you
         use `partition` brick, `unstructured` will detect the file type and route it to the appropriate
         file-specific partitioning brick.
         If you are using the `partition` brick, you may need to install additional parameters via `pip install unstructured[local-inference]`. Ensure you first install `libmagic` using the
         instructions outlined [here](https://unstructured-io.github.io/unstructured/installing.html#filetype-detection)
         `partition` will always apply the default arguments. If you need
         advanced features, use a document-specific brick. The `partition` brick currently works for
-        `.txt`, `.doc`, `.docx`, `.ppt`, `.pptx`, `.jpg`, `.png`, `.eml`, `.msg`, `.html`, and `.pdf` documents.
+        `.txt`, `.doc`, `.docx`, `.ppt`, `.pptx`, `.xlsx`, `.jpg`, `.png`, `.eml`, `.msg`, `.html`, and `.pdf` documents.
         
         ```python
         from unstructured.partition.auto import partition
         
         elements = partition("example-docs/layout-parser-paper.pdf")
         ```
         
@@ -406,13 +407,14 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: huggingface
 Provides-Extra: local-inference
 Provides-Extra: s3
 Provides-Extra: azure
+Provides-Extra: discord
 Provides-Extra: github
 Provides-Extra: gitlab
 Provides-Extra: reddit
 Provides-Extra: slack
 Provides-Extra: wikipedia
 Provides-Extra: google-drive
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.6.6 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.6.7 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -111,42 +111,42 @@
 `pre-commit`, you'll just need to install the hooks with `pre-commit install`
 since the `pre-commit` package is installed as part of `make install` mentioned
 above. Finally, if you decided to use `pre-commit` you can also uninstall the
 hooks with `pre-commit uninstall`. ## :clap: Quick Tour You can run this [Colab
 notebook](https://colab.research.google.com/drive/1U8VCjY2-
 x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below. The following examples
 show how to get started with the `unstructured` library. You can parse **TXT**,
-**HTML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**,
-**ODT**, **PPT**, **PPTX**, **JPG**, and **PNG** documents with one line of
-code!
+**HTML**, **XML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**,
+**DOCX**, **XLSX**, **ODT**, **PPT**, **PPTX**, **JPG**, and **PNG** documents
+with one line of code!
 See our [documentation page](https://unstructured-io.github.io/unstructured)
 for a full description of the features in the library. ### Document Parsing The
 easiest way to parse a document in unstructured is to use the `partition`
 brick. If you use `partition` brick, `unstructured` will detect the file type
 and route it to the appropriate file-specific partitioning brick. If you are
 using the `partition` brick, you may need to install additional parameters via
 `pip install unstructured[local-inference]`. Ensure you first install
 `libmagic` using the instructions outlined [here](https://unstructured-
 io.github.io/unstructured/installing.html#filetype-detection) `partition` will
 always apply the default arguments. If you need advanced features, use a
 document-specific brick. The `partition` brick currently works for `.txt`,
-`.doc`, `.docx`, `.ppt`, `.pptx`, `.jpg`, `.png`, `.eml`, `.msg`, `.html`, and
-`.pdf` documents. ```python from unstructured.partition.auto import partition
-elements = partition("example-docs/layout-parser-paper.pdf") ``` Run `print
-("\n\n".join([str(el) for el in elements]))` to get a string representation of
-the output, which looks like: ``` LayoutParser : A Uniï¬ed Toolkit for Deep
-Learning Based Document Image Analysis Zejiang Shen 1 ( (cid:0) ), Ruochen
-Zhang 2 , Melissa Dell 3 , Benjamin Charles Germain Lee 4 , Jacob Carlson 3 ,
-and Weining Li 5 Abstract. Recent advances in document image analysis (DIA)
-have been primarily driven by the application of neural networks. Ideally,
-research outcomes could be easily deployed in production and extended for
-further investigation. However, various factors like loosely organized
-codebases and sophisticated model conï¬gurations complicate the easy reuse of
-im- portant innovations by a wide audience. Though there have been on-going
-eï¬orts to improve reusability and simplify deep learning (DL) model
+`.doc`, `.docx`, `.ppt`, `.pptx`, `.xlsx`, `.jpg`, `.png`, `.eml`, `.msg`,
+`.html`, and `.pdf` documents. ```python from unstructured.partition.auto
+import partition elements = partition("example-docs/layout-parser-paper.pdf")
+``` Run `print("\n\n".join([str(el) for el in elements]))` to get a string
+representation of the output, which looks like: ``` LayoutParser : A Uniï¬ed
+Toolkit for Deep Learning Based Document Image Analysis Zejiang Shen 1 ( (cid:
+0) ), Ruochen Zhang 2 , Melissa Dell 3 , Benjamin Charles Germain Lee 4 , Jacob
+Carlson 3 , and Weining Li 5 Abstract. Recent advances in document image
+analysis (DIA) have been primarily driven by the application of neural
+networks. Ideally, research outcomes could be easily deployed in production and
+extended for further investigation. However, various factors like loosely
+organized codebases and sophisticated model conï¬gurations complicate the easy
+reuse of im- portant innovations by a wide audience. Though there have been on-
+going eï¬orts to improve reusability and simplify deep learning (DL) model
 development in disciplines like natural language processing and computer
 vision, none of them are optimized for challenges in the domain of DIA. This
 represents a major gap in the existing toolkit, as DIA is central to academic
 research across a wide range of disciplines in the social sciences and
 humanities. This paper introduces LayoutParser , an open-source library for
 streamlining the usage of DL in DIA research and applica- tions. The core
 LayoutParser library comes with a set of simple and intuitive interfaces for
@@ -221,10 +221,10 @@
 Audience :: Education Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.7.0 Description-Content-Type:
 text/markdown Provides-Extra: huggingface Provides-Extra: local-inference
-Provides-Extra: s3 Provides-Extra: azure Provides-Extra: github Provides-Extra:
-gitlab Provides-Extra: reddit Provides-Extra: slack Provides-Extra: wikipedia
-Provides-Extra: google-drive
+Provides-Extra: s3 Provides-Extra: azure Provides-Extra: discord Provides-
+Extra: github Provides-Extra: gitlab Provides-Extra: reddit Provides-Extra:
+slack Provides-Extra: wikipedia Provides-Extra: google-drive
```

### Comparing `unstructured-0.6.6/README.md` & `unstructured-0.6.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -178,31 +178,32 @@
 you can also uninstall the hooks with `pre-commit uninstall`.
 
 ## :clap: Quick Tour
 
 You can run this [Colab notebook](https://colab.research.google.com/drive/1U8VCjY2-x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below.
 
 The following examples show how to get started with the `unstructured` library.
-You can parse **TXT**, **HTML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**,
-**ODT**, **PPT**, **PPTX**, **JPG**,
+
+You can parse **TXT**, **HTML**, **XML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**,
+**XLSX**, **ODT**, **PPT**, **PPTX**, **JPG**,
 and **PNG** documents with one line of code!
 <br></br>
 See our [documentation page](https://unstructured-io.github.io/unstructured) for a full description
 of the features in the library.
 
 ### Document Parsing
 
 The easiest way to parse a document in unstructured is to use the `partition` brick. If you
 use `partition` brick, `unstructured` will detect the file type and route it to the appropriate
 file-specific partitioning brick.
 If you are using the `partition` brick, you may need to install additional parameters via `pip install unstructured[local-inference]`. Ensure you first install `libmagic` using the
 instructions outlined [here](https://unstructured-io.github.io/unstructured/installing.html#filetype-detection)
 `partition` will always apply the default arguments. If you need
 advanced features, use a document-specific brick. The `partition` brick currently works for
-`.txt`, `.doc`, `.docx`, `.ppt`, `.pptx`, `.jpg`, `.png`, `.eml`, `.msg`, `.html`, and `.pdf` documents.
+`.txt`, `.doc`, `.docx`, `.ppt`, `.pptx`, `.xlsx`, `.jpg`, `.png`, `.eml`, `.msg`, `.html`, and `.pdf` documents.
 
 ```python
 from unstructured.partition.auto import partition
 
 elements = partition("example-docs/layout-parser-paper.pdf")
 ```
```

#### html2text {}

```diff
@@ -107,42 +107,42 @@
 `pre-commit`, you'll just need to install the hooks with `pre-commit install`
 since the `pre-commit` package is installed as part of `make install` mentioned
 above. Finally, if you decided to use `pre-commit` you can also uninstall the
 hooks with `pre-commit uninstall`. ## :clap: Quick Tour You can run this [Colab
 notebook](https://colab.research.google.com/drive/1U8VCjY2-
 x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below. The following examples
 show how to get started with the `unstructured` library. You can parse **TXT**,
-**HTML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**,
-**ODT**, **PPT**, **PPTX**, **JPG**, and **PNG** documents with one line of
-code!
+**HTML**, **XML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**,
+**DOCX**, **XLSX**, **ODT**, **PPT**, **PPTX**, **JPG**, and **PNG** documents
+with one line of code!
 See our [documentation page](https://unstructured-io.github.io/unstructured)
 for a full description of the features in the library. ### Document Parsing The
 easiest way to parse a document in unstructured is to use the `partition`
 brick. If you use `partition` brick, `unstructured` will detect the file type
 and route it to the appropriate file-specific partitioning brick. If you are
 using the `partition` brick, you may need to install additional parameters via
 `pip install unstructured[local-inference]`. Ensure you first install
 `libmagic` using the instructions outlined [here](https://unstructured-
 io.github.io/unstructured/installing.html#filetype-detection) `partition` will
 always apply the default arguments. If you need advanced features, use a
 document-specific brick. The `partition` brick currently works for `.txt`,
-`.doc`, `.docx`, `.ppt`, `.pptx`, `.jpg`, `.png`, `.eml`, `.msg`, `.html`, and
-`.pdf` documents. ```python from unstructured.partition.auto import partition
-elements = partition("example-docs/layout-parser-paper.pdf") ``` Run `print
-("\n\n".join([str(el) for el in elements]))` to get a string representation of
-the output, which looks like: ``` LayoutParser : A Uniï¬ed Toolkit for Deep
-Learning Based Document Image Analysis Zejiang Shen 1 ( (cid:0) ), Ruochen
-Zhang 2 , Melissa Dell 3 , Benjamin Charles Germain Lee 4 , Jacob Carlson 3 ,
-and Weining Li 5 Abstract. Recent advances in document image analysis (DIA)
-have been primarily driven by the application of neural networks. Ideally,
-research outcomes could be easily deployed in production and extended for
-further investigation. However, various factors like loosely organized
-codebases and sophisticated model conï¬gurations complicate the easy reuse of
-im- portant innovations by a wide audience. Though there have been on-going
-eï¬orts to improve reusability and simplify deep learning (DL) model
+`.doc`, `.docx`, `.ppt`, `.pptx`, `.xlsx`, `.jpg`, `.png`, `.eml`, `.msg`,
+`.html`, and `.pdf` documents. ```python from unstructured.partition.auto
+import partition elements = partition("example-docs/layout-parser-paper.pdf")
+``` Run `print("\n\n".join([str(el) for el in elements]))` to get a string
+representation of the output, which looks like: ``` LayoutParser : A Uniï¬ed
+Toolkit for Deep Learning Based Document Image Analysis Zejiang Shen 1 ( (cid:
+0) ), Ruochen Zhang 2 , Melissa Dell 3 , Benjamin Charles Germain Lee 4 , Jacob
+Carlson 3 , and Weining Li 5 Abstract. Recent advances in document image
+analysis (DIA) have been primarily driven by the application of neural
+networks. Ideally, research outcomes could be easily deployed in production and
+extended for further investigation. However, various factors like loosely
+organized codebases and sophisticated model conï¬gurations complicate the easy
+reuse of im- portant innovations by a wide audience. Though there have been on-
+going eï¬orts to improve reusability and simplify deep learning (DL) model
 development in disciplines like natural language processing and computer
 vision, none of them are optimized for challenges in the domain of DIA. This
 represents a major gap in the existing toolkit, as DIA is central to academic
 research across a wide range of disciplines in the social sciences and
 humanities. This paper introduces LayoutParser , an open-source library for
 streamlining the usage of DL in DIA research and applica- tions. The core
 LayoutParser library comes with a set of simple and intuitive interfaces for
```

### Comparing `unstructured-0.6.6/setup.py` & `unstructured-0.6.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,14 +77,15 @@
             "transformers",
         ],
         "local-inference": [
             "unstructured-inference==0.4.4",
         ],
         "s3": ["s3fs", "fsspec"],
         "azure": ["adlfs", "fsspec"],
+        "discord": ["discord.py"],
         "github": [
             # NOTE - pygithub==1.58.0 fails due to https://github.com/PyGithub/PyGithub/issues/2436
             # In the future, we can update this to pygithub>1.58.0
             "pygithub==1.57.0",
         ],
         "gitlab": ["python-gitlab"],
         "reddit": ["praw"],
```

### Comparing `unstructured-0.6.6/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.6.7/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.6.7/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/test_unstructured/test_utils.py` & `unstructured-0.6.7/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/cleaners/core.py` & `unstructured-0.6.7/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/cleaners/extract.py` & `unstructured-0.6.7/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/cleaners/translate.py` & `unstructured-0.6.7/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/documents/base.py` & `unstructured-0.6.7/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/documents/elements.py` & `unstructured-0.6.7/unstructured/documents/elements.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import datetime
 import hashlib
 import os
 import pathlib
 from abc import ABC
 from dataclasses import dataclass
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
@@ -12,19 +14,24 @@
 
     pass
 
 
 @dataclass
 class ElementMetadata:
     filename: Optional[str] = None
+    file_directory: Optional[str] = None
     date: Optional[str] = None
+    filetype: Optional[str] = None
 
     # Page numbers currenlty supported for PDF, HTML and PPT documents
     page_number: Optional[int] = None
 
+    # Page name. The sheet name in XLXS documents.
+    page_name: Optional[str] = None
+
     # Webpage specific metadata fields
     url: Optional[str] = None
 
     # E-mail specific metadata fields
     sent_from: Optional[List[str]] = None
     sent_to: Optional[List[str]] = None
     subject: Optional[str] = None
@@ -33,23 +40,31 @@
     text_as_html: Optional[str] = None
 
     def __post_init__(self):
         if isinstance(self.filename, pathlib.Path):
             self.filename = str(self.filename)
 
         if self.filename is not None:
-            self.filename = os.path.basename(self.filename)
+            file_directory, filename = os.path.split(self.filename)
+            self.file_directory = file_directory or None
+            self.filename = filename
 
     def to_dict(self):
         return {key: value for key, value in self.__dict__.items() if value is not None}
 
     @classmethod
     def from_dict(cls, input_dict):
         return cls(**input_dict)
 
+    def merge(self, other: ElementMetadata):
+        for k in self.__dict__:
+            if getattr(self, k) is None:
+                setattr(self, k, getattr(other, k))
+        return self
+
     def get_date(self) -> Optional[datetime.datetime]:
         """Converts the date field to a datetime object."""
         dt = None
         if self.date is not None:
             dt = datetime.datetime.fromisoformat(self.date)
         return dt
```

### Comparing `unstructured-0.6.6/unstructured/documents/email_elements.py` & `unstructured-0.6.7/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/documents/html.py` & `unstructured-0.6.7/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/documents/xml.py` & `unstructured-0.6.7/unstructured/documents/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/file_utils/exploration.py` & `unstructured-0.6.7/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/file_utils/file_conversion.py` & `unstructured-0.6.7/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/file_utils/filetype.py` & `unstructured-0.6.7/unstructured/file_utils/filetype.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,84 +1,43 @@
+import inspect
 import os
 import re
 import zipfile
 from enum import Enum
-from typing import IO, Optional
+from functools import wraps
+from typing import IO, Callable, List, Optional
 
+from unstructured.documents.elements import Element, PageBreak
 from unstructured.nlp.patterns import LIST_OF_DICTS_PATTERN
-from unstructured.partition.common import exactly_one
+from unstructured.partition.common import _add_element_metadata, exactly_one
 
 try:
     import magic
 
     LIBMAGIC_AVAILABLE = True
 except ImportError:  # pragma: nocover
     LIBMAGIC_AVAILABLE = False  # pragma: nocover
 
 from unstructured.logger import logger
 from unstructured.nlp.patterns import EMAIL_HEAD_RE
 
-DOCX_MIME_TYPES = [
-    "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
-]
-
-DOC_MIME_TYPES = [
-    "application/msword",
-]
-
-ODT_MIME_TYPES = [
-    "application/vnd.oasis.opendocument.text",
-]
-
-XLSX_MIME_TYPES = [
-    "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet",
-]
-
-XLS_MIME_TYPES = [
-    "application/vnd.ms-excel",
-]
-
-PPTX_MIME_TYPES = [
-    "application/vnd.openxmlformats-officedocument.presentationml.presentation",
-]
-
-PPT_MIME_TYPES = [
-    "application/vnd.ms-powerpoint",
-]
-
-MSG_MIME_TYPES = [
-    "application/vnd.ms-outlook",
-    "application/x-ole-storage",
-]
-
 TXT_MIME_TYPES = [
     "text/plain",
     "message/rfc822",  # ref: https://www.rfc-editor.org/rfc/rfc822
 ]
 
-MD_MIME_TYPES = [
-    "text/markdown",
-    "text/x-markdown",
-]
-
-EPUB_MIME_TYPES = [
-    "application/epub",
-    "application/epub+zip",
-]
-
 # NOTE(robinson) - .docx.xlsx files are actually zip file with a .docx/.xslx extension.
 # If the MIME type is application/octet-stream, we check if it's a .docx/.xlsx file by
 # looking for expected filenames within the zip file.
 EXPECTED_DOCX_FILES = [
     "docProps/core.xml",
     "word/document.xml",
 ]
 
 EXPECTED_XLSX_FILES = [
-    "docProps/core.xml",
     "xl/workbook.xml",
 ]
 
 EXPECTED_PPTX_FILES = [
     "docProps/core.xml",
     "ppt/presentation.xml",
 ]
@@ -128,37 +87,48 @@
 
 STR_TO_FILETYPE = {
     "application/pdf": FileType.PDF,
     "application/msword": FileType.DOC,
     "application/vnd.openxmlformats-officedocument.wordprocessingml.document": FileType.DOCX,
     "image/jpeg": FileType.JPG,
     "image/png": FileType.PNG,
+    "text/plain": FileType.TXT,
     "text/markdown": FileType.MD,
     "text/x-markdown": FileType.MD,
     "application/epub": FileType.EPUB,
     "application/epub+zip": FileType.EPUB,
+    "application/json": FileType.JSON,
+    "application/rtf": FileType.RTF,
+    "text/rtf": FileType.RTF,
     "text/html": FileType.HTML,
     "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet": FileType.XLSX,
     "application/vnd.ms-excel": FileType.XLS,
     "application/vnd.openxmlformats-officedocument.presentationml.presentation": FileType.PPTX,
     "application/vnd.ms-powerpoint": FileType.PPT,
     "application/xml": FileType.XML,
     "application/vnd.oasis.opendocument.text": FileType.ODT,
+    "message/rfc822": FileType.EML,
+    "application/x-ole-storage": FileType.MSG,
+    "application/vnd.ms-outlook": FileType.MSG,
 }
 
+FILETYPE_TO_MIMETYPE = {
+    v: k for k, v in STR_TO_FILETYPE.items() if k not in ("text/x-markdown", "application/epub+zip")
+}
 
 EXT_TO_FILETYPE = {
     ".pdf": FileType.PDF,
     ".docx": FileType.DOCX,
     ".jpg": FileType.JPG,
     ".jpeg": FileType.JPG,
     ".txt": FileType.TXT,
     ".text": FileType.TXT,
     ".eml": FileType.EML,
     ".xml": FileType.XML,
+    ".htm": FileType.HTML,
     ".html": FileType.HTML,
     ".md": FileType.MD,
     ".xlsx": FileType.XLSX,
     ".pptx": FileType.PPTX,
     ".png": FileType.PNG,
     ".doc": FileType.DOC,
     ".zip": FileType.ZIP,
@@ -191,21 +161,17 @@
 
     if filename or file_filename:
         _filename = filename or file_filename or ""
         _, extension = os.path.splitext(_filename)
         extension = extension.lower()
         if os.path.isfile(_filename) and LIBMAGIC_AVAILABLE:
             mime_type = magic.from_file(filename or file_filename, mime=True)  # type: ignore
-            # NOTE(crag): for older versions of the OS libmagic package, such as is currently
-            # installed on the Unstructured docker image, .json files resolve to "text/plain"
-            # rather than "application/json". this corrects for that case.
-            if mime_type == "text/plain" and extension == ".json":
-                return FileType.JSON
         else:
             return EXT_TO_FILETYPE.get(extension.lower(), FileType.UNK)
+
     elif file is not None:
         extension = None
         # NOTE(robinson) - the python-magic docs recommend reading at least the first 2048 bytes
         # Increased to 4096 because otherwise .xlsx files get detected as a zip file
         # ref: https://github.com/ahupp/python-magic#usage
         if LIBMAGIC_AVAILABLE:
             mime_type = magic.from_buffer(file.read(4096), mime=True)
@@ -214,85 +180,49 @@
                 "libmagic is unavailable. "
                 "Filetype detection on file-like objects requires libmagic. "
                 "Please install libmagic and try again.",
             )
     else:
         raise ValueError("No filename, file, nor file_filename were specified.")
 
-    if mime_type == "application/pdf":
-        return FileType.PDF
+    """Mime type special cases."""
 
-    elif mime_type == "application/json":
+    # NOTE(crag): for older versions of the OS libmagic package, such as is currently
+    # installed on the Unstructured docker image, .json files resolve to "text/plain"
+    # rather than "application/json". this corrects for that case.
+    if mime_type == "text/plain" and extension == ".json":
         return FileType.JSON
 
-    elif mime_type in DOCX_MIME_TYPES:
-        return FileType.DOCX
-
-    elif mime_type in DOC_MIME_TYPES:
-        return FileType.DOC
-
-    elif mime_type in ODT_MIME_TYPES:
-        return FileType.ODT
-
-    elif mime_type in MSG_MIME_TYPES:
-        return FileType.MSG
-
-    elif mime_type == "image/jpeg":
-        return FileType.JPG
-
-    elif mime_type == "image/png":
-        return FileType.PNG
-
-    elif mime_type in MD_MIME_TYPES:
-        # NOTE - I am not sure whether libmagic ever returns these mimetypes.
-        return FileType.MD
-
-    elif mime_type in EPUB_MIME_TYPES:
-        return FileType.EPUB
-
-    # NOTE(robinson) - examples are application/rtf or text/rtf.
-    # magic often returns text/plain for RTF files
-    elif mime_type.endswith("rtf"):
-        return FileType.RTF
-
     elif mime_type.endswith("xml"):
-        if extension and extension == ".html":
+        if extension and (extension == ".html" or extension == ".htm"):
             return FileType.HTML
         else:
             return FileType.XML
 
-    elif mime_type == "text/html":
-        return FileType.HTML
-
     elif mime_type in TXT_MIME_TYPES or mime_type.startswith("text"):
         if extension and extension == ".eml":
             return FileType.EML
         elif extension and extension == ".md":
             return FileType.MD
         elif extension and extension == ".rtf":
             return FileType.RTF
+        elif extension and extension == ".html":
+            return FileType.HTML
 
         if _is_text_file_a_json(file=file, filename=filename):
             return FileType.JSON
 
         if file and not extension and _check_eml_from_buffer(file=file) is True:
             return FileType.EML
-        return FileType.TXT
-
-    elif mime_type in XLSX_MIME_TYPES:
-        return FileType.XLSX
 
-    elif mime_type in XLS_MIME_TYPES:
-        return FileType.XLS
+        # Safety catch
+        if mime_type in STR_TO_FILETYPE:
+            return STR_TO_FILETYPE[mime_type]
 
-    elif mime_type in PPTX_MIME_TYPES:
-        return FileType.PPTX
-
-    elif mime_type in PPT_MIME_TYPES:
-        return FileType.PPT
+        return FileType.TXT
 
     elif mime_type == "application/octet-stream":
         if file and not extension:
             return _detect_filetype_from_octet_stream(file=file)
         else:
             return EXT_TO_FILETYPE.get(extension, FileType.UNK)
 
@@ -306,14 +236,18 @@
 
         extension = extension if extension else ""
         if filetype == FileType.UNK:
             return EXT_TO_FILETYPE.get(extension.lower(), FileType.ZIP)
         else:
             return EXT_TO_FILETYPE.get(extension.lower(), filetype)
 
+    # For everything else
+    elif mime_type in STR_TO_FILETYPE:
+        return STR_TO_FILETYPE[mime_type]
+
     logger.warning(
         f"The MIME type{f' of {filename!r}' if filename else ''} is {mime_type!r}. "
         "This file type is not currently supported in unstructured.",
     )
     return EXT_TO_FILETYPE.get(extension, FileType.UNK)
 
 
@@ -368,7 +302,65 @@
     file_content = file.read(4096)
     if isinstance(file_content, bytes):
         file_head = file_content.decode("utf-8", errors="ignore")
     else:
         file_head = file_content
 
     return EMAIL_HEAD_RE.match(file_head) is not None
+
+
+def document_to_element_list(
+    document,
+    include_page_breaks: bool = False,
+) -> List[Element]:
+    """Converts a DocumentLayout object to a list of unstructured elements."""
+    elements: List[Element] = []
+    image_formats: List[str] = []
+    num_pages = len(document.pages)
+    for i, page in enumerate(document.pages):
+        for element in page.elements:
+            elements.append(element)
+            if hasattr(page, "image"):
+                image_formats.append(page.image.format)
+        if include_page_breaks and i < num_pages - 1:
+            elements.append(PageBreak())
+
+    if image_formats and all(image_format == "PNG" for image_format in image_formats):
+        filetype = FileType.PNG.name
+    elif image_formats and all(image_format == "JPEG" for image_format in image_formats):
+        filetype = FileType.JPG.name
+    else:
+        filetype = None
+    elements = _add_element_metadata(
+        elements,
+        include_page_breaks=include_page_breaks,
+        filetype=filetype,
+    )
+    return elements
+
+
+def add_metadata_with_filetype(filetype: FileType):
+    def decorator(func: Callable):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            elements = func(*args, **kwargs)
+            sig = inspect.signature(func)
+            params = dict(**dict(zip(sig.parameters, args)), **kwargs)
+            for param in sig.parameters.values():
+                if param.name not in params and param.default is not param.empty:
+                    params[param.name] = param.default
+            include_metadata = params.get("include_metadata", True)
+            if include_metadata:
+                metadata_kwargs = {
+                    kwarg: params.get(kwarg) for kwarg in ("include_page_breaks", "filename", "url")
+                }
+                return _add_element_metadata(
+                    elements,
+                    filetype=FILETYPE_TO_MIMETYPE[filetype],
+                    **metadata_kwargs,  # type: ignore
+                )
+            else:
+                return elements
+
+        return wrapper
+
+    return decorator
```

### Comparing `unstructured-0.6.6/unstructured/file_utils/metadata.py` & `unstructured-0.6.7/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/ingest/connector/azure.py` & `unstructured-0.6.7/unstructured/ingest/connector/azure.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Type
 
 from unstructured.ingest.connector.fsspec import (
     FsspecConnector,
     FsspecIngestDoc,
     SimpleFsspecConfig,
 )
+from unstructured.ingest.interfaces import StandardConnectorConfig
 from unstructured.utils import requires_dependencies
 
 
 @dataclass
 class SimpleAzureBlobStorageConfig(SimpleFsspecConfig):
     pass
 
@@ -22,10 +23,11 @@
 
 @requires_dependencies(["adlfs", "fsspec"], extras="azure")
 class AzureBlobStorageConnector(FsspecConnector):
     ingest_doc_cls: Type[AzureBlobStorageIngestDoc] = AzureBlobStorageIngestDoc
 
     def __init__(
         self,
+        standard_config: StandardConnectorConfig,
         config: SimpleAzureBlobStorageConfig,
     ) -> None:
-        super().__init__(config=config)
+        super().__init__(standard_config=standard_config, config=config)
```

### Comparing `unstructured-0.6.6/unstructured/ingest/connector/biomed.py` & `unstructured-0.6.7/unstructured/ingest/connector/biomed.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import json
 import os
 import urllib.request
 from dataclasses import dataclass
 from ftplib import FTP, error_perm
 from pathlib import Path
-from typing import List, Optional, Union
+from typing import List, Union
 
 import requests
 from bs4 import BeautifulSoup
 
 from unstructured.ingest.interfaces import (
     BaseConnector,
     BaseConnectorConfig,
     BaseIngestDoc,
+    StandardConnectorConfig,
 )
 from unstructured.ingest.logger import logger
 from unstructured.utils import (
     validate_date_args,
 )
 
 DOMAIN = "ftp.ncbi.nlm.nih.gov"
@@ -34,34 +35,19 @@
 
 @dataclass
 class SimpleBiomedConfig(BaseConnectorConfig):
     """Connector config where path is the FTP directory path and
     id_, from_, until, format are API parameters."""
 
     path: str
-
     # OA Web Service API Options
     id_: str
     from_: str
     until: str
 
-    # Standard Connector options
-    download_dir: str
-    # where to write structured data, with the directory structure matching FTP path
-    output_dir: str
-    re_download: bool = False
-    download_only: bool = False
-    preserve_downloads: bool = False
-    metadata_include: Optional[str] = None
-    metadata_exclude: Optional[str] = None
-    partition_by_api: bool = False
-    partition_endpoint: str = "https://api.unstructured.io/general/v0/general"
-    fields_include: str = "element_id,text,type,metadata"
-    flatten_metadata: bool = False
-
     def validate_api_inputs(self):
         valid = False
 
         if self.from_:
             valid = validate_date_args(self.from_)
 
         if self.until:
@@ -74,15 +60,15 @@
         self.is_dir = False
         self.is_api = False
 
         if not self.path:
             is_valid = self.validate_api_inputs()
             if not is_valid:
                 raise ValueError(
-                    "Path argument or atleast one of the "
+                    "Path argument or at least one of the "
                     "OA Web Service arguments MUST be provided.",
                 )
 
             self.is_api = True
         else:
             self.path = self.path.strip("/")
             is_valid = self.path.lower().startswith(PDF_DIR)
@@ -122,17 +108,17 @@
         return Path(self.file_meta.download_filepath).resolve()  # type: ignore
 
     def _output_filename(self):
         return Path(f"{self.file_meta.output_filepath}.json").resolve()
 
     def cleanup_file(self):
         if (
-            not self.config.preserve_downloads
+            not self.standard_config.preserve_downloads
             and self.filename.is_file()
-            and not self.config.download_only
+            and not self.standard_config.download_only
         ):
             logger.debug(f"Cleaning up {self}")
             Path.unlink(self.filename)
 
     def has_output(self):
         """Determine if structured output for this doc already exists."""
         output_filename = self._output_filename()
@@ -153,44 +139,50 @@
             self.file_meta.download_filepath,
         )
 
         logger.debug(f"File downloaded: {self.file_meta.download_filepath}")
 
     def write_result(self):
         """Write the structured json result for this doc. result must be json serializable."""
-        if self.config.download_only:
+        if self.standard_config.download_only:
             return
         output_filename = self._output_filename()
         output_filename.parent.mkdir(parents=True, exist_ok=True)
         with open(output_filename, "w") as output_f:
             output_f.write(json.dumps(self.isd_elems_no_filename, ensure_ascii=False, indent=2))
         logger.info(f"Wrote {output_filename}")
 
 
 class BiomedConnector(BaseConnector):
     """Objects of this class support fetching documents from Biomedical literature FTP directory"""
 
-    def __init__(self, config):
-        self.config = config
-        self.cleanup_files = not self.config.preserve_downloads and not self.config.download_only
+    config: SimpleBiomedConfig
+
+    def __init__(self, standard_config: StandardConnectorConfig, config: SimpleBiomedConfig):
+        super().__init__(standard_config, config)
+        self.cleanup_files = (
+            not self.standard_config.preserve_downloads and not self.standard_config.download_only
+        )
 
     def _list_objects_api(self):
         def urls_to_metadata(urls):
             files = []
             for url in urls:
                 parts = url.split(PDF_DIR)
                 if len(parts) > 1:
                     local_path = parts[1].strip("/")
                     files.append(
                         BiomedFileMeta(
                             ftp_path=url,
                             download_filepath=(
-                                Path(self.config.download_dir) / local_path
+                                Path(self.standard_config.download_dir) / local_path
+                            ).resolve(),
+                            output_filepath=(
+                                Path(self.standard_config.output_dir) / local_path
                             ).resolve(),
-                            output_filepath=(Path(self.config.output_dir) / local_path).resolve(),
                         ),
                     )
 
             return files
 
         files: List[BiomedFileMeta] = []
 
@@ -247,18 +239,18 @@
                     for sub_path in sub_paths:
                         ftp_path = f"{FTP_DOMAIN}/{PMC_DIR}/{sub_path}"
                         local_path = "/".join(str(sub_path).split("/")[1:])
                         files.append(
                             BiomedFileMeta(
                                 ftp_path=ftp_path,
                                 download_filepath=(
-                                    Path(self.config.download_dir) / local_path
+                                    Path(self.standard_config.download_dir) / local_path
                                 ).resolve(),
                                 output_filepath=(
-                                    Path(self.config.output_dir) / local_path
+                                    Path(self.standard_config.output_dir) / local_path
                                 ).resolve(),
                             ),
                         )
 
                 else:
                     for sub_path in sub_paths:
                         traverse(sub_path, download_dir, output_dir)
@@ -268,33 +260,35 @@
 
         ftp_path = f"{FTP_DOMAIN}/{PMC_DIR}/{self.config.path}"
         if self.config.is_file:
             local_path = "/".join(self.config.path.split("/")[1:])
             return [
                 BiomedFileMeta(
                     ftp_path=ftp_path,
-                    download_filepath=(Path(self.config.download_dir) / local_path).resolve(),
-                    output_filepath=(Path(self.config.output_dir) / local_path).resolve(),
+                    download_filepath=(
+                        Path(self.standard_config.download_dir) / local_path
+                    ).resolve(),
+                    output_filepath=(Path(self.standard_config.output_dir) / local_path).resolve(),
                 ),
             ]
         else:
             traverse(
                 Path(self.config.path),
-                Path(self.config.download_dir),
-                Path(self.config.output_dir),
+                Path(self.standard_config.download_dir),
+                Path(self.standard_config.output_dir),
             )
 
         return files
 
     def cleanup(self, cur_dir=None):
         if not self.cleanup_files:
             return
 
         if cur_dir is None:
-            cur_dir = self.config.download_dir
+            cur_dir = self.standard_config.download_dir
 
         if cur_dir is None or not Path(cur_dir).is_dir():
             return
 
         sub_dirs = os.listdir(cur_dir)
         os.chdir(cur_dir)
         for sub_dir in sub_dirs:
@@ -306,8 +300,8 @@
             os.rmdir(cur_dir)
 
     def initialize(self):
         pass
 
     def get_ingest_docs(self):
         files = self._list_objects_api() if self.config.is_api else self._list_objects()
-        return [BiomedIngestDoc(self.config, file) for file in files]
+        return [BiomedIngestDoc(self.standard_config, self.config, file) for file in files]
```

### Comparing `unstructured-0.6.6/unstructured/ingest/connector/fsspec.py` & `unstructured-0.6.7/unstructured/ingest/connector/fsspec.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,34 @@
 import json
 import os
 import re
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import Optional, Type
+from typing import Type
 
 from unstructured.ingest.interfaces import (
     BaseConnector,
     BaseConnectorConfig,
     BaseIngestDoc,
+    StandardConnectorConfig,
 )
 from unstructured.ingest.logger import logger
 
 SUPPORTED_REMOTE_FSSPEC_PROTOCOLS = [
     "s3",
     "abfs",
     "az",
 ]
 
 
 @dataclass
 class SimpleFsspecConfig(BaseConnectorConfig):
     # fsspec specific options
     path: str
-
-    # base connector options
-    download_dir: str
-    output_dir: str
-    preserve_downloads: bool = False
-    re_download: bool = False
-    download_only: bool = False
-    metadata_include: Optional[str] = None
-    metadata_exclude: Optional[str] = None
-    partition_by_api: bool = False
-    partition_endpoint: str = "https://api.unstructured.io/general/v0/general"
-    fields_include: str = "element_id,text,type,metadata"
-    flatten_metadata: bool = False
-
-    # fsspec specific options
     access_kwargs: dict = field(default_factory=dict)
-
     protocol: str = field(init=False)
     path_without_protocol: str = field(init=False)
     dir_path: str = field(init=False)
     file_path: str = field(init=False)
 
     def __post_init__(self):
         self.protocol, self.path_without_protocol = self.path.split("://")
@@ -79,22 +64,22 @@
     method is not called, the file is left behind on the filesystem to assist debugging.
     """
 
     config: SimpleFsspecConfig
     remote_file_path: str
 
     def _tmp_download_file(self):
-        return Path(self.config.download_dir) / self.remote_file_path.replace(
+        return Path(self.standard_config.download_dir) / self.remote_file_path.replace(
             f"{self.config.dir_path}/",
             "",
         )
 
     def _output_filename(self):
         return (
-            Path(self.config.output_dir)
+            Path(self.standard_config.output_dir)
             / f"{self.remote_file_path.replace(f'{self.config.dir_path}/', '')}.json"
         )
 
     def has_output(self):
         """Determine if structured output for this doc already exists."""
         return self._output_filename().is_file() and os.path.getsize(self._output_filename())
 
@@ -104,15 +89,15 @@
 
     def get_file(self):
         """Fetches the file from the current filesystem and stores it locally."""
         from fsspec import AbstractFileSystem, get_filesystem_class
 
         self._create_full_tmp_dir_path()
         if (
-            not self.config.re_download
+            not self.standard_config.re_download
             and self._tmp_download_file().is_file()
             and os.path.getsize(self._tmp_download_file())
         ):
             logger.debug(f"File exists: {self._tmp_download_file()}, skipping download")
             return
 
         fs: AbstractFileSystem = get_filesystem_class(self.config.protocol)(
@@ -120,59 +105,63 @@
         )
 
         logger.debug(f"Fetching {self} - PID: {os.getpid()}")
         fs.get(rpath=self.remote_file_path, lpath=self._tmp_download_file().as_posix())
 
     def write_result(self):
         """Write the structured json result for this doc. result must be json serializable."""
-        if self.config.download_only:
+        if self.standard_config.download_only:
             return
         output_filename = self._output_filename()
         output_filename.parent.mkdir(parents=True, exist_ok=True)
         with open(output_filename, "w") as output_f:
             output_f.write(json.dumps(self.isd_elems_no_filename, ensure_ascii=False, indent=2))
         logger.info(f"Wrote {output_filename}")
 
     @property
     def filename(self):
         """The filename of the file after downloading from s3"""
         return self._tmp_download_file()
 
     def cleanup_file(self):
         """Removes the local copy of the file after successful processing."""
-        if not self.config.preserve_downloads and not self.config.download_only:
+        if not self.standard_config.preserve_downloads and not self.standard_config.download_only:
             logger.debug(f"Cleaning up {self}")
             os.unlink(self._tmp_download_file())
 
 
 class FsspecConnector(BaseConnector):
     """Objects of this class support fetching document(s) from"""
 
+    config: SimpleFsspecConfig
     ingest_doc_cls: Type[FsspecIngestDoc] = FsspecIngestDoc
 
     def __init__(
         self,
+        standard_config: StandardConnectorConfig,
         config: SimpleFsspecConfig,
     ):
         from fsspec import AbstractFileSystem, get_filesystem_class
 
-        self.config = config
+        super().__init__(standard_config, config)
         self.fs: AbstractFileSystem = get_filesystem_class(self.config.protocol)(
             **self.config.access_kwargs,
         )
-        self.cleanup_files = not config.preserve_downloads and not config.download_only
+        self.cleanup_files = (
+            not standard_config.preserve_downloads and not standard_config.download_only
+        )
 
     def cleanup(self, cur_dir=None):
         """cleanup linginering empty sub-dirs from s3 paths, but leave remaining files
         (and their paths) in tact as that indicates they were not processed"""
         if not self.cleanup_files:
             return
 
         if cur_dir is None:
-            cur_dir = self.config.download_dir
+            cur_dir = self.standard_config.download_dir
         sub_dirs = os.listdir(cur_dir)
         os.chdir(cur_dir)
         for sub_dir in sub_dirs:
             # don't traverse symlinks, not that there every should be any
             if os.path.isdir(sub_dir) and not os.path.islink(sub_dir):
                 self.cleanup(sub_dir)
         os.chdir("..")
@@ -189,12 +178,13 @@
 
     def _list_files(self):
         return self.fs.ls(self.config.path_without_protocol)
 
     def get_ingest_docs(self):
         return [
             self.ingest_doc_cls(
+                self.standard_config,
                 self.config,
                 file,
             )
             for file in self._list_files()
         ]
```

### Comparing `unstructured-0.6.6/unstructured/ingest/connector/git.py` & `unstructured-0.6.7/unstructured/ingest/connector/git.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,58 +15,47 @@
 
 @dataclass
 class SimpleGitConfig(BaseConnectorConfig):
     url: str
     access_token: Optional[str]
     branch: Optional[str]
     file_glob: Optional[str]
-
-    # Standard Connector options
-    download_dir: str
-    # where to write structured data, with the directory structure matching the github repository
-    output_dir: str
-    preserve_downloads: bool = False
-    re_download: bool = False
-    download_only: bool = False
-    metadata_include: Optional[str] = None
-    metadata_exclude: Optional[str] = None
-    partition_by_api: bool = False
-    partition_endpoint: str = "https://api.unstructured.io/general/v0/general"
-    fields_include: str = "element_id,text,type,metadata"
-    flatten_metadata: bool = False
-
     repo_path: str = field(init=False, repr=False)
 
 
 @dataclass
 class GitIngestDoc(BaseIngestDoc):
     config: SimpleGitConfig = field(repr=False)
     path: str
 
     @property
     def filename(self):
-        return (Path(self.config.download_dir) / self.path).resolve()
+        return (Path(self.standard_config.download_dir) / self.path).resolve()
 
     def _output_filename(self):
-        return Path(self.config.output_dir) / f"{self.path}.json"
+        return Path(self.standard_config.output_dir) / f"{self.path}.json"
 
     def _create_full_tmp_dir_path(self):
         """includes directories in in the gitlab repository"""
         self.filename.parent.mkdir(parents=True, exist_ok=True)
 
     def cleanup_file(self):
         """Removes the local copy of the file (or anything else) after successful processing."""
-        if not self.config.preserve_downloads and not self.config.download_only:
+        if not self.standard_config.preserve_downloads and not self.standard_config.download_only:
             logger.debug(f"Cleaning up {self}")
             os.unlink(self.filename)
 
     def get_file(self):
         """Fetches the "remote" doc and stores it locally on the filesystem."""
         self._create_full_tmp_dir_path()
-        if not self.config.re_download and self.filename.is_file() and self.filename.stat():
+        if (
+            not self.standard_config.re_download
+            and self.filename.is_file()
+            and self.filename.stat()
+        ):
             logger.debug(f"File exists: {self.filename}, skipping download")
             return
 
         logger.debug(f"Fetching {self} - PID: {os.getpid()}")
         self._fetch_and_write()
 
     def _fetch_and_write(self) -> None:
@@ -75,36 +64,38 @@
     def has_output(self):
         """Determine if structured output for this doc already exists."""
         output_filename = self._output_filename()
         return output_filename.is_file() and output_filename.stat()
 
     def write_result(self):
         """Write the structured json result for this doc. result must be json serializable."""
-        if self.config.download_only:
+        if self.standard_config.download_only:
             return
         output_filename = self._output_filename()
         output_filename.parent.mkdir(parents=True, exist_ok=True)
         with open(output_filename, "w", encoding="utf8") as output_f:
             json.dump(self.isd_elems_no_filename, output_f, ensure_ascii=False, indent=2)
         logger.info(f"Wrote {output_filename}")
 
 
 @dataclass
 class GitConnector(BaseConnector):
     config: SimpleGitConfig
 
     def __post_init__(self) -> None:
-        self.cleanup_files = not self.config.preserve_downloads and not self.config.download_only
+        self.cleanup_files = (
+            not self.standard_config.preserve_downloads and not self.standard_config.download_only
+        )
 
     def cleanup(self, cur_dir=None):
         if not self.cleanup_files:
             return
 
         if cur_dir is None:
-            cur_dir = self.config.download_dir
+            cur_dir = self.standard_config.download_dir
         sub_dirs = os.listdir(cur_dir)
         os.chdir(cur_dir)
         for sub_dir in sub_dirs:
             # don't traverse symlinks, not that there every should be any
             if os.path.isdir(sub_dir) and not os.path.islink(sub_dir):
                 self.cleanup(sub_dir)
         os.chdir("..")
```

### Comparing `unstructured-0.6.6/unstructured/ingest/connector/github.py` & `unstructured-0.6.7/unstructured/ingest/connector/github.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,13 +76,13 @@
         repo = self.github.get_repo(self.config.repo_path)
 
         # Load the Git tree with all files, and then create Ingest docs
         # for all blobs, i.e. all files, ignoring directories
         sha = self.config.branch or repo.default_branch
         git_tree = repo.get_git_tree(sha, recursive=True)
         return [
-            GitHubIngestDoc(self.config, element.path, repo)
+            GitHubIngestDoc(self.standard_config, self.config, element.path, repo)
             for element in git_tree.tree
             if element.type == "blob"
             and self.is_file_type_supported(element.path)
             and (not self.config.file_glob or self.does_path_match_glob(element.path))
         ]
```

### Comparing `unstructured-0.6.6/unstructured/ingest/connector/gitlab.py` & `unstructured-0.6.7/unstructured/ingest/connector/gitlab.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,13 +60,13 @@
         git_tree = project.repository_tree(
             ref=ref,
             recursive=True,
             iterator=True,
             all=True,
         )
         return [
-            GitLabIngestDoc(self.config, element["path"], project)
+            GitLabIngestDoc(self.standard_config, self.config, element["path"], project)
             for element in git_tree
             if element["type"] == "blob"
             and self.is_file_type_supported(element["path"])
             and (not self.config.file_glob or self.does_path_match_glob(element["path"]))
         ]
```

### Comparing `unstructured-0.6.6/unstructured/ingest/connector/google_drive.py` & `unstructured-0.6.7/unstructured/ingest/connector/google_drive.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import io
 import json
 import os
 from dataclasses import dataclass
 from mimetypes import guess_extension
 from pathlib import Path
-from typing import Dict, Optional
+from typing import Dict
 
 from unstructured.file_utils.filetype import EXT_TO_FILETYPE
 from unstructured.file_utils.google_filetype import GOOGLE_DRIVE_EXPORT_TYPES
 from unstructured.ingest.interfaces import (
     BaseConnector,
     BaseConnectorConfig,
     BaseIngestDoc,
+    StandardConnectorConfig,
 )
 from unstructured.ingest.logger import logger
 from unstructured.utils import requires_dependencies
 
 FILE_FORMAT = "{id}-{name}{ext}"
 DIRECTORY_FORMAT = "{id}-{name}"
 
@@ -66,29 +67,14 @@
     """Connector config where drive_id is the id of the document to process or
     the folder to process all documents from."""
 
     # Google Drive Specific Options
     drive_id: str
     service_account_key: str
     extension: str
-
-    # Standard Connector options
-    download_dir: str
-    # where to write structured data, with the directory structure matching drive path
-    output_dir: str
-    re_download: bool = False
-    download_only: bool = False
-    preserve_downloads: bool = False
-    metadata_include: Optional[str] = None
-    metadata_exclude: Optional[str] = None
-    partition_by_api: bool = False
-    partition_endpoint: str = "https://api.unstructured.io/general/v0/general"
-    fields_include: str = "element_id,text,type,metadata"
-    flatten_metadata: bool = False
-
     recursive: bool = False
 
     def __post_init__(self):
         if self.extension and self.extension not in EXT_TO_FILETYPE.keys():
             raise ValueError(
                 f"Extension not supported. "
                 f"Value MUST be one of {', '.join([k for k in EXT_TO_FILETYPE if k is not None])}.",
@@ -106,32 +92,36 @@
         return Path(self.file_meta.get("download_filepath")).resolve()  # type: ignore
 
     def _output_filename(self):
         return Path(f"{self.file_meta.get('output_filepath')}.json").resolve()
 
     def cleanup_file(self):
         if (
-            not self.config.preserve_downloads
+            not self.standard_config.preserve_downloads
             and self.filename.is_file()
-            and not self.config.download_only
+            and not self.standard_config.download_only
         ):
             logger.debug(f"Cleaning up {self}")
             Path.unlink(self.filename)
 
     def has_output(self):
         """Determine if structured output for this doc already exists."""
         output_filename = self._output_filename()
         return output_filename.is_file() and output_filename.stat()
 
     @requires_dependencies(["googleapiclient"], extras="google-drive")
     def get_file(self):
         from googleapiclient.errors import HttpError
         from googleapiclient.http import MediaIoBaseDownload
 
-        if not self.config.re_download and self.filename.is_file() and self.filename.stat():
+        if (
+            not self.standard_config.re_download
+            and self.filename.is_file()
+            and self.filename.stat()
+        ):
             logger.debug(f"File exists: {self.filename}, skipping download")
             return
 
         self.config.service = create_service_account_object(self.config.service_account_key)
 
         if self.file_meta.get("mimeType", "").startswith("application/vnd.google-apps"):
             export_mime = GOOGLE_DRIVE_EXPORT_TYPES.get(
@@ -177,29 +167,33 @@
                     logger.debug(f"File downloaded: {self.filename}.")
 
         if not saved:
             logger.error(f"Error while downloading and saving file: {self.filename}.")
 
     def write_result(self):
         """Write the structured json result for this doc. result must be json serializable."""
-        if self.config.download_only:
+        if self.standard_config.download_only:
             return
         output_filename = self._output_filename()
         output_filename.parent.mkdir(parents=True, exist_ok=True)
         with open(output_filename, "w") as output_f:
             output_f.write(json.dumps(self.isd_elems_no_filename, ensure_ascii=False, indent=2))
         logger.info(f"Wrote {output_filename}")
 
 
 class GoogleDriveConnector(BaseConnector):
     """Objects of this class support fetching documents from Google Drive"""
 
-    def __init__(self, config):
-        self.config = config
-        self.cleanup_files = not self.config.preserve_downloads and not self.config.download_only
+    config: SimpleGoogleDriveConfig
+
+    def __init__(self, standard_config: StandardConnectorConfig, config: SimpleGoogleDriveConfig):
+        super().__init__(standard_config, config)
+        self.cleanup_files = (
+            not self.standard_config.preserve_downloads and not self.standard_config.download_only
+        )
 
     def _list_objects(self, drive_id, recursive=False):
         files = []
 
         def traverse(drive_id, download_dir, output_dir, recursive=False):
             page_token = None
             while True:
@@ -256,23 +250,28 @@
                         meta["output_filepath"] = (output_dir / name).resolve()
                         files.append(meta)
 
                 page_token = response.get("nextPageToken", None)
                 if page_token is None:
                     break
 
-        traverse(drive_id, Path(self.config.download_dir), Path(self.config.output_dir), recursive)
+        traverse(
+            drive_id,
+            Path(self.standard_config.download_dir),
+            Path(self.standard_config.output_dir),
+            recursive,
+        )
         return files
 
     def cleanup(self, cur_dir=None):
         if not self.cleanup_files:
             return
 
         if cur_dir is None:
-            cur_dir = self.config.download_dir
+            cur_dir = self.standard_config.download_dir
 
         if cur_dir is None or not Path(cur_dir).is_dir():
             return
 
         sub_dirs = os.listdir(cur_dir)
         os.chdir(cur_dir)
         for sub_dir in sub_dirs:
@@ -286,8 +285,8 @@
     def initialize(self):
         pass
 
     def get_ingest_docs(self):
         files = self._list_objects(self.config.drive_id, self.config.recursive)
         # Setting to None because service object can't be pickled for multiprocessing.
         self.config.service = None
-        return [GoogleDriveIngestDoc(self.config, file) for file in files]
+        return [GoogleDriveIngestDoc(self.standard_config, self.config, file) for file in files]
```

### Comparing `unstructured-0.6.6/unstructured/ingest/connector/local.py` & `unstructured-0.6.7/unstructured/ingest/connector/local.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,36 +6,26 @@
 from pathlib import Path
 from typing import Optional, Type
 
 from unstructured.ingest.interfaces import (
     BaseConnector,
     BaseConnectorConfig,
     BaseIngestDoc,
+    StandardConnectorConfig,
 )
 from unstructured.ingest.logger import logger
 
 
 @dataclass
 class SimpleLocalConfig(BaseConnectorConfig):
-    output_dir: str
-
     # Local specific options
     input_path: str
     recursive: bool = False
     file_glob: Optional[str] = None
 
-    # base connector options
-    download_only: bool = False
-    metadata_include: Optional[str] = None
-    metadata_exclude: Optional[str] = None
-    partition_by_api: bool = False
-    partition_endpoint: str = "https://api.unstructured.io/general/v0/general"
-    fields_include: str = "element_id,text,type,metadata"
-    flatten_metadata: bool = False
-
     def __post_init__(self):
         if os.path.isfile(self.input_path):
             self.input_path_is_file = True
         else:
             self.input_path_is_file = False
 
 
@@ -59,43 +49,45 @@
 
     def get_file(self):
         """Not applicable to local file system"""
         pass
 
     def _output_filename(self):
         return (
-            Path(self.config.output_dir)
+            Path(self.standard_config.output_dir)
             / f"{self.path.replace(f'{self.config.input_path}/', '')}.json"
         )
 
     def has_output(self):
         """Determine if structured output for this doc already exists."""
         return self._output_filename().is_file() and os.path.getsize(self._output_filename())
 
     def write_result(self):
         """Write the structured json result for this doc. result must be json serializable."""
-        if self.config.download_only:
+        if self.standard_config.download_only:
             return
         output_filename = self._output_filename()
         output_filename.parent.mkdir(parents=True, exist_ok=True)
         with open(output_filename, "w") as output_f:
             output_f.write(json.dumps(self.isd_elems_no_filename, ensure_ascii=False, indent=2))
         logger.info(f"Wrote {output_filename}")
 
 
 class LocalConnector(BaseConnector):
     """Objects of this class support fetching document(s) from local file system"""
 
+    config: SimpleLocalConfig
     ingest_doc_cls: Type[LocalIngestDoc] = LocalIngestDoc
 
     def __init__(
         self,
+        standard_config: StandardConnectorConfig,
         config: SimpleLocalConfig,
     ):
-        self.config = config
+        super().__init__(standard_config, config)
 
     def cleanup(self, cur_dir=None):
         """Not applicable to local file system"""
         pass
 
     def initialize(self):
         """Not applicable to local file system"""
@@ -118,13 +110,14 @@
                 return True
         logger.debug(f"The file {path!r} is discarded as it does not match any given glob.")
         return False
 
     def get_ingest_docs(self):
         return [
             self.ingest_doc_cls(
+                self.standard_config,
                 self.config,
                 file,
             )
             for file in self._list_files()
             if os.path.isfile(file) and self.does_path_match_glob(file)
         ]
```

### Comparing `unstructured-0.6.6/unstructured/ingest/connector/reddit.py` & `unstructured-0.6.7/unstructured/ingest/connector/reddit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import json
 import os
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING
 
 from unstructured.ingest.interfaces import (
     BaseConnector,
     BaseConnectorConfig,
     BaseIngestDoc,
+    StandardConnectorConfig,
 )
 from unstructured.ingest.logger import logger
 from unstructured.utils import requires_dependencies
 
 if TYPE_CHECKING:
     from praw.models import Submission
 
@@ -21,58 +22,48 @@
     subreddit_name: str
     client_id: str
     client_secret: str
     user_agent: str
     search_query: str
     num_posts: int
 
-    # Standard Connector options
-    download_dir: str
-    # where to write structured data
-    output_dir: str
-    preserve_downloads: bool = False
-    re_download: bool = False
-    download_only: bool = False
-    metadata_include: Optional[str] = None
-    metadata_exclude: Optional[str] = None
-    partition_by_api: bool = False
-    partition_endpoint: str = "https://api.unstructured.io/general/v0/general"
-    fields_include: str = "element_id,text,type,metadata"
-    flatten_metadata: bool = False
-
     def __post_init__(self):
         if self.num_posts <= 0:
             raise ValueError("The number of Reddit posts to fetch must be positive.")
 
 
 @dataclass
 class RedditIngestDoc(BaseIngestDoc):
     config: SimpleRedditConfig = field(repr=False)
     post: "Submission"
 
     @property
     def filename(self) -> Path:
-        return (Path(self.config.download_dir) / f"{self.post.id}.md").resolve()
+        return (Path(self.standard_config.download_dir) / f"{self.post.id}.md").resolve()
 
     def _output_filename(self):
-        return Path(self.config.output_dir) / f"{self.post.id}.json"
+        return Path(self.standard_config.output_dir) / f"{self.post.id}.json"
 
     def _create_full_tmp_dir_path(self):
         self.filename.parent.mkdir(parents=True, exist_ok=True)
 
     def cleanup_file(self):
         """Removes the local copy of the file (or anything else) after successful processing."""
-        if not self.config.preserve_downloads and not self.config.download_only:
+        if not self.standard_config.preserve_downloads and not self.standard_config.download_only:
             logger.debug(f"Cleaning up {self}")
             os.unlink(self.filename)
 
     def get_file(self):
         """Fetches the "remote" doc and stores it locally on the filesystem."""
         self._create_full_tmp_dir_path()
-        if not self.config.re_download and self.filename.is_file() and self.filename.stat():
+        if (
+            not self.standard_config.re_download
+            and self.filename.is_file()
+            and self.filename.stat()
+        ):
             logger.debug(f"File exists: {self.filename}, skipping download")
             return
 
         logger.debug(f"Fetching {self} - PID: {os.getpid()}")
         # Write the title plus the body, if any
         text_to_write = f"# {self.post.title}\n{self.post.selftext}"
         with open(self.filename, "w", encoding="utf8") as f:
@@ -81,42 +72,46 @@
     def has_output(self):
         """Determine if structured output for this doc already exists."""
         output_filename = self._output_filename()
         return output_filename.is_file() and output_filename.stat()
 
     def write_result(self):
         """Write the structured json result for this doc. result must be json serializable."""
-        if self.config.download_only:
+        if self.standard_config.download_only:
             return
         output_filename = self._output_filename()
         output_filename.parent.mkdir(parents=True, exist_ok=True)
         with open(output_filename, "w", encoding="utf8") as output_f:
             json.dump(self.isd_elems_no_filename, output_f, ensure_ascii=False, indent=2)
         logger.info(f"Wrote {output_filename}")
 
 
 @requires_dependencies(["praw"], extras="reddit")
 class RedditConnector(BaseConnector):
-    def __init__(self, config: SimpleRedditConfig):
+    config: SimpleRedditConfig
+
+    def __init__(self, standard_config: StandardConnectorConfig, config: SimpleRedditConfig):
         from praw import Reddit
 
-        self.config = config
+        super().__init__(standard_config, config)
         self.reddit = Reddit(
             client_id=config.client_id,
             client_secret=config.client_secret,
             user_agent=config.user_agent,
         )
-        self.cleanup_files = not config.preserve_downloads and not config.download_only
+        self.cleanup_files = (
+            not standard_config.preserve_downloads and not standard_config.download_only
+        )
 
     def cleanup(self, cur_dir=None):
         if not self.cleanup_files:
             return
 
         if cur_dir is None:
-            cur_dir = self.config.download_dir
+            cur_dir = self.standard_config.download_dir
         sub_dirs = os.listdir(cur_dir)
         os.chdir(cur_dir)
         for sub_dir in sub_dirs:
             # don't traverse symlinks, not that there every should be any
             if os.path.isdir(sub_dir) and not os.path.islink(sub_dir):
                 self.cleanup(sub_dir)
         os.chdir("..")
@@ -128,8 +123,8 @@
 
     def get_ingest_docs(self):
         subreddit = self.reddit.subreddit(self.config.subreddit_name)
         if self.config.search_query:
             posts = subreddit.search(self.config.search_query, limit=self.config.num_posts)
         else:
             posts = subreddit.hot(limit=self.config.num_posts)
-        return [RedditIngestDoc(self.config, post) for post in posts]
+        return [RedditIngestDoc(self.standard_config, self.config, post) for post in posts]
```

### Comparing `unstructured-0.6.6/unstructured/ingest/connector/s3.py` & `unstructured-0.6.7/unstructured/ingest/connector/s3.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Type
 
 from unstructured.ingest.connector.fsspec import (
     FsspecConnector,
     FsspecIngestDoc,
     SimpleFsspecConfig,
 )
+from unstructured.ingest.interfaces import StandardConnectorConfig
 from unstructured.utils import requires_dependencies
 
 
 @dataclass
 class SimpleS3Config(SimpleFsspecConfig):
     pass
 
@@ -23,9 +24,10 @@
 @requires_dependencies(["s3fs", "fsspec"], extras="s3")
 class S3Connector(FsspecConnector):
     ingest_doc_cls: Type[S3IngestDoc] = S3IngestDoc
 
     def __init__(
         self,
         config: SimpleS3Config,
+        standard_config: StandardConnectorConfig,
     ) -> None:
-        super().__init__(config=config)
+        super().__init__(standard_config, config)
```

### Comparing `unstructured-0.6.6/unstructured/ingest/connector/slack.py` & `unstructured-0.6.7/unstructured/ingest/connector/slack.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import json
 import os
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
-from typing import List, Optional
+from typing import List
 
 from slack_sdk import WebClient
 from slack_sdk.errors import SlackApiError
 
 from unstructured.ingest.interfaces import (
     BaseConnector,
     BaseConnectorConfig,
     BaseIngestDoc,
+    StandardConnectorConfig,
 )
 from unstructured.ingest.logger import logger
 from unstructured.utils import (
     requires_dependencies,
     validate_date_args,
 )
 
@@ -26,27 +27,14 @@
 class SimpleSlackConfig(BaseConnectorConfig):
     """Connector config to process all messages by channel id's."""
 
     channels: List[str]
     token: str
     oldest: str
     latest: str
-
-    # Standard Connector options
-    download_dir: str
-    output_dir: str
-    re_download: bool = False
-    preserve_downloads: bool = False
-    download_only: bool = False
-    metadata_include: Optional[str] = None
-    metadata_exclude: Optional[str] = None
-    partition_by_api: bool = False
-    partition_endpoint: str = "https://api.unstructured.io/general/v0/general"
-    fields_include: str = "element_id,text,type,metadata"
-    flatten_metadata: bool = False
     verbose: bool = False
 
     def validate_inputs(self):
         oldest_valid = True
         latest_valid = True
 
         if self.oldest:
@@ -86,34 +74,34 @@
     latest: str
 
     # NOTE(crag): probably doesn't matter,  but intentionally not defining tmp_download_file
     # __post_init__ for multiprocessing simplicity (no Path objects in initially
     # instantiated object)
     def _tmp_download_file(self):
         channel_file = self.channel + ".txt"
-        return Path(self.config.download_dir) / channel_file
+        return Path(self.standard_config.download_dir) / channel_file
 
     def _output_filename(self):
         output_file = self.channel + ".json"
-        return Path(self.config.output_dir) / output_file
+        return Path(self.standard_config.output_dir) / output_file
 
     def has_output(self):
         """Determine if structured output for this doc already exists."""
         return self._output_filename().is_file() and os.path.getsize(self._output_filename())
 
     def _create_full_tmp_dir_path(self):
         self._tmp_download_file().parent.mkdir(parents=True, exist_ok=True)
 
     @requires_dependencies(dependencies=["slack_sdk"], extras="slack")
     def get_file(self):
         """Fetches the data from a slack channel and stores it locally."""
 
         self._create_full_tmp_dir_path()
         if (
-            not self.config.re_download
+            not self.standard_config.re_download
             and self._tmp_download_file().is_file()
             and os.path.getsize(self._tmp_download_file())
         ):
             if self.config.verbose:
                 logger.debug(f"File exists: {self._tmp_download_file()}, skipping download")
             return
 
@@ -171,36 +159,38 @@
     @property
     def filename(self):
         """The filename of the file created from a slack channel"""
         return self._tmp_download_file()
 
     def cleanup_file(self):
         """Removes the local copy the file after successful processing."""
-        if not self.config.preserve_downloads:
+        if not self.standard_config.preserve_downloads:
             if self.config.verbose:
                 logger.info(f"cleaning up channel {self.channel}")
             os.unlink(self._tmp_download_file())
 
 
 @requires_dependencies(dependencies=["slack_sdk"], extras="slack")
 class SlackConnector(BaseConnector):
     """Objects of this class support fetching document(s) from"""
 
-    def __init__(self, config: SimpleSlackConfig):
-        self.config = config
-        self.cleanup_files = not config.preserve_downloads
+    config: SimpleSlackConfig
+
+    def __init__(self, standard_config: StandardConnectorConfig, config: SimpleSlackConfig):
+        super().__init__(standard_config, config)
+        self.cleanup_files = not standard_config.preserve_downloads
 
     def cleanup(self, cur_dir=None):
         """cleanup linginering empty sub-dirs, but leave remaining files
         (and their paths) in tact as that indicates they were not processed"""
         if not self.cleanup_files:
             return
 
         if cur_dir is None:
-            cur_dir = self.config.download_dir
+            cur_dir = self.standard_config.download_dir
         sub_dirs = os.listdir(cur_dir)
         os.chdir(cur_dir)
         for sub_dir in sub_dirs:
             # don't traverse symlinks, not that there every should be any
             if os.path.isdir(sub_dir) and not os.path.islink(sub_dir):
                 self.cleanup(sub_dir)
         os.chdir("..")
@@ -210,14 +200,15 @@
     def initialize(self):
         """Verify that can get metadata for an object, validates connections info."""
         pass
 
     def get_ingest_docs(self):
         return [
             SlackIngestDoc(
+                self.standard_config,
                 self.config,
                 channel,
                 self.config.token,
                 self.config.oldest,
                 self.config.latest,
             )
             for channel in self.config.channels
```

### Comparing `unstructured-0.6.6/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.6.7/unstructured/ingest/connector/wikipedia.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,30 @@
 import json
 import os
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING
 
 from unstructured.ingest.interfaces import (
     BaseConnector,
     BaseConnectorConfig,
     BaseIngestDoc,
+    StandardConnectorConfig,
 )
 from unstructured.ingest.logger import logger
 
 if TYPE_CHECKING:
     from wikipedia import WikipediaPage
 
 
 @dataclass
 class SimpleWikipediaConfig(BaseConnectorConfig):
     title: str
     auto_suggest: bool
 
-    # Standard Connector options
-    download_dir: str
-    # where to write structured data
-    output_dir: str
-    preserve_downloads: bool = False
-    re_download: bool = False
-    download_only: bool = False
-    metadata_include: Optional[str] = None
-    metadata_exclude: Optional[str] = None
-    partition_by_api: bool = False
-    partition_endpoint: str = "https://api.unstructured.io/general/v0/general"
-    fields_include: str = "element_id,text,type,metadata"
-    flatten_metadata: bool = False
-
 
 @dataclass
 class WikipediaIngestDoc(BaseIngestDoc):
     config: SimpleWikipediaConfig = field(repr=False)
     page: "WikipediaPage"
 
     @property
@@ -52,104 +39,121 @@
         raise NotImplementedError()
 
     def _create_full_tmp_dir_path(self):
         self.filename.parent.mkdir(parents=True, exist_ok=True)
 
     def cleanup_file(self):
         """Removes the local copy of the file (or anything else) after successful processing."""
-        if not self.config.preserve_downloads and not self.config.download_only:
+        if not self.standard_config.preserve_downloads and not self.standard_config.download_only:
             logger.debug(f"Cleaning up {self}")
             os.unlink(self.filename)
 
     def get_file(self):
         """Fetches the "remote" doc and stores it locally on the filesystem."""
         self._create_full_tmp_dir_path()
-        if not self.config.re_download and self.filename.is_file() and self.filename.stat():
+        if (
+            not self.standard_config.re_download
+            and self.filename.is_file()
+            and self.filename.stat()
+        ):
             logger.debug(f"File exists: {self.filename}, skipping download")
             return
 
         logger.debug(f"Fetching {self} - PID: {os.getpid()}")
         with open(self.filename, "w", encoding="utf8") as f:
             f.write(self.text)
 
     def has_output(self):
         """Determine if structured output for this doc already exists."""
         output_filename = self._output_filename()
         return output_filename.is_file() and output_filename.stat()
 
     def write_result(self):
         """Write the structured json result for this doc. result must be json serializable."""
-        if self.config.download_only:
+        if self.standard_config.download_only:
             return
         output_filename = self._output_filename()
         output_filename.parent.mkdir(parents=True, exist_ok=True)
         with open(output_filename, "w", encoding="utf8") as output_f:
             json.dump(self.isd_elems_no_filename, output_f, ensure_ascii=False, indent=2)
         logger.info(f"Wrote {output_filename}")
 
 
 class WikipediaIngestHTMLDoc(WikipediaIngestDoc):
     @property
     def filename(self) -> Path:
         return (
-            Path(self.config.download_dir) / f"{self.page.title}-{self.page.revision_id}.html"
+            Path(self.standard_config.download_dir)
+            / f"{self.page.title}-{self.page.revision_id}.html"
         ).resolve()
 
     @property
     def text(self):
         return self.page.html()
 
     def _output_filename(self):
-        return Path(self.config.output_dir) / f"{self.page.title}-{self.page.revision_id}-html.json"
+        return (
+            Path(self.standard_config.output_dir)
+            / f"{self.page.title}-{self.page.revision_id}-html.json"
+        )
 
 
 class WikipediaIngestTextDoc(WikipediaIngestDoc):
     @property
     def filename(self) -> Path:
         return (
-            Path(self.config.download_dir) / f"{self.page.title}-{self.page.revision_id}.txt"
+            Path(self.standard_config.download_dir)
+            / f"{self.page.title}-{self.page.revision_id}.txt"
         ).resolve()
 
     @property
     def text(self):
         return self.page.content
 
     def _output_filename(self):
-        return Path(self.config.output_dir) / f"{self.page.title}-{self.page.revision_id}-txt.json"
+        return (
+            Path(self.standard_config.output_dir)
+            / f"{self.page.title}-{self.page.revision_id}-txt.json"
+        )
 
 
 class WikipediaIngestSummaryDoc(WikipediaIngestDoc):
     @property
     def filename(self) -> Path:
         return (
-            Path(self.config.download_dir)
+            Path(self.standard_config.download_dir)
             / f"{self.page.title}-{self.page.revision_id}-summary.txt"
         ).resolve()
 
     @property
     def text(self):
         return self.page.summary
 
     def _output_filename(self):
         return (
-            Path(self.config.output_dir) / f"{self.page.title}-{self.page.revision_id}-summary.json"
+            Path(self.standard_config.output_dir)
+            / f"{self.page.title}-{self.page.revision_id}-summary.json"
         )
 
 
 class WikipediaConnector(BaseConnector):
-    def __init__(self, config: SimpleWikipediaConfig):
-        self.config = config
-        self.cleanup_files = not config.preserve_downloads and not config.download_only
+    config: SimpleWikipediaConfig
+
+    def __init__(self, config: SimpleWikipediaConfig, standard_config: StandardConnectorConfig):
+        super().__init__(standard_config, config)
+        self.cleanup_files = (
+            not standard_config.preserve_downloads and not standard_config.download_only
+        )
 
     def cleanup(self, cur_dir=None):
         if not self.cleanup_files:
             return
 
         if cur_dir is None:
-            cur_dir = self.config.download_dir
+            cur_dir = self.standard_config.download_dir
         sub_dirs = os.listdir(cur_dir)
         os.chdir(cur_dir)
         for sub_dir in sub_dirs:
             # don't traverse symlinks, not that there every should be any
             if os.path.isdir(sub_dir) and not os.path.islink(sub_dir):
                 self.cleanup(sub_dir)
         os.chdir("..")
@@ -158,13 +162,16 @@
 
     def initialize(self):
         pass
 
     def get_ingest_docs(self):
         import wikipedia
 
-        page = wikipedia.page(self.config.title, auto_suggest=self.config.auto_suggest)
+        page = wikipedia.page(
+            self.config.title,
+            auto_suggest=self.config.auto_suggest,
+        )
         return [
-            WikipediaIngestTextDoc(self.config, page),
-            WikipediaIngestHTMLDoc(self.config, page),
-            WikipediaIngestSummaryDoc(self.config, page),
+            WikipediaIngestTextDoc(self.standard_config, self.config, page),
+            WikipediaIngestHTMLDoc(self.standard_config, self.config, page),
+            WikipediaIngestSummaryDoc(self.standard_config, self.config, page),
         ]
```

### Comparing `unstructured-0.6.6/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.6.7/unstructured/ingest/doc_processor/generalized.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,23 +13,29 @@
     # Accessing this dictionary triggers standard model downloads for pdf processing.
     # There will be a better way to do this, see
     # https://github.com/Unstructured-IO/unstructured-inference/issues/55
     MODEL_TYPES[None]["model_path"]
     MODEL_TYPES[None]["config_path"]
 
 
-def process_document(doc: "IngestDoc") -> Optional[List[Dict[str, Any]]]:
-    """Process any IngestDoc-like class of document with Unstructured's auto partition logic."""
+def process_document(doc: "IngestDoc", **partition_kwargs) -> Optional[List[Dict[str, Any]]]:
+    """Process any IngestDoc-like class of document with choosen Unstructured's partition logic.
+
+    Parameters
+    ----------
+    partition_kwargs
+        ultimately the parameters passed to partition()
+    """
     isd_elems_no_filename = None
     try:
         # does the work necessary to load file into filesystem
         # in the future, get_file_handle() could also be supported
         doc.get_file()
 
-        isd_elems_no_filename = doc.process_file()
+        isd_elems_no_filename = doc.process_file(**partition_kwargs)
 
         # Note, this may be a no-op if the IngestDoc doesn't do anything to persist
         # the results. Instead, the MainProcess (caller) may work with the aggregate
         # results across all docs in memory.
         doc.write_result()
     except Exception:
         # TODO(crag) save the exception instead of print?
```

### Comparing `unstructured-0.6.6/unstructured/ingest/interfaces.py` & `unstructured-0.6.7/unstructured/ingest/interfaces.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,56 @@
 """Defines Abstract Base Classes (ABC's) core to batch processing documents
 through Unstructured."""
 
 from abc import ABC, abstractmethod
+from dataclasses import dataclass
 from typing import Optional
 
 import requests
 
 from unstructured.ingest.logger import logger
 from unstructured.partition.auto import partition
 from unstructured.staging.base import convert_to_dict
 
 
+@dataclass
+class StandardConnectorConfig:
+    """Common set of config options passed to all connectors."""
+
+    # where raw documents are stored for processing, and then removed if not preserve_downloads
+    download_dir: str
+    # where to write structured data outputs
+    output_dir: str
+    download_only: bool = False
+    fields_include: str = "element_id,text,type,metadata"
+    flatten_metadata: bool = False
+    metadata_exclude: Optional[str] = None
+    metadata_include: Optional[str] = None
+    partition_by_api: bool = False
+    partition_endpoint: str = "https://api.unstructured.io/general/v0/general"
+    preserve_downloads: bool = False
+    re_download: bool = False
+
+
+class BaseConnectorConfig(ABC):
+    """Abstract definition on which to define connector-specific attributes."""
+
+
+@dataclass
 class BaseConnector(ABC):
     """Abstract Base Class for a connector to a remote source, e.g. S3 or Google Drive."""
 
-    def __init__(self, config):
-        """Expects a config object that implements BaseConnectorConfig."""
-        pass
+    standard_config: StandardConnectorConfig
+    config: BaseConnectorConfig
+
+    def __init__(self, standard_config: StandardConnectorConfig, config: BaseConnectorConfig):
+        """Expects a standard_config object that implements StandardConnectorConfig
+        and config object that implements BaseConnectorConfig."""
+        self.standard_config = standard_config
+        self.config = config
 
     @abstractmethod
     def cleanup(self, cur_dir=None):
         """Any additional cleanup up need after processing is complete. E.g., removing
         temporary download dirs that are empty.
 
         By convention, documents that failed to process are typically not cleaned up."""
@@ -37,41 +67,25 @@
         """Returns all ingest docs (derived from BaseIngestDoc).
         This does not imply downloading all the raw documents themselves,
         rather each IngestDoc is capable of fetching its content (in another process)
         with IngestDoc.get_file()."""
         pass
 
 
-class BaseConnectorConfig(ABC):
-    """All connector configs must respect these attr's."""
-
-    # where raw documents are stored for processing, and then removed if not preserve_downloads
-    download_dir: str
-    preserve_downloads: bool = False
-    # where to write structured data outputs
-    output_dir: str
-    re_download: bool = False
-    download_only: bool = False
-    metadata_include: Optional[str] = None
-    metadata_exclude: Optional[str] = None
-    partition_by_api: bool = False
-    partition_endpoint: str = "https://api.unstructured.io/general/v0/general"
-    fields_include: str = "element_id,text,type,metadata"
-    flatten_metadata: bool = False
-
-
+@dataclass
 class BaseIngestDoc(ABC):
     """An "ingest document" is specific to a connector, and provides
     methods to fetch a single raw document, store it locally for processing, any cleanup
     needed after successful processing of the doc, and the ability to write the doc's
     structured outputs once processed.
 
     Crucially, it is not responsible for the actual processing of the raw document.
     """
 
+    standard_config: StandardConnectorConfig
     config: BaseConnectorConfig
 
     @property
     @abstractmethod
     def filename(self):
         """The local filename of the document after fetching from remote source."""
 
@@ -93,68 +107,68 @@
         pass
 
     @abstractmethod
     def write_result(self):
         """Write the structured json result for this doc. result must be json serializable."""
         pass
 
-    def partition_file(self):
-        if not self.config.partition_by_api:
+    def partition_file(self, **partition_kwargs):
+        if not self.standard_config.partition_by_api:
             logger.debug("Using local partition")
-            elements = partition(filename=str(self.filename))
+            elements = partition(filename=str(self.filename), **partition_kwargs)
             return convert_to_dict(elements)
 
         else:
-            endpoint = self.config.partition_endpoint
+            endpoint = self.standard_config.partition_endpoint
 
             logger.debug(f"Using remote partition ({endpoint})")
 
             with open(self.filename, "rb") as f:
                 response = requests.post(
                     f"{endpoint}",
                     files={"files": (str(self.filename), f)},
                 )
 
             if response.status_code != 200:
                 raise RuntimeError(f"Caught {response.status_code} from API: {response.text}")
 
             return response.json()
 
-    def process_file(self):
-        if self.config.download_only:
+    def process_file(self, **partition_kwargs):
+        if self.standard_config.download_only:
             return
         logger.info(f"Processing {self.filename}")
 
-        isd_elems = self.partition_file()
+        isd_elems = self.partition_file(**partition_kwargs)
 
         self.isd_elems_no_filename = []
         for elem in isd_elems:
             # type: ignore
             if (
-                self.config.metadata_exclude is not None
-                and self.config.metadata_include is not None
+                self.standard_config.metadata_exclude is not None
+                and self.standard_config.metadata_include is not None
             ):
                 raise ValueError(
                     "Arguments `--metadata-include` and `--metadata-exclude` are "
                     "mutually exclusive with each other.",
                 )
-            elif self.config.metadata_exclude is not None:
-                ex_list = self.config.metadata_exclude.split(",")
+            elif self.standard_config.metadata_exclude is not None:
+                ex_list = self.standard_config.metadata_exclude.split(",")
                 for ex in ex_list:
                     elem["metadata"].pop(ex, None)  # type: ignore[attr-defined]
-            elif self.config.metadata_include is not None:
-                in_list = self.config.metadata_include.split(",")
+            elif self.standard_config.metadata_include is not None:
+                in_list = self.standard_config.metadata_include.split(",")
                 for k in list(elem["metadata"].keys()):  # type: ignore[attr-defined]
                     if k not in in_list:
                         elem["metadata"].pop(k, None)  # type: ignore[attr-defined]
 
-            in_list = self.config.fields_include.split(",")
+            in_list = self.standard_config.fields_include.split(",")
             elem = {k: v for k, v in elem.items() if k in in_list}
 
-            if self.config.flatten_metadata:
+            if self.standard_config.flatten_metadata:
                 for k, v in elem["metadata"].items():  # type: ignore[attr-defined]
                     elem[k] = v
                 elem.pop("metadata")  # type: ignore[attr-defined]
 
             self.isd_elems_no_filename.append(elem)
 
         return self.isd_elems_no_filename
```

### Comparing `unstructured-0.6.6/unstructured/ingest/main.py` & `unstructured-0.6.7/unstructured/ingest/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 import hashlib
 import logging
 import multiprocessing as mp
 import sys
 import warnings
 from contextlib import suppress
+from functools import partial
 from pathlib import Path
 from urllib.parse import urlparse
 
 import click
 
 from unstructured.ingest.connector.wikipedia import (
     SimpleWikipediaConfig,
@@ -139,14 +140,20 @@
 @click.option(
     "--partition-endpoint",
     default="https://api.unstructured.io/general/v0/general",
     help="If partitioning via api, use the following host. "
     "Default: https://api.unstructured.io/general/v0/general",
 )
 @click.option(
+    "--partition-strategy",
+    default="auto",
+    help="The method that will be used to process the documents. "
+    "Default: auto. Other strategies include `fast` and `hi_res`.",
+)
+@click.option(
     "--local-input-path",
     default=None,
     help="Path to the location in the local file system that will be processed.",
 )
 @click.option(
     "--local-recursive",
     is_flag=True,
@@ -162,20 +169,14 @@
 @click.option(
     "--remote-url",
     default=None,
     help="Remote fsspec URL formatted as `protocol://dir/path`, it can contain both "
     "a directory or a single file. Supported protocols are: `s3`, `s3a`, `abfs`, and `az`.",
 )
 @click.option(
-    "--s3-url",
-    default=None,
-    help="Prefix of s3 objects (files) to download. E.g. s3://bucket1/path/. This value may "
-    "also be a single file. To be deprecated in favor of --remote-url.",
-)
-@click.option(
     "--s3-anonymous",
     is_flag=True,
     default=False,
     help="Connect to s3 without local AWS credentials.",
 )
 @click.option(
     "--azure-account-name",
@@ -341,14 +342,30 @@
 @click.option(
     "--end-date",
     default=None,
     help="End date/time in formats YYYY-MM-DD or YYYY-MM-DDTHH:MM:SS or "
     "YYYY-MM-DD+HH:MM:SS or YYYY-MM-DDTHH:MM:SStz",
 )
 @click.option(
+    "--discord-channels",
+    default=None,
+    help="A comma separated list of discord channel ids to ingest from.",
+)
+@click.option(
+    "--discord-token",
+    default=None,
+    help="Bot token used to access Discord API, must have "
+    "READ_MESSAGE_HISTORY scope for the bot user",
+)
+@click.option(
+    "--discord-period",
+    default=None,
+    help="Number of days to go back in the history of discord channels, must be an number",
+)
+@click.option(
     "--download-dir",
     help="Where files are downloaded to, defaults to `$HOME/.cache/unstructured/ingest/<SHA256>`.",
 )
 @click.option(
     "--preserve-downloads",
     is_flag=True,
     default=False,
@@ -372,15 +389,14 @@
     default=2,
     show_default=True,
     help="Number of parallel processes to process docs in.",
 )
 @click.option("-v", "--verbose", is_flag=True, default=False)
 def main(
     remote_url,
-    s3_url,  # TODO: deprecate this in the next minor release
     s3_anonymous,
     azure_account_name,
     azure_account_key,
     azure_connection_string,
     drive_id,
     drive_service_account_key,
     drive_recursive,
@@ -403,27 +419,31 @@
     reddit_search_query,
     reddit_num_posts,
     re_download,
     slack_channels,
     slack_token,
     start_date,
     end_date,
+    discord_channels,
+    discord_token,
+    discord_period,
     download_dir,
     preserve_downloads,
     structured_output_dir,
     reprocess,
     num_processes,
     verbose,
     metadata_include,
     metadata_exclude,
     fields_include,
     flatten_metadata,
     max_docs,
     partition_by_api,
     partition_endpoint,
+    partition_strategy,
     local_input_path,
     local_recursive,
     local_file_glob,
     download_only,
 ):
     if flatten_metadata and "metadata" not in fields_include:
         logger.warning(
@@ -454,25 +474,20 @@
         )
     if local_input_path is not None and download_dir:
         logger.warning(
             "Files should already be in local file system: there is nothing to download, "
             "but --download-dir is specified.",
         )
         sys.exit(1)
+    from unstructured.ingest.interfaces import StandardConnectorConfig
+
     if local_input_path is None and not download_dir:
         cache_path = Path.home() / ".cache" / "unstructured" / "ingest"
         if not cache_path.exists():
             cache_path.mkdir(parents=True, exist_ok=True)
-        if s3_url:
-            warnings.warn(
-                "The `--s3-url` option will be deprecated in favor of `--remote-url`"
-                " in the next minor release.",
-                DeprecationWarning,
-            )
-            remote_url = s3_url
         if remote_url:
             hashed_dir_name = hashlib.sha256(remote_url.encode("utf-8"))
         elif github_url:
             hashed_dir_name = hashlib.sha256(
                 f"{github_url}_{git_branch}".encode("utf-8"),
             )
         elif gitlab_url:
@@ -507,34 +522,37 @@
             )
         download_dir = cache_path / hashed_dir_name.hexdigest()[:10]
         if preserve_downloads:
             logger.warning(
                 f"Preserving downloaded files but --download-dir is not specified,"
                 f" using {download_dir}",
             )
+    standard_config = StandardConnectorConfig(
+        download_dir=download_dir,
+        output_dir=structured_output_dir,
+        download_only=download_only,
+        fields_include=fields_include,
+        flatten_metadata=flatten_metadata,
+        metadata_exclude=metadata_exclude,
+        metadata_include=metadata_include,
+        partition_by_api=partition_by_api,
+        partition_endpoint=partition_endpoint,
+        preserve_downloads=preserve_downloads,
+        re_download=re_download,
+    )
     if remote_url:
         protocol = urlparse(remote_url).scheme
         if protocol in ("s3", "s3a"):
             from unstructured.ingest.connector.s3 import S3Connector, SimpleS3Config
 
             doc_connector = S3Connector(  # type: ignore
+                standard_config=standard_config,
                 config=SimpleS3Config(
-                    path=s3_url,
+                    path=remote_url,
                     access_kwargs={"anon": s3_anonymous},
-                    download_dir=download_dir,
-                    output_dir=structured_output_dir,
-                    re_download=re_download,
-                    preserve_downloads=preserve_downloads,
-                    metadata_include=metadata_include,
-                    metadata_exclude=metadata_exclude,
-                    partition_by_api=partition_by_api,
-                    partition_endpoint=partition_endpoint,
-                    fields_include=fields_include,
-                    flatten_metadata=flatten_metadata,
-                    download_only=download_only,
                 ),
             )
         elif protocol in ("abfs", "az"):
             from unstructured.ingest.connector.azure import (
                 AzureBlobStorageConnector,
                 SimpleAzureBlobStorageConfig,
             )
@@ -545,28 +563,18 @@
                     "account_key": azure_account_key,
                 }
             elif azure_connection_string:
                 access_kwargs = {"connection_string": azure_connection_string}
             else:
                 access_kwargs = {}
             doc_connector = AzureBlobStorageConnector(  # type: ignore
+                standard_config=standard_config,
                 config=SimpleAzureBlobStorageConfig(
                     path=remote_url,
                     access_kwargs=access_kwargs,
-                    download_dir=download_dir,
-                    output_dir=structured_output_dir,
-                    re_download=re_download,
-                    preserve_downloads=preserve_downloads,
-                    metadata_include=metadata_include,
-                    metadata_exclude=metadata_exclude,
-                    partition_by_api=partition_by_api,
-                    partition_endpoint=partition_endpoint,
-                    fields_include=fields_include,
-                    flatten_metadata=flatten_metadata,
-                    download_only=download_only,
                 ),
             )
         else:
             warnings.warn(
                 f"`fsspec` protocol {protocol} is not directly supported by `unstructured`,"
                 " so use it at your own risk. Supported protocols are `s3`, `s3a`, `abfs`,"
                 " and `az`.",
@@ -575,231 +583,164 @@
 
             from unstructured.ingest.connector.fsspec import (
                 FsspecConnector,
                 SimpleFsspecConfig,
             )
 
             doc_connector = FsspecConnector(  # type: ignore
+                standard_config=standard_config,
                 config=SimpleFsspecConfig(
                     path=remote_url,
-                    download_dir=download_dir,
-                    output_dir=structured_output_dir,
-                    re_download=re_download,
-                    preserve_downloads=preserve_downloads,
-                    metadata_include=metadata_include,
-                    metadata_exclude=metadata_exclude,
-                    partition_by_api=partition_by_api,
-                    partition_endpoint=partition_endpoint,
-                    fields_include=fields_include,
-                    flatten_metadata=flatten_metadata,
-                    download_only=download_only,
                 ),
             )
     elif github_url:
         from unstructured.ingest.connector.github import (
             GitHubConnector,
             SimpleGitHubConfig,
         )
 
         doc_connector = GitHubConnector(  # type: ignore
+            standard_config=standard_config,
             config=SimpleGitHubConfig(
                 url=github_url,
                 access_token=git_access_token,
                 branch=git_branch,
                 file_glob=git_file_glob,
-                # defaults params:
-                download_dir=download_dir,
-                preserve_downloads=preserve_downloads,
-                output_dir=structured_output_dir,
-                re_download=re_download,
-                metadata_include=metadata_include,
-                metadata_exclude=metadata_exclude,
-                partition_by_api=partition_by_api,
-                partition_endpoint=partition_endpoint,
-                fields_include=fields_include,
-                flatten_metadata=flatten_metadata,
-                download_only=download_only,
             ),
         )
     elif gitlab_url:
         from unstructured.ingest.connector.gitlab import (
             GitLabConnector,
             SimpleGitLabConfig,
         )
 
         doc_connector = GitLabConnector(  # type: ignore
+            standard_config=standard_config,
             config=SimpleGitLabConfig(
                 url=gitlab_url,
                 access_token=git_access_token,
                 branch=git_branch,
                 file_glob=git_file_glob,
-                # defaults params:
-                download_dir=download_dir,
-                preserve_downloads=preserve_downloads,
-                output_dir=structured_output_dir,
-                re_download=re_download,
-                metadata_include=metadata_include,
-                metadata_exclude=metadata_exclude,
-                partition_by_api=partition_by_api,
-                partition_endpoint=partition_endpoint,
-                fields_include=fields_include,
-                flatten_metadata=flatten_metadata,
-                download_only=download_only,
             ),
         )
     elif subreddit_name:
         from unstructured.ingest.connector.reddit import (
             RedditConnector,
             SimpleRedditConfig,
         )
 
         doc_connector = RedditConnector(  # type: ignore
+            standard_config=standard_config,
             config=SimpleRedditConfig(
                 subreddit_name=subreddit_name,
                 client_id=reddit_client_id,
                 client_secret=reddit_client_secret,
                 user_agent=reddit_user_agent,
                 search_query=reddit_search_query,
                 num_posts=reddit_num_posts,
-                # defaults params:
-                download_dir=download_dir,
-                preserve_downloads=preserve_downloads,
-                output_dir=structured_output_dir,
-                re_download=re_download,
-                metadata_include=metadata_include,
-                metadata_exclude=metadata_exclude,
-                partition_by_api=partition_by_api,
-                partition_endpoint=partition_endpoint,
-                fields_include=fields_include,
-                flatten_metadata=flatten_metadata,
-                download_only=download_only,
             ),
         )
     elif slack_channels:
         from unstructured.ingest.connector.slack import (
             SimpleSlackConfig,
             SlackConnector,
         )
 
         doc_connector = SlackConnector(  # type: ignore
+            standard_config=standard_config,
             config=SimpleSlackConfig(
                 channels=SimpleSlackConfig.parse_channels(slack_channels),
                 token=slack_token,
                 oldest=start_date,
                 latest=end_date,
-                # defaults params:
-                download_dir=download_dir,
-                preserve_downloads=preserve_downloads,
-                output_dir=structured_output_dir,
-                re_download=re_download,
+                verbose=verbose,
+            ),
+        )
+    elif discord_channels:
+        from unstructured.ingest.connector.discord import (
+            DiscordConnector,
+            SimpleDiscordConfig,
+        )
+
+        doc_connector = DiscordConnector(  # type: ignore
+            standard_config=standard_config,
+            config=SimpleDiscordConfig(
+                channels=SimpleDiscordConfig.parse_channels(discord_channels),
+                days=discord_period,
+                token=discord_token,
                 verbose=verbose,
             ),
         )
     elif wikipedia_page_title:
         doc_connector = WikipediaConnector(  # type: ignore
+            standard_config=standard_config,
             config=SimpleWikipediaConfig(
                 title=wikipedia_page_title,
                 auto_suggest=wikipedia_auto_suggest,
-                # defaults params:
-                download_dir=download_dir,
-                preserve_downloads=preserve_downloads,
-                output_dir=structured_output_dir,
-                re_download=re_download,
-                metadata_include=metadata_include,
-                metadata_exclude=metadata_exclude,
-                partition_by_api=partition_by_api,
-                partition_endpoint=partition_endpoint,
-                fields_include=fields_include,
-                flatten_metadata=flatten_metadata,
-                download_only=download_only,
             ),
         )
     elif drive_id:
         from unstructured.ingest.connector.google_drive import (
             GoogleDriveConnector,
             SimpleGoogleDriveConfig,
         )
 
         doc_connector = GoogleDriveConnector(  # type: ignore
+            standard_config=standard_config,
             config=SimpleGoogleDriveConfig(
                 drive_id=drive_id,
                 service_account_key=drive_service_account_key,
                 recursive=drive_recursive,
                 extension=drive_extension,
-                # defaults params:
-                download_dir=download_dir,
-                preserve_downloads=preserve_downloads,
-                output_dir=structured_output_dir,
-                re_download=re_download,
-                metadata_include=metadata_include,
-                metadata_exclude=metadata_exclude,
-                partition_by_api=partition_by_api,
-                partition_endpoint=partition_endpoint,
-                fields_include=fields_include,
-                flatten_metadata=flatten_metadata,
-                download_only=download_only,
             ),
         )
     elif biomed_path or biomed_api_id or biomed_api_from or biomed_api_until:
         from unstructured.ingest.connector.biomed import (
             BiomedConnector,
             SimpleBiomedConfig,
         )
 
         doc_connector = BiomedConnector(  # type: ignore
+            standard_config=standard_config,
             config=SimpleBiomedConfig(
                 path=biomed_path,
                 id_=biomed_api_id,
                 from_=biomed_api_from,
                 until=biomed_api_until,
-                # defaults params:
-                download_dir=download_dir,
-                preserve_downloads=preserve_downloads,
-                output_dir=structured_output_dir,
-                re_download=re_download,
-                metadata_include=metadata_include,
-                metadata_exclude=metadata_exclude,
-                partition_by_api=partition_by_api,
-                partition_endpoint=partition_endpoint,
-                fields_include=fields_include,
-                flatten_metadata=flatten_metadata,
-                download_only=download_only,
             ),
         )
     elif local_input_path:
         from unstructured.ingest.connector.local import (
             LocalConnector,
             SimpleLocalConfig,
         )
 
         doc_connector = LocalConnector(  # type: ignore
+            standard_config=standard_config,
             config=SimpleLocalConfig(
                 input_path=local_input_path,
                 recursive=local_recursive,
                 file_glob=local_file_glob,
-                # defaults params:
-                output_dir=structured_output_dir,
-                metadata_include=metadata_include,
-                metadata_exclude=metadata_exclude,
-                partition_by_api=partition_by_api,
-                partition_endpoint=partition_endpoint,
-                fields_include=fields_include,
-                flatten_metadata=flatten_metadata,
             ),
         )
     # Check for other connector-specific options here and define the doc_connector object
     # e.g. "elif azure_container:  ..."
 
     else:
         logger.error("No connector-specific option was specified!")
         sys.exit(1)
 
+    process_document_with_partition_strategy = partial(
+        process_document,
+        strategy=partition_strategy,
+    )
+
     MainProcess(
         doc_connector=doc_connector,
-        doc_processor_fn=process_document,
+        doc_processor_fn=process_document_with_partition_strategy,
         num_processes=num_processes,
         reprocess=reprocess,
         verbose=verbose,
         max_docs=max_docs,
     ).run()
```

### Comparing `unstructured-0.6.6/unstructured/nlp/english-words.txt` & `unstructured-0.6.7/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/nlp/english_words.py` & `unstructured-0.6.7/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/nlp/patterns.py` & `unstructured-0.6.7/unstructured/nlp/patterns.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/nlp/tokenize.py` & `unstructured-0.6.7/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/partition/__init__.py` & `unstructured-0.6.7/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/partition/api.py` & `unstructured-0.6.7/unstructured/partition/api.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/partition/auto.py` & `unstructured-0.6.7/unstructured/partition/auto.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import io
 from typing import IO, Callable, Dict, Optional, Tuple
 
 import requests
 
-from unstructured.file_utils.filetype import FileType, detect_filetype
+from unstructured.file_utils.filetype import (
+    FILETYPE_TO_MIMETYPE,
+    STR_TO_FILETYPE,
+    FileType,
+    detect_filetype,
+)
 from unstructured.logger import logger
 from unstructured.partition.common import exactly_one
 from unstructured.partition.doc import partition_doc
 from unstructured.partition.docx import partition_docx
 from unstructured.partition.email import partition_email
 from unstructured.partition.epub import partition_epub
 from unstructured.partition.html import partition_html
@@ -17,30 +22,33 @@
 from unstructured.partition.msg import partition_msg
 from unstructured.partition.odt import partition_odt
 from unstructured.partition.pdf import partition_pdf
 from unstructured.partition.ppt import partition_ppt
 from unstructured.partition.pptx import partition_pptx
 from unstructured.partition.rtf import partition_rtf
 from unstructured.partition.text import partition_text
+from unstructured.partition.xlsx import partition_xlsx
+from unstructured.partition.xml import partition_xml
 
 
 def partition(
     filename: Optional[str] = None,
     content_type: Optional[str] = None,
     file: Optional[IO] = None,
     file_filename: Optional[str] = None,
     url: Optional[str] = None,
     include_page_breaks: bool = False,
-    strategy: str = "hi_res",
+    strategy: str = "auto",
     encoding: str = "utf-8",
     paragraph_grouper: Optional[Callable[[str], str]] = None,
     headers: Dict[str, str] = {},
     ssl_verify: bool = True,
     ocr_languages: str = "eng",
     pdf_infer_table_structure: bool = False,
+    xml_keep_tags: bool = False,
 ):
     """Partitions a document into its constituent elements. Will use libmagic to determine
     the file's type and route it to the appropriate partitioning function. Applies the default
     parameters for each partitioning function. Use the document-type specific partitioning
     functions if you need access to additional kwarg options.
 
     Parameters
@@ -73,14 +81,17 @@
         The languages to use for the Tesseract agent. To use a language, you'll first need
         to isntall the appropriate Tesseract language pack.
     pdf_infer_table_structure
         If True and strategy=hi_res, any Table Elements extracted from a PDF will include an
         additional metadata field, "text_as_html," where the value (string) is a just a
         transformation of the data into an HTML <table>.
         The "text" field for a partitioned Table Element is always present, whether True or False.
+    xml_keep_tags
+        If True, will retain the XML tags in the output. Otherwise it will simply extract
+        the text from within the tags. Only applies to partition_xml.
     """
     exactly_one(file=file, filename=filename, url=url)
 
     if url is not None:
         file, filetype = file_and_type_from_url(
             url=url,
             content_type=content_type,
@@ -116,14 +127,21 @@
     elif filetype == FileType.HTML:
         elements = partition_html(
             filename=filename,
             file=file,
             include_page_breaks=include_page_breaks,
             encoding=encoding,
         )
+    elif filetype == FileType.XML:
+        elements = partition_xml(
+            filename=filename,
+            file=file,
+            encoding=encoding,
+            xml_keep_tags=xml_keep_tags,
+        )
     elif filetype == FileType.EPUB:
         elements = partition_epub(
             filename=filename,
             file=file,
             include_page_breaks=include_page_breaks,
         )
     elif filetype == FileType.MD:
@@ -174,20 +192,29 @@
         elements = partition_pptx(
             filename=filename,
             file=file,
             include_page_breaks=include_page_breaks,
         )
     elif filetype == FileType.JSON:
         elements = partition_json(filename=filename, file=file)
+    elif filetype == FileType.XLSX:
+        elements = partition_xlsx(filename=filename, file=file)
     else:
         msg = "Invalid file" if not filename else f"Invalid file {filename}"
         raise ValueError(f"{msg}. The {filetype} file type is not supported in partition.")
 
     for element in elements:
         element.metadata.url = url
+        if content_type is not None:
+            out_filetype = STR_TO_FILETYPE.get(content_type)
+            element.metadata.filetype = (
+                FILETYPE_TO_MIMETYPE[out_filetype] if out_filetype is not None else None
+            )
+        else:
+            element.metadata.filetype = FILETYPE_TO_MIMETYPE[filetype]
 
     return elements
 
 
 def file_and_type_from_url(
     url: str,
     content_type: Optional[str] = None,
```

### Comparing `unstructured-0.6.6/unstructured/partition/common.py` & `unstructured-0.6.7/unstructured/partition/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 from unstructured.nlp.patterns import ENUMERATED_BULLETS_RE, UNICODE_BULLETS_RE
 
 
 def normalize_layout_element(layout_element) -> Union[Element, List[Element]]:
     """Converts a list of unstructured_inference DocumentLayout objects to a list of
     unstructured Elements."""
 
+    if isinstance(layout_element, Element):
+        return layout_element
+
     if isinstance(layout_element, PageBreak):
         return PageBreak()
 
     if not isinstance(layout_element, dict):
         layout_dict = layout_element.to_dict()
     else:
         layout_dict = layout_element
@@ -60,62 +63,48 @@
             list_items.append(
                 ListItem(text=text_segment.strip(), coordinates=coordinates),
             )
 
     return list_items
 
 
-def document_to_element_list(
-    document,
-    include_page_breaks: bool = False,
-) -> List[Element]:
-    """Converts a DocumentLayout object to a list of unstructured elements."""
-    elements: List[Element] = []
-    num_pages = len(document.pages)
-    for i, page in enumerate(document.pages):
-        for element in page.elements:
-            elements.append(element)
-        if include_page_breaks and i < num_pages - 1:
-            elements.append(PageBreak())
-
-    return elements
-
-
-def add_element_metadata(
+def _add_element_metadata(
     layout_elements,
     include_page_breaks: bool = False,
     filename: Optional[str] = None,
+    filetype: Optional[str] = None,
     url: Optional[str] = None,
 ) -> List[Element]:
     """Adds document metadata to the document element. Document metadata includes information
     like the filename, source url, and page number."""
     elements: List[Element] = []
     page_number: int = 1
     for layout_element in layout_elements:
         element = normalize_layout_element(layout_element)
         if hasattr(layout_element, "text_as_html"):
             text_as_html: Optional[str] = layout_element.text_as_html
         else:
             text_as_html = None
         metadata = ElementMetadata(
             filename=filename,
+            filetype=filetype,
             url=url,
             page_number=page_number,
             text_as_html=text_as_html,
         )
         if isinstance(element, list):
             for _element in element:
-                _element.metadata = metadata
+                _element.metadata = metadata.merge(_element.metadata)
             elements.extend(element)
         elif isinstance(element, PageBreak):
             page_number += 1
-            if include_page_breaks is True:
+            if include_page_breaks:
                 elements.append(element)
         else:
-            element.metadata = metadata
+            element.metadata = metadata.merge(element.metadata)
             elements.append(element)
     return elements
 
 
 def convert_office_doc(input_filename: str, output_directory: str, target_format: str):
     """Converts a .doc file to a .docx file using the libreoffice CLI."""
     # NOTE(robinson) - In the future can also include win32com client as a fallback for windows
```

### Comparing `unstructured-0.6.6/unstructured/partition/doc.py` & `unstructured-0.6.7/unstructured/partition/doc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import os
 import tempfile
 from typing import IO, List, Optional
 
 from unstructured.documents.elements import Element
+from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.common import convert_office_doc, exactly_one
 from unstructured.partition.docx import partition_docx
 
 
+@add_metadata_with_filetype(FileType.DOC)
 def partition_doc(filename: Optional[str] = None, file: Optional[IO] = None) -> List[Element]:
     """Partitions Microsoft Word Documents in .doc format into its document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
```

### Comparing `unstructured-0.6.6/unstructured/partition/docx.py` & `unstructured-0.6.7/unstructured/partition/docx.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     ElementMetadata,
     ListItem,
     NarrativeText,
     Table,
     Text,
     Title,
 )
+from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.common import exactly_one, spooled_to_bytes_io_if_needed
 from unstructured.partition.text_type import (
     is_bulleted_text,
     is_possible_narrative_text,
     is_possible_title,
     is_us_city_state_zip,
 )
@@ -91,14 +92,15 @@
     return list(_get_runs(paragraph._element, paragraph))
 
 
 # Add the runs property to the Paragraph class
 Paragraph.runs = property(lambda self: _get_paragraph_runs(self))
 
 
+@add_metadata_with_filetype(FileType.DOCX)
 def partition_docx(
     filename: Optional[str] = None,
     file: Optional[Union[IO, SpooledTemporaryFile]] = None,
     metadata_filename: Optional[str] = None,
 ) -> List[Element]:
     """Partitions Microsoft Word Documents in .docx format into its document elements.
 
@@ -131,16 +133,18 @@
     for element_item in document.element.body:
         if element_item.tag.endswith("tbl"):
             table = document.tables[table_index]
             html_table = _convert_table_to_text(table, as_html=True)
             text_table = _convert_table_to_text(table, as_html=False)
             element = Table(text_table)
             if element is not None:
-                element.metadata = ElementMetadata(filename=metadata_filename)
-                element.metadata = ElementMetadata(text_as_html=html_table)
+                element.metadata = ElementMetadata(
+                    text_as_html=html_table,
+                    filename=metadata_filename,
+                )
                 elements.append(element)
             table_index += 1
         elif element_item.tag.endswith("p"):
             paragraph = docx.text.paragraph.Paragraph(element_item, document)
             para_element: Optional[Text] = _paragraph_to_element(paragraph)
             if para_element is not None:
                 para_element.metadata = ElementMetadata(filename=metadata_filename)
```

### Comparing `unstructured-0.6.6/unstructured/partition/email.py` & `unstructured-0.6.7/unstructured/partition/email.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from unstructured.documents.email_elements import (
     MetaData,
     ReceivedInfo,
     Recipient,
     Sender,
     Subject,
 )
+from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.logger import logger
 from unstructured.nlp.patterns import EMAIL_DATETIMETZ_PATTERN_RE
 from unstructured.partition.html import partition_html
 from unstructured.partition.text import partition_text, split_by_paragraph
 
 VALID_CONTENT_SOURCES: Final[List[str]] = ["text/html", "text/plain"]
 
@@ -176,14 +177,15 @@
     image_raw_info = element.text[start:end]
     image_info = clean_extra_whitespace(image_raw_info.split(":")[1])
     element.text = element.text.replace("[image: " + image_info[:-1] + "]", "")
 
     return Image(text=image_info[:-1]), element
 
 
+@add_metadata_with_filetype(FileType.EML)
 def partition_email(
     filename: Optional[str] = None,
     file: Optional[IO] = None,
     text: Optional[str] = None,
     content_source: str = "text/html",
     encoding: Optional[str] = None,
     include_headers: bool = False,
```

### Comparing `unstructured-0.6.6/unstructured/partition/epub.py` & `unstructured-0.6.7/unstructured/partition/rtf.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from typing import IO, List, Optional
 
 from unstructured.documents.elements import Element
+from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.html import convert_and_partition_html
 
 
-def partition_epub(
+@add_metadata_with_filetype(FileType.RTF)
+def partition_rtf(
     filename: Optional[str] = None,
     file: Optional[IO] = None,
     include_page_breaks: bool = False,
 ) -> List[Element]:
-    """Partitions an EPUB document. The document is first converted to HTML and then
-    partitoned using partiton_html.
+    """Partitions an RTF document. The document is first converted to HTML and then
+    partitioned using partiton_html.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     include_page_breaks
         If True, the output will include page breaks if the filetype supports it
     """
     return convert_and_partition_html(
-        source_format="epub",
+        source_format="rtf",
         filename=filename,
         file=file,
         include_page_breaks=include_page_breaks,
     )
```

### Comparing `unstructured-0.6.6/unstructured/partition/html.py` & `unstructured-0.6.7/unstructured/partition/html.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,25 @@
 
 import requests
 
 from unstructured.documents.elements import Element
 from unstructured.documents.html import HTMLDocument
 from unstructured.documents.xml import VALID_PARSERS
 from unstructured.file_utils.file_conversion import convert_file_to_html_text
-from unstructured.partition.common import (
-    add_element_metadata,
+from unstructured.file_utils.filetype import (
+    FileType,
+    add_metadata_with_filetype,
     document_to_element_list,
+)
+from unstructured.partition.common import (
     exactly_one,
 )
 
 
+@add_metadata_with_filetype(FileType.HTML)
 def partition_html(
     filename: Optional[str] = None,
     file: Optional[IO] = None,
     text: Optional[str] = None,
     url: Optional[str] = None,
     encoding: Optional[str] = None,
     include_page_breaks: bool = False,
@@ -84,24 +88,15 @@
 
         content_type = response.headers.get("Content-Type", "")
         if not content_type.startswith("text/html"):
             raise ValueError(f"Expected content type text/html. Got {content_type}.")
 
         document = HTMLDocument.from_string(response.text, parser=parser)
 
-    layout_elements = document_to_element_list(document, include_page_breaks=include_page_breaks)
-    if include_metadata:
-        return add_element_metadata(
-            layout_elements,
-            include_page_breaks=include_page_breaks,
-            filename=filename,
-            url=url,
-        )
-    else:
-        return layout_elements
+    return document_to_element_list(document, include_page_breaks=include_page_breaks)
 
 
 def convert_and_partition_html(
     source_format: str,
     filename: Optional[str] = None,
     file: Optional[IO] = None,
     include_page_breaks: bool = False,
```

### Comparing `unstructured-0.6.6/unstructured/partition/image.py` & `unstructured-0.6.7/unstructured/partition/image.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/partition/json.py` & `unstructured-0.6.7/unstructured/partition/json.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import json
 import re
 from typing import IO, List, Optional
 
 from unstructured.documents.elements import Element
+from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.nlp.patterns import LIST_OF_DICTS_PATTERN
 from unstructured.partition.common import exactly_one
 from unstructured.staging.base import dict_to_elements
 
 
+@add_metadata_with_filetype(FileType.JSON)
 def partition_json(
     filename: Optional[str] = None,
     file: Optional[IO] = None,
     text: Optional[str] = None,
 ) -> List[Element]:
     """Partitions an .json document into its constituent elements."""
     if text is not None and text.strip() == "" and not file and not filename:
```

### Comparing `unstructured-0.6.6/unstructured/partition/md.py` & `unstructured-0.6.7/unstructured/partition/md.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from typing import IO, List, Optional, Union
 
 import markdown
 import requests
 
 from unstructured.documents.elements import Element
 from unstructured.documents.xml import VALID_PARSERS
+from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.common import exactly_one
 from unstructured.partition.html import partition_html
 
 
 def optional_decode(contents: Union[str, bytes]) -> str:
     if isinstance(contents, bytes):
         return contents.decode("utf-8")
     return contents
 
 
+@add_metadata_with_filetype(FileType.MD)
 def partition_md(
     filename: Optional[str] = None,
     file: Optional[IO] = None,
     text: Optional[str] = None,
     url: Optional[str] = None,
     include_page_breaks: bool = False,
     include_metadata: bool = True,
```

### Comparing `unstructured-0.6.6/unstructured/partition/msg.py` & `unstructured-0.6.7/unstructured/partition/msg.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import tempfile
 from typing import IO, Dict, List, Optional
 
 import msg_parser
 
 from unstructured.documents.elements import Element, ElementMetadata
+from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.common import exactly_one
 from unstructured.partition.email import convert_to_iso_8601
 from unstructured.partition.html import partition_html
 from unstructured.partition.text import partition_text
 
 
+@add_metadata_with_filetype(FileType.MSG)
 def partition_msg(
     filename: Optional[str] = None,
     file: Optional[IO] = None,
 ) -> List[Element]:
     """Partitions a MSFT Outlook .msg file
 
     Parameters
```

### Comparing `unstructured-0.6.6/unstructured/partition/odt.py` & `unstructured-0.6.7/unstructured/partition/odt.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import IO, List, Optional
 
 from unstructured.documents.elements import Element
+from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.docx import convert_and_partition_docx
 
 
+@add_metadata_with_filetype(FileType.ODT)
 def partition_odt(filename: Optional[str] = None, file: Optional[IO] = None) -> List[Element]:
     """Partitions Open Office Documents in .odt format into its document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
```

### Comparing `unstructured-0.6.6/unstructured/partition/pdf.py` & `unstructured-0.6.7/unstructured/partition/pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 import re
 import warnings
 from tempfile import SpooledTemporaryFile
 from typing import BinaryIO, List, Optional, Union, cast
 
 import pdf2image
-import pytesseract
 from pdfminer.high_level import extract_pages
 from pdfminer.utils import open_filename
 from PIL import Image
 
 from unstructured.cleaners.core import clean_extra_whitespace
 from unstructured.documents.elements import Element, ElementMetadata, PageBreak
+from unstructured.file_utils.filetype import (
+    FileType,
+    add_metadata_with_filetype,
+    document_to_element_list,
+)
 from unstructured.nlp.patterns import PARAGRAPH_PATTERN
 from unstructured.partition import _partition_via_api
 from unstructured.partition.common import (
-    add_element_metadata,
-    document_to_element_list,
     exactly_one,
     spooled_to_bytes_io_if_needed,
 )
 from unstructured.partition.strategies import determine_pdf_or_image_strategy
 from unstructured.partition.text import partition_text
 from unstructured.utils import requires_dependencies
 
 
+@add_metadata_with_filetype(FileType.PDF)
 def partition_pdf(
     filename: str = "",
     file: Optional[Union[BinaryIO, SpooledTemporaryFile]] = None,
     url: Optional[str] = None,
     template: str = "layout/pdf",
     token: Optional[str] = None,
     include_page_breaks: bool = False,
@@ -165,21 +168,18 @@
             file=cast(BinaryIO, file),
             url=url,
             token=token,
             data=data,
             include_page_breaks=True,
         )
 
-    return add_element_metadata(
-        layout_elements,
-        include_page_breaks=include_page_breaks,
-        filename=filename,
-    )
+    return layout_elements
 
 
+@requires_dependencies("unstructured_inference")
 def _partition_pdf_or_image_local(
     filename: str = "",
     file: Optional[Union[bytes, BinaryIO]] = None,
     template: Optional[str] = None,
     is_image: bool = False,
     infer_table_structure: bool = False,
     include_page_breaks: bool = False,
@@ -297,23 +297,26 @@
 
         if include_page_breaks:
             elements.append(PageBreak())
 
     return elements
 
 
+@requires_dependencies("pytesseract")
 def _partition_pdf_or_image_with_ocr(
     filename: str = "",
     file: Optional[Union[bytes, BinaryIO, SpooledTemporaryFile]] = None,
     include_page_breaks: bool = False,
     ocr_languages: str = "eng",
     is_image: bool = False,
 ):
     """Partitions and image or PDF using Tesseract OCR. For PDFs, each page is converted
     to an image prior to processing."""
+    import pytesseract
+
     if is_image:
         if file is not None:
             image = Image.open(file)
             text = pytesseract.image_to_string(image, config=f"-l '{ocr_languages}'")
         else:
             text = pytesseract.image_to_string(filename, config=f"-l '{ocr_languages}'")
         elements = partition_text(text=text)
```

### Comparing `unstructured-0.6.6/unstructured/partition/ppt.py` & `unstructured-0.6.7/unstructured/partition/ppt.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import os
 import tempfile
 from typing import IO, List, Optional
 
 from unstructured.documents.elements import Element
+from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.common import convert_office_doc, exactly_one
 from unstructured.partition.pptx import partition_pptx
 
 
+@add_metadata_with_filetype(FileType.PPT)
 def partition_ppt(
     filename: Optional[str] = None,
     file: Optional[IO] = None,
     include_page_breaks: bool = False,
 ) -> List[Element]:
     """Partitions Microsoft PowerPoint Documents in .ppt format into their document elements.
```

### Comparing `unstructured-0.6.6/unstructured/partition/pptx.py` & `unstructured-0.6.7/unstructured/partition/pptx.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,23 +8,25 @@
     ElementMetadata,
     ListItem,
     NarrativeText,
     PageBreak,
     Text,
     Title,
 )
+from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.common import exactly_one, spooled_to_bytes_io_if_needed
 from unstructured.partition.text_type import (
     is_possible_narrative_text,
     is_possible_title,
 )
 
 OPENXML_SCHEMA_NAME = "{http://schemas.openxmlformats.org/drawingml/2006/main}"
 
 
+@add_metadata_with_filetype(FileType.PPTX)
 def partition_pptx(
     filename: Optional[str] = None,
     file: Optional[Union[IO, SpooledTemporaryFile]] = None,
     include_page_breaks: bool = True,
     metadata_filename: Optional[str] = None,
 ) -> List[Element]:
     """Partitions Microsoft PowerPoint Documents in .pptx format into its document elements.
```

### Comparing `unstructured-0.6.6/unstructured/partition/strategies.py` & `unstructured-0.6.7/unstructured/partition/strategies.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/partition/text.py` & `unstructured-0.6.7/unstructured/partition/text.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,34 +7,38 @@
     Element,
     ElementMetadata,
     ListItem,
     NarrativeText,
     Text,
     Title,
 )
+from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.nlp.patterns import PARAGRAPH_PATTERN
 from unstructured.partition.common import exactly_one
 from unstructured.partition.text_type import (
     is_bulleted_text,
     is_possible_narrative_text,
     is_possible_title,
     is_us_city_state_zip,
 )
 
 
 def split_by_paragraph(content: str) -> List[str]:
     return re.split(PARAGRAPH_PATTERN, content)
 
 
+@add_metadata_with_filetype(FileType.TXT)
 def partition_text(
     filename: Optional[str] = None,
     file: Optional[IO] = None,
     text: Optional[str] = None,
     encoding: Optional[str] = "utf-8",
     paragraph_grouper: Optional[Callable[[str], str]] = None,
+    metadata_filename: Optional[str] = None,
+    include_metadata: bool = True,
 ) -> List[Element]:
     """Partitions an .txt documents into its constituent elements.
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
@@ -42,14 +46,16 @@
     text
         The string representation of the .txt document.
     encoding
         The encoding method used to decode the text input. If None, utf-8 will be used.
     paragrapher_grouper
         A str -> str function for fixing paragraphs that are interrupted by line breaks
         for formatting purposes.
+    include_metadata
+        Determines whether or not metadata is included in the output.
     """
     if text is not None and text.strip() == "" and not file and not filename:
         return []
 
     # Verify that only one of the arguments was provided
     exactly_one(filename=filename, file=file, text=text)
 
@@ -71,16 +77,20 @@
     if paragraph_grouper is not None:
         file_text = paragraph_grouper(file_text)
     else:
         file_text = group_broken_paragraphs(file_text)
 
     file_content = split_by_paragraph(file_text)
 
+    metadata_filename = metadata_filename or filename
+
     elements: List[Element] = []
-    metadata = ElementMetadata(filename=filename)
+    metadata = (
+        ElementMetadata(filename=metadata_filename) if include_metadata else ElementMetadata()
+    )
     for ctext in file_content:
         ctext = ctext.strip()
 
         if ctext == "":
             continue
         if is_bulleted_text(ctext):
             elements.append(ListItem(text=clean_bullets(ctext), metadata=metadata))
```

### Comparing `unstructured-0.6.6/unstructured/partition/text_type.py` & `unstructured-0.6.7/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/staging/argilla.py` & `unstructured-0.6.7/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/staging/base.py` & `unstructured-0.6.7/unstructured/staging/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/staging/baseplate.py` & `unstructured-0.6.7/unstructured/staging/baseplate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/staging/datasaur.py` & `unstructured-0.6.7/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/staging/huggingface.py` & `unstructured-0.6.7/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/staging/label_box.py` & `unstructured-0.6.7/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/staging/label_studio.py` & `unstructured-0.6.7/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/staging/prodigy.py` & `unstructured-0.6.7/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured/utils.py` & `unstructured-0.6.7/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.6/unstructured.egg-info/PKG-INFO` & `unstructured-0.6.7/unstructured.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.6.6
+Version: 0.6.7
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -186,31 +186,32 @@
         you can also uninstall the hooks with `pre-commit uninstall`.
         
         ## :clap: Quick Tour
         
         You can run this [Colab notebook](https://colab.research.google.com/drive/1U8VCjY2-x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below.
         
         The following examples show how to get started with the `unstructured` library.
-        You can parse **TXT**, **HTML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**,
-        **ODT**, **PPT**, **PPTX**, **JPG**,
+        
+        You can parse **TXT**, **HTML**, **XML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**,
+        **XLSX**, **ODT**, **PPT**, **PPTX**, **JPG**,
         and **PNG** documents with one line of code!
         <br></br>
         See our [documentation page](https://unstructured-io.github.io/unstructured) for a full description
         of the features in the library.
         
         ### Document Parsing
         
         The easiest way to parse a document in unstructured is to use the `partition` brick. If you
         use `partition` brick, `unstructured` will detect the file type and route it to the appropriate
         file-specific partitioning brick.
         If you are using the `partition` brick, you may need to install additional parameters via `pip install unstructured[local-inference]`. Ensure you first install `libmagic` using the
         instructions outlined [here](https://unstructured-io.github.io/unstructured/installing.html#filetype-detection)
         `partition` will always apply the default arguments. If you need
         advanced features, use a document-specific brick. The `partition` brick currently works for
-        `.txt`, `.doc`, `.docx`, `.ppt`, `.pptx`, `.jpg`, `.png`, `.eml`, `.msg`, `.html`, and `.pdf` documents.
+        `.txt`, `.doc`, `.docx`, `.ppt`, `.pptx`, `.xlsx`, `.jpg`, `.png`, `.eml`, `.msg`, `.html`, and `.pdf` documents.
         
         ```python
         from unstructured.partition.auto import partition
         
         elements = partition("example-docs/layout-parser-paper.pdf")
         ```
         
@@ -406,13 +407,14 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: huggingface
 Provides-Extra: local-inference
 Provides-Extra: s3
 Provides-Extra: azure
+Provides-Extra: discord
 Provides-Extra: github
 Provides-Extra: gitlab
 Provides-Extra: reddit
 Provides-Extra: slack
 Provides-Extra: wikipedia
 Provides-Extra: google-drive
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.6.6 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.6.7 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -111,42 +111,42 @@
 `pre-commit`, you'll just need to install the hooks with `pre-commit install`
 since the `pre-commit` package is installed as part of `make install` mentioned
 above. Finally, if you decided to use `pre-commit` you can also uninstall the
 hooks with `pre-commit uninstall`. ## :clap: Quick Tour You can run this [Colab
 notebook](https://colab.research.google.com/drive/1U8VCjY2-
 x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below. The following examples
 show how to get started with the `unstructured` library. You can parse **TXT**,
-**HTML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**,
-**ODT**, **PPT**, **PPTX**, **JPG**, and **PNG** documents with one line of
-code!
+**HTML**, **XML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**,
+**DOCX**, **XLSX**, **ODT**, **PPT**, **PPTX**, **JPG**, and **PNG** documents
+with one line of code!
 See our [documentation page](https://unstructured-io.github.io/unstructured)
 for a full description of the features in the library. ### Document Parsing The
 easiest way to parse a document in unstructured is to use the `partition`
 brick. If you use `partition` brick, `unstructured` will detect the file type
 and route it to the appropriate file-specific partitioning brick. If you are
 using the `partition` brick, you may need to install additional parameters via
 `pip install unstructured[local-inference]`. Ensure you first install
 `libmagic` using the instructions outlined [here](https://unstructured-
 io.github.io/unstructured/installing.html#filetype-detection) `partition` will
 always apply the default arguments. If you need advanced features, use a
 document-specific brick. The `partition` brick currently works for `.txt`,
-`.doc`, `.docx`, `.ppt`, `.pptx`, `.jpg`, `.png`, `.eml`, `.msg`, `.html`, and
-`.pdf` documents. ```python from unstructured.partition.auto import partition
-elements = partition("example-docs/layout-parser-paper.pdf") ``` Run `print
-("\n\n".join([str(el) for el in elements]))` to get a string representation of
-the output, which looks like: ``` LayoutParser : A Uniï¬ed Toolkit for Deep
-Learning Based Document Image Analysis Zejiang Shen 1 ( (cid:0) ), Ruochen
-Zhang 2 , Melissa Dell 3 , Benjamin Charles Germain Lee 4 , Jacob Carlson 3 ,
-and Weining Li 5 Abstract. Recent advances in document image analysis (DIA)
-have been primarily driven by the application of neural networks. Ideally,
-research outcomes could be easily deployed in production and extended for
-further investigation. However, various factors like loosely organized
-codebases and sophisticated model conï¬gurations complicate the easy reuse of
-im- portant innovations by a wide audience. Though there have been on-going
-eï¬orts to improve reusability and simplify deep learning (DL) model
+`.doc`, `.docx`, `.ppt`, `.pptx`, `.xlsx`, `.jpg`, `.png`, `.eml`, `.msg`,
+`.html`, and `.pdf` documents. ```python from unstructured.partition.auto
+import partition elements = partition("example-docs/layout-parser-paper.pdf")
+``` Run `print("\n\n".join([str(el) for el in elements]))` to get a string
+representation of the output, which looks like: ``` LayoutParser : A Uniï¬ed
+Toolkit for Deep Learning Based Document Image Analysis Zejiang Shen 1 ( (cid:
+0) ), Ruochen Zhang 2 , Melissa Dell 3 , Benjamin Charles Germain Lee 4 , Jacob
+Carlson 3 , and Weining Li 5 Abstract. Recent advances in document image
+analysis (DIA) have been primarily driven by the application of neural
+networks. Ideally, research outcomes could be easily deployed in production and
+extended for further investigation. However, various factors like loosely
+organized codebases and sophisticated model conï¬gurations complicate the easy
+reuse of im- portant innovations by a wide audience. Though there have been on-
+going eï¬orts to improve reusability and simplify deep learning (DL) model
 development in disciplines like natural language processing and computer
 vision, none of them are optimized for challenges in the domain of DIA. This
 represents a major gap in the existing toolkit, as DIA is central to academic
 research across a wide range of disciplines in the social sciences and
 humanities. This paper introduces LayoutParser , an open-source library for
 streamlining the usage of DL in DIA research and applica- tions. The core
 LayoutParser library comes with a set of simple and intuitive interfaces for
@@ -221,10 +221,10 @@
 Audience :: Education Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.7.0 Description-Content-Type:
 text/markdown Provides-Extra: huggingface Provides-Extra: local-inference
-Provides-Extra: s3 Provides-Extra: azure Provides-Extra: github Provides-Extra:
-gitlab Provides-Extra: reddit Provides-Extra: slack Provides-Extra: wikipedia
-Provides-Extra: google-drive
+Provides-Extra: s3 Provides-Extra: azure Provides-Extra: discord Provides-
+Extra: github Provides-Extra: gitlab Provides-Extra: reddit Provides-Extra:
+slack Provides-Extra: wikipedia Provides-Extra: google-drive
```

### Comparing `unstructured-0.6.6/unstructured.egg-info/SOURCES.txt` & `unstructured-0.6.7/unstructured.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 unstructured/ingest/__init__.py
 unstructured/ingest/interfaces.py
 unstructured/ingest/logger.py
 unstructured/ingest/main.py
 unstructured/ingest/connector/__init__.py
 unstructured/ingest/connector/azure.py
 unstructured/ingest/connector/biomed.py
+unstructured/ingest/connector/discord.py
 unstructured/ingest/connector/fsspec.py
 unstructured/ingest/connector/git.py
 unstructured/ingest/connector/github.py
 unstructured/ingest/connector/gitlab.py
 unstructured/ingest/connector/google_drive.py
 unstructured/ingest/connector/local.py
 unstructured/ingest/connector/reddit.py
@@ -77,14 +78,16 @@
 unstructured/partition/pdf.py
 unstructured/partition/ppt.py
 unstructured/partition/pptx.py
 unstructured/partition/rtf.py
 unstructured/partition/strategies.py
 unstructured/partition/text.py
 unstructured/partition/text_type.py
+unstructured/partition/xlsx.py
+unstructured/partition/xml.py
 unstructured/staging/__init__.py
 unstructured/staging/argilla.py
 unstructured/staging/base.py
 unstructured/staging/baseplate.py
 unstructured/staging/datasaur.py
 unstructured/staging/huggingface.py
 unstructured/staging/label_box.py
```

