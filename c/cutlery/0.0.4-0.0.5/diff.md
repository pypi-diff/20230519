# Comparing `tmp/cutlery-0.0.4.tar.gz` & `tmp/cutlery-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cutlery-0.0.4.tar", last modified: Sun May 14 11:00:56 2023, max compression
+gzip compressed data, was "cutlery-0.0.5.tar", last modified: Fri May 19 14:59:55 2023, max compression
```

## Comparing `cutlery-0.0.4.tar` & `cutlery-0.0.5.tar`

### file list

```diff
@@ -1,230 +1,233 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-14 11:00:56.902857 cutlery-0.0.4/
--rw-r--r--   0 vsts      (1001) docker     (122)     2642 2023-05-14 11:00:37.000000 cutlery-0.0.4/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)     1813 2023-05-14 11:00:56.902857 cutlery-0.0.4/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      895 2023-05-14 11:00:37.000000 cutlery-0.0.4/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-14 11:00:56.870856 cutlery-0.0.4/cutlery/
--rw-r--r--   0 vsts      (1001) docker     (122)      120 2023-05-14 11:00:37.000000 cutlery-0.0.4/cutlery/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      333 2023-05-14 11:00:37.000000 cutlery-0.0.4/cutlery/_bbpe.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     5835 2023-05-14 11:00:37.000000 cutlery-0.0.4/cutlery/_bbpe.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)     2056 2023-05-14 11:00:37.000000 cutlery-0.0.4/cutlery/_spp.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     4015 2023-05-14 11:00:37.000000 cutlery-0.0.4/cutlery/_spp.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      254 2023-05-14 11:00:37.000000 cutlery-0.0.4/cutlery/_wordpiece.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     2919 2023-05-14 11:00:37.000000 cutlery-0.0.4/cutlery/_wordpiece.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      156 2023-05-14 11:00:37.000000 cutlery-0.0.4/cutlery/config.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2126 2023-05-14 11:00:37.000000 cutlery-0.0.4/cutlery/merges.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1470 2023-05-14 11:00:37.000000 cutlery-0.0.4/cutlery/merges.hh
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-14 11:00:56.870856 cutlery-0.0.4/cutlery/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-14 11:00:37.000000 cutlery-0.0.4/cutlery/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)       19 2023-05-14 11:00:37.000000 cutlery-0.0.4/cutlery/tests/incorrect-merges.txt
--rw-r--r--   0 vsts      (1001) docker     (122)     6291 2023-05-14 11:00:37.000000 cutlery-0.0.4/cutlery/tests/robbert-merges-1000.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    16815 2023-05-14 11:00:37.000000 cutlery-0.0.4/cutlery/tests/robbert-vocab-1000.json
--rw-r--r--   0 vsts      (1001) docker     (122)     1854 2023-05-14 11:00:37.000000 cutlery-0.0.4/cutlery/tests/test_bbpe_processor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3640 2023-05-14 11:00:37.000000 cutlery-0.0.4/cutlery/tests/test_sp.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1095 2023-05-14 11:00:37.000000 cutlery-0.0.4/cutlery/tests/test_word_piece_processor.py
--rw-r--r--   0 vsts      (1001) docker     (122)       31 2023-05-14 11:00:37.000000 cutlery-0.0.4/cutlery/tests/toy-word-pieces.txt
--rw-r--r--   0 vsts      (1001) docker     (122)   253270 2023-05-14 11:00:37.000000 cutlery-0.0.4/cutlery/tests/toy.model
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-14 11:00:56.870856 cutlery-0.0.4/cutlery.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1813 2023-05-14 11:00:56.000000 cutlery-0.0.4/cutlery.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    10046 2023-05-14 11:00:56.000000 cutlery-0.0.4/cutlery.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-14 11:00:56.000000 cutlery-0.0.4/cutlery.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       12 2023-05-14 11:00:56.000000 cutlery-0.0.4/cutlery.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        8 2023-05-14 11:00:56.000000 cutlery-0.0.4/cutlery.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-14 11:00:56.000000 cutlery-0.0.4/cutlery.egg-info/zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      107 2023-05-14 11:00:37.000000 cutlery-0.0.4/pyproject.toml
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-14 11:00:56.866856 cutlery-0.0.4/sentencepiece/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-14 11:00:56.870856 cutlery-0.0.4/sentencepiece/python/
--rw-r--r--   0 vsts      (1001) docker     (122)     5858 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/python/once.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-14 11:00:56.890857 cutlery-0.0.4/sentencepiece/src/
--rw-r--r--   0 vsts      (1001) docker     (122)     6648 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/bpe_model.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1748 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/bpe_model.h
--rw-r--r--   0 vsts      (1001) docker     (122)     9294 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/bpe_model_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    10322 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/bpe_model_trainer.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     4416 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/bpe_model_trainer.h
--rw-r--r--   0 vsts      (1001) docker     (122)     4850 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/bpe_model_trainer_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    18401 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/builder.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     5102 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/builder.h
--rw-r--r--   0 vsts      (1001) docker     (122)     7354 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/builder_test.cc
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-14 11:00:56.890857 cutlery-0.0.4/sentencepiece/src/builtin_pb/
--rw-r--r--   0 vsts      (1001) docker     (122)    35154 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/builtin_pb/sentencepiece.pb.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    40648 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/builtin_pb/sentencepiece.pb.h
--rw-r--r--   0 vsts      (1001) docker     (122)   130839 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc
--rw-r--r--   0 vsts      (1001) docker     (122)   189303 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1304 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/char_model.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1061 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/char_model.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3525 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/char_model_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1782 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/char_model_trainer.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1265 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/char_model_trainer.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2506 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/char_model_trainer_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     6007 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/common.h
--rw-r--r--   0 vsts      (1001) docker     (122)     5713 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/compile_charsmap_main.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     4167 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/error.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     3563 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/filesystem.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1852 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/filesystem.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1577 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/filesystem_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2345 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/freelist.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1221 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/freelist_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1341 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/init.h
--rw-r--r--   0 vsts      (1001) docker     (122)     5359 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/init_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1644 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/model_factory.cc
--rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/model_factory.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1743 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/model_factory_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     6609 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/model_interface.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     9527 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/model_interface.h
--rw-r--r--   0 vsts      (1001) docker     (122)    15932 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/model_interface_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)  7198605 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/normalization_rule.h
--rw-r--r--   0 vsts      (1001) docker     (122)    11633 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/normalizer.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     5835 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/normalizer.h
--rw-r--r--   0 vsts      (1001) docker     (122)    16156 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/normalizer_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2024 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/pretokenizer_for_training.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2126 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/pretokenizer_for_training.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2654 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/pretokenizer_for_training_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    30990 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/sentencepiece_processor.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    19673 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/sentencepiece_processor.h
--rw-r--r--   0 vsts      (1001) docker     (122)    47605 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/sentencepiece_processor_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     9966 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/sentencepiece_trainer.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     6527 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/sentencepiece_trainer.h
--rw-r--r--   0 vsts      (1001) docker     (122)    13402 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/sentencepiece_trainer_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    10493 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/spec_parser.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3986 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/spm_decode_main.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     6557 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/spm_encode_main.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2035 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/spm_export_vocab_main.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     4163 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/spm_normalize_main.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    12142 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/spm_train_main.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1026 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/test_main.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1899 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/testharness.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     8718 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/testharness.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2103 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/trainer_factory.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1104 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/trainer_factory.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1656 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/trainer_factory_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    25917 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/trainer_interface.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     5727 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/trainer_interface.h
--rw-r--r--   0 vsts      (1001) docker     (122)    19808 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/trainer_interface_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1239 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/unicode_script.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2807 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/unicode_script.h
--rw-r--r--   0 vsts      (1001) docker     (122)   106446 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/unicode_script_map.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1525 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/unicode_script_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    31219 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/unigram_model.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     6912 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/unigram_model.h
--rw-r--r--   0 vsts      (1001) docker     (122)    32258 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/unigram_model_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    18625 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/unigram_model_trainer.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     3879 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/unigram_model_trainer.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3321 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/unigram_model_trainer_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     7746 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/util.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    11414 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/util.h
--rw-r--r--   0 vsts      (1001) docker     (122)    12866 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/util_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1124 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/word_model.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1045 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/word_model.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2639 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/word_model_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2101 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/word_model_trainer.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1372 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/word_model_trainer.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2464 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/src/word_model_trainer_test.cc
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-14 11:00:56.866856 cutlery-0.0.4/sentencepiece/third_party/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-14 11:00:56.866856 cutlery-0.0.4/sentencepiece/third_party/absl/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-14 11:00:56.890857 cutlery-0.0.4/sentencepiece/third_party/absl/container/
--rw-r--r--   0 vsts      (1001) docker     (122)     1001 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/absl/container/flat_hash_map.h
--rw-r--r--   0 vsts      (1001) docker     (122)      966 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/absl/container/flat_hash_set.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-14 11:00:56.890857 cutlery-0.0.4/sentencepiece/third_party/absl/flags/
--rw-r--r--   0 vsts      (1001) docker     (122)     5614 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/absl/flags/flag.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1673 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/absl/flags/flag.h
--rw-r--r--   0 vsts      (1001) docker     (122)      799 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/absl/flags/parse.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-14 11:00:56.890857 cutlery-0.0.4/sentencepiece/third_party/absl/memory/
--rw-r--r--   0 vsts      (1001) docker     (122)     2592 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/absl/memory/memory.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-14 11:00:56.890857 cutlery-0.0.4/sentencepiece/third_party/absl/strings/
--rw-r--r--   0 vsts      (1001) docker     (122)     1309 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/absl/strings/ascii.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1308 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/absl/strings/match.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1012 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/absl/strings/numbers.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1447 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/absl/strings/str_cat.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/absl/strings/str_format.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2413 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/absl/strings/str_join.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2127 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/absl/strings/str_replace.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2669 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/absl/strings/str_split.h
--rw-r--r--   0 vsts      (1001) docker     (122)     7856 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/absl/strings/string_view.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    20934 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/absl/strings/string_view.h
--rw-r--r--   0 vsts      (1001) docker     (122)      991 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/absl/strings/strip.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-14 11:00:56.890857 cutlery-0.0.4/sentencepiece/third_party/darts_clone/
--rw-r--r--   0 vsts      (1001) docker     (122)    51750 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/darts_clone/darts.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-14 11:00:56.894857 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/
--rw-r--r--   0 vsts      (1001) docker     (122)    15726 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/arena.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     8985 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/arenastring.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     5975 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/bytestream.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    30847 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/coded_stream.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    10999 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/common.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    82338 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/extension_set.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     3573 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     4441 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    30000 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/generated_message_util.cc
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-14 11:00:56.866856 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-14 11:00:56.898857 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/
--rw-r--r--   0 vsts      (1001) docker     (122)     6215 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h
--rw-r--r--   0 vsts      (1001) docker     (122)    29756 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h
--rw-r--r--   0 vsts      (1001) docker     (122)    18092 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h
--rw-r--r--   0 vsts      (1001) docker     (122)    15918 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h
--rw-r--r--   0 vsts      (1001) docker     (122)    96637 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h
--rw-r--r--   0 vsts      (1001) docker     (122)    78585 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h
--rw-r--r--   0 vsts      (1001) docker     (122)    12437 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3993 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3266 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h
--rw-r--r--   0 vsts      (1001) docker     (122)    12532 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h
--rw-r--r--   0 vsts      (1001) docker     (122)    31313 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h
--rw-r--r--   0 vsts      (1001) docker     (122)    10023 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3542 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h
--rw-r--r--   0 vsts      (1001) docker     (122)     7024 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-14 11:00:56.902857 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/io/
--rw-r--r--   0 vsts      (1001) docker     (122)    69376 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h
--rw-r--r--   0 vsts      (1001) docker     (122)     5384 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h
--rw-r--r--   0 vsts      (1001) docker     (122)    10258 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h
--rw-r--r--   0 vsts      (1001) docker     (122)    12750 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h
--rw-r--r--   0 vsts      (1001) docker     (122)    16950 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h
--rw-r--r--   0 vsts      (1001) docker     (122)    48107 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h
--rw-r--r--   0 vsts      (1001) docker     (122)    24921 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h
--rw-r--r--   0 vsts      (1001) docker     (122)     7104 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h
--rw-r--r--   0 vsts      (1001) docker     (122)    31973 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h
--rw-r--r--   0 vsts      (1001) docker     (122)    27172 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h
--rw-r--r--   0 vsts      (1001) docker     (122)     8270 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h
--rw-r--r--   0 vsts      (1001) docker     (122)    32754 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2050 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h
--rw-r--r--   0 vsts      (1001) docker     (122)    20834 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc
--rw-r--r--   0 vsts      (1001) docker     (122)     4209 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc
--rw-r--r--   0 vsts      (1001) docker     (122)   101600 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-14 11:00:56.902857 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/
--rw-r--r--   0 vsts      (1001) docker     (122)    11769 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h
--rw-r--r--   0 vsts      (1001) docker     (122)    17098 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h
--rw-r--r--   0 vsts      (1001) docker     (122)     5733 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h
--rw-r--r--   0 vsts      (1001) docker     (122)     7283 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3911 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h
--rw-r--r--   0 vsts      (1001) docker     (122)    11971 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h
--rw-r--r--   0 vsts      (1001) docker     (122)     8915 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h
--rw-r--r--   0 vsts      (1001) docker     (122)     4903 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h
--rw-r--r--   0 vsts      (1001) docker     (122)    31213 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h
--rw-r--r--   0 vsts      (1001) docker     (122)     6157 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2184 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h
--rw-r--r--   0 vsts      (1001) docker     (122)     5108 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h
--rw-r--r--   0 vsts      (1001) docker     (122)    12765 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3949 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h
--rw-r--r--   0 vsts      (1001) docker     (122)     8558 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3293 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h
--rw-r--r--   0 vsts      (1001) docker     (122)    17861 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3615 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h
--rw-r--r--   0 vsts      (1001) docker     (122)    39629 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3356 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h
--rw-r--r--   0 vsts      (1001) docker     (122)    14401 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h
--rw-r--r--   0 vsts      (1001) docker     (122)    83648 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2756 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     6587 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/int128.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    13526 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/io_win32.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    20751 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/message_lite.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    20703 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/parse_context.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     5500 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/repeated_field.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     4197 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/status.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2096 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/statusor.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     9193 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/stringpiece.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     6283 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/stringprintf.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    26415 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/structurally_valid.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    88575 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/strutil.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    10168 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/time.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    27892 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2392 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    11345 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    13255 2023-05-14 11:00:40.000000 cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1173 2023-05-14 11:00:56.902857 cutlery-0.0.4/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     5856 2023-05-14 11:00:37.000000 cutlery-0.0.4/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-19 14:59:55.188348 cutlery-0.0.5/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2642 2023-05-19 14:59:38.000000 cutlery-0.0.5/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)     1814 2023-05-19 14:59:55.188348 cutlery-0.0.5/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      895 2023-05-19 14:59:38.000000 cutlery-0.0.5/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-19 14:59:55.156348 cutlery-0.0.5/cutlery/
+-rw-r--r--   0 vsts      (1001) docker     (122)      120 2023-05-19 14:59:38.000000 cutlery-0.0.5/cutlery/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      333 2023-05-19 14:59:38.000000 cutlery-0.0.5/cutlery/_bbpe.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     5835 2023-05-19 14:59:38.000000 cutlery-0.0.5/cutlery/_bbpe.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)     2056 2023-05-19 14:59:38.000000 cutlery-0.0.5/cutlery/_spp.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     4015 2023-05-19 14:59:38.000000 cutlery-0.0.5/cutlery/_spp.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      654 2023-05-19 14:59:38.000000 cutlery-0.0.5/cutlery/_wordpiece.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     4395 2023-05-19 14:59:38.000000 cutlery-0.0.5/cutlery/_wordpiece.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      156 2023-05-19 14:59:38.000000 cutlery-0.0.5/cutlery/config.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2126 2023-05-19 14:59:38.000000 cutlery-0.0.5/cutlery/merges.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1190 2023-05-19 14:59:38.000000 cutlery-0.0.5/cutlery/merges.hh
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-19 14:59:55.156348 cutlery-0.0.5/cutlery/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-19 14:59:38.000000 cutlery-0.0.5/cutlery/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       19 2023-05-19 14:59:38.000000 cutlery-0.0.5/cutlery/tests/incorrect-merges.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     6291 2023-05-19 14:59:38.000000 cutlery-0.0.5/cutlery/tests/robbert-merges-1000.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    16815 2023-05-19 14:59:38.000000 cutlery-0.0.5/cutlery/tests/robbert-vocab-1000.json
+-rw-r--r--   0 vsts      (1001) docker     (122)     1854 2023-05-19 14:59:38.000000 cutlery-0.0.5/cutlery/tests/test_bbpe_processor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3640 2023-05-19 14:59:38.000000 cutlery-0.0.5/cutlery/tests/test_sp.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1998 2023-05-19 14:59:38.000000 cutlery-0.0.5/cutlery/tests/test_word_piece_processor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       31 2023-05-19 14:59:38.000000 cutlery-0.0.5/cutlery/tests/toy-word-pieces.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)   253270 2023-05-19 14:59:38.000000 cutlery-0.0.5/cutlery/tests/toy.model
+-rw-r--r--   0 vsts      (1001) docker     (122)      333 2023-05-19 14:59:38.000000 cutlery-0.0.5/cutlery/util.hh
+-rw-r--r--   0 vsts      (1001) docker     (122)     1083 2023-05-19 14:59:38.000000 cutlery-0.0.5/cutlery/wordpiece.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1011 2023-05-19 14:59:38.000000 cutlery-0.0.5/cutlery/wordpiece.hh
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-19 14:59:55.156348 cutlery-0.0.5/cutlery.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1814 2023-05-19 14:59:55.000000 cutlery-0.0.5/cutlery.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    10104 2023-05-19 14:59:55.000000 cutlery-0.0.5/cutlery.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-19 14:59:55.000000 cutlery-0.0.5/cutlery.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       12 2023-05-19 14:59:55.000000 cutlery-0.0.5/cutlery.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        8 2023-05-19 14:59:55.000000 cutlery-0.0.5/cutlery.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-19 14:59:54.000000 cutlery-0.0.5/cutlery.egg-info/zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      107 2023-05-19 14:59:38.000000 cutlery-0.0.5/pyproject.toml
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-19 14:59:55.152348 cutlery-0.0.5/sentencepiece/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-19 14:59:55.156348 cutlery-0.0.5/sentencepiece/python/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5858 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/python/once.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-19 14:59:55.172348 cutlery-0.0.5/sentencepiece/src/
+-rw-r--r--   0 vsts      (1001) docker     (122)     6648 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/bpe_model.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1748 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/bpe_model.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     9294 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/bpe_model_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    10322 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/bpe_model_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4416 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/bpe_model_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     4850 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/bpe_model_trainer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    18401 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/builder.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     5102 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/builder.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     7354 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/builder_test.cc
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-19 14:59:55.172348 cutlery-0.0.5/sentencepiece/src/builtin_pb/
+-rw-r--r--   0 vsts      (1001) docker     (122)    35154 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/builtin_pb/sentencepiece.pb.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    40648 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/builtin_pb/sentencepiece.pb.h
+-rw-r--r--   0 vsts      (1001) docker     (122)   130839 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)   189303 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1304 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/char_model.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1061 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/char_model.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3525 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/char_model_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1782 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/char_model_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1265 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/char_model_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2506 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/char_model_trainer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     6007 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/common.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5713 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/compile_charsmap_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4167 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/error.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     3563 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/filesystem.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1852 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/filesystem.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1577 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/filesystem_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2345 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/freelist.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1221 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/freelist_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1341 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/init.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5359 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/init_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1644 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/model_factory.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/model_factory.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1743 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/model_factory_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     6609 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/model_interface.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     9527 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/model_interface.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    15932 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/model_interface_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)  7198605 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/normalization_rule.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    11633 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/normalizer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     5835 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/normalizer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    16156 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/normalizer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2024 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/pretokenizer_for_training.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2126 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/pretokenizer_for_training.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2654 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/pretokenizer_for_training_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    30990 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/sentencepiece_processor.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    19673 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/sentencepiece_processor.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    47605 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/sentencepiece_processor_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     9966 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/sentencepiece_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     6527 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/sentencepiece_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    13402 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/sentencepiece_trainer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    10493 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/spec_parser.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3986 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/spm_decode_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     6557 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/spm_encode_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2035 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/spm_export_vocab_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4163 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/spm_normalize_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    12142 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/spm_train_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1026 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/test_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1899 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/testharness.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     8718 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/testharness.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2103 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/trainer_factory.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1104 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/trainer_factory.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1656 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/trainer_factory_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    25917 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/trainer_interface.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     5727 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/trainer_interface.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    19808 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/trainer_interface_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1239 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/unicode_script.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2807 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/unicode_script.h
+-rw-r--r--   0 vsts      (1001) docker     (122)   106446 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/unicode_script_map.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1525 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/unicode_script_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    31219 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/unigram_model.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     6912 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/unigram_model.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    32258 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/unigram_model_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    18625 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/unigram_model_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     3879 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/unigram_model_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3321 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/unigram_model_trainer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     7746 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/util.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    11414 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/util.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    12866 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/util_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1124 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/word_model.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1045 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/word_model.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2639 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/word_model_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2101 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/word_model_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1372 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/word_model_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2464 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/src/word_model_trainer_test.cc
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-19 14:59:55.152348 cutlery-0.0.5/sentencepiece/third_party/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-19 14:59:55.152348 cutlery-0.0.5/sentencepiece/third_party/absl/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-19 14:59:55.176348 cutlery-0.0.5/sentencepiece/third_party/absl/container/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1001 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/absl/container/flat_hash_map.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      966 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/absl/container/flat_hash_set.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-19 14:59:55.176348 cutlery-0.0.5/sentencepiece/third_party/absl/flags/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5614 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/absl/flags/flag.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1673 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/absl/flags/flag.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      799 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/absl/flags/parse.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-19 14:59:55.176348 cutlery-0.0.5/sentencepiece/third_party/absl/memory/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2592 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/absl/memory/memory.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-19 14:59:55.176348 cutlery-0.0.5/sentencepiece/third_party/absl/strings/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1309 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/absl/strings/ascii.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1308 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/absl/strings/match.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1012 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/absl/strings/numbers.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1447 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/absl/strings/str_cat.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/absl/strings/str_format.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2413 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/absl/strings/str_join.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2127 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/absl/strings/str_replace.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2669 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/absl/strings/str_split.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     7856 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/absl/strings/string_view.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    20934 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/absl/strings/string_view.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      991 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/absl/strings/strip.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-19 14:59:55.176348 cutlery-0.0.5/sentencepiece/third_party/darts_clone/
+-rw-r--r--   0 vsts      (1001) docker     (122)    51750 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/darts_clone/darts.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-19 14:59:55.180348 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/
+-rw-r--r--   0 vsts      (1001) docker     (122)    15726 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/arena.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     8985 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/arenastring.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     5975 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/bytestream.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    30847 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/coded_stream.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    10999 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/common.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    82338 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/extension_set.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     3573 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4441 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    30000 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/generated_message_util.cc
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-19 14:59:55.152348 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-19 14:59:55.184348 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/
+-rw-r--r--   0 vsts      (1001) docker     (122)     6215 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    29756 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    18092 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    15918 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    96637 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    78585 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    12437 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3993 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3266 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    12532 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    31313 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    10023 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3542 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     7024 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-19 14:59:55.184348 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/io/
+-rw-r--r--   0 vsts      (1001) docker     (122)    69376 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5384 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    10258 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    12750 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    16950 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    48107 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    24921 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     7104 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    31973 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    27172 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     8270 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    32754 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2050 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    20834 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4209 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc
+-rw-r--r--   0 vsts      (1001) docker     (122)   101600 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-19 14:59:55.188348 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/
+-rw-r--r--   0 vsts      (1001) docker     (122)    11769 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    17098 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5733 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     7283 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3911 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    11971 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     8915 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     4903 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    31213 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     6157 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2184 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5108 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    12765 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3949 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     8558 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3293 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    17861 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3615 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    39629 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3356 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    14401 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    83648 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2756 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     6587 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/int128.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    13526 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/io_win32.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    20751 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/message_lite.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    20703 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/parse_context.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     5500 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/repeated_field.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4197 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/status.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2096 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/statusor.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     9193 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/stringpiece.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     6283 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/stringprintf.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    26415 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/structurally_valid.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    88575 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/strutil.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    10168 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/time.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    27892 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2392 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    11345 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    13255 2023-05-19 14:59:42.000000 cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1174 2023-05-19 14:59:55.188348 cutlery-0.0.5/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     5880 2023-05-19 14:59:38.000000 cutlery-0.0.5/setup.py
```

### Comparing `cutlery-0.0.4/LICENSE` & `cutlery-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/PKG-INFO` & `cutlery-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: cutlery
-Version: 0.0.4
+Version: 0.0.5
 Summary: Lightweight piece tokenization library
