# Comparing `tmp/zeroshot-classifier-0.1.0.tar.gz` & `tmp/zeroshot-classifier-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeroshot-classifier-0.1.0.tar", last modified: Fri May 19 16:02:06 2023, max compression
+gzip compressed data, was "zeroshot-classifier-0.1.1.tar", last modified: Fri May 19 16:16:17 2023, max compression
```

## Comparing `zeroshot-classifier-0.1.0.tar` & `zeroshot-classifier-0.1.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:02:06.694786 zeroshot-classifier-0.1.0/
--rw-r--r--   0 stefanhg   (501) staff       (20)     1351 2023-05-19 16:02:06.694155 zeroshot-classifier-0.1.0/PKG-INFO
--rw-r--r--   0 stefanhg   (501) staff       (20)    11394 2023-05-18 16:52:25.000000 zeroshot-classifier-0.1.0/README.md
--rw-r--r--   0 stefanhg   (501) staff       (20)       38 2023-05-19 16:02:06.695055 zeroshot-classifier-0.1.0/setup.cfg
--rw-r--r--   0 stefanhg   (501) staff       (20)     1708 2023-05-19 16:02:03.000000 zeroshot-classifier-0.1.0/setup.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:02:06.645806 zeroshot-classifier-0.1.0/zeroshot_classifier/
--rw-r--r--   0 stefanhg   (501) staff       (20)       64 2022-06-08 21:00:21.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/__init__.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:02:06.657155 zeroshot-classifier-0.1.0/zeroshot_classifier/models/
--rw-r--r--   0 stefanhg   (501) staff       (20)      120 2023-05-15 21:19:13.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/__init__.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     1648 2023-05-11 21:27:47.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/_bert_based_models.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:02:06.658894 zeroshot-classifier-0.1.0/zeroshot_classifier/models/architecture/
--rw-r--r--   0 stefanhg   (501) staff       (20)       21 2023-05-15 21:19:13.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/architecture/__init__.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     2037 2023-05-11 21:06:00.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/architecture/binary_bert.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    20988 2023-05-15 21:19:13.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/architecture/sbert.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     7617 2023-05-11 21:11:58.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/bart.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     9481 2023-05-18 16:57:42.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/bert.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     6623 2022-10-09 05:20:14.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/bert_nli.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     8224 2023-05-15 16:29:41.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/bi-encoder.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     9586 2023-05-11 21:33:02.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/binary_bert.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:02:06.660216 zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/
--rw-r--r--   0 stefanhg   (501) staff       (20)      113 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/__init__.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    13733 2022-10-11 06:06:43.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/dual_bi_encoder.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:02:06.660821 zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/
--rw-r--r--   0 stefanhg   (501) staff       (20)       23 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/__init__.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:02:06.663064 zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/
--rw-r--r--   0 stefanhg   (501) staff       (20)       37 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/__init__.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    12593 2022-06-08 19:09:36.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/bi.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     6981 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/poly.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     4920 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/sent_enc.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:02:06.664647 zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/tests/
--rw-r--r--   0 stefanhg   (501) staff       (20)        0 2022-06-08 19:09:09.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/tests/__init__.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     2168 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/tests/test_biencoder.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    10637 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/tests/test_data.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:02:06.670542 zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/
--rw-r--r--   0 stefanhg   (501) staff       (20)      595 2022-06-08 21:00:21.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/__init__.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     4392 2022-06-08 19:09:36.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/evaluate.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    11707 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/models.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     8478 2022-06-10 19:38:06.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/tokenizer.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    10795 2022-10-08 11:44:22.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/train.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:02:06.675171 zeroshot-classifier-0.1.0/zeroshot_classifier/models/explicit/
--rw-r--r--   0 stefanhg   (501) staff       (20)       27 2022-06-10 19:40:02.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/explicit/__init__.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    18865 2023-05-11 21:11:58.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/explicit/binary_bert.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     5958 2023-05-11 21:11:58.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/explicit/binary_bert_pretrain.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     2467 2023-05-11 21:11:58.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/explicit/explicit_v2.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     4529 2023-05-11 21:11:58.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/explicit/gpt2_pretrain.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    56056 2023-05-17 16:47:57.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/gpt2.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    18487 2023-05-11 21:11:58.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/gpt3.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    11200 2022-10-21 11:22:04.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/models/gpt_neo.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:02:06.677175 zeroshot-classifier-0.1.0/zeroshot_classifier/preprocess/
--rw-r--r--   0 stefanhg   (501) staff       (20)       23 2022-06-10 19:40:02.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/preprocess/__init__.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     6510 2023-05-11 21:18:59.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/preprocess/dataset.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:02:06.690274 zeroshot-classifier-0.1.0/zeroshot_classifier/util/
--rw-r--r--   0 stefanhg   (501) staff       (20)      270 2022-10-21 05:35:42.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/util/__init__.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    20678 2023-05-15 21:23:22.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/util/config.py
--rw-r--r--   0 stefanhg   (501) staff       (20)      684 2022-10-08 11:42:19.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/util/data_path.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     6424 2022-11-21 23:48:12.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/util/explicit_v2_pretrain.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    35035 2023-05-11 21:22:23.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/util/gpt2_train.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    27648 2023-05-11 21:22:23.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/util/load_data.py
--rw-r--r--   0 stefanhg   (501) staff       (20)      614 2023-05-11 21:22:32.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/util/training.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    32754 2023-05-11 21:25:05.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/util/utcd.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     6660 2023-05-11 21:27:47.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/util/util.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:02:06.692905 zeroshot-classifier-0.1.0/zeroshot_classifier/visualize/
--rw-r--r--   0 stefanhg   (501) staff       (20)       60 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/visualize/__init__.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     6868 2022-10-09 11:59:47.000000 zeroshot-classifier-0.1.0/zeroshot_classifier/visualize/visualize_text_sample_loss.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:02:06.648023 zeroshot-classifier-0.1.0/zeroshot_classifier.egg-info/
--rw-r--r--   0 stefanhg   (501) staff       (20)     1351 2023-05-19 16:02:06.000000 zeroshot-classifier-0.1.0/zeroshot_classifier.egg-info/PKG-INFO
--rw-r--r--   0 stefanhg   (501) staff       (20)     2656 2023-05-19 16:02:06.000000 zeroshot-classifier-0.1.0/zeroshot_classifier.egg-info/SOURCES.txt
--rw-r--r--   0 stefanhg   (501) staff       (20)        1 2023-05-19 16:02:06.000000 zeroshot-classifier-0.1.0/zeroshot_classifier.egg-info/dependency_links.txt
--rw-r--r--   0 stefanhg   (501) staff       (20)      115 2023-05-19 16:02:06.000000 zeroshot-classifier-0.1.0/zeroshot_classifier.egg-info/requires.txt
--rw-r--r--   0 stefanhg   (501) staff       (20)       20 2023-05-19 16:02:06.000000 zeroshot-classifier-0.1.0/zeroshot_classifier.egg-info/top_level.txt
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:16:17.318431 zeroshot-classifier-0.1.1/
+-rw-r--r--   0 stefanhg   (501) staff       (20)     1351 2023-05-19 16:16:17.318060 zeroshot-classifier-0.1.1/PKG-INFO
+-rw-r--r--   0 stefanhg   (501) staff       (20)    11394 2023-05-18 16:52:25.000000 zeroshot-classifier-0.1.1/README.md
+-rw-r--r--   0 stefanhg   (501) staff       (20)       38 2023-05-19 16:16:17.318588 zeroshot-classifier-0.1.1/setup.cfg
+-rw-r--r--   0 stefanhg   (501) staff       (20)     1804 2023-05-19 16:16:12.000000 zeroshot-classifier-0.1.1/setup.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:16:17.243898 zeroshot-classifier-0.1.1/zeroshot_classifier/
+-rw-r--r--   0 stefanhg   (501) staff       (20)       64 2022-06-08 21:00:21.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/__init__.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:16:17.271868 zeroshot-classifier-0.1.1/zeroshot_classifier/models/
+-rw-r--r--   0 stefanhg   (501) staff       (20)      120 2023-05-15 21:19:13.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/__init__.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     1648 2023-05-11 21:27:47.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/_bert_based_models.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:16:17.278844 zeroshot-classifier-0.1.1/zeroshot_classifier/models/architecture/
+-rw-r--r--   0 stefanhg   (501) staff       (20)       21 2023-05-15 21:19:13.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/architecture/__init__.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     2037 2023-05-11 21:06:00.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/architecture/binary_bert.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    20988 2023-05-15 21:19:13.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/architecture/sbert.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     7617 2023-05-11 21:11:58.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/bart.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     9481 2023-05-18 16:57:42.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/bert.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     6623 2022-10-09 05:20:14.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/bert_nli.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     8224 2023-05-15 16:29:41.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/bi-encoder.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     9586 2023-05-11 21:33:02.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/binary_bert.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:16:17.280904 zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/
+-rw-r--r--   0 stefanhg   (501) staff       (20)      113 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/__init__.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    13733 2022-10-11 06:06:43.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/dual_bi_encoder.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:16:17.281772 zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/
+-rw-r--r--   0 stefanhg   (501) staff       (20)       23 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/__init__.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:16:17.286443 zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/
+-rw-r--r--   0 stefanhg   (501) staff       (20)       37 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/__init__.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    12593 2022-06-08 19:09:36.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/bi.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     6981 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/poly.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     4920 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/sent_enc.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:16:17.287869 zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/tests/
+-rw-r--r--   0 stefanhg   (501) staff       (20)        0 2022-06-08 19:09:09.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/tests/__init__.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     2168 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/tests/test_biencoder.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    10637 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/tests/test_data.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:16:17.296582 zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/
+-rw-r--r--   0 stefanhg   (501) staff       (20)      595 2022-06-08 21:00:21.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/__init__.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     4392 2022-06-08 19:09:36.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/evaluate.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    11707 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/models.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     8478 2022-06-10 19:38:06.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/tokenizer.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    10795 2022-10-08 11:44:22.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/train.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:16:17.302266 zeroshot-classifier-0.1.1/zeroshot_classifier/models/explicit/
+-rw-r--r--   0 stefanhg   (501) staff       (20)       27 2022-06-10 19:40:02.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/explicit/__init__.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    18865 2023-05-11 21:11:58.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/explicit/binary_bert.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     5958 2023-05-11 21:11:58.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/explicit/binary_bert_pretrain.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     2467 2023-05-11 21:11:58.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/explicit/explicit_v2.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     4529 2023-05-11 21:11:58.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/explicit/gpt2_pretrain.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    56056 2023-05-17 16:47:57.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/gpt2.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    18487 2023-05-11 21:11:58.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/gpt3.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    11200 2022-10-21 11:22:04.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/models/gpt_neo.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:16:17.305034 zeroshot-classifier-0.1.1/zeroshot_classifier/preprocess/
+-rw-r--r--   0 stefanhg   (501) staff       (20)       23 2022-06-10 19:40:02.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/preprocess/__init__.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     6510 2023-05-11 21:18:59.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/preprocess/dataset.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:16:17.313523 zeroshot-classifier-0.1.1/zeroshot_classifier/util/
+-rw-r--r--   0 stefanhg   (501) staff       (20)      270 2022-10-21 05:35:42.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/util/__init__.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    20678 2023-05-15 21:23:22.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/util/config.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)      684 2022-10-08 11:42:19.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/util/data_path.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     6424 2022-11-21 23:48:12.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/util/explicit_v2_pretrain.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    35035 2023-05-11 21:22:23.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/util/gpt2_train.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    27648 2023-05-11 21:22:23.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/util/load_data.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)      614 2023-05-11 21:22:32.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/util/training.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    32754 2023-05-11 21:25:05.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/util/utcd.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     6660 2023-05-11 21:27:47.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/util/util.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:16:17.315602 zeroshot-classifier-0.1.1/zeroshot_classifier/visualize/
+-rw-r--r--   0 stefanhg   (501) staff       (20)       60 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/visualize/__init__.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     6868 2022-10-09 11:59:47.000000 zeroshot-classifier-0.1.1/zeroshot_classifier/visualize/visualize_text_sample_loss.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:16:17.256783 zeroshot-classifier-0.1.1/zeroshot_classifier.egg-info/
+-rw-r--r--   0 stefanhg   (501) staff       (20)     1351 2023-05-19 16:16:17.000000 zeroshot-classifier-0.1.1/zeroshot_classifier.egg-info/PKG-INFO
+-rw-r--r--   0 stefanhg   (501) staff       (20)     2656 2023-05-19 16:16:17.000000 zeroshot-classifier-0.1.1/zeroshot_classifier.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanhg   (501) staff       (20)        1 2023-05-19 16:16:17.000000 zeroshot-classifier-0.1.1/zeroshot_classifier.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanhg   (501) staff       (20)      203 2023-05-19 16:16:17.000000 zeroshot-classifier-0.1.1/zeroshot_classifier.egg-info/requires.txt
+-rw-r--r--   0 stefanhg   (501) staff       (20)       20 2023-05-19 16:16:17.000000 zeroshot-classifier-0.1.1/zeroshot_classifier.egg-info/top_level.txt
```

### Comparing `zeroshot-classifier-0.1.0/PKG-INFO` & `zeroshot-classifier-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroshot-classifier
-Version: 0.1.0
+Version: 0.1.1
 Summary: code and data for the Findings of ACL'23 paper Label Agnostic Pre-training for Zero-shot Text Classification 
 Home-page: https://github.com/ChrisIsKing/zero-shot-text-classification
 Download-URL: https://github.com/ChrisIsKing/zero-shot-text-classification/archive/refs/tags/v0.1.0.tar.gz
 Author: Christopher Clarke & Yuzhao Heng
 Author-email: csclarke@umich.edu
 License: MIT
 Keywords: python,nlp,machine-learning,deep-learning,text-classification,zero-shot-classification
