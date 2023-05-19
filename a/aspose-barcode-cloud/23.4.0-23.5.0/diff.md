# Comparing `tmp/aspose-barcode-cloud-23.4.0.tar.gz` & `tmp/aspose-barcode-cloud-23.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aspose-barcode-cloud-23.4.0.tar", last modified: Thu Apr 27 16:36:19 2023, max compression
+gzip compressed data, was "dist/aspose-barcode-cloud-23.5.0.tar", last modified: Fri May 19 03:57:31 2023, max compression
```

## Comparing `aspose-barcode-cloud-23.4.0.tar` & `aspose-barcode-cloud-23.5.0.tar`

### file list

```diff
@@ -1,95 +1,97 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:36:19.000000 aspose-barcode-cloud-23.4.0/
--rw-r--r--   0 root         (0) root         (0)    16507 2023-04-27 16:36:19.000000 aspose-barcode-cloud-23.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12059 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:36:19.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/
--rw-r--r--   0 root         (0) root         (0)     6716 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:36:19.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/api/
--rw-r--r--   0 root         (0) root         (0)      319 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    99385 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/api/barcode_api.py
--rw-r--r--   0 root         (0) root         (0)    24296 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/api/file_api.py
--rw-r--r--   0 root         (0) root         (0)    22451 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/api/folder_api.py
--rw-r--r--   0 root         (0) root         (0)    16119 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/api/storage_api.py
--rw-r--r--   0 root         (0) root         (0)    26047 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/api_client.py
--rw-r--r--   0 root         (0) root         (0)    10460 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:36:19.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/
--rw-r--r--   0 root         (0) root         (0)     6260 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6521 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/api_error.py
--rw-r--r--   0 root         (0) root         (0)     4574 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/api_error_response.py
--rw-r--r--   0 root         (0) root         (0)     5429 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/australian_post_params.py
--rw-r--r--   0 root         (0) root         (0)     3371 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/auto_size_mode.py
--rw-r--r--   0 root         (0) root         (0)     3417 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/available_graphics_unit.py
--rw-r--r--   0 root         (0) root         (0)     6810 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/aztec_params.py
--rw-r--r--   0 root         (0) root         (0)     3393 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/aztec_symbol_mode.py
--rw-r--r--   0 root         (0) root         (0)     6225 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/barcode_response.py
--rw-r--r--   0 root         (0) root         (0)     4135 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/barcode_response_list.py
--rw-r--r--   0 root         (0) root         (0)     3413 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/border_dash_style.py
--rw-r--r--   0 root         (0) root         (0)     8315 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/caption_params.py
--rw-r--r--   0 root         (0) root         (0)     3371 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/checksum_validation.py
--rw-r--r--   0 root         (0) root         (0)     3361 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/codabar_checksum_mode.py
--rw-r--r--   0 root         (0) root         (0)     6349 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/codabar_params.py
--rw-r--r--   0 root         (0) root         (0)     3345 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/codabar_symbol.py
--rw-r--r--   0 root         (0) root         (0)     5474 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/codablock_params.py
--rw-r--r--   0 root         (0) root         (0)     3399 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/code128_emulation.py
--rw-r--r--   0 root         (0) root         (0)     6513 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/code16_k_params.py
--rw-r--r--   0 root         (0) root         (0)     3351 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/code_location.py
--rw-r--r--   0 root         (0) root         (0)     4238 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/coupon_params.py
--rw-r--r--   0 root         (0) root         (0)     3449 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/customer_information_interpreting_type.py
--rw-r--r--   0 root         (0) root         (0)     8008 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/data_bar_params.py
--rw-r--r--   0 root         (0) root         (0)     3469 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/data_matrix_ecc_type.py
--rw-r--r--   0 root         (0) root         (0)     3527 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/data_matrix_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)    10136 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/data_matrix_params.py
--rw-r--r--   0 root         (0) root         (0)     5679 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/decode_barcode_type.py
--rw-r--r--   0 root         (0) root         (0)     4913 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/disc_usage.py
--rw-r--r--   0 root         (0) root         (0)     3393 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/dot_code_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)     9394 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/dot_code_params.py
--rw-r--r--   0 root         (0) root         (0)     4029 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/eci_encodings.py
--rw-r--r--   0 root         (0) root         (0)     3355 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/enable_checksum.py
--rw-r--r--   0 root         (0) root         (0)     5359 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/encode_barcode_type.py
--rw-r--r--   0 root         (0) root         (0)     5970 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/error.py
--rw-r--r--   0 root         (0) root         (0)     4737 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/error_details.py
--rw-r--r--   0 root         (0) root         (0)     8827 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/file_version.py
--rw-r--r--   0 root         (0) root         (0)     3971 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/file_versions.py
--rw-r--r--   0 root         (0) root         (0)     3995 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/files_list.py
--rw-r--r--   0 root         (0) root         (0)     4770 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/files_upload_result.py
--rw-r--r--   0 root         (0) root         (0)     3317 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/font_mode.py
--rw-r--r--   0 root         (0) root         (0)     5207 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/font_params.py
--rw-r--r--   0 root         (0) root         (0)     3401 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/font_style.py
--rw-r--r--   0 root         (0) root         (0)    55723 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/generator_params.py
--rw-r--r--   0 root         (0) root         (0)     5896 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/generator_params_list.py
--rw-r--r--   0 root         (0) root         (0)     3407 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/itf14_border_type.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/itf_params.py
--rw-r--r--   0 root         (0) root         (0)     3367 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/macro_character.py
--rw-r--r--   0 root         (0) root         (0)     3397 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/maxi_code_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)     3393 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/maxi_code_mode.py
--rw-r--r--   0 root         (0) root         (0)     5685 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/maxi_code_params.py
--rw-r--r--   0 root         (0) root         (0)     4944 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/object_exist.py
--rw-r--r--   0 root         (0) root         (0)     5750 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/padding.py
--rw-r--r--   0 root         (0) root         (0)     5467 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/patch_code_params.py
--rw-r--r--   0 root         (0) root         (0)     3441 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/patch_format.py
--rw-r--r--   0 root         (0) root         (0)     3407 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/pdf417_compaction_mode.py
--rw-r--r--   0 root         (0) root         (0)     3507 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/pdf417_error_level.py
--rw-r--r--   0 root         (0) root         (0)     3381 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/pdf417_macro_terminator.py
--rw-r--r--   0 root         (0) root         (0)    24492 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/pdf417_params.py
--rw-r--r--   0 root         (0) root         (0)     4177 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/postal_params.py
--rw-r--r--   0 root         (0) root         (0)     3523 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/preset_type.py
--rw-r--r--   0 root         (0) root         (0)     3459 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/qr_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)     3369 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/qr_encode_type.py
--rw-r--r--   0 root         (0) root         (0)     3381 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/qr_error_level.py
--rw-r--r--   0 root         (0) root         (0)    11027 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/qr_params.py
--rw-r--r--   0 root         (0) root         (0)     4531 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/qr_version.py
--rw-r--r--   0 root         (0) root         (0)    46322 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/reader_params.py
--rw-r--r--   0 root         (0) root         (0)     4540 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/region_point.py
--rw-r--r--   0 root         (0) root         (0)     5716 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/result_image_info.py
--rw-r--r--   0 root         (0) root         (0)     4045 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/storage_exist.py
--rw-r--r--   0 root         (0) root         (0)     7017 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/storage_file.py
--rw-r--r--   0 root         (0) root         (0)     6065 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/structured_append.py
--rw-r--r--   0 root         (0) root         (0)     3357 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/text_alignment.py
--rw-r--r--   0 root         (0) root         (0)    14400 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:36:19.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16507 2023-04-27 16:36:19.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3966 2023-04-27 16:36:19.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 16:36:19.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-04-27 16:36:19.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-27 16:36:19.000000 aspose-barcode-cloud-23.4.0/aspose_barcode_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 16:36:19.000000 aspose-barcode-cloud-23.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     5750 2023-04-27 16:35:47.000000 aspose-barcode-cloud-23.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:57:31.000000 aspose-barcode-cloud-23.5.0/
+-rw-r--r--   0 root         (0) root         (0)    16613 2023-05-19 03:57:31.000000 aspose-barcode-cloud-23.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12149 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:57:31.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/
+-rw-r--r--   0 root         (0) root         (0)     6863 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:57:31.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/api/
+-rw-r--r--   0 root         (0) root         (0)      319 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    99385 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/api/barcode_api.py
+-rw-r--r--   0 root         (0) root         (0)    24296 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/api/file_api.py
+-rw-r--r--   0 root         (0) root         (0)    22451 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/api/folder_api.py
+-rw-r--r--   0 root         (0) root         (0)    16119 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/api/storage_api.py
+-rw-r--r--   0 root         (0) root         (0)    26047 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    10460 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:57:31.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/
+-rw-r--r--   0 root         (0) root         (0)     6407 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6521 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/api_error.py
+-rw-r--r--   0 root         (0) root         (0)     4574 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/api_error_response.py
+-rw-r--r--   0 root         (0) root         (0)     5429 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/australian_post_params.py
+-rw-r--r--   0 root         (0) root         (0)     3371 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/auto_size_mode.py
+-rw-r--r--   0 root         (0) root         (0)     3417 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/available_graphics_unit.py
+-rw-r--r--   0 root         (0) root         (0)     6810 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/aztec_params.py
+-rw-r--r--   0 root         (0) root         (0)     3393 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/aztec_symbol_mode.py
+-rw-r--r--   0 root         (0) root         (0)     6225 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/barcode_response.py
+-rw-r--r--   0 root         (0) root         (0)     4135 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/barcode_response_list.py
+-rw-r--r--   0 root         (0) root         (0)     3413 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/border_dash_style.py
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/caption_params.py
+-rw-r--r--   0 root         (0) root         (0)     3371 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/checksum_validation.py
+-rw-r--r--   0 root         (0) root         (0)     3361 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/codabar_checksum_mode.py
+-rw-r--r--   0 root         (0) root         (0)     6349 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/codabar_params.py
+-rw-r--r--   0 root         (0) root         (0)     3345 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/codabar_symbol.py
+-rw-r--r--   0 root         (0) root         (0)     5474 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/codablock_params.py
+-rw-r--r--   0 root         (0) root         (0)     3399 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/code128_emulation.py
+-rw-r--r--   0 root         (0) root         (0)     3457 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/code128_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)     4240 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/code128_params.py
+-rw-r--r--   0 root         (0) root         (0)     6513 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/code16_k_params.py
+-rw-r--r--   0 root         (0) root         (0)     3351 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/code_location.py
+-rw-r--r--   0 root         (0) root         (0)     4238 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/coupon_params.py
+-rw-r--r--   0 root         (0) root         (0)     3449 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/customer_information_interpreting_type.py
+-rw-r--r--   0 root         (0) root         (0)     8008 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/data_bar_params.py
+-rw-r--r--   0 root         (0) root         (0)     3469 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/data_matrix_ecc_type.py
+-rw-r--r--   0 root         (0) root         (0)     3527 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/data_matrix_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)    10136 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/data_matrix_params.py
+-rw-r--r--   0 root         (0) root         (0)     5679 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/decode_barcode_type.py
+-rw-r--r--   0 root         (0) root         (0)     4913 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/disc_usage.py
+-rw-r--r--   0 root         (0) root         (0)     3393 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/dot_code_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)     9394 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/dot_code_params.py
+-rw-r--r--   0 root         (0) root         (0)     4029 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/eci_encodings.py
+-rw-r--r--   0 root         (0) root         (0)     3355 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/enable_checksum.py
+-rw-r--r--   0 root         (0) root         (0)     5359 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/encode_barcode_type.py
+-rw-r--r--   0 root         (0) root         (0)     5970 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/error.py
+-rw-r--r--   0 root         (0) root         (0)     4737 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/error_details.py
+-rw-r--r--   0 root         (0) root         (0)     8827 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/file_version.py
+-rw-r--r--   0 root         (0) root         (0)     3971 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/file_versions.py
+-rw-r--r--   0 root         (0) root         (0)     3995 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/files_list.py
+-rw-r--r--   0 root         (0) root         (0)     4770 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/files_upload_result.py
+-rw-r--r--   0 root         (0) root         (0)     3317 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/font_mode.py
+-rw-r--r--   0 root         (0) root         (0)     5207 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/font_params.py
+-rw-r--r--   0 root         (0) root         (0)     3401 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/font_style.py
+-rw-r--r--   0 root         (0) root         (0)    56486 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/generator_params.py
+-rw-r--r--   0 root         (0) root         (0)     5896 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/generator_params_list.py
+-rw-r--r--   0 root         (0) root         (0)     3407 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/itf14_border_type.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/itf_params.py
+-rw-r--r--   0 root         (0) root         (0)     3367 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/macro_character.py
+-rw-r--r--   0 root         (0) root         (0)     3397 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/maxi_code_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)     3393 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/maxi_code_mode.py
+-rw-r--r--   0 root         (0) root         (0)     5685 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/maxi_code_params.py
+-rw-r--r--   0 root         (0) root         (0)     4944 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/object_exist.py
+-rw-r--r--   0 root         (0) root         (0)     5750 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/padding.py
+-rw-r--r--   0 root         (0) root         (0)     5467 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/patch_code_params.py
+-rw-r--r--   0 root         (0) root         (0)     3441 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/patch_format.py
+-rw-r--r--   0 root         (0) root         (0)     3407 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/pdf417_compaction_mode.py
+-rw-r--r--   0 root         (0) root         (0)     3507 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/pdf417_error_level.py
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/pdf417_macro_terminator.py
+-rw-r--r--   0 root         (0) root         (0)    24492 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/pdf417_params.py
+-rw-r--r--   0 root         (0) root         (0)     4177 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/postal_params.py
+-rw-r--r--   0 root         (0) root         (0)     3523 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/preset_type.py
+-rw-r--r--   0 root         (0) root         (0)     3459 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/qr_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)     3369 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/qr_encode_type.py
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/qr_error_level.py
+-rw-r--r--   0 root         (0) root         (0)    11027 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/qr_params.py
+-rw-r--r--   0 root         (0) root         (0)     4531 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/qr_version.py
+-rw-r--r--   0 root         (0) root         (0)    46322 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/reader_params.py
+-rw-r--r--   0 root         (0) root         (0)     4540 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/region_point.py
+-rw-r--r--   0 root         (0) root         (0)     5716 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/result_image_info.py
+-rw-r--r--   0 root         (0) root         (0)     4045 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/storage_exist.py
+-rw-r--r--   0 root         (0) root         (0)     7017 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/storage_file.py
+-rw-r--r--   0 root         (0) root         (0)     6065 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/structured_append.py
+-rw-r--r--   0 root         (0) root         (0)     3357 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/text_alignment.py
+-rw-r--r--   0 root         (0) root         (0)    14400 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:57:31.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16613 2023-05-19 03:57:30.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4063 2023-05-19 03:57:31.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 03:57:30.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-19 03:57:30.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-19 03:57:30.000000 aspose-barcode-cloud-23.5.0/aspose_barcode_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 03:57:31.000000 aspose-barcode-cloud-23.5.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     5750 2023-05-19 03:56:32.000000 aspose-barcode-cloud-23.5.0/setup.py
```

### Comparing `aspose-barcode-cloud-23.4.0/PKG-INFO` & `aspose-barcode-cloud-23.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aspose-barcode-cloud
-Version: 23.4.0
+Version: 23.5.0
 Summary: Aspose.Barcode Cloud API Reference
 Home-page: https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python
 Author: Aspose Barcode Cloud
 License: MIT
 Project-URL: Source With Tests, https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python
 Project-URL: Website, https://www.aspose.cloud
 Project-URL: Product Home, https://products.aspose.cloud/barcode/
