# Comparing `tmp/monai-generative-0.2.1.tar.gz` & `tmp/monai-generative-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monai-generative-0.2.1.tar", last modified: Wed May 17 16:51:24 2023, max compression
+gzip compressed data, was "monai-generative-0.2.2.tar", last modified: Fri May 19 12:29:35 2023, max compression
```

## Comparing `monai-generative-0.2.1.tar` & `monai-generative-0.2.2.tar`

### file list

```diff
@@ -1,87 +1,92 @@
-drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-17 16:51:24.308555 monai-generative-0.2.1/
--rw-rw-r--   0 walter    (1000) walter    (1000)    11357 2022-12-19 11:22:05.000000 monai-generative-0.2.1/LICENSE
--rw-rw-r--   0 walter    (1000) walter    (1000)      179 2023-05-17 16:51:24.308555 monai-generative-0.2.1/PKG-INFO
--rw-rw-r--   0 walter    (1000) walter    (1000)     3033 2023-04-04 12:39:13.000000 monai-generative-0.2.1/README.md
-drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-17 16:51:24.304555 monai-generative-0.2.1/generative/
--rw-rw-r--   0 walter    (1000) walter    (1000)      643 2023-03-12 10:31:18.000000 monai-generative-0.2.1/generative/__init__.py
-drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-17 16:51:24.304555 monai-generative-0.2.1/generative/engines/
--rw-rw-r--   0 walter    (1000) walter    (1000)      724 2023-04-02 11:47:15.000000 monai-generative-0.2.1/generative/engines/__init__.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     4685 2023-04-02 11:47:15.000000 monai-generative-0.2.1/generative/engines/prepare_batch.py
--rw-rw-r--   0 walter    (1000) walter    (1000)    16388 2023-03-20 16:09:39.000000 monai-generative-0.2.1/generative/engines/trainer.py
-drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-17 16:51:24.304555 monai-generative-0.2.1/generative/inferers/
--rw-rw-r--   0 walter    (1000) walter    (1000)      697 2023-03-12 10:31:18.000000 monai-generative-0.2.1/generative/inferers/__init__.py
--rw-rw-r--   0 walter    (1000) walter    (1000)    27940 2023-04-09 13:54:59.000000 monai-generative-0.2.1/generative/inferers/inferer.py
-drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-17 16:51:24.304555 monai-generative-0.2.1/generative/losses/
--rw-rw-r--   0 walter    (1000) walter    (1000)      739 2023-04-02 11:47:15.000000 monai-generative-0.2.1/generative/losses/__init__.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     7671 2023-05-17 14:56:31.000000 monai-generative-0.2.1/generative/losses/adversarial_loss.py
--rw-rw-r--   0 walter    (1000) walter    (1000)    16409 2023-05-17 14:56:31.000000 monai-generative-0.2.1/generative/losses/perceptual.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     3366 2023-03-12 10:31:18.000000 monai-generative-0.2.1/generative/losses/spectral_loss.py
-drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-17 16:51:24.304555 monai-generative-0.2.1/generative/metrics/
--rw-rw-r--   0 walter    (1000) walter    (1000)      735 2023-05-17 14:56:31.000000 monai-generative-0.2.1/generative/metrics/__init__.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     4500 2023-04-09 13:54:59.000000 monai-generative-0.2.1/generative/metrics/fid.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     3206 2023-05-17 14:56:31.000000 monai-generative-0.2.1/generative/metrics/mmd.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     6399 2023-04-09 13:54:59.000000 monai-generative-0.2.1/generative/metrics/ms_ssim.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     9494 2023-04-09 13:54:59.000000 monai-generative-0.2.1/generative/metrics/ssim.py
-drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-17 16:51:24.304555 monai-generative-0.2.1/generative/networks/
--rw-rw-r--   0 walter    (1000) walter    (1000)      573 2022-12-19 11:22:05.000000 monai-generative-0.2.1/generative/networks/__init__.py
-drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-17 16:51:24.304555 monai-generative-0.2.1/generative/networks/blocks/
--rw-rw-r--   0 walter    (1000) walter    (1000)      692 2023-04-09 13:54:59.000000 monai-generative-0.2.1/generative/networks/blocks/__init__.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     5860 2023-04-09 13:54:59.000000 monai-generative-0.2.1/generative/networks/blocks/selfattention.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     3501 2023-04-09 13:54:59.000000 monai-generative-0.2.1/generative/networks/blocks/transformerblock.py
-drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-17 16:51:24.304555 monai-generative-0.2.1/generative/networks/layers/
--rw-rw-r--   0 walter    (1000) walter    (1000)      634 2023-02-10 00:07:32.000000 monai-generative-0.2.1/generative/networks/layers/__init__.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     9742 2023-02-14 11:39:13.000000 monai-generative-0.2.1/generative/networks/layers/vector_quantizer.py
-drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-17 16:51:24.308555 monai-generative-0.2.1/generative/networks/nets/
--rw-rw-r--   0 walter    (1000) walter    (1000)      897 2023-05-17 14:56:31.000000 monai-generative-0.2.1/generative/networks/nets/__init__.py
--rw-rw-r--   0 walter    (1000) walter    (1000)    27823 2023-04-03 20:11:10.000000 monai-generative-0.2.1/generative/networks/nets/autoencoderkl.py
--rw-rw-r--   0 walter    (1000) walter    (1000)    16415 2023-05-17 14:56:31.000000 monai-generative-0.2.1/generative/networks/nets/controlnet.py
--rw-rw-r--   0 walter    (1000) walter    (1000)    79885 2023-05-17 14:56:31.000000 monai-generative-0.2.1/generative/networks/nets/diffusion_model_unet.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     9753 2023-04-02 11:47:15.000000 monai-generative-0.2.1/generative/networks/nets/patchgan_discriminator.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     3981 2023-04-09 13:54:59.000000 monai-generative-0.2.1/generative/networks/nets/transformer.py
--rw-rw-r--   0 walter    (1000) walter    (1000)    17449 2023-03-12 13:56:19.000000 monai-generative-0.2.1/generative/networks/nets/vqvae.py
-drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-17 16:51:24.308555 monai-generative-0.2.1/generative/networks/schedulers/
--rw-rw-r--   0 walter    (1000) walter    (1000)      706 2023-05-17 14:58:43.000000 monai-generative-0.2.1/generative/networks/schedulers/__init__.py
--rw-rw-r--   0 walter    (1000) walter    (1000)    16729 2023-05-17 14:58:43.000000 monai-generative-0.2.1/generative/networks/schedulers/ddim.py
--rw-rw-r--   0 walter    (1000) walter    (1000)    13688 2023-05-17 14:58:43.000000 monai-generative-0.2.1/generative/networks/schedulers/ddpm.py
--rw-rw-r--   0 walter    (1000) walter    (1000)    16592 2023-05-17 14:58:43.000000 monai-generative-0.2.1/generative/networks/schedulers/pndm.py
-drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-17 16:51:24.308555 monai-generative-0.2.1/generative/utils/
--rw-rw-r--   0 walter    (1000) walter    (1000)      673 2023-05-17 14:58:43.000000 monai-generative-0.2.1/generative/utils/__init__.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     2278 2023-03-12 10:31:18.000000 monai-generative-0.2.1/generative/utils/enums.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     8095 2023-03-12 10:31:18.000000 monai-generative-0.2.1/generative/utils/ordering.py
--rw-rw-r--   0 walter    (1000) walter    (1000)      632 2023-05-17 14:56:31.000000 monai-generative-0.2.1/generative/version.py
-drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-17 16:51:24.308555 monai-generative-0.2.1/monai_generative.egg-info/
--rw-rw-r--   0 walter    (1000) walter    (1000)      179 2023-05-17 16:51:24.000000 monai-generative-0.2.1/monai_generative.egg-info/PKG-INFO
--rw-rw-r--   0 walter    (1000) walter    (1000)     2261 2023-05-17 16:51:24.000000 monai-generative-0.2.1/monai_generative.egg-info/SOURCES.txt
--rw-rw-r--   0 walter    (1000) walter    (1000)        1 2023-05-17 16:51:24.000000 monai-generative-0.2.1/monai_generative.egg-info/dependency_links.txt
--rw-rw-r--   0 walter    (1000) walter    (1000)       26 2023-05-17 16:51:24.000000 monai-generative-0.2.1/monai_generative.egg-info/requires.txt
--rw-rw-r--   0 walter    (1000) walter    (1000)       17 2023-05-17 16:51:24.000000 monai-generative-0.2.1/monai_generative.egg-info/top_level.txt
--rw-rw-r--   0 walter    (1000) walter    (1000)     1650 2023-02-19 15:52:11.000000 monai-generative-0.2.1/pyproject.toml
--rw-rw-r--   0 walter    (1000) walter    (1000)     1204 2023-05-17 16:51:24.308555 monai-generative-0.2.1/setup.cfg
--rw-rw-r--   0 walter    (1000) walter    (1000)      913 2023-05-17 16:51:19.000000 monai-generative-0.2.1/setup.py
-drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-17 16:51:24.308555 monai-generative-0.2.1/tests/
--rw-rw-r--   0 walter    (1000) walter    (1000)     1439 2023-02-11 21:51:39.000000 monai-generative-0.2.1/tests/__init__.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     2330 2023-04-02 11:47:15.000000 monai-generative-0.2.1/tests/min_tests.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     5526 2023-04-02 11:47:15.000000 monai-generative-0.2.1/tests/runner.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     4038 2023-04-02 11:47:15.000000 monai-generative-0.2.1/tests/test_adversarial.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     7348 2023-04-02 11:47:15.000000 monai-generative-0.2.1/tests/test_autoencoderkl.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     1201 2023-05-17 14:56:31.000000 monai-generative-0.2.1/tests/test_compute_fid_metric.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     1650 2023-05-17 14:56:31.000000 monai-generative-0.2.1/tests/test_compute_mmd_metric.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     3058 2023-05-17 14:58:43.000000 monai-generative-0.2.1/tests/test_compute_multiscalessim_metric.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     1840 2023-05-17 14:56:31.000000 monai-generative-0.2.1/tests/test_controlnet.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     6719 2023-04-02 11:47:16.000000 monai-generative-0.2.1/tests/test_diffusion_inferer.py
--rw-rw-r--   0 walter    (1000) walter    (1000)    17222 2023-05-17 14:58:43.000000 monai-generative-0.2.1/tests/test_diffusion_model_unet.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     6252 2023-03-12 10:31:18.000000 monai-generative-0.2.1/tests/test_integration_workflows_adversarial.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     9120 2023-03-12 13:56:19.000000 monai-generative-0.2.1/tests/test_latent_diffusion_inferer.py
--rw-rw-r--   0 walter    (1000) walter    (1000)    10326 2023-03-12 10:31:18.000000 monai-generative-0.2.1/tests/test_ordering.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     3350 2023-04-02 11:47:16.000000 monai-generative-0.2.1/tests/test_patch_gan.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     3103 2023-05-17 14:56:31.000000 monai-generative-0.2.1/tests/test_perceptual_loss.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     2848 2023-05-17 14:58:43.000000 monai-generative-0.2.1/tests/test_scheduler_ddim.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     3431 2023-05-17 14:58:43.000000 monai-generative-0.2.1/tests/test_scheduler_ddpm.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     3070 2023-05-17 14:58:43.000000 monai-generative-0.2.1/tests/test_scheduler_pndm.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     2013 2023-04-09 13:54:59.000000 monai-generative-0.2.1/tests/test_selfattention.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     3042 2023-03-12 10:31:18.000000 monai-generative-0.2.1/tests/test_spectral_loss.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     1549 2023-04-09 13:54:59.000000 monai-generative-0.2.1/tests/test_transformer.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     3141 2023-03-12 10:31:18.000000 monai-generative-0.2.1/tests/test_vector_quantizer.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     8331 2023-03-12 13:56:19.000000 monai-generative-0.2.1/tests/test_vqvae.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     9841 2023-04-09 13:54:59.000000 monai-generative-0.2.1/tests/test_vqvaetransformer_inferer.py
--rw-rw-r--   0 walter    (1000) walter    (1000)    30521 2023-04-04 12:39:13.000000 monai-generative-0.2.1/tests/utils.py
+drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-19 12:29:35.797233 monai-generative-0.2.2/
+-rw-rw-r--   0 walter    (1000) walter    (1000)    11357 2022-12-19 11:22:05.000000 monai-generative-0.2.2/LICENSE
+-rw-rw-r--   0 walter    (1000) walter    (1000)      179 2023-05-19 12:29:35.797233 monai-generative-0.2.2/PKG-INFO
+-rw-rw-r--   0 walter    (1000) walter    (1000)     3033 2023-04-04 12:39:13.000000 monai-generative-0.2.2/README.md
+drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-19 12:29:35.793233 monai-generative-0.2.2/generative/
+-rw-rw-r--   0 walter    (1000) walter    (1000)      643 2023-03-12 10:31:18.000000 monai-generative-0.2.2/generative/__init__.py
+drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-19 12:29:35.793233 monai-generative-0.2.2/generative/engines/
+-rw-rw-r--   0 walter    (1000) walter    (1000)      724 2023-04-02 11:47:15.000000 monai-generative-0.2.2/generative/engines/__init__.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     4685 2023-04-02 11:47:15.000000 monai-generative-0.2.2/generative/engines/prepare_batch.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)    16388 2023-03-20 16:09:39.000000 monai-generative-0.2.2/generative/engines/trainer.py
+drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-19 12:29:35.793233 monai-generative-0.2.2/generative/inferers/
+-rw-rw-r--   0 walter    (1000) walter    (1000)      697 2023-03-12 10:31:18.000000 monai-generative-0.2.2/generative/inferers/__init__.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)    27940 2023-04-09 13:54:59.000000 monai-generative-0.2.2/generative/inferers/inferer.py
+drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-19 12:29:35.793233 monai-generative-0.2.2/generative/losses/
+-rw-rw-r--   0 walter    (1000) walter    (1000)      739 2023-04-02 11:47:15.000000 monai-generative-0.2.2/generative/losses/__init__.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     7671 2023-05-17 14:56:31.000000 monai-generative-0.2.2/generative/losses/adversarial_loss.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)    16409 2023-05-17 14:56:31.000000 monai-generative-0.2.2/generative/losses/perceptual.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     3366 2023-03-12 10:31:18.000000 monai-generative-0.2.2/generative/losses/spectral_loss.py
+drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-19 12:29:35.793233 monai-generative-0.2.2/generative/metrics/
+-rw-rw-r--   0 walter    (1000) walter    (1000)      735 2023-05-17 14:56:31.000000 monai-generative-0.2.2/generative/metrics/__init__.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     4500 2023-04-09 13:54:59.000000 monai-generative-0.2.2/generative/metrics/fid.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     3206 2023-05-17 14:56:31.000000 monai-generative-0.2.2/generative/metrics/mmd.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     6399 2023-04-09 13:54:59.000000 monai-generative-0.2.2/generative/metrics/ms_ssim.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     9494 2023-04-09 13:54:59.000000 monai-generative-0.2.2/generative/metrics/ssim.py
+drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-19 12:29:35.793233 monai-generative-0.2.2/generative/networks/
+-rw-rw-r--   0 walter    (1000) walter    (1000)      573 2022-12-19 11:22:05.000000 monai-generative-0.2.2/generative/networks/__init__.py
+drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-19 12:29:35.793233 monai-generative-0.2.2/generative/networks/blocks/
+-rw-rw-r--   0 walter    (1000) walter    (1000)      692 2023-04-09 13:54:59.000000 monai-generative-0.2.2/generative/networks/blocks/__init__.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     5860 2023-04-09 13:54:59.000000 monai-generative-0.2.2/generative/networks/blocks/selfattention.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     3501 2023-04-09 13:54:59.000000 monai-generative-0.2.2/generative/networks/blocks/transformerblock.py
+drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-19 12:29:35.793233 monai-generative-0.2.2/generative/networks/layers/
+-rw-rw-r--   0 walter    (1000) walter    (1000)      634 2023-02-10 00:07:32.000000 monai-generative-0.2.2/generative/networks/layers/__init__.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     9742 2023-02-14 11:39:13.000000 monai-generative-0.2.2/generative/networks/layers/vector_quantizer.py
+drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-19 12:29:35.793233 monai-generative-0.2.2/generative/networks/nets/
+-rw-rw-r--   0 walter    (1000) walter    (1000)      897 2023-05-17 14:56:31.000000 monai-generative-0.2.2/generative/networks/nets/__init__.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)    27823 2023-04-03 20:11:10.000000 monai-generative-0.2.2/generative/networks/nets/autoencoderkl.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)    16415 2023-05-17 14:56:31.000000 monai-generative-0.2.2/generative/networks/nets/controlnet.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)    79885 2023-05-17 14:56:31.000000 monai-generative-0.2.2/generative/networks/nets/diffusion_model_unet.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     9753 2023-04-02 11:47:15.000000 monai-generative-0.2.2/generative/networks/nets/patchgan_discriminator.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     3981 2023-04-09 13:54:59.000000 monai-generative-0.2.2/generative/networks/nets/transformer.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)    17449 2023-03-12 13:56:19.000000 monai-generative-0.2.2/generative/networks/nets/vqvae.py
+drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-19 12:29:35.793233 monai-generative-0.2.2/generative/networks/schedulers/
+-rw-rw-r--   0 walter    (1000) walter    (1000)      755 2023-05-17 18:09:35.000000 monai-generative-0.2.2/generative/networks/schedulers/__init__.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)    13691 2023-05-17 18:09:35.000000 monai-generative-0.2.2/generative/networks/schedulers/ddim.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)    10840 2023-05-17 18:09:35.000000 monai-generative-0.2.2/generative/networks/schedulers/ddpm.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)    14441 2023-05-17 18:09:35.000000 monai-generative-0.2.2/generative/networks/schedulers/pndm.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     9103 2023-05-17 18:09:35.000000 monai-generative-0.2.2/generative/networks/schedulers/scheduler.py
+drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-19 12:29:35.793233 monai-generative-0.2.2/generative/utils/
+-rw-rw-r--   0 walter    (1000) walter    (1000)      767 2023-05-17 18:09:35.000000 monai-generative-0.2.2/generative/utils/__init__.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     4319 2023-05-17 18:09:35.000000 monai-generative-0.2.2/generative/utils/component_store.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     2278 2023-03-12 10:31:18.000000 monai-generative-0.2.2/generative/utils/enums.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     1023 2023-05-17 18:09:35.000000 monai-generative-0.2.2/generative/utils/misc.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     8095 2023-03-12 10:31:18.000000 monai-generative-0.2.2/generative/utils/ordering.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)      632 2023-05-19 12:02:06.000000 monai-generative-0.2.2/generative/version.py
+drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-19 12:29:35.793233 monai-generative-0.2.2/monai_generative.egg-info/
+-rw-rw-r--   0 walter    (1000) walter    (1000)      179 2023-05-19 12:29:35.000000 monai-generative-0.2.2/monai_generative.egg-info/PKG-INFO
+-rw-rw-r--   0 walter    (1000) walter    (1000)     2415 2023-05-19 12:29:35.000000 monai-generative-0.2.2/monai_generative.egg-info/SOURCES.txt
+-rw-rw-r--   0 walter    (1000) walter    (1000)        1 2023-05-19 12:29:35.000000 monai-generative-0.2.2/monai_generative.egg-info/dependency_links.txt
+-rw-rw-r--   0 walter    (1000) walter    (1000)       16 2023-05-19 12:29:35.000000 monai-generative-0.2.2/monai_generative.egg-info/requires.txt
+-rw-rw-r--   0 walter    (1000) walter    (1000)       17 2023-05-19 12:29:35.000000 monai-generative-0.2.2/monai_generative.egg-info/top_level.txt
+-rw-rw-r--   0 walter    (1000) walter    (1000)     1650 2023-02-19 15:52:11.000000 monai-generative-0.2.2/pyproject.toml
+-rw-rw-r--   0 walter    (1000) walter    (1000)     1204 2023-05-19 12:29:35.797233 monai-generative-0.2.2/setup.cfg
+-rw-rw-r--   0 walter    (1000) walter    (1000)      903 2023-05-19 12:29:31.000000 monai-generative-0.2.2/setup.py
+drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2023-05-19 12:29:35.797233 monai-generative-0.2.2/tests/
+-rw-rw-r--   0 walter    (1000) walter    (1000)     1439 2023-02-11 21:51:39.000000 monai-generative-0.2.2/tests/__init__.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     2330 2023-04-02 11:47:15.000000 monai-generative-0.2.2/tests/min_tests.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     5526 2023-04-02 11:47:15.000000 monai-generative-0.2.2/tests/runner.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     4038 2023-04-02 11:47:15.000000 monai-generative-0.2.2/tests/test_adversarial.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     7348 2023-04-02 11:47:15.000000 monai-generative-0.2.2/tests/test_autoencoderkl.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     2393 2023-05-17 18:09:35.000000 monai-generative-0.2.2/tests/test_component_store.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     1201 2023-05-17 14:56:31.000000 monai-generative-0.2.2/tests/test_compute_fid_metric.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     1650 2023-05-17 14:56:31.000000 monai-generative-0.2.2/tests/test_compute_mmd_metric.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     3090 2023-05-17 18:09:35.000000 monai-generative-0.2.2/tests/test_compute_multiscalessim_metric.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     1840 2023-05-17 14:56:31.000000 monai-generative-0.2.2/tests/test_controlnet.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     6719 2023-04-02 11:47:16.000000 monai-generative-0.2.2/tests/test_diffusion_inferer.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)    17136 2023-05-17 18:09:35.000000 monai-generative-0.2.2/tests/test_diffusion_model_unet.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     6252 2023-03-12 10:31:18.000000 monai-generative-0.2.2/tests/test_integration_workflows_adversarial.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     9120 2023-03-12 13:56:19.000000 monai-generative-0.2.2/tests/test_latent_diffusion_inferer.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     1715 2023-05-17 18:09:35.000000 monai-generative-0.2.2/tests/test_misc.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)    10326 2023-03-12 10:31:18.000000 monai-generative-0.2.2/tests/test_ordering.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     3350 2023-04-02 11:47:16.000000 monai-generative-0.2.2/tests/test_patch_gan.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     3103 2023-05-17 14:56:31.000000 monai-generative-0.2.2/tests/test_perceptual_loss.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     2858 2023-05-17 18:09:35.000000 monai-generative-0.2.2/tests/test_scheduler_ddim.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     3895 2023-05-17 18:09:35.000000 monai-generative-0.2.2/tests/test_scheduler_ddpm.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     3080 2023-05-17 18:09:35.000000 monai-generative-0.2.2/tests/test_scheduler_pndm.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     2013 2023-04-09 13:54:59.000000 monai-generative-0.2.2/tests/test_selfattention.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     3042 2023-03-12 10:31:18.000000 monai-generative-0.2.2/tests/test_spectral_loss.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     1549 2023-04-09 13:54:59.000000 monai-generative-0.2.2/tests/test_transformer.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     3141 2023-03-12 10:31:18.000000 monai-generative-0.2.2/tests/test_vector_quantizer.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     8331 2023-03-12 13:56:19.000000 monai-generative-0.2.2/tests/test_vqvae.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     9841 2023-04-09 13:54:59.000000 monai-generative-0.2.2/tests/test_vqvaetransformer_inferer.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)    30521 2023-04-04 12:39:13.000000 monai-generative-0.2.2/tests/utils.py
```

### Comparing `monai-generative-0.2.1/LICENSE` & `monai-generative-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/README.md` & `monai-generative-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/__init__.py` & `monai-generative-0.2.2/generative/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/engines/__init__.py` & `monai-generative-0.2.2/generative/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/engines/prepare_batch.py` & `monai-generative-0.2.2/generative/engines/prepare_batch.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/engines/trainer.py` & `monai-generative-0.2.2/generative/engines/trainer.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/inferers/__init__.py` & `monai-generative-0.2.2/generative/inferers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/inferers/inferer.py` & `monai-generative-0.2.2/generative/inferers/inferer.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/losses/__init__.py` & `monai-generative-0.2.2/generative/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/losses/adversarial_loss.py` & `monai-generative-0.2.2/generative/losses/adversarial_loss.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/losses/perceptual.py` & `monai-generative-0.2.2/generative/losses/perceptual.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/losses/spectral_loss.py` & `monai-generative-0.2.2/generative/losses/spectral_loss.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/metrics/__init__.py` & `monai-generative-0.2.2/generative/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/metrics/fid.py` & `monai-generative-0.2.2/generative/metrics/fid.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/metrics/mmd.py` & `monai-generative-0.2.2/generative/metrics/mmd.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/metrics/ms_ssim.py` & `monai-generative-0.2.2/generative/metrics/ms_ssim.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/metrics/ssim.py` & `monai-generative-0.2.2/generative/metrics/ssim.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/networks/__init__.py` & `monai-generative-0.2.2/generative/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/networks/blocks/__init__.py` & `monai-generative-0.2.2/generative/networks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/networks/blocks/selfattention.py` & `monai-generative-0.2.2/generative/networks/blocks/selfattention.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/networks/blocks/transformerblock.py` & `monai-generative-0.2.2/generative/networks/blocks/transformerblock.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/networks/layers/__init__.py` & `monai-generative-0.2.2/generative/networks/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/networks/layers/vector_quantizer.py` & `monai-generative-0.2.2/generative/networks/layers/vector_quantizer.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/networks/nets/__init__.py` & `monai-generative-0.2.2/generative/networks/nets/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/networks/nets/autoencoderkl.py` & `monai-generative-0.2.2/generative/networks/nets/autoencoderkl.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/networks/nets/controlnet.py` & `monai-generative-0.2.2/generative/networks/nets/controlnet.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/networks/nets/diffusion_model_unet.py` & `monai-generative-0.2.2/generative/networks/nets/diffusion_model_unet.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/networks/nets/patchgan_discriminator.py` & `monai-generative-0.2.2/generative/networks/nets/patchgan_discriminator.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/networks/nets/transformer.py` & `monai-generative-0.2.2/generative/networks/nets/transformer.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/networks/nets/vqvae.py` & `monai-generative-0.2.2/generative/networks/nets/vqvae.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/networks/schedulers/__init__.py` & `monai-generative-0.2.2/generative/networks/schedulers/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,7 +10,8 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 from .ddim import DDIMScheduler
 from .ddpm import DDPMScheduler
 from .pndm import PNDMScheduler
