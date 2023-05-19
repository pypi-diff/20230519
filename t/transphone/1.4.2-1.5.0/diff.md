# Comparing `tmp/transphone-1.4.2.tar.gz` & `tmp/transphone-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/transphone-1.4.2.tar", last modified: Mon May 15 13:58:58 2023, max compression
+gzip compressed data, was "dist/transphone-1.5.0.tar", last modified: Fri May 19 07:10:16 2023, max compression
```

## Comparing `transphone-1.4.2.tar` & `transphone-1.5.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 13:58:58.000000 transphone-1.4.2/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1072 2022-10-27 20:49:08.000000 transphone-1.4.2/LICENSE
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      260 2023-05-15 13:58:58.000000 transphone-1.4.2/PKG-INFO
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     8168 2023-05-15 07:50:03.000000 transphone-1.4.2/README.md
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       38 2023-05-15 13:58:58.000000 transphone-1.4.2/setup.cfg
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      387 2023-05-15 13:58:49.000000 transphone-1.4.2/setup.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 13:58:58.000000 transphone-1.4.2/test/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2730 2023-05-08 16:31:27.000000 transphone-1.4.2/test/test_tokenizer.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 13:58:58.000000 transphone-1.4.2/transphone/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       47 2022-11-23 17:53:06.000000 transphone-1.4.2/transphone/__init__.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 13:58:58.000000 transphone-1.4.2/transphone/bin/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:22.000000 transphone-1.4.2/transphone/bin/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1545 2023-05-08 16:31:27.000000 transphone-1.4.2/transphone/bin/download_model.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3451 2023-05-08 16:31:27.000000 transphone-1.4.2/transphone/bin/eval_epitran.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3551 2023-05-08 16:31:27.000000 transphone-1.4.2/transphone/bin/eval_g2p.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3634 2023-05-08 16:31:27.000000 transphone-1.4.2/transphone/bin/eval_zsl_g2p.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2844 2023-05-08 16:31:27.000000 transphone-1.4.2/transphone/bin/g2p.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2679 2023-05-08 16:31:27.000000 transphone-1.4.2/transphone/bin/tokenize.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3816 2023-05-08 16:31:27.000000 transphone-1.4.2/transphone/bin/train_g2p.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1618 2023-05-08 16:31:27.000000 transphone-1.4.2/transphone/bin/update_model.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      325 2023-05-08 16:31:27.000000 transphone-1.4.2/transphone/config.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 13:58:58.000000 transphone-1.4.2/transphone/data/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:30.000000 transphone-1.4.2/transphone/data/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9356 2023-05-15 07:50:03.000000 transphone-1.4.2/transphone/g2p.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 13:58:58.000000 transphone-1.4.2/transphone/lang/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.4.2/transphone/lang/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1359 2023-05-08 16:31:27.000000 transphone-1.4.2/transphone/lang/base_tokenizer.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 13:58:58.000000 transphone-1.4.2/transphone/lang/cmn/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.4.2/transphone/lang/cmn/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    55821 2022-11-24 02:03:19.000000 transphone-1.4.2/transphone/lang/cmn/normalizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1750 2023-05-15 07:50:03.000000 transphone-1.4.2/transphone/lang/cmn/tokenizer.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 13:58:58.000000 transphone-1.4.2/transphone/lang/eng/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.4.2/transphone/lang/eng/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3341 2023-05-08 16:31:27.000000 transphone-1.4.2/transphone/lang/eng/normalizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2243 2023-05-15 07:50:03.000000 transphone-1.4.2/transphone/lang/eng/tokenizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9371 2023-05-15 13:58:49.000000 transphone-1.4.2/transphone/lang/epitran_tokenizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1822 2023-05-15 07:50:03.000000 transphone-1.4.2/transphone/lang/g2p_tokenizer.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 13:58:58.000000 transphone-1.4.2/transphone/lang/jpn/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.4.2/transphone/lang/jpn/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9740 2022-11-25 20:08:08.000000 transphone-1.4.2/transphone/lang/jpn/conv_table.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    15327 2022-11-25 20:04:35.000000 transphone-1.4.2/transphone/lang/jpn/jaconv.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9520 2023-05-08 16:31:27.000000 transphone-1.4.2/transphone/lang/jpn/kana2phoneme.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     5192 2023-05-08 16:31:27.000000 transphone-1.4.2/transphone/lang/jpn/normalizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2775 2023-05-15 07:50:03.000000 transphone-1.4.2/transphone/lang/jpn/tokenizer.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 13:58:58.000000 transphone-1.4.2/transphone/model/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:35.000000 transphone-1.4.2/transphone/model/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    13693 2023-05-08 16:31:27.000000 transphone-1.4.2/transphone/model/checkpoint_utils.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     6628 2023-05-08 16:31:27.000000 transphone-1.4.2/transphone/model/dataset.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     5388 2022-03-13 19:18:49.000000 transphone-1.4.2/transphone/model/ensemble.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1782 2023-05-08 16:31:27.000000 transphone-1.4.2/transphone/model/grapheme.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      409 2023-05-08 16:31:27.000000 transphone-1.4.2/transphone/model/loader.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     8331 2023-05-08 16:31:27.000000 transphone-1.4.2/transphone/model/lstm.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     7420 2023-05-08 16:31:27.000000 transphone-1.4.2/transphone/model/transformer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1722 2023-05-08 16:31:27.000000 transphone-1.4.2/transphone/model/utils.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1046 2023-05-08 16:31:27.000000 transphone-1.4.2/transphone/model/vocab.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 13:58:58.000000 transphone-1.4.2/transphone/pretrained/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 18:28:14.000000 transphone-1.4.2/transphone/pretrained/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2536 2023-05-08 16:31:27.000000 transphone-1.4.2/transphone/run.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1350 2023-05-15 07:50:03.000000 transphone-1.4.2/transphone/tokenizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      491 2023-05-08 16:31:27.000000 transphone-1.4.2/transphone/utils.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-15 13:58:58.000000 transphone-1.4.2/transphone.egg-info/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      260 2023-05-15 13:58:57.000000 transphone-1.4.2/transphone.egg-info/PKG-INFO
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1478 2023-05-15 13:58:57.000000 transphone-1.4.2/transphone.egg-info/SOURCES.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        1 2023-05-15 13:58:57.000000 transphone-1.4.2/transphone.egg-info/dependency_links.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      111 2023-05-15 13:58:57.000000 transphone-1.4.2/transphone.egg-info/requires.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       11 2023-05-15 13:58:57.000000 transphone-1.4.2/transphone.egg-info/top_level.txt
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-19 07:10:15.000000 transphone-1.5.0/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1072 2022-10-27 20:49:08.000000 transphone-1.5.0/LICENSE
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      260 2023-05-19 07:10:15.000000 transphone-1.5.0/PKG-INFO
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     8168 2023-05-15 07:50:03.000000 transphone-1.5.0/README.md
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       38 2023-05-19 07:10:15.000000 transphone-1.5.0/setup.cfg
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      387 2023-05-19 07:10:11.000000 transphone-1.5.0/setup.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-19 07:10:15.000000 transphone-1.5.0/test/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2730 2023-05-08 16:31:27.000000 transphone-1.5.0/test/test_tokenizer.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       47 2022-11-23 17:53:06.000000 transphone-1.5.0/transphone/__init__.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone/bin/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:22.000000 transphone-1.5.0/transphone/bin/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1545 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/bin/download_model.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3451 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/bin/eval_epitran.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3551 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/bin/eval_g2p.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3634 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/bin/eval_zsl_g2p.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2844 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/bin/g2p.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2679 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/bin/tokenize.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3816 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/bin/train_g2p.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1618 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/bin/update_model.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      325 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/config.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone/data/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:30.000000 transphone-1.5.0/transphone/data/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9371 2023-05-19 07:10:11.000000 transphone-1.5.0/transphone/g2p.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone/lang/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.5.0/transphone/lang/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2128 2023-05-19 07:10:11.000000 transphone-1.5.0/transphone/lang/base_tokenizer.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone/lang/cmn/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.5.0/transphone/lang/cmn/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    55821 2022-11-24 02:03:19.000000 transphone-1.5.0/transphone/lang/cmn/normalizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1750 2023-05-15 07:50:03.000000 transphone-1.5.0/transphone/lang/cmn/tokenizer.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone/lang/eng/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.5.0/transphone/lang/eng/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3341 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/lang/eng/normalizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2284 2023-05-19 07:10:11.000000 transphone-1.5.0/transphone/lang/eng/tokenizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9371 2023-05-15 13:58:49.000000 transphone-1.5.0/transphone/lang/epitran_tokenizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1826 2023-05-19 07:10:11.000000 transphone-1.5.0/transphone/lang/g2p_tokenizer.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone/lang/jpn/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.5.0/transphone/lang/jpn/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9740 2022-11-25 20:08:08.000000 transphone-1.5.0/transphone/lang/jpn/conv_table.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    15327 2022-11-25 20:04:35.000000 transphone-1.5.0/transphone/lang/jpn/jaconv.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9520 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/lang/jpn/kana2phoneme.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     5192 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/lang/jpn/normalizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2775 2023-05-15 07:50:03.000000 transphone-1.5.0/transphone/lang/jpn/tokenizer.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone/model/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:35.000000 transphone-1.5.0/transphone/model/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    13693 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/model/checkpoint_utils.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     6628 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/model/dataset.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     5388 2022-03-13 19:18:49.000000 transphone-1.5.0/transphone/model/ensemble.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1782 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/model/grapheme.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      409 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/model/loader.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     8331 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/model/lstm.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     7420 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/model/transformer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1722 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/model/utils.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1046 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/model/vocab.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone/pretrained/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 18:28:14.000000 transphone-1.5.0/transphone/pretrained/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2536 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/run.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1350 2023-05-15 07:50:03.000000 transphone-1.5.0/transphone/tokenizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      491 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/utils.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone.egg-info/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      260 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone.egg-info/PKG-INFO
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1478 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone.egg-info/SOURCES.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        1 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone.egg-info/dependency_links.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      111 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone.egg-info/requires.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       11 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone.egg-info/top_level.txt
```

### Comparing `transphone-1.4.2/LICENSE` & `transphone-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/README.md` & `transphone-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/test/test_tokenizer.py` & `transphone-1.5.0/test/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/bin/download_model.py` & `transphone-1.5.0/transphone/bin/download_model.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/bin/eval_epitran.py` & `transphone-1.5.0/transphone/bin/eval_epitran.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/bin/eval_g2p.py` & `transphone-1.5.0/transphone/bin/eval_g2p.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/bin/eval_zsl_g2p.py` & `transphone-1.5.0/transphone/bin/eval_zsl_g2p.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/bin/g2p.py` & `transphone-1.5.0/transphone/bin/g2p.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/bin/tokenize.py` & `transphone-1.5.0/transphone/bin/tokenize.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/bin/train_g2p.py` & `transphone-1.5.0/transphone/bin/train_g2p.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/bin/update_model.py` & `transphone-1.5.0/transphone/bin/update_model.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/g2p.py` & `transphone-1.5.0/transphone/g2p.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,18 +37,18 @@
             raise ValueError(f"could not download or read {model_name} model")
 
         if (model_path / "model.pt").exists():
             checkpoint = model_path / "model.pt"
         else:
             checkpoint = find_topk_models(model_path)[0]
 