@@ -15,15 +15,15 @@
 Description: # Aspose.BarCode Cloud SDK for Python
         
         [![License](https://img.shields.io/github/license/aspose-barcode-cloud/aspose-barcode-cloud-python)](LICENSE)
         [![Python package](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml/badge.svg)](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml)
         [![PyPI](https://img.shields.io/pypi/v/aspose-barcode-cloud)](https://pypi.org/project/aspose-barcode-cloud/)
         
         - API version: 3.0
-        - Package version: 23.4.0
+        - Package version: 23.5.0
         
         ## Demo applications
         
         [Scan QR](https://products.aspose.app/barcode/scanqr) | [Generate Barcode](https://products.aspose.app/barcode/generate) | [Recognize Barcode](https://products.aspose.app/barcode/recognize)
         :---: | :---: | :---:
         [![ScanQR](https://products.aspose.app/barcode/scanqr/img/aspose_scanqr-app-48.png)](https://products.aspose.app/barcode/scanqr) | [![Generate](https://products.aspose.app/barcode/generate/img/aspose_generate-app-48.png)](https://products.aspose.app/barcode/generate) | [![Recognize](https://products.aspose.app/barcode/recognize/img/aspose_recognize-app-48.png)](https://products.aspose.app/barcode/recognize)
         [**Generate Wi-Fi QR**](https://products.aspose.app/barcode/wifi-qr) | [**Embed Barcode**](https://products.aspose.app/barcode/embed) | [**Scan Barcode**](https://products.aspose.app/barcode/scan)
@@ -164,14 +164,16 @@
         - [CaptionParams](docs/CaptionParams.md)
         - [ChecksumValidation](docs/ChecksumValidation.md)
         - [CodabarChecksumMode](docs/CodabarChecksumMode.md)
         - [CodabarParams](docs/CodabarParams.md)
         - [CodabarSymbol](docs/CodabarSymbol.md)
         - [CodablockParams](docs/CodablockParams.md)
         - [Code128Emulation](docs/Code128Emulation.md)
+        - [Code128EncodeMode](docs/Code128EncodeMode.md)
+        - [Code128Params](docs/Code128Params.md)
         - [Code16KParams](docs/Code16KParams.md)
         - [CodeLocation](docs/CodeLocation.md)
         - [CouponParams](docs/CouponParams.md)
         - [CustomerInformationInterpretingType](docs/CustomerInformationInterpretingType.md)
         - [DataBarParams](docs/DataBarParams.md)
         - [DataMatrixEccType](docs/DataMatrixEccType.md)
         - [DataMatrixEncodeMode](docs/DataMatrixEncodeMode.md)
```

### Comparing `aspose-barcode-cloud-23.4.0/README.md` & `aspose-barcode-cloud-23.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Aspose.BarCode Cloud SDK for Python
 
 [![License](https://img.shields.io/github/license/aspose-barcode-cloud/aspose-barcode-cloud-python)](LICENSE)
 [![Python package](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml/badge.svg)](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml)
 [![PyPI](https://img.shields.io/pypi/v/aspose-barcode-cloud)](https://pypi.org/project/aspose-barcode-cloud/)
 
 - API version: 3.0
-- Package version: 23.4.0
+- Package version: 23.5.0
 
 ## Demo applications
 
 [Scan QR](https://products.aspose.app/barcode/scanqr) | [Generate Barcode](https://products.aspose.app/barcode/generate) | [Recognize Barcode](https://products.aspose.app/barcode/recognize)
 :---: | :---: | :---:
 [![ScanQR](https://products.aspose.app/barcode/scanqr/img/aspose_scanqr-app-48.png)](https://products.aspose.app/barcode/scanqr) | [![Generate](https://products.aspose.app/barcode/generate/img/aspose_generate-app-48.png)](https://products.aspose.app/barcode/generate) | [![Recognize](https://products.aspose.app/barcode/recognize/img/aspose_recognize-app-48.png)](https://products.aspose.app/barcode/recognize)
 [**Generate Wi-Fi QR**](https://products.aspose.app/barcode/wifi-qr) | [**Embed Barcode**](https://products.aspose.app/barcode/embed) | [**Scan Barcode**](https://products.aspose.app/barcode/scan)
@@ -150,14 +150,16 @@
 - [CaptionParams](docs/CaptionParams.md)
 - [ChecksumValidation](docs/ChecksumValidation.md)
 - [CodabarChecksumMode](docs/CodabarChecksumMode.md)
 - [CodabarParams](docs/CodabarParams.md)
 - [CodabarSymbol](docs/CodabarSymbol.md)
 - [CodablockParams](docs/CodablockParams.md)
 - [Code128Emulation](docs/Code128Emulation.md)
+- [Code128EncodeMode](docs/Code128EncodeMode.md)
+- [Code128Params](docs/Code128Params.md)
 - [Code16KParams](docs/Code16KParams.md)
 - [CodeLocation](docs/CodeLocation.md)
 - [CouponParams](docs/CouponParams.md)
 - [CustomerInformationInterpretingType](docs/CustomerInformationInterpretingType.md)
 - [DataBarParams](docs/DataBarParams.md)
 - [DataMatrixEccType](docs/DataMatrixEccType.md)
 - [DataMatrixEncodeMode](docs/DataMatrixEncodeMode.md)
```

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/__init__.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,16 @@
 from aspose_barcode_cloud.models.caption_params import CaptionParams
 from aspose_barcode_cloud.models.checksum_validation import ChecksumValidation
 from aspose_barcode_cloud.models.codabar_checksum_mode import CodabarChecksumMode
 from aspose_barcode_cloud.models.codabar_params import CodabarParams
 from aspose_barcode_cloud.models.codabar_symbol import CodabarSymbol
 from aspose_barcode_cloud.models.codablock_params import CodablockParams
 from aspose_barcode_cloud.models.code128_emulation import Code128Emulation
+from aspose_barcode_cloud.models.code128_encode_mode import Code128EncodeMode
+from aspose_barcode_cloud.models.code128_params import Code128Params
 from aspose_barcode_cloud.models.code16_k_params import Code16KParams
 from aspose_barcode_cloud.models.code_location import CodeLocation
 from aspose_barcode_cloud.models.coupon_params import CouponParams
 from aspose_barcode_cloud.models.customer_information_interpreting_type import CustomerInformationInterpretingType
 from aspose_barcode_cloud.models.data_bar_params import DataBarParams
 from aspose_barcode_cloud.models.data_matrix_ecc_type import DataMatrixEccType
 from aspose_barcode_cloud.models.data_matrix_encode_mode import DataMatrixEncodeMode
```

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/api/barcode_api.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/api/barcode_api.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/api/file_api.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/api/file_api.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/api/folder_api.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/api/folder_api.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/api/storage_api.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/api/storage_api.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/api_client.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,21 +86,21 @@
         self.configuration = configuration
 
         # Use the pool property to lazily initialize the ThreadPool.
         self._pool = None
         self.rest_client = RESTClientObject(configuration)
         self.default_headers = {
             "x-aspose-client": "python sdk",
-            "x-aspose-client-version": "23.4.0",
+            "x-aspose-client-version": "23.5.0",
         }
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = "Aspose-Barcode-SDK/23.4.0/python"
+        self.user_agent = "Aspose-Barcode-SDK/23.5.0/python"
 
     def __del__(self):
         self.rest_client.close()
         if self._pool is not None:
             self._pool.close()
             self._pool.join()
```

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/configuration.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,15 +282,15 @@
         :return: The report for debugging.
         """
         return (
             "Python SDK Debug Report:\n"
             "OS: {env}\n"
             "Python Version: {pyversion}\n"
             "Version of the API: 3.0\n"
-            "SDK Package Version: 23.4.0".format(env=sys.platform, pyversion=sys.version)
+            "SDK Package Version: 23.5.0".format(env=sys.platform, pyversion=sys.version)
         )
 
     @staticmethod
     def fetch_token(client_id, client_secret, token_url):
         with contextlib.closing(
             RESTClientObject(Configuration(client_id=client_id, client_secret=client_secret, token_url=token_url))
         ) as client:
```

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/__init__.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 from aspose_barcode_cloud.models.caption_params import CaptionParams
 from aspose_barcode_cloud.models.checksum_validation import ChecksumValidation
 from aspose_barcode_cloud.models.codabar_checksum_mode import CodabarChecksumMode
 from aspose_barcode_cloud.models.codabar_params import CodabarParams
 from aspose_barcode_cloud.models.codabar_symbol import CodabarSymbol
 from aspose_barcode_cloud.models.codablock_params import CodablockParams
 from aspose_barcode_cloud.models.code128_emulation import Code128Emulation
+from aspose_barcode_cloud.models.code128_encode_mode import Code128EncodeMode
+from aspose_barcode_cloud.models.code128_params import Code128Params
 from aspose_barcode_cloud.models.code16_k_params import Code16KParams
 from aspose_barcode_cloud.models.code_location import CodeLocation
 from aspose_barcode_cloud.models.coupon_params import CouponParams
 from aspose_barcode_cloud.models.customer_information_interpreting_type import CustomerInformationInterpretingType
 from aspose_barcode_cloud.models.data_bar_params import DataBarParams
 from aspose_barcode_cloud.models.data_matrix_ecc_type import DataMatrixEccType
 from aspose_barcode_cloud.models.data_matrix_encode_mode import DataMatrixEncodeMode
```

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/api_error.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/api_error.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/api_error_response.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/api_error_response.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/australian_post_params.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/australian_post_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/auto_size_mode.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/auto_size_mode.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/available_graphics_unit.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/available_graphics_unit.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/aztec_params.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/aztec_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/aztec_symbol_mode.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/aztec_symbol_mode.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/barcode_response.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/barcode_response.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/barcode_response_list.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/barcode_response_list.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/border_dash_style.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/border_dash_style.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/caption_params.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/caption_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/checksum_validation.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/checksum_validation.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/codabar_checksum_mode.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/codabar_checksum_mode.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/codabar_params.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/codabar_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/codabar_symbol.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/codabar_symbol.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/codablock_params.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/codablock_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/code128_emulation.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/code128_emulation.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/code16_k_params.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/code16_k_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/code_location.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/code_location.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/coupon_params.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/coupon_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/customer_information_interpreting_type.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/customer_information_interpreting_type.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/data_bar_params.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/data_bar_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/data_matrix_ecc_type.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/data_matrix_ecc_type.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/data_matrix_encode_mode.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/data_matrix_encode_mode.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/data_matrix_params.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/data_matrix_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/decode_barcode_type.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/decode_barcode_type.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/disc_usage.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/disc_usage.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/dot_code_encode_mode.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/dot_code_encode_mode.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/dot_code_params.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/dot_code_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/eci_encodings.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/eci_encodings.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/enable_checksum.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/enable_checksum.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/encode_barcode_type.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/encode_barcode_type.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/error.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/error.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/error_details.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/error_details.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/file_version.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/file_version.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/file_versions.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/file_versions.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/files_list.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/files_list.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/files_upload_result.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/files_upload_result.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/font_mode.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/font_mode.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/font_params.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/font_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/font_style.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/font_style.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/generator_params.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/generator_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,15 @@
         "dot_code": "DotCodeParams",
         "itf": "ITFParams",
         "maxi_code": "MaxiCodeParams",
         "pdf417": "Pdf417Params",
         "postal": "PostalParams",
         "qr": "QrParams",
         "patch_code": "PatchCodeParams",
+        "code128": "Code128Params",
     }
 
     attribute_map = {
         "type_of_barcode": "TypeOfBarcode",
         "text": "Text",
         "two_d_display_text": "TwoDDisplayText",
         "text_location": "TextLocation",
@@ -152,14 +153,15 @@
         "dot_code": "DotCode",
         "itf": "ITF",
         "maxi_code": "MaxiCode",
         "pdf417": "Pdf417",
         "postal": "Postal",
         "qr": "QR",
         "patch_code": "PatchCode",
+        "code128": "Code128",
     }
 
     def __init__(
         self,
         type_of_barcode=None,
         text=None,
         two_d_display_text=None,
@@ -210,14 +212,15 @@
         dot_code=None,
         itf=None,
         maxi_code=None,
         pdf417=None,
         postal=None,
         qr=None,
         patch_code=None,
+        code128=None,
     ):  # noqa: E501
         """GeneratorParams - a model defined in Swagger"""  # noqa: E501
 
         self._type_of_barcode = None
         self._text = None
         self._two_d_display_text = None
         self._text_location = None
@@ -267,14 +270,15 @@
         self._dot_code = None
         self._itf = None
         self._maxi_code = None
         self._pdf417 = None
         self._postal = None
         self._qr = None
         self._patch_code = None
+        self._code128 = None
         self.discriminator = None
 
         self.type_of_barcode = type_of_barcode
         self.text = text
         if two_d_display_text is not None:
             self.two_d_display_text = two_d_display_text
         if text_location is not None:
@@ -375,14 +379,16 @@
             self.pdf417 = pdf417
         if postal is not None:
             self.postal = postal
         if qr is not None:
             self.qr = qr
         if patch_code is not None:
             self.patch_code = patch_code
+        if code128 is not None:
+            self.code128 = code128
 
     @property
     def type_of_barcode(self):
         """Gets the type_of_barcode of this GeneratorParams.  # noqa: E501
 
         Type of barcode to generate.  # noqa: E501
 
@@ -1622,14 +1628,37 @@
 
         :param patch_code: The patch_code of this GeneratorParams.  # noqa: E501
         :type: PatchCodeParams
         """
 
         self._patch_code = patch_code
 
+    @property
+    def code128(self):
+        """Gets the code128 of this GeneratorParams.  # noqa: E501
+
+        Code128 params.  # noqa: E501
+
+        :return: The code128 of this GeneratorParams.  # noqa: E501
+        :rtype: Code128Params
+        """
+        return self._code128
+
+    @code128.setter
+    def code128(self, code128):
+        """Sets the code128 of this GeneratorParams.
+
+        Code128 params.  # noqa: E501
+
+        :param code128: The code128 of this GeneratorParams.  # noqa: E501
+        :type: Code128Params
+        """
+
+        self._code128 = code128
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/generator_params_list.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/generator_params_list.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/itf14_border_type.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/itf14_border_type.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/itf_params.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/itf_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/macro_character.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/macro_character.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/maxi_code_encode_mode.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/maxi_code_encode_mode.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/maxi_code_mode.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/maxi_code_mode.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/maxi_code_params.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/maxi_code_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/object_exist.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/object_exist.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/padding.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/padding.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/patch_code_params.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/patch_code_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/patch_format.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/patch_format.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/pdf417_compaction_mode.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/pdf417_compaction_mode.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/pdf417_error_level.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/pdf417_error_level.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/pdf417_macro_terminator.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/pdf417_macro_terminator.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/pdf417_params.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/pdf417_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/postal_params.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/postal_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/preset_type.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/preset_type.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/qr_encode_mode.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/qr_encode_mode.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/qr_encode_type.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/qr_encode_type.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/qr_error_level.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/qr_error_level.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/qr_params.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/qr_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/qr_version.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/qr_version.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/reader_params.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/reader_params.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/region_point.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/region_point.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/result_image_info.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/result_image_info.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/storage_exist.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/storage_exist.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/storage_file.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/storage_file.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/structured_append.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/structured_append.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/models/text_alignment.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/models/text_alignment.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud/rest.py` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud/rest.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud.egg-info/PKG-INFO` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aspose-barcode-cloud
-Version: 23.4.0
+Version: 23.5.0
 Summary: Aspose.Barcode Cloud API Reference
 Home-page: https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python
 Author: Aspose Barcode Cloud
 License: MIT
 Project-URL: Source With Tests, https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python
 Project-URL: Website, https://www.aspose.cloud
 Project-URL: Product Home, https://products.aspose.cloud/barcode/
@@ -15,15 +15,15 @@
 Description: # Aspose.BarCode Cloud SDK for Python
         
         [![License](https://img.shields.io/github/license/aspose-barcode-cloud/aspose-barcode-cloud-python)](LICENSE)
         [![Python package](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml/badge.svg)](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml)
         [![PyPI](https://img.shields.io/pypi/v/aspose-barcode-cloud)](https://pypi.org/project/aspose-barcode-cloud/)
         
         - API version: 3.0
-        - Package version: 23.4.0
+        - Package version: 23.5.0
         
         ## Demo applications
         
         [Scan QR](https://products.aspose.app/barcode/scanqr) | [Generate Barcode](https://products.aspose.app/barcode/generate) | [Recognize Barcode](https://products.aspose.app/barcode/recognize)
         :---: | :---: | :---:
         [![ScanQR](https://products.aspose.app/barcode/scanqr/img/aspose_scanqr-app-48.png)](https://products.aspose.app/barcode/scanqr) | [![Generate](https://products.aspose.app/barcode/generate/img/aspose_generate-app-48.png)](https://products.aspose.app/barcode/generate) | [![Recognize](https://products.aspose.app/barcode/recognize/img/aspose_recognize-app-48.png)](https://products.aspose.app/barcode/recognize)
         [**Generate Wi-Fi QR**](https://products.aspose.app/barcode/wifi-qr) | [**Embed Barcode**](https://products.aspose.app/barcode/embed) | [**Scan Barcode**](https://products.aspose.app/barcode/scan)
@@ -164,14 +164,16 @@
         - [CaptionParams](docs/CaptionParams.md)
         - [ChecksumValidation](docs/ChecksumValidation.md)
         - [CodabarChecksumMode](docs/CodabarChecksumMode.md)
         - [CodabarParams](docs/CodabarParams.md)
         - [CodabarSymbol](docs/CodabarSymbol.md)
         - [CodablockParams](docs/CodablockParams.md)
         - [Code128Emulation](docs/Code128Emulation.md)
+        - [Code128EncodeMode](docs/Code128EncodeMode.md)
+        - [Code128Params](docs/Code128Params.md)
         - [Code16KParams](docs/Code16KParams.md)
         - [CodeLocation](docs/CodeLocation.md)
         - [CouponParams](docs/CouponParams.md)
         - [CustomerInformationInterpretingType](docs/CustomerInformationInterpretingType.md)
         - [DataBarParams](docs/DataBarParams.md)
         - [DataMatrixEccType](docs/DataMatrixEccType.md)
         - [DataMatrixEncodeMode](docs/DataMatrixEncodeMode.md)
```

### Comparing `aspose-barcode-cloud-23.4.0/aspose_barcode_cloud.egg-info/SOURCES.txt` & `aspose-barcode-cloud-23.5.0/aspose_barcode_cloud.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 aspose_barcode_cloud/models/caption_params.py
 aspose_barcode_cloud/models/checksum_validation.py
 aspose_barcode_cloud/models/codabar_checksum_mode.py
 aspose_barcode_cloud/models/codabar_params.py
 aspose_barcode_cloud/models/codabar_symbol.py
 aspose_barcode_cloud/models/codablock_params.py
 aspose_barcode_cloud/models/code128_emulation.py
+aspose_barcode_cloud/models/code128_encode_mode.py
+aspose_barcode_cloud/models/code128_params.py
 aspose_barcode_cloud/models/code16_k_params.py
 aspose_barcode_cloud/models/code_location.py
 aspose_barcode_cloud/models/coupon_params.py
 aspose_barcode_cloud/models/customer_information_interpreting_type.py
 aspose_barcode_cloud/models/data_bar_params.py
 aspose_barcode_cloud/models/data_matrix_ecc_type.py
 aspose_barcode_cloud/models/data_matrix_encode_mode.py
```

### Comparing `aspose-barcode-cloud-23.4.0/setup.py` & `aspose-barcode-cloud-23.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 """
 
 import os
 
 from setuptools import setup, find_packages
 
 NAME = "aspose-barcode-cloud"
-VERSION = "23.4.0"
+VERSION = "23.5.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