+from .scheduler import NoiseSchedules, Scheduler
```

### Comparing `monai-generative-0.2.1/generative/networks/schedulers/ddim.py` & `monai-generative-0.2.2/generative/networks/schedulers/ddim.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,91 +29,87 @@
 # limitations under the License.
 # =========================================================================
 
 from __future__ import annotations
 
 import numpy as np
 import torch
-import torch.nn as nn
+from monai.utils import StrEnum
 
+from .scheduler import Scheduler
 
-class DDIMScheduler(nn.Module):
+
+class DDIMPredictionType(StrEnum):
+    """
+    Set of valid prediction type names for the DDIM scheduler's `prediction_type` argument.
+
+    epsilon: predicting the noise of the diffusion process
+    sample: directly predicting the noisy sample
+    v_prediction: velocity prediction, see section 2.4 https://imagen.research.google/video/paper.pdf
+    """
+
+    EPSILON = "epsilon"
+    SAMPLE = "sample"
+    V_PREDICTION = "v_prediction"
+
+
+class DDIMScheduler(Scheduler):
     """
     Denoising diffusion implicit models is a scheduler that extends the denoising procedure introduced in denoising
     diffusion probabilistic models (DDPMs) with non-Markovian guidance. Based on: Song et al. "Denoising Diffusion
     Implicit Models" https://arxiv.org/abs/2010.02502
 
     Args:
         num_train_timesteps: number of diffusion steps used to train the model.
-        beta_start: the starting `beta` value of inference.
-        beta_end: the final `beta` value.
-        beta_schedule: {``"linear"``, ``"scaled_linear"``}
-            the beta schedule, a mapping from a beta range to a sequence of betas for stepping the model.
+        schedule: member of NoiseSchedules, name of noise schedule function in component store
         clip_sample: option to clip predicted sample between -1 and 1 for numerical stability.
         set_alpha_to_one: each diffusion step uses the value of alphas product at that step and at the previous one.
             For the final step there is no previous alpha. When this option is `True` the previous alpha product is
             fixed to `1`, otherwise it uses the value of alpha at step 0.
         steps_offset: an offset added to the inference steps. You can use a combination of `steps_offset=1` and
             `set_alpha_to_one=False`, to make the last step use step 0 for the previous alpha product, as done in
             stable diffusion.
-        prediction_type: {``"epsilon"``, ``"sample"``, ``"v_prediction"``}
-            prediction type of the scheduler function, one of `epsilon` (predicting the noise of the diffusion
-            process), `sample` (directly predicting the noisy sample`) or `v_prediction` (see section 2.4
-            https://imagen.research.google/video/paper.pdf)
+        prediction_type: member of DDPMPredictionType
+        schedule_args: arguments to pass to the schedule function
+
     """
 
     def __init__(
         self,
         num_train_timesteps: int = 1000,
-        beta_start: float = 1e-4,
-        beta_end: float = 2e-2,
-        beta_schedule: str = "linear",
+        schedule: str = "linear_beta",
         clip_sample: bool = True,
         set_alpha_to_one: bool = True,
         steps_offset: int = 0,
-        prediction_type: str = "epsilon",
+        prediction_type: str = DDIMPredictionType.EPSILON,
+        **schedule_args,
     ) -> None:
-        super().__init__()
-        self.beta_schedule = beta_schedule
-        if beta_schedule == "linear":
-            self.betas = torch.linspace(beta_start, beta_end, num_train_timesteps, dtype=torch.float32)
-        elif beta_schedule == "scaled_linear":
-            # this schedule is very specific to the latent diffusion model.
-            self.betas = (
-                torch.linspace(beta_start**0.5, beta_end**0.5, num_train_timesteps, dtype=torch.float32) ** 2
-            )
-        else:
-            raise NotImplementedError(f"{beta_schedule} does is not implemented for {self.__class__}")
+        super().__init__(num_train_timesteps, schedule, **schedule_args)
 
-        if prediction_type.lower() not in ["epsilon", "sample", "v_prediction"]:
-            raise ValueError(
-                f"prediction_type given as {prediction_type} must be one of `epsilon`, `sample`, or" " `v_prediction`"
-            )
+        if prediction_type not in DDIMPredictionType.__members__.values():
+            raise ValueError("Argument `prediction_type` must be a member of DDIMPredictionType")
 
         self.prediction_type = prediction_type
-        self.num_train_timesteps = num_train_timesteps
-        self.alphas = 1.0 - self.betas
-        self.alphas_cumprod = torch.cumprod(self.alphas, dim=0)
 
         # At every step in ddim, we are looking into the previous alphas_cumprod
         # For the final step, there is no previous alphas_cumprod because we are already at 0
         # `set_alpha_to_one` decides whether we set this parameter simply to one or
         # whether we use the final alpha of the "non-previous" one.
         self.final_alpha_cumprod = torch.tensor(1.0) if set_alpha_to_one else self.alphas_cumprod[0]
 
         # standard deviation of the initial noise distribution
         self.init_noise_sigma = 1.0
 