-Home-page: https://github.com/danieldk/cutlery
+Home-page: https://github.com/explosion/cutlery
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `cutlery-0.0.4/README.md` & `cutlery-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/cutlery/_bbpe.pyx` & `cutlery-0.0.5/cutlery/_bbpe.pyx`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/cutlery/_spp.pxd` & `cutlery-0.0.5/cutlery/_spp.pxd`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/cutlery/_spp.pyx` & `cutlery-0.0.5/cutlery/_spp.pyx`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/cutlery/merges.cc` & `cutlery-0.0.5/cutlery/merges.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/cutlery/tests/robbert-merges-1000.txt` & `cutlery-0.0.5/cutlery/tests/robbert-merges-1000.txt`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/cutlery/tests/robbert-vocab-1000.json` & `cutlery-0.0.5/cutlery/tests/robbert-vocab-1000.json`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/cutlery/tests/test_bbpe_processor.py` & `cutlery-0.0.5/cutlery/tests/test_bbpe_processor.py`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/cutlery/tests/test_sp.py` & `cutlery-0.0.5/cutlery/tests/test_sp.py`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/cutlery/tests/toy.model` & `cutlery-0.0.5/cutlery/tests/toy.model`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/cutlery.egg-info/PKG-INFO` & `cutlery-0.0.5/cutlery.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: cutlery
-Version: 0.0.4
+Version: 0.0.5
 Summary: Lightweight piece tokenization library
-Home-page: https://github.com/danieldk/cutlery
+Home-page: https://github.com/explosion/cutlery
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `cutlery-0.0.4/cutlery.egg-info/SOURCES.txt` & `cutlery-0.0.5/cutlery.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 cutlery/_spp.pxd
 cutlery/_spp.pyx
 cutlery/_wordpiece.pxd
 cutlery/_wordpiece.pyx
 cutlery/config.h
 cutlery/merges.cc
 cutlery/merges.hh