-        if (model_path / 'cache').exists():
-            cache_path = model_path / 'cache'
-        else:
-            cache_path = None
+        cache_path = model_path / 'cache'
+
+        if not (model_path / 'cache').exists():
+            cache_path.mkdir(parents=True, exist_ok=True)
 
     config = read_model_config(model_name)
 
     model = G2P(checkpoint, cache_path, config)
 
     return model
```

### Comparing `transphone-1.4.2/transphone/lang/base_tokenizer.py` & `transphone-1.5.0/transphone/lang/base_tokenizer.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,26 +9,48 @@
         self.inventory = read_inventory(lang_id)
 
         if g2p_model is None:
             self.g2p = None
         else:
             self.g2p = read_g2p(g2p_model, device)
 
+        # cache for g2p
         self.cache = {}
 
+        # this will temporarily store new caches, which will be flashed to disk
+        self.cache_log = {}
+
         if self.g2p is not None and self.g2p.cache_path is not None:
             lang_cache_path = self.g2p.cache_path / f"{lang_id}.txt"
             if lang_cache_path.exists():
                 for line in open(lang_cache_path, 'r'):
                     fields = line.strip().split()
                     self.cache[fields[0]] = fields[1:]
 
         self.punctuation = '!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~'
         self.logger = TransphoneConfig.logger
 