-        self.timesteps = torch.from_numpy(np.arange(0, num_train_timesteps)[::-1].astype(np.int64))
+        self.timesteps = torch.from_numpy(np.arange(0, self.num_train_timesteps)[::-1].astype(np.int64))
 
         self.clip_sample = clip_sample
         self.steps_offset = steps_offset
 
         # default the number of inference timesteps to the number of train steps
-        self.set_timesteps(num_train_timesteps)
+        self.set_timesteps(self.num_train_timesteps)
 
     def set_timesteps(self, num_inference_steps: int, device: str | torch.device | None = None) -> None:
         """
         Sets the discrete timesteps used for the diffusion chain. Supporting function to be run before inference.
 
         Args:
             num_inference_steps: number of diffusion steps used when generating samples with a pre-trained model.
@@ -186,44 +182,44 @@
         alpha_prod_t = self.alphas_cumprod[timestep]
         alpha_prod_t_prev = self.alphas_cumprod[prev_timestep] if prev_timestep >= 0 else self.final_alpha_cumprod
 
         beta_prod_t = 1 - alpha_prod_t
 
         # 3. compute predicted original sample from predicted noise also called
         # "predicted x_0" of formula (12) from https://arxiv.org/pdf/2010.02502.pdf
-        if self.prediction_type == "epsilon":
-            pred_original_sample = (sample - beta_prod_t ** (0.5) * model_output) / alpha_prod_t ** (0.5)
+        if self.prediction_type == DDIMPredictionType.EPSILON:
+            pred_original_sample = (sample - (beta_prod_t**0.5) * model_output) / (alpha_prod_t**0.5)
             pred_epsilon = model_output
-        elif self.prediction_type == "sample":
+        elif self.prediction_type == DDIMPredictionType.SAMPLE:
             pred_original_sample = model_output
-            pred_epsilon = (sample - alpha_prod_t ** (0.5) * pred_original_sample) / beta_prod_t ** (0.5)
-        elif self.prediction_type == "v_prediction":
+            pred_epsilon = (sample - (alpha_prod_t**0.5) * pred_original_sample) / (beta_prod_t**0.5)
+        elif self.prediction_type == DDIMPredictionType.V_PREDICTION:
             pred_original_sample = (alpha_prod_t**0.5) * sample - (beta_prod_t**0.5) * model_output
             pred_epsilon = (alpha_prod_t**0.5) * model_output + (beta_prod_t**0.5) * sample
 
         # 4. Clip "predicted x_0"
         if self.clip_sample:
             pred_original_sample = torch.clamp(pred_original_sample, -1, 1)
 
         # 5. compute variance: "sigma_t(η)" -> see formula (16)
         # σ_t = sqrt((1 − α_t−1)/(1 − α_t)) * sqrt(1 − α_t/α_t−1)
         variance = self._get_variance(timestep, prev_timestep)
-        std_dev_t = eta * variance ** (0.5)
+        std_dev_t = eta * variance**0.5
 
         # 6. compute "direction pointing to x_t" of formula (12) from https://arxiv.org/pdf/2010.02502.pdf
-        pred_sample_direction = (1 - alpha_prod_t_prev - std_dev_t**2) ** (0.5) * pred_epsilon
+        pred_sample_direction = (1 - alpha_prod_t_prev - std_dev_t**2) ** 0.5 * pred_epsilon
 
         # 7. compute x_t-1 without "random noise" of formula (12) from https://arxiv.org/pdf/2010.02502.pdf
-        pred_prev_sample = alpha_prod_t_prev ** (0.5) * pred_original_sample + pred_sample_direction
+        pred_prev_sample = alpha_prod_t_prev**0.5 * pred_original_sample + pred_sample_direction
 
         if eta > 0:
             # randn_like does not support generator https://github.com/pytorch/pytorch/issues/27072
             device = model_output.device if torch.is_tensor(model_output) else "cpu"
             noise = torch.randn(model_output.shape, dtype=model_output.dtype, generator=generator).to(device)
-            variance = self._get_variance(timestep, prev_timestep) ** (0.5) * eta * noise
+            variance = self._get_variance(timestep, prev_timestep) ** 0.5 * eta * noise
 
             pred_prev_sample = pred_prev_sample + variance
 
         return pred_prev_sample, pred_original_sample
 
     def reversed_step(
         self, model_output: torch.Tensor, timestep: int, sample: torch.Tensor
@@ -259,75 +255,28 @@
         alpha_prod_t_prev = self.alphas_cumprod[prev_timestep] if prev_timestep >= 0 else self.final_alpha_cumprod
 
         beta_prod_t = 1 - alpha_prod_t
 
         # 3. compute predicted original sample from predicted noise also called
         # "predicted x_0" of formula (12) from https://arxiv.org/pdf/2010.02502.pdf
 
-        if self.prediction_type == "epsilon":
+        if self.prediction_type == DDIMPredictionType.EPSILON:
             pred_original_sample = (sample - beta_prod_t ** (0.5) * model_output) / alpha_prod_t ** (0.5)
             pred_epsilon = model_output
-        elif self.prediction_type == "sample":
+        elif self.prediction_type == DDIMPredictionType.SAMPLE:
             pred_original_sample = model_output
             pred_epsilon = (sample - alpha_prod_t ** (0.5) * pred_original_sample) / beta_prod_t ** (0.5)
-        elif self.prediction_type == "v_prediction":
+        elif self.prediction_type == DDIMPredictionType.V_PREDICTION:
             pred_original_sample = (alpha_prod_t**0.5) * sample - (beta_prod_t**0.5) * model_output
             pred_epsilon = (alpha_prod_t**0.5) * model_output + (beta_prod_t**0.5) * sample
 
         # 4. Clip "predicted x_0"
         if self.clip_sample:
             pred_original_sample = torch.clamp(pred_original_sample, -1, 1)
 
         # 5. compute "direction pointing to x_t" of formula (12) from https://arxiv.org/pdf/2010.02502.pdf
         pred_sample_direction = (1 - alpha_prod_t_prev) ** (0.5) * pred_epsilon
 
         # 6. compute x_t+1 without "random noise" of formula (12) from https://arxiv.org/pdf/2010.02502.pdf
         pred_post_sample = alpha_prod_t_prev ** (0.5) * pred_original_sample + pred_sample_direction
 
         return pred_post_sample, pred_original_sample
-
-    def add_noise(self, original_samples: torch.Tensor, noise: torch.Tensor, timesteps: torch.Tensor) -> torch.Tensor:
-        """
-        Add noise to the original samples.
-
-        Args:
-            original_samples: original samples
-            noise: noise to add to samples
-            timesteps: timesteps tensor indicating the timestep to be computed for each sample.
-
-        Returns:
-            noisy_samples: sample with added noise
-        """
-        # Make sure alphas_cumprod and timestep have same device and dtype as original_samples
-        self.alphas_cumprod = self.alphas_cumprod.to(device=original_samples.device, dtype=original_samples.dtype)
-        timesteps = timesteps.to(original_samples.device)
-
-        sqrt_alpha_cumprod = self.alphas_cumprod[timesteps] ** 0.5
-        sqrt_alpha_cumprod = sqrt_alpha_cumprod.flatten()
-        while len(sqrt_alpha_cumprod.shape) < len(original_samples.shape):
-            sqrt_alpha_cumprod = sqrt_alpha_cumprod.unsqueeze(-1)
-
-        sqrt_one_minus_alpha_prod = (1 - self.alphas_cumprod[timesteps]) ** 0.5
-        sqrt_one_minus_alpha_prod = sqrt_one_minus_alpha_prod.flatten()
-        while len(sqrt_one_minus_alpha_prod.shape) < len(original_samples.shape):
-            sqrt_one_minus_alpha_prod = sqrt_one_minus_alpha_prod.unsqueeze(-1)
-
-        noisy_samples = sqrt_alpha_cumprod * original_samples + sqrt_one_minus_alpha_prod * noise
-        return noisy_samples
-
-    def get_velocity(self, sample: torch.Tensor, noise: torch.Tensor, timesteps: torch.Tensor) -> torch.Tensor:
-        # Make sure alphas_cumprod and timestep have same device and dtype as sample
-        self.alphas_cumprod = self.alphas_cumprod.to(device=sample.device, dtype=sample.dtype)
-        timesteps = timesteps.to(sample.device)
-
-        sqrt_alpha_prod = self.alphas_cumprod[timesteps] ** 0.5
-        sqrt_alpha_prod = sqrt_alpha_prod.flatten()
-        while len(sqrt_alpha_prod.shape) < len(sample.shape):
-            sqrt_alpha_prod = sqrt_alpha_prod.unsqueeze(-1)
-
-        sqrt_one_minus_alpha_prod = (1 - self.alphas_cumprod[timesteps]) ** 0.5
-        sqrt_one_minus_alpha_prod = sqrt_one_minus_alpha_prod.flatten()
-        while len(sqrt_one_minus_alpha_prod.shape) < len(sample.shape):
-            sqrt_one_minus_alpha_prod = sqrt_one_minus_alpha_prod.unsqueeze(-1)
-
-        velocity = sqrt_alpha_prod * noise - sqrt_one_minus_alpha_prod * sample
-        return velocity
```

### Comparing `monai-generative-0.2.1/generative/networks/schedulers/ddpm.py` & `monai-generative-0.2.2/generative/networks/schedulers/pndm.py`

 * *Files 24% similar despite different names*

```diff
@@ -27,80 +27,97 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========================================================================
 
 from __future__ import annotations
 
+from typing import Any
+
 import numpy as np
 import torch
-import torch.nn as nn
+from monai.utils import StrEnum
+
+from .scheduler import Scheduler
+
+
+class PNDMPredictionType(StrEnum):
+    """
+    Set of valid prediction type names for the PNDM scheduler's `prediction_type` argument.
+
+    epsilon: predicting the noise of the diffusion process
+    v_prediction: velocity prediction, see section 2.4 https://imagen.research.google/video/paper.pdf
+    """
+
+    EPSILON = "epsilon"
+    V_PREDICTION = "v_prediction"
 
 
-class DDPMScheduler(nn.Module):
+class PNDMScheduler(Scheduler):
     """