+cutlery/util.hh
+cutlery/wordpiece.cc
+cutlery/wordpiece.hh
 cutlery.egg-info/PKG-INFO
 cutlery.egg-info/SOURCES.txt
 cutlery.egg-info/dependency_links.txt
 cutlery.egg-info/requires.txt
 cutlery.egg-info/top_level.txt
 cutlery.egg-info/zip-safe
 cutlery/tests/__init__.py
```

### Comparing `cutlery-0.0.4/sentencepiece/python/once.h` & `cutlery-0.0.5/sentencepiece/python/once.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/bpe_model.cc` & `cutlery-0.0.5/sentencepiece/src/bpe_model.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/bpe_model.h` & `cutlery-0.0.5/sentencepiece/src/bpe_model.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/bpe_model_test.cc` & `cutlery-0.0.5/sentencepiece/src/bpe_model_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/bpe_model_trainer.cc` & `cutlery-0.0.5/sentencepiece/src/bpe_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/bpe_model_trainer.h` & `cutlery-0.0.5/sentencepiece/src/bpe_model_trainer.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/bpe_model_trainer_test.cc` & `cutlery-0.0.5/sentencepiece/src/bpe_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/builder.cc` & `cutlery-0.0.5/sentencepiece/src/builder.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/builder.h` & `cutlery-0.0.5/sentencepiece/src/builder.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/builder_test.cc` & `cutlery-0.0.5/sentencepiece/src/builder_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/builtin_pb/sentencepiece.pb.cc` & `cutlery-0.0.5/sentencepiece/src/builtin_pb/sentencepiece.pb.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/builtin_pb/sentencepiece.pb.h` & `cutlery-0.0.5/sentencepiece/src/builtin_pb/sentencepiece.pb.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc` & `cutlery-0.0.5/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h` & `cutlery-0.0.5/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/char_model.cc` & `cutlery-0.0.5/sentencepiece/src/char_model.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/char_model.h` & `cutlery-0.0.5/sentencepiece/src/char_model.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/char_model_test.cc` & `cutlery-0.0.5/sentencepiece/src/char_model_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/char_model_trainer.cc` & `cutlery-0.0.5/sentencepiece/src/char_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/char_model_trainer.h` & `cutlery-0.0.5/sentencepiece/src/char_model_trainer.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/char_model_trainer_test.cc` & `cutlery-0.0.5/sentencepiece/src/char_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/common.h` & `cutlery-0.0.5/sentencepiece/src/common.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/compile_charsmap_main.cc` & `cutlery-0.0.5/sentencepiece/src/compile_charsmap_main.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/error.cc` & `cutlery-0.0.5/sentencepiece/src/error.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/filesystem.cc` & `cutlery-0.0.5/sentencepiece/src/filesystem.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/filesystem.h` & `cutlery-0.0.5/sentencepiece/src/filesystem.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/filesystem_test.cc` & `cutlery-0.0.5/sentencepiece/src/filesystem_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/freelist.h` & `cutlery-0.0.5/sentencepiece/src/freelist.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/freelist_test.cc` & `cutlery-0.0.5/sentencepiece/src/freelist_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/init.h` & `cutlery-0.0.5/sentencepiece/src/init.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/init_test.cc` & `cutlery-0.0.5/sentencepiece/src/init_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/model_factory.cc` & `cutlery-0.0.5/sentencepiece/src/model_factory.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/model_factory.h` & `cutlery-0.0.5/sentencepiece/src/model_factory.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/model_factory_test.cc` & `cutlery-0.0.5/sentencepiece/src/model_factory_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/model_interface.cc` & `cutlery-0.0.5/sentencepiece/src/model_interface.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/model_interface.h` & `cutlery-0.0.5/sentencepiece/src/model_interface.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/model_interface_test.cc` & `cutlery-0.0.5/sentencepiece/src/model_interface_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/normalization_rule.h` & `cutlery-0.0.5/sentencepiece/src/normalization_rule.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/normalizer.cc` & `cutlery-0.0.5/sentencepiece/src/normalizer.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/normalizer.h` & `cutlery-0.0.5/sentencepiece/src/normalizer.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/normalizer_test.cc` & `cutlery-0.0.5/sentencepiece/src/normalizer_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/pretokenizer_for_training.cc` & `cutlery-0.0.5/sentencepiece/src/pretokenizer_for_training.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/pretokenizer_for_training.h` & `cutlery-0.0.5/sentencepiece/src/pretokenizer_for_training.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/pretokenizer_for_training_test.cc` & `cutlery-0.0.5/sentencepiece/src/pretokenizer_for_training_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/sentencepiece_processor.cc` & `cutlery-0.0.5/sentencepiece/src/sentencepiece_processor.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/sentencepiece_processor.h` & `cutlery-0.0.5/sentencepiece/src/sentencepiece_processor.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/sentencepiece_processor_test.cc` & `cutlery-0.0.5/sentencepiece/src/sentencepiece_processor_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/sentencepiece_trainer.cc` & `cutlery-0.0.5/sentencepiece/src/sentencepiece_trainer.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/sentencepiece_trainer.h` & `cutlery-0.0.5/sentencepiece/src/sentencepiece_trainer.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/sentencepiece_trainer_test.cc` & `cutlery-0.0.5/sentencepiece/src/sentencepiece_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/spec_parser.h` & `cutlery-0.0.5/sentencepiece/src/spec_parser.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/spm_decode_main.cc` & `cutlery-0.0.5/sentencepiece/src/spm_decode_main.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/spm_encode_main.cc` & `cutlery-0.0.5/sentencepiece/src/spm_encode_main.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/spm_export_vocab_main.cc` & `cutlery-0.0.5/sentencepiece/src/spm_export_vocab_main.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/spm_normalize_main.cc` & `cutlery-0.0.5/sentencepiece/src/spm_normalize_main.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/spm_train_main.cc` & `cutlery-0.0.5/sentencepiece/src/spm_train_main.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/test_main.cc` & `cutlery-0.0.5/sentencepiece/src/test_main.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/testharness.cc` & `cutlery-0.0.5/sentencepiece/src/testharness.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/testharness.h` & `cutlery-0.0.5/sentencepiece/src/testharness.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/trainer_factory.cc` & `cutlery-0.0.5/sentencepiece/src/trainer_factory.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/trainer_factory.h` & `cutlery-0.0.5/sentencepiece/src/trainer_factory.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/trainer_factory_test.cc` & `cutlery-0.0.5/sentencepiece/src/trainer_factory_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/trainer_interface.cc` & `cutlery-0.0.5/sentencepiece/src/trainer_interface.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/trainer_interface.h` & `cutlery-0.0.5/sentencepiece/src/trainer_interface.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/trainer_interface_test.cc` & `cutlery-0.0.5/sentencepiece/src/trainer_interface_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/unicode_script.cc` & `cutlery-0.0.5/sentencepiece/src/unicode_script.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/unicode_script.h` & `cutlery-0.0.5/sentencepiece/src/unicode_script.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/unicode_script_map.h` & `cutlery-0.0.5/sentencepiece/src/unicode_script_map.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/unicode_script_test.cc` & `cutlery-0.0.5/sentencepiece/src/unicode_script_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/unigram_model.cc` & `cutlery-0.0.5/sentencepiece/src/unigram_model.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/unigram_model.h` & `cutlery-0.0.5/sentencepiece/src/unigram_model.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/unigram_model_test.cc` & `cutlery-0.0.5/sentencepiece/src/unigram_model_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/unigram_model_trainer.cc` & `cutlery-0.0.5/sentencepiece/src/unigram_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/unigram_model_trainer.h` & `cutlery-0.0.5/sentencepiece/src/unigram_model_trainer.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/unigram_model_trainer_test.cc` & `cutlery-0.0.5/sentencepiece/src/unigram_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/util.cc` & `cutlery-0.0.5/sentencepiece/src/util.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/util.h` & `cutlery-0.0.5/sentencepiece/src/util.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/util_test.cc` & `cutlery-0.0.5/sentencepiece/src/util_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/word_model.cc` & `cutlery-0.0.5/sentencepiece/src/word_model.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/word_model.h` & `cutlery-0.0.5/sentencepiece/src/word_model.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/word_model_test.cc` & `cutlery-0.0.5/sentencepiece/src/word_model_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/word_model_trainer.cc` & `cutlery-0.0.5/sentencepiece/src/word_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/word_model_trainer.h` & `cutlery-0.0.5/sentencepiece/src/word_model_trainer.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/src/word_model_trainer_test.cc` & `cutlery-0.0.5/sentencepiece/src/word_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/absl/container/flat_hash_map.h` & `cutlery-0.0.5/sentencepiece/third_party/absl/container/flat_hash_map.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/absl/container/flat_hash_set.h` & `cutlery-0.0.5/sentencepiece/third_party/absl/container/flat_hash_set.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/absl/flags/flag.cc` & `cutlery-0.0.5/sentencepiece/third_party/absl/flags/flag.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/absl/flags/flag.h` & `cutlery-0.0.5/sentencepiece/third_party/absl/flags/flag.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/absl/flags/parse.h` & `cutlery-0.0.5/sentencepiece/third_party/absl/flags/parse.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/absl/memory/memory.h` & `cutlery-0.0.5/sentencepiece/third_party/absl/memory/memory.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/absl/strings/ascii.h` & `cutlery-0.0.5/sentencepiece/third_party/absl/strings/ascii.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/absl/strings/match.h` & `cutlery-0.0.5/sentencepiece/third_party/absl/strings/match.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/absl/strings/numbers.h` & `cutlery-0.0.5/sentencepiece/third_party/absl/strings/numbers.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/absl/strings/str_cat.h` & `cutlery-0.0.5/sentencepiece/third_party/absl/strings/str_cat.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/absl/strings/str_format.h` & `cutlery-0.0.5/sentencepiece/third_party/absl/strings/str_format.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/absl/strings/str_join.h` & `cutlery-0.0.5/sentencepiece/third_party/absl/strings/str_join.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/absl/strings/str_replace.h` & `cutlery-0.0.5/sentencepiece/third_party/absl/strings/str_replace.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/absl/strings/str_split.h` & `cutlery-0.0.5/sentencepiece/third_party/absl/strings/str_split.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/absl/strings/string_view.cc` & `cutlery-0.0.5/sentencepiece/third_party/absl/strings/string_view.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/absl/strings/string_view.h` & `cutlery-0.0.5/sentencepiece/third_party/absl/strings/string_view.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/absl/strings/strip.h` & `cutlery-0.0.5/sentencepiece/third_party/absl/strings/strip.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/darts_clone/darts.h` & `cutlery-0.0.5/sentencepiece/third_party/darts_clone/darts.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/arena.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/arena.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/arenastring.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/arenastring.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/bytestream.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/bytestream.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/coded_stream.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/coded_stream.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/common.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/common.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/extension_set.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/extension_set.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/generated_message_util.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/generated_message_util.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/int128.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/int128.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/io_win32.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/io_win32.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/message_lite.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/message_lite.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/parse_context.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/parse_context.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/repeated_field.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/repeated_field.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/status.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/status.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/statusor.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/statusor.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/stringpiece.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/stringpiece.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/stringprintf.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/stringprintf.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/structurally_valid.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/structurally_valid.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/strutil.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/strutil.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/time.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/time.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc` & `cutlery-0.0.5/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc`

 * *Files identical despite different names*

### Comparing `cutlery-0.0.4/setup.cfg` & `cutlery-0.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 description = Lightweight piece tokenization library
-version = 0.0.4
-url = https://github.com/danieldk/cutlery
+version = 0.0.5
+url = https://github.com/explosion/cutlery
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `cutlery-0.0.4/setup.py` & `cutlery-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
                 "sentencepiece/src/builtin_pb",
                 "sentencepiece/third_party/protobuf-lite",
             ],
             language="c++",
         ),
         Extension(
             "cutlery._wordpiece",
-            ["cutlery/_wordpiece.pyx"],
+            ["cutlery/_wordpiece.pyx", "cutlery/wordpiece.cc"],
             language="c++",
         ),
         Extension(
             "cutlery._bbpe",
             ["cutlery/_bbpe.pyx", "cutlery/merges.cc"],
             include_dirs=["cutlery"],
             language="c++",
```