+    def add_cache(self, word, phonemes):
+
+        self.cache[word] = phonemes
+
+        if self.g2p is None or self.g2p.cache_path is None:
+            return
+
+        # handle new cache
+        self.cache_log[word] = phonemes
+
+        # flash them to disk if the cache is large enough
+        if len(self.cache_log) >= 100 and self.g2p.cache_path is not None and self.g2p.cache_path.exists():
+            w = open(self.g2p.cache_path / f"{self.lang_id}.txt", 'a')
+            for word, phonemes in self.cache_log.items():
+                w.write(f"{word}\t{' '.join(phonemes)}\n")
+            w.close()
+            self.cache_log = {}
+
     def tokenize(self, text: str):
         raise NotImplementedError
 
     def tokenize_words(self, text:str):
         text = text.translate(str.maketrans('', '', self.punctuation)).lower()
 
         return text.split()
```

### Comparing `transphone-1.4.2/transphone/lang/cmn/normalizer.py` & `transphone-1.5.0/transphone/lang/cmn/normalizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/lang/cmn/tokenizer.py` & `transphone-1.5.0/transphone/lang/cmn/tokenizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/lang/eng/normalizer.py` & `transphone-1.5.0/transphone/lang/eng/normalizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/lang/eng/tokenizer.py` & `transphone-1.5.0/transphone/lang/eng/tokenizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,20 +46,21 @@
                     self.logger.info(f"CMUdict: {word} -> {arpa} -> {ipas}")
                     if verbose:
                         print(log)
 
                     self.cache[word] = ipas
 
                 elif use_g2p:
-                    phonemes = self.g2p.inference(word)
+                    phonemes = self.g2p.inference_batch(word, self.lang_id, verbose=verbose)
                     remapped_phonemes = self.inventory.remap(phonemes)
 
                     log = f"g2p {word} ->  {remapped_phonemes}"
                     self.logger.info(log)
                     if verbose:
                         print(log)
-                    self.cache[word] = remapped_phonemes
+
+                    self.add_cache(word, remapped_phonemes)
                     ipa_lst.extend(remapped_phonemes)
                 if use_space:
                     ipa_lst.append('<SPACE>')
 
         return ipa_lst
```

### Comparing `transphone-1.4.2/transphone/lang/epitran_tokenizer.py` & `transphone-1.5.0/transphone/lang/epitran_tokenizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/lang/g2p_tokenizer.py` & `transphone-1.5.0/transphone/lang/g2p_tokenizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
     def __init__(self, lang_id, g2p_model='latest', device=None):
         super().__init__(lang_id, g2p_model, device)
 
         self.lexicon = read_lexicon(lang_id)
 
 
+
     def tokenize(self, text, use_g2p=True, use_space=False, verbose=False):
 
         norm_text = text.translate(str.maketrans('', '', self.punctuation)).lower()
         log = f"normalization: {text} -> {norm_text}"
         self.logger.info(log)
 
         if verbose:
@@ -43,13 +44,13 @@
                 phonemes = self.g2p.inference_batch(word, self.lang_id, verbose=verbose)
                 remapped_phonemes = self.inventory.remap(phonemes)
 
                 log = f"g2p batch mode: {word} ->  {remapped_phonemes}"
                 self.logger.info(log)
                 if verbose:
                     print(log)
-                self.cache[word] = remapped_phonemes
+                self.add_cache(word, remapped_phonemes)
                 result.extend(remapped_phonemes)
             if use_space:
                 result.append('<SPACE>')
 
         return result
```

### Comparing `transphone-1.4.2/transphone/lang/jpn/conv_table.py` & `transphone-1.5.0/transphone/lang/jpn/conv_table.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/lang/jpn/jaconv.py` & `transphone-1.5.0/transphone/lang/jpn/jaconv.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/lang/jpn/kana2phoneme.py` & `transphone-1.5.0/transphone/lang/jpn/kana2phoneme.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/lang/jpn/normalizer.py` & `transphone-1.5.0/transphone/lang/jpn/normalizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/lang/jpn/tokenizer.py` & `transphone-1.5.0/transphone/lang/jpn/tokenizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/model/checkpoint_utils.py` & `transphone-1.5.0/transphone/model/checkpoint_utils.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/model/dataset.py` & `transphone-1.5.0/transphone/model/dataset.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/model/ensemble.py` & `transphone-1.5.0/transphone/model/ensemble.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/model/grapheme.py` & `transphone-1.5.0/transphone/model/grapheme.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/model/lstm.py` & `transphone-1.5.0/transphone/model/lstm.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/model/transformer.py` & `transphone-1.5.0/transphone/model/transformer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/model/utils.py` & `transphone-1.5.0/transphone/model/utils.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/model/vocab.py` & `transphone-1.5.0/transphone/model/vocab.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/run.py` & `transphone-1.5.0/transphone/run.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone/tokenizer.py` & `transphone-1.5.0/transphone/tokenizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.4.2/transphone.egg-info/SOURCES.txt` & `transphone-1.5.0/transphone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

