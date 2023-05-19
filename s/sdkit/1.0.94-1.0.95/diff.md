# Comparing `tmp/sdkit-1.0.94.tar.gz` & `tmp/sdkit-1.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkit-1.0.94.tar", last modified: Fri May 19 11:53:46 2023, max compression
+gzip compressed data, was "sdkit-1.0.95.tar", last modified: Fri May 19 12:12:33 2023, max compression
```

## Comparing `sdkit-1.0.94.tar` & `sdkit-1.0.95.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 11:53:46.938896 sdkit-1.0.94/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4121 2022-12-23 10:54:05.000000 sdkit-1.0.94/LICENSE
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       84 2023-02-06 11:28:37.000000 sdkit-1.0.94/MANIFEST.in
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10532 2023-05-19 11:53:46.934895 sdkit-1.0.94/PKG-INFO
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     9349 2023-04-10 11:16:32.000000 sdkit-1.0.94/README.md
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1441 2023-05-19 11:53:25.000000 sdkit-1.0.94/pyproject.toml
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 11:53:44.472012 sdkit-1.0.94/sdkit/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3719 2023-05-19 11:22:44.000000 sdkit-1.0.94/sdkit/__init__.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 11:53:44.764364 sdkit-1.0.94/sdkit/filter/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       41 2023-04-29 09:00:56.000000 sdkit-1.0.94/sdkit/filter/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1197 2023-05-19 11:22:44.000000 sdkit-1.0.94/sdkit/filter/apply_filters.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      998 2023-02-16 16:25:27.000000 sdkit-1.0.94/sdkit/filter/gfpgan.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1194 2023-05-19 11:22:44.000000 sdkit-1.0.94/sdkit/filter/latent_upscaler.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      614 2023-04-28 10:50:58.000000 sdkit-1.0.94/sdkit/filter/nsfw_checker.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      378 2023-04-10 12:49:03.000000 sdkit-1.0.94/sdkit/filter/realesrgan.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 11:53:44.854323 sdkit-1.0.94/sdkit/generate/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       45 2023-04-29 09:01:13.000000 sdkit-1.0.94/sdkit/generate/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     9985 2023-05-16 10:02:05.000000 sdkit-1.0.94/sdkit/generate/image_generator.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2479 2023-02-17 07:20:50.000000 sdkit-1.0.94/sdkit/generate/prompt_parser.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 11:53:45.044024 sdkit-1.0.94/sdkit/generate/sampler/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       39 2023-04-29 09:01:07.000000 sdkit-1.0.94/sdkit/generate/sampler/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3168 2023-04-10 11:16:32.000000 sdkit-1.0.94/sdkit/generate/sampler/default_samplers.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3396 2023-05-19 11:28:03.000000 sdkit-1.0.94/sdkit/generate/sampler/diffusers_samplers.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2589 2023-02-16 16:25:27.000000 sdkit-1.0.94/sdkit/generate/sampler/k_samplers.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2132 2023-02-16 16:27:22.000000 sdkit-1.0.94/sdkit/generate/sampler/sampler_main.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 11:53:45.123729 sdkit-1.0.94/sdkit/generate/sampler/unipc_samplers/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2737 2023-04-28 10:50:59.000000 sdkit-1.0.94/sdkit/generate/sampler/unipc_samplers/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    40444 2023-04-29 08:59:42.000000 sdkit-1.0.94/sdkit/generate/sampler/unipc_samplers/unipc_sampler.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 11:53:45.226527 sdkit-1.0.94/sdkit/models/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      258 2023-04-29 09:01:22.000000 sdkit-1.0.94/sdkit/models/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     5475 2023-02-16 16:25:27.000000 sdkit-1.0.94/sdkit/models/model_downloader.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 11:53:45.691297 sdkit-1.0.94/sdkit/models/model_loader/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1747 2023-05-19 11:22:44.000000 sdkit-1.0.94/sdkit/models/model_loader/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      609 2023-02-16 16:25:27.000000 sdkit-1.0.94/sdkit/models/model_loader/gfpgan.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 11:53:45.781103 sdkit-1.0.94/sdkit/models/model_loader/hypernetwork/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2337 2023-02-16 16:25:27.000000 sdkit-1.0.94/sdkit/models/model_loader/hypernetwork/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4414 2023-02-16 16:25:27.000000 sdkit-1.0.94/sdkit/models/model_loader/hypernetwork/hypernetwork.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      712 2023-05-19 11:22:44.000000 sdkit-1.0.94/sdkit/models/model_loader/latent_upscaler.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3945 2023-05-10 14:38:42.000000 sdkit-1.0.94/sdkit/models/model_loader/lora.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      513 2023-02-18 08:34:10.000000 sdkit-1.0.94/sdkit/models/model_loader/nsfw_checker.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1117 2023-04-20 10:42:08.000000 sdkit-1.0.94/sdkit/models/model_loader/realesrgan.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 11:53:45.937081 sdkit-1.0.94/sdkit/models/model_loader/stable_diffusion/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    11471 2023-05-19 11:22:44.000000 sdkit-1.0.94/sdkit/models/model_loader/stable_diffusion/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    62271 2023-04-29 08:58:14.000000 sdkit-1.0.94/sdkit/models/model_loader/stable_diffusion/convert_from_ckpt.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    13146 2023-05-19 11:21:30.000000 sdkit-1.0.94/sdkit/models/model_loader/stable_diffusion/optimizations.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2501 2023-04-10 11:16:32.000000 sdkit-1.0.94/sdkit/models/model_loader/vae.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 11:53:46.123742 sdkit-1.0.94/sdkit/models/models_db/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1174 2023-04-28 10:50:59.000000 sdkit-1.0.94/sdkit/models/models_db/__init__.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 11:53:46.594048 sdkit-1.0.94/sdkit/models/models_db/configs/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1873 2022-12-25 10:25:54.000000 sdkit-1.0.94/sdkit/models/models_db/configs/v1-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1991 2022-12-25 10:26:03.000000 sdkit-1.0.94/sdkit/models/models_db/configs/v1-inpainting-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1815 2022-12-25 10:26:48.000000 sdkit-1.0.94/sdkit/models/models_db/configs/v2-inference-v.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1789 2022-12-25 10:26:58.000000 sdkit-1.0.94/sdkit/models/models_db/configs/v2-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4450 2022-12-25 10:26:26.000000 sdkit-1.0.94/sdkit/models/models_db/configs/v2-inpainting-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1869 2022-12-25 10:26:35.000000 sdkit-1.0.94/sdkit/models/models_db/configs/v2-midas-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1847 2023-04-17 10:06:16.000000 sdkit-1.0.94/sdkit/models/models_db/configs/v2.1-inference-v.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1821 2023-04-17 10:06:49.000000 sdkit-1.0.94/sdkit/models/models_db/configs/v2.1-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2251 2022-12-25 10:26:13.000000 sdkit-1.0.94/sdkit/models/models_db/configs/x4-upscaling.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      720 2023-04-22 10:11:26.000000 sdkit-1.0.94/sdkit/models/models_db/gfpgan.json
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      534 2022-12-26 07:39:49.000000 sdkit-1.0.94/sdkit/models/models_db/realesrgan.json
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10084 2023-02-06 10:52:19.000000 sdkit-1.0.94/sdkit/models/models_db/stable_diffusion.json
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      308 2023-04-19 09:15:54.000000 sdkit-1.0.94/sdkit/models/models_db/vae.json
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      206 2023-02-16 16:25:27.000000 sdkit-1.0.94/sdkit/models/scan_models.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 11:53:46.668059 sdkit-1.0.94/sdkit/train/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       39 2023-04-29 09:01:28.000000 sdkit-1.0.94/sdkit/train/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2581 2023-02-16 16:25:27.000000 sdkit-1.0.94/sdkit/train/merge_models.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 11:53:46.900105 sdkit-1.0.94/sdkit/utils/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      984 2023-05-19 11:17:19.000000 sdkit-1.0.94/sdkit/utils/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4005 2023-04-28 10:35:29.000000 sdkit-1.0.94/sdkit/utils/file_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2189 2023-04-28 10:35:29.000000 sdkit-1.0.94/sdkit/utils/hash_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1113 2023-02-16 16:25:27.000000 sdkit-1.0.94/sdkit/utils/http_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2252 2023-05-19 11:18:10.000000 sdkit-1.0.94/sdkit/utils/image_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3962 2023-04-28 10:51:01.000000 sdkit-1.0.94/sdkit/utils/latent_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     6889 2023-05-08 11:11:42.000000 sdkit-1.0.94/sdkit/utils/memory_utils.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 11:53:44.584580 sdkit-1.0.94/sdkit.egg-info/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10532 2023-05-19 11:53:43.000000 sdkit-1.0.94/sdkit.egg-info/PKG-INFO
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2317 2023-05-19 11:53:44.000000 sdkit-1.0.94/sdkit.egg-info/SOURCES.txt
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        1 2023-05-19 11:53:43.000000 sdkit-1.0.94/sdkit.egg-info/dependency_links.txt
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      150 2023-05-19 11:53:43.000000 sdkit-1.0.94/sdkit.egg-info/requires.txt
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        6 2023-05-19 11:53:43.000000 sdkit-1.0.94/sdkit.egg-info/top_level.txt
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       38 2023-05-19 11:53:46.940896 sdkit-1.0.94/setup.cfg
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      397 2023-05-19 11:22:44.000000 sdkit-1.0.94/setup.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 12:12:33.118113 sdkit-1.0.95/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4121 2022-12-23 10:54:05.000000 sdkit-1.0.95/LICENSE
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       84 2023-02-06 11:28:37.000000 sdkit-1.0.95/MANIFEST.in
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10532 2023-05-19 12:12:33.118113 sdkit-1.0.95/PKG-INFO
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     9349 2023-04-10 11:16:32.000000 sdkit-1.0.95/README.md
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1441 2023-05-19 12:12:12.000000 sdkit-1.0.95/pyproject.toml
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 12:12:31.157439 sdkit-1.0.95/sdkit/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3719 2023-05-19 11:22:44.000000 sdkit-1.0.95/sdkit/__init__.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 12:12:31.408642 sdkit-1.0.95/sdkit/filter/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       41 2023-04-29 09:00:56.000000 sdkit-1.0.95/sdkit/filter/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1197 2023-05-19 11:22:44.000000 sdkit-1.0.95/sdkit/filter/apply_filters.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      998 2023-02-16 16:25:27.000000 sdkit-1.0.95/sdkit/filter/gfpgan.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1194 2023-05-19 11:22:44.000000 sdkit-1.0.95/sdkit/filter/latent_upscaler.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      614 2023-04-28 10:50:58.000000 sdkit-1.0.95/sdkit/filter/nsfw_checker.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      378 2023-04-10 12:49:03.000000 sdkit-1.0.95/sdkit/filter/realesrgan.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 12:12:31.489772 sdkit-1.0.95/sdkit/generate/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       45 2023-04-29 09:01:13.000000 sdkit-1.0.95/sdkit/generate/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     9985 2023-05-16 10:02:05.000000 sdkit-1.0.95/sdkit/generate/image_generator.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2479 2023-02-17 07:20:50.000000 sdkit-1.0.95/sdkit/generate/prompt_parser.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 12:12:31.628184 sdkit-1.0.95/sdkit/generate/sampler/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       39 2023-04-29 09:01:07.000000 sdkit-1.0.95/sdkit/generate/sampler/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3168 2023-04-10 11:16:32.000000 sdkit-1.0.95/sdkit/generate/sampler/default_samplers.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3396 2023-05-19 11:28:03.000000 sdkit-1.0.95/sdkit/generate/sampler/diffusers_samplers.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2589 2023-02-16 16:25:27.000000 sdkit-1.0.95/sdkit/generate/sampler/k_samplers.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2132 2023-02-16 16:27:22.000000 sdkit-1.0.95/sdkit/generate/sampler/sampler_main.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 12:12:31.706709 sdkit-1.0.95/sdkit/generate/sampler/unipc_samplers/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2737 2023-04-28 10:50:59.000000 sdkit-1.0.95/sdkit/generate/sampler/unipc_samplers/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    40444 2023-04-29 08:59:42.000000 sdkit-1.0.95/sdkit/generate/sampler/unipc_samplers/unipc_sampler.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 12:12:31.784834 sdkit-1.0.95/sdkit/models/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      258 2023-04-29 09:01:22.000000 sdkit-1.0.95/sdkit/models/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     5475 2023-02-16 16:25:27.000000 sdkit-1.0.95/sdkit/models/model_downloader.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 12:12:32.004784 sdkit-1.0.95/sdkit/models/model_loader/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1747 2023-05-19 11:22:44.000000 sdkit-1.0.95/sdkit/models/model_loader/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      609 2023-02-16 16:25:27.000000 sdkit-1.0.95/sdkit/models/model_loader/gfpgan.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 12:12:32.098935 sdkit-1.0.95/sdkit/models/model_loader/hypernetwork/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2337 2023-02-16 16:25:27.000000 sdkit-1.0.95/sdkit/models/model_loader/hypernetwork/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4414 2023-02-16 16:25:27.000000 sdkit-1.0.95/sdkit/models/model_loader/hypernetwork/hypernetwork.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      712 2023-05-19 11:22:44.000000 sdkit-1.0.95/sdkit/models/model_loader/latent_upscaler.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3945 2023-05-10 14:38:42.000000 sdkit-1.0.95/sdkit/models/model_loader/lora.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      513 2023-02-18 08:34:10.000000 sdkit-1.0.95/sdkit/models/model_loader/nsfw_checker.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1117 2023-04-20 10:42:08.000000 sdkit-1.0.95/sdkit/models/model_loader/realesrgan.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 12:12:32.239978 sdkit-1.0.95/sdkit/models/model_loader/stable_diffusion/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    11522 2023-05-19 12:10:41.000000 sdkit-1.0.95/sdkit/models/model_loader/stable_diffusion/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    62271 2023-04-29 08:58:14.000000 sdkit-1.0.95/sdkit/models/model_loader/stable_diffusion/convert_from_ckpt.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    13146 2023-05-19 11:21:30.000000 sdkit-1.0.95/sdkit/models/model_loader/stable_diffusion/optimizations.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2501 2023-04-10 11:16:32.000000 sdkit-1.0.95/sdkit/models/model_loader/vae.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 12:12:32.412665 sdkit-1.0.95/sdkit/models/models_db/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1174 2023-04-28 10:50:59.000000 sdkit-1.0.95/sdkit/models/models_db/__init__.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 12:12:32.804891 sdkit-1.0.95/sdkit/models/models_db/configs/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1873 2022-12-25 10:25:54.000000 sdkit-1.0.95/sdkit/models/models_db/configs/v1-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1991 2022-12-25 10:26:03.000000 sdkit-1.0.95/sdkit/models/models_db/configs/v1-inpainting-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1815 2022-12-25 10:26:48.000000 sdkit-1.0.95/sdkit/models/models_db/configs/v2-inference-v.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1789 2022-12-25 10:26:58.000000 sdkit-1.0.95/sdkit/models/models_db/configs/v2-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4450 2022-12-25 10:26:26.000000 sdkit-1.0.95/sdkit/models/models_db/configs/v2-inpainting-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1869 2022-12-25 10:26:35.000000 sdkit-1.0.95/sdkit/models/models_db/configs/v2-midas-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1847 2023-04-17 10:06:16.000000 sdkit-1.0.95/sdkit/models/models_db/configs/v2.1-inference-v.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1821 2023-04-17 10:06:49.000000 sdkit-1.0.95/sdkit/models/models_db/configs/v2.1-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2251 2022-12-25 10:26:13.000000 sdkit-1.0.95/sdkit/models/models_db/configs/x4-upscaling.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      720 2023-04-22 10:11:26.000000 sdkit-1.0.95/sdkit/models/models_db/gfpgan.json
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      534 2022-12-26 07:39:49.000000 sdkit-1.0.95/sdkit/models/models_db/realesrgan.json
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10084 2023-02-06 10:52:19.000000 sdkit-1.0.95/sdkit/models/models_db/stable_diffusion.json
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      308 2023-04-19 09:15:54.000000 sdkit-1.0.95/sdkit/models/models_db/vae.json
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      206 2023-02-16 16:25:27.000000 sdkit-1.0.95/sdkit/models/scan_models.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 12:12:32.867405 sdkit-1.0.95/sdkit/train/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       39 2023-04-29 09:01:28.000000 sdkit-1.0.95/sdkit/train/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2581 2023-02-16 16:25:27.000000 sdkit-1.0.95/sdkit/train/merge_models.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 12:12:33.086448 sdkit-1.0.95/sdkit/utils/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      984 2023-05-19 11:17:19.000000 sdkit-1.0.95/sdkit/utils/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4005 2023-04-28 10:35:29.000000 sdkit-1.0.95/sdkit/utils/file_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2189 2023-04-28 10:35:29.000000 sdkit-1.0.95/sdkit/utils/hash_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1113 2023-02-16 16:25:27.000000 sdkit-1.0.95/sdkit/utils/http_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2252 2023-05-19 11:18:10.000000 sdkit-1.0.95/sdkit/utils/image_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3962 2023-04-28 10:51:01.000000 sdkit-1.0.95/sdkit/utils/latent_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     6889 2023-05-08 11:11:42.000000 sdkit-1.0.95/sdkit/utils/memory_utils.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-19 12:12:31.267212 sdkit-1.0.95/sdkit.egg-info/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10532 2023-05-19 12:12:30.000000 sdkit-1.0.95/sdkit.egg-info/PKG-INFO
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2317 2023-05-19 12:12:30.000000 sdkit-1.0.95/sdkit.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        1 2023-05-19 12:12:30.000000 sdkit-1.0.95/sdkit.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      150 2023-05-19 12:12:30.000000 sdkit-1.0.95/sdkit.egg-info/requires.txt
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        6 2023-05-19 12:12:30.000000 sdkit-1.0.95/sdkit.egg-info/top_level.txt
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       38 2023-05-19 12:12:33.118113 sdkit-1.0.95/setup.cfg
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      397 2023-05-19 11:22:44.000000 sdkit-1.0.95/setup.py
```

### Comparing `sdkit-1.0.94/LICENSE` & `sdkit-1.0.95/LICENSE`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/PKG-INFO` & `sdkit-1.0.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkit
-Version: 1.0.94
+Version: 1.0.95
 Summary: sdkit (stable diffusion kit) is an easy-to-use library for using Stable Diffusion in your AI Art projects. It is fast, feature-packed, and memory-efficient. It bundles Stable Diffusion along with commonly-used features (like GFPGAN, RealESRGAN, k-samplers, custom VAE, hypernetworks etc). It also includes a model-downloader with a database of commonly used models, and advanced features like running in parallel on multiple GPUs, auto-scanning for malicious models etc. Supports Stable Diffusion 2.1!
 Author-email: cmdr2 <secondary.cmdr2@gmail.com>
 Project-URL: Homepage, https://github.com/easydiffusion/sdkit
 Project-URL: Bug Tracker, https://github.com/easydiffusion/sdkit/issues
 Keywords: stable diffusion,ai,art
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkit-1.0.94/README.md` & `sdkit-1.0.95/README.md`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/pyproject.toml` & `sdkit-1.0.95/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sdkit"
-version = "1.0.94"
+version = "1.0.95"
 authors = [
   {name="cmdr2", email="secondary.cmdr2@gmail.com"},
 ]
 description = "sdkit (stable diffusion kit) is an easy-to-use library for using Stable Diffusion in your AI Art projects. It is fast, feature-packed, and memory-efficient. It bundles Stable Diffusion along with commonly-used features (like GFPGAN, RealESRGAN, k-samplers, custom VAE, hypernetworks etc). It also includes a model-downloader with a database of commonly used models, and advanced features like running in parallel on multiple GPUs, auto-scanning for malicious models etc. Supports Stable Diffusion 2.1!"
 readme = "README.md"
 requires-python = ">=3.8.5"
 classifiers = [
```

### Comparing `sdkit-1.0.94/sdkit/__init__.py` & `sdkit-1.0.95/sdkit/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/filter/apply_filters.py` & `sdkit-1.0.95/sdkit/filter/apply_filters.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/filter/gfpgan.py` & `sdkit-1.0.95/sdkit/filter/gfpgan.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/filter/latent_upscaler.py` & `sdkit-1.0.95/sdkit/filter/latent_upscaler.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/filter/nsfw_checker.py` & `sdkit-1.0.95/sdkit/filter/nsfw_checker.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/generate/image_generator.py` & `sdkit-1.0.95/sdkit/generate/image_generator.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/generate/prompt_parser.py` & `sdkit-1.0.95/sdkit/generate/prompt_parser.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/generate/sampler/default_samplers.py` & `sdkit-1.0.95/sdkit/generate/sampler/default_samplers.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/generate/sampler/diffusers_samplers.py` & `sdkit-1.0.95/sdkit/generate/sampler/diffusers_samplers.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/generate/sampler/k_samplers.py` & `sdkit-1.0.95/sdkit/generate/sampler/k_samplers.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/generate/sampler/sampler_main.py` & `sdkit-1.0.95/sdkit/generate/sampler/sampler_main.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/generate/sampler/unipc_samplers/__init__.py` & `sdkit-1.0.95/sdkit/generate/sampler/unipc_samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/generate/sampler/unipc_samplers/unipc_sampler.py` & `sdkit-1.0.95/sdkit/generate/sampler/unipc_samplers/unipc_sampler.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/models/model_downloader.py` & `sdkit-1.0.95/sdkit/models/model_downloader.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/models/model_loader/__init__.py` & `sdkit-1.0.95/sdkit/models/model_loader/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/models/model_loader/gfpgan.py` & `sdkit-1.0.95/sdkit/models/model_loader/gfpgan.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/models/model_loader/hypernetwork/__init__.py` & `sdkit-1.0.95/sdkit/models/model_loader/hypernetwork/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/models/model_loader/hypernetwork/hypernetwork.py` & `sdkit-1.0.95/sdkit/models/model_loader/hypernetwork/hypernetwork.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/models/model_loader/latent_upscaler.py` & `sdkit-1.0.95/sdkit/models/model_loader/latent_upscaler.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/models/model_loader/lora.py` & `sdkit-1.0.95/sdkit/models/model_loader/lora.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/models/model_loader/nsfw_checker.py` & `sdkit-1.0.95/sdkit/models/model_loader/nsfw_checker.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/models/model_loader/realesrgan.py` & `sdkit-1.0.95/sdkit/models/model_loader/realesrgan.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/models/model_loader/stable_diffusion/__init__.py` & `sdkit-1.0.95/sdkit/models/model_loader/stable_diffusion/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,33 +167,35 @@
         default_pipe.enable_sequential_cpu_offload()
     else:
         if context.half_precision:
             default_pipe = default_pipe.to(context.device, torch.float16)
         else:
             default_pipe = default_pipe.to(context.device)
 
-    if context.vram_usage_level != "high":
+    if context.vram_usage_level == "high":
+        default_pipe.enable_attention_slicing(4)
+    else:
         default_pipe.enable_attention_slicing(1)
 
     try:
         import xformers
 
         default_pipe.enable_xformers_memory_efficient_attention()
     except:
         pass
 
     if torch.__version__.startswith("2."):
         default_pipe.enable_vae_slicing()
 
     # make the compel prompt parser object
     compel = Compel(
-        tokenizer = default_pipe.tokenizer,
-        text_encoder = default_pipe.text_encoder,
-        truncate_long_prompts = False,
-        use_penultimate_clip_layer = context.clip_skip,
+        tokenizer=default_pipe.tokenizer,
+        text_encoder=default_pipe.text_encoder,
+        truncate_long_prompts=False,
+        use_penultimate_clip_layer=context.clip_skip,
     )
 
     # make samplers
     diffusers_samplers.make_samplers(default_pipe.scheduler)
 
     if isinstance(default_pipe, StableDiffusionInpaintPipeline):
         log.info("Loaded on diffusers")
```

### Comparing `sdkit-1.0.94/sdkit/models/model_loader/stable_diffusion/convert_from_ckpt.py` & `sdkit-1.0.95/sdkit/models/model_loader/stable_diffusion/convert_from_ckpt.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/models/model_loader/stable_diffusion/optimizations.py` & `sdkit-1.0.95/sdkit/models/model_loader/stable_diffusion/optimizations.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/models/model_loader/vae.py` & `sdkit-1.0.95/sdkit/models/model_loader/vae.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/models/models_db/__init__.py` & `sdkit-1.0.95/sdkit/models/models_db/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/models/models_db/configs/v1-inference.yaml` & `sdkit-1.0.95/sdkit/models/models_db/configs/v1-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/models/models_db/configs/v1-inpainting-inference.yaml` & `sdkit-1.0.95/sdkit/models/models_db/configs/v1-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/models/models_db/configs/v2-inference-v.yaml` & `sdkit-1.0.95/sdkit/models/models_db/configs/v2-inference-v.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/models/models_db/configs/v2-inference.yaml` & `sdkit-1.0.95/sdkit/models/models_db/configs/v2-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/models/models_db/configs/v2-inpainting-inference.yaml` & `sdkit-1.0.95/sdkit/models/models_db/configs/v2-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/models/models_db/configs/v2-midas-inference.yaml` & `sdkit-1.0.95/sdkit/models/models_db/configs/v2-midas-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/models/models_db/configs/v2.1-inference-v.yaml` & `sdkit-1.0.95/sdkit/models/models_db/configs/v2.1-inference-v.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/models/models_db/configs/v2.1-inference.yaml` & `sdkit-1.0.95/sdkit/models/models_db/configs/v2.1-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/models/models_db/configs/x4-upscaling.yaml` & `sdkit-1.0.95/sdkit/models/models_db/configs/x4-upscaling.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/models/models_db/gfpgan.json` & `sdkit-1.0.95/sdkit/models/models_db/gfpgan.json`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/models/models_db/realesrgan.json` & `sdkit-1.0.95/sdkit/models/models_db/realesrgan.json`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/models/models_db/stable_diffusion.json` & `sdkit-1.0.95/sdkit/models/models_db/stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/train/merge_models.py` & `sdkit-1.0.95/sdkit/train/merge_models.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/utils/__init__.py` & `sdkit-1.0.95/sdkit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/utils/file_utils.py` & `sdkit-1.0.95/sdkit/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/utils/hash_utils.py` & `sdkit-1.0.95/sdkit/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/utils/http_utils.py` & `sdkit-1.0.95/sdkit/utils/http_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/utils/image_utils.py` & `sdkit-1.0.95/sdkit/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/utils/latent_utils.py` & `sdkit-1.0.95/sdkit/utils/latent_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit/utils/memory_utils.py` & `sdkit-1.0.95/sdkit/utils/memory_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.94/sdkit.egg-info/PKG-INFO` & `sdkit-1.0.95/sdkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkit
-Version: 1.0.94
+Version: 1.0.95
 Summary: sdkit (stable diffusion kit) is an easy-to-use library for using Stable Diffusion in your AI Art projects. It is fast, feature-packed, and memory-efficient. It bundles Stable Diffusion along with commonly-used features (like GFPGAN, RealESRGAN, k-samplers, custom VAE, hypernetworks etc). It also includes a model-downloader with a database of commonly used models, and advanced features like running in parallel on multiple GPUs, auto-scanning for malicious models etc. Supports Stable Diffusion 2.1!
 Author-email: cmdr2 <secondary.cmdr2@gmail.com>
 Project-URL: Homepage, https://github.com/easydiffusion/sdkit
 Project-URL: Bug Tracker, https://github.com/easydiffusion/sdkit/issues
 Keywords: stable diffusion,ai,art
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkit-1.0.94/sdkit.egg-info/SOURCES.txt` & `sdkit-1.0.95/sdkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