```

### Comparing `zeroshot-classifier-0.1.0/README.md` & `zeroshot-classifier-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/setup.py` & `zeroshot-classifier-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = """
 code and data for the Findings of ACL'23 paper Label Agnostic Pre-training for Zero-shot Text Classification 
 by Christopher Clarke, Yuzhao Heng, Yiping Kang, Krisztian Flautner, Lingjia Tang and Jason Mars
  """
 
 setup(
     name='zeroshot-classifier',
@@ -15,18 +15,19 @@
     description=DESCRIPTION,
     long_description=DESCRIPTION,
     url='https://github.com/ChrisIsKing/zero-shot-text-classification',
     download_url='https://github.com/ChrisIsKing/zero-shot-text-classification/archive/refs/tags/v0.1.0.tar.gz',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
-        'gdown', 'openai', 'requests', 'tenacity',
-        'spacy', 'nltk', 'scikit-learn', 'torch', 'sentence-transformers', 'transformers',
-        'datasets',
-        'stefutils'
+        'gdown==4.5.4', 'openai==0.25.0', 'requests==2.28.1', 'tenacity==8.1.0',
+        'spacy==3.2.2', 'nltk==3.7', 'scikit-learn==1.1.3',
+        'torch==1.12.0', 'sentence-transformers==2.2.0', 'transformers==4.16.2',
+        'datasets==1.18.3',
+        'stefutils==0.22.2'
     ],
     keywords=['python', 'nlp', 'machine-learning', 'deep-learning', 'text-classification', 'zero-shot-classification'],
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Environment :: GPU :: NVIDIA CUDA',
         'Environment :: GPU :: NVIDIA CUDA :: 11.6',
         'Intended Audience :: Developers',