-    Denoising diffusion probabilistic models (DDPMs) explores the connections between denoising score matching and
-    Langevin dynamics sampling. Based on: Ho et al., "Denoising Diffusion Probabilistic Models"
-    https://arxiv.org/abs/2006.11239
+    Pseudo numerical methods for diffusion models (PNDM) proposes using more advanced ODE integration techniques,
+    namely Runge-Kutta method and a linear multi-step method. Based on: Liu et al.,
+    "Pseudo Numerical Methods for Diffusion Models on Manifolds"  https://arxiv.org/abs/2202.09778
 
     Args:
         num_train_timesteps: number of diffusion steps used to train the model.
-        beta_start: the starting `beta` value of inference.
-        beta_end: the final `beta` value.
-        beta_schedule: {``"linear"``, ``"scaled_linear"``}
-            the beta schedule, a mapping from a beta range to a sequence of betas for stepping the model.
-        variance_type: {``"fixed_small"``, ``"fixed_large"``, ``"learned"``, ``"learned_range"``}
-            options to clip the variance used when adding noise to the denoised sample.
-        clip_sample: option to clip predicted sample between -1 and 1 for numerical stability.
-        prediction_type: {``"epsilon"``, ``"sample"``, ``"v_prediction"``}
-            prediction type of the scheduler function, one of `epsilon` (predicting the noise of the diffusion
-            process), `sample` (directly predicting the noisy sample`) or `v_prediction` (see section 2.4
-            https://imagen.research.google/video/paper.pdf)
+        schedule: member of NoiseSchedules, name of noise schedule function in component store
+        skip_prk_steps:
+            allows the scheduler to skip the Runge-Kutta steps that are defined in the original paper as being required
+            before plms step.
+        set_alpha_to_one:
+            each diffusion step uses the value of alphas product at that step and at the previous one. For the final
+            step there is no previous alpha. When this option is `True` the previous alpha product is fixed to `1`,
+            otherwise it uses the value of alpha at step 0.
+        prediction_type: member of DDPMPredictionType
+        steps_offset:
+            an offset added to the inference steps. You can use a combination of `offset=1` and
+            `set_alpha_to_one=False`, to make the last step use step 0 for the previous alpha product, as done in
+            stable diffusion.
+        schedule_args: arguments to pass to the schedule function
     """
 
     def __init__(
         self,
         num_train_timesteps: int = 1000,
-        beta_start: float = 1e-4,
-        beta_end: float = 2e-2,
-        beta_schedule: str = "linear",
-        variance_type: str = "fixed_small",
-        clip_sample: bool = True,
-        prediction_type: str = "epsilon",
+        schedule: str = "linear_beta",
+        skip_prk_steps: bool = False,
+        set_alpha_to_one: bool = False,
+        prediction_type: str = PNDMPredictionType.EPSILON,
+        steps_offset: int = 0,
+        **schedule_args,
     ) -> None:
-        super().__init__()
-        self.beta_schedule = beta_schedule
-        if beta_schedule == "linear":
-            self.betas = torch.linspace(beta_start, beta_end, num_train_timesteps, dtype=torch.float32)
-        elif beta_schedule == "scaled_linear":
-            # this schedule is very specific to the latent diffusion model.
-            self.betas = (
-                torch.linspace(beta_start**0.5, beta_end**0.5, num_train_timesteps, dtype=torch.float32) ** 2
-            )
-        else:
-            raise NotImplementedError(f"{beta_schedule} does is not implemented for {self.__class__}")
+        super().__init__(num_train_timesteps, schedule, **schedule_args)
 
-        if prediction_type.lower() not in ["epsilon", "sample", "v_prediction"]:
-            raise ValueError(
-                f"prediction_type given as {prediction_type} must be one of `epsilon`, `sample`, or" " `v_prediction`"
-            )
+        if prediction_type not in PNDMPredictionType.__members__.values():
+            raise ValueError("Argument `prediction_type` must be a member of PNDMPredictionType")
 
         self.prediction_type = prediction_type
 
-        self.num_train_timesteps = num_train_timesteps
-        self.alphas = 1.0 - self.betas
-        self.alphas_cumprod = torch.cumprod(self.alphas, dim=0)
-        self.one = torch.tensor(1.0)
-
-        self.clip_sample = clip_sample
-        self.variance_type = variance_type
-
-        # settable values
-        self.num_inference_steps = None
-        self.timesteps = torch.from_numpy(np.arange(0, num_train_timesteps)[::-1].copy())
+        self.final_alpha_cumprod = torch.tensor(1.0) if set_alpha_to_one else self.alphas_cumprod[0]
+
+        # standard deviation of the initial noise distribution
+        self.init_noise_sigma = 1.0
+
+        # For now we only support F-PNDM, i.e. the runge-kutta method
+        # For more information on the algorithm please take a look at the paper: https://arxiv.org/pdf/2202.09778.pdf
+        # mainly at formula (9), (12), (13) and the Algorithm 2.
+        self.pndm_order = 4
+
+        self.skip_prk_steps = skip_prk_steps
+        self.steps_offset = steps_offset
+
+        # running values
+        self.cur_model_output = 0
+        self.counter = 0
+        self.cur_sample = None
+        self.ets = []
+
+        # default the number of inference timesteps to the number of train steps
+        self.set_timesteps(num_train_timesteps)
 
     def set_timesteps(self, num_inference_steps: int, device: str | torch.device | None = None) -> None:
         """
         Sets the discrete timesteps used for the diffusion chain. Supporting function to be run before inference.
 
         Args:
             num_inference_steps: number of diffusion steps used when generating samples with a pre-trained model.
@@ -113,175 +130,188 @@
                 f" maximal {self.num_train_timesteps} timesteps."
             )
 
         self.num_inference_steps = num_inference_steps
         step_ratio = self.num_train_timesteps // self.num_inference_steps
         # creates integer timesteps by multiplying by ratio
         # casting to int to avoid issues when num_inference_step is power of 3
-        timesteps = (np.arange(0, num_inference_steps) * step_ratio).round()[::-1].astype(np.int64)
+        self._timesteps = (np.arange(0, num_inference_steps) * step_ratio).round().astype(np.int64)
+        self._timesteps += self.steps_offset
+
+        if self.skip_prk_steps:
+            # for some models like stable diffusion the prk steps can/should be skipped to
+            # produce better results. When using PNDM with `self.skip_prk_steps` the implementation
+            # is based on crowsonkb's PLMS sampler implementation: https://github.com/CompVis/latent-diffusion/pull/51
+            self.prk_timesteps = np.array([])
+            self.plms_timesteps = self._timesteps[::-1]
+
+        else:
+            prk_timesteps = np.array(self._timesteps[-self.pndm_order :]).repeat(2) + np.tile(
+                np.array([0, self.num_train_timesteps // num_inference_steps // 2]), self.pndm_order
+            )
+            self.prk_timesteps = (prk_timesteps[:-1].repeat(2)[1:-1])[::-1].copy()
+            self.plms_timesteps = self._timesteps[:-3][
+                ::-1
+            ].copy()  # we copy to avoid having negative strides which are not supported by torch.from_numpy
+
+        timesteps = np.concatenate([self.prk_timesteps, self.plms_timesteps]).astype(np.int64)
         self.timesteps = torch.from_numpy(timesteps).to(device)
+        # update num_inference_steps - necessary if we use prk steps
+        self.num_inference_steps = len(self.timesteps)
 
-    def _get_mean(self, timestep: int, x_0: torch.Tensor, x_t: torch.Tensor) -> torch.Tensor:
+        self.ets = []
+        self.counter = 0
+
+    def step(
+        self, model_output: torch.FloatTensor, timestep: int, sample: torch.FloatTensor
+    ) -> tuple[torch.Tensor, Any]:
         """
-        Compute the mean of the posterior at timestep t.
+        Predict the sample at the previous timestep by reversing the SDE. Core function to propagate the diffusion
+        process from the learned model outputs (most often the predicted noise).
+        This function calls `step_prk()` or `step_plms()` depending on the internal variable `counter`.
 
         Args:
-            timestep: current timestep.
-            x0: the noise-free input.
-            x_t: the input noised to timestep t.
-
+            model_output: direct output from learned diffusion model.
+            timestep: current discrete timestep in the diffusion chain.
+            sample: current instance of sample being created by diffusion process.
         Returns:
-            Returns the mean
+            pred_prev_sample: Predicted previous sample
         """
-        # these attributes are used for calculating the posterior, q(x_{t-1}|x_t,x_0),
-        # (see formula (5-7) from https://arxiv.org/pdf/2006.11239.pdf)
-        alpha_t = self.alphas[timestep]
-        alpha_prod_t = self.alphas_cumprod[timestep]
-        alpha_prod_t_prev = self.alphas_cumprod[timestep - 1] if timestep > 0 else self.one
-
-        x_0_coefficient = alpha_prod_t_prev.sqrt() * self.betas[timestep] / (1 - alpha_prod_t)
-        x_t_coefficient = alpha_t.sqrt() * (1 - alpha_prod_t_prev) / (1 - alpha_prod_t)
-
-        mean = x_0_coefficient * x_0 + x_t_coefficient * x_t
+        # return a tuple for consistency with samplers that return (previous pred, original sample pred)
 
-        return mean
+        if self.counter < len(self.prk_timesteps) and not self.skip_prk_steps:
+            return self.step_prk(model_output=model_output, timestep=timestep, sample=sample), None
+        else:
+            return self.step_plms(model_output=model_output, timestep=timestep, sample=sample), None
 
-    def _get_variance(self, timestep: int, predicted_variance: torch.Tensor | None = None) -> torch.Tensor:
+    def step_prk(self, model_output: torch.FloatTensor, timestep: int, sample: torch.FloatTensor) -> torch.Tensor:
         """
-        Compute the variance of the posterior at timestep t.
+        Step function propagating the sample with the Runge-Kutta method. RK takes 4 forward passes to approximate the
+        solution to the differential equation.
 
         Args:
-            timestep: current timestep.
-            predicted_variance: variance predicted by the model.
+            model_output: direct output from learned diffusion model.
+            timestep: current discrete timestep in the diffusion chain.
+            sample: current instance of sample being created by diffusion process.
 
         Returns:
-            Returns the variance
+            pred_prev_sample: Predicted previous sample
         """
-        alpha_prod_t = self.alphas_cumprod[timestep]
-        alpha_prod_t_prev = self.alphas_cumprod[timestep - 1] if timestep > 0 else self.one
+        if self.num_inference_steps is None:
+            raise ValueError(
+                "Number of inference steps is 'None', you need to run 'set_timesteps' after creating the scheduler"
+            )
 
-        # For t > 0, compute predicted variance βt (see formula (6) and (7) from https://arxiv.org/pdf/2006.11239.pdf)
-        # and sample from it to get previous sample
-        # x_{t-1} ~ N(pred_prev_sample, variance) == add variance to pred_sample
-        variance = (1 - alpha_prod_t_prev) / (1 - alpha_prod_t) * self.betas[timestep]
-        # hacks - were probably added for training stability
-        if self.variance_type == "fixed_small":
-            variance = torch.clamp(variance, min=1e-20)
-        elif self.variance_type == "fixed_large":
-            variance = self.betas[timestep]
-        elif self.variance_type == "learned":
-            return predicted_variance
-        elif self.variance_type == "learned_range":
-            min_log = variance
-            max_log = self.betas[timestep]
-            frac = (predicted_variance + 1) / 2
-            variance = frac * max_log + (1 - frac) * min_log
+        diff_to_prev = 0 if self.counter % 2 else self.num_train_timesteps // self.num_inference_steps // 2
+        prev_timestep = timestep - diff_to_prev
+        timestep = self.prk_timesteps[self.counter // 4 * 4]
+
+        if self.counter % 4 == 0:
+            self.cur_model_output += 1 / 6 * model_output
+            self.ets.append(model_output)
+            self.cur_sample = sample
+        elif (self.counter - 1) % 4 == 0:
+            self.cur_model_output += 1 / 3 * model_output
+        elif (self.counter - 2) % 4 == 0:
+            self.cur_model_output += 1 / 3 * model_output
+        elif (self.counter - 3) % 4 == 0:
+            model_output = self.cur_model_output + 1 / 6 * model_output
+            self.cur_model_output = 0
+
+        # cur_sample should not be `None`
+        cur_sample = self.cur_sample if self.cur_sample is not None else sample
 
-        return variance
+        prev_sample = self._get_prev_sample(cur_sample, timestep, prev_timestep, model_output)
+        self.counter += 1
 
-    def step(
-        self, model_output: torch.Tensor, timestep: int, sample: torch.Tensor, generator: torch.Generator | None = None
-    ) -> tuple[torch.Tensor, torch.Tensor]:
+        return prev_sample
+
+    def step_plms(self, model_output: torch.FloatTensor, timestep: int, sample: torch.FloatTensor) -> torch.Tensor:
         """
-        Predict the sample at the previous timestep by reversing the SDE. Core function to propagate the diffusion
-        process from the learned model outputs (most often the predicted noise).
+        Step function propagating the sample with the linear multi-step method. This has one forward pass with multiple
+        times to approximate the solution.
 
         Args:
             model_output: direct output from learned diffusion model.
             timestep: current discrete timestep in the diffusion chain.
             sample: current instance of sample being created by diffusion process.
-            generator: random number generator.
 
         Returns:
             pred_prev_sample: Predicted previous sample
         """
-        if model_output.shape[1] == sample.shape[1] * 2 and self.variance_type in ["learned", "learned_range"]:
-            model_output, predicted_variance = torch.split(model_output, sample.shape[1], dim=1)
-        else:
-            predicted_variance = None
+        if self.num_inference_steps is None:
+            raise ValueError(
+                "Number of inference steps is 'None', you need to run 'set_timesteps' after creating the scheduler"
+            )
 
-        # 1. compute alphas, betas
-        alpha_prod_t = self.alphas_cumprod[timestep]
-        alpha_prod_t_prev = self.alphas_cumprod[timestep - 1] if timestep > 0 else self.one
-        beta_prod_t = 1 - alpha_prod_t
-        beta_prod_t_prev = 1 - alpha_prod_t_prev
+        if not self.skip_prk_steps and len(self.ets) < 3:
+            raise ValueError(
+                f"{self.__class__} can only be run AFTER scheduler has been run "
+                "in 'prk' mode for at least 12 iterations "
+            )
 
-        # 2. compute predicted original sample from predicted noise also called
-        # "predicted x_0" of formula (15) from https://arxiv.org/pdf/2006.11239.pdf
-        if self.prediction_type == "epsilon":
-            pred_original_sample = (sample - beta_prod_t ** (0.5) * model_output) / alpha_prod_t ** (0.5)
-        elif self.prediction_type == "sample":
-            pred_original_sample = model_output
-        elif self.prediction_type == "v_prediction":
-            pred_original_sample = (alpha_prod_t**0.5) * sample - (beta_prod_t**0.5) * model_output
-
-        # 3. Clip "predicted x_0"
-        if self.clip_sample:
-            pred_original_sample = torch.clamp(pred_original_sample, -1, 1)
-
-        # 4. Compute coefficients for pred_original_sample x_0 and current sample x_t
-        # See formula (7) from https://arxiv.org/pdf/2006.11239.pdf
-        pred_original_sample_coeff = (alpha_prod_t_prev ** (0.5) * self.betas[timestep]) / beta_prod_t
-        current_sample_coeff = self.alphas[timestep] ** (0.5) * beta_prod_t_prev / beta_prod_t
-
-        # 5. Compute predicted previous sample µ_t
-        # See formula (7) from https://arxiv.org/pdf/2006.11239.pdf
-        pred_prev_sample = pred_original_sample_coeff * pred_original_sample + current_sample_coeff * sample
-
-        # 6. Add noise
-        variance = 0
-        if timestep > 0:
-            noise = torch.randn(
-                model_output.size(), dtype=model_output.dtype, layout=model_output.layout, generator=generator
-            ).to(model_output.device)
-            variance = (self._get_variance(timestep, predicted_variance=predicted_variance) ** 0.5) * noise
+        prev_timestep = timestep - self.num_train_timesteps // self.num_inference_steps
 
-        pred_prev_sample = pred_prev_sample + variance
+        if self.counter != 1:
+            self.ets = self.ets[-3:]
+            self.ets.append(model_output)
+        else:
+            prev_timestep = timestep
+            timestep = timestep + self.num_train_timesteps // self.num_inference_steps
 
-        return pred_prev_sample, pred_original_sample
+        if len(self.ets) == 1 and self.counter == 0:
+            model_output = model_output
+            self.cur_sample = sample
+        elif len(self.ets) == 1 and self.counter == 1:
+            model_output = (model_output + self.ets[-1]) / 2
+            sample = self.cur_sample
+            self.cur_sample = None
+        elif len(self.ets) == 2:
+            model_output = (3 * self.ets[-1] - self.ets[-2]) / 2
+        elif len(self.ets) == 3:
+            model_output = (23 * self.ets[-1] - 16 * self.ets[-2] + 5 * self.ets[-3]) / 12
+        else:
+            model_output = (1 / 24) * (55 * self.ets[-1] - 59 * self.ets[-2] + 37 * self.ets[-3] - 9 * self.ets[-4])
 
-    def add_noise(self, original_samples: torch.Tensor, noise: torch.Tensor, timesteps: torch.Tensor) -> torch.Tensor:
-        """
-        Add noise to the original samples.
+        prev_sample = self._get_prev_sample(sample, timestep, prev_timestep, model_output)
+        self.counter += 1
 
-        Args:
-            original_samples: original samples
-            noise: noise to add to samples
-            timesteps: timesteps tensor indicating the timestep to be computed for each sample.
+        return prev_sample
 
-        Returns:
-            noisy_samples: sample with added noise
-        """
-        # Make sure alphas_cumprod and timestep have same device and dtype as original_samples
-        self.alphas_cumprod = self.alphas_cumprod.to(device=original_samples.device, dtype=original_samples.dtype)
-        timesteps = timesteps.to(original_samples.device)
-
-        sqrt_alpha_cumprod = self.alphas_cumprod[timesteps] ** 0.5
-        sqrt_alpha_cumprod = sqrt_alpha_cumprod.flatten()
-        while len(sqrt_alpha_cumprod.shape) < len(original_samples.shape):
-            sqrt_alpha_cumprod = sqrt_alpha_cumprod.unsqueeze(-1)
-
-        sqrt_one_minus_alpha_prod = (1 - self.alphas_cumprod[timesteps]) ** 0.5
-        sqrt_one_minus_alpha_prod = sqrt_one_minus_alpha_prod.flatten()
-        while len(sqrt_one_minus_alpha_prod.shape) < len(original_samples.shape):
-            sqrt_one_minus_alpha_prod = sqrt_one_minus_alpha_prod.unsqueeze(-1)
-
-        noisy_samples = sqrt_alpha_cumprod * original_samples + sqrt_one_minus_alpha_prod * noise
-        return noisy_samples
-
-    def get_velocity(self, sample: torch.Tensor, noise: torch.Tensor, timesteps: torch.Tensor) -> torch.Tensor:
-        # Make sure alphas_cumprod and timestep have same device and dtype as sample
-        self.alphas_cumprod = self.alphas_cumprod.to(device=sample.device, dtype=sample.dtype)
-        timesteps = timesteps.to(sample.device)
-
-        sqrt_alpha_prod = self.alphas_cumprod[timesteps] ** 0.5
-        sqrt_alpha_prod = sqrt_alpha_prod.flatten()
-        while len(sqrt_alpha_prod.shape) < len(sample.shape):
-            sqrt_alpha_prod = sqrt_alpha_prod.unsqueeze(-1)
-
-        sqrt_one_minus_alpha_prod = (1 - self.alphas_cumprod[timesteps]) ** 0.5
-        sqrt_one_minus_alpha_prod = sqrt_one_minus_alpha_prod.flatten()
-        while len(sqrt_one_minus_alpha_prod.shape) < len(sample.shape):
-            sqrt_one_minus_alpha_prod = sqrt_one_minus_alpha_prod.unsqueeze(-1)
+    def _get_prev_sample(self, sample: torch.Tensor, timestep: int, prev_timestep: int, model_output: torch.Tensor):
+        # See formula (9) of PNDM paper https://arxiv.org/pdf/2202.09778.pdf
+        # this function computes x_(t−δ) using the formula of (9)
+        # Note that x_t needs to be added to both sides of the equation
+
+        # Notation (<variable name> -> <name in paper>
+        # alpha_prod_t -> α_t
+        # alpha_prod_t_prev -> α_(t−δ)
+        # beta_prod_t -> (1 - α_t)
+        # beta_prod_t_prev -> (1 - α_(t−δ))
+        # sample -> x_t
+        # model_output -> e_θ(x_t, t)
+        # prev_sample -> x_(t−δ)
+        alpha_prod_t = self.alphas_cumprod[timestep]
+        alpha_prod_t_prev = self.alphas_cumprod[prev_timestep] if prev_timestep >= 0 else self.final_alpha_cumprod
+        beta_prod_t = 1 - alpha_prod_t
+        beta_prod_t_prev = 1 - alpha_prod_t_prev
+
+        if self.prediction_type == PNDMPredictionType.V_PREDICTION:
+            model_output = (alpha_prod_t**0.5) * model_output + (beta_prod_t**0.5) * sample
+
+        # corresponds to (α_(t−δ) - α_t) divided by
+        # denominator of x_t in formula (9) and plus 1
+        # Note: (α_(t−δ) - α_t) / (sqrt(α_t) * (sqrt(α_(t−δ)) + sqr(α_t))) =
+        # sqrt(α_(t−δ)) / sqrt(α_t))
+        sample_coeff = (alpha_prod_t_prev / alpha_prod_t) ** (0.5)
+
+        # corresponds to denominator of e_θ(x_t, t) in formula (9)
+        model_output_denom_coeff = alpha_prod_t * beta_prod_t_prev ** (0.5) + (
+            alpha_prod_t * beta_prod_t * alpha_prod_t_prev
+        ) ** (0.5)
+
+        # full formula (9)
+        prev_sample = (
+            sample_coeff * sample - (alpha_prod_t_prev - alpha_prod_t) * model_output / model_output_denom_coeff
+        )
 
-        velocity = sqrt_alpha_prod * noise - sqrt_one_minus_alpha_prod * sample
-        return velocity
+        return prev_sample
```

### Comparing `monai-generative-0.2.1/generative/utils/__init__.py` & `monai-generative-0.2.2/generative/version.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from .enums import AdversarialIterationEvents, AdversarialKeys
+__version__ = "0.2.2"
```

### Comparing `monai-generative-0.2.1/generative/utils/enums.py` & `monai-generative-0.2.2/generative/utils/enums.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/generative/utils/ordering.py` & `monai-generative-0.2.2/generative/utils/ordering.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/monai_generative.egg-info/SOURCES.txt` & `monai-generative-0.2.2/monai_generative.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -32,35 +32,40 @@
 generative/networks/nets/patchgan_discriminator.py
 generative/networks/nets/transformer.py
 generative/networks/nets/vqvae.py
 generative/networks/schedulers/__init__.py
 generative/networks/schedulers/ddim.py
 generative/networks/schedulers/ddpm.py
 generative/networks/schedulers/pndm.py
+generative/networks/schedulers/scheduler.py
 generative/utils/__init__.py
+generative/utils/component_store.py
 generative/utils/enums.py
+generative/utils/misc.py
 generative/utils/ordering.py
 monai_generative.egg-info/PKG-INFO
 monai_generative.egg-info/SOURCES.txt
 monai_generative.egg-info/dependency_links.txt
 monai_generative.egg-info/requires.txt
 monai_generative.egg-info/top_level.txt
 tests/__init__.py
 tests/min_tests.py
 tests/runner.py
 tests/test_adversarial.py
 tests/test_autoencoderkl.py
+tests/test_component_store.py
 tests/test_compute_fid_metric.py
 tests/test_compute_mmd_metric.py
 tests/test_compute_multiscalessim_metric.py
 tests/test_controlnet.py
 tests/test_diffusion_inferer.py
 tests/test_diffusion_model_unet.py
 tests/test_integration_workflows_adversarial.py
 tests/test_latent_diffusion_inferer.py
+tests/test_misc.py
 tests/test_ordering.py
 tests/test_patch_gan.py
 tests/test_perceptual_loss.py
 tests/test_scheduler_ddim.py
 tests/test_scheduler_ddpm.py
 tests/test_scheduler_pndm.py
 tests/test_selfattention.py
```

### Comparing `monai-generative-0.2.1/pyproject.toml` & `monai-generative-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/setup.cfg` & `monai-generative-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/setup.py` & `monai-generative-0.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 from __future__ import annotations
 
 from setuptools import find_packages, setup
 
 setup(
     name="monai-generative",
     packages=find_packages(exclude=[]),
-    version="0.2.1",
+    version="0.2.2",
     description="Installer to help to use the prototypes from MONAI generative models in other projects.",
-    install_requires=["monai-weekly==1.2.dev2304"],
+    install_requires=["monai>=1.2.0rc1"],
 )
```

### Comparing `monai-generative-0.2.1/tests/__init__.py` & `monai-generative-0.2.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/tests/min_tests.py` & `monai-generative-0.2.2/tests/min_tests.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/tests/runner.py` & `monai-generative-0.2.2/tests/runner.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/tests/test_adversarial.py` & `monai-generative-0.2.2/tests/test_adversarial.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/tests/test_autoencoderkl.py` & `monai-generative-0.2.2/tests/test_autoencoderkl.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/tests/test_compute_fid_metric.py` & `monai-generative-0.2.2/tests/test_compute_fid_metric.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/tests/test_compute_mmd_metric.py` & `monai-generative-0.2.2/tests/test_compute_mmd_metric.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/tests/test_compute_multiscalessim_metric.py` & `monai-generative-0.2.2/tests/test_compute_multiscalessim_metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,24 +55,28 @@
 
         metric = MultiScaleSSIMMetric(spatial_dims=3, data_range=1.0, kernel_type="gaussian", weights=[0.5, 0.5])
         metric(preds, target)
         result = metric.aggregate()
         expected_value = 0.061796
         self.assertTrue(expected_value - result.item() < 0.000001)
 
-    def input_ill_input_shape(self):
+    def input_ill_input_shape2d(self):
+        metric = MultiScaleSSIMMetric(spatial_dims=3, weights=[0.5, 0.5])
+
         with self.assertRaises(ValueError):
-            metric = MultiScaleSSIMMetric(spatial_dims=3, weights=[0.5, 0.5])
             metric(torch.randn(1, 1, 64, 64), torch.randn(1, 1, 64, 64))
 
+    def input_ill_input_shape3d(self):
+        metric = MultiScaleSSIMMetric(spatial_dims=2, weights=[0.5, 0.5])
+
         with self.assertRaises(ValueError):
-            metric = MultiScaleSSIMMetric(spatial_dims=2, weights=[0.5, 0.5])
             metric(torch.randn(1, 1, 64, 64, 64), torch.randn(1, 1, 64, 64, 64))
 
     def small_inputs(self):
+        metric = MultiScaleSSIMMetric(spatial_dims=2)
+
         with self.assertRaises(ValueError):
-            metric = MultiScaleSSIMMetric(spatial_dims=2)
             metric(torch.randn(1, 1, 16, 16, 16), torch.randn(1, 1, 16, 16, 16))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-generative-0.2.1/tests/test_controlnet.py` & `monai-generative-0.2.2/tests/test_controlnet.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/tests/test_diffusion_inferer.py` & `monai-generative-0.2.2/tests/test_diffusion_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/tests/test_diffusion_model_unet.py` & `monai-generative-0.2.2/tests/test_diffusion_model_unet.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,26 +341,27 @@
                 with_conditioning=True,
                 transformer_num_layers=1,
                 cross_attention_dim=None,
                 norm_num_groups=8,
             )
 
     def test_context_with_conditioning_none(self):
