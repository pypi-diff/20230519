# Comparing `tmp/funasr-0.5.3.tar.gz` & `tmp/funasr-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funasr-0.5.3.tar", last modified: Thu May 18 03:46:27 2023, max compression
+gzip compressed data, was "funasr-0.5.4.tar", last modified: Fri May 19 06:15:35 2023, max compression
```

## Comparing `funasr-0.5.3.tar` & `funasr-0.5.4.tar`

### file list

```diff
@@ -1,426 +1,423 @@
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:27.224642 funasr-0.5.3/
--rw-r--r--   0 zhifu      (502) staff       (20)     1063 2023-02-07 07:13:38.000000 funasr-0.5.3/LICENSE
--rw-r--r--   0 zhifu      (502) staff       (20)     8468 2023-05-18 03:46:27.224154 funasr-0.5.3/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)     7446 2023-05-18 02:19:50.000000 funasr-0.5.3/README.md
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.586757 funasr-0.5.3/funasr/
--rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.645149 funasr-0.5.3/funasr/bin/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/bin/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/bin/aggregate_stats_dirs.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21913 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/asr_inference.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11106 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/asr_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)    25965 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/asr_inference_mfcca.py
--rw-r--r--   0 zhifu      (502) staff       (20)    40504 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/asr_inference_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26713 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/asr_inference_paraformer_streaming.py
--rw-r--r--   0 zhifu      (502) staff       (20)    24956 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/asr_inference_rnnt.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23949 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/asr_inference_uniasr.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1068 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/asr_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1027 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/asr_train_paraformer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1036 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/asr_train_transducer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1024 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/asr_train_uniasr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5382 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/build_trainer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-05-18 02:19:38.000000 funasr-0.5.3/funasr/bin/data2vec_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5327 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/diar_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1010 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/diar_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    14137 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/eend_ola_inference.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     6814 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/lm_calc_perplexity.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14544 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/lm_inference.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3816 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/lm_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1019 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/lm_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3049 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/modelscope_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3593 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/punc_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/punc_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11940 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/punctuation_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11101 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/punctuation_infer_vadrealtime.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23328 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/sa_asr_inference.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1071 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/sa_asr_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    20700 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/sond_inference.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    14841 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/sv_inference.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     4718 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/sv_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     8449 2023-02-11 09:29:33.000000 funasr-0.5.3/funasr/bin/tokenize_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13304 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/tp_inference.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3874 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/tp_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19679 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/vad_inference.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4282 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/vad_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11618 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/vad_inference_online.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.649952 funasr-0.5.3/funasr/datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4338 2023-02-09 08:39:15.000000 funasr-0.5.3/funasr/datasets/collate_fn.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15174 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/datasets/dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15562 2023-03-29 08:06:18.000000 funasr-0.5.3/funasr/datasets/iterable_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12671 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/datasets/iterable_dataset_modelscope.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.655228 funasr-0.5.3/funasr/datasets/large_datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/datasets/large_datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3488 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/datasets/large_datasets/build_dataloader.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.657845 funasr-0.5.3/funasr/datasets/large_datasets/datapipes/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/datasets/large_datasets/datapipes/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.5.3/funasr/datasets/large_datasets/datapipes/batch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/datasets/large_datasets/datapipes/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/datasets/large_datasets/datapipes/map.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9294 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/datasets/large_datasets/dataset.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.668058 funasr-0.5.3/funasr/datasets/large_datasets/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/datasets/large_datasets/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.5.3/funasr/datasets/large_datasets/utils/clipping.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.5.3/funasr/datasets/large_datasets/utils/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1566 2023-05-07 09:22:42.000000 funasr-0.5.3/funasr/datasets/large_datasets/utils/hotword_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/datasets/large_datasets/utils/low_frame_rate.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3303 2023-05-07 09:22:42.000000 funasr-0.5.3/funasr/datasets/large_datasets/utils/padding.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2583 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/datasets/large_datasets/utils/tokenize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-05-18 02:19:38.000000 funasr-0.5.3/funasr/datasets/ms_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31032 2023-04-27 08:40:56.000000 funasr-0.5.3/funasr/datasets/preprocessor.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.669732 funasr-0.5.3/funasr/export/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.3/funasr/export/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10699 2023-05-12 02:41:22.000000 funasr-0.5.3/funasr/export/export_model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.677597 funasr-0.5.3/funasr/export/models/
--rw-r--r--   0 zhifu      (502) staff       (20)     5127 2023-05-07 09:22:42.000000 funasr-0.5.3/funasr/export/models/CT_Transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1540 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/export/models/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.679060 funasr-0.5.3/funasr/export/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.3/funasr/export/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.5.3/funasr/export/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.5.3/funasr/export/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/export/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/export/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.691431 funasr-0.5.3/funasr/export/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.3/funasr/export/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.5.3/funasr/export/models/encoder/conformer_encoder.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/export/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-05-05 07:04:25.000000 funasr-0.5.3/funasr/export/models/encoder/sanm_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.695413 funasr-0.5.3/funasr/export/models/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.3/funasr/export/models/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.5.3/funasr/export/models/modules/decoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/export/models/modules/encoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.5.3/funasr/export/models/modules/feedforward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.5.3/funasr/export/models/modules/multihead_att.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.696512 funasr-0.5.3/funasr/export/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.3/funasr/export/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.5.3/funasr/export/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.698593 funasr-0.5.3/funasr/export/test/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/export/test/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/export/test/test_onnx.py
--rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/export/test/test_onnx_punc.py
--rw-r--r--   0 zhifu      (502) staff       (20)      966 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/export/test/test_onnx_punc_vadrealtime.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/export/test/test_onnx_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/export/test/test_torchscripts.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.699101 funasr-0.5.3/funasr/export/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.3/funasr/export/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.5.3/funasr/export/utils/torch_function.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.711222 funasr-0.5.3/funasr/fileio/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/fileio/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2383 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/fileio/datadir_writer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2357 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/fileio/npy_scp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2361 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/fileio/rand_gen_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2273 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/fileio/read_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3539 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/fileio/sound_scp.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.713464 funasr-0.5.3/funasr/iterators/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/iterators/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/iterators/abs_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7808 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/iterators/chunk_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1140 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/iterators/multiple_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5236 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/iterators/sequence_iter_factory.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.718080 funasr-0.5.3/funasr/layers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/layers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      359 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/layers/abs_normalize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/layers/complex_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3503 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/layers/global_mvn.py
--rw-r--r--   0 zhifu      (502) staff       (20)      349 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/layers/inversible_interface.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2539 2023-03-10 07:21:13.000000 funasr-0.5.3/funasr/layers/label_aggregation.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/layers/log_mel.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10488 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/layers/mask_along_axis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9033 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/layers/sinc_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8436 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/layers/stft.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/layers/time_warp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2309 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/layers/utterance_mvn.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.719241 funasr-0.5.3/funasr/lm/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/lm/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5436 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/lm/abs_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5904 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/lm/seq_rnn_lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4243 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/lm/transformer_lm.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.724737 funasr-0.5.3/funasr/losses/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/losses/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4320 2023-05-09 03:02:42.000000 funasr-0.5.3/funasr/losses/label_smoothing_loss.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.727056 funasr-0.5.3/funasr/main_funcs/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/main_funcs/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4687 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/main_funcs/average_nbest_models.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5610 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/main_funcs/calculate_all_attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5029 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/main_funcs/collect_stats.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/main_funcs/pack_funcs.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.755169 funasr-0.5.3/funasr/models/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6541 2023-02-11 09:29:22.000000 funasr-0.5.3/funasr/models/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5298 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/data2vec.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.758931 funasr-0.5.3/funasr/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/decoder/abs_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    40834 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/models/decoder/contextual_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12133 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/decoder/rnn_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8355 2023-05-09 09:17:41.000000 funasr-0.5.3/funasr/models/decoder/rnnt_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    75199 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/decoder/sv_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    43192 2023-05-09 03:02:42.000000 funasr-0.5.3/funasr/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16707 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/e2e_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/e2e_asr_common.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15709 2023-05-07 09:22:42.000000 funasr-0.5.3/funasr/models/e2e_asr_contextual_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11630 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/e2e_asr_mfcca.py
--rw-r--r--   0 zhifu      (502) staff       (20)    74013 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    34796 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/e2e_asr_transducer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10238 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/e2e_diar_eend_ola.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20581 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/e2e_diar_sond.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19501 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/e2e_sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10098 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/e2e_sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6710 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/e2e_tp.py
--rw-r--r--   0 zhifu      (502) staff       (20)    51737 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/e2e_uni_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31100 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.766377 funasr-0.5.3/funasr/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      503 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/encoder/abs_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    43608 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/encoder/conformer_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20993 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/encoder/data2vec_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.5.3/funasr/models/encoder/ecapa_tdnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.5.3/funasr/models/encoder/encoder_layer_mfcca.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.5.3/funasr/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17514 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/encoder/mfcca_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.775833 funasr-0.5.3/funasr/models/encoder/opennmt_encoders/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.5.3/funasr/models/encoder/opennmt_encoders/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.5.3/funasr/models/encoder/opennmt_encoders/ci_scorers.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11046 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/models/encoder/opennmt_encoders/conv_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13971 2023-02-11 09:30:01.000000 funasr-0.5.3/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21170 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    41077 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/encoder/resnet34_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3634 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/encoder/rnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    54458 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/encoder/sanm_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26890 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/encoder/transformer_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.778546 funasr-0.5.3/funasr/models/frontend/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/frontend/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      400 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/frontend/abs_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9106 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/frontend/default.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/models/frontend/eend_ola_feature.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5759 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/frontend/fused.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4990 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/frontend/s3prl.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20471 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/frontend/wav_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6322 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/frontend/wav_frontend_kaldifeat.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2817 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/frontend/windowing.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.779206 funasr-0.5.3/funasr/models/joint_net/
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.5.3/funasr/models/joint_net/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.5.3/funasr/models/joint_net/joint_network.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.801946 funasr-0.5.3/funasr/models/pooling/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/pooling/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3550 2023-05-09 03:02:42.000000 funasr-0.5.3/funasr/models/pooling/statistic_pooling.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.803537 funasr-0.5.3/funasr/models/postencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/postencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/postencoder/abs_postencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3626 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/postencoder/hugging_face_transformers_postencoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.804074 funasr-0.5.3/funasr/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    35684 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.805815 funasr-0.5.3/funasr/models/preencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/preencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/preencoder/abs_preencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1042 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/preencoder/linear.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10296 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/preencoder/sinc.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.840666 funasr-0.5.3/funasr/models/specaug/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/specaug/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/specaug/abs_specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/specaug/specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4661 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/target_delay_transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4715 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/vad_realtime_transformer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.858248 funasr-0.5.3/funasr/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/add_sos_eos.py
--rw-r--r--   0 zhifu      (502) staff       (20)    38235 2023-05-09 03:02:42.000000 funasr-0.5.3/funasr/modules/attention.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.861741 funasr-0.5.3/funasr/modules/beam_search/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/beam_search/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/beam_search/batch_beam_search.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/beam_search/batch_beam_search_online_sim.py
--rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/beam_search/beam_search.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    20115 2023-05-09 03:02:42.000000 funasr-0.5.3/funasr/modules/beam_search/beam_search_sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.5.3/funasr/modules/beam_search/beam_search_transducer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.875203 funasr-0.5.3/funasr/modules/data2vec/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/data2vec/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5831 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/data2vec/data_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/data2vec/ema_module.py
--rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/data2vec/grad_multiply.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/data2vec/multihead_attention.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/data2vec/quant_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/data2vec/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/data2vec/wav2vec2.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/dynamic_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/dynamic_conv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.5.3/funasr/modules/e2e_asr_common.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.876397 funasr-0.5.3/funasr/modules/eend_ola/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.5.3/funasr/modules/eend_ola/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/modules/eend_ola/encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/modules/eend_ola/encoder_decoder_attractor.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17767 2023-04-27 09:38:10.000000 funasr-0.5.3/funasr/modules/embedding.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.878418 funasr-0.5.3/funasr/modules/frontends/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/frontends/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/frontends/beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/frontends/dnn_beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/frontends/dnn_wpe.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/frontends/feature_transform.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/frontends/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2648 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/frontends/mask_estimator.py
--rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/layer_norm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/lightconv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/lightconv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.5.3/funasr/modules/mask.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.5.3/funasr/modules/multi_layer_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    22963 2023-05-09 09:17:41.000000 funasr-0.5.3/funasr/modules/nets_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/positionwise_feed_forward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3687 2023-05-09 09:17:41.000000 funasr-0.5.3/funasr/modules/repeat.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.880688 funasr-0.5.3/funasr/modules/rnn/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/rnn/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/rnn/argument.py
--rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/rnn/attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/rnn/decoders.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/rnn/encoders.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.882676 funasr-0.5.3/funasr/modules/scorers/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/scorers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/scorers/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/scorers/ctc_prefix_score.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/scorers/length_bonus.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/scorers/scorer_interface.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.885276 funasr-0.5.3/funasr/modules/streaming_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/streaming_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/modules/streaming_utils/chunk_utilis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/streaming_utils/load_fr_tf.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/streaming_utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21441 2023-04-25 03:22:30.000000 funasr-0.5.3/funasr/modules/subsampling.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/subsampling_without_posenc.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.886171 funasr-0.5.3/funasr/optimizers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/optimizers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.5.3/funasr/optimizers/fairseq_adam.py
--rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/optimizers/sgd.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.886451 funasr-0.5.3/funasr/runtime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.5.3/funasr/runtime/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.886687 funasr-0.5.3/funasr/runtime/python/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.5.3/funasr/runtime/python/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.887584 funasr-0.5.3/funasr/runtime/python/libtorch/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.5.3/funasr/runtime/python/libtorch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/runtime/python/libtorch/demo.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.888289 funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/
--rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.890005 funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7040 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4845 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1443 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/runtime/python/libtorch/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.892782 funasr-0.5.3/funasr/runtime/python/onnxruntime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      679 2023-05-12 03:37:01.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      724 2023-05-12 03:39:34.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/demo_punc_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      916 2023-05-12 03:39:34.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/demo_punc_online.py
--rw-r--r--   0 zhifu      (502) staff       (20)      316 2023-05-12 03:39:34.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/demo_vad_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      930 2023-05-12 03:39:34.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/demo_vad_online.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.893946 funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/
--rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13093 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.896272 funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15848 2023-04-23 09:14:56.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9221 2023-05-12 02:56:06.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-05-12 03:03:13.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1580 2023-05-12 03:39:34.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:27.056012 funasr-0.5.3/funasr/samplers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/samplers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/samplers/abs_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6231 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/samplers/build_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5716 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/samplers/folded_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5168 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/samplers/length_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5680 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/samplers/num_elements_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3144 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/samplers/sorted_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2940 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/samplers/unsorted_batch_sampler.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:27.059494 funasr-0.5.3/funasr/schedulers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/schedulers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/schedulers/abs_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2067 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/schedulers/noam_lr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3658 2023-02-09 08:39:15.000000 funasr-0.5.3/funasr/schedulers/tri_stage_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1494 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/schedulers/warmup_lr.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:27.081951 funasr-0.5.3/funasr/tasks/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/tasks/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    74340 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/tasks/abs_task.py
--rw-r--r--   0 zhifu      (502) staff       (20)    60814 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/tasks/asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12089 2023-02-09 08:39:15.000000 funasr-0.5.3/funasr/tasks/data2vec.py
--rw-r--r--   0 zhifu      (502) staff       (20)    32463 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/tasks/diar.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6782 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/tasks/lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8029 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/tasks/punctuation.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21378 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/tasks/sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18814 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/tasks/sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12527 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/tasks/vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:27.088644 funasr-0.5.3/funasr/text/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/text/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/text/abs_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2205 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/text/build_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2230 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/text/char_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1479 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/text/cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/text/korean_cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16601 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/text/phoneme_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1294 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/text/sentencepiece_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2100 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/text/token_id_converter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2074 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/text/word_tokenizer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:27.137542 funasr-0.5.3/funasr/torch_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/torch_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/torch_utils/add_gradient_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/torch_utils/device_funcs.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1052 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/torch_utils/forward_adaptor.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3788 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/torch_utils/initialize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3817 2023-05-07 09:22:42.000000 funasr-0.5.3/funasr/torch_utils/load_pretrained_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/torch_utils/model_summary.py
--rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/torch_utils/pytorch_version.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/torch_utils/recursive_op.py
--rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/torch_utils/set_all_random_seed.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:27.172652 funasr-0.5.3/funasr/train/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/train/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1764 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/train/abs_espnet_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7280 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/train/abs_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3017 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/train/class_choices.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.5.3/funasr/train/distributed_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18344 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/train/reporter.py
--rw-r--r--   0 zhifu      (502) staff       (20)    37188 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/train/trainer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:27.218835 funasr-0.5.3/funasr/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/asr_env_checking.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11612 2023-03-29 08:06:19.000000 funasr-0.5.3/funasr/utils/asr_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      582 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/build_dataclass.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/cli_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/compute_eer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/compute_min_dcf.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/config_argparse.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/get_default_kwargs.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5632 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/griffin_lim.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.5.3/funasr/utils/job_runner.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1607 2023-02-11 09:30:01.000000 funasr-0.5.3/funasr/utils/misc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.5.3/funasr/utils/modelscope_param.py
--rw-r--r--   0 zhifu      (502) staff       (20)      571 2023-05-13 04:23:50.000000 funasr-0.5.3/funasr/utils/modelscope_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/nested_dict_action.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7734 2023-05-09 03:02:42.000000 funasr-0.5.3/funasr/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/sized_dict.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13380 2023-05-10 06:41:10.000000 funasr-0.5.3/funasr/utils/timestamp_tools.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/types.py
--rw-r--r--   0 zhifu      (502) staff       (20)      638 2023-05-12 01:37:03.000000 funasr-0.5.3/funasr/utils/vad_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11760 2023-04-25 03:22:30.000000 funasr-0.5.3/funasr/utils/wav_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/yaml_no_alias_safe_dump.py
--rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-05-18 03:46:00.000000 funasr-0.5.3/funasr/version.txt
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.587836 funasr-0.5.3/funasr.egg-info/
--rw-r--r--   0 zhifu      (502) staff       (20)     8468 2023-05-18 03:46:26.000000 funasr-0.5.3/funasr.egg-info/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)    13412 2023-05-18 03:46:26.000000 funasr-0.5.3/funasr.egg-info/SOURCES.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-05-18 03:46:26.000000 funasr-0.5.3/funasr.egg-info/dependency_links.txt
--rw-r--r--   0 zhifu      (502) staff       (20)      857 2023-05-18 03:46:26.000000 funasr-0.5.3/funasr.egg-info/requires.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-05-18 03:46:26.000000 funasr-0.5.3/funasr.egg-info/top_level.txt
--rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-05-18 03:46:27.224818 funasr-0.5.3/setup.cfg
--rw-r--r--   0 zhifu      (502) staff       (20)     4634 2023-05-18 03:45:59.000000 funasr-0.5.3/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:27.223356 funasr-0.5.3/tests/
--rw-r--r--   0 zhifu      (502) staff       (20)    26162 2023-05-08 08:26:24.000000 funasr-0.5.3/tests/test_asr_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1210 2023-03-29 08:06:19.000000 funasr-0.5.3/tests/test_asr_vad_punc_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.5.3/tests/test_lm_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.5.3/tests/test_punctuation_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1949 2023-04-12 07:23:40.000000 funasr-0.5.3/tests/test_sv_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2298 2023-04-25 05:58:46.000000 funasr-0.5.3/tests/test_vad_inference_pipeline.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.981587 funasr-0.5.4/
+-rw-r--r--   0 zhifu      (502) staff       (20)     1063 2023-02-07 07:13:38.000000 funasr-0.5.4/LICENSE
+-rw-r--r--   0 zhifu      (502) staff       (20)     8311 2023-05-19 06:15:35.981337 funasr-0.5.4/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)     7289 2023-05-19 02:44:33.000000 funasr-0.5.4/README.md
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.521860 funasr-0.5.4/funasr/
+-rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.534683 funasr-0.5.4/funasr/bin/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/bin/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/bin/aggregate_stats_dirs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    68858 2023-05-19 06:00:53.000000 funasr-0.5.4/funasr/bin/asr_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    71803 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/bin/asr_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1653 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/bin/asr_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-05-18 02:19:38.000000 funasr-0.5.4/funasr/bin/data2vec_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    12092 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/bin/diar_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    18753 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/bin/diar_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1180 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/bin/diar_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14974 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/bin/lm_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1189 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/bin/lm_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12512 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/bin/punc_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     8675 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/bin/punc_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      999 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/bin/punc_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1241 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/bin/sa_asr_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5299 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/bin/sv_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    10573 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/bin/sv_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     8449 2023-02-11 09:29:33.000000 funasr-0.5.4/funasr/bin/tokenize_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3999 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/bin/tp_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10220 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/bin/tp_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    17459 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/bin/train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7230 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/bin/vad_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13448 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/bin/vad_inference_launch.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.563431 funasr-0.5.4/funasr/build_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/build_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3425 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/build_utils/build_args.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13977 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/build_utils/build_asr_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      672 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/build_utils/build_dataloader.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9592 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/build_utils/build_diar_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1552 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/build_utils/build_distributed.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1418 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/build_utils/build_lm_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      968 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/build_utils/build_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      810 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/build_utils/build_optimizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2993 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/build_utils/build_pretrain_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2211 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/build_utils/build_punc_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1531 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/build_utils/build_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    35626 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/build_utils/build_trainer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2196 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/build_utils/build_vad_model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.567695 funasr-0.5.4/funasr/datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4338 2023-02-09 08:39:15.000000 funasr-0.5.4/funasr/datasets/collate_fn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15174 2023-04-17 03:36:48.000000 funasr-0.5.4/funasr/datasets/dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15562 2023-03-29 08:06:18.000000 funasr-0.5.4/funasr/datasets/iterable_dataset.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.569516 funasr-0.5.4/funasr/datasets/large_datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/datasets/large_datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3716 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/datasets/large_datasets/build_dataloader.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.571350 funasr-0.5.4/funasr/datasets/large_datasets/datapipes/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/datasets/large_datasets/datapipes/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.5.4/funasr/datasets/large_datasets/datapipes/batch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/datasets/large_datasets/datapipes/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/datasets/large_datasets/datapipes/map.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10035 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/datasets/large_datasets/dataset.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.574012 funasr-0.5.4/funasr/datasets/large_datasets/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/datasets/large_datasets/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.5.4/funasr/datasets/large_datasets/utils/clipping.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.5.4/funasr/datasets/large_datasets/utils/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1566 2023-05-07 09:22:42.000000 funasr-0.5.4/funasr/datasets/large_datasets/utils/hotword_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/datasets/large_datasets/utils/low_frame_rate.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3303 2023-05-07 09:22:42.000000 funasr-0.5.4/funasr/datasets/large_datasets/utils/padding.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2574 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/datasets/large_datasets/utils/tokenize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-05-18 02:19:38.000000 funasr-0.5.4/funasr/datasets/ms_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31032 2023-04-27 08:40:56.000000 funasr-0.5.4/funasr/datasets/preprocessor.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.574521 funasr-0.5.4/funasr/export/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.4/funasr/export/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10699 2023-05-12 02:41:22.000000 funasr-0.5.4/funasr/export/export_model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.586159 funasr-0.5.4/funasr/export/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)     5127 2023-05-07 09:22:42.000000 funasr-0.5.4/funasr/export/models/CT_Transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1540 2023-04-17 03:36:48.000000 funasr-0.5.4/funasr/export/models/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.587937 funasr-0.5.4/funasr/export/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.4/funasr/export/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.5.4/funasr/export/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.5.4/funasr/export/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.5.4/funasr/export/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.5.4/funasr/export/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.590720 funasr-0.5.4/funasr/export/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.4/funasr/export/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.5.4/funasr/export/models/encoder/conformer_encoder.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.5.4/funasr/export/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-05-05 07:04:25.000000 funasr-0.5.4/funasr/export/models/encoder/sanm_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.628040 funasr-0.5.4/funasr/export/models/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.4/funasr/export/models/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.5.4/funasr/export/models/modules/decoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.5.4/funasr/export/models/modules/encoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.5.4/funasr/export/models/modules/feedforward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.5.4/funasr/export/models/modules/multihead_att.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.628672 funasr-0.5.4/funasr/export/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.4/funasr/export/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.5.4/funasr/export/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.659213 funasr-0.5.4/funasr/export/test/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.5.4/funasr/export/test/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.5.4/funasr/export/test/test_onnx.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.5.4/funasr/export/test/test_onnx_punc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      927 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/export/test/test_onnx_punc_vadrealtime.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.5.4/funasr/export/test/test_onnx_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-04-17 03:36:48.000000 funasr-0.5.4/funasr/export/test/test_torchscripts.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.659970 funasr-0.5.4/funasr/export/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.4/funasr/export/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.5.4/funasr/export/utils/torch_function.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.662175 funasr-0.5.4/funasr/fileio/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/fileio/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2383 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/fileio/datadir_writer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2357 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/fileio/npy_scp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2361 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/fileio/rand_gen_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2273 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/fileio/read_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4050 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/fileio/sound_scp.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.669900 funasr-0.5.4/funasr/iterators/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/iterators/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/iterators/abs_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7808 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/iterators/chunk_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1140 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/iterators/multiple_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5236 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/iterators/sequence_iter_factory.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.695296 funasr-0.5.4/funasr/layers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/layers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      358 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/layers/abs_normalize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/layers/complex_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3499 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/layers/global_mvn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      348 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/layers/inversible_interface.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2539 2023-03-10 07:21:13.000000 funasr-0.5.4/funasr/layers/label_aggregation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/layers/log_mel.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10488 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/layers/mask_along_axis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9033 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/layers/sinc_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8436 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/layers/stft.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/layers/time_warp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2309 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/layers/utterance_mvn.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.695700 funasr-0.5.4/funasr/losses/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/losses/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4320 2023-05-09 03:02:42.000000 funasr-0.5.4/funasr/losses/label_smoothing_loss.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.733325 funasr-0.5.4/funasr/main_funcs/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/main_funcs/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4687 2023-04-12 07:23:40.000000 funasr-0.5.4/funasr/main_funcs/average_nbest_models.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/main_funcs/calculate_all_attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5018 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/main_funcs/collect_stats.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.5.4/funasr/main_funcs/pack_funcs.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.776857 funasr-0.5.4/funasr/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/models/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      319 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/base_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6541 2023-02-11 09:29:22.000000 funasr-0.5.4/funasr/models/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5285 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/data2vec.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.804075 funasr-0.5.4/funasr/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/models/decoder/abs_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    40834 2023-04-17 03:36:48.000000 funasr-0.5.4/funasr/models/decoder/contextual_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12133 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/models/decoder/rnn_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8355 2023-05-09 09:17:41.000000 funasr-0.5.4/funasr/models/decoder/rnnt_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    75199 2023-04-17 03:36:48.000000 funasr-0.5.4/funasr/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/models/decoder/sv_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    43192 2023-05-09 03:02:42.000000 funasr-0.5.4/funasr/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16699 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/e2e_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/models/e2e_asr_common.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15709 2023-05-07 09:22:42.000000 funasr-0.5.4/funasr/models/e2e_asr_contextual_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11838 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/e2e_asr_mfcca.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    76949 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    34782 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/e2e_asr_transducer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10226 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/e2e_diar_eend_ola.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20567 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/e2e_diar_sond.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19490 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/e2e_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10084 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/e2e_sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6682 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/e2e_tp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    51719 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/e2e_uni_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31101 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.816930 funasr-0.5.4/funasr/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      502 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/encoder/abs_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    43621 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/encoder/conformer_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20992 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/encoder/data2vec_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.5.4/funasr/models/encoder/ecapa_tdnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.5.4/funasr/models/encoder/encoder_layer_mfcca.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.5.4/funasr/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17681 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/encoder/mfcca_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.825923 funasr-0.5.4/funasr/models/encoder/opennmt_encoders/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.5.4/funasr/models/encoder/opennmt_encoders/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.5.4/funasr/models/encoder/opennmt_encoders/ci_scorers.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11046 2023-04-17 03:36:48.000000 funasr-0.5.4/funasr/models/encoder/opennmt_encoders/conv_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13971 2023-02-11 09:30:01.000000 funasr-0.5.4/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21170 2023-04-17 03:36:48.000000 funasr-0.5.4/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    41076 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/encoder/resnet34_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3633 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/encoder/rnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    53990 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/encoder/sanm_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26890 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/models/encoder/transformer_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.843408 funasr-0.5.4/funasr/models/frontend/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/models/frontend/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      399 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/frontend/abs_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9122 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/frontend/default.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.5.4/funasr/models/frontend/eend_ola_feature.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5758 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/frontend/fused.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4989 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/frontend/s3prl.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20470 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/frontend/wav_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2321 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/frontend/wav_frontend_kaldifeat.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2811 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/frontend/windowing.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.844982 funasr-0.5.4/funasr/models/joint_net/
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.5.4/funasr/models/joint_net/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.5.4/funasr/models/joint_net/joint_network.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.845641 funasr-0.5.4/funasr/models/pooling/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/models/pooling/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3550 2023-05-09 03:02:42.000000 funasr-0.5.4/funasr/models/pooling/statistic_pooling.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.846654 funasr-0.5.4/funasr/models/postencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/models/postencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/models/postencoder/abs_postencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3626 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/models/postencoder/hugging_face_transformers_postencoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.847249 funasr-0.5.4/funasr/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    35747 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.865050 funasr-0.5.4/funasr/models/preencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/models/preencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/models/preencoder/abs_preencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1042 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/models/preencoder/linear.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10296 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/models/preencoder/sinc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5906 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/seq_rnn_lm.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.865795 funasr-0.5.4/funasr/models/specaug/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/models/specaug/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      424 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/specaug/abs_specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/models/specaug/specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4476 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/target_delay_transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4246 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/transformer_lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4666 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/models/vad_realtime_transformer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.876607 funasr-0.5.4/funasr/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/add_sos_eos.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    38235 2023-05-09 03:02:42.000000 funasr-0.5.4/funasr/modules/attention.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.882017 funasr-0.5.4/funasr/modules/beam_search/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/beam_search/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/beam_search/batch_beam_search.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/beam_search/batch_beam_search_online_sim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/beam_search/beam_search.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    20115 2023-05-09 03:02:42.000000 funasr-0.5.4/funasr/modules/beam_search/beam_search_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.5.4/funasr/modules/beam_search/beam_search_transducer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.888356 funasr-0.5.4/funasr/modules/data2vec/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/data2vec/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5831 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/data2vec/data_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/data2vec/ema_module.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/data2vec/grad_multiply.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/data2vec/multihead_attention.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/data2vec/quant_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/data2vec/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/data2vec/wav2vec2.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/dynamic_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/dynamic_conv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.5.4/funasr/modules/e2e_asr_common.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.890254 funasr-0.5.4/funasr/modules/eend_ola/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.5.4/funasr/modules/eend_ola/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.5.4/funasr/modules/eend_ola/encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.5.4/funasr/modules/eend_ola/encoder_decoder_attractor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17767 2023-04-27 09:38:10.000000 funasr-0.5.4/funasr/modules/embedding.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.897380 funasr-0.5.4/funasr/modules/frontends/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/frontends/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/frontends/beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/frontends/dnn_beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/frontends/dnn_wpe.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/frontends/feature_transform.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/frontends/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2648 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/frontends/mask_estimator.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/layer_norm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/lightconv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/lightconv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.5.4/funasr/modules/mask.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.5.4/funasr/modules/multi_layer_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    22963 2023-05-09 09:17:41.000000 funasr-0.5.4/funasr/modules/nets_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/positionwise_feed_forward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3687 2023-05-09 09:17:41.000000 funasr-0.5.4/funasr/modules/repeat.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.899877 funasr-0.5.4/funasr/modules/rnn/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/rnn/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/rnn/argument.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/rnn/attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/rnn/decoders.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/rnn/encoders.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.901569 funasr-0.5.4/funasr/modules/scorers/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/scorers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/scorers/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/scorers/ctc_prefix_score.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/scorers/length_bonus.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/scorers/scorer_interface.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.903126 funasr-0.5.4/funasr/modules/streaming_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/streaming_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.5.4/funasr/modules/streaming_utils/chunk_utilis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/streaming_utils/load_fr_tf.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/streaming_utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21441 2023-04-25 03:22:30.000000 funasr-0.5.4/funasr/modules/subsampling.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/modules/subsampling_without_posenc.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.903962 funasr-0.5.4/funasr/optimizers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/optimizers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.5.4/funasr/optimizers/fairseq_adam.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/optimizers/sgd.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.904154 funasr-0.5.4/funasr/runtime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.5.4/funasr/runtime/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.904285 funasr-0.5.4/funasr/runtime/python/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.5.4/funasr/runtime/python/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.904876 funasr-0.5.4/funasr/runtime/python/libtorch/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.5.4/funasr/runtime/python/libtorch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.5.4/funasr/runtime/python/libtorch/demo.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.905540 funasr-0.5.4/funasr/runtime/python/libtorch/funasr_torch/
+-rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.5.4/funasr/runtime/python/libtorch/funasr_torch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.5.4/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.907848 funasr-0.5.4/funasr/runtime/python/libtorch/funasr_torch/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.5.4/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.5.4/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7040 2023-04-12 07:23:40.000000 funasr-0.5.4/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.5.4/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.5.4/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4845 2023-04-17 03:36:48.000000 funasr-0.5.4/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1443 2023-04-17 03:36:48.000000 funasr-0.5.4/funasr/runtime/python/libtorch/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.910600 funasr-0.5.4/funasr/runtime/python/onnxruntime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.5.4/funasr/runtime/python/onnxruntime/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      679 2023-05-12 03:37:01.000000 funasr-0.5.4/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      724 2023-05-12 03:39:34.000000 funasr-0.5.4/funasr/runtime/python/onnxruntime/demo_punc_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      916 2023-05-12 03:39:34.000000 funasr-0.5.4/funasr/runtime/python/onnxruntime/demo_punc_online.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      316 2023-05-12 03:39:34.000000 funasr-0.5.4/funasr/runtime/python/onnxruntime/demo_vad_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      930 2023-05-12 03:39:34.000000 funasr-0.5.4/funasr/runtime/python/onnxruntime/demo_vad_online.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.912013 funasr-0.5.4/funasr/runtime/python/onnxruntime/funasr_onnx/
+-rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.5.4/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr-0.5.4/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13034 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.916877 funasr-0.5.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.5.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr-0.5.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15848 2023-04-23 09:14:56.000000 funasr-0.5.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.5.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.5.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9221 2023-05-12 02:56:06.000000 funasr-0.5.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-05-12 03:03:13.000000 funasr-0.5.4/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1580 2023-05-12 03:39:34.000000 funasr-0.5.4/funasr/runtime/python/onnxruntime/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.931348 funasr-0.5.4/funasr/samplers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/samplers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/samplers/abs_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6231 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/samplers/build_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5716 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/samplers/folded_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5168 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/samplers/length_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5680 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/samplers/num_elements_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3144 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/samplers/sorted_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2940 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/samplers/unsorted_batch_sampler.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.932657 funasr-0.5.4/funasr/schedulers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/schedulers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/schedulers/abs_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2067 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/schedulers/noam_lr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3658 2023-02-09 08:39:15.000000 funasr-0.5.4/funasr/schedulers/tri_stage_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1494 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/schedulers/warmup_lr.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.940487 funasr-0.5.4/funasr/tasks/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/tasks/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    74927 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/tasks/abs_task.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    53537 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/tasks/asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12089 2023-02-09 08:39:15.000000 funasr-0.5.4/funasr/tasks/data2vec.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    32440 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/tasks/diar.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6755 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/tasks/lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7948 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/tasks/punctuation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21367 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/tasks/sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18791 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/tasks/sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10644 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/tasks/vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.949353 funasr-0.5.4/funasr/text/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/text/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/text/abs_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2205 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/text/build_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2230 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/text/char_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1479 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/text/cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/text/korean_cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16601 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/text/phoneme_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1294 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/text/sentencepiece_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2100 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/text/token_id_converter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2074 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/text/word_tokenizer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.954937 funasr-0.5.4/funasr/torch_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/torch_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/torch_utils/add_gradient_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/torch_utils/device_funcs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1052 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/torch_utils/forward_adaptor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3788 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/torch_utils/initialize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3817 2023-05-07 09:22:42.000000 funasr-0.5.4/funasr/torch_utils/load_pretrained_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/torch_utils/model_summary.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/torch_utils/pytorch_version.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/torch_utils/recursive_op.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/torch_utils/set_all_random_seed.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.956709 funasr-0.5.4/funasr/train/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/train/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11513 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/train/abs_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3017 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/train/class_choices.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.5.4/funasr/train/distributed_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18344 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/train/reporter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    37177 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/train/trainer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.977530 funasr-0.5.4/funasr/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/utils/asr_env_checking.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11612 2023-03-29 08:06:19.000000 funasr-0.5.4/funasr/utils/asr_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      582 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/utils/build_dataclass.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/utils/cli_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/utils/compute_eer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/utils/compute_min_dcf.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.5.4/funasr/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/utils/config_argparse.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/utils/get_default_kwargs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5632 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/utils/griffin_lim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.5.4/funasr/utils/job_runner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1607 2023-02-11 09:30:01.000000 funasr-0.5.4/funasr/utils/misc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.5.4/funasr/utils/modelscope_param.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      571 2023-05-13 04:23:50.000000 funasr-0.5.4/funasr/utils/modelscope_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/utils/nested_dict_action.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7734 2023-05-09 03:02:42.000000 funasr-0.5.4/funasr/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10088 2023-05-18 12:04:14.000000 funasr-0.5.4/funasr/utils/prepare_data.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/utils/sized_dict.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13380 2023-05-10 06:41:10.000000 funasr-0.5.4/funasr/utils/timestamp_tools.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/utils/types.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      638 2023-05-12 01:37:03.000000 funasr-0.5.4/funasr/utils/vad_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11760 2023-04-25 03:22:30.000000 funasr-0.5.4/funasr/utils/wav_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.5.4/funasr/utils/yaml_no_alias_safe_dump.py
+-rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-05-19 06:02:21.000000 funasr-0.5.4/funasr/version.txt
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.523311 funasr-0.5.4/funasr.egg-info/
+-rw-r--r--   0 zhifu      (502) staff       (20)     8311 2023-05-19 06:15:35.000000 funasr-0.5.4/funasr.egg-info/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)    13315 2023-05-19 06:15:35.000000 funasr-0.5.4/funasr.egg-info/SOURCES.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-05-19 06:15:35.000000 funasr-0.5.4/funasr.egg-info/dependency_links.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)      864 2023-05-19 06:15:35.000000 funasr-0.5.4/funasr.egg-info/requires.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-05-19 06:15:35.000000 funasr-0.5.4/funasr.egg-info/top_level.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-05-19 06:15:35.981662 funasr-0.5.4/setup.cfg
+-rw-r--r--   0 zhifu      (502) staff       (20)     4641 2023-05-18 04:45:48.000000 funasr-0.5.4/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-19 06:15:35.980814 funasr-0.5.4/tests/
+-rw-r--r--   0 zhifu      (502) staff       (20)    26162 2023-05-08 08:26:24.000000 funasr-0.5.4/tests/test_asr_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1210 2023-03-29 08:06:19.000000 funasr-0.5.4/tests/test_asr_vad_punc_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.5.4/tests/test_lm_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.5.4/tests/test_punctuation_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1949 2023-04-12 07:23:40.000000 funasr-0.5.4/tests/test_sv_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2298 2023-04-25 05:58:46.000000 funasr-0.5.4/tests/test_vad_inference_pipeline.py
```

### Comparing `funasr-0.5.3/LICENSE` & `funasr-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/PKG-INFO` & `funasr-0.5.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.5.3
+Version: 0.5.4
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -117,26 +117,22 @@
 
 ## License
 This project is licensed under the [The MIT License](https://opensource.org/licenses/MIT). FunASR also contains various third-party components and some code modified from other repos under other open source licenses.
 
 ## Citations
 
 ``` bibtex
-@inproceedings{gao2022paraformer,
-  title={Paraformer: Fast and Accurate Parallel Transformer for Non-autoregressive End-to-End Speech Recognition},
-  author={Gao, Zhifu and Zhang, Shiliang and McLoughlin, Ian and Yan, Zhijie},
+@inproceedings{gao2023funasr,
+  author={Zhifu Gao and Zerui Li and Jiaming Wang and Haoneng Luo and Xian Shi and Mengzhe Chen and Yabin Li and Lingyun Zuo and Zhihao Du and Zhangyu Xiao and Shiliang Zhang},
+  title={FunASR: A Fundamental End-to-End Speech Recognition Toolkit},
+  year={2023},
   booktitle={INTERSPEECH},
-  year={2022}
 }
-@inproceedings{gao2020universal,
-  title={Universal ASR: Unifying Streaming and Non-Streaming ASR Using a Single Encoder-Decoder Model},
-  author={Gao, Zhifu and Zhang, Shiliang and Lei, Ming and McLoughlin, Ian},
-  booktitle={arXiv preprint arXiv:2010.14099},
-  year={2020}
-}
-@inproceedings{Shi2023AchievingTP,
-  title={Achieving Timestamp Prediction While Recognizing with Non-Autoregressive End-to-End ASR Model},
-  author={Xian Shi and Yanni Chen and Shiliang Zhang and Zhijie Yan},
-  booktitle={arXiv preprint arXiv:2301.12343}
-  year={2023}
+@inproceedings{gao22b_interspeech,
+  author={Zhifu Gao and ShiLiang Zhang and Ian McLoughlin and Zhijie Yan},
+  title={{Paraformer: Fast and Accurate Parallel Transformer for Non-autoregressive End-to-End Speech Recognition}},
+  year=2022,
+  booktitle={Proc. Interspeech 2022},
+  pages={2063--2067},
+  doi={10.21437/Interspeech.2022-9996}
 }
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.5.3 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.5.4 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
@@ -94,18 +94,16 @@
 RapidAI) for contributing the Paraformer and CT_Transformer-punc runtime. 6. We
 acknowledge [DeepScience](https://www.deepscience.cn) for contributing the grpc
 service. 6. We acknowledge [AiHealthx](http://www.aihealthx.com/) for
 contributing the websocket service and html5. ## License This project is
 licensed under the [The MIT License](https://opensource.org/licenses/MIT).
 FunASR also contains various third-party components and some code modified from
 other repos under other open source licenses. ## Citations ``` bibtex
-@inproceedings{gao2022paraformer, title={Paraformer: Fast and Accurate Parallel
-Transformer for Non-autoregressive End-to-End Speech Recognition}, author={Gao,
-Zhifu and Zhang, Shiliang and McLoughlin, Ian and Yan, Zhijie}, booktitle=
-{INTERSPEECH}, year={2022} } @inproceedings{gao2020universal, title={Universal
-ASR: Unifying Streaming and Non-Streaming ASR Using a Single Encoder-Decoder
-Model}, author={Gao, Zhifu and Zhang, Shiliang and Lei, Ming and McLoughlin,
-Ian}, booktitle={arXiv preprint arXiv:2010.14099}, year={2020} } @inproceedings
-{Shi2023AchievingTP, title={Achieving Timestamp Prediction While Recognizing
-with Non-Autoregressive End-to-End ASR Model}, author={Xian Shi and Yanni Chen
-and Shiliang Zhang and Zhijie Yan}, booktitle={arXiv preprint arXiv:2301.12343}
-year={2023} } ```
+@inproceedings{gao2023funasr, author={Zhifu Gao and Zerui Li and Jiaming Wang
+and Haoneng Luo and Xian Shi and Mengzhe Chen and Yabin Li and Lingyun Zuo and
+Zhihao Du and Zhangyu Xiao and Shiliang Zhang}, title={FunASR: A Fundamental
+End-to-End Speech Recognition Toolkit}, year={2023}, booktitle={INTERSPEECH}, }
+@inproceedings{gao22b_interspeech, author={Zhifu Gao and ShiLiang Zhang and Ian
+McLoughlin and Zhijie Yan}, title={{Paraformer: Fast and Accurate Parallel
+Transformer for Non-autoregressive End-to-End Speech Recognition}}, year=2022,
+booktitle={Proc. Interspeech 2022}, pages={2063--2067}, doi={10.21437/
+Interspeech.2022-9996} } ```
```

### Comparing `funasr-0.5.3/README.md` & `funasr-0.5.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -90,26 +90,22 @@
 
 ## License
 This project is licensed under the [The MIT License](https://opensource.org/licenses/MIT). FunASR also contains various third-party components and some code modified from other repos under other open source licenses.
 
 ## Citations
 
 ``` bibtex
-@inproceedings{gao2022paraformer,
-  title={Paraformer: Fast and Accurate Parallel Transformer for Non-autoregressive End-to-End Speech Recognition},
-  author={Gao, Zhifu and Zhang, Shiliang and McLoughlin, Ian and Yan, Zhijie},
+@inproceedings{gao2023funasr,
+  author={Zhifu Gao and Zerui Li and Jiaming Wang and Haoneng Luo and Xian Shi and Mengzhe Chen and Yabin Li and Lingyun Zuo and Zhihao Du and Zhangyu Xiao and Shiliang Zhang},
+  title={FunASR: A Fundamental End-to-End Speech Recognition Toolkit},
+  year={2023},
   booktitle={INTERSPEECH},
-  year={2022}
 }
-@inproceedings{gao2020universal,
-  title={Universal ASR: Unifying Streaming and Non-Streaming ASR Using a Single Encoder-Decoder Model},
-  author={Gao, Zhifu and Zhang, Shiliang and Lei, Ming and McLoughlin, Ian},
-  booktitle={arXiv preprint arXiv:2010.14099},
-  year={2020}
-}
-@inproceedings{Shi2023AchievingTP,
-  title={Achieving Timestamp Prediction While Recognizing with Non-Autoregressive End-to-End ASR Model},
-  author={Xian Shi and Yanni Chen and Shiliang Zhang and Zhijie Yan},
-  booktitle={arXiv preprint arXiv:2301.12343}
-  year={2023}
+@inproceedings{gao22b_interspeech,
+  author={Zhifu Gao and ShiLiang Zhang and Ian McLoughlin and Zhijie Yan},
+  title={{Paraformer: Fast and Accurate Parallel Transformer for Non-autoregressive End-to-End Speech Recognition}},
+  year=2022,
+  booktitle={Proc. Interspeech 2022},
+  pages={2063--2067},
+  doi={10.21437/Interspeech.2022-9996}
 }
 ```
```

#### html2text {}

```diff
@@ -81,18 +81,16 @@
 RapidAI) for contributing the Paraformer and CT_Transformer-punc runtime. 6. We
 acknowledge [DeepScience](https://www.deepscience.cn) for contributing the grpc
 service. 6. We acknowledge [AiHealthx](http://www.aihealthx.com/) for
 contributing the websocket service and html5. ## License This project is
 licensed under the [The MIT License](https://opensource.org/licenses/MIT).
 FunASR also contains various third-party components and some code modified from
 other repos under other open source licenses. ## Citations ``` bibtex
-@inproceedings{gao2022paraformer, title={Paraformer: Fast and Accurate Parallel
-Transformer for Non-autoregressive End-to-End Speech Recognition}, author={Gao,
-Zhifu and Zhang, Shiliang and McLoughlin, Ian and Yan, Zhijie}, booktitle=
-{INTERSPEECH}, year={2022} } @inproceedings{gao2020universal, title={Universal
-ASR: Unifying Streaming and Non-Streaming ASR Using a Single Encoder-Decoder
-Model}, author={Gao, Zhifu and Zhang, Shiliang and Lei, Ming and McLoughlin,
-Ian}, booktitle={arXiv preprint arXiv:2010.14099}, year={2020} } @inproceedings
-{Shi2023AchievingTP, title={Achieving Timestamp Prediction While Recognizing
-with Non-Autoregressive End-to-End ASR Model}, author={Xian Shi and Yanni Chen
-and Shiliang Zhang and Zhijie Yan}, booktitle={arXiv preprint arXiv:2301.12343}
-year={2023} } ```
+@inproceedings{gao2023funasr, author={Zhifu Gao and Zerui Li and Jiaming Wang
+and Haoneng Luo and Xian Shi and Mengzhe Chen and Yabin Li and Lingyun Zuo and
+Zhihao Du and Zhangyu Xiao and Shiliang Zhang}, title={FunASR: A Fundamental
+End-to-End Speech Recognition Toolkit}, year={2023}, booktitle={INTERSPEECH}, }
+@inproceedings{gao22b_interspeech, author={Zhifu Gao and ShiLiang Zhang and Ian
+McLoughlin and Zhijie Yan}, title={{Paraformer: Fast and Accurate Parallel
+Transformer for Non-autoregressive End-to-End Speech Recognition}}, year=2022,
+booktitle={Proc. Interspeech 2022}, pages={2063--2067}, doi={10.21437/
+Interspeech.2022-9996} } ```
```

### Comparing `funasr-0.5.3/funasr/bin/aggregate_stats_dirs.py` & `funasr-0.5.4/funasr/bin/aggregate_stats_dirs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/bin/asr_inference_launch.py` & `funasr-0.5.4/funasr/bin/punc_inference_launch.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,325 +1,254 @@
+# -*- encoding: utf-8 -*-
 #!/usr/bin/env python3
+# Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
+#  MIT License  (https://opensource.org/licenses/MIT)
 
 import argparse
 import logging
 import os
 import sys
 from typing import Union, Dict, Any
 
 from funasr.utils import config_argparse
 from funasr.utils.cli_utils import get_commandline_args
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
+from funasr.utils.types import float_or_none
+
+import argparse
+import logging
+from pathlib import Path
+import sys
+from typing import Optional
+from typing import Sequence
+from typing import Tuple
+from typing import Union
+from typing import Any
+from typing import List
+
+import numpy as np
+import torch
+from typeguard import check_argument_types
+
+from funasr.datasets.preprocessor import CodeMixTokenizerCommonPreprocessor
+from funasr.utils.cli_utils import get_commandline_args
+from funasr.tasks.punctuation import PunctuationTask
+from funasr.torch_utils.device_funcs import to_device
+from funasr.torch_utils.forward_adaptor import ForwardAdaptor
+from funasr.torch_utils.set_all_random_seed import set_all_random_seed
+from funasr.utils import config_argparse
+from funasr.utils.types import str2triple_str
+from funasr.utils.types import str_or_none
+from funasr.datasets.preprocessor import split_to_mini_sentence
+from funasr.bin.punc_infer import Text2Punc, Text2PuncVADRealtime
+
+def inference_punc(
+    batch_size: int,
+    dtype: str,
+    ngpu: int,
+    seed: int,
+    num_workers: int,
+    log_level: Union[int, str],
+    key_file: Optional[str],
+    train_config: Optional[str],
+    model_file: Optional[str],
+    output_dir: Optional[str] = None,
+    param_dict: dict = None,
+    **kwargs,
+):
+    assert check_argument_types()
+    logging.basicConfig(
+        level=log_level,
+        format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
+    )
+
+    if ngpu >= 1 and torch.cuda.is_available():
+        device = "cuda"
+    else:
+        device = "cpu"
+
+    # 1. Set random-seed
+    set_all_random_seed(seed)
+    text2punc = Text2Punc(train_config, model_file, device)
+
+    def _forward(
+        data_path_and_name_and_type,
+        raw_inputs: Union[List[Any], bytes, str] = None,
+        output_dir_v2: Optional[str] = None,
+        cache: List[Any] = None,
+        param_dict: dict = None,
+    ):
+        results = []
+        split_size = 20
+
+        if raw_inputs != None:
+            line = raw_inputs.strip()
+            key = "demo"
+            if line == "":
+                item = {'key': key, 'value': ""}
+                results.append(item)
+                return results
+            result, _ = text2punc(line)
+            item = {'key': key, 'value': result}
+            results.append(item)
+            return results
+
+        for inference_text, _, _ in data_path_and_name_and_type:
+            with open(inference_text, "r", encoding="utf-8") as fin:
+                for line in fin:
+                    line = line.strip()
+                    segs = line.split("\t")
+                    if len(segs) != 2:
+                        continue
+                    key = segs[0]
+                    if len(segs[1]) == 0:
+                        continue
+                    result, _ = text2punc(segs[1])
+                    item = {'key': key, 'value': result}
+                    results.append(item)
+        output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
+        if output_path != None:
+            output_file_name = "infer.out"
+            Path(output_path).mkdir(parents=True, exist_ok=True)
+            output_file_path = (Path(output_path) / output_file_name).absolute()
+            with open(output_file_path, "w", encoding="utf-8") as fout:
+                for item_i in results:
+                    key_out = item_i["key"]
+                    value_out = item_i["value"]
+                    fout.write(f"{key_out}\t{value_out}\n")
+        return results
+
+    return _forward
+
+def inference_punc_vad_realtime(
+    batch_size: int,
+    dtype: str,
+    ngpu: int,
+    seed: int,
+    num_workers: int,
+    log_level: Union[int, str],
+    #cache: list,
+    key_file: Optional[str],
+    train_config: Optional[str],
+    model_file: Optional[str],
+    output_dir: Optional[str] = None,
+    param_dict: dict = None,
+    **kwargs,
+):
+    assert check_argument_types()
+    ncpu = kwargs.get("ncpu", 1)
+    torch.set_num_threads(ncpu)
+
+    if ngpu >= 1 and torch.cuda.is_available():
+        device = "cuda"
+    else:
+        device = "cpu"
+
+    # 1. Set random-seed
+    set_all_random_seed(seed)
+    text2punc = Text2PuncVADRealtime(train_config, model_file, device)
+
+    def _forward(
+        data_path_and_name_and_type,
+        raw_inputs: Union[List[Any], bytes, str] = None,
+        output_dir_v2: Optional[str] = None,
+        cache: List[Any] = None,
+        param_dict: dict = None,
+    ):
+        results = []
+        split_size = 10
+        cache_in = param_dict["cache"]
+        if raw_inputs != None:
+            line = raw_inputs.strip()
+            key = "demo"
+            if line == "":
+                item = {'key': key, 'value': ""}
+                results.append(item)
+                return results
+            result, _, cache = text2punc(line, cache_in)
+            param_dict["cache"] = cache
+            item = {'key': key, 'value': result}
+            results.append(item)
+            return results
+
+        return results
+
+    return _forward
+
 
 
+def inference_launch(mode, **kwargs):
+    if mode == "punc":
+        return inference_punc(**kwargs)
+    if mode == "punc_VadRealtime":
+        return inference_punc_vad_realtime(**kwargs)
+    else:
+        logging.info("Unknown decoding mode: {}".format(mode))
+        return None
+
 def get_parser():
     parser = config_argparse.ArgumentParser(
-        description="ASR Decoding",
+        description="Punctuation inference",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
-    # Note(kamo): Use '_' instead of '-' as separator.
-    # '-' is confusing if written in yaml.
     parser.add_argument(
         "--log_level",
         type=lambda x: x.upper(),
         default="INFO",
         choices=("CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET"),
         help="The verbose level of logging",
     )
-
     parser.add_argument("--output_dir", type=str, required=True)
+    parser.add_argument("--gpuid_list", type=str, required=True)
     parser.add_argument(
         "--ngpu",
         type=int,
         default=0,
         help="The number of gpus. 0 indicates CPU mode",
     )
-    parser.add_argument(
-        "--njob",
-        type=int,
-        default=1,
-        help="The number of jobs for each gpu",
-    )
-    parser.add_argument(
-        "--gpuid_list",
-        type=str,
-        default="",
-        help="The visible gpus",
-    )
     parser.add_argument("--seed", type=int, default=0, help="Random seed")
+    parser.add_argument("--njob", type=int, default=1, help="Random seed")
     parser.add_argument(
         "--dtype",
         default="float32",
         choices=["float16", "float32", "float64"],
         help="Data type",
     )
     parser.add_argument(
         "--num_workers",
         type=int,
         default=1,
         help="The number of workers used for DataLoader",
     )
-
-    group = parser.add_argument_group("Input data related")
-    group.add_argument(
-        "--data_path_and_name_and_type",
-        type=str2triple_str,
-        required=True,
-        action="append",
-    )
-    group.add_argument("--key_file", type=str_or_none)
-    group.add_argument("--allow_variable_data_keys", type=str2bool, default=False)
-    group.add_argument(
-            "--mc",
-            type=bool,
-            default=False,
-            help="MultiChannel input",
-        )
-        
-    group = parser.add_argument_group("The model configuration related")
-    group.add_argument(
-        "--vad_infer_config",
-        type=str,
-        help="VAD infer configuration",
-    )
-    group.add_argument(
-        "--vad_model_file",
-        type=str,
-        help="VAD model parameter file",
-    )
-    group.add_argument(
-        "--cmvn_file",
-        type=str,
-        help="Global CMVN file",
-    )
-    group.add_argument(
-        "--asr_train_config",
-        type=str,
-        help="ASR training configuration",
-    )
-    group.add_argument(
-        "--asr_model_file",
-        type=str,
-        help="ASR model parameter file",
-    )
-    group.add_argument(
-        "--lm_train_config",
-        type=str,
-        help="LM training configuration",
-    )
-    group.add_argument(
-        "--lm_file",
-        type=str,
-        help="LM parameter file",
-    )
-    group.add_argument(
-        "--word_lm_train_config",
-        type=str,
-        help="Word LM training configuration",
-    )
-    group.add_argument(
-        "--word_lm_file",
-        type=str,
-        help="Word LM parameter file",
-    )
-    group.add_argument(
-        "--ngram_file",
-        type=str,
-        help="N-gram parameter file",
-    )
-    group.add_argument(
-        "--model_tag",
-        type=str,
-        help="Pretrained model tag. If specify this option, *_train_config and "
-             "*_file will be overwritten",
-    )
-    group.add_argument(
-        "--beam_search_config",
-        default={},
-        help="The keyword arguments for transducer beam search.",
-    )
-
-    group = parser.add_argument_group("Beam-search related")
-    group.add_argument(
+    parser.add_argument(
         "--batch_size",
         type=int,
         default=1,
         help="The batch size for inference",
     )
-    group.add_argument("--nbest", type=int, default=5, help="Output N-best hypotheses")
-    group.add_argument("--beam_size", type=int, default=20, help="Beam size")
-    group.add_argument("--penalty", type=float, default=0.0, help="Insertion penalty")
-    group.add_argument(
-        "--maxlenratio",
-        type=float,
-        default=0.0,
-        help="Input length ratio to obtain max output length. "
-             "If maxlenratio=0.0 (default), it uses a end-detect "
-             "function "
-             "to automatically find maximum hypothesis lengths."
-             "If maxlenratio<0.0, its absolute value is interpreted"
-             "as a constant max output length",
-    )
-    group.add_argument(
-        "--minlenratio",
-        type=float,
-        default=0.0,
-        help="Input length ratio to obtain min output length",
-    )
-    group.add_argument(
-        "--ctc_weight",
-        type=float,
-        default=0.0,
-        help="CTC weight in joint decoding",
-    )
-    group.add_argument("--lm_weight", type=float, default=1.0, help="RNNLM weight")
-    group.add_argument("--ngram_weight", type=float, default=0.9, help="ngram weight")
-    group.add_argument("--streaming", type=str2bool, default=False)
-    group.add_argument("--simu_streaming", type=str2bool, default=False)
-    group.add_argument("--chunk_size", type=int, default=16)
-    group.add_argument("--left_context", type=int, default=16)
-    group.add_argument("--right_context", type=int, default=0)
-    group.add_argument(
-        "--display_partial_hypotheses",
-        type=bool,
-        default=False,
-        help="Whether to display partial hypotheses during chunk-by-chunk inference.",
-    )    
-   
-    group = parser.add_argument_group("Dynamic quantization related")
-    group.add_argument(
-        "--quantize_asr_model",
-        type=bool,
-        default=False,
-        help="Apply dynamic quantization to ASR model.",
-    )
-    group.add_argument(
-        "--quantize_modules",
-        nargs="*",
-        default=None,
-        help="""Module names to apply dynamic quantization on.
-        The module names are provided as a list, where each name is separated
-        by a comma (e.g.: --quantize-config=[Linear,LSTM,GRU]).
-        Each specified name should be an attribute of 'torch.nn', e.g.:
-        torch.nn.Linear, torch.nn.LSTM, torch.nn.GRU, ...""",
-    )
-    group.add_argument(
-        "--quantize_dtype",
-        type=str,
-        default="qint8",
-        choices=["float16", "qint8"],
-        help="Dtype for dynamic quantization.",
-    )    
-
-    group = parser.add_argument_group("Text converter related")
-    group.add_argument(
-        "--token_type",
-        type=str_or_none,
-        default=None,
-        choices=["char", "bpe", None],
-        help="The token type for ASR model. "
-             "If not given, refers from the training args",
-    )
-    group.add_argument(
-        "--bpemodel",
-        type=str_or_none,
-        default=None,
-        help="The model path of sentencepiece. "
-             "If not given, refers from the training args",
-    )
-    group.add_argument("--token_num_relax", type=int, default=1, help="")
-    group.add_argument("--decoding_ind", type=int, default=0, help="")
-    group.add_argument("--decoding_mode", type=str, default="model1", help="")
-    group.add_argument(
-        "--ctc_weight2",
-        type=float,
-        default=0.0,
-        help="CTC weight in joint decoding",
-    )
-    return parser
-
 
-
-def inference_launch(**kwargs):
-    if 'mode' in kwargs:
-        mode = kwargs['mode']
-    else:
-        logging.info("Unknown decoding mode.")
-        return None
-    if mode == "asr":
-        from funasr.bin.asr_inference import inference_modelscope
-        return inference_modelscope(**kwargs)
-    elif mode == "uniasr":
-        from funasr.bin.asr_inference_uniasr import inference_modelscope
-        return inference_modelscope(**kwargs)
-    elif mode == "paraformer":
-        from funasr.bin.asr_inference_paraformer import inference_modelscope
-        return inference_modelscope(**kwargs)
-    elif mode == "paraformer_streaming":
-        from funasr.bin.asr_inference_paraformer_streaming import inference_modelscope
-        return inference_modelscope(**kwargs)
-    elif mode.startswith("paraformer_vad"):
-        from funasr.bin.asr_inference_paraformer import inference_modelscope_vad_punc
-        return inference_modelscope_vad_punc(**kwargs)
-    elif mode == "mfcca":
-        from funasr.bin.asr_inference_mfcca import inference_modelscope
-        return inference_modelscope(**kwargs)
-    elif mode == "rnnt":
-        from funasr.bin.asr_inference_rnnt import inference_modelscope
-        return inference_modelscope(**kwargs)
-    else:
-        logging.info("Unknown decoding mode: {}".format(mode))
-        return None
-
-def inference_launch_funasr(**kwargs):
-    if 'mode' in kwargs:
-        mode = kwargs['mode']
-    else:
-        logging.info("Unknown decoding mode.")
-        return None
-    if mode == "asr":
-        from funasr.bin.asr_inference import inference
-        return inference(**kwargs)
-    elif mode == "sa_asr":
-        from funasr.bin.sa_asr_inference import inference
-        return inference(**kwargs)
-    elif mode == "uniasr":
-        from funasr.bin.asr_inference_uniasr import inference
-        return inference(**kwargs)
-    elif mode == "paraformer":
-        from funasr.bin.asr_inference_paraformer import inference_modelscope
-        inference_pipeline = inference_modelscope(**kwargs)
-        return inference_pipeline(kwargs["data_path_and_name_and_type"], hotword=kwargs.get("hotword", None))
-    elif mode.startswith("paraformer_vad"):
-        from funasr.bin.asr_inference_paraformer import inference_modelscope_vad_punc
-        inference_pipeline = inference_modelscope_vad_punc(**kwargs)
-        return inference_pipeline(kwargs["data_path_and_name_and_type"], hotword=kwargs.get("hotword", None))
-    elif mode == "mfcca":
-        from funasr.bin.asr_inference_mfcca import inference_modelscope
-        return inference_modelscope(**kwargs)
-    elif mode == "rnnt":
-        from funasr.bin.asr_inference_rnnt import inference
-        return inference(**kwargs)
-    else:
-        logging.info("Unknown decoding mode: {}".format(mode))
-        return None
+    group = parser.add_argument_group("Input data related")
+    group.add_argument("--data_path_and_name_and_type", type=str2triple_str, action="append", required=False)
+    group.add_argument("--raw_inputs", type=str, required=False)
+    group.add_argument("--key_file", type=str_or_none)
+    group.add_argument("--cache", type=list, required=False)
+    group.add_argument("--param_dict", type=dict, required=False)
+    group = parser.add_argument_group("The model configuration related")
+    group.add_argument("--train_config", type=str)
+    group.add_argument("--model_file", type=str)
+    group.add_argument("--mode", type=str, default="punc")
+    return parser
 
 
 def main(cmd=None):
     print(get_commandline_args(), file=sys.stderr)
     parser = get_parser()
-    parser.add_argument(
-        "--mode",
-        type=str,
-        default="asr",
-        help="The decoding mode",
-    )
     args = parser.parse_args(cmd)
     kwargs = vars(args)
     kwargs.pop("config", None)
 
     # set logging messages
     logging.basicConfig(
         level=args.log_level,
@@ -330,12 +259,16 @@
     # gpu setting
     if args.ngpu > 0:
         jobid = int(args.output_dir.split(".")[-1])
         gpuid = args.gpuid_list.split(",")[(jobid - 1) // args.njob]
         os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
         os.environ["CUDA_VISIBLE_DEVICES"] = gpuid
 
-    inference_launch_funasr(**kwargs)
+    kwargs.pop("gpuid_list", None)
+    kwargs.pop("njob", None)
+    inference_pipeline = inference_launch(**kwargs)
+    return inference_pipeline(kwargs["data_path_and_name_and_type"])
+
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `funasr-0.5.3/funasr/bin/asr_inference_mfcca.py` & `funasr-0.5.4/funasr/modules/data2vec/multihead_attention.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,767 +1,671 @@
-#!/usr/bin/env python3
-# Copyright ESPnet (https://github.com/espnet/espnet). All Rights Reserved.
-#  Apache 2.0  (http://www.apache.org/licenses/LICENSE-2.0)
+# Copyright (c) Facebook, Inc. and its affiliates.
+#
+# This source code is licensed under the MIT license found in the
+# LICENSE file in the root directory of this source tree.
 
-import argparse
 import logging
-import sys
-from pathlib import Path
-from typing import Any
-from typing import List
-from typing import Optional
-from typing import Sequence
-from typing import Tuple
-from typing import Union
-from typing import Dict
+import math
+from typing import Dict, List, Optional, Tuple
 
-import numpy as np
 import torch
-from typeguard import check_argument_types
-from typeguard import check_return_type
+import torch.nn.functional as F
+from torch import Tensor, nn
+from torch.nn import Parameter
+
+from funasr.modules.data2vec.quant_noise import quant_noise
+
+
+class FairseqDropout(nn.Module):
+    def __init__(self, p, module_name=None):
+        super().__init__()
+        self.p = p
+        self.module_name = module_name
+        self.apply_during_inference = False
+
+    def forward(self, x, inplace: bool = False):
+        if self.p > 0 and (self.training or self.apply_during_inference):
+            return F.dropout(x, p=self.p, training=True, inplace=inplace)
+        else:
+            return x
+
+    def make_generation_fast_(
+            self,
+            name: str,
+            retain_dropout: bool = False,
+            retain_dropout_modules: Optional[List[str]] = None,
+            **kwargs
+    ):
+        if retain_dropout:
+            if retain_dropout_modules is not None and self.module_name is None:
+                logging.warning(
+                    "Cannot enable dropout during inference for module {} "
+                    "because module_name was not set".format(name)
+                )
+            elif (
+                    retain_dropout_modules is None  # if None, apply to all modules
+                    or self.module_name in retain_dropout_modules
+            ):
+                logging.info(
+                    "Enabling dropout during inference for module: {}".format(name)
+                )
+                self.apply_during_inference = True
+            else:
+                logging.info("Disabling dropout for module: {}".format(name))
 
-from funasr.fileio.datadir_writer import DatadirWriter
-from funasr.modules.beam_search.batch_beam_search import BatchBeamSearch
-from funasr.modules.beam_search.beam_search import BeamSearch
-from funasr.modules.beam_search.beam_search import Hypothesis
-from funasr.modules.scorers.ctc import CTCPrefixScorer
-from funasr.modules.scorers.length_bonus import LengthBonus
-from funasr.modules.scorers.scorer_interface import BatchScorerInterface
-from funasr.modules.subsampling import TooShortUttError
-from funasr.tasks.asr import ASRTaskMFCCA as ASRTask
-from funasr.tasks.lm import LMTask
-from funasr.text.build_tokenizer import build_tokenizer
-from funasr.text.token_id_converter import TokenIDConverter
-from funasr.torch_utils.device_funcs import to_device
-from funasr.torch_utils.set_all_random_seed import set_all_random_seed
-from funasr.utils import config_argparse
-from funasr.utils.cli_utils import get_commandline_args
-from funasr.utils.types import str2bool
-from funasr.utils.types import str2triple_str
-from funasr.utils.types import str_or_none
-from funasr.utils import asr_utils, wav_utils, postprocess_utils
-import pdb
-
-
-global_asr_language: str = 'zh-cn'
-global_sample_rate: Union[int, Dict[Any, int]] = {
-    'audio_fs': 16000,
-    'model_fs': 16000
-}
-
-class Speech2Text:
-    """Speech2Text class
-
-    Examples:
-        >>> import soundfile
-        >>> speech2text = Speech2Text("asr_config.yml", "asr.pb")
-        >>> audio, rate = soundfile.read("speech.wav")
-        >>> speech2text(audio)
-        [(text, token, token_int, hypothesis object), ...]
 
+class MultiheadAttention(nn.Module):
+    """Multi-headed attention.
+
+    See "Attention Is All You Need" for more details.
     """
 
     def __init__(
             self,
-            asr_train_config: Union[Path, str] = None,
-            asr_model_file: Union[Path, str] = None,
-            cmvn_file: Union[Path, str] = None,
-            lm_train_config: Union[Path, str] = None,
-            lm_file: Union[Path, str] = None,
-            token_type: str = None,
-            bpemodel: str = None,
-            device: str = "cpu",
-            maxlenratio: float = 0.0,
-            minlenratio: float = 0.0,
-            batch_size: int = 1,
-            dtype: str = "float32",
-            beam_size: int = 20,
-            ctc_weight: float = 0.5,
-            lm_weight: float = 1.0,
-            ngram_weight: float = 0.9,
-            penalty: float = 0.0,
-            nbest: int = 1,
-            streaming: bool = False,
-            **kwargs,
+            embed_dim,
+            num_heads,
+            kdim=None,
+            vdim=None,
+            dropout=0.0,
+            bias=True,
+            add_bias_kv=False,
+            add_zero_attn=False,
+            self_attention=False,
+            encoder_decoder_attention=False,
+            q_noise=0.0,
+            qn_block_size=8,
     ):
-        assert check_argument_types()
-
-        # 1. Build ASR model
-        scorers = {}
-        asr_model, asr_train_args = ASRTask.build_model_from_file(
-            asr_train_config, asr_model_file, cmvn_file, device
+        super().__init__()
+        self.embed_dim = embed_dim
+        self.kdim = kdim if kdim is not None else embed_dim
+        self.vdim = vdim if vdim is not None else embed_dim
+        self.qkv_same_dim = self.kdim == embed_dim and self.vdim == embed_dim
+
+        self.num_heads = num_heads
+        self.dropout_module = FairseqDropout(
+            dropout, module_name=self.__class__.__name__
         )
 
-        logging.info("asr_model: {}".format(asr_model))
-        logging.info("asr_train_args: {}".format(asr_train_args))
-        asr_model.to(dtype=getattr(torch, dtype)).eval()
-
-        decoder = asr_model.decoder
-
-        ctc = CTCPrefixScorer(ctc=asr_model.ctc, eos=asr_model.eos)
-        token_list = asr_model.token_list
-        scorers.update(
-            decoder=decoder,
-            ctc=ctc,
-            length_bonus=LengthBonus(len(token_list)),
+        self.head_dim = embed_dim // num_heads
+        assert (
+                self.head_dim * num_heads == self.embed_dim
+        ), "embed_dim must be divisible by num_heads"
+        self.scaling = self.head_dim ** -0.5
+
+        self.self_attention = self_attention
+        self.encoder_decoder_attention = encoder_decoder_attention
+
+        assert not self.self_attention or self.qkv_same_dim, (
+            "Self-attention requires query, key and " "value to be of the same size"
         )
 
-        # 2. Build Language model
-        if lm_train_config is not None:
-            lm, lm_train_args = LMTask.build_model_from_file(
-                lm_train_config, lm_file, device
-            )
-            lm.to(device)
-            scorers["lm"] = lm.lm
-        # 3. Build ngram model
-        # ngram is not supported now
-        ngram = None
-        scorers["ngram"] = ngram
-
-        # 4. Build BeamSearch object
-        # transducer is not supported now
-        beam_search_transducer = None
-
-        weights = dict(
-            decoder=1.0 - ctc_weight,
-            ctc=ctc_weight,
-            lm=lm_weight,
-            ngram=ngram_weight,
-            length_bonus=penalty,
+        self.k_proj = quant_noise(
+            nn.Linear(self.kdim, embed_dim, bias=bias), q_noise, qn_block_size
         )
-        beam_search = BeamSearch(
-            beam_size=beam_size,
-            weights=weights,
-            scorers=scorers,
-            sos=asr_model.sos,
-            eos=asr_model.eos,
-            vocab_size=len(token_list),
-            token_list=token_list,
-            pre_beam_score_key=None if ctc_weight == 1.0 else "full",
+        self.v_proj = quant_noise(
+            nn.Linear(self.vdim, embed_dim, bias=bias), q_noise, qn_block_size
         )
-        #beam_search.__class__ = BatchBeamSearch
-        # 5. [Optional] Build Text converter: e.g. bpe-sym -> Text
-        if token_type is None:
-            token_type = asr_train_args.token_type
-        if bpemodel is None:
-            bpemodel = asr_train_args.bpemodel
-        
-        if token_type is None:
-            tokenizer = None
-        elif token_type == "bpe":
-            if bpemodel is not None:
-                tokenizer = build_tokenizer(token_type=token_type, bpemodel=bpemodel)
-            else:
-                tokenizer = None
+        self.q_proj = quant_noise(
+            nn.Linear(embed_dim, embed_dim, bias=bias), q_noise, qn_block_size
+        )
+
+        self.out_proj = quant_noise(
+            nn.Linear(embed_dim, embed_dim, bias=bias), q_noise, qn_block_size
+        )
+
+        if add_bias_kv:
+            self.bias_k = Parameter(torch.Tensor(1, 1, embed_dim))
+            self.bias_v = Parameter(torch.Tensor(1, 1, embed_dim))
         else:
-            tokenizer = build_tokenizer(token_type=token_type)
-        converter = TokenIDConverter(token_list=token_list)
-        logging.info(f"Text tokenizer: {tokenizer}")
-
-        self.asr_model = asr_model
-        self.asr_train_args = asr_train_args
-        self.converter = converter
-        self.tokenizer = tokenizer
-        self.beam_search = beam_search
-        self.beam_search_transducer = beam_search_transducer
-        self.maxlenratio = maxlenratio
-        self.minlenratio = minlenratio
-        self.device = device
-        self.dtype = dtype
-        self.nbest = nbest
-
-    @torch.no_grad()
-    def __call__(
-            self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None
-    ) -> List[
-        Tuple[
-            Optional[str],
-            List[str],
-            List[int],
-            Union[Hypothesis],
-        ]
-    ]:
-        """Inference
+            self.bias_k = self.bias_v = None
 
-        Args:
-            speech: Input speech data
-        Returns:
-            text, token, token_int, hyp
+        self.add_zero_attn = add_zero_attn
 
-        """
-        assert check_argument_types()
-        # Input as audio signal
-        if isinstance(speech, np.ndarray):
-            speech = torch.tensor(speech)
-        if(speech.dim()==3):
-            speech = torch.squeeze(speech, 2)
-        #speech = speech.unsqueeze(0).to(getattr(torch, self.dtype))
-        speech = speech.to(getattr(torch, self.dtype))
-        # lenghts: (1,)
-        lengths = speech.new_full([1], dtype=torch.long, fill_value=speech.size(1))
-        batch = {"speech": speech, "speech_lengths": lengths}
-
-        # a. To device
-        batch = to_device(batch, device=self.device)
-        
-        # b. Forward Encoder
-        enc, _ = self.asr_model.encode(**batch)
-        
-        assert len(enc) == 1, len(enc)
-
-        # c. Passed the encoder result and the beam search
-        nbest_hyps = self.beam_search(
-            x=enc[0], maxlenratio=self.maxlenratio, minlenratio=self.minlenratio
+        self.reset_parameters()
+
+        self.onnx_trace = False
+        self.skip_embed_dim_check = False
+
+    def prepare_for_onnx_export_(self):
+        self.onnx_trace = True
+
+    def reset_parameters(self):
+        if self.qkv_same_dim:
+            # Empirically observed the convergence to be much better with
+            # the scaled initialization
+            nn.init.xavier_uniform_(self.k_proj.weight, gain=1 / math.sqrt(2))
+            nn.init.xavier_uniform_(self.v_proj.weight, gain=1 / math.sqrt(2))
+            nn.init.xavier_uniform_(self.q_proj.weight, gain=1 / math.sqrt(2))
+        else:
+            nn.init.xavier_uniform_(self.k_proj.weight)
+            nn.init.xavier_uniform_(self.v_proj.weight)
+            nn.init.xavier_uniform_(self.q_proj.weight)
+
+        nn.init.xavier_uniform_(self.out_proj.weight)
+        if self.out_proj.bias is not None:
+            nn.init.constant_(self.out_proj.bias, 0.0)
+        if self.bias_k is not None:
+            nn.init.xavier_normal_(self.bias_k)
+        if self.bias_v is not None:
+            nn.init.xavier_normal_(self.bias_v)
+
+    def _get_reserve_head_index(self, num_heads_to_keep: int):
+        k_proj_heads_norm = []
+        q_proj_heads_norm = []
+        v_proj_heads_norm = []
+
+        for i in range(self.num_heads):
+            start_idx = i * self.head_dim
+            end_idx = (i + 1) * self.head_dim
+            k_proj_heads_norm.append(
+                torch.sum(
+                    torch.abs(
+                        self.k_proj.weight[
+                        start_idx:end_idx,
+                        ]
+                    )
+                ).tolist()
+                + torch.sum(torch.abs(self.k_proj.bias[start_idx:end_idx])).tolist()
+            )
+            q_proj_heads_norm.append(
+                torch.sum(
+                    torch.abs(
+                        self.q_proj.weight[
+                        start_idx:end_idx,
+                        ]
+                    )
+                ).tolist()
+                + torch.sum(torch.abs(self.q_proj.bias[start_idx:end_idx])).tolist()
+            )
+            v_proj_heads_norm.append(
+                torch.sum(
+                    torch.abs(
+                        self.v_proj.weight[
+                        start_idx:end_idx,
+                        ]
+                    )
+                ).tolist()
+                + torch.sum(torch.abs(self.v_proj.bias[start_idx:end_idx])).tolist()
+            )
+
+        heads_norm = []
+        for i in range(self.num_heads):
+            heads_norm.append(
+                k_proj_heads_norm[i] + q_proj_heads_norm[i] + v_proj_heads_norm[i]
+            )
+
+        sorted_head_index = sorted(
+            range(self.num_heads), key=lambda k: heads_norm[k], reverse=True
         )
-        
-        nbest_hyps = nbest_hyps[: self.nbest]
-        
-        results = []
-        for hyp in nbest_hyps:
-            assert isinstance(hyp, (Hypothesis)), type(hyp)
-
-            # remove sos/eos and get results
-            last_pos = -1
-            if isinstance(hyp.yseq, list):
-                token_int = hyp.yseq[1:last_pos]
-            else:
-                token_int = hyp.yseq[1:last_pos].tolist()
+        reserve_head_index = []
+        for i in range(num_heads_to_keep):
+            start = sorted_head_index[i] * self.head_dim
+            end = (sorted_head_index[i] + 1) * self.head_dim
+            reserve_head_index.append((start, end))
+        return reserve_head_index
+
+    def _adaptive_prune_heads(self, reserve_head_index: List[Tuple[int, int]]):
+        new_q_weight = []
+        new_q_bias = []
+        new_k_weight = []
+        new_k_bias = []
+        new_v_weight = []
+        new_v_bias = []
+        new_out_proj_weight = []
+
+        for ele in reserve_head_index:
+            start_idx, end_idx = ele
+            new_q_weight.append(
+                self.q_proj.weight[
+                start_idx:end_idx,
+                ]
+            )
+            new_q_bias.append(self.q_proj.bias[start_idx:end_idx])
 
-            # remove blank symbol id, which is assumed to be 0
-            token_int = list(filter(lambda x: x != 0, token_int))
+            new_k_weight.append(
+                self.k_proj.weight[
+                start_idx:end_idx,
+                ]
+            )
 
-            # Change integer-ids to tokens
-            token = self.converter.ids2tokens(token_int)
+            new_k_bias.append(self.k_proj.bias[start_idx:end_idx])
 
-            if self.tokenizer is not None:
-                text = self.tokenizer.tokens2text(token)
-            else:
-                text = None
-            results.append((text, token, token_int, hyp))
+            new_v_weight.append(
+                self.v_proj.weight[
+                start_idx:end_idx,
+                ]
+            )
+            new_v_bias.append(self.v_proj.bias[start_idx:end_idx])
 
-        assert check_return_type(results)
-        return results
+            new_out_proj_weight.append(self.out_proj.weight[:, start_idx:end_idx])
 
+        new_q_weight = torch.cat(new_q_weight).detach()
+        new_k_weight = torch.cat(new_k_weight).detach()
+        new_v_weight = torch.cat(new_v_weight).detach()
+        new_out_proj_weight = torch.cat(new_out_proj_weight, dim=-1).detach()
+        new_q_weight.requires_grad = True
+        new_k_weight.requires_grad = True
+        new_v_weight.requires_grad = True
+        new_out_proj_weight.requires_grad = True
 
-# def inference(
-#         maxlenratio: float,
-#         minlenratio: float,
-#         batch_size: int,
-#         beam_size: int,
-#         ngpu: int,
-#         ctc_weight: float,
-#         lm_weight: float,
-#         penalty: float,
-#         log_level: Union[int, str],
-#         data_path_and_name_and_type,
-#         asr_train_config: Optional[str],
-#         asr_model_file: Optional[str],
-#         cmvn_file: Optional[str] = None,
-#         lm_train_config: Optional[str] = None,
-#         lm_file: Optional[str] = None,
-#         token_type: Optional[str] = None,
-#         key_file: Optional[str] = None,
-#         word_lm_train_config: Optional[str] = None,
-#         bpemodel: Optional[str] = None,
-#         allow_variable_data_keys: bool = False,
-#         streaming: bool = False,
-#         output_dir: Optional[str] = None,
-#         dtype: str = "float32",
-#         seed: int = 0,
-#         ngram_weight: float = 0.9,
-#         nbest: int = 1,
-#         num_workers: int = 1,
-#         **kwargs,
-# ):
-#     assert check_argument_types()
-#     if batch_size > 1:
-#         raise NotImplementedError("batch decoding is not implemented")
-#     if word_lm_train_config is not None:
-#         raise NotImplementedError("Word LM is not implemented")
-#     if ngpu > 1:
-#         raise NotImplementedError("only single GPU decoding is supported")
-#
-#     logging.basicConfig(
-#         level=log_level,
-#         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
-#     )
-#
-#     if ngpu >= 1 and torch.cuda.is_available():
-#         device = "cuda"
-#     else:
-#         device = "cpu"
-#
-#     # 1. Set random-seed
-#     set_all_random_seed(seed)
-#
-#     # 2. Build speech2text
-#     speech2text_kwargs = dict(
-#         asr_train_config=asr_train_config,
-#         asr_model_file=asr_model_file,
-#         cmvn_file=cmvn_file,
-#         lm_train_config=lm_train_config,
-#         lm_file=lm_file,
-#         token_type=token_type,
-#         bpemodel=bpemodel,
-#         device=device,
-#         maxlenratio=maxlenratio,
-#         minlenratio=minlenratio,
-#         dtype=dtype,
-#         beam_size=beam_size,
-#         ctc_weight=ctc_weight,
-#         lm_weight=lm_weight,
-#         ngram_weight=ngram_weight,
-#         penalty=penalty,
-#         nbest=nbest,
-#         streaming=streaming,
-#     )
-#     logging.info("speech2text_kwargs: {}".format(speech2text_kwargs))
-#     speech2text = Speech2Text(**speech2text_kwargs)
-#
-#     # 3. Build data-iterator
-#     loader = ASRTask.build_streaming_iterator(
-#         data_path_and_name_and_type,
-#         dtype=dtype,
-#         batch_size=batch_size,
-#         key_file=key_file,
-#         num_workers=num_workers,
-#         preprocess_fn=ASRTask.build_preprocess_fn(speech2text.asr_train_args, False),
-#         collate_fn=ASRTask.build_collate_fn(speech2text.asr_train_args, False),
-#         allow_variable_data_keys=allow_variable_data_keys,
-#         inference=True,
-#     )
-#
-#     finish_count = 0
-#     file_count = 1
-#     # 7 .Start for-loop
-#     # FIXME(kamo): The output format should be discussed about
-#     asr_result_list = []
-#     if output_dir is not None:
-#         writer = DatadirWriter(output_dir)
-#     else:
-#         writer = None
-#
-#     for keys, batch in loader:
-#         assert isinstance(batch, dict), type(batch)
-#         assert all(isinstance(s, str) for s in keys), keys
-#         _bs = len(next(iter(batch.values())))
-#         assert len(keys) == _bs, f"{len(keys)} != {_bs}"
-#         #batch = {k: v[0] for k, v in batch.items() if not k.endswith("_lengths")}
-#
-#         # N-best list of (text, token, token_int, hyp_object)
-#         try:
-#             results = speech2text(**batch)
-#         except TooShortUttError as e:
-#             logging.warning(f"Utterance {keys} {e}")
-#             hyp = Hypothesis(score=0.0, scores={}, states={}, yseq=[])
-#             results = [[" ", ["<space>"], [2], hyp]] * nbest
-#
-#         # Only supporting batch_size==1
-#         key = keys[0]
-#         for n, (text, token, token_int, hyp) in zip(range(1, nbest + 1), results):
-#             # Create a directory: outdir/{n}best_recog
-#             if writer is not None:
-#                 ibest_writer = writer[f"{n}best_recog"]
-#
-#                 # Write the result to each file
-#                 ibest_writer["token"][key] = " ".join(token)
-#                 ibest_writer["token_int"][key] = " ".join(map(str, token_int))
-#                 ibest_writer["score"][key] = str(hyp.score)
-#
-#             if text is not None:
-#                 text_postprocessed = postprocess_utils.sentence_postprocess(token)
-#                 item = {'key': key, 'value': text_postprocessed}
-#                 asr_result_list.append(item)
-#                 finish_count += 1
-#                 asr_utils.print_progress(finish_count / file_count)
-#                 if writer is not None:
-#                     ibest_writer["text"][key] = text
-#     return asr_result_list
-
-def inference(
-        maxlenratio: float,
-        minlenratio: float,
-        batch_size: int,
-        beam_size: int,
-        ngpu: int,
-        ctc_weight: float,
-        lm_weight: float,
-        penalty: float,
-        log_level: Union[int, str],
-        data_path_and_name_and_type,
-        asr_train_config: Optional[str],
-        asr_model_file: Optional[str],
-        cmvn_file: Optional[str] = None,
-        raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-        lm_train_config: Optional[str] = None,
-        lm_file: Optional[str] = None,
-        token_type: Optional[str] = None,
-        key_file: Optional[str] = None,
-        word_lm_train_config: Optional[str] = None,
-        bpemodel: Optional[str] = None,
-        allow_variable_data_keys: bool = False,
-        streaming: bool = False,
-        output_dir: Optional[str] = None,
-        dtype: str = "float32",
-        seed: int = 0,
-        ngram_weight: float = 0.9,
-        nbest: int = 1,
-        num_workers: int = 1,
-        **kwargs,
-):
-    inference_pipeline = inference_modelscope(
-        maxlenratio=maxlenratio,
-        minlenratio=minlenratio,
-        batch_size=batch_size,
-        beam_size=beam_size,
-        ngpu=ngpu,
-        ctc_weight=ctc_weight,
-        lm_weight=lm_weight,
-        penalty=penalty,
-        log_level=log_level,
-        asr_train_config=asr_train_config,
-        asr_model_file=asr_model_file,
-        cmvn_file=cmvn_file,
-        raw_inputs=raw_inputs,
-        lm_train_config=lm_train_config,
-        lm_file=lm_file,
-        token_type=token_type,
-        key_file=key_file,
-        word_lm_train_config=word_lm_train_config,
-        bpemodel=bpemodel,
-        allow_variable_data_keys=allow_variable_data_keys,
-        streaming=streaming,
-        output_dir=output_dir,
-        dtype=dtype,
-        seed=seed,
-        ngram_weight=ngram_weight,
-        nbest=nbest,
-        num_workers=num_workers,
-        **kwargs,
-    )
-    return inference_pipeline(data_path_and_name_and_type, raw_inputs)
-
-def inference_modelscope(
-    maxlenratio: float,
-    minlenratio: float,
-    batch_size: int,
-    beam_size: int,
-    ngpu: int,
-    ctc_weight: float,
-    lm_weight: float,
-    penalty: float,
-    log_level: Union[int, str],
-    # data_path_and_name_and_type,
-    asr_train_config: Optional[str],
-    asr_model_file: Optional[str],
-    cmvn_file: Optional[str] = None,
-    lm_train_config: Optional[str] = None,
-    lm_file: Optional[str] = None,
-    token_type: Optional[str] = None,
-    key_file: Optional[str] = None,
-    word_lm_train_config: Optional[str] = None,
-    bpemodel: Optional[str] = None,
-    allow_variable_data_keys: bool = False,
-    streaming: bool = False,
-    output_dir: Optional[str] = None,
-    dtype: str = "float32",
-    seed: int = 0,
-    ngram_weight: float = 0.9,
-    nbest: int = 1,
-    num_workers: int = 1,
-    param_dict: dict = None,
-    **kwargs,
-):
-    assert check_argument_types()
-    ncpu = kwargs.get("ncpu", 1)
-    torch.set_num_threads(ncpu)
-    if batch_size > 1:
-        raise NotImplementedError("batch decoding is not implemented")
-    if word_lm_train_config is not None:
-        raise NotImplementedError("Word LM is not implemented")
-    if ngpu > 1:
-        raise NotImplementedError("only single GPU decoding is supported")
-    
-    logging.basicConfig(
-        level=log_level,
-        format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
-    )
-    
-    if ngpu >= 1 and torch.cuda.is_available():
-        device = "cuda"
-    else:
-        device = "cpu"
-    
-    # 1. Set random-seed
-    set_all_random_seed(seed)
-    
-    # 2. Build speech2text
-    speech2text_kwargs = dict(
-        asr_train_config=asr_train_config,
-        asr_model_file=asr_model_file,
-        cmvn_file=cmvn_file,
-        lm_train_config=lm_train_config,
-        lm_file=lm_file,
-        token_type=token_type,
-        bpemodel=bpemodel,
-        device=device,
-        maxlenratio=maxlenratio,
-        minlenratio=minlenratio,
-        dtype=dtype,
-        beam_size=beam_size,
-        ctc_weight=ctc_weight,
-        lm_weight=lm_weight,
-        ngram_weight=ngram_weight,
-        penalty=penalty,
-        nbest=nbest,
-        streaming=streaming,
-    )
-    logging.info("speech2text_kwargs: {}".format(speech2text_kwargs))
-    speech2text = Speech2Text(**speech2text_kwargs)
-    
-    def _forward(data_path_and_name_and_type,
-                 raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-                 output_dir_v2: Optional[str] = None,
-                 fs: dict = None,
-                 param_dict: dict = None,
-                 **kwargs,
-                 ):
-        # 3. Build data-iterator
-        if data_path_and_name_and_type is None and raw_inputs is not None:
-            if isinstance(raw_inputs, torch.Tensor):
-                raw_inputs = raw_inputs.numpy()
-            data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
-        loader = ASRTask.build_streaming_iterator(
-            data_path_and_name_and_type,
-            dtype=dtype,
-            batch_size=batch_size,
-            fs=fs,
-            mc=True,
-            key_file=key_file,
-            num_workers=num_workers,
-            preprocess_fn=ASRTask.build_preprocess_fn(speech2text.asr_train_args, False),
-            collate_fn=ASRTask.build_collate_fn(speech2text.asr_train_args, False),
-            allow_variable_data_keys=allow_variable_data_keys,
-            inference=True,
+        new_q_bias = torch.cat(new_q_bias).detach()
+        new_q_bias.requires_grad = True
+
+        new_k_bias = torch.cat(new_k_bias).detach()
+        new_k_bias.requires_grad = True
+
+        new_v_bias = torch.cat(new_v_bias).detach()
+        new_v_bias.requires_grad = True
+
+        self.q_proj.weight = torch.nn.Parameter(new_q_weight)
+        self.q_proj.bias = torch.nn.Parameter(new_q_bias)
+
+        self.k_proj.weight = torch.nn.Parameter(new_k_weight)
+        self.k_proj.bias = torch.nn.Parameter(new_k_bias)
+
+        self.v_proj.weight = torch.nn.Parameter(new_v_weight)
+        self.v_proj.bias = torch.nn.Parameter(new_v_bias)
+
+        self.out_proj.weight = torch.nn.Parameter(new_out_proj_weight)
+
+        self.num_heads = len(reserve_head_index)
+        self.embed_dim = self.head_dim * self.num_heads
+        self.q_proj.out_features = self.embed_dim
+        self.k_proj.out_features = self.embed_dim
+        self.v_proj.out_features = self.embed_dim
+
+    def _set_skip_embed_dim_check(self):
+        self.skip_embed_dim_check = True
+
+    def forward(
+            self,
+            query,
+            key: Optional[Tensor],
+            value: Optional[Tensor],
+            key_padding_mask: Optional[Tensor] = None,
+            incremental_state: Optional[Dict[str, Dict[str, Optional[Tensor]]]] = None,
+            need_weights: bool = True,
+            static_kv: bool = False,
+            attn_mask: Optional[Tensor] = None,
+            before_softmax: bool = False,
+            need_head_weights: bool = False,
+    ) -> Tuple[Tensor, Optional[Tensor]]:
+        """Input shape: Time x Batch x Channel
+
+        Args:
+            key_padding_mask (ByteTensor, optional): mask to exclude
+                keys that are pads, of shape `(batch, src_len)`, where
+                padding elements are indicated by 1s.
+            need_weights (bool, optional): return the attention weights,
+                averaged over heads (default: False).
+            attn_mask (ByteTensor, optional): typically used to
+                implement causal attention, where the mask prevents the
+                attention from looking forward in time (default: None).
+            before_softmax (bool, optional): return the raw attention
+                weights and values before the attention softmax.
+            need_head_weights (bool, optional): return the attention
+                weights for each head. Implies *need_weights*. Default:
+                return the average attention weights over all heads.
+        """
+        if need_head_weights:
+            need_weights = True
+
+        is_tpu = query.device.type == "xla"
+
+        tgt_len, bsz, embed_dim = query.size()
+        src_len = tgt_len
+        if not self.skip_embed_dim_check:
+            assert (
+                    embed_dim == self.embed_dim
+            ), f"query dim {embed_dim} != {self.embed_dim}"
+        assert list(query.size()) == [tgt_len, bsz, embed_dim]
+        if key is not None:
+            src_len, key_bsz, _ = key.size()
+            if not torch.jit.is_scripting():
+                assert key_bsz == bsz
+                assert value is not None
+                assert src_len, bsz == value.shape[:2]
+
+        if (
+                not self.onnx_trace
+                and not is_tpu  # don't use PyTorch version on TPUs
+                and incremental_state is None
+                and not static_kv
+                # A workaround for quantization to work. Otherwise JIT compilation
+                # treats bias in linear module as method.
+                and not torch.jit.is_scripting()
+                # The Multihead attention implemented in pytorch forces strong dimension check
+                # for input embedding dimention and K,Q,V projection dimension.
+                # Since pruning will break the dimension check and it is not easy to modify the pytorch API,
+                # it is preferred to bypass the pytorch MHA when we need to skip embed_dim_check
+                and not self.skip_embed_dim_check
+        ):
+            assert key is not None and value is not None
+            return F.multi_head_attention_forward(
+                query,
+                key,
+                value,
+                self.embed_dim,
+                self.num_heads,
+                torch.empty([0]),
+                torch.cat((self.q_proj.bias, self.k_proj.bias, self.v_proj.bias)),
+                self.bias_k,
+                self.bias_v,
+                self.add_zero_attn,
+                self.dropout_module.p,
+                self.out_proj.weight,
+                self.out_proj.bias,
+                self.training or self.dropout_module.apply_during_inference,
+                key_padding_mask,
+                need_weights,
+                attn_mask,
+                use_separate_proj_weight=True,
+                q_proj_weight=self.q_proj.weight,
+                k_proj_weight=self.k_proj.weight,
+                v_proj_weight=self.v_proj.weight,
+            )
+
+        if incremental_state is not None:
+            saved_state = self._get_input_buffer(incremental_state)
+            if saved_state is not None and "prev_key" in saved_state:
+                # previous time steps are cached - no need to recompute
+                # key and value if they are static
+                if static_kv:
+                    assert self.encoder_decoder_attention and not self.self_attention
+                    key = value = None
+        else:
+            saved_state = None
+
+        if self.self_attention:
+            q = self.q_proj(query)
+            k = self.k_proj(query)
+            v = self.v_proj(query)
+        elif self.encoder_decoder_attention:
+            # encoder-decoder attention
+            q = self.q_proj(query)
+            if key is None:
+                assert value is None
+                k = v = None
+            else:
+                k = self.k_proj(key)
+                v = self.v_proj(key)
+
+        else:
+            assert key is not None and value is not None
+            q = self.q_proj(query)
+            k = self.k_proj(key)
+            v = self.v_proj(value)
+        q *= self.scaling
+
+        if self.bias_k is not None:
+            assert self.bias_v is not None
+            k = torch.cat([k, self.bias_k.repeat(1, bsz, 1)])
+            v = torch.cat([v, self.bias_v.repeat(1, bsz, 1)])
+            if attn_mask is not None:
+                attn_mask = torch.cat(
+                    [attn_mask, attn_mask.new_zeros(attn_mask.size(0), 1)], dim=1
+                )
+            if key_padding_mask is not None:
+                key_padding_mask = torch.cat(
+                    [
+                        key_padding_mask,
+                        key_padding_mask.new_zeros(key_padding_mask.size(0), 1),
+                    ],
+                    dim=1,
+                )
+
+        q = (
+            q.contiguous()
+                .view(tgt_len, bsz * self.num_heads, self.head_dim)
+                .transpose(0, 1)
         )
-        
-        finish_count = 0
-        file_count = 1
-        # 7 .Start for-loop
-        # FIXME(kamo): The output format should be discussed about
-        asr_result_list = []
-        output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
-        if output_path is not None:
-            writer = DatadirWriter(output_path)
+        if k is not None:
+            k = (
+                k.contiguous()
+                    .view(-1, bsz * self.num_heads, self.head_dim)
+                    .transpose(0, 1)
+            )
+        if v is not None:
+            v = (
+                v.contiguous()
+                    .view(-1, bsz * self.num_heads, self.head_dim)
+                    .transpose(0, 1)
+            )
+
+        if saved_state is not None:
+            # saved states are stored with shape (bsz, num_heads, seq_len, head_dim)
+            if "prev_key" in saved_state:
+                _prev_key = saved_state["prev_key"]
+                assert _prev_key is not None
+                prev_key = _prev_key.view(bsz * self.num_heads, -1, self.head_dim)
+                if static_kv:
+                    k = prev_key
+                else:
+                    assert k is not None
+                    k = torch.cat([prev_key, k], dim=1)
+                src_len = k.size(1)
+            if "prev_value" in saved_state:
+                _prev_value = saved_state["prev_value"]
+                assert _prev_value is not None
+                prev_value = _prev_value.view(bsz * self.num_heads, -1, self.head_dim)
+                if static_kv:
+                    v = prev_value
+                else:
+                    assert v is not None
+                    v = torch.cat([prev_value, v], dim=1)
+            prev_key_padding_mask: Optional[Tensor] = None
+            if "prev_key_padding_mask" in saved_state:
+                prev_key_padding_mask = saved_state["prev_key_padding_mask"]
+            assert k is not None and v is not None
+            key_padding_mask = MultiheadAttention._append_prev_key_padding_mask(
+                key_padding_mask=key_padding_mask,
+                prev_key_padding_mask=prev_key_padding_mask,
+                batch_size=bsz,
+                src_len=k.size(1),
+                static_kv=static_kv,
+            )
+
+            saved_state["prev_key"] = k.view(bsz, self.num_heads, -1, self.head_dim)
+            saved_state["prev_value"] = v.view(bsz, self.num_heads, -1, self.head_dim)
+            saved_state["prev_key_padding_mask"] = key_padding_mask
+            # In this branch incremental_state is never None
+            assert incremental_state is not None
+            incremental_state = self._set_input_buffer(incremental_state, saved_state)
+        assert k is not None
+        assert k.size(1) == src_len
+
+        # This is part of a workaround to get around fork/join parallelism
+        # not supporting Optional types.
+        if key_padding_mask is not None and key_padding_mask.dim() == 0:
+            key_padding_mask = None
+
+        if key_padding_mask is not None:
+            assert key_padding_mask.size(0) == bsz
+            assert key_padding_mask.size(1) == src_len
+
+        if self.add_zero_attn:
+            assert v is not None
+            src_len += 1
+            k = torch.cat([k, k.new_zeros((k.size(0), 1) + k.size()[2:])], dim=1)
+            v = torch.cat([v, v.new_zeros((v.size(0), 1) + v.size()[2:])], dim=1)
+            if attn_mask is not None:
+                attn_mask = torch.cat(
+                    [attn_mask, attn_mask.new_zeros(attn_mask.size(0), 1)], dim=1
+                )
+            if key_padding_mask is not None:
+                key_padding_mask = torch.cat(
+                    [
+                        key_padding_mask,
+                        torch.zeros(key_padding_mask.size(0), 1).type_as(
+                            key_padding_mask
+                        ),
+                    ],
+                    dim=1,
+                )
+
+        attn_weights = torch.bmm(q, k.transpose(1, 2))
+        attn_weights = self.apply_sparse_mask(attn_weights, tgt_len, src_len, bsz)
+
+        assert list(attn_weights.size()) == [bsz * self.num_heads, tgt_len, src_len]
+
+        if attn_mask is not None:
+            attn_mask = attn_mask.unsqueeze(0)
+            if self.onnx_trace:
+                attn_mask = attn_mask.repeat(attn_weights.size(0), 1, 1)
+            attn_weights += attn_mask
+
+        if key_padding_mask is not None:
+            # don't attend to padding symbols
+            attn_weights = attn_weights.view(bsz, self.num_heads, tgt_len, src_len)
+            if not is_tpu:
+                attn_weights = attn_weights.masked_fill(
+                    key_padding_mask.unsqueeze(1).unsqueeze(2).to(torch.bool),
+                    float("-inf"),
+                )
+            else:
+                attn_weights = attn_weights.transpose(0, 2)
+                attn_weights = attn_weights.masked_fill(key_padding_mask, float("-inf"))
+                attn_weights = attn_weights.transpose(0, 2)
+            attn_weights = attn_weights.view(bsz * self.num_heads, tgt_len, src_len)
+
+        if before_softmax:
+            return attn_weights, v
+
+        attn_weights_float = F.softmax(attn_weights, dim=-1, dtype=torch.float32)
+        attn_weights = attn_weights_float.type_as(attn_weights)
+        attn_probs = self.dropout_module(attn_weights)
+
+        assert v is not None
+        attn = torch.bmm(attn_probs, v)
+        assert list(attn.size()) == [bsz * self.num_heads, tgt_len, self.head_dim]
+        if self.onnx_trace and attn.size(1) == 1:
+            # when ONNX tracing a single decoder step (sequence length == 1)
+            # the transpose is a no-op copy before view, thus unnecessary
+            attn = attn.contiguous().view(tgt_len, bsz, self.embed_dim)
+        else:
+            attn = attn.transpose(0, 1).contiguous().view(tgt_len, bsz, self.embed_dim)
+        attn = self.out_proj(attn)
+        attn_weights: Optional[Tensor] = None
+        if need_weights:
+            attn_weights = attn_weights_float.view(
+                bsz, self.num_heads, tgt_len, src_len
+            ).transpose(1, 0)
+            if not need_head_weights:
+                # average attention weights over heads
+                attn_weights = attn_weights.mean(dim=0)
+
+        return attn, attn_weights
+
+    @staticmethod
+    def _append_prev_key_padding_mask(
+            key_padding_mask: Optional[Tensor],
+            prev_key_padding_mask: Optional[Tensor],
+            batch_size: int,
+            src_len: int,
+            static_kv: bool,
+    ) -> Optional[Tensor]:
+        # saved key padding masks have shape (bsz, seq_len)
+        if prev_key_padding_mask is not None and static_kv:
+            new_key_padding_mask = prev_key_padding_mask
+        elif prev_key_padding_mask is not None and key_padding_mask is not None:
+            new_key_padding_mask = torch.cat(
+                [prev_key_padding_mask.float(), key_padding_mask.float()], dim=1
+            )
+        # During incremental decoding, as the padding token enters and
+        # leaves the frame, there will be a time when prev or current
+        # is None
+        elif prev_key_padding_mask is not None:
+            if src_len > prev_key_padding_mask.size(1):
+                filler = torch.zeros(
+                    (batch_size, src_len - prev_key_padding_mask.size(1)),
+                    device=prev_key_padding_mask.device,
+                )
+                new_key_padding_mask = torch.cat(
+                    [prev_key_padding_mask.float(), filler.float()], dim=1
+                )
+            else:
+                new_key_padding_mask = prev_key_padding_mask.float()
+        elif key_padding_mask is not None:
+            if src_len > key_padding_mask.size(1):
+                filler = torch.zeros(
+                    (batch_size, src_len - key_padding_mask.size(1)),
+                    device=key_padding_mask.device,
+                )
+                new_key_padding_mask = torch.cat(
+                    [filler.float(), key_padding_mask.float()], dim=1
+                )
+            else:
+                new_key_padding_mask = key_padding_mask.float()
         else:
-            writer = None
-        
-        for keys, batch in loader:
-            assert isinstance(batch, dict), type(batch)
-            assert all(isinstance(s, str) for s in keys), keys
-            _bs = len(next(iter(batch.values())))
-            assert len(keys) == _bs, f"{len(keys)} != {_bs}"
-            # batch = {k: v[0] for k, v in batch.items() if not k.endswith("_lengths")}
-            
-            # N-best list of (text, token, token_int, hyp_object)
-            try:
-                results = speech2text(**batch)
-            except TooShortUttError as e:
-                logging.warning(f"Utterance {keys} {e}")
-                hyp = Hypothesis(score=0.0, scores={}, states={}, yseq=[])
-                results = [[" ", ["<space>"], [2], hyp]] * nbest
-            
-            # Only supporting batch_size==1
-            key = keys[0]
-            for n, (text, token, token_int, hyp) in zip(range(1, nbest + 1), results):
-                # Create a directory: outdir/{n}best_recog
-                if writer is not None:
-                    ibest_writer = writer[f"{n}best_recog"]
-                    
-                    # Write the result to each file
-                    ibest_writer["token"][key] = " ".join(token)
-                    # ibest_writer["token_int"][key] = " ".join(map(str, token_int))
-                    ibest_writer["score"][key] = str(hyp.score)
-                
-                if text is not None:
-                    text_postprocessed = postprocess_utils.sentence_postprocess(token)
-                    item = {'key': key, 'value': text_postprocessed}
-                    asr_result_list.append(item)
-                    finish_count += 1
-                    asr_utils.print_progress(finish_count / file_count)
-                    if writer is not None:
-                        ibest_writer["text"][key] = text
-        return asr_result_list
-    
-    return _forward
-
-def get_parser():
-    parser = config_argparse.ArgumentParser(
-        description="ASR Decoding",
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-    )
-
-    # Note(kamo): Use '_' instead of '-' as separator.
-    # '-' is confusing if written in yaml.
-    parser.add_argument(
-        "--log_level",
-        type=lambda x: x.upper(),
-        default="INFO",
-        choices=("CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET"),
-        help="The verbose level of logging",
-    )
-
-    parser.add_argument("--output_dir", type=str, required=True)
-    parser.add_argument(
-        "--ngpu",
-        type=int,
-        default=0,
-        help="The number of gpus. 0 indicates CPU mode",
-    )
-    parser.add_argument(
-        "--gpuid_list",
-        type=str,
-        default="",
-        help="The visible gpus",
-    )
-    parser.add_argument("--seed", type=int, default=0, help="Random seed")
-    parser.add_argument(
-        "--dtype",
-        default="float32",
-        choices=["float16", "float32", "float64"],
-        help="Data type",
-    )
-    parser.add_argument(
-        "--num_workers",
-        type=int,
-        default=1,
-        help="The number of workers used for DataLoader",
-    )
-
-    group = parser.add_argument_group("Input data related")
-    group.add_argument(
-        "--data_path_and_name_and_type",
-        type=str2triple_str,
-        required=False,
-        action="append",
-    )
-    group.add_argument("--raw_inputs", type=list, default=None)
-    # example=[{'key':'EdevDEWdIYQ_0021','file':'/mnt/data/jiangyu.xzy/test_data/speech_io/SPEECHIO_ASR_ZH00007_zhibodaihuo/wav/EdevDEWdIYQ_0021.wav'}])
-    group.add_argument("--key_file", type=str_or_none)
-    group.add_argument("--allow_variable_data_keys", type=str2bool, default=False)
-
-    group = parser.add_argument_group("The model configuration related")
-    group.add_argument(
-        "--asr_train_config",
-        type=str,
-        help="ASR training configuration",
-    )
-    group.add_argument(
-        "--asr_model_file",
-        type=str,
-        help="ASR model parameter file",
-    )
-    group.add_argument(
-        "--cmvn_file",
-        type=str,
-        help="Global cmvn file",
-    )
-    group.add_argument(
-        "--lm_train_config",
-        type=str,
-        help="LM training configuration",
-    )
-    group.add_argument(
-        "--lm_file",
-        type=str,
-        help="LM parameter file",
-    )
-    group.add_argument(
-        "--word_lm_train_config",
-        type=str,
-        help="Word LM training configuration",
-    )
-    group.add_argument(
-        "--word_lm_file",
-        type=str,
-        help="Word LM parameter file",
-    )
-    group.add_argument(
-        "--ngram_file",
-        type=str,
-        help="N-gram parameter file",
-    )
-    group.add_argument(
-        "--model_tag",
-        type=str,
-        help="Pretrained model tag. If specify this option, *_train_config and "
-             "*_file will be overwritten",
-    )
-
-    group = parser.add_argument_group("Beam-search related")
-    group.add_argument(
-        "--batch_size",
-        type=int,
-        default=1,
-        help="The batch size for inference",
-    )
-    group.add_argument("--nbest", type=int, default=1, help="Output N-best hypotheses")
-    group.add_argument("--beam_size", type=int, default=20, help="Beam size")
-    group.add_argument("--penalty", type=float, default=0.0, help="Insertion penalty")
-    group.add_argument(
-        "--maxlenratio",
-        type=float,
-        default=0.0,
-        help="Input length ratio to obtain max output length. "
-             "If maxlenratio=0.0 (default), it uses a end-detect "
-             "function "
-             "to automatically find maximum hypothesis lengths."
-             "If maxlenratio<0.0, its absolute value is interpreted"
-             "as a constant max output length",
-    )
-    group.add_argument(
-        "--minlenratio",
-        type=float,
-        default=0.0,
-        help="Input length ratio to obtain min output length",
-    )
-    group.add_argument(
-        "--ctc_weight",
-        type=float,
-        default=0.5,
-        help="CTC weight in joint decoding",
-    )
-    group.add_argument("--lm_weight", type=float, default=1.0, help="RNNLM weight")
-    group.add_argument("--ngram_weight", type=float, default=0.9, help="ngram weight")
-    group.add_argument("--streaming", type=str2bool, default=False)
-
-    group = parser.add_argument_group("Text converter related")
-    group.add_argument(
-        "--token_type",
-        type=str_or_none,
-        default=None,
-        choices=["char", "bpe", None],
-        help="The token type for ASR model. "
-             "If not given, refers from the training args",
-    )
-    group.add_argument(
-        "--bpemodel",
-        type=str_or_none,
-        default=None,
-        help="The model path of sentencepiece. "
-             "If not given, refers from the training args",
-    )
-
-    return parser
-
-
-def main(cmd=None):
-    print(get_commandline_args(), file=sys.stderr)
-    parser = get_parser()
-    args = parser.parse_args(cmd)
-    kwargs = vars(args)
-    kwargs.pop("config", None)
-    inference(**kwargs)
+            new_key_padding_mask = prev_key_padding_mask
+        return new_key_padding_mask
+
+    @torch.jit.export
+    def reorder_incremental_state(
+            self,
+            incremental_state: Dict[str, Dict[str, Optional[Tensor]]],
+            new_order: Tensor,
+    ):
+        """Reorder buffered internal state (for incremental generation)."""
+        input_buffer = self._get_input_buffer(incremental_state)
+        if input_buffer is not None:
+            for k in input_buffer.keys():
+                input_buffer_k = input_buffer[k]
+                if input_buffer_k is not None:
+                    if self.encoder_decoder_attention and input_buffer_k.size(
+                            0
+                    ) == new_order.size(0):
+                        break
+                    input_buffer[k] = input_buffer_k.index_select(0, new_order)
+            incremental_state = self._set_input_buffer(incremental_state, input_buffer)
+        return incremental_state
+
+    def _get_input_buffer(
+            self, incremental_state: Optional[Dict[str, Dict[str, Optional[Tensor]]]]
+    ) -> Dict[str, Optional[Tensor]]:
+        result = self.get_incremental_state(incremental_state, "attn_state")
+        if result is not None:
+            return result
+        else:
+            empty_result: Dict[str, Optional[Tensor]] = {}
+            return empty_result
+
+    def _set_input_buffer(
+            self,
+            incremental_state: Dict[str, Dict[str, Optional[Tensor]]],
+            buffer: Dict[str, Optional[Tensor]],
+    ):
+        return self.set_incremental_state(incremental_state, "attn_state", buffer)
+
+    def apply_sparse_mask(self, attn_weights, tgt_len: int, src_len: int, bsz: int):
+        return attn_weights
+
+    def upgrade_state_dict_named(self, state_dict, name):
+        prefix = name + "." if name != "" else ""
+        items_to_add = {}
+        keys_to_remove = []
+        for k in state_dict.keys():
+            if k.endswith(prefix + "in_proj_weight"):
+                # in_proj_weight used to be q + k + v with same dimensions
+                dim = int(state_dict[k].shape[0] / 3)
+                items_to_add[prefix + "q_proj.weight"] = state_dict[k][:dim]
+                items_to_add[prefix + "k_proj.weight"] = state_dict[k][dim: 2 * dim]
+                items_to_add[prefix + "v_proj.weight"] = state_dict[k][2 * dim:]
+
+                keys_to_remove.append(k)
+
+                k_bias = prefix + "in_proj_bias"
+                if k_bias in state_dict.keys():
+                    dim = int(state_dict[k].shape[0] / 3)
+                    items_to_add[prefix + "q_proj.bias"] = state_dict[k_bias][:dim]
+                    items_to_add[prefix + "k_proj.bias"] = state_dict[k_bias][
+                                                           dim: 2 * dim
+                                                           ]
+                    items_to_add[prefix + "v_proj.bias"] = state_dict[k_bias][2 * dim:]
+
+                    keys_to_remove.append(prefix + "in_proj_bias")
 
+        for k in keys_to_remove:
+            del state_dict[k]
 
-if __name__ == "__main__":
-    main()
+        for key, value in items_to_add.items():
+            state_dict[key] = value
```

### Comparing `funasr-0.5.3/funasr/bin/asr_inference_paraformer_streaming.py` & `funasr-0.5.4/funasr/datasets/preprocessor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,749 +1,824 @@
-#!/usr/bin/env python3
-import argparse
-import logging
-import sys
-import time
-import copy
-import os
-import codecs
-import tempfile
-import requests
-import yaml
+import re
+from abc import ABC
+from abc import abstractmethod
 from pathlib import Path
-from typing import Optional
-from typing import Sequence
-from typing import Tuple
-from typing import Union
+from typing import Collection
 from typing import Dict
-from typing import Any
+from typing import Iterable
 from typing import List
+from typing import Union
 
 import numpy as np
-import torch
-import torchaudio
+import scipy.signal
+import soundfile
 from typeguard import check_argument_types
+from typeguard import check_return_type
 
-from funasr.fileio.datadir_writer import DatadirWriter
-from funasr.modules.beam_search.beam_search import BeamSearchPara as BeamSearch
-from funasr.modules.beam_search.beam_search import Hypothesis
-from funasr.modules.scorers.ctc import CTCPrefixScorer
-from funasr.modules.scorers.length_bonus import LengthBonus
-from funasr.modules.subsampling import TooShortUttError
-from funasr.tasks.asr import ASRTaskParaformer as ASRTask
-from funasr.tasks.lm import LMTask
 from funasr.text.build_tokenizer import build_tokenizer
+from funasr.text.cleaner import TextCleaner
 from funasr.text.token_id_converter import TokenIDConverter
-from funasr.torch_utils.device_funcs import to_device
-from funasr.torch_utils.set_all_random_seed import set_all_random_seed
-from funasr.utils import config_argparse
-from funasr.utils.cli_utils import get_commandline_args
-from funasr.utils.types import str2bool
-from funasr.utils.types import str2triple_str
-from funasr.utils.types import str_or_none
-from funasr.utils import asr_utils, wav_utils, postprocess_utils
-from funasr.models.frontend.wav_frontend import WavFrontend, WavFrontendOnline
-from funasr.export.models.e2e_asr_paraformer import Paraformer as Paraformer_export
-
-np.set_printoptions(threshold=np.inf)
-
-
-class Speech2Text:
-    """Speech2Text class
-
-    Examples:
-            >>> import soundfile
-            >>> speech2text = Speech2Text("asr_config.yml", "asr.pth")
-            >>> audio, rate = soundfile.read("speech.wav")
-            >>> speech2text(audio)
-            [(text, token, token_int, hypothesis object), ...]
 
+
+class AbsPreprocessor(ABC):
+    def __init__(self, train: bool):
+        self.train = train
+
+    @abstractmethod
+    def __call__(
+            self, uid: str, data: Dict[str, Union[str, np.ndarray]]
+    ) -> Dict[str, np.ndarray]:
+        raise NotImplementedError
+
+
+def forward_segment(text, dic):
+    word_list = []
+    i = 0
+    while i < len(text):
+        longest_word = text[i]
+        for j in range(i + 1, len(text) + 1):
+            word = text[i:j]
+            if word in dic:
+                if len(word) > len(longest_word):
+                    longest_word = word
+        word_list.append(longest_word)
+        i += len(longest_word)
+    return word_list
+
+def seg_tokenize(txt, seg_dict):
+    pattern = re.compile(r'^[\u4E00-\u9FA50-9]+$')
+    out_txt = ""
+    for word in txt:
+        word = word.lower()
+        if word in seg_dict:
+            out_txt += seg_dict[word] + " "
+        else:
+            if pattern.match(word):
+                for char in word:
+                    if char in seg_dict:
+                        out_txt += seg_dict[char] + " "
+                    else:
+                        out_txt += "<unk>" + " "
+            else:
+                out_txt += "<unk>" + " "
+    return out_txt.strip().split()
+
+def seg_tokenize_wo_pattern(txt, seg_dict):
+    out_txt = ""
+    for word in txt:
+        if word in seg_dict:
+            out_txt += seg_dict[word] + " "
+        else:
+            out_txt += "<unk>" + " "
+    return out_txt.strip().split()
+
+
+def framing(
+        x,
+        frame_length: int = 512,
+        frame_shift: int = 256,
+        centered: bool = True,
+        padded: bool = True,
+):
+    if x.size == 0:
+        raise ValueError("Input array size is zero")
+    if frame_length < 1:
+        raise ValueError("frame_length must be a positive integer")
+    if frame_length > x.shape[-1]:
+        raise ValueError("frame_length is greater than input length")
+    if 0 >= frame_shift:
+        raise ValueError("frame_shift must be greater than 0")
+
+    if centered:
+        pad_shape = [(0, 0) for _ in range(x.ndim - 1)] + [
+            (frame_length // 2, frame_length // 2)
+        ]
+        x = np.pad(x, pad_shape, mode="constant", constant_values=0)
+
+    if padded:
+        # Pad to integer number of windowed segments
+        # I.e make x.shape[-1] = frame_length + (nseg-1)*nstep,
+        #  with integer nseg
+        nadd = (-(x.shape[-1] - frame_length) % frame_shift) % frame_length
+        pad_shape = [(0, 0) for _ in range(x.ndim - 1)] + [(0, nadd)]
+        x = np.pad(x, pad_shape, mode="constant", constant_values=0)
+
+    # Created strided array of data segments
+    if frame_length == 1 and frame_length == frame_shift:
+        result = x[..., None]
+    else:
+        shape = x.shape[:-1] + (
+            (x.shape[-1] - frame_length) // frame_shift + 1,
+            frame_length,
+        )
+        strides = x.strides[:-1] + (frame_shift * x.strides[-1], x.strides[-1])
+        result = np.lib.stride_tricks.as_strided(x, shape=shape, strides=strides)
+    return result
+
+
+def detect_non_silence(
+        x: np.ndarray,
+        threshold: float = 0.01,
+        frame_length: int = 1024,
+        frame_shift: int = 512,
+        window: str = "boxcar",
+) -> np.ndarray:
+    """Power based voice activity detection.
+
+    Args:
+        x: (Channel, Time)
+    >>> x = np.random.randn(1000)
+    >>> detect = detect_non_silence(x)
+    >>> assert x.shape == detect.shape
+    >>> assert detect.dtype == np.bool
     """
+    if x.shape[-1] < frame_length:
+        return np.full(x.shape, fill_value=True, dtype=np.bool)
+
+    if x.dtype.kind == "i":
+        x = x.astype(np.float64)
+    # framed_w: (C, T, F)
+    framed_w = framing(
+        x,
+        frame_length=frame_length,
+        frame_shift=frame_shift,
+        centered=False,
+        padded=True,
+    )
+    framed_w *= scipy.signal.get_window(window, frame_length).astype(framed_w.dtype)
+    # power: (C, T)
+    power = (framed_w ** 2).mean(axis=-1)
+    # mean_power: (C, 1)
+    mean_power = np.mean(power, axis=-1, keepdims=True)
+    if np.all(mean_power == 0):
+        return np.full(x.shape, fill_value=True, dtype=np.bool)
+    # detect_frames: (C, T)
+    detect_frames = power / mean_power > threshold
+    # detects: (C, T, F)
+    detects = np.broadcast_to(
+        detect_frames[..., None], detect_frames.shape + (frame_shift,)
+    )
+    # detects: (C, TF)
+    detects = detects.reshape(*detect_frames.shape[:-1], -1)
+    # detects: (C, TF)
+    return np.pad(
+        detects,
+        [(0, 0)] * (x.ndim - 1) + [(0, x.shape[-1] - detects.shape[-1])],
+        mode="edge",
+    )
+
 
+class CommonPreprocessor(AbsPreprocessor):
     def __init__(
             self,
-            asr_train_config: Union[Path, str] = None,
-            asr_model_file: Union[Path, str] = None,
-            cmvn_file: Union[Path, str] = None,
-            lm_train_config: Union[Path, str] = None,
-            lm_file: Union[Path, str] = None,
+            train: bool,
             token_type: str = None,
-            bpemodel: str = None,
-            device: str = "cpu",
-            maxlenratio: float = 0.0,
-            minlenratio: float = 0.0,
-            dtype: str = "float32",
-            beam_size: int = 20,
-            ctc_weight: float = 0.5,
-            lm_weight: float = 1.0,
-            ngram_weight: float = 0.9,
-            penalty: float = 0.0,
-            nbest: int = 1,
-            frontend_conf: dict = None,
-            hotword_list_or_file: str = None,
-            **kwargs,
+            token_list: Union[Path, str, Iterable[str]] = None,
+            bpemodel: Union[Path, str, Iterable[str]] = None,
+            text_cleaner: Collection[str] = None,
+            g2p_type: str = None,
+            unk_symbol: str = "<unk>",
+            space_symbol: str = "<space>",
+            non_linguistic_symbols: Union[Path, str, Iterable[str]] = None,
+            delimiter: str = None,
+            rir_scp: str = None,
+            rir_apply_prob: float = 1.0,
+            noise_scp: str = None,
+            noise_apply_prob: float = 1.0,
+            noise_db_range: str = "3_10",
+            speech_volume_normalize: float = None,
+            speech_name: str = "speech",
+            text_name: str = "text",
+            split_with_space: bool = False,
+            seg_dict_file: str = None,
     ):
-        assert check_argument_types()
-
-        # 1. Build ASR model
-        scorers = {}
-        asr_model, asr_train_args = ASRTask.build_model_from_file(
-            asr_train_config, asr_model_file, cmvn_file, device
-        )
-        frontend = None
-        if asr_train_args.frontend is not None and asr_train_args.frontend_conf is not None:
-            frontend = WavFrontendOnline(cmvn_file=cmvn_file, **asr_train_args.frontend_conf)
-
-        logging.info("asr_model: {}".format(asr_model))
-        logging.info("asr_train_args: {}".format(asr_train_args))
-        asr_model.to(dtype=getattr(torch, dtype)).eval()
-
-        if asr_model.ctc != None:
-            ctc = CTCPrefixScorer(ctc=asr_model.ctc, eos=asr_model.eos)
-            scorers.update(
-                ctc=ctc
+        super().__init__(train)
+        self.train = train
+        self.speech_name = speech_name
+        self.text_name = text_name
+        self.speech_volume_normalize = speech_volume_normalize
+        self.rir_apply_prob = rir_apply_prob
+        self.noise_apply_prob = noise_apply_prob
+        self.split_with_space = split_with_space
+        self.seg_dict = None
+        if seg_dict_file is not None:
+            self.seg_dict = {}
+            with open(seg_dict_file) as f:
+                lines = f.readlines()
+            for line in lines:
+                s = line.strip().split()
+                key = s[0]
+                value = s[1:]
+                self.seg_dict[key] = " ".join(value)
+
+        if token_type is not None:
+            if token_list is None:
+                raise ValueError("token_list is required if token_type is not None")
+            self.text_cleaner = TextCleaner(text_cleaner)
+
+            self.tokenizer = build_tokenizer(
+                token_type=token_type,
+                bpemodel=bpemodel,
+                delimiter=delimiter,
+                space_symbol=space_symbol,
+                non_linguistic_symbols=non_linguistic_symbols,
+                g2p_type=g2p_type,
             )
-        token_list = asr_model.token_list
-        scorers.update(
-            length_bonus=LengthBonus(len(token_list)),
-        )
-
-        # 2. Build Language model
-        if lm_train_config is not None:
-            lm, lm_train_args = LMTask.build_model_from_file(
-                lm_train_config, lm_file, device
+            self.token_id_converter = TokenIDConverter(
+                token_list=token_list,
+                unk_symbol=unk_symbol,
             )
-            scorers["lm"] = lm.lm
-
-        # 3. Build ngram model
-        # ngram is not supported now
-        ngram = None
-        scorers["ngram"] = ngram
-
-        # 4. Build BeamSearch object
-        # transducer is not supported now
-        beam_search_transducer = None
-
-        weights = dict(
-            decoder=1.0 - ctc_weight,
-            ctc=ctc_weight,
-            lm=lm_weight,
-            ngram=ngram_weight,
-            length_bonus=penalty,
-        )
-        beam_search = BeamSearch(
-            beam_size=beam_size,
-            weights=weights,
-            scorers=scorers,
-            sos=asr_model.sos,
-            eos=asr_model.eos,
-            vocab_size=len(token_list),
-            token_list=token_list,
-            pre_beam_score_key=None if ctc_weight == 1.0 else "full",
-        )
-
-        beam_search.to(device=device, dtype=getattr(torch, dtype)).eval()
-        for scorer in scorers.values():
-            if isinstance(scorer, torch.nn.Module):
-                scorer.to(device=device, dtype=getattr(torch, dtype)).eval()
-
-        logging.info(f"Decoding device={device}, dtype={dtype}")
-
-        # 5. [Optional] Build Text converter: e.g. bpe-sym -> Text
-        if token_type is None:
-            token_type = asr_train_args.token_type
-        if bpemodel is None:
-            bpemodel = asr_train_args.bpemodel
-
-        if token_type is None:
-            tokenizer = None
-        elif token_type == "bpe":
-            if bpemodel is not None:
-                tokenizer = build_tokenizer(token_type=token_type, bpemodel=bpemodel)
-            else:
-                tokenizer = None
         else:
-            tokenizer = build_tokenizer(token_type=token_type)
-        converter = TokenIDConverter(token_list=token_list)
-        logging.info(f"Text tokenizer: {tokenizer}")
-
-        self.asr_model = asr_model
-        self.asr_train_args = asr_train_args
-        self.converter = converter
-        self.tokenizer = tokenizer
-
-        # 6. [Optional] Build hotword list from str, local file or url
-
-        is_use_lm = lm_weight != 0.0 and lm_file is not None
-        if (ctc_weight == 0.0 or asr_model.ctc == None) and not is_use_lm:
-            beam_search = None
-        self.beam_search = beam_search
-        logging.info(f"Beam_search: {self.beam_search}")
-        self.beam_search_transducer = beam_search_transducer
-        self.maxlenratio = maxlenratio
-        self.minlenratio = minlenratio
-        self.device = device
-        self.dtype = dtype
-        self.nbest = nbest
-        self.frontend = frontend
-        self.encoder_downsampling_factor = 1
-        if asr_train_args.encoder == "data2vec_encoder" or asr_train_args.encoder_conf["input_layer"] == "conv2d":
-            self.encoder_downsampling_factor = 4
-
-    @torch.no_grad()
-    def __call__(
-            self, cache: dict, speech: Union[torch.Tensor], speech_lengths: Union[torch.Tensor] = None
-    ):
-        """Inference
-
-        Args:
-                speech: Input speech data
-        Returns:
-                text, token, token_int, hyp
-
-        """
-        assert check_argument_types()
-        results = []
-        cache_en = cache["encoder"]
-        if speech.shape[1] < 16 * 60 and cache_en["is_final"]:
-            if cache_en["start_idx"] == 0:
-                return []
-            cache_en["tail_chunk"] = True
-            feats = cache_en["feats"]
-            feats_len = torch.tensor([feats.shape[1]])
-            self.asr_model.frontend = None
-            results = self.infer(feats, feats_len, cache)
-            return results
+            self.text_cleaner = None
+            self.tokenizer = None
+            self.token_id_converter = None
+
+        if train and rir_scp is not None:
+            self.rirs = []
+            with open(rir_scp, "r", encoding="utf-8") as f:
+                for line in f:
+                    sps = line.strip().split(None, 1)
+                    if len(sps) == 1:
+                        self.rirs.append(sps[0])
+                    else:
+                        self.rirs.append(sps[1])
         else:
-            if self.frontend is not None:
-                feats, feats_len = self.frontend.forward(speech, speech_lengths, cache_en["is_final"])
-                feats = to_device(feats, device=self.device)
-                feats_len = feats_len.int()
-                self.asr_model.frontend = None
-            else:
-                feats = speech
-                feats_len = speech_lengths
+            self.rirs = None
 
-            if feats.shape[1] != 0:
-                if cache_en["is_final"]:
-                    if feats.shape[1] + cache_en["chunk_size"][2] < cache_en["chunk_size"][1]:
-                        cache_en["last_chunk"] = True
+        if train and noise_scp is not None:
+            self.noises = []
+            with open(noise_scp, "r", encoding="utf-8") as f:
+                for line in f:
+                    sps = line.strip().split(None, 1)
+                    if len(sps) == 1:
+                        self.noises.append(sps[0])
                     else:
-                        # first chunk
-                        feats_chunk1 = feats[:, :cache_en["chunk_size"][1], :]
-                        feats_len = torch.tensor([feats_chunk1.shape[1]])
-                        results_chunk1 = self.infer(feats_chunk1, feats_len, cache)
-
-                        # last chunk
-                        cache_en["last_chunk"] = True
-                        feats_chunk2 = feats[:, -(feats.shape[1] + cache_en["chunk_size"][2] - cache_en["chunk_size"][1]):, :]
-                        feats_len = torch.tensor([feats_chunk2.shape[1]])
-                        results_chunk2 = self.infer(feats_chunk2, feats_len, cache)
-
-                        return [" ".join(results_chunk1 + results_chunk2)]
-
-                results = self.infer(feats, feats_len, cache)
-
-        return results
-
-    @torch.no_grad()
-    def infer(self, feats: Union[torch.Tensor], feats_len: Union[torch.Tensor], cache: List = None):
-        batch = {"speech": feats, "speech_lengths": feats_len}
-        batch = to_device(batch, device=self.device)
-        # b. Forward Encoder
-        enc, enc_len = self.asr_model.encode_chunk(feats, feats_len, cache=cache)
-        if isinstance(enc, tuple):
-            enc = enc[0]
-        # assert len(enc) == 1, len(enc)
-        enc_len_batch_total = torch.sum(enc_len).item() * self.encoder_downsampling_factor
-
-        predictor_outs = self.asr_model.calc_predictor_chunk(enc, cache)
-        pre_acoustic_embeds, pre_token_length= predictor_outs[0], predictor_outs[1]
-        if torch.max(pre_token_length) < 1:
-            return []
-        decoder_outs = self.asr_model.cal_decoder_with_predictor_chunk(enc, pre_acoustic_embeds, cache)
-        decoder_out = decoder_outs
-
-        results = []
-        b, n, d = decoder_out.size()
-        for i in range(b):
-            x = enc[i, :enc_len[i], :]
-            am_scores = decoder_out[i, :pre_token_length[i], :]
-            if self.beam_search is not None:
-                nbest_hyps = self.beam_search(
-                    x=x, am_scores=am_scores, maxlenratio=self.maxlenratio, minlenratio=self.minlenratio
-                )
-
-                nbest_hyps = nbest_hyps[: self.nbest]
+                        self.noises.append(sps[1])
+            sps = noise_db_range.split("_")
+            if len(sps) == 1:
+                self.noise_db_low, self.noise_db_high = float(sps[0])
+            elif len(sps) == 2:
+                self.noise_db_low, self.noise_db_high = float(sps[0]), float(sps[1])
             else:
-                yseq = am_scores.argmax(dim=-1)
-                score = am_scores.max(dim=-1)[0]
-                score = torch.sum(score, dim=-1)
-                # pad with mask tokens to ensure compatibility with sos/eos tokens
-                yseq = torch.tensor(
-                    [self.asr_model.sos] + yseq.tolist() + [self.asr_model.eos], device=yseq.device
+                raise ValueError(
+                    "Format error: '{noise_db_range}' e.g. -3_4 -> [-3db,4db]"
                 )
-                nbest_hyps = [Hypothesis(yseq=yseq, score=score)]
-
-            for hyp in nbest_hyps:
-                assert isinstance(hyp, (Hypothesis)), type(hyp)
+        else:
+            self.noises = None
 
-                # remove sos/eos and get results
-                last_pos = -1
-                if isinstance(hyp.yseq, list):
-                    token_int = hyp.yseq[1:last_pos]
+    def _speech_process(
+            self, data: Dict[str, Union[str, np.ndarray]]
+    ) -> Dict[str, Union[str, np.ndarray]]:
+        assert check_argument_types()
+        if self.speech_name in data:
+            if self.train and (self.rirs is not None or self.noises is not None):
+                speech = data[self.speech_name]
+                nsamples = len(speech)
+
+                # speech: (Nmic, Time)
+                if speech.ndim == 1:
+                    speech = speech[None, :]
                 else:
-                    token_int = hyp.yseq[1:last_pos].tolist()
+                    speech = speech.T
+                # Calc power on non shlence region
+                power = (speech[detect_non_silence(speech)] ** 2).mean()
+
+                # 1. Convolve RIR
+                if self.rirs is not None and self.rir_apply_prob >= np.random.random():
+                    rir_path = np.random.choice(self.rirs)
+                    if rir_path is not None:
+                        rir, _ = soundfile.read(
+                            rir_path, dtype=np.float64, always_2d=True
+                        )
+
+                        # rir: (Nmic, Time)
+                        rir = rir.T
+
+                        # speech: (Nmic, Time)
+                        # Note that this operation doesn't change the signal length
+                        speech = scipy.signal.convolve(speech, rir, mode="full")[
+                                 :, : speech.shape[1]
+                                 ]
+                        # Reverse mean power to the original power
+                        power2 = (speech[detect_non_silence(speech)] ** 2).mean()
+                        speech = np.sqrt(power / max(power2, 1e-10)) * speech
+
+                # 2. Add Noise
+                if (
+                        self.noises is not None
+                        and self.noise_apply_prob >= np.random.random()
+                ):
+                    noise_path = np.random.choice(self.noises)
+                    if noise_path is not None:
+                        noise_db = np.random.uniform(
+                            self.noise_db_low, self.noise_db_high
+                        )
+                        with soundfile.SoundFile(noise_path) as f:
+                            if f.frames == nsamples:
+                                noise = f.read(dtype=np.float64, always_2d=True)
+                            elif f.frames < nsamples:
+                                offset = np.random.randint(0, nsamples - f.frames)
+                                # noise: (Time, Nmic)
+                                noise = f.read(dtype=np.float64, always_2d=True)
+                                # Repeat noise
+                                noise = np.pad(
+                                    noise,
+                                    [(offset, nsamples - f.frames - offset), (0, 0)],
+                                    mode="wrap",
+                                )
+                            else:
+                                offset = np.random.randint(0, f.frames - nsamples)
+                                f.seek(offset)
+                                # noise: (Time, Nmic)
+                                noise = f.read(
+                                    nsamples, dtype=np.float64, always_2d=True
+                                )
+                                if len(noise) != nsamples:
+                                    raise RuntimeError(f"Something wrong: {noise_path}")
+                        # noise: (Nmic, Time)
+                        noise = noise.T
+
+                        noise_power = (noise ** 2).mean()
+                        scale = (
+                                10 ** (-noise_db / 20)
+                                * np.sqrt(power)
+                                / np.sqrt(max(noise_power, 1e-10))
+                        )
+                        speech = speech + scale * noise
+
+                speech = speech.T
+                ma = np.max(np.abs(speech))
+                if ma > 1.0:
+                    speech /= ma
+                data[self.speech_name] = speech
+
+            if self.speech_volume_normalize is not None:
+                speech = data[self.speech_name]
+                ma = np.max(np.abs(speech))
+                data[self.speech_name] = speech * self.speech_volume_normalize / ma
+        assert check_return_type(data)
+        return data
 
-                # remove blank symbol id, which is assumed to be 0
-                token_int = list(filter(lambda x: x != 0 and x != 2, token_int))
+    def _text_process(
+            self, data: Dict[str, Union[str, np.ndarray]]
+    ) -> Dict[str, np.ndarray]:
+        if self.text_name in data and self.tokenizer is not None:
+            text = data[self.text_name]
+            text = self.text_cleaner(text)
+            if self.split_with_space:
+                tokens = text.strip().split(" ")
+                if self.seg_dict is not None:
+                    tokens = seg_tokenize(tokens, self.seg_dict)
+            else:
+                tokens = self.tokenizer.text2tokens(text)
+            text_ints = self.token_id_converter.tokens2ids(tokens)
+            data[self.text_name] = np.array(text_ints, dtype=np.int64)
+        assert check_return_type(data)
+        return data
 
-                # Change integer-ids to tokens
-                token = self.converter.ids2tokens(token_int)
-                token = " ".join(token)
-
-                results.append(token)
-
-        # assert check_return_type(results)
-        return results
-
-
-def inference(
-        maxlenratio: float,
-        minlenratio: float,
-        batch_size: int,
-        beam_size: int,
-        ngpu: int,
-        ctc_weight: float,
-        lm_weight: float,
-        penalty: float,
-        log_level: Union[int, str],
-        data_path_and_name_and_type,
-        asr_train_config: Optional[str],
-        asr_model_file: Optional[str],
-        cmvn_file: Optional[str] = None,
-        raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-        lm_train_config: Optional[str] = None,
-        lm_file: Optional[str] = None,
-        token_type: Optional[str] = None,
-        key_file: Optional[str] = None,
-        word_lm_train_config: Optional[str] = None,
-        bpemodel: Optional[str] = None,
-        allow_variable_data_keys: bool = False,
-        streaming: bool = False,
-        output_dir: Optional[str] = None,
-        dtype: str = "float32",
-        seed: int = 0,
-        ngram_weight: float = 0.9,
-        nbest: int = 1,
-        num_workers: int = 1,
+    def __call__(
+            self, uid: str, data: Dict[str, Union[str, np.ndarray]]
+    ) -> Dict[str, np.ndarray]:
+        assert check_argument_types()
 
-        **kwargs,
-):
-    inference_pipeline = inference_modelscope(
-        maxlenratio=maxlenratio,
-        minlenratio=minlenratio,
-        batch_size=batch_size,
-        beam_size=beam_size,
-        ngpu=ngpu,
-        ctc_weight=ctc_weight,
-        lm_weight=lm_weight,
-        penalty=penalty,
-        log_level=log_level,
-        asr_train_config=asr_train_config,
-        asr_model_file=asr_model_file,
-        cmvn_file=cmvn_file,
-        raw_inputs=raw_inputs,
-        lm_train_config=lm_train_config,
-        lm_file=lm_file,
-        token_type=token_type,
-        key_file=key_file,
-        word_lm_train_config=word_lm_train_config,
-        bpemodel=bpemodel,
-        allow_variable_data_keys=allow_variable_data_keys,
-        streaming=streaming,
-        output_dir=output_dir,
-        dtype=dtype,
-        seed=seed,
-        ngram_weight=ngram_weight,
-        nbest=nbest,
-        num_workers=num_workers,
+        data = self._speech_process(data)
+        data = self._text_process(data)
+        return data
 
-        **kwargs,
-    )
-    return inference_pipeline(data_path_and_name_and_type, raw_inputs)
+## FIXME
+class LMPreprocessor(CommonPreprocessor):
+    def __init__(
+            self,
+            train: bool,
+            token_type: str = None,
+            token_list: Union[Path, str, Iterable[str]] = None,
+            bpemodel: Union[Path, str, Iterable[str]] = None,
+            text_cleaner: Collection[str] = None,
+            g2p_type: str = None,
+            unk_symbol: str = "<unk>",
+            space_symbol: str = "<space>",
+            non_linguistic_symbols: Union[Path, str, Iterable[str]] = None,
+            delimiter: str = None,
+            rir_scp: str = None,
+            rir_apply_prob: float = 1.0,
+            noise_scp: str = None,
+            noise_apply_prob: float = 1.0,
+            noise_db_range: str = "3_10",
+            speech_volume_normalize: float = None,
+            speech_name: str = "speech",
+            text_name: str = "text",
+            split_with_space: bool = False,
+            seg_dict_file: str = None,
+    ):
+        super().__init__(train,
+                         token_type,
+                         token_list,
+                         bpemodel,
+                         text_cleaner,
+                         g2p_type,
+                         unk_symbol,
+                         space_symbol,
+                         non_linguistic_symbols,
+                         delimiter,
+                         rir_scp,
+                         rir_apply_prob,
+                         noise_scp,
+                         noise_apply_prob,
+                         noise_db_range,
+                         speech_volume_normalize,
+                         speech_name,
+                         text_name,
+                         split_with_space,
+                         seg_dict_file,
+                         )
+
+    def _text_process(
+            self, data: Dict[str, Union[str, np.ndarray]]
+    ) -> Dict[str, np.ndarray]:
+        if self.text_name in data and self.tokenizer is not None:
+            text = data[self.text_name]
+            text = self.text_cleaner(text)
+            if self.split_with_space:
+                tokens = text.strip().split(" ")
+                if self.seg_dict is not None:
+                    tokens = seg_tokenize_wo_pattern(tokens, self.seg_dict)
+            else:
+                tokens = self.tokenizer.text2tokens(text)
+            text_ints = self.token_id_converter.tokens2ids(tokens)
+            data[self.text_name] = np.array(text_ints, dtype=np.int64)
+        assert check_return_type(data)
+        return data
 
 
-def inference_modelscope(
-        maxlenratio: float,
-        minlenratio: float,
-        batch_size: int,
-        beam_size: int,
-        ngpu: int,
-        ctc_weight: float,
-        lm_weight: float,
-        penalty: float,
-        log_level: Union[int, str],
-        # data_path_and_name_and_type,
-        asr_train_config: Optional[str],
-        asr_model_file: Optional[str],
-        cmvn_file: Optional[str] = None,
-        lm_train_config: Optional[str] = None,
-        lm_file: Optional[str] = None,
-        token_type: Optional[str] = None,
-        key_file: Optional[str] = None,
-        word_lm_train_config: Optional[str] = None,
-        bpemodel: Optional[str] = None,
-        allow_variable_data_keys: bool = False,
-        dtype: str = "float32",
-        seed: int = 0,
-        ngram_weight: float = 0.9,
-        nbest: int = 1,
-        num_workers: int = 1,
-        output_dir: Optional[str] = None,
-        param_dict: dict = None,
-        **kwargs,
-):
-    assert check_argument_types()
+class CommonPreprocessor_multi(AbsPreprocessor):
+    def __init__(
+            self,
+            train: bool,
+            token_type: str = None,
+            token_list: Union[Path, str, Iterable[str]] = None,
+            bpemodel: Union[Path, str, Iterable[str]] = None,
+            text_cleaner: Collection[str] = None,
+            g2p_type: str = None,
+            unk_symbol: str = "<unk>",
+            space_symbol: str = "<space>",
+            non_linguistic_symbols: Union[Path, str, Iterable[str]] = None,
+            delimiter: str = None,
+            speech_name: str = "speech",
+            text_name: List[str] = ["text"],
+    ):
+        super().__init__(train)
+        self.train = train
+        self.speech_name = speech_name
+        self.text_name = text_name
+
+        if token_type is not None:
+            if token_list is None:
+                raise ValueError("token_list is required if token_type is not None")
+            self.text_cleaner = TextCleaner(text_cleaner)
+
+            self.tokenizer = build_tokenizer(
+                token_type=token_type,
+                bpemodel=bpemodel,
+                delimiter=delimiter,
+                space_symbol=space_symbol,
+                non_linguistic_symbols=non_linguistic_symbols,
+                g2p_type=g2p_type,
+            )
+            self.token_id_converter = TokenIDConverter(
+                token_list=token_list,
+                unk_symbol=unk_symbol,
+            )
+        else:
+            self.text_cleaner = None
+            self.tokenizer = None
+            self.token_id_converter = None
+
+    def _text_process(
+            self, data: Dict[str, Union[str, np.ndarray]]
+    ) -> Dict[str, np.ndarray]:
+        for text_n in self.text_name:
+            if text_n in data and self.tokenizer is not None:
+                text = data[text_n]
+                text = self.text_cleaner(text)
+                tokens = self.tokenizer.text2tokens(text)
+                text_ints = self.token_id_converter.tokens2ids(tokens)
+                data[text_n] = np.array(text_ints, dtype=np.int64)
+        assert check_return_type(data)
+        return data
 
-    if word_lm_train_config is not None:
-        raise NotImplementedError("Word LM is not implemented")
-    if ngpu > 1:
-        raise NotImplementedError("only single GPU decoding is supported")
-
-    logging.basicConfig(
-        level=log_level,
-        format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
-    )
+    def __call__(
+            self, uid: str, data: Dict[str, Union[str, np.ndarray]]
+    ) -> Dict[str, np.ndarray]:
+        assert check_argument_types()
 
-    export_mode = False
+        if self.speech_name in data:
+            # Nothing now: candidates:
+            # - STFT
+            # - Fbank
+            # - CMVN
+            # - Data augmentation
+            pass
 
-    if ngpu >= 1 and torch.cuda.is_available():
-        device = "cuda"
-    else:
-        device = "cpu"
-        batch_size = 1
+        data = self._text_process(data)
+        return data
 
-    # 1. Set random-seed
-    set_all_random_seed(seed)
 
-    # 2. Build speech2text
-    speech2text_kwargs = dict(
-        asr_train_config=asr_train_config,
-        asr_model_file=asr_model_file,
-        cmvn_file=cmvn_file,
-        lm_train_config=lm_train_config,
-        lm_file=lm_file,
-        token_type=token_type,
-        bpemodel=bpemodel,
-        device=device,
-        maxlenratio=maxlenratio,
-        minlenratio=minlenratio,
-        dtype=dtype,
-        beam_size=beam_size,
-        ctc_weight=ctc_weight,
-        lm_weight=lm_weight,
-        ngram_weight=ngram_weight,
-        penalty=penalty,
-        nbest=nbest,
-    )
+class MutliTokenizerCommonPreprocessor(CommonPreprocessor):
+    def __init__(
+            self,
+            train: bool,
+            token_type: List[str] = [None],
+            token_list: List[Union[Path, str, Iterable[str]]] = [None],
+            bpemodel: List[Union[Path, str, Iterable[str]]] = [None],
+            text_cleaner: Collection[str] = None,
+            g2p_type: str = None,
+            unk_symbol: str = "<unk>",
+            space_symbol: str = "<space>",
+            non_linguistic_symbols: Union[Path, str, Iterable[str]] = None,
+            delimiter: str = None,
+            rir_scp: str = None,
+            rir_apply_prob: float = 1.0,
+            noise_scp: str = None,
+            noise_apply_prob: float = 1.0,
+            noise_db_range: str = "3_10",
+            speech_volume_normalize: float = None,
+            speech_name: str = "speech",
+            text_name: List[str] = ["text"],
+    ):
+        # TODO(jiatong): sync with Kamo and Jing on interface for preprocessor
+        super().__init__(
+            train=train,
+            token_type=token_type[0],
+            token_list=token_list[0],
+            bpemodel=bpemodel[0],
+            text_cleaner=text_cleaner,
+            g2p_type=g2p_type,
+            unk_symbol=unk_symbol,
+            space_symbol=space_symbol,
+            non_linguistic_symbols=non_linguistic_symbols,
+            delimiter=delimiter,
+            speech_name=speech_name,
+            text_name=text_name[0],
+            rir_scp=rir_scp,
+            rir_apply_prob=rir_apply_prob,
+            noise_scp=noise_scp,
+            noise_apply_prob=noise_apply_prob,
+            noise_db_range=noise_db_range,
+            speech_volume_normalize=speech_volume_normalize,
+        )
 
-    speech2text = Speech2Text(**speech2text_kwargs)
+        assert (
+                len(token_type) == len(token_list) == len(bpemodel) == len(text_name)
+        ), "token_type, token_list, bpemodel, or processing text_name mismatched"
+        self.num_tokenizer = len(token_type)
+        self.tokenizer = []
+        self.token_id_converter = []
+
+        for i in range(self.num_tokenizer):
+            if token_type[i] is not None:
+                if token_list[i] is None:
+                    raise ValueError("token_list is required if token_type is not None")
+
+                self.tokenizer.append(
+                    build_tokenizer(
+                        token_type=token_type[i],
+                        bpemodel=bpemodel[i],
+                        delimiter=delimiter,
+                        space_symbol=space_symbol,
+                        non_linguistic_symbols=non_linguistic_symbols,
+                        g2p_type=g2p_type,
+                    )
+                )
+                self.token_id_converter.append(
+                    TokenIDConverter(
+                        token_list=token_list[i],
+                        unk_symbol=unk_symbol,
+                    )
+                )
+            else:
+                self.tokenizer.append(None)
+                self.token_id_converter.append(None)
 
-    def _load_bytes(input):
-        middle_data = np.frombuffer(input, dtype=np.int16)
-        middle_data = np.asarray(middle_data)
-        if middle_data.dtype.kind not in 'iu':
-            raise TypeError("'middle_data' must be an array of integers")
-        dtype = np.dtype('float32')
-        if dtype.kind != 'f':
-            raise TypeError("'dtype' must be a floating point type")
-
-        i = np.iinfo(middle_data.dtype)
-        abs_max = 2 ** (i.bits - 1)
-        offset = i.min + abs_max
-        array = np.frombuffer((middle_data.astype(dtype) - offset) / abs_max, dtype=np.float32)
-        return array
-
-    def _read_yaml(yaml_path: Union[str, Path]) -> Dict:
-        if not Path(yaml_path).exists():
-            raise FileExistsError(f'The {yaml_path} does not exist.')
+        self.text_cleaner = TextCleaner(text_cleaner)
+        self.text_name = text_name  # override the text_name from CommonPreprocessor
 
-        with open(str(yaml_path), 'rb') as f:
-            data = yaml.load(f, Loader=yaml.Loader)
+    def _text_process(
+            self, data: Dict[str, Union[str, np.ndarray]]
+    ) -> Dict[str, np.ndarray]:
+        for i in range(self.num_tokenizer):
+            text_name = self.text_name[i]
+            if text_name in data and self.tokenizer[i] is not None:
+                text = data[text_name]
+                text = self.text_cleaner(text)
+                tokens = self.tokenizer[i].text2tokens(text)
+                text_ints = self.token_id_converter[i].tokens2ids(tokens)
+                data[text_name] = np.array(text_ints, dtype=np.int64)
+        assert check_return_type(data)
         return data
 
-    def _prepare_cache(cache: dict = {}, chunk_size=[5,10,5], batch_size=1):
-        if len(cache) > 0:
-            return cache
-        config = _read_yaml(asr_train_config)
-        enc_output_size = config["encoder_conf"]["output_size"]
-        feats_dims = config["frontend_conf"]["n_mels"] * config["frontend_conf"]["lfr_m"]
-        cache_en = {"start_idx": 0, "cif_hidden": torch.zeros((batch_size, 1, enc_output_size)),
-                    "cif_alphas": torch.zeros((batch_size, 1)), "chunk_size": chunk_size, "last_chunk": False,
-                    "feats": torch.zeros((batch_size, chunk_size[0] + chunk_size[2], feats_dims)), "tail_chunk": False}
-        cache["encoder"] = cache_en
-
-        cache_de = {"decode_fsmn": None}
-        cache["decoder"] = cache_de
-
-        return cache
-
-    def _cache_reset(cache: dict = {}, chunk_size=[5,10,5], batch_size=1):
-        if len(cache) > 0:
-            config = _read_yaml(asr_train_config)
-            enc_output_size = config["encoder_conf"]["output_size"]
-            feats_dims = config["frontend_conf"]["n_mels"] * config["frontend_conf"]["lfr_m"]
-            cache_en = {"start_idx": 0, "cif_hidden": torch.zeros((batch_size, 1, enc_output_size)),
-                        "cif_alphas": torch.zeros((batch_size, 1)), "chunk_size": chunk_size, "last_chunk": False,
-                        "feats": torch.zeros((batch_size, chunk_size[0] + chunk_size[2], feats_dims)), "tail_chunk": False}
-            cache["encoder"] = cache_en
-
-            cache_de = {"decode_fsmn": None}
-            cache["decoder"] = cache_de
-
-        return cache
-
-    def _forward(
-            data_path_and_name_and_type,
-            raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-            output_dir_v2: Optional[str] = None,
-            fs: dict = None,
-            param_dict: dict = None,
-            **kwargs,
+class CodeMixTokenizerCommonPreprocessor(CommonPreprocessor):
+    def __init__(
+            self,
+            train: bool,
+            token_type: str = None,
+            token_list: Union[Path, str, Iterable[str]] = None,
+            bpemodel: Union[Path, str, Iterable[str]] = None,
+            text_cleaner: Collection[str] = None,
+            g2p_type: str = None,
+            unk_symbol: str = "<unk>",
+            space_symbol: str = "<space>",
+            non_linguistic_symbols: Union[Path, str, Iterable[str]] = None,
+            delimiter: str = None,
+            rir_scp: str = None,
+            rir_apply_prob: float = 1.0,
+            noise_scp: str = None,
+            noise_apply_prob: float = 1.0,
+            noise_db_range: str = "3_10",
+            speech_volume_normalize: float = None,
+            speech_name: str = "speech",
+            text_name: str = "text",
+            split_text_name: str = "split_text",
+            split_with_space: bool = False,
+            seg_dict_file: str = None,
     ):
+        super().__init__(
+            train=train,
+            # Force to use word.
+            token_type="word",
+            token_list=token_list,
+            bpemodel=bpemodel,
+            text_cleaner=text_cleaner,
+            g2p_type=g2p_type,
+            unk_symbol=unk_symbol,
+            space_symbol=space_symbol,
+            non_linguistic_symbols=non_linguistic_symbols,
+            delimiter=delimiter,
+            speech_name=speech_name,
+            text_name=text_name,
+            rir_scp=rir_scp,
+            rir_apply_prob=rir_apply_prob,
+            noise_scp=noise_scp,
+            noise_apply_prob=noise_apply_prob,
+            noise_db_range=noise_db_range,
+            speech_volume_normalize=speech_volume_normalize,
+            split_with_space=split_with_space,
+            seg_dict_file=seg_dict_file,
+        )
+        # The data field name for split text.
+        self.split_text_name = split_text_name
 
-        # 3. Build data-iterator
-        if data_path_and_name_and_type is not None and data_path_and_name_and_type[2] == "bytes":
-            raw_inputs = _load_bytes(data_path_and_name_and_type[0])
-            raw_inputs = torch.tensor(raw_inputs)
-        if data_path_and_name_and_type is not None and data_path_and_name_and_type[2] == "sound":
-            raw_inputs = torchaudio.load(data_path_and_name_and_type[0])[0][0]
-        if data_path_and_name_and_type is None and raw_inputs is not None:
-            if isinstance(raw_inputs, np.ndarray):
-                raw_inputs = torch.tensor(raw_inputs)
-        is_final = False
-        cache = {}
-        chunk_size = [5, 10, 5]
-        if param_dict is not None and "cache" in param_dict:
-            cache = param_dict["cache"]
-        if param_dict is not None and "is_final" in param_dict:
-            is_final = param_dict["is_final"]
-        if param_dict is not None and "chunk_size" in param_dict:
-            chunk_size = param_dict["chunk_size"]
-
-        # 7 .Start for-loop
-        # FIXME(kamo): The output format should be discussed about
-        raw_inputs = torch.unsqueeze(raw_inputs, axis=0)
-        asr_result_list = []
-        cache = _prepare_cache(cache, chunk_size=chunk_size, batch_size=1)
-        item = {}
-        if data_path_and_name_and_type is not None and data_path_and_name_and_type[2] == "sound":
-            sample_offset = 0
-            speech_length = raw_inputs.shape[1]
-            stride_size =  chunk_size[1] * 960
-            cache = _prepare_cache(cache, chunk_size=chunk_size, batch_size=1)
-            final_result = ""
-            for sample_offset in range(0, speech_length, min(stride_size, speech_length - sample_offset)):
-                if sample_offset + stride_size >= speech_length - 1:
-                    stride_size = speech_length - sample_offset
-                    cache["encoder"]["is_final"] = True
+    @classmethod
+    def split_words(cls, text: str):
+        words = []
+        segs = text.split()
+        for seg in segs:
+            # There is no space in seg.
+            current_word = ""
+            for c in seg:
+                if len(c.encode()) == 1:
+                    # This is an ASCII char.
+                    current_word += c
                 else:
-                    cache["encoder"]["is_final"] = False
-                input_lens = torch.tensor([stride_size])
-                asr_result = speech2text(cache, raw_inputs[:, sample_offset: sample_offset + stride_size], input_lens)
-                if len(asr_result) != 0: 
-                    final_result += " ".join(asr_result) + " "
-            item = {'key': "utt", 'value': final_result.strip()}
-        else:
-            input_lens = torch.tensor([raw_inputs.shape[1]])
-            cache["encoder"]["is_final"] = is_final
-            asr_result = speech2text(cache, raw_inputs, input_lens)
-            item = {'key': "utt", 'value': " ".join(asr_result)}
-
-        asr_result_list.append(item)
-        if is_final:
-            cache = _cache_reset(cache, chunk_size=chunk_size, batch_size=1)
-        return asr_result_list
-
-    return _forward
-
-
-def get_parser():
-    parser = config_argparse.ArgumentParser(
-        description="ASR Decoding",
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-    )
-
-    # Note(kamo): Use '_' instead of '-' as separator.
-    # '-' is confusing if written in yaml.
-    parser.add_argument(
-        "--log_level",
-        type=lambda x: x.upper(),
-        default="INFO",
-        choices=("CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET"),
-        help="The verbose level of logging",
-    )
-
-    parser.add_argument("--output_dir", type=str, required=True)
-    parser.add_argument(
-        "--ngpu",
-        type=int,
-        default=0,
-        help="The number of gpus. 0 indicates CPU mode",
-    )
-    parser.add_argument("--seed", type=int, default=0, help="Random seed")
-    parser.add_argument(
-        "--dtype",
-        default="float32",
-        choices=["float16", "float32", "float64"],
-        help="Data type",
-    )
-    parser.add_argument(
-        "--num_workers",
-        type=int,
-        default=1,
-        help="The number of workers used for DataLoader",
-    )
-    parser.add_argument(
-        "--hotword",
-        type=str_or_none,
-        default=None,
-        help="hotword file path or hotwords seperated by space"
-    )
-    group = parser.add_argument_group("Input data related")
-    group.add_argument(
-        "--data_path_and_name_and_type",
-        type=str2triple_str,
-        required=False,
-        action="append",
-    )
-    group.add_argument("--key_file", type=str_or_none)
-    group.add_argument("--allow_variable_data_keys", type=str2bool, default=False)
-
-    group = parser.add_argument_group("The model configuration related")
-    group.add_argument(
-        "--asr_train_config",
-        type=str,
-        help="ASR training configuration",
-    )
-    group.add_argument(
-        "--asr_model_file",
-        type=str,
-        help="ASR model parameter file",
-    )
-    group.add_argument(
-        "--cmvn_file",
-        type=str,
-        help="Global cmvn file",
-    )
-    group.add_argument(
-        "--lm_train_config",
-        type=str,
-        help="LM training configuration",
-    )
-    group.add_argument(
-        "--lm_file",
-        type=str,
-        help="LM parameter file",
-    )
-    group.add_argument(
-        "--word_lm_train_config",
-        type=str,
-        help="Word LM training configuration",
-    )
-    group.add_argument(
-        "--word_lm_file",
-        type=str,
-        help="Word LM parameter file",
-    )
-    group.add_argument(
-        "--ngram_file",
-        type=str,
-        help="N-gram parameter file",
-    )
-    group.add_argument(
-        "--model_tag",
-        type=str,
-        help="Pretrained model tag. If specify this option, *_train_config and "
-             "*_file will be overwritten",
-    )
-
-    group = parser.add_argument_group("Beam-search related")
-    group.add_argument(
-        "--batch_size",
-        type=int,
-        default=1,
-        help="The batch size for inference",
-    )
-    group.add_argument("--nbest", type=int, default=1, help="Output N-best hypotheses")
-    group.add_argument("--beam_size", type=int, default=20, help="Beam size")
-    group.add_argument("--penalty", type=float, default=0.0, help="Insertion penalty")
-    group.add_argument(
-        "--maxlenratio",
-        type=float,
-        default=0.0,
-        help="Input length ratio to obtain max output length. "
-             "If maxlenratio=0.0 (default), it uses a end-detect "
-             "function "
-             "to automatically find maximum hypothesis lengths."
-             "If maxlenratio<0.0, its absolute value is interpreted"
-             "as a constant max output length",
-    )
-    group.add_argument(
-        "--minlenratio",
-        type=float,
-        default=0.0,
-        help="Input length ratio to obtain min output length",
-    )
-    group.add_argument(
-        "--ctc_weight",
-        type=float,
-        default=0.5,
-        help="CTC weight in joint decoding",
-    )
-    group.add_argument("--lm_weight", type=float, default=1.0, help="RNNLM weight")
-    group.add_argument("--ngram_weight", type=float, default=0.9, help="ngram weight")
-    group.add_argument("--streaming", type=str2bool, default=False)
-
-    group.add_argument(
-        "--frontend_conf",
-        default=None,
-        help="",
-    )
-    group.add_argument("--raw_inputs", type=list, default=None)
-    # example=[{'key':'EdevDEWdIYQ_0021','file':'/mnt/data/jiangyu.xzy/test_data/speech_io/SPEECHIO_ASR_ZH00007_zhibodaihuo/wav/EdevDEWdIYQ_0021.wav'}])
+                    # This is a Chinese char.
+                    if len(current_word) > 0:
+                        words.append(current_word)
+                        current_word = ""
+                    words.append(c)
+            if len(current_word) > 0:
+                words.append(current_word)
+        return words
 
-    group = parser.add_argument_group("Text converter related")
-    group.add_argument(
-        "--token_type",
-        type=str_or_none,
-        default=None,
-        choices=["char", "bpe", None],
-        help="The token type for ASR model. "
-             "If not given, refers from the training args",
-    )
-    group.add_argument(
-        "--bpemodel",
-        type=str_or_none,
-        default=None,
-        help="The model path of sentencepiece. "
-             "If not given, refers from the training args",
-    )
-
-    return parser
+    def __call__(
+            self, uid: str, data: Dict[str, Union[list, str, np.ndarray]]
+    ) -> Dict[str, Union[list, np.ndarray]]:
+        assert check_argument_types()
+        # Split words.
+        if isinstance(data[self.text_name], str):
+            split_text = self.split_words(data[self.text_name])
+        else:
+            split_text = data[self.text_name]
+        data[self.text_name] = " ".join(split_text)
+        data = self._speech_process(data)
+        data = self._text_process(data)
+        data[self.split_text_name] = split_text
+        return data
 
+    def pop_split_text_data(self, data: Dict[str, Union[str, np.ndarray]]):
+        result = data[self.split_text_name]
+        del data[self.split_text_name]
+        return result
 
-def main(cmd=None):
-    print(get_commandline_args(), file=sys.stderr)
-    parser = get_parser()
-    args = parser.parse_args(cmd)
-    param_dict = {'hotword': args.hotword}
-    kwargs = vars(args)
-    kwargs.pop("config", None)
-    kwargs['param_dict'] = param_dict
-    inference(**kwargs)
+class PuncTrainTokenizerCommonPreprocessor(CommonPreprocessor):
+    def __init__(
+            self,
+            train: bool,
+            token_type: List[str] = [None],
+            token_list: List[Union[Path, str, Iterable[str]]] = [None],
+            bpemodel: List[Union[Path, str, Iterable[str]]] = [None],
+            text_cleaner: Collection[str] = None,
+            g2p_type: str = None,
+            unk_symbol: str = "<unk>",
+            space_symbol: str = "<space>",
+            non_linguistic_symbols: Union[Path, str, Iterable[str]] = None,
+            delimiter: str = None,
+            rir_scp: str = None,
+            rir_apply_prob: float = 1.0,
+            noise_scp: str = None,
+            noise_apply_prob: float = 1.0,
+            noise_db_range: str = "3_10",
+            speech_volume_normalize: float = None,
+            speech_name: str = "speech",
+            text_name: List[str] = ["text"],
+            vad_name: str = "vad_indexes",
+    ):
+        # TODO(jiatong): sync with Kamo and Jing on interface for preprocessor
+        super().__init__(
+            train=train,
+            token_type=token_type[0],
+            token_list=token_list[0],
+            bpemodel=bpemodel[0],
+            text_cleaner=text_cleaner,
+            g2p_type=g2p_type,
+            unk_symbol=unk_symbol,
+            space_symbol=space_symbol,
+            non_linguistic_symbols=non_linguistic_symbols,
+            delimiter=delimiter,
+            speech_name=speech_name,
+            text_name=text_name[0],
+            rir_scp=rir_scp,
+            rir_apply_prob=rir_apply_prob,
+            noise_scp=noise_scp,
+            noise_apply_prob=noise_apply_prob,
+            noise_db_range=noise_db_range,
+            speech_volume_normalize=speech_volume_normalize,
+        )
 
+        assert (
+                len(token_type) == len(token_list) == len(bpemodel) == len(text_name)
+        ), "token_type, token_list, bpemodel, or processing text_name mismatched"
+        self.num_tokenizer = len(token_type)
+        self.tokenizer = []
+        self.token_id_converter = []
+
+        for i in range(self.num_tokenizer):
+            if token_type[i] is not None:
+                if token_list[i] is None:
+                    raise ValueError("token_list is required if token_type is not None")
+
+                self.tokenizer.append(
+                    build_tokenizer(
+                        token_type=token_type[i],
+                        bpemodel=bpemodel[i],
+                        delimiter=delimiter,
+                        space_symbol=space_symbol,
+                        non_linguistic_symbols=non_linguistic_symbols,
+                        g2p_type=g2p_type,
+                    )
+                )
+                self.token_id_converter.append(
+                    TokenIDConverter(
+                        token_list=token_list[i],
+                        unk_symbol=unk_symbol,
+                    )
+                )
+            else:
+                self.tokenizer.append(None)
+                self.token_id_converter.append(None)
 
-if __name__ == "__main__":
-    main()
+        self.text_cleaner = TextCleaner(text_cleaner)
+        self.text_name = text_name  # override the text_name from CommonPreprocessor
+        self.vad_name = vad_name
+
+    def _text_process(
+            self, data: Dict[str, Union[str, np.ndarray]]
+    ) -> Dict[str, np.ndarray]:
+        for i in range(self.num_tokenizer):
+            text_name = self.text_name[i]
+            #import pdb; pdb.set_trace()
+            if text_name in data and self.tokenizer[i] is not None:
+                text = data[text_name]
+                text = self.text_cleaner(text)
+                tokens = self.tokenizer[i].text2tokens(text)
+                if "vad:" in tokens[-1]:
+                    vad = tokens[-1][4:]
+                    tokens = tokens[:-1]
+                    if len(vad) == 0:
+                        vad = -1
+                    else:
+                        vad = int(vad)
+                    data[self.vad_name] = np.array([vad], dtype=np.int64)
+                text_ints = self.token_id_converter[i].tokens2ids(tokens)
+                data[text_name] = np.array(text_ints, dtype=np.int64)
+        return data
 
+def split_to_mini_sentence(words: list, word_limit: int = 20):
+    assert word_limit > 1
+    if len(words) <= word_limit:
+        return [words]
+    sentences = []
+    length = len(words)
+    sentence_len = length // word_limit
+    for i in range(sentence_len):
+        sentences.append(words[i * word_limit:(i + 1) * word_limit])
+    if length % word_limit > 0:
+        sentences.append(words[sentence_len * word_limit:])
+    return sentences
```

### Comparing `funasr-0.5.3/funasr/bin/asr_train.py` & `funasr-0.5.4/funasr/bin/sa_asr_train.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+# -*- encoding: utf-8 -*-
 #!/usr/bin/env python3
+# Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
+#  MIT License  (https://opensource.org/licenses/MIT)
 
 import os
 
-from funasr.tasks.asr import ASRTask
+from funasr.tasks.sa_asr import ASRTask
 
 
 # for ASR Training
 def parse_args():
     parser = ASRTask.get_parser()
     parser.add_argument(
         "--gpu_id",
```

### Comparing `funasr-0.5.3/funasr/bin/asr_train_paraformer.py` & `funasr-0.5.4/funasr/bin/data2vec_train.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 #!/usr/bin/env python3
 
 import os
 
-from funasr.tasks.asr import ASRTaskParaformer as ASRTask
+from funasr.tasks.data2vec import Data2VecTask
 
 
-# for ASR Training
 def parse_args():
-    parser = ASRTask.get_parser()
+    parser = Data2VecTask.get_parser()
     parser.add_argument(
         "--gpu_id",
         type=int,
         default=0,
         help="local gpu id.",
     )
     args = parser.parse_args()
     return args
 
 
 def main(args=None, cmd=None):
-    # for ASR Training
-    ASRTask.main(args=args, cmd=cmd)
+    # for data2vec Training
+    Data2VecTask.main(args=args, cmd=cmd)
 
 
 if __name__ == '__main__':
     args = parse_args()
 
     # setup local gpu_id
     os.environ['CUDA_VISIBLE_DEVICES'] = str(args.gpu_id)
```

### Comparing `funasr-0.5.3/funasr/bin/asr_train_transducer.py` & `funasr-0.5.4/funasr/bin/lm_train.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,33 @@
+# -*- encoding: utf-8 -*-
 #!/usr/bin/env python3
+# Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
+#  MIT License  (https://opensource.org/licenses/MIT)
 
 import os
 
-from funasr.tasks.asr import ASRTransducerTask
+from funasr.tasks.lm import LMTask
 
 
-# for ASR Training
+# for LM Training
 def parse_args():
-    parser = ASRTransducerTask.get_parser()
+    parser = LMTask.get_parser()
     parser.add_argument(
         "--gpu_id",
         type=int,
         default=0,
         help="local gpu id.",
     )
     args = parser.parse_args()
     return args
 
 
 def main(args=None, cmd=None):
-    # for ASR Training
-    ASRTransducerTask.main(args=args, cmd=cmd)
+    # for LM Training
+    LMTask.main(args=args, cmd=cmd)
 
 
 if __name__ == '__main__':
     args = parse_args()
 
     # setup local gpu_id
     os.environ['CUDA_VISIBLE_DEVICES'] = str(args.gpu_id)
@@ -33,14 +36,14 @@
     if args.ngpu > 1:
         args.distributed = True
     else:
         args.distributed = False
     assert args.num_worker_count == 1
 
     # re-compute batch size: when dataset type is small
-    if args.dataset_type == "small":
+    if args.dataset_type == "small" and args.ngpu != 0:
         if args.batch_size is not None:
             args.batch_size = args.batch_size * args.ngpu
         if args.batch_bins is not None:
             args.batch_bins = args.batch_bins * args.ngpu
 
     main(args=args)
```

### Comparing `funasr-0.5.3/funasr/bin/diar_train.py` & `funasr-0.5.4/funasr/bin/diar_train.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+# -*- encoding: utf-8 -*-
 #!/usr/bin/env python3
+# Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
+#  MIT License  (https://opensource.org/licenses/MIT)
 
 import os
 
 from funasr.tasks.diar import DiarTask
 
 
 # for ASR Training
```

### Comparing `funasr-0.5.3/funasr/bin/eend_ola_inference.py` & `funasr-0.5.4/funasr/bin/lm_inference_launch.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,429 +1,409 @@
+# -*- encoding: utf-8 -*-
 #!/usr/bin/env python3
 # Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
 #  MIT License  (https://opensource.org/licenses/MIT)
 
 import argparse
 import logging
 import os
 import sys
+from typing import Union, Dict, Any
+
+from funasr.utils import config_argparse
+from funasr.utils.cli_utils import get_commandline_args
+from funasr.utils.types import str2bool
+from funasr.utils.types import str2triple_str
+from funasr.utils.types import str_or_none
+from funasr.utils.types import float_or_none
+import argparse
+import logging
 from pathlib import Path
-from typing import Any
-from typing import List
+import sys
+import os
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Union
+from typing import Dict
+from typing import Any
+from typing import List
 
 import numpy as np
 import torch
-from scipy.signal import medfilt
+from torch.nn.parallel import data_parallel
 from typeguard import check_argument_types
 
-from funasr.models.frontend.wav_frontend import WavFrontendMel23
-from funasr.tasks.diar import EENDOLADiarTask
+from funasr.tasks.lm import LMTask
+from funasr.datasets.preprocessor import LMPreprocessor
+from funasr.utils.cli_utils import get_commandline_args
+from funasr.fileio.datadir_writer import DatadirWriter
 from funasr.torch_utils.device_funcs import to_device
+from funasr.torch_utils.forward_adaptor import ForwardAdaptor
+from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.utils import config_argparse
-from funasr.utils.cli_utils import get_commandline_args
+from funasr.utils.types import float_or_none
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
 
 
-class Speech2Diarization:
-    """Speech2Diarlization class
-
-    Examples:
-        >>> import soundfile
-        >>> import numpy as np
-        >>> speech2diar = Speech2Diarization("diar_sond_config.yml", "diar_sond.pb")
-        >>> profile = np.load("profiles.npy")
-        >>> audio, rate = soundfile.read("speech.wav")
-        >>> speech2diar(audio, profile)
-        {"spk1": [(int, int), ...], ...}
-
-    """
-
-    def __init__(
-            self,
-            diar_train_config: Union[Path, str] = None,
-            diar_model_file: Union[Path, str] = None,
-            device: str = "cpu",
-            dtype: str = "float32",
-    ):
-        assert check_argument_types()
-
-        # 1. Build Diarization model
-        diar_model, diar_train_args = EENDOLADiarTask.build_model_from_file(
-            config_file=diar_train_config,
-            model_file=diar_model_file,
-            device=device
-        )
-        frontend = None
-        if diar_train_args.frontend is not None and diar_train_args.frontend_conf is not None:
-            frontend = WavFrontendMel23(**diar_train_args.frontend_conf)
-
-        # set up seed for eda
-        np.random.seed(diar_train_args.seed)
-        torch.manual_seed(diar_train_args.seed)
-        torch.cuda.manual_seed(diar_train_args.seed)
-        os.environ['PYTORCH_SEED'] = str(diar_train_args.seed)
-        logging.info("diar_model: {}".format(diar_model))
-        logging.info("diar_train_args: {}".format(diar_train_args))
-        diar_model.to(dtype=getattr(torch, dtype)).eval()
-
-        self.diar_model = diar_model
-        self.diar_train_args = diar_train_args
-        self.device = device
-        self.dtype = dtype
-        self.frontend = frontend
-
-    @torch.no_grad()
-    def __call__(
-            self,
-            speech: Union[torch.Tensor, np.ndarray],
-            speech_lengths: Union[torch.Tensor, np.ndarray] = None
-    ):
-        """Inference
-
-        Args:
-            speech: Input speech data
-        Returns:
-            diarization results
-
-        """
-        assert check_argument_types()
-        # Input as audio signal
-        if isinstance(speech, np.ndarray):
-            speech = torch.tensor(speech)
-
-        if self.frontend is not None:
-            feats, feats_len = self.frontend.forward(speech, speech_lengths)
-            feats = to_device(feats, device=self.device)
-            feats_len = feats_len.int()
-            self.diar_model.frontend = None
-        else:
-            feats = speech
-            feats_len = speech_lengths
-        batch = {"speech": feats, "speech_lengths": feats_len}
-        batch = to_device(batch, device=self.device)
-        results = self.diar_model.estimate_sequential(**batch)
-
-        return results
-
-    @staticmethod
-    def from_pretrained(
-            model_tag: Optional[str] = None,
-            **kwargs: Optional[Any],
-    ):
-        """Build Speech2Diarization instance from the pretrained model.
-
-        Args:
-            model_tag (Optional[str]): Model tag of the pretrained models.
-                Currently, the tags of espnet_model_zoo are supported.
-
-        Returns:
-            Speech2Diarization: Speech2Diarization instance.
-
-        """
-        if model_tag is not None:
-            try:
-                from espnet_model_zoo.downloader import ModelDownloader
-
-            except ImportError:
-                logging.error(
-                    "`espnet_model_zoo` is not installed. "
-                    "Please install via `pip install -U espnet_model_zoo`."
-                )
-                raise
-            d = ModelDownloader()
-            kwargs.update(**d.download_and_unpack(model_tag))
-
-        return Speech2Diarization(**kwargs)
-
-
-def inference_modelscope(
-        diar_train_config: str,
-        diar_model_file: str,
-        output_dir: Optional[str] = None,
-        batch_size: int = 1,
-        dtype: str = "float32",
-        ngpu: int = 1,
-        num_workers: int = 0,
-        log_level: Union[int, str] = "INFO",
-        key_file: Optional[str] = None,
-        model_tag: Optional[str] = None,
-        allow_variable_data_keys: bool = True,
-        streaming: bool = False,
-        param_dict: Optional[dict] = None,
-        **kwargs,
+def inference_lm(
+    batch_size: int,
+    dtype: str,
+    ngpu: int,
+    seed: int,
+    num_workers: int,
+    log_level: Union[int, str],
+    key_file: Optional[str],
+    train_config: Optional[str],
+    model_file: Optional[str],
+    log_base: Optional[float] = 10,
+    allow_variable_data_keys: bool = False,
+    split_with_space: Optional[bool] = False,
+    seg_dict_file: Optional[str] = None,
+    output_dir: Optional[str] = None,
+    param_dict: dict = None,
+    **kwargs,
 ):
     assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
-    if batch_size > 1:
-        raise NotImplementedError("batch decoding is not implemented")
-    if ngpu > 1:
-        raise NotImplementedError("only single GPU decoding is supported")
-
-    logging.basicConfig(
-        level=log_level,
-        format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
-    )
-    logging.info("param_dict: {}".format(param_dict))
-
+    
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
-
-    # 1. Build speech2diar
-    speech2diar_kwargs = dict(
-        diar_train_config=diar_train_config,
-        diar_model_file=diar_model_file,
-        device=device,
-        dtype=dtype,
-    )
-    logging.info("speech2diarization_kwargs: {}".format(speech2diar_kwargs))
-    speech2diar = Speech2Diarization.from_pretrained(
-        model_tag=model_tag,
-        **speech2diar_kwargs,
-    )
-    speech2diar.diar_model.eval()
-
-    def output_results_str(results: dict, uttid: str):
-        rst = []
-        mid = uttid.rsplit("-", 1)[0]
-        for key in results:
-            results[key] = [(x[0] / 100, x[1] / 100) for x in results[key]]
-        template = "SPEAKER {} 0 {:.2f} {:.2f} <NA> <NA> {} <NA> <NA>"
-        for spk, segs in results.items():
-            rst.extend([template.format(mid, st, ed, spk) for st, ed in segs])
-
-        return "\n".join(rst)
-
+    
+    # 1. Set random-seed
+    set_all_random_seed(seed)
+    
+    # 2. Build Model
+    model, train_args = LMTask.build_model_from_file(
+        train_config, model_file, device)
+    wrapped_model = ForwardAdaptor(model, "nll")
+    wrapped_model.to(dtype=getattr(torch, dtype)).to(device=device).eval()
+    logging.info(f"Model:\n{model}")
+    
+    preprocessor = LMPreprocessor(
+        train=False,
+        token_type=train_args.token_type,
+        token_list=train_args.token_list,
+        bpemodel=train_args.bpemodel,
+        text_cleaner=train_args.cleaner,
+        g2p_type=train_args.g2p,
+        text_name="text",
+        non_linguistic_symbols=train_args.non_linguistic_symbols,
+        split_with_space=split_with_space,
+        seg_dict_file=seg_dict_file
+    )
+    
     def _forward(
-            data_path_and_name_and_type: Sequence[Tuple[str, str, str]] = None,
-            raw_inputs: List[List[Union[np.ndarray, torch.Tensor, str, bytes]]] = None,
-            output_dir_v2: Optional[str] = None,
-            param_dict: Optional[dict] = None,
+        data_path_and_name_and_type,
+        raw_inputs: Union[List[Any], bytes, str] = None,
+        output_dir_v2: Optional[str] = None,
+        param_dict: dict = None,
     ):
-        # 2. Build data-iterator
-        if data_path_and_name_and_type is None and raw_inputs is not None:
-            if isinstance(raw_inputs, torch.Tensor):
-                raw_inputs = raw_inputs.numpy()
-            data_path_and_name_and_type = [raw_inputs[0], "speech", "sound"]
-        loader = EENDOLADiarTask.build_streaming_iterator(
+        results = []
+        output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
+        if output_path is not None:
+            writer = DatadirWriter(output_path)
+        else:
+            writer = None
+        
+        if raw_inputs != None:
+            line = raw_inputs.strip()
+            key = "lm demo"
+            if line == "":
+                item = {'key': key, 'value': ""}
+                results.append(item)
+                return results
+            batch = {}
+            batch['text'] = line
+            if preprocessor != None:
+                batch = preprocessor(key, batch)
+            
+            #  Force data-precision
+            for name in batch:
+                value = batch[name]
+                if not isinstance(value, np.ndarray):
+                    raise RuntimeError(
+                        f"All values must be converted to np.ndarray object "
+                        f'by preprocessing, but "{name}" is still {type(value)}.'
+                    )
+                # Cast to desired type
+                if value.dtype.kind == "f":
+                    value = value.astype("float32")
+                elif value.dtype.kind == "i":
+                    value = value.astype("long")
+                else:
+                    raise NotImplementedError(f"Not supported dtype: {value.dtype}")
+                batch[name] = value
+            
+            batch["text_lengths"] = torch.from_numpy(
+                np.array([len(batch["text"])], dtype='int32'))
+            batch["text"] = np.expand_dims(batch["text"], axis=0)
+            
+            with torch.no_grad():
+                batch = to_device(batch, device)
+                if ngpu <= 1:
+                    nll, lengths = wrapped_model(**batch)
+                else:
+                    nll, lengths = data_parallel(
+                        wrapped_model, (), range(ngpu), module_kwargs=batch
+                    )
+                ## compute ppl
+                ppl_out_batch = ""
+                ids2tokens = preprocessor.token_id_converter.ids2tokens
+                for sent_ids, sent_nll in zip(batch['text'], nll):
+                    pre_word = "<s>"
+                    cur_word = None
+                    sent_lst = ids2tokens(sent_ids) + ['</s>']
+                    ppl_out = " ".join(sent_lst) + "\n"
+                    for word, word_nll in zip(sent_lst, sent_nll):
+                        cur_word = word
+                        word_nll = -word_nll.cpu()
+                        if log_base is None:
+                            word_prob = np.exp(word_nll)
+                        else:
+                            word_prob = log_base ** (word_nll / np.log(log_base))
+                        ppl_out += '    p( {cur} | {pre} ) = {prob} [ {word_nll} ]\n'.format(
+                            cur=cur_word,
+                            pre=pre_word,
+                            prob=round(word_prob.item(), 8),
+                            word_nll=round(word_nll.item(), 8)
+                        )
+                        pre_word = cur_word
+                    
+                    sent_nll_mean = sent_nll.mean().cpu().numpy()
+                    sent_nll_sum = sent_nll.sum().cpu().numpy()
+                    if log_base is None:
+                        sent_ppl = np.exp(sent_nll_mean)
+                    else:
+                        sent_ppl = log_base ** (sent_nll_mean / np.log(log_base))
+                    ppl_out += 'logprob= {sent_nll} ppl= {sent_ppl}\n\n'.format(
+                        sent_nll=round(-sent_nll_sum.item(), 4),
+                        sent_ppl=round(sent_ppl.item(), 4)
+                    )
+                    ppl_out_batch += ppl_out
+                    item = {'key': key, 'value': ppl_out}
+                    if writer is not None:
+                        writer["ppl"][key + ":\n"] = ppl_out
+                    results.append(item)
+            
+            return results
+        
+        # 3. Build data-iterator
+        loader = LMTask.build_streaming_iterator(
             data_path_and_name_and_type,
             dtype=dtype,
             batch_size=batch_size,
             key_file=key_file,
             num_workers=num_workers,
-            preprocess_fn=EENDOLADiarTask.build_preprocess_fn(speech2diar.diar_train_args, False),
-            collate_fn=EENDOLADiarTask.build_collate_fn(speech2diar.diar_train_args, False),
+            preprocess_fn=preprocessor,
+            collate_fn=LMTask.build_collate_fn(train_args, False),
             allow_variable_data_keys=allow_variable_data_keys,
             inference=True,
         )
-
-        # 3. Start for-loop
-        output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
-        if output_path is not None:
-            os.makedirs(output_path, exist_ok=True)
-            output_writer = open("{}/result.txt".format(output_path), "w")
-        result_list = []
+        
+        # 4. Start for-loop
+        total_nll = 0.0
+        total_ntokens = 0
+        ppl_out_all = ""
         for keys, batch in loader:
             assert isinstance(batch, dict), type(batch)
             assert all(isinstance(s, str) for s in keys), keys
             _bs = len(next(iter(batch.values())))
             assert len(keys) == _bs, f"{len(keys)} != {_bs}"
-            # batch = {k: v[0] for k, v in batch.items() if not k.endswith("_lengths")}
-
-            results = speech2diar(**batch)
-
-            # post process
-            a = results[0][0].cpu().numpy()
-            a = medfilt(a, (11, 1))
-            rst = []
-            for spkid, frames in enumerate(a.T):
-                frames = np.pad(frames, (1, 1), 'constant')
-                changes, = np.where(np.diff(frames, axis=0) != 0)
-                fmt = "SPEAKER {:s} 1 {:7.2f} {:7.2f} <NA> <NA> {:s} <NA>"
-                for s, e in zip(changes[::2], changes[1::2]):
-                    st = s / 10.
-                    dur = (e - s) / 10.
-                    rst.append(fmt.format(keys[0], st, dur, "{}_{}".format(keys[0], str(spkid))))
-
-            # Only supporting batch_size==1
-            value = "\n".join(rst)
-            item = {"key": keys[0], "value": value}
-            result_list.append(item)
-            if output_path is not None:
-                output_writer.write(value)
-                output_writer.flush()
-
-        if output_path is not None:
-            output_writer.close()
-
-        return result_list
-
+            
+            ppl_out_batch = ""
+            with torch.no_grad():
+                batch = to_device(batch, device)
+                if ngpu <= 1:
+                    # NOTE(kamo): data_parallel also should work with ngpu=1,
+                    # but for debuggability it's better to keep this block.
+                    nll, lengths = wrapped_model(**batch)
+                else:
+                    nll, lengths = data_parallel(
+                        wrapped_model, (), range(ngpu), module_kwargs=batch
+                    )
+                ## print ppl
+                ids2tokens = preprocessor.token_id_converter.ids2tokens
+                for key, sent_ids, sent_nll in zip(keys, batch['text'], nll):
+                    pre_word = "<s>"
+                    cur_word = None
+                    sent_lst = ids2tokens(sent_ids) + ['</s>']
+                    ppl_out = " ".join(sent_lst) + "\n"
+                    for word, word_nll in zip(sent_lst, sent_nll):
+                        cur_word = word
+                        word_nll = -word_nll.cpu()
+                        if log_base is None:
+                            word_prob = np.exp(word_nll)
+                        else:
+                            word_prob = log_base ** (word_nll / np.log(log_base))
+                        ppl_out += '    p( {cur} | {pre} ) = {prob} [ {word_nll} ]\n'.format(
+                            cur=cur_word,
+                            pre=pre_word,
+                            prob=round(word_prob.item(), 8),
+                            word_nll=round(word_nll.item(), 8)
+                        )
+                        pre_word = cur_word
+                    
+                    sent_nll_mean = sent_nll.mean().cpu().numpy()
+                    sent_nll_sum = sent_nll.sum().cpu().numpy()
+                    if log_base is None:
+                        sent_ppl = np.exp(sent_nll_mean)
+                    else:
+                        sent_ppl = log_base ** (sent_nll_mean / np.log(log_base))
+                    ppl_out += 'logprob= {sent_nll} ppl= {sent_ppl}\n\n'.format(
+                        sent_nll=round(-sent_nll_sum.item(), 4),
+                        sent_ppl=round(sent_ppl.item(), 4)
+                    )
+                    ppl_out_batch += ppl_out
+                    utt2nll = round(-sent_nll_sum.item(), 5)
+                    item = {'key': key, 'value': ppl_out}
+                    if writer is not None:
+                        writer["ppl"][key + ":\n"] = ppl_out
+                        writer["utt2nll"][key] = str(utt2nll)
+                    results.append(item)
+            
+            ppl_out_all += ppl_out_batch
+            
+            assert _bs == len(nll) == len(lengths), (_bs, len(nll), len(lengths))
+            # nll: (B, L) -> (B,)
+            nll = nll.detach().cpu().numpy().sum(1)
+            # lengths: (B,)
+            lengths = lengths.detach().cpu().numpy()
+            total_nll += nll.sum()
+            total_ntokens += lengths.sum()
+        
+        if log_base is None:
+            ppl = np.exp(total_nll / total_ntokens)
+        else:
+            ppl = log_base ** (total_nll / total_ntokens / np.log(log_base))
+        
+        avg_ppl = 'logprob= {total_nll} ppl= {total_ppl}\n'.format(
+            total_nll=round(-total_nll.item(), 4),
+            total_ppl=round(ppl.item(), 4)
+        )
+        item = {'key': 'AVG PPL', 'value': avg_ppl}
+        ppl_out_all += avg_ppl
+        if writer is not None:
+            writer["ppl"]["AVG PPL : "] = avg_ppl
+        results.append(item)
+        
+        return results
+    
     return _forward
 
 
-def inference(
-        data_path_and_name_and_type: Sequence[Tuple[str, str, str]],
-        diar_train_config: Optional[str],
-        diar_model_file: Optional[str],
-        output_dir: Optional[str] = None,
-        batch_size: int = 1,
-        dtype: str = "float32",
-        ngpu: int = 0,
-        seed: int = 0,
-        num_workers: int = 1,
-        log_level: Union[int, str] = "INFO",
-        key_file: Optional[str] = None,
-        model_tag: Optional[str] = None,
-        allow_variable_data_keys: bool = True,
-        streaming: bool = False,
-        smooth_size: int = 83,
-        dur_threshold: int = 10,
-        out_format: str = "vad",
-        **kwargs,
-):
-    inference_pipeline = inference_modelscope(
-        diar_train_config=diar_train_config,
-        diar_model_file=diar_model_file,
-        output_dir=output_dir,
-        batch_size=batch_size,
-        dtype=dtype,
-        ngpu=ngpu,
-        seed=seed,
-        num_workers=num_workers,
-        log_level=log_level,
-        key_file=key_file,
-        model_tag=model_tag,
-        allow_variable_data_keys=allow_variable_data_keys,
-        streaming=streaming,
-        smooth_size=smooth_size,
-        dur_threshold=dur_threshold,
-        out_format=out_format,
-        **kwargs,
-    )
-
-    return inference_pipeline(data_path_and_name_and_type, raw_inputs=None)
-
-
+def inference_launch(mode, **kwargs):
+    if mode == "transformer":
+        return inference_lm(**kwargs)
+    else:
+        logging.info("Unknown decoding mode: {}".format(mode))
+        return None
+    
 def get_parser():
     parser = config_argparse.ArgumentParser(
-        description="Speaker verification/x-vector extraction",
+        description="Calc perplexity",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
-    # Note(kamo): Use '_' instead of '-' as separator.
-    # '-' is confusing if written in yaml.
     parser.add_argument(
         "--log_level",
         type=lambda x: x.upper(),
         default="INFO",
         choices=("CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET"),
         help="The verbose level of logging",
     )
-
-    parser.add_argument("--output_dir", type=str, required=False)
+    parser.add_argument("--output_dir", type=str, required=True)
+    parser.add_argument("--gpuid_list", type=str, required=True)
     parser.add_argument(
         "--ngpu",
         type=int,
         default=0,
         help="The number of gpus. 0 indicates CPU mode",
     )
-    parser.add_argument(
-        "--gpuid_list",
-        type=str,
-        default="",
-        help="The visible gpus",
-    )
     parser.add_argument("--seed", type=int, default=0, help="Random seed")
+    parser.add_argument("--njob", type=int, default=1, help="Random seed")
     parser.add_argument(
         "--dtype",
         default="float32",
         choices=["float16", "float32", "float64"],
         help="Data type",
     )
     parser.add_argument(
         "--num_workers",
         type=int,
         default=1,
         help="The number of workers used for DataLoader",
     )
+    parser.add_argument(
+        "--batch_size",
+        type=int,
+        default=1,
+        help="The batch size for inference",
+    )
+    parser.add_argument(
+        "--log_base",
+        type=float_or_none,
+        default=10,
+        help="The base of logarithm for Perplexity. "
+             "If None, napier's constant is used.",
+        required=False
+    )
 
     group = parser.add_argument_group("Input data related")
     group.add_argument(
         "--data_path_and_name_and_type",
         type=str2triple_str,
-        required=False,
         action="append",
-    )
-    group.add_argument("--key_file", type=str_or_none)
-    group.add_argument("--allow_variable_data_keys", type=str2bool, default=False)
-
-    group = parser.add_argument_group("The model configuration related")
-    group.add_argument(
-        "--diar_train_config",
-        type=str,
-        help="diarization training configuration",
-    )
-    group.add_argument(
-        "--diar_model_file",
-        type=str,
-        help="diarization model parameter file",
+        required=False
     )
     group.add_argument(
-        "--dur_threshold",
-        type=int,
-        default=10,
-        help="The threshold for short segments in number frames"
-    )
-    parser.add_argument(
-        "--smooth_size",
-        type=int,
-        default=83,
-        help="The smoothing window length in number frames"
-    )
-    group.add_argument(
-        "--model_tag",
+        "--raw_inputs",
         type=str,
-        help="Pretrained model tag. If specify this option, *_train_config and "
-             "*_file will be overwritten",
-    )
-    parser.add_argument(
-        "--batch_size",
-        type=int,
-        default=1,
-        help="The batch size for inference",
+        required=False
     )
-    parser.add_argument("--streaming", type=str2bool, default=False)
+    group.add_argument("--key_file", type=str_or_none)
+    group.add_argument("--allow_variable_data_keys", type=str2bool, default=False)
 
+    group.add_argument("--split_with_space", type=str2bool, default=False)
+    group.add_argument("--seg_dict_file", type=str_or_none)
+
+    group = parser.add_argument_group("The model configuration related")
+    group.add_argument("--train_config", type=str)
+    group.add_argument("--model_file", type=str)
+    group.add_argument("--mode", type=str, default="lm")
     return parser
 
 
 def main(cmd=None):
     print(get_commandline_args(), file=sys.stderr)
     parser = get_parser()
     args = parser.parse_args(cmd)
     kwargs = vars(args)
     kwargs.pop("config", None)
-    logging.info("args: {}".format(kwargs))
-    if args.output_dir is None:
-        jobid, n_gpu = 1, 1
-        gpuid = args.gpuid_list.split(",")[jobid - 1]
-    else:
+
+    # set logging messages
+    logging.basicConfig(
+        level=args.log_level,
+        format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
+    )
+    logging.info("Decoding args: {}".format(kwargs))
+
+    # gpu setting
+    if args.ngpu > 0:
         jobid = int(args.output_dir.split(".")[-1])
-        n_gpu = len(args.gpuid_list.split(","))
-        gpuid = args.gpuid_list.split(",")[(jobid - 1) % n_gpu]
-    os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
-    os.environ["CUDA_VISIBLE_DEVICES"] = gpuid
-    results_list = inference(**kwargs)
-    for results in results_list:
-        print("{} {}".format(results["key"], results["value"]))
+        gpuid = args.gpuid_list.split(",")[(jobid - 1) // args.njob]
+        os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
+        os.environ["CUDA_VISIBLE_DEVICES"] = gpuid
+
+    kwargs.pop("gpuid_list", None)
+    kwargs.pop("njob", None)
+    results = inference_launch(**kwargs)
 
 
 if __name__ == "__main__":
     main()
+
```

### Comparing `funasr-0.5.3/funasr/bin/lm_calc_perplexity.py` & `funasr-0.5.4/funasr/tasks/punctuation.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,211 +1,227 @@
-#!/usr/bin/env python3
 import argparse
 import logging
-from pathlib import Path
-import sys
+from typing import Callable
+from typing import Collection
+from typing import Dict
+from typing import List
 from typing import Optional
-from typing import Sequence
 from typing import Tuple
-from typing import Union
 
 import numpy as np
 import torch
-from torch.nn.parallel import data_parallel
 from typeguard import check_argument_types
+from typeguard import check_return_type
 
-from funasr.utils.cli_utils import get_commandline_args
-from funasr.fileio.datadir_writer import DatadirWriter
-from funasr.tasks.lm import LMTask
-from funasr.torch_utils.device_funcs import to_device
-from funasr.torch_utils.forward_adaptor import ForwardAdaptor
-from funasr.torch_utils.set_all_random_seed import set_all_random_seed
-from funasr.utils import config_argparse
-from funasr.utils.types import float_or_none
+from funasr.datasets.collate_fn import CommonCollateFn
+from funasr.datasets.preprocessor import PuncTrainTokenizerCommonPreprocessor
+from funasr.train.abs_model import PunctuationModel
+from funasr.models.target_delay_transformer import TargetDelayTransformer
+from funasr.models.vad_realtime_transformer import VadRealtimeTransformer
+from funasr.tasks.abs_task import AbsTask
+from funasr.text.phoneme_tokenizer import g2p_choices
+from funasr.torch_utils.initialize import initialize
+from funasr.train.class_choices import ClassChoices
+from funasr.train.trainer import Trainer
+from funasr.utils.get_default_kwargs import get_default_kwargs
+from funasr.utils.nested_dict_action import NestedDictAction
 from funasr.utils.types import str2bool
-from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
 
-
-def calc_perplexity(
-    output_dir: str,
-    batch_size: int,
-    dtype: str,
-    ngpu: int,
-    seed: int,
-    num_workers: int,
-    log_level: Union[int, str],
-    data_path_and_name_and_type: Sequence[Tuple[str, str, str]],
-    key_file: Optional[str],
-    train_config: Optional[str],
-    model_file: Optional[str],
-    log_base: Optional[float],
-    allow_variable_data_keys: bool,
-):
-    assert check_argument_types()
-    logging.basicConfig(
-        level=log_level,
-        format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
-    )
-
-    if ngpu >= 1:
-        device = "cuda"
-    else:
-        device = "cpu"
-
-    # 1. Set random-seed
-    set_all_random_seed(seed)
-
-    # 2. Build LM
-    model, train_args = LMTask.build_model_from_file(config_file=train_config, model_file=model_file, device=device)
-    # Wrape model to make model.nll() data-parallel
-    wrapped_model = ForwardAdaptor(model, "nll")
-    wrapped_model.to(dtype=getattr(torch, dtype)).eval()
-    logging.info(f"Model:\n{model}")
-
-    # 3. Build data-iterator
-    loader = LMTask.build_streaming_iterator(
-        data_path_and_name_and_type,
-        dtype=dtype,
-        batch_size=batch_size,
-        key_file=key_file,
-        num_workers=num_workers,
-        preprocess_fn=LMTask.build_preprocess_fn(train_args, False),
-        collate_fn=LMTask.build_collate_fn(train_args, False),
-        allow_variable_data_keys=allow_variable_data_keys,
-        inference=True,
-    )
-
-    # 4. Start for-loop
-    with DatadirWriter(output_dir) as writer:
-        total_nll = 0.0
-        total_ntokens = 0
-        for keys, batch in loader:
-            assert isinstance(batch, dict), type(batch)
-            assert all(isinstance(s, str) for s in keys), keys
-            _bs = len(next(iter(batch.values())))
-            assert len(keys) == _bs, f"{len(keys)} != {_bs}"
-
-            with torch.no_grad():
-                batch = to_device(batch, device)
-                if ngpu <= 1:
-                    # NOTE(kamo): data_parallel also should work with ngpu=1,
-                    # but for debuggability it's better to keep this block.
-                    nll, lengths = wrapped_model(**batch)
-                else:
-                    nll, lengths = data_parallel(
-                        wrapped_model, (), range(ngpu), module_kwargs=batch
-                    )
-
-            assert _bs == len(nll) == len(lengths), (_bs, len(nll), len(lengths))
-            # nll: (B, L) -> (B,)
-            nll = nll.detach().cpu().numpy().sum(1)
-            # lengths: (B,)
-            lengths = lengths.detach().cpu().numpy()
-            total_nll += nll.sum()
-            total_ntokens += lengths.sum()
-
-            for key, _nll, ntoken in zip(keys, nll, lengths):
-                if log_base is None:
-                    utt_ppl = np.exp(_nll / ntoken)
-                else:
-                    utt_ppl = log_base ** (_nll / ntoken / np.log(log_base))
-
-                # Write PPL of each utts for debugging or analysis
-                writer["utt2nll"][key] = str(-_nll)
-                writer["utt2ppl"][key] = str(utt_ppl)
-                writer["utt2ntokens"][key] = str(ntoken)
-
-        if log_base is None:
-            ppl = np.exp(total_nll / total_ntokens)
+punc_choices = ClassChoices(
+    "punctuation",
+    classes=dict(target_delay=TargetDelayTransformer, vad_realtime=VadRealtimeTransformer),
+    default="target_delay",
+)
+
+
+class PunctuationTask(AbsTask):
+    # If you need more than one optimizers, change this value
+    num_optimizers: int = 1
+
+    # Add variable objects configurations
+    class_choices_list = [punc_choices]
+
+    # If you need to modify train() or eval() procedures, change Trainer class here
+    trainer = Trainer
+
+    @classmethod
+    def add_task_arguments(cls, parser: argparse.ArgumentParser):
+        # NOTE(kamo): Use '_' instead of '-' to avoid confusion
+        assert check_argument_types()
+        group = parser.add_argument_group(description="Task related")
+
+        # NOTE(kamo): add_arguments(..., required=True) can't be used
+        # to provide --print_config mode. Instead of it, do as
+        required = parser.get_default("required")
+
+        group.add_argument(
+            "--token_list",
+            type=str_or_none,
+            default=None,
+            help="A text mapping int-id to token",
+        )
+        group.add_argument(
+            "--init",
+            type=lambda x: str_or_none(x.lower()),
+            default=None,
+            help="The initialization method",
+            choices=[
+                "chainer",
+                "xavier_uniform",
+                "xavier_normal",
+                "kaiming_uniform",
+                "kaiming_normal",
+                None,
+            ],
+        )
+        group.add_argument(
+            "--model_conf",
+            action=NestedDictAction,
+            default=get_default_kwargs(PunctuationModel),
+            help="The keyword arguments for model class.",
+        )
+
+        group = parser.add_argument_group(description="Preprocess related")
+        group.add_argument(
+            "--use_preprocessor",
+            type=str2bool,
+            default=True,
+            help="Apply preprocessing to data or not",
+        )
+        group.add_argument(
+            "--token_type",
+            type=str,
+            default="bpe",
+            choices=["bpe", "char", "word"],
+            help="",
+        )
+        group.add_argument(
+            "--bpemodel",
+            type=str_or_none,
+            default=None,
+            help="The model file fo sentencepiece",
+        )
+        parser.add_argument(
+            "--non_linguistic_symbols",
+            type=str_or_none,
+            help="non_linguistic_symbols file path",
+        )
+        parser.add_argument(
+            "--cleaner",
+            type=str_or_none,
+            choices=[None, "tacotron", "jaconv", "vietnamese"],
+            default=None,
+            help="Apply text cleaning",
+        )
+        parser.add_argument(
+            "--g2p",
+            type=str_or_none,
+            choices=g2p_choices,
+            default=None,
+            help="Specify g2p method if --token_type=phn",
+        )
+
+        for class_choices in cls.class_choices_list:
+            # Append --<name> and --<name>_conf.
+            # e.g. --encoder and --encoder_conf
+            class_choices.add_arguments(group)
+
+        assert check_return_type(parser)
+        return parser
+
+    @classmethod
+    def build_collate_fn(
+            cls, args: argparse.Namespace, train: bool
+    ) -> Callable[
+        [Collection[Tuple[str, Dict[str, np.ndarray]]]],
+        Tuple[List[str], Dict[str, torch.Tensor]],
+    ]:
+        assert check_argument_types()
+        return CommonCollateFn(int_pad_value=0)
+
+    @classmethod
+    def build_preprocess_fn(
+            cls, args: argparse.Namespace, train: bool
+    ) -> Optional[Callable[[str, Dict[str, np.array]], Dict[str, np.ndarray]]]:
+        assert check_argument_types()
+        token_types = [args.token_type, args.token_type]
+        token_lists = [args.token_list, args.punc_list]
+        bpemodels = [args.bpemodel, args.bpemodel]
+        text_names = ["text", "punc"]
+        if args.use_preprocessor:
+            retval = PuncTrainTokenizerCommonPreprocessor(
+                train=train,
+                token_type=token_types,
+                token_list=token_lists,
+                bpemodel=bpemodels,
+                text_cleaner=args.cleaner,
+                g2p_type=args.g2p,
+                text_name = text_names,
+                non_linguistic_symbols=args.non_linguistic_symbols,
+            )
         else:
-            ppl = log_base ** (total_nll / total_ntokens / np.log(log_base))
-
-        with (Path(output_dir) / "ppl").open("w", encoding="utf-8") as f:
-            f.write(f"{ppl}\n")
-        with (Path(output_dir) / "base").open("w", encoding="utf-8") as f:
-            if log_base is None:
-                _log_base = np.e
-            else:
-                _log_base = log_base
-            f.write(f"{_log_base}\n")
-        logging.info(f"PPL={ppl}")
-
-
-def get_parser():
-    parser = config_argparse.ArgumentParser(
-        description="Calc perplexity",
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-    )
-
-    # Note(kamo): Use '_' instead of '-' as separator.
-    # '-' is confusing if written in yaml.
-    parser.add_argument(
-        "--log_level",
-        type=lambda x: x.upper(),
-        default="INFO",
-        choices=("CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET"),
-        help="The verbose level of logging",
-    )
-
-    parser.add_argument("--output_dir", type=str, required=True)
-    parser.add_argument(
-        "--ngpu",
-        type=int,
-        default=0,
-        help="The number of gpus. 0 indicates CPU mode",
-    )
-    parser.add_argument("--seed", type=int, default=0, help="Random seed")
-    parser.add_argument(
-        "--dtype",
-        default="float32",
-        choices=["float16", "float32", "float64"],
-        help="Data type",
-    )
-    parser.add_argument(
-        "--num_workers",
-        type=int,
-        default=1,
-        help="The number of workers used for DataLoader",
-    )
-    parser.add_argument(
-        "--batch_size",
-        type=int,
-        default=1,
-        help="The batch size for inference",
-    )
-    parser.add_argument(
-        "--log_base",
-        type=float_or_none,
-        default=None,
-        help="The base of logarithm for Perplexity. "
-        "If None, napier's constant is used.",
-    )
-
-    group = parser.add_argument_group("Input data related")
-    group.add_argument(
-        "--data_path_and_name_and_type",
-        type=str2triple_str,
-        required=True,
-        action="append",
-    )
-    group.add_argument("--key_file", type=str_or_none)
-    group.add_argument("--allow_variable_data_keys", type=str2bool, default=False)
-
-    group = parser.add_argument_group("The model configuration related")
-    group.add_argument("--train_config", type=str)
-    group.add_argument("--model_file", type=str)
-
-    return parser
-
-
-def main(cmd=None):
-    print(get_commandline_args(), file=sys.stderr)
-    parser = get_parser()
-    args = parser.parse_args(cmd)
-    kwargs = vars(args)
-    kwargs.pop("config", None)
-    calc_perplexity(**kwargs)
+            retval = None
+        assert check_return_type(retval)
+        return retval
+
+    @classmethod
+    def required_data_names(
+            cls, train: bool = True, inference: bool = False
+    ) -> Tuple[str, ...]:
+        retval = ("text", "punc")
+        if inference:
+            retval = ("text", )
+        return retval
+
+    @classmethod
+    def optional_data_names(
+            cls, train: bool = True, inference: bool = False
+    ) -> Tuple[str, ...]:
+        retval = ("vad",)
+        return retval
+
+    @classmethod
+    def build_model(cls, args: argparse.Namespace) -> PunctuationModel:
+        assert check_argument_types()
+        if isinstance(args.token_list, str):
+            with open(args.token_list, encoding="utf-8") as f:
+                token_list = [line.rstrip() for line in f]
+
+            # "args" is saved as it is in a yaml file by BaseTask.main().
+            # Overwriting token_list to keep it as "portable".
+            args.token_list = token_list.copy()
+        if isinstance(args.punc_list, str):
+            with open(args.punc_list, encoding="utf-8") as f2:
+                pairs = [line.rstrip().split(":") for line in f2]
+            punc_list = [pair[0] for pair in pairs]
+            punc_weight_list = [float(pair[1]) for pair in pairs]
+            args.punc_list = punc_list.copy()
+        elif isinstance(args.punc_list, list):
+            punc_list = args.punc_list.copy()
+            punc_weight_list = [1] * len(punc_list)
+        if isinstance(args.token_list, (tuple, list)):
+            token_list = args.token_list.copy()
+        else:
+            raise RuntimeError("token_list must be str or dict")
 
+        vocab_size = len(token_list)
+        punc_size = len(punc_list)
+        logging.info(f"Vocabulary size: {vocab_size}")
+
+        # 1. Build PUNC model
+        punc_class = punc_choices.get_class(args.punctuation)
+        punc = punc_class(vocab_size=vocab_size, punc_size=punc_size, **args.punctuation_conf)
+
+        # 2. Build ESPnetModel
+        # Assume the last-id is sos_and_eos
+        if "punc_weight" in args.model_conf:
+            args.model_conf.pop("punc_weight")
+        model = PunctuationModel(punc_model=punc, vocab_size=vocab_size, punc_weight=punc_weight_list, **args.model_conf)
+
+        # FIXME(kamo): Should be done in model?
+        # 3. Initialize
+        if args.init is not None:
+            initialize(model, args.init)
 
-if __name__ == "__main__":
-    main()
+        assert check_return_type(model)
+        return model
```

### Comparing `funasr-0.5.3/funasr/bin/lm_inference.py` & `funasr-0.5.4/funasr/bin/vad_inference_launch.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,406 +1,409 @@
+# -*- encoding: utf-8 -*-
 #!/usr/bin/env python3
+# Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
+#  MIT License  (https://opensource.org/licenses/MIT)
+
+
+import torch
+torch.set_num_threads(1)
+
 import argparse
 import logging
-from pathlib import Path
+import os
 import sys
+from typing import Union, Dict, Any
+
+from funasr.utils import config_argparse
+from funasr.utils.cli_utils import get_commandline_args
+from funasr.utils.types import str2bool
+from funasr.utils.types import str2triple_str
+from funasr.utils.types import str_or_none
+
+import argparse
+import logging
 import os
+import sys
+import json
+from pathlib import Path
+from typing import Any
+from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 from typing import Dict
-from typing import Any
-from typing import List
 
+import math
 import numpy as np
 import torch
-from torch.nn.parallel import data_parallel
 from typeguard import check_argument_types
+from typeguard import check_return_type
 
-from funasr.tasks.lm import LMTask
-from funasr.datasets.preprocessor import LMPreprocessor
-from funasr.utils.cli_utils import get_commandline_args
 from funasr.fileio.datadir_writer import DatadirWriter
+from funasr.modules.scorers.scorer_interface import BatchScorerInterface
+from funasr.modules.subsampling import TooShortUttError
+from funasr.tasks.vad import VADTask
 from funasr.torch_utils.device_funcs import to_device
-from funasr.torch_utils.forward_adaptor import ForwardAdaptor
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.utils import config_argparse
-from funasr.utils.types import float_or_none
+from funasr.utils.cli_utils import get_commandline_args
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
-
-def inference(
-    output_dir: str,
-    batch_size: int,
-    dtype: str,
-    ngpu: int,
-    seed: int,
-    num_workers: int,
-    log_level: Union[int, str],
-    train_config: Optional[str],
-    model_file: Optional[str],
-    log_base: Optional[float],
-    key_file: Optional[str] = None,
-    allow_variable_data_keys: bool = False,
-    split_with_space: Optional[bool] = False,
-    seg_dict_file: Optional[str] = None,
-    data_path_and_name_and_type: Sequence[Tuple[str, str, str]] = None,
-    raw_inputs: Union[List[Any], bytes, str] = None,
-    **kwargs,
-):
-    inference_pipeline = inference_modelscope(
-        output_dir=output_dir,
-        raw_inputs=raw_inputs,
-        batch_size=batch_size,
-        dtype=dtype,
-        ngpu=ngpu,
-        seed=seed,
-        num_workers=num_workers,
-        log_level=log_level,
-        key_file=key_file,
-        train_config=train_config,
-        model_file=model_file,
-        log_base = log_base,
-        allow_variable_data_keys = allow_variable_data_keys,
-        split_with_space=split_with_space,
-        seg_dict_file=seg_dict_file,
+from funasr.utils import asr_utils, wav_utils, postprocess_utils
+from funasr.models.frontend.wav_frontend import WavFrontend, WavFrontendOnline
+from funasr.bin.vad_infer import Speech2VadSegment, Speech2VadSegmentOnline
+
+def inference_vad(
+        batch_size: int,
+        ngpu: int,
+        log_level: Union[int, str],
+        # data_path_and_name_and_type,
+        vad_infer_config: Optional[str],
+        vad_model_file: Optional[str],
+        vad_cmvn_file: Optional[str] = None,
+        # raw_inputs: Union[np.ndarray, torch.Tensor] = None,
+        key_file: Optional[str] = None,
+        allow_variable_data_keys: bool = False,
+        output_dir: Optional[str] = None,
+        dtype: str = "float32",
+        seed: int = 0,
+        num_workers: int = 1,
         **kwargs,
-    )
-    return inference_pipeline(data_path_and_name_and_type, raw_inputs)
-
-
-def inference_modelscope(
-    batch_size: int,
-    dtype: str,
-    ngpu: int,
-    seed: int,
-    num_workers: int,
-    log_level: Union[int, str],
-    key_file: Optional[str],
-    train_config: Optional[str],
-    model_file: Optional[str],
-    log_base: Optional[float] = 10,
-    allow_variable_data_keys: bool = False,
-    split_with_space: Optional[bool] = False,
-    seg_dict_file: Optional[str] = None,
-    output_dir: Optional[str] = None,
-    param_dict: dict = None,
-    **kwargs,
 ):
     assert check_argument_types()
-    ncpu = kwargs.get("ncpu", 1)
-    torch.set_num_threads(ncpu)
+    if batch_size > 1:
+        raise NotImplementedError("batch decoding is not implemented")
+
 
+    logging.basicConfig(
+        level=log_level,
+        format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
+    )
 
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
-
+        batch_size = 1
     # 1. Set random-seed
     set_all_random_seed(seed)
 
-    # 2. Build Model
-    model, train_args = LMTask.build_model_from_file(
-        train_config, model_file, device)
-    wrapped_model = ForwardAdaptor(model, "nll")
-    wrapped_model.to(dtype=getattr(torch, dtype)).to(device=device).eval()
-    logging.info(f"Model:\n{model}")
-
-    preprocessor = LMPreprocessor(
-        train=False,
-        token_type=train_args.token_type,
-        token_list=train_args.token_list,
-        bpemodel=train_args.bpemodel,
-        text_cleaner=train_args.cleaner,
-        g2p_type=train_args.g2p,
-        text_name="text",
-        non_linguistic_symbols=train_args.non_linguistic_symbols,
-        split_with_space=split_with_space,
-        seg_dict_file=seg_dict_file
+    # 2. Build speech2vadsegment
+    speech2vadsegment_kwargs = dict(
+        vad_infer_config=vad_infer_config,
+        vad_model_file=vad_model_file,
+        vad_cmvn_file=vad_cmvn_file,
+        device=device,
+        dtype=dtype,
     )
+    logging.info("speech2vadsegment_kwargs: {}".format(speech2vadsegment_kwargs))
+    speech2vadsegment = Speech2VadSegment(**speech2vadsegment_kwargs)
 
     def _forward(
-        data_path_and_name_and_type,
-        raw_inputs: Union[List[Any], bytes, str] = None,
-        output_dir_v2: Optional[str] = None,
-        param_dict: dict = None,
+            data_path_and_name_and_type,
+            raw_inputs: Union[np.ndarray, torch.Tensor] = None,
+            output_dir_v2: Optional[str] = None,
+            fs: dict = None,
+            param_dict: dict = None
     ):
-        results = []
+        # 3. Build data-iterator
+        if data_path_and_name_and_type is None and raw_inputs is not None:
+            if isinstance(raw_inputs, torch.Tensor):
+                raw_inputs = raw_inputs.numpy()
+            data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
+        loader = VADTask.build_streaming_iterator(
+            data_path_and_name_and_type,
+            dtype=dtype,
+            batch_size=batch_size,
+            key_file=key_file,
+            num_workers=num_workers,
+            preprocess_fn=VADTask.build_preprocess_fn(speech2vadsegment.vad_infer_args, False),
+            collate_fn=VADTask.build_collate_fn(speech2vadsegment.vad_infer_args, False),
+            allow_variable_data_keys=allow_variable_data_keys,
+            inference=True,
+        )
+
+        finish_count = 0
+        file_count = 1
+        # 7 .Start for-loop
+        # FIXME(kamo): The output format should be discussed about
         output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
         if output_path is not None:
             writer = DatadirWriter(output_path)
+            ibest_writer = writer[f"1best_recog"]
         else:
             writer = None
+            ibest_writer = None
+
+        vad_results = []
+        for keys, batch in loader:
+            assert isinstance(batch, dict), type(batch)
+            assert all(isinstance(s, str) for s in keys), keys
+            _bs = len(next(iter(batch.values())))
+            assert len(keys) == _bs, f"{len(keys)} != {_bs}"
+
+            # do vad segment
+            _, results = speech2vadsegment(**batch)
+            for i, _ in enumerate(keys):
+                if "MODELSCOPE_ENVIRONMENT" in os.environ and os.environ["MODELSCOPE_ENVIRONMENT"] == "eas":
+                    results[i] = json.dumps(results[i])
+                item = {'key': keys[i], 'value': results[i]}
+                vad_results.append(item)
+                if writer is not None:
+                    ibest_writer["text"][keys[i]] = "{}".format(results[i])
+
+        return vad_results
+
+    return _forward
+
+def inference_vad_online(
+        batch_size: int,
+        ngpu: int,
+        log_level: Union[int, str],
+        # data_path_and_name_and_type,
+        vad_infer_config: Optional[str],
+        vad_model_file: Optional[str],
+        vad_cmvn_file: Optional[str] = None,
+        # raw_inputs: Union[np.ndarray, torch.Tensor] = None,
+        key_file: Optional[str] = None,
+        allow_variable_data_keys: bool = False,
+        output_dir: Optional[str] = None,
+        dtype: str = "float32",
+        seed: int = 0,
+        num_workers: int = 1,
+        **kwargs,
+):
+    assert check_argument_types()
 
-        if raw_inputs != None:
-            line = raw_inputs.strip()
-            key = "lm demo"
-            if line=="":
-                item = {'key': key, 'value': ""}
-                results.append(item)
-                return results
-            batch = {}
-            batch['text'] = line
-            if preprocessor != None:
-                batch = preprocessor(key, batch)
-            
-            #  Force data-precision
-            for name in batch:
-                value = batch[name]
-                if not isinstance(value, np.ndarray):
-                    raise RuntimeError(
-                        f"All values must be converted to np.ndarray object "
-                        f'by preprocessing, but "{name}" is still {type(value)}.'
-                    )
-                # Cast to desired type
-                if value.dtype.kind == "f":
-                    value = value.astype("float32")
-                elif value.dtype.kind == "i":
-                    value = value.astype("long")
-                else:
-                    raise NotImplementedError(f"Not supported dtype: {value.dtype}")
-                batch[name] = value
-            
-            batch["text_lengths"] = torch.from_numpy(
-                np.array([len(batch["text"])], dtype='int32'))
-            batch["text"] = np.expand_dims(batch["text"], axis=0)
-
-            with torch.no_grad():
-                batch = to_device(batch, device)
-                if ngpu <= 1:
-                    nll, lengths = wrapped_model(**batch)
-                else:
-                    nll, lengths = data_parallel(
-                        wrapped_model, (), range(ngpu), module_kwargs=batch
-                    )
-                ## compute ppl
-                ppl_out_batch = ""
-                ids2tokens = preprocessor.token_id_converter.ids2tokens
-                for sent_ids, sent_nll in zip(batch['text'], nll):
-                    pre_word = "<s>"
-                    cur_word = None
-                    sent_lst = ids2tokens(sent_ids) + ['</s>']
-                    ppl_out = " ".join(sent_lst) + "\n"
-                    for word, word_nll in zip(sent_lst, sent_nll):
-                        cur_word = word
-                        word_nll = -word_nll.cpu()
-                        if log_base is None:
-                            word_prob = np.exp(word_nll)
-                        else:
-                            word_prob = log_base ** (word_nll / np.log(log_base))
-                        ppl_out += '    p( {cur} | {pre} ) = {prob} [ {word_nll} ]\n'.format(
-                            cur=cur_word, 
-                            pre=pre_word, 
-                            prob=round(word_prob.item(), 8),
-                            word_nll=round(word_nll.item(), 8)
-                            )
-                        pre_word = cur_word
-                    
-                    sent_nll_mean = sent_nll.mean().cpu().numpy()
-                    sent_nll_sum = sent_nll.sum().cpu().numpy()
-                    if log_base is None:
-                        sent_ppl = np.exp(sent_nll_mean)
-                    else:
-                        sent_ppl = log_base ** (sent_nll_mean / np.log(log_base))
-                    ppl_out += 'logprob= {sent_nll} ppl= {sent_ppl}\n\n'.format(
-                        sent_nll=round(-sent_nll_sum.item(), 4),
-                        sent_ppl=round(sent_ppl.item(), 4)
-                        )
-                    ppl_out_batch += ppl_out
-                    item = {'key': key, 'value': ppl_out}
-                    if writer is not None:
-                        writer["ppl"][key+":\n"] = ppl_out
-                    results.append(item)
 
-            return results
-                
+    logging.basicConfig(
+        level=log_level,
+        format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
+    )
+
+    if ngpu >= 1 and torch.cuda.is_available():
+        device = "cuda"
+    else:
+        device = "cpu"
+        batch_size = 1
+
+    # 1. Set random-seed
+    set_all_random_seed(seed)
+
+    # 2. Build speech2vadsegment
+    speech2vadsegment_kwargs = dict(
+        vad_infer_config=vad_infer_config,
+        vad_model_file=vad_model_file,
+        vad_cmvn_file=vad_cmvn_file,
+        device=device,
+        dtype=dtype,
+    )
+    logging.info("speech2vadsegment_kwargs: {}".format(speech2vadsegment_kwargs))
+    speech2vadsegment = Speech2VadSegmentOnline(**speech2vadsegment_kwargs)
+
+    def _forward(
+            data_path_and_name_and_type,
+            raw_inputs: Union[np.ndarray, torch.Tensor] = None,
+            output_dir_v2: Optional[str] = None,
+            fs: dict = None,
+            param_dict: dict = None,
+    ):
         # 3. Build data-iterator
-        loader = LMTask.build_streaming_iterator(
+        if data_path_and_name_and_type is None and raw_inputs is not None:
+            if isinstance(raw_inputs, torch.Tensor):
+                raw_inputs = raw_inputs.numpy()
+            data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
+        loader = VADTask.build_streaming_iterator(
             data_path_and_name_and_type,
             dtype=dtype,
             batch_size=batch_size,
             key_file=key_file,
             num_workers=num_workers,
-            preprocess_fn=preprocessor,
-            collate_fn=LMTask.build_collate_fn(train_args, False),
+            preprocess_fn=VADTask.build_preprocess_fn(speech2vadsegment.vad_infer_args, False),
+            collate_fn=VADTask.build_collate_fn(speech2vadsegment.vad_infer_args, False),
             allow_variable_data_keys=allow_variable_data_keys,
             inference=True,
         )
 
-        # 4. Start for-loop
-        total_nll = 0.0
-        total_ntokens = 0
-        ppl_out_all = ""
+        finish_count = 0
+        file_count = 1
+        # 7 .Start for-loop
+        # FIXME(kamo): The output format should be discussed about
+        output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
+        if output_path is not None:
+            writer = DatadirWriter(output_path)
+            ibest_writer = writer[f"1best_recog"]
+        else:
+            writer = None
+            ibest_writer = None
+
+        vad_results = []
+        if param_dict is None:
+            param_dict = dict()
+            param_dict['in_cache'] = dict()
+            param_dict['is_final'] = True
+        batch_in_cache = param_dict.get('in_cache', dict())
+        is_final = param_dict.get('is_final', False)
+        max_end_sil = param_dict.get('max_end_sil', 800)
         for keys, batch in loader:
             assert isinstance(batch, dict), type(batch)
             assert all(isinstance(s, str) for s in keys), keys
             _bs = len(next(iter(batch.values())))
             assert len(keys) == _bs, f"{len(keys)} != {_bs}"
+            batch['in_cache'] = batch_in_cache
+            batch['is_final'] = is_final
+            batch['max_end_sil'] = max_end_sil
+
+            # do vad segment
+            _, results, param_dict['in_cache'] = speech2vadsegment(**batch)
+            # param_dict['in_cache'] = batch['in_cache']
+            if results:
+                for i, _ in enumerate(keys):
+                    if results[i]:
+                        if "MODELSCOPE_ENVIRONMENT" in os.environ and os.environ["MODELSCOPE_ENVIRONMENT"] == "eas":
+                            results[i] = json.dumps(results[i])
+                        item = {'key': keys[i], 'value': results[i]}
+                        vad_results.append(item)
+                        if writer is not None:
+                            ibest_writer["text"][keys[i]] = "{}".format(results[i])
 
-            ppl_out_batch = ""
-            with torch.no_grad():
-                batch = to_device(batch, device)
-                if ngpu <= 1:
-                    # NOTE(kamo): data_parallel also should work with ngpu=1,
-                    # but for debuggability it's better to keep this block.
-                    nll, lengths = wrapped_model(**batch)
-                else:
-                    nll, lengths = data_parallel(
-                        wrapped_model, (), range(ngpu), module_kwargs=batch
-                    )
-                ## print ppl
-                ids2tokens = preprocessor.token_id_converter.ids2tokens
-                for key, sent_ids, sent_nll in zip(keys, batch['text'], nll):
-                    pre_word = "<s>"
-                    cur_word = None
-                    sent_lst = ids2tokens(sent_ids) + ['</s>']
-                    ppl_out = " ".join(sent_lst) + "\n"
-                    for word, word_nll in zip(sent_lst, sent_nll):
-                        cur_word = word
-                        word_nll = -word_nll.cpu()
-                        if log_base is None:
-                            word_prob = np.exp(word_nll)
-                        else:
-                            word_prob = log_base ** (word_nll / np.log(log_base))
-                        ppl_out += '    p( {cur} | {pre} ) = {prob} [ {word_nll} ]\n'.format(
-                            cur=cur_word, 
-                            pre=pre_word, 
-                            prob=round(word_prob.item(), 8),
-                            word_nll=round(word_nll.item(), 8)
-                            )
-                        pre_word = cur_word
-                    
-                    sent_nll_mean = sent_nll.mean().cpu().numpy()
-                    sent_nll_sum = sent_nll.sum().cpu().numpy()
-                    if log_base is None:
-                        sent_ppl = np.exp(sent_nll_mean)
-                    else:
-                        sent_ppl = log_base ** (sent_nll_mean / np.log(log_base))
-                    ppl_out += 'logprob= {sent_nll} ppl= {sent_ppl}\n\n'.format(
-                        sent_nll=round(-sent_nll_sum.item(), 4),
-                        sent_ppl=round(sent_ppl.item(), 4)
-                        )
-                    ppl_out_batch += ppl_out
-                    utt2nll = round(-sent_nll_sum.item(), 5)
-                    item = {'key': key, 'value': ppl_out}
-                    if writer is not None:
-                        writer["ppl"][key+":\n"] = ppl_out
-                        writer["utt2nll"][key] = str(utt2nll)
-                    results.append(item)
-
-            ppl_out_all += ppl_out_batch
-            
-            assert _bs == len(nll) == len(lengths), (_bs, len(nll), len(lengths))
-            # nll: (B, L) -> (B,)
-            nll = nll.detach().cpu().numpy().sum(1)
-            # lengths: (B,)
-            lengths = lengths.detach().cpu().numpy()
-            total_nll += nll.sum()
-            total_ntokens += lengths.sum()
+        return vad_results
 
-        if log_base is None:
-            ppl = np.exp(total_nll / total_ntokens)
-        else:
-            ppl = log_base ** (total_nll / total_ntokens / np.log(log_base))
+    return _forward
 
-        avg_ppl = 'logprob= {total_nll} ppl= {total_ppl}\n'.format(
-            total_nll=round(-total_nll.item(), 4),
-            total_ppl=round(ppl.item(), 4)
-            )
-        item = {'key': 'AVG PPL', 'value': avg_ppl}
-        ppl_out_all += avg_ppl
-        if writer is not None:
-            writer["ppl"]["AVG PPL : "] = avg_ppl
-        results.append(item)
 
-        return results
 
-    return _forward
 
+def inference_launch(mode, **kwargs):
+    if mode == "offline":
+        return inference_vad(**kwargs)
+    elif mode == "online":
+        return inference_vad_online(**kwargs)
+    else:
+        logging.info("Unknown decoding mode: {}".format(mode))
+        return None
 
 def get_parser():
     parser = config_argparse.ArgumentParser(
-        description="Calc perplexity",
+        description="VAD Decoding",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
+    # Note(kamo): Use '_' instead of '-' as separator.
+    # '-' is confusing if written in yaml.
     parser.add_argument(
         "--log_level",
         type=lambda x: x.upper(),
         default="INFO",
         choices=("CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET"),
         help="The verbose level of logging",
     )
 
-    parser.add_argument("--output_dir", type=str, required=False)
+    parser.add_argument("--output_dir", type=str, required=True)
     parser.add_argument(
         "--ngpu",
         type=int,
         default=0,
         help="The number of gpus. 0 indicates CPU mode",
     )
+    parser.add_argument(
+        "--njob",
+        type=int,
+        default=1,
+        help="The number of jobs for each gpu",
+    )
+    parser.add_argument(
+        "--gpuid_list",
+        type=str,
+        default="",
+        help="The visible gpus",
+    )
     parser.add_argument("--seed", type=int, default=0, help="Random seed")
     parser.add_argument(
         "--dtype",
         default="float32",
         choices=["float16", "float32", "float64"],
         help="Data type",
     )
     parser.add_argument(
         "--num_workers",
         type=int,
         default=1,
         help="The number of workers used for DataLoader",
     )
-    parser.add_argument(
-        "--batch_size",
-        type=int,
-        default=1,
-        help="The batch size for inference",
-    )
-    parser.add_argument(
-        "--log_base",
-        type=float_or_none,
-        default=10,
-        help="The base of logarithm for Perplexity. "
-             "If None, napier's constant is used.",
-        required=False
-    )
 
     group = parser.add_argument_group("Input data related")
     group.add_argument(
         "--data_path_and_name_and_type",
         type=str2triple_str,
+        required=True,
         action="append",
-        required=False
-    )
-    group.add_argument(
-        "--raw_inputs",
-        type=str,
-        required=False
     )
     group.add_argument("--key_file", type=str_or_none)
     group.add_argument("--allow_variable_data_keys", type=str2bool, default=False)
 
-    group.add_argument("--split_with_space", type=str2bool, default=False)
-    group.add_argument("--seg_dict_file", type=str_or_none)
-
     group = parser.add_argument_group("The model configuration related")
-    group.add_argument("--train_config", type=str)
-    group.add_argument("--model_file", type=str)
+    group.add_argument(
+        "--vad_infer_config",
+        type=str,
+        help="VAD infer configuration",
+    )
+    group.add_argument(
+        "--vad_model_file",
+        type=str,
+        help="VAD model parameter file",
+    )
+    group.add_argument(
+        "--vad_cmvn_file",
+        type=str,
+        help="Global CMVN file",
+    )
+    group.add_argument(
+        "--vad_train_config",
+        type=str,
+        help="VAD training configuration",
+    )
 
+    group = parser.add_argument_group("The inference configuration related")
+    group.add_argument(
+        "--batch_size",
+        type=int,
+        default=1,
+        help="The batch size for inference",
+    )
     return parser
 
 
 def main(cmd=None):
     print(get_commandline_args(), file=sys.stderr)
     parser = get_parser()
+    parser.add_argument(
+        "--mode",
+        type=str,
+        default="vad",
+        help="The decoding mode",
+    )
     args = parser.parse_args(cmd)
     kwargs = vars(args)
-    inference(**kwargs)
+    kwargs.pop("config", None)
+
+    # set logging messages
+    logging.basicConfig(
+        level=args.log_level,
+        format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
+    )
+    logging.info("Decoding args: {}".format(kwargs))
+
+    # gpu setting
+    if args.ngpu > 0:
+        jobid = int(args.output_dir.split(".")[-1])
+        gpuid = args.gpuid_list.split(",")[(jobid - 1) // args.njob]
+        os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
+        os.environ["CUDA_VISIBLE_DEVICES"] = gpuid
+
+    inference_pipeline = inference_launch(**kwargs)
+    return inference_pipeline(kwargs["data_path_and_name_and_type"])
 
 if __name__ == "__main__":
     main()
-
```

### Comparing `funasr-0.5.3/funasr/bin/punctuation_infer.py` & `funasr-0.5.4/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,100 +1,102 @@
-#!/usr/bin/env python3
-import argparse
-import logging
-from pathlib import Path
-import sys
-from typing import Optional
-from typing import Sequence
-from typing import Tuple
-from typing import Union
-from typing import Any
-from typing import List
+# -*- encoding: utf-8 -*-
+# Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
+#  MIT License  (https://opensource.org/licenses/MIT)
 
+import os.path
+from pathlib import Path
+from typing import List, Union, Tuple
 import numpy as np
-import torch
-from typeguard import check_argument_types
 
-from funasr.datasets.preprocessor import CodeMixTokenizerCommonPreprocessor
-from funasr.utils.cli_utils import get_commandline_args
-from funasr.tasks.punctuation import PunctuationTask
-from funasr.torch_utils.device_funcs import to_device
-from funasr.torch_utils.forward_adaptor import ForwardAdaptor
-from funasr.torch_utils.set_all_random_seed import set_all_random_seed
-from funasr.utils import config_argparse
-from funasr.utils.types import str2triple_str
-from funasr.utils.types import str_or_none
-from funasr.datasets.preprocessor import split_to_mini_sentence
-
-
-class Text2Punc:
-
-    def __init__(
-        self,
-        train_config: Optional[str],
-        model_file: Optional[str],
-        device: str = "cpu",
-        dtype: str = "float32",
-    ):
-        #  Build Model
-        model, train_args = PunctuationTask.build_model_from_file(train_config, model_file, device)
-        self.device = device
-        # Wrape model to make model.nll() data-parallel
-        self.wrapped_model = ForwardAdaptor(model, "inference")
-        self.wrapped_model.to(dtype=getattr(torch, dtype)).to(device=device).eval()
-        # logging.info(f"Model:\n{model}")
-        self.punc_list = train_args.punc_list
+from .utils.utils import (ONNXRuntimeError,
+                          OrtInferSession, get_logger,
+                          read_yaml)
+from .utils.utils import (TokenIDConverter, split_to_mini_sentence,code_mix_split_words)
+logging = get_logger()
+
+
+class CT_Transformer():
+    """
+    Author: Speech Lab of DAMO Academy, Alibaba Group
+    CT-Transformer: Controllable time-delay transformer for real-time punctuation prediction and disfluency detection
+    https://arxiv.org/pdf/2003.01309.pdf
+    """
+    def __init__(self, model_dir: Union[str, Path] = None,
+                 batch_size: int = 1,
+                 device_id: Union[str, int] = "-1",
+                 quantize: bool = False,
+                 intra_op_num_threads: int = 4,
+                 cache_dir: str = None,
+                 ):
+    
+        if not Path(model_dir).exists():
+            from modelscope.hub.snapshot_download import snapshot_download
+            try:
+                model_dir = snapshot_download(model_dir, cache_dir=cache_dir)
+            except:
+                raise "model_dir must be model_name in modelscope or local path downloaded from modelscope, but is {}".format(
+                    model_dir)
+    
+        model_file = os.path.join(model_dir, 'model.onnx')
+        if quantize:
+            model_file = os.path.join(model_dir, 'model_quant.onnx')
+        if not os.path.exists(model_file):
+            print(".onnx is not exist, begin to export onnx")
+            from funasr.export.export_model import ModelExport
+            export_model = ModelExport(
+                cache_dir=cache_dir,
+                onnx=True,
+                device="cpu",
+                quant=quantize,
+            )
+            export_model.export(model_dir)
+            
+        config_file = os.path.join(model_dir, 'punc.yaml')
+        config = read_yaml(config_file)
+
+        self.converter = TokenIDConverter(config['token_list'])
+        self.ort_infer = OrtInferSession(model_file, device_id, intra_op_num_threads=intra_op_num_threads)
+        self.batch_size = 1
+        self.punc_list = config['punc_list']
         self.period = 0
         for i in range(len(self.punc_list)):
             if self.punc_list[i] == ",":
                 self.punc_list[i] = "，"
             elif self.punc_list[i] == "?":
                 self.punc_list[i] = "？"
             elif self.punc_list[i] == "。":
                 self.period = i
-        self.preprocessor = CodeMixTokenizerCommonPreprocessor(
-            train=False,
-            token_type=train_args.token_type,
-            token_list=train_args.token_list,
-            bpemodel=train_args.bpemodel,
-            text_cleaner=train_args.cleaner,
-            g2p_type=train_args.g2p,
-            text_name="text",
-            non_linguistic_symbols=train_args.non_linguistic_symbols,
-        )
 
-    @torch.no_grad()
     def __call__(self, text: Union[list, str], split_size=20):
-        data = {"text": text}
-        result = self.preprocessor(data=data, uid="12938712838719")
-        split_text = self.preprocessor.pop_split_text_data(result)
+        split_text = code_mix_split_words(text)
+        split_text_id = self.converter.tokens2ids(split_text)
         mini_sentences = split_to_mini_sentence(split_text, split_size)
-        mini_sentences_id = split_to_mini_sentence(data["text"], split_size)
+        mini_sentences_id = split_to_mini_sentence(split_text_id, split_size)
         assert len(mini_sentences) == len(mini_sentences_id)
         cache_sent = []
-        cache_sent_id = torch.from_numpy(np.array([], dtype='int32'))
+        cache_sent_id = []
         new_mini_sentence = ""
         new_mini_sentence_punc = []
         cache_pop_trigger_limit = 200
         for mini_sentence_i in range(len(mini_sentences)):
             mini_sentence = mini_sentences[mini_sentence_i]
             mini_sentence_id = mini_sentences_id[mini_sentence_i]
             mini_sentence = cache_sent + mini_sentence
-            mini_sentence_id = np.concatenate((cache_sent_id, mini_sentence_id), axis=0)
+            mini_sentence_id = np.array(cache_sent_id + mini_sentence_id, dtype='int32')
             data = {
-                "text": torch.unsqueeze(torch.from_numpy(mini_sentence_id), 0),
-                "text_lengths": torch.from_numpy(np.array([len(mini_sentence_id)], dtype='int32')),
+                "text": mini_sentence_id[None,:],
+                "text_lengths": np.array([len(mini_sentence_id)], dtype='int32'),
             }
-            data = to_device(data, self.device)
-            y, _ = self.wrapped_model(**data)
-            _, indices = y.view(-1, y.shape[-1]).topk(1, dim=1)
-            punctuations = indices
-            if indices.size()[0] != 1:
-                punctuations = torch.squeeze(indices)
-            assert punctuations.size()[0] == len(mini_sentence)
+            try:
+                outputs = self.infer(data['text'], data['text_lengths'])
+                y = outputs[0]
+                punctuations = np.argmax(y,axis=-1)[0]
+                assert punctuations.size == len(mini_sentence)
+            except ONNXRuntimeError:
+                logging.warning("error")
 
             # Search for the last Period/QuestionMark as cache
             if mini_sentence_i < len(mini_sentences) - 1:
                 sentenceEnd = -1
                 last_comma_index = -1
                 for i in range(len(punctuations) - 2, 1, -1):
                     if self.punc_list[punctuations[i]] == "。" or self.punc_list[punctuations[i]] == "？":
@@ -104,23 +106,19 @@
                         last_comma_index = i
 
                 if sentenceEnd < 0 and len(mini_sentence) > cache_pop_trigger_limit and last_comma_index >= 0:
                     # The sentence it too long, cut off at a comma.
                     sentenceEnd = last_comma_index
                     punctuations[sentenceEnd] = self.period
                 cache_sent = mini_sentence[sentenceEnd + 1:]
-                cache_sent_id = mini_sentence_id[sentenceEnd + 1:]
+                cache_sent_id = mini_sentence_id[sentenceEnd + 1:].tolist()
                 mini_sentence = mini_sentence[0:sentenceEnd + 1]
                 punctuations = punctuations[0:sentenceEnd + 1]
 
-            # if len(punctuations) == 0:
-            #    continue
-
-            punctuations_np = punctuations.cpu().numpy()
-            new_mini_sentence_punc += [int(x) for x in punctuations_np]
+            new_mini_sentence_punc += [int(x) for x in punctuations]
             words_with_punc = []
             for i in range(len(mini_sentence)):
                 if i > 0:
                     if len(mini_sentence[i][0].encode()) == 1 and len(mini_sentence[i - 1][0].encode()) == 1:
                         mini_sentence[i] = " " + mini_sentence[i]
                 words_with_punc.append(mini_sentence[i])
                 if self.punc_list[punctuations[i]] != "_":
@@ -134,187 +132,149 @@
                     new_mini_sentence_out = new_mini_sentence[:-1] + "。"
                     new_mini_sentence_punc_out = new_mini_sentence_punc[:-1] + [self.period]
                 elif new_mini_sentence[-1] != "。" and new_mini_sentence[-1] != "？":
                     new_mini_sentence_out = new_mini_sentence + "。"
                     new_mini_sentence_punc_out = new_mini_sentence_punc[:-1] + [self.period]
         return new_mini_sentence_out, new_mini_sentence_punc_out
 
+    def infer(self, feats: np.ndarray,
+              feats_len: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
+        outputs = self.ort_infer([feats, feats_len])
+        return outputs
+
+
+class CT_Transformer_VadRealtime(CT_Transformer):
+    """
+    Author: Speech Lab of DAMO Academy, Alibaba Group
+    CT-Transformer: Controllable time-delay transformer for real-time punctuation prediction and disfluency detection
+    https://arxiv.org/pdf/2003.01309.pdf
+    """
+    def __init__(self, model_dir: Union[str, Path] = None,
+                 batch_size: int = 1,
+                 device_id: Union[str, int] = "-1",
+                 quantize: bool = False,
+                 intra_op_num_threads: int = 4,
+                 cache_dir: str = None
+                 ):
+        super(CT_Transformer_VadRealtime, self).__init__(model_dir, batch_size, device_id, quantize, intra_op_num_threads, cache_dir=cache_dir)
+
+    def __call__(self, text: str, param_dict: map, split_size=20):
+        cache_key = "cache"
+        assert cache_key in param_dict
+        cache = param_dict[cache_key]
+        if cache is not None and len(cache) > 0:
+            precache = "".join(cache)
+        else:
+            precache = ""
+            cache = []
+        full_text = precache + " " + text
+        split_text = code_mix_split_words(full_text)
+        split_text_id = self.converter.tokens2ids(split_text)
+        mini_sentences = split_to_mini_sentence(split_text, split_size)
+        mini_sentences_id = split_to_mini_sentence(split_text_id, split_size)
+        new_mini_sentence_punc = []
+        assert len(mini_sentences) == len(mini_sentences_id)
+
+        cache_sent = []
+        cache_sent_id = np.array([], dtype='int32')
+        sentence_punc_list = []
+        sentence_words_list = []
+        cache_pop_trigger_limit = 200
+        skip_num = 0
+        for mini_sentence_i in range(len(mini_sentences)):
+            mini_sentence = mini_sentences[mini_sentence_i]
+            mini_sentence_id = mini_sentences_id[mini_sentence_i]
+            mini_sentence = cache_sent + mini_sentence
+            mini_sentence_id = np.concatenate((cache_sent_id, mini_sentence_id), axis=0,dtype='int32')
+            text_length = len(mini_sentence_id)
+            vad_mask = self.vad_mask(text_length, len(cache))[None, None, :, :].astype(np.float32)
+            data = {
+                "input": mini_sentence_id[None,:],
+                "text_lengths": np.array([text_length], dtype='int32'),
+                "vad_mask": vad_mask,
+                "sub_masks": vad_mask
+            }
+            try:
+                outputs = self.infer(data['input'], data['text_lengths'], data['vad_mask'], data["sub_masks"])
+                y = outputs[0]
+                punctuations = np.argmax(y,axis=-1)[0]
+                assert punctuations.size == len(mini_sentence)
+            except ONNXRuntimeError:
+                logging.warning("error")
 
-def inference(
-    batch_size: int,
-    dtype: str,
-    ngpu: int,
-    seed: int,
-    num_workers: int,
-    output_dir: str,
-    log_level: Union[int, str],
-    train_config: Optional[str],
-    model_file: Optional[str],
-    key_file: Optional[str] = None,
-    data_path_and_name_and_type: Sequence[Tuple[str, str, str]] = None,
-    raw_inputs: Union[List[Any], bytes, str] = None,
-    cache: List[Any] = None,
-    param_dict: dict = None,
-    **kwargs,
-):
-    inference_pipeline = inference_modelscope(
-        output_dir=output_dir,
-        batch_size=batch_size,
-        dtype=dtype,
-        ngpu=ngpu,
-        seed=seed,
-        num_workers=num_workers,
-        log_level=log_level,
-        key_file=key_file,
-        train_config=train_config,
-        model_file=model_file,
-        param_dict=param_dict,
-        **kwargs,
-    )
-    return inference_pipeline(data_path_and_name_and_type, raw_inputs)
-
-
-def inference_modelscope(
-    batch_size: int,
-    dtype: str,
-    ngpu: int,
-    seed: int,
-    num_workers: int,
-    log_level: Union[int, str],
-    key_file: Optional[str],
-    train_config: Optional[str],
-    model_file: Optional[str],
-    output_dir: Optional[str] = None,
-    param_dict: dict = None,
-    **kwargs,
-):
-    assert check_argument_types()
-    logging.basicConfig(
-        level=log_level,
-        format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
-    )
-
-    if ngpu >= 1 and torch.cuda.is_available():
-        device = "cuda"
-    else:
-        device = "cpu"
-
-    # 1. Set random-seed
-    set_all_random_seed(seed)
-    text2punc = Text2Punc(train_config, model_file, device)
-
-    def _forward(
-        data_path_and_name_and_type,
-        raw_inputs: Union[List[Any], bytes, str] = None,
-        output_dir_v2: Optional[str] = None,
-        cache: List[Any] = None,
-        param_dict: dict = None,
-    ):
-        results = []
-        split_size = 20
-
-        if raw_inputs != None:
-            line = raw_inputs.strip()
-            key = "demo"
-            if line == "":
-                item = {'key': key, 'value': ""}
-                results.append(item)
-                return results
-            result, _ = text2punc(line)
-            item = {'key': key, 'value': result}
-            results.append(item)
-            return results
-
-        for inference_text, _, _ in data_path_and_name_and_type:
-            with open(inference_text, "r", encoding="utf-8") as fin:
-                for line in fin:
-                    line = line.strip()
-                    segs = line.split("\t")
-                    if len(segs) != 2:
-                        continue
-                    key = segs[0]
-                    if len(segs[1]) == 0:
-                        continue
-                    result, _ = text2punc(segs[1])
-                    item = {'key': key, 'value': result}
-                    results.append(item)
-        output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
-        if output_path != None:
-            output_file_name = "infer.out"
-            Path(output_path).mkdir(parents=True, exist_ok=True)
-            output_file_path = (Path(output_path) / output_file_name).absolute()
-            with open(output_file_path, "w", encoding="utf-8") as fout:
-                for item_i in results:
-                    key_out = item_i["key"]
-                    value_out = item_i["value"]
-                    fout.write(f"{key_out}\t{value_out}\n")
-        return results
-
-    return _forward
-
-
-def get_parser():
-    parser = config_argparse.ArgumentParser(
-        description="Punctuation inference",
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-    )
-
-    parser.add_argument(
-        "--log_level",
-        type=lambda x: x.upper(),
-        default="INFO",
-        choices=("CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET"),
-        help="The verbose level of logging",
-    )
-
-    parser.add_argument("--output_dir", type=str, required=False)
-    parser.add_argument(
-        "--ngpu",
-        type=int,
-        default=0,
-        help="The number of gpus. 0 indicates CPU mode",
-    )
-    parser.add_argument("--seed", type=int, default=0, help="Random seed")
-    parser.add_argument(
-        "--dtype",
-        default="float32",
-        choices=["float16", "float32", "float64"],
-        help="Data type",
-    )
-    parser.add_argument(
-        "--num_workers",
-        type=int,
-        default=1,
-        help="The number of workers used for DataLoader",
-    )
-    parser.add_argument(
-        "--batch_size",
-        type=int,
-        default=1,
-        help="The batch size for inference",
-    )
-
-    group = parser.add_argument_group("Input data related")
-    group.add_argument("--data_path_and_name_and_type", type=str2triple_str, action="append", required=False)
-    group.add_argument("--raw_inputs", type=str, required=False)
-    group.add_argument("--cache", type=list, required=False)
-    group.add_argument("--param_dict", type=dict, required=False)
-    group.add_argument("--key_file", type=str_or_none)
-
-    group = parser.add_argument_group("The model configuration related")
-    group.add_argument("--train_config", type=str)
-    group.add_argument("--model_file", type=str)
-
-    return parser
-
-
-def main(cmd=None):
-    print(get_commandline_args(), file=sys.stderr)
-    parser = get_parser()
-    args = parser.parse_args(cmd)
-    kwargs = vars(args)
-    # kwargs.pop("config", None)
-    inference(**kwargs)
+            # Search for the last Period/QuestionMark as cache
+            if mini_sentence_i < len(mini_sentences) - 1:
+                sentenceEnd = -1
+                last_comma_index = -1
+                for i in range(len(punctuations) - 2, 1, -1):
+                    if self.punc_list[punctuations[i]] == "。" or self.punc_list[punctuations[i]] == "？":
+                        sentenceEnd = i
+                        break
+                    if last_comma_index < 0 and self.punc_list[punctuations[i]] == "，":
+                        last_comma_index = i
+
+                if sentenceEnd < 0 and len(mini_sentence) > cache_pop_trigger_limit and last_comma_index >= 0:
+                    # The sentence it too long, cut off at a comma.
+                    sentenceEnd = last_comma_index
+                    punctuations[sentenceEnd] = self.period
+                cache_sent = mini_sentence[sentenceEnd + 1:]
+                cache_sent_id = mini_sentence_id[sentenceEnd + 1:]
+                mini_sentence = mini_sentence[0:sentenceEnd + 1]
+                punctuations = punctuations[0:sentenceEnd + 1]
 
+            punctuations_np = [int(x) for x in punctuations]
+            new_mini_sentence_punc += punctuations_np
+            sentence_punc_list += [self.punc_list[int(x)] for x in punctuations_np]
+            sentence_words_list += mini_sentence
+
+        assert len(sentence_punc_list) == len(sentence_words_list)
+        words_with_punc = []
+        sentence_punc_list_out = []
+        for i in range(0, len(sentence_words_list)):
+            if i > 0:
+                if len(sentence_words_list[i][0].encode()) == 1 and len(sentence_words_list[i - 1][-1].encode()) == 1:
+                    sentence_words_list[i] = " " + sentence_words_list[i]
+            if skip_num < len(cache):
+                skip_num += 1
+            else:
+                words_with_punc.append(sentence_words_list[i])
+            if skip_num >= len(cache):
+                sentence_punc_list_out.append(sentence_punc_list[i])
+                if sentence_punc_list[i] != "_":
+                    words_with_punc.append(sentence_punc_list[i])
+        sentence_out = "".join(words_with_punc)
+
+        sentenceEnd = -1
+        for i in range(len(sentence_punc_list) - 2, 1, -1):
+            if sentence_punc_list[i] == "。" or sentence_punc_list[i] == "？":
+                sentenceEnd = i
+                break
+        cache_out = sentence_words_list[sentenceEnd + 1:]
+        if sentence_out[-1] in self.punc_list:
+            sentence_out = sentence_out[:-1]
+            sentence_punc_list_out[-1] = "_"
+        param_dict[cache_key] = cache_out
+        return sentence_out, sentence_punc_list_out, cache_out
+
+    def vad_mask(self, size, vad_pos, dtype=np.bool):
+        """Create mask for decoder self-attention.
+
+        :param int size: size of mask
+        :param int vad_pos: index of vad index
+        :param torch.dtype dtype: result dtype
+        :rtype: torch.Tensor (B, Lmax, Lmax)
+        """
+        ret = np.ones((size, size), dtype=dtype)
+        if vad_pos <= 0 or vad_pos >= size:
+            return ret
+        sub_corner = np.zeros(
+            (vad_pos - 1, size - vad_pos), dtype=dtype)
+        ret[0:vad_pos - 1, vad_pos:] = sub_corner
+        return ret
+
+    def infer(self, feats: np.ndarray,
+              feats_len: np.ndarray,
+              vad_mask: np.ndarray,
+              sub_masks: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
+        outputs = self.ort_infer([feats, feats_len, vad_mask, sub_masks])
+        return outputs
 
-if __name__ == "__main__":
-    main()
```

### Comparing `funasr-0.5.3/funasr/bin/punctuation_infer_vadrealtime.py` & `funasr-0.5.4/funasr/tasks/data2vec.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,311 +1,376 @@
-#!/usr/bin/env python3
 import argparse
-import logging
-from pathlib import Path
-import sys
+from typing import Callable
+from typing import Collection
+from typing import Dict
+from typing import List
 from typing import Optional
-from typing import Sequence
 from typing import Tuple
-from typing import Union
-from typing import Any
-from typing import List
 
 import numpy as np
 import torch
 from typeguard import check_argument_types
+from typeguard import check_return_type
 
-from funasr.datasets.preprocessor import CodeMixTokenizerCommonPreprocessor
-from funasr.utils.cli_utils import get_commandline_args
-from funasr.tasks.punctuation import PunctuationTask
-from funasr.torch_utils.device_funcs import to_device
-from funasr.torch_utils.forward_adaptor import ForwardAdaptor
-from funasr.torch_utils.set_all_random_seed import set_all_random_seed
-from funasr.utils import config_argparse
-from funasr.utils.types import str2triple_str
+from funasr.datasets.collate_fn import CommonCollateFn
+from funasr.datasets.preprocessor import CommonPreprocessor
+from funasr.layers.abs_normalize import AbsNormalize
+from funasr.layers.global_mvn import GlobalMVN
+from funasr.layers.utterance_mvn import UtteranceMVN
+from funasr.models.data2vec import Data2VecPretrainModel
+from funasr.models.encoder.abs_encoder import AbsEncoder
+from funasr.models.encoder.data2vec_encoder import Data2VecEncoder
+from funasr.models.frontend.abs_frontend import AbsFrontend
+from funasr.models.frontend.default import DefaultFrontend
+from funasr.models.frontend.windowing import SlidingWindow
+from funasr.models.preencoder.abs_preencoder import AbsPreEncoder
+from funasr.models.preencoder.sinc import LightweightSincConvs
+from funasr.models.specaug.abs_specaug import AbsSpecAug
+from funasr.models.specaug.specaug import SpecAug
+from funasr.tasks.abs_task import AbsTask
+from funasr.text.phoneme_tokenizer import g2p_choices
+from funasr.torch_utils.initialize import initialize
+from funasr.train.class_choices import ClassChoices
+from funasr.train.trainer import Trainer
+from funasr.utils.types import float_or_none
+from funasr.utils.types import int_or_none
+from funasr.utils.types import str2bool
 from funasr.utils.types import str_or_none
-from funasr.datasets.preprocessor import split_to_mini_sentence
 
+frontend_choices = ClassChoices(
+    name="frontend",
+    classes=dict(default=DefaultFrontend, sliding_window=SlidingWindow),
+    type_check=AbsFrontend,
+    default="default",
+)
+specaug_choices = ClassChoices(
+    name="specaug",
+    classes=dict(specaug=SpecAug),
+    type_check=AbsSpecAug,
+    default=None,
+    optional=True,
+)
+normalize_choices = ClassChoices(
+    "normalize",
+    classes=dict(
+        global_mvn=GlobalMVN,
+        utterance_mvn=UtteranceMVN,
+    ),
+    type_check=AbsNormalize,
+    default=None,
+    optional=True,
+)
+preencoder_choices = ClassChoices(
+    name="preencoder",
+    classes=dict(
+        sinc=LightweightSincConvs,
+    ),
+    type_check=AbsPreEncoder,
+    default=None,
+    optional=True,
+)
+encoder_choices = ClassChoices(
+    "encoder",
+    classes=dict(
+        data2vec_encoder=Data2VecEncoder,
+    ),
+    type_check=AbsEncoder,
+    default="data2vec_encoder",
+)
+model_choices = ClassChoices(
+    "model",
+    classes=dict(
+        data2vec=Data2VecPretrainModel,
+    ),
+    default="data2vec",
+)
+
+
+class Data2VecTask(AbsTask):
+    # If you need more than one optimizers, change this value
+    num_optimizers: int = 1
+
+    # Add variable objects configurations
+    class_choices_list = [
+        # --frontend and --frontend_conf
+        frontend_choices,
+        # --specaug and --specaug_conf
+        specaug_choices,
+        # --normalize and --normalize_conf
+        normalize_choices,
+        # --preencoder and --preencoder_conf
+        preencoder_choices,
+        # --encoder and --encoder_conf
+        encoder_choices,
+        # --model and --model_conf
+        model_choices,
+    ]
+
+    # If you need to modify train() or eval() procedures, change Trainer class here
+    trainer = Trainer
+
+    @classmethod
+    def add_task_arguments(cls, parser: argparse.ArgumentParser):
+        group = parser.add_argument_group(description="Task related")
+
+        # NOTE(kamo): add_arguments(..., required=True) can't be used
+        # to provide --print_config mode. Instead of it, do as
+        group.add_argument(
+            "--token_list",
+            type=str_or_none,
+            default=None,
+            help="A text mapping int-id to token",
+        )
+        group.add_argument(
+            "--init",
+            type=lambda x: str_or_none(x.lower()),
+            default=None,
+            help="The initialization method",
+            choices=[
+                "chainer",
+                "xavier_uniform",
+                "xavier_normal",
+                "kaiming_uniform",
+                "kaiming_normal",
+                None,
+            ],
+        )
+
+        group.add_argument(
+            "--input_size",
+            type=int_or_none,
+            default=None,
+            help="The number of input dimension of the feature",
+        )
+
+        group = parser.add_argument_group(description="Preprocess related")
+        group.add_argument(
+            "--use_preprocessor",
+            type=str2bool,
+            default=True,
+            help="Apply preprocessing to data or not",
+        )
+        group.add_argument(
+            "--token_type",
+            type=str,
+            default=None,
+            choices=["bpe", "char", "word", "phn"],
+            help="The text will be tokenized " "in the specified level token",
+        )
+
+        group.add_argument(
+            "--feats_type",
+            type=str,
+            default='fbank',
+            help="feats type, e.g. fbank, wav, ark_wav(needed to be scale normalization)",
+        )
+
+        group.add_argument(
+            "--bpemodel",
+            type=str_or_none,
+            default=None,
+            help="The model file of sentencepiece",
+        )
+        parser.add_argument(
+            "--non_linguistic_symbols",
+            type=str_or_none,
+            help="non_linguistic_symbols file path",
+        )
+        parser.add_argument(
+            "--cleaner",
+            type=str_or_none,
+            choices=[None, "tacotron", "jaconv", "vietnamese"],
+            default=None,
+            help="Apply text cleaning",
+        )
+        parser.add_argument(
+            "--g2p",
+            type=str_or_none,
+            choices=g2p_choices,
+            default=None,
+            help="Specify g2p method if --token_type=phn",
+        )
+        parser.add_argument(
+            "--speech_volume_normalize",
+            type=float_or_none,
+            default=None,
+            help="Scale the maximum amplitude to the given value.",
+        )
+        parser.add_argument(
+            "--rir_scp",
+            type=str_or_none,
+            default=None,
+            help="The file path of rir scp file.",
+        )
+        parser.add_argument(
+            "--rir_apply_prob",
+            type=float,
+            default=1.0,
+            help="THe probability for applying RIR convolution.",
+        )
+        parser.add_argument(
+            "--noise_scp",
+            type=str_or_none,
+            default=None,
+            help="The file path of noise scp file.",
+        )
+        parser.add_argument(
+            "--noise_apply_prob",
+            type=float,
+            default=1.0,
+            help="The probability applying Noise adding.",
+        )
+        parser.add_argument(
+            "--noise_db_range",
+            type=str,
+            default="13_15",
+            help="The range of noise decibel level.",
+        )
+        parser.add_argument(
+            "--pred_masked_weight",
+            type=float,
+            default=1.0,
+            help="weight for predictive loss for masked frames",
+        )
+        parser.add_argument(
+            "--pred_nomask_weight",
+            type=float,
+            default=0.0,
+            help="weight for predictive loss for unmasked frames",
+        )
+        parser.add_argument(
+            "--loss_weights",
+            type=float,
+            default=0.0,
+            help="weights for additional loss terms (not first one)",
+        )
+
+        for class_choices in cls.class_choices_list:
+            # Append --<name> and --<name>_conf.
+            # e.g. --encoder and --encoder_conf
+            class_choices.add_arguments(group)
+
+    @classmethod
+    def build_collate_fn(
+            cls, args: argparse.Namespace, train: bool
+    ) -> Callable[
+        [Collection[Tuple[str, Dict[str, np.ndarray]]]],
+        Tuple[List[str], Dict[str, torch.Tensor]],
+    ]:
+        assert check_argument_types()
+        return CommonCollateFn(clipping=True)
+
+    @classmethod
+    def build_preprocess_fn(
+            cls, args: argparse.Namespace, train: bool
+    ) -> Optional[Callable[[str, Dict[str, np.array]], Dict[str, np.ndarray]]]:
+        assert check_argument_types()
+        if args.use_preprocessor:
+            retval = CommonPreprocessor(
+                train=train,
+                bpemodel=args.bpemodel,
+                non_linguistic_symbols=args.non_linguistic_symbols,
+                text_cleaner=args.cleaner,
+                g2p_type=args.g2p,
+                # NOTE(kamo): Check attribute existence for backward compatibility
+                rir_scp=args.rir_scp if hasattr(args, "rir_scp") else None,
+                rir_apply_prob=args.rir_apply_prob
+                if hasattr(args, "rir_apply_prob")
+                else 1.0,
+                noise_scp=args.noise_scp if hasattr(args, "noise_scp") else None,
+                noise_apply_prob=args.noise_apply_prob
+                if hasattr(args, "noise_apply_prob")
+                else 1.0,
+                noise_db_range=args.noise_db_range
+                if hasattr(args, "noise_db_range")
+                else "13_15",
+                speech_volume_normalize=args.speech_volume_normalize
+                if hasattr(args, "rir_scp")
+                else None,
+            )
+        else:
+            retval = None
+        assert check_return_type(retval)
+        return retval
+
+    @classmethod
+    def required_data_names(
+            cls, train: bool = True, inference: bool = False
+    ) -> Tuple[str, ...]:
+        # for pre-training
+        retval = ("speech",)
+        return retval
+
+    @classmethod
+    def optional_data_names(
+            cls, train: bool = True, inference: bool = False
+    ) -> Tuple[str, ...]:
+        retval = ()
+        assert check_return_type(retval)
+        return retval
+
+    @classmethod
+    def build_model(cls, args: argparse.Namespace):
+        assert check_argument_types()
+
+        # 1. frontend
+        if args.input_size is None:
+            # Extract features in the model
+            frontend_class = frontend_choices.get_class(args.frontend)
+            frontend = frontend_class(**args.frontend_conf)
+            input_size = frontend.output_size()
+        else:
+            # Give features from data-loader
+            args.frontend = None
+            args.frontend_conf = {}
+            frontend = None
+            input_size = args.input_size
+
+        # 2. Data augmentation for spectrogram
+        if args.specaug is not None:
+            specaug_class = specaug_choices.get_class(args.specaug)
+            specaug = specaug_class(**args.specaug_conf)
+        else:
+            specaug = None
 
-class Text2Punc:
+        # 3. Normalization layer
+        if args.normalize is not None:
+            normalize_class = normalize_choices.get_class(args.normalize)
+            normalize = normalize_class(**args.normalize_conf)
+        else:
+            normalize = None
 
-    def __init__(
-        self,
-        train_config: Optional[str],
-        model_file: Optional[str],
-        device: str = "cpu",
-        dtype: str = "float32",
-    ):
-        #  Build Model
-        model, train_args = PunctuationTask.build_model_from_file(train_config, model_file, device)
-        self.device = device
-        # Wrape model to make model.nll() data-parallel
-        self.wrapped_model = ForwardAdaptor(model, "inference")
-        self.wrapped_model.to(dtype=getattr(torch, dtype)).to(device=device).eval()
-        # logging.info(f"Model:\n{model}")
-        self.punc_list = train_args.punc_list
-        self.period = 0
-        for i in range(len(self.punc_list)):
-            if self.punc_list[i] == ",":
-                self.punc_list[i] = "，"
-            elif self.punc_list[i] == "?":
-                self.punc_list[i] = "？"
-            elif self.punc_list[i] == "。":
-                self.period = i
-        self.preprocessor = CodeMixTokenizerCommonPreprocessor(
-            train=False,
-            token_type=train_args.token_type,
-            token_list=train_args.token_list,
-            bpemodel=train_args.bpemodel,
-            text_cleaner=train_args.cleaner,
-            g2p_type=train_args.g2p,
-            text_name="text",
-            non_linguistic_symbols=train_args.non_linguistic_symbols,
-        )
-        
-
-    @torch.no_grad()
-    def __call__(self, text: Union[list, str], cache: list, split_size=20):
-        if cache is not None and len(cache) > 0:
-            precache = "".join(cache)
+        # 4. Pre-encoder input block
+        # NOTE(kan-bayashi): Use getattr to keep the compatibility
+        if getattr(args, "preencoder", None) is not None:
+            preencoder_class = preencoder_choices.get_class(args.preencoder)
+            preencoder = preencoder_class(**args.preencoder_conf)
+            input_size = preencoder.output_size()
         else:
-            precache = ""
-            cache = []
-        data = {"text": precache + " " + text}
-        result = self.preprocessor(data=data, uid="12938712838719")
-        split_text = self.preprocessor.pop_split_text_data(result)
-        mini_sentences = split_to_mini_sentence(split_text, split_size)
-        mini_sentences_id = split_to_mini_sentence(data["text"], split_size)
-        assert len(mini_sentences) == len(mini_sentences_id)
-        cache_sent = []
-        cache_sent_id = torch.from_numpy(np.array([], dtype='int32'))
-        sentence_punc_list = []
-        sentence_words_list= []
-        cache_pop_trigger_limit = 200
-        skip_num = 0
-        for mini_sentence_i in range(len(mini_sentences)):
-            mini_sentence = mini_sentences[mini_sentence_i]
-            mini_sentence_id = mini_sentences_id[mini_sentence_i]
-            mini_sentence = cache_sent + mini_sentence
-            mini_sentence_id = np.concatenate((cache_sent_id, mini_sentence_id), axis=0)
-            data = {
-                "text": torch.unsqueeze(torch.from_numpy(mini_sentence_id), 0),
-                "text_lengths": torch.from_numpy(np.array([len(mini_sentence_id)], dtype='int32')),
-                "vad_indexes": torch.from_numpy(np.array([len(cache)], dtype='int32')),
-            }
-            data = to_device(data, self.device)
-            y, _ = self.wrapped_model(**data)
-            _, indices = y.view(-1, y.shape[-1]).topk(1, dim=1)
-            punctuations = indices
-            if indices.size()[0] != 1:
-                punctuations = torch.squeeze(indices)
-            assert punctuations.size()[0] == len(mini_sentence)
-
-            # Search for the last Period/QuestionMark as cache
-            if mini_sentence_i < len(mini_sentences) - 1:
-                sentenceEnd = -1
-                last_comma_index = -1
-                for i in range(len(punctuations) - 2, 1, -1):
-                    if self.punc_list[punctuations[i]] == "。" or self.punc_list[punctuations[i]] == "？":
-                        sentenceEnd = i
-                        break
-                    if last_comma_index < 0 and self.punc_list[punctuations[i]] == "，":
-                        last_comma_index = i
-    
-                if sentenceEnd < 0 and len(mini_sentence) > cache_pop_trigger_limit and last_comma_index >= 0:
-                    # The sentence it too long, cut off at a comma.
-                    sentenceEnd = last_comma_index
-                    punctuations[sentenceEnd] = self.period
-                cache_sent = mini_sentence[sentenceEnd + 1:]
-                cache_sent_id = mini_sentence_id[sentenceEnd + 1:]
-                mini_sentence = mini_sentence[0:sentenceEnd + 1]
-                punctuations = punctuations[0:sentenceEnd + 1]
-
-            punctuations_np = punctuations.cpu().numpy()
-            sentence_punc_list += [self.punc_list[int(x)] for x in punctuations_np]
-            sentence_words_list += mini_sentence
-
-        assert len(sentence_punc_list) == len(sentence_words_list)
-        words_with_punc = []
-        sentence_punc_list_out = []
-        for i in range(0, len(sentence_words_list)):
-            if i > 0:
-                if len(sentence_words_list[i][0].encode()) == 1 and len(sentence_words_list[i - 1][-1].encode()) == 1:
-                    sentence_words_list[i] = " " + sentence_words_list[i]
-            if skip_num < len(cache):
-                skip_num += 1
-            else:
-                words_with_punc.append(sentence_words_list[i])
-            if skip_num >= len(cache):
-                sentence_punc_list_out.append(sentence_punc_list[i])
-                if sentence_punc_list[i] != "_":
-                    words_with_punc.append(sentence_punc_list[i])
-        sentence_out = "".join(words_with_punc)
-
-        sentenceEnd = -1
-        for i in range(len(sentence_punc_list) - 2, 1, -1):
-            if sentence_punc_list[i] == "。" or sentence_punc_list[i] == "？":
-               sentenceEnd = i
-               break
-        cache_out = sentence_words_list[sentenceEnd + 1 :]
-        if sentence_out[-1] in self.punc_list:
-            sentence_out = sentence_out[:-1]
-            sentence_punc_list_out[-1] = "_"
-        return sentence_out, sentence_punc_list_out, cache_out
-
-
-def inference(
-    batch_size: int,
-    dtype: str,
-    ngpu: int,
-    seed: int,
-    num_workers: int,
-    output_dir: str,
-    log_level: Union[int, str],
-    train_config: Optional[str],
-    model_file: Optional[str],
-    key_file: Optional[str] = None,
-    data_path_and_name_and_type: Sequence[Tuple[str, str, str]] = None,
-    raw_inputs: Union[List[Any], bytes, str] = None,
-    cache: List[Any] = None,
-    param_dict: dict = None,
-    **kwargs,
-):
-    inference_pipeline = inference_modelscope(
-        output_dir=output_dir,
-        batch_size=batch_size,
-        dtype=dtype,
-        ngpu=ngpu,
-        seed=seed,
-        num_workers=num_workers,
-        log_level=log_level,
-        key_file=key_file,
-        train_config=train_config,
-        model_file=model_file,
-        param_dict=param_dict,
-        **kwargs,
-    )
-    return inference_pipeline(data_path_and_name_and_type, raw_inputs, cache)
-
-
-def inference_modelscope(
-    batch_size: int,
-    dtype: str,
-    ngpu: int,
-    seed: int,
-    num_workers: int,
-    log_level: Union[int, str],
-    #cache: list,
-    key_file: Optional[str],
-    train_config: Optional[str],
-    model_file: Optional[str],
-    output_dir: Optional[str] = None,
-    param_dict: dict = None,
-    **kwargs,
-):
-    assert check_argument_types()
-    ncpu = kwargs.get("ncpu", 1)
-    torch.set_num_threads(ncpu)
-
-    if ngpu >= 1 and torch.cuda.is_available():
-        device = "cuda"
-    else:
-        device = "cpu"
-
-    # 1. Set random-seed
-    set_all_random_seed(seed)
-    text2punc = Text2Punc(train_config, model_file, device)
-
-    def _forward(
-        data_path_and_name_and_type,
-        raw_inputs: Union[List[Any], bytes, str] = None,
-        output_dir_v2: Optional[str] = None,
-        cache: List[Any] = None,
-        param_dict: dict = None,
-    ):
-        results = []
-        split_size = 10
-        cache_in = param_dict["cache"]
-        if raw_inputs != None:
-            line = raw_inputs.strip()
-            key = "demo"
-            if line == "":
-                item = {'key': key, 'value': ""}
-                results.append(item)
-                return results
-            result, _, cache = text2punc(line, cache_in)
-            param_dict["cache"] = cache
-            item = {'key': key, 'value': result}
-            results.append(item)
-            return results
-
-        return results
-
-    return _forward
-
-
-def get_parser():
-    parser = config_argparse.ArgumentParser(
-        description="Punctuation inference",
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-    )
-
-    parser.add_argument(
-        "--log_level",
-        type=lambda x: x.upper(),
-        default="INFO",
-        choices=("CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET"),
-        help="The verbose level of logging",
-    )
-
-    parser.add_argument("--output_dir", type=str, required=False)
-    parser.add_argument(
-        "--ngpu",
-        type=int,
-        default=0,
-        help="The number of gpus. 0 indicates CPU mode",
-    )
-    parser.add_argument("--seed", type=int, default=0, help="Random seed")
-    parser.add_argument(
-        "--dtype",
-        default="float32",
-        choices=["float16", "float32", "float64"],
-        help="Data type",
-    )
-    parser.add_argument(
-        "--num_workers",
-        type=int,
-        default=1,
-        help="The number of workers used for DataLoader",
-    )
-    parser.add_argument(
-        "--batch_size",
-        type=int,
-        default=1,
-        help="The batch size for inference",
-    )
-
-    group = parser.add_argument_group("Input data related")
-    group.add_argument("--data_path_and_name_and_type", type=str2triple_str, action="append", required=False)
-    group.add_argument("--raw_inputs", type=str, required=False)
-    group.add_argument("--cache", type=list, required=False)
-    group.add_argument("--param_dict", type=dict, required=False)
-    group.add_argument("--key_file", type=str_or_none)
-
-    group = parser.add_argument_group("The model configuration related")
-    group.add_argument("--train_config", type=str)
-    group.add_argument("--model_file", type=str)
-
-    return parser
-
-
-def main(cmd=None):
-    print(get_commandline_args(), file=sys.stderr)
-    parser = get_parser()
-    args = parser.parse_args(cmd)
-    kwargs = vars(args)
-    # kwargs.pop("config", None)
-    inference(**kwargs)
+            preencoder = None
+
+        # 5. Encoder
+        encoder_class = encoder_choices.get_class(args.encoder)
+        encoder = encoder_class(
+            input_size=input_size,
+            **args.encoder_conf,
+        )
+
+        # 6. Build model
+        try:
+            model_class = model_choices.get_class(args.model)
+        except AttributeError:
+            model_class = model_choices.get_class("data2vec")
+        model = model_class(
+            frontend=frontend,
+            specaug=specaug,
+            normalize=normalize,
+            preencoder=preencoder,
+            encoder=encoder,
+        )
 
+        # 7. Initialize
+        if args.init is not None:
+            initialize(model, args.init)
 
-if __name__ == "__main__":
-    main()
+        assert check_return_type(model)
+        return model
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `funasr-0.5.3/funasr/bin/sa_asr_inference.py` & `funasr-0.5.4/funasr/bin/diar_inference_launch.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,547 +1,425 @@
+# -*- encoding: utf-8 -*-
+#!/usr/bin/env python3
+# Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
+#  MIT License  (https://opensource.org/licenses/MIT)
+
+
 import argparse
 import logging
+import os
+import sys
+from typing import Union, Dict, Any
+
+from funasr.utils import config_argparse
+from funasr.utils.cli_utils import get_commandline_args
+from funasr.utils.types import str2bool
+from funasr.utils.types import str2triple_str
+from funasr.utils.types import str_or_none
+
+import argparse
+import logging
+import os
 import sys
 from pathlib import Path
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Union
-from typing import Dict
 
+from collections import OrderedDict
 import numpy as np
+import soundfile
 import torch
+from torch.nn import functional as F
 from typeguard import check_argument_types
 from typeguard import check_return_type
-
-from funasr.fileio.datadir_writer import DatadirWriter
-from funasr.modules.beam_search.batch_beam_search_online_sim import BatchBeamSearchOnlineSim
-from funasr.modules.beam_search.beam_search_sa_asr import BeamSearch
-from funasr.modules.beam_search.beam_search_sa_asr import Hypothesis
-from funasr.modules.scorers.ctc import CTCPrefixScorer
-from funasr.modules.scorers.length_bonus import LengthBonus
-from funasr.modules.scorers.scorer_interface import BatchScorerInterface
-from funasr.modules.subsampling import TooShortUttError
-from funasr.tasks.sa_asr import ASRTask
-from funasr.tasks.lm import LMTask
-from funasr.text.build_tokenizer import build_tokenizer
-from funasr.text.token_id_converter import TokenIDConverter
+from scipy.signal import medfilt
+from funasr.utils.cli_utils import get_commandline_args
+from funasr.tasks.diar import DiarTask
+from funasr.tasks.diar import EENDOLADiarTask
 from funasr.torch_utils.device_funcs import to_device
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.utils import config_argparse
-from funasr.utils.cli_utils import get_commandline_args
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
-from funasr.utils import asr_utils, wav_utils, postprocess_utils
-from funasr.models.frontend.wav_frontend import WavFrontend
-from funasr.tasks.asr import frontend_choices
-
-
-header_colors = '\033[95m'
-end_colors = '\033[0m'
-
-
-class Speech2Text:
-    """Speech2Text class
-
-    Examples:
-        >>> import soundfile
-        >>> speech2text = Speech2Text("asr_config.yml", "asr.pb")
-        >>> audio, rate = soundfile.read("speech.wav")
-        >>> speech2text(audio)
-        [(text, token, token_int, hypothesis object), ...]
-
-    """
-
-    def __init__(
-            self,
-            asr_train_config: Union[Path, str] = None,
-            asr_model_file: Union[Path, str] = None,
-            cmvn_file: Union[Path, str] = None,
-            lm_train_config: Union[Path, str] = None,
-            lm_file: Union[Path, str] = None,
-            token_type: str = None,
-            bpemodel: str = None,
-            device: str = "cpu",
-            maxlenratio: float = 0.0,
-            minlenratio: float = 0.0,
-            batch_size: int = 1,
-            dtype: str = "float32",
-            beam_size: int = 20,
-            ctc_weight: float = 0.5,
-            lm_weight: float = 1.0,
-            ngram_weight: float = 0.9,
-            penalty: float = 0.0,
-            nbest: int = 1,
-            streaming: bool = False,
-            frontend_conf: dict = None,
-            **kwargs,
-    ):
-        assert check_argument_types()
+from scipy.ndimage import median_filter
+from funasr.utils.misc import statistic_model_parameters
+from funasr.datasets.iterable_dataset import load_bytes
+from funasr.bin.diar_infer import Speech2DiarizationSOND, Speech2DiarizationEEND
+
+def inference_sond(
+        diar_train_config: str,
+        diar_model_file: str,
+        output_dir: Optional[str] = None,
+        batch_size: int = 1,
+        dtype: str = "float32",
+        ngpu: int = 0,
+        seed: int = 0,
+        num_workers: int = 0,
+        log_level: Union[int, str] = "INFO",
+        key_file: Optional[str] = None,
+        model_tag: Optional[str] = None,
+        allow_variable_data_keys: bool = True,
+        streaming: bool = False,
+        smooth_size: int = 83,
+        dur_threshold: int = 10,
+        out_format: str = "vad",
+        param_dict: Optional[dict] = None,
+        mode: str = "sond",
+        **kwargs,
+):
+    assert check_argument_types()
+    ncpu = kwargs.get("ncpu", 1)
+    torch.set_num_threads(ncpu)
+    if batch_size > 1:
+        raise NotImplementedError("batch decoding is not implemented")
+    if ngpu > 1:
+        raise NotImplementedError("only single GPU decoding is supported")
 
-        # 1. Build ASR model
-        scorers = {}
-        asr_model, asr_train_args = ASRTask.build_model_from_file(
-            asr_train_config, asr_model_file, cmvn_file, device
-        )
-        frontend = None
-        if asr_train_args.frontend is not None and asr_train_args.frontend_conf is not None:
-            if asr_train_args.frontend=='wav_frontend':
-                frontend = WavFrontend(cmvn_file=cmvn_file, **asr_train_args.frontend_conf)
-            else:
-                frontend_class=frontend_choices.get_class(asr_train_args.frontend)
-                frontend = frontend_class(**asr_train_args.frontend_conf).eval()
+    logging.basicConfig(
+        level=log_level,
+        format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
+    )
+    logging.info("param_dict: {}".format(param_dict))
 
-        logging.info("asr_model: {}".format(asr_model))
-        logging.info("asr_train_args: {}".format(asr_train_args))
-        asr_model.to(dtype=getattr(torch, dtype)).eval()
-
-        decoder = asr_model.decoder
-
-        ctc = CTCPrefixScorer(ctc=asr_model.ctc, eos=asr_model.eos)
-        token_list = asr_model.token_list
-        scorers.update(
-            decoder=decoder,
-            ctc=ctc,
-            length_bonus=LengthBonus(len(token_list)),
-        )
+    if ngpu >= 1 and torch.cuda.is_available():
+        device = "cuda"
+    else:
+        device = "cpu"
 
-        # 2. Build Language model
-        if lm_train_config is not None:
-            lm, lm_train_args = LMTask.build_model_from_file(
-                lm_train_config, lm_file, None, device
-            )
-            scorers["lm"] = lm.lm
+    # 1. Set random-seed
+    set_all_random_seed(seed)
 
-        # 3. Build ngram model
-        # ngram is not supported now
-        ngram = None
-        scorers["ngram"] = ngram
-
-        # 4. Build BeamSearch object
-        # transducer is not supported now
-        beam_search_transducer = None
-
-        weights = dict(
-            decoder=1.0 - ctc_weight,
-            ctc=ctc_weight,
-            lm=lm_weight,
-            ngram=ngram_weight,
-            length_bonus=penalty,
+    # 2a. Build speech2xvec [Optional]
+    if mode == "sond_demo" and param_dict is not None and "extract_profile" in param_dict and param_dict["extract_profile"]:
+        assert "sv_train_config" in param_dict, "sv_train_config must be provided param_dict."
+        assert "sv_model_file" in param_dict, "sv_model_file must be provided in param_dict."
+        sv_train_config = param_dict["sv_train_config"]
+        sv_model_file = param_dict["sv_model_file"]
+        if "model_dir" in param_dict:
+            sv_train_config = os.path.join(param_dict["model_dir"], sv_train_config)
+            sv_model_file = os.path.join(param_dict["model_dir"], sv_model_file)
+        from funasr.bin.sv_infer import Speech2Xvector
+        speech2xvector_kwargs = dict(
+            sv_train_config=sv_train_config,
+            sv_model_file=sv_model_file,
+            device=device,
+            dtype=dtype,
+            streaming=streaming,
+            embedding_node="resnet1_dense"
         )
-        beam_search = BeamSearch(
-            beam_size=beam_size,
-            weights=weights,
-            scorers=scorers,
-            sos=asr_model.sos,
-            eos=asr_model.eos,
-            vocab_size=len(token_list),
-            token_list=token_list,
-            pre_beam_score_key=None if ctc_weight == 1.0 else "full",
+        logging.info("speech2xvector_kwargs: {}".format(speech2xvector_kwargs))
+        speech2xvector = Speech2Xvector.from_pretrained(
+            model_tag=model_tag,
+            **speech2xvector_kwargs,
         )
+        speech2xvector.sv_model.eval()
 
-        # 5. [Optional] Build Text converter: e.g. bpe-sym -> Text
-        if token_type is None:
-            token_type = asr_train_args.token_type
-        if bpemodel is None:
-            bpemodel = asr_train_args.bpemodel
-
-        if token_type is None:
-            tokenizer = None
-        elif token_type == "bpe":
-            if bpemodel is not None:
-                tokenizer = build_tokenizer(token_type=token_type, bpemodel=bpemodel)
-            else:
-                tokenizer = None
-        else:
-            tokenizer = build_tokenizer(token_type=token_type)
-        converter = TokenIDConverter(token_list=token_list)
-        logging.info(f"Text tokenizer: {tokenizer}")
-
-        self.asr_model = asr_model
-        self.asr_train_args = asr_train_args
-        self.converter = converter
-        self.tokenizer = tokenizer
-        self.beam_search = beam_search
-        self.beam_search_transducer = beam_search_transducer
-        self.maxlenratio = maxlenratio
-        self.minlenratio = minlenratio
-        self.device = device
-        self.dtype = dtype
-        self.nbest = nbest
-        self.frontend = frontend
-
-    @torch.no_grad()
-    def __call__(
-            self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray], profile: Union[torch.Tensor, np.ndarray], profile_lengths: Union[torch.Tensor, np.ndarray]
-    ) -> List[
-        Tuple[
-            Optional[str],
-            Optional[str],
-            List[str],
-            List[int],
-            Union[Hypothesis],
-        ]
-    ]:
-        """Inference
-
-        Args:
-            speech: Input speech data
-        Returns:
-            text, text_id, token, token_int, hyp
-
-        """
-        assert check_argument_types()
-
-        # Input as audio signal
-        if isinstance(speech, np.ndarray):
-            speech = torch.tensor(speech)
-
-        if isinstance(profile, np.ndarray):
-            profile = torch.tensor(profile)
-
-        if self.frontend is not None:
-            feats, feats_len = self.frontend.forward(speech, speech_lengths)
-            feats = to_device(feats, device=self.device)
-            feats_len = feats_len.int()
-            self.asr_model.frontend = None
+    # 2b. Build speech2diar
+    speech2diar_kwargs = dict(
+        diar_train_config=diar_train_config,
+        diar_model_file=diar_model_file,
+        device=device,
+        dtype=dtype,
+        streaming=streaming,
+        smooth_size=smooth_size,
+        dur_threshold=dur_threshold,
+    )
+    logging.info("speech2diarization_kwargs: {}".format(speech2diar_kwargs))
+    speech2diar = Speech2DiarizationSOND.from_pretrained(
+        model_tag=model_tag,
+        **speech2diar_kwargs,
+    )
+    speech2diar.diar_model.eval()
+
+    def output_results_str(results: dict, uttid: str):
+        rst = []
+        mid = uttid.rsplit("-", 1)[0]
+        for key in results:
+            results[key] = [(x[0]/100, x[1]/100) for x in results[key]]
+        if out_format == "vad":
+            for spk, segs in results.items():
+                rst.append("{} {}".format(spk, segs))
         else:
-            feats = speech
-            feats_len = speech_lengths
-        lfr_factor = max(1, (feats.size()[-1] // 80) - 1)
-        batch = {"speech": feats, "speech_lengths": feats_len}
-
-        # a. To device
-        batch = to_device(batch, device=self.device)
-
-        # b. Forward Encoder
-        asr_enc, _, spk_enc = self.asr_model.encode(**batch)
-        if isinstance(asr_enc, tuple):
-            asr_enc = asr_enc[0]
-        if isinstance(spk_enc, tuple):
-            spk_enc = spk_enc[0]
-        assert len(asr_enc) == 1, len(asr_enc)
-        assert len(spk_enc) == 1, len(spk_enc)
-
-        # c. Passed the encoder result and the beam search
-        nbest_hyps = self.beam_search(
-            asr_enc[0], spk_enc[0], profile[0], maxlenratio=self.maxlenratio, minlenratio=self.minlenratio
-        )
-
-        nbest_hyps = nbest_hyps[: self.nbest]
+            template = "SPEAKER {} 0 {:.2f} {:.2f} <NA> <NA> {} <NA> <NA>"
+            for spk, segs in results.items():
+                rst.extend([template.format(mid, st, ed, spk) for st, ed in segs])
+
+        return "\n".join(rst)
+
+    def _forward(
+            data_path_and_name_and_type: Sequence[Tuple[str, str, str]] = None,
+            raw_inputs: List[List[Union[np.ndarray, torch.Tensor, str, bytes]]] = None,
+            output_dir_v2: Optional[str] = None,
+            param_dict: Optional[dict] = None,
+    ):
+        logging.info("param_dict: {}".format(param_dict))
+        if data_path_and_name_and_type is None and raw_inputs is not None:
+            if isinstance(raw_inputs, (list, tuple)):
+                if not isinstance(raw_inputs[0], List):
+                    raw_inputs = [raw_inputs]
+
+                assert all([len(example) >= 2 for example in raw_inputs]), \
+                    "The length of test case in raw_inputs must larger than 1 (>=2)."
+
+                def prepare_dataset():
+                    for idx, example in enumerate(raw_inputs):
+                        # read waveform file
+                        example = [load_bytes(x) if isinstance(x, bytes) else x
+                                   for x in example]
+                        example = [soundfile.read(x)[0] if isinstance(x, str) else x
+                                   for x in example]
+                        # convert torch tensor to numpy array
+                        example = [x.numpy() if isinstance(example[0], torch.Tensor) else x
+                                   for x in example]
+                        speech = example[0]
+                        logging.info("Extracting profiles for {} waveforms".format(len(example)-1))
+                        profile = [speech2xvector.calculate_embedding(x) for x in example[1:]]
+                        profile = torch.cat(profile, dim=0)
+                        yield ["test{}".format(idx)], {"speech": [speech], "profile": [profile]}
 
-        results = []
-        for hyp in nbest_hyps:
-            assert isinstance(hyp, (Hypothesis)), type(hyp)
-
-            # remove sos/eos and get results
-            last_pos = -1
-            if isinstance(hyp.yseq, list):
-                token_int = hyp.yseq[1: last_pos]
+                loader = prepare_dataset()
             else:
-                token_int = hyp.yseq[1: last_pos].tolist()
-
-            spk_weigths=torch.stack(hyp.spk_weigths, dim=0)
+                raise TypeError("raw_inputs must be a list or tuple in [speech, profile1, profile2, ...] ")
+        else:
+            # 3. Build data-iterator
+            loader = DiarTask.build_streaming_iterator(
+                data_path_and_name_and_type,
+                dtype=dtype,
+                batch_size=batch_size,
+                key_file=key_file,
+                num_workers=num_workers,
+                preprocess_fn=None,
+                collate_fn=None,
+                allow_variable_data_keys=allow_variable_data_keys,
+                inference=True,
+            )
 
-            token_ori = self.converter.ids2tokens(token_int)
-            text_ori = self.tokenizer.tokens2text(token_ori)
+        # 7. Start for-loop
+        output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
+        if output_path is not None:
+            os.makedirs(output_path, exist_ok=True)
+            output_writer = open("{}/result.txt".format(output_path), "w")
+            pse_label_writer = open("{}/labels.txt".format(output_path), "w")
+        logging.info("Start to diarize...")
+        result_list = []
+        for idx, (keys, batch) in enumerate(loader):
+            assert isinstance(batch, dict), type(batch)
+            assert all(isinstance(s, str) for s in keys), keys
+            _bs = len(next(iter(batch.values())))
+            assert len(keys) == _bs, f"{len(keys)} != {_bs}"
+            batch = {k: v[0] for k, v in batch.items() if not k.endswith("_lengths")}
 
-            text_ori_spklist = text_ori.split('$')
-            cur_index = 0
-            spk_choose = []
-            for i in range(len(text_ori_spklist)):
-                text_ori_split = text_ori_spklist[i]
-                n = len(text_ori_split)
-                spk_weights_local = spk_weigths[cur_index: cur_index + n]
-                cur_index = cur_index + n + 1
-                spk_weights_local = spk_weights_local.mean(dim=0)
-                spk_choose_local = spk_weights_local.argmax(-1)
-                spk_choose.append(spk_choose_local.item() + 1)
+            results, pse_labels = speech2diar(**batch)
+            # Only supporting batch_size==1
+            key, value = keys[0], output_results_str(results, keys[0])
+            item = {"key": key, "value": value}
+            result_list.append(item)
+            if output_path is not None:
+                output_writer.write(value)
+                output_writer.flush()
+                pse_label_writer.write("{} {}\n".format(key, " ".join(pse_labels)))
+                pse_label_writer.flush()
 
-            # remove blank symbol id, which is assumed to be 0
-            token_int = list(filter(lambda x: x != 0, token_int))
+            if idx % 100 == 0:
+                logging.info("Processing {:5d}: {}".format(idx, key))
 
-            # Change integer-ids to tokens
-            token = self.converter.ids2tokens(token_int)
+        if output_path is not None:
+            output_writer.close()
+            pse_label_writer.close()
 
-            if self.tokenizer is not None:
-                text = self.tokenizer.tokens2text(token)
-            else:
-                text = None
+        return result_list
 
-            text_spklist = text.split('$')
-            assert len(spk_choose) == len(text_spklist)
+    return _forward
 
-            spk_list=[]
-            for i in range(len(text_spklist)):
-                text_split = text_spklist[i]
-                n = len(text_split)
-                spk_list.append(str(spk_choose[i]) * n)
-            
-            text_id = '$'.join(spk_list)
-            
-            assert len(text) == len(text_id)
-
-            results.append((text, text_id, token, token_int, hyp))
-
-        assert check_return_type(results)
-        return results
-
-def inference(
-        maxlenratio: float,
-        minlenratio: float,
-        batch_size: int,
-        beam_size: int,
-        ngpu: int,
-        ctc_weight: float,
-        lm_weight: float,
-        penalty: float,
-        log_level: Union[int, str],
-        data_path_and_name_and_type,
-        asr_train_config: Optional[str],
-        asr_model_file: Optional[str],
-        cmvn_file: Optional[str] = None,
-        raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-        lm_train_config: Optional[str] = None,
-        lm_file: Optional[str] = None,
-        token_type: Optional[str] = None,
-        key_file: Optional[str] = None,
-        word_lm_train_config: Optional[str] = None,
-        bpemodel: Optional[str] = None,
-        allow_variable_data_keys: bool = False,
-        streaming: bool = False,
+def inference_eend(
+        diar_train_config: str,
+        diar_model_file: str,
         output_dir: Optional[str] = None,
+        batch_size: int = 1,
         dtype: str = "float32",
-        seed: int = 0,
-        ngram_weight: float = 0.9,
-        nbest: int = 1,
-        num_workers: int = 1,
-        mc: bool = False,
-        **kwargs,
-):
-    inference_pipeline = inference_modelscope(
-        maxlenratio=maxlenratio,
-        minlenratio=minlenratio,
-        batch_size=batch_size,
-        beam_size=beam_size,
-        ngpu=ngpu,
-        ctc_weight=ctc_weight,
-        lm_weight=lm_weight,
-        penalty=penalty,
-        log_level=log_level,
-        asr_train_config=asr_train_config,
-        asr_model_file=asr_model_file,
-        cmvn_file=cmvn_file,
-        raw_inputs=raw_inputs,
-        lm_train_config=lm_train_config,
-        lm_file=lm_file,
-        token_type=token_type,
-        key_file=key_file,
-        word_lm_train_config=word_lm_train_config,
-        bpemodel=bpemodel,
-        allow_variable_data_keys=allow_variable_data_keys,
-        streaming=streaming,
-        output_dir=output_dir,
-        dtype=dtype,
-        seed=seed,
-        ngram_weight=ngram_weight,
-        nbest=nbest,
-        num_workers=num_workers,
-        mc=mc,
+        ngpu: int = 1,
+        num_workers: int = 0,
+        log_level: Union[int, str] = "INFO",
+        key_file: Optional[str] = None,
+        model_tag: Optional[str] = None,
+        allow_variable_data_keys: bool = True,
+        streaming: bool = False,
+        param_dict: Optional[dict] = None,
         **kwargs,
-    )
-    return inference_pipeline(data_path_and_name_and_type, raw_inputs)
-
-def inference_modelscope(
-    maxlenratio: float,
-    minlenratio: float,
-    batch_size: int,
-    beam_size: int,
-    ngpu: int,
-    ctc_weight: float,
-    lm_weight: float,
-    penalty: float,
-    log_level: Union[int, str],
-    # data_path_and_name_and_type,
-    asr_train_config: Optional[str],
-    asr_model_file: Optional[str],
-    cmvn_file: Optional[str] = None,
-    lm_train_config: Optional[str] = None,
-    lm_file: Optional[str] = None,
-    token_type: Optional[str] = None,
-    key_file: Optional[str] = None,
-    word_lm_train_config: Optional[str] = None,
-    bpemodel: Optional[str] = None,
-    allow_variable_data_keys: bool = False,
-    streaming: bool = False,
-    output_dir: Optional[str] = None,
-    dtype: str = "float32",
-    seed: int = 0,
-    ngram_weight: float = 0.9,
-    nbest: int = 1,
-    num_workers: int = 1,
-    mc: bool = False,
-    param_dict: dict = None,
-    **kwargs,
 ):
     assert check_argument_types()
+    ncpu = kwargs.get("ncpu", 1)
+    torch.set_num_threads(ncpu)
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
-    if word_lm_train_config is not None:
-        raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
 
-    for handler in logging.root.handlers[:]:
-        logging.root.removeHandler(handler)
-    
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
-    
+    logging.info("param_dict: {}".format(param_dict))
+
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
-    
-    # 1. Set random-seed
-    set_all_random_seed(seed)
-    
-    # 2. Build speech2text
-    speech2text_kwargs = dict(
-        asr_train_config=asr_train_config,
-        asr_model_file=asr_model_file,
-        cmvn_file=cmvn_file,
-        lm_train_config=lm_train_config,
-        lm_file=lm_file,
-        token_type=token_type,
-        bpemodel=bpemodel,
+
+    # 1. Build speech2diar
+    speech2diar_kwargs = dict(
+        diar_train_config=diar_train_config,
+        diar_model_file=diar_model_file,
         device=device,
-        maxlenratio=maxlenratio,
-        minlenratio=minlenratio,
         dtype=dtype,
-        beam_size=beam_size,
-        ctc_weight=ctc_weight,
-        lm_weight=lm_weight,
-        ngram_weight=ngram_weight,
-        penalty=penalty,
-        nbest=nbest,
-        streaming=streaming,
     )
-    logging.info("speech2text_kwargs: {}".format(speech2text_kwargs))
-    speech2text = Speech2Text(**speech2text_kwargs)
-    
-    def _forward(data_path_and_name_and_type,
-                 raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-                 output_dir_v2: Optional[str] = None,
-                 fs: dict = None,
-                 param_dict: dict = None,
-                 **kwargs,
-                 ):
-        # 3. Build data-iterator
+    logging.info("speech2diarization_kwargs: {}".format(speech2diar_kwargs))
+    speech2diar = Speech2DiarizationEEND.from_pretrained(
+        model_tag=model_tag,
+        **speech2diar_kwargs,
+    )
+    speech2diar.diar_model.eval()
+
+    def output_results_str(results: dict, uttid: str):
+        rst = []
+        mid = uttid.rsplit("-", 1)[0]
+        for key in results:
+            results[key] = [(x[0] / 100, x[1] / 100) for x in results[key]]
+        template = "SPEAKER {} 0 {:.2f} {:.2f} <NA> <NA> {} <NA> <NA>"
+        for spk, segs in results.items():
+            rst.extend([template.format(mid, st, ed, spk) for st, ed in segs])
+
+        return "\n".join(rst)
+
+    def _forward(
+            data_path_and_name_and_type: Sequence[Tuple[str, str, str]] = None,
+            raw_inputs: List[List[Union[np.ndarray, torch.Tensor, str, bytes]]] = None,
+            output_dir_v2: Optional[str] = None,
+            param_dict: Optional[dict] = None,
+    ):
+        # 2. Build data-iterator
         if data_path_and_name_and_type is None and raw_inputs is not None:
             if isinstance(raw_inputs, torch.Tensor):
                 raw_inputs = raw_inputs.numpy()
-            data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
-        loader = ASRTask.build_streaming_iterator(
+            data_path_and_name_and_type = [raw_inputs[0], "speech", "sound"]
+        loader = EENDOLADiarTask.build_streaming_iterator(
             data_path_and_name_and_type,
             dtype=dtype,
-            fs=fs,
-            mc=mc,
             batch_size=batch_size,
             key_file=key_file,
             num_workers=num_workers,
-            preprocess_fn=ASRTask.build_preprocess_fn(speech2text.asr_train_args, False),
-            collate_fn=ASRTask.build_collate_fn(speech2text.asr_train_args, False),
+            preprocess_fn=EENDOLADiarTask.build_preprocess_fn(speech2diar.diar_train_args, False),
+            collate_fn=EENDOLADiarTask.build_collate_fn(speech2diar.diar_train_args, False),
             allow_variable_data_keys=allow_variable_data_keys,
             inference=True,
         )
-        
-        finish_count = 0
-        file_count = 1
-        # 7 .Start for-loop
-        # FIXME(kamo): The output format should be discussed about
-        asr_result_list = []
+
+        # 3. Start for-loop
         output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
         if output_path is not None:
-            writer = DatadirWriter(output_path)
-        else:
-            writer = None
-        
+            os.makedirs(output_path, exist_ok=True)
+            output_writer = open("{}/result.txt".format(output_path), "w")
+        result_list = []
         for keys, batch in loader:
             assert isinstance(batch, dict), type(batch)
             assert all(isinstance(s, str) for s in keys), keys
             _bs = len(next(iter(batch.values())))
             assert len(keys) == _bs, f"{len(keys)} != {_bs}"
             # batch = {k: v[0] for k, v in batch.items() if not k.endswith("_lengths")}
-            # N-best list of (text, token, token_int, hyp_object)
-            try:
-                results = speech2text(**batch)
-            except TooShortUttError as e:
-                logging.warning(f"Utterance {keys} {e}")
-                hyp = Hypothesis(score=0.0, scores={}, states={}, yseq=[])
-                results = [[" ", ["sil"], [2], hyp]] * nbest
-            
+
+            results = speech2diar(**batch)
+
+            # post process
+            a = results[0][0].cpu().numpy()
+            a = medfilt(a, (11, 1))
+            rst = []
+            for spkid, frames in enumerate(a.T):
+                frames = np.pad(frames, (1, 1), 'constant')
+                changes, = np.where(np.diff(frames, axis=0) != 0)
+                fmt = "SPEAKER {:s} 1 {:7.2f} {:7.2f} <NA> <NA> {:s} <NA>"
+                for s, e in zip(changes[::2], changes[1::2]):
+                    st = s / 10.
+                    dur = (e - s) / 10.
+                    rst.append(fmt.format(keys[0], st, dur, "{}_{}".format(keys[0], str(spkid))))
+
             # Only supporting batch_size==1
-            key = keys[0]
-            for n, (text, text_id, token, token_int, hyp) in zip(range(1, nbest + 1), results):
-                # Create a directory: outdir/{n}best_recog
-                if writer is not None:
-                    ibest_writer = writer[f"{n}best_recog"]
-                    
-                    # Write the result to each file
-                    ibest_writer["token"][key] = " ".join(token)
-                    ibest_writer["token_int"][key] = " ".join(map(str, token_int))
-                    ibest_writer["score"][key] = str(hyp.score)
-                    ibest_writer["text_id"][key] = text_id
-                
-                if text is not None:
-                    text_postprocessed, _ = postprocess_utils.sentence_postprocess(token)
-                    item = {'key': key, 'value': text_postprocessed}
-                    asr_result_list.append(item)
-                    finish_count += 1
-                    asr_utils.print_progress(finish_count / file_count)
-                    if writer is not None:
-                        ibest_writer["text"][key] = text
-
-                logging.info("uttid: {}".format(key))
-                logging.info("text predictions: {}".format(text))
-                logging.info("text_id predictions: {}\n".format(text_id))
-        return asr_result_list
-    
+            value = "\n".join(rst)
+            item = {"key": keys[0], "value": value}
+            result_list.append(item)
+            if output_path is not None:
+                output_writer.write(value)
+                output_writer.flush()
+
+        if output_path is not None:
+            output_writer.close()
+
+        return result_list
+
     return _forward
 
+
+
+
+def inference_launch(mode, **kwargs):
+    if mode == "sond":
+        return inference_sond(mode=mode, **kwargs)
+    elif mode == "sond_demo":
+        param_dict = {
+            "extract_profile": True,
+            "sv_train_config": "sv.yaml",
+            "sv_model_file": "sv.pb",
+        }
+        if "param_dict" in kwargs and kwargs["param_dict"] is not None:
+            for key in param_dict:
+                if key not in kwargs["param_dict"]:
+                    kwargs["param_dict"][key] = param_dict[key]
+        else:
+            kwargs["param_dict"] = param_dict
+        return inference_sond(mode=mode, **kwargs)
+    elif mode == "eend-ola":
+        return inference_eend(mode=mode, **kwargs)
+    else:
+        logging.info("Unknown decoding mode: {}".format(mode))
+        return None
+
 def get_parser():
     parser = config_argparse.ArgumentParser(
-        description="ASR Decoding",
+        description="Speaker Verification",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     # Note(kamo): Use '_' instead of '-' as separator.
     # '-' is confusing if written in yaml.
     parser.add_argument(
         "--log_level",
         type=lambda x: x.upper(),
         default="INFO",
         choices=("CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET"),
         help="The verbose level of logging",
     )
 
-    parser.add_argument("--output_dir", type=str, required=True)
+    parser.add_argument("--output_dir", type=str, required=False)
     parser.add_argument(
         "--ngpu",
         type=int,
         default=0,
         help="The number of gpus. 0 indicates CPU mode",
     )
     parser.add_argument(
+        "--njob",
+        type=int,
+        default=1,
+        help="The number of jobs for each gpu",
+    )
+    parser.add_argument(
         "--gpuid_list",
         type=str,
         default="",
         help="The visible gpus",
     )
     parser.add_argument("--seed", type=int, default=0, help="Random seed")
     parser.add_argument(
@@ -560,128 +438,93 @@
     group = parser.add_argument_group("Input data related")
     group.add_argument(
         "--data_path_and_name_and_type",
         type=str2triple_str,
         required=False,
         action="append",
     )
-    group.add_argument("--raw_inputs", type=list, default=None)
-    # example=[{'key':'EdevDEWdIYQ_0021','file':'/mnt/data/jiangyu.xzy/test_data/speech_io/SPEECHIO_ASR_ZH00007_zhibodaihuo/wav/EdevDEWdIYQ_0021.wav'}])
     group.add_argument("--key_file", type=str_or_none)
-    group.add_argument("--allow_variable_data_keys", type=str2bool, default=False)
+    group.add_argument("--allow_variable_data_keys", type=str2bool, default=True)
 
     group = parser.add_argument_group("The model configuration related")
     group.add_argument(
-        "--asr_train_config",
+        "--vad_infer_config",
         type=str,
-        help="ASR training configuration",
-    )
-    group.add_argument(
-        "--asr_model_file",
-        type=str,
-        help="ASR model parameter file",
-    )
-    group.add_argument(
-        "--cmvn_file",
-        type=str,
-        help="Global cmvn file",
+        help="VAD infer configuration",
     )
     group.add_argument(
-        "--lm_train_config",
+        "--vad_model_file",
         type=str,
-        help="LM training configuration",
+        help="VAD model parameter file",
     )
     group.add_argument(
-        "--lm_file",
+        "--diar_train_config",
         type=str,
-        help="LM parameter file",
-    )
-    group.add_argument(
-        "--word_lm_train_config",
-        type=str,
-        help="Word LM training configuration",
+        help="ASR training configuration",
     )
     group.add_argument(
-        "--word_lm_file",
+        "--diar_model_file",
         type=str,
-        help="Word LM parameter file",
+        help="ASR model parameter file",
     )
     group.add_argument(
-        "--ngram_file",
+        "--cmvn_file",
         type=str,
-        help="N-gram parameter file",
+        help="Global CMVN file",
     )
     group.add_argument(
         "--model_tag",
         type=str,
         help="Pretrained model tag. If specify this option, *_train_config and "
              "*_file will be overwritten",
     )
 
-    group = parser.add_argument_group("Beam-search related")
+    group = parser.add_argument_group("The inference configuration related")
     group.add_argument(
         "--batch_size",
         type=int,
         default=1,
         help="The batch size for inference",
     )
-    group.add_argument("--nbest", type=int, default=1, help="Output N-best hypotheses")
-    group.add_argument("--beam_size", type=int, default=20, help="Beam size")
-    group.add_argument("--penalty", type=float, default=0.0, help="Insertion penalty")
-    group.add_argument(
-        "--maxlenratio",
-        type=float,
-        default=0.0,
-        help="Input length ratio to obtain max output length. "
-             "If maxlenratio=0.0 (default), it uses a end-detect "
-             "function "
-             "to automatically find maximum hypothesis lengths."
-             "If maxlenratio<0.0, its absolute value is interpreted"
-             "as a constant max output length",
-    )
     group.add_argument(
-        "--minlenratio",
-        type=float,
-        default=0.0,
-        help="Input length ratio to obtain min output length",
-    )
-    group.add_argument(
-        "--ctc_weight",
-        type=float,
-        default=0.5,
-        help="CTC weight in joint decoding",
-    )
-    group.add_argument("--lm_weight", type=float, default=1.0, help="RNNLM weight")
-    group.add_argument("--ngram_weight", type=float, default=0.9, help="ngram weight")
-    group.add_argument("--streaming", type=str2bool, default=False)
-
-    group = parser.add_argument_group("Text converter related")
-    group.add_argument(
-        "--token_type",
-        type=str_or_none,
-        default=None,
-        choices=["char", "bpe", None],
-        help="The token type for ASR model. "
-             "If not given, refers from the training args",
-    )
-    group.add_argument(
-        "--bpemodel",
-        type=str_or_none,
-        default=None,
-        help="The model path of sentencepiece. "
-             "If not given, refers from the training args",
+        "--diar_smooth_size",
+        type=int,
+        default=121,
+        help="The smoothing size for post-processing"
     )
 
     return parser
 
 
 def main(cmd=None):
     print(get_commandline_args(), file=sys.stderr)
     parser = get_parser()
+    parser.add_argument(
+        "--mode",
+        type=str,
+        default="sond",
+        help="The decoding mode",
+    )
     args = parser.parse_args(cmd)
     kwargs = vars(args)
     kwargs.pop("config", None)
-    inference(**kwargs)
+
+    # set logging messages
+    logging.basicConfig(
+        level=args.log_level,
+        format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
+    )
+    logging.info("Decoding args: {}".format(kwargs))
+
+    # gpu setting
+    if args.ngpu > 0:
+        jobid = int(args.output_dir.split(".")[-1])
+        gpuid = args.gpuid_list.split(",")[(jobid - 1) // args.njob]
+        os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
+        os.environ["CUDA_VISIBLE_DEVICES"] = gpuid
+
+    inference_pipeline = inference_launch(**kwargs)
+    return inference_pipeline(kwargs["data_path_and_name_and_type"])
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `funasr-0.5.3/funasr/bin/tokenize_text.py` & `funasr-0.5.4/funasr/bin/tokenize_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/bin/tp_inference.py` & `funasr-0.5.4/funasr/bin/tp_inference_launch.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+# -*- encoding: utf-8 -*-
+#!/usr/bin/env python3
+# Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
+#  MIT License  (https://opensource.org/licenses/MIT)
+
+
+import argparse
+import logging
+import os
+import sys
+from typing import Union, Dict, Any
+
+from funasr.utils import config_argparse
+from funasr.utils.cli_utils import get_commandline_args
+from funasr.utils.types import str2bool
+from funasr.utils.types import str2triple_str
+from funasr.utils.types import str_or_none
+
 import argparse
 import logging
 from optparse import Option
 import sys
 import json
 from pathlib import Path
 from typing import Any
@@ -25,223 +43,95 @@
 from funasr.utils.cli_utils import get_commandline_args
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
 from funasr.models.frontend.wav_frontend import WavFrontend
 from funasr.text.token_id_converter import TokenIDConverter
 from funasr.utils.timestamp_tools import ts_prediction_lfr6_standard
+from funasr.bin.tp_infer import Speech2Timestamp
 
-
-header_colors = '\033[95m'
-end_colors = '\033[0m'
-
-global_asr_language: str = 'zh-cn'
-global_sample_rate: Union[int, Dict[Any, int]] = {
-    'audio_fs': 16000,
-    'model_fs': 16000
-}
-
-
-class SpeechText2Timestamp:
-    def __init__(
-        self,
-        timestamp_infer_config: Union[Path, str] = None,
-        timestamp_model_file: Union[Path, str] = None,
-        timestamp_cmvn_file: Union[Path, str] = None,
-        device: str = "cpu",
-        dtype: str = "float32",
-        **kwargs,
-    ):
-        assert check_argument_types()
-        # 1. Build ASR model
-        tp_model, tp_train_args = ASRTask.build_model_from_file(
-            timestamp_infer_config, timestamp_model_file, device=device
-        )
-        if 'cuda' in device:
-            tp_model = tp_model.cuda()  # force model to cuda
-
-        frontend = None
-        if tp_train_args.frontend is not None:
-            frontend = WavFrontend(cmvn_file=timestamp_cmvn_file, **tp_train_args.frontend_conf)
-        
-        logging.info("tp_model: {}".format(tp_model))
-        logging.info("tp_train_args: {}".format(tp_train_args))
-        tp_model.to(dtype=getattr(torch, dtype)).eval()
-
-        logging.info(f"Decoding device={device}, dtype={dtype}")
-
-
-        self.tp_model = tp_model
-        self.tp_train_args = tp_train_args
-
-        token_list = self.tp_model.token_list
-        self.converter = TokenIDConverter(token_list=token_list)
-
-        self.device = device
-        self.dtype = dtype
-        self.frontend = frontend
-        self.encoder_downsampling_factor = 1
-        if tp_train_args.encoder_conf["input_layer"] == "conv2d":
-            self.encoder_downsampling_factor = 4
-    
-    @torch.no_grad()
-    def __call__(
-        self, 
-        speech: Union[torch.Tensor, np.ndarray], 
-        speech_lengths: Union[torch.Tensor, np.ndarray] = None, 
-        text_lengths: Union[torch.Tensor, np.ndarray] = None
-    ):
-        assert check_argument_types()
-
-        # Input as audio signal
-        if isinstance(speech, np.ndarray):
-            speech = torch.tensor(speech)
-        if self.frontend is not None:
-            feats, feats_len = self.frontend.forward(speech, speech_lengths)
-            feats = to_device(feats, device=self.device)
-            feats_len = feats_len.int()
-            self.tp_model.frontend = None
-        else:
-            feats = speech
-            feats_len = speech_lengths
-
-        # lfr_factor = max(1, (feats.size()[-1]//80)-1)
-        batch = {"speech": feats, "speech_lengths": feats_len}
-
-        # a. To device
-        batch = to_device(batch, device=self.device)
-
-        # b. Forward Encoder
-        enc, enc_len = self.tp_model.encode(**batch)
-        if isinstance(enc, tuple):
-            enc = enc[0]
-
-        # c. Forward Predictor
-        _, _, us_alphas, us_peaks = self.tp_model.calc_predictor_timestamp(enc, enc_len, text_lengths.to(self.device)+1)
-        return us_alphas, us_peaks
-
-
-def inference(
-        batch_size: int,
-        ngpu: int,
-        log_level: Union[int, str],
-        data_path_and_name_and_type,
-        timestamp_infer_config: Optional[str],
-        timestamp_model_file: Optional[str],
-        timestamp_cmvn_file: Optional[str] = None,
-        raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-        key_file: Optional[str] = None,
-        allow_variable_data_keys: bool = False,
-        output_dir: Optional[str] = None,
-        dtype: str = "float32",
-        seed: int = 0,
-        num_workers: int = 1,
-        split_with_space: bool = True,
-        seg_dict_file: Optional[str] = None,
-        **kwargs,
-):
-    inference_pipeline = inference_modelscope(
-        batch_size=batch_size,
-        ngpu=ngpu,
-        log_level=log_level,
-        timestamp_infer_config=timestamp_infer_config,
-        timestamp_model_file=timestamp_model_file,
-        timestamp_cmvn_file=timestamp_cmvn_file,
-        key_file=key_file,
-        allow_variable_data_keys=allow_variable_data_keys,
-        output_dir=output_dir,
-        dtype=dtype,
-        seed=seed,
-        num_workers=num_workers,
-        split_with_space=split_with_space,
-        seg_dict_file=seg_dict_file,
-        **kwargs,
-    )
-    return inference_pipeline(data_path_and_name_and_type, raw_inputs)
-
-
-def inference_modelscope(
-        batch_size: int,
-        ngpu: int,
-        log_level: Union[int, str],
-        # data_path_and_name_and_type,
-        timestamp_infer_config: Optional[str],
-        timestamp_model_file: Optional[str],
-        timestamp_cmvn_file: Optional[str] = None,
-        # raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-        key_file: Optional[str] = None,
-        allow_variable_data_keys: bool = False,
-        output_dir: Optional[str] = None,
-        dtype: str = "float32",
-        seed: int = 0,
-        num_workers: int = 1,
-        split_with_space: bool = True,
-        seg_dict_file: Optional[str] = None,
-        **kwargs,
+def inference_tp(
+    batch_size: int,
+    ngpu: int,
+    log_level: Union[int, str],
+    # data_path_and_name_and_type,
+    timestamp_infer_config: Optional[str],
+    timestamp_model_file: Optional[str],
+    timestamp_cmvn_file: Optional[str] = None,
+    # raw_inputs: Union[np.ndarray, torch.Tensor] = None,
+    key_file: Optional[str] = None,
+    allow_variable_data_keys: bool = False,
+    output_dir: Optional[str] = None,
+    dtype: str = "float32",
+    seed: int = 0,
+    num_workers: int = 1,
+    split_with_space: bool = True,
+    seg_dict_file: Optional[str] = None,
+    **kwargs,
 ):
     assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
     
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
-
+    
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
-
+    
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
     # 1. Set random-seed
     set_all_random_seed(seed)
-
+    
     # 2. Build speech2vadsegment
     speechtext2timestamp_kwargs = dict(
         timestamp_infer_config=timestamp_infer_config,
         timestamp_model_file=timestamp_model_file,
         timestamp_cmvn_file=timestamp_cmvn_file,
         device=device,
         dtype=dtype,
     )
     logging.info("speechtext2timestamp_kwargs: {}".format(speechtext2timestamp_kwargs))
-    speechtext2timestamp = SpeechText2Timestamp(**speechtext2timestamp_kwargs)
-
+    speechtext2timestamp = Speech2Timestamp(**speechtext2timestamp_kwargs)
+    
     preprocessor = LMPreprocessor(
         train=False,
         token_type=speechtext2timestamp.tp_train_args.token_type,
         token_list=speechtext2timestamp.tp_train_args.token_list,
         bpemodel=None,
         text_cleaner=None,
         g2p_type=None,
         text_name="text",
         non_linguistic_symbols=speechtext2timestamp.tp_train_args.non_linguistic_symbols,
         split_with_space=split_with_space,
         seg_dict_file=seg_dict_file,
     )
-
+    
     if output_dir is not None:
         writer = DatadirWriter(output_dir)
         tp_writer = writer[f"timestamp_prediction"]
         # ibest_writer["token_list"][""] = " ".join(speech2text.asr_train_args.token_list)
     else:
         tp_writer = None
     
     def _forward(
-            data_path_and_name_and_type,
-            raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-            output_dir_v2: Optional[str] = None,
-            fs: dict = None,
-            param_dict: dict = None,
-            **kwargs
-    ):  
+        data_path_and_name_and_type,
+        raw_inputs: Union[np.ndarray, torch.Tensor] = None,
+        output_dir_v2: Optional[str] = None,
+        fs: dict = None,
+        param_dict: dict = None,
+        **kwargs
+    ):
         output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
         writer = None
         if output_path is not None:
             writer = DatadirWriter(output_path)
             tp_writer = writer[f"timestamp_prediction"]
         else:
             tp_writer = None
@@ -258,43 +148,53 @@
             key_file=key_file,
             num_workers=num_workers,
             preprocess_fn=preprocessor,
             collate_fn=ASRTask.build_collate_fn(speechtext2timestamp.tp_train_args, False),
             allow_variable_data_keys=allow_variable_data_keys,
             inference=True,
         )
-
+        
         tp_result_list = []
         for keys, batch in loader:
             assert isinstance(batch, dict), type(batch)
             assert all(isinstance(s, str) for s in keys), keys
             _bs = len(next(iter(batch.values())))
             assert len(keys) == _bs, f"{len(keys)} != {_bs}"
-
+            
             logging.info("timestamp predicting, utt_id: {}".format(keys))
-            _batch = {'speech':batch['speech'], 
-                      'speech_lengths':batch['speech_lengths'],
-                      'text_lengths':batch['text_lengths']}
+            _batch = {'speech': batch['speech'],
+                      'speech_lengths': batch['speech_lengths'],
+                      'text_lengths': batch['text_lengths']}
             us_alphas, us_cif_peak = speechtext2timestamp(**_batch)
-
+            
             for batch_id in range(_bs):
                 key = keys[batch_id]
                 token = speechtext2timestamp.converter.ids2tokens(batch['text'][batch_id])
-                ts_str, ts_list = ts_prediction_lfr6_standard(us_alphas[batch_id], us_cif_peak[batch_id], token, force_time_shift=-3.0)
+                ts_str, ts_list = ts_prediction_lfr6_standard(us_alphas[batch_id], us_cif_peak[batch_id], token,
+                                                              force_time_shift=-3.0)
                 logging.warning(ts_str)
-                item = {'key': key, 'value': ts_str, 'timestamp':ts_list}
+                item = {'key': key, 'value': ts_str, 'timestamp': ts_list}
                 if tp_writer is not None:
-                    tp_writer["tp_sync"][key+'#'] = ts_str
-                    tp_writer["tp_time"][key+'#'] = str(ts_list)
+                    tp_writer["tp_sync"][key + '#'] = ts_str
+                    tp_writer["tp_time"][key + '#'] = str(ts_list)
                 tp_result_list.append(item)
         return tp_result_list
-
+    
     return _forward
 
 
+
+
+def inference_launch(mode, **kwargs):
+    if mode == "tp_norm":
+        return inference_tp(**kwargs)
+    else:
+        logging.info("Unknown decoding mode: {}".format(mode))
+        return None
+
 def get_parser():
     parser = config_argparse.ArgumentParser(
         description="Timestamp Prediction Inference",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     # Note(kamo): Use '_' instead of '-' as separator.
@@ -311,14 +211,20 @@
     parser.add_argument(
         "--ngpu",
         type=int,
         default=0,
         help="The number of gpus. 0 indicates CPU mode",
     )
     parser.add_argument(
+        "--njob",
+        type=int,
+        default=1,
+        help="The number of jobs for each gpu",
+    )
+    parser.add_argument(
         "--gpuid_list",
         type=str,
         default="",
         help="The visible gpus",
     )
     parser.add_argument("--seed", type=int, default=0, help="Random seed")
     parser.add_argument(
@@ -326,27 +232,25 @@
         default="float32",
         choices=["float16", "float32", "float64"],
         help="Data type",
     )
     parser.add_argument(
         "--num_workers",
         type=int,
-        default=0,
+        default=1,
         help="The number of workers used for DataLoader",
     )
 
     group = parser.add_argument_group("Input data related")
     group.add_argument(
         "--data_path_and_name_and_type",
         type=str2triple_str,
-        required=False,
+        required=True,
         action="append",
     )
-    group.add_argument("--raw_inputs", type=list, default=None)
-    # example=[{'key':'EdevDEWdIYQ_0021','file':'/mnt/data/jiangyu.xzy/test_data/speech_io/SPEECHIO_ASR_ZH00007_zhibodaihuo/wav/EdevDEWdIYQ_0021.wav'}])
     group.add_argument("--key_file", type=str_or_none)
     group.add_argument("--allow_variable_data_keys", type=str2bool, default=False)
 
     group = parser.add_argument_group("The model configuration related")
     group.add_argument(
         "--timestamp_infer_config",
         type=str,
@@ -356,44 +260,54 @@
         "--timestamp_model_file",
         type=str,
         help="VAD model parameter file",
     )
     group.add_argument(
         "--timestamp_cmvn_file",
         type=str,
-        help="Global cmvn file",
+        help="Global CMVN file",
     )
 
-    group = parser.add_argument_group("infer related")
+    group = parser.add_argument_group("The inference configuration related")
     group.add_argument(
         "--batch_size",
         type=int,
         default=1,
         help="The batch size for inference",
     )
-    group.add_argument(
-        "--seg_dict_file",
-        type=str,
-        default=None,
-        help="The batch size for inference",
-    )
-    group.add_argument(
-        "--split_with_space",
-        type=bool,
-        default=False,
-        help="The batch size for inference",
-    )
-
     return parser
 
 
 def main(cmd=None):
     print(get_commandline_args(), file=sys.stderr)
     parser = get_parser()
+    parser.add_argument(
+        "--mode",
+        type=str,
+        default="tp_norm",
+        help="The decoding mode",
+    )
     args = parser.parse_args(cmd)
     kwargs = vars(args)
     kwargs.pop("config", None)
-    inference(**kwargs)
+
+    # set logging messages
+    logging.basicConfig(
+        level=args.log_level,
+        format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
+    )
+    logging.info("Decoding args: {}".format(kwargs))
+
+    # gpu setting
+    if args.ngpu > 0:
+        jobid = int(args.output_dir.split(".")[-1])
+        gpuid = args.gpuid_list.split(",")[(jobid - 1) // args.njob]
+        os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
+        os.environ["CUDA_VISIBLE_DEVICES"] = gpuid
+
+    inference_pipeline = inference_launch(**kwargs)
+    return inference_pipeline(kwargs["data_path_and_name_and_type"])
+
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `funasr-0.5.3/funasr/bin/vad_inference_online.py` & `funasr-0.5.4/funasr/bin/sv_inference_launch.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,260 +1,194 @@
+# -*- encoding: utf-8 -*-
+#!/usr/bin/env python3
+# Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
+#  MIT License  (https://opensource.org/licenses/MIT)
+
+import argparse
+import logging
+import os
+import sys
+from typing import Union, Dict, Any
+
+from funasr.utils import config_argparse
+from funasr.utils.cli_utils import get_commandline_args
+from funasr.utils.types import str2bool
+from funasr.utils.types import str2triple_str
+from funasr.utils.types import str_or_none
 import argparse
 import logging
 import os
 import sys
-import json
 from pathlib import Path
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Union
-from typing import Dict
 
 import numpy as np
 import torch
+from kaldiio import WriteHelper
 from typeguard import check_argument_types
 from typeguard import check_return_type
 
-from funasr.fileio.datadir_writer import DatadirWriter
-from funasr.tasks.vad import VADTask
+from funasr.utils.cli_utils import get_commandline_args
+from funasr.tasks.sv import SVTask
 from funasr.torch_utils.device_funcs import to_device
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.utils import config_argparse
-from funasr.utils.cli_utils import get_commandline_args
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
-from funasr.models.frontend.wav_frontend import WavFrontendOnline
-from funasr.models.frontend.wav_frontend import WavFrontend
-from funasr.bin.vad_inference import Speech2VadSegment
-
-header_colors = '\033[95m'
-end_colors = '\033[0m'
-
-
-class Speech2VadSegmentOnline(Speech2VadSegment):
-    """Speech2VadSegmentOnline class
-
-    Examples:
-        >>> import soundfile
-        >>> speech2segment = Speech2VadSegmentOnline("vad_config.yml", "vad.pt")
-        >>> audio, rate = soundfile.read("speech.wav")
-        >>> speech2segment(audio)
-        [[10, 230], [245, 450], ...]
-
-    """
-    def __init__(self, **kwargs):
-        super(Speech2VadSegmentOnline, self).__init__(**kwargs)
-        vad_cmvn_file = kwargs.get('vad_cmvn_file', None)
-        self.frontend = None
-        if self.vad_infer_args.frontend is not None:
-            self.frontend = WavFrontendOnline(cmvn_file=vad_cmvn_file, **self.vad_infer_args.frontend_conf)
-
-
-    @torch.no_grad()
-    def __call__(
-            self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None,
-            in_cache: Dict[str, torch.Tensor] = dict(), is_final: bool = False, max_end_sil: int = 800
-    ) -> Tuple[torch.Tensor, List[List[int]], torch.Tensor]:
-        """Inference
-
-        Args:
-            speech: Input speech data
-        Returns:
-            text, token, token_int, hyp
-
-        """
-        assert check_argument_types()
-
-        # Input as audio signal
-        if isinstance(speech, np.ndarray):
-            speech = torch.tensor(speech)
-        batch_size = speech.shape[0]
-        segments = [[]] * batch_size
-        if self.frontend is not None:
-            feats, feats_len = self.frontend.forward(speech, speech_lengths, is_final)
-            fbanks, _ = self.frontend.get_fbank()
-        else:
-            raise Exception("Need to extract feats first, please configure frontend configuration")
-        if feats.shape[0]:
-            feats = to_device(feats, device=self.device)
-            feats_len = feats_len.int()
-            waveforms = self.frontend.get_waveforms()
-
-            batch = {
-                "feats": feats,
-                "waveform": waveforms,
-                "in_cache": in_cache,
-                "is_final": is_final,
-                "max_end_sil": max_end_sil
-            }
-            # a. To device
-            batch = to_device(batch, device=self.device)
-            segments, in_cache = self.vad_model.forward_online(**batch)
-            # in_cache.update(batch['in_cache'])
-            # in_cache = {key: value for key, value in batch['in_cache'].items()}
-        return fbanks, segments, in_cache
-
-
-def inference(
-        batch_size: int,
-        ngpu: int,
-        log_level: Union[int, str],
-        data_path_and_name_and_type,
-        vad_infer_config: Optional[str],
-        vad_model_file: Optional[str],
-        vad_cmvn_file: Optional[str] = None,
-        raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-        key_file: Optional[str] = None,
-        allow_variable_data_keys: bool = False,
-        output_dir: Optional[str] = None,
-        dtype: str = "float32",
-        seed: int = 0,
-        num_workers: int = 1,
-        **kwargs,
-):
-    inference_pipeline = inference_modelscope(
-        batch_size=batch_size,
-        ngpu=ngpu,
-        log_level=log_level,
-        vad_infer_config=vad_infer_config,
-        vad_model_file=vad_model_file,
-        vad_cmvn_file=vad_cmvn_file,
-        key_file=key_file,
-        allow_variable_data_keys=allow_variable_data_keys,
-        output_dir=output_dir,
-        dtype=dtype,
-        seed=seed,
-        num_workers=num_workers,
-        **kwargs,
-    )
-    return inference_pipeline(data_path_and_name_and_type, raw_inputs)
-
-
-def inference_modelscope(
-        batch_size: int,
-        ngpu: int,
-        log_level: Union[int, str],
-        # data_path_and_name_and_type,
-        vad_infer_config: Optional[str],
-        vad_model_file: Optional[str],
-        vad_cmvn_file: Optional[str] = None,
-        # raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-        key_file: Optional[str] = None,
-        allow_variable_data_keys: bool = False,
-        output_dir: Optional[str] = None,
-        dtype: str = "float32",
-        seed: int = 0,
-        num_workers: int = 1,
-        **kwargs,
+from funasr.utils.misc import statistic_model_parameters
+from funasr.bin.sv_infer import Speech2Xvector
+
+def inference_sv(
+    output_dir: Optional[str] = None,
+    batch_size: int = 1,
+    dtype: str = "float32",
+    ngpu: int = 1,
+    seed: int = 0,
+    num_workers: int = 0,
+    log_level: Union[int, str] = "INFO",
+    key_file: Optional[str] = None,
+    sv_train_config: Optional[str] = "sv.yaml",
+    sv_model_file: Optional[str] = "sv.pb",
+    model_tag: Optional[str] = None,
+    allow_variable_data_keys: bool = True,
+    streaming: bool = False,
+    embedding_node: str = "resnet1_dense",
+    sv_threshold: float = 0.9465,
+    param_dict: Optional[dict] = None,
+    **kwargs,
 ):
     assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
     
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
-
+    if ngpu > 1:
+        raise NotImplementedError("only single GPU decoding is supported")
+    
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
-
+    logging.info("param_dict: {}".format(param_dict))
+    
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
-        batch_size = 1
+    
     # 1. Set random-seed
     set_all_random_seed(seed)
-
-    # 2. Build speech2vadsegment
-    speech2vadsegment_kwargs = dict(
-        vad_infer_config=vad_infer_config,
-        vad_model_file=vad_model_file,
-        vad_cmvn_file=vad_cmvn_file,
+    
+    # 2. Build speech2xvector
+    speech2xvector_kwargs = dict(
+        sv_train_config=sv_train_config,
+        sv_model_file=sv_model_file,
         device=device,
         dtype=dtype,
+        streaming=streaming,
+        embedding_node=embedding_node
     )
-    logging.info("speech2vadsegment_kwargs: {}".format(speech2vadsegment_kwargs))
-    speech2vadsegment = Speech2VadSegmentOnline(**speech2vadsegment_kwargs)
-
+    logging.info("speech2xvector_kwargs: {}".format(speech2xvector_kwargs))
+    speech2xvector = Speech2Xvector.from_pretrained(
+        model_tag=model_tag,
+        **speech2xvector_kwargs,
+    )
+    speech2xvector.sv_model.eval()
+    
     def _forward(
-            data_path_and_name_and_type,
-            raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-            output_dir_v2: Optional[str] = None,
-            fs: dict = None,
-            param_dict: dict = None,
+        data_path_and_name_and_type: Sequence[Tuple[str, str, str]] = None,
+        raw_inputs: Union[np.ndarray, torch.Tensor] = None,
+        output_dir_v2: Optional[str] = None,
+        param_dict: Optional[dict] = None,
     ):
-        # 3. Build data-iterator
+        logging.info("param_dict: {}".format(param_dict))
         if data_path_and_name_and_type is None and raw_inputs is not None:
             if isinstance(raw_inputs, torch.Tensor):
                 raw_inputs = raw_inputs.numpy()
             data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
-        loader = VADTask.build_streaming_iterator(
+        
+        # 3. Build data-iterator
+        loader = SVTask.build_streaming_iterator(
             data_path_and_name_and_type,
             dtype=dtype,
             batch_size=batch_size,
             key_file=key_file,
             num_workers=num_workers,
-            preprocess_fn=VADTask.build_preprocess_fn(speech2vadsegment.vad_infer_args, False),
-            collate_fn=VADTask.build_collate_fn(speech2vadsegment.vad_infer_args, False),
+            preprocess_fn=None,
+            collate_fn=None,
             allow_variable_data_keys=allow_variable_data_keys,
             inference=True,
         )
-
-        finish_count = 0
-        file_count = 1
+        
         # 7 .Start for-loop
-        # FIXME(kamo): The output format should be discussed about
         output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
+        embd_writer, ref_embd_writer, score_writer = None, None, None
         if output_path is not None:
-            writer = DatadirWriter(output_path)
-            ibest_writer = writer[f"1best_recog"]
-        else:
-            writer = None
-            ibest_writer = None
-
-        vad_results = []
-        batch_in_cache = param_dict['in_cache'] if param_dict is not None else dict()
-        is_final = param_dict.get('is_final', False) if param_dict is not None else False
-        max_end_sil = param_dict.get('max_end_sil', 800) if param_dict is not None else 800
+            os.makedirs(output_path, exist_ok=True)
+            embd_writer = WriteHelper("ark,scp:{}/xvector.ark,{}/xvector.scp".format(output_path, output_path))
+        sv_result_list = []
         for keys, batch in loader:
             assert isinstance(batch, dict), type(batch)
             assert all(isinstance(s, str) for s in keys), keys
             _bs = len(next(iter(batch.values())))
             assert len(keys) == _bs, f"{len(keys)} != {_bs}"
-            batch['in_cache'] = batch_in_cache
-            batch['is_final'] = is_final
-            batch['max_end_sil'] = max_end_sil
-
-            # do vad segment
-            _, results, param_dict['in_cache'] = speech2vadsegment(**batch)
-            # param_dict['in_cache'] = batch['in_cache']
-            if results:
-                for i, _ in enumerate(keys):
-                    if results[i]:
-                        if "MODELSCOPE_ENVIRONMENT" in os.environ and os.environ["MODELSCOPE_ENVIRONMENT"] == "eas":
-                            results[i] = json.dumps(results[i])
-                        item = {'key': keys[i], 'value': results[i]}
-                        vad_results.append(item)
-                        if writer is not None:
-                            ibest_writer["text"][keys[i]] = "{}".format(results[i])
+            batch = {k: v[0] for k, v in batch.items() if not k.endswith("_lengths")}
+            
+            embedding, ref_embedding, score = speech2xvector(**batch)
+            # Only supporting batch_size==1
+            key = keys[0]
+            normalized_score = 0.0
+            if score is not None:
+                score = score.item()
+                normalized_score = max(score - sv_threshold, 0.0) / (1.0 - sv_threshold) * 100.0
+                item = {"key": key, "value": normalized_score}
+            else:
+                item = {"key": key, "value": embedding.squeeze(0).cpu().numpy()}
+            sv_result_list.append(item)
+            if output_path is not None:
+                embd_writer(key, embedding[0].cpu().numpy())
+                if ref_embedding is not None:
+                    if ref_embd_writer is None:
+                        ref_embd_writer = WriteHelper(
+                            "ark,scp:{}/ref_xvector.ark,{}/ref_xvector.scp".format(output_path, output_path)
+                        )
+                        score_writer = open(os.path.join(output_path, "score.txt"), "w")
+                    ref_embd_writer(key, ref_embedding[0].cpu().numpy())
+                    score_writer.write("{} {:.6f}\n".format(key, normalized_score))
+        
+        if output_path is not None:
+            embd_writer.close()
+            if ref_embd_writer is not None:
+                ref_embd_writer.close()
+                score_writer.close()
+        
+        return sv_result_list
+    
+    return _forward
+
 
-        return vad_results
 
-    return _forward
 
+def inference_launch(mode, **kwargs):
+    if mode == "sv":
+        return inference_sv(**kwargs)
+    else:
+        logging.info("Unknown decoding mode: {}".format(mode))
+        return None
 
 def get_parser():
     parser = config_argparse.ArgumentParser(
-        description="VAD Decoding",
+        description="Speaker Verification",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     # Note(kamo): Use '_' instead of '-' as separator.
     # '-' is confusing if written in yaml.
     parser.add_argument(
         "--log_level",
@@ -268,14 +202,20 @@
     parser.add_argument(
         "--ngpu",
         type=int,
         default=0,
         help="The number of gpus. 0 indicates CPU mode",
     )
     parser.add_argument(
+        "--njob",
+        type=int,
+        default=1,
+        help="The number of jobs for each gpu",
+    )
+    parser.add_argument(
         "--gpuid_list",
         type=str,
         default="",
         help="The visible gpus",
     )
     parser.add_argument("--seed", type=int, default=0, help="Random seed")
     parser.add_argument(
@@ -294,51 +234,99 @@
     group = parser.add_argument_group("Input data related")
     group.add_argument(
         "--data_path_and_name_and_type",
         type=str2triple_str,
         required=False,
         action="append",
     )
-    group.add_argument("--raw_inputs", type=list, default=None)
-    # example=[{'key':'EdevDEWdIYQ_0021','file':'/mnt/data/jiangyu.xzy/test_data/speech_io/SPEECHIO_ASR_ZH00007_zhibodaihuo/wav/EdevDEWdIYQ_0021.wav'}])
     group.add_argument("--key_file", type=str_or_none)
-    group.add_argument("--allow_variable_data_keys", type=str2bool, default=False)
+    group.add_argument("--allow_variable_data_keys", type=str2bool, default=True)
 
     group = parser.add_argument_group("The model configuration related")
     group.add_argument(
         "--vad_infer_config",
         type=str,
         help="VAD infer configuration",
     )
     group.add_argument(
         "--vad_model_file",
         type=str,
         help="VAD model parameter file",
     )
     group.add_argument(
-        "--vad_cmvn_file",
+        "--sv_train_config",
+        type=str,
+        help="ASR training configuration",
+    )
+    group.add_argument(
+        "--sv_model_file",
+        type=str,
+        help="ASR model parameter file",
+    )
+    group.add_argument(
+        "--cmvn_file",
+        type=str,
+        help="Global CMVN file",
+    )
+    group.add_argument(
+        "--model_tag",
         type=str,
-        help="Global cmvn file",
+        help="Pretrained model tag. If specify this option, *_train_config and "
+             "*_file will be overwritten",
     )
 
-    group = parser.add_argument_group("infer related")
+    group = parser.add_argument_group("The inference configuration related")
     group.add_argument(
         "--batch_size",
         type=int,
         default=1,
         help="The batch size for inference",
     )
+    group.add_argument(
+        "--sv_threshold",
+        type=float,
+        default=0.9465,
+        help="The threshold for verification"
+    )
+    parser.add_argument(
+        "--embedding_node",
+        type=str,
+        default="resnet1_dense",
+        help="The network node to extract embedding"
+    )
 
     return parser
 
 
 def main(cmd=None):
     print(get_commandline_args(), file=sys.stderr)
     parser = get_parser()
+    parser.add_argument(
+        "--mode",
+        type=str,
+        default="sv",
+        help="The decoding mode",
+    )
     args = parser.parse_args(cmd)
     kwargs = vars(args)
     kwargs.pop("config", None)
-    inference(**kwargs)
+
+    # set logging messages
+    logging.basicConfig(
+        level=args.log_level,
+        format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
+    )
+    logging.info("Decoding args: {}".format(kwargs))
+
+    # gpu setting
+    if args.ngpu > 0:
+        jobid = int(args.output_dir.split(".")[-1])
+        gpuid = args.gpuid_list.split(",")[(jobid - 1) // args.njob]
+        os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
+        os.environ["CUDA_VISIBLE_DEVICES"] = gpuid
+
+    inference_pipeline = inference_launch(**kwargs)
+    return inference_pipeline(kwargs["data_path_and_name_and_type"])
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `funasr-0.5.3/funasr/datasets/collate_fn.py` & `funasr-0.5.4/funasr/datasets/collate_fn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/datasets/dataset.py` & `funasr-0.5.4/funasr/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/datasets/iterable_dataset.py` & `funasr-0.5.4/funasr/datasets/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/datasets/large_datasets/build_dataloader.py` & `funasr-0.5.4/funasr/datasets/large_datasets/build_dataloader.py`

 * *Files 9% similar despite different names*

```diff
@@ -60,36 +60,34 @@
         return self.sp.EncodeAsPieces(line)
 
     def tokens2text(self, tokens: Iterable[str]) -> str:
         self._build_sentence_piece_processor()
         return self.sp.DecodePieces(list(tokens))
 
 
-class ArkDataLoader(AbsIterFactory):
-    def __init__(self, data_list, dict_file, dataset_conf, frontend_conf=None, seg_dict_file=None, punc_dict_file=None,
-                 bpemodel_file=None, mode="train"):
-        symbol_table = read_symbol_table(dict_file) if dict_file is not None else None
-        if seg_dict_file is not None:
-            seg_dict = load_seg_dict(seg_dict_file)
-        else:
-            seg_dict = None
-        if punc_dict_file is not None:
-            punc_dict = read_symbol_table(punc_dict_file)
-        else:
-            punc_dict = None
-        self.dataset_conf = dataset_conf
-        self.frontend_conf = frontend_conf
+class LargeDataLoader(AbsIterFactory):
+    def __init__(self, args, mode="train"):
+        symbol_table, seg_dict, punc_dict, bpe_tokenizer = None, None, None, None
+        if hasattr(args, "token_list") and args.token_list is not None:
+            symbol_table = read_symbol_table(args.token_list)
+        if hasattr(args, "seg_dict_file") and args.seg_dict_file is not None:
+            seg_dict = load_seg_dict(args.seg_dict_file)
+        if hasattr(args, "punc_dict_file") and args.punc_dict_file is not None:
+            punc_dict = read_symbol_table(args.punc_dict_file)
+        if hasattr(args, "bpemodel_file") and args.bpemodel_file is not None:
+            bpe_tokenizer = SentencepiecesTokenizer(args.bpemodel_file)
+        self.dataset_conf = args.dataset_conf
+        self.frontend_conf = args.frontend_conf
         logging.info("dataloader config: {}".format(self.dataset_conf))
         batch_mode = self.dataset_conf.get("batch_mode", "padding")
-        if bpemodel_file is not None:
-            bpe_tokenizer = SentencepiecesTokenizer(bpemodel_file)
-        else:
-            bpe_tokenizer = None
+        data_list = args.train_data_file if mode == "train" else args.valid_data_file
         self.dataset = Dataset(data_list, symbol_table, seg_dict, punc_dict, bpe_tokenizer,
-                               self.dataset_conf, self.frontend_conf, mode=mode, batch_mode=batch_mode)
+                               self.dataset_conf, self.frontend_conf,
+                               speed_perturb=args.speed_perturb if mode == "train" else None,
+                               mode=mode, batch_mode=batch_mode)
 
     def build_iter(self, epoch, shuffle=True):
         self.dataset.set_epoch(epoch)
         data_loader = DataLoader(self.dataset,
                                  batch_size=None,
                                  pin_memory=True,
                                  num_workers=self.dataset_conf.get("num_workers", 8))
```

### Comparing `funasr-0.5.3/funasr/datasets/large_datasets/datapipes/batch.py` & `funasr-0.5.4/funasr/datasets/large_datasets/datapipes/batch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/datasets/large_datasets/datapipes/filter.py` & `funasr-0.5.4/funasr/datasets/large_datasets/datapipes/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/datasets/large_datasets/dataset.py` & `funasr-0.5.4/funasr/datasets/large_datasets/dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,53 @@
+import logging
 import os
 import random
-import numpy
 from functools import partial
 
 import torch
-import torchaudio
 import torch.distributed as dist
+import torchaudio
 from kaldiio import ReadHelper
 from torch.utils.data import IterableDataset
 
 from funasr.datasets.large_datasets.datapipes.batch import MaxTokenBucketizerIterDataPipe
 from funasr.datasets.large_datasets.datapipes.filter import FilterIterDataPipe
 from funasr.datasets.large_datasets.datapipes.map import MapperIterDataPipe
+from funasr.datasets.large_datasets.utils.clipping import clipping
 from funasr.datasets.large_datasets.utils.filter import filter
 from funasr.datasets.large_datasets.utils.padding import padding
-from funasr.datasets.large_datasets.utils.clipping import clipping
 from funasr.datasets.large_datasets.utils.tokenize import tokenize
 
 
 def read_lists(list_file):
     lists = []
     with open(list_file, 'r', encoding='utf8') as fin:
         for line in fin:
             parts = line.strip()
             lists.append(parts)
     return lists
 
 
 class AudioDataset(IterableDataset):
-    def __init__(self, scp_lists, data_names, data_types, frontend_conf=None, shuffle=True, mode="train"):
+    def __init__(self, scp_lists, data_names, data_types, frontend_conf=None, shuffle=True, speed_perturb=None,
+                 mode="train"):
         self.scp_lists = scp_lists
         self.data_names = data_names
         self.data_types = data_types
         self.frontend_conf = frontend_conf
         self.shuffle = shuffle
         self.mode = mode
         self.epoch = -1
         self.rank = 0
         self.world_size = 1
         self.worker_id = 0
         self.num_workers = 1
+        self.speed_perturb = speed_perturb
+        if self.speed_perturb is not None:
+            logging.info("Using speed_perturb: {}".format(speed_perturb))
 
     def set_epoch(self, epoch):
         self.epoch = epoch
 
     def get_rank_data_list(self, data_index):
         assert dist.is_available()
         if dist.is_initialized():
@@ -120,17 +124,23 @@
                     elif data_type == "sound":
                         key, path = item.strip().split()
                         waveform, sampling_rate = torchaudio.load(path)
                         if self.frontend_conf is not None:
                             if sampling_rate != self.frontend_conf["fs"]:
                                 waveform = torchaudio.transforms.Resample(orig_freq=sampling_rate,
                                                                           new_freq=self.frontend_conf["fs"])(waveform)
-                                sampling_rate = self.frontend_conf["fs"] 
+                                sampling_rate = self.frontend_conf["fs"]
                         waveform = waveform.numpy()
                         mat = waveform[0]
+                        if self.speed_perturb is not None:
+                            speed = random.choice(self.speed_perturb)
+                            if speed != 1.0:
+                                mat, _ = torchaudio.sox_effects.apply_effects_tensor(
+                                    torch.tensor(mat).view(1, -1), sampling_rate, [['speed', str(speed)], ['rate', str(sampling_rate)]])
+                                mat = mat.view(-1).numpy()
                         sample_dict[data_name] = mat
                         sample_dict["sampling_rate"] = sampling_rate
                         if data_name == "speech":
                             sample_dict["key"] = key
                     elif data_type == "text_hotword":
                         text = item
                         segs = text.strip().split()
@@ -164,14 +174,15 @@
 def Dataset(data_list_file,
             dict,
             seg_dict,
             punc_dict,
             bpe_tokenizer,
             conf,
             frontend_conf,
+            speed_perturb=None,
             mode="train",
             batch_mode="padding"):
     scp_lists = read_lists(data_list_file)
     shuffle = conf.get('shuffle', True)
     data_names = conf.get("data_names", "speech,text")
     data_types = conf.get("data_types", "kaldi_ark,text")
 
@@ -192,15 +203,16 @@
     else:
         pre_hwlist = None
 
     dataset = AudioDataset(scp_lists, 
                            data_names, 
                            data_types, 
                            frontend_conf=frontend_conf, 
-                           shuffle=shuffle, 
+                           shuffle=shuffle,
+                           speed_perturb=speed_perturb,
                            mode=mode, 
                            )
 
     filter_conf = conf.get('filter_conf', {})
     filter_fn = partial(filter, **filter_conf)
     dataset = FilterIterDataPipe(dataset, fn=filter_fn)
```

### Comparing `funasr-0.5.3/funasr/datasets/large_datasets/utils/clipping.py` & `funasr-0.5.4/funasr/datasets/large_datasets/utils/clipping.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/datasets/large_datasets/utils/filter.py` & `funasr-0.5.4/funasr/datasets/large_datasets/utils/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/datasets/large_datasets/utils/hotword_utils.py` & `funasr-0.5.4/funasr/datasets/large_datasets/utils/hotword_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/datasets/large_datasets/utils/low_frame_rate.py` & `funasr-0.5.4/funasr/datasets/large_datasets/utils/low_frame_rate.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/datasets/large_datasets/utils/padding.py` & `funasr-0.5.4/funasr/datasets/large_datasets/utils/padding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/datasets/large_datasets/utils/tokenize.py` & `funasr-0.5.4/funasr/datasets/large_datasets/utils/tokenize.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     assert "text" in data
     assert isinstance(vocab, dict)
     text = data["text"]
     token = []
     vad = -2
 
     if bpe_tokenizer is not None:
-        text = bpe_tokenizer.text2tokens("".join(text))
+        text = bpe_tokenizer.text2tokens(text)
 
     if seg_dict is not None:
         assert isinstance(seg_dict, dict)
         text = seg_tokenize(text, seg_dict)
 
     length = len(text)
     if 'hw_tag' in data:
```

### Comparing `funasr-0.5.3/funasr/datasets/ms_dataset.py` & `funasr-0.5.4/funasr/datasets/ms_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/export/export_model.py` & `funasr-0.5.4/funasr/export/export_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/export/models/CT_Transformer.py` & `funasr-0.5.4/funasr/export/models/CT_Transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/export/models/__init__.py` & `funasr-0.5.4/funasr/export/models/__init__.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/export/models/decoder/sanm_decoder.py` & `funasr-0.5.4/funasr/export/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/export/models/decoder/transformer_decoder.py` & `funasr-0.5.4/funasr/export/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/export/models/e2e_asr_paraformer.py` & `funasr-0.5.4/funasr/export/models/e2e_asr_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/export/models/e2e_vad.py` & `funasr-0.5.4/funasr/export/models/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/export/models/encoder/conformer_encoder.py` & `funasr-0.5.4/funasr/export/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/export/models/encoder/fsmn_encoder.py` & `funasr-0.5.4/funasr/export/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/export/models/encoder/sanm_encoder.py` & `funasr-0.5.4/funasr/export/models/encoder/sanm_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/export/models/modules/decoder_layer.py` & `funasr-0.5.4/funasr/export/models/modules/decoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/export/models/modules/encoder_layer.py` & `funasr-0.5.4/funasr/export/models/modules/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/export/models/modules/feedforward.py` & `funasr-0.5.4/funasr/export/models/modules/feedforward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/export/models/modules/multihead_att.py` & `funasr-0.5.4/funasr/export/models/modules/multihead_att.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/export/models/predictor/cif.py` & `funasr-0.5.4/funasr/export/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/export/test/test_onnx.py` & `funasr-0.5.4/funasr/export/test/test_onnx.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/export/test/test_onnx_punc.py` & `funasr-0.5.4/funasr/export/test/test_onnx_punc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/export/test/test_onnx_punc_vadrealtime.py` & `funasr-0.5.4/funasr/export/test/test_onnx_punc_vadrealtime.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     input_name = [nd.name for nd in sess.get_inputs()]
     output_name = [nd.name for nd in sess.get_outputs()]
 
     def _get_feed_dict(text_length):
         return {'inputs': np.ones((1, text_length), dtype=np.int64),
                 'text_lengths': np.array([text_length,], dtype=np.int32),
                 'vad_masks': np.ones((1, 1, text_length, text_length), dtype=np.float32),
-                'sub_masks': np.tril(np.ones((text_length, text_length), dtype=np.float32))[None, None, :, :].astype(np.float32)
+                'sub_masks': np.ones((1, 1, text_length, text_length), dtype=np.float32),
                 }
 
     def _run(feed_dict):
         output = sess.run(output_name, input_feed=feed_dict)
         for name, value in zip(output_name, output):
             print('{}: {}'.format(name, value))
     _run(_get_feed_dict(10))
```

### Comparing `funasr-0.5.3/funasr/export/test/test_onnx_vad.py` & `funasr-0.5.4/funasr/export/test/test_onnx_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/export/utils/torch_function.py` & `funasr-0.5.4/funasr/export/utils/torch_function.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/fileio/datadir_writer.py` & `funasr-0.5.4/funasr/fileio/datadir_writer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/fileio/npy_scp.py` & `funasr-0.5.4/funasr/fileio/npy_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/fileio/rand_gen_dataset.py` & `funasr-0.5.4/funasr/fileio/rand_gen_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/fileio/read_text.py` & `funasr-0.5.4/funasr/fileio/read_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/fileio/sound_scp.py` & `funasr-0.5.4/funasr/fileio/sound_scp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import collections.abc
 from pathlib import Path
 from typing import Union
 
+import random
 import numpy as np
 import soundfile
 import librosa
 from typeguard import check_argument_types
 
+import torch
+import torchaudio
+
 from funasr.fileio.read_text import read_2column_text
 
 
 class SoundScpReader(collections.abc.Mapping):
     """Reader class for 'wav.scp'.
 
     Examples:
@@ -28,37 +32,48 @@
     def __init__(
         self,
         fname,
         dtype=np.int16,
         always_2d: bool = False,
         normalize: bool = False,
         dest_sample_rate: int = 16000,
+        speed_perturb: Union[list, tuple] = None,
     ):
         assert check_argument_types()
         self.fname = fname
         self.dtype = dtype
         self.always_2d = always_2d
         self.normalize = normalize
         self.data = read_2column_text(fname)
         self.dest_sample_rate = dest_sample_rate
+        self.speed_perturb = speed_perturb
 
     def __getitem__(self, key):
         wav = self.data[key]
         if self.normalize:
             # soundfile.read normalizes data to [-1,1] if dtype is not given
             array, rate = librosa.load(
                 wav, sr=self.dest_sample_rate, mono=self.always_2d
             )
         else:
             array, rate = librosa.load(
                 wav, sr=self.dest_sample_rate, mono=self.always_2d, dtype=self.dtype
             )
 
+        if self.speed_perturb is not None:
+            speed = random.choice(self.speed_perturb)
+            if speed != 1.0:
+                array, _ = torchaudio.sox_effects.apply_effects_tensor(
+                    torch.tensor(array).view(1, -1), rate,
+                    [['speed', str(speed)], ['rate', str(rate)]])
+                array = array.view(-1).numpy()
+
         if array.ndim==2:
             array=array.transpose((1, 0))
+
         return rate, array
 
     def get_path(self, key):
         return self.data[key]
 
     def __contains__(self, item):
         return item
```

### Comparing `funasr-0.5.3/funasr/iterators/chunk_iter_factory.py` & `funasr-0.5.4/funasr/iterators/chunk_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/iterators/multiple_iter_factory.py` & `funasr-0.5.4/funasr/iterators/multiple_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/iterators/sequence_iter_factory.py` & `funasr-0.5.4/funasr/iterators/sequence_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/layers/complex_utils.py` & `funasr-0.5.4/funasr/layers/complex_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/layers/global_mvn.py` & `funasr-0.5.4/funasr/layers/global_mvn.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 from funasr.modules.nets_utils import make_pad_mask
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.layers.inversible_interface import InversibleInterface
 
 
 class GlobalMVN(AbsNormalize, InversibleInterface):
     """Apply global mean and variance normalization
-
     TODO(kamo): Make this class portable somehow
-
     Args:
         stats_file: npy file
         norm_means: Apply mean normalization
         norm_vars: Apply var normalization
         eps:
     """
 
@@ -62,15 +60,14 @@
             f"norm_means={self.norm_means}, norm_vars={self.norm_vars}"
         )
 
     def forward(
         self, x: torch.Tensor, ilens: torch.Tensor = None
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Forward function
-
         Args:
             x: (B, L, ...)
             ilens: (B,)
         """
         if ilens is None:
             ilens = x.new_full([x.size(0)], x.size(1))
         norm_means = self.norm_means
@@ -114,8 +111,8 @@
         if norm_vars:
             x *= self.std
 
         # feat: (B, T, D)
         if norm_means:
             x += self.mean
             x.masked_fill_(make_pad_mask(ilens, x, 1), 0.0)
-        return x, ilens
+        return x, ilens
```

### Comparing `funasr-0.5.3/funasr/layers/label_aggregation.py` & `funasr-0.5.4/funasr/layers/label_aggregation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/layers/log_mel.py` & `funasr-0.5.4/funasr/layers/log_mel.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/layers/mask_along_axis.py` & `funasr-0.5.4/funasr/layers/mask_along_axis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/layers/sinc_conv.py` & `funasr-0.5.4/funasr/layers/sinc_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/layers/stft.py` & `funasr-0.5.4/funasr/layers/stft.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/layers/time_warp.py` & `funasr-0.5.4/funasr/layers/time_warp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/layers/utterance_mvn.py` & `funasr-0.5.4/funasr/layers/utterance_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/lm/seq_rnn_lm.py` & `funasr-0.5.4/funasr/models/seq_rnn_lm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Sequential implementation of Recurrent Neural Network Language Model."""
 from typing import Tuple
 from typing import Union
 
 import torch
 import torch.nn as nn
 from typeguard import check_argument_types
-
-from funasr.lm.abs_model import AbsLM
+from funasr.train.abs_model import AbsLM
 
 
 class SequentialRNNLM(AbsLM):
     """Sequential RNNLM.
 
     See also:
         https://github.com/pytorch/examples/blob/4581968193699de14b56527296262dd76ab43557/word_language_model/model.py
```

### Comparing `funasr-0.5.3/funasr/lm/transformer_lm.py` & `funasr-0.5.4/funasr/models/transformer_lm.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import torch
 import torch.nn as nn
 
 from funasr.modules.embedding import PositionalEncoding
 from funasr.models.encoder.transformer_encoder import TransformerEncoder_s0 as Encoder
 from funasr.modules.mask import subsequent_mask
-from funasr.lm.abs_model import AbsLM
+from funasr.train.abs_model import AbsLM
 
 
 class TransformerLM(AbsLM):
     def __init__(
         self,
         vocab_size: int,
         pos_enc: str = None,
```

### Comparing `funasr-0.5.3/funasr/losses/label_smoothing_loss.py` & `funasr-0.5.4/funasr/losses/label_smoothing_loss.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/main_funcs/average_nbest_models.py` & `funasr-0.5.4/funasr/main_funcs/average_nbest_models.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/main_funcs/calculate_all_attentions.py` & `funasr-0.5.4/funasr/main_funcs/calculate_all_attentions.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 from funasr.modules.rnn.attentions import AttMultiHeadDot
 from funasr.modules.rnn.attentions import AttMultiHeadLoc
 from funasr.modules.rnn.attentions import AttMultiHeadMultiResLoc
 from funasr.modules.rnn.attentions import NoAtt
 from funasr.modules.attention import MultiHeadedAttention
 
 
-from funasr.train.abs_espnet_model import AbsESPnetModel
+from funasr.models.base_model import FunASRModel
 
 
 @torch.no_grad()
 def calculate_all_attentions(
-    model: AbsESPnetModel, batch: Dict[str, torch.Tensor]
+    model: FunASRModel, batch: Dict[str, torch.Tensor]
 ) -> Dict[str, List[torch.Tensor]]:
     """Derive the outputs from the all attention layers
 
     Args:
         model:
         batch: same as forward
     Returns:
```

### Comparing `funasr-0.5.3/funasr/main_funcs/collect_stats.py` & `funasr-0.5.4/funasr/main_funcs/collect_stats.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 from torch.utils.data import DataLoader
 from typeguard import check_argument_types
 
 from funasr.fileio.datadir_writer import DatadirWriter
 from funasr.fileio.npy_scp import NpyScpWriter
 from funasr.torch_utils.device_funcs import to_device
 from funasr.torch_utils.forward_adaptor import ForwardAdaptor
-from funasr.train.abs_espnet_model import AbsESPnetModel
+from funasr.models.base_model import FunASRModel
 
 
 @torch.no_grad()
 def collect_stats(
-    model: AbsESPnetModel,
+    model: FunASRModel,
     train_iter: DataLoader and Iterable[Tuple[List[str], Dict[str, torch.Tensor]]],
     valid_iter: DataLoader and Iterable[Tuple[List[str], Dict[str, torch.Tensor]]],
     output_dir: Path,
     ngpu: Optional[int],
     log_interval: Optional[int],
     write_collected_feats: bool,
 ) -> None:
```

### Comparing `funasr-0.5.3/funasr/main_funcs/pack_funcs.py` & `funasr-0.5.4/funasr/main_funcs/pack_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/models/ctc.py` & `funasr-0.5.4/funasr/models/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/models/data2vec.py` & `funasr-0.5.4/funasr/models/data2vec.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.models.encoder.abs_encoder import AbsEncoder
 from funasr.models.frontend.abs_frontend import AbsFrontend
 from funasr.models.preencoder.abs_preencoder import AbsPreEncoder
 from funasr.models.specaug.abs_specaug import AbsSpecAug
 from funasr.torch_utils.device_funcs import force_gatherable
-from funasr.train.abs_espnet_model import AbsESPnetModel
+from funasr.models.base_model import FunASRModel
 
 if LooseVersion(torch.__version__) >= LooseVersion("1.6.0"):
     from torch.cuda.amp import autocast
 else:
     # Nothing to do if torch<1.6.0
     @contextmanager
     def autocast(enabled=True):
         yield
 
 
-class Data2VecPretrainModel(AbsESPnetModel):
+class Data2VecPretrainModel(FunASRModel):
     """Data2Vec Pretrain model"""
 
     def __init__(
             self,
             frontend: Optional[AbsFrontend],
             specaug: Optional[AbsSpecAug],
             normalize: Optional[AbsNormalize],
@@ -53,15 +53,14 @@
 
     def forward(
             self,
             speech: torch.Tensor,
             speech_lengths: torch.Tensor,
     ) -> Tuple[torch.Tensor, Dict[str, torch.Tensor], torch.Tensor]:
         """Frontend + Encoder + Calc loss
-
         Args:
             speech: (Batch, Length, ...)
             speech_lengths: (Batch, )
         """
         # Check that batch_size is unified
         assert (
                 speech.shape[0]
@@ -102,15 +101,14 @@
 
     def encode(
             self,
             speech: torch.Tensor,
             speech_lengths: torch.Tensor,
     ):
         """Frontend + Encoder.
-
         Args:
             speech: (Batch, Length, ...)
             speech_lengths: (Batch, )
         """
         with autocast(False):
             # 1. Extract feats
             feats, feats_lengths = self._extract_feats(speech, speech_lengths)
```

### Comparing `funasr-0.5.3/funasr/models/decoder/contextual_decoder.py` & `funasr-0.5.4/funasr/models/decoder/contextual_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/models/decoder/rnn_decoder.py` & `funasr-0.5.4/funasr/models/decoder/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/models/decoder/rnnt_decoder.py` & `funasr-0.5.4/funasr/models/decoder/rnnt_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/models/decoder/sanm_decoder.py` & `funasr-0.5.4/funasr/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/models/decoder/sv_decoder.py` & `funasr-0.5.4/funasr/models/decoder/sv_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/models/decoder/transformer_decoder.py` & `funasr-0.5.4/funasr/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/models/e2e_asr.py` & `funasr-0.5.4/funasr/models/e2e_asr.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,50 +24,50 @@
 from funasr.models.postencoder.abs_postencoder import AbsPostEncoder
 from funasr.models.preencoder.abs_preencoder import AbsPreEncoder
 from funasr.models.specaug.abs_specaug import AbsSpecAug
 from funasr.modules.add_sos_eos import add_sos_eos
 from funasr.modules.e2e_asr_common import ErrorCalculator
 from funasr.modules.nets_utils import th_accuracy
 from funasr.torch_utils.device_funcs import force_gatherable
-from funasr.train.abs_espnet_model import AbsESPnetModel
+from funasr.models.base_model import FunASRModel
 
 if LooseVersion(torch.__version__) >= LooseVersion("1.6.0"):
     from torch.cuda.amp import autocast
 else:
     # Nothing to do if torch<1.6.0
     @contextmanager
     def autocast(enabled=True):
         yield
 
 
-class ESPnetASRModel(AbsESPnetModel):
+class ASRModel(FunASRModel):
     """CTC-attention hybrid Encoder-Decoder model"""
 
     def __init__(
             self,
             vocab_size: int,
             token_list: Union[Tuple[str, ...], List[str]],
             frontend: Optional[AbsFrontend],
             specaug: Optional[AbsSpecAug],
             normalize: Optional[AbsNormalize],
-            preencoder: Optional[AbsPreEncoder],
             encoder: AbsEncoder,
-            postencoder: Optional[AbsPostEncoder],
             decoder: AbsDecoder,
             ctc: CTC,
             ctc_weight: float = 0.5,
             interctc_weight: float = 0.0,
             ignore_id: int = -1,
             lsm_weight: float = 0.0,
             length_normalized_loss: bool = False,
             report_cer: bool = True,
             report_wer: bool = True,
             sym_space: str = "<space>",
             sym_blank: str = "<blank>",
             extract_feats_in_collect_stats: bool = True,
+            preencoder: Optional[AbsPreEncoder] = None,
+            postencoder: Optional[AbsPostEncoder] = None,
     ):
         assert check_argument_types()
         assert 0.0 <= ctc_weight <= 1.0, ctc_weight
         assert 0.0 <= interctc_weight < 1.0, interctc_weight
 
         super().__init__()
         # note that eos is the same as sos (equivalent ID)
@@ -129,15 +129,14 @@
             self,
             speech: torch.Tensor,
             speech_lengths: torch.Tensor,
             text: torch.Tensor,
             text_lengths: torch.Tensor,
     ) -> Tuple[torch.Tensor, Dict[str, torch.Tensor], torch.Tensor]:
         """Frontend + Encoder + Decoder + Calc loss
-
         Args:
             speech: (Batch, Length, ...)
             speech_lengths: (Batch, )
             text: (Batch, Length)
             text_lengths: (Batch,)
         """
         assert text_lengths.dim() == 1, text_lengths.shape
@@ -245,15 +244,14 @@
             feats, feats_lengths = speech, speech_lengths
         return {"feats": feats, "feats_lengths": feats_lengths}
 
     def encode(
             self, speech: torch.Tensor, speech_lengths: torch.Tensor
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Frontend + Encoder. Note that this method is used by asr_inference.py
-
         Args:
             speech: (Batch, Length, ...)
             speech_lengths: (Batch, )
         """
         with autocast(False):
             # 1. Extract feats
             feats, feats_lengths = self._extract_feats(speech, speech_lengths)
@@ -327,17 +325,15 @@
             self,
             encoder_out: torch.Tensor,
             encoder_out_lens: torch.Tensor,
             ys_pad: torch.Tensor,
             ys_pad_lens: torch.Tensor,
     ) -> torch.Tensor:
         """Compute negative log likelihood(nll) from transformer-decoder
-
         Normally, this function is called in batchify_nll.
-
         Args:
             encoder_out: (Batch, Length, Dim)
             encoder_out_lens: (Batch,)
             ys_pad: (Batch, Length)
             ys_pad_lens: (Batch,)
         """
         ys_in_pad, ys_out_pad = add_sos_eos(ys_pad, self.sos, self.eos, self.ignore_id)
@@ -366,15 +362,14 @@
             encoder_out: torch.Tensor,
             encoder_out_lens: torch.Tensor,
             ys_pad: torch.Tensor,
             ys_pad_lens: torch.Tensor,
             batch_size: int = 100,
     ):
         """Compute negative log likelihood(nll) from transformer-decoder
-
         To avoid OOM, this fuction seperate the input into batches.
         Then call nll for each batch and combine and return results.
         Args:
             encoder_out: (Batch, Length, Dim)
             encoder_out_lens: (Batch,)
             ys_pad: (Batch, Length)
             ys_pad_lens: (Batch,)
```

### Comparing `funasr-0.5.3/funasr/models/e2e_asr_common.py` & `funasr-0.5.4/funasr/models/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/models/e2e_asr_contextual_paraformer.py` & `funasr-0.5.4/funasr/models/e2e_asr_contextual_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/models/e2e_asr_mfcca.py` & `funasr-0.5.4/funasr/models/e2e_asr_mfcca.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,71 +19,71 @@
 from funasr.models.decoder.abs_decoder import AbsDecoder
 from funasr.models.encoder.abs_encoder import AbsEncoder
 from funasr.models.frontend.abs_frontend import AbsFrontend
 from funasr.models.preencoder.abs_preencoder import AbsPreEncoder
 from funasr.models.specaug.abs_specaug import AbsSpecAug
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.torch_utils.device_funcs import force_gatherable
-from funasr.train.abs_espnet_model import AbsESPnetModel
+from funasr.models.base_model import FunASRModel
 
 if LooseVersion(torch.__version__) >= LooseVersion("1.6.0"):
     from torch.cuda.amp import autocast
 else:
     # Nothing to do if torch<1.6.0
     @contextmanager
     def autocast(enabled=True):
         yield
 import pdb
 import random
 import math
-class MFCCA(AbsESPnetModel):
+
+class MFCCA(FunASRModel):
     """
     Author: Audio, Speech and Language Processing Group (ASLP@NPU), Northwestern Polytechnical University
     MFCCA:Multi-Frame Cross-Channel attention for multi-speaker ASR in Multi-party meeting scenario
     https://arxiv.org/abs/2210.05265
     """
 
     def __init__(
-        self,
-        vocab_size: int,
-        token_list: Union[Tuple[str, ...], List[str]],
-        frontend: Optional[AbsFrontend],
-        specaug: Optional[AbsSpecAug],
-        normalize: Optional[AbsNormalize],
-        preencoder: Optional[AbsPreEncoder],
-        encoder: AbsEncoder,
-        decoder: AbsDecoder,
-        ctc: CTC,
-        rnnt_decoder: None,
-        ctc_weight: float = 0.5,
-        ignore_id: int = -1,
-        lsm_weight: float = 0.0,
-        mask_ratio: float = 0.0,
-        length_normalized_loss: bool = False,
-        report_cer: bool = True,
-        report_wer: bool = True,
-        sym_space: str = "<space>",
-        sym_blank: str = "<blank>",
+            self,
+            vocab_size: int,
+            token_list: Union[Tuple[str, ...], List[str]],
+            frontend: Optional[AbsFrontend],
+            specaug: Optional[AbsSpecAug],
+            normalize: Optional[AbsNormalize],
+            encoder: AbsEncoder,
+            decoder: AbsDecoder,
+            ctc: CTC,
+            rnnt_decoder: None,
+            ctc_weight: float = 0.5,
+            ignore_id: int = -1,
+            lsm_weight: float = 0.0,
+            mask_ratio: float = 0.0,
+            length_normalized_loss: bool = False,
+            report_cer: bool = True,
+            report_wer: bool = True,
+            sym_space: str = "<space>",
+            sym_blank: str = "<blank>",
+            preencoder: Optional[AbsPreEncoder] = None,
     ):
         assert check_argument_types()
         assert 0.0 <= ctc_weight <= 1.0, ctc_weight
         assert rnnt_decoder is None, "Not implemented"
 
         super().__init__()
         # note that eos is the same as sos (equivalent ID)
         self.sos = vocab_size - 1
         self.eos = vocab_size - 1
         self.vocab_size = vocab_size
         self.ignore_id = ignore_id
         self.ctc_weight = ctc_weight
         self.token_list = token_list.copy()
-        
+
         self.mask_ratio = mask_ratio
 
-        
         self.frontend = frontend
         self.specaug = specaug
         self.normalize = normalize
         self.preencoder = preencoder
         self.encoder = encoder
         # we set self.decoder = None in the CTC mode since
         # self.decoder parameters were never used and PyTorch complained
@@ -109,47 +109,46 @@
             self.error_calculator = ErrorCalculator(
                 token_list, sym_space, sym_blank, report_cer, report_wer
             )
         else:
             self.error_calculator = None
 
     def forward(
-        self,
-        speech: torch.Tensor,
-        speech_lengths: torch.Tensor,
-        text: torch.Tensor,
-        text_lengths: torch.Tensor,
+            self,
+            speech: torch.Tensor,
+            speech_lengths: torch.Tensor,
+            text: torch.Tensor,
+            text_lengths: torch.Tensor,
     ) -> Tuple[torch.Tensor, Dict[str, torch.Tensor], torch.Tensor]:
         """Frontend + Encoder + Decoder + Calc loss
-
         Args:
             speech: (Batch, Length, ...)
             speech_lengths: (Batch, )
             text: (Batch, Length)
             text_lengths: (Batch,)
         """
         assert text_lengths.dim() == 1, text_lengths.shape
         # Check that batch_size is unified
         assert (
-            speech.shape[0]
-            == speech_lengths.shape[0]
-            == text.shape[0]
-            == text_lengths.shape[0]
+                speech.shape[0]
+                == speech_lengths.shape[0]
+                == text.shape[0]
+                == text_lengths.shape[0]
         ), (speech.shape, speech_lengths.shape, text.shape, text_lengths.shape)
-        #pdb.set_trace()
-        if(speech.dim()==3 and speech.size(2)==8 and self.mask_ratio !=0):
+        # pdb.set_trace()
+        if (speech.dim() == 3 and speech.size(2) == 8 and self.mask_ratio != 0):
             rate_num = random.random()
-            #rate_num = 0.1
-            if(rate_num<=self.mask_ratio):
-                retain_channel = math.ceil(random.random() *8)
-                if(retain_channel>1):
-                    speech = speech[:,:,torch.randperm(8)[0:retain_channel].sort().values]
+            # rate_num = 0.1
+            if (rate_num <= self.mask_ratio):
+                retain_channel = math.ceil(random.random() * 8)
+                if (retain_channel > 1):
+                    speech = speech[:, :, torch.randperm(8)[0:retain_channel].sort().values]
                 else:
-                    speech = speech[:,:,torch.randperm(8)[0]]
-        #pdb.set_trace()
+                    speech = speech[:, :, torch.randperm(8)[0]]
+        # pdb.set_trace()
         batch_size = speech.shape[0]
         # for data-parallel
         text = text[:, : text_lengths.max()]
 
         # 1. Encoder
         encoder_out, encoder_out_lens = self.encode(speech, speech_lengths)
 
@@ -191,28 +190,27 @@
         )
 
         # force_gatherable: to-device and to-tensor if scalar for DataParallel
         loss, stats, weight = force_gatherable((loss, stats, batch_size), loss.device)
         return loss, stats, weight
 
     def collect_feats(
-        self,
-        speech: torch.Tensor,
-        speech_lengths: torch.Tensor,
-        text: torch.Tensor,
-        text_lengths: torch.Tensor,
+            self,
+            speech: torch.Tensor,
+            speech_lengths: torch.Tensor,
+            text: torch.Tensor,
+            text_lengths: torch.Tensor,
     ) -> Dict[str, torch.Tensor]:
         feats, feats_lengths, channel_size = self._extract_feats(speech, speech_lengths)
         return {"feats": feats, "feats_lengths": feats_lengths}
 
     def encode(
-        self, speech: torch.Tensor, speech_lengths: torch.Tensor
+            self, speech: torch.Tensor, speech_lengths: torch.Tensor
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Frontend + Encoder. Note that this method is used by asr_inference.py
-
         Args:
             speech: (Batch, Length, ...)
             speech_lengths: (Batch, )
         """
         with autocast(False):
             # 1. Extract feats
             feats, feats_lengths, channel_size = self._extract_feats(speech, speech_lengths)
@@ -223,36 +221,36 @@
             # 3. Normalization for feature: e.g. Global-CMVN, Utterance-CMVN
             if self.normalize is not None:
                 feats, feats_lengths = self.normalize(feats, feats_lengths)
 
         # Pre-encoder, e.g. used for raw input data
         if self.preencoder is not None:
             feats, feats_lengths = self.preencoder(feats, feats_lengths)
-        #pdb.set_trace()
+        # pdb.set_trace()
         encoder_out, encoder_out_lens, _ = self.encoder(feats, feats_lengths, channel_size)
 
         assert encoder_out.size(0) == speech.size(0), (
             encoder_out.size(),
             speech.size(0),
         )
-        if(encoder_out.dim()==4):
+        if (encoder_out.dim() == 4):
             assert encoder_out.size(2) <= encoder_out_lens.max(), (
                 encoder_out.size(),
                 encoder_out_lens.max(),
             )
         else:
             assert encoder_out.size(1) <= encoder_out_lens.max(), (
                 encoder_out.size(),
                 encoder_out_lens.max(),
             )
 
         return encoder_out, encoder_out_lens
 
     def _extract_feats(
-        self, speech: torch.Tensor, speech_lengths: torch.Tensor
+            self, speech: torch.Tensor, speech_lengths: torch.Tensor
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         assert speech_lengths.dim() == 1, speech_lengths.shape
         # for data-parallel
         speech = speech[:, : speech_lengths.max()]
         if self.frontend is not None:
             # Frontend
             #  e.g. STFT and Feature extract
@@ -262,19 +260,19 @@
         else:
             # No frontend and no feature extract
             feats, feats_lengths = speech, speech_lengths
             channel_size = 1
         return feats, feats_lengths, channel_size
 
     def _calc_att_loss(
-        self,
-        encoder_out: torch.Tensor,
-        encoder_out_lens: torch.Tensor,
-        ys_pad: torch.Tensor,
-        ys_pad_lens: torch.Tensor,
+            self,
+            encoder_out: torch.Tensor,
+            encoder_out_lens: torch.Tensor,
+            ys_pad: torch.Tensor,
+            ys_pad_lens: torch.Tensor,
     ):
         ys_in_pad, ys_out_pad = add_sos_eos(ys_pad, self.sos, self.eos, self.ignore_id)
         ys_in_lens = ys_pad_lens + 1
 
         # 1. Forward decoder
         decoder_out, _ = self.decoder(
             encoder_out, encoder_out_lens, ys_in_pad, ys_in_lens
@@ -294,33 +292,33 @@
         else:
             ys_hat = decoder_out.argmax(dim=-1)
             cer_att, wer_att = self.error_calculator(ys_hat.cpu(), ys_pad.cpu())
 
         return loss_att, acc_att, cer_att, wer_att
 
     def _calc_ctc_loss(
-        self,
-        encoder_out: torch.Tensor,
-        encoder_out_lens: torch.Tensor,
-        ys_pad: torch.Tensor,
-        ys_pad_lens: torch.Tensor,
+            self,
+            encoder_out: torch.Tensor,
+            encoder_out_lens: torch.Tensor,
+            ys_pad: torch.Tensor,
+            ys_pad_lens: torch.Tensor,
     ):
         # Calc CTC loss
-        if(encoder_out.dim()==4):
+        if (encoder_out.dim() == 4):
             encoder_out = encoder_out.mean(1)
         loss_ctc = self.ctc(encoder_out, encoder_out_lens, ys_pad, ys_pad_lens)
 
         # Calc CER using CTC
         cer_ctc = None
         if not self.training and self.error_calculator is not None:
             ys_hat = self.ctc.argmax(encoder_out).data
             cer_ctc = self.error_calculator(ys_hat.cpu(), ys_pad.cpu(), is_ctc=True)
         return loss_ctc, cer_ctc
 
     def _calc_rnnt_loss(
-        self,
-        encoder_out: torch.Tensor,
-        encoder_out_lens: torch.Tensor,
-        ys_pad: torch.Tensor,
-        ys_pad_lens: torch.Tensor,
+            self,
+            encoder_out: torch.Tensor,
+            encoder_out_lens: torch.Tensor,
+            ys_pad: torch.Tensor,
+            ys_pad_lens: torch.Tensor,
     ):
-        raise NotImplementedError
+        raise NotImplementedError
```

### Comparing `funasr-0.5.3/funasr/models/e2e_asr_paraformer.py` & `funasr-0.5.4/funasr/models/e2e_asr_paraformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,44 +25,41 @@
 from funasr.models.predictor.cif import mae_loss
 from funasr.models.preencoder.abs_preencoder import AbsPreEncoder
 from funasr.models.specaug.abs_specaug import AbsSpecAug
 from funasr.modules.add_sos_eos import add_sos_eos
 from funasr.modules.nets_utils import make_pad_mask, pad_list
 from funasr.modules.nets_utils import th_accuracy
 from funasr.torch_utils.device_funcs import force_gatherable
-from funasr.train.abs_espnet_model import AbsESPnetModel
+from funasr.models.base_model import FunASRModel
 from funasr.models.predictor.cif import CifPredictorV3
 
-
 if LooseVersion(torch.__version__) >= LooseVersion("1.6.0"):
     from torch.cuda.amp import autocast
 else:
     # Nothing to do if torch<1.6.0
     @contextmanager
     def autocast(enabled=True):
         yield
 
 
-class Paraformer(AbsESPnetModel):
+class Paraformer(FunASRModel):
     """
     Author: Speech Lab of DAMO Academy, Alibaba Group
     Paraformer: Fast and Accurate Parallel Transformer for Non-autoregressive End-to-End Speech Recognition
     https://arxiv.org/abs/2206.08317
     """
 
     def __init__(
             self,
             vocab_size: int,
             token_list: Union[Tuple[str, ...], List[str]],
             frontend: Optional[AbsFrontend],
             specaug: Optional[AbsSpecAug],
             normalize: Optional[AbsNormalize],
-            preencoder: Optional[AbsPreEncoder],
             encoder: AbsEncoder,
-            postencoder: Optional[AbsPostEncoder],
             decoder: AbsDecoder,
             ctc: CTC,
             ctc_weight: float = 0.5,
             interctc_weight: float = 0.0,
             ignore_id: int = -1,
             blank_id: int = 0,
             sos: int = 1,
@@ -75,14 +72,17 @@
             sym_blank: str = "<blank>",
             extract_feats_in_collect_stats: bool = True,
             predictor=None,
             predictor_weight: float = 0.0,
             predictor_bias: int = 0,
             sampling_ratio: float = 0.2,
             share_embedding: bool = False,
+            preencoder: Optional[AbsPreEncoder] = None,
+            postencoder: Optional[AbsPostEncoder] = None,
+            use_1st_decoder_loss: bool = False,
     ):
         assert check_argument_types()
         assert 0.0 <= ctc_weight <= 1.0, ctc_weight
         assert 0.0 <= interctc_weight < 1.0, interctc_weight
 
         super().__init__()
         # note that eos is the same as sos (equivalent ID)
@@ -141,23 +141,24 @@
         self.criterion_pre = mae_loss(normalize_length=length_normalized_loss)
         self.step_cur = 0
 
         self.share_embedding = share_embedding
         if self.share_embedding:
             self.decoder.embed = None
 
+        self.use_1st_decoder_loss = use_1st_decoder_loss
+
     def forward(
             self,
             speech: torch.Tensor,
             speech_lengths: torch.Tensor,
             text: torch.Tensor,
             text_lengths: torch.Tensor,
     ) -> Tuple[torch.Tensor, Dict[str, torch.Tensor], torch.Tensor]:
         """Frontend + Encoder + Decoder + Calc loss
-
         Args:
                 speech: (Batch, Length, ...)
                 speech_lengths: (Batch, )
                 text: (Batch, Length)
                 text_lengths: (Batch,)
         """
         assert text_lengths.dim() == 1, text_lengths.shape
@@ -177,15 +178,15 @@
         # 1. Encoder
         encoder_out, encoder_out_lens = self.encode(speech, speech_lengths)
         intermediate_outs = None
         if isinstance(encoder_out, tuple):
             intermediate_outs = encoder_out[1]
             encoder_out = encoder_out[0]
 
-        loss_att, acc_att, cer_att, wer_att = None, None, None, None
+        loss_att, pre_loss_att, acc_att, cer_att, wer_att = None, None, None, None, None
         loss_ctc, cer_ctc = None, None
         loss_pre = None
         stats = dict()
 
         # 1. CTC branch
         if self.ctc_weight != 0.0:
             loss_ctc, cer_ctc = self._calc_ctc_loss(
@@ -218,28 +219,32 @@
             # calculate whole encoder loss
             loss_ctc = (
                                1 - self.interctc_weight
                        ) * loss_ctc + self.interctc_weight * loss_interctc
 
         # 2b. Attention decoder branch
         if self.ctc_weight != 1.0:
-            loss_att, acc_att, cer_att, wer_att, loss_pre = self._calc_att_loss(
+            loss_att, acc_att, cer_att, wer_att, loss_pre, pre_loss_att = self._calc_att_loss(
                 encoder_out, encoder_out_lens, text, text_lengths
             )
 
         # 3. CTC-Att loss definition
         if self.ctc_weight == 0.0:
             loss = loss_att + loss_pre * self.predictor_weight
         elif self.ctc_weight == 1.0:
             loss = loss_ctc
         else:
             loss = self.ctc_weight * loss_ctc + (1 - self.ctc_weight) * loss_att + loss_pre * self.predictor_weight
 
+        if self.use_1st_decoder_loss and pre_loss_att is not None:
+            loss = loss + pre_loss_att
+
         # Collect Attn branch stats
         stats["loss_att"] = loss_att.detach() if loss_att is not None else None
+        stats["pre_loss_att"] = pre_loss_att.detach() if pre_loss_att is not None else None
         stats["acc"] = acc_att
         stats["cer"] = cer_att
         stats["wer"] = wer_att
         stats["loss_pre"] = loss_pre.detach().cpu() if loss_pre is not None else None
 
         stats["loss"] = torch.clone(loss.detach())
 
@@ -266,15 +271,14 @@
             feats, feats_lengths = speech, speech_lengths
         return {"feats": feats, "feats_lengths": feats_lengths}
 
     def encode(
             self, speech: torch.Tensor, speech_lengths: torch.Tensor
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Frontend + Encoder. Note that this method is used by asr_inference.py
-
         Args:
                 speech: (Batch, Length, ...)
                 speech_lengths: (Batch, )
         """
         with autocast(False):
             # 1. Extract feats
             feats, feats_lengths = self._extract_feats(speech, speech_lengths)
@@ -364,17 +368,15 @@
             self,
             encoder_out: torch.Tensor,
             encoder_out_lens: torch.Tensor,
             ys_pad: torch.Tensor,
             ys_pad_lens: torch.Tensor,
     ) -> torch.Tensor:
         """Compute negative log likelihood(nll) from transformer-decoder
-
         Normally, this function is called in batchify_nll.
-
         Args:
                 encoder_out: (Batch, Length, Dim)
                 encoder_out_lens: (Batch,)
                 ys_pad: (Batch, Length)
                 ys_pad_lens: (Batch,)
         """
         ys_in_pad, ys_out_pad = add_sos_eos(ys_pad, self.sos, self.eos, self.ignore_id)
@@ -403,15 +405,14 @@
             encoder_out: torch.Tensor,
             encoder_out_lens: torch.Tensor,
             ys_pad: torch.Tensor,
             ys_pad_lens: torch.Tensor,
             batch_size: int = 100,
     ):
         """Compute negative log likelihood(nll) from transformer-decoder
-
         To avoid OOM, this fuction seperate the input into batches.
         Then call nll for each batch and combine and return results.
         Args:
                 encoder_out: (Batch, Length, Dim)
                 encoder_out_lens: (Batch,)
                 ys_pad: (Batch, Length)
                 ys_pad_lens: (Batch,)
@@ -458,19 +459,24 @@
             _, ys_pad = add_sos_eos(ys_pad, self.sos, self.eos, self.ignore_id)
             ys_pad_lens = ys_pad_lens + self.predictor_bias
         pre_acoustic_embeds, pre_token_length, _, pre_peak_index = self.predictor(encoder_out, ys_pad, encoder_out_mask,
                                                                                   ignore_id=self.ignore_id)
 
         # 0. sampler
         decoder_out_1st = None
+        pre_loss_att = None
         if self.sampling_ratio > 0.0:
             if self.step_cur < 2:
                 logging.info("enable sampler in paraformer, sampling_ratio: {}".format(self.sampling_ratio))
-            sematic_embeds, decoder_out_1st = self.sampler(encoder_out, encoder_out_lens, ys_pad, ys_pad_lens,
-                                                           pre_acoustic_embeds)
+            if self.use_1st_decoder_loss:
+                sematic_embeds, decoder_out_1st, pre_loss_att = self.sampler_with_grad(encoder_out, encoder_out_lens, ys_pad, ys_pad_lens,
+                                                               pre_acoustic_embeds)
+            else:
+                sematic_embeds, decoder_out_1st = self.sampler(encoder_out, encoder_out_lens, ys_pad, ys_pad_lens,
+                                                               pre_acoustic_embeds)
         else:
             if self.step_cur < 2:
                 logging.info("disable sampler in paraformer, sampling_ratio: {}".format(self.sampling_ratio))
             sematic_embeds = pre_acoustic_embeds
 
         # 1. Forward decoder
         decoder_outs = self.decoder(
@@ -492,15 +498,15 @@
         # Compute cer/wer using attention-decoder
         if self.training or self.error_calculator is None:
             cer_att, wer_att = None, None
         else:
             ys_hat = decoder_out_1st.argmax(dim=-1)
             cer_att, wer_att = self.error_calculator(ys_hat.cpu(), ys_pad.cpu())
 
-        return loss_att, acc_att, cer_att, wer_att, loss_pre
+        return loss_att, acc_att, cer_att, wer_att, loss_pre, pre_loss_att
 
     def sampler(self, encoder_out, encoder_out_lens, ys_pad, ys_pad_lens, pre_acoustic_embeds):
 
         tgt_mask = (~make_pad_mask(ys_pad_lens, maxlen=ys_pad_lens.max())[:, :, None]).to(ys_pad.device)
         ys_pad_masked = ys_pad * tgt_mask[:, :, 0]
         if self.share_embedding:
             ys_pad_embed = self.decoder.output_layer.weight[ys_pad_masked]
@@ -525,14 +531,45 @@
             input_mask = input_mask.masked_fill(~nonpad_positions, False)
             input_mask_expand_dim = input_mask.unsqueeze(2).to(pre_acoustic_embeds.device)
 
         sematic_embeds = pre_acoustic_embeds.masked_fill(~input_mask_expand_dim, 0) + ys_pad_embed.masked_fill(
             input_mask_expand_dim, 0)
         return sematic_embeds * tgt_mask, decoder_out * tgt_mask
 
+    def sampler_with_grad(self, encoder_out, encoder_out_lens, ys_pad, ys_pad_lens, pre_acoustic_embeds):
+        tgt_mask = (~make_pad_mask(ys_pad_lens, maxlen=ys_pad_lens.max())[:, :, None]).to(ys_pad.device)
+        ys_pad_masked = ys_pad * tgt_mask[:, :, 0]
+        if self.share_embedding:
+            ys_pad_embed = self.decoder.output_layer.weight[ys_pad_masked]
+        else:
+            ys_pad_embed = self.decoder.embed(ys_pad_masked)
+        decoder_outs = self.decoder(
+            encoder_out, encoder_out_lens, pre_acoustic_embeds, ys_pad_lens
+        )
+        pre_loss_att = self.criterion_att(decoder_outs[0], ys_pad)
+        decoder_out, _ = decoder_outs[0], decoder_outs[1]
+        pred_tokens = decoder_out.argmax(-1)
+        nonpad_positions = ys_pad.ne(self.ignore_id)
+        seq_lens = (nonpad_positions).sum(1)
+        same_num = ((pred_tokens == ys_pad) & nonpad_positions).sum(1)
+        input_mask = torch.ones_like(nonpad_positions)
+        bsz, seq_len = ys_pad.size()
+        for li in range(bsz):
+            target_num = (((seq_lens[li] - same_num[li].sum()).float()) * self.sampling_ratio).long()
+            if target_num > 0:
+                input_mask[li].scatter_(dim=0, index=torch.randperm(seq_lens[li])[:target_num].cuda(), value=0)
+        input_mask = input_mask.eq(1)
+        input_mask = input_mask.masked_fill(~nonpad_positions, False)
+        input_mask_expand_dim = input_mask.unsqueeze(2).to(pre_acoustic_embeds.device)
+
+        sematic_embeds = pre_acoustic_embeds.masked_fill(~input_mask_expand_dim, 0) + ys_pad_embed.masked_fill(
+            input_mask_expand_dim, 0)
+
+        return sematic_embeds * tgt_mask, decoder_out * tgt_mask, pre_loss_att
+
     def _calc_ctc_loss(
             self,
             encoder_out: torch.Tensor,
             encoder_out_lens: torch.Tensor,
             ys_pad: torch.Tensor,
             ys_pad_lens: torch.Tensor,
     ):
@@ -660,15 +697,18 @@
         loss, stats, weight = force_gatherable((loss, stats, batch_size), loss.device)
         return loss, stats, weight
 
     def encode_chunk(
             self, speech: torch.Tensor, speech_lengths: torch.Tensor, cache: dict = None
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Frontend + Encoder. Note that this method is used by asr_inference.py
+<<<<<<< HEAD
+=======
 
+>>>>>>> 4cd79db451786548d8a100f25c3b03da0eb30f4b
         Args:
                 speech: (Batch, Length, ...)
                 speech_lengths: (Batch, )
         """
         with autocast(False):
             # 1. Extract feats
             feats, feats_lengths = self._extract_feats(speech, speech_lengths)
@@ -734,17 +774,15 @@
     def __init__(
             self,
             vocab_size: int,
             token_list: Union[Tuple[str, ...], List[str]],
             frontend: Optional[AbsFrontend],
             specaug: Optional[AbsSpecAug],
             normalize: Optional[AbsNormalize],
-            preencoder: Optional[AbsPreEncoder],
             encoder: AbsEncoder,
-            postencoder: Optional[AbsPostEncoder],
             decoder: AbsDecoder,
             ctc: CTC,
             ctc_weight: float = 0.5,
             interctc_weight: float = 0.0,
             ignore_id: int = -1,
             blank_id: int = 0,
             sos: int = 1,
@@ -759,14 +797,16 @@
             predictor=None,
             predictor_weight: float = 0.0,
             predictor_bias: int = 0,
             sampling_ratio: float = 0.2,
             embeds_id: int = 2,
             embeds_loss_weight: float = 0.0,
             embed_dims: int = 768,
+            preencoder: Optional[AbsPreEncoder] = None,
+            postencoder: Optional[AbsPostEncoder] = None,
     ):
         assert check_argument_types()
         assert 0.0 <= ctc_weight <= 1.0, ctc_weight
         assert 0.0 <= interctc_weight < 1.0, interctc_weight
 
         super().__init__(
             vocab_size=vocab_size,
@@ -890,15 +930,14 @@
             speech_lengths: torch.Tensor,
             text: torch.Tensor,
             text_lengths: torch.Tensor,
             embed: torch.Tensor = None,
             embed_lengths: torch.Tensor = None,
     ) -> Tuple[torch.Tensor, Dict[str, torch.Tensor], torch.Tensor]:
         """Frontend + Encoder + Decoder + Calc loss
-
         Args:
                 speech: (Batch, Length, ...)
                 speech_lengths: (Batch, )
                 text: (Batch, Length)
                 text_lengths: (Batch,)
         """
         assert text_lengths.dim() == 1, text_lengths.shape
@@ -909,17 +948,17 @@
                 == text.shape[0]
                 == text_lengths.shape[0]
         ), (speech.shape, speech_lengths.shape, text.shape, text_lengths.shape)
         batch_size = speech.shape[0]
         self.step_cur += 1
         # for data-parallel
         text = text[:, : text_lengths.max()]
-        speech = speech[:, :speech_lengths.max(), :]
+        speech = speech[:, :speech_lengths.max()]
         if embed is not None:
-            embed = embed[:, :embed_lengths.max(), :]
+            embed = embed[:, :embed_lengths.max()]
 
         # 1. Encoder
         encoder_out, encoder_out_lens = self.encode(speech, speech_lengths)
         intermediate_outs = None
         if isinstance(encoder_out, tuple):
             intermediate_outs = encoder_out[1]
             encoder_out = encoder_out[0]
@@ -999,82 +1038,81 @@
 
         # force_gatherable: to-device and to-tensor if scalar for DataParallel
         loss, stats, weight = force_gatherable((loss, stats, batch_size), loss.device)
         return loss, stats, weight
 
 
 class BiCifParaformer(Paraformer):
-
     """
     Paraformer model with an extra cif predictor
     to conduct accurate timestamp prediction
     """
 
     def __init__(
-        self,
-        vocab_size: int,
-        token_list: Union[Tuple[str, ...], List[str]],
-        frontend: Optional[AbsFrontend],
-        specaug: Optional[AbsSpecAug],
-        normalize: Optional[AbsNormalize],
-        preencoder: Optional[AbsPreEncoder],
-        encoder: AbsEncoder,
-        postencoder: Optional[AbsPostEncoder],
-        decoder: AbsDecoder,
-        ctc: CTC,
-        ctc_weight: float = 0.5,
-        interctc_weight: float = 0.0,
-        ignore_id: int = -1,
-        blank_id: int = 0,
-        sos: int = 1,
-        eos: int = 2,
-        lsm_weight: float = 0.0,
-        length_normalized_loss: bool = False,
-        report_cer: bool = True,
-        report_wer: bool = True,
-        sym_space: str = "<space>",
-        sym_blank: str = "<blank>",
-        extract_feats_in_collect_stats: bool = True,
-        predictor = None,
-        predictor_weight: float = 0.0,
-        predictor_bias: int = 0,
-        sampling_ratio: float = 0.2,
+            self,
+            vocab_size: int,
+            token_list: Union[Tuple[str, ...], List[str]],
+            frontend: Optional[AbsFrontend],
+            specaug: Optional[AbsSpecAug],
+            normalize: Optional[AbsNormalize],
+            encoder: AbsEncoder,
+            decoder: AbsDecoder,
+            ctc: CTC,
+            ctc_weight: float = 0.5,
+            interctc_weight: float = 0.0,
+            ignore_id: int = -1,
+            blank_id: int = 0,
+            sos: int = 1,
+            eos: int = 2,
+            lsm_weight: float = 0.0,
+            length_normalized_loss: bool = False,
+            report_cer: bool = True,
+            report_wer: bool = True,
+            sym_space: str = "<space>",
+            sym_blank: str = "<blank>",
+            extract_feats_in_collect_stats: bool = True,
+            predictor=None,
+            predictor_weight: float = 0.0,
+            predictor_bias: int = 0,
+            sampling_ratio: float = 0.2,
+            preencoder: Optional[AbsPreEncoder] = None,
+            postencoder: Optional[AbsPostEncoder] = None,
     ):
         assert check_argument_types()
         assert 0.0 <= ctc_weight <= 1.0, ctc_weight
         assert 0.0 <= interctc_weight < 1.0, interctc_weight
 
         super().__init__(
-        vocab_size=vocab_size,
-        token_list=token_list,
-        frontend=frontend,
-        specaug=specaug,
-        normalize=normalize,
-        preencoder=preencoder,
-        encoder=encoder,
-        postencoder=postencoder,
-        decoder=decoder,
-        ctc=ctc,
-        ctc_weight=ctc_weight,
-        interctc_weight=interctc_weight,
-        ignore_id=ignore_id,
-        blank_id=blank_id,
-        sos=sos,
-        eos=eos,
-        lsm_weight=lsm_weight,
-        length_normalized_loss=length_normalized_loss,
-        report_cer=report_cer,
-        report_wer=report_wer,
-        sym_space=sym_space,
-        sym_blank=sym_blank,
-        extract_feats_in_collect_stats=extract_feats_in_collect_stats,
-        predictor=predictor,
-        predictor_weight=predictor_weight,
-        predictor_bias=predictor_bias,
-        sampling_ratio=sampling_ratio,
+            vocab_size=vocab_size,
+            token_list=token_list,
+            frontend=frontend,
+            specaug=specaug,
+            normalize=normalize,
+            preencoder=preencoder,
+            encoder=encoder,
+            postencoder=postencoder,
+            decoder=decoder,
+            ctc=ctc,
+            ctc_weight=ctc_weight,
+            interctc_weight=interctc_weight,
+            ignore_id=ignore_id,
+            blank_id=blank_id,
+            sos=sos,
+            eos=eos,
+            lsm_weight=lsm_weight,
+            length_normalized_loss=length_normalized_loss,
+            report_cer=report_cer,
+            report_wer=report_wer,
+            sym_space=sym_space,
+            sym_blank=sym_blank,
+            extract_feats_in_collect_stats=extract_feats_in_collect_stats,
+            predictor=predictor,
+            predictor_weight=predictor_weight,
+            predictor_bias=predictor_bias,
+            sampling_ratio=sampling_ratio,
         )
         assert isinstance(self.predictor, CifPredictorV3), "BiCifParaformer should use CIFPredictorV3"
 
     def _calc_pre2_loss(
             self,
             encoder_out: torch.Tensor,
             encoder_out_lens: torch.Tensor,
@@ -1141,40 +1179,41 @@
         if self.training or self.error_calculator is None:
             cer_att, wer_att = None, None
         else:
             ys_hat = decoder_out_1st.argmax(dim=-1)
             cer_att, wer_att = self.error_calculator(ys_hat.cpu(), ys_pad.cpu())
 
         return loss_att, acc_att, cer_att, wer_att, loss_pre
-    
+
     def calc_predictor(self, encoder_out, encoder_out_lens):
 
         encoder_out_mask = (~make_pad_mask(encoder_out_lens, maxlen=encoder_out.size(1))[:, None, :]).to(
             encoder_out.device)
-        pre_acoustic_embeds, pre_token_length, alphas, pre_peak_index, pre_token_length2 = self.predictor(encoder_out, None, encoder_out_mask,
-                                                                                  ignore_id=self.ignore_id)
+        pre_acoustic_embeds, pre_token_length, alphas, pre_peak_index, pre_token_length2 = self.predictor(encoder_out,
+                                                                                                          None,
+                                                                                                          encoder_out_mask,
+                                                                                                          ignore_id=self.ignore_id)
         return pre_acoustic_embeds, pre_token_length, alphas, pre_peak_index
-    
+
     def calc_predictor_timestamp(self, encoder_out, encoder_out_lens, token_num):
         encoder_out_mask = (~make_pad_mask(encoder_out_lens, maxlen=encoder_out.size(1))[:, None, :]).to(
             encoder_out.device)
         ds_alphas, ds_cif_peak, us_alphas, us_peaks = self.predictor.get_upsample_timestamp(encoder_out,
-                                                                                               encoder_out_mask,
-                                                                                               token_num)
+                                                                                            encoder_out_mask,
+                                                                                            token_num)
         return ds_alphas, ds_cif_peak, us_alphas, us_peaks
 
     def forward(
             self,
             speech: torch.Tensor,
             speech_lengths: torch.Tensor,
             text: torch.Tensor,
             text_lengths: torch.Tensor,
     ) -> Tuple[torch.Tensor, Dict[str, torch.Tensor], torch.Tensor]:
         """Frontend + Encoder + Decoder + Calc loss
-
         Args:
                 speech: (Batch, Length, ...)
                 speech_lengths: (Batch, )
                 text: (Batch, Length)
                 text_lengths: (Batch,)
         """
         assert text_lengths.dim() == 1, text_lengths.shape
@@ -1249,15 +1288,16 @@
 
         # 3. CTC-Att loss definition
         if self.ctc_weight == 0.0:
             loss = loss_att + loss_pre * self.predictor_weight + loss_pre2 * self.predictor_weight * 0.5
         elif self.ctc_weight == 1.0:
             loss = loss_ctc
         else:
-            loss = self.ctc_weight * loss_ctc + (1 - self.ctc_weight) * loss_att + loss_pre * self.predictor_weight + loss_pre2 * self.predictor_weight * 0.5
+            loss = self.ctc_weight * loss_ctc + (
+                        1 - self.ctc_weight) * loss_att + loss_pre * self.predictor_weight + loss_pre2 * self.predictor_weight * 0.5
 
         # Collect Attn branch stats
         stats["loss_att"] = loss_att.detach() if loss_att is not None else None
         stats["acc"] = acc_att
         stats["cer"] = cer_att
         stats["wer"] = wer_att
         stats["loss_pre"] = loss_pre.detach().cpu() if loss_pre is not None else None
@@ -1278,17 +1318,15 @@
     def __init__(
             self,
             vocab_size: int,
             token_list: Union[Tuple[str, ...], List[str]],
             frontend: Optional[AbsFrontend],
             specaug: Optional[AbsSpecAug],
             normalize: Optional[AbsNormalize],
-            preencoder: Optional[AbsPreEncoder],
             encoder: AbsEncoder,
-            postencoder: Optional[AbsPostEncoder],
             decoder: AbsDecoder,
             ctc: CTC,
             ctc_weight: float = 0.5,
             interctc_weight: float = 0.0,
             ignore_id: int = -1,
             blank_id: int = 0,
             sos: int = 1,
@@ -1310,14 +1348,16 @@
             batch_rate: float = 0.5,
             double_rate: float = -1.0,
             target_buffer_length: int = -1,
             inner_dim: int = 256,
             bias_encoder_type: str = 'lstm',
             label_bracket: bool = False,
             use_decoder_embedding: bool = False,
+            preencoder: Optional[AbsPreEncoder] = None,
+            postencoder: Optional[AbsPostEncoder] = None,
     ):
         assert check_argument_types()
         assert 0.0 <= ctc_weight <= 1.0, ctc_weight
         assert 0.0 <= interctc_weight < 1.0, interctc_weight
 
         super().__init__(
             vocab_size=vocab_size,
@@ -1373,15 +1413,14 @@
             self,
             speech: torch.Tensor,
             speech_lengths: torch.Tensor,
             text: torch.Tensor,
             text_lengths: torch.Tensor,
     ) -> Tuple[torch.Tensor, Dict[str, torch.Tensor], torch.Tensor]:
         """Frontend + Encoder + Decoder + Calc loss
-
         Args:
                 speech: (Batch, Length, ...)
                 speech_lengths: (Batch, )
                 text: (Batch, Length)
                 text_lengths: (Batch,)
         """
         assert text_lengths.dim() == 1, text_lengths.shape
@@ -1757,8 +1796,8 @@
                                                                                                     name].size(),
                                                                                                 data_tf.size())
                 var_dict_torch_update[name] = data_tf
                 logging.info(
                     "torch tensor: {}, {}, loading from tf tensor: {}, {}".format(name, data_tf.size(), name_tf,
                                                                                   var_dict_tf[name_tf].shape))
 
-        return var_dict_torch_update
+        return var_dict_torch_update
```

### Comparing `funasr-0.5.3/funasr/models/e2e_asr_transducer.py` & `funasr-0.5.4/funasr/models/e2e_asr_transducer.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 from funasr.models.decoder.rnnt_decoder import RNNTDecoder
 from funasr.models.decoder.abs_decoder import AbsDecoder as AbsAttDecoder
 from funasr.models.encoder.abs_encoder import AbsEncoder
 from funasr.models.joint_net.joint_network import JointNetwork
 from funasr.modules.nets_utils import get_transducer_task_io
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.torch_utils.device_funcs import force_gatherable
-from funasr.train.abs_espnet_model import AbsESPnetModel
+from funasr.models.base_model import FunASRModel
 
 if V(torch.__version__) >= V("1.6.0"):
     from torch.cuda.amp import autocast
 else:
 
     @contextmanager
     def autocast(enabled=True):
         yield
 
 
-class TransducerModel(AbsESPnetModel):
+class TransducerModel(FunASRModel):
     """ESPnet2ASRTransducerModel module definition.
 
     Args:
         vocab_size: Size of complete vocabulary (w/ EOS and blank included).
         token_list: List of token
         frontend: Frontend module.
         specaug: SpecAugment module.
@@ -479,15 +479,15 @@
         )
         loss_lm = loss_lm.masked_fill(ignore.unsqueeze(1), 0).sum() / decoder_out.size(
             0
         )
 
         return loss_lm
 
-class UnifiedTransducerModel(AbsESPnetModel):
+class UnifiedTransducerModel(FunASRModel):
     """ESPnet2ASRTransducerModel module definition.
     Args:
         vocab_size: Size of complete vocabulary (w/ EOS and blank included).
         token_list: List of token
         frontend: Frontend module.
         specaug: SpecAugment module.
         normalize: Normalization module.
```

### Comparing `funasr-0.5.3/funasr/models/e2e_diar_eend_ola.py` & `funasr-0.5.4/funasr/models/e2e_diar_eend_ola.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from typeguard import check_argument_types
 
 from funasr.models.frontend.wav_frontend import WavFrontendMel23
 from funasr.modules.eend_ola.encoder import EENDOLATransformerEncoder
 from funasr.modules.eend_ola.encoder_decoder_attractor import EncoderDecoderAttractor
 from funasr.modules.eend_ola.utils.power import generate_mapping_dict
 from funasr.torch_utils.device_funcs import force_gatherable
-from funasr.train.abs_espnet_model import AbsESPnetModel
+from funasr.models.base_model import FunASRModel
 
 if LooseVersion(torch.__version__) >= LooseVersion("1.6.0"):
     pass
 else:
     # Nothing to do if torch<1.6.0
     @contextmanager
     def autocast(enabled=True):
@@ -30,15 +30,15 @@
 def pad_attractor(att, max_n_speakers):
     C, D = att.shape
     if C < max_n_speakers:
         att = torch.cat([att, torch.zeros(max_n_speakers - C, D).to(torch.float32).to(att.device)], dim=0)
     return att
 
 
-class DiarEENDOLAModel(AbsESPnetModel):
+class DiarEENDOLAModel(FunASRModel):
     """EEND-OLA diarization model"""
 
     def __init__(
             self,
             frontend: WavFrontendMel23,
             encoder: EENDOLATransformerEncoder,
             encoder_decoder_attractor: EncoderDecoderAttractor,
@@ -87,15 +87,14 @@
             self,
             speech: torch.Tensor,
             speech_lengths: torch.Tensor,
             text: torch.Tensor,
             text_lengths: torch.Tensor,
     ) -> Tuple[torch.Tensor, Dict[str, torch.Tensor], torch.Tensor]:
         """Frontend + Encoder + Decoder + Calc loss
-
         Args:
             speech: (Batch, Length, ...)
             speech_lengths: (Batch, )
             text: (Batch, Length)
             text_lengths: (Batch,)
         """
         assert text_lengths.dim() == 1, text_lengths.shape
```

### Comparing `funasr-0.5.3/funasr/models/e2e_diar_sond.py` & `funasr-0.5.4/funasr/models/e2e_diar_sond.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,28 +18,28 @@
 from funasr.modules.nets_utils import make_pad_mask
 from funasr.models.decoder.abs_decoder import AbsDecoder
 from funasr.models.encoder.abs_encoder import AbsEncoder
 from funasr.models.frontend.abs_frontend import AbsFrontend
 from funasr.models.specaug.abs_specaug import AbsSpecAug
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.torch_utils.device_funcs import force_gatherable
-from funasr.train.abs_espnet_model import AbsESPnetModel
+from funasr.models.base_model import FunASRModel
 from funasr.losses.label_smoothing_loss import LabelSmoothingLoss, SequenceBinaryCrossEntropy
 from funasr.utils.misc import int2vec
 
 if LooseVersion(torch.__version__) >= LooseVersion("1.6.0"):
     from torch.cuda.amp import autocast
 else:
     # Nothing to do if torch<1.6.0
     @contextmanager
     def autocast(enabled=True):
         yield
 
 
-class DiarSondModel(AbsESPnetModel):
+class DiarSondModel(FunASRModel):
     """
     Author: Speech Lab, Alibaba Group, China
     SOND: Speaker Overlap-aware Neural Diarization for Multi-party Meeting Analysis
     https://arxiv.org/abs/2211.10243
     TOLD: A Novel Two-Stage Overlap-Aware Framework for Speaker Diarization
     https://arxiv.org/abs/2303.05397
     """
@@ -111,15 +111,14 @@
         speech_lengths: torch.Tensor = None,
         profile: torch.Tensor = None,
         profile_lengths: torch.Tensor = None,
         binary_labels: torch.Tensor = None,
         binary_labels_lengths: torch.Tensor = None,
     ) -> Tuple[torch.Tensor, Dict[str, torch.Tensor], torch.Tensor]:
         """Frontend + Encoder + Speaker Encoder + CI Scorer + CD Scorer + Decoder + Calc loss
-
         Args:
             speech: (Batch, samples) or (Batch, frames, input_size)
             speech_lengths: (Batch,) default None for chunk interator,
                                      because the chunk-iterator does not
                                      have the speech_lengths returned.
                                      see in
                                      espnet2/iterators/chunk_iter_factory.py
@@ -387,15 +386,14 @@
             return logits, [(speech, speech_lengths), (profile, profile_lengths), (ci_simi, cd_simi)]
         return logits
 
     def encode(
         self, speech: torch.Tensor, speech_lengths: torch.Tensor
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Frontend + Encoder
-
         Args:
             speech: (Batch, Length, ...)
             speech_lengths: (Batch,)
         """
         with autocast(False):
             # 1. Extract feats
             feats, feats_lengths = self._extract_feats(speech, speech_lengths)
@@ -487,8 +485,8 @@
             speech_scored,
             speech_miss,
             speech_falarm,
             speaker_scored,
             speaker_miss,
             speaker_falarm,
             speaker_error,
-        )
+        )
```

### Comparing `funasr-0.5.3/funasr/models/e2e_sa_asr.py` & `funasr-0.5.4/funasr/models/e2e_sa_asr.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,26 +25,26 @@
 from funasr.models.postencoder.abs_postencoder import AbsPostEncoder
 from funasr.models.preencoder.abs_preencoder import AbsPreEncoder
 from funasr.models.specaug.abs_specaug import AbsSpecAug
 from funasr.modules.add_sos_eos import add_sos_eos
 from funasr.modules.e2e_asr_common import ErrorCalculator
 from funasr.modules.nets_utils import th_accuracy
 from funasr.torch_utils.device_funcs import force_gatherable
-from funasr.train.abs_espnet_model import AbsESPnetModel
+from funasr.models.base_model import FunASRModel
 
 if LooseVersion(torch.__version__) >= LooseVersion("1.6.0"):
     from torch.cuda.amp import autocast
 else:
     # Nothing to do if torch<1.6.0
     @contextmanager
     def autocast(enabled=True):
         yield
 
 
-class ESPnetASRModel(AbsESPnetModel):
+class ESPnetASRModel(FunASRModel):
     """CTC-attention hybrid Encoder-Decoder model"""
 
     def __init__(
             self,
             vocab_size: int,
             max_spk_num: int,
             token_list: Union[Tuple[str, ...], List[str]],
```

### Comparing `funasr-0.5.3/funasr/models/e2e_sv.py` & `funasr-0.5.4/funasr/models/e2e_sv.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,26 +25,26 @@
 from funasr.models.postencoder.abs_postencoder import AbsPostEncoder
 from funasr.models.preencoder.abs_preencoder import AbsPreEncoder
 from funasr.models.specaug.abs_specaug import AbsSpecAug
 from funasr.modules.add_sos_eos import add_sos_eos
 from funasr.modules.e2e_asr_common import ErrorCalculator
 from funasr.modules.nets_utils import th_accuracy
 from funasr.torch_utils.device_funcs import force_gatherable
-from funasr.train.abs_espnet_model import AbsESPnetModel
+from funasr.models.base_model import FunASRModel
 
 if LooseVersion(torch.__version__) >= LooseVersion("1.6.0"):
     from torch.cuda.amp import autocast
 else:
     # Nothing to do if torch<1.6.0
     @contextmanager
     def autocast(enabled=True):
         yield
 
 
-class ESPnetSVModel(AbsESPnetModel):
+class ESPnetSVModel(FunASRModel):
     """CTC-attention hybrid Encoder-Decoder model"""
 
     def __init__(
             self,
             vocab_size: int,
             token_list: Union[Tuple[str, ...], List[str]],
             frontend: Optional[AbsFrontend],
@@ -76,15 +76,14 @@
             self,
             speech: torch.Tensor,
             speech_lengths: torch.Tensor,
             text: torch.Tensor,
             text_lengths: torch.Tensor,
     ) -> Tuple[torch.Tensor, Dict[str, torch.Tensor], torch.Tensor]:
         """Frontend + Encoder + Decoder + Calc loss
-
         Args:
             speech: (Batch, Length, ...)
             speech_lengths: (Batch, )
             text: (Batch, Length)
             text_lengths: (Batch,)
         """
         assert text_lengths.dim() == 1, text_lengths.shape
@@ -217,15 +216,14 @@
             feats, feats_lengths = speech, speech_lengths
         return {"feats": feats, "feats_lengths": feats_lengths}
 
     def encode(
             self, speech: torch.Tensor, speech_lengths: torch.Tensor
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Frontend + Encoder. Note that this method is used by asr_inference.py
-
         Args:
             speech: (Batch, Length, ...)
             speech_lengths: (Batch, )
         """
         with autocast(False):
             # 1. Extract feats
             feats, feats_lengths = self._extract_feats(speech, speech_lengths)
@@ -267,8 +265,8 @@
             #  e.g. STFT and Feature extract
             #       data_loader may send time-domain signal in this case
             # speech (Batch, NSamples) -> feats: (Batch, NFrames, Dim)
             feats, feats_lengths = self.frontend(speech, speech_lengths)
         else:
             # No frontend and no feature extract
             feats, feats_lengths = speech, speech_lengths
-        return feats, feats_lengths
+        return feats, feats_lengths
```

### Comparing `funasr-0.5.3/funasr/models/e2e_tp.py` & `funasr-0.5.4/funasr/models/e2e_tp.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,28 +13,27 @@
 
 from funasr.models.encoder.abs_encoder import AbsEncoder
 from funasr.models.frontend.abs_frontend import AbsFrontend
 from funasr.models.predictor.cif import mae_loss
 from funasr.modules.add_sos_eos import add_sos_eos
 from funasr.modules.nets_utils import make_pad_mask, pad_list
 from funasr.torch_utils.device_funcs import force_gatherable
-from funasr.train.abs_espnet_model import AbsESPnetModel
+from funasr.models.base_model import FunASRModel
 from funasr.models.predictor.cif import CifPredictorV3
 
-
 if LooseVersion(torch.__version__) >= LooseVersion("1.6.0"):
     from torch.cuda.amp import autocast
 else:
     # Nothing to do if torch<1.6.0
     @contextmanager
     def autocast(enabled=True):
         yield
 
 
-class TimestampPredictor(AbsESPnetModel):
+class TimestampPredictor(FunASRModel):
     """
     Author: Speech Lab of DAMO Academy, Alibaba Group
     """
 
     def __init__(
             self,
             frontend: Optional[AbsFrontend],
@@ -52,24 +51,23 @@
         self.encoder = encoder
         self.encoder.interctc_use_conditioning = False
 
         self.predictor = predictor
         self.predictor_bias = predictor_bias
         self.criterion_pre = mae_loss()
         self.token_list = token_list
-    
+
     def forward(
             self,
             speech: torch.Tensor,
             speech_lengths: torch.Tensor,
             text: torch.Tensor,
             text_lengths: torch.Tensor,
     ) -> Tuple[torch.Tensor, Dict[str, torch.Tensor], torch.Tensor]:
         """Frontend + Encoder + Decoder + Calc loss
-
         Args:
                 speech: (Batch, Length, ...)
                 speech_lengths: (Batch, )
                 text: (Batch, Length)
                 text_lengths: (Batch,)
         """
         assert text_lengths.dim() == 1, text_lengths.shape
@@ -109,30 +107,29 @@
         loss, stats, weight = force_gatherable((loss, stats, batch_size), loss.device)
         return loss, stats, weight
 
     def encode(
             self, speech: torch.Tensor, speech_lengths: torch.Tensor
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Frontend + Encoder. Note that this method is used by asr_inference.py
-
         Args:
                 speech: (Batch, Length, ...)
                 speech_lengths: (Batch, )
         """
         with autocast(False):
             # 1. Extract feats
             feats, feats_lengths = self._extract_feats(speech, speech_lengths)
 
         # 4. Forward encoder
         # feats: (Batch, Length, Dim)
         # -> encoder_out: (Batch, Length2, Dim2)
         encoder_out, encoder_out_lens, _ = self.encoder(feats, feats_lengths)
 
         return encoder_out, encoder_out_lens
-    
+
     def _extract_feats(
             self, speech: torch.Tensor, speech_lengths: torch.Tensor
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         assert speech_lengths.dim() == 1, speech_lengths.shape
 
         # for data-parallel
         speech = speech[:, : speech_lengths.max()]
@@ -147,16 +144,16 @@
             feats, feats_lengths = speech, speech_lengths
         return feats, feats_lengths
 
     def calc_predictor_timestamp(self, encoder_out, encoder_out_lens, token_num):
         encoder_out_mask = (~make_pad_mask(encoder_out_lens, maxlen=encoder_out.size(1))[:, None, :]).to(
             encoder_out.device)
         ds_alphas, ds_cif_peak, us_alphas, us_peaks = self.predictor.get_upsample_timestamp(encoder_out,
-                                                                                               encoder_out_mask,
-                                                                                               token_num)
+                                                                                            encoder_out_mask,
+                                                                                            token_num)
         return ds_alphas, ds_cif_peak, us_alphas, us_peaks
 
     def collect_feats(
             self,
             speech: torch.Tensor,
             speech_lengths: torch.Tensor,
             text: torch.Tensor,
```

### Comparing `funasr-0.5.3/funasr/models/e2e_uni_asr.py` & `funasr-0.5.4/funasr/models/e2e_uni_asr.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 from funasr.models.encoder.abs_encoder import AbsEncoder
 from funasr.models.frontend.abs_frontend import AbsFrontend
 from funasr.models.postencoder.abs_postencoder import AbsPostEncoder
 from funasr.models.preencoder.abs_preencoder import AbsPreEncoder
 from funasr.models.specaug.abs_specaug import AbsSpecAug
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.torch_utils.device_funcs import force_gatherable
-from funasr.train.abs_espnet_model import AbsESPnetModel
+from funasr.models.base_model import FunASRModel
 from funasr.modules.streaming_utils.chunk_utilis import sequence_mask
 from funasr.models.predictor.cif import mae_loss
 
 if LooseVersion(torch.__version__) >= LooseVersion("1.6.0"):
     from torch.cuda.amp import autocast
 else:
     # Nothing to do if torch<1.6.0
     @contextmanager
     def autocast(enabled=True):
         yield
 
 
-class UniASR(AbsESPnetModel):
+class UniASR(FunASRModel):
     """
     Author: Speech Lab of DAMO Academy, Alibaba Group
     """
 
     def __init__(
         self,
         vocab_size: int,
@@ -175,15 +175,14 @@
         speech: torch.Tensor,
         speech_lengths: torch.Tensor,
         text: torch.Tensor,
         text_lengths: torch.Tensor,
         decoding_ind: int = None,
     ) -> Tuple[torch.Tensor, Dict[str, torch.Tensor], torch.Tensor]:
         """Frontend + Encoder + Decoder + Calc loss
-
         Args:
                         speech: (Batch, Length, ...)
                         speech_lengths: (Batch, )
                         text: (Batch, Length)
                         text_lengths: (Batch,)
         """
         assert text_lengths.dim() == 1, text_lengths.shape
@@ -465,15 +464,14 @@
             feats, feats_lengths = speech, speech_lengths
         return {"feats": feats, "feats_lengths": feats_lengths}
 
     def encode(
         self, speech: torch.Tensor, speech_lengths: torch.Tensor, ind: int = 0,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Frontend + Encoder. Note that this method is used by asr_inference.py
-
         Args:
                         speech: (Batch, Length, ...)
                         speech_lengths: (Batch, )
         """
         with autocast(False):
             # 1. Extract feats
             feats, feats_lengths = self._extract_feats(speech, speech_lengths)
@@ -529,15 +527,14 @@
         encoder_out: torch.Tensor,
         encoder_out_lens: torch.Tensor,
         speech: torch.Tensor,
         speech_lengths: torch.Tensor,
         ind: int = 0,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Frontend + Encoder. Note that this method is used by asr_inference.py
-
         Args:
                         speech: (Batch, Length, ...)
                         speech_lengths: (Batch, )
         """
         # with autocast(False):
         # 	# 1. Extract feats
         # 	feats, feats_lengths = self._extract_feats(speech, speech_lengths)
@@ -623,17 +620,15 @@
         self,
         encoder_out: torch.Tensor,
         encoder_out_lens: torch.Tensor,
         ys_pad: torch.Tensor,
         ys_pad_lens: torch.Tensor,
     ) -> torch.Tensor:
         """Compute negative log likelihood(nll) from transformer-decoder
-
         Normally, this function is called in batchify_nll.
-
         Args:
                         encoder_out: (Batch, Length, Dim)
                         encoder_out_lens: (Batch,)
                         ys_pad: (Batch, Length)
                         ys_pad_lens: (Batch,)
         """
         ys_in_pad, ys_out_pad = add_sos_eos(ys_pad, self.sos, self.eos, self.ignore_id)
@@ -662,15 +657,14 @@
         encoder_out: torch.Tensor,
         encoder_out_lens: torch.Tensor,
         ys_pad: torch.Tensor,
         ys_pad_lens: torch.Tensor,
         batch_size: int = 100,
     ):
         """Compute negative log likelihood(nll) from transformer-decoder
-
         To avoid OOM, this fuction seperate the input into batches.
         Then call nll for each batch and combine and return results.
         Args:
                         encoder_out: (Batch, Length, Dim)
                         encoder_out_lens: (Batch,)
                         ys_pad: (Batch, Length)
                         ys_pad_lens: (Batch,)
@@ -1068,8 +1062,7 @@
 
         # Calc CER using CTC
         cer_ctc = None
         if not self.training and self.error_calculator is not None:
             ys_hat = self.ctc2.argmax(encoder_out).data
             cer_ctc = self.error_calculator(ys_hat.cpu(), ys_pad.cpu(), is_ctc=True)
         return loss_ctc, cer_ctc
-
```

### Comparing `funasr-0.5.3/funasr/models/e2e_vad.py` & `funasr-0.5.4/funasr/models/e2e_vad.py`

 * *Files 0% similar despite different names*

```diff
@@ -465,15 +465,15 @@
                 self.noise_average_decibel = cur_decibel
             else:
                 self.noise_average_decibel = (cur_decibel + self.noise_average_decibel * (
                         self.vad_opts.noise_frame_num_used_for_snr
                         - 1)) / self.vad_opts.noise_frame_num_used_for_snr
 
         return frame_state
-     
+
     def forward(self, feats: torch.Tensor, waveform: torch.tensor, in_cache: Dict[str, torch.Tensor] = dict(),
                 is_final: bool = False
                 ) -> Tuple[List[List[List[int]]], Dict[str, torch.Tensor]]:
         self.waveform = waveform  # compute decibel for each frame
         self.ComputeDecibel()
         self.ComputeScores(feats, in_cache)
         if not is_final:
@@ -495,19 +495,19 @@
                 segments.append(segment_batch)
         if is_final:
             # reset class variables and clear the dict for the next query
             self.AllResetDetection()
         return segments, in_cache
 
     def forward_online(self, feats: torch.Tensor, waveform: torch.tensor, in_cache: Dict[str, torch.Tensor] = dict(),
-                is_final: bool = False, max_end_sil: int = 800
-                ) -> Tuple[List[List[List[int]]], Dict[str, torch.Tensor]]:
+                       is_final: bool = False, max_end_sil: int = 800
+                       ) -> Tuple[List[List[List[int]]], Dict[str, torch.Tensor]]:
         self.max_end_sil_frame_cnt_thresh = max_end_sil - self.vad_opts.speech_to_sil_time_thres
         self.waveform = waveform  # compute decibel for each frame
-        
+
         self.ComputeScores(feats, in_cache)
         self.ComputeDecibel()
         if not is_final:
             self.DetectCommonFrames()
         else:
             self.DetectLastFrames()
         segments = []
```

### Comparing `funasr-0.5.3/funasr/models/encoder/conformer_encoder.py` & `funasr-0.5.4/funasr/models/encoder/conformer_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 from typing import Dict
 
 import torch
 from torch import nn
 from typeguard import check_argument_types
 
 from funasr.models.ctc import CTC
-from funasr.models.encoder.abs_encoder import AbsEncoder
 from funasr.modules.attention import (
     MultiHeadedAttention,  # noqa: H301
     RelPositionMultiHeadedAttention,  # noqa: H301
     RelPositionMultiHeadedAttentionChunk,
     LegacyRelPositionMultiHeadedAttention,  # noqa: H301
 )
+from funasr.models.encoder.abs_encoder import AbsEncoder
 from funasr.modules.embedding import (
     PositionalEncoding,  # noqa: H301
     ScaledPositionalEncoding,  # noqa: H301
     RelPositionalEncoding,  # noqa: H301
     LegacyRelPositionalEncoding,  # noqa: H301
     StreamingRelPositionalEncoding,
 )
@@ -1074,15 +1074,15 @@
             raise TooShortUttError(
                 f"has {x.size(1)} frames and is too short for subsampling "
                 + f"(it needs more than {limit_size} frames), return empty results",
                 x.size(1),
                 limit_size,
             )
 
-        mask = make_source_mask(x_len)
+        mask = make_source_mask(x_len).to(x.device)
 
         if self.unified_model_training:
             chunk_size = self.default_chunk_size + torch.randint(-self.jitter_range, self.jitter_range+1, (1,)).item()
             x, mask = self.embed(x, mask, chunk_size)
             pos_enc = self.pos_enc(x)
             chunk_mask = make_chunk_mask(
                 x.size(1),
```

### Comparing `funasr-0.5.3/funasr/models/encoder/data2vec_encoder.py` & `funasr-0.5.4/funasr/models/encoder/data2vec_encoder.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -570,8 +570,8 @@
         self.ema = None
         if last_layer is not None:
             self.encoder.layers = nn.ModuleList(
                 l for i, l in enumerate(self.encoder.layers) if i <= last_layer
             )
 
     def output_size(self) -> int:
-        return self.encoder_embed_dim
+        return self.encoder_embed_dim
```

### Comparing `funasr-0.5.3/funasr/models/encoder/ecapa_tdnn_encoder.py` & `funasr-0.5.4/funasr/models/encoder/ecapa_tdnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/models/encoder/encoder_layer_mfcca.py` & `funasr-0.5.4/funasr/models/encoder/encoder_layer_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/models/encoder/fsmn_encoder.py` & `funasr-0.5.4/funasr/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/models/encoder/mfcca_encoder.py` & `funasr-0.5.4/funasr/models/encoder/mfcca_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,21 +34,20 @@
 from funasr.modules.subsampling import Conv2dSubsampling8
 from funasr.modules.subsampling import TooShortUttError
 from funasr.modules.subsampling import check_short_utt
 from funasr.models.encoder.abs_encoder import AbsEncoder
 import pdb
 import math
 
+
 class ConvolutionModule(nn.Module):
     """ConvolutionModule in Conformer model.
-
     Args:
         channels (int): The number of channels of conv layers.
         kernel_size (int): Kernerl size of conv layers.
-
     """
 
     def __init__(self, channels, kernel_size, activation=nn.ReLU(), bias=True):
         """Construct an ConvolutionModule object."""
         super(ConvolutionModule, self).__init__()
         # kernerl_size should be a odd number for 'SAME' padding
         assert (kernel_size - 1) % 2 == 0
@@ -79,21 +78,18 @@
             padding=0,
             bias=bias,
         )
         self.activation = activation
 
     def forward(self, x):
         """Compute convolution module.
-
         Args:
             x (torch.Tensor): Input tensor (#batch, time, channels).
-
         Returns:
             torch.Tensor: Output tensor (#batch, time, channels).
-
         """
         # exchange the temporal dimension and the feature dimension
         x = x.transpose(1, 2)
 
         # GLU mechanism
         x = self.pointwise_conv1(x)  # (batch, 2*channel, dim)
         x = nn.functional.glu(x, dim=1)  # (batch, channel, dim)
@@ -103,18 +99,16 @@
         x = self.activation(self.norm(x))
 
         x = self.pointwise_conv2(x)
 
         return x.transpose(1, 2)
 
 
-
 class MFCCAEncoder(AbsEncoder):
     """Conformer encoder module.
-
     Args:
         input_size (int): Input dimension.
         output_size (int): Dimention of attention.
         attention_heads (int): The number of heads of multi head attention.
         linear_units (int): The number of units of position-wise feed forward.
         num_blocks (int): The number of decoder blocks.
         dropout_rate (float): Dropout rate.
@@ -136,41 +130,40 @@
         encoder_attn_layer_type (str): Encoder attention layer type.
         activation_type (str): Encoder activation function type.
         macaron_style (bool): Whether to use macaron style for positionwise layer.
         use_cnn_module (bool): Whether to use convolution module.
         zero_triu (bool): Whether to zero the upper triangular part of attention matrix.
         cnn_module_kernel (int): Kernerl size of convolution module.
         padding_idx (int): Padding idx for input_layer=embed.
-
     """
 
     def __init__(
-        self,
-        input_size: int,
-        output_size: int = 256,
-        attention_heads: int = 4,
-        linear_units: int = 2048,
-        num_blocks: int = 6,
-        dropout_rate: float = 0.1,
-        positional_dropout_rate: float = 0.1,
-        attention_dropout_rate: float = 0.0,
-        input_layer: str = "conv2d",
-        normalize_before: bool = True,
-        concat_after: bool = False,
-        positionwise_layer_type: str = "linear",
-        positionwise_conv_kernel_size: int = 3,
-        macaron_style: bool = False,
-        rel_pos_type: str = "legacy",
-        pos_enc_layer_type: str = "rel_pos",
-        selfattention_layer_type: str = "rel_selfattn",
-        activation_type: str = "swish",
-        use_cnn_module: bool = True,
-        zero_triu: bool = False,
-        cnn_module_kernel: int = 31,
-        padding_idx: int = -1,
+            self,
+            input_size: int,
+            output_size: int = 256,
+            attention_heads: int = 4,
+            linear_units: int = 2048,
+            num_blocks: int = 6,
+            dropout_rate: float = 0.1,
+            positional_dropout_rate: float = 0.1,
+            attention_dropout_rate: float = 0.0,
+            input_layer: str = "conv2d",
+            normalize_before: bool = True,
+            concat_after: bool = False,
+            positionwise_layer_type: str = "linear",
+            positionwise_conv_kernel_size: int = 3,
+            macaron_style: bool = False,
+            rel_pos_type: str = "legacy",
+            pos_enc_layer_type: str = "rel_pos",
+            selfattention_layer_type: str = "rel_selfattn",
+            activation_type: str = "swish",
+            use_cnn_module: bool = True,
+            zero_triu: bool = False,
+            cnn_module_kernel: int = 31,
+            padding_idx: int = -1,
     ):
         assert check_argument_types()
         super().__init__()
         self._output_size = output_size
 
         if rel_pos_type == "legacy":
             if pos_enc_layer_type == "rel_pos":
@@ -195,15 +188,15 @@
             assert selfattention_layer_type == "legacy_rel_selfattn"
             pos_enc_class = LegacyRelPositionalEncoding
             logging.warning(
                 "Using legacy_rel_pos and it will be deprecated in the future."
             )
         else:
             raise ValueError("unknown pos_enc_layer: " + pos_enc_layer_type)
-        
+
         if input_layer == "linear":
             self.embed = torch.nn.Sequential(
                 torch.nn.Linear(input_size, output_size),
                 torch.nn.LayerNorm(output_size),
                 torch.nn.Dropout(dropout_rate),
                 pos_enc_class(output_size, positional_dropout_rate),
             )
@@ -279,15 +272,15 @@
                 output_size,
                 attention_dropout_rate,
             )
         elif selfattention_layer_type == "legacy_rel_selfattn":
             assert pos_enc_layer_type == "legacy_rel_pos"
             encoder_selfattn_layer = LegacyRelPositionMultiHeadedAttention
             encoder_selfattn_layer_args = (
-               attention_heads,
+                attention_heads,
                 output_size,
                 attention_dropout_rate,
             )
             logging.warning(
                 "Using legacy_rel_selfattn and it will be deprecated in the future."
             )
         elif selfattention_layer_type == "rel_selfattn":
@@ -322,50 +315,47 @@
                 dropout_rate,
                 normalize_before,
                 concat_after,
             ),
         )
         if self.normalize_before:
             self.after_norm = LayerNorm(output_size)
-        self.conv1 = torch.nn.Conv2d(8, 16, [5,7], stride=[1,1], padding=(2,3))
+        self.conv1 = torch.nn.Conv2d(8, 16, [5, 7], stride=[1, 1], padding=(2, 3))
 
-        self.conv2 = torch.nn.Conv2d(16, 32, [5,7], stride=[1,1], padding=(2,3))
+        self.conv2 = torch.nn.Conv2d(16, 32, [5, 7], stride=[1, 1], padding=(2, 3))
 
-        self.conv3 = torch.nn.Conv2d(32, 16, [5,7], stride=[1,1], padding=(2,3))
+        self.conv3 = torch.nn.Conv2d(32, 16, [5, 7], stride=[1, 1], padding=(2, 3))
 
-        self.conv4 = torch.nn.Conv2d(16, 1, [5,7], stride=[1,1], padding=(2,3))
+        self.conv4 = torch.nn.Conv2d(16, 1, [5, 7], stride=[1, 1], padding=(2, 3))
 
     def output_size(self) -> int:
         return self._output_size
 
     def forward(
-        self,
-        xs_pad: torch.Tensor,
-        ilens: torch.Tensor,
-        channel_size: torch.Tensor,
-        prev_states: torch.Tensor = None,
+            self,
+            xs_pad: torch.Tensor,
+            ilens: torch.Tensor,
+            channel_size: torch.Tensor,
+            prev_states: torch.Tensor = None,
     ) -> Tuple[torch.Tensor, torch.Tensor, Optional[torch.Tensor]]:
         """Calculate forward propagation.
-
         Args:
             xs_pad (torch.Tensor): Input tensor (#batch, L, input_size).
             ilens (torch.Tensor): Input length (#batch).
             prev_states (torch.Tensor): Not to be used now.
-
         Returns:
             torch.Tensor: Output tensor (#batch, L, output_size).
             torch.Tensor: Output length (#batch).
             torch.Tensor: Not to be used now.
-
         """
         masks = (~make_pad_mask(ilens)[:, None, :]).to(xs_pad.device)
         if (
-            isinstance(self.embed, Conv2dSubsampling)
-            or isinstance(self.embed, Conv2dSubsampling6)
-            or isinstance(self.embed, Conv2dSubsampling8)
+                isinstance(self.embed, Conv2dSubsampling)
+                or isinstance(self.embed, Conv2dSubsampling6)
+                or isinstance(self.embed, Conv2dSubsampling8)
         ):
             short_status, limit_size = check_short_utt(self.embed, xs_pad.size(1))
             if short_status:
                 raise TooShortUttError(
                     f"has {xs_pad.size(1)} frames and is too short for subsampling "
                     + f"(it needs more than {limit_size} frames), return empty results",
                     xs_pad.size(1),
@@ -376,56 +366,54 @@
             xs_pad = self.embed(xs_pad)
         xs_pad, masks, channel_size = self.encoders(xs_pad, masks, channel_size)
         if isinstance(xs_pad, tuple):
             xs_pad = xs_pad[0]
 
         t_leng = xs_pad.size(1)
         d_dim = xs_pad.size(2)
-        xs_pad = xs_pad.reshape(-1,channel_size,t_leng,d_dim)
-        #pdb.set_trace()
-        if(channel_size<8):
-            repeat_num = math.ceil(8/channel_size)
-            xs_pad = xs_pad.repeat(1,repeat_num,1,1)[:,0:8,:,:]
+        xs_pad = xs_pad.reshape(-1, channel_size, t_leng, d_dim)
+        # pdb.set_trace()
+        if (channel_size < 8):
+            repeat_num = math.ceil(8 / channel_size)
+            xs_pad = xs_pad.repeat(1, repeat_num, 1, 1)[:, 0:8, :, :]
         xs_pad = self.conv1(xs_pad)
         xs_pad = self.conv2(xs_pad)
         xs_pad = self.conv3(xs_pad)
         xs_pad = self.conv4(xs_pad)
-        xs_pad = xs_pad.squeeze().reshape(-1,t_leng,d_dim)
+        xs_pad = xs_pad.squeeze().reshape(-1, t_leng, d_dim)
         mask_tmp = masks.size(1)
-        masks = masks.reshape(-1,channel_size,mask_tmp,t_leng)[:,0,:,:]
+        masks = masks.reshape(-1, channel_size, mask_tmp, t_leng)[:, 0, :, :]
 
         if self.normalize_before:
             xs_pad = self.after_norm(xs_pad)
 
         olens = masks.squeeze(1).sum(1)
         return xs_pad, olens, None
+
     def forward_hidden(
-        self,
-        xs_pad: torch.Tensor,
-        ilens: torch.Tensor,
-        prev_states: torch.Tensor = None,
+            self,
+            xs_pad: torch.Tensor,
+            ilens: torch.Tensor,
+            prev_states: torch.Tensor = None,
     ) -> Tuple[torch.Tensor, torch.Tensor, Optional[torch.Tensor]]:
         """Calculate forward propagation.
-
         Args:
             xs_pad (torch.Tensor): Input tensor (#batch, L, input_size).
             ilens (torch.Tensor): Input length (#batch).
             prev_states (torch.Tensor): Not to be used now.
-
         Returns:
             torch.Tensor: Output tensor (#batch, L, output_size).
             torch.Tensor: Output length (#batch).
             torch.Tensor: Not to be used now.
-
         """
         masks = (~make_pad_mask(ilens)[:, None, :]).to(xs_pad.device)
         if (
-            isinstance(self.embed, Conv2dSubsampling)
-            or isinstance(self.embed, Conv2dSubsampling6)
-            or isinstance(self.embed, Conv2dSubsampling8)
+                isinstance(self.embed, Conv2dSubsampling)
+                or isinstance(self.embed, Conv2dSubsampling6)
+                or isinstance(self.embed, Conv2dSubsampling8)
         ):
             short_status, limit_size = check_short_utt(self.embed, xs_pad.size(1))
             if short_status:
                 raise TooShortUttError(
                     f"has {xs_pad.size(1)} frames and is too short for subsampling "
                     + f"(it needs more than {limit_size} frames), return empty results",
                     xs_pad.size(1),
@@ -443,8 +431,8 @@
             xs_pad = xs_pad[0]
             hidden_feature = hidden_feature[0]
         if self.normalize_before:
             xs_pad = self.after_norm(xs_pad)
             self.hidden_feature = self.after_norm(hidden_feature)
 
         olens = masks.squeeze(1).sum(1)
-        return xs_pad, olens, None
+        return xs_pad, olens, None
```

### Comparing `funasr-0.5.3/funasr/models/encoder/opennmt_encoders/ci_scorers.py` & `funasr-0.5.4/funasr/models/encoder/opennmt_encoders/ci_scorers.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/models/encoder/opennmt_encoders/conv_encoder.py` & `funasr-0.5.4/funasr/models/encoder/opennmt_encoders/conv_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py` & `funasr-0.5.4/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py` & `funasr-0.5.4/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/models/encoder/resnet34_encoder.py` & `funasr-0.5.4/funasr/models/encoder/resnet34_encoder.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -846,8 +846,8 @@
                         var_dict_torch_update[name] = torch.from_numpy(np.array(map_dict[name])).type(torch.int64).to("cpu")
                         logging.info("torch tensor: {}, manually assigning to: {}".format(
                             name, map_dict[name]
                         ))
                 else:
                     logging.warning("{} is missed from tf checkpoint".format(name))
 
-        return var_dict_torch_update
+        return var_dict_torch_update
```

### Comparing `funasr-0.5.3/funasr/models/encoder/rnn_encoder.py` & `funasr-0.5.4/funasr/models/encoder/rnn_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 
 import numpy as np
 import torch
 from typeguard import check_argument_types
@@ -10,24 +11,22 @@
 from funasr.modules.rnn.encoders import RNN
 from funasr.modules.rnn.encoders import RNNP
 from funasr.models.encoder.abs_encoder import AbsEncoder
 
 
 class RNNEncoder(AbsEncoder):
     """RNNEncoder class.
-
     Args:
         input_size: The number of expected features in the input
         output_size: The number of output features
         hidden_size: The number of hidden features
         bidirectional: If ``True`` becomes a bidirectional LSTM
         use_projection: Use projection layer or not
         num_layers: Number of recurrent layers
         dropout: dropout probability
-
     """
 
     def __init__(
         self,
         input_size: int,
         rnn_type: str = "lstm",
         bidirectional: bool = True,
```

### Comparing `funasr-0.5.3/funasr/models/encoder/sanm_encoder.py` & `funasr-0.5.4/funasr/models/encoder/sanm_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,18 @@
 from funasr.modules.repeat import repeat
 from funasr.modules.subsampling import Conv2dSubsampling
 from funasr.modules.subsampling import Conv2dSubsampling2
 from funasr.modules.subsampling import Conv2dSubsampling6
 from funasr.modules.subsampling import Conv2dSubsampling8
 from funasr.modules.subsampling import TooShortUttError
 from funasr.modules.subsampling import check_short_utt
+from funasr.modules.mask import subsequent_mask, vad_mask
+
 from funasr.models.ctc import CTC
 from funasr.models.encoder.abs_encoder import AbsEncoder
-from funasr.modules.mask import subsequent_mask, vad_mask
 
 class EncoderLayerSANM(nn.Module):
     def __init__(
         self,
         in_size,
         size,
         self_attn,
@@ -350,26 +351,17 @@
         if len(intermediate_outs) > 0:
             return (xs_pad, intermediate_outs), olens, None
         return xs_pad, olens, None
 
     def _add_overlap_chunk(self, feats: np.ndarray, cache: dict = {}):
         if len(cache) == 0:
             return feats
-        # process last chunk
         cache["feats"] = to_device(cache["feats"], device=feats.device)
         overlap_feats = torch.cat((cache["feats"], feats), dim=1)
-        if cache["is_final"]:
-            cache["feats"] = overlap_feats[:, -cache["chunk_size"][0]:, :]
-            if not cache["last_chunk"]:
-               padding_length = sum(cache["chunk_size"]) - overlap_feats.shape[1]
-               overlap_feats = overlap_feats.transpose(1, 2)
-               overlap_feats = F.pad(overlap_feats, (0, padding_length))
-               overlap_feats = overlap_feats.transpose(1, 2)
-        else:
-            cache["feats"] = overlap_feats[:, -(cache["chunk_size"][0] + cache["chunk_size"][2]):, :]
+        cache["feats"] = overlap_feats[:, -(cache["chunk_size"][0] + cache["chunk_size"][2]):, :]
         return overlap_feats
 
     def forward_chunk(self,
                       xs_pad: torch.Tensor,
                       ilens: torch.Tensor,
                       cache: dict = None,
                       ctc: CTC = None,
```

### Comparing `funasr-0.5.3/funasr/models/encoder/transformer_encoder.py` & `funasr-0.5.4/funasr/models/encoder/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/models/frontend/default.py` & `funasr-0.5.4/funasr/models/frontend/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from funasr.models.frontend.abs_frontend import AbsFrontend
 from funasr.modules.frontends.frontend import Frontend
 from funasr.utils.get_default_kwargs import get_default_kwargs
 
 
 class DefaultFrontend(AbsFrontend):
     """Conventional frontend structure for ASR.
-
     Stft -> WPE -> MVDR-Beamformer -> Power-spec -> Mel-Fbank -> CMVN
     """
 
     def __init__(
             self,
             fs: Union[int, str] = 16000,
             n_fft: int = 512,
@@ -98,16 +97,16 @@
             # input_stft: (Batch, Length, [Channel], Freq)
             input_stft, _, mask = self.frontend(input_stft, feats_lens)
 
         # 3. [Multi channel case]: Select a channel
         if input_stft.dim() == 4:
             # h: (B, T, C, F) -> h: (B, T, F)
             if self.training:
-                if self.use_channel == None:
-                    input_stft = input_stft[:, :, 0, :]
+                if self.use_channel is not None:
+                    input_stft = input_stft[:, :, self.use_channel, :]
                 else:
                     # Select 1ch randomly
                     ch = np.random.randint(input_stft.size(2))
                     input_stft = input_stft[:, :, ch, :]
             else:
                 # Use the first channel
                 input_stft = input_stft[:, :, 0, :]
@@ -138,15 +137,14 @@
         return input_stft, feats_lens
 
 
 
 
 class MultiChannelFrontend(AbsFrontend):
     """Conventional frontend structure for ASR.
-
     Stft -> WPE -> MVDR-Beamformer -> Power-spec -> Mel-Fbank -> CMVN
     """
 
     def __init__(
             self,
             fs: Union[int, str] = 16000,
             n_fft: int = 512,
@@ -256,8 +254,8 @@
         assert input_stft.dim() >= 4, input_stft.shape
         # "2" refers to the real/imag parts of Complex
         assert input_stft.shape[-1] == 2, input_stft.shape
 
         # Change torch.Tensor to ComplexTensor
         # input_stft: (..., F, 2) -> (..., F)
         input_stft = ComplexTensor(input_stft[..., 0], input_stft[..., 1])
-        return input_stft, feats_lens
+        return input_stft, feats_lens
```

### Comparing `funasr-0.5.3/funasr/models/frontend/eend_ola_feature.py` & `funasr-0.5.4/funasr/models/frontend/eend_ola_feature.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/models/frontend/fused.py` & `funasr-0.5.4/funasr/models/frontend/fused.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -139,8 +139,8 @@
                 self.feats_final, dim=-1
             )  # change the input size of the preencoder : proj_dim * n_frontends
             feats_lens = torch.ones_like(self.feats[0][1]) * (m)
 
         else:
             raise NotImplementedError
 
-        return input_feats, feats_lens
+        return input_feats, feats_lens
```

### Comparing `funasr-0.5.3/funasr/models/frontend/s3prl.py` & `funasr-0.5.4/funasr/models/frontend/s3prl.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,14 @@
             upstream_device="cpu",
         )
 
         return s3prl_upstream, s3prl_featurizer
 
     def _tile_representations(self, feature):
         """Tile up the representations by `tile_factor`.
-
         Input - sequence of representations
                 shape: (batch_size, seq_len, feature_dim)
         Output - sequence of tiled representations
                  shape: (batch_size, seq_len * factor, feature_dim)
         """
         assert (
                 len(feature.shape) == 3
```

### Comparing `funasr-0.5.3/funasr/models/frontend/wav_frontend.py` & `funasr-0.5.4/funasr/models/frontend/wav_frontend.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -496,8 +496,8 @@
             feats.append(mat)
             feats_lens.append(feat_length)
 
         feats_lens = torch.as_tensor(feats_lens)
         feats_pad = pad_sequence(feats,
                                  batch_first=True,
                                  padding_value=0.0)
-        return feats_pad, feats_lens
+        return feats_pad, feats_lens
```

### Comparing `funasr-0.5.3/funasr/models/frontend/windowing.py` & `funasr-0.5.4/funasr/models/frontend/windowing.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,20 +8,18 @@
 import torch
 from typeguard import check_argument_types
 from typing import Tuple
 
 
 class SlidingWindow(AbsFrontend):
     """Sliding Window.
-
     Provides a sliding window over a batched continuous raw audio tensor.
     Optionally, provides padding (Currently not implemented).
     Combine this module with a pre-encoder compatible with raw audio data,
     for example Sinc convolutions.
-
     Known issues:
     Output length is calculated incorrectly if audio shorter than win_length.
     WARNING: trailing values are discarded - padding not implemented yet.
     There is currently no additional window function applied to input values.
     """
 
     def __init__(
@@ -29,15 +27,14 @@
         win_length: int = 400,
         hop_length: int = 160,
         channels: int = 1,
         padding: int = None,
         fs=None,
     ):
         """Initialize.
-
         Args:
             win_length: Length of frame.
             hop_length: Relative starting point of next frame.
             channels: Number of input channels.
             padding: Padding (placeholder, currently not implemented).
             fs:  Sampling rate (placeholder for compatibility, not used).
         """
@@ -49,19 +46,17 @@
         self.channels = channels
         self.padding = padding
 
     def forward(
         self, input: torch.Tensor, input_lengths: torch.Tensor
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Apply a sliding window on the input.
-
         Args:
             input: Input (B, T, C*D) or (B, T*C*D), with D=C=1.
             input_lengths: Input lengths within batch.
-
         Returns:
             Tensor: Output with dimensions (B, T, C, D), with D=win_length.
             Tensor: Output lengths within batch.
         """
         input_size = input.size()
         B = input_size[0]
         T = input_size[1]
@@ -74,8 +69,8 @@
         output = windowed.permute(1, 0, 2, 3).contiguous()
         # After unfold(), windowed lengths change:
         output_lengths = (input_lengths - self.win_length) // self.hop_length + 1
         return output, output_lengths
 
     def output_size(self) -> int:
         """Return output length of feature dimension D, i.e. the window length."""
-        return self.win_length
+        return self.win_length
```

### Comparing `funasr-0.5.3/funasr/models/joint_net/joint_network.py` & `funasr-0.5.4/funasr/models/joint_net/joint_network.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/models/pooling/statistic_pooling.py` & `funasr-0.5.4/funasr/models/pooling/statistic_pooling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/models/postencoder/hugging_face_transformers_postencoder.py` & `funasr-0.5.4/funasr/models/postencoder/hugging_face_transformers_postencoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/models/predictor/cif.py` & `funasr-0.5.4/funasr/models/predictor/cif.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,21 +217,22 @@
         list_fires = []
         list_frames = []
         cache_alphas = []
         cache_hiddens = []
 
         if cache is not None and "chunk_size" in cache:
             alphas[:, :cache["chunk_size"][0]] = 0.0
-            alphas[:, sum(cache["chunk_size"][:2]):] = 0.0
+            if "is_final" in cache and not cache["is_final"]:
+                alphas[:, sum(cache["chunk_size"][:2]):] = 0.0
         if cache is not None and "cif_alphas" in cache and "cif_hidden" in cache:
             cache["cif_hidden"] = to_device(cache["cif_hidden"], device=hidden.device)
             cache["cif_alphas"] = to_device(cache["cif_alphas"], device=alphas.device)
             hidden = torch.cat((cache["cif_hidden"], hidden), dim=1)
             alphas = torch.cat((cache["cif_alphas"], alphas), dim=1)
-        if cache is not None and "last_chunk" in cache and cache["last_chunk"]:
+        if cache is not None and "is_final" in cache and cache["is_final"]:
             tail_hidden = torch.zeros((batch_size, 1, hidden_size), device=hidden.device)
             tail_alphas = torch.tensor([[self.tail_threshold]], device=alphas.device)
             tail_alphas = torch.tile(tail_alphas, (batch_size, 1))
             hidden = torch.cat((hidden, tail_hidden), dim=1)
             alphas = torch.cat((alphas, tail_alphas), dim=1)
 
         len_time = alphas.shape[1]
```

### Comparing `funasr-0.5.3/funasr/models/preencoder/linear.py` & `funasr-0.5.4/funasr/models/preencoder/linear.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/models/preencoder/sinc.py` & `funasr-0.5.4/funasr/models/preencoder/sinc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/models/specaug/specaug.py` & `funasr-0.5.4/funasr/models/specaug/specaug.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/models/target_delay_transformer.py` & `funasr-0.5.4/funasr/models/target_delay_transformer.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,18 @@
 from typing import List
 from typing import Tuple
 
 import torch
 import torch.nn as nn
 
 from funasr.modules.embedding import SinusoidalPositionEncoder
-#from funasr.models.encoder.transformer_encoder import TransformerEncoder as Encoder
 from funasr.models.encoder.sanm_encoder import SANMEncoder as Encoder
-#from funasr.modules.mask import subsequent_n_mask
-from funasr.train.abs_model import AbsPunctuation
 
 
-class TargetDelayTransformer(AbsPunctuation):
+class TargetDelayTransformer(torch.nn.Module):
     """
     Author: Speech Lab of DAMO Academy, Alibaba Group
     CT-Transformer: Controllable time-delay transformer for real-time punctuation prediction and disfluency detection
     https://arxiv.org/pdf/2003.01309.pdf
     """
     def __init__(
         self,
```

### Comparing `funasr-0.5.3/funasr/models/vad_realtime_transformer.py` & `funasr-0.5.4/funasr/models/vad_realtime_transformer.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 from typing import Tuple
 
 import torch
 import torch.nn as nn
 
 from funasr.modules.embedding import SinusoidalPositionEncoder
 from funasr.models.encoder.sanm_encoder import SANMVadEncoder as Encoder
-from funasr.train.abs_model import AbsPunctuation
 
 
-class VadRealtimeTransformer(AbsPunctuation):
+class VadRealtimeTransformer(torch.nn.Module):
     """
     Author: Speech Lab of DAMO Academy, Alibaba Group
     CT-Transformer: Controllable time-delay transformer for real-time punctuation prediction and disfluency detection
     https://arxiv.org/pdf/2003.01309.pdf
     """
     def __init__(
         self,
```

### Comparing `funasr-0.5.3/funasr/modules/add_sos_eos.py` & `funasr-0.5.4/funasr/modules/add_sos_eos.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/attention.py` & `funasr-0.5.4/funasr/modules/attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/beam_search/batch_beam_search.py` & `funasr-0.5.4/funasr/modules/beam_search/batch_beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/beam_search/batch_beam_search_online_sim.py` & `funasr-0.5.4/funasr/modules/beam_search/batch_beam_search_online_sim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/beam_search/beam_search.py` & `funasr-0.5.4/funasr/modules/beam_search/beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/beam_search/beam_search_sa_asr.py` & `funasr-0.5.4/funasr/modules/beam_search/beam_search_sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/beam_search/beam_search_transducer.py` & `funasr-0.5.4/funasr/modules/beam_search/beam_search_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/data2vec/data_utils.py` & `funasr-0.5.4/funasr/modules/data2vec/data_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/data2vec/ema_module.py` & `funasr-0.5.4/funasr/modules/data2vec/ema_module.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/data2vec/quant_noise.py` & `funasr-0.5.4/funasr/modules/data2vec/quant_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/data2vec/utils.py` & `funasr-0.5.4/funasr/modules/data2vec/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/data2vec/wav2vec2.py` & `funasr-0.5.4/funasr/modules/data2vec/wav2vec2.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/dynamic_conv.py` & `funasr-0.5.4/funasr/modules/dynamic_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/dynamic_conv2d.py` & `funasr-0.5.4/funasr/modules/dynamic_conv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/e2e_asr_common.py` & `funasr-0.5.4/funasr/modules/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/eend_ola/encoder.py` & `funasr-0.5.4/funasr/modules/eend_ola/encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/eend_ola/encoder_decoder_attractor.py` & `funasr-0.5.4/funasr/modules/eend_ola/encoder_decoder_attractor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/embedding.py` & `funasr-0.5.4/funasr/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/frontends/beamformer.py` & `funasr-0.5.4/funasr/modules/frontends/beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/frontends/dnn_beamformer.py` & `funasr-0.5.4/funasr/modules/frontends/dnn_beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/frontends/dnn_wpe.py` & `funasr-0.5.4/funasr/modules/frontends/dnn_wpe.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/frontends/feature_transform.py` & `funasr-0.5.4/funasr/modules/frontends/feature_transform.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/frontends/frontend.py` & `funasr-0.5.4/funasr/modules/frontends/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/frontends/mask_estimator.py` & `funasr-0.5.4/funasr/modules/frontends/mask_estimator.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/layer_norm.py` & `funasr-0.5.4/funasr/modules/layer_norm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/lightconv.py` & `funasr-0.5.4/funasr/modules/lightconv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/lightconv2d.py` & `funasr-0.5.4/funasr/modules/lightconv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/mask.py` & `funasr-0.5.4/funasr/modules/mask.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/multi_layer_conv.py` & `funasr-0.5.4/funasr/modules/multi_layer_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/nets_utils.py` & `funasr-0.5.4/funasr/modules/nets_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/positionwise_feed_forward.py` & `funasr-0.5.4/funasr/modules/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/repeat.py` & `funasr-0.5.4/funasr/modules/repeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/rnn/argument.py` & `funasr-0.5.4/funasr/modules/rnn/argument.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/rnn/attentions.py` & `funasr-0.5.4/funasr/modules/rnn/attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/rnn/decoders.py` & `funasr-0.5.4/funasr/modules/rnn/decoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/rnn/encoders.py` & `funasr-0.5.4/funasr/modules/rnn/encoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/scorers/ctc.py` & `funasr-0.5.4/funasr/modules/scorers/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/scorers/ctc_prefix_score.py` & `funasr-0.5.4/funasr/modules/scorers/ctc_prefix_score.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/scorers/length_bonus.py` & `funasr-0.5.4/funasr/modules/scorers/length_bonus.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/scorers/scorer_interface.py` & `funasr-0.5.4/funasr/modules/scorers/scorer_interface.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/streaming_utils/chunk_utilis.py` & `funasr-0.5.4/funasr/modules/streaming_utils/chunk_utilis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/streaming_utils/load_fr_tf.py` & `funasr-0.5.4/funasr/modules/streaming_utils/load_fr_tf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/streaming_utils/utils.py` & `funasr-0.5.4/funasr/modules/streaming_utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/subsampling.py` & `funasr-0.5.4/funasr/modules/subsampling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/modules/subsampling_without_posenc.py` & `funasr-0.5.4/funasr/modules/subsampling_without_posenc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/optimizers/fairseq_adam.py` & `funasr-0.5.4/funasr/optimizers/fairseq_adam.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/optimizers/sgd.py` & `funasr-0.5.4/funasr/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/runtime/python/libtorch/demo.py` & `funasr-0.5.4/funasr/runtime/python/libtorch/demo.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py` & `funasr-0.5.4/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py` & `funasr-0.5.4/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py` & `funasr-0.5.4/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py` & `funasr-0.5.4/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py` & `funasr-0.5.4/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py` & `funasr-0.5.4/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/runtime/python/libtorch/setup.py` & `funasr-0.5.4/funasr/runtime/python/libtorch/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py` & `funasr-0.5.4/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/runtime/python/onnxruntime/demo_punc_offline.py` & `funasr-0.5.4/funasr/runtime/python/onnxruntime/demo_punc_offline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/runtime/python/onnxruntime/demo_punc_online.py` & `funasr-0.5.4/funasr/runtime/python/onnxruntime/demo_punc_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/runtime/python/onnxruntime/demo_vad_online.py` & `funasr-0.5.4/funasr/runtime/python/onnxruntime/demo_vad_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py` & `funasr-0.5.4/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py` & `funasr-0.5.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py` & `funasr-0.5.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py` & `funasr-0.5.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py` & `funasr-0.5.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py` & `funasr-0.5.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py` & `funasr-0.5.4/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/runtime/python/onnxruntime/setup.py` & `funasr-0.5.4/funasr/runtime/python/onnxruntime/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/samplers/build_batch_sampler.py` & `funasr-0.5.4/funasr/samplers/build_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/samplers/folded_batch_sampler.py` & `funasr-0.5.4/funasr/samplers/folded_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/samplers/length_batch_sampler.py` & `funasr-0.5.4/funasr/samplers/length_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/samplers/num_elements_batch_sampler.py` & `funasr-0.5.4/funasr/samplers/num_elements_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/samplers/sorted_batch_sampler.py` & `funasr-0.5.4/funasr/samplers/sorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/samplers/unsorted_batch_sampler.py` & `funasr-0.5.4/funasr/samplers/unsorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/schedulers/abs_scheduler.py` & `funasr-0.5.4/funasr/schedulers/abs_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/schedulers/noam_lr.py` & `funasr-0.5.4/funasr/schedulers/noam_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/schedulers/tri_stage_scheduler.py` & `funasr-0.5.4/funasr/schedulers/tri_stage_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/schedulers/warmup_lr.py` & `funasr-0.5.4/funasr/schedulers/warmup_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/tasks/abs_task.py` & `funasr-0.5.4/funasr/tasks/abs_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,41 +26,41 @@
 import numpy as np
 import torch
 import torch.distributed as dist
 import torch.multiprocessing
 import torch.nn
 import torch.optim
 import yaml
+from funasr.models.base_model import FunASRModel
 from torch.utils.data import DataLoader
 from typeguard import check_argument_types
 from typeguard import check_return_type
 
 from funasr import __version__
 from funasr.datasets.dataset import AbsDataset
 from funasr.datasets.dataset import DATA_TYPES
 from funasr.datasets.dataset import ESPnetDataset
 from funasr.datasets.iterable_dataset import IterableESPnetDataset
 from funasr.iterators.abs_iter_factory import AbsIterFactory
 from funasr.iterators.chunk_iter_factory import ChunkIterFactory
 from funasr.iterators.multiple_iter_factory import MultipleIterFactory
 from funasr.iterators.sequence_iter_factory import SequenceIterFactory
 from funasr.main_funcs.collect_stats import collect_stats
-from funasr.optimizers.sgd import SGD
 from funasr.optimizers.fairseq_adam import FairseqAdam
+from funasr.optimizers.sgd import SGD
 from funasr.samplers.build_batch_sampler import BATCH_TYPES
 from funasr.samplers.build_batch_sampler import build_batch_sampler
 from funasr.samplers.unsorted_batch_sampler import UnsortedBatchSampler
 from funasr.schedulers.noam_lr import NoamLR
-from funasr.schedulers.warmup_lr import WarmupLR
 from funasr.schedulers.tri_stage_scheduler import TriStageLR
+from funasr.schedulers.warmup_lr import WarmupLR
 from funasr.torch_utils.load_pretrained_model import load_pretrained_model
 from funasr.torch_utils.model_summary import model_summary
 from funasr.torch_utils.pytorch_version import pytorch_cudnn_version
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
-from funasr.train.abs_espnet_model import AbsESPnetModel
 from funasr.train.class_choices import ClassChoices
 from funasr.train.distributed_utils import DistributedOption
 from funasr.train.trainer import Trainer
 from funasr.utils import config_argparse
 from funasr.utils.build_dataclass import build_dataclass
 from funasr.utils.cli_utils import get_commandline_args
 from funasr.utils.get_default_kwargs import get_default_kwargs
@@ -226,16 +226,16 @@
     ) -> Tuple[str, ...]:
         """Define the required names by Task
 
         This function is used by
         >>> cls.check_task_requirements()
         If your model is defined as following,
 
-        >>> from funasr.train.abs_espnet_model import AbsESPnetModel
-        >>> class Model(AbsESPnetModel):
+        >>> from funasr.models.base_model import FunASRModel
+        >>> class Model(FunASRModel):
         ...     def forward(self, input, output, opt=None):  pass
 
         then "required_data_names" should be as
 
         >>> required_data_names = ('input', 'output')
         """
         raise NotImplementedError
@@ -247,29 +247,30 @@
     ) -> Tuple[str, ...]:
         """Define the optional names by Task
 
         This function is used by
         >>> cls.check_task_requirements()
         If your model is defined as follows,
 
-        >>> from funasr.train.abs_espnet_model import AbsESPnetModel
-        >>> class Model(AbsESPnetModel):
+        >>> from funasr.models.base_model import FunASRModel
+        >>> class Model(FunASRModel):
         ...     def forward(self, input, output, opt=None):  pass
 
         then "optional_data_names" should be as
 
         >>> optional_data_names = ('opt',)
         """
         raise NotImplementedError
 
     @classmethod
     @abstractmethod
-    def build_model(cls, args: argparse.Namespace) -> AbsESPnetModel:
+    def build_model(cls, args: argparse.Namespace) -> FunASRModel:
         raise NotImplementedError
 
+
     @classmethod
     def get_parser(cls) -> config_argparse.ArgumentParser:
         assert check_argument_types()
 
         class ArgumentDefaultsRawTextHelpFormatter(
             argparse.RawTextHelpFormatter,
             argparse.ArgumentDefaultsHelpFormatter,
@@ -1168,25 +1169,28 @@
             if args.dataset_type == "small" and args.ngpu > 0:
                 if args.batch_size is not None:
                     args.batch_size = args.batch_size * args.ngpu
                 if args.batch_bins is not None and args.ngpu > 0:
                     args.batch_bins = args.batch_bins * args.ngpu
 
         # filter samples if wav.scp and text are mismatch
-        if (args.train_shape_file is None and args.dataset_type == "small") or args.train_data_file is None and args.dataset_type == "large":
+        if (
+                args.train_shape_file is None and args.dataset_type == "small") or args.train_data_file is None and args.dataset_type == "large":
             if not args.simple_ddp or distributed_option.dist_rank == 0:
                 filter_wav_text(args.data_dir, args.train_set)
                 filter_wav_text(args.data_dir, args.dev_set)
             if args.simple_ddp:
                 dist.barrier()
 
         if args.train_shape_file is None and args.dataset_type == "small":
             if not args.simple_ddp or distributed_option.dist_rank == 0:
-                calc_shape(args.data_dir, args.train_set, args.frontend_conf, args.speech_length_min, args.speech_length_max)
-                calc_shape(args.data_dir, args.dev_set, args.frontend_conf, args.speech_length_min, args.speech_length_max)
+                calc_shape(args.data_dir, args.train_set, args.frontend_conf, args.speech_length_min,
+                           args.speech_length_max)
+                calc_shape(args.data_dir, args.dev_set, args.frontend_conf, args.speech_length_min,
+                           args.speech_length_max)
             if args.simple_ddp:
                 dist.barrier()
             args.train_shape_file = [os.path.join(args.data_dir, args.train_set, "speech_shape")]
             args.valid_shape_file = [os.path.join(args.data_dir, args.dev_set, "speech_shape")]
 
         if args.train_data_file is None and args.dataset_type == "large":
             if not args.simple_ddp or distributed_option.dist_rank == 0:
@@ -1240,17 +1244,17 @@
         torch.backends.cudnn.deterministic = args.cudnn_deterministic
         if args.detect_anomaly:
             logging.info("Invoking torch.autograd.set_detect_anomaly(True)")
             torch.autograd.set_detect_anomaly(args.detect_anomaly)
 
         # 2. Build model
         model = cls.build_model(args=args)
-        if not isinstance(model, AbsESPnetModel):
+        if not isinstance(model, FunASRModel):
             raise RuntimeError(
-                f"model must inherit {AbsESPnetModel.__name__}, but got {type(model)}"
+                f"model must inherit {FunASRModel.__name__}, but got {type(model)}"
             )
         model = model.to(
             dtype=getattr(torch, args.train_dtype),
             device="cuda" if args.ngpu > 0 else "cpu",
         )
         for t in args.freeze_param:
             for k, p in model.named_parameters():
@@ -1370,23 +1374,29 @@
                     oss_bucket=args.oss_bucket,
                 )
 
             # 7. Build iterator factories
             if args.dataset_type == "large":
                 from funasr.datasets.large_datasets.build_dataloader import ArkDataLoader
                 train_iter_factory = ArkDataLoader(args.train_data_file, args.token_list, args.dataset_conf,
-                                                   frontend_conf=args.frontend_conf if hasattr(args, "frontend_conf") else None,
-                                                   seg_dict_file=args.seg_dict_file if hasattr(args, "seg_dict_file") else None,
-                                                   punc_dict_file=args.punc_list if hasattr(args, "punc_list") else None,
+                                                   frontend_conf=args.frontend_conf if hasattr(args,
+                                                                                               "frontend_conf") else None,
+                                                   seg_dict_file=args.seg_dict_file if hasattr(args,
+                                                                                               "seg_dict_file") else None,
+                                                   punc_dict_file=args.punc_list if hasattr(args,
+                                                                                            "punc_list") else None,
                                                    bpemodel_file=args.bpemodel if hasattr(args, "bpemodel") else None,
                                                    mode="train")
-                valid_iter_factory = ArkDataLoader(args.valid_data_file, args.token_list, args.dataset_conf, 
-                                                   frontend_conf=args.frontend_conf if hasattr(args, "frontend_conf") else None,
-                                                   seg_dict_file=args.seg_dict_file if hasattr(args, "seg_dict_file") else None,
-                                                   punc_dict_file=args.punc_list if hasattr(args, "punc_list") else None,
+                valid_iter_factory = ArkDataLoader(args.valid_data_file, args.token_list, args.dataset_conf,
+                                                   frontend_conf=args.frontend_conf if hasattr(args,
+                                                                                               "frontend_conf") else None,
+                                                   seg_dict_file=args.seg_dict_file if hasattr(args,
+                                                                                               "seg_dict_file") else None,
+                                                   punc_dict_file=args.punc_list if hasattr(args,
+                                                                                            "punc_list") else None,
                                                    bpemodel_file=args.bpemodel if hasattr(args, "bpemodel") else None,
                                                    mode="eval")
             elif args.dataset_type == "small":
                 train_iter_factory = cls.build_iter_factory(
                     args=args,
                     distributed_option=distributed_option,
                     mode="train",
@@ -1925,15 +1935,15 @@
     @classmethod
     def build_model_from_file(
             cls,
             config_file: Union[Path, str] = None,
             model_file: Union[Path, str] = None,
             cmvn_file: Union[Path, str] = None,
             device: str = "cpu",
-    ) -> Tuple[AbsESPnetModel, argparse.Namespace]:
+    ) -> Tuple[FunASRModel, argparse.Namespace]:
         """Build model from the files.
 
         This method is used for inference or fine-tuning.
 
         Args:
             config_file: The yaml file saved when training.
             model_file: The model file saved when training.
@@ -1952,17 +1962,17 @@
 
         with config_file.open("r", encoding="utf-8") as f:
             args = yaml.safe_load(f)
         if cmvn_file is not None:
             args["cmvn_file"] = cmvn_file
         args = argparse.Namespace(**args)
         model = cls.build_model(args)
-        if not isinstance(model, AbsESPnetModel):
+        if not isinstance(model, FunASRModel):
             raise RuntimeError(
-                f"model must inherit {AbsESPnetModel.__name__}, but got {type(model)}"
+                f"model must inherit {FunASRModel.__name__}, but got {type(model)}"
             )
         model.to(device)
         if model_file is not None:
             if device == "cuda":
                 # NOTE(kamo): "cuda" for torch.load always indicates cuda:0
                 #   in PyTorch<=1.4
                 device = f"cuda:{torch.cuda.current_device()}"
```

### Comparing `funasr-0.5.3/funasr/tasks/asr.py` & `funasr-0.5.4/funasr/tasks/asr.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 )
 from funasr.models.decoder.transformer_decoder import (
     LightweightConvolutionTransformerDecoder,  # noqa: H301
 )
 from funasr.models.decoder.transformer_decoder import ParaformerDecoderSAN
 from funasr.models.decoder.transformer_decoder import TransformerDecoder
 from funasr.models.decoder.contextual_decoder import ContextualParaformerDecoder
+from funasr.models.e2e_asr import ASRModel
 from funasr.models.decoder.rnnt_decoder import RNNTDecoder
 from funasr.models.joint_net.joint_network import JointNetwork
-from funasr.models.e2e_asr import ESPnetASRModel
 from funasr.models.e2e_asr_paraformer import Paraformer, ParaformerOnline, ParaformerBert, BiCifParaformer, ContextualParaformer
 from funasr.models.e2e_asr_contextual_paraformer import NeatContextualParaformer
 from funasr.models.e2e_tp import TimestampPredictor
 from funasr.models.e2e_asr_mfcca import MFCCA
 from funasr.models.e2e_uni_asr import UniASR
 from funasr.models.e2e_asr_transducer import TransducerModel, UnifiedTransducerModel
 from funasr.models.encoder.abs_encoder import AbsEncoder
@@ -72,15 +72,15 @@
 from funasr.models.specaug.abs_specaug import AbsSpecAug
 from funasr.models.specaug.specaug import SpecAug
 from funasr.models.specaug.specaug import SpecAugLFR
 from funasr.modules.subsampling import Conv1dSubsampling
 from funasr.tasks.abs_task import AbsTask
 from funasr.text.phoneme_tokenizer import g2p_choices
 from funasr.torch_utils.initialize import initialize
-from funasr.train.abs_espnet_model import AbsESPnetModel
+from funasr.models.base_model import FunASRModel
 from funasr.train.class_choices import ClassChoices
 from funasr.train.trainer import Trainer
 from funasr.utils.get_default_kwargs import get_default_kwargs
 from funasr.utils.nested_dict_action import NestedDictAction
 from funasr.utils.types import float_or_none
 from funasr.utils.types import int_or_none
 from funasr.utils.types import str2bool
@@ -118,26 +118,28 @@
     type_check=AbsNormalize,
     default=None,
     optional=True,
 )
 model_choices = ClassChoices(
     "model",
     classes=dict(
-        asr=ESPnetASRModel,
+        asr=ASRModel,
         uniasr=UniASR,
         paraformer=Paraformer,
         paraformer_online=ParaformerOnline,
         paraformer_bert=ParaformerBert,
         bicif_paraformer=BiCifParaformer,
         contextual_paraformer=ContextualParaformer,
         neatcontextual_paraformer=NeatContextualParaformer,
         mfcca=MFCCA,
         timestamp_prediction=TimestampPredictor,
+        rnnt=TransducerModel,
+        rnnt_unified=UnifiedTransducerModel,
     ),
-    type_check=AbsESPnetModel,
+    type_check=FunASRModel,
     default="asr",
 )
 preencoder_choices = ClassChoices(
     name="preencoder",
     classes=dict(
         sinc=LightweightSincConvs,
         linear=LinearProjection,
@@ -220,14 +222,23 @@
     classes=dict(
         rnnt=RNNTDecoder,
     ),
     type_check=RNNTDecoder,
     default="rnnt",
 )
 
+joint_network_choices = ClassChoices(
+    name="joint_network",
+    classes=dict(
+        joint_network=JointNetwork,
+    ),
+    default="joint_network",
+    optional=True,
+)
+
 predictor_choices = ClassChoices(
     name="predictor",
     classes=dict(
         cif_predictor=CifPredictor,
         ctc_predictor=None,
         cif_predictor_v2=CifPredictorV2,
         cif_predictor_v3=CifPredictorV3,
@@ -276,14 +287,26 @@
         preencoder_choices,
         # --encoder and --encoder_conf
         encoder_choices,
         # --postencoder and --postencoder_conf
         postencoder_choices,
         # --decoder and --decoder_conf
         decoder_choices,
+        # --predictor and --predictor_conf
+        predictor_choices,
+        # --encoder2 and --encoder2_conf
+        encoder_choices2,
+        # --decoder2 and --decoder2_conf
+        decoder_choices2,
+        # --predictor2 and --predictor2_conf
+        predictor_choices2,
+        # --stride_conv and --stride_conv_conf
+        stride_conv_choices,
+        # --rnnt_decoder and --rnnt_decoder_conf
+        rnnt_decoder_choices,
     ]
 
     # If you need to modify train() or eval() procedures, change Trainer class here
     trainer = Trainer
 
     @classmethod
     def add_task_arguments(cls, parser: argparse.ArgumentParser):
@@ -337,15 +360,15 @@
         group.add_argument(
             "--ctc_conf",
             action=NestedDictAction,
             default=get_default_kwargs(CTC),
             help="The keyword arguments for CTC class.",
         )
         group.add_argument(
-            "--joint_net_conf",
+            "--joint_network_conf",
             action=NestedDictAction,
             default=None,
             help="The keyword arguments for joint network class.",
         )
 
         group = parser.add_argument_group(description="Preprocess related")
         group.add_argument(
@@ -453,15 +476,15 @@
         assert check_argument_types()
         if args.use_preprocessor:
             retval = CommonPreprocessor(
                 train=train,
                 token_type=args.token_type,
                 token_list=args.token_list,
                 bpemodel=args.bpemodel,
-                non_linguistic_symbols=args.non_linguistic_symbols,
+                non_linguistic_symbols=args.non_linguistic_symbols if hasattr(args, "non_linguistic_symbols") else None,
                 text_cleaner=args.cleaner,
                 g2p_type=args.g2p,
                 split_with_space=args.split_with_space if hasattr(args, "split_with_space") else False,
                 seg_dict_file=args.seg_dict_file if hasattr(args, "seg_dict_file") else None,
                 # NOTE(kamo): Check attribute existence for backward compatibility
                 rir_scp=args.rir_scp if hasattr(args, "rir_scp") else None,
                 rir_apply_prob=args.rir_apply_prob
@@ -823,17 +846,17 @@
 
         with config_file.open("r", encoding="utf-8") as f:
             args = yaml.safe_load(f)
         if cmvn_file is not None:
             args["cmvn_file"] = cmvn_file
         args = argparse.Namespace(**args)
         model = cls.build_model(args)
-        if not isinstance(model, AbsESPnetModel):
+        if not isinstance(model, FunASRModel):
             raise RuntimeError(
-                f"model must inherit {AbsESPnetModel.__name__}, but got {type(model)}"
+                f"model must inherit {FunASRModel.__name__}, but got {type(model)}"
             )
         model.to(device)
         model_dict = dict()
         model_name_pth = None
         if model_file is not None:
             logging.info("model_file is {}".format(model_file))
             if device == "cuda":
@@ -895,35 +918,35 @@
         return var_dict_torch_update
 
 
 class ASRTaskParaformer(ASRTask):
     # If you need more than one optimizers, change this value
     num_optimizers: int = 1
 
-    # Add variable objects configurations
-    class_choices_list = [
-        # --frontend and --frontend_conf
-        frontend_choices,
-        # --specaug and --specaug_conf
-        specaug_choices,
-        # --normalize and --normalize_conf
-        normalize_choices,
-        # --model and --model_conf
-        model_choices,
-        # --preencoder and --preencoder_conf
-        preencoder_choices,
-        # --encoder and --encoder_conf
-        encoder_choices,
-        # --postencoder and --postencoder_conf
-        postencoder_choices,
-        # --decoder and --decoder_conf
-        decoder_choices,
-        # --predictor and --predictor_conf
-        predictor_choices,
-    ]
+    # # Add variable objects configurations
+    # class_choices_list = [
+    #     # --frontend and --frontend_conf
+    #     frontend_choices,
+    #     # --specaug and --specaug_conf
+    #     specaug_choices,
+    #     # --normalize and --normalize_conf
+    #     normalize_choices,
+    #     # --model and --model_conf
+    #     model_choices,
+    #     # --preencoder and --preencoder_conf
+    #     preencoder_choices,
+    #     # --encoder and --encoder_conf
+    #     encoder_choices,
+    #     # --postencoder and --postencoder_conf
+    #     postencoder_choices,
+    #     # --decoder and --decoder_conf
+    #     decoder_choices,
+    #     # --predictor and --predictor_conf
+    #     predictor_choices,
+    # ]
 
     # If you need to modify train() or eval() procedures, change Trainer class here
     trainer = Trainer
 
     @classmethod
     def build_model(cls, args: argparse.Namespace):
         assert check_argument_types()
@@ -1070,17 +1093,17 @@
 
         with config_file.open("r", encoding="utf-8") as f:
             args = yaml.safe_load(f)
         if cmvn_file is not None:
             args["cmvn_file"] = cmvn_file
         args = argparse.Namespace(**args)
         model = cls.build_model(args)
-        if not isinstance(model, AbsESPnetModel):
+        if not isinstance(model, FunASRModel):
             raise RuntimeError(
-                f"model must inherit {AbsESPnetModel.__name__}, but got {type(model)}"
+                f"model must inherit {FunASRModel.__name__}, but got {type(model)}"
             )
         model.to(device)
         model_dict = dict()
         model_name_pth = None
         if model_file is not None:
             logging.info("model_file is {}".format(model_file))
             if device == "cuda":
@@ -1346,264 +1369,31 @@
     def required_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         retval = ("speech", "text")
         return retval
 
 
-class ASRTransducerTask(AbsTask):
+class ASRTransducerTask(ASRTask):
     """ASR Transducer Task definition."""
 
     num_optimizers: int = 1
 
     class_choices_list = [
         frontend_choices,
         specaug_choices,
         normalize_choices,
         encoder_choices,
         rnnt_decoder_choices,
+        joint_network_choices,
     ]
 
     trainer = Trainer
 
     @classmethod
-    def add_task_arguments(cls, parser: argparse.ArgumentParser):
-        """Add Transducer task arguments.
-        Args:
-            cls: ASRTransducerTask object.
-            parser: Transducer arguments parser.
-        """
-        group = parser.add_argument_group(description="Task related.")
-
-        # required = parser.get_default("required")
-        # required += ["token_list"]
-
-        group.add_argument(
-            "--token_list",
-            type=str_or_none,
-            default=None,
-            help="Integer-string mapper for tokens.",
-        )
-        group.add_argument(
-            "--split_with_space",
-            type=str2bool,
-            default=True,
-            help="whether to split text using <space>",
-        )
-        group.add_argument(
-            "--input_size",
-            type=int_or_none,
-            default=None,
-            help="The number of dimensions for input features.",
-        )
-        group.add_argument(
-            "--init",
-            type=str_or_none,
-            default=None,
-            help="Type of model initialization to use.",
-        )
-        group.add_argument(
-            "--model_conf",
-            action=NestedDictAction,
-            default=get_default_kwargs(TransducerModel),
-            help="The keyword arguments for the model class.",
-        )
-        # group.add_argument(
-        #     "--encoder_conf",
-        #     action=NestedDictAction,
-        #     default={},
-        #     help="The keyword arguments for the encoder class.",
-        # )
-        group.add_argument(
-            "--joint_network_conf",
-            action=NestedDictAction,
-            default={},
-            help="The keyword arguments for the joint network class.",
-        )
-        group = parser.add_argument_group(description="Preprocess related.")
-        group.add_argument(
-            "--use_preprocessor",
-            type=str2bool,
-            default=True,
-            help="Whether to apply preprocessing to input data.",
-        )
-        group.add_argument(
-            "--token_type",
-            type=str,
-            default="bpe",
-            choices=["bpe", "char", "word", "phn"],
-            help="The type of tokens to use during tokenization.",
-        )
-        group.add_argument(
-            "--bpemodel",
-            type=str_or_none,
-            default=None,
-            help="The path of the sentencepiece model.",
-        )
-        parser.add_argument(
-            "--non_linguistic_symbols",
-            type=str_or_none,
-            help="The 'non_linguistic_symbols' file path.",
-        )
-        parser.add_argument(
-            "--cleaner",
-            type=str_or_none,
-            choices=[None, "tacotron", "jaconv", "vietnamese"],
-            default=None,
-            help="Text cleaner to use.",
-        )
-        parser.add_argument(
-            "--g2p",
-            type=str_or_none,
-            choices=g2p_choices,
-            default=None,
-            help="g2p method to use if --token_type=phn.",
-        )
-        parser.add_argument(
-            "--speech_volume_normalize",
-            type=float_or_none,
-            default=None,
-            help="Normalization value for maximum amplitude scaling.",
-        )
-        parser.add_argument(
-            "--rir_scp",
-            type=str_or_none,
-            default=None,
-            help="The RIR SCP file path.",
-        )
-        parser.add_argument(
-            "--rir_apply_prob",
-            type=float,
-            default=1.0,
-            help="The probability of the applied RIR convolution.",
-        )
-        parser.add_argument(
-            "--noise_scp",
-            type=str_or_none,
-            default=None,
-            help="The path of noise SCP file.",
-        )
-        parser.add_argument(
-            "--noise_apply_prob",
-            type=float,
-            default=1.0,
-            help="The probability of the applied noise addition.",
-        )
-        parser.add_argument(
-            "--noise_db_range",
-            type=str,
-            default="13_15",
-            help="The range of the noise decibel level.",
-        )
-        for class_choices in cls.class_choices_list:
-            # Append --<name> and --<name>_conf.
-            # e.g. --decoder and --decoder_conf
-            class_choices.add_arguments(group)
-
-    @classmethod
-    def build_collate_fn(
-        cls, args: argparse.Namespace, train: bool
-    ) -> Callable[
-        [Collection[Tuple[str, Dict[str, np.ndarray]]]],
-        Tuple[List[str], Dict[str, torch.Tensor]],
-    ]:
-        """Build collate function.
-        Args:
-            cls: ASRTransducerTask object.
-            args: Task arguments.
-            train: Training mode.
-        Return:
-            : Callable collate function.
-        """
-        assert check_argument_types()
-
-        return CommonCollateFn(float_pad_value=0.0, int_pad_value=-1)
-
-    @classmethod
-    def build_preprocess_fn(
-        cls, args: argparse.Namespace, train: bool
-    ) -> Optional[Callable[[str, Dict[str, np.array]], Dict[str, np.ndarray]]]:
-        """Build pre-processing function.
-        Args:
-            cls: ASRTransducerTask object.
-            args: Task arguments.
-            train: Training mode.
-        Return:
-            : Callable pre-processing function.
-        """
-        assert check_argument_types()
-
-        if args.use_preprocessor:
-            retval = CommonPreprocessor(
-                train=train,
-                token_type=args.token_type,
-                token_list=args.token_list,
-                bpemodel=args.bpemodel,
-                non_linguistic_symbols=args.non_linguistic_symbols,
-                text_cleaner=args.cleaner,
-                g2p_type=args.g2p,
-                split_with_space=args.split_with_space if hasattr(args, "split_with_space") else False,
-                rir_scp=args.rir_scp if hasattr(args, "rir_scp") else None,
-                rir_apply_prob=args.rir_apply_prob
-                if hasattr(args, "rir_apply_prob")
-                else 1.0,
-                noise_scp=args.noise_scp if hasattr(args, "noise_scp") else None,
-                noise_apply_prob=args.noise_apply_prob
-                if hasattr(args, "noise_apply_prob")
-                else 1.0,
-                noise_db_range=args.noise_db_range
-                if hasattr(args, "noise_db_range")
-                else "13_15",
-                speech_volume_normalize=args.speech_volume_normalize
-                if hasattr(args, "rir_scp")
-                else None,
-            )
-        else:
-            retval = None
-
-        assert check_return_type(retval)
-        return retval
-
-    @classmethod
-    def required_data_names(
-        cls, train: bool = True, inference: bool = False
-    ) -> Tuple[str, ...]:
-        """Required data depending on task mode.
-        Args:
-            cls: ASRTransducerTask object.
-            train: Training mode.
-            inference: Inference mode.
-        Return:
-            retval: Required task data.
-        """
-        if not inference:
-            retval = ("speech", "text")
-        else:
-            retval = ("speech",)
-
-        return retval
-
-    @classmethod
-    def optional_data_names(
-        cls, train: bool = True, inference: bool = False
-    ) -> Tuple[str, ...]:
-        """Optional data depending on task mode.
-        Args:
-            cls: ASRTransducerTask object.
-            train: Training mode.
-            inference: Inference mode.
-        Return:
-            retval: Optional task data.
-        """
-        retval = ()
-        assert check_return_type(retval)
-
-        return retval
-
-    @classmethod
     def build_model(cls, args: argparse.Namespace) -> TransducerModel:
         """Required data depending on task mode.
         Args:
             cls: ASRTransducerTask object.
             args: Task arguments.
         Return:
             model: ASR Transducer model.
@@ -1661,15 +1451,15 @@
         decoder = rnnt_decoder_class(
             vocab_size,
             **args.rnnt_decoder_conf,
         )
         decoder_output_size = decoder.output_size
 
         if getattr(args, "decoder", None) is not None:
-            att_decoder_class = decoder_choices.get_class(args.att_decoder)
+            att_decoder_class = decoder_choices.get_class(args.decoder)
 
             att_decoder = att_decoder_class(
                 vocab_size=vocab_size,
                 encoder_output_size=encoder_output_size,
                 **args.decoder_conf,
             )
         else:
@@ -1679,43 +1469,31 @@
             vocab_size,
             encoder_output_size,
             decoder_output_size,
             **args.joint_network_conf,
         )
 
         # 7. Build model
+        try:
+            model_class = model_choices.get_class(args.model)
+        except AttributeError:
+            model_class = model_choices.get_class("asr")
 
-        if hasattr(encoder, 'unified_model_training') and encoder.unified_model_training:
-            model = UnifiedTransducerModel(
-                vocab_size=vocab_size,
-                token_list=token_list,
-                frontend=frontend,
-                specaug=specaug,
-                normalize=normalize,
-                encoder=encoder,
-                decoder=decoder,
-                att_decoder=att_decoder,
-                joint_network=joint_network,
-                **args.model_conf,
-            )
-
-        else:
-            model = TransducerModel(
-                vocab_size=vocab_size,
-                token_list=token_list,
-                frontend=frontend,
-                specaug=specaug,
-                normalize=normalize,
-                encoder=encoder,
-                decoder=decoder,
-                att_decoder=att_decoder,
-                joint_network=joint_network,
-                **args.model_conf,
-            )
-
+        model = model_class(
+            vocab_size=vocab_size,
+            token_list=token_list,
+            frontend=frontend,
+            specaug=specaug,
+            normalize=normalize,
+            encoder=encoder,
+            decoder=decoder,
+            att_decoder=att_decoder,
+            joint_network=joint_network,
+            **args.model_conf,
+        )
         # 8. Initialize model
         if args.init is not None:
             raise NotImplementedError(
                 "Currently not supported.",
                 "Initialization part will be reworked in a short future.",
             )
```

### Comparing `funasr-0.5.3/funasr/tasks/data2vec.py` & `funasr-0.5.4/funasr/tasks/vad.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,129 +1,123 @@
 import argparse
+import logging
+import os
+from pathlib import Path
 from typing import Callable
 from typing import Collection
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
+from typing import Union
 
 import numpy as np
 import torch
+import yaml
 from typeguard import check_argument_types
 from typeguard import check_return_type
 
 from funasr.datasets.collate_fn import CommonCollateFn
-from funasr.datasets.preprocessor import CommonPreprocessor
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.layers.global_mvn import GlobalMVN
 from funasr.layers.utterance_mvn import UtteranceMVN
-from funasr.models.data2vec import Data2VecPretrainModel
-from funasr.models.encoder.abs_encoder import AbsEncoder
-from funasr.models.encoder.data2vec_encoder import Data2VecEncoder
+from funasr.models.e2e_vad import E2EVadModel
+from funasr.models.encoder.fsmn_encoder import FSMN
 from funasr.models.frontend.abs_frontend import AbsFrontend
 from funasr.models.frontend.default import DefaultFrontend
+from funasr.models.frontend.fused import FusedFrontends
+from funasr.models.frontend.s3prl import S3prlFrontend
+from funasr.models.frontend.wav_frontend import WavFrontend, WavFrontendOnline
 from funasr.models.frontend.windowing import SlidingWindow
-from funasr.models.preencoder.abs_preencoder import AbsPreEncoder
-from funasr.models.preencoder.sinc import LightweightSincConvs
 from funasr.models.specaug.abs_specaug import AbsSpecAug
 from funasr.models.specaug.specaug import SpecAug
+from funasr.models.specaug.specaug import SpecAugLFR
 from funasr.tasks.abs_task import AbsTask
-from funasr.text.phoneme_tokenizer import g2p_choices
-from funasr.torch_utils.initialize import initialize
 from funasr.train.class_choices import ClassChoices
 from funasr.train.trainer import Trainer
 from funasr.utils.types import float_or_none
 from funasr.utils.types import int_or_none
-from funasr.utils.types import str2bool
 from funasr.utils.types import str_or_none
 
 frontend_choices = ClassChoices(
     name="frontend",
-    classes=dict(default=DefaultFrontend, sliding_window=SlidingWindow),
+    classes=dict(
+        default=DefaultFrontend,
+        sliding_window=SlidingWindow,
+        s3prl=S3prlFrontend,
+        fused=FusedFrontends,
+        wav_frontend=WavFrontend,
+        wav_frontend_online=WavFrontendOnline,
+    ),
     type_check=AbsFrontend,
     default="default",
 )
 specaug_choices = ClassChoices(
     name="specaug",
-    classes=dict(specaug=SpecAug),
+    classes=dict(
+        specaug=SpecAug,
+        specaug_lfr=SpecAugLFR,
+    ),
     type_check=AbsSpecAug,
     default=None,
     optional=True,
 )
 normalize_choices = ClassChoices(
     "normalize",
     classes=dict(
         global_mvn=GlobalMVN,
         utterance_mvn=UtteranceMVN,
     ),
     type_check=AbsNormalize,
     default=None,
     optional=True,
 )
-preencoder_choices = ClassChoices(
-    name="preencoder",
+model_choices = ClassChoices(
+    "model",
     classes=dict(
-        sinc=LightweightSincConvs,
+        e2evad=E2EVadModel,
     ),
-    type_check=AbsPreEncoder,
-    default=None,
-    optional=True,
+    type_check=object,
+    default="e2evad",
 )
+
 encoder_choices = ClassChoices(
     "encoder",
     classes=dict(
-        data2vec_encoder=Data2VecEncoder,
+        fsmn=FSMN,
     ),
-    type_check=AbsEncoder,
-    default="data2vec_encoder",
-)
-model_choices = ClassChoices(
-    "model",
-    classes=dict(
-        data2vec=Data2VecPretrainModel,
-    ),
-    default="data2vec",
+    type_check=torch.nn.Module,
+    default="fsmn",
 )
 
 
-class Data2VecTask(AbsTask):
+class VADTask(AbsTask):
     # If you need more than one optimizers, change this value
     num_optimizers: int = 1
 
     # Add variable objects configurations
     class_choices_list = [
         # --frontend and --frontend_conf
         frontend_choices,
-        # --specaug and --specaug_conf
-        specaug_choices,
-        # --normalize and --normalize_conf
-        normalize_choices,
-        # --preencoder and --preencoder_conf
-        preencoder_choices,
-        # --encoder and --encoder_conf
-        encoder_choices,
         # --model and --model_conf
         model_choices,
     ]
 
     # If you need to modify train() or eval() procedures, change Trainer class here
     trainer = Trainer
 
     @classmethod
     def add_task_arguments(cls, parser: argparse.ArgumentParser):
         group = parser.add_argument_group(description="Task related")
 
         # NOTE(kamo): add_arguments(..., required=True) can't be used
         # to provide --print_config mode. Instead of it, do as
-        group.add_argument(
-            "--token_list",
-            type=str_or_none,
-            default=None,
-            help="A text mapping int-id to token",
-        )
+        # required = parser.get_default("required")
+        # required += ["token_list"]
+
         group.add_argument(
             "--init",
             type=lambda x: str_or_none(x.lower()),
             default=None,
             help="The initialization method",
             choices=[
                 "chainer",
@@ -139,60 +133,14 @@
             "--input_size",
             type=int_or_none,
             default=None,
             help="The number of input dimension of the feature",
         )
 
         group = parser.add_argument_group(description="Preprocess related")
-        group.add_argument(
-            "--use_preprocessor",
-            type=str2bool,
-            default=True,
-            help="Apply preprocessing to data or not",
-        )
-        group.add_argument(
-            "--token_type",
-            type=str,
-            default=None,
-            choices=["bpe", "char", "word", "phn"],
-            help="The text will be tokenized " "in the specified level token",
-        )
-
-        group.add_argument(
-            "--feats_type",
-            type=str,
-            default='fbank',
-            help="feats type, e.g. fbank, wav, ark_wav(needed to be scale normalization)",
-        )
-
-        group.add_argument(
-            "--bpemodel",
-            type=str_or_none,
-            default=None,
-            help="The model file of sentencepiece",
-        )
-        parser.add_argument(
-            "--non_linguistic_symbols",
-            type=str_or_none,
-            help="non_linguistic_symbols file path",
-        )
-        parser.add_argument(
-            "--cleaner",
-            type=str_or_none,
-            choices=[None, "tacotron", "jaconv", "vietnamese"],
-            default=None,
-            help="Apply text cleaning",
-        )
-        parser.add_argument(
-            "--g2p",
-            type=str_or_none,
-            choices=g2p_choices,
-            default=None,
-            help="Specify g2p method if --token_type=phn",
-        )
         parser.add_argument(
             "--speech_volume_normalize",
             type=float_or_none,
             default=None,
             help="Scale the maximum amplitude to the given value.",
         )
         parser.add_argument(
@@ -204,14 +152,20 @@
         parser.add_argument(
             "--rir_apply_prob",
             type=float,
             default=1.0,
             help="THe probability for applying RIR convolution.",
         )
         parser.add_argument(
+            "--cmvn_file",
+            type=str_or_none,
+            default=None,
+            help="The file path of noise scp file.",
+        )
+        parser.add_argument(
             "--noise_scp",
             type=str_or_none,
             default=None,
             help="The file path of noise scp file.",
         )
         parser.add_argument(
             "--noise_apply_prob",
@@ -221,156 +175,154 @@
         )
         parser.add_argument(
             "--noise_db_range",
             type=str,
             default="13_15",
             help="The range of noise decibel level.",
         )
-        parser.add_argument(
-            "--pred_masked_weight",
-            type=float,
-            default=1.0,
-            help="weight for predictive loss for masked frames",
-        )
-        parser.add_argument(
-            "--pred_nomask_weight",
-            type=float,
-            default=0.0,
-            help="weight for predictive loss for unmasked frames",
-        )
-        parser.add_argument(
-            "--loss_weights",
-            type=float,
-            default=0.0,
-            help="weights for additional loss terms (not first one)",
-        )
 
         for class_choices in cls.class_choices_list:
             # Append --<name> and --<name>_conf.
             # e.g. --encoder and --encoder_conf
             class_choices.add_arguments(group)
 
     @classmethod
     def build_collate_fn(
             cls, args: argparse.Namespace, train: bool
     ) -> Callable[
         [Collection[Tuple[str, Dict[str, np.ndarray]]]],
         Tuple[List[str], Dict[str, torch.Tensor]],
     ]:
         assert check_argument_types()
-        return CommonCollateFn(clipping=True)
+        # NOTE(kamo): int value = 0 is reserved by CTC-blank symbol
+        return CommonCollateFn(float_pad_value=0.0, int_pad_value=-1)
 
     @classmethod
     def build_preprocess_fn(
             cls, args: argparse.Namespace, train: bool
     ) -> Optional[Callable[[str, Dict[str, np.array]], Dict[str, np.ndarray]]]:
         assert check_argument_types()
-        if args.use_preprocessor:
-            retval = CommonPreprocessor(
-                train=train,
-                bpemodel=args.bpemodel,
-                non_linguistic_symbols=args.non_linguistic_symbols,
-                text_cleaner=args.cleaner,
-                g2p_type=args.g2p,
-                # NOTE(kamo): Check attribute existence for backward compatibility
-                rir_scp=args.rir_scp if hasattr(args, "rir_scp") else None,
-                rir_apply_prob=args.rir_apply_prob
-                if hasattr(args, "rir_apply_prob")
-                else 1.0,
-                noise_scp=args.noise_scp if hasattr(args, "noise_scp") else None,
-                noise_apply_prob=args.noise_apply_prob
-                if hasattr(args, "noise_apply_prob")
-                else 1.0,
-                noise_db_range=args.noise_db_range
-                if hasattr(args, "noise_db_range")
-                else "13_15",
-                speech_volume_normalize=args.speech_volume_normalize
-                if hasattr(args, "rir_scp")
-                else None,
-            )
-        else:
-            retval = None
+        # if args.use_preprocessor:
+        #    retval = CommonPreprocessor(
+        #        train=train,
+        #        # NOTE(kamo): Check attribute existence for backward compatibility
+        #        rir_scp=args.rir_scp if hasattr(args, "rir_scp") else None,
+        #        rir_apply_prob=args.rir_apply_prob
+        #        if hasattr(args, "rir_apply_prob")
+        #        else 1.0,
+        #        noise_scp=args.noise_scp if hasattr(args, "noise_scp") else None,
+        #        noise_apply_prob=args.noise_apply_prob
+        #        if hasattr(args, "noise_apply_prob")
+        #        else 1.0,
+        #        noise_db_range=args.noise_db_range
+        #        if hasattr(args, "noise_db_range")
+        #        else "13_15",
+        #        speech_volume_normalize=args.speech_volume_normalize
+        #        if hasattr(args, "rir_scp")
+        #        else None,
+        #    )
+        # else:
+        #    retval = None
+        retval = None
         assert check_return_type(retval)
         return retval
 
     @classmethod
     def required_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
-        # for pre-training
-        retval = ("speech",)
+        if not inference:
+            retval = ("speech", "text")
+        else:
+            # Recognition mode
+            retval = ("speech",)
         return retval
 
     @classmethod
     def optional_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         retval = ()
         assert check_return_type(retval)
         return retval
 
     @classmethod
     def build_model(cls, args: argparse.Namespace):
         assert check_argument_types()
+        # 4. Encoder
+        encoder_class = encoder_choices.get_class(args.encoder)
+        encoder = encoder_class(**args.encoder_conf)
+
+        # 5. Build model
+        try:
+            model_class = model_choices.get_class(args.model)
+        except AttributeError:
+            model_class = model_choices.get_class("e2evad")
 
         # 1. frontend
         if args.input_size is None:
             # Extract features in the model
             frontend_class = frontend_choices.get_class(args.frontend)
-            frontend = frontend_class(**args.frontend_conf)
+            if args.frontend == 'wav_frontend':
+                frontend = frontend_class(cmvn_file=args.cmvn_file, **args.frontend_conf)
+            else:
+                frontend = frontend_class(**args.frontend_conf)
             input_size = frontend.output_size()
         else:
             # Give features from data-loader
             args.frontend = None
             args.frontend_conf = {}
             frontend = None
             input_size = args.input_size
 
-        # 2. Data augmentation for spectrogram
-        if args.specaug is not None:
-            specaug_class = specaug_choices.get_class(args.specaug)
-            specaug = specaug_class(**args.specaug_conf)
-        else:
-            specaug = None
+        model = model_class(encoder=encoder, vad_post_args=args.vad_post_conf, frontend=frontend)
 
-        # 3. Normalization layer
-        if args.normalize is not None:
-            normalize_class = normalize_choices.get_class(args.normalize)
-            normalize = normalize_class(**args.normalize_conf)
-        else:
-            normalize = None
-
-        # 4. Pre-encoder input block
-        # NOTE(kan-bayashi): Use getattr to keep the compatibility
-        if getattr(args, "preencoder", None) is not None:
-            preencoder_class = preencoder_choices.get_class(args.preencoder)
-            preencoder = preencoder_class(**args.preencoder_conf)
-            input_size = preencoder.output_size()
-        else:
-            preencoder = None
+        return model
 
-        # 5. Encoder
-        encoder_class = encoder_choices.get_class(args.encoder)
-        encoder = encoder_class(
-            input_size=input_size,
-            **args.encoder_conf,
-        )
+    # ~~~~~~~~~ The methods below are mainly used for inference ~~~~~~~~~
+    @classmethod
+    def build_model_from_file(
+            cls,
+            config_file: Union[Path, str] = None,
+            model_file: Union[Path, str] = None,
+            device: str = "cpu",
+            cmvn_file: Union[Path, str] = None,
+    ):
+        """Build model from the files.
+
+        This method is used for inference or fine-tuning.
+
+        Args:
+            config_file: The yaml file saved when training.
+            model_file: The model file saved when training.
+            device: Device type, "cpu", "cuda", or "cuda:N".
 
-        # 6. Build model
-        try:
-            model_class = model_choices.get_class(args.model)
-        except AttributeError:
-            model_class = model_choices.get_class("data2vec")
-        model = model_class(
-            frontend=frontend,
-            specaug=specaug,
-            normalize=normalize,
-            preencoder=preencoder,
-            encoder=encoder,
-        )
+        """
+        assert check_argument_types()
+        if config_file is None:
+            assert model_file is not None, (
+                "The argument 'model_file' must be provided "
+                "if the argument 'config_file' is not specified."
+            )
+            config_file = Path(model_file).parent / "config.yaml"
+        else:
+            config_file = Path(config_file)
 
-        # 7. Initialize
-        if args.init is not None:
-            initialize(model, args.init)
+        with config_file.open("r", encoding="utf-8") as f:
+            args = yaml.safe_load(f)
+        # if cmvn_file is not None:
+        args["cmvn_file"] = cmvn_file
+        args = argparse.Namespace(**args)
+        model = cls.build_model(args)
+        model.to(device)
+        model_dict = dict()
+        model_name_pth = None
+        if model_file is not None:
+            logging.info("model_file is {}".format(model_file))
+            if device == "cuda":
+                device = f"cuda:{torch.cuda.current_device()}"
+            model_dir = os.path.dirname(model_file)
+            model_name = os.path.basename(model_file)
+            model_dict = torch.load(model_file, map_location=device)
+        model.encoder.load_state_dict(model_dict)
 
-        assert check_return_type(model)
-        return model
+        return model, args
```

### Comparing `funasr-0.5.3/funasr/tasks/diar.py` & `funasr-0.5.4/funasr/tasks/diar.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 from funasr.models.specaug.abs_specaug import AbsSpecAug
 from funasr.models.specaug.specaug import SpecAug
 from funasr.models.specaug.specaug import SpecAugLFR
 from funasr.modules.eend_ola.encoder import EENDOLATransformerEncoder
 from funasr.modules.eend_ola.encoder_decoder_attractor import EncoderDecoderAttractor
 from funasr.tasks.abs_task import AbsTask
 from funasr.torch_utils.initialize import initialize
-from funasr.train.abs_espnet_model import AbsESPnetModel
+from funasr.models.base_model import FunASRModel
 from funasr.train.class_choices import ClassChoices
 from funasr.train.trainer import Trainer
 from funasr.utils.types import float_or_none
 from funasr.utils.types import int_or_none
 from funasr.utils.types import str2bool
 from funasr.utils.types import str_or_none
 
@@ -110,15 +110,15 @@
 )
 model_choices = ClassChoices(
     "model",
     classes=dict(
         sond=DiarSondModel,
         eend_ola=DiarEENDOLAModel,
     ),
-    type_check=AbsESPnetModel,
+    type_check=FunASRModel,
     default="sond",
 )
 encoder_choices = ClassChoices(
     "encoder",
     classes=dict(
         conformer=ConformerEncoder,
         transformer=TransformerEncoder,
@@ -540,17 +540,17 @@
 
         with config_file.open("r", encoding="utf-8") as f:
             args = yaml.safe_load(f)
         if cmvn_file is not None:
             args["cmvn_file"] = cmvn_file
         args = argparse.Namespace(**args)
         model = cls.build_model(args)
-        if not isinstance(model, AbsESPnetModel):
+        if not isinstance(model, FunASRModel):
             raise RuntimeError(
-                f"model must inherit {AbsESPnetModel.__name__}, but got {type(model)}"
+                f"model must inherit {FunASRModel.__name__}, but got {type(model)}"
             )
         model.to(device)
         model_dict = dict()
         model_name_pth = None
         if model_file is not None:
             logging.info("model_file is {}".format(model_file))
             if device == "cuda":
@@ -898,17 +898,17 @@
         else:
             config_file = Path(config_file)
 
         with config_file.open("r", encoding="utf-8") as f:
             args = yaml.safe_load(f)
         args = argparse.Namespace(**args)
         model = cls.build_model(args)
-        if not isinstance(model, AbsESPnetModel):
+        if not isinstance(model, FunASRModel):
             raise RuntimeError(
-                f"model must inherit {AbsESPnetModel.__name__}, but got {type(model)}"
+                f"model must inherit {FunASRModel.__name__}, but got {type(model)}"
             )
         if model_file is not None:
             if device == "cuda":
                 device = f"cuda:{torch.cuda.current_device()}"
             checkpoint = torch.load(model_file, map_location=device)
             if "state_dict" in checkpoint.keys():
                 model.load_state_dict(checkpoint["state_dict"])
```

### Comparing `funasr-0.5.3/funasr/tasks/lm.py` & `funasr-0.5.4/funasr/tasks/lm.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 import numpy as np
 import torch
 from typeguard import check_argument_types
 from typeguard import check_return_type
 
 from funasr.datasets.collate_fn import CommonCollateFn
 from funasr.datasets.preprocessor import CommonPreprocessor
-from funasr.lm.abs_model import AbsLM
-from funasr.lm.abs_model import LanguageModel
-from funasr.lm.seq_rnn_lm import SequentialRNNLM
-from funasr.lm.transformer_lm import TransformerLM
+from funasr.train.abs_model import AbsLM
+from funasr.train.abs_model import LanguageModel
+from funasr.models.seq_rnn_lm import SequentialRNNLM
+from funasr.models.transformer_lm import TransformerLM
 from funasr.tasks.abs_task import AbsTask
 from funasr.text.phoneme_tokenizer import g2p_choices
 from funasr.torch_utils.initialize import initialize
 from funasr.train.class_choices import ClassChoices
 from funasr.train.trainer import Trainer
 from funasr.utils.get_default_kwargs import get_default_kwargs
 from funasr.utils.nested_dict_action import NestedDictAction
@@ -202,10 +202,8 @@
         # 2. Build ESPnetModel
         # Assume the last-id is sos_and_eos
         model = LanguageModel(lm=lm, vocab_size=vocab_size, **args.model_conf)
 
         # 3. Initialize
         if args.init is not None:
             initialize(model, args.init)
-
-        assert check_return_type(model)
         return model
```

### Comparing `funasr-0.5.3/funasr/tasks/sa_asr.py` & `funasr-0.5.4/funasr/tasks/sa_asr.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,19 +66,19 @@
 from funasr.models.predictor.cif import CifPredictor, CifPredictorV2, CifPredictorV3
 from funasr.models.preencoder.abs_preencoder import AbsPreEncoder
 from funasr.models.preencoder.linear import LinearProjection
 from funasr.models.preencoder.sinc import LightweightSincConvs
 from funasr.models.specaug.abs_specaug import AbsSpecAug
 from funasr.models.specaug.specaug import SpecAug
 from funasr.models.specaug.specaug import SpecAugLFR
+from funasr.models.base_model import FunASRModel
 from funasr.modules.subsampling import Conv1dSubsampling
 from funasr.tasks.abs_task import AbsTask
 from funasr.text.phoneme_tokenizer import g2p_choices
 from funasr.torch_utils.initialize import initialize
-from funasr.train.abs_espnet_model import AbsESPnetModel
 from funasr.train.class_choices import ClassChoices
 from funasr.train.trainer import Trainer
 from funasr.utils.get_default_kwargs import get_default_kwargs
 from funasr.utils.nested_dict_action import NestedDictAction
 from funasr.utils.types import float_or_none
 from funasr.utils.types import int_or_none
 from funasr.utils.types import str2bool
@@ -125,15 +125,15 @@
         paraformer=Paraformer,
         paraformer_bert=ParaformerBert,
         bicif_paraformer=BiCifParaformer,
         contextual_paraformer=ContextualParaformer,
         mfcca=MFCCA,
         timestamp_prediction=TimestampPredictor,
     ),
-    type_check=AbsESPnetModel,
+    type_check=FunASRModel,
     default="asr",
 )
 preencoder_choices = ClassChoices(
     name="preencoder",
     classes=dict(
         sinc=LightweightSincConvs,
         linear=LinearProjection,
```

### Comparing `funasr-0.5.3/funasr/tasks/sv.py` & `funasr-0.5.4/funasr/tasks/sv.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from typeguard import check_return_type
 
 from funasr.datasets.collate_fn import CommonCollateFn
 from funasr.datasets.preprocessor import CommonPreprocessor
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.layers.global_mvn import GlobalMVN
 from funasr.layers.utterance_mvn import UtteranceMVN
-from funasr.models.e2e_asr import ESPnetASRModel
+from funasr.models.e2e_asr import ASRModel
 from funasr.models.decoder.abs_decoder import AbsDecoder
 from funasr.models.encoder.abs_encoder import AbsEncoder
 from funasr.models.encoder.rnn_encoder import RNNEncoder
 from funasr.models.encoder.resnet34_encoder import ResNet34, ResNet34_SP_L2Reg
 from funasr.models.pooling.statistic_pooling import StatisticPooling
 from funasr.models.decoder.sv_decoder import DenseDecoder
 from funasr.models.e2e_sv import ESPnetSVModel
@@ -45,15 +45,15 @@
 from funasr.models.preencoder.abs_preencoder import AbsPreEncoder
 from funasr.models.preencoder.linear import LinearProjection
 from funasr.models.preencoder.sinc import LightweightSincConvs
 from funasr.models.specaug.abs_specaug import AbsSpecAug
 from funasr.models.specaug.specaug import SpecAug
 from funasr.tasks.abs_task import AbsTask
 from funasr.torch_utils.initialize import initialize
-from funasr.train.abs_espnet_model import AbsESPnetModel
+from funasr.models.base_model import FunASRModel
 from funasr.train.class_choices import ClassChoices
 from funasr.train.trainer import Trainer
 from funasr.utils.types import float_or_none
 from funasr.utils.types import int_or_none
 from funasr.utils.types import str2bool
 from funasr.utils.types import str_or_none
 from funasr.models.frontend.wav_frontend import WavFrontend
@@ -90,15 +90,15 @@
     optional=True,
 )
 model_choices = ClassChoices(
     "model",
     classes=dict(
         espnet=ESPnetSVModel,
     ),
-    type_check=AbsESPnetModel,
+    type_check=FunASRModel,
     default="espnet",
 )
 preencoder_choices = ClassChoices(
     name="preencoder",
     classes=dict(
         sinc=LightweightSincConvs,
         linear=LinearProjection,
@@ -484,17 +484,17 @@
 
         with config_file.open("r", encoding="utf-8") as f:
             args = yaml.safe_load(f)
         if cmvn_file is not None:
             args["cmvn_file"] = cmvn_file
         args = argparse.Namespace(**args)
         model = cls.build_model(args)
-        if not isinstance(model, AbsESPnetModel):
+        if not isinstance(model, FunASRModel):
             raise RuntimeError(
-                f"model must inherit {AbsESPnetModel.__name__}, but got {type(model)}"
+                f"model must inherit {FunASRModel.__name__}, but got {type(model)}"
             )
         model.to(device)
         model_dict = dict()
         model_name_pth = None
         if model_file is not None:
             logging.info("model_file is {}".format(model_file))
             if device == "cuda":
```

### Comparing `funasr-0.5.3/funasr/text/build_tokenizer.py` & `funasr-0.5.4/funasr/text/build_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/text/char_tokenizer.py` & `funasr-0.5.4/funasr/text/char_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/text/cleaner.py` & `funasr-0.5.4/funasr/text/cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/text/korean_cleaner.py` & `funasr-0.5.4/funasr/text/korean_cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/text/phoneme_tokenizer.py` & `funasr-0.5.4/funasr/text/phoneme_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/text/sentencepiece_tokenizer.py` & `funasr-0.5.4/funasr/text/sentencepiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/text/token_id_converter.py` & `funasr-0.5.4/funasr/text/token_id_converter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/text/word_tokenizer.py` & `funasr-0.5.4/funasr/text/word_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/torch_utils/add_gradient_noise.py` & `funasr-0.5.4/funasr/torch_utils/add_gradient_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/torch_utils/device_funcs.py` & `funasr-0.5.4/funasr/torch_utils/device_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/torch_utils/forward_adaptor.py` & `funasr-0.5.4/funasr/torch_utils/forward_adaptor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/torch_utils/initialize.py` & `funasr-0.5.4/funasr/torch_utils/initialize.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/torch_utils/load_pretrained_model.py` & `funasr-0.5.4/funasr/torch_utils/load_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/torch_utils/model_summary.py` & `funasr-0.5.4/funasr/torch_utils/model_summary.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/torch_utils/recursive_op.py` & `funasr-0.5.4/funasr/torch_utils/recursive_op.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/train/abs_model.py` & `funasr-0.5.4/funasr/train/abs_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,163 @@
 from abc import ABC
 from abc import abstractmethod
 
-
+from funasr.modules.scorers.scorer_interface import BatchScorerInterface
 from typing import Dict
 from typing import Optional
 from typing import Tuple
 
 import torch
 import torch.nn.functional as F
 from typeguard import check_argument_types
 
 from funasr.modules.nets_utils import make_pad_mask
 from funasr.torch_utils.device_funcs import force_gatherable
-from funasr.train.abs_espnet_model import AbsESPnetModel
-
-from funasr.modules.scorers.scorer_interface import BatchScorerInterface
+from funasr.models.base_model import FunASRModel
 
-
-class AbsPunctuation(torch.nn.Module, BatchScorerInterface, ABC):
-    """The abstract class
+class AbsLM(torch.nn.Module, BatchScorerInterface, ABC):
+    """The abstract LM class
 
     To share the loss calculation way among different models,
     We uses delegate pattern here:
     The instance of this class should be passed to "LanguageModel"
 
     This "model" is one of mediator objects for "Task" class.
 
     """
 
     @abstractmethod
-    def forward(self, input: torch.Tensor, hidden: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
+    def forward(
+        self, input: torch.Tensor, hidden: torch.Tensor
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
         raise NotImplementedError
 
-    @abstractmethod
-    def with_vad(self) -> bool:
-        raise NotImplementedError
+
+class LanguageModel(FunASRModel):
+    def __init__(self, lm: AbsLM, vocab_size: int, ignore_id: int = 0):
+        assert check_argument_types()
+        super().__init__()
+        self.lm = lm
+        self.sos = 1
+        self.eos = 2
+
+        # ignore_id may be assumed as 0, shared with CTC-blank symbol for ASR.
+        self.ignore_id = ignore_id
+
+    def nll(
+        self,
+        text: torch.Tensor,
+        text_lengths: torch.Tensor,
+        max_length: Optional[int] = None,
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        """Compute negative log likelihood(nll)
+
+        Normally, this function is called in batchify_nll.
+        Args:
+            text: (Batch, Length)
+            text_lengths: (Batch,)
+            max_lengths: int
+        """
+        batch_size = text.size(0)
+        # For data parallel
+        if max_length is None:
+            text = text[:, : text_lengths.max()]
+        else:
+            text = text[:, :max_length]
+
+        # 1. Create a sentence pair like '<sos> w1 w2 w3' and 'w1 w2 w3 <eos>'
+        # text: (Batch, Length) -> x, y: (Batch, Length + 1)
+        x = F.pad(text, [1, 0], "constant", self.sos)
+        t = F.pad(text, [0, 1], "constant", self.ignore_id)
+        for i, l in enumerate(text_lengths):
+            t[i, l] = self.eos
+        x_lengths = text_lengths + 1
+
+        # 2. Forward Language model
+        # x: (Batch, Length) -> y: (Batch, Length, NVocab)
+        y, _ = self.lm(x, None)
+
+        # 3. Calc negative log likelihood
+        # nll: (BxL,)
+        nll = F.cross_entropy(y.view(-1, y.shape[-1]), t.view(-1), reduction="none")
+        # nll: (BxL,) -> (BxL,)
+        if max_length is None:
+            nll.masked_fill_(make_pad_mask(x_lengths).to(nll.device).view(-1), 0.0)
+        else:
+            nll.masked_fill_(
+                make_pad_mask(x_lengths, maxlen=max_length + 1).to(nll.device).view(-1),
+                0.0,
+            )
+        # nll: (BxL,) -> (B, L)
+        nll = nll.view(batch_size, -1)
+        return nll, x_lengths
+
+    def batchify_nll(
+        self, text: torch.Tensor, text_lengths: torch.Tensor, batch_size: int = 100
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        """Compute negative log likelihood(nll) from transformer language model
+
+        To avoid OOM, this fuction seperate the input into batches.
+        Then call nll for each batch and combine and return results.
+        Args:
+            text: (Batch, Length)
+            text_lengths: (Batch,)
+            batch_size: int, samples each batch contain when computing nll,
+                        you may change this to avoid OOM or increase
+
+        """
+        total_num = text.size(0)
+        if total_num <= batch_size:
+            nll, x_lengths = self.nll(text, text_lengths)
+        else:
+            nlls = []
+            x_lengths = []
+            max_length = text_lengths.max()
+
+            start_idx = 0
+            while True:
+                end_idx = min(start_idx + batch_size, total_num)
+                batch_text = text[start_idx:end_idx, :]
+                batch_text_lengths = text_lengths[start_idx:end_idx]
+                # batch_nll: [B * T]
+                batch_nll, batch_x_lengths = self.nll(
+                    batch_text, batch_text_lengths, max_length=max_length
+                )
+                nlls.append(batch_nll)
+                x_lengths.append(batch_x_lengths)
+                start_idx = end_idx
+                if start_idx == total_num:
+                    break
+            nll = torch.cat(nlls)
+            x_lengths = torch.cat(x_lengths)
+        assert nll.size(0) == total_num
+        assert x_lengths.size(0) == total_num
+        return nll, x_lengths
+
+    def forward(
+        self, text: torch.Tensor, text_lengths: torch.Tensor
+    ) -> Tuple[torch.Tensor, Dict[str, torch.Tensor], torch.Tensor]:
+        nll, y_lengths = self.nll(text, text_lengths)
+        ntokens = y_lengths.sum()
+        loss = nll.sum() / ntokens
+        stats = dict(loss=loss.detach())
+
+        # force_gatherable: to-device and to-tensor if scalar for DataParallel
+        loss, stats, weight = force_gatherable((loss, stats, ntokens), loss.device)
+        return loss, stats, weight
+
+    def collect_feats(
+        self, text: torch.Tensor, text_lengths: torch.Tensor
+    ) -> Dict[str, torch.Tensor]:
+        return {}
 
 
-class PunctuationModel(AbsESPnetModel):
+class PunctuationModel(FunASRModel):
     
-    def __init__(self, punc_model: AbsPunctuation, vocab_size: int, ignore_id: int = 0, punc_weight: list = None):
+    def __init__(self, punc_model: torch.nn.Module, vocab_size: int, ignore_id: int = 0, punc_weight: list = None):
         assert check_argument_types()
         super().__init__()
         self.punc_model = punc_model
         self.punc_weight = torch.Tensor(punc_weight)
         self.sos = 1
         self.eos = 2
```

### Comparing `funasr-0.5.3/funasr/train/class_choices.py` & `funasr-0.5.4/funasr/train/class_choices.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/train/distributed_utils.py` & `funasr-0.5.4/funasr/train/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/train/reporter.py` & `funasr-0.5.4/funasr/train/reporter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/train/trainer.py` & `funasr-0.5.4/funasr/train/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from funasr.schedulers.abs_scheduler import AbsEpochStepScheduler
 from funasr.schedulers.abs_scheduler import AbsScheduler
 from funasr.schedulers.abs_scheduler import AbsValEpochStepScheduler
 from funasr.torch_utils.add_gradient_noise import add_gradient_noise
 from funasr.torch_utils.device_funcs import to_device
 from funasr.torch_utils.recursive_op import recursive_average
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
-from funasr.train.abs_espnet_model import AbsESPnetModel
+from funasr.models.base_model import FunASRModel
 from funasr.train.distributed_utils import DistributedOption
 from funasr.train.reporter import Reporter
 from funasr.train.reporter import SubReporter
 from funasr.utils.build_dataclass import build_dataclass
 
 if torch.distributed.is_available():
     from torch.distributed import ReduceOp
@@ -162,15 +162,15 @@
                 scaler.load_state_dict(states["scaler"])
 
         logging.info(f"The training was resumed using {checkpoint}")
 
     @classmethod
     def run(
         cls,
-        model: AbsESPnetModel,
+        model: FunASRModel,
         optimizers: Sequence[torch.optim.Optimizer],
         schedulers: Sequence[Optional[AbsScheduler]],
         train_iter_factory: AbsIterFactory,
         valid_iter_factory: AbsIterFactory,
         trainer_options,
         distributed_option: DistributedOption,
     ) -> None:
```

### Comparing `funasr-0.5.3/funasr/utils/asr_env_checking.py` & `funasr-0.5.4/funasr/utils/asr_env_checking.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/utils/asr_utils.py` & `funasr-0.5.4/funasr/utils/asr_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/utils/build_dataclass.py` & `funasr-0.5.4/funasr/utils/build_dataclass.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/utils/cli_utils.py` & `funasr-0.5.4/funasr/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/utils/compute_eer.py` & `funasr-0.5.4/funasr/utils/compute_eer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/utils/compute_min_dcf.py` & `funasr-0.5.4/funasr/utils/compute_min_dcf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/utils/compute_wer.py` & `funasr-0.5.4/funasr/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/utils/config_argparse.py` & `funasr-0.5.4/funasr/utils/config_argparse.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/utils/get_default_kwargs.py` & `funasr-0.5.4/funasr/utils/get_default_kwargs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/utils/griffin_lim.py` & `funasr-0.5.4/funasr/utils/griffin_lim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/utils/job_runner.py` & `funasr-0.5.4/funasr/utils/job_runner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/utils/misc.py` & `funasr-0.5.4/funasr/utils/misc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/utils/modelscope_param.py` & `funasr-0.5.4/funasr/utils/modelscope_param.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/utils/modelscope_utils.py` & `funasr-0.5.4/funasr/utils/modelscope_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/utils/nested_dict_action.py` & `funasr-0.5.4/funasr/utils/nested_dict_action.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/utils/postprocess_utils.py` & `funasr-0.5.4/funasr/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/utils/sized_dict.py` & `funasr-0.5.4/funasr/utils/sized_dict.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/utils/timestamp_tools.py` & `funasr-0.5.4/funasr/utils/timestamp_tools.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/utils/types.py` & `funasr-0.5.4/funasr/utils/types.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/utils/vad_utils.py` & `funasr-0.5.4/funasr/utils/vad_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr/utils/wav_utils.py` & `funasr-0.5.4/funasr/utils/wav_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/funasr.egg-info/PKG-INFO` & `funasr-0.5.4/funasr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.5.3
+Version: 0.5.4
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -117,26 +117,22 @@
 
 ## License
 This project is licensed under the [The MIT License](https://opensource.org/licenses/MIT). FunASR also contains various third-party components and some code modified from other repos under other open source licenses.
 
 ## Citations
 
 ``` bibtex
-@inproceedings{gao2022paraformer,
-  title={Paraformer: Fast and Accurate Parallel Transformer for Non-autoregressive End-to-End Speech Recognition},
-  author={Gao, Zhifu and Zhang, Shiliang and McLoughlin, Ian and Yan, Zhijie},
+@inproceedings{gao2023funasr,
+  author={Zhifu Gao and Zerui Li and Jiaming Wang and Haoneng Luo and Xian Shi and Mengzhe Chen and Yabin Li and Lingyun Zuo and Zhihao Du and Zhangyu Xiao and Shiliang Zhang},
+  title={FunASR: A Fundamental End-to-End Speech Recognition Toolkit},
+  year={2023},
   booktitle={INTERSPEECH},
-  year={2022}
 }
-@inproceedings{gao2020universal,
-  title={Universal ASR: Unifying Streaming and Non-Streaming ASR Using a Single Encoder-Decoder Model},
-  author={Gao, Zhifu and Zhang, Shiliang and Lei, Ming and McLoughlin, Ian},
-  booktitle={arXiv preprint arXiv:2010.14099},
-  year={2020}
-}
-@inproceedings{Shi2023AchievingTP,
-  title={Achieving Timestamp Prediction While Recognizing with Non-Autoregressive End-to-End ASR Model},
-  author={Xian Shi and Yanni Chen and Shiliang Zhang and Zhijie Yan},
-  booktitle={arXiv preprint arXiv:2301.12343}
-  year={2023}
+@inproceedings{gao22b_interspeech,
+  author={Zhifu Gao and ShiLiang Zhang and Ian McLoughlin and Zhijie Yan},
+  title={{Paraformer: Fast and Accurate Parallel Transformer for Non-autoregressive End-to-End Speech Recognition}},
+  year=2022,
+  booktitle={Proc. Interspeech 2022},
+  pages={2063--2067},
+  doi={10.21437/Interspeech.2022-9996}
 }
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.5.3 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.5.4 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
@@ -94,18 +94,16 @@
 RapidAI) for contributing the Paraformer and CT_Transformer-punc runtime. 6. We
 acknowledge [DeepScience](https://www.deepscience.cn) for contributing the grpc
 service. 6. We acknowledge [AiHealthx](http://www.aihealthx.com/) for
 contributing the websocket service and html5. ## License This project is
 licensed under the [The MIT License](https://opensource.org/licenses/MIT).
 FunASR also contains various third-party components and some code modified from
 other repos under other open source licenses. ## Citations ``` bibtex
-@inproceedings{gao2022paraformer, title={Paraformer: Fast and Accurate Parallel
-Transformer for Non-autoregressive End-to-End Speech Recognition}, author={Gao,
-Zhifu and Zhang, Shiliang and McLoughlin, Ian and Yan, Zhijie}, booktitle=
-{INTERSPEECH}, year={2022} } @inproceedings{gao2020universal, title={Universal
-ASR: Unifying Streaming and Non-Streaming ASR Using a Single Encoder-Decoder
-Model}, author={Gao, Zhifu and Zhang, Shiliang and Lei, Ming and McLoughlin,
-Ian}, booktitle={arXiv preprint arXiv:2010.14099}, year={2020} } @inproceedings
-{Shi2023AchievingTP, title={Achieving Timestamp Prediction While Recognizing
-with Non-Autoregressive End-to-End ASR Model}, author={Xian Shi and Yanni Chen
-and Shiliang Zhang and Zhijie Yan}, booktitle={arXiv preprint arXiv:2301.12343}
-year={2023} } ```
+@inproceedings{gao2023funasr, author={Zhifu Gao and Zerui Li and Jiaming Wang
+and Haoneng Luo and Xian Shi and Mengzhe Chen and Yabin Li and Lingyun Zuo and
+Zhihao Du and Zhangyu Xiao and Shiliang Zhang}, title={FunASR: A Fundamental
+End-to-End Speech Recognition Toolkit}, year={2023}, booktitle={INTERSPEECH}, }
+@inproceedings{gao22b_interspeech, author={Zhifu Gao and ShiLiang Zhang and Ian
+McLoughlin and Zhijie Yan}, title={{Paraformer: Fast and Accurate Parallel
+Transformer for Non-autoregressive End-to-End Speech Recognition}}, year=2022,
+booktitle={Proc. Interspeech 2022}, pages={2063--2067}, doi={10.21437/
+Interspeech.2022-9996} } ```
```

### Comparing `funasr-0.5.3/funasr.egg-info/SOURCES.txt` & `funasr-0.5.4/funasr.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,55 +6,53 @@
 funasr.egg-info/PKG-INFO
 funasr.egg-info/SOURCES.txt
 funasr.egg-info/dependency_links.txt
 funasr.egg-info/requires.txt
 funasr.egg-info/top_level.txt
 funasr/bin/__init__.py
 funasr/bin/aggregate_stats_dirs.py
-funasr/bin/asr_inference.py
+funasr/bin/asr_infer.py
 funasr/bin/asr_inference_launch.py
-funasr/bin/asr_inference_mfcca.py
-funasr/bin/asr_inference_paraformer.py
-funasr/bin/asr_inference_paraformer_streaming.py
-funasr/bin/asr_inference_rnnt.py
-funasr/bin/asr_inference_uniasr.py
 funasr/bin/asr_train.py
-funasr/bin/asr_train_paraformer.py
-funasr/bin/asr_train_transducer.py
-funasr/bin/asr_train_uniasr.py
-funasr/bin/build_trainer.py
 funasr/bin/data2vec_train.py
+funasr/bin/diar_infer.py
 funasr/bin/diar_inference_launch.py
 funasr/bin/diar_train.py
-funasr/bin/eend_ola_inference.py
-funasr/bin/lm_calc_perplexity.py
-funasr/bin/lm_inference.py
 funasr/bin/lm_inference_launch.py
 funasr/bin/lm_train.py
-funasr/bin/modelscope_infer.py
+funasr/bin/punc_infer.py
 funasr/bin/punc_inference_launch.py
 funasr/bin/punc_train.py
-funasr/bin/punctuation_infer.py
-funasr/bin/punctuation_infer_vadrealtime.py
-funasr/bin/sa_asr_inference.py
 funasr/bin/sa_asr_train.py
-funasr/bin/sond_inference.py
-funasr/bin/sv_inference.py
+funasr/bin/sv_infer.py
 funasr/bin/sv_inference_launch.py
 funasr/bin/tokenize_text.py
-funasr/bin/tp_inference.py
+funasr/bin/tp_infer.py
 funasr/bin/tp_inference_launch.py
-funasr/bin/vad_inference.py
+funasr/bin/train.py
+funasr/bin/vad_infer.py
 funasr/bin/vad_inference_launch.py
-funasr/bin/vad_inference_online.py
+funasr/build_utils/__init__.py
+funasr/build_utils/build_args.py
+funasr/build_utils/build_asr_model.py
+funasr/build_utils/build_dataloader.py
+funasr/build_utils/build_diar_model.py
+funasr/build_utils/build_distributed.py
+funasr/build_utils/build_lm_model.py
+funasr/build_utils/build_model.py
+funasr/build_utils/build_optimizer.py
+funasr/build_utils/build_pretrain_model.py
+funasr/build_utils/build_punc_model.py
+funasr/build_utils/build_scheduler.py
+funasr/build_utils/build_trainer.py
+funasr/build_utils/build_vad_model.py
 funasr/datasets/__init__.py
 funasr/datasets/collate_fn.py
 funasr/datasets/dataset.py
 funasr/datasets/iterable_dataset.py
-funasr/datasets/iterable_dataset_modelscope.py
 funasr/datasets/ms_dataset.py
 funasr/datasets/preprocessor.py
 funasr/datasets/large_datasets/__init__.py
 funasr/datasets/large_datasets/build_dataloader.py
 funasr/datasets/large_datasets/dataset.py
 funasr/datasets/large_datasets/datapipes/__init__.py
 funasr/datasets/large_datasets/datapipes/batch.py
@@ -114,26 +112,23 @@
 funasr/layers/label_aggregation.py
 funasr/layers/log_mel.py
 funasr/layers/mask_along_axis.py
 funasr/layers/sinc_conv.py
 funasr/layers/stft.py
 funasr/layers/time_warp.py
 funasr/layers/utterance_mvn.py
-funasr/lm/__init__.py
-funasr/lm/abs_model.py
-funasr/lm/seq_rnn_lm.py
-funasr/lm/transformer_lm.py
 funasr/losses/__init__.py
 funasr/losses/label_smoothing_loss.py
 funasr/main_funcs/__init__.py
 funasr/main_funcs/average_nbest_models.py
 funasr/main_funcs/calculate_all_attentions.py
 funasr/main_funcs/collect_stats.py
 funasr/main_funcs/pack_funcs.py
 funasr/models/__init__.py
+funasr/models/base_model.py
 funasr/models/ctc.py
 funasr/models/data2vec.py
 funasr/models/e2e_asr.py
 funasr/models/e2e_asr_common.py
 funasr/models/e2e_asr_contextual_paraformer.py
 funasr/models/e2e_asr_mfcca.py
 funasr/models/e2e_asr_paraformer.py
@@ -141,15 +136,17 @@
 funasr/models/e2e_diar_eend_ola.py
 funasr/models/e2e_diar_sond.py
 funasr/models/e2e_sa_asr.py
 funasr/models/e2e_sv.py
 funasr/models/e2e_tp.py
 funasr/models/e2e_uni_asr.py
 funasr/models/e2e_vad.py
+funasr/models/seq_rnn_lm.py
 funasr/models/target_delay_transformer.py
+funasr/models/transformer_lm.py
 funasr/models/vad_realtime_transformer.py
 funasr/models/decoder/__init__.py
 funasr/models/decoder/abs_decoder.py
 funasr/models/decoder/contextual_decoder.py
 funasr/models/decoder/rnn_decoder.py
 funasr/models/decoder/rnnt_decoder.py
 funasr/models/decoder/sanm_decoder.py
@@ -325,15 +322,14 @@
 funasr/torch_utils/initialize.py
 funasr/torch_utils/load_pretrained_model.py
 funasr/torch_utils/model_summary.py
 funasr/torch_utils/pytorch_version.py
 funasr/torch_utils/recursive_op.py
 funasr/torch_utils/set_all_random_seed.py
 funasr/train/__init__.py
-funasr/train/abs_espnet_model.py
 funasr/train/abs_model.py
 funasr/train/class_choices.py
 funasr/train/distributed_utils.py
 funasr/train/reporter.py
 funasr/train/trainer.py
 funasr/utils/__init__.py
 funasr/utils/asr_env_checking.py
@@ -348,14 +344,15 @@
 funasr/utils/griffin_lim.py
 funasr/utils/job_runner.py
 funasr/utils/misc.py
 funasr/utils/modelscope_param.py
 funasr/utils/modelscope_utils.py
 funasr/utils/nested_dict_action.py
 funasr/utils/postprocess_utils.py
+funasr/utils/prepare_data.py
 funasr/utils/sized_dict.py
 funasr/utils/timestamp_tools.py
 funasr/utils/types.py
 funasr/utils/vad_utils.py
 funasr/utils/wav_utils.py
 funasr/utils/yaml_no_alias_safe_dump.py
 tests/test_asr_inference_pipeline.py
```

### Comparing `funasr-0.5.3/funasr.egg-info/requires.txt` & `funasr-0.5.4/funasr.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 setuptools>=38.5.1
 typeguard==2.13.3
 humanfriendly
 scipy>=1.4.1
-librosa
+librosa==0.8.1
 jamo==0.4.1
 PyYAML>=5.1.2
 soundfile>=0.10.2
 h5py>=2.10.0
 kaldiio>=2.17.0
 torch_complex
 nltk>=3.4.5
```

### Comparing `funasr-0.5.3/setup.py` & `funasr-0.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "install": [
         "setuptools>=38.5.1",
         # "configargparse>=1.2.1",
         "typeguard==2.13.3",
         "humanfriendly",
         "scipy>=1.4.1",
         # "filelock",
-        "librosa",
+        "librosa==0.8.1",
         "jamo==0.4.1",  # For kss
         "PyYAML>=5.1.2",
         "soundfile>=0.10.2",
         "h5py>=2.10.0",
         "kaldiio>=2.17.0",
         "torch_complex",
         "nltk>=3.4.5",
```

### Comparing `funasr-0.5.3/tests/test_asr_inference_pipeline.py` & `funasr-0.5.4/tests/test_asr_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/tests/test_asr_vad_punc_inference_pipeline.py` & `funasr-0.5.4/tests/test_asr_vad_punc_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/tests/test_lm_pipeline.py` & `funasr-0.5.4/tests/test_lm_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/tests/test_punctuation_pipeline.py` & `funasr-0.5.4/tests/test_punctuation_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/tests/test_sv_inference_pipeline.py` & `funasr-0.5.4/tests/test_sv_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.3/tests/test_vad_inference_pipeline.py` & `funasr-0.5.4/tests/test_vad_inference_pipeline.py`

 * *Files identical despite different names*