```

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/_bert_based_models.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/_bert_based_models.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/architecture/binary_bert.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/architecture/binary_bert.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/architecture/sbert.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/architecture/sbert.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/bart.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/bart.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/bert.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/bert.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/bert_nli.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/bert_nli.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/bi-encoder.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/bi-encoder.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/binary_bert.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/binary_bert.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/dual_bi_encoder.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/dual_bi_encoder.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/bi.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/bi.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/poly.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/poly.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/sent_enc.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/sent_enc.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/tests/test_biencoder.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/tests/test_biencoder.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/tests/test_data.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/__init__.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/evaluate.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/models.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/models.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/tokenizer.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/train.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/train.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/explicit/binary_bert.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/explicit/binary_bert.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/explicit/binary_bert_pretrain.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/explicit/binary_bert_pretrain.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/explicit/explicit_v2.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/explicit/explicit_v2.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/explicit/gpt2_pretrain.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/explicit/gpt2_pretrain.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/gpt2.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/gpt3.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/gpt3.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/models/gpt_neo.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/models/gpt_neo.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/preprocess/dataset.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/preprocess/dataset.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/util/config.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/util/config.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/util/data_path.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/util/data_path.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/util/explicit_v2_pretrain.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/util/explicit_v2_pretrain.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/util/gpt2_train.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/util/gpt2_train.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/util/load_data.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/util/load_data.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/util/training.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/util/training.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/util/utcd.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/util/utcd.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/util/util.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/util/util.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier/visualize/visualize_text_sample_loss.py` & `zeroshot-classifier-0.1.1/zeroshot_classifier/visualize/visualize_text_sample_loss.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier.egg-info/PKG-INFO` & `zeroshot-classifier-0.1.1/zeroshot_classifier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroshot-classifier
-Version: 0.1.0
+Version: 0.1.1
 Summary: code and data for the Findings of ACL'23 paper Label Agnostic Pre-training for Zero-shot Text Classification 
 Home-page: https://github.com/ChrisIsKing/zero-shot-text-classification
 Download-URL: https://github.com/ChrisIsKing/zero-shot-text-classification/archive/refs/tags/v0.1.0.tar.gz
 Author: Christopher Clarke & Yuzhao Heng
 Author-email: csclarke@umich.edu
 License: MIT
 Keywords: python,nlp,machine-learning,deep-learning,text-classification,zero-shot-classification
```

### Comparing `zeroshot-classifier-0.1.0/zeroshot_classifier.egg-info/SOURCES.txt` & `zeroshot-classifier-0.1.1/zeroshot_classifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