+        net = DiffusionModelUNet(
+            spatial_dims=2,
+            in_channels=1,
+            out_channels=1,
+            num_res_blocks=1,
+            num_channels=(8, 8, 8),
+            attention_levels=(False, False, True),
+            with_conditioning=False,
+            transformer_num_layers=1,
+            norm_num_groups=8,
+        )
+
         with self.assertRaises(ValueError):
-            net = DiffusionModelUNet(
-                spatial_dims=2,
-                in_channels=1,
-                out_channels=1,
-                num_res_blocks=1,
-                num_channels=(8, 8, 8),
-                attention_levels=(False, False, True),
-                with_conditioning=False,
-                transformer_num_layers=1,
-                norm_num_groups=8,
-            )
             with eval_mode(net):
                 net.forward(
                     x=torch.rand((1, 1, 16, 32)),
                     timesteps=torch.randint(0, 1000, (1,)).long(),
                     context=torch.rand((1, 1, 3)),
                 )
 
@@ -381,26 +382,27 @@
                 x=torch.rand((1, 1, 16, 32)),
                 timesteps=torch.randint(0, 1000, (1,)).long(),
                 class_labels=torch.randint(0, 2, (1,)).long(),
             )
             self.assertEqual(result.shape, (1, 1, 16, 32))
 
     def test_conditioned_models_no_class_labels(self):
+        net = DiffusionModelUNet(
+            spatial_dims=2,
+            in_channels=1,
+            out_channels=1,
+            num_res_blocks=1,
+            num_channels=(8, 8, 8),
+            attention_levels=(False, False, True),
+            norm_num_groups=8,
+            num_head_channels=8,
+            num_class_embeds=2,
+        )
+
         with self.assertRaises(ValueError):
-            net = DiffusionModelUNet(
-                spatial_dims=2,
-                in_channels=1,
-                out_channels=1,
-                num_res_blocks=1,
-                num_channels=(8, 8, 8),
-                attention_levels=(False, False, True),
-                norm_num_groups=8,
-                num_head_channels=8,
-                num_class_embeds=2,
-            )
             net.forward(x=torch.rand((1, 1, 16, 32)), timesteps=torch.randint(0, 1000, (1,)).long())
 
     def test_model_num_channels_not_same_size_of_attention_levels(self):
         with self.assertRaises(ValueError):
             DiffusionModelUNet(
                 spatial_dims=2,
                 in_channels=1,
```

### Comparing `monai-generative-0.2.1/tests/test_integration_workflows_adversarial.py` & `monai-generative-0.2.2/tests/test_integration_workflows_adversarial.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/tests/test_latent_diffusion_inferer.py` & `monai-generative-0.2.2/tests/test_latent_diffusion_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/tests/test_ordering.py` & `monai-generative-0.2.2/tests/test_ordering.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/tests/test_patch_gan.py` & `monai-generative-0.2.2/tests/test_patch_gan.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/tests/test_perceptual_loss.py` & `monai-generative-0.2.2/tests/test_perceptual_loss.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/tests/test_scheduler_ddim.py` & `monai-generative-0.2.2/tests/test_scheduler_ddim.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 
 import torch
 from parameterized import parameterized
 
 from generative.networks.schedulers import DDIMScheduler
 
 TEST_2D_CASE = []
-for beta_schedule in ["linear", "scaled_linear"]:
-    TEST_2D_CASE.append([{"beta_schedule": beta_schedule}, (2, 6, 16, 16), (2, 6, 16, 16)])
+for beta_schedule in ["linear_beta", "scaled_linear_beta"]:
+    TEST_2D_CASE.append([{"schedule": beta_schedule}, (2, 6, 16, 16), (2, 6, 16, 16)])
 
 TEST_3D_CASE = []
-for beta_schedule in ["linear", "scaled_linear"]:
-    TEST_3D_CASE.append([{"beta_schedule": beta_schedule}, (2, 6, 16, 16, 16), (2, 6, 16, 16, 16)])
+for beta_schedule in ["linear_beta", "scaled_linear_beta"]:
+    TEST_3D_CASE.append([{"schedule": beta_schedule}, (2, 6, 16, 16, 16), (2, 6, 16, 16, 16)])
 
 TEST_CASES = TEST_2D_CASE + TEST_3D_CASE
 
 
 class TestDDPMScheduler(unittest.TestCase):
     @parameterized.expand(TEST_CASES)
     def test_add_noise_2d_shape(self, input_param, input_shape, expected_shape):
```

### Comparing `monai-generative-0.2.1/tests/test_scheduler_ddpm.py` & `monai-generative-0.2.2/tests/test_scheduler_ddpm.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 
 import torch
 from parameterized import parameterized
 
 from generative.networks.schedulers import DDPMScheduler
 
 TEST_2D_CASE = []
-for beta_schedule in ["linear", "scaled_linear"]:
+for beta_schedule in ["linear_beta", "scaled_linear_beta"]:
     for variance_type in ["fixed_small", "fixed_large"]:
         TEST_2D_CASE.append(
-            [{"beta_schedule": beta_schedule, "variance_type": variance_type}, (2, 6, 16, 16), (2, 6, 16, 16)]
+            [{"schedule": beta_schedule, "variance_type": variance_type}, (2, 6, 16, 16), (2, 6, 16, 16)]
         )
 
 TEST_3D_CASE = []
-for beta_schedule in ["linear", "scaled_linear"]:
+for beta_schedule in ["linear_beta", "scaled_linear_beta"]:
     for variance_type in ["fixed_small", "fixed_large"]:
         TEST_3D_CASE.append(
-            [{"beta_schedule": beta_schedule, "variance_type": variance_type}, (2, 6, 16, 16, 16), (2, 6, 16, 16, 16)]
+            [{"schedule": beta_schedule, "variance_type": variance_type}, (2, 6, 16, 16, 16), (2, 6, 16, 16, 16)]
         )
 
 TEST_CASES = TEST_2D_CASE + TEST_3D_CASE
 
 
 class TestDDPMScheduler(unittest.TestCase):
     @parameterized.expand(TEST_CASES)
@@ -51,14 +51,22 @@
         scheduler = DDPMScheduler(**input_param)
         model_output = torch.randn(input_shape)
         sample = torch.randn(input_shape)
         output_step = scheduler.step(model_output=model_output, timestep=500, sample=sample)
         self.assertEqual(output_step[0].shape, expected_shape)
         self.assertEqual(output_step[1].shape, expected_shape)
 
+    @parameterized.expand(TEST_CASES)
+    def test_get_velocity_shape(self, input_param, input_shape, expected_shape):
+        scheduler = DDPMScheduler(**input_param)
+        sample = torch.randn(input_shape)
+        timesteps = torch.randint(0, scheduler.num_train_timesteps, (input_shape[0],)).long()
+        velocity = scheduler.get_velocity(sample=sample, noise=sample, timesteps=timesteps)
+        self.assertEqual(velocity.shape, expected_shape)
+
     def test_step_learned(self):
         for variance_type in ["learned", "learned_range"]:
             scheduler = DDPMScheduler(variance_type=variance_type)
         model_output = torch.randn(2, 6, 16, 16)
         sample = torch.randn(2, 3, 16, 16)
         output_step = scheduler.step(model_output=model_output, timestep=500, sample=sample)
         self.assertEqual(output_step[0].shape, sample.shape)
```

### Comparing `monai-generative-0.2.1/tests/test_scheduler_pndm.py` & `monai-generative-0.2.2/tests/test_scheduler_pndm.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 
 import torch
 from parameterized import parameterized
 
 from generative.networks.schedulers import PNDMScheduler
 
 TEST_2D_CASE = []
-for beta_schedule in ["linear", "scaled_linear"]:
-    TEST_2D_CASE.append([{"beta_schedule": beta_schedule}, (2, 6, 16, 16), (2, 6, 16, 16)])
+for beta_schedule in ["linear_beta", "scaled_linear_beta"]:
+    TEST_2D_CASE.append([{"schedule": beta_schedule}, (2, 6, 16, 16), (2, 6, 16, 16)])
 
 TEST_3D_CASE = []
-for beta_schedule in ["linear", "scaled_linear"]:
-    TEST_3D_CASE.append([{"beta_schedule": beta_schedule}, (2, 6, 16, 16, 16), (2, 6, 16, 16, 16)])
+for beta_schedule in ["linear_beta", "scaled_linear_beta"]:
+    TEST_3D_CASE.append([{"schedule": beta_schedule}, (2, 6, 16, 16, 16), (2, 6, 16, 16, 16)])
 
 TEST_CASES = TEST_2D_CASE + TEST_3D_CASE
 
 
 class TestDDPMScheduler(unittest.TestCase):
     @parameterized.expand(TEST_CASES)
     def test_add_noise_2d_shape(self, input_param, input_shape, expected_shape):
```

### Comparing `monai-generative-0.2.1/tests/test_selfattention.py` & `monai-generative-0.2.2/tests/test_selfattention.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/tests/test_spectral_loss.py` & `monai-generative-0.2.2/tests/test_spectral_loss.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/tests/test_transformer.py` & `monai-generative-0.2.2/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/tests/test_vector_quantizer.py` & `monai-generative-0.2.2/tests/test_vector_quantizer.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/tests/test_vqvae.py` & `monai-generative-0.2.2/tests/test_vqvae.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/tests/test_vqvaetransformer_inferer.py` & `monai-generative-0.2.2/tests/test_vqvaetransformer_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-generative-0.2.1/tests/utils.py` & `monai-generative-0.2.2/tests/utils.py`

 * *Files identical despite different names*

